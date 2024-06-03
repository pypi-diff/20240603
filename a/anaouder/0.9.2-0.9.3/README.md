# Comparing `tmp/anaouder-0.9.2.tar.gz` & `tmp/anaouder-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaouder-0.9.2.tar", last modified: Tue May 14 16:51:19 2024, max compression
+gzip compressed data, was "anaouder-0.9.3.tar", last modified: Sun Jun  2 16:34:24 2024, max compression
```

## Comparing `anaouder-0.9.2.tar` & `anaouder-0.9.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.330364 anaouder-0.9.2/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2018 2024-05-14 16:50:44.000000 anaouder-0.9.2/CHANGELOG.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     7264 2024-05-14 16:51:19.330364 anaouder-0.9.2/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5609 2024-05-13 11:51:35.000000 anaouder-0.9.2/README-fr.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5083 2024-05-13 11:52:12.000000 anaouder-0.9.2/README.md
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.2/anaouder/__init__.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11650 2024-05-13 11:54:43.000000 anaouder-0.9.2/anaouder/adskrivan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder/asr/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.2/anaouder/asr/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.2/anaouder/asr/inorm_units.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3698 2024-03-09 16:05:14.000000 anaouder-0.9.2/anaouder/asr/models.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6255 2024-05-13 10:09:57.000000 anaouder-0.9.2/anaouder/asr/post_processing.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/asr/postproc_sub.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4870 2024-05-14 16:45:26.000000 anaouder-0.9.2/anaouder/asr/recognizer.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder/audio/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5482 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/audio/__init__.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.330364 anaouder-0.9.2/anaouder/dicts/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.2/anaouder/dicts/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/acronyms.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/corrected_tokens.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/noun_f.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/noun_m.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/proper_nouns_phon.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.2/anaouder/dicts/standard_tokens.tsv
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.2/anaouder/istitlan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.2/anaouder/linennan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.2/anaouder/mikro.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.2/anaouder/normalizan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.330364 anaouder-0.9.2/anaouder/text/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.2/anaouder/text/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.2/anaouder/text/definitions.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.2/anaouder/text/inverse_normalizer.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.2/anaouder/text/normalizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.2/anaouder/text/tokenizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.2/anaouder/text/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5396 2024-05-13 08:15:45.000000 anaouder-0.9.2/anaouder/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-05-14 16:50:31.000000 anaouder-0.9.2/anaouder/version.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-14 16:51:19.326364 anaouder-0.9.2/anaouder.egg-info/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     7264 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      979 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/SOURCES.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/dependency_links.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      189 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/entry_points.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/requires.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-05-14 16:51:19.000000 anaouder-0.9.2/anaouder.egg-info/top_level.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-05-14 16:51:19.330364 anaouder-0.9.2/setup.cfg
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2083 2024-05-13 11:56:35.000000 anaouder-0.9.2/setup.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.869675 anaouder-0.9.3/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2208 2024-06-02 16:11:42.000000 anaouder-0.9.3/CHANGELOG.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     1078 2023-03-09 20:15:12.000000 anaouder-0.9.3/LICENSE
+-rw-r--r--   0 gweltaz   (1000) gweltaz   (1000)     6544 2024-06-02 16:34:24.868675 anaouder-0.9.3/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5609 2024-05-13 11:51:35.000000 anaouder-0.9.3/README-fr.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4965 2024-05-17 14:24:32.000000 anaouder-0.9.3/README.md
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.854676 anaouder-0.9.3/anaouder/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.3/anaouder/__init__.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11584 2024-05-15 07:55:00.000000 anaouder-0.9.3/anaouder/adskrivan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.860675 anaouder-0.9.3/anaouder/asr/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.3/anaouder/asr/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.3/anaouder/asr/inorm_units.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3711 2024-06-02 16:13:08.000000 anaouder-0.9.3/anaouder/asr/models.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6255 2024-05-13 10:09:57.000000 anaouder-0.9.3/anaouder/asr/post_processing.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/asr/postproc_sub.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4870 2024-05-14 16:45:26.000000 anaouder-0.9.3/anaouder/asr/recognizer.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.861675 anaouder-0.9.3/anaouder/audio/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5690 2024-05-17 20:18:57.000000 anaouder-0.9.3/anaouder/audio/__init__.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.865675 anaouder-0.9.3/anaouder/dicts/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.3/anaouder/dicts/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/acronyms.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/corrected_tokens.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/noun_f.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/noun_m.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/proper_nouns_phon.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.3/anaouder/dicts/standard_tokens.tsv
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.3/anaouder/istitlan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.3/anaouder/linennan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.3/anaouder/mikro.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.3/anaouder/normalizan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.867675 anaouder-0.9.3/anaouder/text/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.3/anaouder/text/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.3/anaouder/text/definitions.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.3/anaouder/text/inverse_normalizer.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.3/anaouder/text/normalizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.3/anaouder/text/tokenizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.3/anaouder/text/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5396 2024-05-13 08:15:45.000000 anaouder-0.9.3/anaouder/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-06-02 16:12:15.000000 anaouder-0.9.3/anaouder/version.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-06-02 16:34:24.868675 anaouder-0.9.3/anaouder.egg-info/
+-rw-r--r--   0 gweltaz   (1000) gweltaz   (1000)     6544 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      987 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      188 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/entry_points.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/requires.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-06-02 16:34:24.000000 anaouder-0.9.3/anaouder.egg-info/top_level.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-06-02 16:34:24.869675 anaouder-0.9.3/setup.cfg
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2083 2024-06-02 16:33:31.000000 anaouder-0.9.3/setup.py
```

### Comparing `anaouder-0.9.2/CHANGELOG.md` & `anaouder-0.9.3/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.3] - 2024-06-02
+
+- Fixed model selection when outputing to a txt file.
+- Fixed inference with progress bar for MKV files.
+- Fixed MacOS compatibility issue when downloading models.
+
 ## [0.9.2] - 2024-05-14
 
 - Better segmentation when decoding to a text file with `-o/--output` option.
 - Shows a progress bar when decoding to a text file with `-o/--output` option.
 - Included Anaouder version in EAF headers.
 - Removed optional use of translation dictionaries.
