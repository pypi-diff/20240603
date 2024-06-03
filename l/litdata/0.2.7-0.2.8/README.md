# Comparing `tmp/litdata-0.2.7.tar.gz` & `tmp/litdata-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litdata-0.2.7.tar", last modified: Fri May 24 18:52:35 2024, max compression
+gzip compressed data, was "litdata-0.2.8.tar", last modified: Mon Jun  3 08:34:23 2024, max compression
```

## Comparing `litdata-0.2.7.tar` & `litdata-0.2.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.936136 litdata-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-24 18:52:27.000000 litdata-0.2.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-24 18:52:27.000000 litdata-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-24 18:52:27.000000 litdata-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-05-24 18:52:35.936136 litdata-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-05-24 18:52:27.000000 litdata-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 18:52:27.000000 litdata-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:52:35.936136 litdata-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-24 18:52:27.000000 litdata-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.928136 litdata-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.928136 litdata-0.2.7/src/litdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.932136 litdata-0.2.7/src/litdata/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.932136 litdata-0.2.7/src/litdata/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    20079 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/item_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18050 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.936136 litdata-0.2.7/src/litdata/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/_pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/shuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.936136 litdata-0.2.7/src/litdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:34:23.891240 litdata-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-03 08:34:13.000000 litdata-0.2.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-06-03 08:34:13.000000 litdata-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-03 08:34:13.000000 litdata-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20617 2024-06-03 08:34:23.891240 litdata-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-06-03 08:34:13.000000 litdata-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-03 08:34:13.000000 litdata-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:34:23.891240 litdata-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-06-03 08:34:13.000000 litdata-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:34:23.883240 litdata-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:34:23.883240 litdata-0.2.8/src/litdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:34:23.887240 litdata-0.2.8/src/litdata/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/processing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/processing/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/processing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:34:23.887240 litdata-0.2.8/src/litdata/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26435 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20169 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/item_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19366 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/streaming/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:34:23.891240 litdata-0.2.8/src/litdata/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/utilities/_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/utilities/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/utilities/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/utilities/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/utilities/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-06-03 08:34:13.000000 litdata-0.2.8/src/litdata/utilities/shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:34:23.891240 litdata-0.2.8/src/litdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20617 2024-06-03 08:34:23.000000 litdata-0.2.8/src/litdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-06-03 08:34:23.000000 litdata-0.2.8/src/litdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:34:23.000000 litdata-0.2.8/src/litdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:34:23.000000 litdata-0.2.8/src/litdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-03 08:34:23.000000 litdata-0.2.8/src/litdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 08:34:23.000000 litdata-0.2.8/src/litdata.egg-info/top_level.txt
```

### Comparing `litdata-0.2.7/LICENSE` & `litdata-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/MANIFEST.in` & `litdata-0.2.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/PKG-INFO` & `litdata-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.7
+Version: 0.2.8
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -220,15 +220,15 @@
 ## The Map Operator
 
 The `map` operator can be used to apply a function over a list of inputs.
 
 Here is an example where the `map` operator is used to apply a `resize_image` function over a folder of large images.
 
 ```python
-from lightning.data import map
+from litdata import map
 from PIL import Image
 
 # Note: Inputs could also refer to files on s3 directly.
 input_dir = "my_large_images"
 inputs = [os.path.join(input_dir, f) for f in os.listdir(input_dir)]
 
 # The resize image takes one of the input (image_path) and the output directory. 
@@ -365,15 +365,15 @@
 ```
 
 ## On-Prem Optimizations
 
 On-prem compute nodes can mount and use a network drive. A network drive is a shared storage device on a local area network. In order to reduce their network overload, the `StreamingDataset` supports `caching` the data chunks.
 
 ```python
-from lightning.data import StreamingDataset
+from litdata import StreamingDataset
 
 dataset = StreamingDataset(input_dir="local:/data/shared-drive/some-data")
 ```
 
 # Benchmarks
 
 In order to measure the effectiveness of LitData, we used a commonly used dataset for benchmarks: [Imagenet-1.2M](https://www.image-net.org/) where the training set contains `1,281,167 images`.
```

### Comparing `litdata-0.2.7/README.md` & `litdata-0.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 ## The Map Operator
 
 The `map` operator can be used to apply a function over a list of inputs.
 
 Here is an example where the `map` operator is used to apply a `resize_image` function over a folder of large images.
 
 ```python
-from lightning.data import map
+from litdata import map
 from PIL import Image
 
 # Note: Inputs could also refer to files on s3 directly.
 input_dir = "my_large_images"
 inputs = [os.path.join(input_dir, f) for f in os.listdir(input_dir)]
 
 # The resize image takes one of the input (image_path) and the output directory. 
@@ -324,15 +324,15 @@
 ```
 
 ## On-Prem Optimizations
 
 On-prem compute nodes can mount and use a network drive. A network drive is a shared storage device on a local area network. In order to reduce their network overload, the `StreamingDataset` supports `caching` the data chunks.
 
 ```python
-from lightning.data import StreamingDataset
+from litdata import StreamingDataset
 
 dataset = StreamingDataset(input_dir="local:/data/shared-drive/some-data")
 ```
 
 # Benchmarks
 
 In order to measure the effectiveness of LitData, we used a commonly used dataset for benchmarks: [Imagenet-1.2M](https://www.image-net.org/) where the training set contains `1,281,167 images`.
```

### Comparing `litdata-0.2.7/setup.py` & `litdata-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/__about__.py` & `litdata-0.2.8/src/litdata/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 __author__ = "Lightning AI et al."
 __author_email__ = "pytorch@lightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2023-{time.strftime('%Y')}, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/lit-data"
 __docs_url__ = "https://lightning.ai/docs/pytorch/stable/"
 # this has to be simple string, see: https://github.com/pypa/twine/issues/522
```

### Comparing `litdata-0.2.7/src/litdata/__init__.py` & `litdata-0.2.8/src/litdata/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/constants.py` & `litdata-0.2.8/src/litdata/constants.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/imports.py` & `litdata-0.2.8/src/litdata/imports.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/processing/__init__.py` & `litdata-0.2.8/src/litdata/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/processing/data_processor.py` & `litdata-0.2.8/src/litdata/processing/data_processor.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/processing/functions.py` & `litdata-0.2.8/src/litdata/processing/functions.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/processing/readers.py` & `litdata-0.2.8/src/litdata/processing/readers.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/processing/utilities.py` & `litdata-0.2.8/src/litdata/processing/utilities.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/__init__.py` & `litdata-0.2.8/src/litdata/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/cache.py` & `litdata-0.2.8/src/litdata/streaming/cache.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/client.py` & `litdata-0.2.8/src/litdata/streaming/client.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/combined.py` & `litdata-0.2.8/src/litdata/streaming/combined.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,19 @@
             dataset.set_epoch(current_epoch)
 
     def set_shuffle(self, shuffle: bool) -> None:
         """Set the current shuffle to the datasets."""
         for dataset in self._datasets:
             dataset.set_shuffle(shuffle)
 
+    def set_drop_last(self, drop_last: bool) -> None:
+        """Set the current drop_last to the datasets."""
+        for dataset in self._datasets:
+            dataset.set_drop_last(drop_last)
+
     def _check_datasets(self, datasets: List[StreamingDataset]) -> None:
         if any(not isinstance(d, StreamingDataset) for d in datasets):
             raise RuntimeError("The provided datasets should be instances of the StreamingDataset.")
 
     def _set_use_streaming_dataloader(self, use_streaming_dataloader: bool) -> None:
         # Used to prevent returning num_samples_yielded when using PyTorch DataLoader
         self._use_streaming_dataloader = use_streaming_dataloader
```

### Comparing `litdata-0.2.7/src/litdata/streaming/compression.py` & `litdata-0.2.8/src/litdata/streaming/compression.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/config.py` & `litdata-0.2.8/src/litdata/streaming/config.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/dataloader.py` & `litdata-0.2.8/src/litdata/streaming/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,25 +536,29 @@
         *args: Any,
         batch_size: int = 1,
         num_workers: int = 0,
         profile_batches: Union[bool, int] = False,
         profile_dir: Optional[str] = None,
         prefetch_factor: Optional[int] = None,
         shuffle: Optional[bool] = None,
+        drop_last: Optional[bool] = False,
         **kwargs: Any,
     ) -> None:  # pyright: ignore
         if not isinstance(dataset, (StreamingDataset, CombinedStreamingDataset)):
             raise RuntimeError(
                 "The provided dataset should be either an instance of StreamingDataset or CombinedStreamingDataset."
                 f" Found {dataset}."
             )
 
         if shuffle is not None:
             dataset.set_shuffle(shuffle)
 
+        if drop_last is not None:
+            dataset.set_drop_last(drop_last)
+
         shuffle = None
 
         if profile_batches and not _VIZ_TRACKER_AVAILABLE:
             raise ModuleNotFoundError("To use profile_batches, viztracer is required. Run `pip install viztracer`")
 
         if profile_batches and num_workers == 0:
             raise ValueError("Profiling is supported only with num_workers >= 1.")
```

### Comparing `litdata-0.2.7/src/litdata/streaming/dataset.py` & `litdata-0.2.8/src/litdata/streaming/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,17 @@
         self._state_dict: Optional[Dict[str, Any]] = None
         self.num_workers: Optional[int] = None
         self.batch_size: Optional[int] = None
 
     def set_shuffle(self, shuffle: bool) -> None:
         self.shuffle = shuffle
 
+    def set_drop_last(self, drop_last: bool) -> None:
+        self.drop_last = drop_last
+
     def set_epoch(self, current_epoch: int) -> None:
         """Set the current epoch to the dataset on epoch starts.
 
         When using the StreamingDataLoader, this is done automatically
 
         """
         # If the state dict has been reloaded, don't override the current epoch
```

### Comparing `litdata-0.2.7/src/litdata/streaming/downloader.py` & `litdata-0.2.8/src/litdata/streaming/downloader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/item_loader.py` & `litdata-0.2.8/src/litdata/streaming/item_loader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/reader.py` & `litdata-0.2.8/src/litdata/streaming/reader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/resolver.py` & `litdata-0.2.8/src/litdata/streaming/resolver.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/sampler.py` & `litdata-0.2.8/src/litdata/streaming/sampler.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/serializers.py` & `litdata-0.2.8/src/litdata/streaming/serializers.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/shuffle.py` & `litdata-0.2.8/src/litdata/streaming/shuffle.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/streaming/writer.py` & `litdata-0.2.8/src/litdata/streaming/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,17 @@
         self._chunks_info: List[Dict[str, Any]] = []
         self._worker_env: Optional[_WorkerEnv] = None
         self._rank: Optional[int] = None
         self._is_done = False
         self._distributed_env = _DistributedEnv.detect()
         self._follow_tensor_dimension = follow_tensor_dimension
 
+        self._per_sample_num_bytes = 0
+        self._per_sample_num_items = 0
+
     @property
     def filled(self) -> bool:
         """Returns whether the caching phase is done."""
         if self._is_done:
             return True
         files = os.listdir(self._cache_dir)
         index_files = [f for f in files if f.endswith(_INDEX_FILENAME)]
@@ -273,55 +276,86 @@
 
         This is handled by the samplers automatically. This ensures we can map an index to a shard from an interval.
 
         """
         self.add_item(index, items)
 
     def add_item(self, index: int, items: Any) -> Optional[str]:
-        # Track the minimum index provided to the writer
-        # Serialize the items and store an Item object.
+        """Given an index and items will serialize the items and store an Item object to the growing
+        `_serialized_items`."""
+
         if index in self._serialized_items:
             raise ValueError(f"The provided index {index} already exists in the cache.")
 
         data, dim = self.serialize(items)
         self._serialized_items[index] = Item(
             index=index,
             data=data,
             bytes=len(data),
             dim=dim,
         )
-
-        if not self._should_write():
+        if self._min_index is None:
+            # When processing the first item for the current chunk
+            indexes = list(self._serialized_items.keys())
+            self._max_index = self._min_index = indexes[0] if len(indexes) == 1 else min(*indexes)
+            self._per_sample_num_items = self._per_sample_num_bytes = 0
+            if not self._should_write():
+                return None
+        elif index < self._min_index:
+            # reset the "temp" chunk
+            self._max_index = self._min_index = index
+            self._per_sample_num_items = self._per_sample_num_bytes = 0
+            if not self._should_write():
+                return None
+        elif index == self._max_index:
+            if not self._should_write():
+                return None
+        else:
             return None
+
         filepath = os.path.join(self._cache_dir, self.get_chunk_filename())
+
         self.write_chunk()
+
+        # now to reset
         self._min_index = None
         self._max_index = None
+        self._per_sample_num_bytes = 0
+        self._per_sample_num_items = 0
+
         return filepath
 
     def _should_write(self) -> bool:
         # TODO: Misleading method name, it modifies `self._min_index` and `self._max_index`!
         if not self._serialized_items:
             return False
-        indexes = list(self._serialized_items.keys())
-        self._min_index = index = indexes[0] if len(indexes) == 1 else min(*indexes)
-        num_bytes = 0
-        num_items = 0
+
+        if not isinstance(self._max_index, int):
+            return False
+
+        # We have already validated the indexes from the interval `min_index` to `max_index`` are in `_serialized_items`
+        # Resetting the num_bytes and  num_items back the values.
+        num_bytes = self._per_sample_num_bytes
+        num_items = self._per_sample_num_items
+        index = self._max_index
         while True:
             item = self._serialized_items.get(index, None)
             if item:
                 num_bytes += item.bytes
                 num_items += item.dim if item.dim else 1
                 index += 1
                 if (self._chunk_bytes and self._chunk_bytes < num_bytes) or (
                     self._chunk_size and num_items > self._chunk_size
                 ):
                     self._max_index = index - 1
                     return True
             else:
+                self._per_sample_num_bytes = num_bytes
+                self._per_sample_num_items = num_items
+                self._max_index = index
                 return False
 
     def write_chunk_to_file(
         self,
         raw_data: bytes,
         filename: str,
     ) -> None:
```

### Comparing `litdata-0.2.7/src/litdata/utilities/__init__.py` & `litdata-0.2.8/src/litdata/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/utilities/_pytree.py` & `litdata-0.2.8/src/litdata/utilities/_pytree.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/utilities/broadcast.py` & `litdata-0.2.8/src/litdata/utilities/broadcast.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/utilities/env.py` & `litdata-0.2.8/src/litdata/utilities/env.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/utilities/format.py` & `litdata-0.2.8/src/litdata/utilities/format.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/utilities/packing.py` & `litdata-0.2.8/src/litdata/utilities/packing.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata/utilities/shuffle.py` & `litdata-0.2.8/src/litdata/utilities/shuffle.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.7/src/litdata.egg-info/PKG-INFO` & `litdata-0.2.8/src/litdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.7
+Version: 0.2.8
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -220,15 +220,15 @@
 ## The Map Operator
 
 The `map` operator can be used to apply a function over a list of inputs.
 
 Here is an example where the `map` operator is used to apply a `resize_image` function over a folder of large images.
 
 ```python
-from lightning.data import map
+from litdata import map
 from PIL import Image
 
 # Note: Inputs could also refer to files on s3 directly.
 input_dir = "my_large_images"
 inputs = [os.path.join(input_dir, f) for f in os.listdir(input_dir)]
 
 # The resize image takes one of the input (image_path) and the output directory. 
@@ -365,15 +365,15 @@
 ```
 
 ## On-Prem Optimizations
 
 On-prem compute nodes can mount and use a network drive. A network drive is a shared storage device on a local area network. In order to reduce their network overload, the `StreamingDataset` supports `caching` the data chunks.
 
 ```python
-from lightning.data import StreamingDataset
+from litdata import StreamingDataset
 
 dataset = StreamingDataset(input_dir="local:/data/shared-drive/some-data")
 ```
 
 # Benchmarks
 
 In order to measure the effectiveness of LitData, we used a commonly used dataset for benchmarks: [Imagenet-1.2M](https://www.image-net.org/) where the training set contains `1,281,167 images`.
```

### Comparing `litdata-0.2.7/src/litdata.egg-info/SOURCES.txt` & `litdata-0.2.8/src/litdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

