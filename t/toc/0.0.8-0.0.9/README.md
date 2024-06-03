# Comparing `tmp/toc-0.0.8.tar.gz` & `tmp/toc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toc-0.0.8.tar", last modified: Fri Nov  1 09:06:52 2013, max compression
+gzip compressed data, was "dist/toc-0.0.9.tar", last modified: Tue Mar  4 06:55:09 2014, max compression
```

## Comparing `toc-0.0.8.tar` & `toc-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 youngrok   (501) staff       (20)        0 2013-11-01 09:06:52.000000 toc-0.0.8/
--rw-r--r--   0 youngrok   (501) staff       (20)      434 2013-11-01 09:06:52.000000 toc-0.0.8/PKG-INFO
--rw-r--r--   0 youngrok   (501) staff       (20)       59 2013-11-01 09:06:52.000000 toc-0.0.8/setup.cfg
--rwxr-xr-x   0 youngrok   (501) staff       (20)      613 2013-11-01 09:06:14.000000 toc-0.0.8/setup.py
-drwxr-xr-x   0 youngrok   (501) staff       (20)        0 2013-11-01 09:06:52.000000 toc-0.0.8/toc/
--rw-r--r--   0 youngrok   (501) staff       (20)     2428 2013-11-01 09:05:54.000000 toc-0.0.8/toc/__init__.py
-drwxr-xr-x   0 youngrok   (501) staff       (20)        0 2013-11-01 09:06:52.000000 toc-0.0.8/toc.egg-info/
--rw-r--r--   0 youngrok   (501) staff       (20)        1 2013-11-01 09:06:52.000000 toc-0.0.8/toc.egg-info/dependency_links.txt
--rw-r--r--   0 youngrok   (501) staff       (20)      434 2013-11-01 09:06:52.000000 toc-0.0.8/toc.egg-info/PKG-INFO
--rw-r--r--   0 youngrok   (501) staff       (20)      132 2013-11-01 09:06:52.000000 toc-0.0.8/toc.egg-info/SOURCES.txt
--rw-r--r--   0 youngrok   (501) staff       (20)        4 2013-11-01 09:06:52.000000 toc-0.0.8/toc.egg-info/top_level.txt
+drwxr-xr-x   0 youngrok   (501) staff       (20)        0 2014-03-04 06:55:09.000000 toc-0.0.9/
+-rw-r--r--   0 youngrok   (501) staff       (20)      434 2014-03-04 06:55:09.000000 toc-0.0.9/PKG-INFO
+-rw-r--r--   0 youngrok   (501) staff       (20)       59 2014-03-04 06:55:09.000000 toc-0.0.9/setup.cfg
+-rwxr-xr-x   0 youngrok   (501) staff       (20)      613 2014-03-04 06:54:16.000000 toc-0.0.9/setup.py
+drwxr-xr-x   0 youngrok   (501) staff       (20)        0 2014-03-04 06:55:09.000000 toc-0.0.9/toc/
+-rw-r--r--   0 youngrok   (501) staff       (20)     2428 2014-03-04 06:54:06.000000 toc-0.0.9/toc/__init__.py
+drwxr-xr-x   0 youngrok   (501) staff       (20)        0 2014-03-04 06:55:09.000000 toc-0.0.9/toc.egg-info/
+-rw-r--r--   0 youngrok   (501) staff       (20)        1 2014-03-04 06:55:08.000000 toc-0.0.9/toc.egg-info/dependency_links.txt
+-rw-r--r--   0 youngrok   (501) staff       (20)      434 2014-03-04 06:55:08.000000 toc-0.0.9/toc.egg-info/PKG-INFO
+-rw-r--r--   0 youngrok   (501) staff       (20)      132 2014-03-04 06:55:08.000000 toc-0.0.9/toc.egg-info/SOURCES.txt
+-rw-r--r--   0 youngrok   (501) staff       (20)        4 2014-03-04 06:55:08.000000 toc-0.0.9/toc.egg-info/top_level.txt
```

### Comparing `toc-0.0.8/setup.py` & `toc-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(name='toc',
       description='Table of contents generator for html',
       author='Youngrok Pak',
       author_email='pak.youngrok@gmail.com',
       keywords= 'toc table contents html',
       url='https://github.com/youngrok/toc',
-      version='0.0.8',
+      version='0.0.9',
       packages=['toc',
                 ],
       classifiers = [
                      'Development Status :: 3 - Alpha',
                      'Topic :: Software Development :: Libraries',
                      'License :: OSI Approved :: BSD License']
       )
```

### Comparing `toc-0.0.8/toc/__init__.py` & `toc-0.0.9/toc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 ol = next_ol
         elif nextdepth < depth:
             for i in range(nextdepth, depth): ol = ol.parentNode
             
         depth = nextdepth
             
         index[depth - 1] += 1
-        label = '.'.join([str(index[d]) for d in range(0, depth) if index[d]])
+        label = '-'.join([str(index[d]) for d in range(0, depth) if index[d]])
 
         li = Element('li')
         a = Element('a')
         a.setAttribute('href', '%s#header-%s' % (url, label))
         a.appendChild(doc.createTextNode(innerText(header)))
         li.appendChild(a)
         ol.appendChild(li)
```

