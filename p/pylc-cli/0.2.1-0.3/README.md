# Comparing `tmp/pylc_cli-0.2.1.tar.gz` & `tmp/pylc_cli-0.3.tar.gz`

## Comparing `pylc_cli-0.2.1.tar` & `pylc_cli-0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/display_question.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/main.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/run_solution.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/solve.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/queries/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/queries/fetch_question.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/queries/fetch_snippets.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/queries/fetch_stats.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/queries/judge.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pylc_cli/queries/status.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/README.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pylc_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/cache.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/display_problem.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/main.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/run_solution.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/solve.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/queries/__init__.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/queries/fetch_all_problems.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/queries/fetch_problem.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/queries/fetch_stats.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/queries/judge.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pylc_cli-0.3/pylc_cli/queries/status.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pylc_cli-0.3/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylc_cli-0.3/README.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pylc_cli-0.3/pyproject.toml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 pylc_cli-0.3/PKG-INFO
```

### Comparing `pylc_cli-0.2.1/pylc_cli/__init__.py` & `pylc_cli-0.3/pylc_cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from pathlib import Path
 from rich.console import Console
+import sqlite3
 import tomllib
 import tomli_w
 
 BASE_DIR = f"{Path.home()}/.pylc"
 Path(f"{BASE_DIR}/code").mkdir(parents=True, exist_ok=True)
