# Comparing `tmp/edne_correios_loader-0.1.2.tar.gz` & `tmp/edne_correios_loader-0.1.3.tar.gz`

## Comparing `edne_correios_loader-0.1.2.tar` & `edne_correios_loader-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/HISTORY.md
--rw-r--r--   0        0        0    13600 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/README-en.md
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/.github/workflows/coverage-report.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/__about__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/__init__.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/cep_querier.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/dbwriter.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/exc.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/loader.py
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/resolver.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/table_set.py
--rw-r--r--   0        0        0    15471 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/tables.py
--rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/unified_table.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/cli/__init__.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/src/edne_correios_loader/cli/logger.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/README.md
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/HISTORY.md
+-rw-r--r--   0        0        0    13600 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/README-en.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/.github/workflows/coverage-report.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/__about__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/__init__.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/cep_querier.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/dbwriter.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/exc.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/loader.py
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/resolver.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/table_set.py
+-rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/tables.py
+-rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/unified_table.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/cli/__init__.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/src/edne_correios_loader/cli/logger.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/README.md
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 edne_correios_loader-0.1.3/PKG-INFO
```

### Comparing `edne_correios_loader-0.1.2/README-en.md` & `edne_correios_loader-0.1.3/README-en.md`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/.github/workflows/coverage-report.yml` & `edne_correios_loader-0.1.3/.github/workflows/coverage-report.yml`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/.github/workflows/lint-and-test.yml` & `edne_correios_loader-0.1.3/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/.github/workflows/publish.yml` & `edne_correios_loader-0.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/cep_querier.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/cep_querier.py`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/dbwriter.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/dbwriter.py`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/loader.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/loader.py`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/resolver.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/resolver.py`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/table_set.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/table_set.py`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/tables.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         "loc_in_tipo_loc",
         Enum(TipoLocalidadeEnum, values_callable=lambda x: [e.value for e in x]),
         comment="Tipo de localidade",
         nullable=False,
     ),
     Column(
         "loc_nu_sub",
-        ForeignKey("log_localidade.loc_nu", ondelete="CASCADE"),
+        ForeignKey("log_localidade.loc_nu", ondelete="NO ACTION"),
         index=True,
         comment="Chave da localidade de subordinação",
     ),
     Column("loc_no_abrev", String(36), comment="Abreviatura do nome da localidade"),
     Column("mun_nu", Integer, comment="Código do município IBGE"),
 )
```

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/unified_table.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/unified_table.py`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/cli/__init__.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 
 class DneLoaderWithProgress(DneLoader):
     DneResolver = DneResolverWithDownloadProgress
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.version_option(version=__version__, prog_name="DNE Correios Loader")
-def edne_correios_loader():
-    ...  # pragma: no cover
+def edne_correios_loader(): ...  # pragma: no cover
 
 
 @edne_correios_loader.command()
 @click.option(
     "-s",
     "--dne-source",
     help="Path or URL with the DNE file/dir to be imported",
```

### Comparing `edne_correios_loader-0.1.2/src/edne_correios_loader/cli/logger.py` & `edne_correios_loader-0.1.3/src/edne_correios_loader/cli/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             msg = self.format(record)
             is_error = record.levelname.upper() in [
                 "WARNING",
                 "ERROR",
                 "CRITICAL",
             ]
             click.echo(msg, err=is_error)
-        except Exception:  # noqa: no cover
+        except Exception:
             self.handleError(record)
 
 
 _default_handler = ClickHandler()
 _default_handler.formatter = ColorFormatter()
