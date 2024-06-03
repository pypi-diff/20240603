# Comparing `tmp/magpylib-5.0.2.tar.gz` & `tmp/magpylib-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magpylib-5.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "magpylib-5.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `magpylib-5.0.2.tar` & `magpylib-5.0.3.tar`

### file list

```diff
@@ -1,248 +1,257 @@
--rw-r--r--   0        0        0       20 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/apt.txt
--rw-r--r--   0        0        0      171 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/labconfig/default_setting_overrides.json
--rw-r--r--   0        0        0      207 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/postBuild
--rw-r--r--   0        0        0        8 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/requirements.txt
--rw-r--r--   0        0        0      187 2024-05-22 07:39:06.741836 magpylib-5.0.2/.binder/start
--rw-r--r--   0        0        0     1562 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      910 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0        0        0      573 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/ISSUE_TEMPLATE/question_magnetics.yaml
--rw-r--r--   0        0        0       27 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       59 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/codeql/codeql-config.yml
--rw-r--r--   0        0        0     1000 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     2113 2024-05-22 07:39:06.741836 magpylib-5.0.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1690 2024-05-22 07:39:06.741836 magpylib-5.0.2/.gitignore
--rw-r--r--   0        0        0     1116 2024-05-22 07:39:06.741836 magpylib-5.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    16348 2024-05-22 07:39:06.741836 magpylib-5.0.2/.pylintrc
--rw-r--r--   0        0        0      807 2024-05-22 07:39:06.741836 magpylib-5.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0    34350 2024-05-22 07:39:06.741836 magpylib-5.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     4790 2024-05-22 07:39:06.741836 magpylib-5.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3287 2024-05-22 07:39:06.741836 magpylib-5.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1332 2024-05-22 07:39:06.741836 magpylib-5.0.2/LICENSE
--rw-r--r--   0        0        0       68 2024-05-22 07:39:06.741836 magpylib-5.0.2/MANIFEST.in
--rw-r--r--   0        0        0     6948 2024-05-22 07:39:06.745836 magpylib-5.0.2/README.md
--rw-r--r--   0        0        0      602 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/Makefile
--rw-r--r--   0        0        0     1720 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/README.md
--rw-r--r--   0        0        0    40241 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_graphics.md
--rw-r--r--   0        0        0      733 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_index.md
--rw-r--r--   0        0        0    39553 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_magpylib_api.md
--rw-r--r--   0        0        0    10878 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/docu/docu_physics.md
--rw-r--r--   0        0        0     2687 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_end_of_shaft.md
--rw-r--r--   0        0        0      477 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_halbach.md
--rw-r--r--   0        0        0     4757 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_helmholtz.md
--rw-r--r--   0        0        0      426 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_app_scales.md
--rw-r--r--   0        0        0     5029 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_index.md
--rw-r--r--   0        0        0     5938 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_misc_compound.md
--rw-r--r--   0        0        0     5283 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_misc_field_interpolation.md
--rw-r--r--   0        0        0      372 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_misc_inhom.md
--rw-r--r--   0        0        0      367 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_3d_models.md
--rw-r--r--   0        0        0     1297 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_convex_hull.md
--rw-r--r--   0        0        0     3878 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_pyvista.md
--rw-r--r--   0        0        0     6628 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_superpos.md
--rw-r--r--   0        0        0     8369 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_triangle.md
--rw-r--r--   0        0        0     8058 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_collection.md
--rw-r--r--   0        0        0     7509 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_custom.md
--rw-r--r--   0        0        0     7845 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_field_computation.md
--rw-r--r--   0        0        0    10548 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md
--rw-r--r--   0        0        0     6804 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_paths.md
--rw-r--r--   0        0        0     1313 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_animations.md
--rw-r--r--   0        0        0     4091 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_mpl_streamplot.md
--rw-r--r--   0        0        0     1657 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_pv_streamlines.md
--rw-r--r--   0        0        0      545 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/gallery/gallery_vis_subplots.md
--rw-r--r--   0        0        0       89 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_changelog.md
--rw-r--r--   0        0        0      102 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_code_of_conduct.md
--rw-r--r--   0        0        0       95 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_contributing.md
--rw-r--r--   0        0        0     7719 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_get_started.md
--rw-r--r--   0        0        0      383 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_license.md
--rw-r--r--   0        0        0      357 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_pages/reso_site_notice.md
--rw-r--r--   0        0        0      252 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/custom.css
--rw-r--r--   0        0        0    21562 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_collection.png
--rw-r--r--   0        0        0    17761 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_cuboid.png
--rw-r--r--   0        0        0    20351 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_custom.png
--rw-r--r--   0        0        0    19925 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_cylinder.png
--rw-r--r--   0        0        0    26491 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_cylindersegment.png
--rw-r--r--   0        0        0    16339 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_dipole.png
--rw-r--r--   0        0        0    13734 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_global_local.png
--rw-r--r--   0        0        0    21266 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_line.png
--rw-r--r--   0        0        0    18823 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_loop.png
--rw-r--r--   0        0        0    20182 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_sensor.png
--rw-r--r--   0        0        0    19936 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_sphere.png
--rw-r--r--   0        0        0    23461 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_tetra.png
--rw-r--r--   0        0        0    21231 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_triangle.png
--rw-r--r--   0        0        0    27786 2024-05-22 07:39:06.745836 magpylib-5.0.2/docs/_static/images/docu_classes_init_trimesh.png
--rw-r--r--   0        0        0   249417 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_field_comp_flow.png
--rw-r--r--   0        0        0    18560 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_field_superpos_cutout.png
--rw-r--r--   0        0        0    18079 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_field_superpos_union.png
--rw-r--r--   0        0        0   236681 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_index_icon_magpylib.png
--rw-r--r--   0        0        0    91437 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_index_icon_magpylib_show.png
--rw-r--r--   0        0        0   319986 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_index_icon_physics.png
--rw-r--r--   0        0        0    49387 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/docu_position_sketch.png
--rw-r--r--   0        0        0    13848 2024-05-22 07:39:06.749836 magpylib-5.0.2/docs/_static/images/favicons/android-chrome-192x192.png
--rw-r--r--   0        0        0    59132 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/android-chrome-512x512.png
--rw-r--r--   0        0        0    12328 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/apple-touch-icon.png
--rw-r--r--   0        0        0      708 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/favicon-16x16.png
--rw-r--r--   0        0        0     1470 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/favicons/favicon.ico
--rw-r--r--   0        0        0    29951 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_WIP.png
--rw-r--r--   0        0        0    36788 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_app_end_of_shaft.png
--rw-r--r--   0        0        0   142838 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_app_helmholtz.png
--rw-r--r--   0        0        0   126489 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_ext_custom_quadrupole.png
--rw-r--r--   0        0        0    52664 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_misc_compound.png
--rw-r--r--   0        0        0    19393 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_misc_field_interpolation.png
--rw-r--r--   0        0        0    28378 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_convex_hull.png
--rw-r--r--   0        0        0    26107 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_pyvista.png
--rw-r--r--   0        0        0    16589 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_superpos.png
--rw-r--r--   0        0        0    31361 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_triangle.png
--rw-r--r--   0        0        0    49507 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_collection.png
--rw-r--r--   0        0        0   270663 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_custom.png
--rw-r--r--   0        0        0    37618 2024-05-22 07:39:06.753836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_field_computation.png
--rw-r--r--   0        0        0    58417 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png
--rw-r--r--   0        0        0    32221 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_paths.png
--rw-r--r--   0        0        0    29154 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_viz_animations.png
--rw-r--r--   0        0        0   133213 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_viz_mpl_streamplot.png
--rw-r--r--   0        0        0   101122 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_icon_viz_pv_streamlines.png
--rw-r--r--   0        0        0   125215 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_LDratio.png
--rw-r--r--   0        0        0   192104 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet.png
--rw-r--r--   0        0        0   115449 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet2.png
--rw-r--r--   0        0        0   105716 2024-05-22 07:39:06.757836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png
--rw-r--r--   0        0        0    82273 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_hysteresis.png
--rw-r--r--   0        0        0    60218 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_table.png
--rw-r--r--   0        0        0    42153 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_animation.png
--rw-r--r--   0        0        0   107905 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_complex_shapes.png
--rw-r--r--   0        0        0   101291 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_fundamentals1.png
--rw-r--r--   0        0        0   114836 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/getting_started_styles.png
--rw-r--r--   0        0        0   240757 2024-05-22 07:39:06.761836 magpylib-5.0.2/docs/_static/images/index_flowchart.png
--rw-r--r--   0        0        0   323052 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_head.png
--rw-r--r--   0        0        0     7837 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_academic.png
--rw-r--r--   0        0        0     5281 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_contributing.png
--rw-r--r--   0        0        0     8741 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_docu.png
--rw-r--r--   0        0        0    12683 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_gallery.png
--rw-r--r--   0        0        0     9752 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_getting_started.png
--rw-r--r--   0        0        0     7864 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/index_icon_github.png
--rw-r--r--   0        0        0   167515 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/magpylib_flag.png
--rw-r--r--   0        0        0    22705 2024-05-22 07:39:06.765836 magpylib-5.0.2/docs/_static/images/magpylib_logo.png
--rw-r--r--   0        0        0   526695 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/_static/videos/axis.mp4
--rw-r--r--   0        0        0     2970 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/_static/webcode/copybutton.js
--rw-r--r--   0        0        0      447 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/_static/webcode/summaryOpen.js
--rw-r--r--   0        0        0    10243 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/conf.py
--rw-r--r--   0        0        0     2316 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/index.md
--rw-r--r--   0        0        0     6715 2024-05-22 07:39:06.769836 magpylib-5.0.2/docs/make.bat
--rw-r--r--   0        0        0     1916 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/__init__.py
--rw-r--r--   0        0        0       11 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/__init__.py
--rw-r--r--   0        0        0       22 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/__init__.py
--rw-r--r--   0        0        0     9448 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/defaults_classes.py
--rw-r--r--   0        0        0    13989 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/defaults_utility.py
--rw-r--r--   0        0        0     5981 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/defaults/defaults_values.py
--rw-r--r--   0        0        0       22 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/__init__.py
--rw-r--r--   0        0        0    14530 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/backend_matplotlib.py
--rw-r--r--   0        0        0    10746 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/backend_plotly.py
--rw-r--r--   0        0        0    12228 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/backend_pyvista.py
--rw-r--r--   0        0        0    17456 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/display.py
--rw-r--r--   0        0        0    11170 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/sensor_mesh.py
--rw-r--r--   0        0        0    21819 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_base.py
--rw-r--r--   0        0        0    22531 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_core.py
--rw-r--r--   0        0        0    33281 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_generic.py
--rw-r--r--   0        0        0    26263 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/display/traces_utility.py
--rw-r--r--   0        0        0      458 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/exceptions.py
--rw-r--r--   0        0        0      312 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/__init__.py
--rw-r--r--   0        0        0     3696 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_circle.py
--rw-r--r--   0        0        0     8994 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_cuboid.py
--rw-r--r--   0        0        0    11016 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder.py
--rw-r--r--   0        0        0    77680 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder_segment.py
--rw-r--r--   0        0        0     2360 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_dipole.py
--rw-r--r--   0        0        0     7223 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_polyline.py
--rw-r--r--   0        0        0     2762 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_sphere.py
--rw-r--r--   0        0        0     3775 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_tetrahedron.py
--rw-r--r--   0        0        0     6453 2024-05-22 07:39:06.769836 magpylib-5.0.2/magpylib/_src/fields/field_BH_triangle.py
--rw-r--r--   0        0        0    19051 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/field_BH_triangularmesh.py
--rw-r--r--   0        0        0    48296 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/field_wrap_BH.py
--rw-r--r--   0        0        0     4396 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/special_cel.py
--rw-r--r--   0        0        0    17650 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/fields/special_el3.py
--rw-r--r--   0        0        0    20731 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/input_checks.py
--rw-r--r--   0        0        0       23 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/__init__.py
--rw-r--r--   0        0        0     4090 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
--rw-r--r--   0        0        0    19372 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseExcitations.py
--rw-r--r--   0        0        0    12717 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseGeo.py
--rw-r--r--   0        0        0    34491 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseTransform.py
--rw-r--r--   0        0        0    36370 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_Collection.py
--rw-r--r--   0        0        0    18854 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_Sensor.py
--rw-r--r--   0        0        0     4535 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Circle.py
--rw-r--r--   0        0        0     4946 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Polyline.py
--rw-r--r--   0        0        0     4421 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cuboid.py
--rw-r--r--   0        0        0     5006 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cylinder.py
--rw-r--r--   0        0        0     6828 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
--rw-r--r--   0        0        0     4681 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Sphere.py
--rw-r--r--   0        0        0     6030 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
--rw-r--r--   0        0        0    36933 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
--rw-r--r--   0        0        0     3520 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_CustomSource.py
--rw-r--r--   0        0        0     4530 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Dipole.py
--rw-r--r--   0        0        0     5934 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Triangle.py
--rw-r--r--   0        0        0    77585 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/style.py
--rw-r--r--   0        0        0    12334 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/_src/utility.py
--rw-r--r--   0        0        0     1048 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/core/__init__.py
--rw-r--r--   0        0        0      398 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/current/__init__.py
--rw-r--r--   0        0        0      260 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/graphics/__init__.py
--rw-r--r--   0        0        0      835 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/graphics/model3d/__init__.py
--rw-r--r--   0        0        0      353 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/graphics/style/__init__.py
--rw-r--r--   0        0        0      632 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/magnet/__init__.py
--rw-r--r--   0        0        0      335 2024-05-22 07:39:06.773836 magpylib-5.0.2/magpylib/misc/__init__.py
--rw-r--r--   0        0        0     2290 2024-05-22 07:39:06.773836 magpylib-5.0.2/pyproject.toml
--rw-r--r--   0        0        0       14 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/__init__.py
--rw-r--r--   0        0        0    25344 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_BHMJ_level.py
--rw-r--r--   0        0        0     7672 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_BaseTransform.py
--rw-r--r--   0        0        0     5503 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_Coumpound_setters.py
--rw-r--r--   0        0        0     2035 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_CustomSource.py
--rw-r--r--   0        0        0      760 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test__missing_optional_modules.py
--rw-r--r--   0        0        0      465 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_core.py
--rw-r--r--   0        0        0    18105 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_core_physics_consistency.py
--rw-r--r--   0        0        0     7060 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_default_utils.py
--rw-r--r--   0        0        0    10878 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_defaults.py
--rw-r--r--   0        0        0    21282 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_matplotlib.py
--rw-r--r--   0        0        0    13771 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_plotly.py
--rw-r--r--   0        0        0     4507 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_pyvista.py
--rw-r--r--   0        0        0     3181 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_display_utility.py
--rw-r--r--   0        0        0     3453 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_elliptics.py
--rw-r--r--   0        0        0     8864 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_exceptions.py
--rw-r--r--   0        0        0    15385 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_field_cylinder.py
--rw-r--r--   0        0        0    13402 2024-05-22 07:39:06.773836 magpylib-5.0.2/tests/test_getBH_dict.py
--rw-r--r--   0        0        0    12196 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_getBH_interfaces.py
--rw-r--r--   0        0        0    19639 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_getBH_level2.py
--rw-r--r--   0        0        0    25249 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_input_checks.py
--rw-r--r--   0        0        0      346 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_misc.py
--rw-r--r--   0        0        0      737 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_numerical_stability.py
--rw-r--r--   0        0        0    20619 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_BaseGeo.py
--rw-r--r--   0        0        0    12300 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_BaseGeo_v4motion.py
--rw-r--r--   0        0        0     2208 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Circle.py
--rw-r--r--   0        0        0    15913 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Collection.py
--rw-r--r--   0        0        0    10301 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Collection_child_parent.py
--rw-r--r--   0        0        0    25232 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Collection_v4motion.py
--rw-r--r--   0        0        0     4516 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Cuboid.py
--rw-r--r--   0        0        0     4140 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Cylinder.py
--rw-r--r--   0        0        0     1087 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_CylinderSegment.py
--rw-r--r--   0        0        0     1038 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Dipole.py
--rw-r--r--   0        0        0     3787 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Polyline.py
--rw-r--r--   0        0        0     3719 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Sensor.py
--rw-r--r--   0        0        0     3105 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Sphere.py
--rw-r--r--   0        0        0     2467 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Tetrahedron.py
--rw-r--r--   0        0        0     2446 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_Triangle.py
--rw-r--r--   0        0        0    16212 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_obj_TriangularMesh.py
--rw-r--r--   0        0        0     1654 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_path.py
--rw-r--r--   0        0        0    10338 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_physics_consistency.py
--rw-r--r--   0        0        0      661 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_scaling.py
--rw-r--r--   0        0        0     2633 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_utility.py
--rw-r--r--   0        0        0     2966 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/test_vs_mag2.py
--rw-r--r--   0        0        0    14641 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/testdata/testdata_Collection.p
--rw-r--r--   0        0        0     1568 2024-05-22 07:39:06.777836 magpylib-5.0.2/tests/testdata/testdata_Collection_setter.npy
--rw-r--r--   0        0        0  1747640 2024-05-22 07:39:06.785836 magpylib-5.0.2/tests/testdata/testdata_Cuboid.p
--rw-r--r--   0        0        0  1746038 2024-05-22 07:39:06.797836 magpylib-5.0.2/tests/testdata/testdata_Sphere.p
--rw-r--r--   0        0        0    17225 2024-05-22 07:39:06.797836 magpylib-5.0.2/tests/testdata/testdata_compound_setter_cases.npy
--rw-r--r--   0        0        0  1095577 2024-05-22 07:39:06.801836 magpylib-5.0.2/tests/testdata/testdata_cy_cases.npy
--rw-r--r--   0        0        0   320128 2024-05-22 07:39:06.801836 magpylib-5.0.2/tests/testdata/testdata_el3.npy
--rw-r--r--   0        0        0  1534592 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_el3_angle.npy
--rw-r--r--   0        0        0    13056 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_femDat_cylinder_tile2.npy
--rw-r--r--   0        0        0   102475 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_field_BH_cuboid.p
--rw-r--r--   0        0        0   240606 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_field_BH_cylinder.p
--rw-r--r--   0        0        0     9728 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_full_cyl.npy
--rw-r--r--   0        0        0     1022 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_path_BaseGeo.p
--rw-r--r--   0        0        0     7362 2024-05-22 07:39:06.809836 magpylib-5.0.2/tests/testdata/testdata_vs_mag2.p
--rw-r--r--   0        0        0      576 2024-05-22 07:39:06.809836 magpylib-5.0.2/tox.ini
--rw-r--r--   0        0        0     9358 1970-01-01 00:00:00.000000 magpylib-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-06-03 12:18:04.233143 magpylib-5.0.3/.binder/apt.txt
+-rw-r--r--   0        0        0      171 2024-06-03 12:18:04.233143 magpylib-5.0.3/.binder/labconfig/default_setting_overrides.json
+-rw-r--r--   0        0        0      207 2024-06-03 12:18:04.233143 magpylib-5.0.3/.binder/postBuild
+-rw-r--r--   0        0        0        8 2024-06-03 12:18:04.233143 magpylib-5.0.3/.binder/requirements.txt
+-rw-r--r--   0        0        0      187 2024-06-03 12:18:04.233143 magpylib-5.0.3/.binder/start
+-rw-r--r--   0        0        0     1562 2024-06-03 12:18:04.233143 magpylib-5.0.3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      910 2024-06-03 12:18:04.233143 magpylib-5.0.3/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0        0        0      573 2024-06-03 12:18:04.233143 magpylib-5.0.3/.github/ISSUE_TEMPLATE/question_magnetics.yaml
+-rw-r--r--   0        0        0       27 2024-06-03 12:18:04.237143 magpylib-5.0.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       59 2024-06-03 12:18:04.237143 magpylib-5.0.3/.github/codeql/codeql-config.yml
+-rw-r--r--   0        0        0     1000 2024-06-03 12:18:04.237143 magpylib-5.0.3/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     2113 2024-06-03 12:18:04.237143 magpylib-5.0.3/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1690 2024-06-03 12:18:04.237143 magpylib-5.0.3/.gitignore
+-rw-r--r--   0        0        0     1116 2024-06-03 12:18:04.237143 magpylib-5.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    16348 2024-06-03 12:18:04.237143 magpylib-5.0.3/.pylintrc
+-rw-r--r--   0        0        0      807 2024-06-03 12:18:04.237143 magpylib-5.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0    34769 2024-06-03 12:18:04.237143 magpylib-5.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     4785 2024-06-03 12:18:04.237143 magpylib-5.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3283 2024-06-03 12:18:04.237143 magpylib-5.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1332 2024-06-03 12:18:04.237143 magpylib-5.0.3/LICENSE
+-rw-r--r--   0        0        0       68 2024-06-03 12:18:04.237143 magpylib-5.0.3/MANIFEST.in
+-rw-r--r--   0        0        0     6948 2024-06-03 12:18:04.237143 magpylib-5.0.3/README.md
+-rw-r--r--   0        0        0      602 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/Makefile
+-rw-r--r--   0        0        0     1713 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/README.md
+-rw-r--r--   0        0        0      143 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/API_reference.md
+-rw-r--r--   0        0        0      222 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/changelog_.md
+-rw-r--r--   0        0        0      140 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/contributing/cont_code_of_conduct.md
+-rw-r--r--   0        0        0      137 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/contributing/cont_contributing.md
+-rw-r--r--   0        0        0      265 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/contributing/cont_index.md
+-rw-r--r--   0        0        0      400 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/contributing/cont_license.md
+-rw-r--r--   0        0        0    19393 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/docs/docs_classes.md
+-rw-r--r--   0        0        0     8150 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/docs/docs_fieldcomp.md
+-rw-r--r--   0        0        0    16308 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/docs/docs_graphics.md
+-rw-r--r--   0        0        0     9123 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/docs/docs_pos_ori.md
+-rw-r--r--   0        0        0    21276 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/docs/docs_styles.md
+-rw-r--r--   0        0        0     3073 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/docs/docs_units_types.md
+-rw-r--r--   0        0        0     4963 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_app_coils.md
+-rw-r--r--   0        0        0     2686 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_app_end_of_shaft.md
+-rw-r--r--   0        0        0     2475 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_app_halbach.md
+-rw-r--r--   0        0        0      468 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_app_scales.md
+-rw-r--r--   0        0        0     5971 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_index.md
+-rw-r--r--   0        0        0     6202 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_misc_compound.md
+-rw-r--r--   0        0        0     5347 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_misc_field_interpolation.md
+-rw-r--r--   0        0        0     5703 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_misc_inhom.md
+-rw-r--r--   0        0        0     1189 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_cad.md
+-rw-r--r--   0        0        0     1298 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_convex_hull.md
+-rw-r--r--   0        0        0     3818 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_pyvista.md
+-rw-r--r--   0        0        0     6533 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_superpos.md
+-rw-r--r--   0        0        0     8365 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_triangle.md
+-rw-r--r--   0        0        0     8413 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_collection.md
+-rw-r--r--   0        0        0     7588 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_custom.md
+-rw-r--r--   0        0        0     7662 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_field_computation.md
+-rw-r--r--   0        0        0    10556 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_modelling_magnets.md
+-rw-r--r--   0        0        0     6822 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_paths.md
+-rw-r--r--   0        0        0     2471 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_vis_animations.md
+-rw-r--r--   0        0        0     2619 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_vis_magnet_colors.md
+-rw-r--r--   0        0        0     3997 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_vis_mpl_streamplot.md
+-rw-r--r--   0        0        0     1644 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_vis_pv_streamlines.md
+-rw-r--r--   0        0        0     2859 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/examples_vis_subplots.md
+-rw-r--r--   0        0        0    57384 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/examples/logo.stl
+-rw-r--r--   0        0        0      564 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/guide_index.md
+-rw-r--r--   0        0        0    10408 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/guide_resources_01_physics.md
+-rw-r--r--   0        0        0      664 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/guide_start_01_install.md
+-rw-r--r--   0        0        0     8785 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_pages/user_guide/guide_start_02_fundamentals.md
+-rw-r--r--   0        0        0      673 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_static/custom.css
+-rw-r--r--   0        0        0    21562 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_static/images/docu_classes_init_collection.png
+-rw-r--r--   0        0        0    17761 2024-06-03 12:18:04.237143 magpylib-5.0.3/docs/_static/images/docu_classes_init_cuboid.png
+-rw-r--r--   0        0        0    20351 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_custom.png
+-rw-r--r--   0        0        0    19925 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_cylinder.png
+-rw-r--r--   0        0        0    26491 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_cylindersegment.png
+-rw-r--r--   0        0        0    16339 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_dipole.png
+-rw-r--r--   0        0        0    13734 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_global_local.png
+-rw-r--r--   0        0        0    21266 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_line.png
+-rw-r--r--   0        0        0    18823 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_loop.png
+-rw-r--r--   0        0        0    20182 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_sensor.png
+-rw-r--r--   0        0        0    19936 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_sphere.png
+-rw-r--r--   0        0        0    23461 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_tetra.png
+-rw-r--r--   0        0        0    21231 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_triangle.png
+-rw-r--r--   0        0        0    27786 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_classes_init_trimesh.png
+-rw-r--r--   0        0        0   249417 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_field_comp_flow.png
+-rw-r--r--   0        0        0    18560 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_field_superpos_cutout.png
+-rw-r--r--   0        0        0    18079 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_field_superpos_union.png
+-rw-r--r--   0        0        0    49387 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/docu_position_sketch.png
+-rw-r--r--   0        0        0    29951 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/examples_icon_WIP.png
+-rw-r--r--   0        0        0    36788 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/examples_icon_app_end_of_shaft.png
+-rw-r--r--   0        0        0    39803 2024-06-03 12:18:04.241143 magpylib-5.0.3/docs/_static/images/examples_icon_app_halbach.png
+-rw-r--r--   0        0        0   142838 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_app_helmholtz.png
+-rw-r--r--   0        0        0   126489 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_ext_custom_quadrupole.png
+-rw-r--r--   0        0        0    52664 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_misc_compound.png
+-rw-r--r--   0        0        0    19393 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_misc_field_interpolation.png
+-rw-r--r--   0        0        0    84343 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_misc_inhom.png
+-rw-r--r--   0        0        0    30947 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_shapes_cad.png
+-rw-r--r--   0        0        0    28378 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_shapes_convex_hull.png
+-rw-r--r--   0        0        0    26107 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_shapes_pyvista.png
+-rw-r--r--   0        0        0    16589 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_shapes_superpos.png
+-rw-r--r--   0        0        0    31361 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_shapes_triangle.png
+-rw-r--r--   0        0        0    49507 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_collection.png
+-rw-r--r--   0        0        0   270663 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_custom.png
+-rw-r--r--   0        0        0    37618 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_field_computation.png
+-rw-r--r--   0        0        0    58417 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_modelling_magnets.png
+-rw-r--r--   0        0        0    32221 2024-06-03 12:18:04.245143 magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_paths.png
+-rw-r--r--   0        0        0    29154 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_icon_vis_animations.png
+-rw-r--r--   0        0        0   117336 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_icon_vis_magnet_colors.png
+-rw-r--r--   0        0        0   133213 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_icon_vis_mpl_streamplot.png
+-rw-r--r--   0        0        0   101122 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_icon_vis_pv_streamlines.png
+-rw-r--r--   0        0        0    74749 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_icon_vis_subplots.png
+-rw-r--r--   0        0        0   125215 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_LDratio.png
+-rw-r--r--   0        0        0   192104 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_datasheet.png
+-rw-r--r--   0        0        0   115449 2024-06-03 12:18:04.249143 magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_datasheet2.png
+-rw-r--r--   0        0        0   105716 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_fieldcomparison.png
+-rw-r--r--   0        0        0    82273 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_hysteresis.png
+-rw-r--r--   0        0        0    60218 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_table.png
+-rw-r--r--   0        0        0    83040 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/examples_vis_magnet_colors.png
+-rw-r--r--   0        0        0    13848 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/favicons/android-chrome-192x192.png
+-rw-r--r--   0        0        0    59132 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/favicons/android-chrome-512x512.png
+-rw-r--r--   0        0        0    12328 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/favicons/apple-touch-icon.png
+-rw-r--r--   0        0        0      708 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/favicons/favicon-16x16.png
+-rw-r--r--   0        0        0     1470 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/favicons/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/favicons/favicon.ico
+-rw-r--r--   0        0        0    42153 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/getting_started_animation.png
+-rw-r--r--   0        0        0   107905 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/getting_started_complex_shapes.png
+-rw-r--r--   0        0        0   101291 2024-06-03 12:18:04.253143 magpylib-5.0.3/docs/_static/images/getting_started_fundamentals1.png
+-rw-r--r--   0        0        0   114836 2024-06-03 12:18:04.257143 magpylib-5.0.3/docs/_static/images/getting_started_styles.png
+-rw-r--r--   0        0        0   383287 2024-06-03 12:18:04.257143 magpylib-5.0.3/docs/_static/images/index_flowchart.png
+-rw-r--r--   0        0        0   323052 2024-06-03 12:18:04.257143 magpylib-5.0.3/docs/_static/images/index_head.png
+-rw-r--r--   0        0        0     8322 2024-06-03 12:18:04.257143 magpylib-5.0.3/docs/_static/images/index_icon_academic.png
+-rw-r--r--   0        0        0    13359 2024-06-03 12:18:04.257143 magpylib-5.0.3/docs/_static/images/index_icon_examples.png
+-rw-r--r--   0        0        0    10392 2024-06-03 12:18:04.257143 magpylib-5.0.3/docs/_static/images/index_icon_get_started.png
+-rw-r--r--   0        0        0   167515 2024-06-03 12:18:04.257143 magpylib-5.0.3/docs/_static/images/magpylib_flag.png
+-rw-r--r--   0        0        0    22705 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/_static/images/magpylib_logo.png
+-rw-r--r--   0        0        0      572 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/_static/switcher.json
+-rw-r--r--   0        0        0   526695 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/_static/videos/axis.mp4
+-rw-r--r--   0        0        0     2970 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/_static/webcode/copybutton.js
+-rw-r--r--   0        0        0      447 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/_static/webcode/summaryOpen.js
+-rw-r--r--   0        0        0    11382 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/conf.py
+-rw-r--r--   0        0        0     1721 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/index.md
+-rw-r--r--   0        0        0     6715 2024-06-03 12:18:04.261143 magpylib-5.0.3/docs/make.bat
+-rw-r--r--   0        0        0     1916 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/__init__.py
+-rw-r--r--   0        0        0       11 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/_src/__init__.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/_src/defaults/__init__.py
+-rw-r--r--   0        0        0     9448 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/_src/defaults/defaults_classes.py
+-rw-r--r--   0        0        0    13989 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/_src/defaults/defaults_utility.py
+-rw-r--r--   0        0        0     5981 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/_src/defaults/defaults_values.py
+-rw-r--r--   0        0        0       22 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/_src/display/__init__.py
+-rw-r--r--   0        0        0    14530 2024-06-03 12:18:04.261143 magpylib-5.0.3/magpylib/_src/display/backend_matplotlib.py
+-rw-r--r--   0        0        0    10746 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/backend_plotly.py
+-rw-r--r--   0        0        0    12228 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/backend_pyvista.py
+-rw-r--r--   0        0        0    17456 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/display.py
+-rw-r--r--   0        0        0    11170 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/sensor_mesh.py
+-rw-r--r--   0        0        0    21819 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/traces_base.py
+-rw-r--r--   0        0        0    22531 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/traces_core.py
+-rw-r--r--   0        0        0    33534 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/traces_generic.py
+-rw-r--r--   0        0        0    26263 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/display/traces_utility.py
+-rw-r--r--   0        0        0      458 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/exceptions.py
+-rw-r--r--   0        0        0      312 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/__init__.py
+-rw-r--r--   0        0        0     3696 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_circle.py
+-rw-r--r--   0        0        0     8994 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_cuboid.py
+-rw-r--r--   0        0        0    11016 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_cylinder.py
+-rw-r--r--   0        0        0    77680 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_cylinder_segment.py
+-rw-r--r--   0        0        0     2360 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_dipole.py
+-rw-r--r--   0        0        0     7223 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_polyline.py
+-rw-r--r--   0        0        0     2762 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_sphere.py
+-rw-r--r--   0        0        0     3775 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_tetrahedron.py
+-rw-r--r--   0        0        0     6453 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_triangle.py
+-rw-r--r--   0        0        0    19051 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_BH_triangularmesh.py
+-rw-r--r--   0        0        0    48296 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/field_wrap_BH.py
+-rw-r--r--   0        0        0     4396 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/special_cel.py
+-rw-r--r--   0        0        0    17650 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/fields/special_el3.py
+-rw-r--r--   0        0        0    20731 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/input_checks.py
+-rw-r--r--   0        0        0       23 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/__init__.py
+-rw-r--r--   0        0        0     4090 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseDisplayRepr.py
+-rw-r--r--   0        0        0    19372 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseExcitations.py
+-rw-r--r--   0        0        0    12717 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseGeo.py
+-rw-r--r--   0        0        0    34491 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseTransform.py
+-rw-r--r--   0        0        0    36370 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_Collection.py
+-rw-r--r--   0        0        0    18854 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_Sensor.py
+-rw-r--r--   0        0        0     4535 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_current_Circle.py
+-rw-r--r--   0        0        0     4946 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_current_Polyline.py
+-rw-r--r--   0        0        0     4421 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Cuboid.py
+-rw-r--r--   0        0        0     5006 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Cylinder.py
+-rw-r--r--   0        0        0     6828 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py
+-rw-r--r--   0        0        0     4681 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Sphere.py
+-rw-r--r--   0        0        0     6030 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py
+-rw-r--r--   0        0        0    36933 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py
+-rw-r--r--   0        0        0     3520 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_misc_CustomSource.py
+-rw-r--r--   0        0        0     4530 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_misc_Dipole.py
+-rw-r--r--   0        0        0     5934 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/obj_classes/class_misc_Triangle.py
+-rw-r--r--   0        0        0    77585 2024-06-03 12:18:04.265143 magpylib-5.0.3/magpylib/_src/style.py
+-rw-r--r--   0        0        0    12334 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/_src/utility.py
+-rw-r--r--   0        0        0     1048 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/core/__init__.py
+-rw-r--r--   0        0        0      398 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/current/__init__.py
+-rw-r--r--   0        0        0      260 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/graphics/__init__.py
+-rw-r--r--   0        0        0      835 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/graphics/model3d/__init__.py
+-rw-r--r--   0        0        0      353 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/graphics/style/__init__.py
+-rw-r--r--   0        0        0      632 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/magnet/__init__.py
+-rw-r--r--   0        0        0      335 2024-06-03 12:18:04.269143 magpylib-5.0.3/magpylib/misc/__init__.py
+-rw-r--r--   0        0        0     2326 2024-06-03 12:18:04.269143 magpylib-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0       14 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    25344 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_BHMJ_level.py
+-rw-r--r--   0        0        0     7672 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_BaseTransform.py
+-rw-r--r--   0        0        0     5503 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_Coumpound_setters.py
+-rw-r--r--   0        0        0     2035 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_CustomSource.py
+-rw-r--r--   0        0        0      760 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test__missing_optional_modules.py
+-rw-r--r--   0        0        0      465 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_core.py
+-rw-r--r--   0        0        0    18105 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_core_physics_consistency.py
+-rw-r--r--   0        0        0     7060 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_default_utils.py
+-rw-r--r--   0        0        0    10878 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_defaults.py
+-rw-r--r--   0        0        0    21282 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_display_matplotlib.py
+-rw-r--r--   0        0        0    13771 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_display_plotly.py
+-rw-r--r--   0        0        0     4507 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_display_pyvista.py
+-rw-r--r--   0        0        0     3181 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_display_utility.py
+-rw-r--r--   0        0        0     3453 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_elliptics.py
+-rw-r--r--   0        0        0     8864 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_exceptions.py
+-rw-r--r--   0        0        0    15385 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_field_cylinder.py
+-rw-r--r--   0        0        0    13402 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_getBH_dict.py
+-rw-r--r--   0        0        0    12196 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_getBH_interfaces.py
+-rw-r--r--   0        0        0    19639 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_getBH_level2.py
+-rw-r--r--   0        0        0    25249 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_input_checks.py
+-rw-r--r--   0        0        0      346 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_misc.py
+-rw-r--r--   0        0        0      737 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_numerical_stability.py
+-rw-r--r--   0        0        0    20619 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_BaseGeo.py
+-rw-r--r--   0        0        0    12300 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_BaseGeo_v4motion.py
+-rw-r--r--   0        0        0     2208 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Circle.py
+-rw-r--r--   0        0        0    15913 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Collection.py
+-rw-r--r--   0        0        0    10301 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Collection_child_parent.py
+-rw-r--r--   0        0        0    25232 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Collection_v4motion.py
+-rw-r--r--   0        0        0     4516 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Cuboid.py
+-rw-r--r--   0        0        0     4140 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Cylinder.py
+-rw-r--r--   0        0        0     1087 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_CylinderSegment.py
+-rw-r--r--   0        0        0     1038 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Dipole.py
+-rw-r--r--   0        0        0     3787 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Polyline.py
+-rw-r--r--   0        0        0     3719 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Sensor.py
+-rw-r--r--   0        0        0     3105 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Sphere.py
+-rw-r--r--   0        0        0     2467 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Tetrahedron.py
+-rw-r--r--   0        0        0     2446 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_Triangle.py
+-rw-r--r--   0        0        0    16212 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_obj_TriangularMesh.py
+-rw-r--r--   0        0        0     1654 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_path.py
+-rw-r--r--   0        0        0    10338 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_physics_consistency.py
+-rw-r--r--   0        0        0      661 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_scaling.py
+-rw-r--r--   0        0        0     2633 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_utility.py
+-rw-r--r--   0        0        0     2966 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/test_vs_mag2.py
+-rw-r--r--   0        0        0    14641 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/testdata/testdata_Collection.p
+-rw-r--r--   0        0        0     1568 2024-06-03 12:18:04.269143 magpylib-5.0.3/tests/testdata/testdata_Collection_setter.npy
+-rw-r--r--   0        0        0  1747640 2024-06-03 12:18:04.281143 magpylib-5.0.3/tests/testdata/testdata_Cuboid.p
+-rw-r--r--   0        0        0  1746038 2024-06-03 12:18:04.289143 magpylib-5.0.3/tests/testdata/testdata_Sphere.p
+-rw-r--r--   0        0        0    17225 2024-06-03 12:18:04.289143 magpylib-5.0.3/tests/testdata/testdata_compound_setter_cases.npy
+-rw-r--r--   0        0        0  1095577 2024-06-03 12:18:04.297143 magpylib-5.0.3/tests/testdata/testdata_cy_cases.npy
+-rw-r--r--   0        0        0   320128 2024-06-03 12:18:04.297143 magpylib-5.0.3/tests/testdata/testdata_el3.npy
+-rw-r--r--   0        0        0  1534592 2024-06-03 12:18:04.301143 magpylib-5.0.3/tests/testdata/testdata_el3_angle.npy
+-rw-r--r--   0        0        0    13056 2024-06-03 12:18:04.301143 magpylib-5.0.3/tests/testdata/testdata_femDat_cylinder_tile2.npy
+-rw-r--r--   0        0        0   102475 2024-06-03 12:18:04.301143 magpylib-5.0.3/tests/testdata/testdata_field_BH_cuboid.p
+-rw-r--r--   0        0        0   240606 2024-06-03 12:18:04.301143 magpylib-5.0.3/tests/testdata/testdata_field_BH_cylinder.p
+-rw-r--r--   0        0        0     9728 2024-06-03 12:18:04.301143 magpylib-5.0.3/tests/testdata/testdata_full_cyl.npy
+-rw-r--r--   0        0        0     1022 2024-06-03 12:18:04.301143 magpylib-5.0.3/tests/testdata/testdata_path_BaseGeo.p
+-rw-r--r--   0        0        0     7362 2024-06-03 12:18:04.301143 magpylib-5.0.3/tests/testdata/testdata_vs_mag2.p
+-rw-r--r--   0        0        0      576 2024-06-03 12:18:04.305143 magpylib-5.0.3/tox.ini
+-rw-r--r--   0        0        0     9420 1970-01-01 00:00:00.000000 magpylib-5.0.3/PKG-INFO
```

