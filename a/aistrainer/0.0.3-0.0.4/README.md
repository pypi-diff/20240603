# Comparing `tmp/aistrainer-0.0.3.tar.gz` & `tmp/aistrainer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistrainer-0.0.3.tar", last modified: Tue May 28 11:09:56 2024, max compression
+gzip compressed data, was "aistrainer-0.0.4.tar", last modified: Mon Jun  3 08:35:42 2024, max compression
```

## Comparing `aistrainer-0.0.3.tar` & `aistrainer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 11:09:56.706328 aistrainer-0.0.3/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-24 14:22:02.000000 aistrainer-0.0.3/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6536 2024-05-28 11:09:56.706328 aistrainer-0.0.3/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)     5826 2024-05-28 09:16:12.000000 aistrainer-0.0.3/README.md
--rw-r--r--   0 man4j     (1000) man4j     (1000)      741 2024-05-28 11:09:45.000000 aistrainer-0.0.3/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-28 11:09:56.706328 aistrainer-0.0.3/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 11:09:56.706328 aistrainer-0.0.3/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 11:09:56.706328 aistrainer-0.0.3/src/aistrainer/
--rw-r--r--   0 man4j     (1000) man4j     (1000)    10328 2024-05-28 11:09:35.000000 aistrainer-0.0.3/src/aistrainer/aistrainer.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1830 2024-05-24 09:19:49.000000 aistrainer-0.0.3/src/aistrainer/models.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-28 11:09:56.706328 aistrainer-0.0.3/src/aistrainer.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6536 2024-05-28 11:09:56.000000 aistrainer-0.0.3/src/aistrainer.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      275 2024-05-28 11:09:56.000000 aistrainer-0.0.3/src/aistrainer.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-28 11:09:56.000000 aistrainer-0.0.3/src/aistrainer.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       90 2024-05-28 11:09:56.000000 aistrainer-0.0.3/src/aistrainer.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       11 2024-05-28 11:09:56.000000 aistrainer-0.0.3/src/aistrainer.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-24 14:22:02.000000 aistrainer-0.0.4/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     7270 2024-06-03 08:35:42.813174 aistrainer-0.0.4/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6560 2024-06-03 08:35:04.000000 aistrainer-0.0.4/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      741 2024-06-03 08:35:11.000000 aistrainer-0.0.4/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-06-03 08:35:42.813174 aistrainer-0.0.4/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/src/aistrainer/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)    10328 2024-05-28 11:25:03.000000 aistrainer-0.0.4/src/aistrainer/aistrainer.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1830 2024-05-24 09:19:49.000000 aistrainer-0.0.4/src/aistrainer/models.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-06-03 08:35:42.813174 aistrainer-0.0.4/src/aistrainer.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     7270 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      275 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       90 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       11 2024-06-03 08:35:42.000000 aistrainer-0.0.4/src/aistrainer.egg-info/top_level.txt
```

### Comparing `aistrainer-0.0.3/LICENSE` & `aistrainer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.3/PKG-INFO` & `aistrainer-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,14 @@
-Metadata-Version: 2.1
-Name: aistrainer
-Version: 0.0.3
-Summary: AI Specialization Trainer for LLM models
-Author-email: Vladimir Petrukhin <man4j@ya.ru>
-Project-URL: Homepage, https://github.com/Equiron-AI/aistrainer
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: transformers>=4.41.1
-Requires-Dist: datasets>=2.19.1
-Requires-Dist: peft>=0.11.1
-Requires-Dist: deepspeed==0.14.0
-Requires-Dist: sentencepiece>=0.2.0
-
 # Welcome to AISTrainer!
 **Aistrainer** is a library built on top of **Hugging Face Transformers**, designed to simplify the process of fine-tuning large language models (LLMs) for developers. It focuses on making LLM fine-tuning feasible even with limited computational resources, such as Nvidia GeForce RTX 3090 GPUs. The library supports training on both GPUs and CPUs, and it includes a feature for offloading model weights to the CPU when using a single GPU. With one **Nvidia GeForce RTX 3090 GPU** and **256 GB of RAM**, Aistrainer can handle fine-tuning models with up to approximately **70 billion** parameters.
 
 ## Environment
 The Aistrainer library is compatible with the Ubuntu 22.04 operating system. To set up the required environment for this library, system tools must be installed using the command: 
 ```console
-sudo apt install -y python3-pip ccache make cmake g++ mpich conda
+sudo apt install -y python3-pip ccache make cmake g++ mpich
 ```
 To create a Python virtual environment with a GPU, use the command:
 ```console
 conda env create -f environment.yml
 ``` 
 In the absence of a GPU, the environment can be set up with the command: 
 ```console
@@ -102,16 +82,19 @@
            lora_alpha=32,
            batch_size=4,  # suitable for most cases, but should be reduced if there is not enough GPU memory
            gradient_steps=2)  # suitable for most cases, but should be reduced if there is not enough GPU memory
 ```
 
 ## Combining/merging LoRA adapters
 ```python
+import logging
 from aistrainer.aistrainer import Aist
 
+logging.basicConfig(level=logging.INFO)
+
 aist = Aist("CohereForAI/c4ai-command-r-v01")
 aist.merge("model_with_safety", "safety_adapter")
 ```
 
 ## Known issues
 Model fine-tuning and combining adapters cannot be performed in the same bash script or Jupyter session. It is essential to separate the processes of fine-tuning and adapter merging. When using JupyterLab, you must restart the kernel after completing each of these processes to ensure proper execution and avoid conflicts.
 
