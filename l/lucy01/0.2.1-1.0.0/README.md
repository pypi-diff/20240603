# Comparing `tmp/lucy01-0.2.1.tar.gz` & `tmp/lucy01-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucy01-0.2.1.tar", last modified: Fri May 17 12:43:28 2024, max compression
+gzip compressed data, was "lucy01-1.0.0.tar", last modified: Mon Jun  3 08:01:50 2024, max compression
```

## Comparing `lucy01-0.2.1.tar` & `lucy01-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.260474 lucy01-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-17 12:43:28.260474 lucy01-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-17 12:43:22.000000 lucy01-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.256474 lucy01-0.2.1/lucy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/dbx_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.260474 lucy01-0.2.1/lucy/parser_/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/parser_/atcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/parser_/contest.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/parser_/parser_.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/update_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.260474 lucy01-0.2.1/lucy01.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-17 12:43:22.000000 lucy01-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:43:28.260474 lucy01-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:01:50.859894 lucy01-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-06-03 08:01:50.859894 lucy01-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-06-03 08:01:47.000000 lucy01-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:01:50.855894 lucy01-1.0.0/lucy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/contest_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:01:50.855894 lucy01-1.0.0/lucy/parser_/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/parser_/atcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/parser_/contest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/parser_/parser_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/update_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-03 08:01:47.000000 lucy01-1.0.0/lucy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:01:50.859894 lucy01-1.0.0/lucy01.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-06-03 08:01:50.000000 lucy01-1.0.0/lucy01.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-06-03 08:01:50.000000 lucy01-1.0.0/lucy01.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:01:50.000000 lucy01-1.0.0/lucy01.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-03 08:01:50.000000 lucy01-1.0.0/lucy01.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-03 08:01:50.000000 lucy01-1.0.0/lucy01.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 08:01:50.000000 lucy01-1.0.0/lucy01.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-06-03 08:01:47.000000 lucy01-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:01:50.859894 lucy01-1.0.0/setup.cfg
```

### Comparing `lucy01-0.2.1/PKG-INFO` & `lucy01-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucy01
-Version: 0.2.1
+Version: 1.0.0
 Summary: CLI companion for CP.
 Author-email: Mehul Todi <mehul116.dev@gmail.com>
 Project-URL: Documentation, https://lucy01.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/kid-116/Lucy
 Project-URL: Issues, https://github.com/kid-116/Lucy/issues
 Keywords: cp,cli,companion,atcoder,codeforces,tester,snippets,lucy
 Classifier: Development Status :: 4 - Beta
@@ -12,45 +12,52 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: click
-Requires-Dist: dropbox
 Requires-Dist: lxml
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: selenium
 Provides-Extra: lint
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: pylint[spelling]; extra == "lint"
 Requires-Dist: yapf; extra == "lint"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-datadir; extra == "test"
