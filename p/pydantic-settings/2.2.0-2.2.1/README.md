# Comparing `tmp/pydantic_settings-2.2.0.tar.gz` & `tmp/pydantic_settings-2.2.1.tar.gz`

## Comparing `pydantic_settings-2.2.0.tar` & `pydantic_settings-2.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/Makefile
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/mkdocs.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/docs/favicon.png
--rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/docs/index.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/docs/logo-white.svg
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/docs/extra/terminal.css
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/docs/extra/tweaks.css
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/docs/theme/main.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/pydantic_settings/__init__.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/pydantic_settings/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/pydantic_settings/py.typed
--rw-r--r--   0        0        0    32193 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/pydantic_settings/sources.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/pydantic_settings/utils.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/pydantic_settings/version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/requirements/all.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/requirements/linting.in
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/requirements/linting.txt
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/requirements/pyproject.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/requirements/testing.in
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/requirements/testing.txt
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/tests/example_test_config.json
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/tests/test_docs.py
--rw-r--r--   0        0        0    67044 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/tests/test_settings.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/LICENSE
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/README.md
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pydantic_settings-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/Makefile
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/mkdocs.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/docs/favicon.png
+-rw-r--r--   0        0        0    25447 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/docs/index.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/docs/logo-white.svg
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/docs/extra/terminal.css
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/docs/extra/tweaks.css
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/docs/theme/main.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/pydantic_settings/__init__.py
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/pydantic_settings/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/pydantic_settings/py.typed
+-rw-r--r--   0        0        0    32230 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/pydantic_settings/sources.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/pydantic_settings/utils.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/pydantic_settings/version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/requirements/all.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/requirements/linting.in
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/requirements/linting.txt
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/requirements/pyproject.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/requirements/testing.in
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/requirements/testing.txt
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/tests/example_test_config.json
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/tests/test_docs.py
+-rw-r--r--   0        0        0    65467 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/tests/test_settings.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/LICENSE
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/README.md
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pydantic_settings-2.2.1/PKG-INFO
```

### Comparing `pydantic_settings-2.2.0/.pre-commit-config.yaml` & `pydantic_settings-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/Makefile` & `pydantic_settings-2.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/mkdocs.yml` & `pydantic_settings-2.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/.github/workflows/ci.yml` & `pydantic_settings-2.2.1/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     - name: test
       run: make test
       env:
         COVERAGE_FILE: .coverage.${{ runner.os }}-py${{ matrix.python }}
         CONTEXT: ${{ runner.os }}-py${{ matrix.python }}
 
     - name: uninstall deps
-      run: pip uninstall -y tomlkit PyYAML
+      run: pip uninstall -y PyYAML
 
     - name: test without deps
       run: make test
       env:
         COVERAGE_FILE: .coverage.${{ runner.os }}-py${{ matrix.python }}-without-deps
         CONTEXT: ${{ runner.os }}-py${{ matrix.python }}-without-deps
```

### Comparing `pydantic_settings-2.2.0/docs/favicon.png` & `pydantic_settings-2.2.1/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/docs/index.md` & `pydantic_settings-2.2.1/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -535,15 +535,15 @@
 docker service create --name pydantic-with-secrets --secret my_secret_data pydantic-app:latest
 ```
 
 ## Other settings source
 
 Other settings sources are available for common configuration files:
 
-- `TomlConfigSettingsSource` using `toml_file` and toml_file_encoding arguments
+- `TomlConfigSettingsSource` using `toml_file` argument
 - `YamlConfigSettingsSource` using `yaml_file` and yaml_file_encoding arguments
 - `JsonConfigSettingsSource` using `json_file` and `json_file_encoding` arguments
 
 You can also provide multiple files by providing a list of path:
 ```py
 toml_file = ['config.default.toml', 'config.custom.toml']
 ```
@@ -566,17 +566,15 @@
 class Nested(BaseModel):
     nested_field: str
 
 
 class Settings(BaseSettings):
     foobar: str
     nested: Nested
-    model_config = SettingsConfigDict(
-        toml_file='config.toml', toml_file_encoding='utf-8'
-    )
+    model_config = SettingsConfigDict(toml_file='config.toml')
 
     @classmethod
     def settings_customise_sources(
         cls,
         settings_cls: Type[BaseSettings],
         init_settings: PydanticBaseSettingsSource,
         env_settings: PydanticBaseSettingsSource,
```

