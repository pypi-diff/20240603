# Comparing `tmp/tracksegnet-1.2.5.tar.gz` & `tmp/tracksegnet-1.3.0.tar.gz`

## Comparing `tracksegnet-1.2.5.tar` & `tracksegnet-1.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/.readthedocs.yaml
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/Dockerfile
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docker-compose.yaml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/parms.csv
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/requirements.txt
--rwxr-xr-x   0        0        0     5751 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/tracksegnet-main.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/.github/workflows/.draft-pdf.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/.github/workflows/.run-code.yml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/.github/workflows/.run-pylint.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/.github/workflows/pr-readthedocs-link.yml
--rw-r--r--   0        0        0    30265 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/data/toy_example/Cell_10/max_projection.tif
--rw-r--r--   0        0        0  6003241 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/data/toy_example/Cell_10/tracks.simple.mdf
--rw-r--r--   0        0        0    30265 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/data/toy_example/Cell_14/max_projection.tif
--rw-r--r--   0        0        0  2392747 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/data/toy_example/Cell_14/tracks.simple.mdf
--rw-r--r--   0        0        0    30265 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/data/toy_example/Cell_6/max_projection.tif
--rw-r--r--   0        0        0  1505238 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/data/toy_example/Cell_6/tracks.simple.mdf
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/analysis-plots.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/analysis.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/compute_features.rst
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/conf.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/contributing.md
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/data-preparation.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/experimental_tracks.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/generate_lstm_model.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/index.rst
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/installation.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/purposes.md
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/run-instruction.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/simulate_tracks.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/utils.rst
--rw-r--r--   0        0        0   106324 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/img/fig_toy_example_angles.png
--rw-r--r--   0        0        0    87383 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/img/fig_toy_example_displ.png
--rw-r--r--   0        0        0   201498 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/img/fig_toy_example_scatterplot_msd.png
--rw-r--r--   0        0        0    51672 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/img/fig_toy_example_tracklet_proportion.png
--rw-r--r--   0        0        0   144278 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/img/fig_toy_example_vac.png
--rw-r--r--   0        0        0   202885 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/docs/source/img/pipeline.png
--rw-r--r--   0        0        0   456866 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/paper/fig_toy_example_scatterplot_msd.png
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/paper/paper.bib
--rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/paper/paper.md
--rw-r--r--   0        0        0   202885 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/paper/pipeline.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/src/tracksegnet/__init__.py
--rw-r--r--   0        0        0    23579 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/src/tracksegnet/analysis.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/src/tracksegnet/compute_features.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/src/tracksegnet/experimental_tracks.py
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/src/tracksegnet/generate_lstm_model.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/src/tracksegnet/simulate_tracks.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/src/tracksegnet/utils.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/LICENSE
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 tracksegnet-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/Dockerfile
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docker-compose.yaml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/parms.csv
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/requirements.txt
+-rwxr-xr-x   0        0        0     5751 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/tracksegnet-main.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/.github/workflows/.draft-pdf.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/.github/workflows/.pr-readthedocs-link.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/.github/workflows/.run-code.yml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/.github/workflows/.run-pylint.yml
+-rw-r--r--   0        0        0    30265 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/data/toy_example/Cell_10/max_projection.tif
+-rw-r--r--   0        0        0  6003241 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/data/toy_example/Cell_10/tracks.simple.mdf
+-rw-r--r--   0        0        0    30265 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/data/toy_example/Cell_14/max_projection.tif
+-rw-r--r--   0        0        0  2392747 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/data/toy_example/Cell_14/tracks.simple.mdf
+-rw-r--r--   0        0        0    30265 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/data/toy_example/Cell_6/max_projection.tif
+-rw-r--r--   0        0        0  1505238 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/data/toy_example/Cell_6/tracks.simple.mdf
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/analysis-plots.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/analysis.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/compute_features.rst
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/contributing.md
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/data-preparation.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/experimental_tracks.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/generate_lstm_model.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/installation.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/purposes.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/run-instruction.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/simulate_tracks.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/utils.rst
+-rw-r--r--   0        0        0   106324 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/img/fig_toy_example_angles.png
+-rw-r--r--   0        0        0    87383 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/img/fig_toy_example_displ.png
+-rw-r--r--   0        0        0   201498 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/img/fig_toy_example_scatterplot_msd.png
+-rw-r--r--   0        0        0    51672 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/img/fig_toy_example_tracklet_proportion.png
+-rw-r--r--   0        0        0   144278 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/img/fig_toy_example_vac.png
+-rw-r--r--   0        0        0   202885 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/docs/source/img/pipeline.png
+-rw-r--r--   0        0        0   456866 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/paper/fig_toy_example_scatterplot_msd.png
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/paper/paper.bib
+-rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/paper/paper.md
+-rw-r--r--   0        0        0   202885 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/paper/pipeline.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/src/tracksegnet/__init__.py
+-rw-r--r--   0        0        0    23579 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/src/tracksegnet/analysis.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/src/tracksegnet/compute_features.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/src/tracksegnet/experimental_tracks.py
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/src/tracksegnet/generate_lstm_model.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/src/tracksegnet/simulate_tracks.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/src/tracksegnet/utils.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 tracksegnet-1.3.0/PKG-INFO
```

### Comparing `tracksegnet-1.2.5/CONTRIBUTING.md` & `tracksegnet-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/requirements.txt` & `tracksegnet-1.3.0/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 fonttools==4.43.0
 gast==0.4.0
 google-auth==2.16.0
 google-auth-oauthlib==0.4.6
 google-pasta==0.2.0
 grpcio>=1.53.0
 h5py==3.8.0
