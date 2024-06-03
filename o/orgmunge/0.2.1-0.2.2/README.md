# Comparing `tmp/orgmunge-0.2.1.tar.gz` & `tmp/orgmunge-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orgmunge-0.2.1.tar", max compression
+gzip compressed data, was "orgmunge-0.2.2.tar", max compression
```

## Comparing `orgmunge-0.2.1.tar` & `orgmunge-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-11-27 03:09:11.255033 orgmunge-0.2.1/LICENSE
--rw-r--r--   0        0        0    15857 2023-12-06 15:23:58.116040 orgmunge-0.2.1/README.org
--rw-r--r--   0        0        0      489 2024-04-03 02:30:19.002869 orgmunge-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-27 03:09:14.538358 orgmunge-0.2.1/src/orgmunge/Untitled Document
--rw-r--r--   0        0        0     9200 2024-03-24 20:22:14.487212 orgmunge-0.2.1/src/orgmunge/__init__.py
--rw-r--r--   0        0        0    29904 2023-12-06 15:23:58.116040 orgmunge-0.2.1/src/orgmunge/classes.py
--rw-r--r--   0        0        0     2802 2023-11-27 03:09:14.731691 orgmunge-0.2.1/src/orgmunge/lexer.py
--rw-r--r--   0        0        0    88741 2024-03-24 20:17:20.317781 orgmunge-0.2.1/src/orgmunge/parser.out
--rw-r--r--   0        0        0     6785 2024-03-24 20:21:57.743911 orgmunge-0.2.1/src/orgmunge/parser.py
--rw-r--r--   0        0        0    17283 2024-03-24 20:17:20.314448 orgmunge-0.2.1/src/orgmunge/parsetab.py
--rw-r--r--   0        0        0      180 2023-11-27 03:09:14.741690 orgmunge-0.2.1/src/orgmunge/todos.json
--rw-r--r--   0        0        0    16379 1970-01-01 00:00:00.000000 orgmunge-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-11-28 04:02:21.453022 orgmunge-0.2.2/LICENSE
+-rw-r--r--   0        0        0    16304 2024-05-25 04:17:09.471674 orgmunge-0.2.2/README.org
+-rw-r--r--   0        0        0      489 2024-06-03 14:55:15.370791 orgmunge-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-28 04:02:21.457955 orgmunge-0.2.2/src/orgmunge/Untitled Document
+-rw-r--r--   0        0        0     9200 2023-11-28 04:02:21.458597 orgmunge-0.2.2/src/orgmunge/__init__.py
+-rw-r--r--   0        0        0    30814 2024-05-25 04:01:21.339799 orgmunge-0.2.2/src/orgmunge/classes.py
+-rw-r--r--   0        0        0     2802 2023-11-28 04:02:21.460260 orgmunge-0.2.2/src/orgmunge/lexer.py
+-rw-r--r--   0        0        0    88741 2024-03-24 20:17:20.317000 orgmunge-0.2.2/src/orgmunge/parser.out
+-rw-r--r--   0        0        0     6785 2024-03-24 20:21:57.743000 orgmunge-0.2.2/src/orgmunge/parser.py
+-rw-r--r--   0        0        0    17283 2024-03-24 20:17:20.314000 orgmunge-0.2.2/src/orgmunge/parsetab.py
+-rw-r--r--   0        0        0      180 2023-11-28 04:02:21.463027 orgmunge-0.2.2/src/orgmunge/todos.json
+-rw-r--r--   0        0        0    16826 1970-01-01 00:00:00.000000 orgmunge-0.2.2/PKG-INFO
```

### Comparing `orgmunge-0.2.1/LICENSE` & `orgmunge-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orgmunge-0.2.1/README.org` & `orgmunge-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: orgmunge
+Version: 0.2.2
+Summary: Programmatically modify Orgmode documents
+License: MIT
+Author: durableOne 
+Author-email: era31asj@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ply (>=3.11,<4.0)
+Description-Content-Type: text/plain
+
 #+title:Orgmunge
 * Motivation and scope
 Orgmunge was born out of the desire to modify Org documents
 programmatically from within Python. The wonderful [[https://github.com/karlicoss/orgparse][orgparse]] can read
 an Org document into a tree object but doesn't offer an interface to
 modify the tree and write it back to file.
 
@@ -116,65 +132,72 @@
      2) A list of [[*Drawer Objects][Drawers]], if any
      3) Body text, if any
 - Important attributes:
   1. =properties=. This is a dict mapping property names to their
      values. The properties are parsed from the =PROPERTIES= drawer if
      it exists. This attribute can also be set by the user (the value
      supplied must be a dict).