```

### Comparing `edne_correios_loader-0.1.2/.gitignore` & `edne_correios_loader-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/LICENSE.txt` & `edne_correios_loader-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/README.md` & `edne_correios_loader-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `edne_correios_loader-0.1.2/pyproject.toml` & `edne_correios_loader-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -87,19 +87,19 @@
     detached = true
     dependencies = [
         "black>=23.1.0",
         "ruff>=0.0.243",
     ]
     [tool.hatch.envs.lint.scripts]
         style = [
-            "ruff {args:.}",
-            "black --check --diff {args:.}",
+            "ruff check {args:.}",
+            "ruff format --diff {args:.}",
         ]
         fmt = [
-            "black {args:.}",
+            "ruff format {args:.}",
             "ruff --fix {args:.}",
             "style",
         ]
         all = [
             "style",
         ]
 
@@ -107,83 +107,84 @@
     target-version = ["py38"]
     line-length = 88
 
 [tool.ruff]
     target-version = "py38"
     line-length = 88
     src = ["src", "tests"]
-    select = [
-        "A",
-        "ARG",
-        "B",
-        "B9",
-        "C",
-        "C4",
-        "DTZ",
-        "E", # pycodestyle errors (https://docs.astral.sh/ruff/rules/#error-e)
-        "EM",
-        "F", # pyflakes (https://docs.astral.sh/ruff/rules/#pyflakes-f)
-        "FBT",
-        "G",
-        "I", # isort (https://docs.astral.sh/ruff/rules/#isort-i)
-        "ICN",
-        "ISC",
-        "N", # pep8-naming (https://docs.astral.sh/ruff/rules/#pep8-naming-n)
-        "PIE",
-        "PLC",
-        "PLE",
-        "PLR",
-        "PLW",
-        "PTH",
-        "Q",
-        "RET",
-        "RUF",
-        "S", # flake8-bandit (https://docs.astral.sh/ruff/rules/#flake8-bandit-s)
-        "SIM",
-        "T",
-        "T10",
-        "T20",
-        "TID",
-        "TRY",
-        "UP", # pyupgrade (https://docs.astral.sh/ruff/rules/#pyupgrade-up)
-        "W", # pycodestyle warnings (https://docs.astral.sh/ruff/rules/#warning-w)
-        "YTT" # flake8-2020 (https://docs.astral.sh/ruff/rules/#flake8-2020-ytt)
-    ]
-    ignore = [
-        # Allow non-abstract empty methods in abstract base classes
-        "B027",
-        # Allow multi-line imports
-        "E401",
-        # Allow boolean positional values in function calls, like `dict.get(... True)`
-        "FBT003",
-        # Ignore checks for possible passwords
-        "S105", "S106", "S107",
-        # Allow nested context manager as they are easier to read
-        "SIM117",
-        # Ignore complexity
-        "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
-        # Allow relative imports
-        "TID252",
-    ]
-    unfixable = [
-        # Don't touch unused imports
-        "F401",
-        # Don't touch unused variables
-        "F841",
-        # Don't touch unused function arguments
-        "ARG001"
-    ]
 
-    [tool.ruff.isort]
+    [tool.ruff.lint]
+        select = [
+            "A",
+            "ARG",
+            "B",
+            "B9",
+            "C",
+            "C4",
+            "DTZ",
+            "E", # pycodestyle errors (https://docs.astral.sh/ruff/rules/#error-e)
+            "EM",
+            "F", # pyflakes (https://docs.astral.sh/ruff/rules/#pyflakes-f)
+            "FBT",
+            "G",
+            "I", # isort (https://docs.astral.sh/ruff/rules/#isort-i)
+            "ICN",
+            "N", # pep8-naming (https://docs.astral.sh/ruff/rules/#pep8-naming-n)
+            "PIE",
+            "PLC",
+            "PLE",
+            "PLR",
+            "PLW",
+            "PTH",
+            "Q",
+            "RET",
+            "RUF",
+            "S", # flake8-bandit (https://docs.astral.sh/ruff/rules/#flake8-bandit-s)
+            "SIM",
+            "T",
+            "T10",
+            "T20",
+            "TID",
+            "TRY",
+            "UP", # pyupgrade (https://docs.astral.sh/ruff/rules/#pyupgrade-up)
+            "W", # pycodestyle warnings (https://docs.astral.sh/ruff/rules/#warning-w)
+            "YTT" # flake8-2020 (https://docs.astral.sh/ruff/rules/#flake8-2020-ytt)
+        ]
+        ignore = [
+            # Allow non-abstract empty methods in abstract base classes
+            "B027",
+            # Allow multi-line imports
+            "E401",
+            # Allow boolean positional values in function calls, like `dict.get(... True)`
+            "FBT003",
+            # Ignore checks for possible passwords
+            "S105", "S106", "S107",
+            # Allow nested context manager as they are easier to read
+            "SIM117",
+            # Ignore complexity
+            "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+            # Allow relative imports
+            "TID252",
+        ]
+        unfixable = [
+            # Don't touch unused imports
+            "F401",
+            # Don't touch unused variables
+            "F841",
+            # Don't touch unused function arguments
+            "ARG001"
+        ]
+
+    [tool.ruff.lint.isort]
         known-first-party = ["edne_correios_loader"]
 
-    [tool.ruff.flake8-tidy-imports]
+    [tool.ruff.lint.flake8-tidy-imports]
         ban-relative-imports = "all"
 
-    [tool.ruff.per-file-ignores]
+    [tool.ruff.lint.per-file-ignores]
         # Tests can use
         "tests/**/*" = [
             # magic values
             "PLR2004",
             # assertions
             "S101",
             # relative imports
```

### Comparing `edne_correios_loader-0.1.2/PKG-INFO` & `edne_correios_loader-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: edne-correios-loader
-Version: 0.1.2
+Version: 0.1.3
 Summary: Load Brazilian Correios' e-DNE Basico text files into your database to enable CEP search
 Project-URL: Documentation, https://github.com/cauethenorio/edne-correios-loader#readme
 Project-URL: Issues, https://github.com/cauethenorio/edne-correios-loader/issues
 Project-URL: Source, https://github.com/cauethenorio/edne-correios-loader
 Author-email: Cauê Thenório <caue@thenorio.com.br>
 License-Expression: MIT
 License-File: LICENSE.txt
```

