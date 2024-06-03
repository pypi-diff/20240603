# Comparing `tmp/lumicks.pylake-1.5.0.tar.gz` & `tmp/lumicks.pylake-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumicks.pylake-1.5.0.tar", last modified: Tue May 28 17:50:23 2024, max compression
+gzip compressed data, was "lumicks.pylake-1.5.1.tar", last modified: Mon Jun  3 11:45:13 2024, max compression
```

## Comparing `lumicks.pylake-1.5.0.tar` & `lumicks.pylake-1.5.1.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.311416 lumicks.pylake-1.5.0/lumicks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.319416 lumicks.pylake-1.5.0/lumicks/pylake/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/adjustments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.323416 lumicks.pylake-1.5.0/lumicks/pylake/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/bead_cropping.py
--rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/confocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/h5_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.323416 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.323416 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum0.npz
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum1.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum2.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum4.npz
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum6.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum7.npz
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_bead_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_widefield.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/timeindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    27375 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/widefield.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fdensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    14770 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/file_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.327416 lumicks.pylake-1.5.0/lumicks/pylake/fitting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.327416 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/derivative_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/link_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    42415 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/model_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    29579 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/fitdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    29584 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35226 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/parameter_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    25485 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/profile_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.327416 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_condition_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fd_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    26073 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stderr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stepping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.331416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41587 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/calibration_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/convenience.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.331416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/drag_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/driving_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/power_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/salty_water.py
--rw-r--r--   0 runner    (1001) docker     (127)    11214 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.331416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.335416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95740 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.335416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/1BGJQSPSHIFNM841G0X0WP2UL.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/3H9KBT8A28K43BCYEHIE0JD4L.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/5OF2DCE6DXL0LGPCPCPHOA3TH.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/7IJO3KH5G90URX2B9RYTYQKPG.json
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/999SUSJ01D14ZSRH7M58HWXHV.json
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/9M9JZPD6GZ6UA62TR9OG5MDUJ.json
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/ALYF6CK1Y54466J549VJ1BSJM.json
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/BCF825GIR11ZFL6ZQKN4D7K21.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/E45ZBFK5MYVRD1J9N8ITG6EQ4.json
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/E6JD3GX1S6X68LXWJED5VFZOJ.json
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_axial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_camera_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_convenience.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_diode_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_driving_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    19093 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_hydro.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    25575 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_touchdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/touchdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    26193 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/image_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    47726 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.335416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.339416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/denoising.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/linalg_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/localization_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    44177 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/msd_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    21264 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/scoring_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/stitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19721 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    81248 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (127)    27371 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/stitching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.339416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.343416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.343416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_no_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_no_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_1d.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_2d.npz
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_denoise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.343416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    61826 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_loc_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_stitching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/correlated_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/undostack.py
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/image_editing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38089 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/range_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_undostack.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/piezo_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/point_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/population/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/fit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    55527 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/dwelltime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    34952 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/exponential_data.npz
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_exponential_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_trace_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/trace_data.npz
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_dwelltimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/test_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.355416 lumicks.pylake-1.5.0/lumicks/pylake/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.355416 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_confocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_widefield.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/test_mock_confocal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/2MOF2FD1NDYBUVE5V2UV5OE5.npz
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/49IRJMNKF3XEAQ6L2D38AFYC6.npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/4RRE8ZG26TWBKKOUPK6CPFBIX.npz
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/4TWTXTHAKH5N6BMWZI6KUMKK5.json
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/5CBUUDH5DX4QNMKTT2J2B96GL.npz
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.npz
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/852E6XRLZFHJN2FQRJQPONQVA.json
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/9WDSTMR98ABMBPK6VPBYU3WFF.npz
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/AELM9ISISBZJQ3AUKZIO6PZ7K.npz
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/CMJN00XGRVG6SLMBMEJH8BKJK.npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/EC0P3CT7JCJYDCD86TWKIQNGY.npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/forced_filename_1.npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/forced_filename_2.npz
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/ref_dict_freezing_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/ref_dict_freezing_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/data/
--rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/21U0E1PWIF4T1V9BXHMY9P90F.npz
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/56OBGN66YAHPLZDQ8KXKGCI2P.npz
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    52907 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/data/
--rw-r--r--   0 runner    (1001) docker     (127)   221862 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_import_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_scalebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_timeindex.py
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.319416 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/setup.manifest
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.861574 lumicks.pylake-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-06-03 11:45:13.861574 lumicks.pylake-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.809574 lumicks.pylake-1.5.1/lumicks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.817574 lumicks.pylake-1.5.1/lumicks/pylake/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/adjustments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.821574 lumicks.pylake-1.5.1/lumicks/pylake/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/bead_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/confocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/h5_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.821574 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.821574 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum0.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum1.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum6.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum7.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/test_bead_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/test_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27375 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/detail/widefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fdensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15833 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/file_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.821574 lumicks.pylake-1.5.1/lumicks/pylake/fitting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.825574 lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/derivative_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/link_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42415 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/model_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29579 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/fitdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29584 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35226 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/parameter_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25485 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/profile_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.825574 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_condition_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_fd_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26073 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_model_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_model_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_parameter_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_stepping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.825574 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41587 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/calibration_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/convenience.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.829574 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/drag_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/hydrodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/power_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/salty_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11214 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/power_spectrum_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.829574 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.829574 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95740 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.833574 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/1BGJQSPSHIFNM841G0X0WP2UL.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/3H9KBT8A28K43BCYEHIE0JD4L.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/5OF2DCE6DXL0LGPCPCPHOA3TH.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/7IJO3KH5G90URX2B9RYTYQKPG.json
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/999SUSJ01D14ZSRH7M58HWXHV.json
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/9M9JZPD6GZ6UA62TR9OG5MDUJ.json
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/ALYF6CK1Y54466J549VJ1BSJM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/BCF825GIR11ZFL6ZQKN4D7K21.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/E45ZBFK5MYVRD1J9N8ITG6EQ4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/E6JD3GX1S6X68LXWJED5VFZOJ.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_active_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_axial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_camera_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_diode_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19093 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_power_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25575 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26193 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/image_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47726 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.833574 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.833574 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/denoising.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/linalg_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/localization_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44177 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/msd_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21264 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/scoring_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/stitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19721 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/trace_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81248 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27371 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/kymotracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/stitching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.837574 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.841574 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.841574 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/1d_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/1d_no_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/2d_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/2d_no_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/output_image_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/output_image_2d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_denoise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.841574 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_image_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61826 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_loc_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_stitching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.841574 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/correlated_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.841574 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/detail/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/detail/undostack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38089 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/kymotracker_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/range_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.845574 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_undostack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.845574 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/piezo_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.845574 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/tests/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/point_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.845574 lumicks.pylake-1.5.1/lumicks/pylake/population/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.845574 lumicks.pylake-1.5.1/lumicks/pylake/population/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/detail/fit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/detail/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/detail/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/detail/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55527 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/dwelltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.845574 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.849574 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    34952 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/exponential_data.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/generate_exponential_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/generate_trace_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/trace_data.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_dwelltimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_hmm_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.849574 lumicks.pylake-1.5.1/lumicks/pylake/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/simulation/diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.849574 lumicks.pylake-1.5.1/lumicks/pylake/simulation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/simulation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/simulation/tests/test_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.849574 lumicks.pylake-1.5.1/lumicks/pylake/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.849574 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_confocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/data/test_mock_confocal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.853574 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/2MOF2FD1NDYBUVE5V2UV5OE5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/49IRJMNKF3XEAQ6L2D38AFYC6.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/4RRE8ZG26TWBKKOUPK6CPFBIX.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/4TWTXTHAKH5N6BMWZI6KUMKK5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/5CBUUDH5DX4QNMKTT2J2B96GL.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/852E6XRLZFHJN2FQRJQPONQVA.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/9WDSTMR98ABMBPK6VPBYU3WFF.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/AELM9ISISBZJQ3AUKZIO6PZ7K.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/CMJN00XGRVG6SLMBMEJH8BKJK.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/EC0P3CT7JCJYDCD86TWKIQNGY.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/forced_filename_1.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/forced_filename_2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/ref_dict_freezing_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/ref_dict_freezing_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.853574 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_fdensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.853574 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19547 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/test_file_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.857574 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.857574 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.857574 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/ref_data/21U0E1PWIF4T1V9BXHMY9P90F.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/ref_data/56OBGN66YAHPLZDQ8KXKGCI2P.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52907 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.857574 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.857574 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   221862 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/lumicks/pylake/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:45:13.813574 lumicks.pylake-1.5.1/lumicks.pylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-06-03 11:45:13.000000 lumicks.pylake-1.5.1/lumicks.pylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-06-03 11:45:13.000000 lumicks.pylake-1.5.1/lumicks.pylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:45:13.000000 lumicks.pylake-1.5.1/lumicks.pylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:45:13.000000 lumicks.pylake-1.5.1/lumicks.pylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 11:45:13.000000 lumicks.pylake-1.5.1/lumicks.pylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 11:45:13.000000 lumicks.pylake-1.5.1/lumicks.pylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-03 11:45:13.861574 lumicks.pylake-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/setup.manifest
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-06-03 11:45:03.000000 lumicks.pylake-1.5.1/setup.py
```

### Comparing `lumicks.pylake-1.5.0/PKG-INFO` & `lumicks.pylake-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.5.0
+Version: 1.5.1
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lumicks.pylake-1.5.0/license.md` & `lumicks.pylake-1.5.1/license.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/__init__.py` & `lumicks.pylake-1.5.1/lumicks/pylake/__init__.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/adjustments.py` & `lumicks.pylake-1.5.1/lumicks/pylake/adjustments.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/benchmark.py` & `lumicks.pylake-1.5.1/lumicks/pylake/benchmark.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/calibration.py` & `lumicks.pylake-1.5.1/lumicks/pylake/calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/channel.py` & `lumicks.pylake-1.5.1/lumicks/pylake/channel.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/alignment.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/alignment.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/bead_cropping.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/bead_cropping.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/confocal.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/h5_helper.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/h5_helper.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/image.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/imaging_mixins.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/imaging_mixins.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/mixin.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/plotting.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum0.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum0.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum1.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum1.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum2.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum2.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum3.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum3.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum4.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum4.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum5.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum5.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum6.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum6.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum7.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/data/kymo_sum7.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_bead_crop.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/test_bead_crop.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_plotting.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_widefield.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/tests/test_widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/timeindex.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/utilities.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/detail/widefield.py` & `lumicks.pylake-1.5.1/lumicks/pylake/detail/widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fdcurve.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fdensemble.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/file.py` & `lumicks.pylake-1.5.1/lumicks/pylake/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,18 @@
     """A convenient HDF5 file wrapper for reading data exported from Bluelake
 
     Parameters
     ----------
     filename : str | os.PathLike
         The HDF5 file to open in read-only mode
 
-    rgb_to_detectors : Dict[Color, str]
-        Dictionary that maps RGB colors to a photon detector channel (either photon counts, or photon time tags)
+    rgb_to_detectors : Optional[Dict[str, str]]
+        Dictionary that maps RGB colors to a photon detector channel (either photon counts, or
+        photon time tags). Note that a channel can be left empty by providing the channel name
+        "None". Valid colors are ("Red", "Green", "Blue").
 
     Examples
     --------
     ::
 
         from lumicks import pylake
 
@@ -44,21 +46,17 @@
     """
 
     SUPPORTED_FILE_FORMAT_VERSIONS = [1, 2]
 
     def __init__(self, filename, *, rgb_to_detectors=None):
         import h5py
 
