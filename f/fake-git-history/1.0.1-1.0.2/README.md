# Comparing `tmp/fake_git_history-1.0.1.tar.gz` & `tmp/fake_git_history-1.0.2.tar.gz`

## Comparing `fake_git_history-1.0.1.tar` & `fake_git_history-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0   288825 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/contribution-graph.gif
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/fake_git_history/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/fake_git_history/__main__.py
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/fake_git_history/cli.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/LICENSE
--rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/README.md
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0   288825 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/contribution-graph.gif
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/fake_git_history/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/fake_git_history/__main__.py
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/fake_git_history/cli.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/LICENSE
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/README.md
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    14874 2020-02-02 00:00:00.000000 fake_git_history-1.0.2/PKG-INFO
```

### Comparing `fake_git_history-1.0.1/contribution-graph.gif` & `fake_git_history-1.0.2/contribution-graph.gif`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.1/.github/workflows/python-publish.yml` & `fake_git_history-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.1/fake_git_history/__main__.py` & `fake_git_history-1.0.2/fake_git_history/__main__.py`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.1/fake_git_history/cli.py` & `fake_git_history-1.0.2/fake_git_history/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import string
 import os
 import subprocess
 import re
 
 import rong  # type: ignore
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 
 class Commit(NamedTuple):
     message: str
     date: str
