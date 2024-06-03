# Comparing `tmp/Agentic_Employment-0.0.1-py3-none-any.whl.zip` & `tmp/Agentic_Employment-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 26042 bytes, number of entries: 10
+Zip file size: 26612 bytes, number of entries: 11
 -rw-rw-rw-  2.0 unx       24 b- defN 24-May-13 21:40 frontend/__init__.py
 -rw-rw-rw-  2.0 unx    61752 b- defN 24-May-13 21:40 frontend/main.py
 -rw-rw-rw-  2.0 unx       26 b- defN 24-May-13 21:40 frontend/components/__init__.py
 -rw-rw-rw-  2.0 unx      194 b- defN 24-May-13 21:40 frontend/components/agent_dashboard.py
 -rw-rw-rw-  2.0 unx      171 b- defN 24-May-13 21:40 frontend/components/settings.py
--rw-rw-rw-  2.0 unx    11357 b- defN 24-Jun-03 04:03 Agentic_Employment-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 unx    11418 b- defN 24-Jun-03 04:03 Agentic_Employment-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 24-Jun-03 04:03 Agentic_Employment-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 24-Jun-03 04:03 Agentic_Employment-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      858 b- defN 24-Jun-03 04:03 Agentic_Employment-0.0.1.dist-info/RECORD
-10 files, 85901 bytes uncompressed, 24560 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 unx    11357 b- defN 24-Jun-03 04:19 Agentic_Employment-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx    11997 b- defN 24-Jun-03 04:19 Agentic_Employment-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 24-Jun-03 04:19 Agentic_Employment-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       71 b- defN 24-Jun-03 04:19 Agentic_Employment-0.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 unx        9 b- defN 24-Jun-03 04:19 Agentic_Employment-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      964 b- defN 24-Jun-03 04:19 Agentic_Employment-0.0.2.dist-info/RECORD
+11 files, 86657 bytes uncompressed, 24952 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: frontend/components/agent_dashboard.py
 Comment: 
 
 Filename: frontend/components/settings.py
 Comment: 
 
-Filename: Agentic_Employment-0.0.1.dist-info/LICENSE
+Filename: Agentic_Employment-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: Agentic_Employment-0.0.1.dist-info/METADATA
+Filename: Agentic_Employment-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Agentic_Employment-0.0.1.dist-info/WHEEL
+Filename: Agentic_Employment-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Agentic_Employment-0.0.1.dist-info/top_level.txt
+Filename: Agentic_Employment-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: Agentic_Employment-0.0.1.dist-info/RECORD
+Filename: Agentic_Employment-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: Agentic_Employment-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Agentic_Employment-0.0.1.dist-info/LICENSE` & `Agentic_Employment-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Agentic_Employment-0.0.1.dist-info/METADATA` & `Agentic_Employment-0.0.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agentic-Employment
-Version: 0.0.1
+Version: 0.0.2
 Summary: an Agentic Employment Infrastructure
 Home-page: https://github.com/ruvnet/agentic-employment
 Author: rUv
 Author-email: null@ruv.net
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,17 @@
 Requires-Dist: twine
 Requires-Dist: setuptools
 Requires-Dist: wheel
 Requires-Dist: flake8
 Requires-Dist: black
 Requires-Dist: pytest
 Requires-Dist: pip-upgrader
