# Comparing `tmp/rstms_testmail-0.2.4.tar.gz` & `tmp/rstms_testmail-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_testmail-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_testmail-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_testmail-0.2.4.tar` & `rstms_testmail-0.2.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      381 2024-05-28 05:14:49.396163 rstms_testmail-0.2.4/.bumpversion.cfg
--rw-r--r--   0        0        0     1375 2024-04-28 12:24:23.591184 rstms_testmail-0.2.4/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.2.4/LICENSE
--rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.2.4/Makefile
--rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.2.4/README.md
--rw-r--r--   0        0        0        6 2024-05-28 05:14:49.392163 rstms_testmail-0.2.4/VERSION
--rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.2.4/docs/Makefile
--rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.2.4/docs/cli.rst
--rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.2.4/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.2.4/docs/contributing.rst
--rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.2.4/docs/index.rst
--rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.2.4/docs/installation.rst
--rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.2.4/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.2.4/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.2.4/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.2.4/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.2.4/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.2.4/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.2.4/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.2.4/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.2.4/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.2.4/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.2.4/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.2.4/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.2.4/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.2.4/make/version.mk
--rw-r--r--   0        0        0     1232 2024-05-28 05:14:49.396163 rstms_testmail-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.2.4/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-28 05:14:49.248164 rstms_testmail-0.2.4/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-28 05:14:49.304164 rstms_testmail-0.2.4/requirements-docs.txt
--rw-r--r--   0        0        0       89 2024-05-28 05:14:49.192165 rstms_testmail-0.2.4/requirements.txt
--rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.2.4/rstms_testmail/__init__.py
--rw-r--r--   0        0        0     5131 2024-05-28 04:45:46.874257 rstms_testmail-0.2.4/rstms_testmail/cli.py
--rw-r--r--   0        0        0     1083 2024-05-28 03:51:36.702296 rstms_testmail-0.2.4/rstms_testmail/counter.py
--rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.2.4/rstms_testmail/exception_handler.py
--rw-r--r--   0        0        0     3690 2024-05-28 05:11:13.522586 rstms_testmail-0.2.4/rstms_testmail/gmail.py
--rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.2.4/rstms_testmail/netstat.py
--rw-r--r--   0        0        0      584 2024-05-17 19:53:22.655493 rstms_testmail-0.2.4/rstms_testmail/sendgrid_server.py
--rw-r--r--   0        0        0     1730 2024-05-28 04:19:47.052744 rstms_testmail-0.2.4/rstms_testmail/settings.py
--rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.2.4/rstms_testmail/shell.py
--rw-r--r--   0        0        0     1454 2024-05-28 04:52:46.146775 rstms_testmail-0.2.4/rstms_testmail/smtp_server.py
--rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.2.4/rstms_testmail/timer.py
--rw-r--r--   0        0        0      127 2024-05-28 05:14:49.392163 rstms_testmail-0.2.4/rstms_testmail/version.py
--rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.2.4/rstms_testmail/watcher.py
--rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-17 19:56:14.241618 rstms_testmail-0.2.4/tests/test_cli.py
--rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.2.4/tests/test_counter.py
--rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.2.4/tests/test_gmail.py
--rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.2.4/tests/test_netstat.py
--rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.2.4/tests/test_sendgrid.py
--rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.2.4/tests/test_watcher.py
--rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.2.4/tox.ini
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      381 2024-06-03 00:12:58.637037 rstms_testmail-0.2.5/.bumpversion.cfg
+-rw-r--r--   0        0        0     1381 2024-06-03 00:12:38.221238 rstms_testmail-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.2.5/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.2.5/Makefile
+-rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.2.5/README.md
+-rw-r--r--   0        0        0        6 2024-06-03 00:12:58.637037 rstms_testmail-0.2.5/VERSION
+-rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.2.5/docs/Makefile
+-rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.2.5/docs/cli.rst
+-rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.2.5/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.2.5/docs/contributing.rst
+-rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.2.5/docs/index.rst
+-rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.2.5/docs/installation.rst
+-rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.2.5/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.2.5/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.2.5/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.2.5/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.2.5/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.2.5/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.2.5/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.2.5/make/docs.mk
+-rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.2.5/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.2.5/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.2.5/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.2.5/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.2.5/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.2.5/make/version.mk
+-rw-r--r--   0        0        0     1232 2024-06-03 00:12:58.637037 rstms_testmail-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.2.5/pytest.ini
+-rw-r--r--   0        0        0       97 2024-06-03 00:12:58.473039 rstms_testmail-0.2.5/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-06-03 00:12:58.537038 rstms_testmail-0.2.5/requirements-docs.txt
+-rw-r--r--   0        0        0       89 2024-06-03 00:12:58.409039 rstms_testmail-0.2.5/requirements.txt
+-rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.2.5/rstms_testmail/__init__.py
+-rw-r--r--   0        0        0     5353 2024-06-03 00:11:57.213640 rstms_testmail-0.2.5/rstms_testmail/cli.py
+-rw-r--r--   0        0        0     1082 2024-06-03 00:11:57.141641 rstms_testmail-0.2.5/rstms_testmail/counter.py
+-rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.2.5/rstms_testmail/exception_handler.py
+-rw-r--r--   0        0        0     3690 2024-05-28 05:11:13.522586 rstms_testmail-0.2.5/rstms_testmail/gmail.py
+-rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.2.5/rstms_testmail/netstat.py
+-rw-r--r--   0        0        0      584 2024-05-17 19:53:22.655493 rstms_testmail-0.2.5/rstms_testmail/sendgrid_server.py
+-rw-r--r--   0        0        0     1730 2024-06-03 00:11:57.157641 rstms_testmail-0.2.5/rstms_testmail/settings.py
+-rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.2.5/rstms_testmail/shell.py
+-rw-r--r--   0        0        0     1454 2024-06-03 00:11:57.137641 rstms_testmail-0.2.5/rstms_testmail/smtp_server.py
+-rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.2.5/rstms_testmail/timer.py
+-rw-r--r--   0        0        0      127 2024-06-03 00:12:58.637037 rstms_testmail-0.2.5/rstms_testmail/version.py
+-rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.2.5/rstms_testmail/watcher.py
+-rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-17 19:56:14.241618 rstms_testmail-0.2.5/tests/test_cli.py
+-rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.2.5/tests/test_counter.py
+-rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.2.5/tests/test_gmail.py
+-rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.2.5/tests/test_netstat.py
+-rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.2.5/tests/test_sendgrid.py
+-rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.2.5/tests/test_watcher.py
+-rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.2.5/tox.ini
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.2.5/PKG-INFO
```

### Comparing `rstms_testmail-0.2.4/.gitignore` & `rstms_testmail-0.2.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -118,7 +118,8 @@
 docker/VERSION
 docker/.build
 docker/*.whl
 postactivate
 .counter
 credentials.json
 token.json
+notes
```

### Comparing `rstms_testmail-0.2.4/LICENSE` & `rstms_testmail-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/Makefile` & `rstms_testmail-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/README.md` & `rstms_testmail-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/docs/Makefile` & `rstms_testmail-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/docs/conf.py` & `rstms_testmail-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/docs/installation.rst` & `rstms_testmail-0.2.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/docs/make.bat` & `rstms_testmail-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/clean.mk` & `rstms_testmail-0.2.5/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/common.mk` & `rstms_testmail-0.2.5/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/docs.mk` & `rstms_testmail-0.2.5/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/lint.mk` & `rstms_testmail-0.2.5/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/publish.mk` & `rstms_testmail-0.2.5/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/release.mk` & `rstms_testmail-0.2.5/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/test.mk` & `rstms_testmail-0.2.5/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/make/version.mk` & `rstms_testmail-0.2.5/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/pyproject.toml` & `rstms_testmail-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-testmail"
-version = "0.2.4"
+version = "0.2.5"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_testmail"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_testmail-0.2.4/rstms_testmail/cli.py` & `rstms_testmail-0.2.5/rstms_testmail/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Console script for rstms_testmail."""
 
 import json
 import subprocess
 import sys
-from pprint import pformat
 from pathlib import Path
+from pprint import pformat
 
 import click
 import click.core
 
 from .counter import Counter
 from .exception_handler import ExceptionHandler
 from .gmail import Gmail
@@ -24,15 +24,15 @@
 def _ehandler(ctx, option, debug):
     ctx.obj = dict(ehandler=ExceptionHandler(debug))
     ctx.obj["debug"] = debug
     return debug
 
 
 def fail(msg):
-    click.echo("Failed: " + msg, err=True)
+    click.echo("testmail: " + msg, err=True)
     sys.exit(-1)
 
 
 @click.command("testmail")
 @click.version_option(message=header)
 @click.option("-d", "--debug", is_eager=True, is_flag=True, callback=_ehandler, help="debug mode")
 @click.option(
@@ -54,15 +54,16 @@
 @click.option("-u", "--username", envvar="TESTMAIL_USERNAME")
 @click.option("-p", "--password", envvar="TESTMAIL_PASSWORD")
 @click.option("-P", "--port", default=465, envvar="TESTMAIL_PORT")
 @click.option("-m", "--message", help="message to send or - to read from stdin")
 @click.option("--profile", "profile_option", default="default", show_envvar=True, envvar="TESTMAIL_PROFILE")
 @click.option("--dryrun", is_flag=True)
 @click.option("--reset-token", is_flag=True)
-@click.option("--show-password", is_flag=True, help='unmask password in dryrun output')
+@click.option("--set-default", is_flag=True)
+@click.option("--show-password", is_flag=True, help="unmask password in dryrun output")
 @click.option("-W", "--write-profile", help="write current profile")
 @click.option("-D", "--delete", "delete_profile", is_flag=True, help="profile name to delete")
 @click.option("-L", "--list", "list_profiles", is_flag=True, help="list available profiles")
 @click.argument("profile", required=False)
 @click.pass_context
 def cli(  # noqa:
     ctx,
@@ -84,32 +85,37 @@
     api_key,
     profile,
     write_profile,
     reset_token,
     delete_profile,
     list_profiles,
     profile_option,
-    show_password
+    show_password,
+    set_default,
 ):
     """send a test email"""
 
-    config_dir = Path.home()/'.testmail'
+    if set_default:
+        write_profile = "default"
+        dryrun = True
+
+    config_dir = Path.home() / ".testmail"
 
     if profile is None:
         profile = profile_option
 
     if "{}" in subject:
         counter = Counter(label="testmail", dir=config_dir)
         count = counter.bump(set_counter)
         subject = subject.replace("{}", str(count))
     else:
         counter = None
 
     settings = Settings(
-        label='testmail',
+        label="testmail",
         dir=config_dir,
         profile=profile,
         from_addr=from_addr,
         to_addr=to_addr,
         system=system,
         exec_command=exec_command,
         username=username,
@@ -121,14 +127,17 @@
 
     if delete_profile:
         settings.delete()
         sys.exit(0)
 
     profiles = settings.profiles()
 
+    if profile not in profiles:
+        fail(f"unknown profile '{profile}'")
+
     if list_profiles:
         click.echo("\n".join(profiles))
         sys.exit(0)
 
     if message in profiles:
         message is None
 
@@ -153,15 +162,15 @@
         server = SMTPServer(settings.system, settings.port, settings.username, settings.password, verbose)
     else:
         fail(f"unknown system: {repr(system)}")
 
     if dryrun:
         output = settings.dict()
         if not show_password:
-            output['password'] = '***************'
+            output["password"] = "***************"
         click.echo(pformat({profile: output}))
         if counter is not None:
             counter.rewind()
         sys.exit(0)
     else:
         error = server.send(settings.from_addr, settings.to_addr, subject, message)
```

### Comparing `rstms_testmail-0.2.4/rstms_testmail/counter.py` & `rstms_testmail-0.2.5/rstms_testmail/counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             self.read()
         else:
             self.value = int(count)
             self.write()
 
         self.initial_value = self.value
 
-
     def read(self):
         if not self.file.is_file():
             self.value = 0
             return self.write()
         self.value = int(self.file.read_text() or "0")
         return self.value
```

### Comparing `rstms_testmail-0.2.4/rstms_testmail/exception_handler.py` & `rstms_testmail-0.2.5/rstms_testmail/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/rstms_testmail/gmail.py` & `rstms_testmail-0.2.5/rstms_testmail/gmail.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/rstms_testmail/sendgrid_server.py` & `rstms_testmail-0.2.5/rstms_testmail/sendgrid_server.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/rstms_testmail/settings.py` & `rstms_testmail-0.2.5/rstms_testmail/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         for item in self.file.parent.iterdir():
             if not item.is_file():
                 continue
             prefix, _, tail = item.name.partition("_")
             if prefix != label:
                 continue
             name, _, tail = tail.partition("_")
-            if tail != 'settings':
+            if tail != "settings":
                 continue
             if name:
                 profiles.append(name)
         return profiles
 
     def read(self):
         if self.file.is_file():
```

### Comparing `rstms_testmail-0.2.4/rstms_testmail/shell.py` & `rstms_testmail-0.2.5/rstms_testmail/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/rstms_testmail/smtp_server.py` & `rstms_testmail-0.2.5/rstms_testmail/smtp_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         - message: str - the body of the email
         """
         # Create the container email message.
         mime_message = MIMEMultipart()
         mime_message["Subject"] = subject
         mime_message["From"] = from_addr
         mime_message["To"] = to_addr
-        mime_message['Message-ID'] = make_msgid()
+        mime_message["Message-ID"] = make_msgid()
         mime_message.attach(MIMEText(message, "plain"))
 
         # Connect to the SMTP server using SSL
         server = smtplib.SMTP_SSL(self.server, self.port)
         server.set_debuglevel(self.debug)
         server.login(self.username, self.password)
         ret = server.sendmail(from_addr, to_addr, mime_message.as_string())
```

### Comparing `rstms_testmail-0.2.4/rstms_testmail/timer.py` & `rstms_testmail-0.2.5/rstms_testmail/timer.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/rstms_testmail/watcher.py` & `rstms_testmail-0.2.5/rstms_testmail/watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/tests/test_cli.py` & `rstms_testmail-0.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/tests/test_sendgrid.py` & `rstms_testmail-0.2.5/tests/test_sendgrid.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/tests/test_watcher.py` & `rstms_testmail-0.2.5/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.4/PKG-INFO` & `rstms_testmail-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-testmail
-Version: 0.2.4
+Version: 0.2.5
 Summary: Top-level package for rstms-testmail.
 Keywords: rstms_testmail
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

