# Comparing `tmp/custom_json_diff-0.5.0.tar.gz` & `tmp/custom_json_diff-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_json_diff-0.5.0.tar", last modified: Sat Jun  1 06:45:02 2024, max compression
+gzip compressed data, was "custom_json_diff-0.6.0.tar", last modified: Sun Jun  2 23:12:16 2024, max compression
```

## Comparing `custom_json_diff-0.5.0.tar` & `custom_json_diff-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/custom_json_diff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/custom_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/custom_diff_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/custom_json_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/test/test_bom_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/test/test_custom_json_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:12:16.769168 custom_json_diff-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-06-02 23:12:16.769168 custom_json_diff-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:12:16.769168 custom_json_diff-0.6.0/custom_json_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/custom_json_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/custom_json_diff/bom_diff_template.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/custom_json_diff/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/custom_json_diff/custom_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/custom_json_diff/custom_diff_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:12:16.769168 custom_json_diff-0.6.0/custom_json_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-06-02 23:12:16.000000 custom_json_diff-0.6.0/custom_json_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-02 23:12:16.000000 custom_json_diff-0.6.0/custom_json_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 23:12:16.000000 custom_json_diff-0.6.0/custom_json_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 23:12:16.000000 custom_json_diff-0.6.0/custom_json_diff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 23:12:16.000000 custom_json_diff-0.6.0/custom_json_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 23:12:16.000000 custom_json_diff-0.6.0/custom_json_diff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 23:12:16.769168 custom_json_diff-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 23:12:16.769168 custom_json_diff-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/test/test_bom_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-02 23:12:12.000000 custom_json_diff-0.6.0/test/test_custom_json_diff.py
```

### Comparing `custom_json_diff-0.5.0/LICENSE` & `custom_json_diff-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_json_diff-0.5.0/PKG-INFO` & `custom_json_diff-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: custom-json-diff
-Version: 0.5.0
+Version: 0.6.0
 Summary: Custom JSON diffing and comparison tool.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/custom-json-diff
 Project-URL: Bug Tracker, https://github.com/appthreat/custom-json-diff/issues
+Project-URL: Funding, https://github.com/sponsors/cerrussell
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jinja2>=3.1.4
 Requires-Dist: json-flatten>=0.3
 Requires-Dist: semver>=3.0.0
 Requires-Dist: toml>=0.10
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
@@ -33,33 +35,46 @@
 
 
 
 ## Installation
 `pip install custom-json-diff`
 
 ## CLI Usage
+
 ```
-usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] [-b] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended})
+usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended}) {bom-diff} ...
+
+positional arguments:
+  {bom-diff}            subcommand help
+    bom-diff            compare CycloneDX BOMs
 
 options:
   -h, --help            show this help message and exit
   -i INPUT INPUT, --input INPUT INPUT
                         Two JSON files to compare.
   -o OUTPUT, --output OUTPUT
                         Export JSON of differences to this file.
-  -a, --allow-new-versions
-                        Allow new versions in BOM comparison.
-  -b, --bom-diff        Produce a comparison of CycloneDX BOMs.
   -c CONFIG, --config-file CONFIG
                         Import TOML configuration file.
   -x EXCLUDE [EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...]
                         Exclude field(s) from comparison.
   -p {cdxgen,cdxgen-extended}, --preset {cdxgen,cdxgen-extended}
                         Preset to use
+```
+
+bom-diff usage
+```
+usage: cjd bom-diff [-h] [-a] [-r REPORT_TEMPLATE]
 
+options:
+  -h, --help            show this help message and exit
+  -a, --allow-new-versions
+                        Allow new versions in BOM comparison.
+  -r REPORT_TEMPLATE, --report-template REPORT_TEMPLATE
+                        Jinja2 template to use for report generation.
 ```
 
 ## Specifying fields to exclude
 
 To exclude fields from comparison, use the `-x` or `--exclude` flag and specify the field name(s) 
 to exclude. The json will be flattened, so fields are specified using dot notation. For example:
 
