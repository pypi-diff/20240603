# Comparing `tmp/bbb_client-0.1.0.tar.gz` & `tmp/bbb_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbb_client-0.1.0.tar", max compression
+gzip compressed data, was "bbb_client-0.1.1.tar", max compression
```

## Comparing `bbb_client-0.1.0.tar` & `bbb_client-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2021-01-29 13:59:04.528218 bbb_client-0.1.0/COPYING
--rw-r--r--   0        0        0      824 2024-05-03 07:38:10.843078 bbb_client-0.1.0/bbb_client/__init__.py
--rw-r--r--   0        0        0      738 2024-05-03 07:38:10.843078 bbb_client-0.1.0/bbb_client/domain/__init__.py
--rw-r--r--   0        0        0      738 2024-05-03 07:38:10.843078 bbb_client-0.1.0/bbb_client/domain/meeting_management/__init__.py
--rw-r--r--   0        0        0     6080 2024-05-03 07:38:10.843078 bbb_client-0.1.0/bbb_client/domain/meeting_management/model.py
--rw-r--r--   0        0        0     1747 2024-05-03 07:38:10.843078 bbb_client-0.1.0/bbb_client/entry_points.py
--rw-r--r--   0        0        0      738 2024-05-03 07:38:10.843078 bbb_client-0.1.0/bbb_client/infrastructure/__init__.py
--rw-r--r--   0        0        0      738 2024-05-03 07:38:10.843078 bbb_client-0.1.0/bbb_client/infrastructure/click/__init__.py
--rw-r--r--   0        0        0     5164 2024-05-03 07:38:10.847077 bbb_client-0.1.0/bbb_client/infrastructure/click/bbb.py
--rw-r--r--   0        0        0     3919 2024-05-03 07:38:10.847077 bbb_client-0.1.0/bbb_client/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0      738 2024-05-03 07:38:10.847077 bbb_client-0.1.0/bbb_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1480 2024-05-03 07:38:10.847077 bbb_client-0.1.0/bbb_client/interfaces/from_terminal.py
--rw-r--r--   0        0        0     2746 2024-05-03 07:38:10.847077 bbb_client-0.1.0/bbb_client/interfaces/to_terminal.py
--rw-r--r--   0        0        0      738 2024-05-03 07:38:10.847077 bbb_client-0.1.0/bbb_client/use_cases/__init__.py
--rw-r--r--   0        0        0     2085 2024-05-03 07:38:10.847077 bbb_client-0.1.0/bbb_client/use_cases/search_meetings.py
--rw-r--r--   0        0        0      940 2024-05-03 07:38:51.014571 bbb_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bbb_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-02-03 08:08:30.797354 bbb_client-0.1.1/COPYING
+-rw-r--r--   0        0        0      824 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/domain/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/domain/meeting_management/__init__.py
+-rw-r--r--   0        0        0     6304 2024-06-03 13:00:59.762048 bbb_client-0.1.1/bbb_client/domain/meeting_management/model.py
+-rw-r--r--   0        0        0     1747 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/entry_points.py
+-rw-r--r--   0        0        0      738 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/infrastructure/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/infrastructure/click/__init__.py
+-rw-r--r--   0        0        0     5233 2024-06-03 12:53:34.712755 bbb_client-0.1.1/bbb_client/infrastructure/click/bbb.py
+-rw-r--r--   0        0        0     4061 2024-05-23 07:59:37.140631 bbb_client-0.1.1/bbb_client/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1480 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/interfaces/from_terminal.py
+-rw-r--r--   0        0        0     2746 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/interfaces/to_terminal.py
+-rw-r--r--   0        0        0      738 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/use_cases/__init__.py
+-rw-r--r--   0        0        0     2085 2024-05-23 07:43:49.185393 bbb_client-0.1.1/bbb_client/use_cases/search_meetings.py
+-rw-r--r--   0        0        0      940 2024-06-03 13:01:51.081279 bbb_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bbb_client-0.1.1/PKG-INFO
```

### Comparing `bbb_client-0.1.0/COPYING` & `bbb_client-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/__init__.py` & `bbb_client-0.1.1/bbb_client/__init__.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/domain/__init__.py` & `bbb_client-0.1.1/bbb_client/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/domain/meeting_management/__init__.py` & `bbb_client-0.1.1/bbb_client/domain/meeting_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/domain/meeting_management/model.py` & `bbb_client-0.1.1/bbb_client/domain/meeting_management/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     createTime: UnixTimestamp
     startTime: UnixTimestamp
     endTime: UnixTimestamp
     attendeePW: str
     moderatorPW: str
     duration: int
     participantCount: int