-        if rgb_to_detectors is None:
-            rgb_to_detectors = {"Red": "Red", "Green": "Green", "Blue": "Blue"}
-
-        self._rgb_to_detectors = rgb_to_detectors
         super().__init__(h5py.File(filename, "r"), lk_file=self)
         self._check_file_format()
-        self._check_detector_mapping()
+        self._rgb_to_detectors = self._get_detector_mapping(rgb_to_detectors)
 
     def _check_file_format(self):
         if "Bluelake version" not in self.h5.attrs:
             raise Exception("Invalid HDF5 file: no Bluelake version tag found")
         if "File format version" not in self.h5.attrs:
             raise Exception("Invalid HDF5 file: no file format version tag found")
         ff_version = int(self.h5.attrs["File format version"])
@@ -76,41 +74,66 @@
             "FD Curve": ("fdcurves", FdCurve),
             "Kymograph": ("kymos", Kymo),
             "Scan": ("scans", Scan),
             "Note": ("notes", Note),
             "Point Scan": ("point_scans", PointScan),
         }
 
-    def _check_detector_mapping(self):
-        detectors = set()
-        if "Photon time tags" in self.h5:
-            detectors = set(self.h5["Photon time tags"])
-        elif "Photon count" in self.h5:
-            detectors = set(self.h5["Photon count"])
-
-        # Only check if detector data was exported
-        if not detectors:
-            return
-
-        if not_found := set(self._rgb_to_detectors.values()) - detectors:
-            raise Exception(
-                f"Invalid RGB to detector mapping: {not_found} photon count channel(s) are missing, images cant't be reconstructed. Available detectors: {detectors}"
-            )
+    def _get_detector_mapping(self, rgb_to_detectors=None):
+        """Returns the detector mapping to be used.
+
+        Parameters
+        ----------
+        rgb_to_detectors : Optional[Dict[str, str]]
+            Dictionary that maps RGB colors to a photon detector channel (either photon counts, or
+            photon time tags). Note that a channel can be left empty by providing the channel name
+            "None".
+        """
+
+        def check_custom_detector_mapping():
+            for key in rgb_to_detectors.keys():
+                if key not in ("Red", "Green", "Blue"):
+                    raise ValueError(
+                        f'Invalid color mapping ({key}). Valid colors are "Red", "Green" or "Blue"'
+                    )
+
+            detectors = set()
+            if "Photon time tags" in self.h5:
+                detectors = set(self.h5["Photon time tags"])
+            elif "Photon count" in self.h5:
+                detectors = set(self.h5["Photon count"])
+
+            # Only check if detector data was exported
+            if not detectors:
+                return
+
+            # "None" indicates that the user doesn't want to plot data for that particular channel.
+            if not_found := (set(rgb_to_detectors.values()) - {"None"}) - detectors:
+                warnings.warn(
+                    RuntimeWarning(
+                        f"Invalid RGB to detector mapping: {not_found} photon count channel(s) are "
+                        f"missing. Those channels will be blank in images. Available detectors: "
+                        f"{detectors}"
+                    )
+                )
+
+        if rgb_to_detectors:
+            check_custom_detector_mapping()
+            return rgb_to_detectors
+        else:
+            return {"Red": "Red", "Green": "Green", "Blue": "Blue"}
 
     @classmethod
     def from_h5py(cls, h5py_file, *, rgb_to_detectors=None):
         """Directly load an existing `h5py.File <https://docs.h5py.org/en/latest/high/file.html>`_"""
         new_file = cls.__new__(cls)
         new_file.h5 = h5py_file
         new_file._lk_file = new_file
         new_file._check_file_format()
