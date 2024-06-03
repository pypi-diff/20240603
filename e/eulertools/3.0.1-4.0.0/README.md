# Comparing `tmp/eulertools-3.0.1.tar.gz` & `tmp/eulertools-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-3.0.1.tar", max compression
+gzip compressed data, was "eulertools-4.0.0.tar", max compression
```

## Comparing `eulertools-3.0.1.tar` & `eulertools-4.0.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     7696 2024-05-03 11:21:21.641696 eulertools-3.0.1/LICENSE.md
--rw-r--r--   0        0        0     2121 2024-05-02 15:56:28.389983 eulertools-3.0.1/docs/README.md
--rw-r--r--   0        0        0     3151 2024-05-20 16:01:27.756682 eulertools-3.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-15 11:17:41.471041 eulertools-3.0.1/src/eulertools/__init__.py
--rw-r--r--   0        0        0     3918 2024-05-20 10:31:59.098734 eulertools-3.0.1/src/eulertools/__main__.py
--rw-r--r--   0        0        0       22 2024-05-20 16:01:32.263348 eulertools-3.0.1/src/eulertools/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 14:48:27.711640 eulertools-3.0.1/src/eulertools/lib/__init__.py
--rw-r--r--   0        0        0      207 2023-10-26 22:44:37.486503 eulertools-3.0.1/src/eulertools/lib/exceptions.py
--rw-r--r--   0        0        0     8978 2024-05-20 15:41:05.526670 eulertools-3.0.1/src/eulertools/lib/utils.py
--rw-r--r--   0        0        0        0 2024-05-17 14:45:18.800978 eulertools-3.0.1/src/eulertools/subcommands/__init__.py
--rw-r--r--   0        0        0     2980 2024-05-20 11:04:41.521205 eulertools-3.0.1/src/eulertools/subcommands/compare.py
--rw-r--r--   0        0        0      917 2024-05-20 10:34:28.119065 eulertools-3.0.1/src/eulertools/subcommands/generate.py
--rw-r--r--   0        0        0     4253 2024-05-20 12:55:58.516489 eulertools-3.0.1/src/eulertools/subcommands/run.py
--rw-r--r--   0        0        0      956 2024-05-20 10:35:55.387334 eulertools-3.0.1/src/eulertools/subcommands/statement.py
--rw-r--r--   0        0        0      979 2024-05-20 11:22:55.712555 eulertools-3.0.1/src/eulertools/subcommands/test.py
--rw-r--r--   0        0        0     3885 2024-05-20 12:12:16.951976 eulertools-3.0.1/src/eulertools/subcommands/time.py
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 eulertools-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-30 11:23:15.612995 eulertools-4.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2121 2024-05-30 11:23:15.609661 eulertools-4.0.0/docs/README.md
+-rw-r--r--   0        0        0     3151 2024-06-03 13:01:55.488646 eulertools-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 11:23:15.552996 eulertools-4.0.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0     1204 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/__main__.py
+-rw-r--r--   0        0        0       22 2024-06-03 13:01:55.488646 eulertools-4.0.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:23:15.616328 eulertools-4.0.0/src/eulertools/lib/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-30 14:13:16.308853 eulertools-4.0.0/src/eulertools/lib/exceptions.py
+-rw-r--r--   0        0        0     3220 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/lib/parser.py
+-rw-r--r--   0        0        0    15164 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/lib/utils.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:23:15.622994 eulertools-4.0.0/src/eulertools/py.typed
+-rw-r--r--   0        0        0        0 2024-05-30 11:23:15.616328 eulertools-4.0.0/src/eulertools/subcommands/__init__.py
+-rw-r--r--   0        0        0     3166 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/subcommands/compare.py
+-rw-r--r--   0        0        0      960 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/subcommands/generate.py
+-rw-r--r--   0        0        0     6719 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/subcommands/run.py
+-rw-r--r--   0        0        0     1020 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/subcommands/statement.py
+-rw-r--r--   0        0        0     2830 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/subcommands/test.py
+-rw-r--r--   0        0        0     5316 2024-06-03 13:01:55.225319 eulertools-4.0.0/src/eulertools/subcommands/time.py
+-rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 eulertools-4.0.0/PKG-INFO
```

### Comparing `eulertools-3.0.1/LICENSE.md` & `eulertools-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulertools-3.0.1/docs/README.md` & `eulertools-4.0.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `eulertools-3.0.1/pyproject.toml` & `eulertools-4.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "3.0.1"
+version = "4.0.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
```

### Comparing `eulertools-3.0.1/src/eulertools/subcommands/compare.py` & `eulertools-4.0.0/src/eulertools/subcommands/compare.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,49 @@
 from itertools import chain
 