-  2. =headline= returns the heading's headline. This attribute can also
+  2. =inherited_properties=. Same format as the =properties= dict but
+     contains only properties inherited from ancestors.
+  3. =tags= returns a list of all tags (those explicitly defined for
+     this heading and those inherited)
+  4. =headline= returns the heading's headline. This attribute can also
      be set by a user (the value must be a [[*Headline Objects][Headline]] instance).
-  3. =scheduling= is a [[*Scheduling Objects][Scheduling]] object containing information about
+  5. =scheduling= is a [[*Scheduling Objects][Scheduling]] object containing information about
      =SCHEDULED/DEADLINE/CLOSED= timestamps of the heading, if any. Can
      also be set by the user (the value must be a Scheduling instance).
-  4. =drawers= is a list of [[*Drawer Objects][Drawer]] objects containing the drawers
+  6. =drawers= is a list of [[*Drawer Objects][Drawer]] objects containing the drawers
      associated with this heading. When you update the heading's
      =properties= attribute, the =PROPERTIES= drawer is updated the next
      time you access it.
-  5. =children= returns a list of Heading objects that are the direct
+  7. =children= returns a list of Heading objects that are the direct
      children of this heading.
-  6. =parent= returns the parent heading of the current one. If the
+  8. =parent= returns the parent heading of the current one. If the
      current heading is a top-level heading, the root heading will be
      returned.
-  7. =sibling= returns the sibling heading of the current one that comes
+  9. =sibling= returns the sibling heading of the current one that comes
      before it in the tree, if any. The reason this is the sibling
      heading that is formally tracked is because it's the one that
      would adopt the current heading whenever the current heading is
      demoted. If you want a list of all siblings of the current
      heading, you can do this:
      #+begin_src python
        siblings = [c for c in current_heading.parent.children if c is not current_heading]
      #+end_src
-  8. =level= is the heading's level, with 1 being the top level and each
-     sub-level after that being incremented by 1 (the heading's level
-     is the number of "stars" before its headline).
+  10. =level= is the heading's level, with 1 being the top level and each
+      sub-level after that being incremented by 1 (the heading's level
+      is the number of "stars" before its headline).
 - Important methods:
   1. =clocking=. This returns a list of [[*Clocking Objects][Clocking]] objects, parsed
      from the heading's =LOGBOOK= drawer, if any. You can also pass the
      optional boolean parameter =include_children=, which, when True,
      includes clocking information of this heading's children as well.
-  2. =add_child= accepts a Heading object to add as a child to the
+  2. =get_all_properties=. This returns a dict of all properties of the
+     heading, whether directly defined or inherited from the heading's
+     ancestors. The latest-defined value of a property wins over. 
+  3. =add_child= accepts a Heading object to add as a child to the
      current heading. The optional boolean parameter =new= should be set
      to =True= when this is a new heading that was created and needs to
      be assigned a parent. It should be set to =False= (default) when
      the addition of a child is due to a promotion/demotion operation.
-  3. =remove_child= accepts a heading object and deletes it from the
+  4. =remove_child= accepts a heading object and deletes it from the
      current heading's children if it's a child of the current
      heading.
-  4. =promote= promotes the current heading one level. If the heading has
+  5. =promote= promotes the current heading one level. If the heading has
      children, they would be orphaned so this raises a
      =ValueError=. Technically, Org allows you to have, say, level 3
      headings under a level 1 heading, but =orgmunge= does not allow
      this to make parsing the tree easier.
-  5. =promote_tree= promotes the current heading and all its
+  6. =promote_tree= promotes the current heading and all its
      descendants. Use this if the heading you want to promote has
      children.
-  6. =demote= demotes the current heading one level. If the current
+  7. =demote= demotes the current heading one level. If the current
      heading has no sibling to adopt it, the demotion attempt fails
      and raises a =ValueError=.
