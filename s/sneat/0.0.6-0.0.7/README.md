# Comparing `tmp/sneat-0.0.6.tar.gz` & `tmp/sneat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneat-0.0.6.tar", last modified: Mon Jun  3 14:56:54 2024, max compression
+gzip compressed data, was "sneat-0.0.7.tar", last modified: Mon Jun  3 15:25:29 2024, max compression
```

## Comparing `sneat-0.0.6.tar` & `sneat-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:54.991489 sneat-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 14:56:47.000000 sneat-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-03 14:56:54.991489 sneat-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-03 14:56:47.000000 sneat-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:56:54.991489 sneat-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-06-03 14:56:47.000000 sneat-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:54.991489 sneat-0.0.6/sneat/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/evolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/neuralnetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/population.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/species.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:54.991489 sneat-0.0.6/sneat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:25:29.239246 sneat-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 15:25:18.000000 sneat-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-03 15:25:29.239246 sneat-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-03 15:25:18.000000 sneat-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 15:25:29.239246 sneat-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-06-03 15:25:18.000000 sneat-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:25:29.235246 sneat-0.0.7/sneat/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/neuralnetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-03 15:25:18.000000 sneat-0.0.7/sneat/species.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:25:29.235246 sneat-0.0.7/sneat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-03 15:25:29.000000 sneat-0.0.7/sneat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 15:25:29.000000 sneat-0.0.7/sneat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:25:29.000000 sneat-0.0.7/sneat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-03 15:25:29.000000 sneat-0.0.7/sneat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 15:25:29.000000 sneat-0.0.7/sneat.egg-info/top_level.txt
```

### Comparing `sneat-0.0.6/LICENSE` & `sneat-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sneat-0.0.6/PKG-INFO` & `sneat-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneat
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simplified implementation of NEAT (Neuro-Evolution of Augmenting Topologies).
 Home-page: https://github.com/bhark/sNEAT
 Author: Adrian E. Bratlann
 Author-email: aeb@tetrabit.coop
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sneat-0.0.6/README.md` & `sneat-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sneat-0.0.6/setup.py` & `sneat-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='sneat',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     package_data={'sneat': ['default_config.ini']},
     install_requires=[
         'matplotlib==3.9.0',
         'networkx==3.3',
         'numpy==1.26.4',
         'tabulate==0.9.0',
```

### Comparing `sneat-0.0.6/sneat/config.py` & `sneat-0.0.7/sneat/config.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.6/sneat/evolve.py` & `sneat-0.0.7/sneat/evolve.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,19 @@
             print(f'[i] Restoring from checkpoint (gen. {pop.generation})...')
             return pop
     except FileNotFoundError:
         return None
 
 def print_stats(pop):
     print(f'\n\n[i] Gen. {pop.generation}:')
-    headers = ['Species', 'Members', 'Best Fitness', 'Average Fitness']
+    headers = ['Species', 'Members', 'Best Fitness', 'Average Fitness', 'Stagnation', 'Best Complexity']
     for s in pop.species:
         s.members = sorted(s.members, key=lambda x: x.fitness, reverse=True)
     species = sorted(pop.species, key=lambda x: x.members[0].fitness, reverse=True)
-    data = [[s.id, len(s.members), round(max(g.fitness for g in s.members), 2), round(np.mean([g.fitness for g in s.members]), 2)] for s in species]
+    data = [[s.id, len(s.members), round(max(g.fitness for g in s.members), 2), round(np.mean([g.fitness for g in s.members]), 2), s.stagnation, f'{len(s.members[0].network.nodes)}n + {len(s.members[0].network.connections)}'] for s in species]
     print(tb(data, headers=headers))
     print('-' * 55)
 
 def evolve(fitness_function):
     config = get_config()
     
     pop = load_checkpoint() or Population()
```

### Comparing `sneat-0.0.6/sneat/genome.py` & `sneat-0.0.7/sneat/genome.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.6/sneat/neuralnetwork.py` & `sneat-0.0.7/sneat/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.6/sneat/normalizer.py` & `sneat-0.0.7/sneat/normalizer.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.6/sneat/population.py` & `sneat-0.0.7/sneat/population.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,21 +38,38 @@
         min_fitness = min(g.fitness for g in self.genomes)
         max_fitness = max(g.fitness for g in self.genomes)
         if max_fitness - min_fitness == 0:
             max_fitness += 0.0001 # avoid division by zero
         for g in self.genomes:
             g.normalized_fitness = (g.fitness - min_fitness) / (max_fitness - min_fitness)
 
-        # assign adjusted fitness scores
         for s in self.species:
-            s_size = len(s.members)
 
+            # bump stagnation
+            if s.members[0].fitness > s.best_fitness:
+                s.best_fitness = s.members[0].fitness
+                s.stagnation = 0
+            else:
+                s.stagnation += 1
+
+            # assign adjusted fitness scores
+            s_size = len(s.members)
             for g in s.members:
                 g.adjusted_fitness = max(g.normalized_fitness / s_size, 0.0001) # avoid division by zero
 
+        # remove stagnant species
+        while len(self.species) >= self.config.getint('Evolution', 'min_species'):
+            stagnant_species = [s for s in self.species if s.stagnation >= self.config.getint('Evolution', 'max_stagnation')]
+            stagnant_species = sorted(stagnant_species, key=lambda x: x.best_fitness, reverse=True)
+            if not stagnant_species:
+                break
+            extinct = stagnant_species.pop()
+            self.species.remove(extinct)
+            print(f'[i] Species {extinct.id} went extinct')
+
         # perform reproduction inside of each species
         offspring = []
         for s in self.species:
             s_offspring = []
 
             # copy elite as-is
             s.members.sort(key=lambda x: x.fitness, reverse=True)
```

### Comparing `sneat-0.0.6/sneat.egg-info/PKG-INFO` & `sneat-0.0.7/sneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneat
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simplified implementation of NEAT (Neuro-Evolution of Augmenting Topologies).
 Home-page: https://github.com/bhark/sNEAT
 Author: Adrian E. Bratlann
 Author-email: aeb@tetrabit.coop
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