```

### Comparing `fake_git_history-1.0.1/LICENSE` & `fake_git_history-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.1/README.md` & `fake_git_history-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Fake Git History Generator
 
 A simple utility to generate fake git history for a Github and Gitlab profile to make your profile look more active than it actually is.
 
 ***Author: [Md. Almas Ali](https://almasali.net)***
 
-[![wakatime](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8.svg)](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8)
 [![PyPI version](https://badge.fury.io/py/fake-git-history.svg)](https://badge.fury.io/py/fake-git-history)
 [![Downloads](https://pepy.tech/badge/fake-git-history)](https://pepy.tech/project/fake-git-history)
-[![Downloads](https://pepy.tech/badge/fake-git-history/month)](https://pepy.tech/project/fake-git-history)
-[![Downloads](https://pepy.tech/badge/fake-git-history/week)](https://pepy.tech/project/fake-git-history)
+[![wakatime](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8.svg)](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8)
+![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FAlmas-Ali%2Ffake-git-history&count_bg=%2379C83D&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=Hits&edge_flat=false)
 
 ![How it works](https://github.com/Almas-Ali/fake-git-history/blob/master/contribution-graph.gif "How it works")
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Support This Project](#support-this-project)
```

#### html2text {}

```diff
@@ -1,100 +1,100 @@
 # Fake Git History Generator A simple utility to generate fake git history for
 a Github and Gitlab profile to make your profile look more active than it
-actually is. ***Author: [Md. Almas Ali](https://almasali.net)*** [![wakatime]
-(https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/
-60aed9e5-281b-4468-8819-5a1cef8d90d8.svg)](https://wakatime.com/badge/user/
-168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-
-5a1cef8d90d8) [![PyPI version](https://badge.fury.io/py/fake-git-history.svg)]
-(https://badge.fury.io/py/fake-git-history) [![Downloads](https://pepy.tech/
-badge/fake-git-history)](https://pepy.tech/project/fake-git-history) [!
-[Downloads](https://pepy.tech/badge/fake-git-history/month)](https://pepy.tech/
-project/fake-git-history) [![Downloads](https://pepy.tech/badge/fake-git-
-history/week)](https://pepy.tech/project/fake-git-history) ![How it works]
-(https://github.com/Almas-Ali/fake-git-history/blob/master/contribution-
-graph.gif "How it works") ## Table of Contents - [Introduction](#introduction)
-- [Support This Project](#support-this-project) - [Installation](#installation)
-- [Options and Usage](#options-and-usage) - [`--commit-per-day` and `-c`](#--
-commit-per-day-and--c) - [`--work-days-only` and `-wd`](#--work-days-only-and--
-wd) - [`--weekends-only` and `-we`](#--weekends-only-and--we) - [`--start-date`
-and `--end-date` or `-sd` and `-ed`](#--start-date-and--end-date-or--sd-and--
-ed) - [`--start-time` and `--end-time` or `-st` and `-et`](#--start-time-and--
-end-time-or--st-and--et) - [`--time-zone` and `-tz`](#--time-zone-and--tz) -
-[`--remote-origin` and `-r`](#--remote-origin-and---r) - [`--auto-git-push` and
-`-a`](#--auto-git-push-and--a) - [`--verbose` and `-vv`](#--verbose-and--vv) -
-[`--version` and `-v`](#--version-and--v) - [`--help` and `-h`](#--help-and--h)
-- [Demo and Examples](#demo-and-examples) - [Example 1](#example-1) - [Example
-2](#example-2) - [Example 3](#example-3) - [Example 4](#example-4) - [Example
-5](#example-5) - [Caution](#caution) - [License](#license) ## Introduction Fake
-Git History Generator is a simple utility to generate fake git history for a
-Github and Gitlab profile to make your profile look more active than it
-actually is. It generates fake commits for the last 90 days (by default config)
-with random commit counts per day (0-3). You can also specify the number of
-commits per day, start date, end date, start time, end time, time zone, work
-days only, weekends only, remote origin, auto git push, and verbose output. It
-uses the `git` command to create commits and push them to the remote
-repository. **Give this project a star, if you like it. (Highly Recommended)
-ð** This project is inspired by [fake-git-history](https://github.com/
-artiebits/fake-git-history) JS project. **Note:** Read the [Caution](#caution)
-section before using this tool. ## Support This Project If you find this
-project useful and want to support my work, you can buy me a coffee. My work is
-open source and free. Your support will allow me to continue my work and build
-more projects. Thank you for your support! _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]## Installation You
-need to have [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-
-Git) and [Python3](https://www.python.org/downloads/) installed on your
-machine. Then you can install it with `pip`. ```bash pip install fake-git-
-history ``` You can also install it from source. If you want then follow this.
-```bash # Clone the git repository git clone https://github.com/Almas-Ali/fake-
-git-history.git fake-git-history # Change your directory to fake-git-history cd
-fake-git-history # Install it with pip pip install . ``` ## Options and Usage
-### `--commit-per-day` and `-c` Specify the number of commits to be created for
-each day. The default value is `0-3`, which means it will randomly generate
-from 0 to 3 commits per day. For example, to generate commits randomly between
-6 and 12 per day, you can do: ```bash fake-git-history --commit-per-day "6-12"
-# or fake-git-history -c "6-12" ``` You can also give a strict number. For
-example, you need 16 contributions every single day. Then use this command. Not
-recommended, this will make views to easily detect your bot. ```bash fake-git-
-history --commit-per-day "16" # or fake-git-history -c "16" ``` ### `--work-
-days-only` and `-wd` Use this option if you don't want to commit on weekends.
-Example: ```bash fake-git-history --work-days-only # or fake-git-history -d ```
-### `--weekends-only` and `-we` Use this option if you only want to contribute
-on weekends. Example: ```bash fake-git-history --weekends-only # or fake-git-
-history -w ``` ### `--start-date` and `--end-date` or `-sd` and `-ed` The
-starting data is by default set to previous 90 days from the current date and
-end date is by default present date. If you don't change, it will create
-commits for the last 90 days. You can change the start date and end date.
-Example: ```bash # User defined start and end date fake-git-history --start-
-date "01/03/2016" --end-date "12/02/2023" # or fake-git-history -s "01/03/2016"
--e "12/02/2023" # Flexible end date fake-git-history --start-date "01/03/2016"
-# or fake-git-history -s "01/03/2016" ``` The date formating is `DD/MM/YYYY`.
-You have to write this way. ### `--start-time` and `--end-time` or `-st` and `-
-et` The starting time is by default set to `00:00:00` and end time is by
-default `23:59:59`. You can change the start time and end time. Example:
-```bash # User defined start and end time fake-git-history --start-time "09:00:
-00" --end-time "17:00:00" # or fake-git-history -st "09:00:00" -et "17:00:00"
-``` The time formating is `HH:MM:SS`. You have to write this way. ### `--time-
-zone` and `-tz` The time zone is by default set to your local time zone. You
-can change the time zone. Example: ```bash # User defined time zone fake-git-
-history --time-zone "+0600" # or fake-git-history -tz "+0600" ``` The time zone
-formating is `+HHMM` or `-HHMM`. You have to write this way. ### `--remote-
-origin` and `-r` Use this option to set the remote origin. Example: ```bash
-fake-git-history --remote-origin "git@github.com:/.git" # or fake-git-history -
-r "git@github.com:/.git" ``` ### `--auto-git-push` and `-a` Use this option to
-automatically push the commits to the remote repository. Example: ```bash fake-
-git-history --auto-git-push # or fake-git-history -a ``` ### `--verbose` and `-
-vv` Use this option to see the verbose output. Without this option you won't be
-able to see much information about the process. Example: ```bash fake-git-
-history --verbose # or fake-git-history -vv ``` ### `--version` and `-v` Use
-this option to check the version of this script. ```bash fake-git-history --
-version # or fake-git-history -v ``` ### `--help` and `-h` You can always refer
-to this help menu to see the options available. Example: ```bash fake-git-
-history --help ``` **Output** ```bash usage: fake-git-history [-h] [--start-
-date START_DATE] [--end-date END_DATE] [--start-time START_TIME] [--end-time
-END_TIME] [--time-zone TIME_ZONE] [--work-days-only] [--weekends-only] [--
-commit-per-day COMMIT_PER_DAY] [--auto-git-push] [--remote-origin
+actually is. ***Author: [Md. Almas Ali](https://almasali.net)*** [![PyPI
+version](https://badge.fury.io/py/fake-git-history.svg)](https://badge.fury.io/
+py/fake-git-history) [![Downloads](https://pepy.tech/badge/fake-git-history)]
+(https://pepy.tech/project/fake-git-history) [![wakatime](https://wakatime.com/
+badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-
+8819-5a1cef8d90d8.svg)](https://wakatime.com/badge/user/168edf9f-71dc-49cc-
+bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8) ![Hits](https:/
+/hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2FAlmas-Ali%2Ffake-git-
+history&count_bg=%2379C83D&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=Hits&edge_flat=false)
+![How it works](https://github.com/Almas-Ali/fake-git-history/blob/master/
+contribution-graph.gif "How it works") ## Table of Contents - [Introduction]
+(#introduction) - [Support This Project](#support-this-project) -
+[Installation](#installation) - [Options and Usage](#options-and-usage) - [`--
+commit-per-day` and `-c`](#--commit-per-day-and--c) - [`--work-days-only` and
+`-wd`](#--work-days-only-and--wd) - [`--weekends-only` and `-we`](#--weekends-
+only-and--we) - [`--start-date` and `--end-date` or `-sd` and `-ed`](#--start-
+date-and--end-date-or--sd-and--ed) - [`--start-time` and `--end-time` or `-st`
+and `-et`](#--start-time-and--end-time-or--st-and--et) - [`--time-zone` and `-
+tz`](#--time-zone-and--tz) - [`--remote-origin` and `-r`](#--remote-origin-and-
+--r) - [`--auto-git-push` and `-a`](#--auto-git-push-and--a) - [`--verbose` and
+`-vv`](#--verbose-and--vv) - [`--version` and `-v`](#--version-and--v) - [`--
+help` and `-h`](#--help-and--h) - [Demo and Examples](#demo-and-examples) -
+[Example 1](#example-1) - [Example 2](#example-2) - [Example 3](#example-3) -
+[Example 4](#example-4) - [Example 5](#example-5) - [Caution](#caution) -
+[License](#license) ## Introduction Fake Git History Generator is a simple
+utility to generate fake git history for a Github and Gitlab profile to make
+your profile look more active than it actually is. It generates fake commits
+for the last 90 days (by default config) with random commit counts per day (0-
+3). You can also specify the number of commits per day, start date, end date,
+start time, end time, time zone, work days only, weekends only, remote origin,
+auto git push, and verbose output. It uses the `git` command to create commits
+and push them to the remote repository. **Give this project a star, if you like
+it. (Highly Recommended) ð** This project is inspired by [fake-git-history]
+(https://github.com/artiebits/fake-git-history) JS project. **Note:** Read the
+[Caution](#caution) section before using this tool. ## Support This Project If
+you find this project useful and want to support my work, you can buy me a
+coffee. My work is open source and free. Your support will allow me to continue
+my work and build more projects. Thank you for your support! _[_B_u_y_ _M_e_ _A
+_C_o_f_f_e_e_]## Installation You need to have [Git](https://git-scm.com/book/en/v2/
+Getting-Started-Installing-Git) and [Python3](https://www.python.org/downloads/
+) installed on your machine. Then you can install it with `pip`. ```bash pip
+install fake-git-history ``` You can also install it from source. If you want
+then follow this. ```bash # Clone the git repository git clone https://
+github.com/Almas-Ali/fake-git-history.git fake-git-history # Change your
+directory to fake-git-history cd fake-git-history # Install it with pip pip
+install . ``` ## Options and Usage ### `--commit-per-day` and `-c` Specify the
+number of commits to be created for each day. The default value is `0-3`, which
+means it will randomly generate from 0 to 3 commits per day. For example, to
+generate commits randomly between 6 and 12 per day, you can do: ```bash fake-
+git-history --commit-per-day "6-12" # or fake-git-history -c "6-12" ``` You can
+also give a strict number. For example, you need 16 contributions every single
+day. Then use this command. Not recommended, this will make views to easily
+detect your bot. ```bash fake-git-history --commit-per-day "16" # or fake-git-
+history -c "16" ``` ### `--work-days-only` and `-wd` Use this option if you
+don't want to commit on weekends. Example: ```bash fake-git-history --work-
+days-only # or fake-git-history -d ``` ### `--weekends-only` and `-we` Use this
+option if you only want to contribute on weekends. Example: ```bash fake-git-
+history --weekends-only # or fake-git-history -w ``` ### `--start-date` and `--
+end-date` or `-sd` and `-ed` The starting data is by default set to previous 90
+days from the current date and end date is by default present date. If you
+don't change, it will create commits for the last 90 days. You can change the
+start date and end date. Example: ```bash # User defined start and end date
+fake-git-history --start-date "01/03/2016" --end-date "12/02/2023" # or fake-
+git-history -s "01/03/2016" -e "12/02/2023" # Flexible end date fake-git-
+history --start-date "01/03/2016" # or fake-git-history -s "01/03/2016" ``` The
+date formating is `DD/MM/YYYY`. You have to write this way. ### `--start-time`
+and `--end-time` or `-st` and `-et` The starting time is by default set to `00:
+00:00` and end time is by default `23:59:59`. You can change the start time and
+end time. Example: ```bash # User defined start and end time fake-git-history -
+-start-time "09:00:00" --end-time "17:00:00" # or fake-git-history -st "09:00:
+00" -et "17:00:00" ``` The time formating is `HH:MM:SS`. You have to write this
+way. ### `--time-zone` and `-tz` The time zone is by default set to your local
+time zone. You can change the time zone. Example: ```bash # User defined time
+zone fake-git-history --time-zone "+0600" # or fake-git-history -tz "+0600" ```
+The time zone formating is `+HHMM` or `-HHMM`. You have to write this way. ###
+`--remote-origin` and `-r` Use this option to set the remote origin. Example:
+```bash fake-git-history --remote-origin "git@github.com:/.git" # or fake-git-
+history -r "git@github.com:/.git" ``` ### `--auto-git-push` and `-a` Use this
+option to automatically push the commits to the remote repository. Example:
+```bash fake-git-history --auto-git-push # or fake-git-history -a ``` ### `--
+verbose` and `-vv` Use this option to see the verbose output. Without this
+option you won't be able to see much information about the process. Example:
+```bash fake-git-history --verbose # or fake-git-history -vv ``` ### `--
+version` and `-v` Use this option to check the version of this script. ```bash
+fake-git-history --version # or fake-git-history -v ``` ### `--help` and `-h`
+You can always refer to this help menu to see the options available. Example:
+```bash fake-git-history --help ``` **Output** ```bash usage: fake-git-history
+[-h] [--start-date START_DATE] [--end-date END_DATE] [--start-time START_TIME]
+[--end-time END_TIME] [--time-zone TIME_ZONE] [--work-days-only] [--weekends-
+only] [--commit-per-day COMMIT_PER_DAY] [--auto-git-push] [--remote-origin
 REMOTE_ORIGIN] [--verbose] [--version] Fake Git History - A simple utility to
 generate fake git history for a Github and Gitlab profile. options: -h, --help
 show this help message and exit --start-date START_DATE, -sd START_DATE Set the
 start date (dd/mm/yyyy) --end-date END_DATE, -ed END_DATE Set the end date (dd/
 mm/yyyy) --start-time START_TIME, -st START_TIME Set the start time (hh:mm:ss)
 --end-time END_TIME, -et END_TIME Set the end time (hh:mm:ss) --time-zone
 TIME_ZONE, -tz TIME_ZONE Set the time zone in the format +0600 --work-days-
```

### Comparing `fake_git_history-1.0.1/pyproject.toml` & `fake_git_history-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.1/PKG-INFO` & `fake_git_history-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fake-git-history
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple utility to generate fake git history for a Github and Gitlab profile.
 Project-URL: Homepage, https://github.com/Almas-Ali/fake-git-history
 Project-URL: Documentation, https://github.com/Almas-Ali/fake-git-history#readme
 Project-URL: Repository, https://github.com/Almas-Ali/fake-git-history
 Project-URL: Bug Tracker, https://github.com/Almas-Ali/fake-git-history/issues
 Author-email: "Md. Almas Ali" <almaspr3@gmail.com>
 Maintainer-email: "Md. Almas Ali" <almaspr3@gmail.com>
@@ -51,19 +51,18 @@
 
 # Fake Git History Generator
 
 A simple utility to generate fake git history for a Github and Gitlab profile to make your profile look more active than it actually is.
 
 ***Author: [Md. Almas Ali](https://almasali.net)***
 
-[![wakatime](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8.svg)](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8)
 [![PyPI version](https://badge.fury.io/py/fake-git-history.svg)](https://badge.fury.io/py/fake-git-history)
 [![Downloads](https://pepy.tech/badge/fake-git-history)](https://pepy.tech/project/fake-git-history)
-[![Downloads](https://pepy.tech/badge/fake-git-history/month)](https://pepy.tech/project/fake-git-history)
-[![Downloads](https://pepy.tech/badge/fake-git-history/week)](https://pepy.tech/project/fake-git-history)
+[![wakatime](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8.svg)](https://wakatime.com/badge/user/168edf9f-71dc-49cc-bf77-592d9c9d4eed/project/60aed9e5-281b-4468-8819-5a1cef8d90d8)
+![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FAlmas-Ali%2Ffake-git-history&count_bg=%2379C83D&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=Hits&edge_flat=false)
 
 ![How it works](https://github.com/Almas-Ali/fake-git-history/blob/master/contribution-graph.gif "How it works")
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Support This Project](#support-this-project)
```

