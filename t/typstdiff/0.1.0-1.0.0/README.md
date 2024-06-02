# Comparing `tmp/typstdiff-0.1.0.tar.gz` & `tmp/typstdiff-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typstdiff-0.1.0.tar", max compression
+gzip compressed data, was "typstdiff-1.0.0.tar", max compression
```

## Comparing `typstdiff-0.1.0.tar` & `typstdiff-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0      830 2024-03-31 22:14:47.982505 typstdiff-0.1.0/README.md
--rw-r--r--   0        0        0      539 2024-03-31 22:12:15.165207 typstdiff-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-31 22:04:06.677265 typstdiff-0.1.0/typstdiff/__init__.py
--rw-r--r--   0        0        0       78 2024-03-31 22:23:43.074862 typstdiff-0.1.0/typstdiff/main.py
--rw-r--r--   0        0        0     1522 2024-03-31 22:46:09.859656 typstdiff-0.1.0/setup.py
--rw-r--r--   0        0        0     1253 2024-03-31 22:46:09.859817 typstdiff-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      880 2024-06-01 13:35:33.225805 typstdiff-1.0.0/README.md
+-rw-r--r--   0        0        0      648 2024-06-02 22:36:42.797230 typstdiff-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-01 12:49:05.845749 typstdiff-1.0.0/typstdiff/__init__.py
+-rw-r--r--   0        0        0    20825 2024-06-01 13:01:49.741765 typstdiff-1.0.0/typstdiff/comparison.py
+-rw-r--r--   0        0        0      818 2024-06-01 12:49:05.845749 typstdiff-1.0.0/typstdiff/errors.py
+-rw-r--r--   0        0        0     2203 2024-06-01 12:49:05.845749 typstdiff-1.0.0/typstdiff/file_converter.py
+-rwxr-xr-x   0        0        0     7430 2024-06-01 20:16:31.670280 typstdiff-1.0.0/typstdiff/main.py
+-rw-r--r--   0        0        0     1691 2024-06-02 22:36:47.102541 typstdiff-1.0.0/setup.py
+-rw-r--r--   0        0        0     1344 2024-06-02 22:36:47.102825 typstdiff-1.0.0/PKG-INFO
```

### Comparing `typstdiff-0.1.0/pyproject.toml` & `typstdiff-1.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [tool.poetry]
 name = "typstdiff"
-version = "0.1.0"
+version = "1.0.0"
 description = "Tool made with Pandoc to compare two files with typst extension."
 authors = ["Sara Fojt <01169167@pw.edu.pl>", "Dominika Ferfecka", "Małgorzata Kozłowska"]
 readme = "README.md"
 packages = [{include = "typstdiff"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandoc = "^2.3"
 typst = "^0.11.0"
+jsondiff = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
+pytest = ">=8.2.0,<9.0.0"
 black = "^24.3.0"
 flake8 = "^7.0.0"
+tox = "^4.14.2"
+mkdocs = "^1.5.3"
+
+[tool.poetry.scripts]
+typstdiff = "main:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typstdiff-0.1.0/setup.py` & `typstdiff-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 packages = \
 ['typstdiff']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandoc>=2.3,<3.0', 'typst>=0.11.0,<0.12.0']
+['jsondiff>=2.0.0,<3.0.0', 'pandoc>=2.3,<3.0', 'typst>=0.11.0,<0.12.0']
+
+entry_points = \
+{'console_scripts': ['typstdiff = main:main']}
 
 setup_kwargs = {
     'name': 'typstdiff',
-    'version': '0.1.0',
+    'version': '1.0.0',
     'description': 'Tool made with Pandoc to compare two files with typst extension.',
-    'long_description': '# TypstDiff\n### Dominika Ferfecka, Sara Fojt, Małgorzata Kozłowska\n\n## Introduction\nTool created with Pandoc to compare two typst files. It marks things\ndeleted from first file and marks differently things added to the second file.\n\n## Run virtual environment\nTo run virtual environment in poetry go to TypstDiff folder and use command\n`poetry shell`\n\nTo exit virtual environment use command\n`exit`\n\n## Installing dependencies\nTo install the same versions of dependencies as used in the project you can use \n`pip install -e .` or `poetry install`\n\n## Run tests\nTo run tests use command\n`poetry run pytest -v`\n\n### Issues\nAs both tools - Pandoc and Typst are new and still developing there is no full support\nfor typst in Pandoc. Because of that it is not possible to notice all changes made\nin files, but tool will be developed.',
+    'long_description': '# TypstDiff\n### Dominika Ferfecka, Sara Fojt, Małgorzata Kozłowska\n\n## Introduction\nTool created with Pandoc to compare two typst files. It marks things\ndeleted from first file and marks differently things added to the second file.\n\n## Run documentation\nAll information about tool, its working process and how to use it is located\nin documentation written in mkdocs. To run documentation server use command\n`mkdocs serve` \nin the folder `documentation`.\nIf mkdocs is not installed use command `pip install mkdocs` or run virtual environment\n`poetry shell` and install all dependencies with `poetry install` (poetry can be installed\nwith `pip install poetry`)\n\n### Issues\nAs both tools - Pandoc and Typst are new and still developing there is no full support\nfor typst in Pandoc. Because of that it is not possible to notice all changes made\nin files, but tool will be developed.',
     'author': 'Sara Fojt',
     'author_email': '01169167@pw.edu.pl',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `typstdiff-0.1.0/PKG-INFO` & `typstdiff-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 Metadata-Version: 2.1
 Name: typstdiff
-Version: 0.1.0
+Version: 1.0.0
 Summary: Tool made with Pandoc to compare two files with typst extension.
 Author: Sara Fojt
 Author-email: 01169167@pw.edu.pl
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: jsondiff (>=2.0.0,<3.0.0)
 Requires-Dist: pandoc (>=2.3,<3.0)
 Requires-Dist: typst (>=0.11.0,<0.12.0)
 Description-Content-Type: text/markdown
 
 # TypstDiff
 ### Dominika Ferfecka, Sara Fojt, Małgorzata Kozłowska
 
 ## Introduction
 Tool created with Pandoc to compare two typst files. It marks things
 deleted from first file and marks differently things added to the second file.
 
-## Run virtual environment
-To run virtual environment in poetry go to TypstDiff folder and use command
-`poetry shell`
-
-To exit virtual environment use command
-`exit`
-
-## Installing dependencies
-To install the same versions of dependencies as used in the project you can use 
-`pip install -e .` or `poetry install`
-
-## Run tests
-To run tests use command
-`poetry run pytest -v`
+## Run documentation
+All information about tool, its working process and how to use it is located
+in documentation written in mkdocs. To run documentation server use command
+`mkdocs serve` 
+in the folder `documentation`.
+If mkdocs is not installed use command `pip install mkdocs` or run virtual environment
+`poetry shell` and install all dependencies with `poetry install` (poetry can be installed
+with `pip install poetry`)
 
 ### Issues
 As both tools - Pandoc and Typst are new and still developing there is no full support
 for typst in Pandoc. Because of that it is not possible to notice all changes made
 in files, but tool will be developed.
```

