# Comparing `tmp/pr_pilot_cli-1.4.2.tar.gz` & `tmp/pr_pilot_cli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.4.2.tar", last modified: Sat Jun  1 05:01:05 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.5.0.tar", last modified: Mon Jun  3 03:23:49 2024, max compression
```

## Comparing `pr_pilot_cli-1.4.2.tar` & `pr_pilot_cli-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/detect_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/status_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:48.998897 pr_pilot_cli-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-03 03:23:48.998897 pr_pilot_cli-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:48.994897 pr_pilot_cli-1.5.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/status_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:48.994897 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 03:23:48.998897 pr_pilot_cli-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/setup.py
```

### Comparing `pr_pilot_cli-1.4.2/LICENSE` & `pr_pilot_cli-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.2/PKG-INFO` & `pr_pilot_cli-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.4.2
+Version: 1.5.0
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
-Requires-Dist: pr-pilot==1.4.1
+Requires-Dist: pr-pilot==1.5.2
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
 Requires-Dist: jinja2==3.1.4
 
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.2 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.5.0 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
-pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
+pilot==1.5.2 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
```

### Comparing `pr_pilot_cli-1.4.2/README.md` & `pr_pilot_cli-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.2/cli/cli.py` & `pr_pilot_cli-1.5.0/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 
 import click
 import yaml
 from pr_pilot.util import create_task
 from rich.console import Console
 from rich.markdown import Markdown
 
@@ -32,35 +33,43 @@
         with open(CONFIG_LOCATION, "w") as f:
             f.write(f"{CONFIG_API_KEY}: {api_key}")
         click.echo(f"Configuration saved in {CONFIG_LOCATION}")
     with open(CONFIG_LOCATION) as f:
         config = yaml.safe_load(f)
     return config
 
+def take_screenshot():
+    """Take a screenshot of a portion of the screen."""
+    screenshot_command = "screencapture -i /tmp/screenshot.png"
+    os.system(screenshot_command)
+    return Path("/tmp/screenshot.png")
+
 
 @click.command()
 @click.option('--wait/--no-wait', is_flag=True, default=True, help='Wait for the result.')
 @click.option('--repo', help='Github repository in the format owner/repo.', required=False)
+@click.option('--snap', is_flag=True, help='Adds a screenshot of a portion of your screen to the task.')
 @click.option('--spinner/--no-spinner', is_flag=True, default=True, help='Display a loading indicator')
 @click.option('--quiet', is_flag=True, default=False, help='No pretty-print, no status indicator or messages.')
 @click.option('--cheap', is_flag=True, default=False, help=f'Use the cheapest GPT model ({CHEAP_MODEL})')
 @click.option('--code', is_flag=True, default=False, help='Optimize prompt and settings for generating code')
 @click.option('--file', '-f', type=click.Path(exists=True), help='Load prompt from a template file.')
 @click.option('--direct', is_flag=True, default=False,
               help='Do not feed the rendered template as a prompt into PR Pilot, but render it directly as output.')
 @click.option('--output', '-o', type=click.Path(exists=False), help='Output file for the result.')
 @click.option('--model', help='GPT model to use.', default='gpt-4-turbo')
 @click.option('--debug', is_flag=True, default=False, help='Display debug information.')
 @click.argument('prompt', nargs=-1)
-def main(wait, repo, spinner, quiet, cheap, code, file, direct, output, model, debug, prompt):
+def main(wait, repo, snap, spinner, quiet, cheap, code, file, direct, output, model, debug, prompt):
     prompt = ' '.join(prompt)
     config = load_config()
     console = Console()
     show_spinner = spinner and not quiet
     status = StatusIndicator(spinner=show_spinner, messages=not quiet, console=console)
+    screenshot = take_screenshot() if snap else None
 
     if not os.getenv("PR_PILOT_API_KEY"):
         os.environ["PR_PILOT_API_KEY"] = config[CONFIG_API_KEY]
     if not repo:
         # No repository provided, try to detect it
         repo = detect_repository()
     if not repo:
@@ -91,15 +100,15 @@
             with open(output, "w") as f:
                 f.write(prompt)
             if not quiet:
                 console.print(Markdown(f"Rendered template `{file}` into `{output}`"))
             return
     status.start()
     status.update("Creating new task")
-    task = create_task(repo, prompt, log=False, gpt_model=model)
+    task = create_task(repo, prompt, log=False, gpt_model=model, image=screenshot)
     status.update(f"Task created: https://app.pr-pilot.ai/dashboard/tasks/{task.id}")
     status.success()
     if debug:
         console.print(task)
     if wait:
         task_handler = TaskHandler(task, status)
         task_handler.wait_for_result(output, quiet)
```

### Comparing `pr_pilot_cli-1.4.2/cli/detect_repository.py` & `pr_pilot_cli-1.5.0/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.2/cli/prompt_template.py` & `pr_pilot_cli-1.5.0/cli/prompt_template.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.2/cli/status_indicator.py` & `pr_pilot_cli-1.5.0/cli/status_indicator.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.2/cli/task_handler.py` & `pr_pilot_cli-1.5.0/cli/task_handler.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.4.2
+Version: 1.5.0
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
-Requires-Dist: pr-pilot==1.4.1
+Requires-Dist: pr-pilot==1.5.2
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
 Requires-Dist: jinja2==3.1.4
 
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.2 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.5.0 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
-pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
+pilot==1.5.2 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
```

### Comparing `pr_pilot_cli-1.4.2/setup.py` & `pr_pilot_cli-1.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.4.2',
+    version='1.5.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