### Comparing `pydantic_settings-2.2.0/docs/logo-white.svg` & `pydantic_settings-2.2.1/docs/logo-white.svg`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/docs/extra/terminal.css` & `pydantic_settings-2.2.1/docs/extra/terminal.css`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/docs/extra/tweaks.css` & `pydantic_settings-2.2.1/docs/extra/tweaks.css`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/pydantic_settings/__init__.py` & `pydantic_settings-2.2.1/pydantic_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/pydantic_settings/main.py` & `pydantic_settings-2.2.1/pydantic_settings/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     env_parse_none_str: str | None
     secrets_dir: str | Path | None
     json_file: PathType | None
     json_file_encoding: str | None
     yaml_file: PathType | None
     yaml_file_encoding: str | None
     toml_file: PathType | None
-    toml_file_encoding: str | None
 
 
 # Extend `config_keys` by pydantic settings config keys to
 # support setting config through class kwargs.
 # Pydantic uses `config_keys` in `pydantic._internal._config.ConfigWrapper.for_model`
 # to extract config keys from model kwargs, So, by adding pydantic settings keys to
 # `config_keys`, they will be considered as valid config keys and will be collected
@@ -203,11 +202,10 @@
         env_nested_delimiter=None,
         env_parse_none_str=None,
         json_file=None,
         json_file_encoding=None,
         yaml_file=None,
         yaml_file_encoding=None,
         toml_file=None,
-        toml_file_encoding=None,
         secrets_dir=None,
         protected_namespaces=('model_', 'settings_'),
     )
```

### Comparing `pydantic_settings-2.2.0/pydantic_settings/sources.py` & `pydantic_settings-2.2.1/pydantic_settings/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,60 +4,60 @@
 import os
 import sys
 import warnings
 from abc import ABC, abstractmethod
 from collections import deque
 from dataclasses import is_dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Sequence, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, List, Mapping, Sequence, Tuple, Union, cast
 
 from dotenv import dotenv_values
-from pydantic import AliasChoices, AliasPath, BaseModel, Json, TypeAdapter
+from pydantic import AliasChoices, AliasPath, BaseModel, Json
 from pydantic._internal._typing_extra import WithArgsTypes, origin_is_union
 from pydantic._internal._utils import deep_update, is_model_class, lenient_issubclass
 from pydantic.fields import FieldInfo
 from typing_extensions import get_args, get_origin
 
 from pydantic_settings.utils import path_type_label
 
 if TYPE_CHECKING:
     if sys.version_info >= (3, 11):
         import tomllib
     else:
         tomllib = None
-    import tomlkit
+    import tomli
     import yaml
 
     from pydantic_settings.main import BaseSettings
 else:
     yaml = None
     tomllib = None
-    tomlkit = None
+    tomli = None
 
 
 def import_yaml() -> None:
     global yaml
     if yaml is not None:
         return
     try:
         import yaml
     except ImportError as e:
         raise ImportError('PyYAML is not installed, run `pip install pydantic-settings[yaml]`') from e
 
 
 def import_toml() -> None:
-    global tomlkit
+    global tomli
     global tomllib
     if sys.version_info < (3, 11):
-        if tomlkit is not None:
+        if tomli is not None:
             return
         try:
-            import tomlkit
+            import tomli
         except ImportError as e:
-            raise ImportError('tomlkit is not installed, run `pip install pydantic-settings[toml]`') from e
+            raise ImportError('tomli is not installed, run `pip install pydantic-settings[toml]`') from e
     else:
         if tomllib is not None:
             return
         import tomllib
 
 
 DotenvType = Union[Path, str, List[Union[Path, str]], Tuple[Union[Path, str], ...]]