-idna==3.4
+idna>=3.7
 importlib-metadata==6.0.0
 keras==2.11.0
 kiwisolver==1.4.4
 libclang==15.0.6.1
 Markdown==3.4.1
 MarkupSafe==2.1.2
 matplotlib==3.6.3
@@ -43,17 +43,18 @@
 tensorboard==2.11.2
 tensorboard-data-server==0.6.1
 tensorboard-plugin-wit==1.8.1
 tensorflow==2.11.1
 tensorflow-estimator==2.11.0
 tensorflow-io-gcs-filesystem==0.30.0
 termcolor==2.2.0
-tqdm==4.64.1
+tqdm>=4.66.3
 typing-extensions==4.4.0
 urllib3>=1.26.18
 werkzeug>=2.3.8
 wrapt==1.14.1
 zipp==3.11.0
 myst_parser>=2.0.0
 sphinx>=7.0.0
 sphinx_rtd_theme>=2.0.0
 readthedocs-sphinx-search>=0.1.1
+tracksegnet==1.3.0
```

### Comparing `tracksegnet-1.2.5/tracksegnet-main.py` & `tracksegnet-1.3.0/tracksegnet-main.py`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/.github/workflows/.draft-pdf.yml` & `tracksegnet-1.3.0/.github/workflows/.draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/.github/workflows/.run-code.yml` & `tracksegnet-1.3.0/.github/workflows/.run-code.yml`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/.github/workflows/.run-pylint.yml` & `tracksegnet-1.3.0/.github/workflows/.run-pylint.yml`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/data/toy_example/Cell_10/max_projection.tif` & `tracksegnet-1.3.0/data/toy_example/Cell_10/max_projection.tif`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/data/toy_example/Cell_10/tracks.simple.mdf` & `tracksegnet-1.3.0/data/toy_example/Cell_10/tracks.simple.mdf`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/data/toy_example/Cell_14/max_projection.tif` & `tracksegnet-1.3.0/data/toy_example/Cell_14/max_projection.tif`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/data/toy_example/Cell_14/tracks.simple.mdf` & `tracksegnet-1.3.0/data/toy_example/Cell_14/tracks.simple.mdf`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/data/toy_example/Cell_6/max_projection.tif` & `tracksegnet-1.3.0/data/toy_example/Cell_6/max_projection.tif`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/data/toy_example/Cell_6/tracks.simple.mdf` & `tracksegnet-1.3.0/data/toy_example/Cell_6/tracks.simple.mdf`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/conf.py` & `tracksegnet-1.3.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'tracksegnet'
 copyright = '2024, H. Kabbech'
 author = 'H. Kabbech'
-release = '1.0.0'
+release = '1.3.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['myst_parser', 'sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `tracksegnet-1.2.5/docs/source/data-preparation.md` & `tracksegnet-1.3.0/docs/source/data-preparation.md`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/index.rst` & `tracksegnet-1.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/installation.md` & `tracksegnet-1.3.0/docs/source/installation.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-# Installation and requirements
+# Installation
 
-## Clone the repository
+## Installation with pip
 
-```bash
+```
+[sudo] pip install tracksegnet
+```
+
+## Installation from the GitHub repository and requirements
+
+- Clone the repository
+```
 git clone https://github.com/hkabbech/TrackSegNet.git
 cd TrackSegNet
 ```
 
