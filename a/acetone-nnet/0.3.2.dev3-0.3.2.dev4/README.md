# Comparing `tmp/acetone_nnet-0.3.2.dev3.tar.gz` & `tmp/acetone_nnet-0.3.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.3.2.dev3.tar", last modified: Fri May 31 09:16:42 2024, max compression
+gzip compressed data, was "acetone_nnet-0.3.2.dev4.tar", last modified: Mon Jun  3 07:48:32 2024, max compression
```

## Comparing `acetone_nnet-0.3.2.dev3.tar` & `acetone_nnet-0.3.2.dev4.tar`

### file list

```diff
@@ -1,159 +1,163 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.993961 acetone_nnet-0.3.2.dev3/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3.2.dev3/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev3/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev3/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-31 09:16:42.993961 acetone_nnet-0.3.2.dev3/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5749 2024-05-27 09:13:18.000000 acetone_nnet-0.3.2.dev3/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-31 09:16:37.000000 acetone_nnet-0.3.2.dev3/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-31 09:16:42.993961 acetone_nnet-0.3.2.dev3/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.969961 acetone_nnet-0.3.2.dev3/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.973961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1883 2024-05-31 09:04:34.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.974961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2764 2024-05-29 09:10:29.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.975961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1934 2024-05-31 09:04:23.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5245 2024-05-24 08:55:18.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.977961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3826 2024-05-23 14:34:41.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6435 2024-05-24 06:37:23.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.979961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1972 2024-05-24 08:54:29.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7432 2024-05-24 08:55:08.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1958 2024-05-24 08:54:22.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:13.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:37.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7661 2024-05-31 08:46:58.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.980961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8516 2024-05-30 09:14:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4311 2024-05-23 11:45:23.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4833 2024-05-23 09:59:18.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3419 2024-05-24 08:55:24.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-05-23 14:35:13.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7642 2024-05-31 08:13:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/GatherElements.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    11596 2024-05-24 08:54:47.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3574 2024-05-24 08:55:32.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5156 2024-05-23 09:45:10.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.981961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4530 2024-05-24 06:51:11.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.981961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7926 2024-05-24 06:28:37.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.982961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14511 2024-05-23 15:03:15.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6989 2024-05-23 14:48:34.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5660 2024-05-23 14:50:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2799 2024-05-29 11:45:24.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4704 2024-05-31 08:59:25.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Tile.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5504 2024-05-30 13:58:05.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Transpose.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2366 2024-05-31 09:04:09.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29508 2024-05-31 08:13:07.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.982961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1370 2024-05-29 07:00:39.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2644 2024-05-27 09:32:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/debug_keras.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3744 2024-05-27 09:35:47.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/debug_onnx.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4417 2024-05-29 06:27:31.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/debug_tools.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.983961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.983961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18708 2024-05-22 15:28:07.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.983961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14564 2024-05-22 15:27:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.983961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5381 2024-05-29 07:48:10.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.984961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35537 2024-05-31 09:15:31.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-28 14:07:15.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.984961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.985961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.987961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.988961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.989961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.990961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.991961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1140 2024-05-31 07:30:51.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_GatherElements.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      656 2024-05-30 07:17:26.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      539 2024-05-31 08:54:45.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Tile.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      494 2024-05-30 13:58:10.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Transpose.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.991961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-05-29 14:00:27.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.992961 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 09:16:42.992961 acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-31 09:16:42.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7431 2024-05-31 09:16:42.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-31 09:16:42.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-31 09:16:42.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-31 09:16:42.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-31 09:16:42.000000 acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:32.113200 acetone_nnet-0.3.2.dev4/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3.2.dev4/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev4/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev4/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-06-03 07:48:32.113200 acetone_nnet-0.3.2.dev4/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5749 2024-05-27 09:13:18.000000 acetone_nnet-0.3.2.dev4/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-06-03 07:48:26.000000 acetone_nnet-0.3.2.dev4/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-06-03 07:48:32.114200 acetone_nnet-0.3.2.dev4/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.674195 acetone_nnet-0.3.2.dev4/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.690195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1883 2024-05-31 09:04:34.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.691195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2764 2024-05-29 09:10:29.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.691195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1957 2024-06-03 07:23:45.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5245 2024-05-24 08:55:18.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.694195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3826 2024-05-23 14:34:41.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6435 2024-05-24 06:37:23.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.695195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1972 2024-05-24 08:54:29.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7432 2024-05-24 08:55:08.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1958 2024-05-24 08:54:22.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:13.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:37.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7661 2024-05-31 08:46:58.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.697195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8516 2024-05-30 09:14:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4311 2024-05-23 11:45:23.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4833 2024-05-23 09:59:18.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3419 2024-05-24 08:55:24.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-05-23 14:35:13.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7642 2024-05-31 09:35:55.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/GatherElements.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    11596 2024-05-24 08:54:47.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3574 2024-05-24 08:55:32.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5156 2024-05-23 09:45:10.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.698195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4530 2024-05-24 06:51:11.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.699195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7926 2024-05-24 06:28:37.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.699195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Reduce_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8970 2024-06-03 07:30:41.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Reduce_layers/Reduce.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1577 2024-06-03 07:23:17.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Reduce_layers/ReduceSum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1148 2024-06-03 07:23:26.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Reduce_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.700195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14511 2024-05-23 15:03:15.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6989 2024-05-23 14:48:34.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5660 2024-05-23 14:50:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2799 2024-05-29 11:45:24.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4704 2024-05-31 09:50:34.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Tile.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5504 2024-05-30 13:58:05.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Transpose.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2467 2024-06-03 07:23:36.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29639 2024-06-03 06:23:47.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.701195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1370 2024-05-29 07:00:39.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2644 2024-05-27 09:32:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/debug_keras.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3744 2024-05-27 09:35:47.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/debug_onnx.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4417 2024-05-29 06:27:31.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/debug_tools.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.701195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.701195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18708 2024-05-22 15:28:07.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.701195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14564 2024-05-22 15:27:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.701195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5381 2024-05-29 07:48:10.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.702195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    36882 2024-06-03 07:46:25.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-28 14:07:15.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.702195 acetone_nnet-0.3.2.dev4/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.793196 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.921198 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:31.985199 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:32.003199 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:32.018199 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:32.060200 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-05-31 14:02:05.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1140 2024-05-31 07:30:51.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_GatherElements.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      656 2024-05-30 07:17:26.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      540 2024-05-31 09:50:25.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Tile.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      494 2024-05-30 13:58:10.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Transpose.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:32.082200 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-05-29 14:00:27.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:32.094200 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1692 2024-06-03 06:20:27.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-06-03 07:48:32.113200 acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-06-03 07:48:31.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7625 2024-06-03 07:48:31.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-06-03 07:48:31.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-06-03 07:48:31.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-06-03 07:48:31.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-06-03 07:48:31.000000 acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.3.2.dev3/AUTHORS.md` & `acetone_nnet-0.3.2.dev4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/COPYING` & `acetone_nnet-0.3.2.dev4/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/LICENSE` & `acetone_nnet-0.3.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/PKG-INFO` & `acetone_nnet-0.3.2.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3.2.dev3
+Version: 0.3.2.dev4
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.3.2.dev3/README.md` & `acetone_nnet-0.3.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/pyproject.toml` & `acetone_nnet-0.3.2.dev4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.3.2.dev3"
+version = "0.3.2.dev4"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .layers import (
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, 
     Softmax, BatchNormalization, Transpose, GatherElements, Tile,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
+    Reduce, ReduceSum,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
 
 from .activation_functions import (
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip, LeakyReLu
 )
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/GatherElements.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/GatherElements.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Tile.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Tile.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/Transpose.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/Transpose.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,24 @@
 
 from . import Pad_layers
 from .Pad_layers import Pad, Constant_Pad, Edge_pad, Reflect_pad, Wrap_pad
 
 from . import Pooling_layers
 from .Pooling_layers import Pooling2D, AveragePooling2D, MaxPooling2D
 
+from . import Reduce_layers
+from .Reduce_layers import Reduce, ReduceSum
+
 from . import Resize_layers
 from .Resize_layers import Resize, ResizeCubic, ResizeLinear, ResizeNearest
 
 
 __all__ = (
     "Add_Bias", "Concatenate", "Dense", "Dot", "Flatten", "Gather", "Gemm", "InputLayer", "MatMul", 
     "Softmax", "BatchNormalization", "Transpose", "GatherElements", "Tile",
     Broadcast_layers.__all__,
     Conv_layers.__all__,
     Pad_layers.__all__,
     Pooling_layers.__all__,
+    Reduce_layers.__all__,
     Resize_layers.__all__
 )
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 from .. import templates
 
 from ..format_importer.parser import parser
 
 from .layers import (
     Dense, Dot, Softmax, Gather, Gemm, MatMul, Concatenate, Pad, 
-    Broadcast, BatchNormalization, GatherElements,
+    Broadcast, BatchNormalization, GatherElements, Reduce,
     ResizeLinear, ResizeCubic, ResizeNearest, 
     Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pooling2D, MaxPooling2D, AveragePooling2D
 )
 
 class CodeGenerator(ABC):
 
@@ -404,14 +404,17 @@
         
         if any(isinstance(layer, ResizeCubic) for layer in self.layers):
             mustach_hash['is_cubic_interpolation'] = True
             
         if any(isinstance(layer, ResizeLinear) for layer in self.layers):
             mustach_hash['is_linear_interpolation'] = True
         
+        if any(isinstance(layer, Reduce) for layer in self.layers):
+            mustach_hash['is_reduced'] = True
+        
         if self.debug_mode:
             mustach_hash['debug_file'] = self.c_files_directory + "debug_file.txt"
         
         mustach_hash['layers'] = []
         for layer in self.layers:
             layer_hash = {'inference_function':layer.generate_inference_code_layer(), 'path':layer.path, 'size':layer.size}
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/debug_keras.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/debug_keras.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/debug_onnx.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/debug_onnx.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/debug_tools/debug_tools.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/debug_tools/debug_tools.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from ...code_generator.layers import (
     AveragePooling2D, GatherElements, MaxPooling2D,
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Add, Multiply, Subtract, Divide, Maximum, Minimum, Average,
     ResizeCubic, ResizeLinear, ResizeNearest,
+    ReduceSum,
     Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul,
     Add_Bias, BatchNormalization, Transpose, Tile
 )
 
 from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm, LeakyReLu
 
 ###### Utility functions ######
@@ -454,26 +455,55 @@
                      perm = attributs['perm'],
                      activation_function = Linear())
 
 def create_Tile(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
-    dict_input[idx] = node.input
+    dict_input[idx] = node.input[0]
     dict_output[node.output[0]] = idx
-    repeats = list(onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model)))
+    repeats = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))
+    repeats = [int(rep) for rep in repeats]
     if len(repeats) < 4:
         for i in range(len(repeats),4):
             repeats.insert(0,1)
     return Tile(idx = idx,
                 size = size,
                 repeats = repeats,
                 input_shape = input_shape,
                 activation_function = Linear())
 