@@ -121,7 +104,24 @@
 llama.cpp/build/bin/quantize model.gguf model_q5_k_m.gguf q5_k_m
 ```
 
 ## Run with Llama.CPP Server on GPU
 ```console
 llama.cpp/build/bin/server -m model_q5_k_m.gguf -ngl 99 -fa -cb -c 4096 --host 0.0.0.0 --port 8000
 ```
+
+## Install CUDA toolkit for Llama.cpp compilation
+Please note that the toolkit version must match the driver version. The driver version can be found using the nvidia-smi command.
+Аor example, to install toolkit for CUDA 12.2 you need to run the following commands:
+```console
+CUDA_TOOLKIT_VERSION=12-2
+wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/cuda-keyring_1.1-1_all.deb
+sudo dpkg -i cuda-keyring_1.1-1_all.deb
+sudo apt update
+sudo apt -y install cuda-toolkit-${CUDA_TOOLKIT_VERSION}
+echo -e '
+export CUDA_HOME=/usr/local/cuda
+export PATH=${CUDA_HOME}/bin:${PATH}
+export LD_LIBRARY_PATH=${CUDA_HOME}/lib64:$LD_LIBRARY_PATH
+' >> ~/.bashrc
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aistrainer-0.0.3/README.md` & `aistrainer-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,34 @@
+Metadata-Version: 2.1
+Name: aistrainer
+Version: 0.0.4
+Summary: AI Specialization Trainer for LLM models
+Author-email: Vladimir Petrukhin <man4j@ya.ru>
+Project-URL: Homepage, https://github.com/Equiron-AI/aistrainer
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: transformers>=4.41.1
+Requires-Dist: datasets>=2.19.1
+Requires-Dist: peft>=0.11.1
+Requires-Dist: deepspeed==0.14.0
+Requires-Dist: sentencepiece>=0.2.0
+
 # Welcome to AISTrainer!
 **Aistrainer** is a library built on top of **Hugging Face Transformers**, designed to simplify the process of fine-tuning large language models (LLMs) for developers. It focuses on making LLM fine-tuning feasible even with limited computational resources, such as Nvidia GeForce RTX 3090 GPUs. The library supports training on both GPUs and CPUs, and it includes a feature for offloading model weights to the CPU when using a single GPU. With one **Nvidia GeForce RTX 3090 GPU** and **256 GB of RAM**, Aistrainer can handle fine-tuning models with up to approximately **70 billion** parameters.
 
 ## Environment
 The Aistrainer library is compatible with the Ubuntu 22.04 operating system. To set up the required environment for this library, system tools must be installed using the command: 
 ```console
-sudo apt install -y python3-pip ccache make cmake g++ mpich conda
+sudo apt install -y python3-pip ccache make cmake g++ mpich
 ```
 To create a Python virtual environment with a GPU, use the command:
 ```console
 conda env create -f environment.yml
 ``` 
 In the absence of a GPU, the environment can be set up with the command: 
 ```console
@@ -82,16 +102,19 @@
            lora_alpha=32,
            batch_size=4,  # suitable for most cases, but should be reduced if there is not enough GPU memory
            gradient_steps=2)  # suitable for most cases, but should be reduced if there is not enough GPU memory
 ```
 
 ## Combining/merging LoRA adapters
 ```python
+import logging
 from aistrainer.aistrainer import Aist
 
+logging.basicConfig(level=logging.INFO)
+
 aist = Aist("CohereForAI/c4ai-command-r-v01")
 aist.merge("model_with_safety", "safety_adapter")
 ```
 
 ## Known issues
 Model fine-tuning and combining adapters cannot be performed in the same bash script or Jupyter session. It is essential to separate the processes of fine-tuning and adapter merging. When using JupyterLab, you must restart the kernel after completing each of these processes to ensure proper execution and avoid conflicts.
 