-## Either create and run a docker container
+- Either create and run a docker container
 
 ```bash
 # Build a docker image (Rebuild the image after changing the parameters):
 docker compose build
 # Run the container:
 docker compose run tracksegnet-env
 ```
 
-## Or create a virtual environment and install the packages
+- Or create a virtual environment and install the packages
 
-Requirement: python3.8 or equivalent and the virtualenv library
+Requirement: python={3.8, 3.9, 3.10} and the virtualenv library
 
 ```bash
 # Create the environment:
-python -m venv tracksegnet-env
-# virtualenv -p /usr/bin/python3 tracksegnet-env
+python -m venv tracksegnet-env # or virtualenv -p /usr/bin/python3 tracksegnet-env
 # Activate the environment:
-source ./tracksegnet-env/bin/activate # for Windows PowerShell: .\tracksegnet-env\Scripts\Activate.ps1 (run as administrator)
+ source ./tracksegnet-env/bin/activate # Or source ./tracksegnet-env/Scripts/activate for Windows. For PowerShell: .\tracksegnet-env\Scripts\Activate.ps1 (run as administrator)
 # Install the required python libraries:
-python -m pip install -r requirements.txt
+pip install -e . # or python -m pip install -r requirements.txt
 ```
 
 Note for later, to deactivate the virtual environment, type `deactivate`.
```

### Comparing `tracksegnet-1.2.5/docs/source/purposes.md` & `tracksegnet-1.3.0/docs/source/purposes.md`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/img/fig_toy_example_angles.png` & `tracksegnet-1.3.0/docs/source/img/fig_toy_example_angles.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/img/fig_toy_example_displ.png` & `tracksegnet-1.3.0/docs/source/img/fig_toy_example_displ.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/img/fig_toy_example_scatterplot_msd.png` & `tracksegnet-1.3.0/docs/source/img/fig_toy_example_scatterplot_msd.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/img/fig_toy_example_tracklet_proportion.png` & `tracksegnet-1.3.0/docs/source/img/fig_toy_example_tracklet_proportion.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/img/fig_toy_example_vac.png` & `tracksegnet-1.3.0/docs/source/img/fig_toy_example_vac.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/docs/source/img/pipeline.png` & `tracksegnet-1.3.0/docs/source/img/pipeline.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/paper/fig_toy_example_scatterplot_msd.png` & `tracksegnet-1.3.0/paper/fig_toy_example_scatterplot_msd.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/paper/paper.bib` & `tracksegnet-1.3.0/paper/paper.bib`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,14 @@
   pages={24128--24164},
   year={2014},
   doi={10.1039/C4CP03465A},
   url={https://doi.org/10.1039/C4CP03465A},
   publisher={Royal Society of Chemistry}
 }
 