-        if rgb_to_detectors is None:
-            rgb_to_detectors = {"Red": "Red", "Green": "Green", "Blue": "Blue"}
-        new_file._rgb_to_detectors = rgb_to_detectors
-        new_file._check_detector_mapping()
+        new_file._rgb_to_detectors = new_file._get_detector_mapping(rgb_to_detectors)
         return new_file
 
     @property
     def bluelake_version(self) -> str:
         """The version of Bluelake which exported this file"""
         return self.h5.attrs["Bluelake version"]
```

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/file_download.py` & `lumicks.pylake-1.5.1/lumicks/pylake/file_download.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/datasets.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/datasets.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/derivative_manipulation.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/derivative_manipulation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/link_functions.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/link_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/model_implementation.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/model_implementation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/utilities.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/fit.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/fitdata.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/fitdata.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/model.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/model.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/parameter_trace.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/parameter_trace.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/parameters.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/parameters.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/profile_likelihood.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/profile_likelihood.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_condition_handling.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_condition_handling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fd_models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_fd_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fit.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_composition.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_model_composition.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_sim.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_model_sim.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_parameter_inversion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_parameters.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_pickling.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_profiles.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stderr.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_stderr.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stepping.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_stepping.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_utilities.py` & `lumicks.pylake-1.5.1/lumicks/pylake/fitting/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/calibration_models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/calibration_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/convenience.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/convenience.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/drag_models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/drag_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/driving_input.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/driving_input.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/hydrodynamics.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/power_models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/power_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/salty_water.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/detail/salty_water.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/power_spectrum.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/power_spectrum_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/1BGJQSPSHIFNM841G0X0WP2UL.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/1BGJQSPSHIFNM841G0X0WP2UL.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/3H9KBT8A28K43BCYEHIE0JD4L.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/3H9KBT8A28K43BCYEHIE0JD4L.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/5OF2DCE6DXL0LGPCPCPHOA3TH.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/5OF2DCE6DXL0LGPCPCPHOA3TH.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/7IJO3KH5G90URX2B9RYTYQKPG.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/7IJO3KH5G90URX2B9RYTYQKPG.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/999SUSJ01D14ZSRH7M58HWXHV.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/999SUSJ01D14ZSRH7M58HWXHV.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/9M9JZPD6GZ6UA62TR9OG5MDUJ.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/9M9JZPD6GZ6UA62TR9OG5MDUJ.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/ALYF6CK1Y54466J549VJ1BSJM.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/ALYF6CK1Y54466J549VJ1BSJM.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/BCF825GIR11ZFL6ZQKN4D7K21.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/BCF825GIR11ZFL6ZQKN4D7K21.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/E45ZBFK5MYVRD1J9N8ITG6EQ4.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/E45ZBFK5MYVRD1J9N8ITG6EQ4.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/E6JD3GX1S6X68LXWJED5VFZOJ.json` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/ref_data/E6JD3GX1S6X68LXWJED5VFZOJ.json`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_active_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_axial.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_axial.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_camera_calibration.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_camera_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_convenience.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_convenience.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_diode_models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_diode_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_driving_input.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_driving_input.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_hydro.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_hydro.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_model.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_power_model.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_power_spectrum.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_simulations.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_touchdown.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/tests/test_touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/touchdown.py` & `lumicks.pylake-1.5.1/lumicks/pylake/force_calibration/touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/group.py` & `lumicks.pylake-1.5.1/lumicks/pylake/group.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/image_stack.py` & `lumicks.pylake-1.5.1/lumicks/pylake/image_stack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymo.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymo.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/denoising.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/denoising.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/geometry_2d.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/linalg_2d.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/linalg_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/localization_models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/localization_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/msd_estimation.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/msd_estimation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/peakfinding.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/scoring_functions.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/sequence.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/stitch.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/stitch.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/detail/trace_line_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotrack.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/kymotrack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotracker.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/kymotracker.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/stitching.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/test_sequence.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_background.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/1d_background.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_no_background.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/1d_no_background.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_background.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/2d_background.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_no_background.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/2d_no_background.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_1d.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/output_image_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_2d.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/ref_data/output_image_2d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_denoise.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_denoise.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_image_sampling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_io.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_kymotrack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_loc_models.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_loc_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_refinement.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_refinement.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_sequence.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_stitching.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_tracing.py` & `lumicks.pylake-1.5.1/lumicks/pylake/kymotracker/tests/test_tracing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/marker.py` & `lumicks.pylake-1.5.1/lumicks/pylake/marker.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/correlated_plot.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/correlated_plot.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/mouse.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/detail/mouse.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/undostack.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/detail/undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/image_editing.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/kymotracker_widgets.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/range_selector.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/range_selector.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_fd_selector.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_mouse.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_mouse.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_undostack.py` & `lumicks.pylake-1.5.1/lumicks/pylake/nb_widgets/tests/test_undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/note.py` & `lumicks.pylake-1.5.1/lumicks/pylake/note.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/baseline.py` & `lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/piezo_tracking.py` & `lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py` & `lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/tests/test_baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py` & `lumicks.pylake-1.5.1/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/point_scan.py` & `lumicks.pylake-1.5.1/lumicks/pylake/point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/detail/fit_info.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/detail/fit_info.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/detail/hmm.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/detail/hmm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/detail/mixin.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/detail/mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/dwelltime.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/dwelltime.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/hmm.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/hmm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/mixture.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/mixture.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/exponential_data.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/exponential_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_exponential_data.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/generate_exponential_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_trace_data.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/generate_trace_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/trace_data.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/data/trace_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_dwelltimes.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_dwelltimes.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_hmm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm_algos.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_hmm_algos.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_mixture.py` & `lumicks.pylake-1.5.1/lumicks/pylake/population/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/scalebar.py` & `lumicks.pylake-1.5.1/lumicks/pylake/scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/scan.py` & `lumicks.pylake-1.5.1/lumicks/pylake/scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/simulation/diffusion.py` & `lumicks.pylake-1.5.1/lumicks/pylake/simulation/diffusion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/test_diffusion.py` & `lumicks.pylake-1.5.1/lumicks/pylake/simulation/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_confocal.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_fdcurve.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_file.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_json.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_json.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_widefield.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/data/mock_widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/test_mock_confocal.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/data/test_mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_arithmetic.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_channels.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_channels/test_channels.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdcurve.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdensemble.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,7 +219,22 @@
 
     freq = 1e9 / 16
     mock_file.make_continuous_channel("Photon count", "Detector 1", np.int64(20e9), freq, counts)
     mock_file.make_continuous_channel("Photon count", "Detector 2", np.int64(20e9), freq, counts)
     mock_file.make_continuous_channel("Photon count", "Detector 3", np.int64(20e9), freq, counts)
     mock_file.make_continuous_channel("Info wave", "Info wave", np.int64(20e9), freq, infowave)
     return mock_file.file
+
+
+@pytest.fixture(scope="module", params=[MockDataFile_v2])
+def h5_two_colors(tmpdir_factory, request):
+    mock_class = request.param
+
+    tmpdir = tmpdir_factory.mktemp("pylake")
+    mock_file = mock_class(tmpdir.join("%s.h5" % mock_class.__class__.__name__))
+    mock_file.write_metadata()
+
+    freq = 1e9 / 16
+    mock_file.make_continuous_channel("Photon count", "Red", np.int64(20e9), freq, counts)
+    mock_file.make_continuous_channel("Photon count", "Blue", np.int64(20e9), freq, counts)
+    mock_file.make_continuous_channel("Info wave", "Info wave", np.int64(20e9), freq, infowave)
+    return mock_file.file
```

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/test_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -467,15 +467,68 @@
         else:
             assert (
                 "PointScan1" not in f["Point Scan"]
                 or not f["Point Scan"]["PointScan1"].red_photon_count
             )
 
 
