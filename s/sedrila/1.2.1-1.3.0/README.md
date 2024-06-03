# Comparing `tmp/sedrila-1.2.1.tar.gz` & `tmp/sedrila-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedrila-1.2.1.tar", max compression
+gzip compressed data, was "sedrila-1.3.0.tar", max compression
```

## Comparing `sedrila-1.2.1.tar` & `sedrila-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-1.2.1/LICENSE
--rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-1.2.1/README.md
--rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-1.2.1/baseresources/favicon-32x32.png
--rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-1.2.1/baseresources/local.css
--rwxr-xr-x   0        0        0     7882 2024-04-04 09:44:27.185644 sedrila-1.2.1/baseresources/sedrila.css
--rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-1.2.1/baseresources/sidebar.js
--rwxr-xr-x   0        0        0     6616 2024-05-31 11:06:56.667135 sedrila-1.2.1/py/base.py
--rwxr-xr-x   0        0        0     3501 2024-04-09 14:20:20.887078 sedrila-1.2.1/py/git.py
--rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-1.2.1/py/sdrl/__init__.py
--rwxr-xr-x   0        0        0    23686 2024-05-31 10:51:06.427633 sedrila-1.2.1/py/sdrl/course.py
--rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-1.2.1/py/sdrl/glossary.py
--rwxr-xr-x   0        0        0     1209 2024-03-28 09:55:55.453116 sedrila-1.2.1/py/sdrl/html.py
--rwxr-xr-x   0        0        0     3990 2024-05-29 16:50:08.943081 sedrila-1.2.1/py/sdrl/interactive.py
--rwxr-xr-x   0        0        0     8393 2024-05-14 17:35:25.529976 sedrila-1.2.1/py/sdrl/macros.py
--rwxr-xr-x   0        0        0     4154 2024-05-14 17:35:25.184525 sedrila-1.2.1/py/sdrl/markdown.py
--rwxr-xr-x   0        0        0     6222 2024-04-09 14:20:22.676239 sedrila-1.2.1/py/sdrl/part.py
--rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-1.2.1/py/sdrl/participant.py
--rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-1.2.1/py/sdrl/replacements.py
--rwxr-xr-x   0        0        0     8344 2024-04-02 17:08:18.901707 sedrila-1.2.1/py/sdrl/repo.py
--rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-1.2.1/py/sdrl/subcmd/__init__.py
--rwxr-xr-x   0        0        0    28479 2024-05-01 09:55:22.353458 sedrila-1.2.1/py/sdrl/subcmd/author.py
--rwxr-xr-x   0        0        0     9005 2024-04-22 15:45:50.721474 sedrila-1.2.1/py/sdrl/subcmd/instructor.py
--rwxr-xr-x   0        0        0     5915 2024-05-14 18:01:22.555644 sedrila-1.2.1/py/sdrl/subcmd/student.py
--rwxr-xr-x   0        0        0      975 2024-02-24 16:55:02.006852 sedrila-1.2.1/py/sedrila.py
--rwxr-xr-x   0        0        0     2329 2024-05-31 11:06:56.678101 sedrila-1.2.1/pyproject.toml
--rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-1.2.1/templates/base.html
--rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-1.2.1/templates/chapter.html
--rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-1.2.1/templates/glossary.html
--rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-1.2.1/templates/homepage.html
--rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-1.2.1/templates/task.html
--rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-1.2.1/templates/taskgroup.html
--rw-r--r--   0        0        0    11173 1970-01-01 00:00:00.000000 sedrila-1.2.1/setup.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-1.3.0/LICENSE
+-rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-1.3.0/README.md
+-rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-1.3.0/baseresources/favicon-32x32.png
+-rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-1.3.0/baseresources/local.css
+-rwxr-xr-x   0        0        0     7882 2024-04-04 09:44:27.185644 sedrila-1.3.0/baseresources/sedrila.css
+-rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-1.3.0/baseresources/sidebar.js
+-rwxr-xr-x   0        0        0     6795 2024-06-03 15:22:08.990112 sedrila-1.3.0/py/base.py
+-rwxr-xr-x   0        0        0     3501 2024-04-09 14:20:20.887078 sedrila-1.3.0/py/git.py
+-rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-1.3.0/py/sdrl/__init__.py
+-rwxr-xr-x   0        0        0    23640 2024-06-03 11:07:08.234232 sedrila-1.3.0/py/sdrl/course.py
+-rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-1.3.0/py/sdrl/glossary.py
+-rwxr-xr-x   0        0        0     1209 2024-03-28 09:55:55.453116 sedrila-1.3.0/py/sdrl/html.py
+-rwxr-xr-x   0        0        0     3990 2024-05-29 16:50:08.943081 sedrila-1.3.0/py/sdrl/interactive.py
+-rwxr-xr-x   0        0        0     8393 2024-05-14 17:35:25.529976 sedrila-1.3.0/py/sdrl/macros.py
+-rwxr-xr-x   0        0        0     4154 2024-05-14 17:35:25.184525 sedrila-1.3.0/py/sdrl/markdown.py
+-rwxr-xr-x   0        0        0     6348 2024-06-03 14:50:18.720853 sedrila-1.3.0/py/sdrl/part.py
+-rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-1.3.0/py/sdrl/participant.py
+-rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-1.3.0/py/sdrl/replacements.py
+-rwxr-xr-x   0        0        0     8344 2024-04-02 17:08:18.901707 sedrila-1.3.0/py/sdrl/repo.py
+-rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-1.3.0/py/sdrl/subcmd/__init__.py
+-rwxr-xr-x   0        0        0    29819 2024-06-03 13:06:16.449911 sedrila-1.3.0/py/sdrl/subcmd/author.py
+-rwxr-xr-x   0        0        0     9005 2024-04-22 15:45:50.721474 sedrila-1.3.0/py/sdrl/subcmd/instructor.py
+-rwxr-xr-x   0        0        0     5915 2024-05-14 18:01:22.555644 sedrila-1.3.0/py/sdrl/subcmd/student.py
+-rwxr-xr-x   0        0        0      994 2024-06-03 15:15:10.020674 sedrila-1.3.0/py/sedrila.py
+-rwxr-xr-x   0        0        0     2329 2024-06-03 15:22:08.998385 sedrila-1.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-1.3.0/templates/base.html
+-rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-1.3.0/templates/chapter.html
+-rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-1.3.0/templates/glossary.html
+-rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-1.3.0/templates/homepage.html
+-rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-1.3.0/templates/task.html
+-rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-1.3.0/templates/taskgroup.html
+-rw-r--r--   0        0        0    11208 1970-01-01 00:00:00.000000 sedrila-1.3.0/setup.py
+-rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-1.3.0/PKG-INFO
```

### Comparing `sedrila-1.2.1/LICENSE` & `sedrila-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/README.md` & `sedrila-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/baseresources/favicon-32x32.png` & `sedrila-1.3.0/baseresources/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/baseresources/sedrila.css` & `sedrila-1.3.0/baseresources/sedrila.css`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/baseresources/sidebar.js` & `sedrila-1.3.0/baseresources/sidebar.js`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/base.py` & `sedrila-1.3.0/py/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import requests
 import rich
 import rich.table
 import yaml
 
 
