# Comparing `tmp/annarchy-4.8.0.2.tar.gz` & `tmp/annarchy-4.8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annarchy-4.8.0.2.tar", last modified: Wed May 29 12:54:17 2024, max compression
+gzip compressed data, was "annarchy-4.8.0.3.tar", last modified: Mon Jun  3 12:33:07 2024, max compression
```

## Comparing `annarchy-4.8.0.2.tar` & `annarchy-4.8.0.3.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.600081 annarchy-4.8.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.564080 annarchy-4.8.0.2/ANNarchy/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.568080 annarchy-4.8.0.2/ANNarchy/core/
--rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/ConnectorMethods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Constant.py
--rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Dendrite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Global.py
--rw-r--r--   0 runner    (1001) docker     (127)    20348 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/IO.py
--rw-r--r--   0 runner    (1001) docker     (127)    38733 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    34060 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)    34285 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Population.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/PopulationView.py
--rw-r--r--   0 runner    (1001) docker     (127)    68627 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Random.py
--rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Synapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.568080 annarchy-4.8.0.2/ANNarchy/cython_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/cython_ext/Connector.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/cython_ext/Connector.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/cython_ext/Coordinates.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/cython_ext/Coordinates.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/cython_ext/Transformations.pyx
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/cython_ext/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/cython_ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.568080 annarchy-4.8.0.2/ANNarchy/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.568080 annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/ReadOut.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.572080 annarchy-4.8.0.2/ANNarchy/extensions/bold/
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/bold/AccProjection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/bold/BoldModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/bold/BoldMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/bold/NormProjection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26705 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/bold/PredefinedModels.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/bold/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.572080 annarchy-4.8.0.2/ANNarchy/extensions/convolution/
--rw-r--r--   0 runner    (1001) docker     (127)    52674 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/Convolve.py
--rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/ConvolveTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/Copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/CopyTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/Pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/PoolingTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/Transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/convolution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.572080 annarchy-4.8.0.2/ANNarchy/extensions/diagonal/
--rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/diagonal/DiagonalProjection.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/diagonal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.572080 annarchy-4.8.0.2/ANNarchy/extensions/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/hybrid/HybridPopulation.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/hybrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.572080 annarchy-4.8.0.2/ANNarchy/extensions/image/
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/image/ImagePopulation.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.572080 annarchy-4.8.0.2/ANNarchy/extensions/tensorboard/
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/tensorboard/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/extensions/tensorboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.576080 annarchy-4.8.0.2/ANNarchy/generator/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/CmdLineArgParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    43837 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/CodeGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    35511 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/MonitorGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.576080 annarchy-4.8.0.2/ANNarchy/generator/Population/
--rw-r--r--   0 runner    (1001) docker     (127)    62308 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/CUDAGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26864 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/CUDATemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/OpenMPGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/OpenMPTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/PopulationGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/SingleThreadGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/SingleThreadTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Population/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.580080 annarchy-4.8.0.2/ANNarchy/generator/Profile/
--rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Profile/CPP11Profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Profile/CUDAProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Profile/PAPIProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Profile/ProfileGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    30855 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Profile/ProfileTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.580080 annarchy-4.8.0.2/ANNarchy/generator/Projection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.580080 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/
--rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/BSR.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/COO.py
--rw-r--r--   0 runner    (1001) docker     (127)    39116 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR_T.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/Dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/Dense_T.py
--rw-r--r--   0 runner    (1001) docker     (127)    15625 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/ELL.py
--rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/ELLR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/HYB.py
--rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/SELL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77871 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDAGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.584080 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/BSR.py
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/COO.py
--rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR_P.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR_T.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/DIA.py
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/Dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/Dense_T.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/ELL.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/ELLR.py
--rw-r--r--   0 runner    (1001) docker     (127)    52044 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/LIL.py
--rw-r--r--   0 runner    (1001) docker     (127)    22029 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/LIL_P.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/SELL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64299 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMPGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    52009 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/ProjectionGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.588081 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/
--rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/BSR.py
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/COO.py
--rw-r--r--   0 runner    (1001) docker     (127)    36733 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/CSR.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/CSR_T.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/DIA.py
--rw-r--r--   0 runner    (1001) docker     (127)    16946 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense_T.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/ELL.py
--rw-r--r--   0 runner    (1001) docker     (127)    16164 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/ELLR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/HYB.py
--rw-r--r--   0 runner    (1001) docker     (127)    45605 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/LIL.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/SELL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59725 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThreadGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Projection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55116 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/PyxGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Sanity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.588081 annarchy-4.8.0.2/ANNarchy/generator/Template/
--rw-r--r--   0 runner    (1001) docker     (127)    34682 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Template/BaseTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Template/GlobalOperationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Template/MakefileTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Template/MonitorTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Template/PyxTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/Utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.592080 annarchy-4.8.0.2/ANNarchy/include/
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/BSRInvMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/BSRMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/BSRMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/COOMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/COOMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/CSRCMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/CSRCMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/CSRCMatrixCUDAT.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22788 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/CSRCMatrixT.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23175 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/CSRMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/CSRMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30929 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/DenseMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/DenseMatrixOffsets.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17710 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/DiaMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/ELLMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/ELLMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31389 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/ELLRMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/ELLRMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/HYBMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/HYBMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/LILInvMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    40266 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/LILMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    25175 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/PartitionedMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26099 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/SELLMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/SELLMatrixCUDA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/Specific.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/VecTransformation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/include/helper_functions.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.596080 annarchy-4.8.0.2/ANNarchy/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/CurrentInjection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/DecodingProjection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/InputArray.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/PoissonPopulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/SpikeSourceArray.py
--rw-r--r--   0 runner    (1001) docker     (127)    32989 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/SpikeTrains.py
--rw-r--r--   0 runner    (1001) docker     (127)    47618 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/TimedArray.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/inputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.596080 annarchy-4.8.0.2/ANNarchy/intern/
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/ConfigManagement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/GlobalObjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/Messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    17369 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/NetworkManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/SpecificPopulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/SpecificProjection.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/intern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.596080 annarchy-4.8.0.2/ANNarchy/models/
--rw-r--r--   0 runner    (1001) docker     (127)    45463 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/models/Neurons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/models/Synapses.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.596080 annarchy-4.8.0.2/ANNarchy/parser/
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/AnalyseNeuron.py
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/AnalyseSynapse.py
--rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/CoupledEquations.py
--rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/Equation.py
--rw-r--r--   0 runner    (1001) docker     (127)    28252 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/Extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/Function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/ITE.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/ParserTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/StringManipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.600081 annarchy-4.8.0.2/ANNarchy/parser/report/
--rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/report/LatexParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/report/LatexReport.py
--rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/report/MarkdownReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/report/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/parser/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.600081 annarchy-4.8.0.2/ANNarchy/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)    26759 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/ANNarchy/thirdparty/randutils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.600081 annarchy-4.8.0.2/ANNarchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-29 12:54:17.000000 annarchy-4.8.0.2/ANNarchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-29 12:54:17.000000 annarchy-4.8.0.2/ANNarchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:54:17.000000 annarchy-4.8.0.2/ANNarchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 12:54:17.000000 annarchy-4.8.0.2/ANNarchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 12:54:17.000000 annarchy-4.8.0.2/ANNarchy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-29 12:54:17.600081 annarchy-4.8.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:54:17.600081 annarchy-4.8.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:54:17.600081 annarchy-4.8.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/tests/test_CUDA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/tests/test_openmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-29 12:54:06.000000 annarchy-4.8.0.2/tests/test_single_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.681027 annarchy-4.8.0.3/ANNarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.685027 annarchy-4.8.0.3/ANNarchy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/ConnectorMethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Dendrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Global.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20348 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/IO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38733 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34060 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34285 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Population.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/PopulationView.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68623 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Synapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.685027 annarchy-4.8.0.3/ANNarchy/cython_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/cython_ext/Connector.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/cython_ext/Connector.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/cython_ext/Coordinates.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/cython_ext/Coordinates.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/cython_ext/Transformations.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/cython_ext/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/cython_ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.689027 annarchy-4.8.0.3/ANNarchy/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.689027 annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/ReadOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.689027 annarchy-4.8.0.3/ANNarchy/extensions/bold/
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/bold/AccProjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/bold/BoldModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/bold/BoldMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/bold/NormProjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26705 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/bold/PredefinedModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/bold/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.689027 annarchy-4.8.0.3/ANNarchy/extensions/convolution/
+-rw-r--r--   0 runner    (1001) docker     (127)    52674 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/Convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/ConvolveTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/CopyTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/Pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/PoolingTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/Transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/convolution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.689027 annarchy-4.8.0.3/ANNarchy/extensions/diagonal/
+-rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/diagonal/DiagonalProjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/diagonal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.693027 annarchy-4.8.0.3/ANNarchy/extensions/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/hybrid/HybridPopulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/hybrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.693027 annarchy-4.8.0.3/ANNarchy/extensions/image/
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/image/ImagePopulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.693027 annarchy-4.8.0.3/ANNarchy/extensions/tensorboard/
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/tensorboard/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/extensions/tensorboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.693027 annarchy-4.8.0.3/ANNarchy/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/CmdLineArgParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43837 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/CodeGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/MonitorGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.697027 annarchy-4.8.0.3/ANNarchy/generator/Population/
+-rw-r--r--   0 runner    (1001) docker     (127)    62308 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/CUDAGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26864 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/CUDATemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/OpenMPGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/OpenMPTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/PopulationGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/SingleThreadGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/SingleThreadTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Population/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.697027 annarchy-4.8.0.3/ANNarchy/generator/Profile/
+-rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Profile/CPP11Profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Profile/CUDAProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Profile/PAPIProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Profile/ProfileGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30855 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Profile/ProfileTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.697027 annarchy-4.8.0.3/ANNarchy/generator/Projection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.701027 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/BSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/COO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39116 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23959 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/Dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/Dense_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15625 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/ELL.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/ELLR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/HYB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/SELL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77869 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDAGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.705027 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/BSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/COO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36651 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/DIA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/Dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/ELL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/ELLR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52044 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/LIL.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22029 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/SELL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64299 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMPGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52009 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/ProjectionGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.705027 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/
+-rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/BSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/COO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36733 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/CSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/DIA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16946 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/ELL.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16164 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/ELLR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/HYB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45605 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/LIL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/SELL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59721 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThreadGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Projection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55116 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/PyxGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.709027 annarchy-4.8.0.3/ANNarchy/generator/Template/
+-rw-r--r--   0 runner    (1001) docker     (127)    34682 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Template/BaseTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Template/GlobalOperationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Template/MakefileTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Template/MonitorTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Template/PyxTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.713027 annarchy-4.8.0.3/ANNarchy/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/BSRInvMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/BSRMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/BSRMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/COOMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/COOMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/CSRCMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/CSRCMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/CSRCMatrixCUDAT.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22788 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/CSRCMatrixT.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23175 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/CSRMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/CSRMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30929 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/DenseMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/DenseMatrixOffsets.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17710 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/DiaMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/ELLMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/ELLMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31389 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/ELLRMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/ELLRMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/HYBMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/HYBMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/LILInvMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    40266 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/LILMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25175 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/PartitionedMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26099 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/SELLMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/SELLMatrixCUDA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/Specific.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/VecTransformation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/include/helper_functions.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.717027 annarchy-4.8.0.3/ANNarchy/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/CurrentInjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/DecodingProjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/InputArray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/PoissonPopulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/SpikeSourceArray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32987 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/SpikeTrains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47618 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/TimedArray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/inputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.717027 annarchy-4.8.0.3/ANNarchy/intern/
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/ConfigManagement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/GlobalObjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/Messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17369 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/NetworkManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/SpecificPopulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/SpecificProjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/intern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.717027 annarchy-4.8.0.3/ANNarchy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    45463 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/models/Neurons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/models/Synapses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/ANNarchy/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/AnalyseNeuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20763 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/AnalyseSynapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/CoupledEquations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/Equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28252 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/Extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/ITE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/ParserTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/StringManipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/ANNarchy/parser/report/
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/report/LatexParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/report/LatexReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/report/MarkdownReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/report/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/parser/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/ANNarchy/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)    26759 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/ANNarchy/thirdparty/randutils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/ANNarchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-06-03 12:33:07.000000 annarchy-4.8.0.3/ANNarchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-06-03 12:33:07.000000 annarchy-4.8.0.3/ANNarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:33:07.000000 annarchy-4.8.0.3/ANNarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-03 12:33:07.000000 annarchy-4.8.0.3/ANNarchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 12:33:07.000000 annarchy-4.8.0.3/ANNarchy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:33:07.721027 annarchy-4.8.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/tests/test_CUDA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/tests/test_openmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-06-03 12:32:58.000000 annarchy-4.8.0.3/tests/test_single_thread.py
```

### Comparing `annarchy-4.8.0.2/ANNarchy/__init__.py` & `annarchy-4.8.0.3/ANNarchy/__init__.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/ConnectorMethods.py` & `annarchy-4.8.0.3/ANNarchy/core/ConnectorMethods.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Constant.py` & `annarchy-4.8.0.3/ANNarchy/core/Constant.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Dendrite.py` & `annarchy-4.8.0.3/ANNarchy/core/Dendrite.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Global.py` & `annarchy-4.8.0.3/ANNarchy/core/Global.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/IO.py` & `annarchy-4.8.0.3/ANNarchy/core/IO.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Monitor.py` & `annarchy-4.8.0.3/ANNarchy/core/Monitor.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Network.py` & `annarchy-4.8.0.3/ANNarchy/core/Network.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Neuron.py` & `annarchy-4.8.0.3/ANNarchy/core/Neuron.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Population.py` & `annarchy-4.8.0.3/ANNarchy/core/Population.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/PopulationView.py` & `annarchy-4.8.0.3/ANNarchy/core/PopulationView.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Projection.py` & `annarchy-4.8.0.3/ANNarchy/core/Projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,15 +659,15 @@
 
     def nb_efferent_synapses(self):
         "Number of efferent connections. Intended only for spiking models."
         if self.cyInstance is None:
              Messages._warning("Access 'nb_efferent_synapses()' of a Projection is only valid after compile()")
              return None
         if self.synapse_type.type == "rate":
