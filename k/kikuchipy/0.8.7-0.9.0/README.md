# Comparing `tmp/kikuchipy-0.8.7.tar.gz` & `tmp/kikuchipy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kikuchipy-0.8.7.tar", last modified: Mon Jul 24 16:10:12 2023, max compression
+gzip compressed data, was "kikuchipy-0.9.0.tar", last modified: Fri Nov  3 12:13:44 2023, max compression
```

## Comparing `kikuchipy-0.8.7.tar` & `kikuchipy-0.9.0.tar`

### file list

```diff
@@ -1,261 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.710459 kikuchipy-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)    53262 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-24 16:10:12.710459 kikuchipy-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.666459 kikuchipy-0.8.7/kikuchipy/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/_rotation/
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_rotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/_rotation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_rotation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_rotation/tests/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/_util/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_util/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_util/_transfer_axes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/_util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_util/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_util/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/_util/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27981 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    73176 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    59696 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5
--rw-r--r--   0 runner    (1001) docker     (123)    55824 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/data/edax_binary/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/edax_binary/edax_binary.up1
--rw-r--r--   0 runner    (1001) docker     (123)    72042 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/edax_binary/edax_binary.up2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy/data/edax_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   938661 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/edax_h5ebsd/patterns.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.674459 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   351168 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.678459 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/BetheParameters.nml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    61872 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml
--rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out
--rw-r--r--   0 runner    (1001) docker     (123)   908492 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.678459 kikuchipy-0.8.7/kikuchipy/data/emsoft_ecp_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    62296 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.678459 kikuchipy-0.8.7/kikuchipy/data/emsoft_tkd_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    61600 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.678459 kikuchipy-0.8.7/kikuchipy/data/kikuchipy_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   149400 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    46480 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.682459 kikuchipy-0.8.7/kikuchipy/data/nordif/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Background acquisition pattern.bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Background calibration pattern.bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Calibration (294,532).bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Calibration (425,447).bmp
--rw-r--r--   0 runner    (1001) docker     (123)    32400 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Pattern.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Setting.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Setting_bad1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Setting_bad2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/nordif/Setting_bad3.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.682459 kikuchipy-0.8.7/kikuchipy/data/oxford_binary/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    32786 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/oxford_binary/patterns.ebsp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.682459 kikuchipy-0.8.7/kikuchipy/data/oxford_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    59152 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/oxford_h5ebsd/patterns.h5oina
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.682459 kikuchipy-0.8.7/kikuchipy/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/data/tests/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.682459 kikuchipy-0.8.7/kikuchipy/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/detectors/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    67124 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/detectors/ebsd_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.682459 kikuchipy-0.8.7/kikuchipy/detectors/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/detectors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/detectors/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    39863 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/detectors/tests/test_ebsd_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.682459 kikuchipy-0.8.7/kikuchipy/draw/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/_navigators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/_plot_pattern_positions_in_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.686459 kikuchipy-0.8.7/kikuchipy/draw/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/tests/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/tests/test_navigators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.686459 kikuchipy-0.8.7/kikuchipy/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/filters/fft_barnes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.686459 kikuchipy-0.8.7/kikuchipy/filters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/filters/tests/test_fft_barnes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/filters/tests/test_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/filters/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.686459 kikuchipy-0.8.7/kikuchipy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.686459 kikuchipy-0.8.7/kikuchipy/generators/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/generators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/generators/tests/test_virtual_bse_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/generators/virtual_bse_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/hyperspy_extension.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.686459 kikuchipy-0.8.7/kikuchipy/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/imaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.686459 kikuchipy-0.8.7/kikuchipy/imaging/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/imaging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/imaging/tests/test_virtual_bse_imager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/imaging/vbse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.690459 kikuchipy-0.8.7/kikuchipy/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_dictionary_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_hough_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_merge_crystal_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_orientation_similarity_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.690459 kikuchipy-0.8.7/kikuchipy/indexing/_refinement/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_refinement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_refinement/_objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    44415 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_refinement/_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/_refinement/_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.690459 kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/_similarity_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.690459 kikuchipy-0.8.7/kikuchipy/indexing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/tests/test_dictionary_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/tests/test_ebsd_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/tests/test_merge_crystal_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/tests/test_orientation_similarity_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/indexing/tests/test_similarity_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.694459 kikuchipy-0.8.7/kikuchipy/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.694459 kikuchipy-0.8.7/kikuchipy/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/_emsoft_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/ebsd_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/edax_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/edax_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/kikuchipy_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/nordif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/nordif_calibration_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/oxford_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/oxford_h5ebsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.698459 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_ebsd_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_edax_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_nordif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_oxford_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.698459 kikuchipy-0.8.7/kikuchipy/io/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/io/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.702459 kikuchipy-0.8.7/kikuchipy/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/pattern/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/pattern/chunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.702459 kikuchipy-0.8.7/kikuchipy/pattern/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/pattern/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/pattern/tests/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/pattern/tests/test_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.702459 kikuchipy-0.8.7/kikuchipy/projections/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/gnomonic_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/hesse_normal_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/lambert_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/spherical_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.702459 kikuchipy-0.8.7/kikuchipy/projections/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/tests/test_gnomonic_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/tests/test_hesse_normal_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/tests/test_lambert_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/projections/tests/test_spherical_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.706459 kikuchipy-0.8.7/kikuchipy/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/_kikuchi_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    22408 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/_kikuchipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/ecp_master_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.706459 kikuchipy-0.8.7/kikuchipy/signals/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88067 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/tests/test_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/tests/test_ebsd_hough_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/tests/test_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/tests/test_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/tests/test_kikuchi_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/tests/test_virtual_bse_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.706459 kikuchipy-0.8.7/kikuchipy/signals/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/_crystal_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/_map_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/_overwrite_hyperspy_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/array_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.710459 kikuchipy-0.8.7/kikuchipy/signals/util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/tests/test_array_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/tests/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/signals/virtual_bse_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.710459 kikuchipy-0.8.7/kikuchipy/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/simulations/_kikuchi_pattern_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/simulations/_kikuchi_pattern_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/simulations/kikuchi_pattern_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.710459 kikuchipy-0.8.7/kikuchipy/simulations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/simulations/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:10:12.670459 kikuchipy-0.8.7/kikuchipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-24 16:10:12.000000 kikuchipy-0.8.7/kikuchipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-24 16:10:12.000000 kikuchipy-0.8.7/kikuchipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:10:12.000000 kikuchipy-0.8.7/kikuchipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 16:10:12.000000 kikuchipy-0.8.7/kikuchipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 16:10:12.000000 kikuchipy-0.8.7/kikuchipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 16:10:12.000000 kikuchipy-0.8.7/kikuchipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:10:12.000000 kikuchipy-0.8.7/kikuchipy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 16:10:12.710459 kikuchipy-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-24 16:09:59.000000 kikuchipy-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.341985 kikuchipy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    56036 2023-11-03 12:13:33.000000 kikuchipy-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2023-11-03 12:13:33.000000 kikuchipy-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-03 12:13:33.000000 kikuchipy-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-11-03 12:13:33.000000 kikuchipy-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-03 12:13:33.000000 kikuchipy-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2023-11-03 12:13:44.341985 kikuchipy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2023-11-03 12:13:33.000000 kikuchipy-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2023-11-03 12:13:33.000000 kikuchipy-0.9.0/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.301985 kikuchipy-0.9.0/kikuchipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.301985 kikuchipy-0.9.0/kikuchipy/_rotation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_rotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.301985 kikuchipy-0.9.0/kikuchipy/_rotation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_rotation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_rotation/tests/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.301985 kikuchipy-0.9.0/kikuchipy/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_util/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_util/_transfer_axes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.305985 kikuchipy-0.9.0/kikuchipy/_util/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_util/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9565 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_util/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/_util/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14809 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.305985 kikuchipy-0.9.0/kikuchipy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22535 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.305985 kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (127)    16614 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73176 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    59696 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    55824 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.305985 kikuchipy-0.9.0/kikuchipy/data/edax_binary/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32416 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/edax_binary/edax_binary.up1
+-rw-r--r--   0 runner    (1001) docker     (127)    72042 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/edax_binary/edax_binary.up2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.305985 kikuchipy-0.9.0/kikuchipy/data/edax_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (127)   938661 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/edax_h5ebsd/patterns.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.309985 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd/
+-rw-r--r--   0 runner    (1001) docker     (127)   351168 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35624 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.313985 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/BetheParameters.nml
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61872 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml
+-rw-r--r--   0 runner    (1001) docker     (127)    19638 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out
+-rw-r--r--   0 runner    (1001) docker     (127)   908492 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.313985 kikuchipy-0.9.0/kikuchipy/data/emsoft_ecp_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62296 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.313985 kikuchipy-0.9.0/kikuchipy/data/emsoft_tkd_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61600 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.313985 kikuchipy-0.9.0/kikuchipy/data/kikuchipy_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (127)   149400 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    46480 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.313985 kikuchipy-0.9.0/kikuchipy/data/nordif/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4678 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Background acquisition pattern.bmp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4678 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Background calibration pattern.bmp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4678 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Calibration (294,532).bmp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4678 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Calibration (425,447).bmp
+-rw-r--r--   0 runner    (1001) docker     (127)    32400 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Pattern.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Setting.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Setting_bad1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Setting_bad2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/nordif/Setting_bad3.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.317985 kikuchipy-0.9.0/kikuchipy/data/oxford_binary/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32786 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/oxford_binary/patterns.ebsp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.317985 kikuchipy-0.9.0/kikuchipy/data/oxford_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59152 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/oxford_h5ebsd/patterns.h5oina
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.317985 kikuchipy-0.9.0/kikuchipy/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10633 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/data/tests/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.317985 kikuchipy-0.9.0/kikuchipy/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/detectors/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68538 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/detectors/ebsd_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.317985 kikuchipy-0.9.0/kikuchipy/detectors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/detectors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/detectors/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40279 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/detectors/tests/test_ebsd_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.317985 kikuchipy-0.9.0/kikuchipy/draw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/_navigators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/_plot_pattern_positions_in_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.321985 kikuchipy-0.9.0/kikuchipy/draw/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/tests/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/tests/test_navigators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.321985 kikuchipy-0.9.0/kikuchipy/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/filters/fft_barnes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.321985 kikuchipy-0.9.0/kikuchipy/filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/filters/tests/test_fft_barnes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15640 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/filters/tests/test_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/filters/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/hyperspy_extension.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.321985 kikuchipy-0.9.0/kikuchipy/imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/imaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.321985 kikuchipy-0.9.0/kikuchipy/imaging/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/imaging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9960 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/imaging/tests/test_virtual_bse_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16334 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/imaging/vbse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.321985 kikuchipy-0.9.0/kikuchipy/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_dictionary_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16011 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_hough_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_merge_crystal_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_orientation_similarity_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.321985 kikuchipy-0.9.0/kikuchipy/indexing/_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_refinement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_refinement/_objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_refinement/_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21304 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/_refinement/_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.325985 kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/_similarity_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.325985 kikuchipy-0.9.0/kikuchipy/indexing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/tests/test_dictionary_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47403 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/tests/test_ebsd_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23728 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/tests/test_merge_crystal_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/tests/test_orientation_similarity_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/indexing/tests/test_similarity_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.325985 kikuchipy-0.9.0/kikuchipy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.329985 kikuchipy-0.9.0/kikuchipy/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/_emsoft_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16041 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/ebsd_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/edax_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/edax_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17736 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/kikuchipy_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14826 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/nordif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/nordif_calibration_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19627 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/oxford_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/oxford_h5ebsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.329985 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_ebsd_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_edax_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14640 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13546 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_nordif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_oxford_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.329985 kikuchipy-0.9.0/kikuchipy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/io/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.333985 kikuchipy-0.9.0/kikuchipy/pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25808 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/pattern/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/pattern/chunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.333985 kikuchipy-0.9.0/kikuchipy/pattern/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/pattern/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/pattern/tests/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18739 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/pattern/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.333985 kikuchipy-0.9.0/kikuchipy/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/_kikuchi_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22408 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/_kikuchipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131002 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18279 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/ecp_master_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.333985 kikuchipy-0.9.0/kikuchipy/signals/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88067 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/tests/test_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15297 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/tests/test_ebsd_hough_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28202 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/tests/test_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/tests/test_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/tests/test_kikuchi_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/tests/test_virtual_bse_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.337985 kikuchipy-0.9.0/kikuchipy/signals/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/_crystal_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/_map_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24095 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/_overwrite_hyperspy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/array_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.337985 kikuchipy-0.9.0/kikuchipy/signals/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/tests/test_array_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/signals/virtual_bse_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.337985 kikuchipy-0.9.0/kikuchipy/simulations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/simulations/_kikuchi_pattern_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26380 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/simulations/_kikuchi_pattern_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27443 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/simulations/kikuchi_pattern_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.337985 kikuchipy-0.9.0/kikuchipy/simulations/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/simulations/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11838 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 12:13:44.301985 kikuchipy-0.9.0/kikuchipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2023-11-03 12:13:44.000000 kikuchipy-0.9.0/kikuchipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2023-11-03 12:13:44.000000 kikuchipy-0.9.0/kikuchipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 12:13:44.000000 kikuchipy-0.9.0/kikuchipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-03 12:13:44.000000 kikuchipy-0.9.0/kikuchipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-11-03 12:13:44.000000 kikuchipy-0.9.0/kikuchipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-03 12:13:44.000000 kikuchipy-0.9.0/kikuchipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 12:13:44.000000 kikuchipy-0.9.0/kikuchipy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-03 12:13:44.345985 kikuchipy-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-11-03 12:13:34.000000 kikuchipy-0.9.0/setup.py
```

### Comparing `kikuchipy-0.8.7/CHANGELOG.rst` & `kikuchipy-0.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,71 @@
 All user facing changes to this project are documented in this file. The format is based
 on `Keep a Changelog <https://keepachangelog.com/en/1.1.0>`__, and this project tries
 its best to adhere to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`__.
 
 List entries are sorted in descending chronological order. Contributors to each release
 were listed in alphabetical order by first name until version 0.7.0.
 
+0.9.0 (2023-11-03)
+==================
+
+Added
+-----
+- Explicit support for Python 3.11.
+  (`#646 <https://github.com/pyxem/kikuchipy/pull/646>`_)
+- Allow Hough indexing of all Laue groups with PyEBSDIndex v0.2 (not just *m-3m*, i.e.
+  FCC and BCC). (`#652 <https://github.com/pyxem/kikuchipy/pull/652>`_)
+- Control of reflector lists in Hough indexing. One reflector list per phase in the
+  phase list can be passed to ``EBSDDetector.get_indexer()`` to obtain an
+  ``EBSDIndexer`` for use in ``EBSD.hough_indexing()``.
+  (`#652 <https://github.com/pyxem/kikuchipy/pull/652>`_)
+- Allow passing keyword arguments to ``EBSD.hough_indexing_optimize_pc()`` to control
+  the new particle swarm optimization algorithm in PyEBSDIndex v0.2.
+  (`#652 <https://github.com/pyxem/kikuchipy/pull/652>`_)
+- Allow getting one projection center (PC) per pattern when optimizing PCs using the new
+  particle swarm optimization in PyEBSDIndex v0.2 (passing ``batch=True``).
+  (`#652 <https://github.com/pyxem/kikuchipy/pull/652>`_)
+
+Changed
+-------
+- Parameter ``zone_axes_kwargs`` in
+  ``GeometricalKikuchiPatternSimulation.as_collections()`` does not accept ``color``
+  internally to set the default color to white anymore. It accepts ``fc`` (facecolor)
+  instead. This change was necessary to improve handling of other keyword arguments.
+  (`#643 <https://github.com/pyxem/kikuchipy/pull/643>`_)
+- Increase minimal versions of diffsims, NumPy, Matplotlib, and PyEBSDIndex to 0.5.1,
+  1.21.6, 3.5, and 0.2, respectively.
+  (`#646 <https://github.com/pyxem/kikuchipy/pull/646>`_,
+  `#652 <https://github.com/pyxem/kikuchipy/pull/652>`_)
+- Remove dependency on Panel for documentation, and with that the interactive 3D
+  visualization of master patterns in the documentation. The plan is to reintroduce the
+  interactive plots with trame later on.
+  (`#652 <https://github.com/pyxem/kikuchipy/pull/652>`_)
+- Restrict HyperSpy to below the forthcoming version 2. The plan is to remove this
+  restriction once kikuchipy is compatible with this version.
+  (`#657 <https://github.com/pyxem/kikuchipy/pull/657>`_)
+
+Removed
+-------
+- ``generators`` and ``projections`` modules which were deprecated in version 0.8.
+  (`#612 <https://github.com/pyxem/kikuchipy/pull/612>`_)
+- The deprecated PyPI selector ``viz`` is removed.
+  (`#643 <https://github.com/pyxem/kikuchipy/pull/643>`_)
+- The data module functions ``silicon_ebsd_moving_screen_x()``, where "x" is "in",
+  "out5mm" or "out10mm". They were deprecated in version 0.8.
+  (`#656 <https://github.com/pyxem/kikuchipy/pull/656>`_)
+
+Fixed
+-----
+- Conversion from EDAX TSL projection center (PC) convention for (PCy, PCz) for
+  rectangular detectors is corrected.
+  (`#652 <https://github.com/pyxem/kikuchipy/pull/652>`_)
+- Downloading files in the ``data`` module to the local cache on Windows.
+  (`#655 <https://github.com/pyxem/kikuchipy/pull/655>`_)
+
 0.8.7 (2023-07-24)
 ==================
 
 Fixed
 -----
 - Passing a 3-component PC array with more than one dimension to
   ``EBSD.hough_indexing_optimize_pc()`` works.
@@ -183,15 +240,15 @@
   experimental. (`#578 <https://github.com/pyxem/kikuchipy/pull/578>`_)
 - ``EBSDDetector.crop()`` method to get a new detector with its shape cropped, also
   updating the PC values accordingly.
   (`#578 <https://github.com/pyxem/kikuchipy/pull/578>`_)
 
 Changed
 -------
-- Minimal version of orix set to >= 0.11 and of numba set to >= 0.55.
+- Minimal version of orix set to >= 0.11 and of Numba set to >= 0.55.
   (`#608 <https://github.com/pyxem/kikuchipy/pull/608>`_)
 - Added warnings when trying to perform adaptive histogram equalization on a signal with
   data in floating type or when some of the data is NaN.
   (`#606 <https://github.com/pyxem/kikuchipy/pull/606>`_)
 - Dask arrays returned from EBSD refinement methods has the number of function
   evaluations as the second element after the score.
   (`#593 <https://github.com/pyxem/kikuchipy/pull/593>`_)
@@ -202,16 +259,14 @@
 - Passing two crystal maps with identical phases when merging returns a map with one
   phase instead of two and does not raise a warning, as before.
   (`#593 <https://github.com/pyxem/kikuchipy/pull/593>`_)
 - Exclude documentation and tests from source distribution.
   (`#588 <https://github.com/pyxem/kikuchipy/pull/588>`_)
 - Minimal version of HyperSpy increased to >= 1.7.3.
   (`#585 <https://github.com/pyxem/kikuchipy/pull/585>`_)
-- Minimal version of Numba increased to >= 0.52.
-  (`#585 <https://github.com/pyxem/kikuchipy/pull/585>`_)
 - When binning the navigation dimension(s) with ``EBSD.rebin()``, the class attributes
   ``xmap`` and ``static_background`` are set to ``None`` and ``detector.pc`` is set to
   ``[0.5, 0.5, 0.5]`` in the appropriate navigation shape. If the signal dimension(s)
   are binned, the ``static_background`` is binned similarly while the ``detector.shape``
   and ``detector.binning`` are updated. If this handling of attributes fails, the old
   behavior is retained. This handling is experimental.
   (`#578 <https://github.com/pyxem/kikuchipy/pull/578>`_)
```

### Comparing `kikuchipy-0.8.7/CODE_OF_CONDUCT.rst` & `kikuchipy-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,157 +1,164 @@
 =========================
 kikuchipy Code of Conduct
 =========================
 
 Introduction
 ============
 
-This code of conduct applies to all spaces managed by the kikuchipy project,
-including all public and private mailing lists, issue trackers, wikis, blogs,
-Twitter, and any other communication channel used by our community. The
-kikuchipy project does not organise in-person events, however events related to
-our community should have a code of conduct similar in spirit to this one.
-
-This code of conduct should be honoured by everyone who participates in the
-kikuchipy community formally or informally, or claims any affiliation with the
-project, in any project-related activities and especially when representing the
-project, in any role.
-
-This code is not exhaustive or complete. It serves to distill our common
-understanding of a collaborative, shared environment and goals. Please try to
-follow this code in spirit as much as in letter, to create a friendly and
+This code of conduct applies to all spaces managed by the kikuchipy project, including
+all public and private mailing lists, issue trackers, wikis, blogs, and any other
+communication channel used by our community.
+The kikuchipy project does not organise in-person events, however events related to our
+community should have a code of conduct similar in spirit to this one.
+
+This code of conduct should be honoured by everyone who participates in the kikuchipy
+community formally or informally, or claims any affiliation with the project, in any
+project-related activities and especially when representing the project, in any role.
+
+This code is not exhaustive or complete. It serves to distill our common understanding
+of a collaborative, shared environment and goals.
+Please try to follow this code in spirit as much as in letter, to create a friendly and
 productive environment that enriches the surrounding community.
 
 Specific guidelines
 ===================
 
 We strive to:
 
