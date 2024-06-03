# Comparing `tmp/librus_apix-1.0.5.tar.gz` & `tmp/librus_apix-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-1.0.5.tar", last modified: Thu May 30 07:47:16 2024, max compression
+gzip compressed data, was "librus_apix-1.0.6.tar", last modified: Mon Jun  3 13:13:20 2024, max compression
```

## Comparing `librus_apix-1.0.5.tar` & `librus_apix-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:47:16.023748 librus_apix-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 07:47:12.000000 librus_apix-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 07:47:16.023748 librus_apix-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-30 07:47:12.000000 librus_apix-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:47:16.023748 librus_apix-1.0.5/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-30 07:47:12.000000 librus_apix-1.0.5/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:47:16.023748 librus_apix-1.0.5/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-30 07:47:16.000000 librus_apix-1.0.5/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 07:47:15.000000 librus_apix-1.0.5/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 07:47:12.000000 librus_apix-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-30 07:47:16.023748 librus_apix-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:47:12.000000 librus_apix-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:13:20.271956 librus_apix-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 13:13:12.000000 librus_apix-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-03 13:13:20.271956 librus_apix-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-06-03 13:13:12.000000 librus_apix-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:13:20.271956 librus_apix-1.0.6/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18214 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-06-03 13:13:12.000000 librus_apix-1.0.6/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:13:20.271956 librus_apix-1.0.6/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-03 13:13:20.000000 librus_apix-1.0.6/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-06-03 13:13:20.000000 librus_apix-1.0.6/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:13:20.000000 librus_apix-1.0.6/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 13:13:20.000000 librus_apix-1.0.6/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 13:13:20.000000 librus_apix-1.0.6/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 13:13:12.000000 librus_apix-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-06-03 13:13:20.275956 librus_apix-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:13:12.000000 librus_apix-1.0.6/setup.py
```

### Comparing `librus_apix-1.0.5/LICENSE` & `librus_apix-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/README.md` & `librus_apix-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/librus_apix/__init__.py` & `librus_apix-1.0.6/librus_apix/__init__.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/librus_apix/announcements.py` & `librus_apix-1.0.6/librus_apix/announcements.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 client.get_token(username, password)
 
 # Retrieve announcements
 announcements = get_announcements(client)
 ```
 """
 
-
 from typing import List
 from bs4 import BeautifulSoup
 from librus_apix.client import Client
 from librus_apix.helpers import no_access_check
 from dataclasses import dataclass
 from librus_apix.exceptions import ParseError
 
@@ -68,17 +67,19 @@
     if len(announcement_tables) < 1:
         raise ParseError("Error in parsing announcements")
     for table in announcement_tables:
         title = table.select_one("thead > tr > td")
         title = title.text if title is not None else ""
 
         data = [
-            line.select_one("td").text.strip()
-            if line.select_one("td") is not None
-            else ""
+            (
+                line.select_one("td").text.strip()
+                if line.select_one("td") is not None
+                else ""
+            )
             for line in table.find_all("tr", attrs={"class": ["line0", "line1"]})
         ]
         if len(data) != 3:
             raise ParseError(f"Expected 3 items in Announcement data, got {len(data)}")
         author, date, desc = data
         a = Announcement(title, author, desc, date)
         announcements.append(a)
```

### Comparing `librus_apix-1.0.5/librus_apix/attendance.py` & `librus_apix-1.0.6/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/librus_apix/client.py` & `librus_apix-1.0.6/librus_apix/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 #Alternatively, you can use the classes directly:
 my_token = Token(API_Key="your_api_key")
 my_client = Client(token=my_token)
 ```
 """
 
-
 from typing import Dict, Optional
 
 from requests import Session
 from requests.models import Response
 from requests.sessions import RequestsCookieJar
 from requests.utils import cookiejar_from_dict, dict_from_cookiejar
```

### Comparing `librus_apix-1.0.5/librus_apix/completed_lessons.py` & `librus_apix-1.0.6/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/librus_apix/exceptions.py` & `librus_apix-1.0.6/librus_apix/exceptions.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/librus_apix/grades.py` & `librus_apix-1.0.6/librus_apix/grades.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     # Handle invalid argument error
     ...
 except ParseError as e:
     # Handle parse error
     ...
 ```
 """
+
 import re
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import DefaultDict, List, Tuple, Union
 
 from bs4 import BeautifulSoup, Tag
 
@@ -115,17 +116,15 @@
     date: str
     href: str
     desc: str
     semester: int
     teacher: str
 
 
-def get_grades(
-    client: Client, sort_by: str = "all"
-) -> Tuple[
+def get_grades(client: Client, sort_by: str = "all") -> Tuple[
     List[DefaultDict[str, List[Grade]]],
     DefaultDict[str, List[Gpa]],
     List[DefaultDict[str, List[GradeDescriptive]]],
 ]:
     """
     Fetches and returns the grades, semestral averages and descriptive grades from librus.
```

### Comparing `librus_apix-1.0.5/librus_apix/helpers.py` & `librus_apix-1.0.6/librus_apix/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module defines a function for checking access to Librus resources by examining the content of a BeautifulSoup object.
 
 Functions:
     - no_access_check: Checks for access to Librus resources by examining the content of a BeautifulSoup object.
 
 """
+
 from bs4 import BeautifulSoup
 from librus_apix.exceptions import TokenError
 
 
 def no_access_check(soup: BeautifulSoup) -> BeautifulSoup:
     pattern = "Brak dostępu"
     no_access = soup.select_one("h2.inside")
```

### Comparing `librus_apix-1.0.5/librus_apix/homework.py` & `librus_apix-1.0.6/librus_apix/homework.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 homework_assignments = get_homework(client, date_from, date_to)
 
 # Retrieve detailed information about a specific homework assignment
 for homework in homework_assignments:
     homework_details = homework_detail(client, homework.href)
 ```
 """
