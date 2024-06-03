# Comparing `tmp/bwalign-1.6.3.tar.gz` & `tmp/bwalign-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bwalign-1.6.3.tar", last modified: Mon Jun  3 11:21:39 2024, max compression
+gzip compressed data, was "bwalign-1.6.4.tar", last modified: Mon Jun  3 11:31:15 2024, max compression
```

## Comparing `bwalign-1.6.3.tar` & `bwalign-1.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:21:39.230229 bwalign-1.6.3/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:21:39.229374 bwalign-1.6.3/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.3/README.md
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:21:39.219212 bwalign-1.6.3/bwalign/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 11:21:18.000000 bwalign-1.6.3/bwalign/__init__.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)     2228 2024-06-03 11:21:12.000000 bwalign-1.6.3/bwalign/main.py
--rw-r--r--   0 adrianlayer   (501) staff       (20)    18518 2024-06-03 11:20:34.000000 bwalign-1.6.3/bwalign/utils.py
-drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:21:39.226788 bwalign-1.6.3/bwalign.egg-info/
--rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/PKG-INFO
--rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/SOURCES.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/dependency_links.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/entry_points.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/requires.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 11:21:39.000000 bwalign-1.6.3/bwalign.egg-info/top_level.txt
--rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 11:21:39.230383 bwalign-1.6.3/setup.cfg
--rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 11:21:16.000000 bwalign-1.6.3/setup.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:31:15.648918 bwalign-1.6.4/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:31:15.648024 bwalign-1.6.4/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1744 2024-05-29 18:41:22.000000 bwalign-1.6.4/README.md
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:31:15.638998 bwalign-1.6.4/bwalign/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      142 2024-06-03 11:31:05.000000 bwalign-1.6.4/bwalign/__init__.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     2231 2024-06-03 11:30:53.000000 bwalign-1.6.4/bwalign/main.py
+-rw-r--r--   0 adrianlayer   (501) staff       (20)    18538 2024-06-03 11:27:05.000000 bwalign-1.6.4/bwalign/utils.py
+drwxr-xr-x   0 adrianlayer   (501) staff       (20)        0 2024-06-03 11:31:15.646607 bwalign-1.6.4/bwalign.egg-info/
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      934 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/PKG-INFO
+-rw-r--r--   0 adrianlayer   (501) staff       (20)      259 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        1 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       46 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/entry_points.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       21 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/requires.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)        8 2024-06-03 11:31:15.000000 bwalign-1.6.4/bwalign.egg-info/top_level.txt
+-rw-r--r--   0 adrianlayer   (501) staff       (20)       38 2024-06-03 11:31:15.649127 bwalign-1.6.4/setup.cfg
+-rw-r--r--   0 adrianlayer   (501) staff       (20)     1224 2024-06-03 11:31:01.000000 bwalign-1.6.4/setup.py
```

### Comparing `bwalign-1.6.3/PKG-INFO` & `bwalign-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.3
+Version: 1.6.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.3/README.md` & `bwalign-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bwalign-1.6.3/bwalign/main.py` & `bwalign-1.6.4/bwalign/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,21 +40,21 @@
             
             #create a SAM entry for the aligned read
             a = pysam.AlignedSegment()
             a.query_name = read_id
             a.query_sequence = read_seq
             a.flag = 0
             a.reference_id = 0
-            if alignment_s == None:
-                a.reference_start = 0
-                a.mapping_quality = 0
-                a.cigarstring = '0M'
-            else:
+            if score != float('-inf'):
                 a.reference_start = best_idx
                 a.mapping_quality = calculate_mapping_quality(score, read_length)
                 a.cigarstring = calculate_cigar(alignment_s, alignment_t)
+            else:
+                a.reference_start = 0
+                a.mapping_quality = 0
+                a.cigarstring = '0M'
             a.query_qualities = qual_scores
             
             samfile.write(a)
 
 if __name__ == "__main__":
     main()
```

### Comparing `bwalign-1.6.3/bwalign/utils.py` & `bwalign-1.6.4/bwalign/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,21 +65,21 @@
 def banded_alignment(mr: int, mmp: int, indp: int, bp: int, s: str, t: str) -> int:
     l = np.full((len(s)+1,len(t)+1), -np.inf)
     for i in range(0, len(s) + 1):
         for j in range(0, len(t) + 1):
             if i == 0 and j == 0:
                 l[i,j] = 0
                 continue
-            elif i == 0:
-                l[i,j] = j * (-indp)
-                continue
-            elif j == 0:
-                l[i,j] = i * (-indp)
-                continue
             if abs(j-i) < bp:
+                if i == 0:
+                    l[i,j] = j * (-indp)
+                    continue
+                if j == 0:
+                    l[i,j] = i * (-indp)
+                    continue
                 match = -mmp
                 if s[i-1] == t[j-1]:
                     match = mr
                 l[i,j] = max(l[i-1][j] - indp, l[i][j-1] - indp, l[i-1][j-1] + match)
             else:
                 continue
     score = l[len(s),len(t)]
```

### Comparing `bwalign-1.6.3/bwalign.egg-info/PKG-INFO` & `bwalign-1.6.4/bwalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bwalign
-Version: 1.6.3
+Version: 1.6.4
 Summary: A burrows-wheeler seed and extend aligner
 Home-page: https://github.com/NabilHKhoury/bwalign
 Author: ['Adrian Layer, Nabil Khoury, Yasmin Jabir']
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `bwalign-1.6.3/setup.py` & `bwalign-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bwalign',
-    version='1.6.3',    
+    version='1.6.4',    
     description='A burrows-wheeler seed and extend aligner',
     url='https://github.com/NabilHKhoury/bwalign',
     author=['Adrian Layer, Nabil Khoury, Yasmin Jabir'],
     license='MIT',
     packages=find_packages(),
     install_requires=['biopython',
                       'pysam',
```