### Comparing `magpylib-5.0.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `magpylib-5.0.3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/.github/ISSUE_TEMPLATE/feature_request.yaml` & `magpylib-5.0.3/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/.github/ISSUE_TEMPLATE/question_magnetics.yaml` & `magpylib-5.0.3/.github/ISSUE_TEMPLATE/question_magnetics.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/.github/workflows/codeql.yml` & `magpylib-5.0.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/.github/workflows/python-app.yml` & `magpylib-5.0.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/.gitignore` & `magpylib-5.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/.pre-commit-config.yaml` & `magpylib-5.0.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
 
 
   - repo: https://github.com/psf/black
-    rev: "24.4.0"
+    rev: "24.4.2"
     hooks:
       - id: black
 
 
   # - repo: local
   #   hooks:
   #     - id: pylint
```

### Comparing `magpylib-5.0.2/.pylintrc` & `magpylib-5.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/.readthedocs.yaml` & `magpylib-5.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/CHANGELOG.md` & `magpylib-5.0.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-All notable changes to magpylib are documented here.
+# Changelog
 
+## [5.0.3] - 2024-06-03
 
-# Changelog
+- Fix subplot object properties propagation ([#780](https://github.com/magpylib/magpylib/pull/780))
+- Migrate to pydata-sphinx-theme and fix docs search function ([#762](https://github.com/magpylib/magpylib/pull/762))
+- Fix docs version-switcher ([#782](https://github.com/magpylib/magpylib/pull/782))
 
 ## [5.0.2] - 2024-05-21
-- Fixed a display issue causing incorrect calculation of viewbox limits ([#772](https://github.com/magpylib/magpylib/pull/772))
+- Fixed a display issue causing incorrect calculation of view box limits ([#772](https://github.com/magpylib/magpylib/pull/772))
 - Removed support for python 3.8 and 3.9 by now following the scientific-python.org support timelines ([#773](https://github.com/magpylib/magpylib/pull/773))
 - Fixed CI testing with newer backend versions ([#774](https://github.com/magpylib/magpylib/pull/774))
 - Updated site notice to mention the awarded "small development grant" by NumFocus. ([#758](https://github.com/magpylib/magpylib/pull/758))
 - Fix inaccurate citation year for Yang publication ([#764](https://github.com/magpylib/magpylib/pull/764), with thanks to @feldnerd for the contribution!)
 
 ## [5.0.1] - 2024-04-12
 - Fixed a bug where `getBHJM` of a Collection would produce one extra dimension ([#753](https://github.com/magpylib/magpylib/issues/753))
@@ -52,23 +55,23 @@
 - `legend` style option ([#650](https://github.com/magpylib/magpylib/issues/650))
 - Changed unit naming in text to comply with DIN Norm 641 ([#614](https://github.com/magpylib/magpylib/issues/614))
 - Improved documentation now boasting a contribution guide, a news-blog, an example and tutorial gallery, a getting started section and many other improvements ([#621](https://github.com/magpylib/magpylib/issues/621), [#596](https://github.com/magpylib/magpylib/issues/596), [#580](https://github.com/magpylib/magpylib/issues/580))
 - Improved numerical stability of `CylinderSegment`, ([#648](https://github.com/magpylib/magpylib/issues/648), [#651](https://github.com/magpylib/magpylib/issues/651))
 
 
 ## [4.3.0] - 2023-06-25
-- New `TriangularMesh` magnet class added to conveniently work with triangular surface meshes instead of large collections of individual `Triangle` objects. The `TriangularMesh` class performs important checks (closed, connected, oriented) and can directly import pyvista objects and for convex hull bodies. ([#569](https://github.com/magpylib/magpylib/issues/569), [#598](https://github.com/magpylib/magpylib/pull/598)).
+- New `TriangularMesh` magnet class added to conveniently work with triangular surface meshes instead of large collections of individual `Triangle` objects. The `TriangularMesh` class performs important checks (closed, connected, oriented) and can directly import Pyvista objects and for convex hull bodies. ([#569](https://github.com/magpylib/magpylib/issues/569), [#598](https://github.com/magpylib/magpylib/pull/598)).
 - Added magnetization coloring for `matplotlib` backend ([#597](https://github.com/magpylib/magpylib/pull/597))
 - New automatic backend behavior, set to a dynamic default `auto` depending on the current environment and the given `canvas`, if provided. ([#617](https://github.com/magpylib/magpylib/pull/617))
 - Drop python 3.7 support, following python life cycle. ([#616](https://github.com/magpylib/magpylib/pull/616))
 
 ## [4.2.0] - 2023-01-27
 - (Re)introducing the powerful `misc.Triangle` class that can be used to compute magnetic fields of arbitrarily shaped bodies by approximating their surface with triangular faces. ([#568](https://github.com/magpylib/magpylib/issues/568))
 - Introducing the `magnet.Tetrahedron` class as a derivate of the Triangle class. ([#289](https://github.com/magpylib/magpylib/issues/289))
-- Change pyvista plotting defaults when using `show(backend='pyvista')` to fit better with other libraries. ([#551](https://github.com/magpylib/magpylib/issues/551))
+- Change Pyvista plotting defaults when using `show(backend='pyvista')` to fit better with other libraries. ([#551](https://github.com/magpylib/magpylib/issues/551))
 - Added code of conduct attempting to align with NumFocus standards ([#558](https://github.com/magpylib/magpylib/issues/558))
 - Improved Loop field computation in terms of performance and numerical stability ([#374](https://github.com/magpylib/magpylib/issues/374))
 - Add `magnetization.mode` style to allow showing magnetization direction for any backend ([#576](https://github.com/magpylib/magpylib/pull/576))
 - Documentation changes:
     - Correct conda install command
     - Integration of Triangle and Tetrahedron
     - Changed example gallery substructure
@@ -96,20 +99,20 @@
 
 ## [4.0.3] - 2022-05-13
 
 - Fix copy order Bug ([#530](https://github.com/magpylib/magpylib/issues/530))
 
 ## [4.0.2] - 2022-05-04
 
-- Fix magnetization coloring with mesh grouping (plotly) ([#526](https://github.com/magpylib/magpylib/pull/526))
+- Fix magnetization coloring with mesh grouping (Plotly) ([#526](https://github.com/magpylib/magpylib/pull/526))
 - Allow float color quadruples ([#529](https://github.com/magpylib/magpylib/pull/529))
 
 ## [4.0.1] - 2022-04-29
 
-- Graphic performance update for plotly when showing a large number of objects. ([#524](https://github.com/magpylib/magpylib/pull/524))
+- Graphic performance update for Plotly when showing a large number of objects. ([#524](https://github.com/magpylib/magpylib/pull/524))
 
 ## [4.0.0] - 2022-04-14
 
 This is a major update that includes
 
 - API changes
 - New features
@@ -127,23 +130,23 @@
 ### Field computation changes/fixes:
 - New computation core. Added top level subpackage `magpylib.core` where all field implementations can be accessed directly without the position/orientation interface. ([#376](https://github.com/magpylib/magpylib/issues/376))
 - Direct interface functions `getBdict` and `getHdict` (previously `getBv` and `getHv`) are now integrated into `getB` and `getH`. See docs for details ([#449](https://github.com/magpylib/magpylib/pull/449))
 - Generally improved field expressions: ([#374](https://github.com/magpylib/magpylib/issues/374))
   - Negative dimension input taken as absolute when only positive dimensions are allowed.
   - Scale invariant field evaluations.
   - Special cases caught within 1e-15 rtol and atol to account for numerical imprecision with positioning (e.g. object rotation).
-  - Suppress numpy divide/invalid warnings. return `np.nan` as `(0,0,0)` (e.g. on magnet edges or on line currents) and allow return of `np.inf`.
+  - Suppress Numpy divide/invalid warnings. return `np.nan` as `(0,0,0)` (e.g. on magnet edges or on line currents) and allow return of `np.inf`.
   - New closed form implementation for `Cylinder` with diametral magnetization is much faster (100-1000x) and numerically stable for small `r`. ([#404](https://github.com/magpylib/magpylib/issues/404), [#370](https://github.com/magpylib/magpylib/issues/370))
   - Improved numerical stability of current loop field. Now 12-14 correct digits everywhere. ([#374](https://github.com/magpylib/magpylib/issues/374))
   - Fixed `Collection` of `Lines` field computation error. ([#368](https://github.com/magpylib/magpylib/issues/368))
 - Object oriented interface fixes and modifications:
   - Improved performance of `getB` and `getH`.
-  - Fixed array dimension wrongly reduced when `sumup=True` and `squeeze=False` ind `getB` and `getH` functions ([#425](https://github.com/magpylib/magpylib/issues/425), [#426](https://github.com/magpylib/magpylib/pull/426))
+  - Fixed array dimension wrongly reduced when `sumup=True` and `squeeze=False` in `getB` and `getH` functions ([#425](https://github.com/magpylib/magpylib/issues/425), [#426](https://github.com/magpylib/magpylib/pull/426))
   - Minimal non-squeeze output shape is (1,1,1,1,3), meaning that a single pixel is now also represented. ([#493](https://github.com/magpylib/magpylib/pull/493))
-- With the new kwarg `pixel_agg` it is now possible to apply a numpy function with reducing functionality (like `mean`, `min`, `average`) to the pixel output. In this case, it is allowed to provide `getB` and `getH` with different observer input shapes. ([#503](https://github.com/magpylib/magpylib/pull/503))
+- With the new kwarg `pixel_agg` it is now possible to apply a Numpy function with reducing functionality (like `mean`, `min`, `average`) to the pixel output. In this case, it is allowed to provide `getB` and `getH` with different observer input shapes. ([#503](https://github.com/magpylib/magpylib/pull/503))
 
 ### Major graphic output overhaul:
 - Styles:
   - All object now have the `style` attribute for graphical output customization. Arguments can be passed as dictionaries, class attributes or with underscore magic.
   - Style defaults stored in `magpylib.defaults.display`. ([#291](https://github.com/magpylib/magpylib/issues/291), [#396](https://github.com/magpylib/magpylib/pull/396))
   - Possibility to add a custom 3D-model to any object. ([#416](https://github.com/magpylib/magpylib/pull/416))
 - `display` now called `show`, to be more in-line with standard graphic backends. Functionality completely overhauled to function with styles. ([#453](https://github.com/magpylib/magpylib/pull/453), [#451](https://github.com/magpylib/magpylib/issues/451))
@@ -164,18 +167,18 @@
   - UI fix empty display ([#401](https://github.com/magpylib/magpylib/issues/401))
   - Error msg when `show` is called without argument ([#448](https://github.com/magpylib/magpylib/issues/448))
 
 ### New documentation:
 - Completely new structure and layout. ([#399](https://github.com/magpylib/magpylib/issues/399), [#294](https://github.com/magpylib/magpylib/issues/294))
 - Binder links and live code. ([#389](https://github.com/magpylib/magpylib/issues/389))
 - Example galleries with practical user examples
-- Guidelines for advanced subclassing of `Collection` to form complex dynamic compound objects that seamlessly integrate into the MAgpylib interface.
+- Guidelines for advanced subclassing of `Collection` to form complex dynamic compound objects that seamlessly integrate into the Magpylib interface.
 
 ### Geometry interface modification
-- Added all scipy Rotation forms as rotation object methods. ([#427](https://github.com/magpylib/magpylib/pull/427))
+- Added all Scipy Rotation forms as rotation object methods. ([#427](https://github.com/magpylib/magpylib/pull/427))
 - `move` and `rotate` inputs differentiate between scalar and vector input. Scalar input is applied to the whole path vector input is merged. ([#438](https://github.com/magpylib/magpylib/discussions/438), [#444](https://github.com/magpylib/magpylib/issues/444), [#442](https://github.com/magpylib/magpylib/issues/443))
 - `move` and `rotate` methods have default `start='auto'` (scalar input: `start=0`-> applied to whole path, vector input: `start=len_path`-> append) instead of `start=-1`.
 - `move` and `rotate` methods maintain collection geometry when applied to a collection.
 - Improved `position` and `orientation` setter methods in line with `move` and `rotate` functionality and maintain `Collection` geometry.
 - Removed `increment` argument from `move` and `rotate` functions ([#438](https://github.com/magpylib/magpylib/discussions/438), [#444](https://github.com/magpylib/magpylib/issues/444))
 
 ### Modifications to the `Collection` class
@@ -235,16 +238,16 @@
 - Improved internal workings
 ### Added
 
 - New `orientation` property:
   - The `orientation` attribute stores the relative rotation of an object with respect to the reference orientation (defined in each class docstring).
   - The default (`orientation=None`) corresponds to a unit rotation.
   - `orientation` is stored as a `scipy.spatial.transform.Rotation` object.
-  - Calling the attribute `source.orientation` returns a scipy Rotation object `R`.
-  - Make use of all advantages of this great scipy package:
+  - Calling the attribute `source.orientation` returns a Scipy Rotation object `R`.
+  - Make use of all advantages of this great Scipy package:
     - define `R.from_rotvec()` or `R.from_quat()` or ...
     - view with `R.as_rotvec()` or `R.as_quat()` or ...
     - combine subsequent rotations `R1 * R2 * R3`
 - Sensor pixel:
   - The new `Sensor(position, pixel, orientation)` class has the argument `pixel` which is `(0,0,0)` by default and refers to pixel positions inside the Sensor (in the Sensor local CS). `pixel` is an arbitrary array_like of the shape (N1, N2, ..., 3).
 - Geometry paths:
   - The `position` and `orientation` attributes can now store paths in the global CS. For a path of length M the attribute `position` is an array of the shape (M,3) and `orientation` is a Rotation object with length M. Each path position is associated with a respective rotation.
@@ -293,41 +296,41 @@
     - The argument `sources` refers to a source/Collection or to a 1D list of L sources and/or Collections.
     - The argument `observers` refers to a set of positions of shape (N1, N2, ..., 3) or a Sensor with `pixel` shape (N1, N2, ..., 3) or a 1D list of K Sensors.
   - With Magpylib3 there are several ways to compute the field:
     1. `source.getB(*observers)`
     2. `sensor.getB(*sources)`
     3. `magpylib.getB(sources, observers)`
       - The output shape is always (L, M, K, N1, N2, ..., 3) with L sources, M path positions, K sensors and N (pixel) positions.
-      - Objects with shorter paths will be considered as static once their path ends while other paths still continue.
+      - Objects with shorter paths will be considered as static once their path ends while other paths continue.
     4. `magpylib.getBv(**kwargs)` gives direct access to the field formulas and mostly replaces the `getBv_XXX()` functionality of v2. All inputs must be arrays of length N or of length 1 (statics will be tiled).
   - While `getBv` is the fastest way to compute the fields it is much more convenient to use `getB()` which mostly provides the same performance. Specifically,the new `getB()` automatically groups all inputs for combined vectorized evaluation. This leads to a massive speedup when dealing with large Collections of similar sources.
   - In addition to `getB`, the new `getH` returns the field in kA/m.
 
 ### Removed
 - the kwarg `niter=50` does not exist anymore for the Cylinder field computation. The functionality was completely replaced by the config setting `Config.ITER_CYLINDER=50`.
 
 ---
 ## [2.3.0b] - 2020-01-17
 
 ### Changed
-- Improved performance of getB for diametral magnetized Cylinders by 20%.
-- GetB of Line current now uses vectorized code which leads to massive performance enhancement.
+- Improved performance of `getB` for diametral magnetized Cylinders by 20%.
+- `getB` of Line current now uses vectorized code which leads to massive performance enhancement.
 - **IMPORTANT:** position arguments of `getBv` functions have been flipped! First comes the source position POSm THEN the observer position POSo!
 
 
 ### Added
 - completed the library vector functionality adding magnet Cylinder, moment Dipole, current Loop and Line. This includes adding several private vectorized functions (e.g. ellipticV) to mathLib_vector, adding respective tests and docs examples.
 
 ---
 
 ## [2.1.0b] - 2019-12-06
 
 ### Added
 - Docstrings for vector functions.
-- displaySystem kwarg `figsize`
+- `displaySystem` kwarg `figsize`
 - bringing documentation up to speed
 
 ### Fixed
 - init file bug
 
 ---
 
@@ -354,26 +357,26 @@
 - Performance computation trough vector functionality included in new top-level subpackage "vector"
 - Vectorized versions of math functions added to "math" subpackage
 
 ---
 
 ## [1.2.1b0] - 2019-07-31
 ### Changed
-- Optimized getB call (utility integrated)
+- Optimized `getB` call (utility integrated)
 - Improved Documentation (added Sensor class v1)
 
 ---
 
 ## [1.2.0b0] - 2019-07-16
 ### Added
 - Sensor Class
-  - This allows users to create a coordinate system-enabled Sensor object, which can be placed, rotated, moved and oriented.
+  - This allows users to create a coordinate system-enabled Sensor object, which can be placed, rotated, moved, and oriented.
   - This object can take the B-Field of a system (be it single source or a Collection) with the added functionality of having its own reference in the coordinate space, allowing users to easily acquire relative B-Field measurements of a system from an arbitrarily placed sensor object.
   - Sensors in a list may be displayed in the `Collection.displaySystem()` by using the `sensors` keyword argument.
-- Added content to the `__repr__` builtin to all source classes for quick console evaluations, simply call a defined object in your Python shell to print out its attributes.
+- Added content to the `__repr__` built-in to all source classes for quick console evaluations, simply call a defined object in your Python shell to print out its attributes.
 ### Changed
 - Edge cases in field calculations now return a proper [RuntimeWarning](https://docs.python.org/3/library/exceptions.html#RuntimeWarning) instead of console prints
 ### Fixed
 - Unused imports and variables
 
 ---
 
@@ -394,80 +397,82 @@
 ## [1.1.0b0] - 2019-06-14
 ### Added
 - Implemented one new kwarg for `Collection.displaySystem()`:
 
     > `subplotAx=None`
         Draw into a subplot axe that already exists. The subplot needs to be 3D projected
 
-  This allows for creating side-by-side plots using displaySystem.
-  Figure information must be set manually in pyplot.figure() in order to not squash the plots upon subplotting.
+  This allows for creating side-by-side plots using `displaySystem`.
+  Figure information must be set manually in pyplot.figure() in order to not squash the plots upon sub plotting.
 
 
     <details>
     <summary> Click here for Example </summary>
 
     Code: https://gist.github.com/lucasgcb/77d55f2fda688e2fb8e1e4a68bb830b8
 
     **Output:**
     ![image](https://user-images.githubusercontent.com/7332704/58973138-86b4a600-87bf-11e9-9e63-35892b7a6713.png)
 
     </details>
 
 ### Changed
 
-- `getBsweep()` for Collections and Sources now always returns a numpy array
+- `getBsweep()` for Collections and Sources now always returns a Numpy array
 - Zero-length segments in Line sources now return `[0,0,0]` and a warning, making it easier to draw spirals without letting users do this unaware.
 
 ### Fixed
 - Added a workaround fix for a rotation bug we are still working on.
 
 ---
 
 ## [1.0.2b0] - 2019-05-29
 
 ### Added
 
-- `MANIFEST.in` file containing the LICENSE for bundling in PyPi
+- `MANIFEST.in` file containing the LICENSE for bundling in PyPI
 
 ---
 
 ## [1.0.1b0] - 2019-05-28
 
 ### Added
 
 - Issue and Pull Request Templates to Repository
 - Continuous Integration settings (Azure and Appveyor)
-- Code Coverage Reports with codecov
+- Code Coverage Reports with Codecov
 
 
 
 ### Removed
 
 - Support for Python 3.5 and under.
 
 ---
 
 ## [1.0.0b0] - 2019-05-21
 
-The first official release of the magpylib library.
+The first official release of the Magpylib library.
 
 ### Added
 
 - Source classes:
    - Box
    - Cylinder
    - Sphere
    - Loop Current
    - Current Line
    - Dipole
 - Collection class
 
 ---
 
-[5.0.2]:https://github.com/magpylib/magpylib/compare/5.0.1...HEAD
+[Unreleased]:https://github.com/magpylib/magpylib/compare/5.0.3...HEAD
+[5.0.3]:https://github.com/magpylib/magpylib/compare/5.0.2...5.0.3
+[5.0.2]:https://github.com/magpylib/magpylib/compare/5.0.1...5.0.2
 [5.0.1]:https://github.com/magpylib/magpylib/compare/5.0.0...5.0.1
 [5.0.0]:https://github.com/magpylib/magpylib/compare/4.5.1...5.0.0
 [4.5.1]:https://github.com/magpylib/magpylib/compare/4.5.0...4.5.1
 [4.5.0]:https://github.com/magpylib/magpylib/compare/4.4.0...4.5.0
 [4.4.1]:https://github.com/magpylib/magpylib/compare/4.4.0...4.4.1
 [4.4.0]:https://github.com/magpylib/magpylib/compare/4.3.0...4.4.0
 [4.3.0]:https://github.com/magpylib/magpylib/compare/4.2.0...4.3.0
```

### Comparing `magpylib-5.0.2/CODE_OF_CONDUCT.md` & `magpylib-5.0.3/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Community leaders are responsible for clarifying and enforcing our standards of acceptable behavior and will take appropriate and fair corrective action in response to any behavior that they deem inappropriate, threatening, offensive, or harmful.
 
 Community leaders have the right and responsibility to remove, edit, or reject comments, commits, code, wiki edits, issues, and other contributions that are not aligned to this Code of Conduct, and will communicate reasons for moderation decisions when appropriate.
 
 ## Scope
 
-This Code of Conduct applies within all community spaces, and also applies when an individual is officially representing the community in public spaces. Examples of representing our community include using an official e-mail address, posting via an official social media account, or acting as an appointed representative at an online or offline event.
+This Code of Conduct applies within all community spaces, and applies when an individual is officially representing the community in public spaces. Examples of representing our community include using an official e-mail address, posting via an official social media account, or acting as an appointed representative at an online or offline event.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be reported to the community leaders responsible for enforcement at [magpylib@gmail.com](mailto:magpylib@gmail.com). All complaints will be reviewed and investigated promptly and fairly.
 
 All community leaders are obligated to respect the privacy and security of the reporter of any incident.
```

### Comparing `magpylib-5.0.2/CONTRIBUTING.md` & `magpylib-5.0.3/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Contribute
+# Contribution Guide
 
 The success of Magpylib relies on its user-friendliness. Your feedback and participation in discussions is strongly encouraged. Ask questions about Magpylib. Tell us what you like and what you dislike. Start general discussions in our informal [Discussions](https://github.com/magpylib/magpylib/discussions) channel on GitHub.
 
-We use GitHub [Issues and Milestones](https://github.com/magpylib/magpylib/issues) to plan and track the Magpylib project. Open new Issues to report a bug, to point out a problem, or to  make a feature request, e.g. following a fruitful discussion. Within the Issue we will together define in detail what should be done. For small bug fixes, code cleanups, and other small improvements its not necessary to create issues.
+We use GitHub [Issues and Milestones](https://github.com/magpylib/magpylib/issues) to plan and track the Magpylib project. Open new Issues to report a bug, to point out a problem, or to make a feature request, e.g. following a fruitful discussion. Within the issue we will define in detail what should be done. For small bug fixes, code cleanups, and other small improvements it's not necessary to create issues.
 
 Always feel free to reach out through the official email <magpylib@gmail.com>.
 
-## How to Contribute with Coding...
+## How to Contribute with Coding
 
 You are most welcome to become a project contributor by helping us with coding. This includes the implementation of new features, fixing bugs, code cleanup and restructuring as well as documentation improvements. Please abide by the following procedure to make things easy for us to review and to manage the project.
 
 1. Fork the Magpylib repository to your GitHub account
 2. Edit your new repository (good practice: clone to local machine, edit, push changes).
 3. Rebase your new repository (or pull from upstream) regularly to include upstream changes.
 4. Once your changes are complete (see [Coding requirements](coding-requ) below), or you want some feedback, make a pull request (PR) targeting the Magpylib repository. Explain your feature in the PR, and/or refer to the respective issue that you address. Add illustrative code examples.
 5. Once a PR is created, our pipeline tests will automatically check your code. A Magpylib member will review your contributions and discuss your changes. Possible improvements will be requested.
 6. When satisfied, the reviewer will merge your PR and you become an official Magpylib contributor.
 
 (coding-requ)=
 ## Coding Requirements
 
-- All code is well documented and all top level doc strings abide by the [Numpy docstring style](https://numpydoc.readthedocs.io/en/latest/format.html).
+- All code is well documented and all top level doc strings abide by the [NumPy docstring style](https://numpydoc.readthedocs.io/en/latest/format.html).
 - All unit tests are running. We recommend using the [Pytest](https://docs.pytest.org/en/7.4.x/) package.
 - New unit tests are written aiming for 100% code coverage. We use [Coverage](https://coverage.readthedocs.io/en/) to test this.
 - [Pylint](https://pylint.readthedocs.io/en/stable/) rates your code 10/10 and there are no formatting issues reported (e.g. line-too-long).
 - Your code is PEP8 compliant and formatted with [Black](https://black.readthedocs.io/en/stable/) default settings.
 
 We strongly suggest that you use the [Pre-Commit](https://pre-commit.com/) hooks that apply important code checks which each commit.
```

### Comparing `magpylib-5.0.2/LICENSE` & `magpylib-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/README.md` & `magpylib-5.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 </a>
 <a href="https://codecov.io/gh/magpylib/magpylib"> <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg">
 </a>
 <a href="https://pypi.org/project/magpylib/"> <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18">
 </a>
 <a href="https://anaconda.org/conda-forge/magpylib"> <img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18">
 </a>
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.2?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.3?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
 </a>
 <a href="https://github.com/psf/black"> <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" height="18">
 </a>
 </div>
 
 Magpylib is a Python package for calculating **3D static magnetic fields** of magnets, line currents and other sources. The computation is based on explicit expressions and is therefore **extremely fast**. A **user friendly API** enables convenient positioning of sources and observers.
 
@@ -34,15 +34,15 @@
 ```
 pip install magpylib
 ```
 Install from conda forge using **conda**
 ```
 conda install -c conda-forge magpylib
 ```
-Magpylib supports _Python3.10+_ and relies on common scientific computation libraries _Numpy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
+Magpylib supports _Python3.10+_ and relies on common scientific computation libraries _NumPy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
 
 # Resources
 
  - Check out our **[Documentation](https://magpylib.readthedocs.io/en/latest)** for detailed information.
  - Please abide by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/CODE_OF_CONDUCT.md)**.
  - Contribute through **[Discussions](https://github.com/magpylib/magpylib/discussions)** and coding by following the **[Contribution Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The Git project **[Issues](https://github.com/magpylib/magpylib/issues)** give an up-to-date list of potential enhancements and planned milestones. Propose new ones.
  - A **[Youtube video](https://www.youtube.com/watch?v=LeUx6cM1vcs)** introduction to Magpylib v4.0.0 within the **[GSC network](https://www.internationalcollaboration.org/).**
@@ -132,11 +132,11 @@
 A valid software citation could be
 
 ```
 @software{magpylib,
     author = {{Michael-Ortner et al.}},
     title = {magpylib},
     url = {https://magpylib.readthedocs.io/en/latest/},
-    version = {5.0.2},
+    version = {5.0.3},
     date = {2023-06-25},
 }
 ```
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 _[_M_y_B_i_n_d_e_r_ _l_i_n_k_]_[_b_l_a_c_k_]
 Magpylib is a Python package for calculating **3D static magnetic fields** of
 magnets, line currents and other sources. The computation is based on explicit
 expressions and is therefore **extremely fast**. A **user friendly API**
 enables convenient positioning of sources and observers. # Installation Install
 from PyPI using **pip** ``` pip install magpylib ``` Install from conda forge
 using **conda** ``` conda install -c conda-forge magpylib ``` Magpylib supports
-_Python3.10+_ and relies on common scientific computation libraries _Numpy_,
+_Python3.10+_ and relies on common scientific computation libraries _NumPy_,
 _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as
 graphical backend. # Resources - Check out our **[Documentation](https://
 magpylib.readthedocs.io/en/latest)** for detailed information. - Please abide
 by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/
 CODE_OF_CONDUCT.md)**. - Contribute through **[Discussions](https://github.com/
 magpylib/magpylib/discussions)** and coding by following the **[Contribution
 Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The
@@ -72,9 +72,9 @@
 bibtex entry for the [2020 open-access paper](https://www.sciencedirect.com/
 science/article/pii/S2352711020300170) would be ``` @article
 {ortner2020magpylib, title={Magpylib: A free Python package for magnetic field
 computation}, author={Ortner, Michael and Bandeira, Lucas Gabriel Coliado},
 journal={SoftwareX}, volume={11}, pages={100466}, year={2020}, publisher=
 {Elsevier} } ``` A valid software citation could be ``` @software{magpylib,
 author = {{Michael-Ortner et al.}}, title = {magpylib}, url = {https://
-magpylib.readthedocs.io/en/latest/}, version = {5.0.2}, date = {2023-06-25}, }
+magpylib.readthedocs.io/en/latest/}, version = {5.0.3}, date = {2023-06-25}, }
 ```
```

### Comparing `magpylib-5.0.2/docs/Makefile` & `magpylib-5.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/README.md` & `magpylib-5.0.3/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## About Magpylib Documentation
 
-The Documentation is built with [Sphinx](http://www.sphinx-doc.org/en/main/) v5.3.0 and the configuration file is [conf.py](./conf.py). Files get converted to `.html` files by Sphinx during build time. Images, web code and videos are kept in the [_static](./_static) folder.
+The Documentation is built with [Sphinx](http://www.sphinx-doc.org/en/main/) and the configuration file is [conf.py](./conf.py). Files get converted to `.html` files by Sphinx during build time. Images, web code and videos are kept in the [_static](./_static) folder.
 
 ### API docs
- The docstring format is under the [Numpy Convention](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_numpy.html). Sphinx is configured to read Docstring information from the codebase and convert it into pages utilizing the [autodoc extension](http://www.sphinx-doc.org/en/main/usage/extensions/autodoc.html). The generated files are created at build time and put into a folder called `_autogen`
+ The docstring format is under the [NumPy Convention](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_numpy.html). Sphinx is configured to read Docstring information from the codebase and convert it into pages utilizing the [autodoc extension](http://www.sphinx-doc.org/en/main/usage/extensions/autodoc.html). The generated files are created at build time and put into a folder called `_autogen`
 
 ### Handwritten documents
 Handwritten pages and guides are kept in the [_pages](./_pages) folder. They are all written in [Markdown](https://www.markdownguide.org/) using [myst-parser](https://github.com/executablebooks/MyST-Parser) as interface. Some documents like in the examples folder are dynamically computed with [myst-nb](https://github.com/executablebooks/myst-nb) as jupyter notebooks. With the help of the [jupytext](https://github.com/mwouts/jupytext) library ands its jupyterlab extension, examples can be written and executed within the jupyterlab ecosystem and saved as markdown file. It is recommended to use the [jupyterlab-myst](https://github.com/executablebooks/jupyterlab-myst) extension to be able to work with the full set of myst markdown flavor within jupyterlab. When editing the docs with vscode, use the [MyST-Markdown](https://marketplace.visualstudio.com/items?itemName=ExecutableBookProject.myst-highlight) extension to visualize the rendered document.
```

### Comparing `magpylib-5.0.2/docs/_pages/docu/docu_physics.md` & `magpylib-5.0.3/docs/_pages/user_guide/guide_resources_01_physics.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,122 +1,123 @@
----
-jupytext:
-  text_representation:
-    extension: .md
-    format_name: myst
-    format_version: 0.13
-    jupytext_version: 1.14.5
-kernelspec:
-  display_name: Python 3
-  language: python
-  name: python3
----
-
-(docu-physics)=
-
-# Physics
+(guide-ressources-physics)=
+# Physics and Computation
 
 ## What is implemented ?
 
-The expressions used in Magpylib describe perfectly homogeneous magnets, surface charges, and line currents with natural boundary conditions. Magpylib is at its best when dealing with static air-coils (no eddy currents, no soft-magnetic cores) and high grade permanent magnets (Ferrite, NdFeB, SmCo or similar materials). When **magnet** permeabilities are below $\mu_r < 1.1$ the error typically undercuts few %. Demagnetization factors are not included. The line **current** solutions give the exact same field as outside of a wire that carries a homogeneous current.
+The expressions used in Magpylib describe perfectly homogeneous magnets, surface charges, and line currents with natural boundary conditions. Magpylib is at its best when dealing with static air-coils (no eddy currents, no soft-magnetic cores) and high-grade permanent magnets (Ferrite, NdFeB, SmCo or similar materials). When **magnet** permeabilities are below $\mu_r < 1.1$ the error typically undercuts few %. Demagnetization factors are not included. The line **current** solutions give the exact same field as outside of a wire that carries a homogeneous current.
 
 ## The analytical solutions
 
 Magnetic field computations in Magpylib are based on known analytical solutions (closed form expressions) to permanent magnet and current problems. The Magpylib implementations are based on the following literature references:
 
-- Field of cuboid magnets: \[Yang1990, Engel-Herbert2005, Camacho2013, Cichon2019\]
-- Field of cylindrical magnets: \[Furlani1994, Derby2009, Caciagli2018, Slanovc2021\]
-- Field of triangular surfaces: \[Guptasarma1999, Janssen2009, Rubeck2013\]
-- Field of the current loop: \[Ortner2022\]
+- Field of cuboid magnets [^1] [^2] [^3] [^4]
+- Field of cylindrical magnets: [^5] [^6] [^7] [^8]
+- Field of triangular surfaces: [^9] [^10] [^11]
+- Field of the current loop: [^12]
 - all others derived by hand
 
 A short reflection on how these formulas can be achieved: In magnetostatics the magnetic field becomes conservative (Maxwell: $\nabla \times {\bf H} = 0$) and can thus be expressed through the magnetic scalar potential $\Phi_m$:
 
 $$
 {\bf H} = -\nabla\cdot\Phi_m
 $$
 
 The solution to this equation can be expressed by an integral over the magnetization distribution ${\bf M}({\bf r})$ as
 
 $$
 \Phi_m({\bf r}) = \frac{1}{4\pi}\int_{V'}\frac{\nabla'\cdot {\bf M}({\bf r}')}{|{\bf r}-{\bf r}'|}dV'+\frac{1}{4\pi}\oint_{S'}\frac{{\bf n}'\cdot {\bf M}({\bf r}')}{|{\bf r}-{\bf r}'|}dS'
 $$
 
-where ${\bf r}$ denotes the position, $V$ is the magnetized volume with surface $S$ and normal vector ${\bf n}$ onto the surface. This solution is derived in detail e.g. in \[Jackson1999\].
+where ${\bf r}$ denotes the position, $V$ is the magnetized volume with surface $S$ and normal vector ${\bf n}$ onto the surface. This solution is derived in detail e.g. in [^13].
 
 The fields of currents are directly derived using the law of Biot-Savart with the current distribution ${\bf J}({\bf r})$:
 
 $$
 {\bf B}({\bf r}) = \frac{\mu_0}{4\pi}\int_{V'} {\bf J}({\bf r}')\times \frac{{\bf r}-{\bf r}'}{|{\bf r}-{\bf r}'|^3} dV'
 $$
 
-In some special cases (simple shapes, homogeneous magnetizations and current distributions) the above integrals can be worked out directly to give analytical formulas (or simple, fast converging series). The derivations can be found in the respective references. A noteworthy comparison between the Coulombian approach and the Amperian current model is given in \[Ravaud2009\].
+In some special cases (simple shapes, homogeneous magnetisations, and current distributions) the above integrals can be worked out directly to give analytical formulas (or simple, fast converging series). The derivations can be found in the respective references. A noteworthy comparison between the Coulombian approach and the Amperian current model is given in [^14].
 
 ## Accuracy of the Solutions and Demagnetization
 
 ### Line currents:
 
 The magnetic field of a wire carrying a homogeneous current density is (on the outside) similar to the field of a line current positioned in the center of the wire, which carries the same total current. Current distributions become inhomogeneous at bends of the wire or when eddy currents (finite frequencies) are involved.
 
+(guide-physics-demag)=
 ### Magnets and Demagnetization
 
 The analytical solutions are exact when bodies have a homogeneous magnetization. However, real materials always have a material response which results in an inhomogeneous magnetization even when the initial magnetization is perfectly homogeneous. There is a lot of literature on such [demagnetization effects](https://en.wikipedia.org/wiki/Demagnetizing_field).
 
-Modern high grade permanent magnets (NdFeB, SmCo, Ferrite) have a very weak material responses (local slope of the magnetization curve, remanent permeability) of the order of $\mu_r \approx 1.05$. In this case the analytical solutions provide an excellent approximation with less than 1% error even at close distance from the magnet surface. A detailed error analysis and discussion is presented in the appendix of \[Malago2020\].
+Modern high grade permanent magnets (NdFeB, SmCo, Ferrite) have a very weak material responses (local slope of the magnetization curve, remanent permeability) of the order of $\mu_r \approx 1.05$. In this case the analytical solutions provide an excellent approximation with less than 1% error even at close distance from the magnet surface. A detailed error analysis and discussion is presented in the appendix of [^15].
 
 Error estimation as a result of the material response is evaluated in more detail in the appendix of [Malagò2020](https://www.mdpi.com/1424-8220/20/23/6873).
 
 Demagnetization factors can be used to compensate a large part of the demagnetization effect. Analytical expressions for the demagnetization factors of cuboids can be found at [magpar.net](http://www.magpar.net/static/magpar/doc/html/demagcalc.html).
 
 
 (phys-remanence)=
 ### Modelling a datasheet magnet
 
 The material remanence, often found in data sheets, simply corresponds to the material magnetization/polarization when not under the influence of external fields. This can never happen, as the material itself generates a magnetic field. Such self-interactions result in self-demagnetization that can be approximated using the demagnetization factors and the material permeability (or susceptibility).
 
 For example, a cube with 1 mm sides has a demagnetization factor is 0.333, see [magpar.net](http://www.magpar.net/static/magpar/doc/html/demagcalc.html). When the remanence field of this cube is 1 T, and its susceptibility is 0.1, the magnetization resulting from self-interaction is reduced to 1 T - 0.3333*0.1 T = 0.9667 T, assuming linear material laws.
 
-A [tutorial](gallery-tutorial-modelling-magnets) explains how to deal with demagnetization effects and how real magnets can be modeled using datasheet values.
+A [tutorial](examples-tutorial-modelling-magnets) explains how to deal with demagnetization effects and how real magnets can be modeled using datasheet values.
 
 It must be understood that the change in magnetization resulting from self-interaction has a homogeneous contribution which is approximated by the demagnetization factor, and an inhomogeneous contribution which cannot be modeled easily with analytical solutions. The inhomogeneous part, however, is typically an order of magnitude lower than the homogenous part. You can use the Magpylib extension [Magpylib material response](https://github.com/magpylib/magpylib-material-response) to model the self-interactions.
 
 ### Soft-Magnetic Materials
 
 Soft-magnetic materials like iron or steel with large permeabilities $\mu_r \sim 1000$ and low remanence fields are dominated by the material response. It is not possible to describe such bodies with analytical solutions. However, recent developments showed that the **Magnetostatic Method of Moments** can be a powerful tool in combination with Magpylib to compute such a material response. An integration into Magpylib is planned in the future.
 
 When a magnet lies in front of a soft-magnetic plate, the contribution from the plate can be modeled with high accuracy using a **mirror**-approach, similar to the electrostatic "mirror charge".
 
 
 (docu-performance)=
-## Computation and Performance
+## Computation Performance
 
 Magpylib code is fully [vectorized](https://en.wikipedia.org/wiki/Array_programming), written almost completely in numpy native. Magpylib automatically vectorizes the computation with complex inputs (many sources, many observers, paths) and never falls back on using loops.
 
 ```{note}
 Maximal performance is achieved when `.getB(sources, observers)` is called only a single time in your program. Try not to use loops.
 ```
 
-The object oriented interface comes with an overhead. If you want to achieve maximal performance this overhead can be avoided with {ref}`docu-functional-interface`.
+The object-oriented interface comes with an overhead. If you want to achieve maximal performance this overhead can be avoided with {ref}`docs-field-functional`.
 
 The analytical solutions provide extreme performance. Single field evaluations take of the order of `100 µs`. For large input arrays (e.g. many observer positions or many similar magnets) the computation time can drop below `1 µs` per evaluation point on single state-of-the-art x86 mobile cores (tested on `Intel Core i5-8365U @ 1.60GHz`), depending on the source type.
 
 ## Numerical stability
 
-Many expressions provided in the literature have very questionable numerical stability. Many of these problems are fixed in Magpylib, but one should be aware that accuracy can be a problem very close to objects, close the z-axis in cylindrical symmetries, at edge extensions, and at large distances. We are working on fixing these problems. Some details can be found in \[Ortner2022\].
+Many expressions provided in the literature have very questionable numerical stability. Many of these problems are fixed in Magpylib, but one should be aware that accuracy can be a problem very close to objects, close the z-axis in cylindrical symmetries, at edge extensions, and at large distances. We are working on fixing these problems. Some details can be found in [^12].
 
 **References**
 
-- \[Yang1990\] Z. J. Yang et al., "Potential and force between a magnet and a bulk Y1Ba2Cu3O7-d superconductor studied by a mechanical pendulum", Superconductor Science and Technology 3(12):591, 1990
-- \[Engel-Herbert2005\] R. Engel-Herbert et al., Journal of Applied Physics 97(7):074504 - 074504-4 (2005)
-- \[Camacho2013\] J.M. Camacho and V. Sosa, "Alternative method to calculate the magnetic field of permanent magnets with azimuthal symmetry", Revista Mexicana de Fisica E 59 8–17, 2013
-- \[Cichon2019\] D. Cichon, R. Psiuk and H. Brauer, "A Hall-Sensor-Based Localization Method With Six Degrees of Freedom Using Unscented Kalman Filter", IEEE Sensors Journal, Vol. 19, No. 7, April 1, 2019.
-- \[Furlani1994\] E. P. Furlani, S. Reanik and W. Janson, "A Three-Dimensional Field Solution for Bipolar Cylinders", IEEE Transaction on Magnetics, VOL. 30, NO. 5, 1994
-- \[Derby2009\] N. Derby, "Cylindrical Magnets and Ideal Solenoids", arXiv:0909.3880v1, 2009
-- \[Caciagli2018\] A. Caciagli, R. J. Baars, A. P. Philipse and B. W. M. Kuipers, "Exact expression for the magnetic field of a finite cylinder with arbitrary uniform magnetization", Journal of Magnetism and Magnetic Materials 456 (2018) 423–432.
-- \[Slanovc2022\] F. Slanovc, M. Ortner, M. Moridi, C. Abert and D. Suess, "Full analytical solution for the magnetic field of uniformly magnetized cylinder tiles", submitted to Journal of Magnetism and Magnetic Materials.
-- \[Ortner2022\] M. Ortner, S. Slanovc and P. Leitner, "Numerically Stable and Computationally Efficient Expression for the Magnetic Field of a Current Loop", MDPI Magnetism, 3(1), 11-31, 2022.
-- \[Guptasarma1911\] D. Guptasarma and B. Singh, "New scheme for computing the magnetic field resulting from a uniformly magnetized arbitrary polyhedron", Geophysics (1999), 64(1):70.
-- \[Janssen2009\] J.L.G. Janssen, J.J.H. Paulides and E.A. Lomonova, "3D ANALYTICAL FIELD CALCULATION USING TRIANGULAR MAGNET SEGMENTS APPLIED TO A SKEWED LINEAR PERMANENT MAGNET ACTUATOR", ISEF 2009 - XIV International Symposium on Electromagnetic Fields in Mechatronics, Electrical and Electronic Engineering Arras, France, September 10-12, 2009
-- \[Rubeck2013\] C. Rubeck et al., "Analytical Calculation of Magnet Systems: Magnetic Field Created by Charged Triangles and Polyhedra", IEEE Transactions on Magnetics, VOL. 49, NO. 1, 2013
-- \[Jackson1999\] J. D. Jackson, "Classical Electrodynamics", 1999 Wiley, New York
-- \[Ravaud2009\] R. Ravaud and G. Lamarquand, "Comparison of the coulombian and amperian current models for calculating the magnetic field produced by radially magnetized arc-shaped permanent magnets", HAL Id: hal-00412346
-- \[Malago2020\] P. Malagò et al., Magnetic Position System Design Method Applied to Three-Axis Joystick Motion Tracking. Sensors, 2020, 20. Jg., Nr. 23, S. 6873.
+[^1]: Z. J. Yang et al., "Potential and force between a magnet and a bulk Y1Ba2Cu3O7-d superconductor studied by a mechanical pendulum", Superconductor Science and Technology 3(12):591, 1990
+
+[^2]: R. Engel-Herbert et al., Journal of Applied Physics 97(7):074504 - 074504-4 (2005)
+
+[^3]: J.M. Camacho and V. Sosa, "Alternative method to calculate the magnetic field of permanent magnets with azimuthal symmetry", Revista Mexicana de Fisica E 59 8–17, 2013
+
+[^4]: D. Cichon, R. Psiuk and H. Brauer, "A Hall-Sensor-Based Localization Method With Six Degrees of Freedom Using Unscented Kalman Filter", IEEE Sensors Journal, Vol. 19, No. 7, April 1, 2019.
+
+[^5]: E. P. Furlani, S. Reanik and W. Janson, "A Three-Dimensional Field Solution for Bipolar Cylinders", IEEE Transaction on Magnetics, VOL. 30, NO. 5, 1994
+
+[^6]: N. Derby, "Cylindrical Magnets and Ideal Solenoids", arXiv:0909.3880v1, 2009
+
+[^7]: A. Caciagli, R. J. Baars, A. P. Philipse and B. W. M. Kuipers, "Exact expression for the magnetic field of a finite cylinder with arbitrary uniform magnetization", Journal of Magnetism and Magnetic Materials 456 (2018) 423–432.
+
+[^8]: F. Slanovc, M. Ortner, M. Moridi, C. Abert and D. Suess, "Full analytical solution for the magnetic field of uniformly magnetized cylinder tiles", submitted to Journal of Magnetism and Magnetic Materials.
+
+[^9]: D. Guptasarma and B. Singh, "New scheme for computing the magnetic field resulting from a uniformly magnetized arbitrary polyhedron", Geophysics (1999), 64(1):70.
+
+[^10]: J.L.G. Janssen, J.J.H. Paulides and E.A. Lomonova, "3D ANALYTICAL FIELD CALCULATION USING TRIANGULAR MAGNET SEGMENTS APPLIED TO A SKEWED LINEAR PERMANENT MAGNET ACTUATOR", ISEF 2009 - XIV International Symposium on Electromagnetic Fields in Mechatronics, Electrical and Electronic Engineering Arras, France, September 10-12, 2009
+
+[^11]: C. Rubeck et al., "Analytical Calculation of Magnet Systems: Magnetic Field Created by Charged Triangles and Polyhedra", IEEE Transactions on Magnetics, VOL. 49, NO. 1, 2013
+
+[^12]: M. Ortner, S. Slanovc and P. Leitner, "Numerically Stable and Computationally Efficient Expression for the Magnetic Field of a Current Loop", MDPI Magnetism, 3(1), 11-31, 2022.
+
+[^13]: J. D. Jackson, "Classical Electrodynamics", 1999 Wiley, New York
+
+[^14]: R. Ravaud and G. Lamarquand, "Comparison of the coulombian and amperian current models for calculating the magnetic field produced by radially magnetized arc-shaped permanent magnets", HAL Id: hal-00412346
+
+[^15]: P. Malagò et al., Magnetic Position System Design Method Applied to Three-Axis Joystick Motion Tracking. Sensors, 2020, 20. Jg., Nr. 23, S. 6873.
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_app_end_of_shaft.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_app_end_of_shaft.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,75 +8,75 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-app-end-of-shaft)=
+(examples-app-end-of-shaft)=
 
 # Magnetic Angle Sensor
 
-End of shaft angle sensing is a classical example for a magnetic position system. The goal is to determine the angular position of a rotating shaft. A magnet, typically a diametrically magnetized cylinder, is mounted at the end of the shaft. A 2D sensor is mounted below. When the shaft rotates the two sensor outputs will be $s_1=B_0 sin(\varphi)$ and $s_2=B_0 cos(\varphi)$, so that the angle is uniquely given by $\varphi = arctan_2(s_1,s_2)$.
+End of shaft angle sensing is a classic example for a magnetic position system. The goal is to determine the angular position of a rotating shaft. A magnet, typically a diametrically magnetized cylinder, is mounted at the end of the shaft. A 2D sensor is mounted below. When the shaft rotates the two sensor outputs will be $s_1=B_0 sin(\varphi)$ and $s_2=B_0 cos(\varphi)$, so that the angle is uniquely given by $\varphi = arctan_2(s_1,s_2)$.
 
 In the example below we show such a typical end-of-shaft system with a 2-pixel sensor, that is commonly used to eliminate external stray fields. In addition, we assume that the magnet is not perfectly mounted at the end of the shaft, but slightly displaced to the side, which results in a wobble motion. Such tolerances are easily implemented with Magpylib, they can be visualized and their influence on the sensor output signal can be tested quickly.
 
 ```{code-cell} ipython3
 import numpy as np
 import plotly.express as px
 import magpylib as magpy
 import plotly.graph_objects as go
 
-# create magnet
+# Create magnet
 magnet = magpy.magnet.Cylinder(
     polarization=(1, 0, 0),
     dimension=(.06, .02),
     position=(0, 0, .015),
     style_label="Magnet",
     style_color=".7",
 )
 
-# create shaft dummy with 3D model
+# Create shaft dummy with 3D model
 shaft = magpy.misc.CustomSource(
     position=(0, 0, .07),
     style_color=".7",
     style_model3d_showdefault=False,
     style_label="Shaft",
 )
 shaft_trace = magpy.graphics.model3d.make_Prism(
     base=20,
     diameter=.1,
     height=.1,
     opacity=0.3,
 )
 shaft.style.model3d.add_trace(shaft_trace)
 
-# shaft rotation / magnet wobble motion
+# Shaft rotation / magnet wobble motion
 displacement = .01
 angles = np.linspace(0, 360, 72)
 coll = magnet + shaft
 magnet.move((displacement, 0, 0))
 coll.rotate_from_angax(angles, "z", anchor=0, start=0)
 
-# create sensor
+# Create sensor
 gap = .03
 sens = magpy.Sensor(
     position=(0, 0, -gap),
     pixel=[(.01, 0, 0), (-.01, 0, 0)],
     style_pixel_size=0.5,
     style_size=1.5,
 )
 
-# show 3D animation of wobble motion
+# Show 3D animation of wobble motion
 fig1 = go.Figure()
 magpy.show(magnet, sens, shaft, animation=True, backend="plotly", canvas=fig1)
 fig1.update_layout(scene_camera_eye_z=-1.1)
 fig1.show()
 
-# show sensor output in plotly
+# Show sensor output in plotly
 fig2 = go.Figure()
 df = sens.getB(magnet, output="dataframe")
 df["angle (deg)"] = angles[df["path"]]
 
 fig2 = px.line(
     df,
     x="angle (deg)",
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_app_helmholtz.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_app_coils.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     jupytext_version: 1.13.7
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 ---
 
-(gallery-app-helmholtz)=
+(examples-app-helmholtz)=
 
 # Coils
 
 In this example we show how to model air-coils, then combine two coils into a Helmholtz-pair and visualize the homogeneity of the resulting magnetic field. A nice explanation of coils and the magnetic field is given [here](https://www.nagwa.com/en/explainers/186157825721/#:~:text=The%20magnetic%20field%20strength%2C%20%F0%9D%90%B5,%EF%8A%AD%20T%E2%8B%85m%2FA.). With the code examples below you can easily compare Magpylib results to results presented in this tutorial.
 
 ## Coil models
 
@@ -53,15 +53,17 @@
 
 coil2.show()
 ```
 
 **Model 3:** A [Helmholtz coil](https://en.wikipedia.org/wiki/Helmholtz_coil) is a device for producing a region of nearly uniform magnetic field. It consists of two coils on the same axis, carrying an equal electric current in the same direction. In classical layouts, the distance between the coils is similar to the coil radius.
 
 ```{code-cell} ipython3
-# create a finite sized Helmholtz coil-pair
+# Continuation from above - ensure previous code is executed
+
+# Create a finite sized Helmholtz coil-pair
 coil1 = magpy.Collection()
 for z in np.linspace(-1, 1, 5):
     for r in np.linspace(4, 5, 5):
         winding = magpy.current.Circle(
             current=10,
             diameter=2*r,
             position=(0,0,z),
@@ -77,78 +79,81 @@
 ```
 
 ## Plotting the field
 
 Streamplot from Matplotlib is a powerful tool to outline the field lines. However, it must be understood that streamplot shows only a projection of the field onto the observation plane. All field components that point out of the plane become invisible. In out example we choose symmetry planes, where the perpendicular component is negligible.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 import matplotlib.pyplot as plt
 fig, ax = plt.subplots(1, 1, figsize=(6,5))
 
-# create grid
-ts = np.linspace(-13, 13, 20)
-grid = np.array([[(x,0,z) for x in ts] for z in ts])
+# Compute field and plot the coil pair field on yz-grid
+grid = np.mgrid[0:0:1j, -13:13:20j, -13:13:20j].T[:,:,0]
+_, Y, Z = np.moveaxis(grid, 2, 0)
 
-# compute and plot field of Helmholtz
 B = magpy.getB(helmholtz, grid)
+_, By, Bz = np.moveaxis(B, 2, 0)
+
 Bamp = np.linalg.norm(B, axis=2)
 Bamp /= np.amax(Bamp)
 
-sp = ax.streamplot(
-    grid[:,:,0], grid[:,:,2], B[:,:,0], B[:,:,2],
-    density=2,
-    color=Bamp,
-    linewidth=np.sqrt(Bamp)*3,
-    cmap='coolwarm',
+sp = ax.streamplot(Y, Z, By, Bz, density=2, color=Bamp,
+    linewidth=np.sqrt(Bamp)*3, cmap='coolwarm',
 )
 
-# plot coil outline
+# Plot coil outline
 from matplotlib.patches import Rectangle
 for loc in [(4,4), (4,-6), (-6,4), (-6,-6)]:
     ax.add_patch(Rectangle(loc, 2, 2, color='k', zorder=10))
 
-# figure styling
+# Figure styling
 ax.set(
     title='Magnetic field of Helmholtz',
-    xlabel='x-position (m)',
+    xlabel='y-position (m)',
     ylabel='z-position (m)',
     aspect=1,
 )
 plt.colorbar(sp.lines, ax=ax, label='(T)')
 
 plt.tight_layout()
 plt.show()
 ```
 
 ## Helmholtz field homogeneity
 
 While the optimal solution is given by two current loops, real world applications must deal with finite sizes and limited construction space. Here Magpylib enables fast analysis of different possible geometries.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
+import matplotlib.pyplot as plt
 fig, ax = plt.subplots(1, 1, figsize=(6,5))
 
-# compute field of the coil pair on grid
-ts = np.linspace(-3, 3, 20)
-grid = np.array([[(x,0,z) for x in ts] for z in ts])
+# Compute field of the coil pair on yz-grid
+grid = np.mgrid[0:0:1j, -3:3:20j, -3:3:20j].T[:,:,0]
+_, Y, Z = np.moveaxis(grid, 2, 0)
+
 B = helmholtz.getB(grid)
 
-# field at center
+# Field at center
 B0 = helmholtz.getB((0,0,0))
 B0amp = np.linalg.norm(B0)
 
-# homogeneity error
+# Homogeneity error
 err = np.linalg.norm((B-B0)/B0amp, axis=2)
 
-# plot error on grid
-sp = ax.contourf(grid[:,:,0], grid[:,:,2], err*100)
+# Plot error on grid
+sp = ax.contourf(Y, Z, err*100)
 
-# figure styling
+# Figure styling
 ax.set(
     title='Helmholtz homogeneity error',
-    xlabel='x-position (m)',
+    xlabel='y-position (m)',
     ylabel='z-position (m)',
     aspect=1,
 )
 plt.colorbar(sp, ax=ax, label='(% of B0)')
 
 plt.tight_layout()
 plt.show()
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_misc_compound.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_misc_compound.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-misc-compound)=
+(examples-misc-compound)=
 
 # Compounds
 
 The `Collection` class is a powerful tool for grouping and tracking object assemblies. However, it is often convenient to have assembly parameters themselves, like number of magnets, as variables. This is achieved by sub-classing `Collection`. We refer to such classes as "**Compounds**" and show how to seamlessly integrate them into Magpylib.
 
 ## Subclassing collections
 
-In the following example we design a compound class `MagnetRing` which represents a ring of cuboid magnets with the parameter `cubes` that should refer to the number of magnets on the ring. The ring will automatically adjust its size when `cubes` is modified. We also add an encompassing 3D model.
+In the following example we design a compound class `MagnetRing` which represents a ring of cuboid magnets with the parameter `cubes` that should refer to the number of magnets on the ring. The ring will automatically adjust its size when `cubes` is modified, including an additionally added encompassing 3D model that may, for example, represent a mechanical magnet holder.
 
 ```{code-cell} ipython3
 import magpylib as magpy
 
 class MagnetRing(magpy.Collection):
     """ A ring of cuboid magnets
 
@@ -86,14 +86,16 @@
 
         return self
 ```
 
 This new `MagnetRing` class seamlessly integrates into Magpylib and makes use of the position and orientation interface, field computation and graphic display.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 # Add a sensor
 sensor = magpy.Sensor(position=(0, 0, 0))
 
 # Create a MagnetRing object
 ring = MagnetRing()
 
 # Move MagnetRing around
@@ -105,14 +107,16 @@
 # Display graphically
 magpy.show(ring, sensor, backend='plotly')
 ```
 
 The `MagnetRing` parameter `cubes` can be modified dynamically:
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 print(f"B-field at sensor for modified ring → {ring.getB(sensor).round(3)}")
 
 ring.cubes = 10
 
 print(f"B-field at sensor for modified ring → {ring.getB(sensor).round(3)}")
 
 magpy.show(ring, sensor, backend='plotly')
@@ -186,14 +190,16 @@
         )
         return trace
 ```
 
 We have removed the trace construction from the `_update` method, and instead provided `_custom_trace3d` as a callable.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 ring0 = MagnetRing()
 %time for _ in range(10): ring0.cubes=10
 
 ring1 = MagnetRingAdv()
 %time for _ in range(10): ring1.cubes=10
 ```
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_misc_field_interpolation.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_misc_field_interpolation.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-misc-field-interpolation)=
+(examples-misc-field-interpolation)=
 
 # Field Interpolation
 
 There are several reasons for working with field interpolations rather than computing the field on demand.
 
 1. Very large grids take a lot of time to compute, even with Magpylib.
 2. The field might not be accessible through Magpylib, e.g. when demagnetization is included, but it can be computed with a 3rd party FE tool or is the result of an experiment.
@@ -114,17 +114,19 @@
 
 # Display custom
 magpy.show(custom, cube, zoom=1, backend="matplotlib")
 ```
 
 ## Testing Interpolation Accuracy
 
-Finally, we compare the "exact" field of the cuboid source with the interpolated field of the custom source. For this purpose a sensor is added and a generic rotation is applied to the sources. Naturally there is some error that can be reduced by increasing the interpolation grid finesse.
+Finally, we compare the "exact" field of the cuboid source with the interpolated field of the custom source. For this purpose, a sensor is added and a generic rotation is applied to the sources. Naturally there is some error that can be reduced by increasing the interpolation grid finesse.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 import matplotlib.pyplot as plt
 
 # Modify orientation of cube and custom
 for src in [cube, custom]:
     src.rotate_from_angax(angle=45, axis=(1,1,1))
 
 # Add a sensor for testing
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_convex_hull.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_convex_hull.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-shapes-convex-hull)=
+(examples-shapes-convex-hull)=
 
 # Convex Hull
 
 In geometry the convex hull of a point cloud is the smallest convex shape that contains all points, see [Wikipedia](https://en.wikipedia.org/wiki/Convex_hull).
 
-Magpylib offers construction of convex hull magnets by combining the `magpylib.magnets.TriangularMesh` and the [scipy.spatial.ConvexHull](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.ConvexHull.html) classes via the classmethod `from_ConvexHull`. Note, that the Scipy method does not guarantee correct face orientations if `reorient_faces` is disabled.
+Magpylib offers construction of convex hull magnets by combining the `magpylib.magnets.TriangularMesh` and the [scipy.spatial.ConvexHull](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.ConvexHull.html) classes via the class method `from_ConvexHull`. Note, that the Scipy method does not guarantee correct face orientations if `reorient_faces` is disabled.
 
 ## Pyramid magnet
 
 This is the fastest way to construct a pyramid magnet.
 
 ```{code-cell} ipython3
 import numpy as np
-
 import magpylib as magpy
 
 # Create pyramid magnet
 points = np.array([(-2, -2, 0), (-2, 2, 0), (2, -2, 0), (2, 2, 0), (0, 0, 3)]) / 100
 tmesh_pyramid = magpy.magnet.TriangularMesh.from_ConvexHull(
     polarization=(0, 0, 1),
     points=points,
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_pyvista.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_pyvista.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-shapes-pyvista)=
+(examples-shapes-pyvista)=
 
 # Pyvista Bodies
 
 [Pyvista](https://docs.pyvista.org/version/stable/) is a powerful open-source tool for the creation and visualization of meshes. Pyvista `PolyData` objects can be directly transformed into Magpylib `TriangularMesh` magnets via the classmethod `from_pyvista`.
 
 ```{note}
 The Pyvista library used in the following examples is not automatically installed with Magpylib. A Pyvista installation guide is found [here](https://docs.pyvista.org/getting-started/installation.html).
@@ -84,21 +84,21 @@
 ```
 
 The result cannot be used for magnetic field computation. Even if all faces were present, the reorient-faces algorithm would fail when these faces are disconnected. Such problems can be fixed by
 
 1. giving Pyvista a finer mesh to work with from the start
 2. Pyvista mesh cleaning (merge duplicate points, remove unused points, remove degenerate faces)
 
-The following code produces a clean magnet .
+The following code produces a clean magnet.
 
 ```{code-cell} ipython3
 import pyvista as pv
 import magpylib as magpy
 
-# Create a complex pyvista PolyData object using a boolean operation. Start with
+# Create a complex Pyvista PolyData object using a boolean operation. Start with
 # finer mesh and clean after operation
 sphere = pv.Sphere(radius=0.6)
 cube = pv.Cube().triangulate().subdivide(2)
 obj = cube.boolean_difference(sphere)
 obj = obj.clean()
 obj = obj.scale([1e-2]*3)
 
@@ -112,15 +112,7 @@
 print(f'mesh status open: {magnet.status_open}')
 print(f'mesh status disconnected: {magnet.status_disconnected}')
 print(f"mesh status self-intersecting: {magnet.status_selfintersecting}")
 print(f'mesh status reoriented: {magnet.status_reoriented}')
 
 magnet.show(backend="plotly")
 ```
-
-```{code-cell} ipython3
-
-```
-
-```{code-cell} ipython3
-
-```
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_superpos.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_superpos.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-shapes-superpos)=
+(examples-shapes-superpos)=
 
 # Superposition
 
 The [superposition principle](https://en.wikipedia.org/wiki/Superposition_principle) states that the net response caused by two or more stimuli is the sum of the responses caused by each stimulus individually. This principle holds in magnetostatics when there is no material response, and simply states that the total field created by multiple magnets and currents is the sum of the individual fields.
 
 When two magnets overlap geometrically, the magnetization in the overlap region is given by the vector sum of the two individual magnetizations. This enables two geometric operations,
 
 :::::{grid} 1 2 2 2
 :gutter: 4
 
 ::::{grid-item-card} Union
-:img-bottom: ../../_static/images/docu_field_superpos_union.png
+:img-bottom: ../../../_static/images/docu_field_superpos_union.png
 :shadow: None
 Build complex forms by aligning base shapes (no overlap) with each other with similar magnetization vector.
 ::::
 
 ::::{grid-item-card} Cut-Out
-:img-bottom: ../../_static/images/docu_field_superpos_cutout.png
+:img-bottom: ../../../_static/images/docu_field_superpos_cutout.png
 :shadow: None
 When two objects with opposing magnetization vectors of similar amplitude overlap, they will just cancel in the overlap region. This enables geometric cut-out operations.
 ::::
 :::::
 
 
 ## Union operation
@@ -72,44 +72,45 @@
 with magpy.show_context(magnet, sensor, backend="plotly", style_legend_show=False) as s:
     s.show(col=1)
     s.show(output="B", col=2)
 ```
 
 ## Cut-out operation
 
-When two objects with opposing magnetization vectors of similar amplitude overlap, they will just cancel in the overlap region. This enables geometric cut-out operations. In the following example we construct an exact hollow cylinder solution from two concentric cylinder shapes with opposite magnetizations, and compare the result to the `CylinderSegment` class solution.
+When two objects with opposing magnetization vectors of similar amplitude overlap, they will just cancel in the overlap region. This enables geometric cut-out operations. In the following example we construct an exact hollow cylinder solution from two concentric cylinder shapes with opposite magnetizations and compare the result to the `CylinderSegment` class solution.
 
 Here the `getM` and `getJ` functions come in handy. They allow us to see the magnetization distribution that is the result of the superposition.
 
 ```{code-cell} ipython3
 import numpy as np
 import matplotlib.pyplot as plt
 import magpylib as magpy
 
 fig, [ax1, ax2] = plt.subplots(1, 2, figsize=(12, 5))
 
-# Create an observer grid in the xy-symmetry plane
-X, Y = np.mgrid[-4:4:100j, -4:4:100j].transpose((0, 2, 1))
-grid_xy = np.stack([X, Y, np.zeros((100, 100))], axis=2)
-grid_xz = np.stack([X, np.zeros((100, 100)), Y], axis=2)
-
 # Create ring with cut-out
 inner = magpy.magnet.Cylinder(polarization=(0, 0, -1), dimension=(4, 5))
 outer = magpy.magnet.Cylinder(polarization=(0, 0, 1), dimension=(6, 5))
 ring0 = inner + outer
 
-# Compute J-field of ring
-M_xy = np.linalg.norm(ring0.getM(grid_xy), axis=2)
-M_xz = np.linalg.norm(ring0.getM(grid_xz), axis=2)
-
-# Display field with Pyplot
-ax1.contourf(grid_xy[:, :, 0], grid_xy[:, :, 1], M_xy, cmap=plt.cm.hot_r)
-ax2.contourf(grid_xz[:, :, 0], grid_xz[:, :, 2], M_xz, cmap=plt.cm.hot_r)
+# Compute and plot Magnetization in xy-plane
+grid = np.mgrid[-4:4:100j, -4:4:100j, 0:0:1j].T[0]
+X, Y, _ = np.moveaxis(grid, 2, 0)
+
+M = np.linalg.norm(ring0.getM(grid), axis=2)
+ax1.contourf(X, Y, M, cmap=plt.cm.hot_r)
+
+# Compute and plot Magnetization in xz-plane
+grid = np.mgrid[-4:4:100j, 0:0:1j, -4:4:100j].T[:,0]
+X, _, Z = np.moveaxis(grid, 2, 0)
 
-# plot styling
+M = np.linalg.norm(ring0.getM(grid), axis=2)
+ax2.contourf(X, Z, M, cmap=plt.cm.hot_r)
+
+# Plot styling
 ax1.set(
     title="|M| in xy-plane",
     xlabel="x-position",
     ylabel="y-position",
     aspect=1,
     xlim=(-4,4),
     ylim=(-4,4),
@@ -125,30 +126,32 @@
 
 plt.tight_layout()
 plt.show()
 ```
 
 The two figures show that the magnetization is zero outside of the cylinder, as well as in the overlap region where the two magnetizations cancel.
 
-Finally we want to show that the superposition gives the same result as a computation from the CylinderSegment solution.
+Finally, we want to show that the superposition gives the same result as a computation from the CylinderSegment solution.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 from magpylib.magnet import Cylinder, CylinderSegment
 
 # Create ring with CylinderSegment
 ring1 = CylinderSegment(polarization=(0, 0, .1), dimension=(2, 3, 5, 0, 360))
 
 # Print results
 print("CylinderSegment result:", ring1.getB((.01, .02, .03)))
 print("        Cut-out result:", ring0.getB((.01, .02, .03)))
 ```
 
-Note that, it is faster to compute the `Cylinder` field two times than computing the `CylinderSegment` field one time. This is why Magpylib automatically falls back to the `Cylinder` solution whenever `CylinderSegment` is called with 360 deg section angles.
+Note that it is faster to compute the `Cylinder` field two times than computing the `CylinderSegment` field one time. This is why Magpylib automatically falls back to the `Cylinder` solution whenever `CylinderSegment` is called with 360 deg section angles.
 
-Unfortunately, with respect to 3D-models, cut-out operations cannot be displayed graphically at the moment, but {ref}`examples-own-3d-models` offer custom solutions.
+Unfortunately, with respect to 3D-models, cut-out operations cannot be displayed graphically at this point in time, but {ref}`examples-own-3d-models` offer custom solutions.
 
 ## Nice example
 
 The following example combines union and cut-out to create a complex magnet shape which is then displayed by combining a streamplot with a contourplot in matplotlib.
 
 ```{code-cell} ipython3
 import numpy as np
@@ -166,29 +169,25 @@
 )
 pt3 = magpy.magnet.Cuboid(
     polarization=(-1/np.sqrt(2), 1/np.sqrt(2), 0), dimension=(4, 4, 2),
 ).rotate_from_angax(45, 'z')
 magnet = magpy.Collection(pt1, pt2, pt3)
 
 # Compute J on mesh and plot with streamplot
-X, Y = np.mgrid[-6:6:100j, -6:6:100j].transpose((0, 2, 1))
-grid = np.stack([X, Y, np.zeros((100, 100))], axis=2)
+grid = np.mgrid[-6:6:100j, -6:6:100j, 0:0:1j].T[0]
+X, Y, _ = np.moveaxis(grid, 2, 0)
 
 J = magnet.getJ(grid)
 J[J<1e-12] = 0 # cut off numerically small values
+Jx, Jy, _ = np.moveaxis(J, 2, 0)
 
-ax.contourf(grid[:, :, 0], grid[:, :, 1], np.linalg.norm(J,axis=2), cmap=plt.cm.cool)
-ax.streamplot(
-    grid[:, :, 0],
-    grid[:, :, 1],
-    J[:, :, 0],
-    J[:, :, 1], color='k', density=1.5,
-)
+ax.contourf(X, Y, np.linalg.norm(J,axis=2), cmap=plt.cm.cool)
+ax.streamplot(X, Y, Jx, Jy, color='k', density=1.5)
 
-# plot styling
+# Plot styling
 ax.set(
     title="Polarization J in xy-plane",
     xlabel="x-position",
     ylabel="y-position",
     aspect=1,
 )
 plt.tight_layout()
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_shapes_triangle.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_shapes_triangle.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 kernelspec:
   display_name: Python 3 (ipykernel)
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-shapes-triangle)=
+(examples-shapes-triangle)=
 
 # Triangular Meshes
 
-The magnetic field of a homogeneously magnetized body is equivalent to the field of a charged surface. The surface is the hull of the body and the charge density is proportional to the projection of the magnetization vector onto the surface normal.
+The magnetic field of a homogeneously magnetized body is equivalent to the field of a charged surface. The surface is the hull of the body, and the charge density is proportional to the projection of the magnetization vector onto the surface normal.
 
 It is very common to approximate the surface of bodies by triangular meshes, which can then be transformed into magnets using the `Triangle` and the `TriangularMesh` classes. When using these classes one should abide by the following rules:
 
-1. The surface must be closed, or, all missing faces must have zero charge (magnetization vector perpendicular to surface normal).
+1. The surface must be closed, or all missing faces must have zero charge (magnetization vector perpendicular to surface normal).
 2. All triangles are oriented outwards (right-hand-rule)
 3. The surface must not be self-intersecting.
-4. For the B-field the magnetic polarization must be added on the inside of the body.
+4. For the B-field magnetic polarization must be added on the inside of the body.
 
 ## Cuboctahedron Magnet
 
 In this example `Triangle` is used to create a magnet with cuboctahedral shape. Notice that triangle orientation is displayed by default for convenience.
 
 ```{code-cell} ipython3
 import magpylib as magpy
@@ -73,17 +73,17 @@
     style_magnetization_mode="arrow",
     style_orientation_color="yellow",
 )
 ```
 
 ## Triangular Prism Magnet
 
-Consider a prism with triangular base that is magnetized orthogonal to the base. All surface normals of the sides of the prism are orthogonal to the magnetization vector. As a result the sides do not contribute to the magnetic field because their charge density disappears. Only top and bottom surfaces contribute. One must be very careful when defining those surfaces in such a way that the surface normals point outwards.
+Consider a prism with triangular base that is magnetized orthogonal to the base. All surface normals of the sides of the prism are orthogonal to the magnetization vector. As a result, the sides do not contribute to the magnetic field because their charge density disappears. Only the top and bottom surfaces contribute. One must be very careful when defining those surfaces in such a way that the surface normals point outwards.
 
-Leaving out parts of the surface that do not contribute to the field is beneficial for the computation speed.
+Leaving out parts of the surface that do not contribute to the field is beneficial for computation speed.
 
 ```{code-cell} ipython3
 import magpylib as magpy
 
 # Create prism magnet as triangle collection
 top = magpy.misc.Triangle(
     polarization=(0, 0, 1),
@@ -99,21 +99,21 @@
 
 # Display graphically
 magpy.show(*prism, backend="plotly", style_opacity=0.5, style_magnetization_show=False)
 ```
 
 ## TriangularMesh class
 
-While `Triangle` simply provides the field of a charged triangle and can be used to contruct complex forms, it is prone to error and tedious to work with when meshes become large. For this purpose the `TriangularMesh` class ensures proper and convenient magnet creation by automatically checking mesh integrity and by orienting the faces at initialization.
+While `Triangle` simply provides the field of a charged triangle and can be used to construct complex forms, it is prone to error and tedious to work with when meshes become large. For this purpose, the `TriangularMesh` class ensures proper and convenient magnet creation by automatically checking mesh integrity and by orienting the faces at initialization.
 
 ```{attention}
 Automatic face reorientation of `TriangularMesh` may fail when the mesh is open.
 ```
 
-In this example we revisit the cuboctahedron, but generate it through the `TriangularMesh` class.
+In this example we revisit the cuboctahedron but generate it through the `TriangularMesh` class.
 
 ```{code-cell} ipython3
 import magpylib as magpy
 import numpy as np
 
 # Create cuboctahedron magnet (vertices and faces are transposed here for more compact display)
 vertices_cm = [
@@ -134,29 +134,29 @@
 
 # Display TriangularMesh body
 magpy.show(
     cuboc, backend="plotly", style_mesh_grid_show=True, style_mesh_grid_line_width=4
 )
 ```
 
-The `TriangularMesh` class is extremely powerful as it enables almost arbitrary magnet shapes. It is described in detail in {ref}`docu-magpylib-api-trimesh`. There are many ways to generate such triangular meshes. An example thereof is shown in {ref}`gallery-shapes-pyvista`.
+The `TriangularMesh` class is extremely powerful as it enables almost arbitrary magnet shapes. It is described in detail in {ref}`docu-magpylib-api-trimesh`. There are many ways to generate such triangular meshes. An example thereof is shown in {ref}`examples-shapes-pyvista`.
 
 ```{caution}
 * `getB` and `getH` compute the fields correctly only if the mesh is closed, not self-intersecting, and all faces are properly oriented outwards.
 
 * Input checks and face reorientation can be computationally expensive. The checks can individually be deactivated by setting `reorient_faces="skip"`, `check_open="skip"`, `check_disconnected="skip"`, and `check_selfintersecting="skip"` at initialization of `TriangularMesh` objects. The checks can also be performed by hand after initialization.
 
-* Meshing tools such as the [Pyvista](https://docs.pyvista.org/) library can be very convenient for building complex shapes, but often do not guarantee that the mesh is properly closed or connected - see {ref}`gallery-shapes-pyvista`.
+* Meshing tools such as the [Pyvista](https://docs.pyvista.org/) library can be very convenient for building complex shapes, but often do not guarantee that the mesh is properly closed or connected - see {ref}`examples-shapes-pyvista`.
 
-* Meshing tools often create meshes with a lot of faces, especially when working with curved surfaces. Keep in mind that the field computation takes of the order of a few microseconds per observer position per face, and that RAM is a limited resource.
+* Meshing tools often create meshes with a lot of faces, especially when working with curved surfaces. Keep in mind that field computation takes of the order of a few microseconds per observer position per face, and that RAM is a limited resource.
 ```
 
 ## Open TriangularMesh
 
-In some cases it may be desirable to generate a `TriangularMesh` object from an open mesh (see Prism example above). In this case one has to be extremely careful because one cannot rely on the checks. Not to generate warnings or error messages, these checks can be disabled with `"skip"` or their outcome can be ignored with `"ignore"`. The `show` function can be used to view open edges and disconnected parts. In the following example we generate such an open mesh directly from `Triangle` objects.
+In some cases, it may be desirable to generate a `TriangularMesh` object from an open mesh (see Prism example above). In this case one must be extremely careful because one cannot rely on the checks. Not to generate warnings or error messages, these checks can be disabled with `"skip"` or their outcome can be ignored with `"ignore"`. The `show` function can be used to view open edges and disconnected parts. In the following example we generate such an open mesh directly from `Triangle` objects.
 
 ```{code-cell} ipython3
 import magpylib as magpy
 import numpy as np
 
 # Create top and bottom faces of a prism magnet
 top = magpy.misc.Triangle(
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_collection.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_collection.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-tutorial-collection)=
+(examples-tutorial-collection)=
 
 # Working with Collections
 
-The top level class `Collection` allows users to group objects by reference for common manipulation. The idea is that
+The top-level class `Collection` allows users to group objects by reference for common manipulation. The following concepts apply to Magpylib Collections:
 
 1. A collection spans its own local frame of reference with position and orientation, to which the children are added. Thus, any operation applied to the collection is individually applied to all its children.
 2. The collection itself behaves like a single Magpylib object (can be source and/or observer).
-3. All children inside the collection can be individually addressed and manipulated at all times.
+3. All children inside the collection can be individually addressed and manipulated, which will automatically manipulate their state inside the parent collection.
 4. Collections have their own `style` attributes, their paths are displayed in `show`, and all children are automatically assigned their parent color.
 
 ## Constructing Collections
 
 Collections have the attributes `children`, `sources`, `sensors` and `collections`. These attributes are ordered lists that contain objects that are added to the collection by reference (not copied). `children` returns a list of all objects in the collection. `sources` returns a list of the sources, `sensors` a list of the sensors and `collections` a list of "sub-collections" within the collection.
 
 ```{code-cell} ipython3
@@ -41,14 +41,16 @@
 print(f"sensors:     {coll.sensors}")
 print(f"collections: {coll.collections}")
 ```
 
 New additions are always added at the end. Use the **`add`** method or the parameters.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 # Copy adjusts object label automatically
 x2 = x1.copy()
 s2 = s1.copy()
 c2 = c1.copy()
 
 # Add objects with add method
 coll.add(x2, s2)
@@ -61,14 +63,16 @@
 print(f"sensors:     {coll.sensors}")
 print(f"collections: {coll.collections}")
 ```
 
 The **`describe`** method is a very convenient way to view a Collection structure, especially when the collection is nested, i.e., when containing other collections.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 # Add more objects
 c1.add(x2.copy())
 c2.add(s2.copy())
 
 coll.describe(format="label+type")
 ```
 
@@ -138,41 +142,42 @@
 for child in coll:
     print(child)
 ```
 
 and makes it possible to directly reference to a child object by index:
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 print(coll[0])
 ```
 
 Collection nesting is powerful to create a self-consistent hierarchical structure, however, it is often in the way of quick child access in nested trees. For this, the `children_all`, `sources_all`, `sensors_all` and `collections_all` read-only parameters, return all objects in the tree:
 
 ```{code-cell} ipython3
 import magpylib as magpy
 
 s1 = magpy.Sensor(style_label="s1")
 s2 = s1.copy()
 s3 = s2.copy()
 
-# this creates a nested collection
+# This creates a nested collection
 coll = s1 + s2 + s3
 coll.describe(format="label")
 
 # _all gives access to the whole tree
 print([s.style.label for s in coll.sensors_all])
 ```
 
 ## Practical Example
 
-The following example demonstrates how collections enable user-friendly manipulation of groups, sub-groups and individual objects.
+The following example demonstrates how collections enable user-friendly manipulation of groups, sub-groups, and individual objects.
 
 ```{code-cell} ipython3
 import numpy as np
-
 import magpylib as magpy
 
 # Construct two coils from windings
 coil1 = magpy.Collection(style_label="coil1")
 for z in np.linspace(-0.0005, 0.0005, 5):
     coil1.add(magpy.current.Circle(current=1, diameter=0.02, position=(0, 0, z)))
 coil1.position = (0, 0, -0.005)
@@ -197,14 +202,16 @@
 # Display as animation
 magpy.show(*helmholtz, animation=True, style_path_show=False)
 ```
 
 For magnetic field computation, a collection with source children behaves like a single source object, and a collection with sensor children behaves like a flat list of its sensors when provided as `sources` and `observers` input respectively.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 import matplotlib.pyplot as plt
 
 B = magpy.getB(helmholtz, (0.01, 0, 0))
 plt.plot(
     B * 1000,  # T -> mT
     label=["Bx", "By", "Bz"],
 )
@@ -215,15 +222,15 @@
 plt.gca().grid(color=".9")
 plt.gca().legend()
 plt.show()
 ```
 
 ## Efficient 3D Models
 
-The graphical backend libraries were not designed for complex 3D graphic output. As a result, it becomes often inconvenient and slow when attempting to display many 3D objects. One solution to this problem when dealing with large collections is to represent the latter by a single encompassing body, and to deactivate the individual 3D models of all children.
+The graphical backend libraries were not designed for complex 3D graphic output. As a result, it often becomes inconvenient and slow when attempting to display many 3D objects. One solution to this problem when dealing with large collections is to represent the latter by a single encompassing body, and to deactivate the individual 3D models of all children.
 
 ```{code-cell} ipython3
 import magpylib as magpy
 
 # Create collection
 coll = magpy.Collection()
 for index in range(10):
@@ -249,8 +256,8 @@
 coll.set_children_styles(model3d_showdefault=False)
 coll.style.label = "Collection with hidden children"
 coll.show()
 ```
 
 ## Compound Objects
 
-Collections can be subclassed to form dynamic groups that seamlessly integrate into Magpylib. Such classes are referred to as **compounds**. An example how this is done is shown in {ref}`gallery-misc-compound`.
+Collections can be subclassed to form dynamic groups that seamlessly integrate into Magpylib. Such classes are referred to as **compounds**. An example of how this is done is shown in {ref}`examples-misc-compound`.
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_custom.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_custom.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-tutorial-custom)=
+(examples-tutorial-custom)=
 
 # CustomSource
 
-The {ref}`docu-magpylib-api-custom` class was implemented to offer easy integration of user field implementations into Magpylib's object-oriented interface.
+The {ref}`guide-docs-classes-custom-source` class was implemented to offer easy integration of user field implementations into Magpylib's object-oriented interface.
 
 ```{note}
 Obviously, any field implementation can be integrated. Specifically, fields where superposition holds and interactions do not disturb the sources (e.g. electric, gravitational, ...) can benefit from Magpylib's position and orientation interface.
 ```
 
 ## Magnetic Monopole
 
@@ -32,83 +32,90 @@
 
 Here the monopole lies in the origin of the local coordinates, $Q_m$ is the monopole charge and ${\bf r}$ is the observer position.
 
 We create this field as a Python function and hand it over to a CustomSource `field_func` argument. The `field_func` input must be a callable with two positional arguments `field` (can be `'B'` or `'H'`) and `observers` (must accept ndarrays of shape (n,3)), and return the respective fields in units of T and A/m in the same shape.
 
 ```{code-cell} ipython3
 import numpy as np
-
 import magpylib as magpy
 
-
 # Create monopole field
 def mono_field(field, observers):
     """
     Monopole field
 
     field: string, "B" or "H
         return B or H-field
 
     observers: array_like of shape (n,3)
         Observer positions
 
     Returns: np.ndarray, shape (n,3)
         Magnetic monopole field
     """
-    Qm = 1e-6  # unit T·m²
+    Qm = 1  # unit T·m²
     obs = np.array(observers).T  # unit m
     B = Qm * (obs / np.linalg.norm(obs, axis=0) ** 3).T  # unit T
     if field == "B":
         return B  # unit T
     elif field == "H":
         H = B / magpy.mu_0  # unit A/m
         return H
     else:
         raise ValueError("Field Value must be either B or H")
 
-
 # Create CustomSource with monopole field
 mono = magpy.misc.CustomSource(field_func=mono_field)
 
 # Compute field
-print(mono.getB((0.001, 0, 0)))
-print(mono.getH((0.001, 0, 0)))
+print(mono.getB((1, 0, 0)))
+print(mono.getH((1, 0, 0)))
 ```
 
 Multiple of these sources can now be combined, making use of the Magpylib position/orientation interface.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 import matplotlib.pyplot as plt
 
 # Create two monopole charges
-mono1 = magpy.misc.CustomSource(field_func=mono_field, position=(0.002, 0.002, 0))
-mono2 = magpy.misc.CustomSource(field_func=mono_field, position=(-0.002, -0.002, 0))
+mono1 = magpy.misc.CustomSource(field_func=mono_field, position=(2, 2, 0))
+mono2 = magpy.misc.CustomSource(field_func=mono_field, position=(-2, -2, 0))
 
 # Compute field on observer-grid
-X, Y = np.mgrid[-0.005:0.005:40j, -0.005:0.005:40j].transpose((0, 2, 1))
-grid = np.stack([X, Y, np.zeros((40, 40))], axis=2)
+grid = np.mgrid[-5:5:100j, -5:5:100j, 0:0:1j].T[0]
+X, Y, _ = np.moveaxis(grid, 2, 0)
+
 B = magpy.getB([mono1, mono2], grid, sumup=True)
+Bx, By, _ = np.moveaxis(B, 2, 0)
 normB = np.linalg.norm(B, axis=2)
 
 # Plot field in x-y symmetry plane
 cp = plt.contourf(X, Y, np.log10(normB), cmap="gray_r", levels=10)
-plt.streamplot(X, Y, B[:, :, 0], B[:, :, 1], color="k", density=1)
+plt.streamplot(X, Y, Bx, By, color="k", density=1)
+
+plt.title("Field of two Monopoles")
+plt.xlabel("x-position (m)")
+plt.ylabel("y-position (m)")
 
 plt.tight_layout()
 plt.show()
 ```
 
 ## Adding a 3D model
 
-While the CustomSource is graphically represented by a simple marker by default, we can easily add a 3D model as described in {ref}`examples-own-3d-models`.
+While `CustomSource` is graphically represented by a simple marker by default, we can easily add a 3D model as described in {ref}`examples-own-3d-models`.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 # Load Sphere model
 trace_pole = magpy.graphics.model3d.make_Ellipsoid(
-    dimension=np.array([3, 3, 3]) * 1e-4,
+    dimension=np.array([.3, .3, .3]),
 )
 
 for mono in [mono1, mono2]:
     # Turn off default model
     mono.style.model3d.showdefault = False
 
     # Add sphere model
@@ -116,17 +123,20 @@
 
 # Display models
 magpy.show(mono1, mono2)
 ```
 
 ## Subclassing CustomSource
 
-In the above example it would be nice to make the CustomSource dynamic, so that it would have a property `charge` that can be changed at will, rather than having to redefine the `field_func` and initialize a new object every time. In the following example we show how to sub-class `CustomSource` to achieve this. The problem is reminiscent of {ref}`gallery-misc-compound`.
+In the above example it would be nice to make the `CustomSource` dynamic, so that it would have a property `charge` that can be changed at will, rather than having to redefine the `field_func` and initialize a new object every time. In the following example we show how to sub-class `CustomSource` to achieve this. The problem is reminiscent of {ref}`examples-misc-compound`.
 
 ```{code-cell} ipython3
+import numpy as np
+import magpylib as magpy
+
 class Monopole(magpy.misc.CustomSource):
     """Magnetic Monopole class
 
     Parameters
     ----------
     charge: float
         Monopole charge in units of T·m²
@@ -134,15 +144,15 @@
 
     def __init__(self, charge, **kwargs):
         super().__init__(**kwargs)  # hand over style kwargs
         self._charge = charge
 
         # Add spherical 3d model
         trace_pole = magpy.graphics.model3d.make_Ellipsoid(
-            dimension=np.array([3, 3, 3]) * 1e-4,
+            dimension=np.array([.3, .3, .3]),
         )
         self.style.model3d.showdefault = False
         self.style.model3d.add_trace(trace_pole)
 
         # Add monopole field_func
         self._update()
 
@@ -172,97 +182,71 @@
 
     @charge.setter
     def charge(self, input):
         """Set charge"""
         self._charge = input
         self._update()
 
-
 # Use new class
-mono = Monopole(charge=1e-6)
-print(mono.getB((0.001, 0, 0)))
+mono = Monopole(charge=1)
+print(mono.getB((1, 0, 0)))
 
-# Make use of new property
-mono.charge = -1e-6
-print(mono.getB((0.001, 0, 0)))
+# Change property charge of object
+mono.charge = -1
+print(mono.getB((1, 0, 0)))
 ```
 
-The new class seamlessly integrates into the Magpylib interface as we show in the following example where we have a look at the Quadrupole field
+The new class seamlessly integrates into the Magpylib interface as we show in the following example where we have a look at the Quadrupole field.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 import matplotlib.pyplot as plt
 
 # Create a quadrupole from four monopoles
-mono1 = Monopole(charge=1e-6, style_color="r", position=(0.001, 0, 0))
-mono2 = Monopole(charge=1e-6, style_color="r", position=(-0.001, 0, 0))
-mono3 = Monopole(charge=-1e-6, style_color="b", position=(0, 0, 0.001))
-mono4 = Monopole(charge=-1e-6, style_color="b", position=(0, 0, -0.001))
+mono1 = Monopole(charge=1, style_color="r", position=(1, 0, 0))
+mono2 = Monopole(charge=1, style_color="r", position=(-1, 0, 0))
+mono3 = Monopole(charge=-1, style_color="b", position=(0, 0, 1))
+mono4 = Monopole(charge=-1, style_color="b", position=(0, 0, -1))
 qpole = magpy.Collection(mono1, mono2, mono3, mono4)
 
 # Matplotlib figure with 3d and 2d axis
-fig = plt.figure(figsize=(12, 5))
-ax1 = fig.add_subplot(
-    121,
-    projection="3d",
-    azim=-80,
-    elev=15,
-)
-ax2 = fig.add_subplot(
-    122,
-)
+fig = plt.figure(figsize=(10, 5))
+ax1 = fig.add_subplot(121, projection="3d", azim=-80, elev=15)
+ax2 = fig.add_subplot(122)
 
 # Show 3D model in ax1
-magpy.show(*qpole, canvas=ax1)
+magpy.show(*qpole, canvas=ax1, style_legend_show=False)
 
 # Compute B-field on xz-grid and display in ax2
-ts = np.linspace(-3, 3, 30)
-grid = np.array([[(x / 1000, 0, z / 1000) for x in ts] for z in ts])
+grid = np.mgrid[-2:2:100j, 0:0:1j, -2:2:100j].T[:,0]
+X, _, Z = np.moveaxis(grid, 2, 0)
+
 B = qpole.getB(grid)
+Bx, _, Bz = np.moveaxis(B, 2, 0)
+scale = np.linalg.norm(B, axis=2)**.3
 
-scale = np.linalg.norm(B, axis=2)
-cp = ax2.contourf(
-    grid[:, :, 0],
-    grid[:, :, 2],
-    np.log(scale),
-    levels=100,
-    cmap="rainbow",
-)
-ax2.streamplot(
-    grid[:, :, 0],
-    grid[:, :, 2],
-    B[:, :, 0],
-    B[:, :, 2],
-    density=2,
-    color="k",
-    linewidth=scale**0.3,
-)
+cp = ax2.contourf(X, Z, np.log(scale), levels=100, cmap="rainbow")
+ax2.streamplot(X, Z, Bx, Bz, density=2, color="k", linewidth=scale)
 
 # Display pole position in ax2
-pole_pos = np.array([mono.position for mono in qpole])
-ax2.plot(
-    pole_pos[:, 0],
-    pole_pos[:, 2],
-    marker="o",
-    ms=10,
-    mfc="k",
-    mec="w",
-    ls="",
-)
+ppos = np.array([mono.position for mono in qpole])
+ax2.plot(ppos[:, 0], ppos[:, 2], marker="o", ms=10, mfc="k", mec="w", ls="")
 
 # Figure styling
 ax1.set(
     title="3D model",
     xlabel="x-position (m)",
     ylabel="y-position (m)",
     zlabel="z-position (m)",
 )
 ax2.set(
     title="Quadrupole field",
     xlabel="x-position (m)",
     ylabel="z-position (m)",
     aspect=1,
 )
-fig.colorbar(cp, label="[$charge/m^2$]", ax=ax2)
+fig.colorbar(cp, ax=ax2)
 
 plt.tight_layout()
 plt.show()
 ```
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_field_computation.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_field_computation.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-tutorial-field-computation)=
+(examples-tutorial-field-computation)=
 
 # Computing the Field
 
 ## Most basic Example
 
 The v2 slogan was *"The magnetic field is only three lines of code away"*, which is demonstrated by the following most fundamental and self-explanatory example,
 
@@ -28,76 +28,48 @@
 print(B)
 ```
 
 ## Field on a Grid
 
 There are four field computation functions: `getB` will compute the B-field in T. `getH` computes the H-field in A/m. `getJ` computes the magnetic polarization in units of T. `getM` computes the magnetization in units of A/m.
 
-All these functions will return the field in the shape of the input. In the following example, BHJM-fields of a diametrically magnetized cylinder magnet are computed on a position grid in the symmetry plane, and are then displayed using Matplotlib.
+All these functions will return the field in the shape of the input. In the following example, BHJM-fields of a diametrically magnetized cylinder magnet are computed on a position grid in the symmetry plane and are then displayed using Matplotlib.
 
 ```{code-cell} ipython3
 import matplotlib.pyplot as plt
 import numpy as np
-
+from numpy.linalg import norm
 import magpylib as magpy
 
 fig, [[ax1,ax2], [ax3,ax4]] = plt.subplots(2, 2, figsize=(10, 10))
 
-# Create an observer grid in the xz-symmetry plane
-X, Y = np.mgrid[-50:50:100j, -50:50:100j].transpose((0, 2, 1))
-grid = np.stack([X, Y, np.zeros((100, 100))], axis=2)
+# Create an observer grid in the xy-symmetry plane
+grid = np.mgrid[-50:50:100j, -50:50:100j, 0:0:1j].T[0]
+X, Y, _ = np.moveaxis(grid, 2, 0)
 
 # Compute BHJM-fields of a cylinder magnet on the grid
 cyl = magpy.magnet.Cylinder(polarization=(0.5, 0.5, 0), dimension=(40, 20))
+
 B = cyl.getB(grid)
+Bx, By, _ = np.moveaxis(B, 2, 0)
+
 H = cyl.getH(grid)
+Hx, Hy, _ = np.moveaxis(H, 2, 0)
+
 J = cyl.getJ(grid)
+Jx, Jy, _ = np.moveaxis(J, 2, 0)
+
 M = cyl.getM(grid)
+Mx, My, _ = np.moveaxis(M, 2, 0)
 
 # Display field with Pyplot
-ax1.streamplot(
-    grid[:, :, 0],
-    grid[:, :, 1],
-    B[:, :, 0],
-    B[:, :, 1],
-    density=1.5,
-    color=np.log(np.linalg.norm(B, axis=2)),
-    linewidth=1,
-    cmap="spring_r",
-)
-ax2.streamplot(
-    grid[:, :, 0],
-    grid[:, :, 1],
-    H[:, :, 0],
-    H[:, :, 1],
-    density=1.5,
-    color=np.log(np.linalg.norm(H, axis=2)),
-    linewidth=1,
-    cmap="winter_r",
-)
-ax3.streamplot(
-    grid[:, :, 0],
-    grid[:, :, 1],
-    J[:, :, 0],
-    J[:, :, 1],
-    density=1.5,
-    color=np.linalg.norm(J, axis=2),
-    linewidth=1,
-    cmap="summer_r",
-)
-ax4.streamplot(
-    grid[:, :, 0],
-    grid[:, :, 1],
-    M[:, :, 0],
-    M[:, :, 1],
-    density=1.5,
-    color=np.linalg.norm(M, axis=2),
-    linewidth=1,
-    cmap="autumn_r",
-)
+ax1.streamplot(X, Y, Bx, By, color=np.log(norm(B, axis=2)), cmap="spring_r")
+ax2.streamplot(X, Y, Hx, Hy, color=np.log(norm(H, axis=2)), cmap="winter_r")
+ax3.streamplot(X, Y, Jx, Jy, color=norm(J, axis=2), cmap="summer_r")
+ax4.streamplot(X, Y, Mx, My, color=norm(M, axis=2), cmap="autumn_r")
 
 ax1.set_title("B-Field")
 ax2.set_title("H-Field")
 ax3.set_title("J-Field")
 ax4.set_title("M-Field")
 
 for ax in [ax1,ax2,ax3,ax4]:
@@ -112,25 +84,24 @@
     ts = np.linspace(0, 2 * np.pi, 50)
     ax.plot(20 * np.sin(ts), 20 * np.cos(ts), "k--")
 
 plt.tight_layout()
 plt.show()
 ```
 
-(gallery-tutorial-field-computation-sensors)=
+(examples-tutorial-field-computation-sensors)=
 
 ## Using Sensors
 
 The `Sensor` class enables relative positioning of observer grids in the global coordinate system. The observer grid is stored in the `pixel` parameter of the sensor object which is `(0,0,0)` by default (sensor position = observer position).
 
 The following example shows a moving and rotating sensor with two pixels. At the same time, the source objects are moving to demonstrate the versatility of the field computation.
 
 ```{code-cell} ipython3
 import numpy as np
-
 import magpylib as magpy
 
 # Reset defaults set in previous example
 magpy.defaults.reset()
 
 
 # Define sensor with path
@@ -152,15 +123,15 @@
 with magpy.show_context(sensor, coll, animation=True, backend="plotly"):
     magpy.show(col=1)
     magpy.show(output="Bx", col=2, pixel_agg=None)
 ```
 
 ## Multiple Inputs
 
-When `getBHJM` receive multiple inputs for sources and observers they will compute all possible combinations. It is still beneficial to call the field computation only a single time, because similar sources will be grouped and the computation will be vectorized automatically.
+When `getBHJM` receive multiple inputs for sources and observers they will compute all possible combinations. It is still beneficial to call the field computation only a single time, because similar sources will be grouped, and the computation will be vectorized automatically.
 
 ```{code-cell} ipython3
 import magpylib as magpy
 
 # Three sources
 cube1 = magpy.magnet.Cuboid(polarization=(0, 0, 1), dimension=(0.1, 0.1, 0.1))
 cube2 = cube1.copy()
@@ -177,26 +148,27 @@
 # The result includes all combinations
 B.shape
 ```
 
 Select the second cube (first index), the first sensor (second index), pixel 3-4 (index three and four) and the Bz-component of the field (index five)
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 B[1, 0, 2, 3, 2]
 ```
 
 A path will add another index. Every higher pixel dimension will add another index as well.
 
 ## Field as Pandas Dataframe
 
-Instead of a Numpy `ndarray`, the field computation can also return a [pandas](https://pandas.pydata.org/).[dataframe](https://pandas.pydata.org/docs/user_guide/dsintro.html#dataframe) using the `output='dataframe'` kwarg.
+Instead of a NumPy `ndarray`, the field computation can also return a [pandas](https://pandas.pydata.org/).[dataframe](https://pandas.pydata.org/docs/user_guide/dsintro.html#dataframe) using the `output='dataframe'` kwarg.
 
 ```{code-cell} ipython3
 import numpy as np
-
 import magpylib as magpy
 
 cube = magpy.magnet.Cuboid(
     polarization=(0, 0, 1), dimension=(0.01, 0.01, 0.01), style_label="cube"
 )
 loop = magpy.current.Circle(
     current=200,
@@ -218,46 +190,47 @@
 
 B
 ```
 
 Plotting libraries such as [plotly](https://plotly.com/python/plotly-express/) or [seaborn](https://seaborn.pydata.org/introduction.html) can take advantage of this feature, as they can deal with `dataframes` directly.
 
 ```{code-cell} ipython3
+# Continuation from above - ensure previous code is executed
+
 import plotly.express as px
 
 fig = px.line(
     B,
     x="path",
     y="Bx",
     color="pixel",
     line_group="source",
     facet_col="source",
     symbol="sensor",
 )
 fig.show()
 ```
 
-(gallery-tutorial-field-computation-functional-interface)=
+(examples-tutorial-field-computation-functional-interface)=
 
 ## Functional Interface
 
-All above computations demonstrate the convenient object oriented interface of Magpylib. However, there are instances when it is better to work with the functional interface instead.
+All above computations demonstrate the convenient object-oriented interface of Magpylib. However, there are instances when it is better to work with the functional interface instead.
 
 1. Reduce overhead of Python objects
 2. Complex computation instances
 
 In the following example we show how complex instances are computed using the functional interface.
 
 ```{important}
-The functional interface will only outperform the object oriented interface if you use numpy operations for input array creation, such as `tile`, `repeat`, `reshape`, ... !
+The functional interface will only outperform the object oriented interface if you use NumPy operations for input array creation, such as `tile`, `repeat`, `reshape`, ... !
 ```
 
 ```{code-cell} ipython3
 import numpy as np
-
 import magpylib as magpy
 
 # Two different magnet dimensions
 dim1 = (0.02, 0.04, 0.04)
 dim2 = (0.04, 0.02, 0.02)
 DIM = np.vstack(
     (
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_modelling_magnets.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_modelling_magnets.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,76 +1,72 @@
----
-orphan: true
----
-
-(gallery-tutorial-modelling-magnets)=
+(examples-tutorial-modelling-magnets)=
 
 # Modelling a real magnet
 
-Whenever you wish to compare Magpylib simulations with experimental data obtained using a real permanent magnet, you might wonder how to properly set up a Magpylib magnet object to reflect the physical permanent magnet in question. The goal of this tutorial is explaining how to extract this information from respective datasheets, to provide better understanding of permanent magnets, and show how to align Magpylib simulations with experimental measurements.
+Whenever you wish to compare Magpylib simulations with experimental data obtained using a real permanent magnet, you might wonder how to properly set up a Magpylib magnet object to reflect the physical permanent magnet in question. The goal of this tutorial is to explain how to extract this information from respective datasheets, to provide better understanding of permanent magnets, and show how to align Magpylib simulations with experimental measurements.
 
 This tutorial was supported by [BOMATEC](https://www.bomatec.com/de) by providing excellent data sheets and by supplying magnets for the experimental demonstration below.
 
 ## Short summary
 
-In a magnet data sheet you should find B-H curves and J-H curves. These curves coincide at H=0, which gives the intrinsic material remanence $B_r$. As a result of material response and self-interaction, the magnet "demagnetizes" itself so that the mean magnetic polarization of a real magnet is always below the remanence. How much below depends strongly on the shape of the magnet, and is expressed in the data sheet through the permeance coefficient lines (grey lines). The numbers at the end indicate the typical magnet length to diameter ratio (L/D).
+In a magnet data sheet, you should find B-H curves and J-H curves. These curves coincide at H=0, which gives the intrinsic material remanence $B_r$. As a result of material response and self-interaction, the magnet "demagnetizes" itself so that the mean magnetic polarization of a real magnet is always below the remanence. How much below depends strongly on the shape of the magnet and is expressed in the data sheet through the permeance coefficient lines (grey lines). The numbers at the end indicate the typical magnet length to diameter ratio (L/D).
 
 To obtain the correct magnetic polarization of a magnet from the data sheet, one must find the crossing between B-H curve and respective permeance coefficient line. This gives the "working point" which corresponds to the mean demagnetizing H-field inside the magnet. The correct polarization to use in the Magpylib simulation is the J-value at the working point which can be read off from the J-H curve.
 
-![data sheet snippet](../../_static/images/gallery_tutorial_magnet_datasheet2.png)
+![data sheet snippet](../../../_static/images/examples_tutorial_magnet_datasheet2.png)
 
 The following sections provide further explanation on the matter.
 
 ## Hysteresis loop
 
-If you've worked with magnetism, chances are very high that you have seen a magnetic hysteresis loop. Hysteresis loops describe the connection between the **mean values** of an externally applied H-field and the resulting B-field, polarization J or magnetization M **within a defined volume**. This connection depends strongly on size and shape of this volume and what is inside and what is outside.
+If you've worked with magnetism, chances are very high that you have seen a magnetic hysteresis loop. Hysteresis loops describe the connection between the **mean values** of an externally applied H-field and the resulting B-field, polarization J or magnetization M **within a defined volume**. This connection depends strongly on the size and shape of this volume and what is inside and what is outside.
 
 The B-H curve is called the "normal loop", while J-H and M-H curves are called "intrinsic loops". Hereon we only make use of the J-H loops, but the discussion is similar for M-H. Normal and intrinsic loops are connected via $B = \mu_0 H + J$. In free space the B-H connection is just a straight line defined via $B = \mu_0 H$. When the whole space is filled with magnetic material you will see something like this within an arbitrary volume:
 
 ::::{grid} 2
 :::{grid-item}
 :columns: 3
 :::
 :::{grid-item}
 :columns: 6
-![hysteresis loops](../../_static/images/gallery_tutorial_magnet_hysteresis.png)
+![hysteresis loops](../../../_static/images/examples_tutorial_magnet_hysteresis.png)
 :::
 ::::
 
-**1st quadrant**: Initially we have $J=0$ and $H=0$. The magnetic material is not magnetized and no external H-field is applied. When increasing the H-field, the material polarization will follow the "virgin curve" and will increase until it reaches its maximum possible value, the saturation polarization $J_S$. Higher values of $H$ will not affect $J$, while $B$ will keep increasing linearly. Now we are on the "major loop" - we will never return to the virgin curve. After reaching a large H-value we slowly turn the H-field off. As it drops to zero the material will retain its strong polarization at saturation level while the resulting $B$ decreases. At $H = 0$ the B-field then approaches the "remanence field" $B_r$, and its only contribution is $J_S$.
+**1st quadrant**: Initially we have $J=0$ and $H=0$. The magnetic material is not magnetized, and no external H-field is applied. When increasing the H-field, the material polarization will follow the "virgin curve" and will increase until it reaches its maximum possible value, the saturation polarization $J_S$. Higher values of $H$ will not affect $J$, while $B$ will keep increasing linearly. Now we are on the "major loop" - we will never return to the virgin curve. After reaching a large H-value we slowly turn the H-field off. As it drops to zero the material will retain its strong polarization at saturation level while the resulting $B$ decreases. At $H = 0$ the B-field then approaches the "remanence field" $B_r$, and its only contribution is $J_S$.
 
-**2nd quadrant**: Now the H-field becomes negative. Its amplitude increases but it is oriented opposite to the initial direction. Therefore it is also opposite to the magnetic polarization. In the 2nd quadrant we are now trying to actively demagnetize the material. This part of the hysteresis loop is often referred to as the "demagnetization curve". With increasing negative H, the B-field continues to become smaller until it reaches zero at the "coercive field" $H_c$. At this point the net B-field inside the volume is zero, however, the material is still magnetized! In the example loop above, the polarization at $H_c$ is still at the $J_S$ level. By increasing the H-field further, a point will be reached where the material will start to demagnetize. This can be seen by the non-linear drop of $J$. The point where $J$ reaches zero is called the "intrinsic coercive field" $H_{ci}$. At this point the net polarization in the observed volume is zero. The material is demagnetized. The intrinsic coercive field is a measure of how well a magnetized material can resist a demagnetizing field. Having large values of $H_{ci}$ is a property of "hard magnets", as they are able to keep their magnetization $J$ even for strong external fields in the opposite direction.
+**2nd quadrant**: Now the H-field becomes negative. Its amplitude increases but it is oriented opposite to the initial direction. Therefore, it is also opposite to the magnetic polarization. In the 2nd quadrant we are now trying to actively demagnetize the material. This part of the hysteresis loop is often referred to as the "demagnetization curve". With increasing negative H, the B-field continues to become smaller until it reaches zero at the "coercive field" $H_c$. At this point the net B-field inside the volume is zero, however, the material is still magnetized! In the example loop above, the polarization at $H_c$ is still at the $J_S$ level. By increasing the H-field further, a point will be reached where the material will start to demagnetize. This can be seen by the non-linear drop of $J$. The point where $J$ reaches zero is called the "intrinsic coercive field" $H_{ci}$. At this point the net polarization in the observed volume is zero. The material is demagnetized. The intrinsic coercive field is a measure of how well a magnetized material can resist a demagnetizing field. Having large values of $H_{ci}$ is a property of "hard magnets", as they can keep their magnetization $J$ even for strong external fields in the opposite direction.
 
 **3rd and 4th quadrants**: Moving to the third quadrant the behavior is now mirrored. As $H$ increases past $H_{ci}$, polarization quickly aligns with the external field and the material becomes saturated $J=-J_S$. By turning the field around again, we move through the fourth quadrant to complete the hysteresis loop.
 
 Hysteresis in magnetism as presented here is a macroscopic model that is the result of a complex interplay between dipole and exchange interaction, material texture and resulting domain formation at a microscopic level. Details can be found, for example, in Aharoni's classical textbook "Introduction to the Theory of Ferromagnetism".
 
 ## The demagnetizing field
 
 If in an application the applied external H-field is zero, it seems intuitive to use the remanence $B_r$ for the magnetic polarization in the Magpylib simulation. It is a value that you will find in the data sheet.
 
-![data sheet snippet](../../_static/images/gallery_tutorial_magnet_table.png)
+![data sheet snippet](../../../_static/images/examples_tutorial_magnet_table.png)
 
-However, if considering $J=B_r$, you will quickly see that the experimental results are up to ~30 % below of what you would expect. The reason for this is the self-induced demagnetizing field of the magnet which is generated by the magnetic polarization itself. Just like $J$ generates an H-field on the outside of the magnet, it also generates a H-field inside the magnet, along the opposite direction of the polarization. The H-field outside the magnet is known as the stray field, and the H-field inside the magnet is called the demagnetizing field (as it opposes the magnetic polarization). This is demonstrated by the following figure:
+However, if considering $J=B_r$, you will quickly see that the experimental results are up to ~30 % below of what you would expect. The reason for this is the self-induced demagnetizing field of the magnet which is generated by the magnetic polarization itself. Just like $J$ generates an H-field on the outside of the magnet, it also generates an H-field inside the magnet, along the opposite direction of the polarization. The H-field outside the magnet is known as the stray field, and the H-field inside the magnet is called the demagnetizing field (as it opposes the magnetic polarization). This is demonstrated by the following figure:
 
-![demagnetization field simulation](../../_static/images/gallery_tutorial_magnet_fieldcomparison.png)
+![demagnetization field simulation](../../../_static/images/examples_tutorial_magnet_fieldcomparison.png)
 
-Making use of the [streamplot example](gallery-vis-mpl-streamplot), on the left side we show the cross-section of a Cuboid magnet and its homogeneous polarization. And on the right we see the H-field generated by it. Inside the magnet the generated H-field opposes the polarization. As a result, the polarization of a magnet will not be $B_r$, but instead will be some value of $J$ in the 2nd quadrant of the J-H loop that corresponds to the mean H-field inside the magnet. This H-value is often referred to as the "working point".
+Making use of the [streamplot example](examples-vis-mpl-streamplot), on the left side we show the cross-section of a Cuboid magnet and its homogeneous polarization. And on the right, we see the H-field generated by it. Inside the magnet the generated H-field opposes the polarization. As a result, the polarization of a magnet will not be $B_r$, but instead will be some value of $J$ in the 2nd quadrant of the J-H loop that corresponds to the mean H-field inside the magnet. This H-value is often referred to as the "working point".
 
 ## Finding the correct polarization
 
 As explained above, the hysteresis loop depends strongly on the chosen observation volume geometry, the material inside, and what is outside of the volume. Magnet manufacturers provide such loops (usually only the 2nd quadrant) for their magnets, meaning that the observation volume is the whole magnet with air outside.
 
-To obtain the correct mean polarization of a magnet we only have to compute the mean demagnetizing field (= working point) and read the resulting $J$ off the provided J-H loop. Computing the mean demagnetizing field, however, is not a simple task. In addition to the material response (permeability), it depends strongly on the magnet geometry. Fortunately, the working points can be read off from well written data sheets.
+To obtain the correct mean polarization of a magnet we simply must compute the mean demagnetizing field (= working point) and read the resulting $J$ off the provided J-H loop. Computing the mean demagnetizing field, however, is not a simple task. In addition to the material response (permeability), it depends strongly on the magnet geometry. Fortunately, the working points can be read off from well written data sheets.
 
-![data sheet snippet](../../_static/images/gallery_tutorial_magnet_datasheet.png)
+![data sheet snippet](../../../_static/images/examples_tutorial_magnet_datasheet.png)
 
 This datasheet snippet shows the second quadrant of the B-H and J-H loops, even for two different temperatures. The working point is given by the intersection between the "permeance coefficient" lines (gray) and the B-H curve. The number at the end of these lines indicate the length to diameter ratio (L/D) of the magnet, which is the critical geometric factor. Different lines are for different L/D values, which allows one to select the correct working point for different magnets made from this specific material. Once the working point is found, the correct magnetic polarization, here denoted by $J_W$ (the magnetic polarization at the working point), can be read off. The following figure exemplifies the changes in $J_W$ for different L/D values, considering a cylinder magnet:
 
-![finding the working point](../../_static/images/gallery_tutorial_magnet_LDratio.png)
+![finding the working point](../../../_static/images/examples_tutorial_magnet_LDratio.png)
 
 Permanent magnets with different geometries, such as a parallelepiped shape, will have different behavior in terms of L/D values. Make sure you are reading the data from the correct part number.
 ## Warning
 
 Keep in mind that there are still many reasons why your simulation might not fit well to your experiment. Here are some of the most common problems:
 
 1. Small position errors of less than 100 um can have a large impact on the measurement result. The reference should be the sensitive element inside a sensor package. These elements can be displaced by 10-100 um and even rotated by a few degrees. The sensor might also not be well calibrated.
@@ -84,18 +80,18 @@
 
 ::::{grid} 2
 :::{grid-item}
 :columns: 3
 :::
 :::{grid-item}
 :columns: 6
-![](../../_static/images/gallery_icon_WIP.png)
+![](../../../_static/images/examples_icon_WIP.png)
 :::
 ::::
 
 coming soon:
 1. Magpylib simulation code
 2. Experimental data
 3. Comparison and discussion
 
 **Exterior reference**
-G. Martinek, S. Ruoho and U. Wyss. (2021).*Magnetic Properties of Permanents Magnets & Measuring Techniques* [White paper]. Arnold Magnetic Technologies. https://www.arnoldmagnetics.com/blog/measuring-permanent-magnets-white-paper/
+G. Martinek, S. Ruoho and U. Wyss. (2021). *Magnetic Properties of Permanents Magnets & Measuring Techniques* [White paper]. Arnold Magnetic Technologies. https://www.arnoldmagnetics.com/blog/measuring-permanent-magnets-white-paper/
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_tutorial_paths.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_tutorial_paths.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-tutorial-paths)=
+(examples-tutorial-paths)=
 
 # Working with Paths
 
-The position and orientation attributes are key elements of Magpylib. The documentation section {ref}`docu-position` describes how they work. However, these definitions can seem abstract, but the interface was constructed as intuitive as possible.
+The position and orientation attributes are key elements of Magpylib. The documentation section {ref}`docs-position` describes how they work in detail. Wile these definitions can seem abstract, the interface was constructed as intuitively as possible which is demonstrated in this tutorial.
 
 ```{important}
 Always make use of paths when computing with multiple Magpylib object position and orientation instances. This enables vectorized computation. Avoid Python loops at all costs!
 ```
 
 In this tutorial we show some good practice examples.
 
 ## Assigning Absolute Paths
 
 Absolute object paths are assigned at initialization or through the object properties.
 
 ```{code-cell} ipython3
 import numpy as np
 from scipy.spatial.transform import Rotation as R
-
 import magpylib as magpy
 
 # Create paths
 ts = np.linspace(0, 10, 31)
 pos = np.array([(0.1 * t, 0, 0.1 * np.sin(t)) for t in ts])
 ori = R.from_rotvec(np.array([(0, -0.1 * np.cos(t) * 0.785, 0) for t in ts]))
 
@@ -54,15 +53,14 @@
 ## Relative Paths
 
 `move` and `rotate` input is interpreted relative to the existing path. When the input is scalar the whole existing path is moved.
 
 ```{code-cell} ipython3
 import numpy as np
 from scipy.spatial.transform import Rotation as R
-
 import magpylib as magpy
 
 # Create paths
 ts = np.linspace(0, 10, 21)
 pos = np.array([(0.1 * t, 0, 0.1 * np.sin(t)) for t in ts])
 ori = R.from_rotvec(np.array([(0, -0.1 * np.cos(t) * 0.785, 0) for t in ts]))
 
@@ -81,15 +79,14 @@
 magpy.show(sens1, sens2, sens3)
 ```
 
 When the input is a vector, the path is by default appended.
 
 ```{code-cell} ipython3
 import numpy as np
-
 from magpylib.magnet import Sphere
 
 # Create paths
 x_path = np.linspace((0, 0, 0), (0.1, 0, 0), 10)[1:]
 z_path = np.linspace((0, 0, 0), (0, 0, 0.1), 10)[1:]
 
 # Create sphere object
@@ -101,19 +98,18 @@
 
 # Display paths
 sphere.show()
 ```
 
 ## Merging paths
 
-Complex paths can be created by merging multiple path operations. This is done with vector input for the `move` and `rotate` methods, and choosing values for `start` that will make the paths overlap. In the following example we combine a linear path with a rotation about self (`anchor=None`) until path index 30. Thereon, a second rotation about the origin is applied, creating a spiral.
+Complex paths can be created by merging multiple path operations. This is done with vector input for the `move` and `rotate` methods and choosing values for `start` that will make the paths overlap. In the following example we combine a linear path with a rotation about self (`anchor=None`) until path index 30. Thereon, a second rotation about the origin is applied, creating a spiral.
 
 ```{code-cell} ipython3
 import numpy as np
-
 from magpylib.magnet import Cuboid
 
 # Create cube and set linear path
 cube = Cuboid(polarization=(0, 0, 0.1), dimension=(0.02, 0.02, 0.02))
 cube.position = np.linspace((0, 0, 0), (0.1, 0, 0), 60)
 
 # Apply rotation about self - starting at index 0
@@ -141,27 +137,25 @@
 # Reset path
 sensor.reset_path()
 
 print(sensor.position)
 print(sensor.orientation.as_quat())
 ```
 
-(gallery-tutorial-paths-edge-padding-end-slicing)=
-
+(examples-tutorial-paths-edge-padding-end-slicing)=
 ## Edge-padding and end-slicing
 
 Magpylib will always make sure that object paths are in the right format, i.e., `position` and `orientation` attributes are of the same length. In addition, when objects with different path lengths are combined, e.g., when computing the field, the shorter paths are treated as static beyond their end to make the computation sensible. Internally, Magpylib follows a philosophy of edge-padding and end-slicing when adjusting paths.
 
-The idea behind **edge-padding** is that, whenever path entries beyond the existing path length are needed, the edge-entries of the existing path are returned. This means that the object is considered to be "static" beyond its existing path.
+The idea behind **edge-padding** is that, whenever path entries beyond the existing path length are needed, the edge-entries of the existing path are returned. This means that the object is static beyond its existing path.
 
 In the following example the orientation attribute is padded by its edge value `(0,0,.2)` as the position attribute length is increased.
 
 ```{code-cell} ipython3
 from scipy.spatial.transform import Rotation as R
-
 import magpylib as magpy
 
 sensor = magpy.Sensor(
     position=[(0, 0, 0), (0.01, 0.01, 0.01)],
     orientation=R.from_rotvec([(0, 0, 0.1), (0, 0, 0.2)]),
 )
 sensor.position = [(i / 100, i / 100, i / 100) for i in range(4)]
@@ -181,15 +175,14 @@
 print(B)
 ```
 
 The idea behind **end-slicing** is that, whenever a path is automatically reduced in length, Magpylib will slice to keep the ending of the path. While this occurs rarely, the following example shows how the `orientation` attribute is automatically end-sliced, keeping the values `[(0,0,.3), (0,0,.4)]`, when the `position` attribute is reduced in length:
 
 ```{code-cell} ipython3
 from scipy.spatial.transform import Rotation as R
-
 from magpylib import Sensor
 
 sensor = Sensor(
     position=[(0, 0, 0), (0.01, 0.01, 0.01), (0.02, 0.02, 2), (0.03, 0.03, 0.03)],
     orientation=R.from_rotvec([(0, 0, 0.1), (0, 0, 0.2), (0, 0, 0.3), (0, 0, 0.4)]),
 )
 sensor.position = [(0.01, 0.02, 0.03), (0.02, 0.03, 0.04)]
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_vis_mpl_streamplot.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_vis_mpl_streamplot.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,49 +8,47 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-vis-mpl-streamplot)=
+(examples-vis-mpl-streamplot)=
 
 # Matplotlib Streamplot
 
 ## Example 1: Cuboid Magnet
 
 In this example we show the B-field of a cuboid magnet using Matplotlib streamlines. Streamlines are not magnetic field lines in the sense that the field amplitude cannot be derived from their density. However, Matplotlib streamlines can show the field amplitude via color and line thickness. One must be careful that streamlines can only display two components of the field. In the following example the third field component is always zero - but this is generally not the case.
 
-In the example we make use of the [scaling property](docu-api-scale-invariance). We assume that all length inputs are in units of mm, and that the polarization input is in units of millitesla. The resulting `getB` output will also be in millitesla. One must be careful with scaling - the conversion to H would ofc give units of mA/m.
+In the example we make use of the [scaling property](guide-docs-io-scale-invariance). We assume that all length inputs are in units of mm, and that the polarization input is in units of millitesla. The resulting `getB` output will also be in millitesla. One must be careful with scaling - the conversion to H would ofc give units of mA/m.
 
 ```{code-cell} ipython3
 import matplotlib.pyplot as plt
 import numpy as np
 
 import magpylib as magpy
 
 # Create a Matplotlib figure
 fig, ax = plt.subplots()
 
 # Create an observer grid in the xz-symmetry plane
 ts = np.linspace(-5, 5, 40)
 grid = np.array([[(x, 0, z) for x in ts] for z in ts])
+X, _, Z = np.moveaxis(grid, 2, 0)
 
 # Compute the B-field of a cube magnet on the grid
 cube = magpy.magnet.Cuboid(polarization=(500,0,500), dimension=(2,2,2))
 B = cube.getB(grid)
+Bx, _, Bz = np.moveaxis(B, 2, 0)
 log10_norm_B = np.log10(np.linalg.norm(B, axis=2))
 
 # Display the B-field with streamplot using log10-scaled
 # color function and linewidth
-splt = ax.streamplot(
-    grid[:, :, 0],
-    grid[:, :, 2],
-    B[:, :, 0],
-    B[:, :, 2],
+splt = ax.streamplot(X, Z, Bx, Bz,
     density=1.5,
     color=log10_norm_B,
     linewidth=log10_norm_B,
     cmap="autumn",
 )
 
 # Add colorbar with logarithmic labels
@@ -74,15 +72,15 @@
 )
 
 plt.tight_layout()
 plt.show()
 ```
 
 ```{note}
-Be aware that the above code is not very performant, but quite readable. The following example creates the grid with numpy commands only instead of Python loops, and uses the {ref}`gallery-tutorial-field-computation-functional-interface` for field computation.
+Be aware that the above code is not very performant, but quite readable. The following example creates the grid with NumPy commands only instead of Python loops and uses the {ref}`examples-tutorial-field-computation-functional-interface` for field computation.
 ```
 
 ## Example 2 - Hollow Cylinder Magnet
 
 A nice visualization is achieved by combining `streamplot` with `contourf`. In this example we show the B-field of a hollow Cylinder magnet with diametral polarization in the xy-symmetry plane.
 
 ```{code-cell} ipython3
@@ -91,49 +89,34 @@
 
 import magpylib as magpy
 
 # Create a Matplotlib figure
 fig, ax = plt.subplots()
 
 # Create an observer grid in the xy-symmetry plane - using pure numpy
-X, Y = np.mgrid[-0.05:0.05:100j, -0.05:0.05:100j].transpose((0, 2, 1))
-grid = np.stack([X, Y, np.zeros((100, 100))], axis=2)
+grid = np.mgrid[-.05:.05:100j, -.05:.05:100j, 0:0:1j].T[0]
+X, Y, _ = np.moveaxis(grid, 2, 0)
 
 # Compute magnetic field on grid - using the functional interface
 B = magpy.getB(
     "CylinderSegment",
     observers=grid.reshape(-1, 3),
     dimension=(0.02, 0.03, 0.05, 0, 360),
     polarization=(0.1, 0, 0),
 )
 B = B.reshape(grid.shape)
+Bx, By, _ = np.moveaxis(B, 2, 0)
 normB = np.linalg.norm(B, axis=2)
 
-# combine streamplot with contourf
-cp = ax.contourf(
-    X,
-    Y,
-    normB*1000, #T->mT
-    cmap="rainbow",
-    levels=100,
-    zorder=1,
-)
-splt = ax.streamplot(
-    X,
-    Y,
-    B[:, :, 0],
-    B[:, :, 1],
-    color="k",
-    density=1.5,
-    linewidth=1,
-    zorder=3,
-)
+# Combine streamplot with contourf
+cp = ax.contourf(X, Y, normB, cmap="rainbow", levels=100)
+splt = ax.streamplot(X, Y, Bx, By, color="k", density=1.5, linewidth=1)
 
 # Add colorbar
-fig.colorbar(cp, ax=ax, label="|B| (mT)")
+fig.colorbar(cp, ax=ax, label="|B| (T)")
 
 # Outline magnet boundary
 ts = np.linspace(0, 2 * np.pi, 50)
 ax.plot(.03*np.cos(ts), .03*np.sin(ts), "w-", lw=2, zorder=2)
 ax.plot(.02*np.cos(ts), .02*np.sin(ts), "w-", lw=2, zorder=2)
 
 # Figure styling
```

### Comparing `magpylib-5.0.2/docs/_pages/gallery/gallery_vis_pv_streamlines.md` & `magpylib-5.0.3/docs/_pages/user_guide/examples/examples_vis_pv_streamlines.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 orphan: true
 ---
 
-(gallery-vis-pv-streamlines)=
+(examples-vis-pv-streamlines)=
 
-# Field lines with Pyvista streamlines
+# Pyvista 3D field lines
 
 Pyvista offers field-line computation and visualization in 3D. In addition to the field computation, Magpylib offers magnet visualization that seamlessly integrates into a Pyvista plotting scene.
 
 ```{code-cell} ipython3
 import magpylib as magpy
 import pyvista as pv
```

### Comparing `magpylib-5.0.2/docs/_pages/reso_get_started.md` & `magpylib-5.0.3/docs/_pages/user_guide/guide_start_02_fundamentals.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,23 @@
----
-jupytext:
-  text_representation:
-    extension: .md
-    format_name: myst
-    format_version: 0.13
-    jupytext_version: 1.16.0
-kernelspec:
-  display_name: Python 3
-  language: python
-  name: python3
----
-
-(get-started)=
-
-# Get Started
-
-## Installation and Dependencies
-
-Magpylib supports *Python3.10+* and relies on common scientific computation libraries *Numpy*, *Scipy*, *Matplotlib* and *Plotly*. Optionally, *Pyvista* is recommended as graphical backend.
-
-::::{grid} 1 1 2 2
-:margin: 4 4 0 0
-:gutter: 4
-
-:::{grid-item-card} Install with pip:
-:text-align: center
-:shadow: none
-```console
-pip install magpylib
-```
-:::
-:::{grid-item-card} Install with conda:
-:text-align: center
-:shadow: none
-```console
-conda install -c conda-forge magpylib
-```
-:::
-::::
+(getting-started)=
+# The Magpylib fundamentals
+
+In this section we present the most important Magpylib features, focussing on the intuitive object-oriented interface.
+
+## Basic features
 
-## Magpylib fundamentals
+Learn the Magpylib fundamentals (create magnets, view system, compute field) in 5 minutes. This requires a basic understanding of the Python programming language, the [NumPy array class](https://numpy.org/doc/stable/) and the [Scipy Rotation class](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.transform.Rotation.html).
+
+```{hint}
+Since v5 all Magpylib inputs and ouputs are by default in SI-units. See {ref}`guide-docs-io-scale-invariance` for convenient use.
+```
 
-Learn the Magpylib fundamentals in 5 minutes. This requires a basic understanding of the Python programming language, the [Numpy array class](https://numpy.org/doc/stable/) and the [Scipy Rotation class](https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.transform.Rotation.html).
+### Create sources and observers as Python objects
 
-### Step 1: Create sources and observers as Python objects
+In the object oriented interface sources of the magnetic field (magnets, currents, others) and observers of the magnetic field (sensors) are created as Python objects.
 
 ```python
 import magpylib as magpy
 
 # Create a Cuboid magnet with magnetic polarization
 # of 1 T pointing in x-direction and sides of
 # 1,2 and 3 cm respectively (notice the use of SI units).
@@ -55,15 +25,19 @@
 cube = magpy.magnet.Cuboid(polarization=(1,0,0), dimension=(0.01,0.02,0.03))
 
 # Create a Sensor for measuring the field
 
 sensor = magpy.Sensor()
 ```
 
-### Step2: Manipulate object position and orientation
+Find detailed information on the Magpylib classes [here](docs-classes).
+
+### Position and orientation
+
+All Magpylib objects (sources and observers) have position and orientation in a global Cartesian coordinate system that can be manipulated.
 
 ```python
 # By default, the position of a Magpylib object is
 # (0,0,0) and its orientation is the unit rotation,
 # given by a scipy rotation object.
 
 print(cube.position)                   # -> [0. 0. 0.]
@@ -84,52 +58,65 @@
 sensor.move((-0.01,0,0))
 sensor.rotate_from_angax(angle=-45, axis='z')
 
 print(sensor.position)                            # -> [-0.01  0.    0.  ]
 print(sensor.orientation.as_rotvec(degrees=True)) # -> [ 0.  0. -45.]
 ```
 
-### Step 3: View your system
+Find detailed information on position and orientation attributes and how to manipulate them [here](docs-position).
+
+### 3D view of objects
+
+In-built 3D graphic output helps to see if all Magpylib objects are positioned properly. The magnet polarization is represented by default by a 3-color scheme, the sensor by an axes cross.
 
 ```python
 # Use the `show` function to view your system
 # through Matplotlib, Plotly or Pyvista backends.
 
 magpy.show(cube, sensor, backend='plotly')
 ```
 
-<img src="/_static/images/getting_started_fundamentals1.png" width=50% align="center">
+<img src="../../_static/images/getting_started_fundamentals1.png" width=50% align="center">
+
+Detailed information on the graphical output with `show` is given [here](guide-graphics).
 
-### Step 4: Computing the field
+### Computing the field
+
+The field can be computed at sensor objects, or simply by specifying a position of interest.
 
 ```python
-# Compute the B-field in units of T for some points.
+# Compute the B-field for some positions.
 
 points = [(0,0,-.01), (0,0,0), (0,0,.01)] # in SI Units (m)
 B = magpy.getB(cube, points)
 
 print(B.round(2)) # -> [[ 0.26  0.07  0.08]
-                     # [ 0.28  0.05  0.  ]
-                     # [ 0.26  0.07 -0.08]] # in SI Units (T)
+                  #     [ 0.28  0.05  0.  ]
+                  #     [ 0.26  0.07 -0.08]] # in SI Units (T)
 
-# Compute the H-field in units of A/m at the sensor.
+# Compute the H-field at the sensor.
 
 H = magpy.getH(cube, sensor)
 
 print(H.round()) # -> [51017. 24210.     0.] # in SI Units (A/m)
 ```
 
-```{warning}
+```{hint}
 Magpylib makes use of vectorized computation (massive speedup). This requires that you hand over all field computation instances (multiple objects with multiple positions (=paths)) at the same time to `getB`, `getH`, `getJ` and `getM`. Avoid Python loops at all costs !!!
 ```
 
-## Other important features
+Detailed information on field computation is provided [here](docs-fieldcomp).
+
+## Advanced features
+
+While most things can be achieved with the above, the following features will make your live much easier.
 
-:::{dropdown} Paths
-Magpylib position and orientation attributes can store multiple values that are referred to as paths. The field will automatically be computed for all path positions. Use this to model objects that move to multiple locations.
+### Paths
+
+Magpylib position and orientation attributes can store multiple values that are referred to as paths. The field will automatically be computed for all path positions. Use this feature to model objects that move to multiple locations.
 
 ```python
 import numpy as np
 import magpylib as magpy
 
 # Create magnet
 sphere = magpy.magnet.Sphere(
@@ -146,20 +133,19 @@
                       # [ 0.013  0.     0.001]
                       # [ 0.033  0.     0.026]
                       # [ 0.     0.     0.083]
                       # [-0.033  0.     0.026]
                       # [-0.013  0.     0.001]
                       # [-0.004  0.    -0.001]]
 ```
-:::
-
 
+More information on paths is provided [here](docs-position).
 
-:::{dropdown} Collections
-Magpylib objects can be grouped into Collections. An operation applied to a Collection is applied to every object in it.
+### Collections
+Magpylib objects can be grouped into Collections. An operation applied to a Collection is applied to every object in it. The Collection itself behaves like a single source object.
 
 ```python
 import magpylib as magpy
 
 # Create objects
 obj1 = magpy.Sensor()
 obj2 = magpy.magnet.Cuboid(
@@ -171,20 +157,19 @@
 
 # Manipulate Collection
 coll.move((.001,.002,.003))
 
 print(obj1.position) # -> [0.001 0.002 0.003]
 print(obj2.position) # -> [0.001 0.002 0.003]
 ```
-:::
 
+Collections are dicussed in detail [here](guide-docs-classes-collections).
 
-
-:::{dropdown} Complex Magnet Shapes
-There most convenient way to create a magnet with complex shape is by using the convex hull of a point cloud (= simplest form that includes all given points) and transform it into a triangular surface mesh.
+### Complex Magnet Shapes
+There most convenient way to create a magnet with complex shape is by using the convex hull of a point cloud (= simplest geometric form that includes all given points) and transform it into a triangular surface mesh.
 
 ```python
 import numpy as np
 
 import magpylib as magpy
 
 # Create a Pyramid magnet
@@ -203,52 +188,50 @@
     magnetization=(0, 0, 1e6),
     points=points,
 )
 
 # Display the magnet graphically
 pyramid.show()
 ```
-<img src="../_static/images/getting_started_complex_shapes.png" width=50% align="center">
+<img src="../../_static/images/getting_started_complex_shapes.png" width=50% align="center">
 
-However, there are several other possibilities to create complex magnet shapes. Some can be found in the [gallery](gallery).
-:::
+There are several other possibilities to create complex magnet shapes. Some can be found in the [examples](examples-complex-magnet-shapes).
 
 
-:::{dropdown} Graphic Styles
+### Graphic Styles
 Magpylib offers many ways to customize the graphic output.
 
 ```python
 import magpylib as magpy
 
-# create Cuboid magnet with custom style
+# Create Cuboid magnet with custom style
 cube = magpy.magnet.Cuboid(
     polarization=(0,0,1),
     dimension=(.01,.01,.01),
     style_color='r',
     style_magnetization_mode='arrow'
 )
 
-# create Cylinder magnet with custom style
+# Create Cylinder magnet with custom style
 cyl = magpy.magnet.Cylinder(
     polarization=(0,0,1),
     dimension=(.01,.01),
     position=(.02,0,0),
     style_magnetization_color_mode='bicolor',
     style_magnetization_color_north='m',
     style_magnetization_color_south='c',
 )
 magpy.show(cube, cyl)
 ```
-<img src="../_static/images/getting_started_styles.png" width=50% align="center">
-:::
-
+<img src="../../_static/images/getting_started_styles.png" width=50% align="center">
 
+The many options for graphic styling can be found [here](guide-graphic-styles).
 
-:::{dropdown} Animation
-Object paths can be animated
+### Animation
+Object paths can be animated. For this feature the plotly graphic backend is recommended.
 
 ```python
 import numpy as np
 import magpylib as magpy
 
 
 # Create magnet with path
@@ -260,21 +243,20 @@
     angle=np.linspace(10,360,18),
     axis='x'
 )
 
 # Generate an animation with `show`
 cube.show(animation=True, backend="plotly")
 ```
-<img src="../_static/images/getting_started_animation.png" width=50% align="center">
-:::
-
+<img src="../../_static/images/getting_started_animation.png" width=50% align="center">
 
+Nice animation examples are shown [here](examples-vis-animations), and a detailed discussion is provided [here](guide-graphic-animations).
 
-:::{dropdown} Functional interface
-Magpylib's object oriented interface is convenient to work with but is also slowed down by object initialization and handling. The functional interface bypasses this load and enables field computation for a set of input parameters.
+### Functional interface
+Magpylib's object oriented interface is convenient to work with but is also slowed down by object initialization and handling. The functional interface bypasses this load and enables fast field computation for an arbitrary set of input parameters.
 
 ```python
 import magpylib as magpy
 
 # Compute the magnetic field via the functional interface.
 B = magpy.getB(
     sources="Cuboid",
@@ -283,12 +265,9 @@
     polarization=(0, 0, 1),
 )
 
 print(B.round(3))  # -> [[-0.043  0.     0.014]
                        # [ 0.     0.     0.135]
                        # [ 0.043  0.     0.014]]
 ```
-:::
 
-```{code-cell} ipython3
-
-```
+Details on the functional interface are found [here](docs-field-functional).
```

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_collection.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_collection.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_cuboid.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_cuboid.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_custom.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_custom.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_cylinder.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_cylinder.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_cylindersegment.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_cylindersegment.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_dipole.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_dipole.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_global_local.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_global_local.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_line.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_line.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_loop.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_loop.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_sensor.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_sensor.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_sphere.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_sphere.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_tetra.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_tetra.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_triangle.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_triangle.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_classes_init_trimesh.png` & `magpylib-5.0.3/docs/_static/images/docu_classes_init_trimesh.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_field_comp_flow.png` & `magpylib-5.0.3/docs/_static/images/docu_field_comp_flow.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_field_superpos_cutout.png` & `magpylib-5.0.3/docs/_static/images/docu_field_superpos_cutout.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_field_superpos_union.png` & `magpylib-5.0.3/docs/_static/images/docu_field_superpos_union.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/docu_position_sketch.png` & `magpylib-5.0.3/docs/_static/images/docu_position_sketch.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/favicons/android-chrome-192x192.png` & `magpylib-5.0.3/docs/_static/images/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/favicons/android-chrome-512x512.png` & `magpylib-5.0.3/docs/_static/images/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/favicons/apple-touch-icon.png` & `magpylib-5.0.3/docs/_static/images/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/favicons/favicon-16x16.png` & `magpylib-5.0.3/docs/_static/images/favicons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/favicons/favicon-32x32.png` & `magpylib-5.0.3/docs/_static/images/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/favicons/favicon.ico` & `magpylib-5.0.3/docs/_static/images/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_WIP.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_WIP.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_app_end_of_shaft.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_app_end_of_shaft.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_app_helmholtz.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_app_helmholtz.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_ext_custom_quadrupole.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_ext_custom_quadrupole.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_misc_compound.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_misc_compound.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_misc_field_interpolation.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_misc_field_interpolation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_convex_hull.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_shapes_convex_hull.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_pyvista.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_shapes_pyvista.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_superpos.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_shapes_superpos.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_shapes_triangle.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_shapes_triangle.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_collection.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_collection.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_custom.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_custom.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_field_computation.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_field_computation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_modelling_magnets.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_modelling_magnets.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_tutorial_paths.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_tutorial_paths.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_viz_animations.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_vis_animations.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_viz_mpl_streamplot.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_vis_mpl_streamplot.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_icon_viz_pv_streamlines.png` & `magpylib-5.0.3/docs/_static/images/examples_icon_vis_pv_streamlines.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_LDratio.png` & `magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_LDratio.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet.png` & `magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_datasheet.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_datasheet2.png` & `magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_datasheet2.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_fieldcomparison.png` & `magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_fieldcomparison.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_hysteresis.png` & `magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_hysteresis.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/gallery_tutorial_magnet_table.png` & `magpylib-5.0.3/docs/_static/images/examples_tutorial_magnet_table.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/getting_started_animation.png` & `magpylib-5.0.3/docs/_static/images/getting_started_animation.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/getting_started_complex_shapes.png` & `magpylib-5.0.3/docs/_static/images/getting_started_complex_shapes.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/getting_started_fundamentals1.png` & `magpylib-5.0.3/docs/_static/images/getting_started_fundamentals1.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/getting_started_styles.png` & `magpylib-5.0.3/docs/_static/images/getting_started_styles.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/index_head.png` & `magpylib-5.0.3/docs/_static/images/index_head.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/magpylib_flag.png` & `magpylib-5.0.3/docs/_static/images/magpylib_flag.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/images/magpylib_logo.png` & `magpylib-5.0.3/docs/_static/images/magpylib_logo.png`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/videos/axis.mp4` & `magpylib-5.0.3/docs/_static/videos/axis.mp4`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/_static/webcode/copybutton.js` & `magpylib-5.0.3/docs/_static/webcode/copybutton.js`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/docs/conf.py` & `magpylib-5.0.3/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import sys
 
 # This is for pyvista
 os.system("/usr/bin/Xvfb :99 -screen 0 1024x768x24 > /dev/null 2>&1 &")
 os.environ["DISPLAY"] = ":99"
 os.environ["PYVISTA_OFF_SCREEN"] = "true"
 os.environ["PYVISTA_USE_IPYVTK"] = "true"
-
 os.environ["MAGPYLIB_MPL_SVG"] = "true"
 
 # Location of Sphinx files
 sys.path.insert(0, os.path.abspath("./../"))  ##Add the folder one level above
 os.environ["SPHINX_APIDOC_OPTIONS"] = (
     "members,show-inheritance"  ## Hide undocumented members
 )
@@ -56,15 +55,15 @@
         ]
     )
 
 
 # -- Project information -----------------------------------------------------
 
 project = "Magpylib"
-copyright = "2022, SAL - Silicon Austria Labs"
+copyright = "2019-2024, Magpylib developers, License: BSD 2-clause, Built with Sphinx Pydata-Theme"
 author = "The Magpylib Project <magpylib@gmail.com>"
 
 # The short X.Y version
 version = ""
 # The full version, including alpha/beta/rc tags
 from magpylib import __version__ as release
 
@@ -119,62 +118,86 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_book_theme"
+html_theme = "pydata_sphinx_theme"
 
-html_logo = "./_static/images/magpylib_flag.png"
+html_logo = "./_static/images/magpylib_logo.png"
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 
-# announcement = """
-# <p>⚠️ <b>Upcoming Soon: New Version 5 with breaking changes. We recommended to pin your dependencies to magpylib>=4.5<5 to avoid breaking changes!
-# <a href="https://github.com/magpylib/magpylib/discussions/647">(see details)</a>
-# ⚠️</b></p>
-# """
+# Define the json_url for our version switcher.
+json_url = "https://magpylib.readthedocs.io/en/latest/_static/switcher.json"
+
+# Define the version we use for matching in the version switcher.
+version_match = os.environ.get("READTHEDOCS_VERSION")
+
+# If READTHEDOCS_VERSION doesn't exist, we're not on RTD
+# If it is an integer, we're in a PR build and the version isn't correct.
+# If it's "latest" → change to "dev" (that's what we want the switcher to call it)
+if not version_match or version_match.isdigit() or version_match == "latest":
+    # For local development, infer the version to match from the package.
+    if "dev" in release or "rc" in release:
+        version_match = "dev"
+        # We want to keep the relative reference if we are in dev mode
+        # but we want the whole url if we are effectively in a released version
+        json_url = "_static/switcher.json"
+    else:
+        version_match = f"{release}"
+elif version_match == "stable":
+    version_match = f"{release}"
+
+
 html_theme_options = {
     # "announcement": announcement,
-    "repository_url": "https://github.com/magpylib/magpylib",
-    "path_to_docs": "docs/",
-    "repository_branch": release,
-    "use_repository_button": True,
-    "use_download_button": True,
-    "use_source_button": True,
-    "use_edit_page_button": True,
-    "use_issues_button": True,
-    "launch_buttons": {
-        "binderhub_url": "https://mybinder.org",
-        "thebe": True,
-        "notebook_interface": "jupyterlab",
+    "logo": {
+        "text": "Magpylib",
+        "image_dark": "./_static/images/magpylib_logo.png",
+    },
+    "header_links_before_dropdown": 4,
+    "show_version_warning_banner": True,
+    "navbar_align": "content",  # [left, content, right] For testing that the navbar items align properly
+    "navbar_center": ["navbar-nav"],
+    "navbar_persistent": ["version-switcher"],
+    "switcher": {
+        "json_url": json_url,
+        "version_match": version_match,
     },
+    "check_switcher": True,
     "icon_links": [
         {
             "name": "Github",
             "url": "https://github.com/magpylib/magpylib",
             "icon": "https://img.shields.io/github/stars/magpylib/magpylib?style=social",
             "type": "url",
         },
-        {
-            "name": "PyPI",
-            "url": "https://pypi.org/project/magpylib/",
-            "icon": "https://img.shields.io/pypi/v/magpylib",
-            "type": "url",
-        },
-        {
-            "name": "Conda",
-            "url": "https://anaconda.org/conda-forge/magpylib",
-            "icon": "https://img.shields.io/conda/vn/conda-forge/magpylib",
-            "type": "url",
-        },
     ],
+    "navigation_with_keys": False,
+    "footer_start": ["copyright"],
+    "footer_end": [],
+    "use_edit_page_button": True,
+    "navigation_depth": 3,
+    "collapse_navigation": False,
+}
+
+# "show_nav_level": 2,  # Show navigation up to the second level
+# "navigation_depth": 4,  # Adjust the depth as needed
+# "collapse_navigation": True,  # Option to collapse navigation sections
+
+html_context = {
+    # "github_url": "https://github.com", # or your GitHub Enterprise site
+    "github_user": "magpylib",
+    "github_repo": "magpylib",
+    "github_version": "main",
+    "doc_path": "docs/",
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["custom.css"]
@@ -183,16 +206,17 @@
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
 # 'searchbox.html']``.
 #
-# html_sidebars = {}
-
+html_sidebars = {
+    "**": ["search-field.html", "sidebar-nav-bs.html", "sidebar-ethical-ads.html"],
+}
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "magpylibdoc"
 
 
@@ -329,11 +353,12 @@
 #     "doc_module": "pyvista",
 #     "image_scrapers": ("pyvista", "matplotlib"),
 # }
 
 # import pyvista
 # pyvista.BUILDING_GALLERY = True
 
-html_last_updated_fmt = ""
-html_show_copyright = False
-html_show_sphinx = False
-show_authors = False
+# html_last_updated_fmt = ""
+# html_show_copyright = False
+# html_show_sphinx = False
+# show_authors = False
+# html_show_sourcelink = False
```

### Comparing `magpylib-5.0.2/docs/make.bat` & `magpylib-5.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/__init__.py` & `magpylib-5.0.3/magpylib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 The original software publication (version 2):
 
 https://www.sciencedirect.com/science/article/pii/S2352711020300170
 
 """
 # module level dunders
-__version__ = "5.0.2"
+__version__ = "5.0.3"
 __author__ = "Michael Ortner & Alexandre Boisselet"
 __credits__ = "The Magpylib community"
 __all__ = [
     "magnet",
     "current",
     "misc",
     "getB",
```

### Comparing `magpylib-5.0.2/magpylib/_src/defaults/defaults_classes.py` & `magpylib-5.0.3/magpylib/_src/defaults/defaults_classes.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/defaults/defaults_utility.py` & `magpylib-5.0.3/magpylib/_src/defaults/defaults_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/defaults/defaults_values.py` & `magpylib-5.0.3/magpylib/_src/defaults/defaults_values.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/backend_matplotlib.py` & `magpylib-5.0.3/magpylib/_src/display/backend_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/backend_plotly.py` & `magpylib-5.0.3/magpylib/_src/display/backend_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/backend_pyvista.py` & `magpylib-5.0.3/magpylib/_src/display/backend_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/display.py` & `magpylib-5.0.3/magpylib/_src/display/display.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/sensor_mesh.py` & `magpylib-5.0.3/magpylib/_src/display/sensor_mesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/traces_base.py` & `magpylib-5.0.3/magpylib/_src/display/traces_base.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/traces_core.py` & `magpylib-5.0.3/magpylib/_src/display/traces_core.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/display/traces_generic.py` & `magpylib-5.0.3/magpylib/_src/display/traces_generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,33 +775,38 @@
             traces_to_resize_dict[obj] = {**params}
             # temporary coordinates to be able to calculate ranges
             x, y, z = obj._position.T
             traces_dict[obj] = [{"x": x, "y": y, "z": z}]
         else:
             traces_dict[obj] = []
             rco_obj = params.pop("row_cols")
-            for rco in rco_obj:
-                params["row"], params["col"], output_typ = rco
-                if output_typ == "model3d":
-                    orig_style = None
-                    try:
-                        # temporary replace style attribute
-                        orig_style = obj.style
-                        obj._style = params.pop("style", None)
+            orig_style = getattr(obj, "_style", None)
+            try:
+                style_temp = params.pop("style", None)
+                for rco in rco_obj:
+                    # temporary replace style attribute
+                    obj._style = style_temp
+                    if len(rco_obj) >= 2 and style_temp:
+                        # deepcopy style only if obj is in multiple subplots.
+                        obj._style = style_temp.copy()
+                    params["row"], params["col"], output_typ = rco
+                    if output_typ == "model3d":
                         out_traces = get_generic_traces(
                             obj,
                             extra_backend=extra_backend,
                             autosize=autosize,
                             **params,
                         )
-                    finally:
-                        obj._style = orig_style
-                    if extra_backend:
-                        extra_backend_traces.extend(out_traces.get(extra_backend, []))
-                    traces_dict[obj].extend(out_traces["generic"])
+                        if extra_backend:
+                            extra_backend_traces.extend(
+                                out_traces.get(extra_backend, [])
+                            )
+                        traces_dict[obj].extend(out_traces["generic"])
+            finally:
+                obj._style = orig_style
     return traces_dict, traces_to_resize_dict, extra_backend_traces
 
 
 def get_frames(
     objs,
     colorsequence=None,
     zoom=1,
```

### Comparing `magpylib-5.0.2/magpylib/_src/display/traces_utility.py` & `magpylib-5.0.3/magpylib/_src/display/traces_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_circle.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_cuboid.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_cylinder_segment.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_cylinder_segment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_dipole.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_polyline.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_sphere.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_tetrahedron.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_triangle.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_BH_triangularmesh.py` & `magpylib-5.0.3/magpylib/_src/fields/field_BH_triangularmesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/field_wrap_BH.py` & `magpylib-5.0.3/magpylib/_src/fields/field_wrap_BH.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/special_cel.py` & `magpylib-5.0.3/magpylib/_src/fields/special_cel.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/fields/special_el3.py` & `magpylib-5.0.3/magpylib/_src/fields/special_el3.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/input_checks.py` & `magpylib-5.0.3/magpylib/_src/input_checks.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseDisplayRepr.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseDisplayRepr.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseExcitations.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseExcitations.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseGeo.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseGeo.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_BaseTransform.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_Collection.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_Collection.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_Sensor.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Circle.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_current_Circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_current_Polyline.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_current_Polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cuboid.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Cylinder.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Sphere.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_magnet_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_CustomSource.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_misc_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Dipole.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_misc_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/obj_classes/class_misc_Triangle.py` & `magpylib-5.0.3/magpylib/_src/obj_classes/class_misc_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/style.py` & `magpylib-5.0.3/magpylib/_src/style.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/_src/utility.py` & `magpylib-5.0.3/magpylib/_src/utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/core/__init__.py` & `magpylib-5.0.3/magpylib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/graphics/model3d/__init__.py` & `magpylib-5.0.3/magpylib/graphics/model3d/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/magpylib/magnet/__init__.py` & `magpylib-5.0.3/magpylib/magnet/__init__.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/pyproject.toml` & `magpylib-5.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,25 +35,26 @@
 ]
 
 [project.optional-dependencies]
 code_style = [
     "pre-commit",
 ]
 docs = [
-    "sphinx==7.2",
+    "pydata-sphinx-theme",
+    "sphinx==7.3",
     "sphinx-design",
     "sphinx-thebe",
     "sphinx-favicon",
     "sphinx-gallery",
     "sphinx-copybutton",
-    "sphinx-book-theme",
     "myst-nb",
     "pandas",
     "numpy-stl",
     "pyvista",
+    "magpylib-material-response",
 ]
 test = [
     "tox>=4.11",
     "pytest>=7.4",
     "pylint>3.0",
     "coverage",
     "pandas",
```

### Comparing `magpylib-5.0.2/tests/test_BHMJ_level.py` & `magpylib-5.0.3/tests/test_BHMJ_level.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_BaseTransform.py` & `magpylib-5.0.3/tests/test_BaseTransform.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_Coumpound_setters.py` & `magpylib-5.0.3/tests/test_Coumpound_setters.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_CustomSource.py` & `magpylib-5.0.3/tests/test_CustomSource.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test__missing_optional_modules.py` & `magpylib-5.0.3/tests/test__missing_optional_modules.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_core_physics_consistency.py` & `magpylib-5.0.3/tests/test_core_physics_consistency.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_default_utils.py` & `magpylib-5.0.3/tests/test_default_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_defaults.py` & `magpylib-5.0.3/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_display_matplotlib.py` & `magpylib-5.0.3/tests/test_display_matplotlib.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_display_plotly.py` & `magpylib-5.0.3/tests/test_display_plotly.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_display_pyvista.py` & `magpylib-5.0.3/tests/test_display_pyvista.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_display_utility.py` & `magpylib-5.0.3/tests/test_display_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_elliptics.py` & `magpylib-5.0.3/tests/test_elliptics.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_exceptions.py` & `magpylib-5.0.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_field_cylinder.py` & `magpylib-5.0.3/tests/test_field_cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_getBH_dict.py` & `magpylib-5.0.3/tests/test_getBH_dict.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_getBH_interfaces.py` & `magpylib-5.0.3/tests/test_getBH_interfaces.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_getBH_level2.py` & `magpylib-5.0.3/tests/test_getBH_level2.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_input_checks.py` & `magpylib-5.0.3/tests/test_input_checks.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_numerical_stability.py` & `magpylib-5.0.3/tests/test_numerical_stability.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_BaseGeo.py` & `magpylib-5.0.3/tests/test_obj_BaseGeo.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_BaseGeo_v4motion.py` & `magpylib-5.0.3/tests/test_obj_BaseGeo_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Circle.py` & `magpylib-5.0.3/tests/test_obj_Circle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Collection.py` & `magpylib-5.0.3/tests/test_obj_Collection.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Collection_child_parent.py` & `magpylib-5.0.3/tests/test_obj_Collection_child_parent.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Collection_v4motion.py` & `magpylib-5.0.3/tests/test_obj_Collection_v4motion.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Cuboid.py` & `magpylib-5.0.3/tests/test_obj_Cuboid.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Cylinder.py` & `magpylib-5.0.3/tests/test_obj_Cylinder.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_CylinderSegment.py` & `magpylib-5.0.3/tests/test_obj_CylinderSegment.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Dipole.py` & `magpylib-5.0.3/tests/test_obj_Dipole.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Polyline.py` & `magpylib-5.0.3/tests/test_obj_Polyline.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Sensor.py` & `magpylib-5.0.3/tests/test_obj_Sensor.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Sphere.py` & `magpylib-5.0.3/tests/test_obj_Sphere.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Tetrahedron.py` & `magpylib-5.0.3/tests/test_obj_Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_Triangle.py` & `magpylib-5.0.3/tests/test_obj_Triangle.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_obj_TriangularMesh.py` & `magpylib-5.0.3/tests/test_obj_TriangularMesh.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_path.py` & `magpylib-5.0.3/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_physics_consistency.py` & `magpylib-5.0.3/tests/test_physics_consistency.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_scaling.py` & `magpylib-5.0.3/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_utility.py` & `magpylib-5.0.3/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/test_vs_mag2.py` & `magpylib-5.0.3/tests/test_vs_mag2.py`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_Collection.p` & `magpylib-5.0.3/tests/testdata/testdata_Collection.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_Collection_setter.npy` & `magpylib-5.0.3/tests/testdata/testdata_Collection_setter.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_Cuboid.p` & `magpylib-5.0.3/tests/testdata/testdata_Cuboid.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_Sphere.p` & `magpylib-5.0.3/tests/testdata/testdata_Sphere.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_compound_setter_cases.npy` & `magpylib-5.0.3/tests/testdata/testdata_compound_setter_cases.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_cy_cases.npy` & `magpylib-5.0.3/tests/testdata/testdata_cy_cases.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_el3.npy` & `magpylib-5.0.3/tests/testdata/testdata_el3.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_el3_angle.npy` & `magpylib-5.0.3/tests/testdata/testdata_el3_angle.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_femDat_cylinder_tile2.npy` & `magpylib-5.0.3/tests/testdata/testdata_femDat_cylinder_tile2.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_field_BH_cuboid.p` & `magpylib-5.0.3/tests/testdata/testdata_field_BH_cuboid.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_field_BH_cylinder.p` & `magpylib-5.0.3/tests/testdata/testdata_field_BH_cylinder.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_full_cyl.npy` & `magpylib-5.0.3/tests/testdata/testdata_full_cyl.npy`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_path_BaseGeo.p` & `magpylib-5.0.3/tests/testdata/testdata_path_BaseGeo.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tests/testdata/testdata_vs_mag2.p` & `magpylib-5.0.3/tests/testdata/testdata_vs_mag2.p`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/tox.ini` & `magpylib-5.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `magpylib-5.0.2/PKG-INFO` & `magpylib-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib
-Version: 5.0.2
+Version: 5.0.3
 Summary: Free Python3 package to compute magnetic fields.
 Keywords: magnetism,physics,analytical,electromagnetic,magnetic-field,B-field
 Author-email: Michael Ortner <magpylib@gmail.com>
 Maintainer-email: Alexandre Boisselet <alexabois+magpylib@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,25 +20,26 @@
 Requires-Dist: scipy>=1.8
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: plotly>=5.16
 Requires-Dist: jupytext ; extra == "binder"
 Requires-Dist: jupyterlab>=3.2 ; extra == "binder"
 Requires-Dist: jupyterlab-myst ; extra == "binder"
 Requires-Dist: pre-commit ; extra == "code_style"
-Requires-Dist: sphinx==7.2 ; extra == "docs"
+Requires-Dist: pydata-sphinx-theme ; extra == "docs"
+Requires-Dist: sphinx==7.3 ; extra == "docs"
 Requires-Dist: sphinx-design ; extra == "docs"
 Requires-Dist: sphinx-thebe ; extra == "docs"
 Requires-Dist: sphinx-favicon ; extra == "docs"
 Requires-Dist: sphinx-gallery ; extra == "docs"
 Requires-Dist: sphinx-copybutton ; extra == "docs"
-Requires-Dist: sphinx-book-theme ; extra == "docs"
 Requires-Dist: myst-nb ; extra == "docs"
 Requires-Dist: pandas ; extra == "docs"
 Requires-Dist: numpy-stl ; extra == "docs"
 Requires-Dist: pyvista ; extra == "docs"
+Requires-Dist: magpylib-material-response ; extra == "docs"
 Requires-Dist: tox>=4.11 ; extra == "test"
 Requires-Dist: pytest>=7.4 ; extra == "test"
 Requires-Dist: pylint>3.0 ; extra == "test"
 Requires-Dist: coverage ; extra == "test"
 Requires-Dist: pandas ; extra == "test"
 Requires-Dist: pyvista ; extra == "test"
 Requires-Dist: ipywidgets ; extra == "test"
@@ -71,15 +72,15 @@
 </a>
 <a href="https://codecov.io/gh/magpylib/magpylib"> <img src="https://codecov.io/gh/magpylib/magpylib/branch/main/graph/badge.svg">
 </a>
 <a href="https://pypi.org/project/magpylib/"> <img src="https://badge.fury.io/py/magpylib.svg" alt="PyPI version" height="18">
 </a>
 <a href="https://anaconda.org/conda-forge/magpylib"> <img src="https://anaconda.org/conda-forge/magpylib/badges/version.svg" alt="Conda Cloud" height="18">
 </a>
-<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.2?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
+<a href="https://mybinder.org/v2/gh/magpylib/magpylib/5.0.3?filepath=docs%2Fexamples"> <img src="https://mybinder.org/badge_logo.svg" alt="MyBinder link" height="18">
 </a>
 <a href="https://github.com/psf/black"> <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black" height="18">
 </a>
 </div>
 
 Magpylib is a Python package for calculating **3D static magnetic fields** of magnets, line currents and other sources. The computation is based on explicit expressions and is therefore **extremely fast**. A **user friendly API** enables convenient positioning of sources and observers.
 
@@ -89,15 +90,15 @@
 ```
 pip install magpylib
 ```
 Install from conda forge using **conda**
 ```
 conda install -c conda-forge magpylib
 ```
-Magpylib supports _Python3.10+_ and relies on common scientific computation libraries _Numpy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
+Magpylib supports _Python3.10+_ and relies on common scientific computation libraries _NumPy_, _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as graphical backend.
 
 # Resources
 
  - Check out our **[Documentation](https://magpylib.readthedocs.io/en/latest)** for detailed information.
  - Please abide by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/CODE_OF_CONDUCT.md)**.
  - Contribute through **[Discussions](https://github.com/magpylib/magpylib/discussions)** and coding by following the **[Contribution Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The Git project **[Issues](https://github.com/magpylib/magpylib/issues)** give an up-to-date list of potential enhancements and planned milestones. Propose new ones.
  - A **[Youtube video](https://www.youtube.com/watch?v=LeUx6cM1vcs)** introduction to Magpylib v4.0.0 within the **[GSC network](https://www.internationalcollaboration.org/).**
@@ -187,12 +188,12 @@
 A valid software citation could be
 
 ```
 @software{magpylib,
     author = {{Michael-Ortner et al.}},
     title = {magpylib},
     url = {https://magpylib.readthedocs.io/en/latest/},
-    version = {5.0.2},
+    version = {5.0.3},
     date = {2023-06-25},
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: magpylib Version: 5.0.2 Summary: Free Python3
+Metadata-Version: 2.1 Name: magpylib Version: 5.0.3 Summary: Free Python3
 package to compute magnetic fields. Keywords:
 magnetism,physics,analytical,electromagnetic,magnetic-field,B-field Author-
 email: Michael Ortner
 gmail.com> Maintainer-email: Alexandre Boisselet
 magpylib@gmail.com> Requires-Python: >=3.10 Description-Content-Type: text/
 markdown Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -10,22 +10,23 @@
 Programming Language :: Python :: 3.12 Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: Education Classifier: Operating System :: OS Independent
 Requires-Dist: numpy>=1.23 Requires-Dist: scipy>=1.8 Requires-Dist:
 matplotlib>=3.6 Requires-Dist: plotly>=5.16 Requires-Dist: jupytext ; extra ==
 "binder" Requires-Dist: jupyterlab>=3.2 ; extra == "binder" Requires-Dist:
 jupyterlab-myst ; extra == "binder" Requires-Dist: pre-commit ; extra ==
-"code_style" Requires-Dist: sphinx==7.2 ; extra == "docs" Requires-Dist:
-sphinx-design ; extra == "docs" Requires-Dist: sphinx-thebe ; extra == "docs"
-Requires-Dist: sphinx-favicon ; extra == "docs" Requires-Dist: sphinx-gallery ;
-extra == "docs" Requires-Dist: sphinx-copybutton ; extra == "docs" Requires-
-Dist: sphinx-book-theme ; extra == "docs" Requires-Dist: myst-nb ; extra ==
-"docs" Requires-Dist: pandas ; extra == "docs" Requires-Dist: numpy-stl ; extra
-== "docs" Requires-Dist: pyvista ; extra == "docs" Requires-Dist: tox>=4.11 ;
-extra == "test" Requires-Dist: pytest>=7.4 ; extra == "test" Requires-Dist:
+"code_style" Requires-Dist: pydata-sphinx-theme ; extra == "docs" Requires-
+Dist: sphinx==7.3 ; extra == "docs" Requires-Dist: sphinx-design ; extra ==
+"docs" Requires-Dist: sphinx-thebe ; extra == "docs" Requires-Dist: sphinx-
+favicon ; extra == "docs" Requires-Dist: sphinx-gallery ; extra == "docs"
+Requires-Dist: sphinx-copybutton ; extra == "docs" Requires-Dist: myst-nb ;
+extra == "docs" Requires-Dist: pandas ; extra == "docs" Requires-Dist: numpy-
+stl ; extra == "docs" Requires-Dist: pyvista ; extra == "docs" Requires-Dist:
+magpylib-material-response ; extra == "docs" Requires-Dist: tox>=4.11 ; extra
+== "test" Requires-Dist: pytest>=7.4 ; extra == "test" Requires-Dist:
 pylint>3.0 ; extra == "test" Requires-Dist: coverage ; extra == "test"
 Requires-Dist: pandas ; extra == "test" Requires-Dist: pyvista ; extra ==
 "test" Requires-Dist: ipywidgets ; extra == "test" Requires-Dist: imageio
 [tifffile, ffmpeg] ; extra == "test" Requires-Dist: jupyterlab ; extra ==
 "test" Project-URL: Bug Tracker, https://github.com/magpylib/magpylib/issues
 Project-URL: Changelog, https://github.com/magpylib/magpylib/blob/master/
 CHANGELOG.md Project-URL: Documentation, https://magpylib.readthedocs.io/en/
@@ -44,15 +45,15 @@
 _[_M_y_B_i_n_d_e_r_ _l_i_n_k_]_[_b_l_a_c_k_]
 Magpylib is a Python package for calculating **3D static magnetic fields** of
 magnets, line currents and other sources. The computation is based on explicit
 expressions and is therefore **extremely fast**. A **user friendly API**
 enables convenient positioning of sources and observers. # Installation Install
 from PyPI using **pip** ``` pip install magpylib ``` Install from conda forge
 using **conda** ``` conda install -c conda-forge magpylib ``` Magpylib supports
-_Python3.10+_ and relies on common scientific computation libraries _Numpy_,
+_Python3.10+_ and relies on common scientific computation libraries _NumPy_,
 _Scipy_, _Matplotlib_ and _Plotly_. Optionally, _Pyvista_ is recommended as
 graphical backend. # Resources - Check out our **[Documentation](https://
 magpylib.readthedocs.io/en/latest)** for detailed information. - Please abide
 by our **[Code of Conduct](https://github.com/magpylib/magpylib/blob/main/
 CODE_OF_CONDUCT.md)**. - Contribute through **[Discussions](https://github.com/
 magpylib/magpylib/discussions)** and coding by following the **[Contribution
 Guide](https://github.com/magpylib/magpylib/blob/main/CONTRIBUTING.md)**. The
@@ -105,9 +106,9 @@
 bibtex entry for the [2020 open-access paper](https://www.sciencedirect.com/
 science/article/pii/S2352711020300170) would be ``` @article
 {ortner2020magpylib, title={Magpylib: A free Python package for magnetic field
 computation}, author={Ortner, Michael and Bandeira, Lucas Gabriel Coliado},
 journal={SoftwareX}, volume={11}, pages={100466}, year={2020}, publisher=
 {Elsevier} } ``` A valid software citation could be ``` @software{magpylib,
 author = {{Michael-Ortner et al.}}, title = {magpylib}, url = {https://
-magpylib.readthedocs.io/en/latest/}, version = {5.0.2}, date = {2023-06-25}, }
+magpylib.readthedocs.io/en/latest/}, version = {5.0.3}, date = {2023-06-25}, }
 ```
```