-SEDRILA_VERSION = "1.2.1"  # keep in sync with pyproject.toml
+SEDRILA_VERSION = "1.3.0"  # keep in sync with pyproject.toml
 CONFIG_FILENAME = "sedrila.yaml"  # at top-level of source dir
 GLOSSARY_BASENAME = "glossary"  # .md at top-level of chapterdir, .html in build directory
 METADATA_FILE = "course.json"  # at top-level of build directory
 CACHE_FILE = "course.pickle"  # at top-level of instructor build directory
 TEMPLATES_DIR = "templates"
 SEDRILA_COMMAND_ENV = "SEDRILA_COMMAND"
 
@@ -71,27 +71,29 @@
         return [a.strip() for a in attrlist.split(',')]
     mustcopy_names = names_in(mustcopy_attrs)  # mandatory
     cancopy_names = names_in(cancopy_attrs)  # optional
     mustexist_names = names_in(mustexist_attrs)  # further mandatory
     if not source:
         source = dict()
     source_names = set(source.keys())
-    for m in mustcopy_names:  # transport these
-        value = source.get(m, ValueError)
+    for mname in mustcopy_names:  # transport these
+        value = source.get(mname, ValueError)
         if value is ValueError:
-            error(f"{context}: required attribute is missing: {m}")
+            error(f"{context}: required attribute is missing: {mname}")
             exit_if_errors()
         else:
-            mysetattr(target, m, value)
-    for o in cancopy_names:  # transport these if present
-        if o in source:
-            if hasattr(target, o) and not overwrite:
+            mysetattr(target, mname, value)
+    for cname in cancopy_names:  # transport these if present, set them to None if not
+        if cname in source:
+            if hasattr(target, cname) and not overwrite:
                 warning("%s: %soverwriting '%s': old value '%s', new value '%s'" %
-                        (context, "" if overwrite else "not ", o, getattr(target, o), source[o]))
-            mysetattr(target, o, source[o])
+                        (context, "" if overwrite else "not ", cname, getattr(target, cname), source[cname]))
+            mysetattr(target, cname, source[cname])
+        elif cname not in source and not hasattr(target, cname):
+            setattr(target, cname, None)
     extra_attrs = source_names - set(mustcopy_names) - set(cancopy_names) - set(mustexist_names)
     if extra_attrs:
         error(f"{context}: unexpected extra attributes found: {extra_attrs}")
     for attrname, its_type in typecheck.items():
         value = getattr(target, attrname, None)
         if value and not isinstance(value, its_type):
             error(f"'{context}': attribute '{attrname}' should be {str(its_type)} (is '{value}')")
```

### Comparing `sedrila-1.2.1/py/git.py` & `sedrila-1.3.0/py/git.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/course.py` & `sedrila-1.3.0/py/sdrl/course.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,15 @@
       for bookkeeping/reporting.
     """
     configfile: str
     breadcrumb_title: str
     baseresourcedir: str = f"{sedrila_libdir}/baseresources"
     chapterdir: str
     altdir: str
+    itreedir: str|None
     templatedir: str = f"{sedrila_libdir}/templates"
     blockmacro_topmatter: dict[str, str]
     instructors: list[b.StrAnyDict]
     htaccess_template: str = None  # structure of .htaccess file generated in instructor website
     chapters: list['Chapter']
     stages: list[str]  # list of allowed values of stage in parts 
 
@@ -211,27 +212,27 @@
     def __init__(self, configfile: str, read_contentfiles: bool, include_stage: str):
         self.configfile = self.sourcefile = configfile
         configdict = b.slurp_yaml(configfile)
         b.copyattrs(configfile, 
                     configdict, self,
                     mustcopy_attrs=('title, breadcrumb_title, chapterdir, altdir, '
                                     'instructors, stages, allowed_attempts'),
-                    cancopy_attrs=('baseresourcedir, templatedir, '
+                    cancopy_attrs=('baseresourcedir, itreedir, templatedir, '
                                    'blockmacro_topmatter, htaccess_template, init_data'),
                     mustexist_attrs='chapters')
         self.allowed_attempts_base, self.allowed_attempts_hourly = self._parse_allowed_attempts()
         self.slug = self.breadcrumb_title
         self.outputfile = "index.html"
         self.namespace = dict()
         self.namespace_add(configfile, self)
         if read_contentfiles:
             self.read_partsfile(f"{self.chapterdir}/index.md")
             self.glossary = glossary.Glossary(self.chapterdir)
             self.namespace_add("", self.glossary)
-            self.find_zipdirs(self.chapterdir)
+            self.find_zipdirs()
         if include_stage in self.stages:
             self.include_stage = include_stage
             self.include_stage_index = self.stages.index(include_stage)
         else:
             if include_stage != '':  # empty is allowed
                 b.error(f"'--include_stage {include_stage}' not allowed, must be one of {self.stages}")
             self.include_stage = ''  # include only parts with no stage
@@ -266,15 +267,15 @@
             else:
                 result[t.slug] = t
         return result
 
     def as_json(self) -> b.StrAnyDict:
         result = dict(title=self.title,
                       breadcrumb_title=self.breadcrumb_title,
-                      chapterdir="", altdir="",  stages=[],  # are mustcopy_attrs but are not needed
+                      chapterdir="", stages=[],  # are mustcopy_attrs but are not needed
                       instructors=self.instructors,
                       init_data=self.init_data,
                       allowed_attempts=self.allowed_attempts,
                       chapters=[chapter.as_json() for chapter in self.chapters])
         result.update(super().as_json())
         return result
 
@@ -454,15 +455,15 @@
         if read_contentfiles:
             self.read_partsfile(f"{self.course.chapterdir}/{self.slug}/index.md")
             b.copyattrs(context, 
                         self.metadata, self,
                         mustcopy_attrs='title',
                         cancopy_attrs='stage, todo',
                         mustexist_attrs='', overwrite=True)
-            self.find_zipdirs(self.course.chapterdir)
+            self.find_zipdirs()
         self.evaluate_stage(context, course)
         course.namespace_add(self.sourcefile, self)
         self.taskgroups = [Taskgroup(self, taskgroup, read_contentfiles) 
                            for taskgroup in (chapter.get('taskgroups') or [])]
 
     @property
     def breadcrumb_item(self) -> str:
@@ -502,15 +503,15 @@
         if read_contentfiles:
             self.read_partsfile(f"{self.chapter.course.chapterdir}/{self.chapter.slug}/{self.slug}/index.md")
             b.copyattrs(context,
                         self.metadata, self,
                         mustcopy_attrs='title',
                         cancopy_attrs='minimum, stage, todo',
                         mustexist_attrs='', overwrite=True)
-            self.find_zipdirs(self.chapter.course.chapterdir)
+            self.find_zipdirs()
         self.evaluate_stage(context, chapter.course)
         chapter.course.namespace_add(self.sourcefile, self)
         if read_contentfiles:
             self._create_tasks()
         else:
             self.tasks = [Task().from_json(taskdict, taskgroup=self)
                           for taskdict in taskgroupdict['tasks']]
```

### Comparing `sedrila-1.2.1/py/sdrl/glossary.py` & `sedrila-1.3.0/py/sdrl/glossary.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/html.py` & `sedrila-1.3.0/py/sdrl/html.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/interactive.py` & `sedrila-1.3.0/py/sdrl/interactive.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/macros.py` & `sedrila-1.3.0/py/sdrl/macros.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/markdown.py` & `sedrila-1.3.0/py/sdrl/markdown.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/part.py` & `sedrila-1.3.0/py/sdrl/part.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,34 +102,35 @@
 
 
 class Zipdir(Structurepart):
     """
     Turn directories named ch/mychapter/mytaskgroup/myzipdir.zip 
     containing a tree of files, say, myfile.txt
     into an output file myzipdir.zip