```

### Comparing `anaouder-0.9.2/PKG-INFO` & `anaouder-0.9.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,142 @@
 Metadata-Version: 2.1
 Name: anaouder
-Version: 0.9.2
+Version: 0.9.3
 Summary: Breton language speech-to-text tools
 Home-page: https://github.com/gweltou/vosk-br
 Author: Gweltaz Duval-Guennoc
 Author-email: gweltou@hotmail.com
 License: MIT
-Description: [![pypi version](https://img.shields.io/pypi/v/anaouder)](https://pypi.org/project/anaouder/)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
-        
-        # Anaouder
-        
-        [E brezhoneg](./README.md)
-        
-        Reconnaissance vocale pour le breton avec Vosk.
-        
-        Ce projet est développé bénévolement. Vous pouvez le soutenir par un don :
-        [![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
-        
-        Une [version en ligne](https://translate.bzh/), développée par Philippe Argouarch, est également disponible.
-        
-        ## Présentation
-        
-        Modèle de reconnaissance vocale (*speech-to-text*) entraîné avec le framework [Kaldi](https://www.kaldi-asr.org/), au format [Vosk](https://github.com/alphacep/vosk-api).\
-        Il est accompagné de scripts permettant la retranscription automatique de fichiers audio et video, l'alignement texte/son pour la création de sous-titres, ou encore l'inférence en temps réel à l'aide d'un microphone.
-        
-        Principaux avantages :
-        
-        * **Léger**. Les modèles Vosk pèsent moins de 100 Mo et peuvent tourner sur une large gamme d'appareils : ordinateurs **sans GPU**, RaspberryPi, smartphone Android...
-        * **Rapide**. L'inférence se fait en **temps réel**, même sur une machine un peu datée.
-        * **Local**. Fonctionne sans connexion internet. Vos données restent donc sur votre appareil.
-        * **Libre et gratuit**. La licence MIT vous permet de modifier le logiciel et de l'intégrer dans d'autres applications.
-        
-        Le nombre d'heures d'enregistrement audio utilisé pour entraîner le modèle est relativement faible mais progresse peu à peu.
-        En dehors du projet [Common Voice](https://commonvoice.mozilla.org/br) de Mozilla, les enregistrements retranscrits [libres de droit](https://creativecommons.org/licenses/) sont rares pour le breton. Toute aide sur ce terrain sera la bienvenue !
-        
-        ## Installation
-        
-        Les scripts nécessitent l'installation de [Python3](https://www.python.org/downloads/). L'installation du module de reconnaissance vocale se fera ensuite dans un terminal, en exécutant la commande suivante :
-        
-        ```bash
-        pip install anaouder
-        ```
-        
-        Une fois installé, et à mesure que de nouvelles versions du modèle de reconnaissance vocale seront proposées, vous pourrez mettre à jour le logiciel avec :
-        
-        ```bash
-        pip install --upgrade anaouder
-        ```
-        
-        
-        ## Retranscrire un fichier audio ou video
-        
-        Une fois le module installé, la commande `adskrivan` permet de retranscrire un fichier audio ou video depuis le terminal. A la première exécution de la commande, il vous faudra patienter le temps de l'installation du module `static_ffmpeg` (programme de conversion pour les fichiers audio/video). Cette installation ne se fera qu'une seule fois.
-        
-        ```bash
-        adskrivan NOM_DU_FICHIER
-        ```
-        
-        Le résultat de la transcription s'affichera dans le terminal par défaut. Vous pouvez toutefois préciser le nom d'un fichier dans lequel écrire, avec l'option `-o`
-        
-        ```bash
-        adskrivan NOM_DU_FICHIER -o SORTIE.txt
-        ```
-        
-        ## Utilisation avec un microphone
-        
-        Depuis un terminal, invoquez la commande `mikro`.
-        
-        Si aucun texte n'apparaît, vous pouvez afficher la liste des interfaces audio avec la commande :
-        
-        ```bash
-        mikro -l
-        ```
-        
-        Vous pourrez ensuite préciser, en argument, le numéro de l'interface à utiliser pour l'inférence :
-        
-        ```bash
-        mikro -d NUMERO_INTERFACE
-        ```
-        
-        ## Alignement d'un texte d'après un audio
-        
-        Il est possible d'aligner un texte d'après un fichier audio ou video à l'aide de la commande `linennan`. Vous obtiendrez un fichier contenant le texte original, accompagné de marqueurs temporels, au format `srt` (fichier de sous-titres Subrip).\
-        Le fichier texte doit être un texte brut (extension `.txt`) où chaque ligne correspondra à une ligne de sous-titre.
-        
-        ```bash
-        linennan FICHIER_SON_OU_VIDEO FICHIER_TEXTE -o sous-titres.srt
-        ```
-        
-        (export au format `eaf`, pour le logiciel ELAN, à venir...)
-        
-        ## Création automatique de sous-titres
-        
-        Vous pouvez également laisser le modèle de reconnaissance vocale retranscrire les paroles pour la création de sous-titres, au format `srt` (Subrip).
-        
-        ```bash
-        istitlan FICHIER_SON_OU_VIDEO
-        ```
-        
-        ## Utilisation du modèle avec d'autres logiciel 
-        
-        *L'utilisation du modèle brut dans d'autres logiciel est possible mais n'est pas conseillé, puisque qu'elle omettra le post-traitement proposé par le module `anaouder` : le replacement des tirets de liaison et la normalisation-inverse des nombres notamment.*
-        
-        Le modèle brut est accessible sous le dossier `anaouder/models` ou par le lien [releases](https://github.com/gweltou/vosk-br/releases).
-        
-        ### Audapolis
-        
-        Il est possible d'utiliser le modèle avec le logiciel [Audapolis](https://github.com/bugbakery/audapolis), qui offre également le confort d'une interface graphique.
-        
-        ### Kdenlive
-        
-        Le logiciel de montage video [Kdenlive](https://kdenlive.org/) permet l'utilisation de modèles Vosk pour la retranscription automatique de sous-titres.\
-        Voir la [documentation](https://docs.kdenlive.org/en/effects_and_compositions/speech_to_text.html).
-        
-        ## Remerciements
-        
-        Le développement de cet outil a été possible grâce aux logiciels libres sur lesquels il se base : Kaldi, Vosk et le correcteur automatique [Hunspell](https://github.com/Drouizig/hunspell-br) de An Drouizig.\
-        Le modèle de reconnaissance vocale n'aurait jamais pu être entraîne sans les voix et les textes de nombreux contributeurs, issus de : Mozilla Common Voice, Dizale, Brezhoweb, RKB, Kaouen.net, Ya!, Becedia, France3 et Dastum.\
-        Je remercie enfin Elen Cariou, Jean-Mari Ollivier, Karen Treguier, Mélanie Jouitteau et Pêr Morvan pour leur aide et leur soutien.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: static_ffmpeg
+Requires-Dist: sounddevice
+Requires-Dist: vosk
+Requires-Dist: srt
+Requires-Dist: jiwer
+Requires-Dist: pydub>=0.25.1
+Requires-Dist: pytz
+Requires-Dist: tqdm==4.64.1
+
+[![pypi version](https://img.shields.io/pypi/v/anaouder)](https://pypi.org/project/anaouder/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
+
+# Anaouder
+
+[E brezhoneg](./README.md)
+
+Reconnaissance vocale pour le breton avec Vosk.
+
+Ce projet est développé bénévolement. Vous pouvez le soutenir par un don :
+[![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
+
+Une [version en ligne](https://translate.bzh/), développée par Philippe Argouarch, est également disponible.
+
+## Présentation
+
+Modèle de reconnaissance vocale (*speech-to-text*) entraîné avec le framework [Kaldi](https://www.kaldi-asr.org/), au format [Vosk](https://github.com/alphacep/vosk-api).\
+Il est accompagné de scripts permettant la retranscription automatique de fichiers audio et video, l'alignement texte/son pour la création de sous-titres, ou encore l'inférence en temps réel à l'aide d'un microphone.
+
+Principaux avantages :
+
+* **Léger**. Les modèles Vosk pèsent moins de 100 Mo et peuvent tourner sur une large gamme d'appareils : ordinateurs **sans GPU**, RaspberryPi, smartphone Android...
+* **Rapide**. L'inférence se fait en **temps réel**, même sur une machine un peu datée.
+* **Local**. Fonctionne sans connexion internet. Vos données restent donc sur votre appareil.
+* **Libre et gratuit**. La licence MIT vous permet de modifier le logiciel et de l'intégrer dans d'autres applications.
+
+Le nombre d'heures d'enregistrement audio utilisé pour entraîner le modèle est relativement faible mais progresse peu à peu.
+En dehors du projet [Common Voice](https://commonvoice.mozilla.org/br) de Mozilla, les enregistrements retranscrits [libres de droit](https://creativecommons.org/licenses/) sont rares pour le breton. Toute aide sur ce terrain sera la bienvenue !
+
+## Installation
+
+Les scripts nécessitent l'installation de [Python3](https://www.python.org/downloads/). L'installation du module de reconnaissance vocale se fera ensuite dans un terminal, en exécutant la commande suivante :
+
+```bash
+pip install anaouder
+```
+
+Une fois installé, et à mesure que de nouvelles versions du modèle de reconnaissance vocale seront proposées, vous pourrez mettre à jour le logiciel avec :
+
+```bash
+pip install --upgrade anaouder
+```
+
+
+## Retranscrire un fichier audio ou video
+
+Une fois le module installé, la commande `adskrivan` permet de retranscrire un fichier audio ou video depuis le terminal. A la première exécution de la commande, il vous faudra patienter le temps de l'installation du module `static_ffmpeg` (programme de conversion pour les fichiers audio/video). Cette installation ne se fera qu'une seule fois.
+
+```bash
+adskrivan NOM_DU_FICHIER
+```
+
+Le résultat de la transcription s'affichera dans le terminal par défaut. Vous pouvez toutefois préciser le nom d'un fichier dans lequel écrire, avec l'option `-o`
+
+```bash
+adskrivan NOM_DU_FICHIER -o SORTIE.txt
+```
+
+## Utilisation avec un microphone
+
+Depuis un terminal, invoquez la commande `mikro`.
+
+Si aucun texte n'apparaît, vous pouvez afficher la liste des interfaces audio avec la commande :
+
+```bash
+mikro -l
+```
+
+Vous pourrez ensuite préciser, en argument, le numéro de l'interface à utiliser pour l'inférence :
+
+```bash
+mikro -d NUMERO_INTERFACE
+```
+
+## Alignement d'un texte d'après un audio
+
+Il est possible d'aligner un texte d'après un fichier audio ou video à l'aide de la commande `linennan`. Vous obtiendrez un fichier contenant le texte original, accompagné de marqueurs temporels, au format `srt` (fichier de sous-titres Subrip).\
+Le fichier texte doit être un texte brut (extension `.txt`) où chaque ligne correspondra à une ligne de sous-titre.
+
+```bash
+linennan FICHIER_SON_OU_VIDEO FICHIER_TEXTE -o sous-titres.srt
+```
+
+(export au format `eaf`, pour le logiciel ELAN, à venir...)
+
+## Création automatique de sous-titres
+
+Vous pouvez également laisser le modèle de reconnaissance vocale retranscrire les paroles pour la création de sous-titres, au format `srt` (Subrip).
+
+```bash
+istitlan FICHIER_SON_OU_VIDEO
+```
+
+## Utilisation du modèle avec d'autres logiciel 
+
+*L'utilisation du modèle brut dans d'autres logiciel est possible mais n'est pas conseillé, puisque qu'elle omettra le post-traitement proposé par le module `anaouder` : le replacement des tirets de liaison et la normalisation-inverse des nombres notamment.*
+
+Le modèle brut est accessible sous le dossier `anaouder/models` ou par le lien [releases](https://github.com/gweltou/vosk-br/releases).
+
+### Audapolis
+
+Il est possible d'utiliser le modèle avec le logiciel [Audapolis](https://github.com/bugbakery/audapolis), qui offre également le confort d'une interface graphique.
+
+### Kdenlive
+
+Le logiciel de montage video [Kdenlive](https://kdenlive.org/) permet l'utilisation de modèles Vosk pour la retranscription automatique de sous-titres.\
+Voir la [documentation](https://docs.kdenlive.org/en/effects_and_compositions/speech_to_text.html).
+
+## Remerciements
+
+Le développement de cet outil a été possible grâce aux logiciels libres sur lesquels il se base : Kaldi, Vosk et le correcteur automatique [Hunspell](https://github.com/Drouizig/hunspell-br) de An Drouizig.\
+Le modèle de reconnaissance vocale n'aurait jamais pu être entraîne sans les voix et les textes de nombreux contributeurs, issus de : Mozilla Common Voice, Dizale, Brezhoweb, RKB, Kaouen.net, Ya!, Becedia, France3 et Dastum.\
+Je remercie enfin Elen Cariou, Jean-Mari Ollivier, Karen Treguier, Mélanie Jouitteau et Pêr Morvan pour leur aide et leur soutien.
```

### Comparing `anaouder-0.9.2/README-fr.md` & `anaouder-0.9.3/README-fr.md`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/README.md` & `anaouder-0.9.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,23 @@
 
 Dre ziouer, adskrivet e vo pep tra e diabarzh an terminal. Gallout a rit ivez implij an opsion `-o` evit resisaat anv ur restr, e lec'h ma vo skrivet an titouroù. Tu zo implij an option-se gant an holl urzhioù eus ar meziant.
 
 ```bash
 adskrivan RESTR_SON_PE_VIDEO -o DISOC'H.txt
 ```
 
-Evit kaout listennad an opsionoù, implijit an opsion `-h`.
+Evit kaout listennad an opsionoù, implijit an opsioñ `-h`.
+
+## Adskrivañ istitloù evit ur video
+
+Gallout a rit adskrivañ istitloù diouzh teuliadoù son pe video, e stumm `srt` (Subrip).
+
+```bash
+istitlan RESTR_SON_PE_VIDEO -o istitloù.srt
+```
 
 ## Implijout gant ur mikro
 
 Dre an an urzh `mikro` e c'heller implij an anaouder gant ho vouezh e amzer real.
 
 Ma n'ez eus skrid ebet o tont, klaskit niverenn an etrefas son gant :
 
@@ -77,26 +85,14 @@
 
 M'ho peus un teul skrid adskrivet dre dorn (e stumm `.txt`) e c'heller linennañ ar skrid gant ar son, evit krouiñ ur restr istitloù (e stumm `srt`).
 
 ```bash
 linennan RESTR_SON_PE_VIDEO RESTR_SKRID
 ```
 
-## Adskrivañ istitloù evit ur video
-
-Gallout a rit adskrivañ istitloù diouzh teuliadoù son pe video, e stumm `srt` (Subrip).
-
-```bash
-istitlan RESTR_SON_PE_VIDEO -o istitloù.srt
-```
-
-An oberiadur-se a gemero kalzig a amzer (hervez padelezh an teuliad son). Klaskit gant un teul film berr da gentañ !
-
-https://user-images.githubusercontent.com/10166907/213805292-63becbe2-ffb5-492f-9bac-1330c4b2d07d.mp4
-
 ## Implijout gant meziantoù all
 
 *N'eo ket aliet, dre ma vez kollet un nebeut perzhioù e-keñver ar pezh vez graet gant ar modul `anaouder` : adlakaat ar varennigoù-stag hag amdreiñ an niverennoù da skouer.*
 
 Ar model noazh a c'hellit kavout en dosser `anaouder/models` pe dre al liamm [releases](https://github.com/gweltou/vosk-br/releases).
 
 ### Audapolis
@@ -109,7 +105,9 @@
 Ar mod-implij a c'heller kavout [amañ](https://docs.kdenlive.org/en/effects_and_compositions/speech_to_text.html).
 
 ## Trugarez
 
 Ar meziant-se zo bet diorroet o kemer harp war meziantoù dieub all : Kaldi, Vosk ha difazier [Hunspell](https://github.com/Drouizig/hunspell-br) an Drouizig (evit naetaat an testennoù a-raok ar pleustr).\
 Lakaat da bleustriñ ar model a zo bet posubl a-drugarez d'an danvez prizius, krouet ha rannet gant ur bern tud all : ar raktres Mozilla Common Voice, enrolladennoù Dizale, Brezhoweb, RKB, Kaouen.net, Ya!, Becedia, abadennoù France3 ha Dastum.\
 Trugarez da Elen Cariou, Jean-Mari Ollivier, Karen Treguier, Mélanie Jouitteau ha Pêr Morvan evit o sikour hag o souten.
+
+https://user-images.githubusercontent.com/10166907/213805292-63becbe2-ffb5-492f-9bac-1330c4b2d07d.mp4
```

### Comparing `anaouder-0.9.2/anaouder/adskrivan.py` & `anaouder-0.9.3/anaouder/adskrivan.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
             if ext.lower() in ("srt", "seg", "eaf"):
                 args.type = ext.lower()
             else:
                 args.type = "txt"	# Default type
         else:
             args.type = "txt"
 
+    model = load_model(args.model)
+
     if args.type == "txt":
         # No need of timecodes
 
         if args.output:
             # Whole file decoding
             # Different segmentation algorithm than online decoding
             # Shows a progress bar
@@ -144,15 +146,14 @@
             ]
             sentences = [ ' '.join([token['word'] for token in seg]) for seg in token_segments ]
 
             fout.write('\n'.join(sentences))
         else:
             # Online decoding
             # Print decoded sentences one-by-one
-            model = load_model(args.model)
             rec = KaldiRecognizer(model, 16000)
             rec.SetWords(True)
         
             with subprocess.Popen([ffmpeg_path, "-loglevel", "quiet", "-i",
                                     args.filename,
                                     "-ar", "16000" , "-ac", "1", "-f", "s16le", "-"],
                                     stdout=subprocess.PIPE).stdout as stream:
@@ -168,17 +169,14 @@
                 sentence = json.loads(rec.FinalResult())["text"]
                 sentence = post_process_text(sentence, normalize=args.normalize, keep_fillers=args.keep_fillers)
                 if sentence: print(sentence, file=fout)
 
 
     elif args.type in ("srt", "seg", "eaf"):
         # Transcribe with timecodes
-
-        if args.model:
-            load_model(args.model)
         
         if args.autosplit:
             song = AudioSegment.from_file(args.filename)
             song = song.set_channels(1)
             if song.frame_rate != 16000:
                 song = song.set_frame_rate(16000)
             if song.sample_width != 2:
```

### Comparing `anaouder-0.9.2/anaouder/asr/models.py` & `anaouder-0.9.3/anaouder/asr/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     if model_name == _loaded_model_name:
         return _loaded_model
 
     if model_name in _MODELS_ALIASES:
         model_name = _MODELS_ALIASES[model_name]
 
     if download_root is None:
-        if platform.system() == "Linux":
+        if platform.system() in ("Linux", "Darwin"):
             default = os.path.join(os.path.expanduser("~"), ".cache")
         elif platform.system() == "Windows":
             default = os.getenv("LOCALAPPDATA")
         else:
             raise OSError('Unsupported operating system')
         download_root = os.path.join(os.getenv("XDG_CACHE_HOME", default), "anaouder", "models")
 
@@ -118,8 +118,8 @@
                 loop.update(len(buffer))
     
     with zipfile.ZipFile(download_target, 'r') as zip_ref:
         zip_ref.extractall(root)
 
     os.remove(download_target)
 
-    return model_path
+    return model_path
```

### Comparing `anaouder-0.9.2/anaouder/asr/post_processing.py` & `anaouder-0.9.3/anaouder/asr/post_processing.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/asr/postproc_sub.tsv` & `anaouder-0.9.3/anaouder/asr/postproc_sub.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/asr/recognizer.py` & `anaouder-0.9.3/anaouder/asr/recognizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/audio/__init__.py` & `anaouder-0.9.3/anaouder/audio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 
 
 
 def get_audiofile_length(filename):
     """
         Get audio file length in seconds
     """
-    return float(get_audiofile_info(filename)['duration'])
+    info = get_audiofile_info(filename)
+    if "duration" in info:
+        return float(info["duration"])
+    elif "tags" in info:
+        # For MKV files
+        h, m, s = info["tags"]["DURATION"].split(':')
+        return float(h) * 3600 + float(m) * 60 + float(s)
 
 
 
 def convert_to_wav(src: str, dst: str, verbose=True, keep_orig=True):
     """
         Convert to 16kHz mono pcm
         Validate filename
```

### Comparing `anaouder-0.9.2/anaouder/dicts/__init__.py` & `anaouder-0.9.3/anaouder/dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/dicts/acronyms.tsv` & `anaouder-0.9.3/anaouder/dicts/acronyms.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/dicts/corrected_tokens.tsv` & `anaouder-0.9.3/anaouder/dicts/corrected_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/dicts/noun_f.tsv` & `anaouder-0.9.3/anaouder/dicts/noun_f.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/dicts/noun_m.tsv` & `anaouder-0.9.3/anaouder/dicts/noun_m.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/dicts/proper_nouns_phon.tsv` & `anaouder-0.9.3/anaouder/dicts/proper_nouns_phon.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/dicts/standard_tokens.tsv` & `anaouder-0.9.3/anaouder/dicts/standard_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/linennan.py` & `anaouder-0.9.3/anaouder/linennan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/mikro.py` & `anaouder-0.9.3/anaouder/mikro.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/normalizan.py` & `anaouder-0.9.3/anaouder/normalizan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/text/__init__.py` & `anaouder-0.9.3/anaouder/text/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/text/definitions.py` & `anaouder-0.9.3/anaouder/text/definitions.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/text/inverse_normalizer.py` & `anaouder-0.9.3/anaouder/text/inverse_normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/text/normalizer.py` & `anaouder-0.9.3/anaouder/text/normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/text/tokenizer.py` & `anaouder-0.9.3/anaouder/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/text/utils.py` & `anaouder-0.9.3/anaouder/text/utils.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder/utils.py` & `anaouder-0.9.3/anaouder/utils.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.2/anaouder.egg-info/PKG-INFO` & `anaouder-0.9.3/anaouder.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,142 @@
 Metadata-Version: 2.1
 Name: anaouder
-Version: 0.9.2
+Version: 0.9.3
 Summary: Breton language speech-to-text tools
 Home-page: https://github.com/gweltou/vosk-br
 Author: Gweltaz Duval-Guennoc
 Author-email: gweltou@hotmail.com
 License: MIT
-Description: [![pypi version](https://img.shields.io/pypi/v/anaouder)](https://pypi.org/project/anaouder/)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
-        
-        # Anaouder
-        
-        [E brezhoneg](./README.md)
-        
-        Reconnaissance vocale pour le breton avec Vosk.
-        
-        Ce projet est développé bénévolement. Vous pouvez le soutenir par un don :
-        [![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
-        
-        Une [version en ligne](https://translate.bzh/), développée par Philippe Argouarch, est également disponible.
-        
-        ## Présentation
-        
-        Modèle de reconnaissance vocale (*speech-to-text*) entraîné avec le framework [Kaldi](https://www.kaldi-asr.org/), au format [Vosk](https://github.com/alphacep/vosk-api).\
-        Il est accompagné de scripts permettant la retranscription automatique de fichiers audio et video, l'alignement texte/son pour la création de sous-titres, ou encore l'inférence en temps réel à l'aide d'un microphone.
-        
-        Principaux avantages :
-        
-        * **Léger**. Les modèles Vosk pèsent moins de 100 Mo et peuvent tourner sur une large gamme d'appareils : ordinateurs **sans GPU**, RaspberryPi, smartphone Android...
-        * **Rapide**. L'inférence se fait en **temps réel**, même sur une machine un peu datée.
-        * **Local**. Fonctionne sans connexion internet. Vos données restent donc sur votre appareil.
-        * **Libre et gratuit**. La licence MIT vous permet de modifier le logiciel et de l'intégrer dans d'autres applications.
-        
-        Le nombre d'heures d'enregistrement audio utilisé pour entraîner le modèle est relativement faible mais progresse peu à peu.
-        En dehors du projet [Common Voice](https://commonvoice.mozilla.org/br) de Mozilla, les enregistrements retranscrits [libres de droit](https://creativecommons.org/licenses/) sont rares pour le breton. Toute aide sur ce terrain sera la bienvenue !
-        
-        ## Installation
-        
-        Les scripts nécessitent l'installation de [Python3](https://www.python.org/downloads/). L'installation du module de reconnaissance vocale se fera ensuite dans un terminal, en exécutant la commande suivante :
-        
-        ```bash
-        pip install anaouder
-        ```
-        
-        Une fois installé, et à mesure que de nouvelles versions du modèle de reconnaissance vocale seront proposées, vous pourrez mettre à jour le logiciel avec :
-        
-        ```bash
-        pip install --upgrade anaouder
-        ```
-        
-        
-        ## Retranscrire un fichier audio ou video
-        
-        Une fois le module installé, la commande `adskrivan` permet de retranscrire un fichier audio ou video depuis le terminal. A la première exécution de la commande, il vous faudra patienter le temps de l'installation du module `static_ffmpeg` (programme de conversion pour les fichiers audio/video). Cette installation ne se fera qu'une seule fois.
-        
-        ```bash
-        adskrivan NOM_DU_FICHIER
-        ```
-        
-        Le résultat de la transcription s'affichera dans le terminal par défaut. Vous pouvez toutefois préciser le nom d'un fichier dans lequel écrire, avec l'option `-o`
-        
-        ```bash
-        adskrivan NOM_DU_FICHIER -o SORTIE.txt
-        ```
-        
-        ## Utilisation avec un microphone
-        
-        Depuis un terminal, invoquez la commande `mikro`.
-        
-        Si aucun texte n'apparaît, vous pouvez afficher la liste des interfaces audio avec la commande :
-        
-        ```bash
-        mikro -l
-        ```
-        
-        Vous pourrez ensuite préciser, en argument, le numéro de l'interface à utiliser pour l'inférence :
-        
-        ```bash
-        mikro -d NUMERO_INTERFACE
-        ```
-        
-        ## Alignement d'un texte d'après un audio
-        
-        Il est possible d'aligner un texte d'après un fichier audio ou video à l'aide de la commande `linennan`. Vous obtiendrez un fichier contenant le texte original, accompagné de marqueurs temporels, au format `srt` (fichier de sous-titres Subrip).\
-        Le fichier texte doit être un texte brut (extension `.txt`) où chaque ligne correspondra à une ligne de sous-titre.
-        
-        ```bash
-        linennan FICHIER_SON_OU_VIDEO FICHIER_TEXTE -o sous-titres.srt
-        ```
-        
-        (export au format `eaf`, pour le logiciel ELAN, à venir...)
-        
-        ## Création automatique de sous-titres
-        
-        Vous pouvez également laisser le modèle de reconnaissance vocale retranscrire les paroles pour la création de sous-titres, au format `srt` (Subrip).
-        
-        ```bash
-        istitlan FICHIER_SON_OU_VIDEO
-        ```
-        
-        ## Utilisation du modèle avec d'autres logiciel 
-        
-        *L'utilisation du modèle brut dans d'autres logiciel est possible mais n'est pas conseillé, puisque qu'elle omettra le post-traitement proposé par le module `anaouder` : le replacement des tirets de liaison et la normalisation-inverse des nombres notamment.*
-        
-        Le modèle brut est accessible sous le dossier `anaouder/models` ou par le lien [releases](https://github.com/gweltou/vosk-br/releases).
-        
-        ### Audapolis
-        
-        Il est possible d'utiliser le modèle avec le logiciel [Audapolis](https://github.com/bugbakery/audapolis), qui offre également le confort d'une interface graphique.
-        
-        ### Kdenlive
-        
-        Le logiciel de montage video [Kdenlive](https://kdenlive.org/) permet l'utilisation de modèles Vosk pour la retranscription automatique de sous-titres.\
-        Voir la [documentation](https://docs.kdenlive.org/en/effects_and_compositions/speech_to_text.html).
-        
-        ## Remerciements
-        
-        Le développement de cet outil a été possible grâce aux logiciels libres sur lesquels il se base : Kaldi, Vosk et le correcteur automatique [Hunspell](https://github.com/Drouizig/hunspell-br) de An Drouizig.\
-        Le modèle de reconnaissance vocale n'aurait jamais pu être entraîne sans les voix et les textes de nombreux contributeurs, issus de : Mozilla Common Voice, Dizale, Brezhoweb, RKB, Kaouen.net, Ya!, Becedia, France3 et Dastum.\
-        Je remercie enfin Elen Cariou, Jean-Mari Ollivier, Karen Treguier, Mélanie Jouitteau et Pêr Morvan pour leur aide et leur soutien.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: static_ffmpeg
+Requires-Dist: sounddevice
+Requires-Dist: vosk
+Requires-Dist: srt
+Requires-Dist: jiwer
+Requires-Dist: pydub>=0.25.1
+Requires-Dist: pytz
+Requires-Dist: tqdm==4.64.1
+
+[![pypi version](https://img.shields.io/pypi/v/anaouder)](https://pypi.org/project/anaouder/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
+
+# Anaouder
+
+[E brezhoneg](./README.md)
+
+Reconnaissance vocale pour le breton avec Vosk.
+
+Ce projet est développé bénévolement. Vous pouvez le soutenir par un don :
+[![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
+
+Une [version en ligne](https://translate.bzh/), développée par Philippe Argouarch, est également disponible.
+
+## Présentation
+
+Modèle de reconnaissance vocale (*speech-to-text*) entraîné avec le framework [Kaldi](https://www.kaldi-asr.org/), au format [Vosk](https://github.com/alphacep/vosk-api).\
+Il est accompagné de scripts permettant la retranscription automatique de fichiers audio et video, l'alignement texte/son pour la création de sous-titres, ou encore l'inférence en temps réel à l'aide d'un microphone.
+
+Principaux avantages :
+
+* **Léger**. Les modèles Vosk pèsent moins de 100 Mo et peuvent tourner sur une large gamme d'appareils : ordinateurs **sans GPU**, RaspberryPi, smartphone Android...
+* **Rapide**. L'inférence se fait en **temps réel**, même sur une machine un peu datée.
+* **Local**. Fonctionne sans connexion internet. Vos données restent donc sur votre appareil.
+* **Libre et gratuit**. La licence MIT vous permet de modifier le logiciel et de l'intégrer dans d'autres applications.
+
+Le nombre d'heures d'enregistrement audio utilisé pour entraîner le modèle est relativement faible mais progresse peu à peu.
+En dehors du projet [Common Voice](https://commonvoice.mozilla.org/br) de Mozilla, les enregistrements retranscrits [libres de droit](https://creativecommons.org/licenses/) sont rares pour le breton. Toute aide sur ce terrain sera la bienvenue !
+
+## Installation
+
+Les scripts nécessitent l'installation de [Python3](https://www.python.org/downloads/). L'installation du module de reconnaissance vocale se fera ensuite dans un terminal, en exécutant la commande suivante :
+
+```bash
+pip install anaouder
+```
+
+Une fois installé, et à mesure que de nouvelles versions du modèle de reconnaissance vocale seront proposées, vous pourrez mettre à jour le logiciel avec :
+
+```bash
+pip install --upgrade anaouder
+```
+
+
+## Retranscrire un fichier audio ou video
+
+Une fois le module installé, la commande `adskrivan` permet de retranscrire un fichier audio ou video depuis le terminal. A la première exécution de la commande, il vous faudra patienter le temps de l'installation du module `static_ffmpeg` (programme de conversion pour les fichiers audio/video). Cette installation ne se fera qu'une seule fois.
+
+```bash
+adskrivan NOM_DU_FICHIER
+```
+
+Le résultat de la transcription s'affichera dans le terminal par défaut. Vous pouvez toutefois préciser le nom d'un fichier dans lequel écrire, avec l'option `-o`
+
+```bash
+adskrivan NOM_DU_FICHIER -o SORTIE.txt
+```
+
+## Utilisation avec un microphone
+
+Depuis un terminal, invoquez la commande `mikro`.
+
+Si aucun texte n'apparaît, vous pouvez afficher la liste des interfaces audio avec la commande :
+
+```bash
+mikro -l
+```
+
+Vous pourrez ensuite préciser, en argument, le numéro de l'interface à utiliser pour l'inférence :
+
+```bash
+mikro -d NUMERO_INTERFACE
+```
+
+## Alignement d'un texte d'après un audio
+
+Il est possible d'aligner un texte d'après un fichier audio ou video à l'aide de la commande `linennan`. Vous obtiendrez un fichier contenant le texte original, accompagné de marqueurs temporels, au format `srt` (fichier de sous-titres Subrip).\
+Le fichier texte doit être un texte brut (extension `.txt`) où chaque ligne correspondra à une ligne de sous-titre.
+
+```bash
+linennan FICHIER_SON_OU_VIDEO FICHIER_TEXTE -o sous-titres.srt
+```
+
+(export au format `eaf`, pour le logiciel ELAN, à venir...)
+
+## Création automatique de sous-titres
+
+Vous pouvez également laisser le modèle de reconnaissance vocale retranscrire les paroles pour la création de sous-titres, au format `srt` (Subrip).
+
+```bash
+istitlan FICHIER_SON_OU_VIDEO
+```
+
+## Utilisation du modèle avec d'autres logiciel 
+
+*L'utilisation du modèle brut dans d'autres logiciel est possible mais n'est pas conseillé, puisque qu'elle omettra le post-traitement proposé par le module `anaouder` : le replacement des tirets de liaison et la normalisation-inverse des nombres notamment.*
+
+Le modèle brut est accessible sous le dossier `anaouder/models` ou par le lien [releases](https://github.com/gweltou/vosk-br/releases).
+
+### Audapolis
+
+Il est possible d'utiliser le modèle avec le logiciel [Audapolis](https://github.com/bugbakery/audapolis), qui offre également le confort d'une interface graphique.
+
+### Kdenlive
+
+Le logiciel de montage video [Kdenlive](https://kdenlive.org/) permet l'utilisation de modèles Vosk pour la retranscription automatique de sous-titres.\
+Voir la [documentation](https://docs.kdenlive.org/en/effects_and_compositions/speech_to_text.html).
+
+## Remerciements
+
+Le développement de cet outil a été possible grâce aux logiciels libres sur lesquels il se base : Kaldi, Vosk et le correcteur automatique [Hunspell](https://github.com/Drouizig/hunspell-br) de An Drouizig.\
+Le modèle de reconnaissance vocale n'aurait jamais pu être entraîne sans les voix et les textes de nombreux contributeurs, issus de : Mozilla Common Voice, Dizale, Brezhoweb, RKB, Kaouen.net, Ya!, Becedia, France3 et Dastum.\
+Je remercie enfin Elen Cariou, Jean-Mari Ollivier, Karen Treguier, Mélanie Jouitteau et Pêr Morvan pour leur aide et leur soutien.
```

### Comparing `anaouder-0.9.2/anaouder.egg-info/SOURCES.txt` & `anaouder-0.9.3/anaouder.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+LICENSE
 README-fr.md
 README.md
 setup.py
 anaouder/__init__.py
 anaouder/adskrivan.py
 anaouder/istitlan.py
 anaouder/linennan.py
```

### Comparing `anaouder-0.9.2/setup.py` & `anaouder-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 setup(
     name=NAME,
     url=URL,
     version=VERSION,
     author=AUTHOR,
-    licence="MIT",
+    license="MIT",
     author_email=EMAIL,
     description=DESCRIPTION,
     long_description=open("README-fr.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     python_requires=REQUIRES_PYTHON,
     install_requires=REQUIREMENTS,
     classifiers=[
```