-  7. =demote_tree= is the equivalent of =promote_tree= for demotion.
+  8. =demote_tree= is the equivalent of =promote_tree= for demotion.
 *** Headline Objects
 - Important attributes:
   1. =done= is a boolean attribute that determines whether the headline
      is in one of the done states. You can't set this attribute directly.
   2. =level= is the headline's level (the number of "stars" before the
      title)
   3. =comment= is a boolean attribute that determines whether a headline
@@ -318,7 +341,8 @@
 CLOCK: [2023-07-08 Sat 15:54]--[2023-07-08 Sat 15:54] =>  0:00
 :END:
 Thanks to these wonderful people for contributing time and code:
 
 - [[https://github.com/Nalisarc][Nalisarc]]
 - [[https://github.com/ispringle][ispringle]]
 - [[https://github.com/crdoconnor][crdoconnor]]
+
```

### Comparing `orgmunge-0.2.1/src/orgmunge/__init__.py` & `orgmunge-0.2.2/src/orgmunge/__init__.py`

 * *Files identical despite different names*

### Comparing `orgmunge-0.2.1/src/orgmunge/classes.py` & `orgmunge-0.2.2/src/orgmunge/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,14 @@
         return f'[#{self.priority}]' if self.priority is not None else ''
             
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         else:
             return str(self) == str(other)
-
 class Headline:
     def __init__(self, todos, level: str, comment: bool = False,
                todo: Optional[str] = None, priority: Optional[str] = None,
                title: str = "", cookie: Optional[str] = None, tags: Optional[List[str]] = None):
         self._level = len(re.sub(r'\s+', '', level)) # Number of leading asterisks
         self._comment = comment
         self._todo = todo
@@ -155,18 +154,18 @@
         return self._is_done()
 
     @done.setter
     def done(self, _):
         raise AttributeError("Can't set the 'done' attribute")
 
     def _is_done(self):
-        if self.todo in self._done_states:
-            return True
-        elif self.todo is None or self.todo in self._todo_states:
+        if self.todo is None or self.todo in self._todo_states:
             return False
+        elif self.todo in self._done_states:
+            return True
         else:
             raise ValueError(f"Uncategorized todo state {self.todo}")
 
     @property
     def level(self):
         return self._level
 
@@ -248,15 +247,14 @@
         return f"{'*' * self.level} {todo}{comment}{priority}{self.title}{cookie}{tags}"
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         else:
             return str(self) == str(other)
-
 class TimeStamp:
     def __init__(self, timestamp_str: str):
         is_active = re.search(Lexer.ATIMESTAMP, timestamp_str)
         is_inactive = re.search(Lexer.ITIMESTAMP, timestamp_str)
         self._active = True if is_active else False
         match = is_active if self._active else is_inactive
         date, day_of_week, start_time, end_time, repeater, deadline_warn = match.groups()
@@ -372,15 +370,14 @@
         return ldelim + timestamp + rdelim
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         else:
             return str(self) == str(other)
-
 class Scheduling:
     _closed = None
     _scheduled = None
     _deadline = None
 
     # Helper class to group together common getter and setter code for all keywords
     class Keyword:
@@ -438,15 +435,14 @@
         return ' '.join(data)
         
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         else:
             return str(self) == str(other)
-
 class Drawer:
     def __init__(self, drawer_string: str):
         self.name = re.sub(r':', '', drawer_string.split('\n')[0])
         self.contents = drawer_string.strip().split('\n')[1:-1]
     def __repr__(self):
         contents = "\n".join(self.contents)
         return f''':{self.name}:
@@ -454,15 +450,14 @@
 :END:
 '''    
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         else:
             return str(self) == str(other)
-        
 class Clocking:
     def __init__(self, start_time: str, end_time: Optional[str] = None):
         self._start_time = dt.strptime(start_time, ORG_TIME_FORMAT)
         if end_time is not None:
             self._end_time = dt.strptime(end_time, ORG_TIME_FORMAT)
         else:
             self._end_time = None
@@ -522,22 +517,22 @@
             return f'[{self.start_time.strftime(ORG_TIME_FORMAT)}]--[{self.end_time.strftime(ORG_TIME_FORMAT)}] =>  {self.duration}'
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         else:
             return str(self) == str(other)
-
 class Heading():
     def __init__(self, headline: Headline, contents: Tuple[Scheduling, List[Drawer], str]):
         self._headline = headline
         self._scheduling, self._drawers, self.body = contents
         self._children = []
         self._parent = None
         self._sibling = None
+        self._inherited_properties = dict()
         if self.body:
             self.timestamps = [TimeStamp(t[0]) for t in re.findall(fr'({Lexer.ATIMESTAMP}|{Lexer.ITIMESTAMP})', self.body)]
         if self._drawers:
             properties_drawer = [d for d in self._drawers if d.name == 'PROPERTIES']
             if properties_drawer:
                 self._properties = self._get_properties_dict(properties_drawer[0].contents)
             else:
@@ -577,26 +572,50 @@
         return {k: v for (k, v) in [re.search(r':([^:]+):\s+(.*)', line).groups()
                                     for line in contents]} 
 
     def _get_properties_string(self) -> str:
         return "\n".join([f":{k}:{' '*7}{v}" for k, v in self.properties.items()])
 
     @property
+    def inherited_properties(self):
+        if not self._inherited_properties:
+            if self.parent:
+                self._inherited_properties = {**self.parent.inherited_properties, **self.parent.properties}
+        return self._inherited_properties
+
+    @inherited_properties.setter
+    def inherited_properties(self, _):
+        raise AttributeError("Can't set the inherited properties of a heading")
+    
+    @property
+    def tags(self):
+        self_tags = self.headline.tags or []
+        parent_tags = (self.parent.tags if self.parent else None) or []
+        return list(set(self_tags + parent_tags))
+
+    @tags.setter
+    def tags(self, _):
+        raise AttributeError("Can't set the tags of a heading, use headline instead.")
+    
+    @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, val: Dict[str, str]):
         if type(val) is not dict:
             raise TypeError("Heading properties must be given in the form of a dict")
         else:
             self._properties = dict()
             for key in val:
                 self._properties[key] = val[key]
 
+    def get_all_properties(self) -> Dict[str, str]:
+        return {**self.inherited_properties, **self.properties}
+
     def clocking(self, include_children: bool = False) -> List[Clocking]:
         "Return the clocking information of the given headline and possibly its children."
         own_clocking = self._get_clocking_info()
         if include_children and self.children != []:
             return own_clocking + reduce(add, [c.clocking(include_children=True) for c in self.children])
         else:
             return own_clocking
```

### Comparing `orgmunge-0.2.1/src/orgmunge/lexer.py` & `orgmunge-0.2.2/src/orgmunge/lexer.py`

 * *Files identical despite different names*

### Comparing `orgmunge-0.2.1/src/orgmunge/parser.out` & `orgmunge-0.2.2/src/orgmunge/parser.out`

 * *Files identical despite different names*

### Comparing `orgmunge-0.2.1/src/orgmunge/parser.py` & `orgmunge-0.2.2/src/orgmunge/parser.py`

 * *Files identical despite different names*

### Comparing `orgmunge-0.2.1/src/orgmunge/parsetab.py` & `orgmunge-0.2.2/src/orgmunge/parsetab.py`

 * *Files identical despite different names*

### Comparing `orgmunge-0.2.1/PKG-INFO` & `orgmunge-0.2.2/README.org`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: orgmunge
-Version: 0.2.1
-Summary: Programmatically modify Orgmode documents
-License: MIT
-Author: durableOne 
-Author-email: era31asj@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ply (>=3.11,<4.0)
-Description-Content-Type: text/plain
-
 #+title:Orgmunge
 * Motivation and scope
 Orgmunge was born out of the desire to modify Org documents
 programmatically from within Python. The wonderful [[https://github.com/karlicoss/orgparse][orgparse]] can read
 an Org document into a tree object but doesn't offer an interface to
 modify the tree and write it back to file.
 
@@ -132,65 +116,72 @@
      2) A list of [[*Drawer Objects][Drawers]], if any
      3) Body text, if any
 - Important attributes:
   1. =properties=. This is a dict mapping property names to their
      values. The properties are parsed from the =PROPERTIES= drawer if
      it exists. This attribute can also be set by the user (the value
      supplied must be a dict).
-  2. =headline= returns the heading's headline. This attribute can also
+  2. =inherited_properties=. Same format as the =properties= dict but
+     contains only properties inherited from ancestors.
+  3. =tags= returns a list of all tags (those explicitly defined for
+     this heading and those inherited)
+  4. =headline= returns the heading's headline. This attribute can also
      be set by a user (the value must be a [[*Headline Objects][Headline]] instance).
-  3. =scheduling= is a [[*Scheduling Objects][Scheduling]] object containing information about
+  5. =scheduling= is a [[*Scheduling Objects][Scheduling]] object containing information about
      =SCHEDULED/DEADLINE/CLOSED= timestamps of the heading, if any. Can
      also be set by the user (the value must be a Scheduling instance).
-  4. =drawers= is a list of [[*Drawer Objects][Drawer]] objects containing the drawers
+  6. =drawers= is a list of [[*Drawer Objects][Drawer]] objects containing the drawers
      associated with this heading. When you update the heading's
      =properties= attribute, the =PROPERTIES= drawer is updated the next
      time you access it.
-  5. =children= returns a list of Heading objects that are the direct
+  7. =children= returns a list of Heading objects that are the direct
      children of this heading.
-  6. =parent= returns the parent heading of the current one. If the
+  8. =parent= returns the parent heading of the current one. If the
      current heading is a top-level heading, the root heading will be
      returned.
-  7. =sibling= returns the sibling heading of the current one that comes
+  9. =sibling= returns the sibling heading of the current one that comes
      before it in the tree, if any. The reason this is the sibling
      heading that is formally tracked is because it's the one that
      would adopt the current heading whenever the current heading is
      demoted. If you want a list of all siblings of the current
      heading, you can do this:
      #+begin_src python
        siblings = [c for c in current_heading.parent.children if c is not current_heading]
      #+end_src
-  8. =level= is the heading's level, with 1 being the top level and each
-     sub-level after that being incremented by 1 (the heading's level
-     is the number of "stars" before its headline).
+  10. =level= is the heading's level, with 1 being the top level and each
+      sub-level after that being incremented by 1 (the heading's level
+      is the number of "stars" before its headline).
 - Important methods:
   1. =clocking=. This returns a list of [[*Clocking Objects][Clocking]] objects, parsed
      from the heading's =LOGBOOK= drawer, if any. You can also pass the
      optional boolean parameter =include_children=, which, when True,
      includes clocking information of this heading's children as well.
-  2. =add_child= accepts a Heading object to add as a child to the
+  2. =get_all_properties=. This returns a dict of all properties of the
+     heading, whether directly defined or inherited from the heading's
+     ancestors. The latest-defined value of a property wins over. 
+  3. =add_child= accepts a Heading object to add as a child to the
      current heading. The optional boolean parameter =new= should be set
      to =True= when this is a new heading that was created and needs to
      be assigned a parent. It should be set to =False= (default) when
      the addition of a child is due to a promotion/demotion operation.
-  3. =remove_child= accepts a heading object and deletes it from the
+  4. =remove_child= accepts a heading object and deletes it from the
      current heading's children if it's a child of the current
      heading.
-  4. =promote= promotes the current heading one level. If the heading has
+  5. =promote= promotes the current heading one level. If the heading has
      children, they would be orphaned so this raises a
      =ValueError=. Technically, Org allows you to have, say, level 3
      headings under a level 1 heading, but =orgmunge= does not allow
      this to make parsing the tree easier.
-  5. =promote_tree= promotes the current heading and all its
+  6. =promote_tree= promotes the current heading and all its
      descendants. Use this if the heading you want to promote has
      children.
-  6. =demote= demotes the current heading one level. If the current
+  7. =demote= demotes the current heading one level. If the current
      heading has no sibling to adopt it, the demotion attempt fails
      and raises a =ValueError=.
-  7. =demote_tree= is the equivalent of =promote_tree= for demotion.
+  8. =demote_tree= is the equivalent of =promote_tree= for demotion.
 *** Headline Objects
 - Important attributes:
   1. =done= is a boolean attribute that determines whether the headline
      is in one of the done states. You can't set this attribute directly.
   2. =level= is the headline's level (the number of "stars" before the
      title)
   3. =comment= is a boolean attribute that determines whether a headline
@@ -334,8 +325,7 @@
 CLOCK: [2023-07-08 Sat 15:54]--[2023-07-08 Sat 15:54] =>  0:00
 :END:
 Thanks to these wonderful people for contributing time and code:
 
 - [[https://github.com/Nalisarc][Nalisarc]]
 - [[https://github.com/ispringle][ispringle]]
 - [[https://github.com/crdoconnor][crdoconnor]]
-
```