-    that contains myzipdir/myfile.txt.  
+    that contains paths like myzipdir/myfile.txt.  
     """
     innerpath: str  # relative pathname of the zipdir, to be re-created in the ZIP archive
 
-    def __init__(self, dirprefix: str, dirname: str, outputdir: str):
-        assert dirname.startswith(dirprefix)
-        assert dirname[-1] != '/'  # dirprefix must not end with a slash, else our logic would break
-        self.sourcefile = dirname
-        self.slug = self.title = self.outputfile = os.path.basename(dirname)  # e.g. myfile.zip
-        self.innerpath = self.slug[:-len(".zip")]  # e.g. myfile
+    def __init__(self, zipdirpath: str):
+        assert zipdirpath[-1] != '/'  # dirprefix must not end with a slash, else our logic would break
+        self.sourcefile = zipdirpath  # e.g. ch/mychapter/mytaskgroup/myzipdir.zip 
+        self.slug = self.title = self.outputfile = os.path.basename(zipdirpath)  # e.g. myzipdir.zip
+        self.innerpath = self.slug[:-len(".zip")]  # e.g. myzipdir
 
     @property
     def to_be_skipped(self) -> bool:
-        return False  # TODO 3: should be skipped if no [PARTREF] to it exists anywhere
+        return False  # TODO 3: within course(!) could be skipped if no [PARTREF] to it exists anywhere
 
     def render(self, targetdir: str):
-        with zipfile.ZipFile(f"{targetdir}/{self.outputfile}", mode='w') as archive:
+        with zipfile.ZipFile(f"{targetdir}/{self.outputfile}", mode='w', 
+                             compression=zipfile.ZIP_DEFLATED) as archive:  # prefer deflate for build speed
             self._zip_the_files(archive)
 
     def _zip_the_files(self, archive: zipfile.ZipFile):
+        assert os.path.exists(self.sourcefile), f"'{self.sourcefile}' is missing!"
         for dirpath, dirnames, filenames in os.walk(self.sourcefile):
             for filename in sorted(filenames):
                 sourcename = f"{dirpath}/{filename}"
                 targetname = self._path_in_zip(sourcename)
                 archive.write(sourcename, targetname)
 
     def _path_in_zip(self, sourcename: str) -> str:
@@ -141,22 +142,21 @@
         return f"{self.innerpath}/{remainder}"
 
 
 class Partscontainer(Structurepart):
     """A Structurepart that can contain other Structureparts."""
     zipdirs: list[Zipdir] = []
     
-    def find_zipdirs(self, dirprefix: str):
-        """find all dirs (not files!) *.zip in inputdir (not below!), warns about *.zip files"""
+    def find_zipdirs(self):
+        """find all dirs (not files!) *.zip in self.sourcefile dir (not below!), warns about *.zip files"""
         self.zipdirs = []
         inputdir = os.path.dirname(self.sourcefile)
-        outputdir = os.path.dirname(self.outputfile)
         zipdirs = glob.glob(f"{inputdir}/*.zip")
-        for dirname in zipdirs:
-            if os.path.isdir(dirname):
-                self.zipdirs.append(Zipdir(dirprefix, dirname, outputdir))
+        for zipdirname in zipdirs:
+            if os.path.isdir(zipdirname):
+                self.zipdirs.append(Zipdir(zipdirname))
             else:
-                b.warning(f"'{dirname}' is a file, not a dir, and will be ignored.")
+                b.warning(f"'{zipdirname}' is a file, not a dir, and will be ignored.")
 
     def render_zipdirs(self, targetdir):
         for zipdir in self.zipdirs:
             zipdir.render(targetdir)
```

### Comparing `sedrila-1.2.1/py/sdrl/participant.py` & `sedrila-1.3.0/py/sdrl/participant.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/replacements.py` & `sedrila-1.3.0/py/sdrl/replacements.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/repo.py` & `sedrila-1.3.0/py/sdrl/repo.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/subcmd/author.py` & `sedrila-1.3.0/py/sdrl/subcmd/author.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     subparser.add_argument('targetdir',
                            help=f"Directory to which output will be written.")
 
 
 def execute(pargs: argparse.Namespace):
     b.set_loglevel(pargs.log)
     course = get_course(pargs)
-    b.info(f"## chapter {course.chapters[-1].slug} status: {getattr(course.chapters[-1], 'status', '-')}")
     generate(course)
     if pargs.sums:
         print_volume_report(course)
     b.exit_if_errors()
 
 
 def get_course(pargs):
@@ -87,14 +86,15 @@
     copy_baseresources(course)
     remove_empty_partscontainers(course)
     add_tocs_to_upper_parts(course)
     register_macros(course)
     generate_upper_parts_files(course, env)
     generate_task_files(course, env)
     generate_metadata_and_glossary(course, env)
+    generate_itree_zipfile(course)
     generate_htaccess(course)
     if course.cache_mode == sdrl.course.CacheMode.READ:
         os.utime(cache_filename(course))  # update mtime of cache file to now
     else:
         print(f"wrote student files to  '{targetdir_s}'")
         print(f"wrote instructor files to  '{targetdir_i}'")
 
@@ -125,14 +125,25 @@
     htaccess_txt = (course.htaccess_template.format( 
                        userlist_commas=",".join(userlist), 
                        userlist_spaces=" ".join(userlist),
                        userlist_quotes_spaces=" ".join((f'"{u}"' for u in userlist))))
     b.spit(f"{targetfile}", htaccess_txt)
 
 
+def generate_itree_zipfile(course: sdrl.course.Course):
+    if not course.itreedir or course.cache_mode == sdrl.course.CacheMode.READ:
+        return  # nothing to do
+    b.info(f"generating itreedir ZIP file to '{course.targetdir_i}/{course.itreedir}'")
+    if not course.itreedir.endswith(".zip"):
+        b.critical(f"itreedir = '{course.itreedir}'; must end with '.zip'")
+    itreedir = sdrl.part.Partscontainer()
+    itreedir.zipdirs = [sdrl.part.Zipdir(course.itreedir)]
+    itreedir.render_zipdirs(course.targetdir_i)
+
+
 def generate_metadata_and_glossary(course: sdrl.course.Course, env):
     if course.cache_mode == sdrl.course.CacheMode.READ:
         return  # nothing to do
     b.info(f"generating metadata file '{course.targetdir_s}/{b.METADATA_FILE}'")
     write_metadata(course, f"{course.targetdir_s}/{b.METADATA_FILE}")
     render_glossary(course, env, course.targetdir_s, b.Mode.STUDENT)
     render_glossary(course, env, course.targetdir_i, b.Mode.INSTRUCTOR)
@@ -282,14 +293,16 @@
                           functools.partial(expand_href, course))  # show and link a URL
     macros.register_macro('PARTREF', 1, MM.INNER, 
                           functools.partial(expand_partref, course))  # slug as linktext
     macros.register_macro('PARTREFTITLE', 1, MM.INNER, 
                           functools.partial(expand_partref, course))  # title as linktext
     macros.register_macro('PARTREFMANUAL', 2, MM.INNER, 
                           functools.partial(expand_partref, course))  # explicit linktext
+    macros.register_macro('TREEREF', 1, MM.INNER, 
+                          functools.partial(expand_treeref, course))  # show full path in itree
     macros.register_macro('EC', 0, MM.INNER, expand_enumeration, partswitch_enumeration)
     macros.register_macro('EQ', 0, MM.INNER, expand_enumeration, partswitch_enumeration)
     macros.register_macro('ER', 0, MM.INNER, expand_enumeration, partswitch_enumeration)
     macros.register_macro('EREFC', 1, MM.INNER, expand_enumerationref)
     macros.register_macro('EREFQ', 1, MM.INNER, expand_enumerationref)
     macros.register_macro('EREFR', 1, MM.INNER, expand_enumerationref)
     macros.register_macro('DIFF', 1, MM.INNER, sdrl.course.Task.expand_diff)
@@ -323,14 +336,26 @@
     part = course.get_part(macrocall.filename, macrocall.arg1)
     linktext = dict(PARTREF=part.slug, 
                     PARTREFTITLE=part.title, 
                     PARTREFMANUAL=macrocall.arg2)[macrocall.macroname]
     return f"<a href='{part.outputfile}' class='partref-link'>{html.escape(linktext)}</a>"
 
 
+def expand_treeref(course: sdrl.course.Course, macrocall: macros.Macrocall) -> str:
+    actualpath = includefile_path(course, macrocall, itree_mode=True)
+    showpath = actualpath[len(course.itreedir)+1:]  # skip itreedir part of path
+    if not os.path.exists(actualpath):
+        b.warning(f"{macrocall.macrocall_text}: itreedir file '{actualpath}' not found")
+        showpath = "???"
+    prefix = "<span class='treeref-prefix'></span>"
+    mainpart = f"<span class='treeref'>{html.escape(showpath, quote=False)}</span>"
+    suffix = "<span class='treeref-suffix'></span>"
+    return f"{prefix}{mainpart}{suffix}"
+
+
 def expand_section(macrocall: macros.Macrocall) -> str:
     """
     [SECTION::goal::subtype1,subtype2] etc.
     [INNERSECTION] is equivalent and serves for one level of proper nesting if needed.
     (Nesting [SECTION][ENDSECTION] blocks happens to work, but for the wrong reasons.)
     A section [SECTION]...[ENDSECTION] like the ahove gets rendered into the following structure:
     <div class='section section-goal'>