-
-@misc{chollet2015,
-  title={Keras},
-  author={Chollet, F. and others},
-  year={2015},
-  howpublished={\url{https://keras.io}},
-}
-
-
 @article{lundahl1986,
   title={Fractional Brownian motion: A maximum likelihood estimator and its application to image texture},
   author={Lundahl, T. and Ohley, W. J. and Kay, S. M. and Siffert, R.},
   journal={IEEE transactions on Medical Imaging},
   volume={5},
   number={3},
   pages={152--161},
```

### Comparing `tracksegnet-1.2.5/paper/paper.md` & `tracksegnet-1.3.0/paper/paper.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,80 @@
 ---
 title: 'TrackSegNet: a tool for trajectory segmentation into diffusive states using supervised deep learning'
 tags:
-  - Python
   - single-particle tracking
   - trajectory segmentation
   - supervised deep learning
   - mean squared displacement
 authors:
   - name: Hélène Kabbech
     orcid: 0000-0002-9200-2112
-    affiliation: "1"
   - name: Ihor Smal
-    orcid: 0000-0001-7576-7028 
-    affiliation: "1"
+    orcid: 0000-0001-7576-7028
 affiliations:
  - name: Department of Cell Biology, Erasmus University Medical Center, Rotterdam, the Netherlands
-   index: 1
-date: 14 March 2023
+date: June 2024
 bibliography: paper.bib
 ---
 
 # Summary
 
-`TrackSegNet` is a command-line python program, which permits the classification and segmentation of trajectories into diffusive states. A deep neural network is trained for each particular case using synthetic data and trajectory features as inputs. After classification on the experimental data using the trained network, the trajectories are segmentated and grouped per diffusive state. `TrackSegNet` further estimates the motion parameters (the diffusion constant $D$ and anomalous exponent $\alpha$) for each segmented track using the mean squared displacement (MSD) analysis, and computes additional geometric measurements per tracklet state such as the angular distribution and velocity autocorrelation curve. The resulting segmentation and motion parameters are stored as CSV files. Originally developped for the quantification of protein dynamics using single-particle tracking imaging, its use can be extended to any type of trajectory dataset.
+`TrackSegNet` is a command-line python program, which permits the classification and segmentation of trajectories into diffusive states. A deep neural network is trained for each particular case using synthetic data and trajectory features as inputs. After classification on the experimental data using the trained network, the trajectories are segmented and grouped per diffusive state. `TrackSegNet` further estimates the motion parameters (the diffusion constant $D$ and anomalous exponent $\alpha$) for each segmented track using the mean squared displacement (MSD) analysis, and computes additional geometric measurements per tracklet state such as the angular distribution and velocity autocorrelation curve. The resulting segmentation and motion parameters are stored as CSV files. Originally developed for the quantification of protein dynamics using single-particle tracking imaging, its use can be extended to any type of trajectory dataset.
 
 ![Analysis pipeline of TrackSegNet described in two steps. \label{fig:pipeline}](pipeline.png)
 
 # Statement of need
 
-Recent advances in the field of microscopy allow the capture, at nanometer resolution, of the motion of fluorescently-labeled particles in live cells such as proteins or chromatin loci. Therefore, the development of methods to characterize the dynamics of a group of particles has become more than necessary [@munoz2021]. A typical analysis is the classification and segmentation of trajectories into diverse diffusive states when multiple types of motion are present in a dataset (e.g., confined, superdiffusive) due to the properties of the labeled molecule (e.g., protein bound/unbound to the DNA). A few trajectory classification methods have recently been developed by the community, among which can be cited @wagner2017, @hansen2018, @arts2019, @pinholt2021 and @kabbech2022. However, more practical analysis software is needed for direct application use.
+Recent advances in the field of microscopy allow the capture, at nanometer resolution, of the motion of fluorescently-labeled particles in live cells such as proteins or chromatin loci. Therefore, the development of methods to characterize the dynamics of a group of particles has become more than necessary [@munoz2021]. A typical analysis is the classification and segmentation of trajectories into diverse diffusive states when multiple types of motion are present in a dataset (e.g., confined, superdiffusive) due to the properties of the labeled molecule (e.g., protein bound/unbound to the DNA).
 
+Several trajectory classification methods have recently been developed by the community exhibiting a diverse range of methodologies. For instance, @wagner2017 utilizes Random Forests, @hansen2018 relies on histogram of displacements, @pinholt2021 employs hidden  Markov  model (HMM) and @kabbech2022 utilizes an unsupervised denoising technique. However, not all methods have readily available tools for direct application. Consequently, there is a growing need for the development of more user-friendly software tailored for practical implementation.
 
 # Method
 
-This software is based on the method of @arts2019 with major improvements and allows replicability on other datasets.
+This software is based on the method of @arts2019 with major improvements, making use of a stack of LSTM layers trained on synthetic trajectory features. The improvements include the calculation of angles as a feature to better distinguish the trajectory confinment, better management of trajectory gaps, and the use of the mean squared displacement (MSD) instead of the moment scaling spectrum (MSS) analysis to better estimate the dynamics. This version includes a user-friendly software allowing the replicability for other datasets.
 
 ## Neural Network
 
-Tracking particles from 2-dimensional images results in a set $\mathcal{S}$ of trajectories $r_i \in \mathcal{S}$, $i = \left\{1, \dots, P \right\}$,  where $P$ is the total number of trajectories and $r_i(t) = (x_i(t), y_i(t))$ are the 2D coordinates of the particle $i$ at time $t$.
+Tracking particles from 2-dimensional images results in a set $\mathcal{S}$ of trajectories $r_i \in \mathcal{S}$, $i = \left\{1, \dots, P \right\}$,  where $P$ is the total number of trajectories, and $r_i(t) = (x_i(t), y_i(t))$ are the 2D coordinates of the particle $i$ at time $t$.
 
-The network is built using functions from the Keras library [@chollet2015], and is composed of a bidirectional long short-term memory (LSTM) layer (having 200 hidden units) followed by a fully connected time-distributed layer with a `SoftMax` activation function. The inputs of the network are of six trajectory features computed beforehand, while the outputs are probabilities for each trajectory point of belonging to one of the $N$ diffusive states, the predicted state is defined by the highest probability.
+The network is built using functions from the Keras library, and is composed of a bidirectional long short-term memory (LSTM) layer (having 200 hidden units), followed by a fully connected time-distributed layer with a `SoftMax` activation function. The inputs of the network are of six trajectory features previously computed, while the outputs are probabilities for each trajectory point of belonging to one of the $N$ diffusive states, the predicted state is defined by the highest probability.
 
-The computed features along a given trajectory are: the displacements $\Delta x_{\delta=1}$ and $\Delta y_{\delta=1}$ at the first discrete time interval $\delta=1$ (with $\Delta r_\delta (t) = r(t) - r(t+\delta)$), the distances $d_{\delta=1}$ (with $d_\delta (t) = \sqrt{\Delta x_\delta (t)^2 + \Delta y_\delta (t)^2}$), the mean of displacements $\overline{d_{\delta=1,p=1}}$ and $\overline{d_{\delta=2,p=1}}$ (with $\overline{d_{\delta,p}}(t) = \frac{1}{2p+1}\sum_{k=t-p}^{t+p} d_{\delta}(k)$ with $p\geq 1$) and the angles $\theta_{\delta=1}$ between two consecutive displacements. The last feature is an addition to the initial method, used for a better distinction of the trajectory confinement. The first and last trajectory points of each trajectory vector are discarded due to missing computed feature(s).
+The computed features along a given trajectory are: the displacements $\Delta x_{\delta=1}$ and $\Delta y_{\delta=1}$ at the first discrete time interval $\delta=1$ (with $\Delta r_\delta (t) = r(t) - r(t+\delta)$), the distances $d_{\delta=1}$ (with $d_\delta (t) = \sqrt{\Delta x_\delta (t)^2 + \Delta y_\delta (t)^2}$), the mean of displacements $\overline{d_{\delta=1,p=1}}$ and $\overline{d_{\delta=2,p=1}}$ (with $\overline{d_{\delta,p}}(t) = \frac{1}{2p+1}\sum_{k=t-p}^{t+p} d_{\delta}(k)$ with $p\geq 1$) and the angles $\theta_{\delta=1}$ between consecutive displacements. The last feature is an addition to the initial method, used for a better distinction of the trajectory confinement. The first and last trajectory points of each trajectory vector are discarded due to missing computed feature(s).
 
 
 ## Training
 
-The network is trained using synthetic fractional Brownian motion (fBm) trajectories of mixed diffusive states. For this purpose, 10,000 fBm trajectories with a switching mode between states and a total length of 27 frames are generated for each independent training. The fBm process is characterized using the fBm kernel [@lundahl1986] defined as $k_{\text{FBM}}(t) = D\left[\ \lvert t+1\rvert^\alpha  - 2 \lvert t\rvert^\alpha + \lvert t-1\rvert^\alpha\right]$, with $t=\Delta t / \delta$ ($\Delta t$ the time measured between two frames) and the pre-defined motion parameters $m = (D, \alpha)$.
+The network is trained using synthetic fractional Brownian motion (fBm) trajectories exhibiting mixed diffusive states. For this purpose, 10,000 fBm trajectories with a switching mode between states and a total length of 27 frames are generated for each independent training. The fBm process is characterized using the fBm kernel [@lundahl1986] defined as $k_{\text{FBM}}(t) = D\left[\ \lvert t+1\rvert^\alpha  - 2 \lvert t\rvert^\alpha + \lvert t-1\rvert^\alpha\right]$, with $t=\Delta t / \delta$ ($\Delta t$ the time measured between two frames) and the pre-defined motion parameters $m = (D, \alpha)$.
 
 The model is optimized using `Adam` during the training and a categorical cross-entropy loss function.
 
 
 ## Model parameters
 
 The main parameters of the training are tunable from the `params.csv` file to create a new variant of the model:
 
 * `num_states` is an important parameter permitting to decide the number $N$ of diffusive states. This number can vary from 2 to 6 states, but it is recommended to choose 2 to 4 states.
 * `state_i_diff` and `state_i_alpha` the approximate motion parameters $m$ for each of the $N$ diffusive state. The diffusion constant $D$ is dimensionless, and the anomalous exponent value $\alpha$ is ranging from 0 to 2 (]0-1[: subdiffusion, 1: Brownian motion, ]1-2[: superdiffusion).
-* `pt_i_j` the probability of transitionning from the state i to the state j. The total number of probabilities should be $N^2$.
+* `pt_i_j` the probability of transitioning from the state i to the state j. The total number of probabilities should be $N^2$.
 
 The remaining parameters are related to the experimental dataset:
 
 * `data_path`, the path of the dataset of trajectories to segment.
-* `track_format`, the format of the files containing the trajectory coordinates, either `MDF` (see `MTrackJ` data file format) or `CSV`
+* `track_format`, the format of the files containing the trajectory coordinates, either in `MDF` (see `MTrackJ` data file format) or `CSV`
 * `time_frame`, the time interval between two trajectory points in seconds.
 * `pixel_size`, the dimension of a pixel in $\mu m$.
 
 
 ## Classification and MSD analysis
 
 Before computing the features for each experimental trajectory, gaps in trajectories of length 1 are filled by a randomly generated point; while the larger gaps are split in two separate trajectories. Each point is therefore classified as one of the $N$ diffusive states using the trained LSTM model. Based on the state classification, the trajectories are segmented and the motion parameters are estimated for each segmented track (longer than 5 frames) using the MSD analysis. The latter consists of applying a least-square fit from the logarithm form of the MSD power-law equation [@metzler2014]. Both $D$ and $\alpha$ distributions can be plotted in a scatterplot as shown in \autoref{fig:pipeline}. The new probability transition matrix and proportion of tracklet points in each diffusive state are also calculated.
 
+In brief, the outputs of this software permit the segmentation of trajectories into shorter segments based on their type of diffusion. Measurements are then performed (MSD analysis, angles and distributions) to evaluate the dynamics for each state group/segment.
+
 
 # Acknowledgements
 
-We would like to thanks Selçuk Yavuz and Martin E. van Royen for sharing SPT data used as a toy example, and Maarten W. Paul for testing the software and fixing minor mistakes. \autoref{fig:pipeline} was partially created using Biorender. This work was supported by the Dutch Research Council (NWO) through the Building Blocks of Life research program (GENOMETRACK project, Grant No. 737.016.014).
+We would like to thank Selçuk Yavuz and Martin E. van Royen for sharing SPT data used as a toy example, and Maarten W. Paul for testing the software and fixing minor mistakes. \autoref{fig:pipeline} was partially created using Biorender. This work was supported by the Dutch Research Council (NWO) through the Building Blocks of Life research program (GENOMETRACK project, Grant No. 737.016.014).
 
 
 # References
```

### Comparing `tracksegnet-1.2.5/paper/pipeline.png` & `tracksegnet-1.3.0/paper/pipeline.png`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/src/tracksegnet/analysis.py` & `tracksegnet-1.3.0/src/tracksegnet/analysis.py`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/src/tracksegnet/compute_features.py` & `tracksegnet-1.3.0/src/tracksegnet/compute_features.py`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/src/tracksegnet/experimental_tracks.py` & `tracksegnet-1.3.0/src/tracksegnet/experimental_tracks.py`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/src/tracksegnet/generate_lstm_model.py` & `tracksegnet-1.3.0/src/tracksegnet/generate_lstm_model.py`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/src/tracksegnet/simulate_tracks.py` & `tracksegnet-1.3.0/src/tracksegnet/simulate_tracks.py`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/src/tracksegnet/utils.py` & `tracksegnet-1.3.0/src/tracksegnet/utils.py`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/LICENSE` & `tracksegnet-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tracksegnet-1.2.5/README.md` & `tracksegnet-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-![Python version](https://img.shields.io/badge/python-3.8-brightgreen.svg) [![DOI](https://zenodo.org/badge/583738628.svg)](https://zenodo.org/badge/latestdoi/583738628)
-
+![Python version](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-brightgreen.svg) [![pypi](https://img.shields.io/pypi/v/tracksegnet.svg?maxAge=3600)](https://pypi.org/project/tracksegnet/) [![DOI](https://zenodo.org/badge/583738628.svg)](https://zenodo.org/badge/latestdoi/583738628)
 
 # TrackSegNet
 
 ## Purposes
 
 Recent advances in the field of microscopy allow the capture, at nanometer resolution, of the motion of fluorescently-labeled particles in live cells such as proteins or chromatin loci. Therefore, the development of methods to characterize the dynamics of a group of particles has become more than necessary.
 
@@ -14,42 +13,50 @@
 - Upon completion of the training process, the experimental trajectories are classified at each point using the trained model. Subsequently, the trajectories are segmented and grouped based on their respective diffusive states. In this context, "diffusive states" refer to the distinct modes or patterns observed in the movement of particles.
 
 - For each segmented track, the diffusion constant (![equation](https://latex.codecogs.com/svg.image?\inline&space;D)) and anomalous exponent (![equation](https://latex.codecogs.com/svg.image?\inline&space;\alpha)) are further estimated. This is accomplished by computing the mean squared displacement (MSD), providing valuable insights into the dynamic behavior of the particles within each identified diffusive state.
 
 
 ![pipeline](paper/pipeline.png)
 
-## Installation and requirements
+## Installation
+
+### Installation with pip
+
+```
+[sudo] pip install tracksegnet
+```
+
+### Installation from the GitHub repository and requirements
 
-### Clone the repository
+- Clone the repository
 ```
 git clone https://github.com/hkabbech/TrackSegNet.git
 cd TrackSegNet
 ```
 
-### Either create and run a docker container
+- Either create and run a docker container
 
 ```bash
 # Build a docker image (Rebuild the image after changing the parameters):
 docker compose build
 # Run the container:
 docker compose run tracksegnet-env
 ```
 
-### Or create a virtual environment and install the packages
+- Or create a virtual environment and install the packages
 
-Requirement: python3.8 or equivalent and the virtualenv library
+Requirement: python={3.8, 3.9, 3.10} and the virtualenv library
 
 ```bash
 # Create the environment:
-python -m venv tracksegnet-env # virtualenv -p /usr/bin/python3 tracksegnet-env
+python -m venv tracksegnet-env # or virtualenv -p /usr/bin/python3 tracksegnet-env
 # Activate the environment:
-source ./tracksegnet-env/bin/activate # for Windows PowerShell: .\tracksegnet-env\Scripts\Activate.ps1 (run as administrator)
+ source ./tracksegnet-env/bin/activate # Or source ./tracksegnet-env/Scripts/activate for Windows. For PowerShell: .\tracksegnet-env\Scripts\Activate.ps1 (run as administrator)
 # Install the required python libraries:
-pip install -e . # python -m pip install -r requirements.txt
+pip install -e . # or python -m pip install -r requirements.txt
 ```
 
 Note for later, to deactivate the virtual environment, type `deactivate`.
 
 
 ## Prepare your data
```

### Comparing `tracksegnet-1.2.5/pyproject.toml` & `tracksegnet-1.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tracksegnet"
-version = "1.2.5"
+version = "1.3.0"
 dynamic = ["dependencies"]
 authors = [
   { name="Hélène Kabbech", email="helene.kabbech@gmail.com" },
 ]
 description = "Segmentation of trajectories into diffusive states using supervised LSTM network"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tracksegnet-1.2.5/PKG-INFO` & `tracksegnet-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tracksegnet
-Version: 1.2.5
+Version: 1.3.0
 Summary: Segmentation of trajectories into diffusive states using supervised LSTM network
 Project-URL: Homepage, https://github.com/hkabbech/TrackSegNet
 Project-URL: Issues, https://github.com/hkabbech/TrackSegNet/issues
 Author-email: Hélène Kabbech <helene.kabbech@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Requires-Dist: fonttools==4.43.0
 Requires-Dist: gast==0.4.0
 Requires-Dist: google-auth-oauthlib==0.4.6
 Requires-Dist: google-auth==2.16.0
 Requires-Dist: google-pasta==0.2.0
 Requires-Dist: grpcio>=1.53.0
 Requires-Dist: h5py==3.8.0
-Requires-Dist: idna==3.4
+Requires-Dist: idna>=3.7
 Requires-Dist: importlib-metadata==6.0.0
 Requires-Dist: keras==2.11.0
 Requires-Dist: kiwisolver==1.4.4
 Requires-Dist: libclang==15.0.6.1
 Requires-Dist: markdown==3.4.1
 Requires-Dist: markupsafe==2.1.2
 Requires-Dist: matplotlib==3.6.3
@@ -59,24 +59,24 @@
 Requires-Dist: tensorboard-data-server==0.6.1
 Requires-Dist: tensorboard-plugin-wit==1.8.1
 Requires-Dist: tensorboard==2.11.2
 Requires-Dist: tensorflow-estimator==2.11.0
 Requires-Dist: tensorflow-io-gcs-filesystem==0.30.0
 Requires-Dist: tensorflow==2.11.1
 Requires-Dist: termcolor==2.2.0
-Requires-Dist: tqdm==4.64.1
+Requires-Dist: tqdm>=4.66.3
+Requires-Dist: tracksegnet==1.3.0
 Requires-Dist: typing-extensions==4.4.0
 Requires-Dist: urllib3>=1.26.18
 Requires-Dist: werkzeug>=2.3.8
 Requires-Dist: wrapt==1.14.1
 Requires-Dist: zipp==3.11.0
 Description-Content-Type: text/markdown
 
-![Python version](https://img.shields.io/badge/python-3.8-brightgreen.svg) [![DOI](https://zenodo.org/badge/583738628.svg)](https://zenodo.org/badge/latestdoi/583738628)
-
+![Python version](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-brightgreen.svg) [![pypi](https://img.shields.io/pypi/v/tracksegnet.svg?maxAge=3600)](https://pypi.org/project/tracksegnet/) [![DOI](https://zenodo.org/badge/583738628.svg)](https://zenodo.org/badge/latestdoi/583738628)
 
 # TrackSegNet
 
 ## Purposes
 
 Recent advances in the field of microscopy allow the capture, at nanometer resolution, of the motion of fluorescently-labeled particles in live cells such as proteins or chromatin loci. Therefore, the development of methods to characterize the dynamics of a group of particles has become more than necessary.
 
@@ -87,42 +87,50 @@
 - Upon completion of the training process, the experimental trajectories are classified at each point using the trained model. Subsequently, the trajectories are segmented and grouped based on their respective diffusive states. In this context, "diffusive states" refer to the distinct modes or patterns observed in the movement of particles.
 
 - For each segmented track, the diffusion constant (![equation](https://latex.codecogs.com/svg.image?\inline&space;D)) and anomalous exponent (![equation](https://latex.codecogs.com/svg.image?\inline&space;\alpha)) are further estimated. This is accomplished by computing the mean squared displacement (MSD), providing valuable insights into the dynamic behavior of the particles within each identified diffusive state.
 
 
 ![pipeline](paper/pipeline.png)
 
-## Installation and requirements
+## Installation
+
+### Installation with pip
+
+```
+[sudo] pip install tracksegnet
+```
+
+### Installation from the GitHub repository and requirements
 
-### Clone the repository
+- Clone the repository
 ```
 git clone https://github.com/hkabbech/TrackSegNet.git
 cd TrackSegNet
 ```
 
-### Either create and run a docker container
+- Either create and run a docker container
 
 ```bash
 # Build a docker image (Rebuild the image after changing the parameters):
 docker compose build
 # Run the container:
 docker compose run tracksegnet-env
 ```
 
-### Or create a virtual environment and install the packages
+- Or create a virtual environment and install the packages
 
-Requirement: python3.8 or equivalent and the virtualenv library
+Requirement: python={3.8, 3.9, 3.10} and the virtualenv library
 
 ```bash
 # Create the environment:
-python -m venv tracksegnet-env # virtualenv -p /usr/bin/python3 tracksegnet-env
+python -m venv tracksegnet-env # or virtualenv -p /usr/bin/python3 tracksegnet-env
 # Activate the environment:
-source ./tracksegnet-env/bin/activate # for Windows PowerShell: .\tracksegnet-env\Scripts\Activate.ps1 (run as administrator)
+ source ./tracksegnet-env/bin/activate # Or source ./tracksegnet-env/Scripts/activate for Windows. For PowerShell: .\tracksegnet-env\Scripts\Activate.ps1 (run as administrator)
 # Install the required python libraries:
-pip install -e . # python -m pip install -r requirements.txt
+pip install -e . # or python -m pip install -r requirements.txt
 ```
 
 Note for later, to deactivate the virtual environment, type `deactivate`.
 
 
 ## Prepare your data
```

