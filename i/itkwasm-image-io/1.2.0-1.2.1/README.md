# Comparing `tmp/itkwasm_image_io-1.2.0.tar.gz` & `tmp/itkwasm_image_io-1.2.1.tar.gz`

## Comparing `itkwasm_image_io-1.2.0.tar` & `itkwasm_image_io-1.2.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/docs/conf.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/docs/make.bat
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/docs/_static/favicon.png
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/docs/_static/logo.svg
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/_version.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_read_image.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_read_image_async.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_write_image.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_write_image_async.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_read_image.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_read_image_async.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_write_image.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_write_image_async.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_read_image.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_read_image_async.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_write_image.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_write_image_async.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_read_image.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_read_image_async.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_write_image.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_write_image_async.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_read_image.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_read_image_async.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_write_image.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_write_image_async.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/meta_read_image.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/meta_read_image_async.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/meta_write_image.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/meta_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_write_image_async.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_read_image.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_read_image_async.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_write_image.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_write_image_async.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_read_image.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_read_image_async.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_write_image.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/png_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/png_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/png_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/png_write_image_async.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/read_image.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/read_image_async.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_read_image.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_read_image_async.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_write_image.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_write_image_async.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_read_image.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_read_image_async.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_write_image.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_write_image_async.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_read_image.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_read_image_async.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_write_image.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_write_image_async.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_read_image.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_read_image_async.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_write_image.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_write_image_async.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_read_image.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_read_image_async.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_write_image.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_write_image_async.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/write_image.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/itkwasm_image_io/write_image_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/common.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/fixtures.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/test_bio_rad_async.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/test_metaimage_async.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/test_png.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/test_read_write_image.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/tests/test_read_write_image_async.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/.gitignore
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/README.md
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/docs/conf.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/docs/_static/favicon.png
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/docs/_static/logo.svg
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/_version.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_read_image.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_read_image_async.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_write_image.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_write_image_async.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_read_image.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_read_image_async.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_write_image.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_write_image_async.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_read_image.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_read_image_async.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_write_image.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_write_image_async.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_read_image.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_read_image_async.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_write_image.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_write_image_async.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_read_image.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_read_image_async.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_write_image.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_write_image_async.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/meta_read_image.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/meta_read_image_async.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/meta_write_image.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/meta_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_write_image_async.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_read_image.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_read_image_async.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_write_image.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_write_image_async.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_read_image.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_read_image_async.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_write_image.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/png_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/png_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/png_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/png_write_image_async.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/read_image.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/read_image_async.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_read_image.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_read_image_async.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_write_image.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_write_image_async.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_read_image.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_read_image_async.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_write_image.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_write_image_async.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_read_image.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_read_image_async.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_write_image.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_write_image_async.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_read_image.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_read_image_async.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_write_image.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_write_image_async.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_read_image.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_read_image_async.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_write_image.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_write_image_async.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/write_image.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/itkwasm_image_io/write_image_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/common.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/fixtures.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/test_bio_rad_async.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/test_metaimage_async.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/test_png.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/test_read_write_image.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/tests/test_read_write_image_async.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/.gitignore
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/README.md
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 itkwasm_image_io-1.2.1/PKG-INFO
```

### Comparing `itkwasm_image_io-1.2.0/docs/Makefile` & `itkwasm_image_io-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/docs/conf.py` & `itkwasm_image_io-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/docs/index.md` & `itkwasm_image_io-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/docs/make.bat` & `itkwasm_image_io-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/docs/_static/favicon.png` & `itkwasm_image_io-1.2.1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/docs/_static/logo.svg` & `itkwasm_image_io-1.2.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/__init__.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bio_rad_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bio_rad_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/bmp_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/bmp_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/fdf_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/fdf_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gdcm_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gdcm_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge4_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge4_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge5_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge5_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/ge_adw_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/ge_adw_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/gipl_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/gipl_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/jpeg_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/jpeg_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/lsm_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/lsm_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/meta_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/meta_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/meta_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/meta_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/meta_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/meta_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/meta_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/meta_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mgh_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mgh_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/mrc_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/mrc_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nifti_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nifti_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/nrrd_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/nrrd_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/png_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/png_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/png_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/png_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/png_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/png_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/png_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/png_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/scanco_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/scanco_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/tiff_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/tiff_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/vtk_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/vtk_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_read_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_read_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_read_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_read_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/wasm_zstd_write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/wasm_zstd_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/write_image.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/itkwasm_image_io/write_image_async.py` & `itkwasm_image_io-1.2.1/itkwasm_image_io/write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/tests/fixtures.py` & `itkwasm_image_io-1.2.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/tests/test_bio_rad_async.py` & `itkwasm_image_io-1.2.1/tests/test_bio_rad_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/tests/test_metaimage_async.py` & `itkwasm_image_io-1.2.1/tests/test_metaimage_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/tests/test_png.py` & `itkwasm_image_io-1.2.1/tests/test_png.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/tests/test_read_write_image.py` & `itkwasm_image_io-1.2.1/tests/test_read_write_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/tests/test_read_write_image_async.py` & `itkwasm_image_io-1.2.1/tests/test_read_write_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_image_io-1.2.0/pyproject.toml` & `itkwasm_image_io-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 [tool.hatch.envs.default.scripts]
 test = [
   "hatch build -t wheel ./dist/pyodide/",
   "pytest --dist-dir=./dist/pyodide --rt=chrome",
 ]
 download-pyodide = [
-  "curl -L https://github.com/pyodide/pyodide/releases/download/0.24.1/pyodide-0.24.1.tar.bz2 -o pyodide.tar.bz2",
+  "curl -L https://github.com/pyodide/pyodide/releases/download/0.25.1/pyodide-0.25.1.tar.bz2 -o pyodide.tar.bz2",
   "tar xjf pyodide.tar.bz2",
   "rm -rf dist/pyodide pyodide.tar.bz2",
   "mkdir -p dist",
   "mv pyodide dist",
 ]
 serve = [
   "hatch build -t wheel ./dist/pyodide/",
```

### Comparing `itkwasm_image_io-1.2.0/PKG-INFO` & `itkwasm_image_io-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-image-io
-Version: 1.2.0
+Version: 1.2.1
 Summary: Input and output for scientific and medical image file formats.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