-from eulertools.lib.utils import Language, Problem, get_all_keyed_problems, get_timings
+from eulertools.lib.utils import CaseId, Language, Problem, get_summary
+
+PROBLEM = "problem"
+CASE_KEY = "case_key"
+MISSING = "N/A"
 
 
 class Compare:
+    __slots__ = (
+        "languages",
+        "problems",
+        "summary",
+        "case_ids",
+        "pad_length",
+    )
+
     def __init__(self, languages: list[Language], problems: list[Problem]):
         self.languages = languages
-        self.timings = {language: get_timings(language) for language in languages}
-        self.keyed_problems = self.get_keyed_problems(languages, problems)
+        self.problems = problems
+        self.summary = get_summary()
+        self.case_ids = self.get_case_ids()
         self.pad_length = self._pad_length()
 
     def run(self) -> None:
-        labels = [
-            ["problem", "id"],
-            *[[problem, str(key)] for problem, key in self.keyed_problems],
-        ]
         matrix = [
-            *self.transpose(labels),
+            *self.transpose(self.labels),
             *(self.get_language_timings(language) for language in self.languages),
         ]
         self.print_table(self.transpose(matrix))
 
+    @property
+    def labels(self) -> list[list[str]]:
+        return [
+            [PROBLEM, CASE_KEY],
+            *(
+                [case_id.problem.name, str(case_id.case_key)]
+                for case_id in self.case_ids
+            ),
+        ]
+
     def print_table(self, matrix: list[list[str]]) -> None:
         n = len(self.languages) + 2
         spacing = ["─" * self.pad_length for _ in range(n)]
         top = "┌" + "┬".join(spacing) + "┐"
         mid = "├" + "┼".join(spacing) + "┤"
         btm = "└" + "┴".join(spacing) + "┘"
         print(top)
@@ -36,48 +55,47 @@
                 "│".join(self.padded_print(item, heading=(i == 0)) for item in row),
                 "│",
                 sep="",
             )
         print(btm)
 
     def get_language_timings(self, language: Language) -> list[str]:
-        timings = get_timings(language)
         return [
             language.name,
             *(
-                str(timings.get(problem, {}).get(key, "N/A"))
-                for problem, key in self.keyed_problems
+                str(
+                    self.summary.problems[case_id.problem]
+                    .cases[case_id]
+                    .timings.get(language, MISSING)
+                )
+                for case_id in self.case_ids
             ),
         ]
 
-    @staticmethod
-    def transpose(matrix: list[list[str]]) -> list[list[str]]:
-        new_lines = (list(row) for row in zip(*matrix, strict=True))
-        return [line for line in new_lines if any(item != "N/A" for item in line[1:])]
+    @classmethod
+    def transpose(cls, matrix: list[list[str]]) -> list[list[str]]:
+        return [list(row) for row in zip(*matrix, strict=True)]
 
     def padded_print(self, string: str, *, heading: bool) -> str:
         if heading:
             return string.center(self.pad_length)
         return string.rjust(self.pad_length)
 
-    def get_keyed_problems(
-        self, languages: list[Language], problems: list[Problem]
-    ) -> list[tuple[str, int]]:
-        problem_ids = {problem.id for problem in problems}
-        return [
-            (problem, key)
-            for problem, key in get_all_keyed_problems()
-            if any(
-                problem_key
-                for language in languages
-                for problem_key in self.timings[language].get(problem, {})
-            )
-            and problem in problem_ids
-        ]
+    def get_case_ids(self) -> list[CaseId]:
+        return sorted(
+            (
+                case_id
+                for problem_summary in self.summary.problems.values()
+                if problem_summary.problem in self.problems
+                for case_id, case_summary in problem_summary.cases.items()
+                if any(language in case_summary.timings for language in self.languages)
+            ),
+            key=lambda case_id: (case_id.problem.name, case_id.case_key),
+        )
 
     def _pad_length(self) -> int:
         lengths = chain(
-            (len(problem) + len(str(key)) for problem, key in self.keyed_problems),
+            [len(MISSING)],
             (len(language.name) for language in self.languages),
-            [len("problem"), len("id")],
+            [len(row) for label in self.labels for row in label],
         )
         return max(lengths) + 2
```

### Comparing `eulertools-3.0.1/src/eulertools/subcommands/generate.py` & `eulertools-4.0.0/src/eulertools/subcommands/generate.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     get_context,
     get_solution,
     get_template,
 )
 
 
 class Generate:
+    __slots__ = ("languages", "problems")
+
     def __init__(self, languages: list[Language], problems: list[Problem]):
         self.languages = languages
         self.problems = problems
 
     def run(self) -> None:
         for problem in self.problems:
             for language in self.languages:
```

### Comparing `eulertools-3.0.1/src/eulertools/subcommands/statement.py` & `eulertools-4.0.0/src/eulertools/subcommands/statement.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from pyutilkit.term import SGRCodes, SGRString
 
 from eulertools.lib.utils import Problem, get_statement
 
 
 class Statement:
+    __slots__ = ("problems", "show_hints")
+
     def __init__(self, problems: list[Problem], *, show_hints: bool):
         self.problems = problems
         self.show_hints = show_hints
 
     def run(self) -> None:
         for problem in self.problems:
             self.show_statement(problem)
+            print()
 
     def show_statement(self, problem: Problem) -> None:
         statement = get_statement(problem)["common"]
         if title := statement.get("title", ""):
             print(SGRString(title, params=[SGRCodes.GREEN]))
             print(SGRString("~" * len(title), params=[SGRCodes.GREEN]))
         print(statement["description"].strip())
```

### Comparing `eulertools-3.0.1/src/eulertools/subcommands/time.py` & `eulertools-4.0.0/src/eulertools/subcommands/time.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,143 @@
-from itertools import product
-
-from pyutilkit.term import SGRCodes, SGRString
+import sys
 
 from eulertools.lib.utils import (
+    CaseResult,
     Language,
-    Modes,
+    ParseResult,
     Problem,
+    Summary,
+    UpdateMode,
     get_average,
-    get_solution,
-    get_timings,
-    update_timings,
+    update_summary,
 )
 from eulertools.subcommands.run import Run
 
 
 class Time:
+
+    __slots__ = (
+        "success",
+        "languages",
+        "problems",
+        "times",
+        "verbosity",
+        "update_mode",
+    )
+
     def __init__(
         self,
         languages: list[Language],
         problems: list[Problem],
         times: int,
         verbosity: int,
-        *,
-        run_update: bool,
-        append_new: bool,
+        update_mode: UpdateMode,
     ):
+        self.success = True
         self.languages = languages
         self.problems = problems
         self.times = times
         self.verbosity = verbosity
-        self.run_update = run_update
-        self.append_new = append_new
-        self.timings = {language: get_timings(language) for language in languages}
+        self.update_mode = update_mode
 
     def run(self) -> None:
-        for run_index, (language, problem) in enumerate(
-            product(self.languages, self.problems)
+        runner = Run(
+            self.languages, self.problems, verbosity=self.verbosity, times=self.times
+        )
+        for language, problem, summary in runner.get_summaries(
+            self.languages, self.problems
         ):
-            self.time_single_problem(language, problem, run_index)
-        if self.run_update or self.append_new:
-            for language in self.languages:
-                update_timings(language, self.timings[language])
+            if not summary.problem_successful(language, problem):
+                self.success = False
+            self.print_summary(language, problem, summary)
+            if self.update_mode != UpdateMode.NONE:
+                self.prepare_summary(language, problem, summary)
+        if self.update_mode != UpdateMode.NONE:
+            update_summary(summary)
+        if not self.success:
+            sys.exit(81)
 
-    def time_single_problem(
-        self, language: Language, problem: Problem, run_index: int
+    def print_summary(
+        self, language: Language, problem: Problem, summary: Summary
     ) -> None:
-        self.timings[language].setdefault(problem.id, {})
-        solution = get_solution(language, problem)
-        if not solution.exists():
+        problem_summary = summary.problems[problem]
+        parse_result = problem_summary.result[language]
+        if parse_result == ParseResult.FAILURE:
+            print(
+                f"🔴 Timing {language.name} // {problem.id}... Failed to parse results",
+                file=sys.stderr,
+            )
             return
+        for case_id, case_summary in problem_summary.cases.items():
+            case_key = case_id.case_key
+            time_text = f"Timing {language.name} // {problem.id} // {case_key}..."
+            if case_summary.result.get(language) in {
+                CaseResult.WRONG_RESPONSE,
+                CaseResult.MISSING_KEY,
+                CaseResult.NON_DETERMINISTIC,
+            }:
+                print(f"🔴 {time_text}... Unsuccessful run", file=sys.stderr)
+                continue
+            old_timing = case_summary.timings.get(language)
+            raw_timings = case_summary.new_timings[language]
+            new_timing = get_average(raw_timings)
 
-        raw_timings = Run(
-            [language],
-            [problem],
-            verbosity=self.verbosity,
-            mode=Modes.TIMING,
-            times=self.times,
-        ).run()[language][problem.id]
-        old_timings = self.timings[language][problem.id]
-        new_timings = {
-            run_id: get_average(timings) for run_id, timings in raw_timings.items()
-        }
-        for key_index, key in enumerate(sorted(new_timings)):
-            old_timing = old_timings.get(key)
-            raw_timing = raw_timings[key]
-            new_timing = new_timings[key]
             if old_timing is None:
-                overall_difference = None
-            elif old_timing < new_timing:
-                overall_difference = "🔴"
+                general_prefix = "🟠"
+                suffix = f"initial timing: {new_timing}"
             elif old_timing > new_timing:
-                overall_difference = "🟢"
+                general_prefix = "🟢"
+                suffix = f"timing changed from {old_timing} to {new_timing}"
+            elif old_timing < new_timing:
+                general_prefix = "🔴"
+                suffix = f"timing changed from {old_timing} to {new_timing}"
             else:
-                overall_difference = "🔵"
-            if self.run_update or (self.append_new and old_timing is None):
-                self.timings[language][problem.id][key] = new_timing
-            title = f"Timing {language.name} // {problem.id} // {key}..."
-            if run_index or key_index:
-                print()
-            print(SGRString(title, params=[SGRCodes.GREEN]))
-            print(SGRString("~" * len(title), params=[SGRCodes.GREEN]))
-            if old_timing:
-                print(f"🟤 Old timing: {old_timing}")
-            prefix = (
-                f"{overall_difference} New" if old_timing is not None else "🔵 Initial"
+                general_prefix = "🔵"
+                suffix = f"timing remained unchanged at: {new_timing}"
+            print(
+                f"{general_prefix} {time_text} {suffix if self.verbosity == 0 else ''}"
             )
-            print(f"{prefix} timing: {new_timing}")
             if self.verbosity > 0:
-                print("    ⏱️  New timings:")
-                for i, timing in enumerate(raw_timing):
-                    if old_timing is None:
-                        prefix = "🔵"
-                    elif timing > old_timing:
-                        prefix = "⬆️ "
-                    elif timing < old_timing:
-                        prefix = "⬇️ "
-                    else:
-                        prefix = "↔️ "
-                    print(f"       {prefix} Run {i + 1} took: {timing}")
-            if self.verbosity > 1 and old_timing is not None:
-                old_nanoseconds = old_timing.nanoseconds
-                new_nanoseconds = new_timing.nanoseconds
-                change = 100 * (old_nanoseconds - new_nanoseconds) / old_nanoseconds
-                print(f"{overall_difference} Performance difference: {change:.2f}%")
+                prefix = "    ⏱️"
+                if old_timing:
+                    print(f"{prefix} Old timing: {old_timing}")
+                print(f"{prefix} New timing: {new_timing}")
+                if old_timing is not None:
+                    old_nanoseconds = old_timing.nanoseconds
+                    new_nanoseconds = new_timing.nanoseconds
+                    change = 100 * (old_nanoseconds - new_nanoseconds) / old_nanoseconds
+                    print(f"    {general_prefix} Performance difference: {change:.2f}%")
+                if self.verbosity > 1:
+                    print(f"{prefix} Detailed new timings:")
+                    for i, timing in enumerate(raw_timings):
+                        if old_timing is None:
+                            prefix = "         "
+                        elif timing > old_timing:
+                            prefix = "       ⬆️"
+                        elif timing < old_timing:
+                            prefix = "       ⬇️"
+                        else:
+                            prefix = "       ↔️"
+                        print(f"{prefix} Run {i + 1} took: {timing}")
+
+    def prepare_summary(
+        self, language: Language, problem: Problem, summary: Summary
+    ) -> None:
+        problem_summary = summary.problems[problem]
+        parse_result = problem_summary.result[language]
+        if parse_result == ParseResult.FAILURE:
+            return
+
+        for case_summary in problem_summary.cases.values():
+            case_result = case_summary.result[language]
+            if case_result in {
+                CaseResult.MISSING_KEY,
+                CaseResult.NON_DETERMINISTIC,
+            }:
+                continue
+            if (
+                case_result in {CaseResult.SUCCESS, CaseResult.WRONG_RESPONSE}
+                and self.update_mode == UpdateMode.APPEND
+            ):
+                continue
+            new_timing = get_average(case_summary.new_timings[language])
+            case_summary.timings[language] = new_timing
```

### Comparing `eulertools-3.0.1/PKG-INFO` & `eulertools-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulertools
-Version: 3.0.1
+Version: 4.0.0
 Summary: Multilanguage competitive coding toolbox
 Home-page: https://eulertools.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: leetcode,topcoder,project_euler
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.11,<4.0
```

