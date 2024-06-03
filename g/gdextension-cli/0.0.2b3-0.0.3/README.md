# Comparing `tmp/gdextension_cli-0.0.2b3.tar.gz` & `tmp/gdextension_cli-0.0.3.tar.gz`

## Comparing `gdextension_cli-0.0.2b3.tar` & `gdextension_cli-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.pylintrc
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/requirements-publish.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/requirements.txt
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/.gitignore
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/gdextension-cli.iml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/vcs.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/main.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/__version__.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/command_line_args.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/template_renderer.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/commands/new_project_from_git.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/commands/new_project_from_local.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/tests/test_command_line_arguments.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/tests/test_template_renderer.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/LICENSE
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/README.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/pyproject.toml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/PKG-INFO
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.pylintrc
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/requirements-publish.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/gdextension-cli.iml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/main.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/release.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/gdextension_cli/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/gdextension_cli/__version__.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/gdextension_cli/command_line_args.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/gdextension_cli/git.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/gdextension_cli/template_renderer.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/gdextension_cli/commands/new_project_from_git.py
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/src/gdextension_cli/commands/new_project_from_local.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/tests/test_command_line_arguments.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/tests/test_template_renderer.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 gdextension_cli-0.0.3/PKG-INFO
```

### Comparing `gdextension_cli-0.0.2b3/.pylintrc` & `gdextension_cli-0.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/.github/workflows/lint-and-test.yml` & `gdextension_cli-0.0.3/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/.github/workflows/publish.yml` & `gdextension_cli-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/.idea/gdextension-cli.iml` & `gdextension_cli-0.0.3/.idea/gdextension-cli.iml`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/.idea/inspectionProfiles/Project_Default.xml` & `gdextension_cli-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/src/gdextension_cli/__init__.py` & `gdextension_cli-0.0.3/src/gdextension_cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,14 @@
                 NewProjectFromLocalCommand.from_arguments(args).run()
             elif args.from_git:
                 NewProjectFromGitCommand.from_arguments(args).run()
             else:
                 raise AssertionError(
                     "Expected arguments '--from-local' or '--from-git'"
                 )
-        case "build":
-            print("BUILD")
         case _:
             command_line.print_help()
 
 
 def initialize_logging(verbose: bool):
     """
     Initializes the logging module with a log level based on the given verbose argument.
```

### Comparing `gdextension_cli-0.0.2b3/src/gdextension_cli/command_line_args.py` & `gdextension_cli-0.0.3/src/gdextension_cli/command_line_args.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,33 +19,38 @@
     )
 
     HELP_REPOSITORY_URL = (
         "URL of a project template repository. "
         "Default is https://github.com/3LK3/gdextension-template.git"
     )
 
+    HELP_TEMPLATE_VERSION = (
+        "Branch name in template repository. "
+        "ONLY valid in combination with --from-git. Default: 4.2"
+    )
+
+    HELP_GODOT_VERSION = (
+        "Godot version (branch name in godot-cpp repository)."
+        "Use master for latest version. Default: 4.2"
+    )
+
     def __init__(self):
         self._parser = argparse.ArgumentParser(prog="gdextension-cli")
         self._subcommands = self._parser.add_subparsers(dest="subcommand")
         self._parser.add_argument(
             "-v", "--version", action="version", version=__version__
         )
 
     def create(self):
         """Created all subcommands and arguments"""
         self._create_command_new()
-        self._create_command_build()
+        # self._create_command_build()
         self._subcommands.add_parser("help", help="Shows this help")
         return self
 
-    def _create_command_build(self):
-        """Creates the parser for the build project command"""
-        build_parser = self._subcommands.add_parser("build", help="Build a project")
-        build_parser.add_argument("path", type=str, help="Path of the project to build")
-
     def _create_command_new(self):
         """Creates the parser for the new project command"""
         new_parser = self._subcommands.add_parser("new", help="Create a new project")
         new_parser.add_argument(
             "-v", "--verbose", action="store_true", help="More output!"
         )
         new_parser.add_argument("name", type=str, help="Name of the new project")
