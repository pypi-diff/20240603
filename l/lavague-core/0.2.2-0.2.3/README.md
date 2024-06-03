# Comparing `tmp/lavague_core-0.2.2.tar.gz` & `tmp/lavague_core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.2.2.tar", max compression
+gzip compressed data, was "lavague_core-0.2.3.tar", max compression
```

## Comparing `lavague_core-0.2.2.tar` & `lavague_core-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-05-28 08:59:04.851483 lavague_core-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2024-05-28 08:59:04.851521 lavague_core-0.2.2/README.md
--rw-r--r--   0        0        0     1065 2024-05-31 09:04:25.699400 lavague_core-0.2.2/lavague/core/__init__.py
--rw-r--r--   0        0        0     5639 2024-05-31 09:22:12.315340 lavague_core-0.2.2/lavague/core/action_engine.py
--rw-r--r--   0        0        0      374 2024-05-28 08:59:04.852005 lavague_core-0.2.2/lavague/core/action_template.py
--rw-r--r--   0        0        0     2839 2024-05-31 09:13:21.375968 lavague_core-0.2.2/lavague/core/agents.py
--rw-r--r--   0        0        0     3084 2024-05-31 09:04:25.700281 lavague_core-0.2.2/lavague/core/base_driver.py
--rw-r--r--   0        0        0      248 2024-05-31 09:04:25.700517 lavague_core-0.2.2/lavague/core/base_engine.py
--rw-r--r--   0        0        0     1189 2024-05-29 15:40:38.733494 lavague_core-0.2.2/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-28 08:59:04.852453 lavague_core-0.2.2/lavague/core/extractors.py
--rw-r--r--   0        0        0     1282 2024-05-31 09:04:25.700605 lavague_core-0.2.2/lavague/core/logger.py
--rw-r--r--   0        0        0     1710 2024-05-31 09:04:25.700831 lavague_core-0.2.2/lavague/core/memory.py
--rw-r--r--   0        0        0    12884 2024-05-31 09:22:47.918942 lavague_core-0.2.2/lavague/core/navigation.py
--rw-r--r--   0        0        0     3641 2024-05-31 09:09:03.128947 lavague_core-0.2.2/lavague/core/python_engine.py
--rw-r--r--   0        0        0    12117 2024-05-28 08:59:04.852935 lavague_core-0.2.2/lavague/core/retrievers.py
--rw-r--r--   0        0        0     1795 2024-05-28 08:59:04.853008 lavague_core-0.2.2/lavague/core/rewriter.py
--rw-r--r--   0        0        0     5661 2024-05-31 09:04:25.701914 lavague_core-0.2.2/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     2056 2024-05-31 09:04:25.702490 lavague_core-0.2.2/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1430 2024-05-31 09:04:25.702632 lavague_core-0.2.2/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0     3402 2024-05-31 09:04:25.702910 lavague_core-0.2.2/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0    15134 2024-05-31 09:09:25.856069 lavague_core-0.2.2/lavague/core/world_model.py
--rw-r--r--   0        0        0     1128 2024-05-31 09:22:54.991300 lavague_core-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 lavague_core-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 08:59:04.851483 lavague_core-0.2.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-28 08:59:04.851521 lavague_core-0.2.3/README.md
+-rw-r--r--   0        0        0     1073 2024-06-03 07:24:25.756717 lavague_core-0.2.3/lavague/core/__init__.py
+-rw-r--r--   0        0        0     5639 2024-05-31 09:22:12.315340 lavague_core-0.2.3/lavague/core/action_engine.py
+-rw-r--r--   0        0        0      374 2024-05-28 08:59:04.852005 lavague_core-0.2.3/lavague/core/action_template.py
+-rw-r--r--   0        0        0     3409 2024-06-03 07:24:25.757053 lavague_core-0.2.3/lavague/core/agents.py
+-rw-r--r--   0        0        0     3084 2024-05-31 09:04:25.700281 lavague_core-0.2.3/lavague/core/base_driver.py
+-rw-r--r--   0        0        0      248 2024-05-31 09:04:25.700517 lavague_core-0.2.3/lavague/core/base_engine.py
+-rw-r--r--   0        0        0     1189 2024-05-29 15:40:38.733494 lavague_core-0.2.3/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-28 08:59:04.852453 lavague_core-0.2.3/lavague/core/extractors.py
+-rw-r--r--   0        0        0     1282 2024-05-31 09:04:25.700605 lavague_core-0.2.3/lavague/core/logger.py
+-rw-r--r--   0        0        0     1710 2024-05-31 09:04:25.700831 lavague_core-0.2.3/lavague/core/memory.py
+-rw-r--r--   0        0        0    17057 2024-06-03 07:24:25.757319 lavague_core-0.2.3/lavague/core/navigation.py
+-rw-r--r--   0        0        0     3641 2024-05-31 09:09:03.128947 lavague_core-0.2.3/lavague/core/python_engine.py
+-rw-r--r--   0        0        0    12117 2024-05-28 08:59:04.852935 lavague_core-0.2.3/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     1795 2024-05-28 08:59:04.853008 lavague_core-0.2.3/lavague/core/rewriter.py
+-rw-r--r--   0        0        0     6129 2024-06-03 07:24:25.757691 lavague_core-0.2.3/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     2966 2024-06-03 07:24:25.757922 lavague_core-0.2.3/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1430 2024-05-31 09:04:25.702632 lavague_core-0.2.3/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0     3402 2024-05-31 09:04:25.702910 lavague_core-0.2.3/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0    15134 2024-05-31 09:09:25.856069 lavague_core-0.2.3/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1128 2024-06-03 07:24:25.758175 lavague_core-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 lavague_core-0.2.3/PKG-INFO
```

### Comparing `lavague_core-0.2.2/LICENSE` & `lavague_core-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/__init__.py` & `lavague_core-0.2.3/lavague/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from lavague.core.agents import WebAgent
 
 import os
 import warnings
 
 
 def telemetry_warning():
