# Comparing `tmp/ai_alchemy-0.1.9.tar.gz` & `tmp/ai_alchemy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_alchemy-0.1.9.tar", max compression
+gzip compressed data, was "ai_alchemy-1.0.1.tar", max compression
```

## Comparing `ai_alchemy-0.1.9.tar` & `ai_alchemy-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1265 2024-05-26 14:16:20.744590 ai_alchemy-0.1.9/README.md
--rw-r--r--   0        0        0       45 2024-05-26 15:24:57.954957 ai_alchemy-0.1.9/ai_alchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.9/ai_alchemy/core/__init__.py
--rw-r--r--   0        0        0     1174 2024-05-26 16:29:09.853607 ai_alchemy-0.1.9/ai_alchemy/core/ai.py
--rw-r--r--   0        0        0     3905 2024-05-26 15:38:51.615577 ai_alchemy-0.1.9/ai_alchemy/core/cast.py
--rw-r--r--   0        0        0      623 2024-05-26 16:30:24.158354 ai_alchemy-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 ai_alchemy-0.1.9/setup.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 ai_alchemy-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1265 2024-05-26 14:16:20.744590 ai_alchemy-1.0.1/README.md
+-rw-r--r--   0        0        0       45 2024-05-26 15:24:57.954957 ai_alchemy-1.0.1/ai_alchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-1.0.1/ai_alchemy/core/__init__.py
+-rw-r--r--   0        0        0     5468 2024-06-03 01:40:51.861566 ai_alchemy-1.0.1/ai_alchemy/core/ai.py
+-rw-r--r--   0        0        0     7606 2024-06-03 01:42:25.134801 ai_alchemy-1.0.1/ai_alchemy/core/cast.py
+-rw-r--r--   0        0        0        0 2024-05-26 16:39:17.815727 ai_alchemy-1.0.1/ai_alchemy/core/py.typed
+-rw-r--r--   0        0        0      728 2024-06-03 01:47:25.078772 ai_alchemy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 ai_alchemy-1.0.1/setup.py
+-rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 ai_alchemy-1.0.1/PKG-INFO
```

### Comparing `ai_alchemy-0.1.9/README.md` & `ai_alchemy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ai_alchemy-0.1.9/setup.py` & `ai_alchemy-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['openai>=1.30.1,<2.0.0',
  'pandas-stubs>=2.2.2.240514,<3.0.0.0',
- 'pandas>=2.2.2,<3.0.0',
  'pydantic>=2.7.1,<3.0.0',
  'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'ai-alchemy',
-    'version': '0.1.9',
+    'version': '1.0.1',
     'description': 'Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic.',
     'long_description': '# AI Alchemy\n\nAI Alchemy is a Python library that provides a convenient way to interact with AI models, such as OpenAI\'s GPT-3.5 Turbo, and perform transformations on data.\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nYou need to have Python installed on your machine. You can download Python [here](https://www.python.org/downloads/).\n\n### Installation\n\nYou can install AI Alchemy via pip:\n\n```bash\npip install ai_alchemy\n```\n\n### Usage\nHere\'s a basic example of how to use AI Alchemy:\n\n```python\n# Import necessary libraries\nimport os\nimport ai_alchemy\nfrom ai_alchemy.ai import OpenAIWrapper\nfrom pydantic import BaseModel\n\n# Instantiate a wrapper for an AI model\nopenai = OpenAIWrapper(api_key=os.environ["OPENAI_API_KEY"], model="gpt-3.5-turbo")\n\n# Define a Pydantic model\nclass User(BaseModel):\n    name: str\n    age: int\n\n# Input data\ndata = "John Smith is 25 years old, five foot ten inches tall, and weighs 150 pounds."\n\n# Use AI Alchemy to transform the data into a Pydantic model\nmodel = ai_alchemy.cast.str_to_pydantic_model(data, openai, User)\n\n# Now `model` is a `User` instance with `name` and `age` populated from `data`\n```',
     'author': 'Josh Mogil',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ai_alchemy-0.1.9/PKG-INFO` & `ai_alchemy-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: ai-alchemy
-Version: 0.1.9
+Version: 1.0.1
 Summary: Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic.
 Author: Josh Mogil
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=1.30.1,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.2.2.240514,<3.0.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # AI Alchemy
```