+    participants: list[str]
     maxUsers: int
     voiceBridge: str
 
 
 @dataclass()
 class MeetingFilters:
     voiceBridge: Optional[str] = ""
@@ -119,24 +120,30 @@
             raise ChecksumError()
         raise Exception(xml)
 
     def __is_success(self, element: untangle.Element) -> bool:
         return bool(element.response.returncode.cdata == "SUCCESS")
 
     def __element_to_meeting_info(self, element: Any) -> MeetingInfo:
+        try:
+            participants = [a.fullName.cdata for a in element.attendees.attendee]
+        except AttributeError:
+            participants = []
+
         return MeetingInfo(
             meetingName=element.meetingName.cdata,
             meetingID=element.meetingID.cdata,
             createTime=element.createTime.cdata,
             startTime=element.startTime.cdata,
             endTime=element.endTime.cdata,
             attendeePW=element.attendeePW.cdata,
             moderatorPW=element.moderatorPW.cdata,
             duration=element.duration.cdata,
             participantCount=element.participantCount.cdata,
+            participants=participants,
             maxUsers=element.maxUsers.cdata,
             voiceBridge=element.voiceBridge.cdata,
         )
 
     def create_meeting(
         self,
         a_meeting_id: str,
```

### Comparing `bbb_client-0.1.0/bbb_client/entry_points.py` & `bbb_client-0.1.1/bbb_client/entry_points.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/infrastructure/__init__.py` & `bbb_client-0.1.1/bbb_client/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/infrastructure/click/__init__.py` & `bbb_client-0.1.1/bbb_client/infrastructure/click/__init__.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/infrastructure/click/bbb.py` & `bbb_client-0.1.1/bbb_client/infrastructure/click/bbb.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,15 +143,16 @@
     """Show information for a given meeting."""
 
     bbb: Bbb = ctx.obj["bbb"]
     try:
         info = bbb.meeting_info(id)
         click.echo(f'Name: "{info.meetingName}"')
         click.echo(f"ID: {info.meetingID}")
-        click.echo(f"Participants: {info.participantCount}")
+        participants = ", ".join(info.participants)
+        click.echo(f"Participants: {info.participantCount} ({participants})")
         click.echo(f"Audio-conf. PIN: {info.voiceBridge}")
     except MeetingDoesNotExist:
         click.echo(f"[ER] Meeting '{id}' does not exist!")
 
 
 @meetings.command()
 @click.argument("id")
```

### Comparing `bbb_client-0.1.0/bbb_client/infrastructure/requests/__init__.py` & `bbb_client-0.1.1/bbb_client/infrastructure/requests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 class AccessForbidden(BbbException):
     def __init__(self, url: str):
         super().__init__("Access forbidden! Make sure your secret is correct.")
         self.url = url
 
 
 class RequestsBbbApi(BbbApi):
+    """Class defining methods for low level interactions with a BBB API.
+
+    See: <https://docs.bigbluebutton.org/development/api>.
+    """
+
     def __init__(self, an_url: str, a_secret: str) -> None:
         self.__url = an_url
         self.__secret = a_secret
 
     def get_meetings(self) -> str:
         return self.__get_xml(self.__build_url("getMeetings"))
```

### Comparing `bbb_client-0.1.0/bbb_client/interfaces/__init__.py` & `bbb_client-0.1.1/bbb_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/interfaces/from_terminal.py` & `bbb_client-0.1.1/bbb_client/interfaces/from_terminal.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/interfaces/to_terminal.py` & `bbb_client-0.1.1/bbb_client/interfaces/to_terminal.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/use_cases/__init__.py` & `bbb_client-0.1.1/bbb_client/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/bbb_client/use_cases/search_meetings.py` & `bbb_client-0.1.1/bbb_client/use_cases/search_meetings.py`

 * *Files identical despite different names*

### Comparing `bbb_client-0.1.0/pyproject.toml` & `bbb_client-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbb-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "Client library and CLI to interact with the BBB API"
 authors = [
     "Tanguy Le Carrour <tlecarrour@easter-eggs.com>",
     "Loïc Dachary <ldachary@easter-eggs.com>",
 ]
 license = "GPL-3.0-or-later"
```

### Comparing `bbb_client-0.1.0/PKG-INFO` & `bbb_client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Client library and CLI to interact with the BBB API
 License: GPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tlecarrour@easter-eggs.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