@@ -87,14 +102,17 @@
 ```
 
 To exclude field2, you would specify `field1.field2`. To exclude the `a` field in the array of 
 objects, you would specify `field1.field3.[].a` (do NOT include the array index, just do `[]`). 
 Multiple fields may be specified separated by a space. To better understand what your fields should
 be, check out json-flatten, which is the package used for this function.
 
+>Note: In the context of BOM diffing, this list is only used for the metadata, not the components, 
+> services, or dependencies.
+
 ## Sorting
 
 custom-json-diff will sort the imported JSON alphabetically. If your JSON document contains arrays 
 of objects, you will need to specify any keys you want to sort by in a toml file or use a preset.
 The first key located from the provided keys that is present in the object will be used for sorting.
 
 ## TOML config file example
@@ -102,8 +120,9 @@
 ```toml
 [settings]
 excluded_fields = ["serialNumber", "metadata.timestamp"]
 sort_keys = ["url", "content", "ref", "name", "value"]
 
 [bom_diff]
 allow_new_versions = false
+report_template = "my_template.j2"
 ```
```

### Comparing `custom_json_diff-0.5.0/README.md` & `custom_json_diff-0.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,33 +7,46 @@
 
 
 
 ## Installation
 `pip install custom-json-diff`
 
 ## CLI Usage
+
 ```
-usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] [-b] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended})
+usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended}) {bom-diff} ...
+
+positional arguments:
+  {bom-diff}            subcommand help
+    bom-diff            compare CycloneDX BOMs
 
 options:
   -h, --help            show this help message and exit
   -i INPUT INPUT, --input INPUT INPUT
                         Two JSON files to compare.
   -o OUTPUT, --output OUTPUT
                         Export JSON of differences to this file.
-  -a, --allow-new-versions
-                        Allow new versions in BOM comparison.
-  -b, --bom-diff        Produce a comparison of CycloneDX BOMs.
   -c CONFIG, --config-file CONFIG
                         Import TOML configuration file.
   -x EXCLUDE [EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...]
                         Exclude field(s) from comparison.
   -p {cdxgen,cdxgen-extended}, --preset {cdxgen,cdxgen-extended}
                         Preset to use
+```
+
+bom-diff usage
+```
+usage: cjd bom-diff [-h] [-a] [-r REPORT_TEMPLATE]
 
+options:
+  -h, --help            show this help message and exit
+  -a, --allow-new-versions
+                        Allow new versions in BOM comparison.
+  -r REPORT_TEMPLATE, --report-template REPORT_TEMPLATE
+                        Jinja2 template to use for report generation.
 ```
 
 ## Specifying fields to exclude
 
 To exclude fields from comparison, use the `-x` or `--exclude` flag and specify the field name(s) 
 to exclude. The json will be flattened, so fields are specified using dot notation. For example:
 
@@ -61,14 +74,17 @@
 ```
 
 To exclude field2, you would specify `field1.field2`. To exclude the `a` field in the array of 
 objects, you would specify `field1.field3.[].a` (do NOT include the array index, just do `[]`). 
 Multiple fields may be specified separated by a space. To better understand what your fields should
 be, check out json-flatten, which is the package used for this function.
 
+>Note: In the context of BOM diffing, this list is only used for the metadata, not the components, 
+> services, or dependencies.
+
 ## Sorting
 
 custom-json-diff will sort the imported JSON alphabetically. If your JSON document contains arrays 
 of objects, you will need to specify any keys you want to sort by in a toml file or use a preset.
 The first key located from the provided keys that is present in the object will be used for sorting.
 
 ## TOML config file example
@@ -76,8 +92,9 @@
 ```toml
 [settings]
 excluded_fields = ["serialNumber", "metadata.timestamp"]
 sort_keys = ["url", "content", "ref", "name", "value"]
 
 [bom_diff]
 allow_new_versions = false
+report_template = "my_template.j2"
 ```
```

