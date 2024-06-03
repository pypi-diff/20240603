# Comparing `tmp/sneat-0.0.3.tar.gz` & `tmp/sneat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneat-0.0.3.tar", last modified: Thu May 30 23:41:26 2024, max compression
+gzip compressed data, was "sneat-0.0.5.tar", last modified: Mon Jun  3 14:45:08 2024, max compression
```

## Comparing `sneat-0.0.3.tar` & `sneat-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:41:26.034417 sneat-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 23:41:18.000000 sneat-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 23:41:26.034417 sneat-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-30 23:41:18.000000 sneat-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:41:26.034417 sneat-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 23:41:18.000000 sneat-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:41:26.034417 sneat-0.0.3/sneat/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/evolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/neuralnetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/population.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 23:41:18.000000 sneat-0.0.3/sneat/species.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:41:26.034417 sneat-0.0.3/sneat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-30 23:41:25.000000 sneat-0.0.3/sneat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-30 23:41:26.000000 sneat-0.0.3/sneat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:41:25.000000 sneat-0.0.3/sneat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 23:41:25.000000 sneat-0.0.3/sneat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 23:41:25.000000 sneat-0.0.3/sneat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:08.982520 sneat-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 14:44:58.000000 sneat-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-03 14:45:08.982520 sneat-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-03 14:44:58.000000 sneat-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:45:08.982520 sneat-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-03 14:44:58.000000 sneat-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:08.982520 sneat-0.0.5/sneat/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/neuralnetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/species.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:08.982520 sneat-0.0.5/sneat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/top_level.txt
```

### Comparing `sneat-0.0.3/LICENSE` & `sneat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sneat-0.0.3/README.md` & `sneat-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SNEAT (Simplified NEAT)
+# sNEAT (Simplified NEAT)
 
 ![GitHub Tag](https://img.shields.io/github/v/tag/bhark/sneat) 
 ![PyPI - Version](https://img.shields.io/pypi/v/sneat)
 ![PyPI - License](https://img.shields.io/pypi/l/sneat)
 
 A simplified implementation of [Neuro-evolution of Augmenting Topologies](https://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf), a novel technique for neuro-evolution developed by Kenneth O. Stanley.
```

### Comparing `sneat-0.0.3/setup.py` & `sneat-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sneat',
-    version='0.0.3',
+    version='0.0.5',
     packages=find_packages(),
     package_data={'sneat': ['default_config.ini']},
     install_requires=[
         'matplotlib==3.9.0',
         'networkx==3.3',
         'numpy==1.26.4',
         'tabulate==0.9.0',
         'tqdm==4.66.4'
     ],
+    extras_require={
+        'examples': [
+            'gymnasium',
+            'gymnasium[box2d]',
+            'gymnasium[classic_control]',
+        ]
+    },
     author='Adrian E. Bratlann',
     author_email='aeb@tetrabit.coop',
     description='Simplified implementation of NEAT (Neuro-Evolution of Augmenting Topologies).',
     license='GPLv3'
 )
```

### Comparing `sneat-0.0.3/sneat/config.py` & `sneat-0.0.5/sneat/config.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.3/sneat/evolve.py` & `sneat-0.0.5/sneat/evolve.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,21 +53,23 @@
             pop.reproduce()
 
             best_fitness = max(g.fitness for g in pop.genomes)
             if best_fitness >= max_fitness:
                 winner = max(pop.genomes, key=lambda x: x.fitness)
                 save_genome(winner, 'winner.pkl')
                 print(f'\n\n[+] Winner found with fitness: {winner.fitness}\n\n')
-                break
+                return winner
             
             if pop.generation >= max_generations:
                 winner = max(pop.genomes, key=lambda x: x.fitness)
                 save_genome(winner, 'winner.pkl')
                 print(f'\n\n[+] Reached max generations, and achieved a fitness of: {winner.fitness}\n\n')
-                break
+                return winner
+                
     except KeyboardInterrupt:
             winner = max(pop.genomes, key=lambda x: x.fitness)
             print(f'\n\n[+] Best genome saved, with a fitness of {winner.fitness}\n')
             save_genome(winner, 'winner.pkl')
+            return winner
```

### Comparing `sneat-0.0.3/sneat/genome.py` & `sneat-0.0.5/sneat/genome.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.3/sneat/neuralnetwork.py` & `sneat-0.0.5/sneat/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.3/sneat/normalizer.py` & `sneat-0.0.5/sneat/normalizer.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.3/sneat/population.py` & `sneat-0.0.5/sneat/population.py`

 * *Files identical despite different names*