@@ -428,38 +453,36 @@
         rawcontent = f.read()
     if fullfilename.endswith('.md'):
         return macros.expand_macros(md.md.context_sourcefile, md.md.partname, rawcontent)
     else:
         return rawcontent
 
 
-def includefile_path(course: sdrl.course.Course, macrocall: macros.Macrocall) -> str:
+def includefile_path(course: sdrl.course.Course, macrocall: macros.Macrocall, itree_mode=False) -> str:
+    """
+    Normal mode constructs normal paths in chapterdir and those with prefix 'ALT:' in altdir.
+    itree mode constructs normal paths in itreedir and warns about 'ALT:' prefix if present.
+    """
     arg_re = r"(?P<alt>" + ALTDIR_KEYWORD + r")?(?P<slash>/)?(?P<incfile>.*)"
     mm = re.fullmatch(arg_re, macrocall.arg1)
     is_alt = mm.group("alt") is not None
+    if is_alt and itree_mode:
+        b.warning(f"{macrocall.macrocall_text}: '{ALTDIR_KEYWORD}' prefix makes no sense here")
+        is_alt = False  # ignore the prefix
     is_abs = mm.group("slash") is not None
-    inc_filepath = mm.group("incfile")
+    inc_filepath = mm.group("incfile")  # e.g. ../chapterlevel_includefile
     ctx_filepath = macrocall.filename  # e.g. ch/chapter/group/task.md
     ctx_dirpath = os.path.dirname(ctx_filepath)  # e.g. ch/chapter/group
     ctx_basename = os.path.basename(ctx_filepath)  # e.g. task.md