-    telemetry_var = os.getenv("TELEMETRY_VAR")
+    telemetry_var = os.getenv("LAVAGUE_TELEMETRY")
     if telemetry_var != "NONE":
-        warning_message = "\033[93mTelemetry is turned on. To turn off telemetry, set your TELEMETRY_VAR to 'NONE'\033[0m"
+        warning_message = "\033[93mTelemetry is turned on. To turn off telemetry, set your LAVAGUE_TELEMETRY to 'NONE'\033[0m"
         warnings.warn(warning_message, UserWarning)
 
 
 def exec_warning():
     warning_message = "\033[93mSecurity warning: This package executes LLM-generated code. Consider using this package in a sandboxed environment.\033[0m"
     warnings.warn(warning_message, UserWarning)
```

### Comparing `lavague_core-0.2.2/lavague/core/action_engine.py` & `lavague_core-0.2.3/lavague/core/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/agents.py` & `lavague_core-0.2.3/lavague/core/agents.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import shutil
 from typing import Dict
 from lavague.core.action_engine import ActionEngine
 from lavague.core.python_engine import PythonEngine
 from lavague.core.world_model import WorldModel
 from lavague.core.navigation import NavigationControl
@@ -11,33 +12,45 @@
 )
 from lavague.core.logger import AgentLogger
 from lavague.core.memory import ShortTermMemory
 from lavague.core.base_driver import BaseDriver
 
 from lavague.core.utilities.telemetry import send_telemetry
 