@@ -57,15 +62,22 @@
             help=self.HELP_OUTPUT_PATH,
         )
         new_parser.add_argument(
             "-g",
             "--godot-version",
             type=str,
             default="4.2",
-            help="Godot version and branch name for template repositories",
+            help=self.HELP_GODOT_VERSION,
+        )
+        new_parser.add_argument(
+            "-t",
+            "--template-version",
+            type=str,
+            default="4.2",
+            help=self.HELP_TEMPLATE_VERSION,
         )
 
         from_group = new_parser.add_mutually_exclusive_group(required=False)
         from_group.add_argument(
             "--from-git",
             metavar="GIT_URL",
             type=str,
```

### Comparing `gdextension_cli-0.0.2b3/src/gdextension_cli/template_renderer.py` & `gdextension_cli-0.0.3/src/gdextension_cli/template_renderer.py`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/src/gdextension_cli/commands/new_project_from_git.py` & `gdextension_cli-0.0.3/src/gdextension_cli/commands/new_project_from_git.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,70 +3,69 @@
 """
 
 import tempfile
 import logging
 from argparse import Namespace
 from pathlib import Path
 
-from git import Repo
-
 from gdextension_cli.commands.new_project_from_local import NewProjectFromLocalCommand
+from gdextension_cli.git import Repository
 
 
 class NewProjectFromGitCommand:
     """Command that creates a new project from a git repository."""
 
     def __init__(
         self,
         project_name: str,
         project_path: Path,
         godot_version: str,
-        template_repository_url: str,
     ):
         """
         Initializes the command.
         :param project_name: Name of the project.
         :param project_path: Path to the project.
         :param godot_version: Version of godot.
-        :param template_repository_url: URL of the template repository.
         """
         self.project_name = project_name
         self.project_path = project_path
         self.godot_version = godot_version
-        self.template_repository_url = template_repository_url
+        self.template_repository_url = None
+        self.template_version = None
 
     @staticmethod
     def from_arguments(args: Namespace) -> "NewProjectFromGitCommand":
         """
         Initializes the command from command line arguments.
         :param args: Command line arguments.
         :return: The created NewProjectFromGitCommand.
         """
-        return NewProjectFromGitCommand(
+        command = NewProjectFromGitCommand(
             args.name,
             args.output_path if args.output_path else Path.cwd() / args.name,
             args.godot_version,
-            args.from_git,
         )
+        command.template_repository_url = args.from_git
+        command.template_version = args.template_version
+        return command
 
     def run(self):
         """Runs the command to create a new project from a git repository."""
         logging.info("Creating new project '%s'", self.project_name)
         logging.info("Project path: %s", self.project_path)
         logging.info("Godot version: %s", self.godot_version)
         logging.info("Template repository: %s", self.template_repository_url)
+        logging.info("Template version: %s", self.template_version)
+        logging.info("########################################")
 
         with tempfile.TemporaryDirectory() as temp_dir:
-            logging.debug(
-                "Using temp directory to clone project template: %s", temp_dir
-            )
             logging.info("Cloning template repository to %s", temp_dir)
-            repo = Repo.clone_from(self.template_repository_url, temp_dir)
-            new_project = NewProjectFromLocalCommand(
+            Repository(temp_dir).clone(
+                self.template_repository_url, self.template_version
+            )
+
+            NewProjectFromLocalCommand(
                 self.project_name,
                 self.project_path,
                 self.godot_version,
-                Path(repo.working_dir),
-            )
-            new_project.check_directories()
-            new_project.copy_non_template_files()
-            new_project.render_template_files()
+                temp_dir,
+            ).run_processes()
```

### Comparing `gdextension_cli-0.0.2b3/src/gdextension_cli/commands/new_project_from_local.py` & `gdextension_cli-0.0.3/src/gdextension_cli/commands/new_project_from_local.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,40 +4,43 @@
 
 import glob
 import logging
 import shutil
 from argparse import Namespace
 from pathlib import Path
 
+from gdextension_cli.git import Repository
 from gdextension_cli.template_renderer import TemplateRenderer
 
 
 class NewProjectFromLocalCommand:
     """Command that creates a new project from a local directory."""
 
     TEMPLATE_FILE_EXTENSION = ".tmpl"
+    GODOT_CPP_URL = "https://github.com/godotengine/godot-cpp"
+    IGNORED_DIRECTORIES = ["godot-cpp", "godot_cpp"]
 
     def __init__(
         self,
         project_name: str,
         project_path: Path,
         godot_version: str,
-        template_path: Path,
+        template_path: Path | str,
     ):
         """
         Initializes the command.
         :param project_name: Name of the project.
         :param project_path: Path to the project.
         :param godot_version: Version of godot.
         :param template_path: Path to the template directory.
         """
         self.project_name = project_name
         self.project_path = project_path
         self.godot_version = godot_version
-        self.template_path = template_path
+        self.template_path = Path(template_path)
 
     @staticmethod
     def from_arguments(args: Namespace) -> "NewProjectFromLocalCommand":
         """
         Initializes the command from command line arguments.
         :param args: Command line arguments.
         :return: The created NewProjectFromLocalCommand.
@@ -46,49 +49,116 @@
             args.name,
             args.output_path if args.output_path else Path.cwd() / args.name,
             args.godot_version,
             args.from_local,
         )
 
     def run(self):
-        """Runs the command to create a new project from a local template directory."""
+        """
+        Runs the command to create a new project from a local template directory.
+        """
         logging.info("Creating new project '%s'", self.project_name)
         logging.info("Project path: %s", self.project_path)
         logging.info("Godot version: %s", self.godot_version)
         logging.info("Template path: %s", self.template_path)
 
-        self.check_directories()
-        self.copy_non_template_files()
-        self.render_template_files()
+        self.run_processes()
+
+    def run_processes(self):
+        """
+        Runs the main logic of creating a new project.
+         - checks for template and project directories
+         - creates a git repository in the project directory
+         - copies files and renders templates to the project directory
+         - adds godot-cpp as a submodule the projects git repository
+        """
+        self._check_directories()
+
+        project_repo = Repository(self.project_path)
+        project_repo.init()
+
+        self._copy_non_template_files()
+        self._render_template_files()
+
+        logging.info("Adding submodule godot-cpp from %s", self.GODOT_CPP_URL)
+        project_repo.add_submodule(self.GODOT_CPP_URL, self.godot_version)
+
+    def get_template_data(self) -> dict[str, str]:
+        """
+        Returns a dictionary containing the data used for templating.
+        :return: Dictionary containing the data
+        """
+        return {
+            "name": self.project_name,
+            "lib_name": self.project_name.lower().replace("_", ""),
+            "class_name": self._get_class_name(),
+        }
+
+    def _check_directories(self):
+        """
+        Checks for project and template directories.
+        Creates project directory if it doesn't exist.
+        """
+        if not self.template_path.exists():
+            raise FileNotFoundError(f"Template path not found: {self.template_path}")
+        if not self.project_path.exists():
+            logging.debug("Creating project directory at %s", self.project_path)
+            self.project_path.mkdir(parents=True)
+
+    def _copy_file(self, file: Path | str):
+        """
+        Copies the given relative file from template path to the corresponding new project.
+        :param file: The relative file path.
+        """
+        source_file = self.template_path / file
+        if source_file.is_dir():
+            return
+
+        target_file = self.project_path / file
+        if not target_file.parent.exists():
+            logging.debug("Creating directory at %s", target_file.parent)
+            target_file.parent.mkdir(parents=True)
 
-    def copy_non_template_files(self):
+        logging.info("Copy file %s to %s", file, target_file)
+        shutil.copy(source_file, target_file)
+
+    def _copy_non_template_files(self):
         """
         Copies all non template files from template_path to project_path.
         Non template files are all file without the extension '.tmpl'.
         """
         logging.info("Copying non template files ...")
-        non_template_files = glob.glob(
-            f"**/*[!{self.TEMPLATE_FILE_EXTENSION}]",
-            root_dir=self.template_path,
-            recursive=True,
-        )
+        non_template_files = self._get_non_template_files()
 
         for file in non_template_files:
-            source_file = self.template_path / file
-            if source_file.is_dir():
+            if self._should_ignore(file):
                 continue
+            self._copy_file(file)
 
-            target_file = self.project_path / file
-            if not target_file.parent.exists():
-                logging.debug("Creating directory at %s", target_file.parent)
-                target_file.parent.mkdir(parents=True)
-            logging.info("Copy file %s to %s", file, target_file)
-            shutil.copy(source_file, target_file)
+        self._copy_file(".gitignore")
+
+    def _get_class_name(self) -> str:
+        class_name = ""
+        for part in self.project_name.lower().split("_"):
+            class_name += part.capitalize()
+        return class_name
+
+    def _get_non_template_files(self) -> list[str]:
+        """
+        Returns a list of all non-template files.
+        :return: All non-template files.
+        """
+        files = glob.glob(
+            "**/*",
+            root_dir=self.template_path,
+            recursive=True,
+        )
+        return [file for file in files if not file.endswith(self.TEMPLATE_FILE_EXTENSION)]
 
-    def render_template_files(self):
+    def _render_template_files(self):
         """
         Renders all template files from template_path to project_path.
         Template files are all files with the extension '.tmpl'.
         """
         logging.info("Copying template files ...")
         template_files = glob.glob(
             f"**/*{self.TEMPLATE_FILE_EXTENSION}",
@@ -111,34 +181,18 @@
             if not target_file.parent.exists():
                 logging.debug("Creating directory at %s", target_file.parent)
                 target_file.parent.mkdir(parents=True)
 
             logging.info("Render template %s to %s", file, target_file)
             template_renderer.render_file(str(file), target_file)
 
-    def check_directories(self):
-        """
-        Checks for project and template directories.
-        Creates project directory if it doesn't exist.
+    def _should_ignore(self, file_path) -> bool:
         """
-        if not self.template_path.exists():
-            raise FileNotFoundError(f"Template path not found: {self.template_path}")
-        if not self.project_path.exists():
-            logging.debug("Creating project directory at %s", self.project_path)
-            self.project_path.mkdir(parents=True)
-
-    def get_template_data(self) -> dict[str, str]:
-        """
-        Returns a dictionary containing the data used for templating.
-        :return: Dictionary containing the data
-        """
-        return {
-            "name": self.project_name,
-            "lib_name": self.project_name.lower().replace("_", ""),
-            "class_name": self._get_class_name(),
-        }
-
-    def _get_class_name(self) -> str:
-        class_name = ""
-        for part in self.project_name.lower().split("_"):
-            class_name += part.capitalize()
-        return class_name
+        Whether to ignore the given file or not.
+        :param file_path: The file path to be checked.
+        :return: True if the file should be ignored. False otherwise.
+        """
+        for ignored in self.IGNORED_DIRECTORIES:
+            if file_path.startswith(ignored):
+                logging.debug("Ignoring %s", file_path)
+                return True
+        return False
```

### Comparing `gdextension_cli-0.0.2b3/.gitignore` & `gdextension_cli-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/LICENSE` & `gdextension_cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b3/pyproject.toml` & `gdextension_cli-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,15 @@
     { name = "Sören Spindler", email = "soeren.s89@gmail.com" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "Jinja2==3.1.4",
-    "GitPython==3.1.43"
+    "Jinja2==3.1.4"
 ]
 dynamic = [
     "version"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/3LK3/gdextension-cli"
```