+CACHE_PATH = f"{BASE_DIR}/cache.sqlite"
+
+con = sqlite3.connect(CACHE_PATH)
+con.row_factory = sqlite3.Row
 
 EXT_MAP = {
     "c": "c",
     "cpp": "cpp",
     "java": "java",
     "python": "py",
     "python3": "py",
```

### Comparing `pylc_cli-0.2.1/pylc_cli/main.py` & `pylc_cli-0.3/pylc_cli/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 import argparse
-from pathlib import Path
-from . import BASE_DIR, EXT_MAP, prefs
-from .display_question import display_question
+from . import EXT_MAP, prefs
+from .display_problem import display_problem
 from .run_solution import run
 from .solve import solve
-from .queries.fetch_question import fetch_daily
+from .cache import update_cache
+from .queries.fetch_problem import fetch_daily
 
 
 def main():
     lang = prefs["lang"]
     editor = prefs["editor"]
     editor_args = prefs["editor_args"]
 
     parser = argparse.ArgumentParser()
 
     subparsers = parser.add_subparsers(dest="command")
 
     daily_parser = subparsers.add_parser("daily")
 
     pick_parser = subparsers.add_parser("pick")
-    pick_parser.add_argument("titleslug")
+    pick_parser.add_argument("id", type=int)
 
     solve_parser = subparsers.add_parser("solve")
-    solve_parser.add_argument("titleslug")
+    solve_parser.add_argument("id", type=int)
     solve_parser.add_argument("--lang", default=lang, choices=EXT_MAP.keys())
 
     test_parser = subparsers.add_parser("test")
-    test_parser.add_argument("titleslug")
+    test_parser.add_argument("id", type=int)
     test_parser.add_argument("--lang", default=lang, choices=EXT_MAP.keys())
 
     submit_parser = subparsers.add_parser("submit")
-    submit_parser.add_argument("titleslug")
+    submit_parser.add_argument("id", type=int)
     submit_parser.add_argument("--lang", default=lang, choices=EXT_MAP.keys())
 
+    update_parser = subparsers.add_parser("update")
+
     args = parser.parse_args()
 
     if args.command == "daily":
-        display_question(title_slug=fetch_daily())
+        display_problem(id=fetch_daily())
 
     if args.command == "pick":
-        display_question(title_slug=args.titleslug)
+        display_problem(id=args.id)
 
     elif args.command == "solve":
         solve(
-            title_slug=args.titleslug,
+            id=args.id,
             lang=args.lang,
             editor=editor,
             editor_args=editor_args,
         )
 
     elif args.command == "test":
-        run(title_slug=args.titleslug, lang=args.lang, test=True)
+        run(id=args.id, lang=args.lang, test=True)
 
     elif args.command == "submit":
-        run(title_slug=args.titleslug, lang=args.lang, test=False)
+        run(id=args.id, lang=args.lang, test=False)
+
+    elif args.command == "update":
+        update_cache()
```

### Comparing `pylc_cli-0.2.1/pylc_cli/run_solution.py` & `pylc_cli-0.3/pylc_cli/run_solution.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import ast
 from pathlib import Path
 from rich.padding import Padding
-from . import BASE_DIR, console, EXT_MAP
-from .queries.fetch_question import fetch_question
+from . import BASE_DIR, console, EXT_MAP, con
 from .queries.judge import send_judge
 from .queries.status import get_status
 
 
 def stringify_code(file_path: str) -> str:
     if not Path(file_path).is_file():
         # TODO: handle code file generation
@@ -14,94 +12,95 @@
 
     with open(file_path, "r") as f:
         lines = f.readlines()
 
     return "".join(lines)
 
 
-def run(title_slug: str, lang: str, test: bool):
-    question = fetch_question(title_slug=title_slug)
-    id = question["questionFrontendId"]
+def run(id: int, lang: str, test: bool):
+    res = con.execute(
+        f"SELECT id, title_slug FROM metadata WHERE frontend_id = {id}"
+    )
+    data = res.fetchone()
+    title_slug = data["title_slug"]
     ext = EXT_MAP[lang]
 
     file_path = f"{BASE_DIR}/code/{id}.{title_slug}.{lang}.{ext}"
     if not Path(file_path).is_file():
         raise FileNotFoundError
 
     typed_code = stringify_code(file_path=file_path)
 
     with console.status(status="Sending code to server...", spinner="monkey"):
         run_id = send_judge(
-            title_slug=title_slug, lang=lang, typed_code=typed_code, test=test
+            title_slug=title_slug,
+            id=data["id"],
+            lang=lang,
+            typed_code=typed_code,
+            test=test
         )
         status = get_status(title_slug=title_slug, id=run_id, test=test)
 
     if test:
         if status["status_msg"] == "Accepted":
             if status["correct_answer"]:
                 console.print(Padding("Accepted", (1, 2), style="bold green"))
             else:
                 console.print(Padding("Wrong Answer", (1, 2), style="bold red"))
 
             console.print(Padding(
-                f"Expected answer: {status["expected_code_answer"]}", 
-                (0, 2)
-            ))
-            console.print(Padding(
-                f"Your answer: {status["code_answer"]}",
-                (0, 2)
-            ))
-            console.print(Padding(
+                f"Expected answer: {status["expected_code_answer"]}\n"
+                f"Your answer: {status["code_answer"]}\n"
                 f"stdout: {status["code_output"]}",
-                (1, 2)
+                (0, 2, 1, 2)
             ))
+
         elif status["status_msg"] == "Runtime Error":
             console.print(Padding("Runtime Error", (1, 2), style="bold red"))
-            console.print(Padding(status["runtime_error"], (0, 2)))
-            
+            console.print(Padding(status["runtime_error"], (0, 2, 1, 2)))
+        
+        elif status["status_msg"] == "Compile Error":
+            console.print(Padding("Compile Error", (1, 2), style="bold red"))
+            console.print(Padding(status["compile_error"], (0, 2, 1, 2)))            
 
     else:
         if status["status_msg"] == "Accepted":
             console.print(Padding(status["status_msg"], (1, 2), style="bold green"))
             console.print(Padding(
                 f"Runtime: {status["status_runtime"]} "
                 f"beats {round(status["runtime_percentile"], 2)}% of users "
-                f"using {status["pretty_lang"]}.",
-                (0, 2)
-            ))
-            console.print(Padding(
+                f"using {status["pretty_lang"]}.\n"
                 f"Memory: {status["status_memory"]} "
                 f"beats {round(status["memory_percentile"], 2)}% of users "
                 f"using {status["pretty_lang"]}.",
-                (0, 2)
+                (0, 2, 1, 2)
             ))
+
         else:
-            console.print(Padding(status["status_msg"], (1, 2), style="bold red"))
+            console.print(
+                Padding(status["status_msg"], (1, 2), style="bold red")
+            )
             if status["status_msg"] == "Wrong Answer":
                 console.print(Padding(
-                    f"Last testcase: {status["input_formatted"]}",
-                    (0, 2)
-                ))
-                console.print(Padding(
-                    f"Expected Answer: {status["expected_output"]}",
-                    (0, 2)
-                ))
-                console.print(Padding(
+                    f"Last testcase: {status["input_formatted"]}\n"
+                    f"Expected Answer: {status["expected_output"]}\n"
                     f"Your Answer: {status["code_output"]}",
-                    (0, 2)
+                    (0, 2, 1, 2)
                 ))
+
             elif status["status_msg"] == "Runtime Error":
-                console.print(Padding(status["full_runtime_error"], (0, 2)))
+                console.print(Padding(status["full_runtime_error"], (1, 2)))
+
             elif status["status_msg"] == "Compile Error":
-                console.print(Padding(status["full_compile_error"], (0, 2)))
+                console.print(Padding(status["full_compile_error"], (1, 2)))
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("titleslug")
-    parser.add_argument("lang")
-    parser.add_argument("test")
+    parser.add_argument("id", type=int)
+    parser.add_argument("lang", choices=EXT_MAP.keys())
+    parser.add_argument("test", type=bool)
     args = parser.parse_args()
 
-    run(args.titleslug, args.lang, ast.literal_eval(args.test))    
+    run(args.titleslug, args.lang, args.test)
```

### Comparing `pylc_cli-0.2.1/pylc_cli/queries/fetch_question.py` & `pylc_cli-0.3/pylc_cli/queries/fetch_problem.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,73 @@
 import requests
-
 from . import generate_headers, GRAPHQL_URL
 
 
-def fetch_daily() -> str:
+def fetch_daily() -> int:
     headers = generate_headers()
     query = """
     query {
       activeDailyCodingChallengeQuestion {
         question {
-          titleSlug
+          questionFrontendId
         }
       }
     }
     """
 
     response = requests.post(url=GRAPHQL_URL, json={"query": query}, headers=headers)
     if response.status_code != 200:
         # TODO: handle 403 errors nicely
         raise ConnectionError
 
     json = response.json()
-    return json["data"]["activeDailyCodingChallengeQuestion"]["question"]["titleSlug"]
+    return int(
+        json["data"]["activeDailyCodingChallengeQuestion"]["question"][
+            "questionFrontendId"
+        ]
+    )
 
 
-def fetch_question(title_slug: str) -> dict:
+def fetch_problem_snippets(title_slug: str) -> dict:
     headers = generate_headers()
     query = """
     query ($titleSlug: String!) {
       question(titleSlug: $titleSlug) {
-        questionId
-        questionFrontendId
-        title
-        difficulty
-        content
-        mysqlSchemas
-        exampleTestcaseList
-        topicTags {
-          name
+        codeSnippets {
+          langSlug
+          code
         }
       }
+    }       
+    """
+    variables = {"titleSlug": title_slug}
+    response = requests.post(
+        url=GRAPHQL_URL, json={"query": query, "variables": variables}, headers=headers
+    )
+    if response.status_code != 200:
+        # TODO: handle 403 errors nicely
+        raise ConnectionError
+
+    json = response.json()
+
+    snippets = {
+        snippet_map["langSlug"]: snippet_map["code"]
+        for snippet_map in json["data"]["question"]["codeSnippets"]
+    }
+
+    return snippets
+
+
+def fetch_problem_testcases(title_slug: str) -> dict:
+    headers = generate_headers()
+    query = """
+    query ($titleSlug: String!) {
+      question(titleSlug: $titleSlug) {
+        exampleTestcaseList
+      }
     }
     """
     variables = {"titleSlug": title_slug}
 
     response = requests.post(
         url=GRAPHQL_URL, json={"query": query, "variables": variables}, headers=headers
     )
```

### Comparing `pylc_cli-0.2.1/pylc_cli/queries/fetch_stats.py` & `pylc_cli-0.3/pylc_cli/queries/fetch_stats.py`

 * *Files identical despite different names*

### Comparing `pylc_cli-0.2.1/pylc_cli/queries/judge.py` & `pylc_cli-0.3/pylc_cli/queries/judge.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import requests
 import json
 from . import generate_headers, BASE_URL
-from .fetch_question import fetch_question
+from .fetch_problem import fetch_problem_testcases
 
 
-def send_judge(title_slug: str, lang: str, typed_code: str, test: bool):
+def send_judge(title_slug: str, id: int, lang: str, typed_code: str, test: bool):
     url = f"{BASE_URL}/problems/{title_slug}"
     if test:
         url += "/interpret_solution/"
     else:
         url += "/submit/"
 
     headers = generate_headers()
     headers["Referer"] = f"{BASE_URL}/problems/{title_slug}"
 
-    question = fetch_question(title_slug=title_slug)
-    questionId = question["questionId"]
+    test_cases = fetch_problem_testcases(title_slug=title_slug)["exampleTestcaseList"]
 
     payload = {
         "lang": lang,
-        "question_id": questionId,
+        "question_id": id,
         "typed_code": typed_code,
     }
 
     if test:
         input_str = ""
-        for i in question["exampleTestcaseList"]:
+        for i in test_cases:
             input_str += i + "\n"
 
         payload["data_input"] = input_str
 
     response = requests.post(url=url, headers=headers, data=json.dumps(payload))
 
     _json = response.json()
```

### Comparing `pylc_cli-0.2.1/pylc_cli/queries/status.py` & `pylc_cli-0.3/pylc_cli/queries/status.py`

 * *Files identical despite different names*

### Comparing `pylc_cli-0.2.1/.gitignore` & `pylc_cli-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pylc_cli-0.2.1/pyproject.toml` & `pylc_cli-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pylc_cli"
-version = "0.2.1"
+version = "0.3"
 description = "A small CLI tool to solve leetcode problems from your favorite text editor!"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

