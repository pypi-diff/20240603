# Comparing `tmp/useful_rdkit_utils-0.5.tar.gz` & `tmp/useful_rdkit_utils-0.51.tar.gz`

## Comparing `useful_rdkit_utils-0.5.tar` & `useful_rdkit_utils-0.51.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.gitattributes
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.lgtm.yml
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/CHANGELOG.md
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/MANIFEST.in
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/requirements.txt
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/ring_freq_test.csv
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/ring_test.csv
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.github/workflows/CI.yaml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/.gitignore
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/misc.xml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/useful_rdkit_utils.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/vcs.xml
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0  3405081 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/data/chembl_ring_systems.csv
--rw-r--r--   0        0        0    40140 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/data/hia_hou.tab
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/data/test.smi
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/Makefile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/conf.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/descriptors.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/geometry.rst
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/index.rst
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/installation.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/jupyter.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/misc_utils.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/pandas.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/reactions.rst
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/reos.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/ring_systems.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/seaborn.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/stats.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/units.rst
--rw-r--r--   0        0        0    33382 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/bootstrap_AUC.ipynb
--rw-r--r--   0        0        0   342969 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_REOS.ipynb
--rw-r--r--   0        0        0    54099 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_descriptors.ipynb
--rw-r--r--   0        0        0   461614 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_ring_systems.ipynb
--rw-r--r--   0        0        0   457681 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_useful_rdkit_utils.ipynb
--rw-r--r--   0        0        0    15105 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/explore_functional_group_filters.ipynb
--rw-r--r--   0        0        0   590968 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/zinc_sample.smi
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/ring_freq_test.csv
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/ring_test.csv
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test.smi
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test_reos.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test_ring_systems.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test_useful_rdkit_utils.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/__init__.py
--rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/descriptors.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/geometry.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/jupyter_utils.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/misc_utils.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/pandas_utils.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/reactions.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/reos.py
--rwxr-xr-x   0        0        0    11513 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/ring_systems.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/seaborn_utils.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/split_utils.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/stat_utils.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/units.py
--rw-r--r--   0        0        0  1097792 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/LICENSE
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/README.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/pyproject.toml
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.gitattributes
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.lgtm.yml
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.readthedocs.yaml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/CHANGELOG.md
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/MANIFEST.in
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/requirements.txt
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/ring_freq_test.csv
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/ring_test.csv
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.github/workflows/CI.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.idea/.gitignore
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.idea/misc.xml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.idea/useful_rdkit_utils.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.idea/vcs.xml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0  3405081 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/data/chembl_ring_systems.csv
+-rw-r--r--   0        0        0    40140 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/data/hia_hou.tab
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/data/test.smi
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/Makefile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/conf.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/descriptors.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/geometry.rst
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/index.rst
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/installation.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/jupyter.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/misc_utils.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/pandas.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/reactions.rst
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/reos.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/ring_systems.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/seaborn.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/stats.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/docs/source/units.rst
+-rw-r--r--   0        0        0    33382 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/bootstrap_AUC.ipynb
+-rw-r--r--   0        0        0   349052 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/demo_REOS.ipynb
+-rw-r--r--   0        0        0    54099 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/demo_descriptors.ipynb
+-rw-r--r--   0        0        0   461614 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/demo_ring_systems.ipynb
+-rw-r--r--   0        0        0   457681 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/demo_useful_rdkit_utils.ipynb
+-rw-r--r--   0        0        0    15105 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/explore_functional_group_filters.ipynb
+-rw-r--r--   0        0        0   590968 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/zinc_sample.smi
+-rw-r--r--   0        0        0    40140 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/notebooks/data/hia_hou.tab
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/tests/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/tests/ring_freq_test.csv
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/tests/ring_test.csv
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/tests/test.smi
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/tests/test_reos.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/tests/test_ring_systems.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/tests/test_useful_rdkit_utils.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/__init__.py
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/descriptors.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/geometry.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/jupyter_utils.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/misc_utils.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/reactions.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/reos.py
+-rwxr-xr-x   0        0        0    11513 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/ring_systems.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/seaborn_utils.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/split_utils.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/stat_utils.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/units.py
+-rw-r--r--   0        0        0  1097792 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/LICENSE
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/README.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/pyproject.toml
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.51/PKG-INFO
```

### Comparing `useful_rdkit_utils-0.5/.readthedocs.yaml` & `useful_rdkit_utils-0.51/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/CHANGELOG.md` & `useful_rdkit_utils-0.51/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/CODE_OF_CONDUCT.md` & `useful_rdkit_utils-0.51/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/ring_freq_test.csv` & `useful_rdkit_utils-0.51/ring_freq_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/ring_test.csv` & `useful_rdkit_utils-0.51/ring_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/.github/CONTRIBUTING.md` & `useful_rdkit_utils-0.51/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/.github/workflows/CI.yaml` & `useful_rdkit_utils-0.51/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/.idea/inspectionProfiles/Project_Default.xml` & `useful_rdkit_utils-0.51/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/data/chembl_ring_systems.csv` & `useful_rdkit_utils-0.51/data/chembl_ring_systems.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/data/hia_hou.tab` & `useful_rdkit_utils-0.51/data/hia_hou.tab`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/data/test.smi` & `useful_rdkit_utils-0.51/data/test.smi`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/docs/Makefile` & `useful_rdkit_utils-0.51/docs/Makefile`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/docs/source/conf.py` & `useful_rdkit_utils-0.51/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/docs/source/installation.rst` & `useful_rdkit_utils-0.51/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/notebooks/bootstrap_AUC.ipynb` & `useful_rdkit_utils-0.51/notebooks/bootstrap_AUC.ipynb`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/notebooks/demo_REOS.ipynb` & `useful_rdkit_utils-0.51/notebooks/demo_REOS.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931050174186431%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1}, 8: {'outputs': {0: {'data': {'text/plain': ['(1251, "*

 * *            '8)\']}}}}, 10: {\'outputs\': {0: {\'data\': {\'text/plain\': {insert: [(1, "       '*

 * *            '\'Inpharmatica\', \'LINT\'], dtype=object)")], delete: [1]}}}}}, 26: {\'outputs\': '*

 * *            "{0: {'data': {'text/html': {insert: [(38, '      <td>&lt;rdkit.Chem.rdchem.Mol object "*

 * *            "at 0x295f34040&gt;</td>\\n'), (49, '      <td>&lt;rdkit.Chem.rdchem.Mol object at "*

 * *            "0x295f3412 […]*

```diff
@@ -16,15 +16,15 @@
             "outputs": [],
             "source": [
                 "!pip install PyTDC mols2grid "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 1,
             "id": "afe65cfe",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from rdkit import Chem\n",
                 "from tdc.single_pred import ADME\n",
                 "import mols2grid\n",
@@ -94,15 +94,15 @@
             "execution_count": 4,
             "id": "9b86ec5d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(1325, 8)"
+                            "(1251, 8)"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -124,15 +124,15 @@
             "id": "a2ce4c65",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(['Glaxo', 'Dundee', 'BMS', 'PAINS', 'SureChEMBL', 'MLSMR',\n",
-                            "       'Inpharmatica', 'LINT', 'PW'], dtype=object)"
+                            "       'Inpharmatica', 'LINT'], dtype=object)"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -372,609 +372,609 @@
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R1 Reactive alkyl halides</td>\n",
                             "      <td>[Br,Cl,I][CX4;CH,CH2]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3e810&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34040&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>2</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R2 Acid halides</td>\n",
                             "      <td>[S,C](=[O,S])[F,Br,Cl,I]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3ece0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34120&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>3</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R3 Carbazides</td>\n",
                             "      <td>O=CN=[N+]=[N-]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3ed50&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34190&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>4</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R4 Sulphate esters</td>\n",
                             "      <td>COS(=O)O[C,c]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3edc0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34200&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>5</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R5 Sulphonates</td>\n",
                             "      <td>COS(=O)(=O)[C,c]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3ee30&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34270&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>6</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R6 Acid anhydrides</td>\n",
                             "      <td>C(=O)OC(=O)</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3eea0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f342e0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
                             "      <td>7</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R7 Peroxides</td>\n",
                             "      <td>OO</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3ef10&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34350&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
                             "      <td>8</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R8 Pentafluorophenyl esters</td>\n",
                             "      <td>C(=O)Oc1c(F)c(F)c(F)c(F)c1(F)</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3ef80&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f343c0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
                             "      <td>9</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R9 Paranitrophenyl esters</td>\n",
                             "      <td>C(=O)Oc1ccc(N(=O)~[OX1])cc1</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3eff0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34430&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
                             "      <td>10</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R10 esters of HOBT</td>\n",
                             "      <td>C(=O)Onnn</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f060&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f344a0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
                             "      <td>11</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R11 Isocyanates &amp; Isothiocyanates</td>\n",
                             "      <td>N=C=[S,O]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f0d0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34510&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>11</th>\n",
                             "      <td>12</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R12 Triflates</td>\n",
                             "      <td>OS(=O)(=O)C(F)(F)F</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f140&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34580&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>12</th>\n",
                             "      <td>13</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R13 lawesson's reagent and derivatives</td>\n",
                             "      <td>P(=S)(S)S</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f1b0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f345f0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>13</th>\n",
                             "      <td>14</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R14 phosphoramides</td>\n",
                             "      <td>NP(=O)(N)N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f220&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34660&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>14</th>\n",
                             "      <td>15</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R15 Aromatic azides</td>\n",
                             "      <td>cN=[N+]=[N-]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f290&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f346d0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>15</th>\n",
                             "      <td>16</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R16 beta carbonyl quaternary Nitrogen</td>\n",
                             "      <td>C(=O)C[N+,n+]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f300&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34740&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>16</th>\n",
                             "      <td>17</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R17 acylhydrazide</td>\n",
                             "      <td>[N;R0][N;R0]C(=O)</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f370&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f347b0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>17</th>\n",
                             "      <td>18</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R18 Quaternary C, Cl, I, P or S</td>\n",
                             "      <td>[C+,Cl+,I+,P+,S+]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f3e0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34820&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>18</th>\n",
                             "      <td>19</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R19 Phosphoranes</td>\n",
                             "      <td>C=P</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f450&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34890&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>19</th>\n",
                             "      <td>20</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R20 Chloramidines</td>\n",
                             "      <td>[Cl]C([C&amp;R0])=N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f4c0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34900&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>20</th>\n",
                             "      <td>21</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R21 Nitroso</td>\n",
                             "      <td>[N&amp;D2](=O)</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f530&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34970&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>21</th>\n",
                             "      <td>22</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R22 P/S Halides</td>\n",
                             "      <td>[P,S][Cl,Br,F,I]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f5a0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f349e0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>22</th>\n",
                             "      <td>23</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R23 Carbodiimide</td>\n",
                             "      <td>N=C=N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f610&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34a50&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>23</th>\n",
                             "      <td>24</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R24 Isonitrile</td>\n",
                             "      <td>[N+]#[C-]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f680&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34ac0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>24</th>\n",
                             "      <td>25</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R25 Triacyloximes</td>\n",
                             "      <td>C(=O)N(C(=O))OC(=O)</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f6f0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34b30&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>25</th>\n",
                             "      <td>26</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R26 Cyanohydrins</td>\n",
                             "      <td>N#CC[OH]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f760&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34ba0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>26</th>\n",
                             "      <td>27</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R27 Acyl cyanides</td>\n",
                             "      <td>N#CC(=O)</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f7d0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34c10&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>27</th>\n",
                             "      <td>28</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R28 Sulfonyl cyanides</td>\n",
                             "      <td>S(=O)(=O)C#N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f840&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34c80&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>28</th>\n",
                             "      <td>29</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R29 Cyanophosphonates</td>\n",
                             "      <td>P(OCC)(OCC)(=O)C#N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f8b0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34cf0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>29</th>\n",
                             "      <td>30</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R30 Azocyanamides</td>\n",
                             "      <td>[N;R0]=[N;R0]C#N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f920&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34d60&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>30</th>\n",
                             "      <td>31</td>\n",
                             "      <td>1</td>\n",
                             "      <td>R31 Azoalkanals</td>\n",
                             "      <td>[N;R0]=[N;R0]CC=O</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3f990&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34dd0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>31</th>\n",
                             "      <td>32</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I1 Aliphatic methylene chains 7 or more long</td>\n",
                             "      <td>[CD2;R0][CD2;R0][CD2;R0][CD2;R0][CD2;R0][CD2;R...</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fa00&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34e40&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>32</th>\n",
                             "      <td>33</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I2 Compounds with 4 or more acidic groups</td>\n",
                             "      <td>[C,S,P](=O)[OH].[C,S,P](=O)[OH].[C,S,P](=O)[OH...</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fa70&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34eb0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>33</th>\n",
                             "      <td>34</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I3 Crown ethers</td>\n",
                             "      <td>[O;R1][C;R1][C;R1][O;R1][C;R1][C;R1][O;R1]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fae0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34f20&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>34</th>\n",
                             "      <td>35</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I4 Disulphides</td>\n",
                             "      <td>SS</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fb50&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f34f90&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>35</th>\n",
                             "      <td>36</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I5 Thiols</td>\n",
                             "      <td>[SH]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fbc0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35000&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>36</th>\n",
                             "      <td>37</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I6 Epoxides, Thioepoxides, Aziridines</td>\n",
                             "      <td>C1[O,S,N]C1</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fc30&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35070&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>37</th>\n",
                             "      <td>38</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I7 2,4,5 trihydroxyphenyl</td>\n",
                             "      <td>c([OH])c([OH])c([OH])</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fca0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f350e0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>38</th>\n",
                             "      <td>39</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I8 2,3,4 trihydroxyphenyl</td>\n",
                             "      <td>c([OH])c([OH])cc([OH])</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fd10&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35150&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>39</th>\n",
                             "      <td>40</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I9 Hydrazothiourea</td>\n",
                             "      <td>N=NC(=S)N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fd80&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f351c0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>40</th>\n",
                             "      <td>41</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I10 Thiocyanate</td>\n",
                             "      <td>SC#N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fdf0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35230&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>41</th>\n",
                             "      <td>42</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I11 Benzylic quaternary Nitrogen</td>\n",
                             "      <td>cC[N+]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fe60&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f352a0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>42</th>\n",
                             "      <td>43</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I12 Thioesters</td>\n",
                             "      <td>C[O,S;R0][C;R0](=S)</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3fed0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35310&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>43</th>\n",
                             "      <td>44</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I13 Cyanamides</td>\n",
                             "      <td>N[CH2]C#N</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e3ff40&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35380&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>44</th>\n",
                             "      <td>45</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I14 Four membered lactones</td>\n",
                             "      <td>C1(=O)OCC1</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e54040&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f353f0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>45</th>\n",
                             "      <td>46</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I15 Di and Triphosphates</td>\n",
                             "      <td>P(=O)([OH])OP(=O)[OH]</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e540b0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35460&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>46</th>\n",
                             "      <td>47</td>\n",
                             "      <td>1</td>\n",
                             "      <td>I16 Betalactams</td>\n",
                             "      <td>N1CCC1=O</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e54120&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f354d0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>47</th>\n",
                             "      <td>48</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N1 Quinones</td>\n",
                             "      <td>O=C1[#6]~[#6]C(=O)[#6]~[#6]1</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e54190&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35540&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>48</th>\n",
                             "      <td>49</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N2 Polyenes</td>\n",
                             "      <td>C=CC=CC=CC=C</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e54200&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f355b0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>49</th>\n",
                             "      <td>50</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N3 Saponin derivatives</td>\n",
                             "      <td>O1CCCCC1OC2CCC3CCCCC3C2</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e54270&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35620&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>50</th>\n",
                             "      <td>51</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N4 Cytochalasin derivatives</td>\n",
                             "      <td>O=C1NCC2CCCCC21</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e542e0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35690&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>51</th>\n",
                             "      <td>52</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N5 Cycloheximide derivatives</td>\n",
                             "      <td>O=C1CCCC(N1)=O</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e54350&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35700&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>52</th>\n",
                             "      <td>53</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N6 Monensin derivatives</td>\n",
                             "      <td>O1CCCCC1C2CCCO2</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e543c0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35770&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>53</th>\n",
                             "      <td>54</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N7 Cyanidin derivatives</td>\n",
                             "      <td>[OH]c1cc([OH])cc2=[O+]C(=C([OH])Cc21)c3cc([OH]...</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e54430&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f357e0&gt;</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>54</th>\n",
                             "      <td>55</td>\n",
                             "      <td>1</td>\n",
                             "      <td>N8 Squalestatin derivatives</td>\n",
                             "      <td>C12OCCC(O1)CC2</td>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>8</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x287e544a0&gt;</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295f35850&gt;</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "    rule_id  rule_set                                   description  \\\n",
@@ -1088,69 +1088,69 @@
                             "50                                    O=C1NCC2CCCCC21         Glaxo         8   \n",
                             "51                                     O=C1CCCC(N1)=O         Glaxo         8   \n",
                             "52                                    O1CCCCC1C2CCCO2         Glaxo         8   \n",
                             "53  [OH]c1cc([OH])cc2=[O+]C(=C([OH])Cc21)c3cc([OH]...         Glaxo         8   \n",
                             "54                                     C12OCCC(O1)CC2         Glaxo         8   \n",
                             "\n",
                             "    max                                            pat  \n",
-                            "0     0  <rdkit.Chem.rdchem.Mol object at 0x287e3e810>  \n",
-                            "1     0  <rdkit.Chem.rdchem.Mol object at 0x287e3ece0>  \n",
-                            "2     0  <rdkit.Chem.rdchem.Mol object at 0x287e3ed50>  \n",
-                            "3     0  <rdkit.Chem.rdchem.Mol object at 0x287e3edc0>  \n",
-                            "4     0  <rdkit.Chem.rdchem.Mol object at 0x287e3ee30>  \n",
-                            "5     0  <rdkit.Chem.rdchem.Mol object at 0x287e3eea0>  \n",
-                            "6     0  <rdkit.Chem.rdchem.Mol object at 0x287e3ef10>  \n",
-                            "7     0  <rdkit.Chem.rdchem.Mol object at 0x287e3ef80>  \n",
-                            "8     0  <rdkit.Chem.rdchem.Mol object at 0x287e3eff0>  \n",
-                            "9     0  <rdkit.Chem.rdchem.Mol object at 0x287e3f060>  \n",
-                            "10    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f0d0>  \n",
-                            "11    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f140>  \n",
-                            "12    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f1b0>  \n",
-                            "13    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f220>  \n",
-                            "14    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f290>  \n",
-                            "15    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f300>  \n",
-                            "16    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f370>  \n",
-                            "17    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f3e0>  \n",
-                            "18    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f450>  \n",
-                            "19    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f4c0>  \n",
-                            "20    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f530>  \n",
-                            "21    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f5a0>  \n",
-                            "22    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f610>  \n",
-                            "23    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f680>  \n",
-                            "24    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f6f0>  \n",
-                            "25    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f760>  \n",
-                            "26    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f7d0>  \n",
-                            "27    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f840>  \n",
-                            "28    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f8b0>  \n",
-                            "29    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f920>  \n",
-                            "30    0  <rdkit.Chem.rdchem.Mol object at 0x287e3f990>  \n",
-                            "31    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fa00>  \n",
-                            "32    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fa70>  \n",
-                            "33    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fae0>  \n",
-                            "34    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fb50>  \n",
-                            "35    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fbc0>  \n",
-                            "36    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fc30>  \n",
-                            "37    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fca0>  \n",
-                            "38    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fd10>  \n",
-                            "39    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fd80>  \n",
-                            "40    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fdf0>  \n",
-                            "41    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fe60>  \n",
-                            "42    0  <rdkit.Chem.rdchem.Mol object at 0x287e3fed0>  \n",
-                            "43    0  <rdkit.Chem.rdchem.Mol object at 0x287e3ff40>  \n",
-                            "44    0  <rdkit.Chem.rdchem.Mol object at 0x287e54040>  \n",
-                            "45    0  <rdkit.Chem.rdchem.Mol object at 0x287e540b0>  \n",
-                            "46    0  <rdkit.Chem.rdchem.Mol object at 0x287e54120>  \n",
-                            "47    0  <rdkit.Chem.rdchem.Mol object at 0x287e54190>  \n",
-                            "48    0  <rdkit.Chem.rdchem.Mol object at 0x287e54200>  \n",
-                            "49    0  <rdkit.Chem.rdchem.Mol object at 0x287e54270>  \n",
-                            "50    0  <rdkit.Chem.rdchem.Mol object at 0x287e542e0>  \n",
-                            "51    0  <rdkit.Chem.rdchem.Mol object at 0x287e54350>  \n",
-                            "52    0  <rdkit.Chem.rdchem.Mol object at 0x287e543c0>  \n",
-                            "53    0  <rdkit.Chem.rdchem.Mol object at 0x287e54430>  \n",
-                            "54    0  <rdkit.Chem.rdchem.Mol object at 0x287e544a0>  "
+                            "0     0  <rdkit.Chem.rdchem.Mol object at 0x295f34040>  \n",
+                            "1     0  <rdkit.Chem.rdchem.Mol object at 0x295f34120>  \n",
+                            "2     0  <rdkit.Chem.rdchem.Mol object at 0x295f34190>  \n",
+                            "3     0  <rdkit.Chem.rdchem.Mol object at 0x295f34200>  \n",
+                            "4     0  <rdkit.Chem.rdchem.Mol object at 0x295f34270>  \n",
+                            "5     0  <rdkit.Chem.rdchem.Mol object at 0x295f342e0>  \n",
+                            "6     0  <rdkit.Chem.rdchem.Mol object at 0x295f34350>  \n",
+                            "7     0  <rdkit.Chem.rdchem.Mol object at 0x295f343c0>  \n",
+                            "8     0  <rdkit.Chem.rdchem.Mol object at 0x295f34430>  \n",
+                            "9     0  <rdkit.Chem.rdchem.Mol object at 0x295f344a0>  \n",
+                            "10    0  <rdkit.Chem.rdchem.Mol object at 0x295f34510>  \n",
+                            "11    0  <rdkit.Chem.rdchem.Mol object at 0x295f34580>  \n",
+                            "12    0  <rdkit.Chem.rdchem.Mol object at 0x295f345f0>  \n",
+                            "13    0  <rdkit.Chem.rdchem.Mol object at 0x295f34660>  \n",
+                            "14    0  <rdkit.Chem.rdchem.Mol object at 0x295f346d0>  \n",
+                            "15    0  <rdkit.Chem.rdchem.Mol object at 0x295f34740>  \n",
+                            "16    0  <rdkit.Chem.rdchem.Mol object at 0x295f347b0>  \n",
+                            "17    0  <rdkit.Chem.rdchem.Mol object at 0x295f34820>  \n",
+                            "18    0  <rdkit.Chem.rdchem.Mol object at 0x295f34890>  \n",
+                            "19    0  <rdkit.Chem.rdchem.Mol object at 0x295f34900>  \n",
+                            "20    0  <rdkit.Chem.rdchem.Mol object at 0x295f34970>  \n",
+                            "21    0  <rdkit.Chem.rdchem.Mol object at 0x295f349e0>  \n",
+                            "22    0  <rdkit.Chem.rdchem.Mol object at 0x295f34a50>  \n",
+                            "23    0  <rdkit.Chem.rdchem.Mol object at 0x295f34ac0>  \n",
+                            "24    0  <rdkit.Chem.rdchem.Mol object at 0x295f34b30>  \n",
+                            "25    0  <rdkit.Chem.rdchem.Mol object at 0x295f34ba0>  \n",
+                            "26    0  <rdkit.Chem.rdchem.Mol object at 0x295f34c10>  \n",
+                            "27    0  <rdkit.Chem.rdchem.Mol object at 0x295f34c80>  \n",
+                            "28    0  <rdkit.Chem.rdchem.Mol object at 0x295f34cf0>  \n",
+                            "29    0  <rdkit.Chem.rdchem.Mol object at 0x295f34d60>  \n",
+                            "30    0  <rdkit.Chem.rdchem.Mol object at 0x295f34dd0>  \n",
+                            "31    0  <rdkit.Chem.rdchem.Mol object at 0x295f34e40>  \n",
+                            "32    0  <rdkit.Chem.rdchem.Mol object at 0x295f34eb0>  \n",
+                            "33    0  <rdkit.Chem.rdchem.Mol object at 0x295f34f20>  \n",
+                            "34    0  <rdkit.Chem.rdchem.Mol object at 0x295f34f90>  \n",
+                            "35    0  <rdkit.Chem.rdchem.Mol object at 0x295f35000>  \n",
+                            "36    0  <rdkit.Chem.rdchem.Mol object at 0x295f35070>  \n",
+                            "37    0  <rdkit.Chem.rdchem.Mol object at 0x295f350e0>  \n",
+                            "38    0  <rdkit.Chem.rdchem.Mol object at 0x295f35150>  \n",
+                            "39    0  <rdkit.Chem.rdchem.Mol object at 0x295f351c0>  \n",
+                            "40    0  <rdkit.Chem.rdchem.Mol object at 0x295f35230>  \n",
+                            "41    0  <rdkit.Chem.rdchem.Mol object at 0x295f352a0>  \n",
+                            "42    0  <rdkit.Chem.rdchem.Mol object at 0x295f35310>  \n",
+                            "43    0  <rdkit.Chem.rdchem.Mol object at 0x295f35380>  \n",
+                            "44    0  <rdkit.Chem.rdchem.Mol object at 0x295f353f0>  \n",
+                            "45    0  <rdkit.Chem.rdchem.Mol object at 0x295f35460>  \n",
+                            "46    0  <rdkit.Chem.rdchem.Mol object at 0x295f354d0>  \n",
+                            "47    0  <rdkit.Chem.rdchem.Mol object at 0x295f35540>  \n",
+                            "48    0  <rdkit.Chem.rdchem.Mol object at 0x295f355b0>  \n",
+                            "49    0  <rdkit.Chem.rdchem.Mol object at 0x295f35620>  \n",
+                            "50    0  <rdkit.Chem.rdchem.Mol object at 0x295f35690>  \n",
+                            "51    0  <rdkit.Chem.rdchem.Mol object at 0x295f35700>  \n",
+                            "52    0  <rdkit.Chem.rdchem.Mol object at 0x295f35770>  \n",
+                            "53    0  <rdkit.Chem.rdchem.Mol object at 0x295f357e0>  \n",
+                            "54    0  <rdkit.Chem.rdchem.Mol object at 0x295f35850>  "
                         ]
                     },
                     "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1202,15 +1202,15 @@
             "id": "29cbab7e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x287e3d690>"
+                            "<rdkit.Chem.rdchem.Mol at 0x295f069d0>"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1254,16 +1254,15 @@
             "id": "06c6150a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Downloading...\n",
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 40.1k/40.1k [00:00<00:00, 9.65MiB/s]\n",
+                        "Found local copy...\n",
                         "Loading...\n",
                         "Done!\n"
                     ]
                 }
             ],
             "source": [
                 "hia_data = ADME(name = 'HIA_Hou').get_data()"
@@ -1594,15 +1593,15 @@
             "execution_count": 22,
             "id": "5714c50a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "378d57b466b94b44848866fb8f874272",
+                            "model_id": "fdeb840023ac4f8f840d5e74a518b1c5",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "MolGridWidget()"
                         ]
                     },
@@ -2772,26 +2771,26 @@
                             "            \n",
                             "            &lt;div class=&quot;m2g-list&quot;&gt;&lt;div class=&quot;m2g-cell&quot; data-mols2grid-id=&quot;0&quot; tabindex=&quot;0&quot;&gt;&lt;div class=&quot;m2g-cb-wrap&quot;&gt;&lt;input type=&quot;checkbox&quot; tabindex=&quot;-1&quot; class=&quot;position-relative float-left cached_checkbox&quot;&gt;&lt;div class=&quot;m2g-cb&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data-mols2grid-id-display&quot;&gt;&lt;/div&gt;&lt;/div&gt;&lt;div class=&quot;m2g-cell-actions&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-img copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-Drug_ID copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-reos copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-rule_set_name copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-Drug copy-me&quot; style=&quot;display: none;&quot;&gt;&lt;/div&gt;&lt;/div&gt;&lt;/div&gt;\n",
                             "        &lt;/div&gt;\n",
                             "        &lt;script&gt;\n",
                             "            // list.js\n",
                             "var listObj = new List(&#x27;mols2grid&#x27;, {\n",
                             "    listClass: &#x27;m2g-list&#x27;,\n",
-                            "    valueNames: [{data: [&#x27;mols2grid-id&#x27;]}, &#x27;data-Drug&#x27;, &#x27;data-reos&#x27;, &#x27;data-rule_set_name&#x27;, &#x27;data-Drug_ID&#x27;, &#x27;data-img&#x27;, &#x27;data-mols2grid-id&#x27;, &#x27;data-mols2grid-id-display&#x27;],\n",
+                            "    valueNames: [{data: [&#x27;mols2grid-id&#x27;]}, &#x27;data-reos&#x27;, &#x27;data-rule_set_name&#x27;, &#x27;data-mols2grid-id&#x27;, &#x27;data-img&#x27;, &#x27;data-Drug_ID&#x27;, &#x27;data-Drug&#x27;, &#x27;data-mols2grid-id-display&#x27;],\n",
                             "    item: &#x27;&lt;div class=&quot;m2g-cell&quot; data-mols2grid-id=&quot;0&quot; tabindex=&quot;0&quot;&gt;&lt;div class=&quot;m2g-cb-wrap&quot;&gt;&lt;input type=&quot;checkbox&quot; tabindex=&quot;-1&quot; class=&quot;position-relative float-left cached_checkbox&quot;&gt;&lt;div class=&quot;m2g-cb&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data-mols2grid-id-display&quot;&gt;&lt;/div&gt;&lt;/div&gt;&lt;div class=&quot;m2g-cell-actions&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-img copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-Drug_ID copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-reos copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-rule_set_name copy-me&quot;&gt;&lt;/div&gt;&lt;div class=&quot;data data-Drug copy-me&quot; style=&quot;display: none;&quot;&gt;&lt;/div&gt;&lt;/div&gt;&#x27;,\n",
                             "    page: 24,\n",
                             "    pagination: {\n",
                             "        paginationClass: &quot;m2g-pagination&quot;,\n",
                             "        item: &#x27;&lt;li class=&quot;page-item&quot;&gt;&lt;a class=&quot;page page-link&quot; href=&quot;#&quot; onclick=&quot;event.preventDefault()&quot;&gt;&lt;/a&gt;&lt;/li&gt;&#x27;,\n",
                             "        innerWindow: 1,\n",
                             "        outerWindow: 1,\n",
                             "    },\n",
                             "});\n",
                             "listObj.remove(&quot;mols2grid-id&quot;, &quot;0&quot;);\n",
-                            "listObj.add([{&quot;data-Drug&quot;: &quot;COc1ccc(C[C@H]2c3cc(OC)c(OC)cc3CC[N@@+]2(C)CCC(=O)OCCCCCOC(=O)CC[N@+]2(C)CCc3cc(OC)c(OC)cc3[C@@H]2Cc2ccc(OC)c(OC)c2)cc1OC&quot;, &quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Atracurium.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 0, &quot;data-mols2grid-id-display&quot;: 0}, {&quot;data-Drug&quot;: &quot;C[N+](C)(CCOc1ccccc1)Cc1ccccc1&quot;, &quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Bephenium&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 1, &quot;data-mols2grid-id-display&quot;: 1}, {&quot;data-Drug&quot;: &quot;CC[N+](C)(C)Cc1ccccc1Br&quot;, &quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Bretylium.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 2, &quot;data-mols2grid-id-display&quot;: 2}, {&quot;data-Drug&quot;: &quot;COc1cc2c(cc1OC)[C@H](Cc1cc(OC)c(OC)c(OC)c1)[N@+](C)(CCCOC(=O)CC/C=C/CCC(=O)OCCC[N@+]1(C)CCc3cc(OC)c(OC)cc3[C@@H]1Cc1cc(OC)c(OC)c(OC)c1)CC2&quot;, &quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Mivacurium.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 3, &quot;data-mols2grid-id-display&quot;: 3}, {&quot;data-Drug&quot;: &quot;COc1cc2c3cc1Oc1cc(ccc1O)C[C@@H]1c4c(cc(OC)c(O)c4Oc4ccc(cc4)C[C@@H]3[N+](C)(C)CC2)CC[N+]1(C)C&quot;, &quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Tubocurarine&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 4, &quot;data-mols2grid-id-display&quot;: 4}, {&quot;data-Drug&quot;: &quot;CC1=C(C(=O)O)N2C(=O)[C@H](NC(=O)[C@@H](N)C3=CCC=CC3)[C@@H]2SC1&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Cephradine.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 5, &quot;data-mols2grid-id-display&quot;: 5}, {&quot;data-Drug&quot;: &quot;Cc1onc(-c2c(F)cccc2Cl)c1C(=O)N[C@@H]1C(=O)N2[C@H]1SC(C)(C)[C@H]2C(=O)O&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Floxacillin.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 6, &quot;data-mols2grid-id-display&quot;: 6}, {&quot;data-Drug&quot;: &quot;O=C(O)[C@@H]1C(=CCO)O[C@H]2CC(=O)N21&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Clavulanic_acid.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 7, &quot;data-mols2grid-id-display&quot;: 7}, {&quot;data-Drug&quot;: &quot;CO/N=C(\\\\C(=O)N[C@@H]1C(=O)N2C(C(=O)O)=CCS[C@@H]12)c1csc(N)n1&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Ceftizoxime.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 8, &quot;data-mols2grid-id-display&quot;: 8}, {&quot;data-Drug&quot;: &quot;COCC1=C(C(=O)O[C@H](C)OC(=O)OC(C)C)N2C(=O)[C@H](NC(=O)C(=NOC)c3csc(N)n3)[C@@H]2SC1&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Cefpodoxime_proxetil.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 9, &quot;data-mols2grid-id-display&quot;: 9}, {&quot;data-Drug&quot;: &quot;CO[C@@]1(NC(=O)CSCC#N)C(=O)N2C(C(=O)O)=C(CSc3nnnn3C)CS[C@H]21&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Cefmetazole&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 10, &quot;data-mols2grid-id-display&quot;: 10}, {&quot;data-Drug&quot;: &quot;C=C(N[C@@H]1C(=O)N2C(C(=O)O)=C(COC(C)=O)CS[C@@H]12)C(=NOC)c1csc(N)n1&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Cefotaxime&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 11, &quot;data-mols2grid-id-display&quot;: 11}, {&quot;data-Drug&quot;: &quot;C[C@H](O)[C@@H]1C(=O)N2C(C(=O)O)=C(SCC/N=C/N)C[C@@H]12&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Imipenem.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 12, &quot;data-mols2grid-id-display&quot;: 12}, {&quot;data-Drug&quot;: &quot;CC1(C)[C@H](C(=O)O)N2C(=O)C[C@@H]2S1(=O)=O&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Sulbactam&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 13, &quot;data-mols2grid-id-display&quot;: 13}, {&quot;data-Drug&quot;: &quot;CC1(C)S[C@H]2[C@@H](NC(=O)[C@@H](C(=O)O)c3ccsc3)C(=O)N2[C@@H]1C(=O)O&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Ticarcillin&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 14, &quot;data-mols2grid-id-display&quot;: 14}, {&quot;data-Drug&quot;: &quot;C[C@@H]1[C@@H](NC(=O)/C(=N\\\\OC(C)(C)C(=O)O)c2csc(N)n2)C(=O)N1S(=O)(=O)O&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Aztreonam.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 15, &quot;data-mols2grid-id-display&quot;: 15}, {&quot;data-Drug&quot;: &quot;CON=C(C(=O)N[C@H]1C(=O)N2C(C(=O)O)=C(CSc3nc(=O)c(O)nn3C)CS[C@@H]12)c1csc(N)n1&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Ceftriaxone.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 16, &quot;data-mols2grid-id-display&quot;: 16}, {&quot;data-Drug&quot;: &quot;CC1(C)S[C@H]2[C@@H](NC(=O)[C@@H](NC(=O)N3CCNC3=O)c3ccccc3)C(=O)N2[C@@H]1C(=O)O&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Azlocillin.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 17, &quot;data-mols2grid-id-display&quot;: 17}, {&quot;data-Drug&quot;: &quot;CON=C(C(=O)N[C@H]1C(=O)N2C(C(=O)O)=C(CSc3nc(C)c(CC(=O)O)s3)CS[C@@H]12)c1csc(N)n1&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Cefodizime.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 18, &quot;data-mols2grid-id-display&quot;: 18}, {&quot;data-Drug&quot;: &quot;C[C@H](O)[C@H]1C(=O)N2C(C(=O)O)=C(S[C@@H]3CC[C@H](C(=O)N(C)C)N3)[C@@H](C)[C@H]12&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Meropenem.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 19, &quot;data-mols2grid-id-display&quot;: 19}, {&quot;data-Drug&quot;: &quot;CC1(C)S[C@H]2[C@@H](NC(=O)[C@@H](NC(=O)N3CCN(S(C)(=O)=O)C3=O)c3ccccc3)C(=O)N2[C@@H]1C(=O)O&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Mezlocillin&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 20, &quot;data-mols2grid-id-display&quot;: 20}, {&quot;data-Drug&quot;: &quot;CO/N=C(\\\\C(=O)N[C@@H]1C(=O)N2C(C(=O)O)=C(C[n+]3ccccc3)CS[C@@H]12)c1csc(N)n1&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Cefpirome&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 21, &quot;data-mols2grid-id-display&quot;: 21}, {&quot;data-Drug&quot;: &quot;CC(C)(O/N=C(\\\\C(=O)N[C@@H]1C(=O)N2C(C(=O)O)=C(C[n+]3ccccc3)CS[C@@H]12)c1csc(N)n1)C(=O)O&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Ceftazidime.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 22, &quot;data-mols2grid-id-display&quot;: 22}, {&quot;data-Drug&quot;: &quot;CO[C@@]1(NC(=O)[C@@H](C(=O)O)c2ccc(O)cc2)C(=O)N2C(C(=O)O)=C(CSc3nnnn3C)CO[C@H]21&quot;, &quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Moxalactam.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 23, &quot;data-mols2grid-id-display&quot;: 23}, {&quot;data-Drug&quot;: &quot;O=C(O)CN(CCN(CC(=O)O)CC(=O)O)CC(=O)O&quot;, &quot;data-reos&quot;: &quot;I2 Compounds with 4 or more acidic groups&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Edetic_acid&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 24, &quot;data-mols2grid-id-display&quot;: 24}, {&quot;data-Drug&quot;: &quot;CCN(CC)C(=S)SSC(=S)N(CC)CC&quot;, &quot;data-reos&quot;: &quot;I4 Disulphides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Disulfiram&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 25, &quot;data-mols2grid-id-display&quot;: 25}, {&quot;data-Drug&quot;: &quot;CN1[C@H]2C[C@H](OC(=O)[C@@H](CO)c3ccccc3)C[C@@H]1[C@@H]1O[C@H]12&quot;, &quot;data-reos&quot;: &quot;I6 Epoxides, Thioepoxides, Aziridines&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Scopolamine.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 26, &quot;data-mols2grid-id-display&quot;: 26}, {&quot;data-Drug&quot;: &quot;CCCC[N+]1(C)[C@@H]2C[C@@H](OC(=O)[C@@H](CO)c3ccccc3)C[C@@H]1[C@H]1O[C@H]12&quot;, &quot;data-reos&quot;: &quot;I6 Epoxides, Thioepoxides, Aziridines&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Butylscopolamine&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 27, &quot;data-mols2grid-id-display&quot;: 27}, {&quot;data-Drug&quot;: &quot;CC[N+]1(C)[C@@H]2C[C@@H](OC(=O)[C@@H](CO)c3ccccc3)C[C@@H]1[C@H]1O[C@H]12&quot;, &quot;data-reos&quot;: &quot;I6 Epoxides, Thioepoxides, Aziridines&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Oxitropium.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 28, &quot;data-mols2grid-id-display&quot;: 28}, {&quot;data-Drug&quot;: &quot;O=C1c2c(O)ccc(O)c2C(=O)c2c(NCCNCCO)ccc(NCCNCCO)c21&quot;, &quot;data-reos&quot;: &quot;N1 Quinones&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Mitoxantrone&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 29, &quot;data-mols2grid-id-display&quot;: 29}, {&quot;data-Drug&quot;: &quot;CC(=CC(=O)O)/C=C/C=C(C)\\\\C=C/C1=C(C)CCCC1(C)C&quot;, &quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Isotretinoin.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 30, &quot;data-mols2grid-id-display&quot;: 30}, {&quot;data-Drug&quot;: &quot;CC(=CCO)/C=C/C=C(C)\\\\C=C\\\\C1=C(C)CCCC1(C)C&quot;, &quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Vitamin_A&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 31, &quot;data-mols2grid-id-display&quot;: 31}, {&quot;data-Drug&quot;: &quot;C[C@@H]1OC(=O)C[C@H](O)C[C@H](O)CC[C@@H](O)[C@H](O)C[C@H](O)C[C@@]2(O)C[C@@H](O)[C@@H](C(=O)O)[C@H](C[C@@](O)(O[C@@H]3O[C@@H](C)[C@@H](O)[C@H](N)[C@@H]3O)C=CC=CC=CC=CC=CC=CC=C[C@@H](C)[C@H](O)[C@@H]1C)O2&quot;, &quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Amphotericin_B.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 32, &quot;data-mols2grid-id-display&quot;: 32}, {&quot;data-Drug&quot;: &quot;COc1cc(C)c(/C=C/C(C)=C/C=C/C(C)=CC(=O)O)c(C)c1C&quot;, &quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Acitretin.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 33, &quot;data-mols2grid-id-display&quot;: 33}, {&quot;data-Drug&quot;: &quot;C=C[C@@]12CC[C@@H](O[C@H]3C[C@@H](OC)[C@@H](O)[C@H](C)O3)C[C@]1(O)CC[C@@H]1[C@@H]2CC[C@]2(C)[C@H](C3=CC(=O)OC3)CC[C@@]12O&quot;, &quot;data-reos&quot;: &quot;N3 Saponin derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Cymarin&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 34, &quot;data-mols2grid-id-display&quot;: 34}, {&quot;data-Drug&quot;: &quot;CCN(CC)CC[C@]1(c2ccccc2)CCC(=O)NC1=O&quot;, &quot;data-reos&quot;: &quot;N5 Cycloheximide derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Phenglutarimide&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 35, &quot;data-mols2grid-id-display&quot;: 35}, {&quot;data-Drug&quot;: &quot;CC[C@@]1(c2ccc(N)cc2)CCC(=O)NC1=O&quot;, &quot;data-reos&quot;: &quot;N5 Cycloheximide derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Aminoglutethimide&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 36, &quot;data-mols2grid-id-display&quot;: 36}, {&quot;data-Drug&quot;: &quot;O=C1CC2(CCCC2)CC(=O)N1CCCCN1CCN(c2ncccn2)CC1&quot;, &quot;data-reos&quot;: &quot;N5 Cycloheximide derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Buspirone.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 37, &quot;data-mols2grid-id-display&quot;: 37}, {&quot;data-Drug&quot;: &quot;O=NN(CCCl)C(=O)NCCCl&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Carmustine&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 38, &quot;data-mols2grid-id-display&quot;: 38}, {&quot;data-Drug&quot;: &quot;CN(C)CCOc1ccc(C(=C(CCCl)c2ccccc2)c2ccccc2)cc1&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Toremifene.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 39, &quot;data-mols2grid-id-display&quot;: 39}, {&quot;data-Drug&quot;: &quot;O=[P@@]1(N(CCCl)CCCl)OCCCN1CCCl&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Trofosfamide&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 40, &quot;data-mols2grid-id-display&quot;: 40}, {&quot;data-Drug&quot;: &quot;Cc1ncsc1CCCl&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Clomethiazole.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 41, &quot;data-mols2grid-id-display&quot;: 41}, {&quot;data-Drug&quot;: &quot;CN(C(=O)C(Cl)Cl)c1ccc(O)cc1&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Diloxanide&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 42, &quot;data-mols2grid-id-display&quot;: 42}, {&quot;data-Drug&quot;: &quot;CCC[C@@H]1C[C@H](C(=O)N[C@@H]([C@H](C)Cl)[C@@H]2O[C@@H](SC)[C@@H](O)[C@@H](O)[C@@H]2O)N(C)C1&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Clindamycin.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 43, &quot;data-mols2grid-id-display&quot;: 43}, {&quot;data-Drug&quot;: &quot;O=C(O)CCCc1ccc(N(CCCl)CCCl)cc1&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Chlorambucil.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 44, &quot;data-mols2grid-id-display&quot;: 44}, {&quot;data-Drug&quot;: &quot;O=C(N[C@H](CO)[C@@H](O)c1ccc([N+](=O)[O-])cc1)C(Cl)Cl&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Chloramphenicol.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 45, &quot;data-mols2grid-id-display&quot;: 45}, {&quot;data-Drug&quot;: &quot;C[C@@]12CC[C@@H]3c4ccc(OC(=O)N(CCCl)CCCl)cc4CC[C@@H]3[C@H]1CC[C@@H]2O&quot;, &quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Estramustine&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 46, &quot;data-mols2grid-id-display&quot;: 46}, {&quot;data-Drug&quot;: &quot;NNC(=O)c1ccncc1&quot;, &quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Isoniazid.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 47, &quot;data-mols2grid-id-display&quot;: 47}, {&quot;data-Drug&quot;: &quot;N[C@H](CO)C(=O)NNCc1ccc(O)c(O)c1O&quot;, &quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Benserazide&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 48, &quot;data-mols2grid-id-display&quot;: 48}, {&quot;data-Drug&quot;: &quot;Cc1cc(C(=O)NNCc2ccccc2)no1&quot;, &quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Isocarboxazid&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 49, &quot;data-mols2grid-id-display&quot;: 49}, {&quot;data-Drug&quot;: &quot;CN(N=O)C(=O)N[C@H]1[C@@H](O)O[C@@H](CO)[C@@H](O)[C@H]1O&quot;, &quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Streptozocin.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 50, &quot;data-mols2grid-id-display&quot;: 50}, {&quot;data-Drug&quot;: &quot;NNC(=O)NNN1C(=O)c2cc(S(=O)(=O)O)cc3c(N)c(S(=O)(=O)O)cc(c23)C1=O&quot;, &quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;data-Drug_ID&quot;: &quot;Lucifer_Yellow_CH.mol&quot;, &quot;data-img&quot;: null, &quot;mols2grid-id&quot;: 51, &quot;data-mols2grid-id-display&quot;: 51}]);\n",
+                            "listObj.add([{&quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 0, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Atracurium.mol&quot;, &quot;data-Drug&quot;: &quot;COc1ccc(C[C@H]2c3cc(OC)c(OC)cc3CC[N@@+]2(C)CCC(=O)OCCCCCOC(=O)CC[N@+]2(C)CCc3cc(OC)c(OC)cc3[C@@H]2Cc2ccc(OC)c(OC)c2)cc1OC&quot;, &quot;data-mols2grid-id-display&quot;: 0}, {&quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 1, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Bephenium&quot;, &quot;data-Drug&quot;: &quot;C[N+](C)(CCOc1ccccc1)Cc1ccccc1&quot;, &quot;data-mols2grid-id-display&quot;: 1}, {&quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 2, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Bretylium.mol&quot;, &quot;data-Drug&quot;: &quot;CC[N+](C)(C)Cc1ccccc1Br&quot;, &quot;data-mols2grid-id-display&quot;: 2}, {&quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 3, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Mivacurium.mol&quot;, &quot;data-Drug&quot;: &quot;COc1cc2c(cc1OC)[C@H](Cc1cc(OC)c(OC)c(OC)c1)[N@+](C)(CCCOC(=O)CC/C=C/CCC(=O)OCCC[N@+]1(C)CCc3cc(OC)c(OC)cc3[C@@H]1Cc1cc(OC)c(OC)c(OC)c1)CC2&quot;, &quot;data-mols2grid-id-display&quot;: 3}, {&quot;data-reos&quot;: &quot;I11 Benzylic quaternary Nitrogen&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 4, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Tubocurarine&quot;, &quot;data-Drug&quot;: &quot;COc1cc2c3cc1Oc1cc(ccc1O)C[C@@H]1c4c(cc(OC)c(O)c4Oc4ccc(cc4)C[C@@H]3[N+](C)(C)CC2)CC[N+]1(C)C&quot;, &quot;data-mols2grid-id-display&quot;: 4}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 5, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Cephradine.mol&quot;, &quot;data-Drug&quot;: &quot;CC1=C(C(=O)O)N2C(=O)[C@H](NC(=O)[C@@H](N)C3=CCC=CC3)[C@@H]2SC1&quot;, &quot;data-mols2grid-id-display&quot;: 5}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 6, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Floxacillin.mol&quot;, &quot;data-Drug&quot;: &quot;Cc1onc(-c2c(F)cccc2Cl)c1C(=O)N[C@@H]1C(=O)N2[C@H]1SC(C)(C)[C@H]2C(=O)O&quot;, &quot;data-mols2grid-id-display&quot;: 6}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 7, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Clavulanic_acid.mol&quot;, &quot;data-Drug&quot;: &quot;O=C(O)[C@@H]1C(=CCO)O[C@H]2CC(=O)N21&quot;, &quot;data-mols2grid-id-display&quot;: 7}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 8, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Ceftizoxime.mol&quot;, &quot;data-Drug&quot;: &quot;CO/N=C(\\\\C(=O)N[C@@H]1C(=O)N2C(C(=O)O)=CCS[C@@H]12)c1csc(N)n1&quot;, &quot;data-mols2grid-id-display&quot;: 8}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 9, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Cefpodoxime_proxetil.mol&quot;, &quot;data-Drug&quot;: &quot;COCC1=C(C(=O)O[C@H](C)OC(=O)OC(C)C)N2C(=O)[C@H](NC(=O)C(=NOC)c3csc(N)n3)[C@@H]2SC1&quot;, &quot;data-mols2grid-id-display&quot;: 9}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 10, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Cefmetazole&quot;, &quot;data-Drug&quot;: &quot;CO[C@@]1(NC(=O)CSCC#N)C(=O)N2C(C(=O)O)=C(CSc3nnnn3C)CS[C@H]21&quot;, &quot;data-mols2grid-id-display&quot;: 10}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 11, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Cefotaxime&quot;, &quot;data-Drug&quot;: &quot;C=C(N[C@@H]1C(=O)N2C(C(=O)O)=C(COC(C)=O)CS[C@@H]12)C(=NOC)c1csc(N)n1&quot;, &quot;data-mols2grid-id-display&quot;: 11}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 12, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Imipenem.mol&quot;, &quot;data-Drug&quot;: &quot;C[C@H](O)[C@@H]1C(=O)N2C(C(=O)O)=C(SCC/N=C/N)C[C@@H]12&quot;, &quot;data-mols2grid-id-display&quot;: 12}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 13, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Sulbactam&quot;, &quot;data-Drug&quot;: &quot;CC1(C)[C@H](C(=O)O)N2C(=O)C[C@@H]2S1(=O)=O&quot;, &quot;data-mols2grid-id-display&quot;: 13}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 14, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Ticarcillin&quot;, &quot;data-Drug&quot;: &quot;CC1(C)S[C@H]2[C@@H](NC(=O)[C@@H](C(=O)O)c3ccsc3)C(=O)N2[C@@H]1C(=O)O&quot;, &quot;data-mols2grid-id-display&quot;: 14}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 15, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Aztreonam.mol&quot;, &quot;data-Drug&quot;: &quot;C[C@@H]1[C@@H](NC(=O)/C(=N\\\\OC(C)(C)C(=O)O)c2csc(N)n2)C(=O)N1S(=O)(=O)O&quot;, &quot;data-mols2grid-id-display&quot;: 15}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 16, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Ceftriaxone.mol&quot;, &quot;data-Drug&quot;: &quot;CON=C(C(=O)N[C@H]1C(=O)N2C(C(=O)O)=C(CSc3nc(=O)c(O)nn3C)CS[C@@H]12)c1csc(N)n1&quot;, &quot;data-mols2grid-id-display&quot;: 16}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 17, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Azlocillin.mol&quot;, &quot;data-Drug&quot;: &quot;CC1(C)S[C@H]2[C@@H](NC(=O)[C@@H](NC(=O)N3CCNC3=O)c3ccccc3)C(=O)N2[C@@H]1C(=O)O&quot;, &quot;data-mols2grid-id-display&quot;: 17}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 18, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Cefodizime.mol&quot;, &quot;data-Drug&quot;: &quot;CON=C(C(=O)N[C@H]1C(=O)N2C(C(=O)O)=C(CSc3nc(C)c(CC(=O)O)s3)CS[C@@H]12)c1csc(N)n1&quot;, &quot;data-mols2grid-id-display&quot;: 18}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 19, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Meropenem.mol&quot;, &quot;data-Drug&quot;: &quot;C[C@H](O)[C@H]1C(=O)N2C(C(=O)O)=C(S[C@@H]3CC[C@H](C(=O)N(C)C)N3)[C@@H](C)[C@H]12&quot;, &quot;data-mols2grid-id-display&quot;: 19}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 20, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Mezlocillin&quot;, &quot;data-Drug&quot;: &quot;CC1(C)S[C@H]2[C@@H](NC(=O)[C@@H](NC(=O)N3CCN(S(C)(=O)=O)C3=O)c3ccccc3)C(=O)N2[C@@H]1C(=O)O&quot;, &quot;data-mols2grid-id-display&quot;: 20}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 21, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Cefpirome&quot;, &quot;data-Drug&quot;: &quot;CO/N=C(\\\\C(=O)N[C@@H]1C(=O)N2C(C(=O)O)=C(C[n+]3ccccc3)CS[C@@H]12)c1csc(N)n1&quot;, &quot;data-mols2grid-id-display&quot;: 21}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 22, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Ceftazidime.mol&quot;, &quot;data-Drug&quot;: &quot;CC(C)(O/N=C(\\\\C(=O)N[C@@H]1C(=O)N2C(C(=O)O)=C(C[n+]3ccccc3)CS[C@@H]12)c1csc(N)n1)C(=O)O&quot;, &quot;data-mols2grid-id-display&quot;: 22}, {&quot;data-reos&quot;: &quot;I16 Betalactams&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 23, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Moxalactam.mol&quot;, &quot;data-Drug&quot;: &quot;CO[C@@]1(NC(=O)[C@@H](C(=O)O)c2ccc(O)cc2)C(=O)N2C(C(=O)O)=C(CSc3nnnn3C)CO[C@H]21&quot;, &quot;data-mols2grid-id-display&quot;: 23}, {&quot;data-reos&quot;: &quot;I2 Compounds with 4 or more acidic groups&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 24, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Edetic_acid&quot;, &quot;data-Drug&quot;: &quot;O=C(O)CN(CCN(CC(=O)O)CC(=O)O)CC(=O)O&quot;, &quot;data-mols2grid-id-display&quot;: 24}, {&quot;data-reos&quot;: &quot;I4 Disulphides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 25, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Disulfiram&quot;, &quot;data-Drug&quot;: &quot;CCN(CC)C(=S)SSC(=S)N(CC)CC&quot;, &quot;data-mols2grid-id-display&quot;: 25}, {&quot;data-reos&quot;: &quot;I6 Epoxides, Thioepoxides, Aziridines&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 26, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Scopolamine.mol&quot;, &quot;data-Drug&quot;: &quot;CN1[C@H]2C[C@H](OC(=O)[C@@H](CO)c3ccccc3)C[C@@H]1[C@@H]1O[C@H]12&quot;, &quot;data-mols2grid-id-display&quot;: 26}, {&quot;data-reos&quot;: &quot;I6 Epoxides, Thioepoxides, Aziridines&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 27, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Butylscopolamine&quot;, &quot;data-Drug&quot;: &quot;CCCC[N+]1(C)[C@@H]2C[C@@H](OC(=O)[C@@H](CO)c3ccccc3)C[C@@H]1[C@H]1O[C@H]12&quot;, &quot;data-mols2grid-id-display&quot;: 27}, {&quot;data-reos&quot;: &quot;I6 Epoxides, Thioepoxides, Aziridines&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 28, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Oxitropium.mol&quot;, &quot;data-Drug&quot;: &quot;CC[N+]1(C)[C@@H]2C[C@@H](OC(=O)[C@@H](CO)c3ccccc3)C[C@@H]1[C@H]1O[C@H]12&quot;, &quot;data-mols2grid-id-display&quot;: 28}, {&quot;data-reos&quot;: &quot;N1 Quinones&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 29, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Mitoxantrone&quot;, &quot;data-Drug&quot;: &quot;O=C1c2c(O)ccc(O)c2C(=O)c2c(NCCNCCO)ccc(NCCNCCO)c21&quot;, &quot;data-mols2grid-id-display&quot;: 29}, {&quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 30, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Isotretinoin.mol&quot;, &quot;data-Drug&quot;: &quot;CC(=CC(=O)O)/C=C/C=C(C)\\\\C=C/C1=C(C)CCCC1(C)C&quot;, &quot;data-mols2grid-id-display&quot;: 30}, {&quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 31, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Vitamin_A&quot;, &quot;data-Drug&quot;: &quot;CC(=CCO)/C=C/C=C(C)\\\\C=C\\\\C1=C(C)CCCC1(C)C&quot;, &quot;data-mols2grid-id-display&quot;: 31}, {&quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 32, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Amphotericin_B.mol&quot;, &quot;data-Drug&quot;: &quot;C[C@@H]1OC(=O)C[C@H](O)C[C@H](O)CC[C@@H](O)[C@H](O)C[C@H](O)C[C@@]2(O)C[C@@H](O)[C@@H](C(=O)O)[C@H](C[C@@](O)(O[C@@H]3O[C@@H](C)[C@@H](O)[C@H](N)[C@@H]3O)C=CC=CC=CC=CC=CC=CC=C[C@@H](C)[C@H](O)[C@@H]1C)O2&quot;, &quot;data-mols2grid-id-display&quot;: 32}, {&quot;data-reos&quot;: &quot;N2 Polyenes&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 33, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Acitretin.mol&quot;, &quot;data-Drug&quot;: &quot;COc1cc(C)c(/C=C/C(C)=C/C=C/C(C)=CC(=O)O)c(C)c1C&quot;, &quot;data-mols2grid-id-display&quot;: 33}, {&quot;data-reos&quot;: &quot;N3 Saponin derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 34, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Cymarin&quot;, &quot;data-Drug&quot;: &quot;C=C[C@@]12CC[C@@H](O[C@H]3C[C@@H](OC)[C@@H](O)[C@H](C)O3)C[C@]1(O)CC[C@@H]1[C@@H]2CC[C@]2(C)[C@H](C3=CC(=O)OC3)CC[C@@]12O&quot;, &quot;data-mols2grid-id-display&quot;: 34}, {&quot;data-reos&quot;: &quot;N5 Cycloheximide derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 35, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Phenglutarimide&quot;, &quot;data-Drug&quot;: &quot;CCN(CC)CC[C@]1(c2ccccc2)CCC(=O)NC1=O&quot;, &quot;data-mols2grid-id-display&quot;: 35}, {&quot;data-reos&quot;: &quot;N5 Cycloheximide derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 36, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Aminoglutethimide&quot;, &quot;data-Drug&quot;: &quot;CC[C@@]1(c2ccc(N)cc2)CCC(=O)NC1=O&quot;, &quot;data-mols2grid-id-display&quot;: 36}, {&quot;data-reos&quot;: &quot;N5 Cycloheximide derivatives&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 37, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Buspirone.mol&quot;, &quot;data-Drug&quot;: &quot;O=C1CC2(CCCC2)CC(=O)N1CCCCN1CCN(c2ncccn2)CC1&quot;, &quot;data-mols2grid-id-display&quot;: 37}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 38, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Carmustine&quot;, &quot;data-Drug&quot;: &quot;O=NN(CCCl)C(=O)NCCCl&quot;, &quot;data-mols2grid-id-display&quot;: 38}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 39, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Toremifene.mol&quot;, &quot;data-Drug&quot;: &quot;CN(C)CCOc1ccc(C(=C(CCCl)c2ccccc2)c2ccccc2)cc1&quot;, &quot;data-mols2grid-id-display&quot;: 39}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 40, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Trofosfamide&quot;, &quot;data-Drug&quot;: &quot;O=[P@@]1(N(CCCl)CCCl)OCCCN1CCCl&quot;, &quot;data-mols2grid-id-display&quot;: 40}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 41, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Clomethiazole.mol&quot;, &quot;data-Drug&quot;: &quot;Cc1ncsc1CCCl&quot;, &quot;data-mols2grid-id-display&quot;: 41}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 42, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Diloxanide&quot;, &quot;data-Drug&quot;: &quot;CN(C(=O)C(Cl)Cl)c1ccc(O)cc1&quot;, &quot;data-mols2grid-id-display&quot;: 42}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 43, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Clindamycin.mol&quot;, &quot;data-Drug&quot;: &quot;CCC[C@@H]1C[C@H](C(=O)N[C@@H]([C@H](C)Cl)[C@@H]2O[C@@H](SC)[C@@H](O)[C@@H](O)[C@@H]2O)N(C)C1&quot;, &quot;data-mols2grid-id-display&quot;: 43}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 44, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Chlorambucil.mol&quot;, &quot;data-Drug&quot;: &quot;O=C(O)CCCc1ccc(N(CCCl)CCCl)cc1&quot;, &quot;data-mols2grid-id-display&quot;: 44}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 45, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Chloramphenicol.mol&quot;, &quot;data-Drug&quot;: &quot;O=C(N[C@H](CO)[C@@H](O)c1ccc([N+](=O)[O-])cc1)C(Cl)Cl&quot;, &quot;data-mols2grid-id-display&quot;: 45}, {&quot;data-reos&quot;: &quot;R1 Reactive alkyl halides&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 46, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Estramustine&quot;, &quot;data-Drug&quot;: &quot;C[C@@]12CC[C@@H]3c4ccc(OC(=O)N(CCCl)CCCl)cc4CC[C@@H]3[C@H]1CC[C@@H]2O&quot;, &quot;data-mols2grid-id-display&quot;: 46}, {&quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 47, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Isoniazid.mol&quot;, &quot;data-Drug&quot;: &quot;NNC(=O)c1ccncc1&quot;, &quot;data-mols2grid-id-display&quot;: 47}, {&quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 48, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Benserazide&quot;, &quot;data-Drug&quot;: &quot;N[C@H](CO)C(=O)NNCc1ccc(O)c(O)c1O&quot;, &quot;data-mols2grid-id-display&quot;: 48}, {&quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 49, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Isocarboxazid&quot;, &quot;data-Drug&quot;: &quot;Cc1cc(C(=O)NNCc2ccccc2)no1&quot;, &quot;data-mols2grid-id-display&quot;: 49}, {&quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 50, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Streptozocin.mol&quot;, &quot;data-Drug&quot;: &quot;CN(N=O)C(=O)N[C@H]1[C@@H](O)O[C@@H](CO)[C@@H](O)[C@H]1O&quot;, &quot;data-mols2grid-id-display&quot;: 50}, {&quot;data-reos&quot;: &quot;R17 acylhydrazide&quot;, &quot;data-rule_set_name&quot;: &quot;Glaxo&quot;, &quot;mols2grid-id&quot;: 51, &quot;data-img&quot;: null, &quot;data-Drug_ID&quot;: &quot;Lucifer_Yellow_CH.mol&quot;, &quot;data-Drug&quot;: &quot;NNC(=O)NNN1C(=O)c2cc(S(=O)(=O)O)cc3c(N)c(S(=O)(=O)O)cc(c23)C1=O&quot;, &quot;data-mols2grid-id-display&quot;: 51}]);\n",
                             "\n",
                             "\n",
                             "// filter\n",
                             "if (window.parent.mols2grid_lists === undefined) {\n",
                             "    window.parent.mols2grid_lists = {};\n",
                             "}\n",
                             "window.parent.mols2grid_lists[&quot;default&quot;] = listObj;\n",
@@ -3473,15 +3472,15 @@
             "metadata": {},
             "source": [
                 "We can also get REOS data as a Pandas dataframe.  To look at this, let's first reload the HIA data. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 23,
             "id": "d0b3b27e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -3493,15 +3492,15 @@
             ],
             "source": [
                 "hia_data = ADME(name = 'HIA_Hou').get_data()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 24,
             "id": "f1cccee9",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -3612,15 +3611,15 @@
                             "575      Kanamycin.mol  CC(=O)NC[C@@H]1O[C@@H](O[C@H]2[C@@H](N)C[C@H](...  0\n",
                             "576       Amikacin.mol  NCC[C@@H](O)C(=O)N[C@@H]1C[C@H](N)[C@H](O[C@@H...  0\n",
                             "577     Moxalactam.mol  CO[C@@]1(NC(=O)[C@@H](C(=O)O)c2ccc(O)cc2)C(=O)...  0\n",
                             "\n",
                             "[578 rows x 3 columns]"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "hia_data"
             ]
@@ -3631,22 +3630,22 @@
             "metadata": {},
             "source": [
                 "We can the call the **pandas_smiles** method to calculate REOS for a list of SMILES.  "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 25,
             "id": "dc0af315",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "d816c11a54cf471a92e858fb85dd0f23",
+                            "model_id": "0fa19fcebd2d4baca172beda178ff853",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/578 [00:00<?, ?it/s]"
                         ]
                     },
@@ -3664,15 +3663,15 @@
             "metadata": {},
             "source": [
                 "Let's look at the molecules that triggered an alert"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": 26,
             "id": "8bfd265a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -3757,15 +3756,15 @@
                             "17          Glaxo     R1 Reactive alkyl halides  \n",
                             "89          Glaxo  N5 Cycloheximide derivatives  \n",
                             "114         Glaxo     R1 Reactive alkyl halides  \n",
                             "118         Glaxo     R1 Reactive alkyl halides  \n",
                             "176         Glaxo               I16 Betalactams  "
                         ]
                     },
-                    "execution_count": 48,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "combo_df = pd.concat([hia_data,reos_results],axis=1)\n",
                 "combo_df.query(\"description != 'ok'\").head()"
@@ -3777,32 +3776,32 @@
             "metadata": {},
             "source": [
                 "We can use the **pandas_mols** method to perfrom a similar function with a set of RDKit molecules. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 66,
+            "execution_count": 27,
             "id": "dff40432",
             "metadata": {},
             "outputs": [],
             "source": [
                 "hia_data['mol'] = hia_data.Drug.apply(Chem.MolFromSmiles)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 67,
+            "execution_count": 28,
             "id": "1d28f62e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "89a997269b674aadb12ed46b697d0b21",
+                            "model_id": "2f85485a2ddf4c88b319b7c4c43ebf86",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/578 [00:00<?, ?it/s]"
                         ]
                     },
@@ -3828,107 +3827,95 @@
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>rule_set_name</th>\n",
                             "      <th>description</th>\n",
-                            "      <th>smarts</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>573</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>574</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>575</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>576</th>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>577</th>\n",
                             "      <td>Glaxo</td>\n",
                             "      <td>I16 Betalactams</td>\n",
-                            "      <td>N1CCC1=O</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>578 rows \u00d7 3 columns</p>\n",
+                            "<p>578 rows \u00d7 2 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "    rule_set_name      description    smarts\n",
-                            "0              ok               ok        ok\n",
-                            "1              ok               ok        ok\n",
-                            "2              ok               ok        ok\n",
-                            "3              ok               ok        ok\n",
-                            "4              ok               ok        ok\n",
-                            "..            ...              ...       ...\n",
-                            "573            ok               ok        ok\n",
-                            "574            ok               ok        ok\n",
-                            "575            ok               ok        ok\n",
-                            "576            ok               ok        ok\n",
-                            "577         Glaxo  I16 Betalactams  N1CCC1=O\n",
+                            "    rule_set_name      description\n",
+                            "0              ok               ok\n",
+                            "1              ok               ok\n",
+                            "2              ok               ok\n",
+                            "3              ok               ok\n",
+                            "4              ok               ok\n",
+                            "..            ...              ...\n",
+                            "573            ok               ok\n",
+                            "574            ok               ok\n",
+                            "575            ok               ok\n",
+                            "576            ok               ok\n",
+                            "577         Glaxo  I16 Betalactams\n",
                             "\n",
-                            "[578 rows x 3 columns]"
+                            "[578 rows x 2 columns]"
                         ]
                     },
-                    "execution_count": 67,
+                    "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "reos.pandas_mols(hia_data.mol)"
             ]
@@ -3939,15 +3926,15 @@
             "metadata": {},
             "source": [
                 "The **reos_smiles** and **reos_mols** method will return a **None** for SMILES or molecules where parsing failed.  We can use dropna to drop these molecules.  Here's an example. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 51,
+            "execution_count": 29,
             "id": "d111a18a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -3995,34 +3982,34 @@
                         "text/plain": [
                             "     SMILES      Name\n",
                             "0       CCC    butane\n",
                             "1      xxxx      junk\n",
                             "2  c1ccccn1  pyridine"
                         ]
                     },
-                    "execution_count": 51,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "test_df = pd.DataFrame({\"SMILES\": [\"CCC\",\"xxxx\",\"c1ccccn1\"], \"Name\": [\"butane\",\"junk\",\"pyridine\"]})\n",
                 "test_df"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 52,
+            "execution_count": 30,
             "id": "822ab126",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "932771bf0fa2490eac4a671d2acfc17a",
+                            "model_id": "e8481365f8c24b328e58fb6001f9afde",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/3 [00:00<?, ?it/s]"
                         ]
                     },
@@ -4036,16 +4023,16 @@
                         "Error parsing SMILES xxxx\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[13:40:00] SMILES Parse Error: syntax error while parsing: xxxx\n",
-                        "[13:40:00] SMILES Parse Error: Failed parsing SMILES 'xxxx' for input: 'xxxx'\n"
+                        "[13:46:55] SMILES Parse Error: syntax error while parsing: xxxx\n",
+                        "[13:46:55] SMILES Parse Error: Failed parsing SMILES 'xxxx' for input: 'xxxx'\n"
                     ]
                 }
             ],
             "source": [
                 "test_reos = reos.pandas_smiles(test_df.SMILES)"
             ]
         },
@@ -4055,15 +4042,15 @@
             "metadata": {},
             "source": [
                 "Combine the REOS result with the original dataframe"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 59,
+            "execution_count": 31,
             "id": "93f61a72",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -4084,54 +4071,50 @@
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>SMILES</th>\n",
                             "      <th>Name</th>\n",
                             "      <th>rule_set_name</th>\n",
                             "      <th>description</th>\n",
-                            "      <th>smarts</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>CCC</td>\n",
                             "      <td>butane</td>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>xxxx</td>\n",
                             "      <td>junk</td>\n",
                             "      <td>None</td>\n",
                             "      <td>None</td>\n",
-                            "      <td>None</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>c1ccccn1</td>\n",
                             "      <td>pyridine</td>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "     SMILES      Name rule_set_name description smarts\n",
-                            "0       CCC    butane            ok          ok     ok\n",
-                            "1      xxxx      junk          None        None   None\n",
-                            "2  c1ccccn1  pyridine            ok          ok     ok"
+                            "     SMILES      Name rule_set_name description\n",
+                            "0       CCC    butane            ok          ok\n",
+                            "1      xxxx      junk          None        None\n",
+                            "2  c1ccccn1  pyridine            ok          ok"
                         ]
                     },
-                    "execution_count": 59,
+                    "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "test_combo_df = pd.concat([test_df,test_reos],axis=1)\n",
                 "test_combo_df"
@@ -4143,15 +4126,15 @@
             "metadata": {},
             "source": [
                 "Drop the bad row"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 56,
+            "execution_count": 32,
             "id": "898997cb",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -4172,45 +4155,42 @@
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>SMILES</th>\n",
                             "      <th>Name</th>\n",
                             "      <th>rule_set_name</th>\n",
                             "      <th>description</th>\n",
-                            "      <th>smarts</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>CCC</td>\n",
                             "      <td>butane</td>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>c1ccccn1</td>\n",
                             "      <td>pyridine</td>\n",
                             "      <td>ok</td>\n",
                             "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "     SMILES      Name rule_set_name description smarts\n",
-                            "0       CCC    butane            ok          ok     ok\n",
-                            "2  c1ccccn1  pyridine            ok          ok     ok"
+                            "     SMILES      Name rule_set_name description\n",
+                            "0       CCC    butane            ok          ok\n",
+                            "2  c1ccccn1  pyridine            ok          ok"
                         ]
                     },
-                    "execution_count": 56,
+                    "execution_count": 32,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "test_combo_df.dropna()"
             ]
@@ -4221,15 +4201,15 @@
             "metadata": {},
             "source": [
                 "A couple of settings to improve the RDKit rendering quality"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 33,
             "id": "aa335191",
             "metadata": {},
             "outputs": [],
             "source": [
                 "uru.rd_make_structures_pretty()\n",
                 "uru.rd_enable_svg()"
             ]
@@ -4240,15 +4220,170 @@
             "metadata": {},
             "source": [
                 "We can't (yet) highlight the matches with mols2grid, but we can do this with the RDKit's [MolsToGridImage](https://www.rdkit.org/docs/source/rdkit.Chem.Draw.html)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 34,
+            "id": "927eea84-70d6-4750-ad82-fe2f3c18d896",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>Drug_ID</th>\n",
+                            "      <th>Drug</th>\n",
+                            "      <th>Y</th>\n",
+                            "      <th>mol</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>Acetanilide</td>\n",
+                            "      <td>CC(=O)Nc1ccccc1</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd8890&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>Acetazolamide.mol</td>\n",
+                            "      <td>CC(=O)Nc1nnc(S(N)(=O)=O)s1</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9620&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>Alfacalcidol</td>\n",
+                            "      <td>C=C1/C(=C\\C=C2/CCC[C@]3(C)[C@@H]2CC[C@H]3[C@@H...</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9a80&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>Aminopyrine</td>\n",
+                            "      <td>Cc1c(N(C)C)c(=N)n(-c2ccccc2)n1C</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd99a0&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>Amosulalol.mol</td>\n",
+                            "      <td>COc1ccccc1OCCNC[C@@H](O)c1ccc(C)cc1S(N)(=O)=O</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9af0&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>...</th>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>573</th>\n",
+                            "      <td>Tiludronic_acid</td>\n",
+                            "      <td>O=P(O)(O)C(Cc1ccc(Cl)cc1)P(=O)(O)O</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009690&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>574</th>\n",
+                            "      <td>Zanamivir.mol</td>\n",
+                            "      <td>CC(=O)N[C@H]1[C@@H]([C@@H](O)[C@H](O)CO)OC(C(=...</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009700&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>575</th>\n",
+                            "      <td>Kanamycin.mol</td>\n",
+                            "      <td>CC(=O)NC[C@@H]1O[C@@H](O[C@H]2[C@@H](N)C[C@H](...</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009770&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>576</th>\n",
+                            "      <td>Amikacin.mol</td>\n",
+                            "      <td>NCC[C@@H](O)C(=O)N[C@@H]1C[C@H](N)[C@H](O[C@@H...</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x2960097e0&gt;</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>577</th>\n",
+                            "      <td>Moxalactam.mol</td>\n",
+                            "      <td>CO[C@@]1(NC(=O)[C@@H](C(=O)O)c2ccc(O)cc2)C(=O)...</td>\n",
+                            "      <td>0</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009850&gt;</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "<p>578 rows \u00d7 4 columns</p>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "               Drug_ID                                               Drug  Y  \\\n",
+                            "0          Acetanilide                                    CC(=O)Nc1ccccc1  1   \n",
+                            "1    Acetazolamide.mol                         CC(=O)Nc1nnc(S(N)(=O)=O)s1  1   \n",
+                            "2         Alfacalcidol  C=C1/C(=C\\C=C2/CCC[C@]3(C)[C@@H]2CC[C@H]3[C@@H...  1   \n",
+                            "3          Aminopyrine                    Cc1c(N(C)C)c(=N)n(-c2ccccc2)n1C  1   \n",
+                            "4       Amosulalol.mol      COc1ccccc1OCCNC[C@@H](O)c1ccc(C)cc1S(N)(=O)=O  1   \n",
+                            "..                 ...                                                ... ..   \n",
+                            "573    Tiludronic_acid                 O=P(O)(O)C(Cc1ccc(Cl)cc1)P(=O)(O)O  0   \n",
+                            "574      Zanamivir.mol  CC(=O)N[C@H]1[C@@H]([C@@H](O)[C@H](O)CO)OC(C(=...  0   \n",
+                            "575      Kanamycin.mol  CC(=O)NC[C@@H]1O[C@@H](O[C@H]2[C@@H](N)C[C@H](...  0   \n",
+                            "576       Amikacin.mol  NCC[C@@H](O)C(=O)N[C@@H]1C[C@H](N)[C@H](O[C@@H...  0   \n",
+                            "577     Moxalactam.mol  CO[C@@]1(NC(=O)[C@@H](C(=O)O)c2ccc(O)cc2)C(=O)...  0   \n",
+                            "\n",
+                            "                                               mol  \n",
+                            "0    <rdkit.Chem.rdchem.Mol object at 0x295fd8890>  \n",
+                            "1    <rdkit.Chem.rdchem.Mol object at 0x295fd9620>  \n",
+                            "2    <rdkit.Chem.rdchem.Mol object at 0x295fd9a80>  \n",
+                            "3    <rdkit.Chem.rdchem.Mol object at 0x295fd99a0>  \n",
+                            "4    <rdkit.Chem.rdchem.Mol object at 0x295fd9af0>  \n",
+                            "..                                             ...  \n",
+                            "573  <rdkit.Chem.rdchem.Mol object at 0x296009690>  \n",
+                            "574  <rdkit.Chem.rdchem.Mol object at 0x296009700>  \n",
+                            "575  <rdkit.Chem.rdchem.Mol object at 0x296009770>  \n",
+                            "576  <rdkit.Chem.rdchem.Mol object at 0x2960097e0>  \n",
+                            "577  <rdkit.Chem.rdchem.Mol object at 0x296009850>  \n",
+                            "\n",
+                            "[578 rows x 4 columns]"
+                        ]
+                    },
+                    "execution_count": 34,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "hia_data"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 35,
             "id": "9e9a68c0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/svg+xml": [
                             "<svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:rdkit=\"http://www.rdkit.org/xml\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" version=\"1.1\" baseProfile=\"full\" xml:space=\"preserve\" width=\"900px\" height=\"900px\" viewBox=\"0 0 900 900\">\n",
@@ -4794,29 +4929,29 @@
                             "<path class=\"atom-31\" d=\"M 790.2 649.6 L 791.5 649.6 L 791.5 653.8 L 796.6 653.8 L 796.6 649.6 L 798.0 649.6 L 798.0 659.6 L 796.6 659.6 L 796.6 655.0 L 791.5 655.0 L 791.5 659.6 L 790.2 659.6 L 790.2 649.6 \" fill=\"#000000\"/>\n",
                             "</svg>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.SVG object>"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 35,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "rule_set = \"Glaxo\"\n",
                 "rule_name = 'R1 Reactive alkyl halides'\n",
                 "query = reos.active_rule_df.query(\"rule_set_name == @rule_set and description == @rule_name\").pat.values\n",
                 "img = None\n",
                 "if len(query) != 1:\n",
                 "    print(f\"no query match for {rule_set}/{rule_name}\")\n",
                 "else:\n",
                 "    query = query[0]\n",
-                "    smiles_list = hia_data.query(\"rule_set_name == @rule_set and reos == @rule_name\").Drug\n",
+                "    smiles_list = combo_df.query(\"rule_set_name == @rule_set and description == @rule_name\").Drug\n",
                 "    mol_list = [Chem.MolFromSmiles(x) for x in smiles_list]\n",
                 "    match_list = [x.GetSubstructMatch(query) for x in mol_list]\n",
                 "    img = MolsToGridImage(mol_list,molsPerRow=3,highlightAtomLists=match_list,subImgSize=(300, 300))\n",
                 "img"
             ]
         },
         {
@@ -4825,15 +4960,15 @@
             "metadata": {},
             "source": [
                 "Let's add some Rule of 5 properties to the dataframe.  First, we'll instantiate an Ro5Calculator."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 36,
             "id": "1ce13ae3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ro5_calc = uru.Ro5Calculator()"
             ]
         },
@@ -4843,25 +4978,25 @@
             "metadata": {},
             "source": [
                 "Next add the properties to the dataframe."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 37,
             "id": "d80f1fd6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "hia_data[ro5_calc.names] = hia_data.Drug.apply(ro5_calc.calc_smiles).to_list()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 38,
             "id": "38a367f7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -4881,83 +5016,77 @@
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Drug_ID</th>\n",
                             "      <th>Drug</th>\n",
                             "      <th>Y</th>\n",
-                            "      <th>rule_set_name</th>\n",
-                            "      <th>reos</th>\n",
+                            "      <th>mol</th>\n",
                             "      <th>MolWt</th>\n",
                             "      <th>LogP</th>\n",
                             "      <th>HBD</th>\n",
                             "      <th>HBA</th>\n",
                             "      <th>TPSA</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Acetanilide</td>\n",
                             "      <td>CC(=O)Nc1ccccc1</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd8890&gt;</td>\n",
                             "      <td>135.166</td>\n",
                             "      <td>1.64500</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>29.10</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>Acetazolamide.mol</td>\n",
                             "      <td>CC(=O)Nc1nnc(S(N)(=O)=O)s1</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9620&gt;</td>\n",
                             "      <td>222.251</td>\n",
                             "      <td>-0.85610</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>6.0</td>\n",
                             "      <td>115.04</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>Alfacalcidol</td>\n",
                             "      <td>C=C1/C(=C\\C=C2/CCC[C@]3(C)[C@@H]2CC[C@H]3[C@@H...</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9a80&gt;</td>\n",
                             "      <td>400.647</td>\n",
                             "      <td>6.58980</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>40.46</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>Aminopyrine</td>\n",
                             "      <td>Cc1c(N(C)C)c(=N)n(-c2ccccc2)n1C</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd99a0&gt;</td>\n",
                             "      <td>230.315</td>\n",
                             "      <td>1.66969</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>4.0</td>\n",
                             "      <td>36.95</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>Amosulalol.mol</td>\n",
                             "      <td>COc1ccccc1OCCNC[C@@H](O)c1ccc(C)cc1S(N)(=O)=O</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9af0&gt;</td>\n",
                             "      <td>380.466</td>\n",
                             "      <td>1.35302</td>\n",
                             "      <td>3.0</td>\n",
                             "      <td>6.0</td>\n",
                             "      <td>110.88</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
@@ -4967,84 +5096,78 @@
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>573</th>\n",
                             "      <td>Tiludronic_acid</td>\n",
                             "      <td>O=P(O)(O)C(Cc1ccc(Cl)cc1)P(=O)(O)O</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009690&gt;</td>\n",
                             "      <td>300.571</td>\n",
                             "      <td>1.56400</td>\n",
                             "      <td>4.0</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>115.06</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>574</th>\n",
                             "      <td>Zanamivir.mol</td>\n",
                             "      <td>CC(=O)N[C@H]1[C@@H]([C@@H](O)[C@H](O)CO)OC(C(=...</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009700&gt;</td>\n",
                             "      <td>332.313</td>\n",
                             "      <td>-3.57583</td>\n",
                             "      <td>8.0</td>\n",
                             "      <td>7.0</td>\n",
                             "      <td>198.22</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>575</th>\n",
                             "      <td>Kanamycin.mol</td>\n",
                             "      <td>CC(=O)NC[C@@H]1O[C@@H](O[C@H]2[C@@H](N)C[C@H](...</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009770&gt;</td>\n",
                             "      <td>526.540</td>\n",
                             "      <td>-7.11400</td>\n",
                             "      <td>11.0</td>\n",
                             "      <td>15.0</td>\n",
                             "      <td>285.69</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>576</th>\n",
                             "      <td>Amikacin.mol</td>\n",
                             "      <td>NCC[C@@H](O)C(=O)N[C@@H]1C[C@H](N)[C@H](O[C@@H...</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x2960097e0&gt;</td>\n",
                             "      <td>585.608</td>\n",
                             "      <td>-8.42420</td>\n",
                             "      <td>13.0</td>\n",
                             "      <td>17.0</td>\n",
                             "      <td>331.94</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>577</th>\n",
                             "      <td>Moxalactam.mol</td>\n",
                             "      <td>CO[C@@]1(NC(=O)[C@@H](C(=O)O)c2ccc(O)cc2)C(=O)...</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>Glaxo</td>\n",
-                            "      <td>I16 Betalactams</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009850&gt;</td>\n",
                             "      <td>520.480</td>\n",
                             "      <td>-1.12770</td>\n",
                             "      <td>4.0</td>\n",
                             "      <td>12.0</td>\n",
                             "      <td>206.30</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>578 rows \u00d7 10 columns</p>\n",
+                            "<p>578 rows \u00d7 9 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "               Drug_ID                                               Drug  Y  \\\n",
                             "0          Acetanilide                                    CC(=O)Nc1ccccc1  1   \n",
                             "1    Acetazolamide.mol                         CC(=O)Nc1nnc(S(N)(=O)=O)s1  1   \n",
                             "2         Alfacalcidol  C=C1/C(=C\\C=C2/CCC[C@]3(C)[C@@H]2CC[C@H]3[C@@H...  1   \n",
@@ -5053,31 +5176,44 @@
                             "..                 ...                                                ... ..   \n",
                             "573    Tiludronic_acid                 O=P(O)(O)C(Cc1ccc(Cl)cc1)P(=O)(O)O  0   \n",
                             "574      Zanamivir.mol  CC(=O)N[C@H]1[C@@H]([C@@H](O)[C@H](O)CO)OC(C(=...  0   \n",
                             "575      Kanamycin.mol  CC(=O)NC[C@@H]1O[C@@H](O[C@H]2[C@@H](N)C[C@H](...  0   \n",
                             "576       Amikacin.mol  NCC[C@@H](O)C(=O)N[C@@H]1C[C@H](N)[C@H](O[C@@H...  0   \n",
                             "577     Moxalactam.mol  CO[C@@]1(NC(=O)[C@@H](C(=O)O)c2ccc(O)cc2)C(=O)...  0   \n",
                             "\n",
-                            "    rule_set_name             reos    MolWt     LogP   HBD   HBA    TPSA  \n",
-                            "0              ok               ok  135.166  1.64500   1.0   1.0   29.10  \n",
-                            "1              ok               ok  222.251 -0.85610   2.0   6.0  115.04  \n",
-                            "2              ok               ok  400.647  6.58980   2.0   2.0   40.46  \n",
-                            "3              ok               ok  230.315  1.66969   1.0   4.0   36.95  \n",
-                            "4              ok               ok  380.466  1.35302   3.0   6.0  110.88  \n",
-                            "..            ...              ...      ...      ...   ...   ...     ...  \n",
-                            "573            ok               ok  300.571  1.56400   4.0   2.0  115.06  \n",
-                            "574            ok               ok  332.313 -3.57583   8.0   7.0  198.22  \n",
-                            "575            ok               ok  526.540 -7.11400  11.0  15.0  285.69  \n",
-                            "576            ok               ok  585.608 -8.42420  13.0  17.0  331.94  \n",
-                            "577         Glaxo  I16 Betalactams  520.480 -1.12770   4.0  12.0  206.30  \n",
+                            "                                               mol    MolWt     LogP   HBD  \\\n",
+                            "0    <rdkit.Chem.rdchem.Mol object at 0x295fd8890>  135.166  1.64500   1.0   \n",
+                            "1    <rdkit.Chem.rdchem.Mol object at 0x295fd9620>  222.251 -0.85610   2.0   \n",
+                            "2    <rdkit.Chem.rdchem.Mol object at 0x295fd9a80>  400.647  6.58980   2.0   \n",
+                            "3    <rdkit.Chem.rdchem.Mol object at 0x295fd99a0>  230.315  1.66969   1.0   \n",
+                            "4    <rdkit.Chem.rdchem.Mol object at 0x295fd9af0>  380.466  1.35302   3.0   \n",
+                            "..                                             ...      ...      ...   ...   \n",
+                            "573  <rdkit.Chem.rdchem.Mol object at 0x296009690>  300.571  1.56400   4.0   \n",
+                            "574  <rdkit.Chem.rdchem.Mol object at 0x296009700>  332.313 -3.57583   8.0   \n",
+                            "575  <rdkit.Chem.rdchem.Mol object at 0x296009770>  526.540 -7.11400  11.0   \n",
+                            "576  <rdkit.Chem.rdchem.Mol object at 0x2960097e0>  585.608 -8.42420  13.0   \n",
+                            "577  <rdkit.Chem.rdchem.Mol object at 0x296009850>  520.480 -1.12770   4.0   \n",
+                            "\n",
+                            "      HBA    TPSA  \n",
+                            "0     1.0   29.10  \n",
+                            "1     6.0  115.04  \n",
+                            "2     2.0   40.46  \n",
+                            "3     4.0   36.95  \n",
+                            "4     6.0  110.88  \n",
+                            "..    ...     ...  \n",
+                            "573   2.0  115.06  \n",
+                            "574   7.0  198.22  \n",
+                            "575  15.0  285.69  \n",
+                            "576  17.0  331.94  \n",
+                            "577  12.0  206.30  \n",
                             "\n",
-                            "[578 rows x 10 columns]"
+                            "[578 rows x 9 columns]"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 38,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "hia_data"
             ]
@@ -5088,25 +5224,25 @@
             "metadata": {},
             "source": [
                 "With this in hand, we can define a query to select the molecules that pass our functional group filters and meet a set of property criteria. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 41,
             "id": "f3db1aa0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "criteria_query = \"\"\"reos == 'ok' and MolWt <= 500 and LogP <= 5 and HBD <= 5 and HBA <= 10 and TPSA <= 140\"\"\""
+                "criteria_query = \"\"\"MolWt <= 500 and LogP <= 5 and HBD <= 5 and HBA <= 10 and TPSA <= 140\"\"\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 42,
             "id": "3334eec7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -5126,83 +5262,77 @@
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Drug_ID</th>\n",
                             "      <th>Drug</th>\n",
                             "      <th>Y</th>\n",
-                            "      <th>rule_set_name</th>\n",
-                            "      <th>reos</th>\n",
+                            "      <th>mol</th>\n",
                             "      <th>MolWt</th>\n",
                             "      <th>LogP</th>\n",
                             "      <th>HBD</th>\n",
                             "      <th>HBA</th>\n",
                             "      <th>TPSA</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Acetanilide</td>\n",
                             "      <td>CC(=O)Nc1ccccc1</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd8890&gt;</td>\n",
                             "      <td>135.166</td>\n",
                             "      <td>1.64500</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>29.10</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>Acetazolamide.mol</td>\n",
                             "      <td>CC(=O)Nc1nnc(S(N)(=O)=O)s1</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9620&gt;</td>\n",
                             "      <td>222.251</td>\n",
                             "      <td>-0.85610</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>6.0</td>\n",
                             "      <td>115.04</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>Aminopyrine</td>\n",
                             "      <td>Cc1c(N(C)C)c(=N)n(-c2ccccc2)n1C</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd99a0&gt;</td>\n",
                             "      <td>230.315</td>\n",
                             "      <td>1.66969</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>4.0</td>\n",
                             "      <td>36.95</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>Amosulalol.mol</td>\n",
                             "      <td>COc1ccccc1OCCNC[C@@H](O)c1ccc(C)cc1S(N)(=O)=O</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9af0&gt;</td>\n",
                             "      <td>380.466</td>\n",
                             "      <td>1.35302</td>\n",
                             "      <td>3.0</td>\n",
                             "      <td>6.0</td>\n",
                             "      <td>110.88</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>Anastrozole.mol</td>\n",
                             "      <td>CC(C)(C#N)c1cc(Cn2cncn2)cc(C(C)(C)C#N)c1</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x295fd9b60&gt;</td>\n",
                             "      <td>293.374</td>\n",
                             "      <td>2.92876</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>5.0</td>\n",
                             "      <td>78.29</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
@@ -5212,84 +5342,78 @@
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>568</th>\n",
                             "      <td>Hydrochlorothiazide.mol</td>\n",
                             "      <td>NS(=O)(=O)c1cc2c(cc1Cl)NCNS2(=O)=O</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009460&gt;</td>\n",
                             "      <td>297.745</td>\n",
                             "      <td>-0.35130</td>\n",
                             "      <td>3.0</td>\n",
                             "      <td>5.0</td>\n",
                             "      <td>118.36</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>569</th>\n",
                             "      <td>Metolazone.mol</td>\n",
                             "      <td>Cc1ccccc1N1C(=O)c2cc(S(N)(=O)=O)c(Cl)cc2N[C@@H]1C</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x2960094d0&gt;</td>\n",
                             "      <td>365.842</td>\n",
                             "      <td>2.71412</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>4.0</td>\n",
                             "      <td>92.50</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>570</th>\n",
                             "      <td>Reproterol</td>\n",
                             "      <td>Cn1c(=O)c2c(ncn2CCCNC[C@@H](O)c2cc(O)cc(O)c2)n...</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009540&gt;</td>\n",
                             "      <td>389.412</td>\n",
                             "      <td>-0.44180</td>\n",
                             "      <td>4.0</td>\n",
                             "      <td>10.0</td>\n",
                             "      <td>134.54</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>571</th>\n",
                             "      <td>Tranexamic_acid.mol</td>\n",
                             "      <td>NC[C@H]1CC[C@@H](C(=O)O)CC1</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x2960095b0&gt;</td>\n",
                             "      <td>157.213</td>\n",
                             "      <td>0.83610</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>63.32</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>573</th>\n",
                             "      <td>Tiludronic_acid</td>\n",
                             "      <td>O=P(O)(O)C(Cc1ccc(Cl)cc1)P(=O)(O)O</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>ok</td>\n",
-                            "      <td>ok</td>\n",
+                            "      <td>&lt;rdkit.Chem.rdchem.Mol object at 0x296009690&gt;</td>\n",
                             "      <td>300.571</td>\n",
                             "      <td>1.56400</td>\n",
                             "      <td>4.0</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>115.06</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>468 rows \u00d7 10 columns</p>\n",
+                            "<p>493 rows \u00d7 9 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                     Drug_ID  \\\n",
                             "0                Acetanilide   \n",
                             "1          Acetazolamide.mol   \n",
                             "3                Aminopyrine   \n",
@@ -5298,44 +5422,57 @@
                             "..                       ...   \n",
                             "568  Hydrochlorothiazide.mol   \n",
                             "569           Metolazone.mol   \n",
                             "570               Reproterol   \n",
                             "571      Tranexamic_acid.mol   \n",
                             "573          Tiludronic_acid   \n",
                             "\n",
-                            "                                                  Drug  Y rule_set_name reos  \\\n",
-                            "0                                      CC(=O)Nc1ccccc1  1            ok   ok   \n",
-                            "1                           CC(=O)Nc1nnc(S(N)(=O)=O)s1  1            ok   ok   \n",
-                            "3                      Cc1c(N(C)C)c(=N)n(-c2ccccc2)n1C  1            ok   ok   \n",
-                            "4        COc1ccccc1OCCNC[C@@H](O)c1ccc(C)cc1S(N)(=O)=O  1            ok   ok   \n",
-                            "5             CC(C)(C#N)c1cc(Cn2cncn2)cc(C(C)(C)C#N)c1  1            ok   ok   \n",
-                            "..                                                 ... ..           ...  ...   \n",
-                            "568                 NS(=O)(=O)c1cc2c(cc1Cl)NCNS2(=O)=O  1            ok   ok   \n",
-                            "569  Cc1ccccc1N1C(=O)c2cc(S(N)(=O)=O)c(Cl)cc2N[C@@H]1C  1            ok   ok   \n",
-                            "570  Cn1c(=O)c2c(ncn2CCCNC[C@@H](O)c2cc(O)cc(O)c2)n...  1            ok   ok   \n",
-                            "571                        NC[C@H]1CC[C@@H](C(=O)O)CC1  1            ok   ok   \n",
-                            "573                 O=P(O)(O)C(Cc1ccc(Cl)cc1)P(=O)(O)O  0            ok   ok   \n",
-                            "\n",
-                            "       MolWt     LogP  HBD   HBA    TPSA  \n",
-                            "0    135.166  1.64500  1.0   1.0   29.10  \n",
-                            "1    222.251 -0.85610  2.0   6.0  115.04  \n",
-                            "3    230.315  1.66969  1.0   4.0   36.95  \n",
-                            "4    380.466  1.35302  3.0   6.0  110.88  \n",
-                            "5    293.374  2.92876  0.0   5.0   78.29  \n",
-                            "..       ...      ...  ...   ...     ...  \n",
-                            "568  297.745 -0.35130  3.0   5.0  118.36  \n",
-                            "569  365.842  2.71412  2.0   4.0   92.50  \n",
-                            "570  389.412 -0.44180  4.0  10.0  134.54  \n",
-                            "571  157.213  0.83610  2.0   2.0   63.32  \n",
-                            "573  300.571  1.56400  4.0   2.0  115.06  \n",
+                            "                                                  Drug  Y  \\\n",
+                            "0                                      CC(=O)Nc1ccccc1  1   \n",
+                            "1                           CC(=O)Nc1nnc(S(N)(=O)=O)s1  1   \n",
+                            "3                      Cc1c(N(C)C)c(=N)n(-c2ccccc2)n1C  1   \n",
+                            "4        COc1ccccc1OCCNC[C@@H](O)c1ccc(C)cc1S(N)(=O)=O  1   \n",
+                            "5             CC(C)(C#N)c1cc(Cn2cncn2)cc(C(C)(C)C#N)c1  1   \n",
+                            "..                                                 ... ..   \n",
+                            "568                 NS(=O)(=O)c1cc2c(cc1Cl)NCNS2(=O)=O  1   \n",
+                            "569  Cc1ccccc1N1C(=O)c2cc(S(N)(=O)=O)c(Cl)cc2N[C@@H]1C  1   \n",
+                            "570  Cn1c(=O)c2c(ncn2CCCNC[C@@H](O)c2cc(O)cc(O)c2)n...  1   \n",
+                            "571                        NC[C@H]1CC[C@@H](C(=O)O)CC1  1   \n",
+                            "573                 O=P(O)(O)C(Cc1ccc(Cl)cc1)P(=O)(O)O  0   \n",
+                            "\n",
+                            "                                               mol    MolWt     LogP  HBD  \\\n",
+                            "0    <rdkit.Chem.rdchem.Mol object at 0x295fd8890>  135.166  1.64500  1.0   \n",
+                            "1    <rdkit.Chem.rdchem.Mol object at 0x295fd9620>  222.251 -0.85610  2.0   \n",
+                            "3    <rdkit.Chem.rdchem.Mol object at 0x295fd99a0>  230.315  1.66969  1.0   \n",
+                            "4    <rdkit.Chem.rdchem.Mol object at 0x295fd9af0>  380.466  1.35302  3.0   \n",
+                            "5    <rdkit.Chem.rdchem.Mol object at 0x295fd9b60>  293.374  2.92876  0.0   \n",
+                            "..                                             ...      ...      ...  ...   \n",
+                            "568  <rdkit.Chem.rdchem.Mol object at 0x296009460>  297.745 -0.35130  3.0   \n",
+                            "569  <rdkit.Chem.rdchem.Mol object at 0x2960094d0>  365.842  2.71412  2.0   \n",
+                            "570  <rdkit.Chem.rdchem.Mol object at 0x296009540>  389.412 -0.44180  4.0   \n",
+                            "571  <rdkit.Chem.rdchem.Mol object at 0x2960095b0>  157.213  0.83610  2.0   \n",
+                            "573  <rdkit.Chem.rdchem.Mol object at 0x296009690>  300.571  1.56400  4.0   \n",
+                            "\n",
+                            "      HBA    TPSA  \n",
+                            "0     1.0   29.10  \n",
+                            "1     6.0  115.04  \n",
+                            "3     4.0   36.95  \n",
+                            "4     6.0  110.88  \n",
+                            "5     5.0   78.29  \n",
+                            "..    ...     ...  \n",
+                            "568   5.0  118.36  \n",
+                            "569   4.0   92.50  \n",
+                            "570  10.0  134.54  \n",
+                            "571   2.0   63.32  \n",
+                            "573   2.0  115.06  \n",
                             "\n",
-                            "[468 rows x 10 columns]"
+                            "[493 rows x 9 columns]"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 42,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "hia_data.query(criteria_query)"
             ]
@@ -5361,13 +5498,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `useful_rdkit_utils-0.5/notebooks/demo_descriptors.ipynb` & `useful_rdkit_utils-0.51/notebooks/demo_descriptors.ipynb`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/notebooks/demo_ring_systems.ipynb` & `useful_rdkit_utils-0.51/notebooks/demo_ring_systems.ipynb`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/notebooks/demo_useful_rdkit_utils.ipynb` & `useful_rdkit_utils-0.51/notebooks/demo_useful_rdkit_utils.ipynb`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/notebooks/explore_functional_group_filters.ipynb` & `useful_rdkit_utils-0.51/notebooks/explore_functional_group_filters.ipynb`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/notebooks/zinc_sample.smi` & `useful_rdkit_utils-0.51/notebooks/zinc_sample.smi`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/tests/ring_freq_test.csv` & `useful_rdkit_utils-0.51/tests/ring_freq_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/tests/ring_test.csv` & `useful_rdkit_utils-0.51/tests/ring_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/tests/test.smi` & `useful_rdkit_utils-0.51/tests/test.smi`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/tests/test_reos.py` & `useful_rdkit_utils-0.51/tests/test_reos.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/tests/test_ring_systems.py` & `useful_rdkit_utils-0.51/tests/test_ring_systems.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/tests/test_useful_rdkit_utils.py` & `useful_rdkit_utils-0.51/tests/test_useful_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/descriptors.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/descriptors.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/geometry.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/geometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
 import numpy as np
 import py3Dmol
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from rdkit.Chem.Descriptors3D import NPR1, NPR2
+from rdkit.Chem.rdFMCS import FindMCS
 from rdkit.Chem.rdMolTransforms import ComputeCentroid
 from rdkit.Chem.rdchem import Mol
 
 
 # ----------- Molecular geometry
 def get_center(mol) -> np.ndarray:
     """Get the geometric center of an RDKit molecule
@@ -57,14 +58,37 @@
         AllChem.MMFFOptimizeMoleculeConfs(mol)
         mol = Chem.RemoveHs(mol)
     except ValueError:
         mol = None
     return mol
 
 
+def mcs_rmsd(mol_1: Mol, mol_2: Mol) -> float:
+    """
+    Calculate the minimum Root Mean Square Deviation (RMSD) between the Maximum Common Substructure (MCS)
+    of two RDKit molecule objects.
+
+    :param mol_1: The first RDKit molecule object.
+    :param mol_2: The second RDKit molecule object.
+    :return: The minimum RMSD as a float.
+    """
+    mcs_res = FindMCS([mol_1, mol_2])
+    pat = Chem.MolFromSmarts(mcs_res.smartsString)
+    match_1 = mol_1.GetSubstructMatches(pat)
+    match_2 = mol_2.GetSubstructMatches(pat)
+    min_rmsd = 1e6
+    for m1 in match_1:
+        for m2 in match_2:
+            crd_1 = mol_1.GetConformer(0).GetPositions()[list(m1)]
+            crd_2 = mol_2.GetConformer(0).GetPositions()[list(m2)]
+            rmsd = np.sqrt((((crd_1 - crd_2) ** 2).sum()).mean())
+            min_rmsd = min(min_rmsd, rmsd)
+    return min_rmsd
+
+
 # from https://birdlet.github.io/2019/10/02/py3dmol_example/
 def MolTo3DView(mol, size=(300, 300), style="stick", surface=False, opacity=0.5) -> py3Dmol.view:
     """Draw molecule in 3D
 
     :mol: rdMol, molecule to show
     :size: tuple(int, int), canvas size
     :style: str, type of drawing molecule,
```

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/jupyter_utils.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/misc_utils.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/pandas_utils.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/reactions.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/reactions.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/reos.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/reos.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/ring_systems.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/ring_systems.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/split_utils.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/split_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/stat_utils.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/units.py` & `useful_rdkit_utils-0.51/useful_rdkit_utils/units.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet` & `useful_rdkit_utils-0.51/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/.gitignore` & `useful_rdkit_utils-0.51/.gitignore`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/LICENSE` & `useful_rdkit_utils-0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/README.md` & `useful_rdkit_utils-0.51/README.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/pyproject.toml` & `useful_rdkit_utils-0.51/pyproject.toml`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.5/PKG-INFO` & `useful_rdkit_utils-0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: useful_rdkit_utils
-Version: 0.5
+Version: 0.51
 Summary: A collection of useful RDKit functions
 Project-URL: Homepage, https://github.com/PatWalters/useful_rdkit_utils
 Project-URL: Bug Tracker, https://github.com/PatWalters/useful_rdkit_utils/issues
 Author-email: Pat Walters <wpwalters@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