### Comparing `custom_json_diff-0.5.0/custom_json_diff/cli.py` & `custom_json_diff-0.6.0/custom_json_diff/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,35 @@
 import argparse
 
 from custom_json_diff.custom_diff import (
     compare_dicts, get_diff, perform_bom_diff, report_results
 )
+from custom_json_diff.custom_diff_classes import Options
 
 
 def build_args():
     parser = argparse.ArgumentParser()
+    parser.set_defaults(bom_diff=False, allow_new_versions=False, report_template=None)
+    subparsers = parser.add_subparsers(help="subcommand help")
+    parser_bom_diff = subparsers.add_parser("bom-diff", help="compare CycloneDX BOMs")
+    parser_bom_diff.set_defaults(bom_diff=True)
+    parser_bom_diff.add_argument(
+        "-a",
+        "--allow-new-versions",
+        action="store_true",
+        help="Allow new versions in BOM comparison.",
+        dest="allow_new_versions",
+    )
+    parser_bom_diff.add_argument(
+        "-r",
+        "--report-template",
+        action="store",
+        help="Jinja2 template to use for report generation.",
+        dest="report_template",
+    )
     parser.add_argument(
         "-i",
         "--input",
         action="store",
         help="Two JSON files to compare.",
         required=True,
         nargs=2,
@@ -19,29 +38,15 @@
     parser.add_argument(
         "-o",
         "--output",
         action="store",
         help="Export JSON of differences to this file.",
         dest="output",
     )
-    parser.add_argument(
-        "-a",
-        "--allow-new-versions",
-        action="store_true",
-        help="Allow new versions in BOM comparison.",
-        dest="allow_new_versions",
-    )
-    parser.add_argument(
-        "-b",
-        "--bom-diff",
-         action="store_true",
-         help="Produce a comparison of CycloneDX BOMs.",
-         dest="bom_diff",
-    )
-    arg_group = parser.add_mutually_exclusive_group(required=True)
+    arg_group = parser.add_mutually_exclusive_group()
     arg_group.add_argument(
         "-c",
         "--config-file",
         action="store",
         help="Import TOML configuration file.",
         dest="config"
     )
@@ -54,28 +59,39 @@
         dest="exclude",
         nargs="+",
     )
     arg_group.add_argument(
         "-p",
         "--preset",
         action="store",
-        help="Preset to use",
+        help="Preset to use.",
         choices=["cdxgen", "cdxgen-extended"],
         dest="preset",
     )
     return parser.parse_args()
 
 
 def main():
     args = build_args()
-    settings = args.preset or args.config or args.exclude
-    result, j1, j2 = compare_dicts(args.input[0], args.input[1], settings, args.bom_diff, args.allow_new_versions)
+    options = Options(
+        allow_new_versions=args.allow_new_versions,
+        bom_diff=args.bom_diff,
+        config=args.config,
+        exclude=args.exclude,
+        file_1=args.input[0],
+        file_2=args.input[1],
+        output=args.output,
+        preset=args.preset,
+        report_template=args.report_template,
+        sort_keys=[],
+    )
+    result, j1, j2 = compare_dicts(options)
 
     if args.bom_diff:
-        result_summary = perform_bom_diff(j1, j2)
+        result_summary = perform_bom_diff(j1, j2, options)
     else:
-        result_summary = get_diff(args.input[0], args.input[1], j1, j2)
-    report_results(result, result_summary, args.output)
+        result_summary = get_diff(j1, j2, options)
+    report_results(result, result_summary, options)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `custom_json_diff-0.5.0/custom_json_diff/custom_diff_classes.py` & `custom_json_diff-0.6.0/custom_json_diff/custom_diff_classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import contextlib
+import logging
 import re
+import sys
+from dataclasses import dataclass, field
 from typing import Dict, List, Set, Tuple
 
 import semver
+import toml
 from json_flatten import unflatten  # type: ignore
 
 
 class BomComponent:
     def __init__(self, comp: Dict, allow_new_versions: bool, component_type: str):
         self.version = set_version(comp.get("version", ""), allow_new_versions)
         self.search_key = create_comp_key(comp, allow_new_versions, component_type)
@@ -43,15 +47,15 @@
         self.data, self.components, self.services, self.dependencies = import_bom_dict(
             allow_new_versions, data, metadata, components, services, dependencies)
         self.filename = filename
         self.allow_new_versions = allow_new_versions
 
     def __eq__(self, other):
         return (self.data == other.data and self.components == other.components and
-                self.services == other.services)
+                self.services == other.services and self.dependencies == other.dependencies)
 
     def __ne__(self, other):
         return not self == other
 
 
 class FlatDicts:
 
@@ -92,15 +96,15 @@
         return result
 
     def intersection(self, other: "FlatDicts") -> "FlatDicts":
         """Returns the intersection of two FlatDicts as a new FlatDicts"""
         intersection = [i for i in self.data if i in other.data]
         return FlatDicts(intersection)
 
-    def filter_out_keys(self, exclude_keys: Set[str]) -> "FlatDicts":
+    def filter_out_keys(self, exclude_keys: Set[str] | List[str]) -> "FlatDicts":
         filtered_data = [i for i in self.data if check_key(i.search_key, exclude_keys)]
         self.data = filtered_data
         return self
 
 
 class FlatElement:
     def __init__(self, key, value):
@@ -108,15 +112,47 @@
         self.value = value
         self.search_key = create_search_key(key, value)
 
     def __eq__(self, other):
         return self.search_key == other.search_key
 
 
-def check_key(key: str, exclude_keys: Set[str]) -> bool:
+@dataclass
+class Options:  # type: ignore
+    allow_new_versions: bool = False
+    bom_diff: bool = False
+    config: str = ""
+    exclude: list | set = field(default_factory=set)
+    file_1: str = ""
+    file_2: str = ""
+    output: str = ""
+    preset: str = ""
+    report_template: str = ""
+    sort_keys: list = field(default_factory=list)
+
+    def __post_init__(self):
+        if self.config:
+            with open(self.config, "r", encoding="utf-8") as f:
+                try:
+                    toml_data = toml.load(f)
+                except toml.TomlDecodeError:
+                    logging.error("Invalid TOML.")
+                    sys.exit(1)
+            self.allow_new_versions = toml_data.get("bom_diff", {}).get("allow_new_versions", False)
+            self.report_template = toml_data.get("bom_diff", {}).get("report_template", "")
+            self.sort_keys = toml_data.get("settings", {}).get("sort_keys", [])
+            self.exclude = set(toml_data.get("settings", {}).get("excluded_fields", []))
+        elif self.preset:
+            self.exclude, self.sort_keys = set_excluded_fields(self.preset)
+        elif self.exclude:
+            self.exclude = set(self.exclude)
+            self.sort_keys = []
+
+
+def check_key(key: str, exclude_keys: Set[str] | List[str]) -> bool:
     return not any(key.startswith(k) for k in exclude_keys)
 
 
 def create_search_key(key: str, value: str) -> str:
     combined_key = re.sub(r"(?<=\[)[0-9]+(?=])", "", key)
     combined_key += f"|>{value}"
     return combined_key
@@ -178,12 +214,29 @@
                 services.append(BomComponent(i, allow_new_versions, "service"))
         elif key == "dependencies":
             for i in value:
                 dependencies.append(BomDependency(i, allow_new_versions, ))
     return metadata, components, services, dependencies
 
 
+def set_excluded_fields(preset: str) -> Tuple[Set[str], List[str]]:
+    excluded = []
+    sort_fields = []
+    if preset.startswith("cdxgen"):
+        excluded.extend(["metadata.timestamp", "serialNumber",
+                         "metadata.tools.components.[].version",
+                         "metadata.tools.components.[].purl",
+                         "metadata.tools.components.[].bom-ref",
+                         "components.[].properties",
+                         "components.[].evidence"
+                         ])
+        if preset == "cdxgen-extended":
+            excluded.append("components.[].licenses")
+        sort_fields.extend(["url", "content", "ref", "name", "value"])
+    return set(excluded), sort_fields
+
+
 def set_version(version: str, allow_new_versions: bool = False) -> semver.Version | str:
     with contextlib.suppress(ValueError):
         if allow_new_versions and version:
             return semver.Version.parse(version, True)
     return version
```