+logging_print = logging.getLogger(__name__)
+logging_print.setLevel(logging.INFO)
+format = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
+ch = logging.StreamHandler()
+ch.setLevel(logging.INFO)
+ch.setFormatter(format)
+logging_print.addHandler(ch)
+logging_print.propagate = False
+
 
 class WebAgent:
     """
     Web agent class, for now only works with selenium.
     """
 
     def __init__(
         self,
         world_model: WorldModel,
         action_engine: ActionEngine,
         n_steps: int = 10,
+        clean_screenshot_folder: bool = True,
     ):
         self.driver: BaseDriver = action_engine.driver
         self.action_engine: ActionEngine = action_engine
         self.world_model: WorldModel = world_model
         self.st_memory = ShortTermMemory()
 
         self.n_steps = n_steps
 
+        self.clean_screenshot_folder = clean_screenshot_folder
+
         self.logger: AgentLogger = AgentLogger()
 
         self.action_engine.set_logger_all(self.logger)
         self.world_model.set_logger(self.logger)
         self.st_memory.set_logger(self.logger)
 
     def get(self, url):
@@ -48,36 +61,38 @@
         logger = self.logger
         n_steps = self.n_steps
         self.action_engine.set_display(display)
 
         st_memory = self.st_memory
         world_model = self.world_model
 
-        try:
-            if os.path.isdir("screenshots"):
-                shutil.rmtree("screenshots")
-        except:
-            pass
+        if self.clean_screenshot_folder:
+            try:
+                if os.path.isdir("screenshots"):
+                    shutil.rmtree("screenshots")
+                logging_print.info("Screenshot folder cleared")
+            except:
+                pass
 
         obs = driver.get_obs()
 
         logger.new_run()
         for _ in range(n_steps):
             current_state, past = st_memory.get_state()
 
             world_model_output = world_model.get_instruction(
                 objective, current_state, past, obs
             )
-            print(world_model_output)
+            logging_print.info(world_model_output)
             next_engine_name = extract_next_engine(world_model_output)
             instruction = extract_world_model_instruction(world_model_output)
 
             if next_engine_name == "COMPLETE" or next_engine_name == "SUCCESS":
                 output = instruction
-                print("Objective reached. Stopping...")
+                logging_print.info("Objective reached. Stopping...")
 
                 logger.add_log(obs)
                 logger.end_step()
                 break
 
             success, output = self.action_engine.dispatch_instruction(
                 next_engine_name, instruction
```

### Comparing `lavague_core-0.2.2/lavague/core/base_driver.py` & `lavague_core-0.2.3/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/context.py` & `lavague_core-0.2.3/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/extractors.py` & `lavague_core-0.2.3/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/logger.py` & `lavague_core-0.2.3/lavague/core/logger.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/memory.py` & `lavague_core-0.2.3/lavague/core/memory.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/navigation.py` & `lavague_core-0.2.3/lavague/core/navigation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from io import BytesIO
+import logging
 import time
 from typing import Any, List, Optional, Tuple
+from string import Template
+import ast
 from lavague.core.action_template import ActionTemplate
 from lavague.core.context import Context, get_default_context
 from lavague.core.extractors import BaseExtractor, PythonFromMarkdownExtractor
 from lavague.core.retrievers import BaseHtmlRetriever, OpsmSplitRetriever
+from lavague.core.utilities.format_utils import extract_and_eval
 from lavague.core.utilities.web_utils import (
     display_screenshot,
     get_highlighted_element,
     sort_files_by_creation,
 )
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.common.keys import Keys
@@ -33,14 +37,23 @@
 Query: {query_str}
 Completion:
 
 """,
     PythonFromMarkdownExtractor(),
 )
 
+logging_print = logging.getLogger(__name__)
+logging_print.setLevel(logging.INFO)
+format = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
+ch = logging.StreamHandler()
+ch.setLevel(logging.INFO)
+ch.setFormatter(format)
+logging_print.addHandler(ch)
+logging_print.propagate = False
+
 
 class NavigationEngine(BaseEngine):
     """
     NavigationEngine leverages the llm model and the embedding model to output code from the prompt and the html page.
 
     Args:
         driver (`BaseDriver`):
@@ -70,18 +83,18 @@
         prompt_template: PromptTemplate = NAVIGATION_ENGINE_PROMPT_TEMPLATE.prompt_template,
         extractor: BaseExtractor = NAVIGATION_ENGINE_PROMPT_TEMPLATE.extractor,
         time_between_actions: float = 1.5,
         n_attempts: int = 5,
         logger: AgentLogger = None,
         display: bool = False,
     ):
