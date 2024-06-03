# Comparing `tmp/sssekai-0.1.1.tar.gz` & `tmp/sssekai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssekai-0.1.1.tar", last modified: Fri May 24 12:52:02 2024, max compression
+gzip compressed data, was "sssekai-0.1.2.tar", last modified: Mon Jun  3 13:00:31 2024, max compression
```

## Comparing `sssekai-0.1.1.tar` & `sssekai-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.722165 sssekai-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-24 12:52:02.722165 sssekai-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-24 12:51:54.000000 sssekai-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:52:02.722165 sssekai-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-24 12:51:54.000000 sssekai-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.714165 sssekai-0.1.1/sssekai/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/abcache/
--rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/abcache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/crypto/APIManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/crypto/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/abcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/abdecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/apidecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/live2dextract.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/mitm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/mvdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/spineextract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/usmdemux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/fmt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/fmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/fmt/moc3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/unity/
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/AnimationClip.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.722165 sssekai-0.1.1/sssekai/unity/constant/
--rw-r--r--   0 runner    (1001) docker     (127)    60945 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/constant/SekaiLive2DPathNames.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/constant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.722165 sssekai-0.1.1/sssekai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.919962 sssekai-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-06-03 13:00:31.919962 sssekai-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-06-03 13:00:22.000000 sssekai-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:00:31.919962 sssekai-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-06-03 13:00:22.000000 sssekai-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.915962 sssekai-0.1.2/sssekai/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.915962 sssekai-0.1.2/sssekai/abcache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/abcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.919962 sssekai-0.1.2/sssekai/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/crypto/APIManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/crypto/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.919962 sssekai-0.1.2/sssekai/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/abcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/abdecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/apidecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/live2dextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/mitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/mvdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/spineextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/entrypoint/usmdemux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.919962 sssekai-0.1.2/sssekai/fmt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/fmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/fmt/moc3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.919962 sssekai-0.1.2/sssekai/unity/
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/unity/AnimationClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/unity/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/unity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.919962 sssekai-0.1.2/sssekai/unity/constant/
+-rw-r--r--   0 runner    (1001) docker     (127)    60945 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/unity/constant/SekaiLive2DPathNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:22.000000 sssekai-0.1.2/sssekai/unity/constant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:00:31.919962 sssekai-0.1.2/sssekai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-06-03 13:00:31.000000 sssekai-0.1.2/sssekai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-06-03 13:00:31.000000 sssekai-0.1.2/sssekai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:00:31.000000 sssekai-0.1.2/sssekai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-03 13:00:31.000000 sssekai-0.1.2/sssekai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:00:31.000000 sssekai-0.1.2/sssekai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 13:00:31.000000 sssekai-0.1.2/sssekai.egg-info/top_level.txt
```

### Comparing `sssekai-0.1.1/setup.py` & `sssekai-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/__main__.py` & `sssekai-0.1.2/sssekai/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sssekai.entrypoint.abdecrypt import main_abdecrypt
 from sssekai.entrypoint.mitm import main_mitm
 from sssekai.entrypoint.mvdata import main_mvdata
 from sssekai.entrypoint.usmdemux import main_usmdemux
 from sssekai.entrypoint.abcache import main_abcache
 from sssekai.entrypoint.live2dextract import main_live2dextract
 from sssekai.entrypoint.spineextract import main_spineextract