### Comparing `custom_json_diff-0.5.0/custom_json_diff.egg-info/PKG-INFO` & `custom_json_diff-0.6.0/custom_json_diff.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: custom-json-diff
-Version: 0.5.0
+Version: 0.6.0
 Summary: Custom JSON diffing and comparison tool.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/custom-json-diff
 Project-URL: Bug Tracker, https://github.com/appthreat/custom-json-diff/issues
+Project-URL: Funding, https://github.com/sponsors/cerrussell
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jinja2>=3.1.4
 Requires-Dist: json-flatten>=0.3
 Requires-Dist: semver>=3.0.0
 Requires-Dist: toml>=0.10
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
@@ -33,33 +35,46 @@
 
 
 
 ## Installation
 `pip install custom-json-diff`
 
 ## CLI Usage
+
 ```
-usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] [-b] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended})
+usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended}) {bom-diff} ...
+
+positional arguments:
+  {bom-diff}            subcommand help
+    bom-diff            compare CycloneDX BOMs
 
 options:
   -h, --help            show this help message and exit
   -i INPUT INPUT, --input INPUT INPUT
                         Two JSON files to compare.
   -o OUTPUT, --output OUTPUT
                         Export JSON of differences to this file.
-  -a, --allow-new-versions
-                        Allow new versions in BOM comparison.
-  -b, --bom-diff        Produce a comparison of CycloneDX BOMs.
   -c CONFIG, --config-file CONFIG
                         Import TOML configuration file.
   -x EXCLUDE [EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...]
                         Exclude field(s) from comparison.
   -p {cdxgen,cdxgen-extended}, --preset {cdxgen,cdxgen-extended}
                         Preset to use
+```
+
+bom-diff usage
+```
+usage: cjd bom-diff [-h] [-a] [-r REPORT_TEMPLATE]
 
+options:
+  -h, --help            show this help message and exit
+  -a, --allow-new-versions
+                        Allow new versions in BOM comparison.
+  -r REPORT_TEMPLATE, --report-template REPORT_TEMPLATE
+                        Jinja2 template to use for report generation.
 ```
 
 ## Specifying fields to exclude
 
 To exclude fields from comparison, use the `-x` or `--exclude` flag and specify the field name(s) 
 to exclude. The json will be flattened, so fields are specified using dot notation. For example:
 
@@ -87,14 +102,17 @@
 ```
 
 To exclude field2, you would specify `field1.field2`. To exclude the `a` field in the array of 
 objects, you would specify `field1.field3.[].a` (do NOT include the array index, just do `[]`). 
 Multiple fields may be specified separated by a space. To better understand what your fields should
 be, check out json-flatten, which is the package used for this function.
 
+>Note: In the context of BOM diffing, this list is only used for the metadata, not the components, 
+> services, or dependencies.
+
 ## Sorting
 
 custom-json-diff will sort the imported JSON alphabetically. If your JSON document contains arrays 
 of objects, you will need to specify any keys you want to sort by in a toml file or use a preset.
 The first key located from the provided keys that is present in the object will be used for sorting.
 
 ## TOML config file example
@@ -102,8 +120,9 @@
 ```toml
 [settings]
 excluded_fields = ["serialNumber", "metadata.timestamp"]
 sort_keys = ["url", "content", "ref", "name", "value"]
 
 [bom_diff]
 allow_new_versions = false
+report_template = "my_template.j2"
 ```
```

### Comparing `custom_json_diff-0.5.0/pyproject.toml` & `custom_json_diff-0.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "custom-json-diff"
-version = "0.5.0"
+version = "0.6.0"
 description = "Custom JSON diffing and comparison tool."
 authors = [
   { name = "Caroline Russell", email = "caroline@appthreat.dev" },
 ]