-        if llm is None: 
-            llm: BaseLLM = get_default_context().llm,
+        if llm is None:
+            llm: BaseLLM = get_default_context().llm
         if embedding is None:
-            embedding: BaseEmbedding = get_default_context().embedding,
+            embedding: BaseEmbedding = get_default_context().embedding
         self.driver: BaseDriver = driver
         self.llm: BaseLLM = llm
         self.embedding: BaseEmbedding = embedding
         self.retriever: BaseHtmlRetriever = retriever
         self.prompt_template: PromptTemplate = prompt_template.partial_format(
             driver_capability=driver.get_capability()
         )
@@ -164,14 +177,49 @@
         response = self.llm.complete(prompt).text
         code = self.extractor.extract(response)
         return code
 
     def set_display(self, display: bool):
         self.display = display
 
+    def rephrase_query(self, query: str) -> List[dict]:
+        """
+        Rephrase the query
+        Args:
+            query (`str`): The query to rephrase
+        Return:
+            `List[dict]`: The rephrased query as a list of dictionaries
+        """
+        rephrase_prompt = Template("""
+        You are an AI system designed to convert text-based instructions for web actions into standardized instructions.
+        Here are previous examples:
+        Text instruction: Type 'Command R plus' on the search bar with placeholder "Search ..."
+        Standardized instruction: [{'query':'input"Search ..."', 'action':'Click on the input "Search ..." and type "Command R plus"'}]
+        Text instruction: Click on the search bar with placeholder "Rechercher sur Wikipédia", type "Yann LeCun," and press Enter.
+        Standardized instruction: [{'query':'input"Rechercher sur Wikipédia"', 'action':'Click on the input "Rechercher sur Wikipédia", type "Yann LeCun," and press Enter'}]
+        Text instruction: Click on 'Installation', next to 'Effective and efficient diffusion'
+        Standardized instruction: [{'query':'button"Installation"', 'action':'Click on "Installation"'}]
+        
+        Text instruction:  Locate the input element labeled "Email Address" and type in "example@example.com". Locate the input element labeled "First name" and type in "John". Locate the input element labeled "Last name" and type in "Doe". Locate the input element labeled "Phone" and type in "555-555-5555".
+        Standardized instruction: [{'query':'input"Email Address"', 'action':'Click on the input "Email Address" and type "example@example.com"'}, {'query':'input"First name"', 'action':'Click on the input "First name" and type "John"'}, {'query':'input"Last name"', 'action':'Click on the input "Last name" and type "Doe"'}, {'query':'input"Phone"', 'action':'Click on the input "Phone" and type "555-555-5555"'}]
+        Text instruction: In the login form, locate the input element labeled “Username” and type “user123”. Locate the input element labeled “Password” and type “pass456”.
+        Standardized instruction: [{'query':'input”Username”', 'action':'Click on the input “Username” and type “user123”'}, {'query':'input”Password”', 'action':'Click on the input “Password” and type “pass456”'}]
+        
+        Text instruction: Press the button labeled “Submit” at the bottom of the form.
+        Standardized instruction: [{'query':'button”Submit”', 'action':'Click on the button “Submit”'}]
+        
+        Text instruction: ${instruction}
+        Standardized instruction:
+        """)
+        rephrase_prompt = rephrase_prompt.safe_substitute(instruction=query)
+        response = self.llm.complete(rephrase_prompt).text
+        response = response.strip("```json\n").strip("\n``` \n")
+        rephrased_query = extract_and_eval(response)
+        return rephrased_query
+
     def get_action(self, query: str) -> Optional[str]:
         # TODO: Rename query to instruction to be consistent with other engines
         """
         Generate the code from a query
 
         Args:
             query (`str`): Instructions given at the end of the prompt to tell the model what to do on the html page
@@ -194,100 +242,111 @@
         Return:
             `bool`: True if the code was executed without error
             `Any`: The output of the code
         """
 
         # Navigation has no output
 