+Requires-Dist: fastapi
+Requires-Dist: uvicorn
+Requires-Dist: python-dotenv
 
 # 🪰 Agentic Employment Infrastructure
 [![Agentic Employment](https://github.com/ruvnet/agentic-employment/blob/main/assets/agentic-one.png.png?raw=true)](https://huggingface.co/spaces/ruv/agentic-employment)
 
 This project implements an Agentic Employment Infrastructure using FastAPI, Flask, Websockets, LiteLLM, and Gradio. The infrastructure aims to manage and enhance various aspects of workforce management through advanced autonomous agents.
 
 The primary focus of the Agentic Employment Infrastructure is to streamline and optimize employment processes. It automates routine tasks, facilitates real-time communication, and integrates seamlessly with existing systems. The platform supports a wide range of functionalities, including agent management, task automation, collaboration tools, and advanced configuration options.
@@ -40,14 +43,35 @@
 
 Check out the demo of the Agentic Employment Infrastructure on Hugging Face Spaces: [Agentic Employment Demo](https://huggingface.co/spaces/ruv/agentic-employment)
 
 ## Purpose of the Application
 
 The Agentic Employment Infrastructure aims to revolutionize the way businesses manage and interact with their workforce. By leveraging cutting-edge AI and machine learning technologies, this platform automates routine tasks, optimizes workforce management, and provides insightful analytics to drive decision-making.
 
+## Installation
+
+You can install the Agentic Employment package using `pip`. Make sure you have Python installed, then run the following command:
+
+```bash
+pip install Agentic-Employment
+```
+
+## Run
+```
+agentic-employment
+```
+
+Configuration
+The application uses environment variables for configuration. You can set these variables in a .env file in the root directory of your project. Here is an example of the .env file:
+
+```
+SECRET_KEY=your_secret_key
+ALGORITHM=HS256
+ACCESS_TOKEN_EXPIRE_MINUTES=30
+```
 ## Benefits
 
 - **Efficiency**: Automates routine and complex tasks, reducing the need for manual intervention and speeding up processes.
 - **Scalability**: Easily scales to meet the needs of any organization size, from small businesses to large enterprises.
 - **Customization**: Highly customizable to fit specific organizational needs and workflows.
 - **Insightful Analytics**: Offers deep insights into workforce performance and operational efficiency, enabling better strategic planning.
 - **Cost-Effective**: Reduces operational costs by automating tasks and optimizing resource allocation.
```

## Comparing `Agentic_Employment-0.0.1.dist-info/RECORD` & `Agentic_Employment-0.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 frontend/__init__.py,sha256=rMHLnSWzM4xnImRv_jFUGOMMxQM3YHKXYN3jt_mW_KM,24
 frontend/main.py,sha256=5hAtrmnLNInY3cKz7E2qTfehsDD4qjEQOzvI8IUpm_o,61752
 frontend/components/__init__.py,sha256=JPnT9i5YNWg4RmjwIHcGG7Ttr0T0wF0alY-a6Abgf1Y,26
 frontend/components/agent_dashboard.py,sha256=G4bOh6Hy35VXGgoD9B7OpXZywWqroMRzoBlKfzcyoiQ,194
 frontend/components/settings.py,sha256=dQ5eD6AGeNQJrm4Hn8s9ubdz3L7lYh8mHgUmVuv-HaI,171
-Agentic_Employment-0.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-Agentic_Employment-0.0.1.dist-info/METADATA,sha256=bD3lH9tM9ApycuQQeQYpaGHpaW_H4MO-hJrKjuHEUXI,11418
-Agentic_Employment-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Agentic_Employment-0.0.1.dist-info/top_level.txt,sha256=PqYVS3-YFgm6PaA3CFiN65TIrNSJkrAsNSmI0SKBeAU,9
-Agentic_Employment-0.0.1.dist-info/RECORD,,
+Agentic_Employment-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+Agentic_Employment-0.0.2.dist-info/METADATA,sha256=U1M-E58leZ3H18eOgryiYibgyQXEQtmIv7Ixoucp0JE,11997
+Agentic_Employment-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Agentic_Employment-0.0.2.dist-info/entry_points.txt,sha256=UFyb5YR8o9xLpZH9FwJafOUlbVu8rRS3H6mVZEMU8sE,71
+Agentic_Employment-0.0.2.dist-info/top_level.txt,sha256=PqYVS3-YFgm6PaA3CFiN65TIrNSJkrAsNSmI0SKBeAU,9
+Agentic_Employment-0.0.2.dist-info/RECORD,,
```