-dependencies = ["json-flatten>=0.3", "semver >= 3.0.0", "toml>=0.10"]
+dependencies = ["jinja2>=3.1.4", "json-flatten>=0.3", "semver>=3.0.0", "toml>=0.10"]
 license = { text = "Apache-2.0" }
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
@@ -19,14 +19,15 @@
   "Operating System :: OS Independent",
   "Topic :: Utilities",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/appthreat/custom-json-diff"
 "Bug Tracker" = "https://github.com/appthreat/custom-json-diff/issues"
+"Funding" = "https://github.com/sponsors/cerrussell"
 
 [project.scripts]
 cjd = "custom_json_diff.cli:main"
 custom-json-diff = "custom_json_diff.cli:main"
 
 [project.optional-dependencies]
 dev = [
@@ -38,9 +39,10 @@
 requires = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = [
   "custom_json_diff",
 ]
+include-package-data = true
```

### Comparing `custom_json_diff-0.5.0/test/test_bom_diff.py` & `custom_json_diff-0.6.0/test/test_bom_diff.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 import json
 
 import pytest
 
 from custom_json_diff.custom_diff import compare_dicts, load_json, perform_bom_diff
+from custom_json_diff.custom_diff_classes import Options
 
 
 @pytest.fixture
 def java_1_bom():
-    return load_json("test/sbom-java.json", False, "cdxgen", bom_diff=True)
+    options = Options(file_1="test/sbom-java.json", file_2="test/sbom-java2.json", bom_diff=True)
+    return load_json("test/sbom-java.json", options)
 
 
 @pytest.fixture
 def java_2_bom():
-    return load_json("test/sbom-java2.json", False, "cdxgen", bom_diff=True)
+    options = Options(file_1="test/sbom-java.json", file_2="test/sbom-java2.json", bom_diff=True)
+    return load_json("test/sbom-java2.json", options)
 
 
 @pytest.fixture
 def python_1_bom():
-    return load_json("test/sbom-python.json", False, "cdxgen", bom_diff=True)
+    options = Options(file_1="test/sbom-python.json", file_2="test/sbom-python2.json", bom_diff=True)
+    return load_json("test/sbom-python.json", options)
 
 
 @pytest.fixture
 def python_2_bom():
-    return load_json("test/sbom-python2.json", False, "cdxgen", bom_diff=True)
+    options = Options(file_1="test/sbom-python.json", file_2="test/sbom-python2.json", bom_diff=True)
+    return load_json("test/sbom-python2.json", options)
+
+
+@pytest.fixture
+def options_1():
+    return Options(file_1="test/sbom-java.json", file_2="test/sbom-java2.json", bom_diff=True)
+
+
+@pytest.fixture
+def options_2():
+    return Options(file_1="test/sbom-python.json", file_2="test/sbom-python2.json", bom_diff=True, allow_new_versions=True)
 
 
 @pytest.fixture
 def results():
     with open("test/test_data.json", "r", encoding="utf-8") as f:
         return json.load(f)
 
 
-def test_bom_diff(java_1_bom, java_2_bom, python_1_bom, python_2_bom, results):
-    result, j1, j2 = compare_dicts(
-        java_1_bom.filename, java_2_bom.filename, "cdxgen", True, False)
-    result_summary = perform_bom_diff(j1, j2)
+def test_bom_diff(java_1_bom, java_2_bom, python_1_bom, python_2_bom, results, options_1, options_2):
+    result, j1, j2 = compare_dicts(options_1)
+    result_summary = perform_bom_diff(j1, j2, options_1)
     assert result_summary == results["result_1"]
-    result, p1, p2 = compare_dicts(python_1_bom.filename, python_2_bom.filename, "cdxgen", True, True)
-    result_summary = perform_bom_diff(p1, p2)
+    result, p1, p2 = compare_dicts(options_2)
+    result_summary = perform_bom_diff(p1, p2, options_2)
     assert result_summary == results["result_2"]
```

