# Comparing `tmp/audalign-1.2.4.tar.gz` & `tmp/audalign-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audalign-1.2.4.tar", last modified: Mon Jan  8 04:51:17 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `audalign-1.2.4.tar` & `audalign-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.966697 audalign-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-08 04:51:07.000000 audalign-1.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-01-08 04:51:17.966697 audalign-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-01-08 04:51:07.000000 audalign-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.962697 audalign-1.2.4/audalign/
--rw-r--r--   0 runner    (1001) docker     (127)    34505 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.962697 audalign-1.2.4/audalign/align/
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/align/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.962697 audalign-1.2.4/audalign/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/config/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/config/correlation_spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/config/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/config/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/datalign.py
--rw-r--r--   0 runner    (1001) docker     (127)    27519 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/filehandler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.962697 audalign-1.2.4/audalign/recognizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.966697 audalign-1.2.4/audalign/recognizers/correcognize/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/correcognize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/correcognize/correcognize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.966697 audalign-1.2.4/audalign/recognizers/correcognizeSpectrogram/
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/correcognizeSpectrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22722 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.966697 audalign-1.2.4/audalign/recognizers/fingerprint/
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/fingerprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/fingerprint/fingerprinter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15345 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/fingerprint/recognize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.966697 audalign-1.2.4/audalign/recognizers/visrecognize/
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/visrecognize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19646 2024-01-08 04:51:07.000000 audalign-1.2.4/audalign/recognizers/visrecognize/visrecognize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.966697 audalign-1.2.4/audalign.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-01-08 04:51:17.000000 audalign-1.2.4/audalign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-01-08 04:51:17.000000 audalign-1.2.4/audalign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 04:51:17.000000 audalign-1.2.4/audalign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-08 04:51:17.000000 audalign-1.2.4/audalign.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-08 04:51:17.000000 audalign-1.2.4/audalign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 04:51:17.966697 audalign-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-01-08 04:51:07.000000 audalign-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:17.966697 audalign-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 04:51:07.000000 audalign-1.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-01-08 04:51:07.000000 audalign-1.2.4/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-01-08 04:51:07.000000 audalign-1.2.4/tests/test_audalign.py
--rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-01-08 04:51:07.000000 audalign-1.2.4/tests/test_recognize.py
+-rw-r--r--   0        0        0    34505 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/datalign.py
+-rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/filehandler.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/align/__init__.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/config/__init__.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/config/correlation.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/config/correlation_spectrogram.py
+-rw-r--r--   0        0        0     7227 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/config/fingerprint.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/config/visual.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/__init__.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/correcognize/__init__.py
+-rw-r--r--   0        0        0    22006 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/correcognize/correcognize.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/correcognizeSpectrogram/__init__.py
+-rw-r--r--   0        0        0    22722 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py
+-rw-r--r--   0        0        0    15555 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/fingerprint/__init__.py
+-rw-r--r--   0        0        0    13400 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/fingerprint/fingerprinter.py
+-rw-r--r--   0        0        0    15345 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/fingerprint/recognize.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/visrecognize/__init__.py
+-rw-r--r--   0        0        0    19713 2020-02-02 00:00:00.000000 audalign-1.3.0/audalign/recognizers/visrecognize/visrecognize.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 audalign-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 audalign-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 audalign-1.3.0/README.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 audalign-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 audalign-1.3.0/PKG-INFO
```

### Comparing `audalign-1.2.4/LICENSE.md` & `audalign-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/PKG-INFO` & `audalign-1.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,279 +1,223 @@
-Metadata-Version: 2.1
-Name: audalign
-Version: 1.2.4
-Summary: Audio Alignment and Recognition in Python
-Home-page: http://github.com/benfmiller/audalign
-Author: Ben Miller
-Author-email: benfmiller132@gmail.com
-Maintainer: Ben Miller
-Maintainer-email: benfmiller132@gmail.com
-License: MIT
-Keywords: python,audio,align,alignment,fingerprinting,music
-Platform: Unix
-Platform: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: appdirs==1.4.4
-Requires-Dist: attrs==22.2.0
-Requires-Dist: audioread==3.0.0
-Requires-Dist: certifi==2022.12.7
-Requires-Dist: cffi==1.15.1
-Requires-Dist: charset-normalizer==2.1.1
-Requires-Dist: contourpy==1.0.6
-Requires-Dist: cycler==0.11.0
-Requires-Dist: decorator==5.1.1
-Requires-Dist: exceptiongroup==1.1.0
-Requires-Dist: execnet==1.9.0
-Requires-Dist: fonttools==4.38.0
-Requires-Dist: idna==3.4
-Requires-Dist: imageio==2.23.0
-Requires-Dist: iniconfig==2.0.0
-Requires-Dist: joblib==1.2.0
-Requires-Dist: kiwisolver==1.4.4
-Requires-Dist: librosa==0.10.1
-Requires-Dist: llvmlite==0.41.1
-Requires-Dist: matplotlib==3.6.2
-Requires-Dist: networkx==3.0
-Requires-Dist: noisereduce==2.0.1
-Requires-Dist: numba==0.58.1
-Requires-Dist: numpy==1.26.2
-Requires-Dist: packaging==23.0
-Requires-Dist: Pillow==9.4.0
-Requires-Dist: pluggy==1.0.0
-Requires-Dist: pooch==1.6.0
-Requires-Dist: pycparser==2.21
-Requires-Dist: pydub==0.25.1
-Requires-Dist: pyparsing==3.1.1
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: PyWavelets==1.4.1
-Requires-Dist: requests==2.28.1
-Requires-Dist: resampy==0.4.2
-Requires-Dist: scikit-image==0.19.3
-Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scipy==1.11.4
-Requires-Dist: six==1.16.0
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: threadpoolctl==3.1.0
-Requires-Dist: tifffile==2022.10.10
-Requires-Dist: tomli==2.0.1
-Requires-Dist: tqdm==4.64.1
-Requires-Dist: urllib3==1.26.13
-
-# Audalign
-
-Package for processing and aligning audio files using audio fingerprinting, cross-correlation, cross-correlation with spectrograms, or visual alignment techniques.
-
-![gif of audalign aligning](audalign.gif)
-
-This package offers tools to align many recordings of the same event. It has two main purposes: to accurately align recordings, and to process the audio files prior to alignments. All main functions are accessed through functions in the audalign.\_\_init\_\_ file. The recognizers themselves are objects in the recognizer directory which in turn have configurations in the config directories.
-
- Alignments are primarily accomplished with fingerprinting, though where fingerprinting fails, correlation, correlation with spectrograms, and visual alignment techniques can be used to get a closer result. After an initial alignment is found, that alignment can be passed to "fine_align," which will find smaller, relative alignments to the main one.
-
----
-
-Each alignment technique has different degrees of adjustment for accuracy settings. Fingerprinting parameters can be generally set to get consistent results using it's config's `set_accuracy` method. Visual alignment has many parameters that can be adjusted and requires case by case adjustment. Parameters for correlation are focused on sample rate or scipy's find_peaks.
-
-[Noisereduce](https://timsainburg.com/noise-reduction-python.html) is very useful for this application and a wrapper is implemented for ease of use. Uniformly leveling prior to noise reduction using uniform_level_file boosts quiet but important sound features.
-
-Alignment and recognition results consist of a dictionary. If an output directory is given, silence is placed before all target files so that they will automatically be aligned and writen to the output directory along with an audio file containing the combined sum. A `rankings` key is included in each alignment and recognition result. This helps determine the strength of the alignment, but is not definitive proof. Values range from 1-10.
-
----
-
-All formats that ffmpeg or libav support are supported here.
-
-All fingerprints are stored in memory in the `FingerprintRecognzier` and must be saved to disk with the `save_fingerprinted_files` method in order to persist them.
-
-Regular file recogniton can also be done with Audalign similar to [dejavu](https://github.com/worldveil/dejavu).
-
-For more details on implementation and results, see the [wiki!!](https://github.com/benfmiller/audalign/wiki)
-
-## Installation
-
-Install from PyPI:
-
-Don't forget to install ffmpeg/avlib (Below in the Readme)!
-
-```bash
-pip install audalign
-```
-
-OR
-
-```bash
-git clone https://github.com/benfmiller/audalign.git
-cd audalign/
-pip install audalign
-```
-
-OR
-
-Download and extract audalign then
-
-```bash
-pip install audalign
-```
-
-in the directory
-
-## Recognizers
-
-There are currently four included recognizers, each with their own config objects.
-
-```python
-import audalign as ad
-
-fingerprint_rec = ad.FingerprintRecognizer()
-correlation_rec = ad.CorrelationRecognizer()
-cor_spec_rec = ad.CorrelationSpectrogramRecognizer()
-visual_rec = ad.VisualRecognizer()
-
-fingerprint_rec.config.set_accuracy(3)
-# recognizer.config.some_item
-```
-
-For more info about the configuration objects, check out the [wiki](https://github.com/benfmiller/audalign/wiki) or the config objects themselves. They are relatively nicely commented.
-
-Recognizers are then passed to recognize and align functions.
-
-```python
-results = ad.align("target/folder/", recognizer=fingerprint_rec)
-results = ad.align("target/folder/", recognizer=correlation_rec)
-results = ad.align("target/folder/", recognizer=cor_spec_rec)
-results = ad.align("target/folder/", recognizer=visual_rec)
-results = ad.recognize("target/file1", "target/file2", recognizer=fingerprint_rec)
-results = ad.recognize("target/file1", "target/folder", recognizer=fingerprint_rec)
-# or
-results = ad.target_align(
-    "target/files",
-    "target/folder/",
-    destination_path="write/alignments/to/folder",
-    recognizer=fingerprint_rec
-)
-# or
-results = ad.align_files(
-    "target/file1",
-    "target/file2",
-    destination_path="write/alignments/to/folder",
-    recognizer=correlation_rec
-)
-
-# results can then be sent to fine_align
-fine_results = ad.fine_align(
-    results,
-    recognizer=cor_spec_rec,
-)
-```
-
-Correlation is more precise than fingerprints and will always give a best alignment unlike fingerprinting, which can return no alignment. `max_lags` is very important for fine aligning. `locality` can be very useful for all alignments and recognitions.
-
-## Other Functions
-
-```python
-# wrapper for timsainb/noisereduce
-ad.remove_noise_file(
-    "target/file",
-    "5", # noise start in seconds
-    "20", # noise end in seconds
-    "destination/file",
-    alt_noise_filepath="different/sound/file",
-    prop_decrease="0.5", # If you want noise half reduced
-)
-
-ad.remove_noise_directory(
-    "target/directory/",
-    "noise/file",
-    "5", # noise start in seconds
-    "20", # noise end in seconds
-    "destination/directory",
-    prop_decrease="0.5", # If you want noise half reduced
-)
-
-ad.uniform_level_file(
-    "target/file",
-    "destination",
-    mode="normalize",
-    width=5,
-)
-
-ad.plot("file.wav") # Plots spectrogram with peaks overlaid
-ad.convert_audio_file("audio.wav", "audio.mp3") # Also convert video file to audio file
-ad.get_metadata("file.wav") # Returns metadata from ffmpeg/ avlib
-```
-
-You can easily recalcute the alignment shifts from previous results using recalc_shifts.
-You can then write those shifts using write_shifts_from_results. write_shifts_from_results also
-lets you use different source files for alignments too.
-
-```python
-recalculated_results = ad.recalc_shifts(older_results)
-ad.write_shifts_from_results(recalculated_results, "destination", "source_files_folder_or_file_list")
-```
-
-## Fingerprinting
-
-Fingerprinting is only used in the FingerprintRecognizer object. Alignments are not independent, so fingerprints created before alignments will be used for the alignment. The exception of this is in fine_aligning, where new fingerprints are always created.
-
-Running recognitions will fingerprint all files in the recognitions not already fingerprinted.
-
-```python
-fingerprint_rec = ad.FingerprintRecognizer()
-
-fingerprint_rec.fingerprint_file("test_file.wav")
-
-# or
-
-fingerprint_rec.fingerprint_directory("audio/directory")
-```
-
-fingerprints are stored in fingerprint_rec and can be saved by
-
-```python
-fingerprint_rec.save_fingerprinted_files("save_file.json") # or .pickle
-# or loaded with
-fingerprint_rec.load_fingerprinted_files("save_file.json") # or .pickle
-```
-
-## Resources and Tools
-
-For more tools to align audio and video files, see [forart/HyMPS's collection of alignment resources.](https://github.com/forart/HyMPS/blob/main/A_Tools.md#alignmentsynch-)
-
-[forart/HyMPS](https://github.com/forart/HyMPS/tree/main) also has many other audio/video resources.
-
-
-## Getting ffmpeg set up
-
-You can use **ffmpeg or libav**.
-
-Mac (using [homebrew](http://brew.sh)):
-
-```bash
-# ffmpeg
-brew install ffmpeg --with-libvorbis --with-sdl2 --with-theora
-
-####    OR    #####
-
-# libav
-brew install libav --with-libvorbis --with-sdl --with-theora
-```
-
-Linux (using apt):
-
-```bash
-# ffmpeg
-apt-get install ffmpeg libavcodec-extra
-
-####    OR    #####
-
-# libav
-apt-get install libav-tools libavcodec-extra
-```
-
-Windows:
-
-1. Download and extract ffmpeg from [Windows binaries provided here](https://ffmpeg.org/download.html).
-2. Add the ffmpeg `/bin` folder to your PATH environment variable
-
-OR
-
-1. Download and extract libav from [Windows binaries provided here](http://builds.libav.org/windows/).
-2. Add the libav `/bin` folder to your PATH environment variable
+# Audalign
+
+Package for processing and aligning audio files using audio fingerprinting, cross-correlation, cross-correlation with spectrograms, or visual alignment techniques.
+
+![gif of audalign aligning](audalign.gif)
+
+This package offers tools to align many recordings of the same event. It has two main purposes: to accurately align recordings, and to process the audio files prior to alignments. All main functions are accessed through functions in the audalign.\_\_init\_\_ file. The recognizers themselves are objects in the recognizer directory which in turn have configurations in the config directories.
+
+ Alignments are primarily accomplished with fingerprinting, though where fingerprinting fails, correlation, correlation with spectrograms, and visual alignment techniques can be used to get a closer result. After an initial alignment is found, that alignment can be passed to "fine_align," which will find smaller, relative alignments to the main one.
+
+---
+
+Each alignment technique has different degrees of adjustment for accuracy settings. Fingerprinting parameters can be generally set to get consistent results using it's config's `set_accuracy` method. Visual alignment has many parameters that can be adjusted and requires case by case adjustment. Parameters for correlation are focused on sample rate or scipy's find_peaks.
+
+[Noisereduce](https://timsainburg.com/noise-reduction-python.html) is very useful for this application and a wrapper is implemented for ease of use. Uniformly leveling prior to noise reduction using uniform_level_file boosts quiet but important sound features.
+
+Alignment and recognition results consist of a dictionary. If an output directory is given, silence is placed before all target files so that they will automatically be aligned and writen to the output directory along with an audio file containing the combined sum. A `rankings` key is included in each alignment and recognition result. This helps determine the strength of the alignment, but is not definitive proof. Values range from 1-10.
+
+---
+
+All formats that ffmpeg or libav support are supported here.
+
+All fingerprints are stored in memory in the `FingerprintRecognzier` and must be saved to disk with the `save_fingerprinted_files` method in order to persist them.
+
+Regular file recogniton can also be done with Audalign similar to [dejavu](https://github.com/worldveil/dejavu).
+
+For more details on implementation and results, see the [wiki!!](https://github.com/benfmiller/audalign/wiki)
+
+## Installation
+
+Install from PyPI:
+
+Don't forget to install ffmpeg/avlib (Below in the Readme)!
+
+```bash
+pip install audalign
+```
+
+OR
+
+```bash
+git clone https://github.com/benfmiller/audalign.git
+cd audalign/
+pip install audalign
+```
+
+OR
+
+Download and extract audalign then
+
+```bash
+pip install audalign
+```
+
+in the directory
+
+### Optional dependencies
+
+- visrecognize: additional recognizer based on spectrogram image comparison. `pip install audalign[visrecognize]`
+- noisereduce: wrapper utils around [timsainb/noisereduce](https://github.com/timsainb/noisereduce). `pip install audalign[noisereduce]`
+
+## Recognizers
+
+There are currently four included recognizers, each with their own config objects.
+
+```python
+import audalign as ad
+
+fingerprint_rec = ad.FingerprintRecognizer()
+correlation_rec = ad.CorrelationRecognizer()
+cor_spec_rec = ad.CorrelationSpectrogramRecognizer()
+visual_rec = ad.VisualRecognizer() # requires installting optional visrecognize dependencies
+
+fingerprint_rec.config.set_accuracy(3)
+# recognizer.config.some_item
+```
+
+For more info about the configuration objects, check out the [wiki](https://github.com/benfmiller/audalign/wiki) or the config objects themselves. They are relatively nicely commented.
+
+Recognizers are then passed to recognize and align functions.
+
+```python
+results = ad.align("target/folder/", recognizer=fingerprint_rec)
+results = ad.align("target/folder/", recognizer=correlation_rec)
+results = ad.align("target/folder/", recognizer=cor_spec_rec)
+results = ad.align("target/folder/", recognizer=visual_rec)
+results = ad.recognize("target/file1", "target/file2", recognizer=fingerprint_rec)
+results = ad.recognize("target/file1", "target/folder", recognizer=fingerprint_rec)
+# or
+results = ad.target_align(
+    "target/files",
+    "target/folder/",
+    destination_path="write/alignments/to/folder",
+    recognizer=fingerprint_rec
+)
+# or
+results = ad.align_files(
+    "target/file1",
+    "target/file2",
+    destination_path="write/alignments/to/folder",
+    recognizer=correlation_rec
+)
+
+# results can then be sent to fine_align
+fine_results = ad.fine_align(
+    results,
+    recognizer=cor_spec_rec,
+)
+```
+
+Correlation is more precise than fingerprints and will always give a best alignment unlike fingerprinting, which can return no alignment. `max_lags` is very important for fine aligning. `locality` can be very useful for all alignments and recognitions.
+
+## Other Functions
+
+```python
+# wrapper for timsainb/noisereduce, optional dependency
+ad.remove_noise_file(
+    "target/file",
+    "5", # noise start in seconds
+    "20", # noise end in seconds
+    "destination/file",
+    alt_noise_filepath="different/sound/file",
+    prop_decrease="0.5", # If you want noise half reduced
+)
+
+ad.remove_noise_directory(
+    "target/directory/",
+    "noise/file",
+    "5", # noise start in seconds
+    "20", # noise end in seconds
+    "destination/directory",
+    prop_decrease="0.5", # If you want noise half reduced
+)
+
+ad.uniform_level_file(
+    "target/file",
+    "destination",
+    mode="normalize",
+    width=5,
+)
+
+ad.plot("file.wav") # Plots spectrogram with peaks overlaid
+ad.convert_audio_file("audio.wav", "audio.mp3") # Also convert video file to audio file
+ad.get_metadata("file.wav") # Returns metadata from ffmpeg/ avlib
+```
+
+You can easily recalcute the alignment shifts from previous results using recalc_shifts.
+You can then write those shifts using write_shifts_from_results. write_shifts_from_results also
+lets you use different source files for alignments too.
+
+```python
+recalculated_results = ad.recalc_shifts(older_results)
+ad.write_shifts_from_results(recalculated_results, "destination", "source_files_folder_or_file_list")
+```
+
+## Fingerprinting
+
+Fingerprinting is only used in the FingerprintRecognizer object. Alignments are not independent, so fingerprints created before alignments will be used for the alignment. The exception of this is in fine_aligning, where new fingerprints are always created.
+
+Running recognitions will fingerprint all files in the recognitions not already fingerprinted.
+
+```python
+fingerprint_rec = ad.FingerprintRecognizer()
+
+fingerprint_rec.fingerprint_file("test_file.wav")
+
+# or
+
+fingerprint_rec.fingerprint_directory("audio/directory")
+```
+
+fingerprints are stored in fingerprint_rec and can be saved by
+
+```python
+fingerprint_rec.save_fingerprinted_files("save_file.json") # or .pickle
+# or loaded with
+fingerprint_rec.load_fingerprinted_files("save_file.json") # or .pickle
+```
+
+## Resources and Tools
+
+For more tools to align audio and video files, see [forart/HyMPS's collection of alignment resources.](https://github.com/forart/HyMPS/blob/main/A_Tools.md#alignmentsynch-)
+
+[forart/HyMPS](https://github.com/forart/HyMPS/tree/main) also has many other audio/video resources.
+
+
+## Getting ffmpeg set up
+
+You can use **ffmpeg or libav**.
+
+Mac (using [homebrew](http://brew.sh)):
+
+```bash
+# ffmpeg
+brew install ffmpeg --with-libvorbis --with-sdl2 --with-theora
+
+####    OR    #####
+
+# libav
+brew install libav --with-libvorbis --with-sdl --with-theora
+```
+
+Linux (using apt):
+
+```bash
+# ffmpeg
+apt-get install ffmpeg libavcodec-extra
+
+####    OR    #####
+
+# libav
+apt-get install libav-tools libavcodec-extra
+```
+
+Windows:
+
+1. Download and extract ffmpeg from [Windows binaries provided here](https://ffmpeg.org/download.html).
+2. Add the ffmpeg `/bin` folder to your PATH environment variable
+
+OR
+
+1. Download and extract libav from [Windows binaries provided here](http://builds.libav.org/windows/).
+2. Add the libav `/bin` folder to your PATH environment variable
```

### Comparing `audalign-1.2.4/audalign/__init__.py` & `audalign-1.3.0/audalign/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/align/__init__.py` & `audalign-1.3.0/audalign/align/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/config/__init__.py` & `audalign-1.3.0/audalign/config/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/config/correlation.py` & `audalign-1.3.0/audalign/config/correlation.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/config/correlation_spectrogram.py` & `audalign-1.3.0/audalign/config/correlation_spectrogram.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/config/fingerprint.py` & `audalign-1.3.0/audalign/config/fingerprint.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/config/visual.py` & `audalign-1.3.0/audalign/config/visual.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/datalign.py` & `audalign-1.3.0/audalign/datalign.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/filehandler.py` & `audalign-1.3.0/audalign/filehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import fnmatch
 import math
 import multiprocessing
 import os
 import typing
 from functools import partial
+from functools import wraps
 
-import noisereduce
 import numpy as np
 from numpy.core.defchararray import array
 from pydub import AudioSegment, effects
 from pydub.exceptions import CouldntDecodeError
 
 from audalign.config import BaseConfig
 
+try:
+    import noisereduce
+except ImportError:
+    # Optional dependency
+    ...
+
+
 cant_write_ext = [".mov", ".mp4", ".m4a"]
 cant_read_ext = [".txt", ".md", ".pkf", ".py", ".pyc"]
 can_read_ext = [
     ".mov",
     ".mp4",
     ".m4a",
     ".wav",
@@ -26,14 +33,26 @@
     ".ogg",
     ".aiff",
     ".aac",
     ".wma",
     ".flac",
 ]
 
+def _import_optional_dependencies(func):
+    @wraps(func)
+    def wrapper_decorator(*args, **kwargs):
+        try:
+            import noisereduce
+        except ImportError:
+            raise ImportError("skimage not found, please install 'visrecognize' module")
+        results = func(*args, **kwargs)
+        return results
+
+    return wrapper_decorator
+
 
 def find_files(path, extensions=["*"]):
     """
     Yields all files with given extension in path and all subdirectories
 
     Args
         path (str): path to folder
@@ -188,14 +207,15 @@
 
 def _int16ify_data(data: array):
     data[np.where(data < 0)] *= 32768
     data[np.where(data > 0)] *= 32767
     return data.astype(np.int16)
 
 
+@_import_optional_dependencies
 def noise_remove(
     filepath,
     noise_start,
     noise_end,
     destination,
     write_extension: str = None,
     alt_noise_filepath=None,
@@ -292,14 +312,15 @@
             pool.close()
             pool.join()
     else:
         for i in file_names:
             _reduce_noise(i)
 
 
+@_import_optional_dependencies
 def _remove_noise(
     file_path,
     noise_section=[],
     write_extension: str = None,
     destination_directory="",
     prop_decrease=1,
     **kwargs,
```

### Comparing `audalign-1.2.4/audalign/recognizers/__init__.py` & `audalign-1.3.0/audalign/recognizers/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/correcognize/__init__.py` & `audalign-1.3.0/audalign/recognizers/correcognize/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/correcognize/correcognize.py` & `audalign-1.3.0/audalign/recognizers/correcognize/correcognize.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/correcognizeSpectrogram/__init__.py` & `audalign-1.3.0/audalign/recognizers/correcognizeSpectrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py` & `audalign-1.3.0/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/fingerprint/__init__.py` & `audalign-1.3.0/audalign/recognizers/fingerprint/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/fingerprint/fingerprinter.py` & `audalign-1.3.0/audalign/recognizers/fingerprint/fingerprinter.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/fingerprint/recognize.py` & `audalign-1.3.0/audalign/recognizers/fingerprint/recognize.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.4/audalign/recognizers/visrecognize/visrecognize.py` & `audalign-1.3.0/audalign/recognizers/visrecognize/visrecognize.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import tqdm
 from audalign.config.visual import VisualConfig
 from audalign.filehandler import find_files, get_shifted_file, read
 from PIL import Image
 from pydub.exceptions import CouldntDecodeError
-from skimage.metrics import mean_squared_error
-from skimage.metrics import structural_similarity as ssim
+try:
+    from skimage.metrics import mean_squared_error
+    from skimage.metrics import structural_similarity as ssim
+except ImportError:
+    # Optional dependency
+    ...
 
 upper_clip = 255
 
 # ------------------------------------------------------------------------------------------
 
 
 def visrecognize(target_file_path: str, against_file_path: str, config: VisualConfig):
```

### Comparing `audalign-1.2.4/audalign.egg-info/PKG-INFO` & `audalign-1.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: audalign
-Version: 1.2.4
+Version: 1.3.0
 Summary: Audio Alignment and Recognition in Python
-Home-page: http://github.com/benfmiller/audalign
-Author: Ben Miller
-Author-email: benfmiller132@gmail.com
-Maintainer: Ben Miller
-Maintainer-email: benfmiller132@gmail.com
-License: MIT
-Keywords: python,audio,align,alignment,fingerprinting,music
-Platform: Unix
-Platform: Windows
-Description-Content-Type: text/markdown
+Project-URL: Homepage, http://github.com/benfmiller/audalign
+Project-URL: Documentation, https://github.com/benfmiller/audalign/wiki
+Project-URL: Changelog, https://github.com/benfmiller/audalign/blob/main/CHANGELOG.md
+Author-email: Ben Miller <benfmiller132@gmail.com>
+Maintainer-email: Ben Miller <benfmiller132@gmail.com>
+License-Expression: MIT
 License-File: LICENSE.md
-Requires-Dist: appdirs==1.4.4
-Requires-Dist: attrs==22.2.0
-Requires-Dist: audioread==3.0.0
-Requires-Dist: certifi==2022.12.7
-Requires-Dist: cffi==1.15.1
-Requires-Dist: charset-normalizer==2.1.1
-Requires-Dist: contourpy==1.0.6
-Requires-Dist: cycler==0.11.0
-Requires-Dist: decorator==5.1.1
-Requires-Dist: exceptiongroup==1.1.0
-Requires-Dist: execnet==1.9.0
-Requires-Dist: fonttools==4.38.0
-Requires-Dist: idna==3.4
-Requires-Dist: imageio==2.23.0
-Requires-Dist: iniconfig==2.0.0
-Requires-Dist: joblib==1.2.0
-Requires-Dist: kiwisolver==1.4.4
-Requires-Dist: librosa==0.10.1
-Requires-Dist: llvmlite==0.41.1
-Requires-Dist: matplotlib==3.6.2
-Requires-Dist: networkx==3.0
-Requires-Dist: noisereduce==2.0.1
-Requires-Dist: numba==0.58.1
-Requires-Dist: numpy==1.26.2
-Requires-Dist: packaging==23.0
-Requires-Dist: Pillow==9.4.0
-Requires-Dist: pluggy==1.0.0
-Requires-Dist: pooch==1.6.0
-Requires-Dist: pycparser==2.21
+Keywords: align,alignment,audio,fingerprinting,music,python
+Requires-Python: >=3.8
+Requires-Dist: matplotlib==3.8.2
+Requires-Dist: numpy==1.26.4
 Requires-Dist: pydub==0.25.1
-Requires-Dist: pyparsing==3.1.1
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: PyWavelets==1.4.1
-Requires-Dist: requests==2.28.1
-Requires-Dist: resampy==0.4.2
-Requires-Dist: scikit-image==0.19.3
-Requires-Dist: scikit-learn==1.3.2
-Requires-Dist: scipy==1.11.4
-Requires-Dist: six==1.16.0
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: threadpoolctl==3.1.0
-Requires-Dist: tifffile==2022.10.10
-Requires-Dist: tomli==2.0.1
-Requires-Dist: tqdm==4.64.1
-Requires-Dist: urllib3==1.26.13
+Requires-Dist: scipy==1.12.0
+Requires-Dist: setuptools==59.6.0
+Requires-Dist: tqdm==4.66.2
+Provides-Extra: noisereduce
+Requires-Dist: noisereduce==2.0.1; extra == 'noisereduce'
+Requires-Dist: torch==2.2.0; extra == 'noisereduce'
+Provides-Extra: test
+Requires-Dist: pytest-xdist==3.1.0; extra == 'test'
+Requires-Dist: pytest==8.0.0; extra == 'test'
+Provides-Extra: visrecognize
+Requires-Dist: pillow==10.2.0; extra == 'visrecognize'
+Requires-Dist: scikit-image==0.19.3; extra == 'visrecognize'
+Description-Content-Type: text/markdown
 
 # Audalign
 
 Package for processing and aligning audio files using audio fingerprinting, cross-correlation, cross-correlation with spectrograms, or visual alignment techniques.
 
 ![gif of audalign aligning](audalign.gif)
 
@@ -111,25 +80,30 @@
 
 ```bash
 pip install audalign
 ```
 
 in the directory
 
+### Optional dependencies
+
+- visrecognize: additional recognizer based on spectrogram image comparison. `pip install audalign[visrecognize]`
+- noisereduce: wrapper utils around [timsainb/noisereduce](https://github.com/timsainb/noisereduce). `pip install audalign[noisereduce]`
+
 ## Recognizers
 
 There are currently four included recognizers, each with their own config objects.
 
 ```python
 import audalign as ad
 
 fingerprint_rec = ad.FingerprintRecognizer()
 correlation_rec = ad.CorrelationRecognizer()
 cor_spec_rec = ad.CorrelationSpectrogramRecognizer()
-visual_rec = ad.VisualRecognizer()
+visual_rec = ad.VisualRecognizer() # requires installting optional visrecognize dependencies
 
 fingerprint_rec.config.set_accuracy(3)
 # recognizer.config.some_item
 ```
 
 For more info about the configuration objects, check out the [wiki](https://github.com/benfmiller/audalign/wiki) or the config objects themselves. They are relatively nicely commented.
 
@@ -165,15 +139,15 @@
 ```
 
 Correlation is more precise than fingerprints and will always give a best alignment unlike fingerprinting, which can return no alignment. `max_lags` is very important for fine aligning. `locality` can be very useful for all alignments and recognitions.
 
 ## Other Functions
 
 ```python
-# wrapper for timsainb/noisereduce
+# wrapper for timsainb/noisereduce, optional dependency
 ad.remove_noise_file(
     "target/file",
     "5", # noise start in seconds
     "20", # noise end in seconds
     "destination/file",
     alt_noise_filepath="different/sound/file",
     prop_decrease="0.5", # If you want noise half reduced
```