-
         output = None
         driver = self.driver.get_driver()
-
-        start = time.time()
-        source_nodes = self.get_nodes(instruction)
-        end = time.time()
-        retrieval_time = end - start
-
-        llm_context = "\n".join(source_nodes)
         success = False
-        logger = self.logger
-        
-        navigation_log = {
-            "navigation_engine_input": instruction,
-            "retrieved_html": source_nodes,
-            "retrieval_time": retrieval_time,
-            "retrieval_name": self.retriever.__class__.__name__,
-        }
-
-        action_outcomes = []
-        for _ in range(self.n_attempts):
-            if success:
-                break
-            if self.display:
-                try:
-                    scr_path = self.driver.get_current_screenshot_folder()
-                    lst = sort_files_by_creation(scr_path)
-                    for scr in lst:
-                        img = Image.open(scr_path.as_posix() + "/" + scr)
-                        display_screenshot(img)
-                        time.sleep(0.35)
-                except:
-                    pass
+
+        list_instructions = self.rephrase_query(instruction)
+        original_instruction = instruction
+        action_nb = 0
+        navigation_log_total = []
+
+        for action in list_instructions:
+            logging_print.debug("Rephrased instruction: " + action["action"])
+            instruction = action["action"]
             start = time.time()
-            prompt = self.prompt_template.format(
-                context_str=llm_context, query_str=instruction
-            )
-            response = self.llm.complete(prompt).text
-            action = self.extractor.extract(response)
+            source_nodes = self.get_nodes(instruction)
             end = time.time()