+
 from typing import List, Dict
 from bs4 import BeautifulSoup, NavigableString
 from librus_apix.client import Client
 from librus_apix.helpers import no_access_check
 from librus_apix.exceptions import ParseError
 from dataclasses import dataclass
```

### Comparing `librus_apix-1.0.5/librus_apix/messages.py` & `librus_apix-1.0.6/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/librus_apix/notifications.py` & `librus_apix-1.0.6/librus_apix/notifications.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Functions:
     - get_initial_notification_data(client: Client) -> Tuple[NotificationData, NotificationIds]: Fetches and parses the initial notification data and their IDs for a new token.
     - get_new_notification_data(client: Client, seen_notifications: NotificationIds) -> Tuple[NotificationData, NotificationIds]: Fetches and parses new notifications using NotificationIds, returns data and updates seen notification IDs.
 """
 
 from dataclasses import dataclass
 from datetime import datetime, timedelta
+from hashlib import md5
 from typing import Any, DefaultDict, List, Tuple
 
 from bs4 import BeautifulSoup, Tag
 
 from librus_apix.announcements import Announcement, get_announcements
 from librus_apix.attendance import Attendance, get_attendance
 from librus_apix.client import Client
@@ -92,14 +93,28 @@
     return notifications
 
 
 def _compare_hrefs(object_href: str, href_ids: List[str]):
     return object_href in href_ids
 
 
+def _parse_recent_schedule_notification(
+    schedule: List[RecentEvent], seen_ids: List[str] = []
+):
+    new_schedule = []
+    for event in schedule:
+        data_bytes = event.data.encode("utf-8")
+        _id = md5(data_bytes).hexdigest()
+        if _compare_hrefs(_id, seen_ids):
+            continue
+        seen_ids.append(_id)
+        new_schedule.append(event)
+    return new_schedule, seen_ids
+
+
 def _parse_announcements_notification(
     announcements: List[Announcement], seen_ids: List[str] = []
 ):
     new_announcements = []
     for announcement in announcements:
         _id = announcement.title + announcement.date
         if _compare_hrefs(_id, seen_ids):
@@ -310,15 +325,19 @@
     today = datetime.now()
     homework = get_homework(
         client,
         (today - timedelta(days=7)).strftime("%Y-%m-%d"),
         today.strftime("%Y-%m-%d"),
     )[::-1]
 
-    new_schedule = get_recently_added_schedule(client)
+    schedule = get_recently_added_schedule(client)
+
+    new_schedule, seen_events = _parse_recent_schedule_notification(
+        schedule, seen_notifications.schedule
+    )
     new_grades, seen_grades = _parse_grades_notifications(
         grades, seen_notifications.grades
     )
     new_attendance, seen_attendance = _parse_attendance_notification(
         attendance, seen_notifications.attendance
     )
     new_messages, seen_messages = _parse_messages_notification(
@@ -339,10 +358,10 @@
         new_schedule,
         new_homework,
     ), NotificationIds(
         seen_grades,
         seen_attendance,
         seen_messages,
         seen_announcements,
-        [],
+        seen_events,
         seen_homework,
     )
```

### Comparing `librus_apix-1.0.5/librus_apix/schedule.py` & `librus_apix-1.0.6/librus_apix/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     # Fetch detailed schedule information
     day_one = monthly_schedule[1].href
     prefix, suffix = day_one.split("/")
     detailed_schedule = schedule_detail(client, prefix, detail_url)
     ```
 """
+
 import re
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import DefaultDict, Dict, List, Union
 
 from bs4 import BeautifulSoup, NavigableString, Tag
```

### Comparing `librus_apix-1.0.5/librus_apix/student_information.py` & `librus_apix-1.0.6/librus_apix/student_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     print(student_info.class_name)
     print(student_info.number)
     print(student_info.tutor)
     print(student_info.school)
     print(student_info.lucky_number)
     ```
 """
+
 from typing import Union
 from bs4 import BeautifulSoup
 from dataclasses import dataclass
 from librus_apix.exceptions import ParseError
 from librus_apix.helpers import no_access_check
 from librus_apix.client import Client
```

### Comparing `librus_apix-1.0.5/librus_apix/timetable.py` & `librus_apix-1.0.6/librus_apix/timetable.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             print(period.subject, period.date, period.date_from, period.date_to)
 except DateError as e:
     print(e)
 except ParseError as e:
     print(e)
 ```
 """
+
 from typing import List, Dict
 from librus_apix.client import Client
 from librus_apix.exceptions import ParseError, DateError
 from librus_apix.helpers import no_access_check
 from datetime import datetime, timedelta
 from bs4 import BeautifulSoup
 from dataclasses import dataclass
```

### Comparing `librus_apix-1.0.5/librus_apix/urls.py` & `librus_apix-1.0.6/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/librus_apix.egg-info/SOURCES.txt` & `librus_apix-1.0.6/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.5/setup.cfg` & `librus_apix-1.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v1.0.5
+version = v1.0.6
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

