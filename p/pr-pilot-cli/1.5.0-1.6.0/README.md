# Comparing `tmp/pr_pilot_cli-1.5.0.tar.gz` & `tmp/pr_pilot_cli-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.5.0.tar", last modified: Mon Jun  3 03:23:49 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.6.0.tar", last modified: Mon Jun  3 03:56:36 2024, max compression
```

## Comparing `pr_pilot_cli-1.5.0.tar` & `pr_pilot_cli-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:48.998897 pr_pilot_cli-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-03 03:23:48.998897 pr_pilot_cli-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:48.994897 pr_pilot_cli-1.5.0/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/detect_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/status_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/cli/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:23:48.994897 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 03:23:48.000000 pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 03:23:48.998897 pr_pilot_cli-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-03 03:23:44.000000 pr_pilot_cli-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:56:36.323601 pr_pilot_cli-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-06-03 03:56:36.323601 pr_pilot_cli-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:56:36.323601 pr_pilot_cli-1.6.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/cli/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/cli/status_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/cli/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:56:36.323601 pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-06-03 03:56:36.000000 pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-03 03:56:36.000000 pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:56:36.000000 pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 03:56:36.000000 pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-03 03:56:36.000000 pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-03 03:56:36.000000 pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 03:56:36.323601 pr_pilot_cli-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-03 03:56:28.000000 pr_pilot_cli-1.6.0/setup.py
```

### Comparing `pr_pilot_cli-1.5.0/LICENSE` & `pr_pilot_cli-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.5.0/PKG-INFO` & `pr_pilot_cli-1.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.5.0
+Version: 1.6.0
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,94 +31,88 @@
 PR Pilot gives you a natural language interface for your Github projects.
 Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
 and Github issues.
 
 Using [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create powerful,
 reusable commands that can be executed by PR Pilot.
 
-## Usage
+## 🛠️ Usage
 
 Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
-### Examples
+### 📋 Examples
 
 You can run a prompt directly on the command line:
 
 ```bash
-pilot -o README_German.md "translate the README into German"
+pilot "Tell me about this project!"
+```
+
+Ask PR Pilot to edit a file for you:
+
+```bash
+pilot --edit cli/cli.py "Make sure all functions and classes have docstrings."
 ```
 
 Generate code quickly:
 
 ```bash
 pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
-Get an organized view of your Github issues:
+Ask about something on your screen:
 
 ```bash
-pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
+pilot --snap "What is this code doing?"
 ```
 
-Get some advice on your code:
+Get an organized view of your Github issues:
 
 ```bash
-pilot "The 'TaskEngine' class is too complex. Read it and suggest refactoring options."
+pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
 Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
 pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
 For more examples, check out the [prompts](./prompts) directory in this repository.
 
-### Options and Parameters
+### ⚙️ Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
 Usage: python -m cli.cli [OPTIONS] [PROMPT]...
 
+  Main function to handle the CLI commands and options.
+
 Options:
   --wait / --no-wait        Wait for the result.
   --repo TEXT               Github repository in the format owner/repo.
+  --snap                    Adds a part of your screen as an image to the
+                            task.
+  -e, --edit PATH           Let PR Pilot edit a file for you.
   --spinner / --no-spinner  Display a loading indicator
   --quiet                   No pretty-print, no status indicator or messages.
   --cheap                   Use the cheapest GPT model (gpt-3.5-turbo)
   --code                    Optimize prompt and settings for generating code
   -f, --file PATH           Load prompt from a template file.
   --direct                  Do not feed the rendered template as a prompt into
                             PR Pilot, but render it directly as output.
   -o, --output PATH         Output file for the result.
-  --model TEXT              GPT model to use.
+  -m, --model TEXT          GPT model to use.
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
-## Installation
-
-Prerequisites:
-1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
-2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
-
-Install via pip:
-```
-pip install --upgrade pr-pilot-cli
-```
-
-Install via Homebrew:
-```
-brew tap PR-Pilot-AI/pr-pilot-homebrew
-brew install pr-pilot-cli
-```
-
-## Configuration
+## ⚙️ Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
-## Contributing
+## 🤝 Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
 
-## License
+## 📜 License
 The PR Pilot CLI is open-source software licensed under the GPL-3 license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,46 +1,44 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.5.0 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.6.0 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.5.2 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
-powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
-terminal and `ls` into a repository you have [installed](https://github.com/
-apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
-directly on the command line: ```bash pilot -o README_German.md "translate the
-README into German" ``` Generate code quickly: ```bash pilot -o test_utils.py -
--code "Write some unit tests for the utils.py file." ``` Get an organized view
-of your Github issues: ```bash pilot "Find all open Github issues labeled as
-'bug', categorize and prioritize them" ``` Get some advice on your code:
-```bash pilot "The 'TaskEngine' class is too complex. Read it and suggest
-refactoring options." ``` Generate parts of your README with a [template](./
+powerful, reusable commands that can be executed by PR Pilot. ## ð ï¸ Usage
+Open a terminal and `ls` into a repository you have [installed](https://
+github.com/apps/pr-pilot-ai/installations/new) PR Pilot. ### ð Examples You
+can run a prompt directly on the command line: ```bash pilot "Tell me about
+this project!" ``` Ask PR Pilot to edit a file for you: ```bash pilot --edit
+cli/cli.py "Make sure all functions and classes have docstrings." ``` Generate
+code quickly: ```bash pilot -o test_utils.py --code "Write some unit tests for
+the utils.py file." ``` Ask about something on your screen: ```bash pilot --
+snap "What is this code doing?" ``` Get an organized view of your Github
+issues: ```bash pilot "Find all open Github issues labeled as 'bug', categorize
+and prioritize them" ``` Generate parts of your README with a [template](./
 prompts/README.md.jinja2): ```bash pilot --direct -f prompts/README.md.jinja2 -
 o README.md ``` For more examples, check out the [prompts](./prompts) directory
-in this repository. ### Options and Parameters You can change the default
-settings with parameters and options: ```bash Usage: python -m cli.cli
-[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
-TEXT Github repository in the format owner/repo. --spinner / --no-spinner
-Display a loading indicator --quiet No pretty-print, no status indicator or
-messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
-prompt and settings for generating code -f, --file PATH Load prompt from a
-template file. --direct Do not feed the rendered template as a prompt into PR
-Pilot, but render it directly as output. -o, --output PATH Output file for the
-result. --model TEXT GPT model to use. --debug Display debug information. --
-help Show this message and exit. ``` ## Installation Prerequisites: 1. **
-[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/
-new)** on your Github repository 2. **[Generate an API key](https://app.pr-
-pilot.ai/dashboard/api-keys/)** in the dashboard Install via pip: ``` pip
-install --upgrade pr-pilot-cli ``` Install via Homebrew: ``` brew tap PR-Pilot-
-AI/pr-pilot-homebrew brew install pr-pilot-cli ``` ## Configuration The
-configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
-Contributors are welcome to improve the CLI by submitting pull requests or
-reporting issues. For more details, check the project's GitHub repository. ##
-License The PR Pilot CLI is open-source software licensed under the GPL-
-3 license.
+in this repository. ### âï¸ Options and Parameters You can change the
+default settings with parameters and options: ```bash Usage: python -m cli.cli
+[OPTIONS] [PROMPT]... Main function to handle the CLI commands and options.
+Options: --wait / --no-wait Wait for the result. --repo TEXT Github repository
+in the format owner/repo. --snap Adds a part of your screen as an image to the
+task. -e, --edit PATH Let PR Pilot edit a file for you. --spinner / --no-
+spinner Display a loading indicator --quiet No pretty-print, no status
+indicator or messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --
+code Optimize prompt and settings for generating code -f, --file PATH Load
+prompt from a template file. --direct Do not feed the rendered template as a
+prompt into PR Pilot, but render it directly as output. -o, --output PATH
+Output file for the result. -m, --model TEXT GPT model to use. --debug Display
+debug information. --help Show this message and exit. ``` ## âï¸
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ## ð¤
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## ð License The PR Pilot CLI is open-source software licensed
+under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.5.0/README.md` & `pr_pilot_cli-1.6.0/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: pr-pilot-cli
+Version: 1.6.0
+Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
+Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
+Author: Marco Lamina
+Author-email: marco@pr-pilot.ai
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click==8.1.7
+Requires-Dist: pr-pilot==1.5.2
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: yaspin==3.0.2
+Requires-Dist: rich==13.7.1
+Requires-Dist: jinja2==3.1.4
+
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> |
@@ -14,94 +31,88 @@
 PR Pilot gives you a natural language interface for your Github projects.
 Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
 and Github issues.
 
 Using [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create powerful,
 reusable commands that can be executed by PR Pilot.
 
-## Usage
+## 🛠️ Usage
 
 Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
-### Examples
+### 📋 Examples
 
 You can run a prompt directly on the command line:
 
 ```bash
-pilot -o README_German.md "translate the README into German"
+pilot "Tell me about this project!"
+```
+
+Ask PR Pilot to edit a file for you:
+
+```bash
+pilot --edit cli/cli.py "Make sure all functions and classes have docstrings."
 ```
 
 Generate code quickly:
 
 ```bash
 pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
-Get an organized view of your Github issues:
+Ask about something on your screen:
 
 ```bash
-pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
+pilot --snap "What is this code doing?"
 ```
 
-Get some advice on your code:
+Get an organized view of your Github issues:
 
 ```bash
-pilot "The 'TaskEngine' class is too complex. Read it and suggest refactoring options."
+pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
 Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
 pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
 For more examples, check out the [prompts](./prompts) directory in this repository.
 
-### Options and Parameters
+### ⚙️ Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
 Usage: python -m cli.cli [OPTIONS] [PROMPT]...
 
+  Main function to handle the CLI commands and options.
+
 Options:
   --wait / --no-wait        Wait for the result.
   --repo TEXT               Github repository in the format owner/repo.
+  --snap                    Adds a part of your screen as an image to the
+                            task.
+  -e, --edit PATH           Let PR Pilot edit a file for you.
   --spinner / --no-spinner  Display a loading indicator
   --quiet                   No pretty-print, no status indicator or messages.
   --cheap                   Use the cheapest GPT model (gpt-3.5-turbo)
   --code                    Optimize prompt and settings for generating code
   -f, --file PATH           Load prompt from a template file.
   --direct                  Do not feed the rendered template as a prompt into
                             PR Pilot, but render it directly as output.
   -o, --output PATH         Output file for the result.
-  --model TEXT              GPT model to use.
+  -m, --model TEXT          GPT model to use.
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
-## Installation
-
-Prerequisites:
-1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
-2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
-
-Install via pip:
-```
-pip install --upgrade pr-pilot-cli
-```
-
-Install via Homebrew:
-```
-brew tap PR-Pilot-AI/pr-pilot-homebrew
-brew install pr-pilot-cli
-```
-
-## Configuration
+## ⚙️ Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
-## Contributing
+## 🤝 Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
 
-## License
-The PR Pilot CLI is open-source software licensed under the GPL-3 license.
+## 📜 License
+The PR Pilot CLI is open-source software licensed under the GPL-3 license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,39 +1,44 @@
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.6.0 Summary: CLI for PR
+Pilot, a text-to-task automation platform for Github. Home-page: https://
+github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
+marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
+pilot==1.5.2 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
+Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
-powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
-terminal and `ls` into a repository you have [installed](https://github.com/
-apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
-directly on the command line: ```bash pilot -o README_German.md "translate the
-README into German" ``` Generate code quickly: ```bash pilot -o test_utils.py -
--code "Write some unit tests for the utils.py file." ``` Get an organized view
-of your Github issues: ```bash pilot "Find all open Github issues labeled as
-'bug', categorize and prioritize them" ``` Get some advice on your code:
-```bash pilot "The 'TaskEngine' class is too complex. Read it and suggest
-refactoring options." ``` Generate parts of your README with a [template](./
+powerful, reusable commands that can be executed by PR Pilot. ## ð ï¸ Usage
+Open a terminal and `ls` into a repository you have [installed](https://
+github.com/apps/pr-pilot-ai/installations/new) PR Pilot. ### ð Examples You
+can run a prompt directly on the command line: ```bash pilot "Tell me about
+this project!" ``` Ask PR Pilot to edit a file for you: ```bash pilot --edit
+cli/cli.py "Make sure all functions and classes have docstrings." ``` Generate
+code quickly: ```bash pilot -o test_utils.py --code "Write some unit tests for
+the utils.py file." ``` Ask about something on your screen: ```bash pilot --
+snap "What is this code doing?" ``` Get an organized view of your Github
+issues: ```bash pilot "Find all open Github issues labeled as 'bug', categorize
+and prioritize them" ``` Generate parts of your README with a [template](./
 prompts/README.md.jinja2): ```bash pilot --direct -f prompts/README.md.jinja2 -
 o README.md ``` For more examples, check out the [prompts](./prompts) directory
-in this repository. ### Options and Parameters You can change the default
-settings with parameters and options: ```bash Usage: python -m cli.cli
-[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
-TEXT Github repository in the format owner/repo. --spinner / --no-spinner
-Display a loading indicator --quiet No pretty-print, no status indicator or
-messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
-prompt and settings for generating code -f, --file PATH Load prompt from a
-template file. --direct Do not feed the rendered template as a prompt into PR
-Pilot, but render it directly as output. -o, --output PATH Output file for the
-result. --model TEXT GPT model to use. --debug Display debug information. --
-help Show this message and exit. ``` ## Installation Prerequisites: 1. **
-[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/
-new)** on your Github repository 2. **[Generate an API key](https://app.pr-
-pilot.ai/dashboard/api-keys/)** in the dashboard Install via pip: ``` pip
-install --upgrade pr-pilot-cli ``` Install via Homebrew: ``` brew tap PR-Pilot-
-AI/pr-pilot-homebrew brew install pr-pilot-cli ``` ## Configuration The
-configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
-Contributors are welcome to improve the CLI by submitting pull requests or
-reporting issues. For more details, check the project's GitHub repository. ##
-License The PR Pilot CLI is open-source software licensed under the GPL-
-3 license.
+in this repository. ### âï¸ Options and Parameters You can change the
+default settings with parameters and options: ```bash Usage: python -m cli.cli
+[OPTIONS] [PROMPT]... Main function to handle the CLI commands and options.
+Options: --wait / --no-wait Wait for the result. --repo TEXT Github repository
+in the format owner/repo. --snap Adds a part of your screen as an image to the
+task. -e, --edit PATH Let PR Pilot edit a file for you. --spinner / --no-
+spinner Display a loading indicator --quiet No pretty-print, no status
+indicator or messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --
+code Optimize prompt and settings for generating code -f, --file PATH Load
+prompt from a template file. --direct Do not feed the rendered template as a
+prompt into PR Pilot, but render it directly as output. -o, --output PATH
+Output file for the result. -m, --model TEXT GPT model to use. --debug Display
+debug information. --help Show this message and exit. ``` ## âï¸
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ## ð¤
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## ð License The PR Pilot CLI is open-source software licensed
+under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.5.0/cli/cli.py` & `pr_pilot_cli-1.6.0/cli/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from cli.task_handler import TaskHandler
 
 CONFIG_LOCATION = os.path.expanduser('~/.pr-pilot.yaml')
 CONFIG_API_KEY = "api_key"
 CODE_MODEL = "gpt-4o"
 CHEAP_MODEL = "gpt-3.5-turbo"
 POLL_INTERVAL = 2
+CODE_PRIMER = "Do not write anything to file, but ONLY respond with the code/content, no other text. Do not wrap it in triple backticks."
+DEFAULT_MODEL = "gpt-4o"
 
 
 def load_config():
     """Load the configuration from the default location. If it doesn't exist,
     ask user to enter API key and save config."""
     if not os.path.exists(CONFIG_LOCATION):
         if os.getenv("PR_PILOT_API_KEY"):
@@ -43,27 +45,29 @@
     os.system(screenshot_command)
     return Path("/tmp/screenshot.png")
 
 
 @click.command()
 @click.option('--wait/--no-wait', is_flag=True, default=True, help='Wait for the result.')
 @click.option('--repo', help='Github repository in the format owner/repo.', required=False)
-@click.option('--snap', is_flag=True, help='Adds a screenshot of a portion of your screen to the task.')
+@click.option('--snap', is_flag=True, help='Adds a part of your screen as an image to the task.')
+@click.option('--edit', '-e', type=click.Path(exists=True), help='Let PR Pilot edit a file for you.')
 @click.option('--spinner/--no-spinner', is_flag=True, default=True, help='Display a loading indicator')
 @click.option('--quiet', is_flag=True, default=False, help='No pretty-print, no status indicator or messages.')
 @click.option('--cheap', is_flag=True, default=False, help=f'Use the cheapest GPT model ({CHEAP_MODEL})')
 @click.option('--code', is_flag=True, default=False, help='Optimize prompt and settings for generating code')
 @click.option('--file', '-f', type=click.Path(exists=True), help='Load prompt from a template file.')
 @click.option('--direct', is_flag=True, default=False,
               help='Do not feed the rendered template as a prompt into PR Pilot, but render it directly as output.')
 @click.option('--output', '-o', type=click.Path(exists=False), help='Output file for the result.')
-@click.option('--model', help='GPT model to use.', default='gpt-4-turbo')
+@click.option('--model', '-m', help='GPT model to use.', default=DEFAULT_MODEL)
 @click.option('--debug', is_flag=True, default=False, help='Display debug information.')
 @click.argument('prompt', nargs=-1)
-def main(wait, repo, snap, spinner, quiet, cheap, code, file, direct, output, model, debug, prompt):
+def main(wait, repo, snap, edit, spinner, quiet, cheap, code, file, direct, output, model, debug, prompt):
+    """Main function to handle the CLI commands and options."""
     prompt = ' '.join(prompt)
     config = load_config()
     console = Console()
     show_spinner = spinner and not quiet
     status = StatusIndicator(spinner=show_spinner, messages=not quiet, console=console)
     screenshot = take_screenshot() if snap else None
 
@@ -83,28 +87,40 @@
         renderer = PromptTemplate(file, repo, model, status)
         prompt = renderer.render()
     if not prompt:
         prompt = click.edit("", extension=".md")
         if not prompt:
             console.print("No prompt provided.")
             return
+
+    if edit:
+        file_content = Path(edit).read_text()
+        user_prompt = prompt
+        prompt = f"I have the following file content:\n\n---\n{file_content}\n---\n\n"
+        prompt += f"Please edit the file content above in the following way:\n\n{user_prompt}\n\n{CODE_PRIMER}"
+        if not output:
+            output = edit
+
     if cheap:
         model = CHEAP_MODEL
     if code:
-        prompt += "\n\nONLY respond with the code, no other text. Do not wrap it in triple backticks."
+        prompt += "\n\n" + CODE_PRIMER
         if not model:
             model = CODE_MODEL
 
     if direct:
         # Do not send the prompt, just return it as the result
         if output:
             with open(output, "w") as f:
                 f.write(prompt)
+            status.stop()
             if not quiet:
+                console.line()
                 console.print(Markdown(f"Rendered template `{file}` into `{output}`"))
+                console.line()
             return
     status.start()
     status.update("Creating new task")
     task = create_task(repo, prompt, log=False, gpt_model=model, image=screenshot)
     status.update(f"Task created: https://app.pr-pilot.ai/dashboard/tasks/{task.id}")
     status.success()
     if debug:
```

### Comparing `pr_pilot_cli-1.5.0/cli/detect_repository.py` & `pr_pilot_cli-1.6.0/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.5.0/cli/prompt_template.py` & `pr_pilot_cli-1.6.0/cli/prompt_template.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.5.0/cli/status_indicator.py` & `pr_pilot_cli-1.6.0/cli/status_indicator.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.5.0/cli/task_handler.py` & `pr_pilot_cli-1.6.0/cli/task_handler.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.5.0/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pr-pilot-cli
-Version: 1.5.0
-Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
-Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
-Author: Marco Lamina
-Author-email: marco@pr-pilot.ai
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click==8.1.7
-Requires-Dist: pr-pilot==1.5.2
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: yaspin==3.0.2
-Requires-Dist: rich==13.7.1
-Requires-Dist: jinja2==3.1.4
-
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> |
@@ -31,94 +14,88 @@
 PR Pilot gives you a natural language interface for your Github projects.
 Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
 and Github issues.
 
 Using [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create powerful,
 reusable commands that can be executed by PR Pilot.
 
-## Usage
+## 🛠️ Usage
 
 Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
-### Examples
+### 📋 Examples
 
 You can run a prompt directly on the command line:
 
 ```bash
-pilot -o README_German.md "translate the README into German"
+pilot "Tell me about this project!"
+```
+
+Ask PR Pilot to edit a file for you:
+
+```bash
+pilot --edit cli/cli.py "Make sure all functions and classes have docstrings."
 ```
 
 Generate code quickly:
 
 ```bash
 pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
-Get an organized view of your Github issues:
+Ask about something on your screen:
 
 ```bash
-pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
+pilot --snap "What is this code doing?"
 ```
 
-Get some advice on your code:
+Get an organized view of your Github issues:
 
 ```bash
-pilot "The 'TaskEngine' class is too complex. Read it and suggest refactoring options."
+pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
 Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
 pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
 For more examples, check out the [prompts](./prompts) directory in this repository.
 
-### Options and Parameters
+### ⚙️ Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
 Usage: python -m cli.cli [OPTIONS] [PROMPT]...
 
+  Main function to handle the CLI commands and options.
+
 Options:
   --wait / --no-wait        Wait for the result.
   --repo TEXT               Github repository in the format owner/repo.
+  --snap                    Adds a part of your screen as an image to the
+                            task.
+  -e, --edit PATH           Let PR Pilot edit a file for you.
   --spinner / --no-spinner  Display a loading indicator
   --quiet                   No pretty-print, no status indicator or messages.
   --cheap                   Use the cheapest GPT model (gpt-3.5-turbo)
   --code                    Optimize prompt and settings for generating code
   -f, --file PATH           Load prompt from a template file.
   --direct                  Do not feed the rendered template as a prompt into
                             PR Pilot, but render it directly as output.
   -o, --output PATH         Output file for the result.
-  --model TEXT              GPT model to use.
+  -m, --model TEXT          GPT model to use.
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
-## Installation
-
-Prerequisites:
-1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
-2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
-
-Install via pip:
-```
-pip install --upgrade pr-pilot-cli
-```
-
-Install via Homebrew:
-```
-brew tap PR-Pilot-AI/pr-pilot-homebrew
-brew install pr-pilot-cli
-```
-
-## Configuration
+## ⚙️ Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
-## Contributing
+## 🤝 Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
 
-## License
-The PR Pilot CLI is open-source software licensed under the GPL-3 license.
+## 📜 License
+The PR Pilot CLI is open-source software licensed under the GPL-3 license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,46 +1,37 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.5.0 Summary: CLI for PR
-Pilot, a text-to-task automation platform for Github. Home-page: https://
-github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
-marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
-pilot==1.5.2 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
-Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
-powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
-terminal and `ls` into a repository you have [installed](https://github.com/
-apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
-directly on the command line: ```bash pilot -o README_German.md "translate the
-README into German" ``` Generate code quickly: ```bash pilot -o test_utils.py -
--code "Write some unit tests for the utils.py file." ``` Get an organized view
-of your Github issues: ```bash pilot "Find all open Github issues labeled as
-'bug', categorize and prioritize them" ``` Get some advice on your code:
-```bash pilot "The 'TaskEngine' class is too complex. Read it and suggest
-refactoring options." ``` Generate parts of your README with a [template](./
+powerful, reusable commands that can be executed by PR Pilot. ## ð ï¸ Usage
+Open a terminal and `ls` into a repository you have [installed](https://
+github.com/apps/pr-pilot-ai/installations/new) PR Pilot. ### ð Examples You
+can run a prompt directly on the command line: ```bash pilot "Tell me about
+this project!" ``` Ask PR Pilot to edit a file for you: ```bash pilot --edit
+cli/cli.py "Make sure all functions and classes have docstrings." ``` Generate
+code quickly: ```bash pilot -o test_utils.py --code "Write some unit tests for
+the utils.py file." ``` Ask about something on your screen: ```bash pilot --
+snap "What is this code doing?" ``` Get an organized view of your Github
+issues: ```bash pilot "Find all open Github issues labeled as 'bug', categorize
+and prioritize them" ``` Generate parts of your README with a [template](./
 prompts/README.md.jinja2): ```bash pilot --direct -f prompts/README.md.jinja2 -
 o README.md ``` For more examples, check out the [prompts](./prompts) directory
-in this repository. ### Options and Parameters You can change the default
-settings with parameters and options: ```bash Usage: python -m cli.cli
-[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
-TEXT Github repository in the format owner/repo. --spinner / --no-spinner
-Display a loading indicator --quiet No pretty-print, no status indicator or
-messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
-prompt and settings for generating code -f, --file PATH Load prompt from a
-template file. --direct Do not feed the rendered template as a prompt into PR
-Pilot, but render it directly as output. -o, --output PATH Output file for the
-result. --model TEXT GPT model to use. --debug Display debug information. --
-help Show this message and exit. ``` ## Installation Prerequisites: 1. **
-[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/
-new)** on your Github repository 2. **[Generate an API key](https://app.pr-
-pilot.ai/dashboard/api-keys/)** in the dashboard Install via pip: ``` pip
-install --upgrade pr-pilot-cli ``` Install via Homebrew: ``` brew tap PR-Pilot-
-AI/pr-pilot-homebrew brew install pr-pilot-cli ``` ## Configuration The
-configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
-Contributors are welcome to improve the CLI by submitting pull requests or
-reporting issues. For more details, check the project's GitHub repository. ##
-License The PR Pilot CLI is open-source software licensed under the GPL-
-3 license.
+in this repository. ### âï¸ Options and Parameters You can change the
+default settings with parameters and options: ```bash Usage: python -m cli.cli
+[OPTIONS] [PROMPT]... Main function to handle the CLI commands and options.
+Options: --wait / --no-wait Wait for the result. --repo TEXT Github repository
+in the format owner/repo. --snap Adds a part of your screen as an image to the
+task. -e, --edit PATH Let PR Pilot edit a file for you. --spinner / --no-
+spinner Display a loading indicator --quiet No pretty-print, no status
+indicator or messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --
+code Optimize prompt and settings for generating code -f, --file PATH Load
+prompt from a template file. --direct Do not feed the rendered template as a
+prompt into PR Pilot, but render it directly as output. -o, --output PATH
+Output file for the result. -m, --model TEXT GPT model to use. --debug Display
+debug information. --help Show this message and exit. ``` ## âï¸
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ## ð¤
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## ð License The PR Pilot CLI is open-source software licensed
+under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.5.0/setup.py` & `pr_pilot_cli-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.5.0',
+    version='1.6.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