-    # print(f"## {macrocall.arg1} -> alt:{is_alt}, abs:{is_abs}, inc:{inc_filepath}, ctx:{ctx_dirpath}, {course.altdir}")
-    if is_alt:  # construct path in altdir tree:
-        abs_filepath = macrocall.filename.replace(course.chapterdir, course.altdir, 1)
-        abs_dirpath = os.path.dirname(abs_filepath)
-        # print(f"### is_alt: {abs_dirpath}")
-        if is_abs:
-            fullfilename = os.path.join(course.altdir, inc_filepath)
-        else:
-            fullfilename = os.path.join(abs_dirpath, inc_filepath or ctx_basename)
-    else:  # in chapterdir tree:
-        if is_abs:
-            fullfilename = os.path.join(course.chapterdir, inc_filepath)
-        else:
-            fullfilename = os.path.join(ctx_dirpath, inc_filepath)
-    return fullfilename
+    abs_topdir = (is_alt and course.altdir) or (itree_mode and course.itreedir) or course.chapterdir
+    rel_dirpath = ctx_dirpath.replace(course.chapterdir, abs_topdir, 1)
+    # print(f"## {macrocall.arg1} -> alt:{is_alt}, abs:{is_abs}, inc:{inc_filepath}, ctx:{ctx_dirpath}, "
+    #       f"abs_topdir:{abs_topdir}, rel_dirpath:{rel_dirpath}")
+    fullpath = os.path.join(abs_topdir if is_abs else rel_dirpath, inc_filepath or ctx_basename)
+    return fullpath
 
 
 def render_homepage(course: sdrl.course.Course, env, targetdir: str, mode: b.Mode):
     template = env.get_template("homepage.html")
     render_structure(course, template, course, targetdir, mode)
     course.render_zipdirs(targetdir)
