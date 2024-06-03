# Comparing `tmp/citrixnetscalermemoryleak-0.0.1.tar.gz` & `tmp/citrixnetscalermemoryleak-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrixnetscalermemoryleak-0.0.1.tar", last modified: Wed May 29 09:08:41 2024, max compression
+gzip compressed data, was "citrixnetscalermemoryleak-0.0.2.tar", last modified: Mon Jun  3 06:41:00 2024, max compression
```

## Comparing `citrixnetscalermemoryleak-0.0.1.tar` & `citrixnetscalermemoryleak-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,13 @@
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-29 09:08:41.008948 citrixnetscalermemoryleak-0.0.1/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1069 2024-05-29 08:47:08.000000 citrixnetscalermemoryleak-0.0.1/LICENSE
--rw-r--r--   0 karthikeyan   (501) staff       (20)     5738 2024-05-29 09:08:41.008747 citrixnetscalermemoryleak-0.0.1/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)     5259 2024-05-29 09:08:18.000000 citrixnetscalermemoryleak-0.0.1/README.md
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-29 09:08:41.001752 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-05-29 08:49:44.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/__init__.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-29 09:08:41.006921 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/includes/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-05-29 08:47:08.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/includes/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      748 2024-05-29 08:55:57.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/includes/bot.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      524 2024-05-29 08:55:57.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/includes/filereader.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     2541 2024-05-29 08:55:57.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/includes/scan.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      313 2024-05-29 08:47:08.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/includes/writefile.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1902 2024-05-29 08:55:57.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/main.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-29 09:08:41.008261 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/utils/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-05-29 08:47:08.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/utils/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     2014 2024-05-29 08:55:58.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/utils/configure.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1046 2024-05-29 08:58:53.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/utils/const.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     3114 2024-05-29 08:47:08.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/utils/helpers.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-05-29 08:47:08.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak/utils/status.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-05-29 09:08:41.005293 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak.egg-info/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     5738 2024-05-29 09:08:40.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak.egg-info/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)      838 2024-05-29 09:08:40.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak.egg-info/SOURCES.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-05-29 09:08:40.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak.egg-info/dependency_links.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       82 2024-05-29 09:08:40.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak.egg-info/entry_points.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-05-29 09:08:40.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak.egg-info/requires.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       26 2024-05-29 09:08:40.000000 citrixnetscalermemoryleak-0.0.1/citrixnetscalermemoryleak.egg-info/top_level.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-05-29 09:08:41.009027 citrixnetscalermemoryleak-0.0.1/setup.cfg
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1053 2024-05-29 08:56:41.000000 citrixnetscalermemoryleak-0.0.1/setup.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-06-03 06:41:00.627246 citrixnetscalermemoryleak-0.0.2/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1069 2024-05-29 08:47:08.000000 citrixnetscalermemoryleak-0.0.2/LICENSE
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     5807 2024-06-03 06:41:00.626892 citrixnetscalermemoryleak-0.0.2/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     5328 2024-06-03 06:24:17.000000 citrixnetscalermemoryleak-0.0.2/README.md
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-06-03 06:41:00.626567 citrixnetscalermemoryleak-0.0.2/citrixnetscalermemoryleak.egg-info/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     5807 2024-06-03 06:41:00.000000 citrixnetscalermemoryleak-0.0.2/citrixnetscalermemoryleak.egg-info/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      322 2024-06-03 06:41:00.000000 citrixnetscalermemoryleak-0.0.2/citrixnetscalermemoryleak.egg-info/SOURCES.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-06-03 06:41:00.000000 citrixnetscalermemoryleak-0.0.2/citrixnetscalermemoryleak.egg-info/dependency_links.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       85 2024-06-03 06:41:00.000000 citrixnetscalermemoryleak-0.0.2/citrixnetscalermemoryleak.egg-info/entry_points.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-06-03 06:41:00.000000 citrixnetscalermemoryleak-0.0.2/citrixnetscalermemoryleak.egg-info/requires.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-06-03 06:41:00.000000 citrixnetscalermemoryleak-0.0.2/citrixnetscalermemoryleak.egg-info/top_level.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-06-03 06:41:00.627317 citrixnetscalermemoryleak-0.0.2/setup.cfg
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1061 2024-06-03 06:40:59.000000 citrixnetscalermemoryleak-0.0.2/setup.py
```

### Comparing `citrixnetscalermemoryleak-0.0.1/LICENSE` & `citrixnetscalermemoryleak-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citrixnetscalermemoryleak-0.0.1/PKG-INFO` & `citrixnetscalermemoryleak-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-Metadata-Version: 2.1
-Name: citrixnetscalermemoryleak
-Version: 0.0.1
-Author: @karthithehacker
-Author-email: <contact@karthithehacker.com>
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 <div align="center">
   <img src="https://blogs.cappriciosec.com/uploaders/citrixnetscalermemoryleak-tool.png" alt="logo">
 </div>
 
 
 ## Badges
 
 
 
 [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
-![PyPI - Version](https://img.shields.io/pypi/v/citrixnetscalermemoryleak)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/citrixnetscalermemoryleak)
-![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/citrixnetscalermemoryleak/total)
-<a href="https://github.com/Cappricio-Securities/citrixnetscalermemoryleak/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/citrixnetscalermemoryleak"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+![PyPI - Version](https://img.shields.io/pypi/v/citrix-netscaler-memory-leak)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/citrix-netscaler-memory-leak)
+![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/citrix-netscaler-memory-leak/total)
+<a href="https://github.com/Cappricio-Securities/citrix-netscaler-memory-leak/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/citrix-netscaler-memory-leak"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
 [![Follow Twitter](https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
 <p align="center">
 
 <p align="center">
 
 
 
@@ -46,46 +32,46 @@
 
 ## Installation 
 
 1. Install Python3 and pip [Instructions Here](https://www.python.org/downloads/) (If you can't figure this out, you shouldn't really be using this)
 
    - Install via pip
      - ```bash
-          pip install citrixnetscalermemoryleak 
+          pip install citrix-netscaler-memory-leak 
         ```
    - Run bellow command to check
-     - `citrixnetscalermemoryleak -h`
+     - `citrix-netscaler-memory-leak -h`
 
 ## Configurations 
 2. We integrated with the Telegram API to receive instant notifications for vulnerability detection.
    
    - Telegram Notification
      - ```bash
-          citrixnetscalermemoryleak --chatid <YourTelegramChatID>
+          citrix-netscaler-memory-leak --chatid <YourTelegramChatID>
         ```
    - Open your telegram and search for [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/#@CappricioSecuritiesTools_bot) and click start
 
 ## Usages 
 3. This tool has multiple use cases.
    
    - To Check Single URL
      - ```bash
-          citrixnetscalermemoryleak -u http://example.com 
+          citrix-netscaler-memory-leak -u http://example.com 
         ```
    - To Check List of URL 
       - ```bash
-          citrixnetscalermemoryleak -i urls.txt 
+          citrix-netscaler-memory-leak -i urls.txt 
         ```
    - Save output into TXT file
       - ```bash
-          citrixnetscalermemoryleak -i urls.txt -o out.txt
+          citrix-netscaler-memory-leak -i urls.txt -o out.txt
         ```
-   - Want to Learn about [`citrixnetscalermemoryleak`](https://blogs.cappriciosec.com/cve/167/The%20Potential%20Citrix%20NetScaler%20Memory%20Leak)? Then Type Below command
+   - Want to Learn about [`citrix-netscaler-memory-leak`](https://blogs.cappriciosec.com/cve/167/The%20Potential%20Citrix%20NetScaler%20Memory%20Leak)? Then Type Below command
       - ```bash
-          citrixnetscalermemoryleak -b
+          citrix-netscaler-memory-leak -b
         ```
      
 <p align="center">
   <b>🚨 Disclaimer</b>
   
 </p>
 <p align="center">
@@ -111,30 +97,30 @@
    ____  ___  / /_______________ _/ /__  _____      ____ ___  ___  ____ ___  ____  _______  __      / /__  ____ _/ /__
   / __ \/ _ \/ __/ ___/ ___/ __ `/ / _ \/ ___/_____/ __ `__ \/ _ \/ __ `__ \/ __ \/ ___/ / / /_____/ / _ \/ __ `/ //_/
  / / / /  __/ /_(__  ) /__/ /_/ / /  __/ /  /_____/ / / / / /  __/ / / / / / /_/ / /  / /_/ /_____/ /  __/ /_/ / ,<
 /_/ /_/\___/\__/____/\___/\__,_/_/\___/_/        /_/ /_/ /_/\___/_/ /_/ /_/\____/_/   \__, /     /_/\___/\__,_/_/|_|
                                                                                      /____/
                               Developed By https://cappriciosec.com
 
-citrixnetscalermemoryleak : Bug scanner for WebPentesters and Bugbounty Hunters 
+citrix-netscaler-memory-leak : Bug scanner for WebPentesters and Bugbounty Hunters 
 
-$ citrixnetscalermemoryleak [option]
+$ citrix-netscaler-memory-leak [option]
 
-Usage: citrixnetscalermemoryleak [options]
+Usage: citrix-netscaler-memory-leak [options]
 ```
 
 
 | Argument | Type     | Description                | Examples |
 | :-------- | :------- | :------------------------- | :------------------------- |
-| `-u` | `--url` | URL to scan | citrixnetscalermemoryleak -u https://target.com |
-| `-i` | `--input` | filename Read input from txt  | citrixnetscalermemoryleak -i target.txt | 
-| `-o` | `--output` | filename Write output in txt file | citrixnetscalermemoryleak -i target.txt -o output.txt |
-| `-c` | `--chatid` | Creating Telegram Notification | citrixnetscalermemoryleak --chatid yourid |
-| `-b` | `--blog` | To Read about citrixnetscalermemoryleak Bug | citrixnetscalermemoryleak -b |
-| `-h` | `--help` | Help Menu | citrixnetscalermemoryleak -h |
+| `-u` | `--url` | URL to scan | citrix-netscaler-memory-leak -u https://target.com |
+| `-i` | `--input` | filename Read input from txt  | citrix-netscaler-memory-leak -i target.txt | 
+| `-o` | `--output` | filename Write output in txt file | citrix-netscaler-memory-leak -i target.txt -o output.txt |
+| `-c` | `--chatid` | Creating Telegram Notification | citrix-netscaler-memory-leak --chatid yourid |
+| `-b` | `--blog` | To Read about citrix-netscaler-memory-leak Bug | citrix-netscaler-memory-leak -b |
+| `-h` | `--help` | Help Menu | citrix-netscaler-memory-leak -h |
 
 
 
 ## 🔗 Links
 [![Website](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://cappriciosec.com/)
 [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan--v/)
 [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/karthithehacker)
```

#### html2text {}

```diff
@@ -1,69 +1,61 @@
-Metadata-Version: 2.1 Name: citrixnetscalermemoryleak Version: 0.0.1 Author:
-@karthithehacker Author-email:
-karthithehacker.com> Classifier: Development Status :: 1 - Planning Classifier:
-Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
-MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
-Content-Type: text/markdown License-File: LICENSE
                                     [logo]
 ## Badges [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)]
 (https://choosealicense.com/licenses/mit/) ![PyPI - Version](https://
-img.shields.io/pypi/v/citrixnetscalermemoryleak) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/citrixnetscalermemoryleak) ![GitHub all releases](https:
-//img.shields.io/github/downloads/Cappricio-Securities/
-citrixnetscalermemoryleak/total) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
-_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_c_i_t_r_i_x_n_e_t_s_c_a_l_e_r_m_e_m_o_r_y_l_e_a_k_]![Profile_view](https://
-komarev.com/ghpvc/?username=Cappricio-
-Securities&label=Profile%20views&color=0e75b6&style=flat) [![Follow Twitter]
-(https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://
-twitter.com/cappricio_sec)
+img.shields.io/pypi/v/citrix-netscaler-memory-leak) ![PyPI - Downloads](https:/
+/img.shields.io/pypi/dm/citrix-netscaler-memory-leak) ![GitHub all releases]
+(https://img.shields.io/github/downloads/Cappricio-Securities/citrix-netscaler-
+memory-leak/total) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/
+_c_i_t_r_i_x_-_n_e_t_s_c_a_l_e_r_-_m_e_m_o_r_y_-_l_e_a_k_]![Profile_view](https://komarev.com/ghpvc/
+?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+[![Follow Twitter](https://img.shields.io/twitter/follow/
+cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
  ## License [MIT](https://choosealicense.com/licenses/mit/) ## Installation 1.
 Install Python3 and pip [Instructions Here](https://www.python.org/downloads/)
  (If you can't figure this out, you shouldn't really be using this) - Install
-   via pip - ```bash pip install citrixnetscalermemoryleak ``` - Run bellow
-   command to check - `citrixnetscalermemoryleak -h` ## Configurations 2. We
+  via pip - ```bash pip install citrix-netscaler-memory-leak ``` - Run bellow
+ command to check - `citrix-netscaler-memory-leak -h` ## Configurations 2. We
      integrated with the Telegram API to receive instant notifications for
-          vulnerability detection. - Telegram Notification - ```bash
-  citrixnetscalermemoryleak --chatid ``` - Open your telegram and search for
+ vulnerability detection. - Telegram Notification - ```bash citrix-netscaler-
+         memory-leak --chatid ``` - Open your telegram and search for
          [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/
   #@CappricioSecuritiesTools_bot) and click start ## Usages 3. This tool has
-multiple use cases. - To Check Single URL - ```bash citrixnetscalermemoryleak -
-           u http://example.com ``` - To Check List of URL - ```bash
-citrixnetscalermemoryleak -i urls.txt ``` - Save output into TXT file - ```bash
-  citrixnetscalermemoryleak -i urls.txt -o out.txt ``` - Want to Learn about
-     [`citrixnetscalermemoryleak`](https://blogs.cappriciosec.com/cve/167/
+ multiple use cases. - To Check Single URL - ```bash citrix-netscaler-memory-
+    leak -u http://example.com ``` - To Check List of URL - ```bash citrix-
+  netscaler-memory-leak -i urls.txt ``` - Save output into TXT file - ```bash
+citrix-netscaler-memory-leak -i urls.txt -o out.txt ``` - Want to Learn about
+   [`citrix-netscaler-memory-leak`](https://blogs.cappriciosec.com/cve/167/
 The%20Potential%20Citrix%20NetScaler%20Memory%20Leak)? Then Type Below command
-                  - ```bash citrixnetscalermemoryleak -b ```
+                 - ```bash citrix-netscaler-memory-leak -b ```
                                 ?ð???¨ DDiissccllaaiimmeerr
 TThhiiss ttooooll iiss ccrreeaatteedd ffoorr sseeccuurriittyy bbuugg iiddeennttiiffiiccaattiioonn aanndd aassssiissttaannccee;; CCaapppprriicciioo
 SSeeccuurriittiieess iiss nnoott lliiaabbllee ffoorr aannyy iilllleeggaall uussee.. UUssee rreessppoonnssiibbllyy wwiitthhiinn lleeggaall aanndd
                         eetthhiiccaall bboouunnddaarriieess.. ?ð????ð???¡?ï?¸?
 ## Working PoC Video [![asciicast](https://blogs.cappriciosec.com/uploaders/
 Screenshot%202024-05-29%20at%202.37.45%20PM.png)](https://asciinema.org/a/
 ARfK9usVLsdseyuqCfmWFhXKG) ## Help menu #### Get all items ```bash ð Hey
 Hacker v1.0 __ __ __ __ ____ ___ / /_______________ _/ /__ _____ ____ ___ ___
 ____ ___ ____ _______ __ / /__ ____ _/ /__ / __ \/ _ \/ __/ ___/ ___/ __ `/ / _
 \/ ___/_____/ __ `__ \/ _ \/ __ `__ \/ __ \/ ___/ / / /_____/ / _ \/ __ `/ //_/
 / / / / __/ /_(__ ) /__/ /_/ / / __/ / /_____/ / / / / / __/ / / / / / /_/ / /
 / /_/ /_____/ / __/ /_/ / ,< /_/ /_/\___/\__/____/\___/\__,_/_/\___/_/ /_/ /_/
 /_/\___/_/ /_/ /_/\____/_/ \__, / /_/\___/\__,_/_/|_| /____/ Developed By
-https://cappriciosec.com citrixnetscalermemoryleak : Bug scanner for
-WebPentesters and Bugbounty Hunters $ citrixnetscalermemoryleak [option] Usage:
-citrixnetscalermemoryleak [options] ``` | Argument | Type | Description |
-Examples | | :-------- | :------- | :------------------------- | :-------------
------------- | | `-u` | `--url` | URL to scan | citrixnetscalermemoryleak -
-u https://target.com | | `-i` | `--input` | filename Read input from txt |
-citrixnetscalermemoryleak -i target.txt | | `-o` | `--output` | filename Write
-output in txt file | citrixnetscalermemoryleak -i target.txt -o output.txt | |
-`-c` | `--chatid` | Creating Telegram Notification | citrixnetscalermemoryleak
---chatid yourid | | `-b` | `--blog` | To Read about citrixnetscalermemoryleak
-Bug | citrixnetscalermemoryleak -b | | `-h` | `--help` | Help Menu |
-citrixnetscalermemoryleak -h | ## ð Links [![Website](https://
-img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-
-fi&logoColor=white)](https://cappriciosec.com/) [![linkedin](https://
-img.shields.io/badge/linkedin-0A66C2?style=for-the-
+https://cappriciosec.com citrix-netscaler-memory-leak : Bug scanner for
+WebPentesters and Bugbounty Hunters $ citrix-netscaler-memory-leak [option]
+Usage: citrix-netscaler-memory-leak [options] ``` | Argument | Type |
+Description | Examples | | :-------- | :------- | :------------------------- |
+:------------------------- | | `-u` | `--url` | URL to scan | citrix-netscaler-
+memory-leak -u https://target.com | | `-i` | `--input` | filename Read input
+from txt | citrix-netscaler-memory-leak -i target.txt | | `-o` | `--output` |
+filename Write output in txt file | citrix-netscaler-memory-leak -i target.txt
+-o output.txt | | `-c` | `--chatid` | Creating Telegram Notification | citrix-
+netscaler-memory-leak --chatid yourid | | `-b` | `--blog` | To Read about
+citrix-netscaler-memory-leak Bug | citrix-netscaler-memory-leak -b | | `-h` |
+`--help` | Help Menu | citrix-netscaler-memory-leak -h | ## ð Links [!
+[Website](https://img.shields.io/badge/my_portfolio-000?style=for-the-
+badge&logo=ko-fi&logoColor=white)](https://cappriciosec.com/) [![linkedin]
+(https://img.shields.io/badge/linkedin-0A66C2?style=for-the-
 badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan--
 v/) [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/karthithehacker) ##
 Author - [@karthithehacker](https://github.com/karthi-the-hacker/) ## Feedback
 If you have any feedback, please reach out to us at contact@karthithehacker.com
```

### Comparing `citrixnetscalermemoryleak-0.0.1/setup.py` & `citrixnetscalermemoryleak-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
 
-VERSION = '0.0.1'
-DESCRIPTION = 'A Tool to find an Easy Bounty - citrixnetscalermemoryleak'
-LONG_DESCRIPTION = 'This is a tool used by several security researchers to find citrixnetscalermemoryleak.'
+VERSION = '0.0.2'
+DESCRIPTION = 'A Tool to find an Easy Bounty - citrix-netscaler-memory-leak'
+LONG_DESCRIPTION = 'This is a tool used by several security researchers to find citrix-netscaler-memoryleak.'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="citrixnetscalermemoryleak",
     version=VERSION,
     author="@karthithehacker",
     author_email="<contact@karthithehacker.com>",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
-            'citrixnetscalermemoryleak = citrixnetscalermemoryleak.main:main',
+            'citrix-netscaler-memory-leak = citrixnetscalermemoryleak.main:main',
         ],
     },
     install_requires=['urllib3', 'requests', 'click'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

