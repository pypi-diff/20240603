# Comparing `tmp/mutt_html_reply-0.4.2.tar.gz` & `tmp/mutt_html_reply-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutt_html_reply-0.4.2.tar", last modified: Sat Jun  1 02:32:55 2024, max compression
+gzip compressed data, was "mutt_html_reply-0.4.3.tar", last modified: Mon Jun  3 01:21:28 2024, max compression
```

## Comparing `mutt_html_reply-0.4.2.tar` & `mutt_html_reply-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 02:32:55.748567 mutt_html_reply-0.4.2/
--rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.4.2/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-06-01 02:32:55.748567 mutt_html_reply-0.4.2/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      807 2024-05-30 03:23:26.000000 mutt_html_reply-0.4.2/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-06-01 02:32:36.000000 mutt_html_reply-0.4.2/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-06-01 02:32:55.748567 mutt_html_reply-0.4.2/setup.cfg
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 02:32:55.748567 mutt_html_reply-0.4.2/src/
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 02:32:55.748567 mutt_html_reply-0.4.2/src/mutt_html_reply/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.4.2/src/mutt_html_reply/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4980 2024-06-01 02:24:13.000000 mutt_html_reply-0.4.2/src/mutt_html_reply/mutt_html_reply.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 02:32:55.748567 mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-06-01 02:32:55.000000 mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-06-01 02:32:55.000000 mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-06-01 02:32:55.000000 mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-06-01 02:32:55.000000 mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-06-01 02:32:55.000000 mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-06-01 02:32:55.000000 mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-03 01:21:28.490952 mutt_html_reply-0.4.3/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.4.3/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-06-03 01:21:28.490952 mutt_html_reply-0.4.3/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      807 2024-05-30 03:23:26.000000 mutt_html_reply-0.4.3/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-06-03 01:20:59.000000 mutt_html_reply-0.4.3/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-06-03 01:21:28.490952 mutt_html_reply-0.4.3/setup.cfg
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-03 01:21:28.490952 mutt_html_reply-0.4.3/src/
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-03 01:21:28.490952 mutt_html_reply-0.4.3/src/mutt_html_reply/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.4.3/src/mutt_html_reply/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     6034 2024-06-03 01:20:59.000000 mutt_html_reply-0.4.3/src/mutt_html_reply/mutt_html_reply.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-03 01:21:28.490952 mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-06-03 01:21:28.000000 mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-06-03 01:21:28.000000 mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-06-03 01:21:28.000000 mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-06-03 01:21:28.000000 mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-06-03 01:21:28.000000 mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-06-03 01:21:28.000000 mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/top_level.txt
```

### Comparing `mutt_html_reply-0.4.2/LICENSE` & `mutt_html_reply-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.4.2/PKG-INFO` & `mutt_html_reply-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.4.2
+Version: 0.4.3
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `mutt_html_reply-0.4.2/README.md` & `mutt_html_reply-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.4.2/pyproject.toml` & `mutt_html_reply-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mutt-html-reply"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
 	"bs4",
 	"css_inline"
 ]
 authors = [
 	{name = "Erik Rogers", email = "erik@rogers-family.net"}
 ]
```

### Comparing `mutt_html_reply-0.4.2/src/mutt_html_reply/mutt_html_reply.py` & `mutt_html_reply-0.4.3/src/mutt_html_reply/mutt_html_reply.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import argparse
+import datetime
+from zoneinfo import ZoneInfo
 import email
 from email.header import decode_header
 import html
 import sys
 from bs4 import BeautifulSoup, Doctype
 import css_inline
 
@@ -23,24 +25,29 @@
                         default=sys.stdin,
                         help="HTML reply, file or defaults to stdin")
     parser.add_argument("-o", "--output",
                         nargs='?',
                         type=argparse.FileType('w'),
                         default=sys.stdout,
                         help="HTML output, file or defaults to stdout")
+    parser.add_argument("-z", "--zoneinfo",
+                        nargs='?',
+                        type=str,
+                        default="America/New_York",
+                        help="ZoneInfo for header display, defaults to 'America/New_York'")
 
     args = parser.parse_args()
 
     # Get the reply html from file/stdin
     html_reply = args.reply.read()
 
     # Get the original headers and html from the original email (rfc822 format)
     rfc822_original = email.message_from_file(args.message)
     html_original_msg = _get_message_html(rfc822_original)
-    html_original_headers = _get_header_html(rfc822_original)
+    html_original_headers = _get_header_html(rfc822_original, args.zoneinfo)
 
     # Convert HTML text to BeautifulSoup object and inline all CSS
 
     ## reply
     bs4_msg = BeautifulSoup(css_inline.inline(html_reply),'html.parser')
 
     ## message
@@ -62,33 +69,47 @@
     bs4_final.body.append(BeautifulSoup('<br></br>', 'html.parser')) #type: ignore
     bs4_final.body.append(bs4_original_msg) #type: ignore
 
     # Write output
     args.output.write(str(bs4_final))
 
 
-def _get_header_html(message):
+def _get_header_html(message, tz_str):
     headers = '''\
         <div>
         <div style=&quot;border:none;border-top:solid;padding:3.0pt 0in 0in 0in&quot;>
         <span style=font-size:11.0pt;font-family:&quot;Calibri&quot;,sans-serif>
         '''
     if message['from'] is not None:
         headers = headers + '<b>From:</b> ' + html.escape(message['from'].replace('"','')) + '<br></br>'
     if message['date'] is not None:
-        headers = headers + '<b>Sent:</b> ' + html.escape(message['date'].replace('"','')) + '<br></br>'
+        # Try to make it pretty
+        try:
+            header_date = datetime.datetime.strptime(html.escape(message['date'].replace('"','')),'%a, %d %b %Y %H:%M:%S%z').astimezone(ZoneInfo(tz_str))
+            header_date = str(header_date.strftime('%A, %B %d, %Y %I:%M %p'))
+        except:
+            pass
+        try:
+            header_date = datetime.datetime.strptime(html.escape(message['date'].replace('"','')),'%a, %d %b %Y %H:%M:%S %z').astimezone(ZoneInfo("America/New_York"))
+            header_date = str(header_date.strftime('%A, %B %d, %Y %I:%M %p'))
+        except:
+            header_date = message['date']
+        headers = headers + '<b>Sent:</b> ' + header_date +'<br></br>'
     if message['to'] is not None:
         headers = headers + '<b>To:</b> ' + html.escape(message['to'].replace('"','')) + '<br></br>'
     if message['cc'] is not None:
         headers = headers + '<b>Cc:</b> ' + html.escape(message['cc'].replace('"','')) + '<br></br>'
     if message['subject'] is not None:
         decoded_subject_list = decode_header(message['subject'])
         first_subject_line = decoded_subject_list[0]
-        decoded_subject = first_subject_line[0].decode(first_subject_line[1])
-        headers = headers + '<b>Subject:</b> ' + html.escape(decoded_subject) + '<br></br>'
+        try:
+            decoded_subject = first_subject_line[0].decode(first_subject_line[1])
+            headers = headers + '<b>Subject:</b> ' + html.escape(decoded_subject) + '<br></br>'
+        except:
+            headers = headers + '<b>Subject:</b> ' + html.escape(message['subject']) + '<br></br>'
 
     headers = headers + '''\
         </span>
         </div>
         </div>
         '''
```

### Comparing `mutt_html_reply-0.4.2/src/mutt_html_reply.egg-info/PKG-INFO` & `mutt_html_reply-0.4.3/src/mutt_html_reply.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.4.2
+Version: 0.4.3
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