-def test_detector_mapping(h5_custom_detectors):
-    f = pylake.File.from_h5py(
+def test_detector_mapping(h5_custom_detectors, h5_two_colors):
+    custom_correct = pylake.File.from_h5py(
         h5_custom_detectors,
         rgb_to_detectors={"Red": "Detector 1", "Green": "Detector 2", "Blue": "Detector 3"},
     )
-    with pytest.raises(Exception):
-        f = pylake.File.from_h5py(h5_custom_detectors, match="Invalid RGB to detector mapping")
-    assert np.any(f.red_photon_count.data)
+    assert custom_correct.red_photon_count.data.size
+    assert custom_correct.green_photon_count.data.size
+    assert custom_correct.blue_photon_count.data.size
+
+    # None of these exist, since this is a custom photon count file
+    with pytest.warns(RuntimeWarning, match="Invalid RGB to detector mapping"):
+        custom_empty = pylake.File.from_h5py(
+            h5_custom_detectors, rgb_to_detectors={"Red": "Red", "Green": "Green", "Blue": "Blue"}
+        )
+        assert not custom_empty.red_photon_count.data.size
+        assert not custom_empty.green_photon_count.data.size
+        assert not custom_empty.blue_photon_count.data.size
+
+    # Green photon count channel doesn't exist, so we issue a warning about this
+    with pytest.warns(RuntimeWarning, match="Invalid RGB to detector mapping"):
+        two_color = pylake.File.from_h5py(
+            h5_two_colors, rgb_to_detectors={"Red": "Red", "Green": "Green", "Blue": "Blue"}
+        )
+        assert two_color.red_photon_count.data.size
+        assert not two_color.green_photon_count.data.size
+        assert two_color.blue_photon_count.data.size
+
+    # Green photon count channel doesn't exist, _but_ we are using defaults, so we do not explicitly
+    # issue a warning (this is the old reference behavior). People may not even want to show
+    # images, so it's weird to bother them with a warning.
+    two_color_default = pylake.File.from_h5py(h5_two_colors)
+    assert two_color_default.red_photon_count.data.size
+    assert not two_color_default.green_photon_count.data.size
+    assert two_color_default.blue_photon_count.data.size
+
+    # Valid mapping
+    double_red = pylake.File.from_h5py(
+        h5_two_colors, rgb_to_detectors={"Red": "Red", "Green": "Red", "Blue": "Blue"}
+    )
+    np.testing.assert_allclose(double_red.green_photon_count.data, two_color.red_photon_count.data)
+    assert double_red.blue_photon_count.data.size
+
+    # Explicitly setting `"None"` doesn't issue a warning
+    no_green = pylake.File.from_h5py(
+        h5_two_colors, rgb_to_detectors={"Red": "Red", "Green": "None", "Blue": "Blue"}
+    )
+    assert no_green.red_photon_count.data.size
+    assert not no_green.green_photon_count.data.size
+    assert no_green.blue_photon_count.data.size
+
+
+@pytest.mark.parametrize(
+    "mapping",
+    [
+        {"red": "Red", "green": "Red", "blue": "Blue"},  # Incorrect capitalization
+        {"Red": "Red", "Magenta": "Red", "Blue": "Blue"},  # Wrong name
+    ],
+)
+def test_detector_mapping_invalid_color(h5_two_colors, mapping):
+    with pytest.raises(ValueError, match="Invalid color mapping"):
+        pylake.File.from_h5py(h5_two_colors, rgb_to_detectors=mapping)
```

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file_items.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file/test_file_items.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file_download.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_file_download.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_image.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/21U0E1PWIF4T1V9BXHMY9P90F.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/ref_data/21U0E1PWIF4T1V9BXHMY9P90F.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/56OBGN66YAHPLZDQ8KXKGCI2P.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/ref_data/56OBGN66YAHPLZDQ8KXKGCI2P.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_export.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/test_export.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1201,15 +1201,15 @@
 
     pixelsize = pixel_size if pixel_size else 1
     tether_start, half_window = 2, 1
     with_tether = stack.define_tether(
         (tether_start * pixelsize, 10 * pixelsize), (26 * pixelsize, 10 * pixelsize)
     )
     kymo = with_tether.to_kymo(half_window=half_window, reduce=np.sum)
-    lines = track_greedy(kymo, "red", pixel_threshold=3)
+    lines = track_greedy(kymo, "red", pixel_threshold=4)
     np.testing.assert_allclose(
         lines[0].position, [(position - tether_start) * pixelsize] * num_images
     )
     np.testing.assert_allclose(np.max(kymo.get_image("red")), 5 * (1 + 2 * half_window))
     np.testing.assert_equal(kymo.pixelsize_um[0], pixel_size)
```

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/conftest.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_export.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_export.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_plotting.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_mixins.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_imaging_mixins.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_import_time.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_import_time.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_mixin.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_scalebar.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_timeindex.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_utilities.py` & `lumicks.pylake-1.5.1/lumicks/pylake/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/lumicks.pylake.egg-info/PKG-INFO` & `lumicks.pylake-1.5.1/lumicks.pylake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.5.0
+Version: 1.5.1
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lumicks.pylake-1.5.0/lumicks.pylake.egg-info/SOURCES.txt` & `lumicks.pylake-1.5.1/lumicks.pylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/readme.md` & `lumicks.pylake-1.5.1/readme.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.5.0/setup.py` & `lumicks.pylake-1.5.1/setup.py`

 * *Files identical despite different names*