+
+[![Lint](https://github.com/kid-116/Lucy/actions/workflows/pylint.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/pylint.yml)
+[![Test](https://github.com/kid-116/Lucy/actions/workflows/pytest.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/pytest.yml)
+[![Publish PyPI](https://github.com/kid-116/Lucy/actions/workflows/publish.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/publish.yml)
+[![GitHub Release](https://github.com/kid-116/Lucy/actions/workflows/gh-release.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/gh-release.yml)
 
 # Lucy
 
 Lucy, a CLI companion for competitive programming on AtCoder and Codeforces, frees you from tedious
 tasks. It automatically fetches sample tests, sets up directories, and lets you test your code with
 just a few commands, streamlining your workflow and letting you focus on writing brilliant
 solutions.
 
 [Demo](https://github.com/kid-116/Lucy/assets/75692643/1b7195f7-fcd3-4e05-b23e-48061f6ef1b1)
 
-## Support Languages
+## Supported Languages
 - [x] C++
 - [ ] Python
 
 ## Supported Platforms
 - [x] AtCoder
 - [ ] Codeforces
 
 ## Featues
 - [x] Fetch Sample Test Cases
-- [x] Fetch Hidden Test Cases (after the contest 🤪)
+- [ ] Fetch Hidden Test Cases (after the contest 🤪)
 - [x] Test Solution
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
 ```
@@ -58,22 +65,14 @@
 ```
 
 ## Environment Variables
 - `LUCY_HOME`
 
     Specify home directory for `lucy`.
 
-- `DROPBOX_TOKEN`
-
-
-    Dropbox developer access token with `sharing.read` permission. It can be generated at
-    [DBX Platform for Developers](https://www.dropbox.com/developers). This is necessary to fetch
-    hidden AtCoder test cases releaved after the contest has ended. All AtCoder test cases may be
-    found [here](https://www.dropbox.com/sh/nx3tnilzqz7df8a/AAAYlTq2tiEHl5hsESw6-yfLa?dl=0).
-
 ## Getting Started
 1. Set the environment variable `$LUCY_HOME` as preferred. By default, it uses the `~/.lucy`.
 2. Get help!
     ```
     lucy --help
     ```
     Check out the [documentation](https://lucy01.readthedocs.io/en/latest/).
```

### Comparing `lucy01-0.2.1/lucy/filesystem.py` & `lucy01-1.0.0/lucy/filesystem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,48 @@
+import hashlib
 import os
+from pathlib import Path
 import shutil
 from typing import Generator, Optional, Tuple
 
-import click
-
-from lucy.config import Config, SampleType, Website
+from lucy.config import config, SampleType, Website
 from lucy.parser_.parser_ import Task
 
 
 class LocalFS:
 
     @staticmethod
+    def get_contest_root_dir(website: Website, contest_id: str) -> Path:
+        return config.home / str(website) / contest_id
+
+    @staticmethod
     def get_impl_path(website: Website,
                       contest_id: str,
                       task_id: str,
                       dir_: bool = False,
-                      bin_: bool = False) -> str:
-        impl_path = f'{Config.LUCY_HOME}/{website}/{contest_id.upper()}/{task_id.upper()}'
+                      bin_: bool = False) -> Path:
+        impl_path = LocalFS.get_contest_root_dir(website, contest_id) / task_id
         if bin_:
-            return f'{impl_path}/{Config.IMPL_BIN}'
+            return impl_path / config.impl.bin_name
         if not dir_:
-            impl_path = f'{impl_path}/{Config.IMPL_MAIN}'
+            impl_path = impl_path / config.impl.src_name
         return impl_path
 
     @staticmethod
     def get_sample_path(website: Website,
                         contest_id: str,
                         task_id: str,
                         type_: Optional[SampleType] = None,
-                        idx: Optional[int] = None) -> str:
-        sample_path = LocalFS.get_impl_path(website, contest_id, task_id, dir_=True)
-        sample_path += f'/{Config.SAMPLES_DIR}'
+                        idx: Optional[int] = None) -> Path:
+        sample_path = LocalFS.get_impl_path(website, contest_id, task_id,
+                                            dir_=True) / config.samples_dir_name
         if type_:
-            sample_path += f'/{type_}'
+            sample_path = sample_path / str(type_)
             if idx is not None:
-                sample_path += f'/{idx:02d}.txt'
+                sample_path = sample_path / f'{idx:02d}.txt'
         return sample_path
 
     @staticmethod
     def delete_samples(website: Website, contest_id: str, task_id: str) -> bool:
         samples_dir = LocalFS.get_sample_path(website, contest_id, task_id)
         if os.path.exists(samples_dir):
             shutil.rmtree(samples_dir)
@@ -47,15 +51,15 @@
 
     @staticmethod
     def num_samples(website: Website, contest_id: str, task_id: str) -> int:
         return len(os.listdir(LocalFS.get_sample_path(website, contest_id, task_id, SampleType.IN)))
 
     @staticmethod
     def get_new_sample_paths(website: Website, contest_id: str,
-                             task_id: str) -> Tuple[str, str, int]:
+                             task_id: str) -> Tuple[Path, Path, int]:
         idx = LocalFS.num_samples(website, contest_id, task_id)
         in_path = LocalFS.get_sample_path(website, contest_id, task_id, SampleType.IN, idx)
         out_path = LocalFS.get_sample_path(website, contest_id, task_id, SampleType.OUT, idx)
         return in_path, out_path, idx
 
     @staticmethod
     def store_sample(website: Website, contest_id: str, task_id: str, sample: Tuple[str,
@@ -79,39 +83,45 @@
                     exist_ok=True)
         for sample in task.samples:
             LocalFS.store_sample(website, contest_id, task.id_, sample)
         return len(task.samples)
 
     @staticmethod
     def setup() -> None:
-        if not os.path.exists(Config.LUCY_HOME):
-            click.echo(f'Creating LUCY_HOME ({Config.LUCY_HOME}).')
-            os.makedirs(Config.LUCY_HOME, exist_ok=True)
-
-        if not os.path.exists(Config.SNIPPETS_DIR):
-            click.echo(f'Creating SNIPPETS_DIR ({Config.SNIPPETS_DIR}).')
-            os.makedirs(Config.SNIPPETS_DIR, exist_ok=True)
-
-        if not os.path.exists(Config.COMMONS_DIR):
-            click.echo(f'Creating COMMONS_DIR ({Config.COMMONS_DIR}).')
-            os.makedirs(Config.COMMONS_DIR, exist_ok=True)
-
-        if not os.path.exists(Config.TEMPLATE_PATH):
-            with open(Config.TEMPLATE_PATH, 'w+', encoding='utf-8'):
-                pass
+        dir_checks: list[Path] = [
+            config.home,
+            config.snippets.dir_,
+            config.commons.dir_,
+            config.storage_path,
+        ]
+
+        for dir_ in dir_checks:
+            if not dir_.exists():
+                os.makedirs(dir_)
+
+        if not os.path.exists(config.commons.template_path):
+            with open(config.commons.template_path, 'w+', encoding='utf-8') as template:
+                template.write("""#include <iostream>
+
+using namespace std;
+
+int main() {
+    return 0;
+}
+""")
 
     @staticmethod
-    def create_impl_file(website: Website, contest_id: str, task_id: str) -> str:
+    def create_impl_file(website: Website, contest_id: str, task_id: str) -> Path:
         impl_path = LocalFS.get_impl_path(website, contest_id, task_id)
         if not os.path.exists(impl_path):
-            shutil.copy(Config.TEMPLATE_PATH, impl_path)
+            shutil.copy(config.commons.template_path, impl_path)
         return impl_path
 
     @staticmethod
-    def read(path: str) -> str:
+    def read(path: Path) -> str:
         with open(path) as f:  # pylint: disable=unspecified-encoding
             return f.read()
 
     @staticmethod
     def tests(website: Website, contest_id: str, task_id: str,
               test_ids: list[int]) -> Generator[Tuple[str, str], None, None]:
         for idx in test_ids:
@@ -122,23 +132,26 @@
     @staticmethod
     def parse_active_path() -> Tuple[Optional[str], Optional[str], Optional[str]]:
         site = None
         contest_id = None
         task_id = None
 
         active_path = os.path.realpath(os.getcwd())
-        home_dir = os.path.realpath(Config.LUCY_HOME)
+        home_dir = os.path.realpath(config.home)
         if active_path.startswith(home_dir):
             active_path = active_path[len(home_dir):]
             active_path = active_path.lstrip('/')
 
             parts = active_path.split('/')[:3]
             if len(parts) >= 1:
                 site = parts[0]
             if len(parts) >= 2:
                 contest_id = parts[1]
             if len(parts) >= 3:
                 task_id = parts[2]
-            if site:
-                site = site.lower()
 
         return site, contest_id, task_id
+
+    @staticmethod
+    def get_impl_hash(website: Website, contest_id: str, task_id: str) -> str:
+        content = LocalFS.read(LocalFS.get_impl_path(website, contest_id, task_id))
+        return hashlib.md5(content.encode()).hexdigest()
```

### Comparing `lucy01-0.2.1/lucy/parser_/atcoder.py` & `lucy01-1.0.0/lucy/parser_/atcoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,55 @@
+import concurrent
+from concurrent.futures import ThreadPoolExecutor
+import concurrent.futures
 from typing import Any, Generator, Optional, Tuple
 
 import click
 
 from lucy import utils
-from lucy.config import Config, Website
+from lucy.config import config, Website
 from lucy.scraper import Scraper
 
 from lucy.parser_.parser_ import Parser, Task
 
 
 class AtCoderParser(Parser):
 
     @staticmethod
     def __parse_samples(task_page: Any) -> Generator[Tuple[str, str], None, None]:
         for input, output in utils.batched(task_page.select('pre[id]'), 2):
             yield input.text, output.text
 
-    def __parse_tasks(self, page: Any) -> list[Task]:
-        tasks: list[Task] = []
+    def __parse_tasks(self, row: Any) -> Optional[Task]:
+        data = row.find_all('td')
+        task_id, task_name = data[0].text, data[1].text
+
+        if self.task_id is not None and task_id != self.task_id:
+            return None
+
+        task_path = f'{self.contest_id}_{task_id.lower()}'
+        task_page = Scraper().get(f'{self.tasks_page_url}/{task_path}')
+        samples = list(AtCoderParser.__parse_samples(task_page))
+        click.secho(f'Found {len(samples)} samples for task {task_id}.', fg='green', bold=True)
+        task = Task(task_id, task_name, samples)
+        return task
 
-        tasks_table = page.select('table.table tbody tr')
-        for row in tasks_table:
-            data = row.find_all('td')
-            task_id, task_name = data[0].text, data[1].text
-
-            if self.task_id is not None and task_id != self.task_id:
-                continue
-
-            task_path = f'{self.contest_id}_{task_id.lower()}'
-            task_page = Scraper().get(f'{self.tasks_page_url}/{task_path}')
-            samples = [sample for sample in AtCoderParser.__parse_samples(task_page)]
-            click.secho(f'Found {len(samples)} samples for task {task_id}.', fg='green', bold=True)
-
-            task = Task(task_id, task_name, samples)
-            tasks.append(task)
-
-        return tasks
-
-    def __init__(self, contest_id: str, task_id: Optional[str]) -> None:
+    def __init__(self, contest_id: str, task_id: Optional[str], n_threads: int) -> None:
         self.contest_id = contest_id
         self.task_id = task_id
 
         scraper = Scraper()
 
-        self.tasks_page_url = f'{Config.WEBSITE_HOST[Website.ATCODER]}/contests/{contest_id}/tasks'
+        self.tasks_page_url = f'{config.website[Website.ATCODER].host}/contests/{contest_id}/tasks'
         tasks_page = scraper.get(self.tasks_page_url)
 
-        tasks = self.__parse_tasks(tasks_page)
+        tasks = []
+        with ThreadPoolExecutor(max_workers=n_threads) as executor:
+            tasks_table = tasks_page.select('table.table tbody tr')
+            click.echo(f'Found {len(tasks_table)} tasks.')
+            futures = [executor.submit(self.__parse_tasks, row) for row in tasks_table]
+            for future in concurrent.futures.as_completed(futures):
+                task = future.result()
+                if task:
+                    tasks.append(task)
 
         super().__init__(tasks)
```

### Comparing `lucy01-0.2.1/lucy/scraper.py` & `lucy01-1.0.0/lucy/scraper.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.2.1/lucy/tester.py` & `lucy01-1.0.0/lucy/tester.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,18 +41,19 @@
             out_txt = process.stdout.read().decode()
             process.wait()
         return out_txt.strip() == truth_txt.strip(), out_txt
 
     def run(self, verbose: bool = False, continue_: bool = False) -> None:
         self.__compile()
 
+        total_n_tests = LocalFS.num_samples(self.website, self.contest_id, self.task_id)
         for i, (in_txt, truth_txt) in zip(
                 self.test_ids,
                 LocalFS.tests(self.website, self.contest_id, self.task_id, self.test_ids)):
-            click.echo(f'Test#{i:02d}', nl=False)
+            click.echo(f'Test#{i:02d}/{total_n_tests - 1:02d}', nl=False)
             click.echo(f'{"." * 50}', nl=False)
             passes, out_txt = self.__exec(in_txt, truth_txt)
             if passes:
                 click.secho('AC', bg='green')
             else:
                 click.secho('WA', bg='red')
                 if verbose:
```

### Comparing `lucy01-0.2.1/lucy/update_snippets.py` & `lucy01-1.0.0/lucy/update_snippets.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.2.1/lucy01.egg-info/PKG-INFO` & `lucy01-1.0.0/lucy01.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucy01
-Version: 0.2.1
+Version: 1.0.0
 Summary: CLI companion for CP.
 Author-email: Mehul Todi <mehul116.dev@gmail.com>
 Project-URL: Documentation, https://lucy01.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/kid-116/Lucy
 Project-URL: Issues, https://github.com/kid-116/Lucy/issues
 Keywords: cp,cli,companion,atcoder,codeforces,tester,snippets,lucy
 Classifier: Development Status :: 4 - Beta
@@ -12,45 +12,52 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: click
-Requires-Dist: dropbox
 Requires-Dist: lxml
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: selenium
 Provides-Extra: lint
 Requires-Dist: mypy; extra == "lint"
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: pylint[spelling]; extra == "lint"
 Requires-Dist: yapf; extra == "lint"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-datadir; extra == "test"
+
+[![Lint](https://github.com/kid-116/Lucy/actions/workflows/pylint.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/pylint.yml)
+[![Test](https://github.com/kid-116/Lucy/actions/workflows/pytest.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/pytest.yml)
+[![Publish PyPI](https://github.com/kid-116/Lucy/actions/workflows/publish.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/publish.yml)
+[![GitHub Release](https://github.com/kid-116/Lucy/actions/workflows/gh-release.yml/badge.svg)](https://github.com/kid-116/Lucy/actions/workflows/gh-release.yml)
 
 # Lucy
 
 Lucy, a CLI companion for competitive programming on AtCoder and Codeforces, frees you from tedious
 tasks. It automatically fetches sample tests, sets up directories, and lets you test your code with
 just a few commands, streamlining your workflow and letting you focus on writing brilliant
 solutions.
 
 [Demo](https://github.com/kid-116/Lucy/assets/75692643/1b7195f7-fcd3-4e05-b23e-48061f6ef1b1)
 
-## Support Languages
+## Supported Languages
 - [x] C++
 - [ ] Python
 
 ## Supported Platforms
 - [x] AtCoder
 - [ ] Codeforces
 
 ## Featues
 - [x] Fetch Sample Test Cases
-- [x] Fetch Hidden Test Cases (after the contest 🤪)
+- [ ] Fetch Hidden Test Cases (after the contest 🤪)
 - [x] Test Solution
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
 ```
@@ -58,22 +65,14 @@
 ```
 
 ## Environment Variables
 - `LUCY_HOME`
 
     Specify home directory for `lucy`.
 
-- `DROPBOX_TOKEN`
-
-
-    Dropbox developer access token with `sharing.read` permission. It can be generated at
-    [DBX Platform for Developers](https://www.dropbox.com/developers). This is necessary to fetch
-    hidden AtCoder test cases releaved after the contest has ended. All AtCoder test cases may be
-    found [here](https://www.dropbox.com/sh/nx3tnilzqz7df8a/AAAYlTq2tiEHl5hsESw6-yfLa?dl=0).
-
 ## Getting Started
 1. Set the environment variable `$LUCY_HOME` as preferred. By default, it uses the `~/.lucy`.
 2. Get help!
     ```
     lucy --help
     ```
     Check out the [documentation](https://lucy01.readthedocs.io/en/latest/).
```

### Comparing `lucy01-0.2.1/pyproject.toml` & `lucy01-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [project]
 name = "lucy01"
-version = "0.2.1"
+version = "1.0.0"
 description = "CLI companion for CP."
 readme = "README.md"
 dependencies = [
     "bs4",
     "click",
-    "dropbox",
     "lxml",
     "python-dotenv",
     "requests",
     "selenium",
 ]
 requires-python = ">=3.10"
 authors = [{ name = "Mehul Todi", email = "mehul116.dev@gmail.com" }]
@@ -43,14 +42,15 @@
 Repository = "https://github.com/kid-116/Lucy"
 Issues = "https://github.com/kid-116/Lucy/issues"
 # Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 
 [project.optional-dependencies]
 lint = ["mypy", "pylint", "pylint[spelling]", "yapf"]
 # docs = ["mkdocs", "md-click@git+https://github.com/kid-116/md-click.git@support-arguments"]
+test = ["pytest", "pytest-datadir"]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 lucy = "lucy.main:lucy"
```