-            Messages._erroror("Projection.nb_efferent_synapses() is not available for rate-coded projections.")
+            Messages._error("Projection.nb_efferent_synapses() is not available for rate-coded projections.")
 
         return self.cyInstance.nb_efferent_synapses()
 
     @property
     def post_ranks(self):
         if self.cyInstance is None:
              Messages._warning("Access 'post_ranks' attribute of a Projection is only valid after compile()")
@@ -856,15 +856,15 @@
 
         # A list is given
         if isinstance(value, list):
             if len(value) == len(self.post_ranks):
                 if attribute in self.synapse_type.description['local']:
                     for idx, n in enumerate(self.post_ranks):
                         if not len(value[idx]) == self.cyInstance.dendrite_size(idx):
-                            Messages._erroror('The post-synaptic neuron ' + str(n) + ' of population ' + str(self.post.id) + ' receives '+ str(self.cyInstance.dendrite_size(idx))+ ' synapses and not ' + str(len(value[idx])) + '.')
+                            Messages._error('The post-synaptic neuron ' + str(n) + ' of population ' + str(self.post.id) + ' receives '+ str(self.cyInstance.dendrite_size(idx))+ ' synapses and not ' + str(len(value[idx])) + '.')
                         self.cyInstance.set_local_attribute_row(attribute, idx, value[idx], ctype)
                 elif attribute in self.synapse_type.description['semiglobal']:
                     self.cyInstance.set_semiglobal_attribute_all(attribute, value, ctype)
                 else:
                     Messages._error('The parameter', attribute, 'is global to the population, cannot assign a list.')
             else:
                 Messages._error('The projection has', self.size, 'post-synaptic neurons, the list must have the same size.')