+def create_ReduceSum(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
+    input_shape = get_shape(node.input[0],model)
+    output_shape = get_shape(node.output[0],model)
+    size = find_size(output_shape)
+    dict_input[idx] = node.input[0]
+    dict_output[node.output[0]] = idx
+    attributs = extract_attribut(node)
+    if model.opset_import[0].version < 13:
+        if 'keepdims' not in attributs:
+            attributs['keepdims'] = 1
+        attributs['noop_with_empty_axes'] = 0
+    else:
+        if 'keepdims' not in attributs:
+            attributs['keepdims'] = 1
+        if 'noop_with_empty_axes' not in attributs:
+            attributs['noop_with_empty_axes'] = 0
+        if len(node.input) == 2:
+            attributs['axes'] = look_for_initializer(node.input[1],model)
+        else:
+            attributs['axes'] = []
+    
+    return ReduceSum(idx = idx,
+                     size = size,
+                     axis = onnx.numpy_helper.to_array(attributs['axes']),
+                     keepdims = attributs['keepdims'],
+                     noop_with_empty_axes = attributs['noop_with_empty_axes'],
+                     input_shape = input_shape,
+                     activation_layers = Linear())
 
 ### Pooling layers ###
 
 #Create a layer MaxPool
 def create_MaxPool(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
@@ -734,14 +764,15 @@
          "Concat":create_Concat,
          "Gather":create_Gather,
          "GatherElements":create_GatherElements,
          "Gemm":create_Gemm,
          "MatMul":create_MatMul,
          "Transpose":create_Transpose,
          "Tile":create_Tile,
+         "ReduceSum":create_ReduceSum,
          "MaxPool":create_MaxPool,
          "AveragePool":create_AveragePool,
          "GlobalAveragePool":create_GlobalAveragePool,
          "Add":create_Add,
          "Mul":create_Mul,
          "Div":create_Div,
          "Sub":create_Sub,
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_GatherElements.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_GatherElements.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/layers/template_Tile.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/layers/template_Tile.c.tpl`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
     // {{name}}_{{idx}}{{comment}}
     for (f = 0; f < {{output_channels}}; f++)
     {
         for (i = 0; i < {{output_height}}; i++)
         {
             for (j = 0; j < {{output_width}}; j++)
             {
-                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f%{{input_channels}}))]
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f%{{input_channels}}))];
             }
         }
     }
     for (k = 0; k < {{size}}; ++k)
     {
         output_{{road}}[k] = {{{activation_function}}};
     }
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 {{/is_linear_interpolation}}
 {{#is_gather}}
     int position;
     {{#indices}}
     int indice_Gather_{{idx}}[{{lenght}}] = {{list}};
     {{/indices}}
 {{/is_gather}}
+{{#is_reduced}}
+    {{data_type}} reduced;
+{{/is_reduced}}
 
 {{{pre_processing}}}
 {{#layers}}
 {{{inference_function}}}
 {{#debug_layer}}
     fprintf(fp, "{{name}} {{idx}} {{to_transpose}} {{channels}} {{height}} {{width}}\n");
     for (k = 0; k < {{size}}; ++k)
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3.2.dev3
+Version: 0.3.2.dev4
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.3.2.dev3/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.3.2.dev4/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
 src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
 src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+src/acetone_nnet/code_generator/layers/Reduce_layers/Reduce.py
+src/acetone_nnet/code_generator/layers/Reduce_layers/ReduceSum.py
+src/acetone_nnet/code_generator/layers/Reduce_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
 src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
 src/acetone_nnet/debug_tools/__init__.py
 src/acetone_nnet/debug_tools/debug_keras.py
```