-            action_generation_time = end - start
-            action_outcome = {
-                "action": action,
-                "action_generation_time": action_generation_time,
-                "navigation_engine_full_prompt": prompt,
-                "navigation_engine_llm": get_model_name(self.llm),
+            retrieval_time = end - start
+
+            llm_context = "\n".join(source_nodes)
+            success = False
+            logger = self.logger
+
+            navigation_log = {
+                "original_instruction": original_instruction,
+                "navigation_engine_input": instruction,
+                "retrieved_html": source_nodes,
+                "retrieval_time": retrieval_time,
+                "retrieval_name": self.retriever.__class__.__name__,
             }
-            try:
-                local_scope = {"driver": driver}
-                code_to_execute = f"""
-{self.driver.import_lines}
-{action}"""
-                # Get information to see which elements are selected
-                vision_data = get_highlighted_element(driver, action)
-                if self.display:
-                    for item in vision_data:
-                        display_screenshot(item["screenshot"])
-                        time.sleep(0.2)
 
-                exec(code_to_execute, local_scope, local_scope)
-                time.sleep(self.time_between_actions)
+            action_outcomes = []
+            for _ in range(self.n_attempts):
+                if success:
+                    break
                 if self.display:
                     try:
-                        screenshot = self.driver.get_screenshot_as_png()
-                        screenshot = BytesIO(screenshot)
-                        screenshot = Image.open(screenshot)
-                        display_screenshot(screenshot)
+                        scr_path = self.driver.get_current_screenshot_folder()
+                        lst = sort_files_by_creation(scr_path)
+                        for scr in lst:
+                            img = Image.open(scr_path.as_posix() + "/" + scr)
+                            display_screenshot(img)
+                            time.sleep(0.35)
                     except:
                         pass
-                success = True
-                action_outcome["success"] = True
-                navigation_log["vision_data"] = vision_data
-            except Exception as e:
-                action_outcome["success"] = False
-                action_outcome["error"] = str(e)
-
-            action_outcomes.append(action_outcome)
-
-        navigation_log["action_outcomes"] = action_outcomes
-
+                start = time.time()
+                prompt = self.prompt_template.format(
+                    context_str=llm_context, query_str=instruction
+                )
+                response = self.llm.complete(prompt).text
+                action = self.extractor.extract(response)
+                end = time.time()
+                action_generation_time = end - start
+                action_outcome = {
+                    "action": action,
+                    "action_generation_time": action_generation_time,
+                    "navigation_engine_full_prompt": prompt,
+                    "navigation_engine_llm": get_model_name(self.llm),
+                }
+                try:
+                    local_scope = {"driver": driver}
+                    code_to_execute = f"""
+{self.driver.import_lines}
+{action}"""
+                    # Get information to see which elements are selected
+                    vision_data = get_highlighted_element(driver, action)
+                    if self.display:
+                        for item in vision_data:
+                            display_screenshot(item["screenshot"])
+                            time.sleep(0.2)
+
+                    exec(code_to_execute, local_scope, local_scope)
+                    time.sleep(self.time_between_actions)
+                    if self.display:
+                        try:
+                            screenshot = self.driver.get_screenshot_as_png()
+                            screenshot = BytesIO(screenshot)
+                            screenshot = Image.open(screenshot)
+                            display_screenshot(screenshot)
+                        except:
+                            pass
+                    success = True
+                    action_outcome["success"] = True
+                    navigation_log["vision_data"] = vision_data
+                except Exception as e:
+                    action_outcome["success"] = False
+                    action_outcome["error"] = str(e)
+
+                action_outcomes.append(action_outcome)
+
+            navigation_log["action_outcomes"] = action_outcomes
+            navigation_log["action_nb"] = action_nb
+            action_nb += 1
+            navigation_log_total.append(navigation_log)
         if logger:
             log = {
                 "engine": "Navigation Engine",
                 "instruction": instruction,
-                "engine_log": navigation_log,
+                "engine_log": navigation_log_total,
                 "success": success,
                 "output": None,
                 "code": action,
             }
 
             logger.add_log(log)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lavague_core-0.2.2/lavague/core/python_engine.py` & `lavague_core-0.2.3/lavague/core/python_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/retrievers.py` & `lavague_core-0.2.3/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/rewriter.py` & `lavague_core-0.2.3/lavague/core/rewriter.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/utilities/format_utils.py` & `lavague_core-0.2.3/lavague/core/utilities/format_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -110,14 +110,28 @@
     for pattern in next_engine_patterns:
         next_engine_match = re.search(pattern, text)
         if next_engine_match:
             return next_engine_match.group(1).strip()
     raise ValueError("No next engine found in the text.")
 
 
+def extract_and_eval(string):
+    # Regular expression to match a list inside a string
+    match = re.search(r"\[.*?\]", string, re.DOTALL)
+    if match:
+        list_string = match.group(0)
+        try:
+            result = ast.literal_eval(list_string)
+            return result
+        except (SyntaxError, ValueError):
+            return "Error: The extracted string is not a valid Python literal."
+    else:
+        return "Error: No list found in the string."
+
+
 def clean_html(
     html_to_clean: str,
     tags_to_remove: List[str] = ["style", "svg", "script"],
     attributes_to_keep: List[str] = ["id", "href"],
 ) -> str:
     """
     Clean HTML content by removing specified tags and attributes while keeping specified attributes.
```

### Comparing `lavague_core-0.2.2/lavague/core/utilities/version_checker.py` & `lavague_core-0.2.3/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/utilities/web_utils.py` & `lavague_core-0.2.3/lavague/core/utilities/web_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/lavague/core/world_model.py` & `lavague_core-0.2.3/lavague/core/world_model.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.2/pyproject.toml` & `lavague_core-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.2.2"
+version = "0.2.3"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_core-0.2.2/PKG-INFO` & `lavague_core-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