@@ -101,7 +124,24 @@
 llama.cpp/build/bin/quantize model.gguf model_q5_k_m.gguf q5_k_m
 ```
 
 ## Run with Llama.CPP Server on GPU
 ```console
 llama.cpp/build/bin/server -m model_q5_k_m.gguf -ngl 99 -fa -cb -c 4096 --host 0.0.0.0 --port 8000
 ```
+
+## Install CUDA toolkit for Llama.cpp compilation
+Please note that the toolkit version must match the driver version. The driver version can be found using the nvidia-smi command.
+Аor example, to install toolkit for CUDA 12.2 you need to run the following commands:
+```console
+CUDA_TOOLKIT_VERSION=12-2
+wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/cuda-keyring_1.1-1_all.deb
+sudo dpkg -i cuda-keyring_1.1-1_all.deb
+sudo apt update
+sudo apt -y install cuda-toolkit-${CUDA_TOOLKIT_VERSION}
+echo -e '
+export CUDA_HOME=/usr/local/cuda
+export PATH=${CUDA_HOME}/bin:${PATH}
+export LD_LIBRARY_PATH=${CUDA_HOME}/lib64:$LD_LIBRARY_PATH
+' >> ~/.bashrc
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aistrainer-0.0.3/pyproject.toml` & `aistrainer-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aistrainer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
 description = "AI Specialization Trainer for LLM models"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `aistrainer-0.0.3/src/aistrainer/aistrainer.py` & `aistrainer-0.0.4/src/aistrainer/aistrainer.py`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.3/src/aistrainer/models.py` & `aistrainer-0.0.4/src/aistrainer/models.py`

 * *Files identical despite different names*

### Comparing `aistrainer-0.0.3/src/aistrainer.egg-info/PKG-INFO` & `aistrainer-0.0.4/src/aistrainer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistrainer
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI Specialization Trainer for LLM models
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aistrainer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 
 # Welcome to AISTrainer!
 **Aistrainer** is a library built on top of **Hugging Face Transformers**, designed to simplify the process of fine-tuning large language models (LLMs) for developers. It focuses on making LLM fine-tuning feasible even with limited computational resources, such as Nvidia GeForce RTX 3090 GPUs. The library supports training on both GPUs and CPUs, and it includes a feature for offloading model weights to the CPU when using a single GPU. With one **Nvidia GeForce RTX 3090 GPU** and **256 GB of RAM**, Aistrainer can handle fine-tuning models with up to approximately **70 billion** parameters.
 
 ## Environment
 The Aistrainer library is compatible with the Ubuntu 22.04 operating system. To set up the required environment for this library, system tools must be installed using the command: 
 ```console
-sudo apt install -y python3-pip ccache make cmake g++ mpich conda
+sudo apt install -y python3-pip ccache make cmake g++ mpich
 ```
 To create a Python virtual environment with a GPU, use the command:
 ```console
 conda env create -f environment.yml
 ``` 
 In the absence of a GPU, the environment can be set up with the command: 
 ```console
@@ -102,16 +102,19 @@
            lora_alpha=32,
            batch_size=4,  # suitable for most cases, but should be reduced if there is not enough GPU memory
            gradient_steps=2)  # suitable for most cases, but should be reduced if there is not enough GPU memory
 ```
 
 ## Combining/merging LoRA adapters
 ```python
+import logging
 from aistrainer.aistrainer import Aist
 
+logging.basicConfig(level=logging.INFO)
+
 aist = Aist("CohereForAI/c4ai-command-r-v01")
 aist.merge("model_with_safety", "safety_adapter")
 ```
 
 ## Known issues
 Model fine-tuning and combining adapters cannot be performed in the same bash script or Jupyter session. It is essential to separate the processes of fine-tuning and adapter merging. When using JupyterLab, you must restart the kernel after completing each of these processes to ensure proper execution and avoid conflicts.
 
@@ -121,7 +124,24 @@
 llama.cpp/build/bin/quantize model.gguf model_q5_k_m.gguf q5_k_m
 ```
 
 ## Run with Llama.CPP Server on GPU
 ```console
 llama.cpp/build/bin/server -m model_q5_k_m.gguf -ngl 99 -fa -cb -c 4096 --host 0.0.0.0 --port 8000
 ```
+
+## Install CUDA toolkit for Llama.cpp compilation
+Please note that the toolkit version must match the driver version. The driver version can be found using the nvidia-smi command.
+Аor example, to install toolkit for CUDA 12.2 you need to run the following commands:
+```console
+CUDA_TOOLKIT_VERSION=12-2
+wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/cuda-keyring_1.1-1_all.deb
+sudo dpkg -i cuda-keyring_1.1-1_all.deb
+sudo apt update
+sudo apt -y install cuda-toolkit-${CUDA_TOOLKIT_VERSION}
+echo -e '
+export CUDA_HOME=/usr/local/cuda
+export PATH=${CUDA_HOME}/bin:${PATH}
+export LD_LIBRARY_PATH=${CUDA_HOME}/lib64:$LD_LIBRARY_PATH
+' >> ~/.bashrc
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