-1. Be open. We invite anyone to participate in our community. We prefer to use
-   public methods of communication for project-related messages, unless
-   discussing something sensitive. This applies to messages for help or
-   project-related support, too; not only is a public-support request much more
-   likely to result in an answer to a question, it also ensures that any
-   inadvertent mistakes in answering are more easily detected and corrected.
-
-2. Be empathetic, welcoming, friendly, and patient. We work together to resolve
-   conflict, and assume good intentions. We may all experience some frustration
-   from time to time, but we do not allow frustration to turn into a personal
-   attack. A community where people feel uncomfortable or threatened is not a
-   productive one.
-
-3. Be collaborative. Our work will be used by other people, and in turn we will
-   depend on the work of others. When we make something for the benefit of the
-   project, we are willing to explain to others how it works, so that they can
-   build on the work to make it even better. Any decision we make will affect
-   users and colleagues, and we take those consequences seriously when making
-   decisions.
-
-4. Be inquisitive. Nobody knows everything! Asking questions early avoids many
-   problems later, so we encourage questions, although we may direct them to the
-   appropriate forum. We will try hard to be responsive and helpful.
-
-5. Be careful in the words that we choose. We are careful and respectful in our
-   communication and we take responsibility for our own speech. Be kind
-   others. Do not insult or put down other participants. We will not accept
-   harassment or other exclusionary behaviour, such as:
+1. Be open.
+   We invite anyone to participate in our community.
+   We prefer to use public methods of communication for project-related messages, unless
+   discussing something sensitive.
+   This applies to messages for help or project-related support, too; not only is a
+   public-support request much more likely to result in an answer to a question, it also
+   ensures that any inadvertent mistakes in answering are more easily detected and
+   corrected.
+
+2. Be empathetic, welcoming, friendly, and patient.
+   We work together to resolve conflict, and assume good intentions.
+   We may all experience some frustration from time to time, but we do not allow
+   frustration to turn into a personal attack.
+   A community where people feel uncomfortable or threatened is not a productive one.
+
+3. Be collaborative.
+   Our work will be used by other people, and in turn we will depend on the work of
+   others.
+   When we make something for the benefit of the project, we are willing to explain to
+   others how it works, so that they can build on the work to make it even better.
+   Any decision we make will affect users and colleagues, and we take those consequences
+   seriously when making decisions.
+
+4. Be inquisitive.
+   Nobody knows everything!
+   Asking questions early avoids many problems later, so we encourage questions,
+   although we may direct them to the appropriate forum.
+   We will try hard to be responsive and helpful.
+
+5. Be careful in the words that we choose.
+   We are careful and respectful in our communication and we take responsibility for our
+   own speech.
+   Be kind others.
+   Do not insult or put down other participants.
+   We will not accept harassment or other exclusionary behaviour, such as:
 
    - Violent threats or language directed against another person.
    - Sexist, racist, ableist, or otherwise discriminatory jokes and language.
    - Posting sexually explicit or violent material.
-   - Posting (or threatening to post) other people's personally identifying
-     information ("doxing").
-   - Sharing private content, such as emails sent privately or non-publicly, or
-     unlogged forums such as IRC channel history, without the sender's consent.
+   - Posting (or threatening to post) other people's personally identifying information
+     ("doxing").
+   - Sharing private content, such as emails sent privately or non-publicly, or unlogged
+     forums such as IRC channel history, without the sender's consent.
    - Personal insults, especially those using racist, sexist, or ableist terms.
-   - Intentional or repeated misgendering of participants who have explicitly
-     requested to be addressed by specific pronouns.
+   - Intentional or repeated misgendering of participants who have explicitly requested
+     to be addressed by specific pronouns.
    - Unwelcome sexual attention.
-   - Excessive profanity. Please avoid swearwords; people differ greatly in
-     their sensitivity to swearing.
-   - Repeated harassment of others. In general, if someone asks you to stop,
-     then stop.
+   - Excessive profanity.
+     Please avoid swearwords; people differ greatly in their sensitivity to swearing.
+   - Repeated harassment of others.
+     In general, if someone asks you to stop, then stop.
    - Advocating for, or encouraging, any of the above behaviour.
 
 Diversity statement
 ===================
 
-The kikuchipy project welcomes and encourages participation by everyone. We are
-committed to being a community that everyone enjoys being part of. Although we
-may not always be able to accommodate each individual's preferences, we try our
-best to treat everyone kindly.
+The kikuchipy project welcomes and encourages participation by everyone.
+We are committed to being a community that everyone enjoys being part of.
+Although we may not always be able to accommodate each individual's preferences, we try
+our best to treat everyone kindly.
 
 No matter how you identify yourself or how others perceive you: we welcome you.
-Though no list can hope to be comprehensive, we explicitly honour diversity in:
-age, culture, ethnicity, genotype, gender identity or expression, language,
-national origin, neurotype, phenotype, political beliefs, profession, race,
-religion, sexual orientation, socioeconomic status, subculture and technical
-ability, to the extent that these do not conflict with this code of conduct.
-
-Though we welcome people fluent in all languages, kikuchipy development is
-conducted in English.
-
-Standards for behaviour in the kikuchipy community are detailed in the Code of
-Conduct above. Participants in our community should uphold these standards in
-all their interactions and help others to do so as well (see next section).
+Though no list can hope to be comprehensive, we explicitly honour diversity in: age,
+culture, ethnicity, genotype, gender identity or expression, language, national origin,
+neurotype, phenotype, political beliefs, profession, race, religion, sexual orientation,
+socioeconomic status, subculture and technical ability, to the extent that these do not
+conflict with this code of conduct.
+
+Though we welcome people fluent in all languages, kikuchipy development is conducted in
+English.
+
+Standards for behaviour in the kikuchipy community are detailed in the Code of Conduct
+above.
+Participants in our community should uphold these standards in all their interactions
+and help others to do so as well (see next section).
 
 Reporting guidelines
 ====================
 
-We know that it is painfully common for internet communication to start at or
-devolve into obvious and flagrant abuse. We also recognize that sometimes people
-may have had a bad day, or be unaware of some of the guidelines in this Code of
-Conduct. Please keep this in mind when deciding how to respond to a breach of
-this Code.
-
-For clearly intentional breaches, report those to the Code of Conduct Committee
-(see below). For possibly unintentional breaches, you may reply to the person
-and point out this Code of Conduct (either in public or in private, whatever is
-most appropriate). If you would prefer not to do that, please feel free to
-report to the code of conduct committee directly, or ask the committee for
-advice, in confidence.
+We know that it is painfully common for internet communication to start at or devolve
+into obvious and flagrant abuse.
+We also recognize that sometimes people may have had a bad day, or be unaware of some of
+the guidelines in this Code of Conduct.
+Please keep this in mind when deciding how to respond to a breach of this Code.
+
+For clearly intentional breaches, report those to the Code of Conduct Committee (see
+below).
+For possibly unintentional breaches, you may reply to the person and point out this Code
+of Conduct (either in public or in private, whatever is most appropriate).
+If you would prefer not to do that, please feel free to report to the code of conduct
+committee directly, or ask the committee for advice, in confidence.
 
 You can report issues to the kikuchipy Code of Conduct Committee, at
-kikuchipy-conduct@googlegroups.com. Currently, the committee consists of:
+kikuchipy-conduct@googlegroups.com.
+Currently, the committee consists of:
 
 * `Håkon Wiik Ånes <https://github.com/hakonanes>`_ (chair)
 * `Tina Bergh <https://github.com/tinabe>`_
 
 Incident reporting resolution & Code of Conduct enforcement
 ===========================================================
 
-*This section summarizes the most important points, more details can be found
-in* :doc:`report_handling_manual`.
+*This section summarizes the most important points, more details can be found in*
+:doc:`report_handling_manual`.
 
-We will investigate and respond to all complaints. The kikuchipy Code of Conduct
-Committee will protect the identity of the reporter, and treat the content of
-complaints as confidential (unless the reporter agrees otherwise).
-
-In case of severe and obvious breaches, e.g. personal threat or violent,
-sexist or racist language, we will immediately disconnect the originator from
-kikuchipy communication channels; please see the manual for details.
-
-In cases not involving clear severe and obvious breaches of this code of
-conduct, the process for acting on any received code of conduct violation report
-will be:
+We will investigate and respond to all complaints.
+The kikuchipy Code of Conduct Committee will protect the identity of the reporter, and
+treat the content of complaints as confidential (unless the reporter agrees otherwise).
+
+In case of severe and obvious breaches, e.g. personal threat or violent, sexist or
+racist language, we will immediately disconnect the originator from kikuchipy
+communication channels; please see the manual for details.
+
+In cases not involving clear severe and obvious breaches of this code of conduct, the
+process for acting on any received code of conduct violation report will be:
 
 1. acknowledge report is received
 
 2. reasonable discussion/feedback
 
 3. mediation (if feedback didn't help, and only if both reporter and reportee
    agree to this)
 
 4. enforcement via transparent decision (see :ref:`resolutions`) by the Code of
    Conduct Committee
 
-The committee will respond to any report as soon as possible, and at most within
-72 hours.
+The committee will respond to any report as soon as possible, and at most within 72
+hours.
 
 Endnotes
 ========
 
-We are thankful to the groups behind the following documents, from which we drew
-content and inspiration:
+We are thankful to the groups behind the following documents, from which we drew content
+and inspiration:
 
 * `napari Code of Conduct <https://napari.org/community/code_of_conduct.html>`_
 * `NumPy Code of Conduct <https://numpy.org/code-of-conduct>`_
```

### Comparing `kikuchipy-0.8.7/LICENSE` & `kikuchipy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/PKG-INFO` & `kikuchipy-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,7 @@
-Metadata-Version: 2.1
-Name: kikuchipy
-Version: 0.8.7
-Summary: Processing, simulating and indexing of electron backscatter diffraction (EBSD) patterns.
-Home-page: https://kikuchipy.org
-Download-URL: https://pypi.python.org/pypi/kikuchipy
-Author: kikuchipy developers
-Author-email: hakon.w.anes@ntnu.no
-Maintainer: Håkon Wiik Ånes
-Maintainer-email: hakon.w.anes@ntnu.no
-License: GPLv3+
-Project-URL: Bug Tracker, https://github.com/pyxem/kikuchipy/issues
-Project-URL: Documentation, https://kikuchipy.org
-Project-URL: Source Code, https://github.com/pyxem/kikuchipy
-Keywords: EBSD,electron backscatter diffraction,EBSP,electron backscatter pattern,BKD,backscatter kikuchi diffraction,SEM,scanning electron microscopy,kikuchi pattern,dictionary indexing
-Platform: "Linux"
-Platform: "MacOS X"
-Platform: "Windows"
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: doc
-Provides-Extra: tests
-Provides-Extra: all
-Provides-Extra: viz
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
   <a href="https://kikuchipy.org">
     <img width="60%" src="https://raw.githubusercontent.com/pyxem/kikuchipy/develop/doc/_static/logo/plasma_banner.png">
   </a>
 </div>
 
 kikuchipy [ki-ko-chi-pai] is a library for processing, simulating and indexing of
@@ -87,31 +48,33 @@
 ## Citing kikuchipy
 
 If you are using kikuchipy in your scientific research, please help our scientific
 visibility by citing the Zenodo DOI: https://doi.org/10.5281/zenodo.3597646.
 
 ## Contributors ✨
 
-Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+Thanks go to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ericpre"><img src="https://avatars.githubusercontent.com/u/11851990?v=4?s=100" width="100px;" alt="Eric Prestat"/><br /><sub><b>Eric Prestat</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=ericpre" title="Code">💻</a> <a href="#maintenance-ericpre" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AndreasBugten"><img src="https://avatars.githubusercontent.com/u/106192446?v=4?s=100" width="100px;" alt="AndreasBugten"/><br /><sub><b>AndreasBugten</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=AndreasBugten" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/CSSFrancis"><img src="https://avatars.githubusercontent.com/u/41125831?v=4?s=100" width="100px;" alt="Carter Francis"/><br /><sub><b>Carter Francis</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=CSSFrancis" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ericpre"><img src="https://avatars.githubusercontent.com/u/11851990?v=4?s=100" width="100px;" alt="Eric Prestat"/><br /><sub><b>Eric Prestat</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=ericpre" title="Code">💻</a> <a href="#maintenance-ericpre" title="Maintenance">🚧</a> <a href="https://github.com/pyxem/kikuchipy/issues?q=author%3Aericpre" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.ntnu.edu/employees/hakon.w.anes"><img src="https://avatars.githubusercontent.com/u/12139781?v=4?s=100" width="100px;" alt="Håkon Wiik Ånes"/><br /><sub><b>Håkon Wiik Ånes</b></sub></a><br /></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/friedkitteh"><img src="https://avatars.githubusercontent.com/u/11888052?v=4?s=100" width="100px;" alt="Lars Lervik"/><br /><sub><b>Lars Lervik</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/issues?q=author%3Afriedkitteh" title="Bug reports">🐛</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=friedkitteh" title="Code">💻</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=friedkitteh" title="Documentation">📖</a> <a href="#question-friedkitteh" title="Answering Questions">💬</a> <a href="https://github.com/pyxem/kikuchipy/pulls?q=is%3Apr+reviewed-by%3Afriedkitteh" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=friedkitteh" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.ntnu.edu/employees/magnus.nord"><img src="https://avatars.githubusercontent.com/u/1690979?v=4?s=100" width="100px;" alt="Magnus Nord"/><br /><sub><b>Magnus Nord</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=magnunor" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/onatlandsmyr"><img src="https://avatars.githubusercontent.com/u/34620114?v=4?s=100" width="100px;" alt="Ole Natlandsmyr"/><br /><sub><b>Ole Natlandsmyr</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=onatlandsmyr" title="Code">💻</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=onatlandsmyr" title="Documentation">📖</a> <a href="#question-onatlandsmyr" title="Answering Questions">💬</a> <a href="https://github.com/pyxem/kikuchipy/pulls?q=is%3Apr+reviewed-by%3Aonatlandsmyr" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=onatlandsmyr" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tinabe"><img src="https://avatars.githubusercontent.com/u/22915119?v=4?s=100" width="100px;" alt="Tina Bergh"/><br /><sub><b>Tina Bergh</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=tinabe" title="Code">💻</a> <a href="https://github.com/pyxem/kikuchipy/pulls?q=is%3Apr+reviewed-by%3Atinabe" title="Reviewed Pull Requests">👀</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/IMBalENce"><img src="https://avatars.githubusercontent.com/u/2986794?v=4?s=100" width="100px;" alt="Zhou Xu"/><br /><sub><b>Zhou Xu</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/issues?q=author%3AIMBalENce" title="Bug reports">🐛</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=IMBalENce" title="Code">💻</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=IMBalENce" title="Documentation">📖</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=IMBalENce" title="Tests">⚠️</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tinabe"><img src="https://avatars.githubusercontent.com/u/22915119?v=4?s=100" width="100px;" alt="Tina Bergh"/><br /><sub><b>Tina Bergh</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/commits?author=tinabe" title="Code">💻</a> <a href="https://github.com/pyxem/kikuchipy/pulls?q=is%3Apr+reviewed-by%3Atinabe" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/IMBalENce"><img src="https://avatars.githubusercontent.com/u/2986794?v=4?s=100" width="100px;" alt="Zhou Xu"/><br /><sub><b>Zhou Xu</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/issues?q=author%3AIMBalENce" title="Bug reports">🐛</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=IMBalENce" title="Code">💻</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=IMBalENce" title="Documentation">📖</a> <a href="https://github.com/pyxem/kikuchipy/commits?author=IMBalENce" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Erlendos12"><img src="https://avatars.githubusercontent.com/u/99336047?v=4?s=100" width="100px;" alt="erlenmos"/><br /><sub><b>erlenmos</b></sub></a><br /><a href="https://github.com/pyxem/kikuchipy/issues?q=author%3AErlendos12" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.7 Summary: Processing,
-simulating and indexing of electron backscatter diffraction (EBSD) patterns.
-Home-page: https://kikuchipy.org Download-URL: https://pypi.python.org/pypi/
-kikuchipy Author: kikuchipy developers Author-email: hakon.w.anes@ntnu.no
-Maintainer: HÃ¥kon Wiik Ãnes Maintainer-email: hakon.w.anes@ntnu.no License:
-GPLv3+ Project-URL: Bug Tracker, https://github.com/pyxem/kikuchipy/issues
-Project-URL: Documentation, https://kikuchipy.org Project-URL: Source Code,
-https://github.com/pyxem/kikuchipy Keywords: EBSD,electron backscatter
-diffraction,EBSP,electron backscatter pattern,BKD,backscatter kikuchi
-diffraction,SEM,scanning electron microscopy,kikuchi pattern,dictionary
-indexing Platform: "Linux" Platform: "MacOS X" Platform: "Windows" Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Development Status :: 4 - Beta Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Physics Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: doc
-Provides-Extra: tests Provides-Extra: all Provides-Extra: viz Provides-Extra:
-dev License-File: LICENSE
  _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_y_x_e_m_/_k_i_k_u_c_h_i_p_y_/_d_e_v_e_l_o_p_/_d_o_c_/___s_t_a_t_i_c_/_l_o_g_o_/
                               _p_l_a_s_m_a___b_a_n_n_e_r_._p_n_g_]
 kikuchipy [ki-ko-chi-pai] is a library for processing, simulating and indexing
 of electron backscatter diffraction (EBSD) patterns in Python, built on the
 tools for multi-dimensional data analysis provided by the HyperSpy library. |
 Deployment | [![PyPI version](https://img.shields.io/pypi/v/
 kikuchipy.svg?logo=python&logoColor=white)](https://pypi.org/project/kikuchipy/
@@ -55,25 +33,27 @@
 `conda`: ```bash conda install kikuchipy -c conda-forge ``` You can also visit
 [PyPI](https://pypi.org/project/kikuchipy), [Anaconda](https://anaconda.org/
 conda-forge/kikuchipy), or [GitHub](https://github.com/pyxem/kikuchipy) to
 download the source. Further details are available in the [installation guide]
 (https://kikuchipy.org/en/latest/user/installation.html). ## Citing kikuchipy
 If you are using kikuchipy in your scientific research, please help our
 scientific visibility by citing the Zenodo DOI: https://doi.org/10.5281/
-zenodo.3597646. ## Contributors â¨ Thanks goes to these wonderful people (
-[emoji key](https://allcontributors.org/docs/en/emoji-key)):
-  _[_E_r_i_c     _[_H_Ã_¥_k_o_n     _[_L_a_r_s     _[_M_a_g_n_u_s       _[_O_l_e       _[_T_i_n_a     _[_Z_h_o_u_ _X_u_]
- _P_r_e_s_t_a_t_]     _W_i_i_k     _L_e_r_v_i_k_]     _N_o_r_d_]    _N_a_t_l_a_n_d_s_m_y_r_]   _B_e_r_g_h_]     _ZZ_hh_oo_uu_ _XX_uu
-   _EE_rr_ii_cc      _Ã__n_e_s_]     _LL_aa_rr_ss    _MM_aa_gg_nn_uu_ss_ _NN_oo_rr_dd     _OO_ll_ee      _TT_ii_nn_aa_ _BB_ee_rr_gg_hh  _ð___ _ð___»
- _PP_rr_ee_ss_tt_aa_tt     _HH_?Ã_?¥_kk_oo_nn    _LL_ee_rr_vv_ii_kk      _ð___     _NN_aa_tt_ll_aa_nn_dd_ss_mm_yy_rr  _ð___» _ð___  _ð___ _â__ _ï_¸_
-_ð___» _ð___§  _WW_ii_ii_kk_ _?Ã_?_nn_ee_ss _ð___ _ð___»              _ð___» _ð___
-                      _ð___ _ð___¬              _ð___¬ _ð___
-                        _ð___                   _â__ _ï_¸_
-                       _â__ _ï_¸_
-_[_e_r_l_e_n_m_o_s_]
- _ee_rr_ll_ee_nn_mm_oo_ss
-   _ð___
+zenodo.3597646. ## Contributors â¨ Thanks go to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)):
+_[_A_n_d_r_e_a_s_B_u_g_t_e_n_]  _[_C_a_r_t_e_r    _[_E_r_i_c     _[_H_Ã_¥_k_o_n     _[_L_a_r_s   _[_M_a_g_n_u_s     _[_O_l_e
+ _AA_nn_dd_rr_ee_aa_ss_BB_uu_gg_tt_ee_nn  _F_r_a_n_c_i_s_]   _P_r_e_s_t_a_t_]     _W_i_i_k     _L_e_r_v_i_k_]   _N_o_r_d_]  _N_a_t_l_a_n_d_s_m_y_r_]
+     _ð___        _CC_aa_rr_tt_ee_rr      _EE_rr_ii_cc      _Ã__n_e_s_]     _LL_aa_rr_ss    _MM_aa_gg_nn_uu_ss      _OO_ll_ee
+                 _FF_rr_aa_nn_cc_ii_ss   _PP_rr_ee_ss_tt_aa_tt     _HH_?Ã_?¥_kk_oo_nn    _LL_ee_rr_vv_ii_kk    _NN_oo_rr_dd   _NN_aa_tt_ll_aa_nn_dd_ss_mm_yy_rr
+                  _ð___    _ð___» _ð___§  _WW_ii_ii_kk_ _?Ã_?_nn_ee_ss _ð___ _ð___»  _ð___    _ð___» _ð___
+                             _ð___               _ð___ _ð___¬          _ð___¬ _ð___
+                                                  _ð___               _â__ _ï_¸_
+                                                 _â__ _ï_¸_
+  _[_T_i_n_a_ _B_e_r_g_h_]  _[_Z_h_o_u_ _X_u_] _[_e_r_l_e_n_m_o_s_]
+   _TT_ii_nn_aa_ _BB_ee_rr_gg_hh    _ZZ_hh_oo_uu_ _XX_uu   _ee_rr_ll_ee_nn_mm_oo_ss
+    _ð___» _ð___   _ð___ _ð___»    _ð___
+                  _ð___
+                 _â__ _ï_¸_
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! Please see our [contributing guide](https://kikuchipy.org/en/latest/
 dev/index.html) for information on how best to contribute (or just explain what
 you want to do [in an issue](https://github.com/pyxem/kikuchipy/issues/new)).
```

### Comparing `kikuchipy-0.8.7/RELEASE.rst` & `kikuchipy-0.9.0/RELEASE.rst`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 - Increment the version number in ``kikuchipy/release.py``.
   Review and clean up ``CHANGELOG.rst`` as per Keep a Changelog.
 
 - Make a PR of the release branch to ``main``.
   Discuss the changelog with others, and make any changes *directly* to the release
   branch.
-  Merge the branch onto ``main``.
+  Merge the branch into ``main``.
 
 Tag and release
 ---------------
 - If the ``__version__`` in ``kikuchipy/release.py`` on ``main`` has changed in a new
   commit, a tagged, annotated release *draft* is automatically created.
   If ``__version__`` is now "0.42.0", the release name is "kikuchipy 0.42.0", and the
   tag name is "v0.42.0".
@@ -47,15 +47,15 @@
   before publishing.
 
 - Monitor the publish workflow to ensure the release is successfully published to PyPI.
 
 Post-release action
 -------------------
 - Monitor the `documentation build <https://readthedocs.org/projects/kikuchipy/builds>`__
-  ensure that the new stable documentation is successfully built from the release.
+  to ensure that the new stable documentation is successfully built from the release.
 
 - Ensure that `Zenodo <https://doi.org/10.5281/zenodo.3597646>`__ displays the new
   release.
 
 - Ensure that Binder can run the user guide notebooks by clicking the Binder badges in
   the top banner of one of the tutorials via `Read The Docs
   <https://kikuchipy.org/en/stable>`__.
```

### Comparing `kikuchipy-0.8.7/kikuchipy/__init__.py` & `kikuchipy-0.9.0/kikuchipy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,21 +103,19 @@
     "__version__",
     "_pyebsdindex_installed",
     "_pyvista_installed",
     "data",
     "detectors",
     "draw",
     "filters",
-    "generators",
     "imaging",
     "indexing",
     "io",
     "load",
     "pattern",
-    "projections",
     "release",
     "set_log_level",
     "signals",
     "simulations",
 ]
```

### Comparing `kikuchipy-0.8.7/kikuchipy/_rotation/__init__.py` & `kikuchipy-0.9.0/kikuchipy/_rotation/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_rotation/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/_rotation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_rotation/tests/test_rotation.py` & `kikuchipy-0.9.0/kikuchipy/_rotation/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_util/__init__.py` & `kikuchipy-0.9.0/kikuchipy/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_util/_deprecated.py` & `kikuchipy-0.9.0/kikuchipy/_util/_deprecated.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_util/_transfer_axes.py` & `kikuchipy-0.9.0/kikuchipy/_util/_transfer_axes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_util/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/_util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_util/tests/test_deprecated.py` & `kikuchipy-0.9.0/kikuchipy/_util/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/_util/tests/test_import.py` & `kikuchipy-0.9.0/kikuchipy/_util/tests/test_import.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,24 +75,14 @@
         for obj_name in kikuchipy.filters.__all__:
             getattr(kikuchipy.filters, obj_name)
         with pytest.raises(
             AttributeError, match="module 'kikuchipy.filters' has no attribute 'foo'"
         ):
             _ = kikuchipy.filters.foo
 
-    def test_import_generators(self):
-        import kikuchipy.generators
-
-        for obj_name in kikuchipy.generators.__all__:
-            getattr(kikuchipy.generators, obj_name)
-        with pytest.raises(
-            AttributeError, match="module 'kikuchipy.generators' has no attribute 'foo'"
-        ):
-            _ = kikuchipy.generators.foo
-
     def test_import_imaging(self):
         import kikuchipy.imaging
 
         for obj_name in kikuchipy.imaging.__all__:
             getattr(kikuchipy.imaging, obj_name)
         with pytest.raises(
             AttributeError, match="module 'kikuchipy.imaging' has no attribute 'foo'"
@@ -140,25 +130,14 @@
         for obj_name in kikuchipy.pattern.__all__:
             getattr(kikuchipy.pattern, obj_name)
         with pytest.raises(
             AttributeError, match="module 'kikuchipy.pattern' has no attribute 'foo'"
         ):
             _ = kikuchipy.pattern.foo
 
-    def test_import_projections(self):
-        import kikuchipy.projections
-
-        for obj_name in kikuchipy.projections.__all__:
-            getattr(kikuchipy.projections, obj_name)
-        with pytest.raises(
-            AttributeError,
-            match="module 'kikuchipy.projections' has no attribute 'foo'",
-        ):
-            _ = kikuchipy.projections.foo
-
     def test_import_signals(self):
         import kikuchipy.signals
 
         for obj_name in kikuchipy.signals.__all__:
             getattr(kikuchipy.signals, obj_name)
         with pytest.raises(
             AttributeError, match="module 'kikuchipy.signals' has no attribute 'foo'"
@@ -194,21 +173,19 @@
             "__version__",
             "_pyebsdindex_installed",
             "_pyvista_installed",
             "data",
             "detectors",
             "draw",
             "filters",
-            "generators",
             "imaging",
             "indexing",
             "io",
             "load",
             "pattern",
-            "projections",
             "release",
             "set_log_level",
             "signals",
             "simulations",
         ]
 
     def test_dir_data(self):
@@ -219,17 +196,14 @@
             "ni_gain",
             "ni_gain_calibration",
             "nickel_ebsd_large",
             "nickel_ebsd_master_pattern_small",
             "nickel_ebsd_small",
             "si_ebsd_moving_screen",
             "si_wafer",
-            "silicon_ebsd_moving_screen_in",
-            "silicon_ebsd_moving_screen_out10mm",
-            "silicon_ebsd_moving_screen_out5mm",
         ]
 
     def test_dir_detectors(self):
         import kikuchipy.detectors
 
         assert dir(kikuchipy.detectors) == ["EBSDDetector", "PCCalibrationMovingScreen"]
 
@@ -248,21 +222,14 @@
             "Window",
             "distance_to_origin",
             "highpass_fft_filter",
             "lowpass_fft_filter",
             "modified_hann",
         ]
 
-    def test_dir_generators(self):
-        import kikuchipy.generators
-
-        assert dir(kikuchipy.generators) == [
-            "VirtualBSEGenerator",
-        ]
-
     def test_dir_imaging(self):
         import kikuchipy.imaging
 
         assert dir(kikuchipy.imaging) == [
             "VirtualBSEImager",
         ]
 
@@ -318,24 +285,14 @@
             "get_image_quality",
             "ifft",
             "normalize_intensity",
             "remove_dynamic_background",
             "rescale_intensity",
         ]
 
-    def test_dir_projections(self):
-        import kikuchipy.projections
-
-        assert dir(kikuchipy.projections) == [
-            "GnomonicProjection",
-            "HesseNormalForm",
-            "LambertProjection",
-            "SphericalProjection",
-        ]
-
     def test_dir_signals(self):
         import kikuchipy.signals
 
         assert dir(kikuchipy.signals) == [
             "EBSD",
             "EBSDMasterPattern",
             "ECPMasterPattern",
```

### Comparing `kikuchipy-0.8.7/kikuchipy/_util/tests/test_logging.py` & `kikuchipy-0.9.0/kikuchipy/_util/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/conftest.py` & `kikuchipy-0.9.0/kikuchipy/conftest.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/__init__.py` & `kikuchipy-0.9.0/kikuchipy/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,14 @@
     "ni_gain",
     "ni_gain_calibration",
     "nickel_ebsd_large",
     "nickel_ebsd_master_pattern_small",
     "nickel_ebsd_small",
     "si_wafer",
     "si_ebsd_moving_screen",
-    "silicon_ebsd_moving_screen_in",
-    "silicon_ebsd_moving_screen_out10mm",
-    "silicon_ebsd_moving_screen_out5mm",
 ]
 
 
 def __dir__():
     return sorted(__all__)
 
 
@@ -56,17 +53,14 @@
         "ni_gain": "_data",
         "ni_gain_calibration": "_data",
         "nickel_ebsd_large": "_data",
         "nickel_ebsd_master_pattern_small": "_data",
         "nickel_ebsd_small": "_data",
         "si_wafer": "_data",
         "si_ebsd_moving_screen": "_data",
-        "silicon_ebsd_moving_screen_in": "_data",
-        "silicon_ebsd_moving_screen_out10mm": "_data",
-        "silicon_ebsd_moving_screen_out5mm": "_data",
     }
     if name in __all__:
         import importlib
 
         if name in _import_mapping.keys():
             import_path = f"{__name__}.{_import_mapping.get(name)}"
             return getattr(importlib.import_module(import_path), name)
```

### Comparing `kikuchipy-0.8.7/kikuchipy/data/_data.py` & `kikuchipy-0.9.0/kikuchipy/data/_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import hyperspy.api as hs
 import pooch
 
 from kikuchipy.signals import EBSD, EBSDMasterPattern
 from kikuchipy import load
 from kikuchipy.release import version
 from kikuchipy.data._registry import registry_hashes, registry_urls
-from kikuchipy._util import deprecated
 
 
 marshall = pooch.create(
     path=pooch.os_cache("kikuchipy"),
     base_url="",
     version=version.replace(".dev", "+"),
     version_dev="develop",
@@ -318,178 +317,14 @@
 
     SiEBSDMovingScreen = Dataset(f"silicon_ebsd_moving_screen/si_{suffix}.h5")
     file_path = SiEBSDMovingScreen.fetch_file_path(allow_download, show_progressbar)
 
     return load(file_path, **kwargs)
 
 
-@deprecated("0.8", "si_ebsd_moving_screen", removal="0.9")
-def silicon_ebsd_moving_screen_in(
-    allow_download: bool = False, show_progressbar: Optional[bool] = None, **kwargs
-) -> EBSD:
-    """One EBSD pattern of (480, 480) pixels from a single crystal
-    silicon sample, acquired on a NORDIF UF-420 detector
-    :cite:`aanes2022electron3`.
-
-    This pattern and two other patterns from the same sample position
-    but with 5 mm and 10 mm greater sample-screen-distances were
-    acquired to test the moving-screen projection center estimation
-    technique :cite:`hjelen1991electron`.
-
-    Parameters
-    ----------
-    allow_download
-        Whether to allow downloading the dataset from the internet to
-        the local cache with the pooch Python package. Default is
-        ``False``.
-    show_progressbar
-        Whether to show a progressbar when downloading. If not given,
-        the value of
-        :obj:`hyperspy.api.preferences.General.show_progressbar` is
-        used.
-    **kwargs
-        Keyword arguments passed to :func:`~kikuchipy.load`.
-
-    Returns
-    -------
-    ebsd_signal
-        EBSD signal.
-
-    Notes
-    -----
-    The dataset is hosted in the GitHub repository
-    https://github.com/pyxem/kikuchipy-data.
-
-    The dataset carries a CC BY 4.0 license.
-
-    Examples
-    --------
-    >>> import kikuchipy as kp
-    >>> s = kp.data.si_ebsd_moving_screen(0, allow_download=True)
-    >>> s
-    <EBSD, title: si_in Scan 1, dimensions: (|480, 480)>
-    >>> s.plot()
-    """
-    SiEBSDMovingScreenIn = Dataset("silicon_ebsd_moving_screen/si_in.h5")
-    file_path = SiEBSDMovingScreenIn.fetch_file_path(allow_download, show_progressbar)
-    return load(file_path, **kwargs)
-
-
-@deprecated("0.8", "si_ebsd_moving_screen", removal="0.9")
-def silicon_ebsd_moving_screen_out5mm(
-    allow_download: bool = False, show_progressbar: Optional[bool] = None, **kwargs
-) -> EBSD:
-    """One EBSD pattern of (480, 480) pixels from a single crystal
-    silicon sample, acquired on a NORDIF UF-420 detector
-    :cite:`aanes2022electron3`.
-
-    This pattern and two other patterns from the same sample position
-    but with sample-screen-distances 5 mm shorter
-    (:func:`silicon_ebsd_moving_screen_in`) and 5 mm greater
-    (:func:`silicon_ebsd_moving_screen_out10mm`) were acquired to test
-    the moving-screen projection center estimation technique
-    :cite:`hjelen1991electron`.
-
-    Parameters
-    ----------
-    allow_download
-        Whether to allow downloading the dataset from the internet to
-        the local cache with the pooch Python package. Default is
-        ``False``.
-    show_progressbar
-        Whether to show a progressbar when downloading. If not given,
-        the value of
-        :obj:`hyperspy.api.preferences.General.show_progressbar` is
-        used.
-    **kwargs
-        Keyword arguments passed to :func:`~kikuchipy.load`.
-
-    Returns
-    -------
-    ebsd_signal
-        EBSD signal.
-
-    Notes
-    -----
-    The dataset is hosted in the GitHub repository
-    https://github.com/pyxem/kikuchipy-data.
-
-    The dataset carries a CC BY 4.0 license.
-
-    Examples
-    --------
-    >>> import kikuchipy as kp
-    >>> s = kp.data.si_ebsd_moving_screen(5, allow_download=True)
-    >>> s
-    <EBSD, title: si_out5mm Scan 1, dimensions: (|480, 480)>
-    >>> s.plot()
-    """
-    SiEBSDMovingScreenOut5mm = Dataset("silicon_ebsd_moving_screen/si_out5mm.h5")
-    file_path = SiEBSDMovingScreenOut5mm.fetch_file_path(
-        allow_download, show_progressbar
-    )
-    return load(file_path, **kwargs)
-
-
-@deprecated("0.8", "si_ebsd_moving_screen", removal="0.9")
-def silicon_ebsd_moving_screen_out10mm(
-    allow_download: bool = False, show_progressbar: Optional[bool] = None, **kwargs
-) -> EBSD:
-    """One EBSD pattern of (480, 480) pixels from a single crystal
-    silicon sample, acquired on a NORDIF UF-420 detector
-    :cite:`aanes2022electron3`.
-
-    This pattern and two other patterns from the same sample position
-    but with sample-screen-distances 10 mm shorter
-    (:func:`silicon_ebsd_moving_screen_in`) and 5 mm shorter
-    (:func:`silicon_ebsd_moving_screen_out5mm`) were acquired to test
-    the moving-screen projection center estimation technique
-    :cite:`hjelen1991electron`.
-
-    Parameters
-    ----------
-    allow_download
-        Whether to allow downloading the dataset from the internet to
-        the local cache with the pooch Python package. Default is
-        ``False``.
-    show_progressbar
-        Whether to show a progressbar when downloading. If not given,
-        the value of
-        :obj:`hyperspy.api.preferences.General.show_progressbar` is
-        used.
-    **kwargs
-        Keyword arguments passed to :func:`~kikuchipy.load`.
-
-    Returns
-    -------
-    ebsd_signal
-        EBSD signal.
-
-    Notes
-    -----
-    The dataset is hosted in the GitHub repository
-    https://github.com/pyxem/kikuchipy-data.
-
-    The dataset carries a CC BY 4.0 license.
-
-    Examples
-    --------
-    >>> import kikuchipy as kp
-    >>> s = kp.data.si_ebsd_moving_screen(10, allow_download=True)
-    >>> s
-    <EBSD, title: si_out10mm Scan 1, dimensions: (|480, 480)>
-    >>> s.plot()
-    """
-    SiEBSDMovingScreenOut10mm = Dataset("silicon_ebsd_moving_screen/si_out10mm.h5")
-    file_path = SiEBSDMovingScreenOut10mm.fetch_file_path(
-        allow_download, show_progressbar
-    )
-    return load(file_path, **kwargs)
-
-
 def si_wafer(
     allow_download: bool = False, show_progressbar: Optional[bool] = None, **kwargs
 ) -> EBSD:
     """EBSD dataset of (50, 50) patterns of (480, 480) pixels from a
     single crystal silicon wafer, acquired on a NORDIF UF-420 detector
     :cite:`aanes2022electron3`.
 
@@ -765,20 +600,20 @@
         else:
             return None
 
     def fetch_file_path_from_collection(
         self, downloader: pooch.HTTPDownloader
     ) -> file_path:  # pragma: no cover
         file_paths = marshall.fetch(
-            os.path.join("data", self.collection_name),
+            "data/" + self.collection_name,
             downloader=downloader,
             processor=pooch.Unzip(extract_dir=self.file_directory),
         )
 
-        os.remove(os.path.join(marshall.path, "data", self.collection_name))
+        os.remove(Path(marshall.path) / "data" / self.collection_name)
 
         # Ensure the file is in the collection
         desired_name = self.file_relpath.name
         for fpath in map(Path, file_paths):
             if desired_name == fpath.name:
                 break
         else:
```

### Comparing `kikuchipy-0.8.7/kikuchipy/data/_registry.py` & `kikuchipy-0.9.0/kikuchipy/data/_registry.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py` & `kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/patterns.h5` & `kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5` & `kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5` & `kikuchipy-0.9.0/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py` & `kikuchipy-0.9.0/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/edax_binary/edax_binary.up1` & `kikuchipy-0.9.0/kikuchipy/data/edax_binary/edax_binary.up1`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/edax_binary/edax_binary.up2` & `kikuchipy-0.9.0/kikuchipy/data/edax_binary/edax_binary.up2`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/edax_h5ebsd/patterns.h5` & `kikuchipy-0.9.0/kikuchipy/data/edax_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5` & `kikuchipy-0.9.0/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5` & `kikuchipy-0.9.0/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5` & `kikuchipy-0.9.0/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Background acquisition pattern.bmp` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Background acquisition pattern.bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Background calibration pattern.bmp` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Background calibration pattern.bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Calibration (294,532).bmp` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Calibration (294,532).bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Calibration (425,447).bmp` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Calibration (425,447).bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Pattern.dat` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Pattern.dat`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Setting.txt` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Setting.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Setting_bad1.txt` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Setting_bad1.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Setting_bad2.txt` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Setting_bad2.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/nordif/Setting_bad3.txt` & `kikuchipy-0.9.0/kikuchipy/data/nordif/Setting_bad3.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py` & `kikuchipy-0.9.0/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/oxford_binary/patterns.ebsp` & `kikuchipy-0.9.0/kikuchipy/data/oxford_binary/patterns.ebsp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py` & `kikuchipy-0.9.0/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/oxford_h5ebsd/patterns.h5oina` & `kikuchipy-0.9.0/kikuchipy/data/oxford_h5ebsd/patterns.h5oina`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/data/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/data/tests/test_data.py` & `kikuchipy-0.9.0/kikuchipy/data/tests/test_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,62 +113,23 @@
         """Download from external."""
         s = kp.data.nickel_ebsd_large(lazy=True, allow_download=True)
 
         assert isinstance(s, kp.signals.LazyEBSD)
         assert s.data.shape == (55, 75, 60, 60)
         assert np.issubdtype(s.data.dtype, np.uint8)
 
-    # TODO: Remove test after 0.8 is released
-    def test_load_si_ebsd_moving_screen_in(self):
-        """Download external Si pattern."""
-        with pytest.warns(
-            np.VisibleDeprecationWarning,
-            match=r"Function `silicon_ebsd_moving_screen_in\(\)` is deprecated and ",
-        ):
-            s = kp.data.silicon_ebsd_moving_screen_in(allow_download=True)
-
-        assert s.data.shape == (480, 480)
-        assert s.data.dtype == np.uint8
-        assert isinstance(s.static_background, np.ndarray)
-
-    # TODO: Remove test after 0.8 is released
-    def test_load_si_ebsd_moving_screen_out5mm(self):
-        """Download external Si pattern."""
-        with pytest.warns(
-            np.VisibleDeprecationWarning,
-            match=r"Function `silicon_ebsd_moving_screen_out5mm\(\)` is deprecated ",
-        ):
-            s = kp.data.silicon_ebsd_moving_screen_out5mm(allow_download=True)
-
-        assert s.data.shape == (480, 480)
-        assert s.data.dtype == np.uint8
-        assert isinstance(s.static_background, np.ndarray)
-
-    # TODO: Remove test after 0.8 is released
-    def test_load_si_ebsd_moving_screen_out10mm(self):
-        """Download external Si pattern."""
-        with pytest.warns(
-            np.VisibleDeprecationWarning,
-            match=r"Function `silicon_ebsd_moving_screen_out10mm\(\)` is deprecated ",
-        ):
-            s = kp.data.silicon_ebsd_moving_screen_out10mm(allow_download=True)
-
-        assert s.data.shape == (480, 480)
-        assert s.data.dtype == np.uint8
-        assert isinstance(s.static_background, np.ndarray)
-
     def test_load_si_ebsd_moving_screen(self):
         """Download external Si pattern."""
         s = kp.data.si_ebsd_moving_screen(allow_download=True)
         assert s.data.shape == (480, 480)
         assert s.data.dtype == np.uint8
         assert isinstance(s.static_background, np.ndarray)
 
-        _ = kp.data.si_ebsd_moving_screen(5)
-        _ = kp.data.si_ebsd_moving_screen(10)
+        _ = kp.data.si_ebsd_moving_screen(5, allow_download=True)
+        _ = kp.data.si_ebsd_moving_screen(10, allow_download=True)
 
     def test_si_wafer(self):
         """Test set up of Si wafer dataset (without downloading)."""
         file_path = "si_wafer/Pattern.dat"
 
         dset = Dataset(file_path, collection_name="ebsd_si_wafer.zip")
         assert not dset.is_in_package
```

### Comparing `kikuchipy-0.8.7/kikuchipy/detectors/__init__.py` & `kikuchipy-0.9.0/kikuchipy/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/detectors/calibration.py` & `kikuchipy-0.9.0/kikuchipy/detectors/calibration.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/detectors/ebsd_detector.py` & `kikuchipy-0.9.0/kikuchipy/detectors/ebsd_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,34 +109,45 @@
     in fractions of :math:`N_x`, :math:`N_y`, and :math:`N_y`,
     respectively, with :math:`x_B^*` and :math:`y_B^*` defined with
     respect to the upper left corner of the detector. These coordinates
     are used internally, called :math:`(PC_x, PC_y, PC_z)` in the rest
     of the documentation when there is no reference to Bruker
     specifically.
 
-    The EDAX TSL PC coordinates :math:`(x_T^*, y_T^*, z_T^*)` and Oxford
-    Instruments PC coordinates :math:`(x_O^*, y_O^*, z_O^*)` are
-    identical and defined in fractions of :math:`N_x` with respect to
-    the lower left corner of the detector.
+    The EDAX TSL PC coordinates :math:`(x_T^*, y_T^*, z_T^*)` are
+    defined in fractions of :math:`(N_x, N_y, min(N_x, N_y))` with
+    respect to the lower left corner of the detector.
+
+    The Oxford Instruments PC coordinates :math:`(x_O^*, y_O^*, z_O^*)`
+    are defined in fractions of :math:`N_x` with respect to the lower
+    left corner of the detector.
 
     The EMsoft PC coordinates :math:`(x_{pc}, y_{pc})` are defined as
     number of pixels (subpixel accuracy) with respect to the center of
     the detector, with :math:`x_{pc}` towards the right and
     :math:`y_{pc}` upwards. The final PC coordinate :math:`L` is the
     detector distance in microns. Note that prior to EMsoft v5.0,
     :math:`x_{pc}` was defined towards the left.
 
-    Given these definitions, the following is the conversion from
-    TSL/Oxford to Bruker
+    Given these definitions, the following is the conversion from EDAX
+    TSL to Bruker
 
     .. math::
 
         x_B^* &= x_T^*,\\
-        y_B^* &= 1 - \frac{N_x}{N_y} y_T^*,\\
-        z_B^* &= \frac{N_x}{N_y} z_T^*.
+        y_B^* &= 1 - y_T^*,\\
+        z_B^* &= \frac{min(N_x, N_y)}{N_y} z_T^*.
+
+    The conversion from Oxford Instruments to Bruker is given as
+
+    .. math::
+
+        x_B^* &= x_O^*,\\
+        y_B^* &= 1 - y_O^* \frac{N_x}{N_y},\\
+        z_B^* &= \frac{N_x}{N_y} z_O^*.
 
     The conversion from EMsoft to Bruker is given as
 
     .. math::
 
         x_B^* &= \frac{1}{2} - \frac{x_{pc}}{N_x b},\\
         y_B^* &= \frac{1}{2} - \frac{y_{pc}}{N_y b},\\
@@ -1091,23 +1102,38 @@
             fig = None
 
         if return_figure and fig:
             return new_detector, fig
         else:
             return new_detector
 
-    def get_indexer(self, phase_list: PhaseList, **kwargs) -> "EBSDIndexer":
-        """Return a PyEBSDIndex EBSD indexer.
+    def get_indexer(
+        self,
+        phase_list: PhaseList,
+        reflectors: Optional[
+            List[Union["ReciprocalLatticeVector", np.ndarray, list, tuple, None]]
+        ] = None,
+        **kwargs,
+    ) -> "EBSDIndexer":
+        r"""Return a PyEBSDIndex EBSD indexer.
 
         Parameters
         ----------
         phase_list
             List of phases. :class:`~pyebsdindex.ebsd_index.EBSDIndexer`
             only supports a list containing one face-centered cubic
             (FCC) phase, one body-centered cubic (BCC) phase or both.
+        reflectors
+            List of reflectors or pole families :math:`\{hkl\}` to use
+            in indexing for each phase. If not passed, the default in
+            :func:`pyebsdindex.tripletvote.addphase` is used. For each
+            phase, the reflectors can either be a NumPy array, a list,
+            a tuple, a
+            :class:`~diffsis.crystallography.ReciprocalLatticeVector`,
+            or None.
         **kwargs
             Keyword arguments passed to
             :class:`~pyebsdindex.ebsd_index.EBSDIndexer`, except for the
             following arguments which cannot be passed since they are
             determined from the detector or ``phase_list``:
             ``phaselist`` (not to be confused with ``phase_list``),
             ``vendor``, ``PC``, ``sampleTilt``, ``camElev`` and
@@ -1121,21 +1147,26 @@
             ``indexer.PC`` is set equal to :attr:`pc_flattened`.
 
         Notes
         -----
         Requires that PyEBSDIndex is installed, which is an optional
         dependency of kikuchipy. See :ref:`optional-dependencies` for
         details.
+
+        See Also
+        --------
+        pyebsdindex.tripletvote.addphase
         """
         return _get_indexer_from_detector(
             phase_list=phase_list,
             shape=self.shape,
             pc=self.pc_flattened.squeeze(),
             sample_tilt=self.sample_tilt,
             tilt=self.tilt,
+            reflectors=reflectors,
             **kwargs,
         )
 
     def pc_emsoft(self, version: int = 5) -> np.ndarray:
         r"""Return PC in the EMsoft convention.
 
         Parameters
@@ -1238,21 +1269,16 @@
     def pc_oxford(self) -> np.ndarray:
         """Return PC in the Oxford convention.
 
         Returns
         -------
         new_pc
             PC in the Oxford convention.
-
-        Notes
-        -----
-        The Oxford PC coordinates are identical to the TSL coordinates,
-        see :meth:`pc_tsl`.
         """
-        return self._pc_bruker2tsl()
+        return self._pc_bruker2oxford()
 
     def plot(
         self,
         coordinates: str = "detector",
         show_pc: bool = True,
         pc_kwargs: Optional[dict] = None,
         pattern: Optional[np.ndarray] = None,
@@ -1641,16 +1667,18 @@
         -------
         pc
             PC array in Bruker's convention.
         """
         conv = convention.lower()
         if conv in CONVENTION_ALIAS["bruker"]:
             return self.pc
-        elif conv in CONVENTION_ALIAS["tsl"] + CONVENTION_ALIAS["oxford"]:
+        elif conv in CONVENTION_ALIAS["tsl"]:
             return self._pc_tsl2bruker()
+        elif conv in CONVENTION_ALIAS["oxford"]:
+            return self._pc_oxford2bruker()
         elif conv in CONVENTION_ALIAS["emsoft"]:
             try:
                 version = int(convention[-1])
             except ValueError:
                 version = 5
             return self._pc_emsoft2bruker(version)
         else:
@@ -1676,16 +1704,18 @@
         -------
         pc
             PC array in specified convention.
         """
         conv = convention.lower()
         if conv in CONVENTION_ALIAS["bruker"]:
             return self.pc
-        elif conv in CONVENTION_ALIAS["tsl"] + CONVENTION_ALIAS["oxford"]:
+        elif conv in CONVENTION_ALIAS["tsl"]:
             return self._pc_bruker2tsl()
+        elif conv in CONVENTION_ALIAS["oxford"]:
+            return self._pc_bruker2oxford()
         elif conv in CONVENTION_ALIAS["emsoft"]:
             try:
                 version = int(convention[-1])
             except ValueError:
                 version = 5
             return self._pc_bruker2emsoft(version)
         else:
@@ -1702,14 +1732,20 @@
         new_pc[..., 0] = 0.5 - (pcx / (self.ncols * self.binning))
         new_pc[..., 1] = 0.5 - (self.pcy / (self.nrows * self.binning))
         new_pc[..., 2] = self.pcz / (self.nrows * self.binning * self.px_size)
         return new_pc
 
     def _pc_tsl2bruker(self) -> np.ndarray:
         new_pc = deepcopy(self.pc)
+        new_pc[..., 1] = 1 - self.pcy
+        new_pc[..., 2] *= min([self.nrows, self.ncols]) / self.nrows
+        return new_pc
+
+    def _pc_oxford2bruker(self) -> np.ndarray:
+        new_pc = deepcopy(self.pc)
         new_pc[..., 1] = 1 - self.pcy * self.aspect_ratio
         new_pc[..., 2] *= self.aspect_ratio
         return new_pc
 
     def _pc_bruker2emsoft(self, version: int = 5) -> np.ndarray:
         new_pc = np.zeros_like(self.pc, dtype=float)
         new_pc[..., 0] = (0.5 - self.pcx) * self.ncols * self.binning
@@ -1717,14 +1753,20 @@
             new_pc[..., 0] = -new_pc[..., 0]
         new_pc[..., 1] = (0.5 - self.pcy) * self.nrows * self.binning
         new_pc[..., 2] = self.pcz * self.nrows * self.binning * self.px_size
         return new_pc
 
     def _pc_bruker2tsl(self) -> np.ndarray:
         new_pc = deepcopy(self.pc)
+        new_pc[..., 1] = 1 - self.pcy
+        new_pc[..., 2] /= min([self.nrows, self.ncols]) / self.nrows
+        return new_pc
+
+    def _pc_bruker2oxford(self) -> np.ndarray:
+        new_pc = deepcopy(self.pc)
         new_pc[..., 1] = (1 - self.pcy) / self.aspect_ratio
         new_pc[..., 2] /= self.aspect_ratio
         return new_pc
 
 
 def _fit_hyperplane(
     pc_centered: np.ndarray,
```

### Comparing `kikuchipy-0.8.7/kikuchipy/detectors/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/detectors/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/detectors/tests/test_calibration.py` & `kikuchipy-0.9.0/kikuchipy/detectors/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/detectors/tests/test_ebsd_detector.py` & `kikuchipy-0.9.0/kikuchipy/detectors/tests/test_ebsd_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -261,34 +261,40 @@
                 4,
                 [0.50153, 0.52708, 0.66980],
             ),
             ((480, 640), [0, 0, 15000], 50, 1, 5, [0.5, 0.5, 0.625]),
         ],
     )
     def test_set_pc_from_emsoft(self, shape, pc, px_size, binning, version, desired_pc):
-        """PC EMsoft -> Bruker -> EMsoft, also checking to_tsl() and
-        to_bruker().
+        """PC EMsoft -> Bruker -> EMsoft, also checking to_tsl(),
+        to_oxford(), and to_bruker().
         """
         det = kp.detectors.EBSDDetector(
             shape=shape,
             pc=pc,
             px_size=px_size,
             binning=binning,
             convention=f"emsoft{version}",
         )
 
         assert np.allclose(det.pc, desired_pc, atol=1e-5)
         assert np.allclose(det.pc_emsoft(version=version), pc, atol=1e-5)
         assert np.allclose(det.pc_bruker(), desired_pc, atol=1e-5)
 
+        # EDAX
         pc_tsl = deepcopy(det.pc)
         pc_tsl[..., 1] = 1 - pc_tsl[..., 1]
-        pc_tsl[..., 1:] /= det.aspect_ratio
+        pc_tsl[..., 2] /= min([det.nrows, det.ncols]) / det.nrows
         assert np.allclose(det.pc_tsl(), pc_tsl, atol=1e-5)
-        assert np.allclose(det.pc_oxford(), pc_tsl, atol=1e-5)
+
+        # Oxford
+        pc_oxford = deepcopy(det.pc)
+        pc_oxford[..., 1] = 1 - pc_oxford[..., 1]
+        pc_oxford[..., 1:] /= det.aspect_ratio
+        assert np.allclose(det.pc_oxford(), pc_oxford, atol=1e-5)
 
     def test_set_pc_from_emsoft_no_version(self):
         """PC EMsoft -> Bruker, no EMsoft version specified gives v5."""
         assert np.allclose(
             kp.detectors.EBSDDetector(
                 shape=(60, 60),
                 pc=[3.4848, 114.2016, 15767.7],
@@ -300,35 +306,53 @@
             atol=1e-5,
         )
 
     @pytest.mark.parametrize(
         "shape, pc, convention, desired_pc",
         [
             ((60, 60), [0.35, 1, 0.65], "tsl", [0.35, 0, 0.65]),
-            ((60, 80), [0.35, 1, 0.65], "tsl", [0.35, -0.33, 0.87]),
-            ((60, 60), [0.25, 0, 0.75], "oxford", [0.25, 1, 0.75]),
-            ((60, 80), [0.25, 0, 0.75], "oxford", [0.25, 1, 1]),
+            ((60, 80), [0.35, 1, 0.65], "tsl", [0.35, 0, 0.65]),
             ((60, 60), [0.1, 0.2, 0.3], "amatek", [0.1, 0.8, 0.3]),
-            ((60, 80), [0.1, 0.2, 0.3], "amatek", [0.1, 0.73, 0.4]),
+            ((60, 80), [0.1, 0.2, 0.3], "amatek", [0.1, 0.8, 0.3]),
             ((60, 60), [0.6, 0.6, 0.6], "edax", [0.6, 0.4, 0.6]),
-            ((60, 80), [0.6, 0.6, 0.6], "edax", [0.6, 0.2, 0.8]),
+            ((60, 80), [0.6, 0.6, 0.6], "edax", [0.6, 0.4, 0.6]),
         ],
     )
-    def test_set_pc_from_tsl_oxford(self, shape, pc, convention, desired_pc):
+    def test_set_pc_from_tsl(self, shape, pc, convention, desired_pc):
         """PC TSL -> Bruker -> TSL."""
         det = kp.detectors.EBSDDetector(shape=shape, pc=pc, convention=convention)
         assert np.allclose(det.pc, desired_pc, atol=1e-2)
         assert np.allclose(det.pc_tsl(), pc, atol=1e-3)
         assert np.allclose(
             kp.detectors.EBSDDetector(pc=det.pc_tsl(), convention="tsl").pc_tsl(),
             pc,
             atol=1e-2,
         )
 
     @pytest.mark.parametrize(
+        "shape, pc, desired_pc",
+        [
+            ((60, 60), [0.25, 0, 0.75], [0.25, 1, 0.75]),
+            ((60, 80), [0.25, 0, 0.75], [0.25, 1, 1]),
+        ],
+    )
+    def test_set_pc_from_oxford(self, shape, pc, desired_pc):
+        """PC Oxford -> Bruker -> Oxford."""
+        det = kp.detectors.EBSDDetector(shape=shape, pc=pc, convention="oxford")
+        assert np.allclose(det.pc, desired_pc, atol=1e-2)
+        assert np.allclose(det.pc_oxford(), pc, atol=1e-3)
+        assert np.allclose(
+            kp.detectors.EBSDDetector(
+                pc=det.pc_oxford(), convention="oxford"
+            ).pc_oxford(),
+            pc,
+            atol=1e-2,
+        )
+
+    @pytest.mark.parametrize(
         "pc, convention",
         [
             ([0.35, 1, 0.65], None),
             ([0.25, 0, 0.75], None),
             ([0.1, 0.2, 0.3], "Bruker"),
             ([0.6, 0.6, 0.6], "bruker"),
         ],
@@ -1024,64 +1048,52 @@
         with pytest.raises(ValueError, match="pyebsdindex must be installed. Install "):
             _ = self.det.get_indexer(pl)
 
     @pytest.mark.skipif(
         not kp._pyebsdindex_installed, reason="pyebsdindex is not installed"
     )
     def test_get_indexer_invalid_phase_lists(self):
-        # More than two phases
-        with pytest.raises(ValueError, match="Hough indexing only supports indexing "):
-            _ = self.det.get_indexer(
-                PhaseList(names=["a", "b", "c"], space_groups=[225, 227, 229])
-            )
-
         # Not all phases have space groups
         pl = PhaseList(names=["a", "b"], point_groups=["m-3m", "432"])
         pl["a"].space_group = 225
         with pytest.raises(ValueError, match="Space group for each phase must be set,"):
             _ = self.det.get_indexer(pl)
 
-        # Not FCC or BCC
-        with pytest.raises(ValueError, match="Hough indexing only supports indexing "):
-            _ = self.det.get_indexer(PhaseList(names="sic", space_groups=186))
-
     @pytest.mark.skipif(
         not kp._pyebsdindex_installed, reason="pyebsdindex is not installed"
     )
     def test_get_indexer(self):
-        indexer1 = self.det.get_indexer(
-            PhaseList(names=["a", "b"], space_groups=[225, 229]), nBands=6
-        )
-        assert indexer1.vendor == "KIKUCHIPY"
-        assert np.isclose(indexer1.sampleTilt, self.det.sample_tilt)
-        assert np.isclose(indexer1.camElev, self.det.tilt)
-        assert tuple(indexer1.bandDetectPlan.patDim) == self.det.shape
-        assert indexer1.bandDetectPlan.nBands == 6
-        assert np.allclose(indexer1.PC, self.det.pc_flattened)
-        assert indexer1.phaselist == ["FCC", "BCC"]
-
-        indexer2 = self.det.get_indexer(PhaseList(names="a", space_groups=225))
-        assert indexer2.phaselist == ["FCC"]
-
-        indexer3 = self.det.get_indexer(PhaseList(names="a", space_groups=220))
-        assert indexer3.phaselist == ["BCC"]
+        # fmt: off
+        #               -1  2/m  222   -3   -3m   4/m   4/mmm   6/m  6/mmm    m-3  m-3m
+        space_groups = [ 1,  15,  74,  75,  142,  143,    167,  168,   194,   195,  207]
+        laue_codes =   [ 1,   2,  22,   4,   42,    3,     32,    6,    62,    23,   43]
+        # fmt: on
+        names = "abcdefghijk"
 
-        indexer4 = self.det.get_indexer(
-            PhaseList(names=["a", "b"], space_groups=[220, 225])
-        )
-        assert indexer4.phaselist == ["BCC", "FCC"]
+        pl = PhaseList(names=list(names), space_groups=space_groups)
+        indexer = self.det.get_indexer(pl, nBands=6)
+        assert indexer.vendor == "KIKUCHIPY"
+        assert np.isclose(indexer.sampleTilt, self.det.sample_tilt)
+        assert np.isclose(indexer.camElev, self.det.tilt)
+        assert tuple(indexer.bandDetectPlan.patDim) == self.det.shape
+        assert indexer.bandDetectPlan.nBands == 6
+        assert np.allclose(indexer.PC, self.det.pc_flattened)
+        for phase, sg, code in zip(indexer.phaselist, pl.space_groups, laue_codes):
+            assert phase.spacegroup == sg.number
+            assert phase.lauecode == code
 
 
 class TestSaveLoadDetector:
     @pytest.mark.parametrize(
         "nav_shape, shape, convention, sample_tilt, tilt, px_size, binning, azimuthal",
         [
             ((3, 4), (10, 20), "bruker", 70, 0, 70, 1, 0),
             ((1, 5), (5, 5), "tsl", 69.5, 3.14, 57.2, 2, 3.7),
             ((4, 3), (6, 7), "emsoft", -69.5, -3.14, 57.2, 2, -3.7),
+            ((3, 2), (5, 7), "oxford", 71.3, 1.2, 90.3, 3, 0.1),
         ],
     )
     def test_save_load_detector(
         self,
         tmp_path,
         nav_shape,
         shape,
```

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/__init__.py` & `kikuchipy-0.9.0/kikuchipy/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/_navigators.py` & `kikuchipy-0.9.0/kikuchipy/draw/_navigators.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/_plot_pattern_positions_in_map.py` & `kikuchipy-0.9.0/kikuchipy/draw/_plot_pattern_positions_in_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/colors.py` & `kikuchipy-0.9.0/kikuchipy/draw/colors.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/markers.py` & `kikuchipy-0.9.0/kikuchipy/draw/markers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/draw/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/tests/test_colors.py` & `kikuchipy-0.9.0/kikuchipy/draw/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/tests/test_markers.py` & `kikuchipy-0.9.0/kikuchipy/draw/tests/test_markers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/tests/test_navigators.py` & `kikuchipy-0.9.0/kikuchipy/draw/tests/test_navigators.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py` & `kikuchipy-0.9.0/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/filters/__init__.py` & `kikuchipy-0.9.0/kikuchipy/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/filters/fft_barnes.py` & `kikuchipy-0.9.0/kikuchipy/filters/fft_barnes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/filters/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/filters/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/filters/tests/test_fft_barnes.py` & `kikuchipy-0.9.0/kikuchipy/filters/tests/test_fft_barnes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/filters/tests/test_window.py` & `kikuchipy-0.9.0/kikuchipy/filters/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/filters/window.py` & `kikuchipy-0.9.0/kikuchipy/filters/window.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/generators/__init__.py` & `kikuchipy-0.9.0/kikuchipy/imaging/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,31 +11,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
-"""*[Deprecated]* Generate signals from other signals.
-
-Use :mod:`kikuchipy.imaging` instead.
-"""
+"""Imaging using the EBSD detector."""
 
 __all__ = [
-    "VirtualBSEGenerator",
+    "VirtualBSEImager",
 ]
 
 
 def __dir__():
     return sorted(__all__)
 
 
 def __getattr__(name):
     _import_mapping = {
-        "VirtualBSEGenerator": "virtual_bse_generator",
+        "VirtualBSEImager": "vbse",
     }
     if name in __all__:
         import importlib
 
         if name in _import_mapping.keys():
             import_path = f"{__name__}.{_import_mapping.get(name)}"
             return getattr(importlib.import_module(import_path), name)
```

### Comparing `kikuchipy-0.8.7/kikuchipy/generators/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/imaging/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/generators/tests/test_virtual_bse_generator.py` & `kikuchipy-0.9.0/kikuchipy/imaging/tests/test_virtual_bse_imager.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,44 +14,37 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
 import os
 
 from hyperspy.roi import RectangularROI
-from matplotlib.pyplot import close
+import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 
-from kikuchipy import load
-from kikuchipy.generators import VirtualBSEGenerator
-from kikuchipy.signals import EBSD, LazyEBSD, VirtualBSEImage
+import kikuchipy as kp
 
 
 DIR_PATH = os.path.dirname(__file__)
 KIKUCHIPY_FILE = os.path.join(DIR_PATH, "../../data/kikuchipy_h5ebsd/patterns.h5")
 
 
-@pytest.mark.filterwarnings("ignore:Class `VirtualBSEGenerator` ")
-class TestVirtualBSEGenerator:
+class TestVirtualBSEImager:
     def test_init(self, dummy_signal):
-        with pytest.warns(
-            np.VisibleDeprecationWarning,
-            match="Class `VirtualBSEGenerator` is deprecated and will be removed in ",
-        ):
-            vbse_gen = VirtualBSEGenerator(dummy_signal)
+        vbse_imager = kp.imaging.VirtualBSEImager(dummy_signal)
 
-        assert isinstance(vbse_gen.signal, EBSD)
-        assert vbse_gen.grid_shape == (5, 5)
+        assert isinstance(vbse_imager.signal, kp.signals.EBSD)
+        assert vbse_imager.grid_shape == (5, 5)
 
     def test_init_lazy(self, dummy_signal):
         lazy_signal = dummy_signal.as_lazy()
-        vbse_gen = VirtualBSEGenerator(lazy_signal)
+        vbse_imager = kp.imaging.VirtualBSEImager(lazy_signal)
 
-        assert isinstance(vbse_gen.signal, LazyEBSD)
+        assert isinstance(vbse_imager.signal, kp.signals.LazyEBSD)
 
     @pytest.mark.parametrize(
         "grid_shape, desired_rows, desired_cols",
         [
             (
                 (10, 10),
                 np.linspace(0, 60, 10 + 1),
@@ -61,216 +54,218 @@
                 (13, 7),
                 np.linspace(0, 60, 13 + 1),
                 np.linspace(0, 60, 7 + 1),
             ),
         ],
     )
     def test_set_grid_shape(self, grid_shape, desired_rows, desired_cols):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
-        vbse_gen.grid_shape = grid_shape
-
-        assert vbse_gen.grid_shape == grid_shape
-        assert np.allclose(vbse_gen.grid_rows, desired_rows)
-        assert np.allclose(vbse_gen.grid_cols, desired_cols)
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
+        vbse_imager.grid_shape = grid_shape
+
+        assert vbse_imager.grid_shape == grid_shape
+        assert np.allclose(vbse_imager.grid_rows, desired_rows)
+        assert np.allclose(vbse_imager.grid_cols, desired_cols)
 
     def test_repr(self, dummy_signal):
-        vbse_gen = VirtualBSEGenerator(dummy_signal)
+        vbse_imager = kp.imaging.VirtualBSEImager(dummy_signal)
 
-        assert vbse_gen.__repr__() == (
-            "VirtualBSEGenerator for <EBSD, title: , dimensions: (3, 3|3, 3)>"
+        assert repr(vbse_imager) == (
+            "VirtualBSEImager for <EBSD, title: , dimensions: (3, 3|3, 3)>"
         )
 
     @pytest.mark.parametrize(
         "grid_shape, desired_n_markers",
         [((3, 3), 9 + 3 + 8), ((1, 1), 1 + 3 + 4), ((2, 3), 6 + 3 + 7)],
     )
     def test_plot_grid(self, grid_shape, desired_n_markers):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
-        vbse_gen.grid_shape = grid_shape
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
+        vbse_imager.grid_shape = grid_shape
         rgb_channels = [(0, 0), (0, 1), (1, 0)]
         pattern_idx = (2, 2)
-        p = vbse_gen.plot_grid(pattern_idx=pattern_idx, rgb_channels=rgb_channels)
-        p2 = vbse_gen.plot_grid()
+        p = vbse_imager.plot_grid(pattern_idx=pattern_idx, rgb_channels=rgb_channels)
+        p2 = vbse_imager.plot_grid()
 
         # Check data type and values
-        assert isinstance(p, EBSD)
+        assert isinstance(p, kp.signals.EBSD)
         assert np.allclose(p.data, s.inav[pattern_idx].data)
         assert np.allclose(p2.data, s.inav[0, 0].data)
 
         # Check markers
         assert len(p.metadata.Markers) == desired_n_markers
         assert p.metadata.Markers.has_item("text")
         assert p.metadata.Markers["text"].marker._color == "r"
         assert p.metadata.Markers["horizontal_line"].marker._color == "w"
         assert p.metadata.Markers["rectangle"].marker._edgecolor == (1, 0, 0, 1)
 
-        close("all")
+        plt.close("all")
 
     @pytest.mark.parametrize("color", ["c", "m", "k"])
     def test_plot_grid_text_color(self, color):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
-        p = vbse_gen.plot_grid(color=color)
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
+        p = vbse_imager.plot_grid(color=color)
 
         assert p.metadata.Markers["text"].marker._color == color
 
-        close("all")
+        plt.close("all")
 
 
-@pytest.mark.filterwarnings("ignore:Class `VirtualBSEGenerator` ")
 class TestGetImagesFromGrid:
     def test_get_single_image_from_grid(self, dummy_signal):
-        vbse_gen = VirtualBSEGenerator(dummy_signal)
-        vbse_gen.grid_shape = (1, 1)
-        vbse_img = vbse_gen.get_images_from_grid()
+        vbse_imager = kp.imaging.VirtualBSEImager(dummy_signal)
+        vbse_imager.grid_shape = (1, 1)
+        vbse_img = vbse_imager.get_images_from_grid()
 
         assert np.allclose(vbse_img.data.mean(), 40.666668)
 
     @pytest.mark.parametrize("dtype_out", [np.float32, np.float64])
     def test_dtype_out(self, dummy_signal, dtype_out):
-        vbse_gen = VirtualBSEGenerator(dummy_signal)
-        vbse_gen.grid_shape = (1, 1)
-        vbse_images = vbse_gen.get_images_from_grid(dtype_out=dtype_out)
+        vbse_imager = kp.imaging.VirtualBSEImager(dummy_signal)
+        vbse_imager.grid_shape = (1, 1)
+        vbse_images = vbse_imager.get_images_from_grid(dtype_out=dtype_out)
 
         assert vbse_images.data.dtype == dtype_out
 
     def test_axes_manager_transfer(self):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
-        vbse_img = vbse_gen.get_images_from_grid()
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
+        vbse_img = vbse_imager.get_images_from_grid()
 
         s_nav_axes = s.axes_manager.navigation_axes
         vbse_sig_axes = vbse_img.axes_manager.signal_axes
 
         assert all([vbse_sig_axes[i].scale == s_nav_axes[i].scale for i in range(2)])
         assert all([vbse_sig_axes[i].name == s_nav_axes[i].name for i in range(2)])
         assert all([vbse_sig_axes[i].units == s_nav_axes[i].units for i in range(2)])
 
     def test_get_images_lazy(self, dummy_signal):
-        vbse_gen = VirtualBSEGenerator(dummy_signal.as_lazy())
-        vbse_img = vbse_gen.get_images_from_grid()
+        vbse_imager = kp.imaging.VirtualBSEImager(dummy_signal.as_lazy())
+        vbse_img = vbse_imager.get_images_from_grid()
 
 
-@pytest.mark.filterwarnings("ignore:Class `VirtualBSEGenerator` ")
 class TestGetRGBImage:
     def test_get_rgb_image_rois(self):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
 
         # Get channels by ROIs
-        rois1 = [vbse_gen.roi_from_grid(i) for i in np.ndindex(vbse_gen.grid_shape)][:3]
-        vbse_rgb_img1 = vbse_gen.get_rgb_image(r=rois1[0], g=rois1[1], b=rois1[2])
+        rois1 = [
+            vbse_imager.roi_from_grid(i) for i in np.ndindex(vbse_imager.grid_shape)
+        ][:3]
+        vbse_rgb_img1 = vbse_imager.get_rgb_image(r=rois1[0], g=rois1[1], b=rois1[2])
 
         # Get channels from grid tile indices
         rois2 = [(0, 0), (0, 1), (0, 2)]
-        vbse_rgb_img2 = vbse_gen.get_rgb_image(r=rois2[0], g=rois2[1], b=rois2[2])
+        vbse_rgb_img2 = vbse_imager.get_rgb_image(r=rois2[0], g=rois2[1], b=rois2[2])
 
-        assert isinstance(vbse_rgb_img1, VirtualBSEImage)
+        assert isinstance(vbse_rgb_img1, kp.signals.VirtualBSEImage)
         assert vbse_rgb_img1.data.dtype == np.dtype(
             [("R", "u1"), ("G", "u1"), ("B", "u1")]
         )
 
         vbse_rgb_img1.change_dtype("uint8")
         vbse_rgb_img2.change_dtype("uint8")
         assert np.allclose(vbse_rgb_img1.data, vbse_rgb_img2.data)
 
     def test_get_rgb_image_dtype(self):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
-        vbse_rgb_img = vbse_gen.get_rgb_image(
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
+        vbse_rgb_img = vbse_imager.get_rgb_image(
             r=(0, 0), g=(0, 1), b=(0, 2), dtype_out=np.uint16
         )
 
         assert vbse_rgb_img.data.dtype == np.dtype(
             [("R", "u2"), ("G", "u2"), ("B", "u2")]
         )
 
     @pytest.mark.parametrize(
         "percentile, desired_mean_intensity",
         [(None, 136.481481), ((1, 99), 134.740740)],
     )
     def test_get_rgb_image_contrast_stretching(
         self, percentile, desired_mean_intensity
     ):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
-        vbse_rgb_img = vbse_gen.get_rgb_image(
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
+        vbse_rgb_img = vbse_imager.get_rgb_image(
             r=(0, 0), g=(0, 1), b=(0, 2), percentiles=percentile
         )
         vbse_rgb_img.change_dtype("uint8")
 
         assert np.allclose(vbse_rgb_img.data.mean(), desired_mean_intensity)
 
     @pytest.mark.parametrize(
         "alpha_add, desired_mean_intensity", [(0, 88.5), (10, 107.9)]
     )
     def test_get_rgb_alpha(self, alpha_add, desired_mean_intensity):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
 
         alpha = np.arange(9).reshape((3, 3))
         alpha[0] += alpha_add
 
-        vbse_rgb_img = vbse_gen.get_rgb_image(r=(0, 0), g=(0, 1), b=(0, 2), alpha=alpha)
+        vbse_rgb_img = vbse_imager.get_rgb_image(
+            r=(0, 0), g=(0, 1), b=(0, 2), alpha=alpha
+        )
         vbse_rgb_img.change_dtype("uint8")
 
         assert np.allclose(vbse_rgb_img.data.mean(), desired_mean_intensity, atol=0.1)
 
     def test_get_rgb_alpha_signal(self):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
 
         vbse_img = s.get_virtual_bse_intensity(roi=RectangularROI(0, 0, 10, 10))
 
-        vbse_rgb_img1 = vbse_gen.get_rgb_image(
+        vbse_rgb_img1 = vbse_imager.get_rgb_image(
             r=(0, 1), g=(0, 2), b=(0, 3), alpha=vbse_img
         )
-        vbse_rgb_img2 = vbse_gen.get_rgb_image(
+        vbse_rgb_img2 = vbse_imager.get_rgb_image(
             r=(0, 1), g=(0, 2), b=(0, 3), alpha=vbse_img.data
         )
         vbse_rgb_img1.change_dtype("uint8")
         vbse_rgb_img2.change_dtype("uint8")
 
         assert np.allclose(vbse_rgb_img1.data, vbse_rgb_img2.data)
 
     def test_get_rgb_image_lazy(self):
-        s = load(KIKUCHIPY_FILE, lazy=True)
-        vbse_gen = VirtualBSEGenerator(s)
+        s = kp.load(KIKUCHIPY_FILE, lazy=True)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
 
-        assert isinstance(vbse_gen.signal, LazyEBSD)
+        assert isinstance(vbse_imager.signal, kp.signals.LazyEBSD)
 
-        vbse_rgb_img = vbse_gen.get_rgb_image(r=(0, 0), g=(0, 1), b=(0, 2))
+        vbse_rgb_img = vbse_imager.get_rgb_image(r=(0, 0), g=(0, 1), b=(0, 2))
 
         assert isinstance(vbse_rgb_img.data, np.ndarray)
 
     def test_get_rgb_1d(self):
-        s = EBSD(np.random.random(9 * 3600).reshape((9, 60, 60)))
-        vbse_gen = VirtualBSEGenerator(s)
+        s = kp.signals.EBSD(np.random.random(9 * 3600).reshape((9, 60, 60)))
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
 
         with pytest.raises(ValueError, match="The signal dimension cannot be "):
-            _ = vbse_gen.get_rgb_image(r=(0, 0), g=(0, 1), b=(0, 2))
+            _ = vbse_imager.get_rgb_image(r=(0, 0), g=(0, 1), b=(0, 2))
 
     @pytest.mark.parametrize(
         "r, g, b, desired_mean_intensity",
         [
             ([(0, 1), (0, 2)], [(1, 1), (1, 2)], [(2, 1), (2, 2)], 125.1),
             ([(2, 1), (2, 2)], [(3, 1), (3, 2)], [(4, 1), (4, 2)], 109.0),
         ],
     )
     def test_get_rgb_multiple_rois_per_channel(self, r, g, b, desired_mean_intensity):
-        s = load(KIKUCHIPY_FILE)
-        vbse_gen = VirtualBSEGenerator(s)
+        s = kp.load(KIKUCHIPY_FILE)
+        vbse_imager = kp.imaging.VirtualBSEImager(s)
 
-        vbse_rgb_img1 = vbse_gen.get_rgb_image(r=r, g=g, b=b)
+        vbse_rgb_img1 = vbse_imager.get_rgb_image(r=r, g=g, b=b)
         vbse_rgb_img1.change_dtype("uint8")
 
         assert np.allclose(vbse_rgb_img1.data.mean(), desired_mean_intensity, atol=0.1)
 
-        roi_r = vbse_gen.roi_from_grid(r)
-        roi_g = vbse_gen.roi_from_grid(g)
-        roi_b = vbse_gen.roi_from_grid(b)
-        vbse_rgb_img2 = vbse_gen.get_rgb_image(r=roi_r, g=roi_g, b=roi_b)
+        roi_r = vbse_imager.roi_from_grid(r)
+        roi_g = vbse_imager.roi_from_grid(g)
+        roi_b = vbse_imager.roi_from_grid(b)
+        vbse_rgb_img2 = vbse_imager.get_rgb_image(r=roi_r, g=roi_g, b=roi_b)
         vbse_rgb_img2.change_dtype("uint8")
 
         assert np.allclose(vbse_rgb_img1.data, vbse_rgb_img2.data)
```

### Comparing `kikuchipy-0.8.7/kikuchipy/generators/virtual_bse_generator.py` & `kikuchipy-0.9.0/kikuchipy/imaging/vbse.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,67 +12,52 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import List, Optional, Tuple, Union
-import warnings
 
 from dask.array import Array
 from hyperspy.drawing._markers.horizontal_line import HorizontalLine
 from hyperspy.drawing._markers.vertical_line import VerticalLine
 from hyperspy.drawing._markers.rectangle import Rectangle
 from hyperspy.drawing._markers.text import Text
 from hyperspy.roi import BaseInteractiveROI, RectangularROI
 from hyperspy._signals.signal2d import Signal2D
 import numpy as np
 
 from kikuchipy.signals import EBSD, LazyEBSD
 from kikuchipy.signals import VirtualBSEImage
+from kikuchipy.pattern import rescale_intensity
 from kikuchipy._util._transfer_axes import _transfer_navigation_axes_to_signal_axes
-from kikuchipy.imaging.vbse import _get_rgb_image
 
 
-class VirtualBSEGenerator:
-    """*[Deprecated]* Generates virtual backscatter electron (BSE)
-    images for an EBSD signal and a set of EBSD detector areas in a
-    convenient manner.
+class VirtualBSEImager:
+    """Generate virtual backscatter electron (BSE) images for an
+    electron backscatter diffraction (EBSD) signal and a set
+    of EBSD detector areas in a convenient manner.
 
     Parameters
     ----------
     signal
         EBSD signal.
 
     See Also
     --------
     kikuchipy.signals.EBSD.plot_virtual_bse_intensity,
     kikuchipy.signals.EBSD.get_virtual_bse_intensity
-
-    Notes
-    -----
-    Deprecated since version 0.8: Class ``VirtualBSEGenerator`` is
-    deprecated and will be removed in version 0.9. Use
-    :class:`~kikuchipy.imaging.VirtualBSEImager` instead.
     """
 
     def __init__(self, signal: Union[EBSD, LazyEBSD]):
         self.signal = signal
         self._grid_shape = (5, 5)
 
-        warnings.warn(
-            message=(
-                "Class `VirtualBSEGenerator` is deprecated and will be removed in "
-                "version 0.9. Use `kikuchipy.imaging.VirtualBSEImager` instead."
-            ),
-            category=np.VisibleDeprecationWarning,
-        )
-
     def __repr__(self):
-        return f"VirtualBSEGenerator for {self.signal}"
+        return self.__class__.__name__ + " for " + repr(self.signal)
 
     @property
     def grid_rows(self) -> np.ndarray:
         """Return the detector grid rows, defined by :attr:`grid_shape`."""
         gy = self.grid_shape[0]
         sy = self.signal.axes_manager.signal_shape[1]
         return np.linspace(0, sy, gy + 1)
@@ -207,15 +192,15 @@
         return vbse_rgb_image
 
     def get_images_from_grid(
         self, dtype_out: Union[str, np.dtype, type] = "float32"
     ) -> VirtualBSEImage:
         """Return an in-memory signal with a stack of virtual
         backscatter electron (BSE) images by integrating the intensities
-        within regions of interest (ROI) defined by the generator
+        within regions of interest (ROI) defined by the image generator
         :attr:`grid_shape`.
 
         Parameters
         ----------
         dtype_out
             Output data type, default is ``"float32"``.
 
@@ -226,17 +211,17 @@
 
         Examples
         --------
         >>> import kikuchipy as kp
         >>> s = kp.data.nickel_ebsd_small()
         >>> s
         <EBSD, title: patterns Scan 1, dimensions: (3, 3|60, 60)>
-        >>> vbse_gen = kp.generators.VirtualBSEGenerator(s)
-        >>> vbse_gen.grid_shape = (5, 5)
-        >>> vbse = vbse_gen.get_images_from_grid()
+        >>> vbse_imager = kp.imaging.VirtualBSEImager(s)
+        >>> vbse_imager.grid_shape = (5, 5)
+        >>> vbse = vbse_imager.get_images_from_grid()
         >>> vbse
         <VirtualBSEImage, title: , dimensions: (5, 5|3, 3)>
         """
         dtype_out = np.dtype(dtype_out)
 
         grid_shape = self.grid_shape
         new_shape = grid_shape + self.signal.axes_manager.navigation_shape[::-1]
@@ -250,16 +235,16 @@
             new_axes=vbse_images.axes_manager, old_axes=self.signal.axes_manager
         )
 
         return vbse_images
 
     def roi_from_grid(self, index: Union[Tuple, List[Tuple]]) -> RectangularROI:
         """Return a rectangular region of interest (ROI) on the EBSD
-        detector from one or multiple generator grid tile indices as
-        row(s) and column(s).
+        detector from one or multiple grid tile indices as row(s) and
+        column(s).
 
         Parameters
         ----------
         index
             Row and column of one or multiple grid tiles as a tuple or a
             list of tuples.
 
@@ -362,7 +347,120 @@
         # Get pattern and add list of markers
         if pattern_idx is None:
             pattern_idx = (0,) * axes_manager.navigation_dimension
         pattern = self.signal.inav[pattern_idx]
         pattern.add_marker(markers, permanent=True)
 
         return pattern
+
+
+def _normalize_image(
+    image: np.ndarray,
+    add_bright: int = 0,
+    contrast: float = 1.0,
+    dtype_out: Union[str, np.dtype, type] = "uint8",
+) -> np.ndarray:
+    """Normalize an image's intensities to a mean of 0 and a standard
+    deviation of 1, with the possibility to also scale by a contrast
+    factor and shift the brightness values.
+
+    Clips intensities to uint8 data type range, ``[0, 255]``.
+
+    Adapted from the aloe/xcdskd package.
+
+    Parameters
+    ----------
+    image
+        Image to normalize.
+    add_bright
+        Brightness offset to for each array. Default is ``0``.
+    contrast
+        Contrast factor for each array. Default is ``1.0``.
+    dtype_out
+        Output data type, either ``"uint8"`` (default) or ``"uint16"``.
+
+    Returns
+    -------
+    normalized_image
+        Normalized image.
+    """
+    dtype_out = np.dtype(dtype_out)
+    dtype_max = np.iinfo(dtype_out).max
+
+    offset = (dtype_max // 2) + add_bright
+    contrast *= dtype_max * 0.3125
+    median = np.median(image)
+    std = np.std(image)
+    normalized_image = offset + ((contrast * (image - median)) / std)
+
+    return np.clip(normalized_image, 0, dtype_max)
+
+
+def _get_rgb_image(
+    channels: List[np.ndarray],
+    percentiles: Optional[Tuple] = None,
+    normalize: bool = True,
+    alpha: Optional[np.ndarray] = None,
+    dtype_out: Union[str, np.dtype, type] = "uint8",
+    add_bright: int = 0,
+    contrast: float = 1.0,
+) -> np.ndarray:
+    """Return an RGB image from three numpy arrays, with a potential
+    alpha channel.
+
+    Parameters
+    ----------
+    channels
+        A list of np.ndarray for the red, green and blue channel,
+        respectively.
+    percentiles
+        Whether to apply contrast stretching with a given percentile
+        tuple with percentages, e.g. (0.5, 99.5), after creating the
+        RGB image. If not given (default), no contrast stretching is
+        performed.
+    normalize
+        Whether to normalize the individual ``channels`` before
+        RGB image creation. Default is ``True``.
+    alpha
+        Potential alpha channel. If not given (default), no alpha
+        channel is added to the image.
+    dtype_out
+        Output data type, either ``"uint8"`` (default) or ``"uint16"``.
+    add_bright
+        Brightness offset to for each array. Default is ``0``.
+    contrast
+        Contrast factor for each array. Default is ``1.0``.
+
+    Returns
+    -------
+    rgb_image
+        RGB image.
+    """
+    dtype_out = np.dtype(dtype_out)
+
+    n_channels = 3
+    rgb_image = np.zeros(channels[0].shape + (n_channels,), np.float32)
+    for i, channel in enumerate(channels):
+        if normalize:
+            channel = _normalize_image(
+                channel.astype(np.float32),
+                dtype_out=dtype_out,
+                add_bright=add_bright,
+                contrast=contrast,
+            )
+        rgb_image[..., i] = channel
+
+    # Apply alpha channel if desired
+    if alpha is not None:
+        alpha_min = np.nanmin(alpha)
+        rescaled_alpha = (alpha - alpha_min) / (np.nanmax(alpha) - alpha_min)
+        for i in range(n_channels):
+            rgb_image[..., i] *= rescaled_alpha
+
+    # Rescale to fit data type range
+    if percentiles is not None:
+        in_range = tuple(np.percentile(rgb_image, q=percentiles))
+    else:
+        in_range = None
+    rgb_image = rescale_intensity(rgb_image, in_range=in_range, dtype_out=dtype_out)
+
+    return rgb_image.astype(dtype_out)
```

### Comparing `kikuchipy-0.8.7/kikuchipy/hyperspy_extension.yaml` & `kikuchipy-0.9.0/kikuchipy/hyperspy_extension.yaml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/imaging/__init__.py` & `kikuchipy-0.9.0/kikuchipy/release.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
-"""Imaging using the EBSD detector."""
+from datetime import datetime
 
-__all__ = [
-    "VirtualBSEImager",
-]
-
-
-def __dir__():
-    return sorted(__all__)
 
-
-def __getattr__(name):
-    _import_mapping = {
-        "VirtualBSEImager": "vbse",
-    }
-    if name in __all__:
-        import importlib
-
-        if name in _import_mapping.keys():
-            import_path = f"{__name__}.{_import_mapping.get(name)}"
-            return getattr(importlib.import_module(import_path), name)
-        else:  # pragma: no cover
-            return importlib.import_module("." + name, __name__)
-    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
+author = "kikuchipy developers"
+copyright = f"Copyright 2019-{datetime.now().year}, kikuchipy"
+# Initial committer first, then sorted by line contributions
+credits = [
+    "Håkon Wiik Ånes",
+    "Lars Andreas Hastad Lervik",
+    "Ole Natlandsmyr",
+    "Tina Bergh",
+    "Eric Prestat",
+    "Andreas V. Bugten",
+    "Erlend Mikkelsen Østvold",
+    "Zhou Xu",
+    "Carter Francis",
+    "Magnus Nord",
+]
+license = "GPLv3+"
+maintainer = "Håkon Wiik Ånes"
+maintainer_email = "hakon.w.anes@ntnu.no"
+name = "kikuchipy"
+platforms = ["Linux", "MacOS X", "Windows"]
+status = "Development"
+version = "0.9.0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kikuchipy-0.8.7/kikuchipy/imaging/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/indexing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/__init__.py` & `kikuchipy-0.9.0/kikuchipy/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_dictionary_indexing.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_dictionary_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_hough_indexing.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_hough_indexing.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Most of these tools are private and not meant to be used by users.
 """
 
 from time import time
 from typing import List, Optional, Tuple, Union
 
 import dask.array as da
-import matplotlib.pyplot as plt
+from diffsims.crystallography import ReciprocalLatticeVector
 import numpy as np
 from orix.crystal_map import create_coordinate_arrays, CrystalMap, PhaseList
 from orix.quaternion import Rotation
 
 from kikuchipy import _pyebsdindex_installed
 
 
@@ -113,30 +113,41 @@
 
 def _get_indexer_from_detector(
     phase_list: PhaseList,
     shape: tuple,
     pc: np.ndarray,
     sample_tilt: float,
     tilt: float,
+    reflectors: Optional[
+        List[Union[ReciprocalLatticeVector, np.ndarray, list, tuple, None]]
+    ] = None,
     **kwargs,
 ) -> "EBSDIndexer":
-    """Return a PyEBSDIndex EBSD indexer.
+    r"""Return a PyEBSDIndex EBSD indexer.
 
     Parameters
     ----------
     phase_list
-        List of supported phases, only ``"FCC"`` and/or ``"BCC"``.
+        List of phases.
     shape
         Detector shape (n rows, n columns).
     pc
         Projection center(s).
     sample_tilt
         Sample tilt in degrees.
     tilt
         Detector tilt in degrees.
+    reflectors
+        List of reflectors or pole families :math:`\{hkl\}` to use in
+        indexing for each phase. If not passed, the default in
+        :func:`pyebsdindex.tripletvote.addphase` is used. For each
+        phase, the reflectors can either be a NumPy array, a list, a
+        tuple, a
+        :class:`~diffsis.crystallography.ReciprocalLatticeVector`, or
+        None.
     **kwargs
         Keyword arguments passed to
         :class:`~pyebsdindex.ebsd_index.EBSDIndexer`.
 
     Returns
     -------
     indexer
@@ -147,21 +158,20 @@
     Requires that :mod:`pyebsdindex` is installed, which is an optional
     dependency of kikuchipy. See :ref:`optional-dependencies` for
     details.
     """
     if not _pyebsdindex_installed:  # pragma: no cover
         raise ValueError(
             "pyebsdindex must be installed. Install with pip install pyebsdindex. "
-            "See https://kikuchipy.org/en/stable/user/installation.html for "
-            "details."
+            "See https://kikuchipy.org/en/stable/user/installation.html for details."
         )
 
     from pyebsdindex.ebsd_index import EBSDIndexer
 
-    phase_list_pei = _get_pyebsdindex_phaselist(phase_list)
+    phase_list_pei = _get_pyebsdindex_phaselist(phase_list, reflectors)
 
     indexer = EBSDIndexer(
         phaselist=phase_list_pei,
         vendor="KIKUCHIPY",
         PC=pc,
         sampleTilt=sample_tilt,
         camElev=tilt,
@@ -179,15 +189,15 @@
     step_sizes: tuple,
     indexer,
     chunksize: int,
     verbose: int,
 ) -> Tuple[CrystalMap, np.ndarray, np.ndarray]:
     """Perform Hough indexing with PyEBSDIndex.
 
-    Function can only be called if PyEBSDIndex is installed.
+    Requires PyEBSDIndex to be installed.
 
     Parameters
     ----------
     patterns
         Array of patterns of shape (n patterns, n detector rows, n
         detector columns).
     phase_list
@@ -217,17 +227,14 @@
         details.
     """
     n_patterns = patterns.shape[0]
 
     info_message = _get_info_message(n_patterns, chunksize, indexer)
     print(info_message)
 
-    if verbose == 2:
-        plt.figure()
-
     tic = time()
     index_data, band_data, _, _ = indexer.index_pats(
         patsin=patterns, verbose=verbose, chunksize=chunksize
     )
     toc = time()
     patterns_per_second = n_patterns / (toc - tic)
     print(f"  Indexing speed: {patterns_per_second:.5f} patterns/s")
@@ -238,97 +245,125 @@
         navigation_shape=nav_shape,
         step_sizes=step_sizes,
     )
 
     return xmap, index_data, band_data
 
 
-def _get_pyebsdindex_phaselist(phase_list: PhaseList) -> List[str]:
-    """Return a phase list compatible with PyEBSDIndex or raise a
-    ``ValueError`` if the given phase list is incompatible.
+def _get_pyebsdindex_phaselist(
+    phase_list: PhaseList,
+    reflectors: Optional[
+        List[Union[ReciprocalLatticeVector, np.ndarray, list, tuple, None]]
+    ] = None,
+) -> List["BandIndexer"]:
+    r"""Return a phase list compatible with PyEBSDIndex from an orix
+    phase list.
+
+    A ``ValueError`` is raised if the orix phase list contains phases
+    without the space group set or if the length of the reflector list
+    is unequal to the list of phases.
 
     Parameters
     ----------
     phase_list
         Phase list to convert to one compatible with PyEBSDIndex.
+    reflectors
+        List of reflectors or pole families :math:`\{hkl\}` to use in
+        indexing for each phase. If not passed, the default in
+        :func:`pyebsdindex.tripletvote.addphase` is used. For each
+        phase, the reflectors can either be a NumPy array, a list, a
+        tuple, a
+        :class:`~diffsis.crystallography.ReciprocalLatticeVector`, or
+        None.
 
     Returns
     -------
-    phase_list_pei
-        Phase list compatible with PyEBSDIndex.
+    phase_list_pei : list of pyebsdindex.tripletvote.BandIndexer
+        Phase list of phases (band indexers) compatible with
+        PyEBSDIndex.
 
     Raises
     ------
     ValueError
-        Raised if the phase list has more than two phases, if one of the
-        phases are not FCC or BCC, or if both phases are either FCC or
-        BCC.
+        Raised if the phase list contains a phase without a space group
+        set or if the reflector list is invalid.
     """
-    compatible = True
-    error_msg = None
+    from pyebsdindex.tripletvote import addphase
 
-    msg_supported_phases = (
-        "Hough indexing only supports indexing of generic face-centered cubic (FCC) and"
-        " body-centered cubic (BCC) phases.\nThus the phase list can only contain one "
-        "FCC and/or one BCC phase."
-    )
+    # Make list of reflectors iterable
+    if reflectors is None:
+        reflectors = [None] * phase_list.size
+    elif isinstance(reflectors, (np.ndarray, ReciprocalLatticeVector)) or (
+        isinstance(reflectors, (list, tuple)) and len(reflectors) != phase_list.size
+    ):
+        reflectors = [reflectors]
 
-    if phase_list.size > 2:
-        compatible = False
-        error_msg = msg_supported_phases
+    if len(reflectors) != phase_list.size:
+        raise ValueError(
+            "One set of reflectors or None must be passed per phase in the phase list."
+        )
 
-    sg = phase_list.space_groups
-    centering = None
-    if compatible and any(sg_i is None for sg_i in sg):
-        compatible = False
-        error_msg = (
-            "Space group for each phase must be set, otherwise the Bravais lattice(s) "
-            "cannot be determined."
+    phase_list_pei = []
+    i = 0
+    for _, phase in phase_list:
+        sg = phase.space_group
+        if sg is None:
+            raise ValueError(
+                "Space group for each phase must be set, otherwise the Bravais "
+                "lattice(s) cannot be determined."
+            )
+
+        ref = reflectors[i]
+        if isinstance(ref, ReciprocalLatticeVector):
+            ref = ref.unique(use_symmetry=True).hkl
+        elif isinstance(ref, (np.ndarray, list, tuple)):
+            ref = ReciprocalLatticeVector(phase, hkl=ref).unique(use_symmetry=True).hkl
+        else:
+            ref = None
+
+        phase_pei = addphase(
+            phasename=phase.name,
+            spacegroup=sg.number,
+            latticeparameter=phase.structure.lattice.abcABG(),
+            polefamilies=ref,
         )
-    else:
-        centering = [sg_i.short_name[0] for sg_i in sg]
-        if "I" in centering:
-            centering[centering.index("I")] = "B"
-        allowed_centering = [["F"], ["B"], ["F", "B"], ["B", "F"]]
-        if compatible and centering not in allowed_centering:
-            compatible = False
-            error_msg = msg_supported_phases
 
-    if not compatible:
-        raise ValueError(error_msg)
-    else:
-        phase_list_pei = [c + "CC" for c in centering]
-        return phase_list_pei
+        phase_list_pei.append(phase_pei)
+
+        i += 1
+
+    return phase_list_pei
 
 
 def _indexer_is_compatible_with_kikuchipy(
     indexer,
     sig_shape: tuple,
     nav_size: Optional[int] = None,
     check_pc: bool = True,
     raise_if_not: bool = False,
 ) -> bool:
-    """Check whether an indexer is compatible with kikuchipy or raise a
-    ``ValueError`` if it is not.
+    """Check whether an indexer is compatible with kikuchipy.
+
+    A ``ValueError`` is raised if it is not.
 
     Parameters
     ----------
     indexer : pyebsdindex.ebsd_index.EBSDIndexer
         Indexer instance.
     sig_shape
         Signal shape (n detector rows, n detector columns), checked
         against ``indexer.patDim``.
     nav_size
         Number of patterns. If given, it is checked against
         ``indexer.PC`` if ``check_pc=True``.
     check_pc
         Whether to check ``indexer.PC`` (default is ``True``).
     raise_if_not
-        Whether to raise a ``ValueError`` if the indexer is not
-        compatible with the signal. Default is ``False``.
+        Whether to raise a ``ValueError`` if the indexer is incompatible
+        with the signal. Default is ``False``.
 
     Returns
     -------
     compatible
         Whether the indexer is compatible with the signal.
     """
     compatible = True
@@ -359,22 +394,100 @@
         if compatible and (len(pc_shape) > 2 or pc_shape not in allowed_shapes):
             compatible = False
             error_msg = (
                 f"`indexer.PC` must be an array of shape {allowed_shapes_str}, but was "
                 f"{pc_shape} instead."
             )
 
+    if raise_if_not and not compatible:
+        raise ValueError(error_msg)
+    else:
+        return compatible
+
+
+def _phase_lists_are_compatible(
+    phase_list: PhaseList,
+    indexer,
+    raise_if_not: bool = False,
+) -> bool:
+    """Check whether phase lists made with orix and PyEBSDIndex are
+    compatible.
+
+    A ``ValueError`` is raised if they are not.
+
+    They are compatible if the lists have an equal number of phases in
+    the same order and if the corresponding phases have equal lattice
+    parameters (to the 12th decimal) and the same space group number.
+
+    Parameters
+    ----------
+    phase_list
+        Phase list made with orix.
+    indexer : pyebsdindex.ebsd_index.EBSDIndexer
+        EBSD indexer with a phase list from PyEBSDIndex.
+    raise_if_not
+        Whether to raise a ``ValueError`` if the phase lists are
+        incompatible. Default is ``False``.
+
+    Returns
+    -------
+    compatible
+        Whether the phase lists are compatible.
+
+    Raises
+    ------
+    ValueError
+        Raised if the phase lists are incompatible.
+    """
+    compatible = True
+
     phase_list_pei = indexer.phaselist
-    allowed_lists = [["FCC"], ["BCC"], ["FCC", "BCC"], ["BCC", "FCC"]]
-    if compatible and phase_list_pei not in allowed_lists:
+
+    msg = (
+        f"`indexer.phaselist` {phase_list_pei} and the list determined from"
+        f" `phase_list` must be the same"
+    )
+
+    n_phases = phase_list.size
+    n_phases_pei = len(phase_list_pei)
+    if n_phases != n_phases_pei:
         compatible = False
-        error_msg = f"`indexer.phaselist` must be one of {allowed_lists}"
+        msg = (
+            f"`phase_list` ({n_phases}) and `indexer.phaselist` ({n_phases_pei}) have "
+            "unequal number of phases"
+        )
+    else:
+        i = 0
+        for (_, phase), phase_pei in zip(phase_list, phase_list_pei):
+            lat = phase.structure.lattice.abcABG()
+            lat_pei = phase_pei.latticeparameter
+            sg = phase.space_group.number
+            sg_pei = phase_pei.spacegroup
+
+            if not np.allclose(lat, lat_pei, atol=1e-12):
+                compatible = False
+                msg = (
+                    f"Phase '{phase.name}' in `phase_list` and phase number {i} in "
+                    f"`indexer.phaselist` have unequal lattice parameters {lat} and "
+                    f"{lat_pei}"
+                )
+                break
+            elif sg != sg_pei:
+                compatible = False
+                msg = (
+                    f"Phase '{phase.name}' in `phase_list` and phase number {i} in "
+                    f"`indexer.phaselist` have unequal space group numbers {sg} and "
+                    f"{sg_pei}"
+                )
+                break
+
+            i += 1
 
     if raise_if_not and not compatible:
-        raise ValueError(error_msg)
+        raise ValueError(msg)
     else:
         return compatible
 
 
 def _get_info_message(nav_size: int, chunksize: int, indexer: "EBSDIndexer") -> str:
     from kikuchipy import _pyopencl_context_available
 
@@ -399,13 +512,14 @@
 
 def _optimize_pc(
     pc0: List[float],
     patterns: Union[np.ndarray, da.Array],
     indexer: "EBSDIndexer",
     batch: bool,
     method: str,
+    **kwargs,
 ) -> np.ndarray:
     if method == "pso":
         from pyebsdindex.pcopt import optimize_pso as optimize_func
     else:
         from pyebsdindex.pcopt import optimize as optimize_func
-    return optimize_func(pats=patterns, indexer=indexer, PC0=pc0, batch=batch)
+    return optimize_func(pats=patterns, indexer=indexer, PC0=pc0, batch=batch, **kwargs)
```

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_merge_crystal_maps.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_merge_crystal_maps.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_orientation_similarity_map.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_orientation_similarity_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_refinement/__init__.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_refinement/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_refinement/_objective_functions.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_refinement/_objective_functions.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_refinement/_refinement.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_refinement/_refinement.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/_refinement/_solvers.py` & `kikuchipy-0.9.0/kikuchipy/indexing/_refinement/_solvers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/__init__.py` & `kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py` & `kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py` & `kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/similarity_metrics/_similarity_metric.py` & `kikuchipy-0.9.0/kikuchipy/indexing/similarity_metrics/_similarity_metric.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/tests/test_dictionary_indexing.py` & `kikuchipy-0.9.0/kikuchipy/indexing/tests/test_dictionary_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/tests/test_ebsd_refinement.py` & `kikuchipy-0.9.0/kikuchipy/indexing/tests/test_ebsd_refinement.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/tests/test_merge_crystal_maps.py` & `kikuchipy-0.9.0/kikuchipy/indexing/tests/test_merge_crystal_maps.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/tests/test_orientation_similarity_map.py` & `kikuchipy-0.9.0/kikuchipy/indexing/tests/test_orientation_similarity_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/indexing/tests/test_similarity_metrics.py` & `kikuchipy-0.9.0/kikuchipy/indexing/tests/test_similarity_metrics.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/__init__.py` & `kikuchipy-0.9.0/kikuchipy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/_io.py` & `kikuchipy-0.9.0/kikuchipy/io/_io.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/_util.py` & `kikuchipy-0.9.0/kikuchipy/io/_util.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/__init__.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/_emsoft_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/_emsoft_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/bruker_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/ebsd_directory.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/ebsd_directory.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/edax_binary.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/edax_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/edax_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/edax_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/kikuchipy_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/kikuchipy_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/nordif.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/nordif.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/nordif_calibration_patterns.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/nordif_calibration_patterns.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/oxford_binary.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/oxford_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/oxford_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/oxford_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_ebsd_directory.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_ebsd_directory.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_edax_binary.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_edax_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_nordif.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_nordif.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_oxford_binary.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_oxford_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py` & `kikuchipy-0.9.0/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/pattern/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/tests/test_io.py` & `kikuchipy-0.9.0/kikuchipy/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/io/tests/test_util.py` & `kikuchipy-0.9.0/kikuchipy/io/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/pattern/__init__.py` & `kikuchipy-0.9.0/kikuchipy/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/pattern/_pattern.py` & `kikuchipy-0.9.0/kikuchipy/pattern/_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/pattern/chunk.py` & `kikuchipy-0.9.0/kikuchipy/pattern/chunk.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/pattern/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/signals/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/pattern/tests/test_chunk.py` & `kikuchipy-0.9.0/kikuchipy/pattern/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/pattern/tests/test_pattern.py` & `kikuchipy-0.9.0/kikuchipy/pattern/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/projections/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/__init__.py` & `kikuchipy-0.9.0/kikuchipy/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/_kikuchi_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/signals/_kikuchi_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/_kikuchipy_signal.py` & `kikuchipy-0.9.0/kikuchipy/signals/_kikuchipy_signal.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/ebsd.py` & `kikuchipy-0.9.0/kikuchipy/signals/ebsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 
 from kikuchipy import _pyebsdindex_installed, _pyopencl_context_available
 from kikuchipy.detectors import EBSDDetector
 from kikuchipy.filters.fft_barnes import _fft_filter, _fft_filter_setup
 from kikuchipy.filters.window import Window
 from kikuchipy.indexing._dictionary_indexing import _dictionary_indexing
 from kikuchipy.indexing._hough_indexing import (
-    _get_pyebsdindex_phaselist,
     _indexer_is_compatible_with_kikuchipy,
     _hough_indexing,
     _optimize_pc,
+    _phase_lists_are_compatible,
 )
 from kikuchipy.indexing._refinement._refinement import (
     _refine_orientation,
     _refine_orientation_pc,
     _refine_pc,
 )
 from kikuchipy.indexing.similarity_metrics import (
@@ -1602,17 +1602,16 @@
 
         Currently, PyEBSDIndex only supports indexing with a single
         mean projection center (PC).
 
         Parameters
         ----------
         phase_list
-            List of phases. The list can only contain one face-centered
-            cubic (FCC) phase, one body-centered cubic (BCC) phase or
-            both types.
+            List of phases. The list must correspond to the phase list
+            in the passed.
         indexer
             PyEBSDIndex EBSD indexer instance of which the
             :meth:`~pyebsdindex.ebsd_index.EBSDIndexer.index_pats`
             method is called. Its `phaselist` must be compatible with
             the given ``phase_list``, and the ``indexer.vendor`` must be
             ``"KIKUCHIPY"``. An indexer can be obtained with
             :meth:`~kikuchipy.detectors.EBSDDetector.get_indexer`.
@@ -1670,24 +1669,19 @@
 
         am = self.axes_manager
         nav_shape = am.navigation_shape[::-1]
         nav_size = int(np.prod(nav_shape))
         sig_shape = am.signal_shape[::-1]
         step_sizes = tuple([a.scale for a in am.navigation_axes[::-1]])
 
-        # Check indexer
-        phase_list_pei = _get_pyebsdindex_phaselist(phase_list)
+        # Check indexer (but not the reflectors)
         _ = _indexer_is_compatible_with_kikuchipy(
             indexer, sig_shape, nav_size, raise_if_not=True
         )
-        if indexer.phaselist != phase_list_pei:
-            raise ValueError(
-                f"`indexer.phaselist` {indexer.phaselist} and the list determined from"
-                f" `phase_list` {phase_list_pei} must be the same"
-            )
+        _ = _phase_lists_are_compatible(phase_list, indexer, raise_if_not=True)
 
         # Prepare patterns
         chunksize = min(chunksize, max(am.navigation_size, 1))
         patterns = self.data.reshape((-1,) + sig_shape)
         if self._lazy:  # pragma: no cover
             patterns = patterns.rechunk({0: chunksize, 1: -1, 2: -1})
 
@@ -1714,40 +1708,41 @@
 
     def hough_indexing_optimize_pc(
         self,
         pc0: Union[list, tuple, np.ndarray],
         indexer: "EBSDIndexer",
         batch: bool = False,
         method: str = "Nelder-Mead",
+        **kwargs,
     ) -> "EBSDDetector":
         """Return a detector with one projection center (PC) per
         pattern optimized using Hough indexing from :mod:`pyebsdindex`.
 
         See :class:`~pyebsdindex.ebsd_index.EBSDIndexer` and
-        :mod:`~pyebsdindex.pcopt.optimize` for details.
+        :mod:`~pyebsdindex.pcopt` for details.
 
         Parameters
         ----------
         pc0
             A single initial guess of PC for all patterns in Bruker's
             convention, (PCx, PCy, PCz).
         indexer
             PyEBSDIndex EBSD indexer instance to pass on to the
-            optimization function. Its `phaselist` must be compatible
-            with ``phase_list``, if given, and the ``indexer.vendor``
-            must be ``"KIKUCHIPY"``. An indexer can be obtained with
+            optimization function. An indexer can be obtained with
             :meth:`~kikuchipy.detectors.EBSDDetector.get_indexer`.
         batch
             Whether the fit for the patterns should be optimized using
             the cumulative fit for all patterns (``False``, default), or
             if an optimization is run for each pattern individually.
         method
             Which optimization method to use, either ``"Nelder-Mead"``
-            from SciPy (default) or ``"PSO"`` (particle swarm). The
-            latter method does not support ``batch=True``.
+            from SciPy (default) or ``"PSO"`` (particle swarm).
+        **kwargs
+            Keyword arguments passed on to PyEBSDIndex' optimization
+            method (depending on the chosen ``method``).
 
         Returns
         -------
         new_detector
             EBSD detector with one PC if ``batch=False`` or one PC per
             pattern if ``batch=True``. The detector attributes are
             extracted from ``indexer.sampleTilt`` etc.
@@ -1778,16 +1773,14 @@
         supported_methods = ["nelder-mead", "pso"]
         method = method.lower()
         if method not in supported_methods:
             raise ValueError(
                 f"`method` '{method}' must be one of the supported methods "
                 f"{supported_methods}"
             )
-        elif batch and method == "pso":
-            raise ValueError("PSO optimization method does not support `batch=True`")
 
         am = self.axes_manager
         nav_shape = am.navigation_shape[::-1]
         nav_size = int(np.prod(nav_shape))
         sig_shape = am.signal_shape[::-1]
 
         # Check indexer
@@ -1797,15 +1790,20 @@
 
         # Prepare patterns
         patterns = self.data.reshape((-1,) + sig_shape)
         if self._lazy:  # pragma: no cover
             patterns = patterns.rechunk({0: "auto", 1: -1, 2: -1})
 
         pc = _optimize_pc(
-            pc0=pc0, patterns=patterns, indexer=indexer, batch=batch, method=method
+            pc0=pc0,
+            patterns=patterns,
+            indexer=indexer,
+            batch=batch,
+            method=method,
+            **kwargs,
         )
 
         if batch:
             pc = pc.reshape(nav_shape + (3,))
 
         new_detector = EBSDDetector(
             shape=sig_shape,
```

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/ebsd_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/signals/ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/ecp_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/signals/ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/tests/__init__.py` & `kikuchipy-0.9.0/kikuchipy/simulations/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/tests/test_ebsd.py` & `kikuchipy-0.9.0/kikuchipy/signals/tests/test_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/tests/test_ebsd_hough_indexing.py` & `kikuchipy-0.9.0/kikuchipy/signals/tests/test_ebsd_hough_indexing.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,102 +11,95 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with kikuchipy. If not, see <http://www.gnu.org/licenses/>.
 
-import matplotlib.pyplot as plt
+from diffpy.structure import Lattice, Structure
+from diffsims.crystallography import ReciprocalLatticeVector
 import numpy as np
-from orix.crystal_map import CrystalMap, PhaseList
+from orix.crystal_map import CrystalMap, Phase, PhaseList
 import pytest
 
 import kikuchipy as kp
 from kikuchipy.indexing._hough_indexing import (
     _get_info_message,
     _indexer_is_compatible_with_kikuchipy,
+    _phase_lists_are_compatible,
 )
 
 
 @pytest.mark.skipif(
     not kp._pyebsdindex_installed, reason="pyebsdindex is not installed"
 )
 class TestHoughIndexing:
     def setup_method(self):
         s = kp.data.nickel_ebsd_small()
         s.remove_static_background()
         s.remove_dynamic_background()
 
         self.signal = s
-        self.xmap = s.xmap
-        self.phase_list = s.xmap.phases
-        self.detector = s.detector
         self.indexer = s.detector.get_indexer(s.xmap.phases)
 
     def test_hough_indexing_print_information(self):
-        det = self.detector
+        det = self.signal.detector
         det.shape = (4, 5)  # Save time on indexer creation
 
-        indexer1 = det.get_indexer(self.phase_list)
+        indexer1 = det.get_indexer(self.signal.xmap.phases)
 
         info = _get_info_message(
             self.signal.axes_manager.navigation_size, chunksize=3, indexer=indexer1
         )
         info_list = info.split("\n")
         # fmt: off
         assert info_list[0] ==     "Hough indexing with PyEBSDIndex information:"
         assert info_list[1][:12] == "  PyOpenCL: "
         assert info_list[2] ==     "  Projection center (Bruker, mean): (0.4251, 0.2134, 0.5007)"
         assert info_list[3] ==     "  Indexing 9 pattern(s) in 3 chunk(s)"
         # fmt: on
 
         det_pc_mean = det.deepcopy()
         det_pc_mean.pc = det_pc_mean.pc_average
-        indexer2 = det_pc_mean.get_indexer(self.phase_list)
+        indexer2 = det_pc_mean.get_indexer(self.signal.xmap.phases)
         info2 = _get_info_message(
             self.signal.axes_manager.navigation_size, chunksize=3, indexer=indexer2
         )
         info_list2 = info2.split("\n")
         assert info_list2[2] == "  Projection center (Bruker): (0.4251, 0.2134, 0.5007)"
 
     def test_hough_indexing(self):
         # Reference results (Hough indexing + refinement)
-        xmap_ref = self.xmap
+        xmap_ref = self.signal.xmap
 
-        phase_list = self.phase_list
+        phase_list = xmap_ref.phases
         indexer = self.indexer
 
         xmap = self.signal.hough_indexing(phase_list, indexer)
 
         assert isinstance(xmap, CrystalMap)
         assert xmap.phases.names == phase_list.names
         angles = xmap.orientations.angle_with(xmap_ref.orientations, degrees=True)
         assert np.all(angles < 1)
 
-    def test_hough_indexing_plot_transform(self):
-        _ = self.signal.hough_indexing(self.phase_list, self.indexer, verbose=2)
-        ax = plt.gca()
-        assert len(ax.texts) == 9
-        for i, text in enumerate(ax.texts):
-            assert text.get_text() == str(i + 1)
-
     def test_hough_indexing_lazy(self):  # pragma: no cover
         s = self.signal.as_lazy()
 
+        phase_list = self.signal.xmap.phases
         if kp._pyopencl_context_available:
-            xmap1 = s.hough_indexing(self.phase_list, self.indexer)
-            xmap2 = self.signal.hough_indexing(self.phase_list, self.indexer)
+            xmap1 = s.hough_indexing(phase_list, self.indexer)
+            xmap2 = self.signal.hough_indexing(phase_list, self.indexer)
             assert np.allclose(xmap1.rotations.data, xmap2.rotations.data)
             assert np.allclose(xmap1.fit, xmap2.fit)
         else:
             with pytest.raises(ValueError, match="Hough indexing of lazy signals must"):
-                _ = s.hough_indexing(self.phase_list, self.indexer, verbose=2)
+                _ = s.hough_indexing(phase_list, self.indexer, verbose=2)
 
     def test_hough_indexing_return_index_data(self):
-        phase_list = self.phase_list
+        phase_list = self.signal.xmap.phases
         xmap, index_data = self.signal.hough_indexing(
             phase_list, self.indexer, return_index_data=True
         )
 
         index_data_dtypes = index_data.dtype.fields.keys()
         for field in ["quat", "iq", "pq", "cm", "phase", "fit", "nmatch"]:
             assert field in index_data_dtypes
@@ -117,35 +110,38 @@
         xmap2 = kp.indexing.xmap_from_hough_indexing_data(index_data, phase_list)
         assert xmap2.shape == (9,)
         assert np.allclose(xmap2.rotations.data, xmap.rotations.data)
         assert np.allclose(xmap2.fit, xmap.fit)
         assert np.allclose(xmap2.cm, xmap.cm)
 
     def test_hough_indexing_return_band_data(self):
-        indexer = self.detector.get_indexer(self.phase_list, nBands=8)
+        phase_list = self.signal.xmap.phases
+        indexer = self.signal.detector.get_indexer(phase_list, nBands=8)
         _, band_data = self.signal.hough_indexing(
-            self.phase_list, indexer, return_band_data=True
+            phase_list, indexer, return_band_data=True
         )
         assert isinstance(band_data, np.ndarray)
         assert band_data.shape == (
             self.signal.axes_manager.navigation_size,
             indexer.bandDetectPlan.nBands,
         )
 
         _, index_data, band_data = self.signal.hough_indexing(
-            self.phase_list, self.indexer, return_index_data=True, return_band_data=True
+            phase_list, self.indexer, return_index_data=True, return_band_data=True
         )
         assert isinstance(index_data, np.ndarray)
         assert isinstance(band_data, np.ndarray)
         assert index_data.shape == (2, 9)
         assert band_data.shape == (9, 9)
 
     def test_hough_indexing_raises_dissimilar_phase_lists(self):
         phase_list = PhaseList(names=["a", "b"], space_groups=[225, 229])
-        with pytest.raises(ValueError, match=r"`indexer.phaselist` \['FCC'\] and the "):
+        with pytest.raises(
+            ValueError, match=r"`phase_list` \(2\) and `indexer.phaselist` \(1\) have "
+        ):
             _ = self.signal.hough_indexing(phase_list, self.indexer)
 
     def test_indexer_is_compatible_with_signal(self):
         indexer = self.indexer
 
         # Vendor
         indexer.vendor = "EDAX"
@@ -154,17 +150,17 @@
             _indexer_is_compatible_with_kikuchipy(indexer, (60, 60), raise_if_not=True)
         indexer.vendor = "kikuchipy"
 
         # Signal shape
         assert not _indexer_is_compatible_with_kikuchipy(indexer, (60, 59), 9)
         with pytest.raises(ValueError, match=r"Indexer signal shape \(60, 60\) must "):
             _indexer_is_compatible_with_kikuchipy(indexer, (60, 59), raise_if_not=True)
-        det2 = self.detector.deepcopy()
+        det2 = self.signal.detector.deepcopy()
         det2.shape = (60, 59)
-        indexer2 = det2.get_indexer(self.phase_list)
+        indexer2 = det2.get_indexer(self.signal.xmap.phases)
         assert not _indexer_is_compatible_with_kikuchipy(indexer2, (60, 60), 9)
         with pytest.raises(ValueError, match=r"Indexer signal shape \(60, 59\) must "):
             _indexer_is_compatible_with_kikuchipy(indexer2, (60, 60), raise_if_not=True)
 
         # PC
         assert not _indexer_is_compatible_with_kikuchipy(indexer, (60, 60))
         with pytest.raises(
@@ -176,27 +172,16 @@
             ValueError,
             match=r"`indexer.PC` must be an array of shape \(3,\) or \(8, 3\), but was ",
         ):
             _indexer_is_compatible_with_kikuchipy(
                 indexer, (60, 60), 8, raise_if_not=True
             )
 
-        # Phase list
-        indexer.phaselist = ["FCC", "FCC"]
-        assert not _indexer_is_compatible_with_kikuchipy(indexer, (60, 60), 9)
-        with pytest.raises(
-            ValueError,
-            match=r"`indexer.phaselist` must be one of \[\['FCC'\], \['BCC'\], \['FCC',",
-        ):
-            _indexer_is_compatible_with_kikuchipy(
-                indexer, (60, 60), 9, raise_if_not=True
-            )
-
     def test_hough_indexing_get_xmap_from_index_data(self):
-        phase_list = self.phase_list
+        phase_list = self.signal.xmap.phases
         xmap, index_data = self.signal.hough_indexing(
             phase_list, self.indexer, return_index_data=True
         )
 
         with pytest.raises(ValueError, match="`nav_shape` cannot be a tuple of more "):
             _ = kp.indexing.xmap_from_hough_indexing_data(
                 index_data, phase_list, navigation_shape=(1, 2, 3)
@@ -223,67 +208,162 @@
             scan_unit="um",
         )
         assert np.allclose(xmap2.phase_id, [-1] + [0] * 8)
         assert xmap2.scan_unit == "um"
         assert xmap2.dy == 2
         assert xmap2.dx == 3
 
+    def test_reflector_list(self):
+        phase_list = self.signal.xmap.phases
+
+        hkl = [[2, 0, 0], [2, 2, 0], [1, 1, 1], [3, 1, 1], [3, 3, 1]]
+
+        ref = ReciprocalLatticeVector(hkl=hkl, phase=phase_list[0])
+        reflectors = [hkl, tuple(hkl), np.array(hkl), ref]
+
+        indexers = [self.signal.detector.get_indexer(phase_list)]
+        for i in range(len(reflectors)):
+            indexer = self.signal.detector.get_indexer(
+                phase_list, reflectors=reflectors[i]
+            )
+            indexers.append(indexer)
+
+            assert np.allclose(indexer.phaselist[0].polefamilies, hkl)
+
+    def test_reflector_lists(self):
+        phase_list = PhaseList(names=["a", "b"], space_groups=[186, 225])
+        hkl = [
+            [[0, 0, 6], [0, 0, -6], [1, 0, 0], [2, 0, 0]],
+            [[2, 0, 0], [2, 2, 0]],
+            [[1, 1, 1], [3, 1, 1], [3, 3, 1]],
+        ]
+
+        _ = self.signal.detector.get_indexer(phase_list, hkl[:2])
+        _ = self.signal.detector.get_indexer(phase_list, [hkl[0], None])
+        _ = self.signal.detector.get_indexer(phase_list, [None, None])
+
+        with pytest.raises(ValueError, match="One set of reflectors or None must be "):
+            _ = self.signal.detector.get_indexer(phase_list, hkl)
+
+    def test_compatible_phase_lists(self):
+        phase_list = PhaseList(
+            names=["a", "b"],
+            space_groups=[186, 225],
+            structures=[
+                Structure(lattice=Lattice(1, 1, 2, 90, 90, 120)),
+                Structure(lattice=Lattice(1, 1, 1, 90, 90, 90)),
+            ],
+        )
+        indexer = self.signal.detector.get_indexer(phase_list)
+
+        assert _phase_lists_are_compatible(phase_list, indexer, True)
+
+        # Differing number of phases
+        phase_list2 = phase_list.deepcopy()
+        phase_list2.add(Phase("c", space_group=1))
+        assert not _phase_lists_are_compatible(phase_list2, indexer)
+        with pytest.raises(
+            ValueError, match=r"`phase_list` \(3\) and `indexer.phaselist` \(2\)"
+        ):
+            _ = _phase_lists_are_compatible(phase_list2, indexer, True)
+
+        # Differing lattice parameters
+        phase_list3 = phase_list.deepcopy()
+        lat = phase_list3["a"].structure.lattice
+        lat.setLatPar(lat.a * 10)
+        with pytest.raises(
+            ValueError, match="Phase 'a' in `phase_list` and phase number 0 in "
+        ):
+            _ = _phase_lists_are_compatible(phase_list3, indexer, True)
+
+        # Differing space groups
+        phase_list4 = phase_list.deepcopy()
+        phase_list4["b"].space_group = 224
+        with pytest.raises(
+            ValueError, match="Phase 'b' in `phase_list` and phase number 1 in "
+        ):
+            _ = _phase_lists_are_compatible(phase_list4, indexer, True)
+
+
+@pytest.mark.skipif(
+    not kp._pyebsdindex_installed, reason="pyebsdindex is not installed"
+)
+class TestPCOptimization:
+    def setup_method(self):
+        s = kp.data.nickel_ebsd_small()
+        s.remove_static_background()
+        s.remove_dynamic_background()
+
+        self.signal = s
+        self.indexer = s.detector.get_indexer(s.xmap.phases)
+
     def test_optimize_pc(self):
-        det2 = self.signal.hough_indexing_optimize_pc(
-            self.detector.pc_average, self.indexer
-        )
-        assert det2.navigation_shape == (1,)
-        assert np.allclose(det2.pc_average, self.detector.pc_average, atol=1e-2)
+        det0 = self.signal.detector
+
+        det = self.signal.hough_indexing_optimize_pc(det0.pc_average, self.indexer)
+        assert det.navigation_shape == (1,)
+        assert np.allclose(det.pc_average, det0.pc_average, atol=1e-2)
 
         # Batch with PC array with more than one dimension
-        pc0 = np.atleast_2d(self.detector.pc_average)
-        det3 = self.signal.hough_indexing_optimize_pc(pc0, self.indexer, batch=True)
-        assert det3.navigation_shape == (3, 3)
-        assert np.allclose(det2.pc_average, det3.pc_average, atol=1e-2)
+        det2 = self.signal.hough_indexing_optimize_pc(
+            det0.pc_average, self.indexer, batch=True
+        )
+        assert det2.navigation_shape == (3, 3)
+        assert np.allclose(det.pc_average, det2.pc_average, atol=1e-2)
 
         # Detector parameters
-        assert det2.shape == self.detector.shape
-        assert np.isclose(det2.sample_tilt, self.detector.sample_tilt)
-        assert np.isclose(det2.tilt, self.detector.tilt)
-        assert np.isclose(det2.px_size, self.detector.px_size)
+        assert det.shape == det0.shape
+        assert np.isclose(det.sample_tilt, det0.sample_tilt)
+        assert np.isclose(det.tilt, det0.tilt)
+        assert np.isclose(det.px_size, det0.px_size)
+
+    def test_optimize_pc_pso(self, worker_id):
+        det0 = self.signal.detector
 
-    def test_optimize_pc_pso(self):
         det = self.signal.hough_indexing_optimize_pc(
-            self.detector.pc_average, self.indexer, method="PSO"
+            det0.pc_average, self.indexer, method="PSO"
         )
         # Results are not deterministic, so we give a wide range here...
-        assert abs(self.detector.pc_average - det.pc_average).max() < 0.05
+        assert abs(det0.pc_average - det.pc_average).max() < 0.03
+
+        if worker_id == "master":  # pragma: no cover
+            # Batch with PC array with more than one dimension
+            det2 = self.signal.hough_indexing_optimize_pc(
+                det0.pc_average,
+                self.indexer,
+                batch=True,
+                method="PSO",
+                search_limit=0.1,
+            )
+            assert det2.navigation_shape == (3, 3)
+            assert abs(det.pc_average - det2.pc_average).max() < 0.03
 
     def test_optimize_pc_raises(self):
         with pytest.raises(ValueError, match="`pc0` must be of size 3"):
             _ = self.signal.hough_indexing_optimize_pc([0.5, 0.5], self.indexer)
 
         with pytest.raises(ValueError, match="`method` 'powell' must be one of the "):
             _ = self.signal.hough_indexing_optimize_pc(
                 [0.5, 0.5, 0.5], self.indexer, method="Powell"
             )
 
-        with pytest.raises(ValueError, match="PSO optimization method does not "):
-            _ = self.signal.hough_indexing_optimize_pc(
-                [0.5, 0.5, 0.5], self.indexer, method="PSO", batch=True
-            )
-
     def test_optimize_pc_lazy(self):  # pragma: no cover
         s = self.signal.as_lazy()
+        det = self.signal.detector
 
         if kp._pyopencl_context_available:
-            det = s.hough_indexing_optimize_pc(self.detector.pc_average, self.indexer)
-            assert np.allclose(det.pc_average, self.detector.pc_average, atol=1e-2)
+            det = s.hough_indexing_optimize_pc(det.pc_average, self.indexer)
+            assert np.allclose(det.pc_average, det.pc_average, atol=1e-2)
         else:
             with pytest.raises(ValueError, match="Hough indexing of lazy signals must"):
-                _ = s.hough_indexing_optimize_pc(self.detector.pc_average, self.indexer)
+                _ = s.hough_indexing_optimize_pc(det.pc_average, self.indexer)
 
 
 @pytest.mark.skipif(kp._pyebsdindex_installed, reason="pyebsdindex is installed")
-class TestHoughIndexingNopyebsdindex:  # pragma: no cover
+class TestHoughIndexingNoPyEBSDIndex:  # pragma: no cover
     def setup_method(self):
         s = kp.data.nickel_ebsd_small()
 
         self.signal = s
 
     def test_get_indexer(self):
         with pytest.raises(ValueError, match="pyebsdindex must be installed"):
```

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/tests/test_ebsd_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/signals/tests/test_ebsd_master_pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     _get_direction_cosines_for_varying_pc,
     _get_lambert_interpolation_parameters,
     _get_pixel_from_master_pattern,
     _lambert2vector,
     _project_patterns_from_master_pattern_with_fixed_pc,
     _project_patterns_from_master_pattern_with_varying_pc,
     _project_single_pattern_from_master_pattern,
+    _vector2lambert,
 )
 from kikuchipy.indexing.similarity_metrics import (
     NormalizedCrossCorrelationMetric,
     NormalizedDotProductMetric,
 )
 
 
@@ -717,7 +718,37 @@
             mp_sp.adaptive_histogram_equalization()
 
         # Spreads intensities within data range
         mp_lp = nickel_ebsd_master_pattern_small(projection="lambert")
         mp_lp2 = mp_lp.adaptive_histogram_equalization(inplace=False)
         assert all([mp_lp2.data.min() >= 0, mp_lp2.data.max() <= 255])
         assert abs(np.unique(mp_lp2.data).size - 255) < 2
+
+
+class TestLambertProjection:
+    def test_vector2xy(self):
+        """Works for numpy arrays."""
+        xyz = np.array(
+            [
+                [0, 0, 1],
+                [0, 1, 0],
+                [2, 0, 0],
+                [0, 0, -3],
+                [0, 0, -1],
+                [0, -1, 0],
+                [-2, 0, 0],
+                [0, 0, 3],
+            ],
+            dtype=np.float64,
+        )
+        lambert_xy = [
+            [0, 0],
+            [0, np.sqrt(np.pi / 2)],
+            [np.sqrt(np.pi / 2), 0],
+            [0, 0],
+            [0, 0],
+            [0, -np.sqrt(np.pi / 2)],
+            [-np.sqrt(np.pi / 2), 0],
+            [0, 0],
+        ]
+        assert np.allclose(_vector2lambert.py_func(xyz), lambert_xy)
+        assert np.allclose(_vector2lambert(xyz), lambert_xy)
```

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/tests/test_ecp_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/signals/tests/test_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/tests/test_kikuchi_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/signals/tests/test_kikuchi_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/tests/test_virtual_bse_image.py` & `kikuchipy-0.9.0/kikuchipy/signals/tests/test_virtual_bse_image.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/__init__.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/_crystal_map.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/_crystal_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/_dask.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/_dask.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/_detector.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/_detector.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/_map_helper.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/_map_helper.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/_master_pattern.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/_master_pattern.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,20 +61,22 @@
 from typing import Optional, Tuple, Union
 
 from numba import njit
 import numba as nb
 import numpy as np
 
 from kikuchipy.pattern._pattern import _rescale_with_min_max
-from kikuchipy.projections.lambert_projection import _vector2xy
 from kikuchipy._rotation import _rotate_vector
 
 
 # Reusable constants
+SQRT_PI = np.sqrt(np.pi)
 SQRT_PI_HALF = np.sqrt(np.pi / 2)
+SQRT_PI_OVER_2 = SQRT_PI / 2
+TWO_OVER_SQRT_PI = 2 / SQRT_PI
 
 
 def _get_direction_cosines_from_detector(
     detector: "EBSDDetector", signal_mask: Optional[np.ndarray] = None
 ) -> np.ndarray:
     """Return direction cosines for one or more projection centers
     (PCs).
@@ -565,14 +567,55 @@
         pattern = _rescale_with_min_max(
             pattern, np.min(pattern), np.max(pattern), out_min, out_max
         )
 
     return pattern.astype(dtype_out)
 
 
+@nb.jit("float64[:, :](float64[:, :])", nogil=True, cache=True, nopython=True)
+def _vector2lambert(v: np.ndarray) -> np.ndarray:
+    """Lambert projection of vector(s) :cite:`callahan2013dynamical`.
+
+    Parameters
+    ----------
+    v
+        Vector(s) in an array of shape (n, 3) and 64-bit float data
+        type in Cartesian coordinates.
+
+    Returns
+    -------
+    lambert
+        Square Lambert coordinates (X, Y) in array of shape (n, 2) and
+        data type 64-bit float.
+    """
+    # Normalize vectors (vectorized operation is faster than per vector)
+    norm = np.sqrt(np.sum(np.square(v), axis=1))
+    norm = np.expand_dims(norm, axis=1)
+    w = v / norm
+
+    n_vectors = v.shape[0]
+    lambert_xy = np.zeros((n_vectors, 2))
+    for i in nb.prange(n_vectors):
+        x, y, z = w[i]
+        abs_z = np.abs(z)
+        sqrt_z = np.sqrt(2 * (1 - abs_z))
+        if abs_z == 1:  # (X, Y) = (0, 0)
+            continue
+        elif np.abs(y) <= np.abs(x):
+            sign_x = np.sign(x)
+            lambert_xy[i, 0] = sign_x * sqrt_z * SQRT_PI_OVER_2
+            lambert_xy[i, 1] = sign_x * sqrt_z * TWO_OVER_SQRT_PI * np.arctan(y / x)
+        else:
+            sign_y = np.sign(y)
+            lambert_xy[i, 0] = sign_y * sqrt_z * TWO_OVER_SQRT_PI * np.arctan(x / y)
+            lambert_xy[i, 1] = sign_y * sqrt_z * SQRT_PI_OVER_2
+
+    return lambert_xy
+
+
 @njit(
     (
         "Tuple((int32[:], int32[:], int32[:], int32[:], float64[:], float64[:], "
         "float64[:], float64[:]))(float64[:, :], int64, int64, float64)"
     ),
     cache=True,
     nogil=True,
@@ -630,15 +673,15 @@
     dim
         1D array of each vector's neighbouring row interpolation weight
         factor as 64-bit floats.
     djm
         1D array of each vector's neighbouring column interpolation
         weight factor as 64-bit floats.
     """
-    xy = scale * _vector2xy(v) / SQRT_PI_HALF
+    xy = scale * _vector2lambert(v) / SQRT_PI_HALF
 
     i = xy[:, 1]
     j = xy[:, 0]
 
     dtype = np.int32
     n = i.size
     nii = np.zeros(n, dtype=dtype)
```

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/_overwrite_hyperspy_methods.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/_overwrite_hyperspy_methods.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/array_tools.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/array_tools.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/tests/test_array_tools.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/tests/test_array_tools.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/tests/test_dask.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py` & `kikuchipy-0.9.0/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/signals/virtual_bse_image.py` & `kikuchipy-0.9.0/kikuchipy/signals/virtual_bse_image.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/simulations/__init__.py` & `kikuchipy-0.9.0/kikuchipy/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/simulations/_kikuchi_pattern_features.py` & `kikuchipy-0.9.0/kikuchipy/simulations/_kikuchi_pattern_features.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/simulations/_kikuchi_pattern_simulation.py` & `kikuchipy-0.9.0/kikuchipy/simulations/_kikuchi_pattern_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -456,20 +456,23 @@
         Returns
         -------
         collection
             Collection of lines.
         """
         coords = self.lines_coordinates(index, coordinates)
         coords = coords.reshape((coords.shape[0], 2, 2))
-        line_defaults = dict(
-            color="r", linewidth=1, alpha=1, zorder=1, label="kikuchi_lines"
-        )
-        for k, v in line_defaults.items():
-            kwargs.setdefault(k, v)
-        return mcollections.LineCollection(segments=list(coords), **kwargs)
+        kw = {
+            "color": "r",
+            "linewidth": 1,
+            "alpha": 1,
+            "zorder": 1,
+            "label": "kikuchi_lines",
+        }
+        kw.update(kwargs)
+        return mcollections.LineCollection(segments=list(coords), **kw)
 
     def _lines_as_markers(self, **kwargs) -> List[line_segment]:
         """Get Kikuchi lines as a list of HyperSpy markers.
 
         Parameters
         ----------
         **kwargs
@@ -479,27 +482,26 @@
         Returns
         -------
         lines_list
             List with line segment markers.
         """
         coords = self.lines_coordinates(index=(), exclude_nan=False)
         lines_list = []
-        segment_defaults = dict(color="r", zorder=1)
-        for k, v in segment_defaults.items():
-            kwargs.setdefault(k, v)
+        kw = {"color": "r", "zorder": 1}
+        kw.update(kwargs)
 
         for i in range(self._lines.vector.size):
             line = coords[..., i, :]
             if not np.all(np.isnan(line)):
                 # TODO: Inefficient, squeeze before the loop if possible
                 x1 = line[..., 0].squeeze()
                 y1 = line[..., 1].squeeze()
                 x2 = line[..., 2].squeeze()
                 y2 = line[..., 3].squeeze()
-                marker = line_segment(x1=x1, y1=y1, x2=x2, y2=y2, **kwargs)
+                marker = line_segment(x1=x1, y1=y1, x2=x2, y2=y2, **kw)
                 lines_list.append(marker)
 
         return lines_list
 
     def _pc_as_markers(self, **kwargs) -> list:
         """Return a list of projection center (PC) point markers.
 
@@ -529,18 +531,18 @@
 
         nrows, ncols = det.shape
         if nrows > 1:
             pcy *= nrows - 1
         if ncols > 1:
             pcx *= ncols - 1
 
-        for k, v in dict(size=300, marker="*", fc="gold", ec="k", zorder=4).items():
-            kwargs.setdefault(k, v)
+        kw = {"size": 300, "marker": "*", "fc": "gold", "ec": "k", "zorder": 4}
+        kw.update(kwargs)
 
-        pc_marker = point(x=pcx, y=pcy, **kwargs)
+        pc_marker = point(x=pcx, y=pcy, **kw)
 
         return [pc_marker]
 
     def _set_lines_detector_coordinates(self) -> None:
         """Set the start and end point coordinates of bands in
         uncalibrated detector coordinates (a scale of 1 and offset of
         0).
@@ -635,18 +637,17 @@
         if coordinates == "detector":
             scatter_size = 0.01 * self.detector.nrows
         else:  # gnomonic
             scatter_size = 0.01 * np.diff(self.detector.x_range)[0]
         circles = []
         for x, y in coords:
             circles.append(mpath.Path.circle((x, y), scatter_size))
-        path_defaults = dict(color="w", ec="k", zorder=1, label="zone_axes")
-        for k, v in path_defaults.items():
-            kwargs.setdefault(k, v)
-        return mcollections.PathCollection(circles, **kwargs)
+        kw = {"ec": "k", "fc": "w", "zorder": 1, "label": "zone_axes"}
+        kw.update(kwargs)
+        return mcollections.PathCollection(circles, **kw)
 
     def _zone_axes_labels_as_list(
         self, index: Union[int, tuple], coordinates: str, **kwargs
     ) -> list:
         """Get zone axes labels as a list of texts.
 
         Parameters
@@ -663,29 +664,28 @@
 
         Returns
         -------
         texts
             List of zone axes labels.
         """
         za = self._zone_axes
-        za_labels = za.vector.coordinates.round(0).astype(np.int64)
+        za_labels = za.vector.coordinates.round().astype(np.int64)
         za_labels_str = np.array2string(za_labels, threshold=za_labels.size)
         za_labels_list = re.sub("[][ ]", "", za_labels_str[1:-1]).split("\n")
         xy = self.zone_axes_coordinates(index, coordinates, exclude_nan=False)
         if coordinates == "detector":
             xy[..., 1] -= 0.03 * self.detector.nrows
         else:  # gnomonic
             xy[..., 1] += 0.03 * np.diff(self.detector.y_range)[0]
-        text_defaults = dict(ha="center", bbox=dict(boxstyle="square", fc="w", pad=0.1))
-        for k, v in text_defaults.items():
-            kwargs.setdefault(k, v)
+        kw = {"ha": "center", "bbox": {"boxstyle": "square", "fc": "w", "pad": 0.1}}
+        kw.update(kwargs)
         texts = []
         for (x, y), label in zip(xy, za_labels_list):
             if np.all(~np.isnan([x, y])):
-                text_i = mtext.Text(x, y, label, **kwargs)
+                text_i = mtext.Text(x, y, label, **kw)
                 texts.append(text_i)
         return texts
 
     def _zone_axes_as_markers(self, **kwargs) -> list:
         """Return a list of zone axes point markers.
 
         Parameters
@@ -698,22 +698,22 @@
         -------
         zone_axes_list
             List with zone axes markers.
         """
         coords = self.zone_axes_coordinates(index=(), exclude_nan=False)
         zone_axes_list = []
 
-        for k, v in dict(ec="none", zorder=2).items():
-            kwargs.setdefault(k, v)
+        kw = {"ec": "none", "zorder": 2}
+        kw.update(kwargs)
 
         for i in range(self._zone_axes.vector.size):
             # TODO: Inefficient, squeeze before the loop if possible
             zone_axis = coords[..., i, :].squeeze()
             if not np.all(np.isnan(zone_axis)):
-                marker = point(x=zone_axis[..., 0], y=zone_axis[..., 1], **kwargs)
+                marker = point(x=zone_axis[..., 0], y=zone_axis[..., 1], **kw)
                 zone_axes_list.append(marker)
 
         return zone_axes_list
 
     def _zone_axes_labels_as_markers(self, **kwargs) -> list:
         """Return a list of zone axes label text markers.
 
@@ -726,37 +726,37 @@
         Returns
         -------
         zone_axes_label_list
             List of text markers.
         """
         coords = self.zone_axes_coordinates(index=(), exclude_nan=False)
 
-        zone_axes = self._zone_axes.vector.coordinates.round(0).astype(np.int64)
+        zone_axes = self._zone_axes.vector.coordinates.round().astype(np.int64)
         array_str = np.array2string(zone_axes, threshold=zone_axes.size)
         texts = re.sub("[][ ]", "", array_str).split("\n")
 
-        for k, v in dict(
-            color="k",
-            zorder=3,
-            ha="center",
-            va="bottom",
-            bbox=dict(fc="w", ec="k", boxstyle="square", pad=0.2),
-        ).items():
-            kwargs.setdefault(k, v)
+        kw = {
+            "color": "k",
+            "zorder": 3,
+            "ha": "center",
+            "va": "bottom",
+            "bbox": {"fc": "w", "ec": "k", "boxstyle": "square", "pad": 0.2},
+        }
+        kw.update(kwargs)
 
         zone_axes_label_list = []
         is_finite = np.isfinite(coords)[..., 0]
         coords[~is_finite] = -1
 
         for i in range(zone_axes.shape[0]):
             if not np.allclose(coords[..., i, :], -1):  # All NaNs
                 x = coords[..., i, 0]
                 y = coords[..., i, 1]
                 x[~is_finite[..., i]] = np.nan
                 y[~is_finite[..., i]] = np.nan
                 # TODO: Inefficient, squeeze before the loop if possible
                 x = x.squeeze()
                 y = y.squeeze()
-                text_marker = text(x=x, y=y, text=texts[i], **kwargs)
+                text_marker = text(x=x, y=y, text=texts[i], **kw)
                 zone_axes_label_list.append(text_marker)
 
         return zone_axes_label_list
```

### Comparing `kikuchipy-0.8.7/kikuchipy/simulations/kikuchi_pattern_simulator.py` & `kikuchipy-0.9.0/kikuchipy/simulations/kikuchi_pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py` & `kikuchipy-0.9.0/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     ref.calculate_theta(20e3)
     return ref
 
 
 class TestGeometricalKikuchiPatternSimulation:
     """General features of the GeometricalKikuchiPatternSimulation
     class.
-
     """
 
     def setup_method(self):
         self.reflectors = setup_reflectors()
         self.detector = kp.detectors.EBSDDetector(shape=(60, 60))
         self.rotations = Rotation.stack(
             (Rotation.from_axes_angles([(0, 0, 1), (0, 0, -1)], np.deg2rad(80)),) * 2
@@ -143,15 +142,14 @@
         filters = logging.getLogger("matplotlib.text").filters
         assert filters == [kp.simulations.DisableMatplotlibWarningFilter]
 
 
 class TestAsCollections:
     """Getting lines, zone axes, zone axes labels and PC as Matplotlib
     collections.
-
     """
 
     def setup_method(self):
         self.reflectors = setup_reflectors()
         self.detector = kp.detectors.EBSDDetector(shape=(60, 60))
         self.rotations = Rotation.stack(
             (Rotation.from_axes_angles([(0, 0, 1), (0, 0, -1)], np.deg2rad(80)),) * 2
@@ -203,21 +201,22 @@
     def test_kwargs(self):
         simulator = kp.simulations.KikuchiPatternSimulator(self.reflectors)
         sim = simulator.on_detector(self.detector, self.rotations)
 
         coll = sim.as_collections(
             zone_axes=True,
             zone_axes_labels=True,
-            lines_kwargs=dict(linewidth=2),  # Default is 1
-            zone_axes_kwargs=dict(color="k"),  # Default is white
-            zone_axes_labels_kwargs=dict(fontsize=5),  # Default is 10
+            lines_kwargs={"linewidth": 2},  # Default is 1
+            zone_axes_kwargs={"fc": "r", "ec": "b"},
+            zone_axes_labels_kwargs={"fontsize": 5},  # Default is 10
         )
 
         assert coll[0].get_linewidth() == 2
-        assert np.allclose(coll[1].get_facecolor()[0][:3], 0)
+        assert np.allclose(coll[1].get_facecolor()[0][:3], [1, 0, 0])
+        assert np.allclose(coll[1].get_edgecolor()[0][:3], [0, 0, 1])
         assert coll[2][0].get_fontsize() == 5
 
     def test_coordinates(self):
         hkl_sets = self.reflectors.get_hkl_sets()
         ref200 = self.reflectors[hkl_sets[2, 0, 0]]
         simulator = kp.simulations.KikuchiPatternSimulator(ref200)
         sim = simulator.on_detector(self.detector, self.rotations)
@@ -240,15 +239,14 @@
         za_labels_coords2 = coll2[2][0]
         assert np.allclose(za_labels_coords2.get_position(), [0, 0.42], atol=0.01)
 
 
 class TestAsMarkers:
     """Getting lines, zone axes, zone axes labels and PC as HyperSpy
     markers.
-
     """
 
     def setup_method(self):
         self.reflectors = setup_reflectors()
         self.detector = kp.detectors.EBSDDetector(shape=(60, 60))
         self.rotations = Rotation.stack(
             (Rotation.from_axes_angles([(0, 0, 1), (0, 0, -1)], np.deg2rad(80)),) * 2
```

### Comparing `kikuchipy-0.8.7/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py` & `kikuchipy-0.9.0/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.7/kikuchipy.egg-info/SOURCES.txt` & `kikuchipy-0.9.0/kikuchipy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -93,18 +93,14 @@
 kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py
 kikuchipy/filters/__init__.py
 kikuchipy/filters/fft_barnes.py
 kikuchipy/filters/window.py
 kikuchipy/filters/tests/__init__.py
 kikuchipy/filters/tests/test_fft_barnes.py
 kikuchipy/filters/tests/test_window.py
-kikuchipy/generators/__init__.py
-kikuchipy/generators/virtual_bse_generator.py
-kikuchipy/generators/tests/__init__.py
-kikuchipy/generators/tests/test_virtual_bse_generator.py
 kikuchipy/imaging/__init__.py
 kikuchipy/imaging/vbse.py
 kikuchipy/imaging/tests/__init__.py
 kikuchipy/imaging/tests/test_virtual_bse_imager.py
 kikuchipy/indexing/__init__.py
 kikuchipy/indexing/_dictionary_indexing.py
 kikuchipy/indexing/_hough_indexing.py
@@ -163,24 +159,14 @@
 kikuchipy/io/tests/test_util.py
 kikuchipy/pattern/__init__.py
 kikuchipy/pattern/_pattern.py
 kikuchipy/pattern/chunk.py
 kikuchipy/pattern/tests/__init__.py
 kikuchipy/pattern/tests/test_chunk.py
 kikuchipy/pattern/tests/test_pattern.py
-kikuchipy/projections/__init__.py
-kikuchipy/projections/gnomonic_projection.py
-kikuchipy/projections/hesse_normal_form.py
-kikuchipy/projections/lambert_projection.py
-kikuchipy/projections/spherical_projection.py
-kikuchipy/projections/tests/__init__.py
-kikuchipy/projections/tests/test_gnomonic_projection.py
-kikuchipy/projections/tests/test_hesse_normal_form.py
-kikuchipy/projections/tests/test_lambert_projection.py
-kikuchipy/projections/tests/test_spherical_projection.py
 kikuchipy/signals/__init__.py
 kikuchipy/signals/_kikuchi_master_pattern.py
 kikuchipy/signals/_kikuchipy_signal.py
 kikuchipy/signals/ebsd.py
 kikuchipy/signals/ebsd_master_pattern.py
 kikuchipy/signals/ecp_master_pattern.py
 kikuchipy/signals/virtual_bse_image.py
```

### Comparing `kikuchipy-0.8.7/kikuchipy.egg-info/requires.txt` & `kikuchipy-0.9.0/kikuchipy.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,72 @@
 dask[array]>=2021.8.1
 diffpy.structure>=3
-diffsims>=0.5
-hyperspy>=1.7.3
+diffsims>=0.5.1
+hyperspy<2,>=1.7.3
 h5py>=2.10
 imageio
-matplotlib>=3.3
+matplotlib>=3.5
 numba>=0.55
-numpy>=1.19
+numpy>=1.21.6
 orix>=0.11.1
-pooch>=0.13
+pooch>=1.3.0
 pyyaml
 tqdm>=0.5.2
 scikit-image>=0.16.2
 scikit-learn
 scipy>=1.7
 
 [all]
 matplotlib>=3.5
 nlopt
-pyebsdindex~=0.1
+pyebsdindex~=0.2
 pyvista
 
 [dev]
 black[jupyter]>=23.1
 manifix
 outdated
 pre-commit>=1.16
 memory_profiler
 nbsphinx>=0.7
 numpydoc
 nlopt
-panel
 pydata-sphinx-theme
-pyebsdindex>=0.1.1
+pyebsdindex~=0.2
 pyvista
 sphinx>=3.0.2
 sphinx-codeautolink[ipython]<0.14
 sphinx-copybutton>=0.2.5
 sphinx-design
 sphinx-gallery
 sphinxcontrib-bibtex>=1.0
 coverage>=5.0
 pytest>=5.4
 pytest-benchmark
 pytest-cov>=2.8.1
+pytest-rerunfailures
 pytest-xdist
 matplotlib>=3.5
-pyebsdindex~=0.1
 
 [doc]
 memory_profiler
 nbsphinx>=0.7
 numpydoc
 nlopt
-panel
 pydata-sphinx-theme
-pyebsdindex>=0.1.1
+pyebsdindex~=0.2
 pyvista
 sphinx>=3.0.2
 sphinx-codeautolink[ipython]<0.14
 sphinx-copybutton>=0.2.5
 sphinx-design
 sphinx-gallery
 sphinxcontrib-bibtex>=1.0
 
 [tests]
 coverage>=5.0
 numpydoc
 pytest>=5.4
 pytest-benchmark
 pytest-cov>=2.8.1
+pytest-rerunfailures
 pytest-xdist
-
-[viz]
-matplotlib>=3.5
-pyvista
```

### Comparing `kikuchipy-0.8.7/readthedocs.yaml` & `kikuchipy-0.9.0/readthedocs.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 sphinx:
   configuration: doc/conf.py
 
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-22.04
   tools:
-    python: "3.10"
+    python: "mambaforge-22.9"
     nodejs: "19"
-  # See https://docs.pyvista.org/user-guide/jupyter/panel.html#configuration-considerations.
-  # These packages are needed by PyVista/panel to render 3D plots from
-  # RTD's server.
+  # Some of these packages are needed by PyVista/Trame to render 3D
+  # plots from RTD's server.
   apt_packages:
+    - imagemagick
     - libgl1-mesa-dev
     - xvfb
 
 # Build doc in all formats (HTML, PDF and ePub)
 formats:
   - htmlzip
   - pdf
 
+conda:
+  environment: doc/environment.yml
+
 # Python environment for building the docs
 python:
   install:
     - method: pip
       path: .
       extra_requirements:
         - doc
-        - viz
```

### Comparing `kikuchipy-0.8.7/setup.cfg` & `kikuchipy-0.9.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 	--ignore=kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py
 	--ignore=kikuchipy/data/edax_binary/create_edax_binary_file.py
 	--ignore=kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py
 	--ignore=kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py
 	--ignore=kikuchipy/data/oxford_binary/create_oxford_binary_file.py
 	--ignore-glob=kikuchipy/data/emsoft_ebsd_master_pattern/*.py
 doctest_optionflags = NORMALIZE_WHITESPACE
+filterwarnings = 
+	ignore:Deprecated call to \`pkg_resources:DeprecationWarning
+	ignore:pkg_resources is deprecated as an API:DeprecationWarning
+	ignore:module \'sre_:DeprecationWarning
 
 [coverage:run]
 source = kikuchipy
 omit = 
 	setup.py
 	kikuchipy/release.py
 relative_files = True
```

### Comparing `kikuchipy-0.8.7/setup.py` & `kikuchipy-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,42 +43,43 @@
 # fmt: off
 extra_feature_requirements = {
     "doc": [
         "memory_profiler",
         "nbsphinx                       >= 0.7",
         "numpydoc",
         "nlopt",
-        "panel",  # Used in the docs by PyVista
         "pydata-sphinx-theme",
-        "pyebsdindex                    >= 0.1.1",
+        "pyebsdindex                    ~= 0.2",
         "pyvista",
         "sphinx                         >= 3.0.2",
         "sphinx-codeautolink[ipython]   < 0.14",
         "sphinx-copybutton              >= 0.2.5",
         "sphinx-design",
         "sphinx-gallery",
         "sphinxcontrib-bibtex           >= 1.0",
     ],
     "tests": [
         "coverage                       >= 5.0",
         "numpydoc",
         "pytest                         >= 5.4",
         "pytest-benchmark",
         "pytest-cov                     >= 2.8.1",
+        "pytest-rerunfailures",
         "pytest-xdist",
     ],
     "all": [
         "matplotlib                     >= 3.5",
         "nlopt",
-        "pyebsdindex                    ~= 0.1",
-        "pyvista",
-    ],
-    # TODO: Remove this option in release 0.9
-    "viz": [
-        "matplotlib                     >= 3.5",
+        # We ask for a compatible release of PyEBSDIndex as we
+        # anticipate breaking changes in coming releases. We do so
+        # because there were breaking changes between 0.1.2 and 0.2.0.
+        # We can change from ~= to >= once we consider PyEBSDIndex
+        # stable. This is typically when a minor release with no or
+        # only minor breaking changes is made available.
+        "pyebsdindex                    ~= 0.2",
         "pyvista",
     ],
 }
 # fmt: on
 
 # Create a development project including all extra dependencies
 extra_feature_requirements["dev"] = [
@@ -104,14 +105,15 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         (
             "License :: OSI Approved :: GNU General Public License v3 or later "
             "(GPLv3+)"
         ),
         "Natural Language :: English",
@@ -146,23 +148,23 @@
     },
     # Dependencies
     extras_require=extra_feature_requirements,
     # fmt: off
     install_requires=[
         "dask[array]        >= 2021.8.1",
         "diffpy.structure   >= 3",
-        "diffsims           >= 0.5",
-        "hyperspy           >= 1.7.3",
+        "diffsims           >= 0.5.1",
+        "hyperspy           >= 1.7.3, < 2",
         "h5py               >= 2.10",
         "imageio",
-        "matplotlib         >= 3.3",
+        "matplotlib         >= 3.5",
         "numba              >= 0.55",
-        "numpy              >= 1.19",
+        "numpy              >= 1.21.6",
         "orix               >= 0.11.1",
-        "pooch              >= 0.13",
+        "pooch              >= 1.3.0",
         "pyyaml",
         "tqdm               >= 0.5.2",
         "scikit-image       >= 0.16.2",
         "scikit-learn",
         "scipy              >= 1.7",
     ],
     # fmt: on
```