@@ -161,15 +161,15 @@
         super().__init__(settings_cls)
 
     def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
         # Nothing to do here. Only implement the return statement to make mypy happy
         return None, '', False
 
     def __call__(self) -> dict[str, Any]:
-        return TypeAdapter(Dict[str, Any]).dump_python(self.init_kwargs)
+        return self.init_kwargs
 
     def __repr__(self) -> str:
         return f'InitSettingsSource(init_kwargs={self.init_kwargs!r})'
 
 
 class PydanticBaseEnvSettingsSource(PydanticBaseSettingsSource):
     def __init__(
@@ -679,28 +679,34 @@
                     )
                 )
 
         return dotenv_vars
 
     def __call__(self) -> dict[str, Any]:
         data: dict[str, Any] = super().__call__()
+        is_extra_allowed = self.config.get('extra') != 'forbid'
 
         # As `extra` config is allowed in dotenv settings source, We have to
-        # update data with extra env variabels from dotenv file.
+        # update data with extra env variables from dotenv file.
         for env_name, env_value in self.env_vars.items():
             if not env_value:
                 continue
             env_used = False
             for field_name, field in self.settings_cls.model_fields.items():
                 for _, field_env_name, _ in self._extract_field_info(field, field_name):
                     if env_name.startswith(field_env_name):
                         env_used = True
                         break
             if not env_used:
-                data[env_name] = env_value
+                if is_extra_allowed and env_name.startswith(self.env_prefix):
+                    # env_prefix should be respected and removed from the env_name
+                    normalized_env_name = env_name[len(self.env_prefix) :]
+                    data[normalized_env_name] = env_value
+                else:
+                    data[env_name] = env_value
         return data
 
     def __repr__(self) -> str:
         return (
             f'DotEnvSettingsSource(env_file={self.env_file!r}, env_file_encoding={self.env_file_encoding!r}, '
             f'env_nested_delimiter={self.env_nested_delimiter!r}, env_prefix_len={self.env_prefix_len!r})'
         )
