# Comparing `tmp/jetson_examples-0.1.2.tar.gz` & `tmp/jetson_examples-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson_examples-0.1.2.tar", last modified: Fri May 31 06:54:32 2024, max compression
+gzip compressed data, was "jetson_examples-0.1.3.tar", last modified: Mon Jun  3 02:21:40 2024, max compression
```

## Comparing `jetson_examples-0.1.2.tar` & `jetson_examples-0.1.3.tar`

### file list

```diff
@@ -1,81 +1,88 @@
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1066 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/LICENSE
--rw-r--r--   0 youjiang  (1000) youjiang  (1000)     5007 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/PKG-INFO
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     4357 2024-05-31 06:53:02.000000 jetson_examples-0.1.2/README.md
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/jetson_examples.egg-info/
--rw-r--r--   0 youjiang  (1000) youjiang  (1000)     5007 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/PKG-INFO
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2114 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/SOURCES.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        1 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/dependency_links.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       58 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/entry_points.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       27 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/top_level.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1081 2024-05-30 07:28:59.000000 jetson_examples-0.1.2/pyproject.toml
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       22 2024-05-30 07:29:30.000000 jetson_examples-0.1.2/reComputer/__init__.py
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2088 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/main.py
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      237 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/audiocraft/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      951 2024-05-29 08:42:13.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/README.md
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       77 2024-05-29 07:36:41.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/clean.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:41.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:41.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/run.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      127 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/check.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      898 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/clean.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/live-llava/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/live-llava/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)    10137 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/live-llava/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llama3/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llama3/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      328 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llama3/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llava/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       70 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava/clean.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llava-v1.5-7b/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.5-7b/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.5-7b/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llava-v1.6-vicuna-7b/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.6-vicuna-7b/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      269 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/nanodb/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanodb/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      247 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanodb/readme.md
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2571 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanodb/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/nanoowl/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanoowl/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      264 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanoowl/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/ollama/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/ollama/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      246 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/ollama/run.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1032 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/stable-diffusion-webui/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/stable-diffusion-webui/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/stable-diffusion-webui/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/text-generation-webui/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/text-generation-webui/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      407 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/text-generation-webui/run.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      900 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/update.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/whisper/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/whisper/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      146 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/whisper/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/yolov10/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      466 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/Dockerfile
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     3123 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/README.md
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/yolov10/assets/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)  2600779 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/assets/webui.png
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      106 2024-05-31 06:49:00.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/clean.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1679 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      289 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2008 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/readme.md
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      809 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      167 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/Dockerfile
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1122 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/README.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1307 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/app.py
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      130 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/templates/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      524 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/templates/index.html
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       38 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/setup.cfg
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.571802 jetson_examples-0.1.3/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1066 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/LICENSE
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     5146 2024-06-03 02:21:40.571802 jetson_examples-0.1.3/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     4496 2024-06-03 02:20:59.000000 jetson_examples-0.1.3/README.md
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.571802 jetson_examples-0.1.3/jetson_examples.egg-info/
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     5146 2024-06-03 02:21:40.000000 jetson_examples-0.1.3/jetson_examples.egg-info/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2365 2024-06-03 02:21:40.000000 jetson_examples-0.1.3/jetson_examples.egg-info/SOURCES.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        1 2024-06-03 02:21:40.000000 jetson_examples-0.1.3/jetson_examples.egg-info/dependency_links.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       58 2024-06-03 02:21:40.000000 jetson_examples-0.1.3/jetson_examples.egg-info/entry_points.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       27 2024-06-03 02:21:40.000000 jetson_examples-0.1.3/jetson_examples.egg-info/top_level.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1081 2024-06-03 02:21:20.000000 jetson_examples-0.1.3/pyproject.toml
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       22 2024-06-03 02:21:16.000000 jetson_examples-0.1.3/reComputer/__init__.py
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2088 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/main.py
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      237 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/audiocraft/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      951 2024-05-29 08:42:13.000000 jetson_examples-0.1.3/reComputer/scripts/audiocraft/README.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       77 2024-05-29 07:36:41.000000 jetson_examples-0.1.3/reComputer/scripts/audiocraft/clean.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:41.000000 jetson_examples-0.1.3/reComputer/scripts/audiocraft/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:41.000000 jetson_examples-0.1.3/reComputer/scripts/audiocraft/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      127 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/check.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      898 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/clean.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/live-llava/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/live-llava/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)    10137 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/live-llava/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/llama3/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llama3/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      328 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llama3/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/llava/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       70 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llava/clean.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llava/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llava/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/llava-v1.5-7b/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llava-v1.5-7b/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llava-v1.5-7b/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/llava-v1.6-vicuna-7b/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llava-v1.6-vicuna-7b/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      269 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/nanodb/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/nanodb/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      247 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/nanodb/readme.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2571 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/nanodb/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/nanoowl/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/nanoowl/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      264 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/nanoowl/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/ollama/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/ollama/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      246 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/ollama/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1032 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/stable-diffusion-webui/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/stable-diffusion-webui/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/stable-diffusion-webui/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.563801 jetson_examples-0.1.3/reComputer/scripts/text-generation-webui/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/text-generation-webui/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      407 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/text-generation-webui/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.567802 jetson_examples-0.1.3/reComputer/scripts/ultralytics-yolo/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2337 2024-06-03 02:20:59.000000 jetson_examples-0.1.3/reComputer/scripts/ultralytics-yolo/README.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       63 2024-06-03 02:20:59.000000 jetson_examples-0.1.3/reComputer/scripts/ultralytics-yolo/clean.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.567802 jetson_examples-0.1.3/reComputer/scripts/ultralytics-yolo/images/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)  1315335 2024-06-03 02:20:59.000000 jetson_examples-0.1.3/reComputer/scripts/ultralytics-yolo/images/Ultralytics-yolo.gif
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)   275724 2024-06-03 02:20:59.000000 jetson_examples-0.1.3/reComputer/scripts/ultralytics-yolo/images/tasks.png
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      287 2024-06-03 02:20:59.000000 jetson_examples-0.1.3/reComputer/scripts/ultralytics-yolo/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      900 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/update.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.567802 jetson_examples-0.1.3/reComputer/scripts/whisper/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/whisper/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      146 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/whisper/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.567802 jetson_examples-0.1.3/reComputer/scripts/yolov10/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      466 2024-05-31 06:47:18.000000 jetson_examples-0.1.3/reComputer/scripts/yolov10/Dockerfile
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     3623 2024-05-31 09:22:10.000000 jetson_examples-0.1.3/reComputer/scripts/yolov10/README.md
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.567802 jetson_examples-0.1.3/reComputer/scripts/yolov10/assets/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)  2600779 2024-05-31 06:47:18.000000 jetson_examples-0.1.3/reComputer/scripts/yolov10/assets/webui.png
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      106 2024-05-31 06:49:00.000000 jetson_examples-0.1.3/reComputer/scripts/yolov10/clean.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1679 2024-05-31 06:47:18.000000 jetson_examples-0.1.3/reComputer/scripts/yolov10/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      289 2024-05-31 06:47:18.000000 jetson_examples-0.1.3/reComputer/scripts/yolov10/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.567802 jetson_examples-0.1.3/reComputer/scripts/yolov8-rail-inspection/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2008 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/yolov8-rail-inspection/readme.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      809 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/yolov8-rail-inspection/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.567802 jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      167 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/Dockerfile
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1122 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/README.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1307 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/app.py
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      130 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-06-03 02:21:40.571802 jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/templates/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      524 2024-05-29 07:36:02.000000 jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/templates/index.html
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       38 2024-06-03 02:21:40.571802 jetson_examples-0.1.3/setup.cfg
```

### Comparing `jetson_examples-0.1.2/LICENSE` & `jetson_examples-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/PKG-INFO` & `jetson_examples-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.1.2
+Version: 0.1.3
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -66,14 +66,15 @@
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
 | [yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+| [ultralytics-yolo](/reComputer/scripts/ultralytics-yolo/README.md) |Computer Vision |  | 15.4GB  | `reComputer run  ultralytics-yolo`  |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 ## Development
 Want to add your own example? Check out the [development guide](./docs/develop.md).
```

### Comparing `jetson_examples-0.1.2/README.md` & `jetson_examples-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
 | [yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+| [ultralytics-yolo](/reComputer/scripts/ultralytics-yolo/README.md) |Computer Vision |  | 15.4GB  | `reComputer run  ultralytics-yolo`  |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 ## Development
 Want to add your own example? Check out the [development guide](./docs/develop.md).
```

### Comparing `jetson_examples-0.1.2/jetson_examples.egg-info/PKG-INFO` & `jetson_examples-0.1.3/jetson_examples.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.1.2
+Version: 0.1.3
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -66,14 +66,15 @@
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
 | [yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+| [ultralytics-yolo](/reComputer/scripts/ultralytics-yolo/README.md) |Computer Vision |  | 15.4GB  | `reComputer run  ultralytics-yolo`  |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 ## Development
 Want to add your own example? Check out the [development guide](./docs/develop.md).
```

### Comparing `jetson_examples-0.1.2/jetson_examples.egg-info/SOURCES.txt` & `jetson_examples-0.1.3/jetson_examples.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 reComputer/scripts/nanoowl/run.sh
 reComputer/scripts/ollama/init.sh
 reComputer/scripts/ollama/run.sh
 reComputer/scripts/stable-diffusion-webui/init.sh
 reComputer/scripts/stable-diffusion-webui/run.sh
 reComputer/scripts/text-generation-webui/init.sh
 reComputer/scripts/text-generation-webui/run.sh
+reComputer/scripts/ultralytics-yolo/README.md
+reComputer/scripts/ultralytics-yolo/clean.sh
+reComputer/scripts/ultralytics-yolo/run.sh
+reComputer/scripts/ultralytics-yolo/images/Ultralytics-yolo.gif
+reComputer/scripts/ultralytics-yolo/images/tasks.png
 reComputer/scripts/whisper/init.sh
 reComputer/scripts/whisper/run.sh
 reComputer/scripts/yolov10/Dockerfile
 reComputer/scripts/yolov10/README.md
 reComputer/scripts/yolov10/clean.sh
 reComputer/scripts/yolov10/init.sh
 reComputer/scripts/yolov10/run.sh
```

### Comparing `jetson_examples-0.1.2/pyproject.toml` & `jetson_examples-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jetson-examples"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "luozhixin", email = "zhixin.luo@seeed.cc" }]
 description = "Running Gen AI models and applications on NVIDIA Jetson devices with one-line command"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `jetson_examples-0.1.2/reComputer/main.py` & `jetson_examples-0.1.3/reComputer/main.py`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/audiocraft/README.md` & `jetson_examples-0.1.3/reComputer/scripts/audiocraft/README.md`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/clean.sh` & `jetson_examples-0.1.3/reComputer/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/live-llava/run.sh` & `jetson_examples-0.1.3/reComputer/scripts/live-llava/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/nanodb/run.sh` & `jetson_examples-0.1.3/reComputer/scripts/nanodb/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/run.sh` & `jetson_examples-0.1.3/reComputer/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/update.sh` & `jetson_examples-0.1.3/reComputer/scripts/update.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/yolov10/assets/webui.png` & `jetson_examples-0.1.3/reComputer/scripts/yolov10/assets/webui.png`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/yolov10/init.sh` & `jetson_examples-0.1.3/reComputer/scripts/yolov10/init.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/readme.md` & `jetson_examples-0.1.3/reComputer/scripts/yolov8-rail-inspection/readme.md`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/run.sh` & `jetson_examples-0.1.3/reComputer/scripts/yolov8-rail-inspection/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/README.txt` & `jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/README.txt`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/app.py` & `jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/app.py`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/templates/index.html` & `jetson_examples-0.1.3/reComputer/scripts/yolov8:detect/templates/index.html`

 * *Files identical despite different names*

