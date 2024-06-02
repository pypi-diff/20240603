# Comparing `tmp/wsgintegrate-0.1.3.tar.gz` & `tmp/wsgintegrate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wsgintegrate-0.1.3.tar", last modified: Wed Apr 12 17:57:59 2017, max compression
+gzip compressed data, was "dist/wsgintegrate-0.1.5.tar", last modified: Sun Jun  2 23:20:36 2024, max compression
```

## Comparing `wsgintegrate-0.1.3.tar` & `wsgintegrate-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     5935 2017-04-12 17:57:03.000000 wsgintegrate-0.1.3/README.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      852 2017-04-12 17:57:44.000000 wsgintegrate-0.1.3/setup.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     7939 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/PKG-INFO
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       59 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/setup.cfg
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      881 2015-04-26 16:33:55.000000 wsgintegrate-0.1.3/wsgintegrate/web.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     2524 2015-04-26 16:33:55.000000 wsgintegrate-0.1.3/wsgintegrate/main.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1425 2015-04-26 16:33:55.000000 wsgintegrate-0.1.3/wsgintegrate/server.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     5813 2015-04-26 16:33:55.000000 wsgintegrate-0.1.3/wsgintegrate/match.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      916 2015-04-26 16:33:55.000000 wsgintegrate-0.1.3/wsgintegrate/factory.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)      907 2015-04-26 16:33:55.000000 wsgintegrate-0.1.3/wsgintegrate/dispatcher.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2015-04-26 16:33:55.000000 wsgintegrate-0.1.3/wsgintegrate/__init__.py
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2015-04-26 16:41:40.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/not-zip-safe
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     7939 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/PKG-INFO
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/dependency_links.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       13 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/top_level.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       75 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/entry_points.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      434 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/SOURCES.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        6 2017-04-12 17:57:59.000000 wsgintegrate-0.1.3/wsgintegrate.egg-info/requires.txt
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     4160 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     3029 2024-06-02 23:06:26.000000 wsgintegrate-0.1.5/README.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/setup.cfg
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      934 2024-06-02 23:17:38.000000 wsgintegrate-0.1.5/setup.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2024-06-02 23:06:26.000000 wsgintegrate-0.1.5/wsgintegrate/__init__.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)      950 2024-06-02 23:13:55.000000 wsgintegrate-0.1.5/wsgintegrate/dispatcher.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      918 2024-06-02 23:10:47.000000 wsgintegrate-0.1.5/wsgintegrate/factory.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     2529 2024-06-02 23:06:26.000000 wsgintegrate-0.1.5/wsgintegrate/main.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     5813 2024-06-02 23:06:26.000000 wsgintegrate-0.1.5/wsgintegrate/match.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     1426 2024-06-02 23:06:26.000000 wsgintegrate-0.1.5/wsgintegrate/server.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      881 2024-06-02 23:06:26.000000 wsgintegrate-0.1.5/wsgintegrate/web.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     4160 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      434 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       75 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/entry_points.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-06-02 23:06:28.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/not-zip-safe
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       22 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/requires.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       13 2024-06-02 23:20:36.000000 wsgintegrate-0.1.5/wsgintegrate.egg-info/top_level.txt
```

### Comparing `wsgintegrate-0.1.3/setup.py` & `wsgintegrate-0.1.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from setuptools import setup
 import os
+from setuptools import setup
 
-version = '0.1.3'
+version = '0.1.5'
 
 # description
 try:
-  filename = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'README.txt')
-  description = file(filename).read()
+  filename = os.path.join(os.path.dirname(os.path.abspath(__file__)),
+                          'README.txt')
+  description = open(filename).read()
 except:
   description = ''
 
-dependencies = ['webob']
+dependencies = ['webob', 'pyloader>=0.1.5']
 
 setup(name='wsgintegrate',
       version=version,
       description='WSGI integration layer',
       long_description=description,
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
       keywords='',
       author='Jeff Hammel',
       author_email='k0scist@gmail.com',
-      url='http://k0s.org/',
+      url='http://k0s.org/hg/wsgintegrate',
       license='GPL',
       packages=['wsgintegrate'],
       include_package_data=True,
       zip_safe=False,
       install_requires=dependencies,
+      tests_require=['tox'],
       entry_points="""
       [console_scripts]
       wsgintegrate = wsgintegrate.main:main
-      """,
-      )
+      """
+)
```

### Comparing `wsgintegrate-0.1.3/wsgintegrate/web.py` & `wsgintegrate-0.1.5/wsgintegrate/web.py`

 * *Files identical despite different names*

### Comparing `wsgintegrate-0.1.3/wsgintegrate/main.py` & `wsgintegrate-0.1.5/wsgintegrate/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 """
 command line interface for wsgintegrate.
 serves an application from a .ini file
 (really, a DAG)
 """
 
 import sys
-from factory import WSGIfactory
+from .factory import WSGIfactory
+from .server import servers
 from optparse import OptionParser
-from server import servers
+
 
 def main(args=sys.argv[1:]):
     """CLI"""
 
     # parse command line options
     usage = '%prog [options] config-file'
     parser = OptionParser(usage=usage, description=__doc__)
@@ -46,25 +47,26 @@
     # create a factory from configuration
     # TODO: interpret if the configuration is .ini, JSON, etc
     factory = WSGIfactory(config, main=options.app)
 
     # print configuration, if specified
     if options.list_apps:
         for app in sorted(factory.config.keys()):
-            print app
+            print(app)
         return
     if options.print_json:
-        print factory.json_config()
+        print(factory.json_config())
         return
     if options.print_ini:
-        print factory.ini_config()
+        print(factory.ini_config())
         return
 
     # serve it
     server_name = getattr(options, 'server', 'wsgiref')
-    print ("Serving with %s" % (server_name))
+    print("Serving with %s" % (server_name))
     server = servers[server_name]
-    print ('http://localhost:%d/' % options.port)
+    print('http://localhost:%d/' % options.port)
     server(app=factory.load(), port=options.port)
 
+
 if __name__ == '__main__':
   main()
```

### Comparing `wsgintegrate-0.1.3/wsgintegrate/server.py` & `wsgintegrate-0.1.5/wsgintegrate/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 front-ends for various WSGI servers
 """
 
-from factory import WSGIfactory
+from .factory import WSGIfactory
 
 __all__ = ['wsgiref', 'servers', 'paster']
 
 
 ### wsgiref
 
 def wsgiref(app, host='0.0.0.0', port=80):
```

### Comparing `wsgintegrate-0.1.3/wsgintegrate/match.py` & `wsgintegrate-0.1.5/wsgintegrate/match.py`

 * *Files identical despite different names*

### Comparing `wsgintegrate-0.1.3/wsgintegrate/factory.py` & `wsgintegrate-0.1.5/wsgintegrate/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     def __call__(self, environ, start_response):
         """WSGI application"""
 
         # if the configuration has changed,
         # reload the .ini file
         mtime = os.path.getmtime(self.inifile)
         if mtime > self.mtime:
-            print "Reloading '%s': %s > %s" % (self.inifile, mtime, self.mtime)
+            print("Reloading '%s': %s > %s" % (self.inifile, mtime, self.mtime))
             try:
                 config = self.read(self.inifile)
                 self.configure(config)
-            except Exception, e:
-                print >> sys.stderr, "Error reading '%s': %s" % (self.inifile, e)
+            except Exception as e:
+                sys.stderr.write("Error reading '%s': %s\n" % (self.inifile, e))
             self.mtime = mtime
 
         app = self.load(self.main)
         return app(environ, start_response)
```