@@ -754,30 +760,24 @@
     A source class that loads variables from a JSON file
     """
 
     def __init__(
         self,
         settings_cls: type[BaseSettings],
         toml_file: PathType | None = DEFAULT_PATH,
-        toml_file_encoding: str | None = None,
     ):
         self.toml_file_path = toml_file if toml_file != DEFAULT_PATH else settings_cls.model_config.get('toml_file')
-        self.toml_file_encoding = (
-            toml_file_encoding
-            if toml_file_encoding is not None
-            else settings_cls.model_config.get('toml_file_encoding')
-        )
         self.toml_data = self._read_files(self.toml_file_path)
         super().__init__(settings_cls, self.toml_data)
 
     def _read_file(self, file_path: Path) -> dict[str, Any]:
         import_toml()
-        with open(file_path, mode='rb', encoding=self.toml_file_encoding) as toml_file:
+        with open(file_path, mode='rb') as toml_file:
             if sys.version_info < (3, 11):
-                return tomlkit.load(toml_file)
+                return tomli.load(toml_file)
             return tomllib.load(toml_file)
 
 
 class YamlConfigSettingsSource(InitSettingsSource, ConfigFileSourceMixin):
     """
     A source class that loads variables from a yaml file
     """
```

### Comparing `pydantic_settings-2.2.0/pydantic_settings/utils.py` & `pydantic_settings-2.2.1/pydantic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/requirements/linting.txt` & `pydantic_settings-2.2.1/requirements/linting.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --output-file=requirements/linting.txt requirements/linting.in
 #
 black==24.2.0
     # via -r requirements/linting.in
 cfgv==3.4.0
@@ -28,28 +28,34 @@
     # via black
 pathspec==0.12.1
     # via black
 platformdirs==4.2.0
     # via
     #   black
     #   virtualenv
-pre-commit==3.6.1
+pre-commit==3.5.0
     # via -r requirements/linting.in
 pyupgrade==3.15.0
     # via -r requirements/linting.in
 pyyaml==6.0.1
     # via
     #   -r requirements/linting.in
     #   pre-commit
-ruff==0.2.1
+ruff==0.2.2
     # via -r requirements/linting.in
 tokenize-rt==5.2.0
     # via pyupgrade
+tomli==2.0.1
+    # via
+    #   black
+    #   mypy
 types-pyyaml==6.0.12.12
     # via -r requirements/linting.in
 typing-extensions==4.9.0
-    # via mypy
+    # via
+    #   black
+    #   mypy
 virtualenv==20.25.0
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `pydantic_settings-2.2.0/requirements/pyproject.txt` & `pydantic_settings-2.2.1/requirements/pyproject.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     # via pydantic-settings (pyproject.toml)
 pydantic-core==2.16.2
     # via pydantic
 python-dotenv==1.0.1
     # via pydantic-settings (pyproject.toml)
 pyyaml==6.0.1
     # via pydantic-settings (pyproject.toml)
-tomlkit==0.12.3
+tomli==2.0.1
     # via pydantic-settings (pyproject.toml)
 typing-extensions==4.9.0
     # via
     #   pydantic
     #   pydantic-core
```

### Comparing `pydantic_settings-2.2.0/requirements/testing.txt` & `pydantic_settings-2.2.1/requirements/testing.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,29 +28,29 @@
     # via black
 platformdirs==4.2.0
     # via black
 pluggy==1.4.0
     # via pytest
 pygments==2.17.2
     # via rich
-pytest==8.0.0
+pytest==8.0.1
     # via
     #   -r requirements/testing.in
     #   pytest-examples
     #   pytest-mock
     #   pytest-pretty
 pytest-examples==0.0.10
     # via -r requirements/testing.in
 pytest-mock==3.12.0
     # via -r requirements/testing.in
 pytest-pretty==1.2.0
     # via -r requirements/testing.in
 rich==13.7.0
     # via pytest-pretty
-ruff==0.2.1
+ruff==0.2.2
     # via pytest-examples
 tomli==2.0.1
     # via
     #   black
     #   coverage
     #   pytest
 typing-extensions==4.9.0
```

### Comparing `pydantic_settings-2.2.0/tests/conftest.py` & `pydantic_settings-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/tests/test_docs.py` & `pydantic_settings-2.2.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/tests/test_settings.py` & `pydantic_settings-2.2.1/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 except ImportError:
     dotenv = None
 try:
     import yaml
 except ImportError:
     yaml = None
 try:
-    import tomlkit
+    import tomli
 except ImportError:
-    tomlkit = None
+    tomli = None
 
 
 class SimpleSettings(BaseSettings):
     apple: str
 
 
 class SettingWithIgnoreEmpty(BaseSettings):
@@ -643,51 +643,14 @@
     env.set('BAR', 'env setting')
 
     s = Settings(foo='123', bar='argument')
     assert s.foo == 123
     assert s.bar == 'env setting'
 
 
-def test_env_deep_override(env):
-    class DeepSubModel(BaseModel):
-        v4: str
-
-    class SubModel(BaseModel):
-        v1: str
-        v2: bytes
-        v3: int
-        deep: DeepSubModel
-
-    class Settings(BaseSettings, env_nested_delimiter='__'):
-        v0: str
-        sub_model: SubModel
-
-        @classmethod
-        def settings_customise_sources(
-            cls, settings_cls, init_settings, env_settings, dotenv_settings, file_secret_settings
-        ):
-            return env_settings, dotenv_settings, init_settings, file_secret_settings
-
-    env.set('SUB_MODEL__DEEP__V4', 'override-v4')
-
-    s_final = {'v0': '0', 'sub_model': {'v1': 'init-v1', 'v2': b'init-v2', 'v3': 3, 'deep': {'v4': 'override-v4'}}}
-
-    s = Settings(v0='0', sub_model={'v1': 'init-v1', 'v2': b'init-v2', 'v3': 3, 'deep': {'v4': 'init-v4'}})
-    assert s.model_dump() == s_final
-
-    s = Settings(v0='0', sub_model=SubModel(v1='init-v1', v2=b'init-v2', v3=3, deep=DeepSubModel(v4='init-v4')))
-    assert s.model_dump() == s_final
-
-    s = Settings(v0='0', sub_model=SubModel(v1='init-v1', v2=b'init-v2', v3=3, deep={'v4': 'init-v4'}))
-    assert s.model_dump() == s_final
-
-    s = Settings(v0='0', sub_model={'v1': 'init-v1', 'v2': b'init-v2', 'v3': 3, 'deep': DeepSubModel(v4='init-v4')})
-    assert s.model_dump() == s_final
-
-
 def test_config_file_settings_nornir(env):
     """
     See https://github.com/pydantic/pydantic/pull/341#issuecomment-450378771
     """
 
     def nornir_settings_source() -> Dict[str, Any]:
         return {'param_a': 'config a', 'param_b': 'config b', 'param_c': 'config c'}
@@ -1183,42 +1146,14 @@
         ) -> Tuple[PydanticBaseSettingsSource, ...]:
             return (YamlConfigSettingsSource(settings_cls),)
 
     with pytest.raises(ImportError, match=r'^PyYAML is not installed, run `pip install pydantic-settings\[yaml\]`$'):
         Settings()
 
 
-@pytest.mark.skipif(sys.version_info >= (3, 11) or tomlkit, reason='tomlkit/tomllib is installed')
-def test_toml_not_installed(tmp_path):
-    p = tmp_path / '.env'
-    p.write_text(
-        """
-    foobar = "Hello"
-    """
-    )
-
-    class Settings(BaseSettings):
-        foobar: str
-        model_config = SettingsConfigDict(toml_file=p)
-
-        @classmethod
-        def settings_customise_sources(
-            cls,
-            settings_cls: Type[BaseSettings],
-            init_settings: PydanticBaseSettingsSource,
-            env_settings: PydanticBaseSettingsSource,
-            dotenv_settings: PydanticBaseSettingsSource,
-            file_secret_settings: PydanticBaseSettingsSource,
-        ) -> Tuple[PydanticBaseSettingsSource, ...]:
-            return (TomlConfigSettingsSource(settings_cls),)
-
-    with pytest.raises(ImportError, match=r'^tomlkit is not installed, run `pip install pydantic-settings\[toml\]`$'):
-        Settings()
-
-
 def test_alias_set(env):
     class Settings(BaseSettings):
         foo: str = Field('default foo', validation_alias='foo_env')
         bar: str = 'bar default'
 
     assert Settings.model_fields['bar'].alias is None
     assert Settings.model_fields['bar'].validation_alias is None
@@ -2155,15 +2090,15 @@
         ) -> Tuple[PydanticBaseSettingsSource, ...]:
             return (YamlConfigSettingsSource(settings_cls),)
 
     s = Settings()
     assert s.model_dump() == {}
 
 
-@pytest.mark.skipif(sys.version_info <= (3, 11) and tomlkit is None, reason='tomlkit/tomllib is not installed')
+@pytest.mark.skipif(sys.version_info <= (3, 11) and tomli is None, reason='tomli/tomllib is not installed')
 def test_toml_file(tmp_path):
     p = tmp_path / '.env'
     p.write_text(
         """
     foobar = "Hello"
 
     [nested]