```

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Random.py` & `annarchy-4.8.0.3/ANNarchy/core/Random.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Simulate.py` & `annarchy-4.8.0.3/ANNarchy/core/Simulate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Synapse.py` & `annarchy-4.8.0.3/ANNarchy/core/Synapse.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/core/Utils.py` & `annarchy-4.8.0.3/ANNarchy/core/Utils.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/cython_ext/Connector.pxd` & `annarchy-4.8.0.3/ANNarchy/cython_ext/Connector.pxd`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/cython_ext/Connector.pyx` & `annarchy-4.8.0.3/ANNarchy/cython_ext/Connector.pyx`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/cython_ext/Coordinates.pxd` & `annarchy-4.8.0.3/ANNarchy/cython_ext/Coordinates.pxd`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/cython_ext/Coordinates.pyx` & `annarchy-4.8.0.3/ANNarchy/cython_ext/Coordinates.pyx`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/cython_ext/Transformations.pyx` & `annarchy-4.8.0.3/ANNarchy/cython_ext/Transformations.pyx`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py` & `annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py` & `annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/ann_to_snn_conversion/ReadOut.py` & `annarchy-4.8.0.3/ANNarchy/extensions/ann_to_snn_conversion/ReadOut.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/bold/AccProjection.py` & `annarchy-4.8.0.3/ANNarchy/extensions/bold/AccProjection.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/bold/BoldModel.py` & `annarchy-4.8.0.3/ANNarchy/extensions/bold/BoldModel.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/bold/BoldMonitor.py` & `annarchy-4.8.0.3/ANNarchy/extensions/bold/BoldMonitor.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/bold/NormProjection.py` & `annarchy-4.8.0.3/ANNarchy/extensions/bold/NormProjection.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/bold/PredefinedModels.py` & `annarchy-4.8.0.3/ANNarchy/extensions/bold/PredefinedModels.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/Convolve.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/Convolve.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/ConvolveTemplate.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/ConvolveTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/Copy.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/Copy.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/CopyTemplate.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/CopyTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/Pooling.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/Pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         :param delays: synaptic delay in ms
         """
 
         # process extent
         self.extent_init = extent
         if extent is None:  # compute the extent automatically
             if self.pre.dimension != self.post.dimension:
-                Messages._erroror(
+                Messages._error(
                     'Pooling: If you do not provide the extent parameter, the two populations must have the same number of dimensions.')
 
             extent = list(self.pre.geometry)
             for dim in range(self.pre.dimension):
                 extent[dim] /= self.post.geometry[dim]
                 if self.pre.geometry[dim] != extent[dim] * self.post.geometry[dim]:
                     Messages._error(
```

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/PoolingTemplate.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/PoolingTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/Transpose.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/Transpose.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/Utils.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/Utils.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/convolution/__init__.py` & `annarchy-4.8.0.3/ANNarchy/extensions/convolution/__init__.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/diagonal/DiagonalProjection.py` & `annarchy-4.8.0.3/ANNarchy/extensions/diagonal/DiagonalProjection.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/hybrid/HybridPopulation.py` & `annarchy-4.8.0.3/ANNarchy/extensions/hybrid/HybridPopulation.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/image/ImagePopulation.py` & `annarchy-4.8.0.3/ANNarchy/extensions/image/ImagePopulation.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/extensions/tensorboard/Logger.py` & `annarchy-4.8.0.3/ANNarchy/extensions/tensorboard/Logger.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/CmdLineArgParser.py` & `annarchy-4.8.0.3/ANNarchy/generator/CmdLineArgParser.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/CodeGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/CodeGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Compiler.py` & `annarchy-4.8.0.3/ANNarchy/generator/Compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     # If not in the same folder as python, use the default
     with subprocess.Popen("%(cython)s -V > /dev/null 2> /dev/null" % {'cython': cython}, shell=True) as test:
         if test.wait() != 0:
             cython = shutil.which("cython"+str(py_major))
             if cython is None:
                 cython = shutil.which("cython")
                 if cython is None:
-                    Messages._erroror("Unable to detect the path to cython.")
+                    Messages._error("Unable to detect the path to cython.")
 
     return py_version, py_major, python_include, python_lib, python_libpath, cython
 
 class Compiler(object):
     " Main class to generate C++ code efficiently"
 
     def __init__(self, annarchy_dir, clean, compiler, compiler_flags, add_sources, extra_libs, path_to_json, silent, cuda_config, debug_build,
@@ -348,15 +348,15 @@
                 self.user_config = json.load(rfile)
 
         # Sanity check if the NVCC compiler is available
         if _check_paradigm("cuda"):
             cmd = self.user_config['cuda']['compiler'] + " --version 1> /dev/null"
 
             if os.system(cmd) != 0:
-                Messages._erroror("CUDA is not available on your system. Please check the CUDA installation or the annarchy.json configuration.")
+                Messages._error("CUDA is not available on your system. Please check the CUDA installation or the annarchy.json configuration.")
 
             self.cuda_config['cuda_version'] = check_cuda_version(self.user_config['cuda']['compiler'])
 
     def generate(self):
         "Perform the code generation for the C++ code and create the Makefile."
         if Profiler().enabled or get_global_config('show_time'):
             t0 = time.time()
```

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/MonitorGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/MonitorGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Population/CUDAGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Population/CUDAGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Population/CUDATemplates.py` & `annarchy-4.8.0.3/ANNarchy/generator/Population/CUDATemplates.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Population/OpenMPGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Population/OpenMPGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Population/OpenMPTemplates.py` & `annarchy-4.8.0.3/ANNarchy/generator/Population/OpenMPTemplates.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Population/PopulationGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Population/PopulationGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Population/SingleThreadGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Population/SingleThreadGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Population/SingleThreadTemplates.py` & `annarchy-4.8.0.3/ANNarchy/generator/Population/SingleThreadTemplates.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Profile/CPP11Profile.py` & `annarchy-4.8.0.3/ANNarchy/generator/Profile/CPP11Profile.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Profile/CUDAProfile.py` & `annarchy-4.8.0.3/ANNarchy/generator/Profile/CUDAProfile.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Profile/PAPIProfile.py` & `annarchy-4.8.0.3/ANNarchy/generator/Profile/PAPIProfile.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Profile/ProfileGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Profile/ProfileGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Profile/ProfileTemplate.py` & `annarchy-4.8.0.3/ANNarchy/generator/Profile/ProfileTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/BSR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/BSR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/BaseTemplates.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/COO.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/COO.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR_T.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR_T.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/CSR_Vector.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/Dense.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/Dense.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/Dense_T.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/Dense_T.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/ELL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/ELL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/ELLR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/ELLR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/HYB.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/HYB.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/SELL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/SELL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDA/__init__.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDA/__init__.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/CUDAGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/CUDAGenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1414,15 +1414,15 @@
                 add_args_call += ', pop%(id)s.gpu_%(name)s' % attr_ids
 
         # select code template
         try:
             templates = self._templates['post_event']
 
         except KeyError:
-            raise Messages._erroror("No CUDA code template for post_event ( format =", proj._storage_format, " and order =", proj._storage_order,")")
+            raise Messages._error("No CUDA code template for post_event ( format =", proj._storage_format, " and order =", proj._storage_order,")")
 
         # Fill code templates
         postevent_body = templates['device_kernel'] % {
             'id_proj': proj.id,
             'conn_args': self._templates['conn_header'] % ids,
             'add_args': add_args_header,
             'event_driven': tabify(event_driven_code % ids, 2),
```

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/BSR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/BSR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/COO.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/COO.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR_P.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR_T.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/DIA.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/DIA.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/Dense.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/Dense.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/Dense_T.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/ELL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/ELL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/ELLR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/ELLR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/LIL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/LIL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/LIL_P.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/SELL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/SELL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMP/__init__.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMP/__init__.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/OpenMPGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/OpenMPGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/ProjectionGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/ProjectionGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/BSR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/BSR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/COO.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/COO.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/CSR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/CSR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/CSR_T.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/DIA.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/DIA.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense_PV.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/Dense_T.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/ELL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/ELL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/ELLR.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/ELLR.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/HYB.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/HYB.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/LIL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/LIL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/SELL.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/SELL.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThread/__init__.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThread/__init__.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Projection/SingleThreadGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/Projection/SingleThreadGenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -984,15 +984,15 @@
                 pre_array = "%(pre_prefix)s_delayed_spike[delay-1]" % ids
                 template = self._templates['spiking_sum_fixed_delay']
         else:
             pre_array = "%(pre_prefix)sspiked" % ids
             template = self._templates['spiking_sum_fixed_delay']
 
         if template == None:
-            Messages._erroror("Code generation error: no template available")
+            Messages._error("Code generation error: no template available")
 
         complete_code = ""
 
         # Axonal spike events
         spiked_array_fusion_code = ""
         if proj.synapse_type.pre_axon_spike:
             if proj.synapse_type.description['raw_pre_spike'] == proj.synapse_type.description['raw_axon_spike']:
@@ -1356,15 +1356,15 @@
 
         # Choose the template
         try:
             template = self._templates['update_variables']
 
         except KeyError:
             # either no template code at all, or no 'update_variables' field.
-            Messages._erroror("No synaptic plasticity template found for format = " + proj._storage_format, " and order = " + proj._storage_order)
+            Messages._error("No synaptic plasticity template found for format = " + proj._storage_format, " and order = " + proj._storage_order)
 
         template_ids = deepcopy(self._template_ids) # will be extended at the end of this function
         template_ids.update({
             'global': global_eq % self._template_ids,
             'semiglobal': semiglobal_eq % self._template_ids,
             'local': local_eq % self._template_ids,
         })
```

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/PyxGenerator.py` & `annarchy-4.8.0.3/ANNarchy/generator/PyxGenerator.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Sanity.py` & `annarchy-4.8.0.3/ANNarchy/generator/Sanity.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Template/BaseTemplate.py` & `annarchy-4.8.0.3/ANNarchy/generator/Template/BaseTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Template/GlobalOperationTemplate.py` & `annarchy-4.8.0.3/ANNarchy/generator/Template/GlobalOperationTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Template/MakefileTemplate.py` & `annarchy-4.8.0.3/ANNarchy/generator/Template/MakefileTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Template/MonitorTemplate.py` & `annarchy-4.8.0.3/ANNarchy/generator/Template/MonitorTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Template/PyxTemplate.py` & `annarchy-4.8.0.3/ANNarchy/generator/Template/PyxTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/generator/Utils.py` & `annarchy-4.8.0.3/ANNarchy/generator/Utils.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/BSRInvMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/BSRInvMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/BSRMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/BSRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/BSRMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/BSRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/COOMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/COOMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/COOMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/COOMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/CSRCMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/CSRCMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/CSRCMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/CSRCMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/CSRCMatrixCUDAT.hpp` & `annarchy-4.8.0.3/ANNarchy/include/CSRCMatrixCUDAT.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/CSRCMatrixT.hpp` & `annarchy-4.8.0.3/ANNarchy/include/CSRCMatrixT.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/CSRMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/CSRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/CSRMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/CSRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/DenseMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/DenseMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/DenseMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/DenseMatrixOffsets.hpp` & `annarchy-4.8.0.3/ANNarchy/include/DenseMatrixOffsets.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/DiaMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/DiaMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/ELLMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/ELLMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/ELLMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/ELLMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/ELLRMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/ELLRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/ELLRMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/ELLRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/HYBMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/HYBMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/HYBMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/HYBMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/LILInvMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/LILInvMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/LILMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/LILMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/PartitionedMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/PartitionedMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/SELLMatrix.hpp` & `annarchy-4.8.0.3/ANNarchy/include/SELLMatrix.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/SELLMatrixCUDA.hpp` & `annarchy-4.8.0.3/ANNarchy/include/SELLMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/Specific.hpp` & `annarchy-4.8.0.3/ANNarchy/include/Specific.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/VecTransformation.hpp` & `annarchy-4.8.0.3/ANNarchy/include/VecTransformation.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/include/helper_functions.hpp` & `annarchy-4.8.0.3/ANNarchy/include/helper_functions.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/CurrentInjection.py` & `annarchy-4.8.0.3/ANNarchy/inputs/CurrentInjection.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/DecodingProjection.py` & `annarchy-4.8.0.3/ANNarchy/inputs/DecodingProjection.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.window = window
 
         # Disable openMP post-synaptic matrix split
         self._no_split_matrix = True
 
         # Not on CUDA
         if _check_paradigm('cuda'):
-            Messages._erroror('DecodingProjections are not available on CUDA yet.')
+            Messages._error('DecodingProjections are not available on CUDA yet.')
 
     def _copy(self, pre, post):
         "Returns a copy of the population when creating networks. Internal use only."
         copied_proj = DecodingProjection(pre=pre, post=post, target=self.target, window=self.window, name=self.name, copied=True)
         copied_proj._no_split_matrix = True
         return copied_proj
```

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/InputArray.py` & `annarchy-4.8.0.3/ANNarchy/inputs/InputArray.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/PoissonPopulation.py` & `annarchy-4.8.0.3/ANNarchy/inputs/PoissonPopulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                  rates:float|str=None, 
                  target:str=None, 
                  parameters:str=None, 
                  refractory:float=None, 
                  copied:bool=False):
 
         if rates is None and target is None:
-            Messages._erroror('A PoissonPopulation must define either rates or target.')
+            Messages._error('A PoissonPopulation must define either rates or target.')
 
         self.target = target
         self.parameters = parameters
         self.refractory_init = refractory
         self.rates_init = rates
 
         if target is not None: # hybrid population
```

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/SpikeSourceArray.py` & `annarchy-4.8.0.3/ANNarchy/inputs/SpikeSourceArray.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/SpikeTrains.py` & `annarchy-4.8.0.3/ANNarchy/inputs/SpikeTrains.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,15 +787,15 @@
         elif name == 'corr': 
             if self._has_schedule:
                 if not isinstance(value, (list, np.ndarray)):
                     value = np.full((self.schedule.size, ), value)
                 else:
                     value = np.array(value)
                     if not value.size == self.schedule.size:
-                        Messages._erroror("HomogeneousCorrelatedSpikeTrains: corr must have the same length as schedule.")
+                        Messages._error("HomogeneousCorrelatedSpikeTrains: corr must have the same length as schedule.")
             else:
                 value = np.array([float(value)])
             if self.initialized:
                 Population.__setattr__(self, name, value)
                 try:
                     # Correction of mu and sigma everytime r, c or tau is changed
                     mu, sigma = self._correction(self.rates, self.corr, self.tau)
```

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/TimedArray.py` & `annarchy-4.8.0.3/ANNarchy/inputs/TimedArray.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/inputs/__init__.py` & `annarchy-4.8.0.3/ANNarchy/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/intern/ConfigManagement.py` & `annarchy-4.8.0.3/ANNarchy/intern/ConfigManagement.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/intern/GlobalObjects.py` & `annarchy-4.8.0.3/ANNarchy/intern/GlobalObjects.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/intern/Messages.py` & `annarchy-4.8.0.3/ANNarchy/intern/Messages.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/intern/NetworkManager.py` & `annarchy-4.8.0.3/ANNarchy/intern/NetworkManager.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/intern/Profiler.py` & `annarchy-4.8.0.3/ANNarchy/intern/Profiler.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/intern/SpecificPopulation.py` & `annarchy-4.8.0.3/ANNarchy/intern/SpecificPopulation.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/intern/SpecificProjection.py` & `annarchy-4.8.0.3/ANNarchy/intern/SpecificProjection.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/models/Neurons.py` & `annarchy-4.8.0.3/ANNarchy/models/Neurons.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/models/Synapses.py` & `annarchy-4.8.0.3/ANNarchy/models/Synapses.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/AnalyseNeuron.py` & `annarchy-4.8.0.3/ANNarchy/parser/AnalyseNeuron.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/AnalyseSynapse.py` & `annarchy-4.8.0.3/ANNarchy/parser/AnalyseSynapse.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
             if isinstance(code, list): # an ode in a pre/post statement
                 Messages._print(eq)
                 if variable in description['pre_spike']:
                     Messages._error('It is forbidden to use ODEs in a pre_spike term.')
                 elif variable in description['posz_spike']:
                     Messages._error('It is forbidden to use ODEs in a post_spike term.')
                 else:
-                    Messages._erroror('It is forbidden to use ODEs here.')
+                    Messages._error('It is forbidden to use ODEs here.')
 
             # Replace untouched variables with their original name
             for prev, new in sorted(list(untouched.items()), key = lambda key : len(key[0]), reverse=True):
                 code = code.replace(prev, new)
 
             # Process the bounds
             if 'min' in variable['bounds'].keys():
```

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/CoupledEquations.py` & `annarchy-4.8.0.3/ANNarchy/parser/CoupledEquations.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         "Main method called after creating the object."
         # Check if the numerical method is the same for all ODEs
         methods = []
         for var in self.variables:
             methods.append(var['method'])
         if len(list(set(methods))) > 1: # mixture of methods
             Messages._print(methods)
-            Messages._erroror('Can not mix different numerical methods when solving a coupled system of equations.')
+            Messages._error('Can not mix different numerical methods when solving a coupled system of equations.')
             
         else:
             method = methods[0]
 
         if method == 'implicit' or method == 'semiimplicit':
             return self.solve_implicit(self.expression_list)
         elif method == 'midpoint':
```

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/Equation.py` & `annarchy-4.8.0.3/ANNarchy/parser/Equation.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/Extraction.py` & `annarchy-4.8.0.3/ANNarchy/parser/Extraction.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/Function.py` & `annarchy-4.8.0.3/ANNarchy/parser/Function.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         try:
             eq = parse_expr(expression,
                 local_dict = self.local_dict,
                 transformations = ((auto_number, convert_xor,))
             )
         except:
             Messages._print(expression)
-            Messages._erroror('The function depends on unknown variables.')
+            Messages._error('The function depends on unknown variables.')
 
         return sp.ccode(eq, precision=8,
             user_functions=self.user_functions)
 
     def dependencies(self):
         "For compatibility with Equation."
         return self.args
```

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/ITE.py` & `annarchy-4.8.0.3/ANNarchy/parser/ITE.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/ParserTemplate.py` & `annarchy-4.8.0.3/ANNarchy/parser/ParserTemplate.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/StringManipulation.py` & `annarchy-4.8.0.3/ANNarchy/parser/StringManipulation.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/report/LatexParser.py` & `annarchy-4.8.0.3/ANNarchy/parser/report/LatexParser.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/report/LatexReport.py` & `annarchy-4.8.0.3/ANNarchy/parser/report/LatexReport.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/report/MarkdownReport.py` & `annarchy-4.8.0.3/ANNarchy/parser/report/MarkdownReport.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/parser/report/Report.py` & `annarchy-4.8.0.3/ANNarchy/parser/report/Report.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy/thirdparty/randutils.hpp` & `annarchy-4.8.0.3/ANNarchy/thirdparty/randutils.hpp`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/ANNarchy.egg-info/PKG-INFO` & `annarchy-4.8.0.3/ANNarchy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANNarchy
-Version: 4.8.0.2
+Version: 4.8.0.3
 Summary: Artificial Neural Networks architect
 Author-email: Julien Vitay <julien.vitay@informatik.tu-chemnitz.de>, Helge Dinkelbach <helge-uelo.dinkelbach@informatik.tu-chemnitz.de>, Fred Hamker <fred.hamker@informatik.tu-chemnitz.de>
 License: GPLv2+
 Project-URL: Documentation, https://annarchy.github.io
 Project-URL: Issues, https://github.com/ANNarchy/ANNarchy/issues
 Project-URL: Source, https://github.com/ANNarchy/ANNarchy
 Keywords: neural simulator
```

### Comparing `annarchy-4.8.0.2/ANNarchy.egg-info/SOURCES.txt` & `annarchy-4.8.0.3/ANNarchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/LICENSE` & `annarchy-4.8.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/PKG-INFO` & `annarchy-4.8.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANNarchy
-Version: 4.8.0.2
+Version: 4.8.0.3
 Summary: Artificial Neural Networks architect
 Author-email: Julien Vitay <julien.vitay@informatik.tu-chemnitz.de>, Helge Dinkelbach <helge-uelo.dinkelbach@informatik.tu-chemnitz.de>, Fred Hamker <fred.hamker@informatik.tu-chemnitz.de>
 License: GPLv2+
 Project-URL: Documentation, https://annarchy.github.io
 Project-URL: Issues, https://github.com/ANNarchy/ANNarchy/issues
 Project-URL: Source, https://github.com/ANNarchy/ANNarchy
 Keywords: neural simulator
```

### Comparing `annarchy-4.8.0.2/README.md` & `annarchy-4.8.0.3/README.md`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/pyproject.toml` & `annarchy-4.8.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "Cython", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ANNarchy"
-version = "4.8.0.2"
+version = "4.8.0.3"
 description = 'Artificial Neural Networks architect'
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "GPLv2+"}
 keywords = ["neural simulator"]
 authors = [
   { name = "Julien Vitay", email = "julien.vitay@informatik.tu-chemnitz.de" },
```

### Comparing `annarchy-4.8.0.2/setup.py` & `annarchy-4.8.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/tests/test_CUDA.py` & `annarchy-4.8.0.3/tests/test_CUDA.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/tests/test_openmp.py` & `annarchy-4.8.0.3/tests/test_openmp.py`

 * *Files identical despite different names*

### Comparing `annarchy-4.8.0.2/tests/test_single_thread.py` & `annarchy-4.8.0.3/tests/test_single_thread.py`

 * *Files identical despite different names*