```

### Comparing `sedrila-1.2.1/py/sdrl/subcmd/instructor.py` & `sedrila-1.3.0/py/sdrl/subcmd/instructor.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sdrl/subcmd/student.py` & `sedrila-1.3.0/py/sdrl/subcmd/student.py`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/py/sedrila.py` & `sedrila-1.3.0/py/sedrila.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,10 +25,10 @@
     parser.execute_subcommand(args)
 
 
 if __name__ == "__main__":
     print_profile = False
     if print_profile:
         import cProfile
-        cProfile.run('main()')
+        cProfile.run('main()', sort='cumulative')
     else:
         main()  # normal life
```

### Comparing `sedrila-1.2.1/pyproject.toml` & `sedrila-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # https://packaging.python.org/en/latest/
 # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "sedrila"
-version = "1.2.1"  # keep in sync with base.py
+version = "1.3.0"  # keep in sync with base.py
 description = "Tool infrastructure for building and running \"self-driven lab\" courses"
 license = "MIT"
 authors = ["Lutz Prechelt <prechelt@inf.fu-berlin.de>"]
 readme = "README.md"
 homepage = "https://github.com/fubinf/sedrila"
 repository = "https://github.com/fubinf/sedrila"
 keywords = ["static site generator"]
```

### Comparing `sedrila-1.2.1/templates/base.html` & `sedrila-1.3.0/templates/base.html`

 * *Files identical despite different names*

### Comparing `sedrila-1.2.1/setup.py` & `sedrila-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
               'input/ch/*',
               'input/ch/ch1/*',
               'input/ch/ch1/myarchive.zip/*',
               'input/ch/ch1/tg11/*',
               'input/ch/ch1/tg12/*',
               'input/ch/ch1/tg13draft/*',
               'input/ch/ch2draft/*',
