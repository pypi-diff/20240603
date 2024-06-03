# Comparing `tmp/sneat-0.0.5.tar.gz` & `tmp/sneat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneat-0.0.5.tar", last modified: Mon Jun  3 14:45:08 2024, max compression
+gzip compressed data, was "sneat-0.0.6.tar", last modified: Mon Jun  3 14:56:54 2024, max compression
```

## Comparing `sneat-0.0.5.tar` & `sneat-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:08.982520 sneat-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 14:44:58.000000 sneat-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-03 14:45:08.982520 sneat-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-03 14:44:58.000000 sneat-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:45:08.982520 sneat-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-03 14:44:58.000000 sneat-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:08.982520 sneat-0.0.5/sneat/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/evolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/neuralnetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/population.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-03 14:44:58.000000 sneat-0.0.5/sneat/species.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:45:08.982520 sneat-0.0.5/sneat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:45:08.000000 sneat-0.0.5/sneat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:54.991489 sneat-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 14:56:47.000000 sneat-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-03 14:56:54.991489 sneat-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-03 14:56:47.000000 sneat-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:56:54.991489 sneat-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-06-03 14:56:47.000000 sneat-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:54.991489 sneat-0.0.6/sneat/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/neuralnetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-03 14:56:47.000000 sneat-0.0.6/sneat/species.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:56:54.991489 sneat-0.0.6/sneat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:56:54.000000 sneat-0.0.6/sneat.egg-info/top_level.txt
```

### Comparing `sneat-0.0.5/LICENSE` & `sneat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sneat-0.0.5/README.md` & `sneat-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sneat-0.0.5/sneat/config.py` & `sneat-0.0.6/sneat/config.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.5/sneat/evolve.py` & `sneat-0.0.6/sneat/evolve.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,41 @@
     print('\n')
     with Pool() as p:
         # set the fitness of all genomes using evaluate_genome (which returns a single fitness score), and tqdm for multiprocessing
         fitness_scores = list(tqdm(p.imap(evaluate_genome, [(g, ff) for g in pop.genomes]), total=len(pop.genomes), desc='[-] Evaluating', leave=False))
         for g, fitness in zip(pop.genomes, fitness_scores):
             g.fitness = fitness
 
+def save_checkpoint(pop):
+    with open('checkpoint.pkl', 'wb') as f:
+        pkl.dump(pop, f)
+
+def load_checkpoint():
+    try:
+        with open('checkpoint.pkl', 'rb') as f:
+            pop = pkl.load(f)
+            print(f'[i] Restoring from checkpoint (gen. {pop.generation})...')
+            return pop
+    except FileNotFoundError:
+        return None
+
 def print_stats(pop):
     print(f'\n\n[i] Gen. {pop.generation}:')
     headers = ['Species', 'Members', 'Best Fitness', 'Average Fitness']
     for s in pop.species:
         s.members = sorted(s.members, key=lambda x: x.fitness, reverse=True)
     species = sorted(pop.species, key=lambda x: x.members[0].fitness, reverse=True)
     data = [[s.id, len(s.members), round(max(g.fitness for g in s.members), 2), round(np.mean([g.fitness for g in s.members]), 2)] for s in species]
     print(tb(data, headers=headers))
     print('-' * 55)
 
 def evolve(fitness_function):
     config = get_config()
-    pop = Population()
+    
+    pop = load_checkpoint() or Population()
 
     max_generations = config.getint('Evolution', 'max_generations') or np.inf
     max_fitness = config.getfloat('Evolution', 'max_fitness') or np.inf
 
     try:
         for _ in range(max_generations):
             
@@ -48,14 +62,18 @@
 
             # print stats
             print_stats(pop)
 
             # reproduce
             pop.reproduce()
 
+            # save checkpoint
+            if pop.generation % 10 == 0:
+                save_checkpoint(pop)
+
             best_fitness = max(g.fitness for g in pop.genomes)
             if best_fitness >= max_fitness:
                 winner = max(pop.genomes, key=lambda x: x.fitness)
                 save_genome(winner, 'winner.pkl')
                 print(f'\n\n[+] Winner found with fitness: {winner.fitness}\n\n')
                 return winner
```

### Comparing `sneat-0.0.5/sneat/genome.py` & `sneat-0.0.6/sneat/genome.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.5/sneat/neuralnetwork.py` & `sneat-0.0.6/sneat/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.5/sneat/normalizer.py` & `sneat-0.0.6/sneat/normalizer.py`

 * *Files identical despite different names*

### Comparing `sneat-0.0.5/sneat/population.py` & `sneat-0.0.6/sneat/population.py`

 * *Files identical despite different names*