-from sssekai.unity import SEKAI_UNITY_VERSION
+from sssekai.unity import sssekai_get_unity_version,sssekai_set_unity_version
 from sssekai.abcache import DEFAULT_CACHE_DIR, DEFAULT_SEKAI_APP_PLATFORM, DEFAULT_SEKAI_APP_VERSION, DEFAULT_SEKAI_APP_HASH
 def __main__():
     from tqdm.std import tqdm as tqdm_c
     class SemaphoreStdout:
         @staticmethod
         def write(__s):
             # Blocks tqdm's output until write on this stream is done
             # Solves cases where progress bars gets re-rendered when logs
             # spews out too fast
             with tqdm_c.external_write_mode(file=sys.stdout, nolock=False):
                 return sys.stdout.write(__s)
     parser = argparse.ArgumentParser(description='''SSSekai Proejct SEKAI feat. Hatsune Miku (Android) Modding Tools
 Installation:
-    pip install git+https://github.com/mos9527/sssekai                                    
+    pip install sssekai                                    
 ''', formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('--log-level', type=str, help='logging level (default: %(default)s)', default='INFO', choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'])
+    parser.add_argument('--unity-version', type=str, help='''Unity version to use (default: %(default)s)
+Prior to game version 3.6.0, this has always been 2020.3.21f1.
+This has been changed to 2022.3.21f1 since. However, some assets are still using the old version.
+If you encounter any issues, try switching to the new version, or vice versa.''', default=sssekai_get_unity_version())
     subparsers = parser.add_subparsers(title='subcommands', description='valid subcommands', help='additional help')
     # apidecrypt
     apidecrypt_parser = subparsers.add_parser('apidecrypt', help='''API crypto dumper
 This crypto applies to:
     - API request/response body dumped by packet sniffer (mitmproxy, wireshark, etc.)
     - AssetBundleInfo (can be found at /sdcard/Android/data/com.hermes.mk.asia/files/data/AssetBundleInfo,or see sssekai.abcache)''')
     apidecrypt_parser.add_argument('infile', type=str, help='input dump file')
@@ -48,15 +52,15 @@
     usmdemux_parser.add_argument('outdir', type=str, help='output directory')
     usmdemux_parser.set_defaults(func=main_usmdemux)
     # abcache
     abcache_parser = subparsers.add_parser('abcache', help='''Sekai AssetBundle local cache
 Downloads/Updates *ALL* PJSK JP assets to local devices.
 NOTE: The assets can take quite a lot of space (est. 42.5GB for app version 3.3.1) so be prepared
 NOTE: The AssetBundles *cached* are NOT OBFUSCATED. They can be used as is by various Unity ripping tools (and sssekai by extension)
-      that supports stripped Unity version (should be %s. the version is ripped).''' % SEKAI_UNITY_VERSION)
+      that supports stripped Unity version (should be %s. the version is ripped).''' % sssekai_get_unity_version())
     abcache_parser.add_argument('--cache-dir', type=str, help='cache directory (default: %(default)s)',default=DEFAULT_CACHE_DIR)
     abcache_parser.add_argument('--skip-update',action='store_true',help='skip all updates and use cached assets as is.')
     abcache_parser.add_argument('--version', type=str, help='PJSK app version (default: %(default)s)', default=DEFAULT_SEKAI_APP_VERSION)
     abcache_parser.add_argument('--platform', type=str, help='PJSK app platform (default: %(default)s)', default=DEFAULT_SEKAI_APP_PLATFORM)
     abcache_parser.add_argument('--appHash', type=str, help='PJSK app hash (default: %(default)s)', default=DEFAULT_SEKAI_APP_HASH)
     abcache_parser.add_argument('--open', action='store_true',help='open cache directory. this will skip all updates.')
     abcache_parser.set_defaults(func=main_abcache)
@@ -89,14 +93,16 @@
             fmt="%(asctime)s %(name)s [%(levelname).4s] %(message)s",
             isatty=True,
             stream=SemaphoreStdout
         )
     basicConfig(
         level=args.log_level, format="[%(levelname).4s] %(name)s %(message)s", stream=SemaphoreStdout
     )
+    # override unity version
+    sssekai_set_unity_version(args.unity_version)
     if 'func' in args:
         args.func(args)
     else:
         parser.print_help()
 
 
 if __name__ == "__main__":
```

### Comparing `sssekai-0.1.1/sssekai/abcache/__init__.py` & `sssekai-0.1.2/sssekai/abcache/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass, asdict
 from requests import Session
 from logging import getLogger
 from pathlib import Path
 from concurrent.futures import ThreadPoolExecutor
 
 from sssekai import __version__
-from sssekai.unity import SEKAI_UNITY_VERSION
+from sssekai.unity import sssekai_get_unity_version
 logger = getLogger('sssekai.abcache')
 
 from sssekai.crypto.APIManager import decrypt, encrypt
 from sssekai.crypto.AssetBundle import decrypt_headaer_inplace, SEKAI_AB_MAGIC
 from msgpack import unpackb, dump, load, packb
 from tqdm import tqdm
 DEFAULT_CACHE_DIR = '~/.sssekai/abcache'
@@ -357,19 +357,19 @@
         super().__init__()
         self.config = config
         self.config.app_platform = self.config.app_platform.lower()
         self.headers.update({
             'Accept': 'application/octet-stream',
             'Content-Type': 'application/octet-stream',
             'Accept-Encoding': 'deflate, gzip',
-            'User-Agent': 'UnityPlayer/%s' % SEKAI_UNITY_VERSION,
+            'User-Agent': 'UnityPlayer/%s' % sssekai_get_unity_version(),
             'X-Platform': self.config.app_platform.capitalize(),
             'X-DeviceModel': 'sssekai/%s' % __version__,
             'X-OperatingSystem': self.config.app_platform.capitalize(),
-            'X-Unity-Version': SEKAI_UNITY_VERSION,
+            'X-Unity-Version': sssekai_get_unity_version(),
             'X-App-Version': self.SEKAI_APP_VERSION,
             'X-App-Hash': self.SEKAI_APP_HASH
         })
         self.downloader = AbCacheDownloader(self)
         makedirs(self.config.cache_dir,exist_ok=True)
         try:
             self.load()
```

### Comparing `sssekai-0.1.1/sssekai/crypto/APIManager.py` & `sssekai-0.1.2/sssekai/crypto/APIManager.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/crypto/AssetBundle.py` & `sssekai-0.1.2/sssekai/crypto/AssetBundle.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/entrypoint/abcache.py` & `sssekai-0.1.2/sssekai/entrypoint/abcache.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/entrypoint/live2dextract.py` & `sssekai-0.1.2/sssekai/entrypoint/live2dextract.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/entrypoint/mvdata.py` & `sssekai-0.1.2/sssekai/entrypoint/mvdata.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/entrypoint/spineextract.py` & `sssekai-0.1.2/sssekai/entrypoint/spineextract.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/entrypoint/usmdemux.py` & `sssekai-0.1.2/sssekai/entrypoint/usmdemux.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/fmt/moc3.py` & `sssekai-0.1.2/sssekai/fmt/moc3.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/unity/AnimationClip.py` & `sssekai-0.1.2/sssekai/unity/AnimationClip.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai/unity/constant/SekaiLive2DPathNames.py` & `sssekai-0.1.2/sssekai/unity/constant/SekaiLive2DPathNames.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.1/sssekai.egg-info/SOURCES.txt` & `sssekai-0.1.2/sssekai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