-              'input/ch/ch2draft/tg21/*'],
+              'input/ch/ch2draft/tg21/*',
+              'input/itree.zip/*'],
  'sdrl.tests': ['data/*',
                 'data/sedrila-test1/*',
                 'data/sedrila-test1/.git/*',
                 'data/sedrila-test1/.git/hooks/*',
                 'data/sedrila-test1/.git/info/*',
                 'data/sedrila-test1/.git/logs/*',
                 'data/sedrila-test1/.git/logs/refs/heads/*',
@@ -139,15 +140,15 @@
  'rich>=13.7,<14.0']
 
 entry_points = \
 {'console_scripts': ['sedrila = sedrila:main']}
 
 setup_kwargs = {
     'name': 'sedrila',
-    'version': '1.2.1',
+    'version': '1.3.0',
     'description': 'Tool infrastructure for building and running "self-driven lab" courses',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/sedrila/badge/?version=latest)](https://sedrila.readthedocs.io/en/latest/?badge=latest)\n\n# `sedrila`: Tool infrastructure for building and running "self-driven lab" courses\n\nA "self-driven lab" (SeDriLa) course is one where students select freely \na subset from a large set of tasks.\nThe tasks are described with sufficient detail that no guidance from an instructor\nis needed most of the time.\n\nsedrila is a command-line tool supporting course authors for authoring a course\nand then course instructors and students for executing it.\n\nFind the [documentation at readthedocs](https://sedrila.readthedocs.io).\n\n\n## Ideas for future versions\n\n- Process `SEDRILA_INSTRUCTOR_COURSE_URLS` as described in the instructor documentation.\n- `sedrila instructor` should keep a JSON file `student_course_urls.json` that maps student usernames\n  to the course URL first seen for that student, because if a student ever changed\n  the URL in the `student.yaml`, prior signed commits of instructors might become \n  invalid semantically if the new course has a different set of tasks.  \n  The map is added to when a `student.yaml` is first seen\n  and checked against at each later time.  \n  Note that a student taking part a second time, with a fresh repo,\n  might require manual editing of that JSON file to remove that entry.\n- Better yet, there could be an option `sedrial instructor --allow-repo2` that \n  performs that editing automatically\n  and also checks that the new repo contains no instructor-signed commits.\n- Command `sedrila instructor --clean-up-repos-home`\n  to clean up instructor work directory trees-of-trees\n  by deleting all level-1 subtrees in which the `student.yaml`\n  has a `course_url` that is not mentioned in the \n  `SEDRILA_INSTRUCTOR_COURSE_URLS`environment variable.\n  This option should ask a safety question before starting to work.\n\n\n## Development process: TODO-handling during development\n\nWe use this convention for the development of `sedrila`.\nIt may also be helpful for course authors if the team is small enough.\n\nIf something is incomplete, add a TODO marker with a priorization digit:\n- `TODO 1`: to be completed soon (within a few days)\n- `TODO 2`: to be completed once the prio 1 things are done (within days or a few weeks)\n- `TODO 3`: to be completed at some later time (usually several weeks or more into the future,\n  because it is big) or never (because it is not-so-important: "nice-to-have features")\n\nAdd a short description of what needs to be done. Examples:\n- `TODO 1: find proper formulation`\n- `TODO 2: restructure to use ACME lib`\n- `TODO 3: add automatic grammar correction`\n\nIf you intend to do it yourself, add your name in parens:  \n`TODO 1: find proper formulation (Lutz)`\n\nThen use the IDE global search to work through these layer-by-layer.\nDemote items to a lower priority when they become stale or remove them.\nKick out prio 3 items when they become unlikely.\n\n\n## A currently needed refactoring: Target directory structure\n\nThe current layout of the source tree is wrong.\nCurrently, the `templates` and `baseresources` directories will end up \nas top-level directories when the package is installed,\nwhich means they will clash with any top-level modules of that name\nanywhere in our dependencies.\n\nWe need to perform the following refactorings to arrive at a proper structure:\n\n- `py` --> `sedrila`: This will be the top level directory that gets installed.\n- `sedrila/sdrl/*` --> `sedrila/*`: We remove the now-intermediate namespace.\n  This implies joining the current `sdrl/tests` into `sedrila/tests`.\n- `templates` --> `sedrila/templates`: The HTML templates simply become part of the\n  tree to be installed.\n- `baseresources` --> `sedrila/baseresources`: Ditto.\n\nThese changes require a lot of changes of import statements.\nFor instance, the current module `base` will become `sedrila.base`\nand `sdrl.course` will become `sedrila.course`.\nThe logic for computing `sedrila_libdir` in `courses.py` must be adapted.\nThe files lists in `pyproject.toml` must be corrected.\n',
     'author': 'Lutz Prechelt',
     'author_email': 'prechelt@inf.fu-berlin.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fubinf/sedrila',
```

### Comparing `sedrila-1.2.1/PKG-INFO` & `sedrila-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sedrila
-Version: 1.2.1
+Version: 1.3.0
 Summary: Tool infrastructure for building and running "self-driven lab" courses
 Home-page: https://github.com/fubinf/sedrila
 License: MIT
 Keywords: static site generator
 Author: Lutz Prechelt
 Author-email: prechelt@inf.fu-berlin.de
 Requires-Python: >=3.11,<4.0
```