@@ -2191,15 +2126,15 @@
             return (TomlConfigSettingsSource(settings_cls),)
 
     s = Settings()
     assert s.foobar == 'Hello'
     assert s.nested.nested_field == 'world!'
 
 
-@pytest.mark.skipif(sys.version_info <= (3, 11) and tomlkit is None, reason='tomlkit/tomllib is not installed')
+@pytest.mark.skipif(sys.version_info <= (3, 11) and tomli is None, reason='tomli/tomllib is not installed')
 def test_toml_no_file():
     class Settings(BaseSettings):
         model_config = SettingsConfigDict(toml_file=None)
 
         @classmethod
         def settings_customise_sources(
             cls,
@@ -2211,15 +2146,15 @@
         ) -> Tuple[PydanticBaseSettingsSource, ...]:
             return (TomlConfigSettingsSource(settings_cls),)
 
     s = Settings()
     assert s.model_dump() == {}
 
 
-@pytest.mark.skipif(sys.version_info <= (3, 11) and tomlkit is None, reason='tomlkit/tomllib is not installed')
+@pytest.mark.skipif(sys.version_info <= (3, 11) and tomli is None, reason='tomli/tomllib is not installed')
 def test_multiple_file_toml(tmp_path):
     p1 = tmp_path / '.env.toml1'
     p2 = tmp_path / '.env.toml2'
     p1.write_text(
         """
     toml1=1
     """
@@ -2350,7 +2285,31 @@
 
         foo: str = ''
         bar_alias: str = Field('', alias='xxx__bar')
         nested_alias: NestedSettings = Field(default_factory=NestedSettings, alias='xxx__nested')
 
     s = Settings()
     assert s.model_dump() == {'foo': '', 'bar_alias': '0', 'nested_alias': {'a': '1', 'b': '2'}}
+
+
+def test_dotenv_with_extra_and_env_prefix(tmp_path):
+    p = tmp_path / '.env'
+    p.write_text('xxx__foo=1\nxxx__extra_var=extra_value')
+
+    class Settings(BaseSettings):
+        model_config = SettingsConfigDict(extra='allow', env_file=p, env_prefix='xxx__')
+
+        foo: str = ''
+
+    s = Settings()
+    assert s.model_dump() == {'foo': '1', 'extra_var': 'extra_value'}
+
+
+def test_nested_field_with_alias_init_source():
+    class NestedSettings(BaseModel):
+        foo: str = Field(alias='fooAlias')
+
+    class Settings(BaseSettings):
+        nested_foo: NestedSettings
+
+    s = Settings(nested_foo=NestedSettings(fooAlias='EXAMPLE'))
+    assert s.model_dump() == {'nested_foo': {'foo': 'EXAMPLE'}}
```

### Comparing `pydantic_settings-2.2.0/LICENSE` & `pydantic_settings-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/README.md` & `pydantic_settings-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.2.0/pyproject.toml` & `pydantic_settings-2.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     'pydantic>=2.3.0',
     'python-dotenv>=0.21.0',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 yaml = ["pyyaml>=6.0.1"]
-toml = ["tomlkit>=0.12"]
+toml = ["tomli>=2.0.1"]
 
 [project.urls]
 Homepage = 'https://github.com/pydantic/pydantic-settings'
 Funding = 'https://github.com/sponsors/samuelcolvin'
 Source = 'https://github.com/pydantic/pydantic-settings'
 Changelog = 'https://github.com/pydantic/pydantic-settings/releases'
 Documentation = 'https://docs.pydantic.dev/dev-v2/concepts/pydantic_settings/'
```

### Comparing `pydantic_settings-2.2.0/PKG-INFO` & `pydantic_settings-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-settings
-Version: 2.2.0
+Version: 2.2.1
 Summary: Settings management using Pydantic
 Project-URL: Homepage, https://github.com/pydantic/pydantic-settings
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic-settings
 Project-URL: Changelog, https://github.com/pydantic/pydantic-settings/releases
 Project-URL: Documentation, https://docs.pydantic.dev/dev-v2/concepts/pydantic_settings/
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>
@@ -31,15 +31,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: pydantic>=2.3.0
 Requires-Dist: python-dotenv>=0.21.0
 Provides-Extra: toml
-Requires-Dist: tomlkit>=0.12; extra == 'toml'
+Requires-Dist: tomli>=2.0.1; extra == 'toml'
 Provides-Extra: yaml
 Requires-Dist: pyyaml>=6.0.1; extra == 'yaml'
 Description-Content-Type: text/markdown
 
 # pydantic-settings
 
 [![CI](https://github.com/pydantic/pydantic-settings/workflows/CI/badge.svg?event=push)](https://github.com/pydantic/pydantic-settings/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
```

