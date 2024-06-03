# Comparing `tmp/sage_lib-0.1.5.6.tar.gz` & `tmp/sage_lib-0.1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_lib-0.1.5.6.tar", last modified: Sun Jun  2 09:46:50 2024, max compression
+gzip compressed data, was "sage_lib-0.1.5.7.tar", last modified: Sun Jun  2 16:06:03 2024, max compression
```

## Comparing `sage_lib-0.1.5.6.tar` & `sage_lib-0.1.5.7.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.336952 sage_lib-0.1.5.6/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-06-02 09:46:50.336740 sage_lib-0.1.5.6/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.6/README.md
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.314051 sage_lib-0.1.5.6/sage_lib/
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.317924 sage_lib-0.1.5.6/sage_lib/IO/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.6/sage_lib/IO/BashScriptManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.6/sage_lib/IO/BinaryDataHandler.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.6/sage_lib/IO/ChargeFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.6/sage_lib/IO/DOSManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.6/sage_lib/IO/EigenvalueFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.6/sage_lib/IO/ForceFieldManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.6/sage_lib/IO/KPointsManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    17984 2024-05-31 14:22:32.000000 sage_lib-0.1.5.6/sage_lib/IO/OutFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.6/sage_lib/IO/PROFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.6/sage_lib/IO/PotentialManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.6/sage_lib/IO/WaveFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/IO/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.319348 sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputClassic.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputFile.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.322007 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPosition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5789 2024-05-21 15:53:34.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6242 2024-05-24 12:11:00.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24117 2024-05-27 10:02:52.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    47905 2024-05-29 15:35:27.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    32829 2024-05-22 08:19:10.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/plot.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.325090 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rw-r--r--   0 dimitry    (501) staff       (20)     8851 2024-05-21 15:56:27.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rw-r--r--   0 dimitry    (501) staff       (20)    12684 2024-05-29 12:51:56.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-05-31 14:04:06.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5410 2024-06-02 09:28:02.000000 sage_lib-0.1.5.6/sage_lib/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.325958 sage_lib-0.1.5.6/sage_lib/descriptor/
--rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.6/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.6/sage_lib/descriptor/MDTR_rev.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/descriptor/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.326546 sage_lib-0.1.5.6/sage_lib/ensemble/
--rw-rw-r--   0 dimitry    (501) staff       (20)     1752 2024-06-02 08:27:45.000000 sage_lib-0.1.5.6/sage_lib/ensemble/DFTEnsemble.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.6/sage_lib/ensemble/FFEnsembleManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/ensemble/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    64934 2024-06-02 09:28:57.000000 sage_lib-0.1.5.6/sage_lib/main.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    60371 2024-05-26 18:50:36.000000 sage_lib-0.1.5.6/sage_lib/main2.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    63292 2024-05-24 08:50:37.000000 sage_lib-0.1.5.6/sage_lib/main_rev.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.327592 sage_lib-0.1.5.6/sage_lib/master/
--rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.6/sage_lib/master/AtomicProperties.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.6/sage_lib/master/FileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/master/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.328654 sage_lib-0.1.5.6/sage_lib/miscellaneous/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.6/sage_lib/miscellaneous/BandPathGenerator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.6/sage_lib/miscellaneous/MD_tools.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.6/sage_lib/miscellaneous/periodic_kdtree.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.329700 sage_lib-0.1.5.6/sage_lib/partition/
--rw-rw-r--   0 dimitry    (501) staff       (20)    18348 2024-06-02 06:52:28.000000 sage_lib-0.1.5.6/sage_lib/partition/Partition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-27 11:12:35.000000 sage_lib-0.1.5.6/sage_lib/partition/PartitionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/partition/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.335284 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/BandStructure_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Blender_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    14429 2024-06-02 07:17:44.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Config_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24171 2024-05-29 14:35:56.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/CrystalDefect_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Crystal_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Dataset_builder.py
--rw-r--r--   0 dimitry    (501) staff       (20)     6623 2024-06-02 09:37:05.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Extract_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Filter_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    15646 2024-05-24 14:03:21.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Molecule_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/partition/partition_builder/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.336383 sage_lib-0.1.5.6/sage_lib/single_run/
--rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.6/sage_lib/single_run/FF_Gap.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.6/sage_lib/single_run/SingleRun.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.6/sage_lib/single_run/SingleRunDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.6/sage_lib/single_run/SingleRunManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.6/sage_lib/single_run/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 09:46:50.336524 sage_lib-0.1.5.6/sage_lib.egg-info/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-06-02 09:46:50.000000 sage_lib-0.1.5.6/sage_lib.egg-info/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)     3892 2024-06-02 09:46:50.000000 sage_lib-0.1.5.6/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-06-02 09:46:50.000000 sage_lib-0.1.5.6/sage_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-06-02 09:46:50.000000 sage_lib-0.1.5.6/sage_lib.egg-info/entry_points.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-06-02 09:46:50.000000 sage_lib-0.1.5.6/sage_lib.egg-info/requires.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-06-02 09:46:50.000000 sage_lib-0.1.5.6/sage_lib.egg-info/top_level.txt
--rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-06-02 09:46:50.337000 sage_lib-0.1.5.6/setup.cfg
--rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-06-02 09:46:17.000000 sage_lib-0.1.5.6/setup.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.960067 sage_lib-0.1.5.7/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-06-02 16:06:03.959873 sage_lib-0.1.5.7/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.7/README.md
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.937922 sage_lib-0.1.5.7/sage_lib/
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.941767 sage_lib-0.1.5.7/sage_lib/IO/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.7/sage_lib/IO/BashScriptManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.7/sage_lib/IO/BinaryDataHandler.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.7/sage_lib/IO/ChargeFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.7/sage_lib/IO/DOSManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.7/sage_lib/IO/EigenvalueFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.7/sage_lib/IO/ForceFieldManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.7/sage_lib/IO/KPointsManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    17984 2024-05-31 14:22:32.000000 sage_lib-0.1.5.7/sage_lib/IO/OutFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.7/sage_lib/IO/PROFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.7/sage_lib/IO/PotentialManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.7/sage_lib/IO/WaveFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/IO/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.943088 sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputClassic.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputFile.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.945506 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPosition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5789 2024-05-21 15:53:34.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6242 2024-05-24 12:11:00.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24117 2024-05-27 10:02:52.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    47906 2024-06-02 15:53:17.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    32829 2024-05-22 08:19:10.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/plot.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.948495 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rw-r--r--   0 dimitry    (501) staff       (20)     8851 2024-05-21 15:56:27.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rw-r--r--   0 dimitry    (501) staff       (20)    12684 2024-05-29 12:51:56.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-05-31 14:04:06.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5410 2024-06-02 09:28:02.000000 sage_lib-0.1.5.7/sage_lib/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.949313 sage_lib-0.1.5.7/sage_lib/descriptor/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.7/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.7/sage_lib/descriptor/MDTR_rev.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/descriptor/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.949894 sage_lib-0.1.5.7/sage_lib/ensemble/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1752 2024-06-02 08:27:45.000000 sage_lib-0.1.5.7/sage_lib/ensemble/DFTEnsemble.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.7/sage_lib/ensemble/FFEnsembleManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/ensemble/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    66976 2024-06-02 16:05:36.000000 sage_lib-0.1.5.7/sage_lib/main.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    60371 2024-05-26 18:50:36.000000 sage_lib-0.1.5.7/sage_lib/main2.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    63292 2024-05-24 08:50:37.000000 sage_lib-0.1.5.7/sage_lib/main_rev.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.950839 sage_lib-0.1.5.7/sage_lib/master/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.7/sage_lib/master/AtomicProperties.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.7/sage_lib/master/FileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/master/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.951710 sage_lib-0.1.5.7/sage_lib/miscellaneous/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.7/sage_lib/miscellaneous/BandPathGenerator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.7/sage_lib/miscellaneous/MD_tools.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.7/sage_lib/miscellaneous/periodic_kdtree.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.952810 sage_lib-0.1.5.7/sage_lib/partition/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    18348 2024-06-02 06:52:28.000000 sage_lib-0.1.5.7/sage_lib/partition/Partition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-27 11:12:35.000000 sage_lib-0.1.5.7/sage_lib/partition/PartitionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/partition/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.958326 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Blender_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14429 2024-06-02 07:17:44.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Config_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24171 2024-05-29 14:35:56.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Crystal_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Dataset_builder.py
+-rw-r--r--   0 dimitry    (501) staff       (20)     6623 2024-06-02 09:37:05.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Extract_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Filter_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    15646 2024-05-24 14:03:21.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Molecule_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/partition/partition_builder/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.959482 sage_lib-0.1.5.7/sage_lib/single_run/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.7/sage_lib/single_run/FF_Gap.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.7/sage_lib/single_run/SingleRun.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.7/sage_lib/single_run/SingleRunDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.7/sage_lib/single_run/SingleRunManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.7/sage_lib/single_run/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-06-02 16:06:03.959650 sage_lib-0.1.5.7/sage_lib.egg-info/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-06-02 16:06:03.000000 sage_lib-0.1.5.7/sage_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3892 2024-06-02 16:06:03.000000 sage_lib-0.1.5.7/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-06-02 16:06:03.000000 sage_lib-0.1.5.7/sage_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-06-02 16:06:03.000000 sage_lib-0.1.5.7/sage_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-06-02 16:06:03.000000 sage_lib-0.1.5.7/sage_lib.egg-info/requires.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-06-02 16:06:03.000000 sage_lib-0.1.5.7/sage_lib.egg-info/top_level.txt
+-rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-06-02 16:06:03.960119 sage_lib-0.1.5.7/setup.cfg
+-rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-06-02 16:05:17.000000 sage_lib-0.1.5.7/setup.py
```

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.5.7/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/OutFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,14 +711,15 @@
 
                 if  B>A and (periodic or np.linalg.norm( (position_A-self.atomPositions[B]) ) < AB_bond_distance):
                     connection_list.append([A, B])
         
         return connection_list
         #[(n1, n2) for n1 in range(self.atomCount) for n2 in range(n1 + 1, self.atomCount) if self.is_bond(n1, n2, periodic=periodic)]
 
+
     # =========== NEIGHBORS =========== # # =========== NEIGHBORS =========== # # =========== NEIGHBORS =========== # # =========== NEIGHBORS =========== # 
 
     # =========== OPERATIONS =========== # # =========== OPERATIONS =========== # # =========== OPERATIONS =========== # # =========== OPERATIONS =========== # 
     def get_plane(self, atom1, atom2, atom3):
         v1 = self.atomPositions[atom1, :] - self.atomPositions[atom2, :]
         v2 = self.atomPositions[atom2, :] - self.atomPositions[atom3, :]
         # | i        j     k   | #
```

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.5.7/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/__init__.py` & `sage_lib-0.1.5.7/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.5.7/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.5.7/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.5.7/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.5.7/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/main.py` & `sage_lib-0.1.5.7/sage_lib/main_rev.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,32 +620,14 @@
         'camera': camera,
         'repeat': repeat,
         'verbose': verbose,
     }
 
     PT.handleBLENDER( values={f'{plot}':values}  )
 
-def generate_extract(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, 
-                g:str=None, f:list=None,  last:bool=None,
-                verbose:bool=False, conteiner_index:int=None):
-    
-    # Initialize the DFTPartition object
-    PT = Partition()
-
-    # Read files and apply configurations
-    PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
-
-    values = {
-        'g'         :   g,
-        'format'    :   f,
-        'last'      :   last, 
-    }
-
-    PT.generate_extract(values=values, verbose=verbose)
-
 def add_arguments(parser):
     """
     Adds common arguments to the given subparser. This includes arguments for file paths, 
     verbosity, and other common settings used across various sub-commands.
     """
     structure_list = ['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS', 'gen', 'POSCAR', 'AIMS', 'ASE', 'PDB', 'DUMP', 'LAMMPS']
     parser.add_argument('--path', type=str, default='.', help='Path to the files directory')
@@ -657,16 +639,14 @@
     parser.add_argument('--output_path', type=str, default='.', help='Path for exporting VASP partition and scripts')
     parser.add_argument('--output_source', type=str, choices=structure_list, help='Source for exporting partition and scripts')
 
     parser.add_argument('--verbose', default=False, action='store_true', help='Display additional information')
     parser.add_argument('--subfolders', default=False, action='store_true', help='Read from all subfolders under the specified path')    
     parser.add_argument('--conteiner_index', type=int, help='')    
 
-
-
 def parse_dynamic_groups(args):
     atom_groups = [None] * 10  # Suponiendo hasta 10 grupos
     group_numbers = [None] * 10
 
     for key, value in vars(args).items():
         if key.startswith('g') and not key.startswith('gn') and value is not None:
             index = int(key[1:]) - 1  # Obtener el índice del grupo
@@ -794,15 +774,15 @@
     parser_edit.add_argument('--degree', type=int, required=False, default=1, help='')
     parser_edit.add_argument('--first_neighbor', required=False, default=False, action='store_true', help='')
 
     # ========== Sub-command: edit_configuration ===========
     parser_edit_config = subparsers.add_parser('edit_configuration', help='Modify the configuration settings of your simulation or calculation process.')
     add_arguments(parser_edit_config)
     parser_edit_config.add_argument('--edit', type=str, choices=['atom_id', 'atom_index'], help='Specify the type of configuration modification.')
-    parser_edit_config.add_argument('--search', type=str, choices=['full', 'random', 'exact'], required=False, help='')
+    parser_edit_config.add_argument('--search', type=str, choices=['full', 'random'], required=False, help='')
     parser_edit_config.add_argument('--index', type=int, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--ID', type=str, nargs='+', required=False, help='Identifier for the configuration element to modify.')
     parser_edit_config.add_argument('--new_ID', type=str, nargs='+', required=False, help='New identifier to assign to the configuration element.')
     parser_edit_config.add_argument('--weights', type=float, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--N', default=1, type=int, required=False, help='.')
     parser_edit_config.add_argument('--seed', default=1, type=int, required=False, help='.')
 
@@ -861,24 +841,15 @@
     parser_blender.add_argument('--samples', type=int, default=15, required=False, help='')
     parser_blender.add_argument('--fog', action='store_true', default=False, required=False, help='')
     parser_blender.add_argument('--render', action='store_true', default=False, required=False, help='')
     parser_blender.add_argument('--sigma', type=float, default=1.1, required=False, help='')
     parser_blender.add_argument('--scale', type=float, default=1.0, required=False, help='')
     parser_blender.add_argument('--camera', type=str, nargs='+', default=['x', 'y', 'z'], choices=['x', '-x', 'y', '-y', 'z', '-z'], required=False, help='')
     parser_blender.add_argument('--repeat', type=int, nargs=3, default=[0,0,0], required=False, help='')
-   
-    # ========== EXTRACT ===========
-    parser_extract = subparsers.add_parser('extract', help='')
-    add_arguments(parser_extract)
-    #parser_extract.add_argument('--plot', type=str, choices=['correlation'], default='xyz', required=False, help='')
-    #parser_extract.add_argument('--resolution', type=int, nargs=2, default=[1920, 1920], required=False, help='')
-    parser_extract.add_argument(f'--g', nargs='+', help=f'List of atom indices for group')
-    parser_extract.add_argument(f'--f', type=str, choices=['h5'], help=f'')
-    parser_extract.add_argument('--last', default=False, action='store_true', help='')    
-
+    
     args = parser.parse_args()
 
     # Handle execution based on the specified sub-command
     if args.command == 'defect':
         atom_groups, group_numbers = parse_dynamic_groups(args)
         generate_defects(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             output_path=args.output_path, output_source=args.output_source,
@@ -973,15 +944,9 @@
     elif args.command == 'blender':
         generate_BLENDER(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             verbose=args.verbose, output_path=args.output_path, 
             plot=args.plot, resolution=args.resolution, samples=args.samples, fog=args.fog, render=args.render,
             scale=args.scale, camera=args.camera, repeat=args.repeat, 
             sigma=args.sigma, )
 
-
-    elif args.command == 'extract':
-        generate_extract(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
-            verbose=args.verbose, output_path=args.output_path, 
-            g=args.g, f=args.f,  last=args.last)
-
 if __name__ == '__main__':
     main()
```

### Comparing `sage_lib-0.1.5.6/sage_lib/main2.py` & `sage_lib-0.1.5.7/sage_lib/main2.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/main_rev.py` & `sage_lib-0.1.5.7/sage_lib/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -620,14 +620,86 @@
         'camera': camera,
         'repeat': repeat,
         'verbose': verbose,
     }
 
     PT.handleBLENDER( values={f'{plot}':values}  )
 
+def generate_extract(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, 
+                g:str=None, f:list=None,  last:bool=None,
+                verbose:bool=False, conteiner_index:int=None):
+    
+
+    import ast
+
+    with open('data.txt', 'r') as file:
+        content = file.read()
+    data = ast.literal_eval(content)
+
+    print(data)
+
+    for item1, key1 in data.items():
+        path = item1['init']+'/OUTCAR'
+        PT_init = Partition()
+        PT_init.read_files(file_location=path, source='OUTCAR', energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
+        PT_init.containers = [PT_init.containers[-1]]
+
+        path = item1['end']+'/OUTCAR'
+        PT_end = Partition()
+        PT_end.read_files(file_location=path, source='OUTCAR', energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
+        PT_end.containers = [PT_end.containers[-1]]
+
+        path = item1['ts']+'/OUTCAR'
+        PT_ts = Partition()
+        PT_ts.read_files(file_location=path, source='OUTCAR', energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
+        PT_ts.containers = [PT_ts.containers[-1]]
+
+        # Condición para labels
+        condition_labels = (PT_ts.containers[0].AtomPositionManager.atomLabelsList == 'Fe') | (PT_ts.containers[0].AtomPositionManager.atomLabelsList == 'Ni')
+
+        # Condición para la coordenada z
+        condition_z = PT_ts.containers[0].AtomPositionManager.atomPositions[:, 2] > 25.5
+
+        # Índices que cumplen ambas condiciones
+        indices = np.where(condition_labels & condition_z)[0]
+        
+        values = {
+                    'g'         :   ['H2O'],
+                    'format'    :   f,
+                    'last'      :   last, 
+                }
+
+        indices = np.concatenate((indices, PT_end.generate_extract(values=values, verbose=verbose)))
+
+        values = {
+                    'g'         :   ['OOH'],
+                    'format'    :   f,
+                    'last'      :   last, 
+                }
+        indices = np.concatenate((indices, PT_init.generate_extract(values=values, verbose=verbose)))
+
+        indices = list(set(indices))
+        print(indices)
+    '''
+    # Initialize the DFTPartition object
+    PT = Partition()
+
+    # Read files and apply configurations
+    PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
+
+    values = {
+        'g'         :   g,
+        'format'    :   f,
+        'last'      :   last, 
+    }
+
+
+    PT.generate_extract(values=values, verbose=verbose)
+    '''
+
 def add_arguments(parser):
     """
     Adds common arguments to the given subparser. This includes arguments for file paths, 
     verbosity, and other common settings used across various sub-commands.
     """
     structure_list = ['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS', 'gen', 'POSCAR', 'AIMS', 'ASE', 'PDB', 'DUMP', 'LAMMPS']
     parser.add_argument('--path', type=str, default='.', help='Path to the files directory')
@@ -639,14 +711,16 @@
     parser.add_argument('--output_path', type=str, default='.', help='Path for exporting VASP partition and scripts')
     parser.add_argument('--output_source', type=str, choices=structure_list, help='Source for exporting partition and scripts')
 
     parser.add_argument('--verbose', default=False, action='store_true', help='Display additional information')
     parser.add_argument('--subfolders', default=False, action='store_true', help='Read from all subfolders under the specified path')    
     parser.add_argument('--conteiner_index', type=int, help='')    
 
+
+
 def parse_dynamic_groups(args):
     atom_groups = [None] * 10  # Suponiendo hasta 10 grupos
     group_numbers = [None] * 10
 
     for key, value in vars(args).items():
         if key.startswith('g') and not key.startswith('gn') and value is not None:
             index = int(key[1:]) - 1  # Obtener el índice del grupo
@@ -774,15 +848,15 @@
     parser_edit.add_argument('--degree', type=int, required=False, default=1, help='')
     parser_edit.add_argument('--first_neighbor', required=False, default=False, action='store_true', help='')
 
     # ========== Sub-command: edit_configuration ===========
     parser_edit_config = subparsers.add_parser('edit_configuration', help='Modify the configuration settings of your simulation or calculation process.')
     add_arguments(parser_edit_config)
     parser_edit_config.add_argument('--edit', type=str, choices=['atom_id', 'atom_index'], help='Specify the type of configuration modification.')
-    parser_edit_config.add_argument('--search', type=str, choices=['full', 'random'], required=False, help='')
+    parser_edit_config.add_argument('--search', type=str, choices=['full', 'random', 'exact'], required=False, help='')
     parser_edit_config.add_argument('--index', type=int, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--ID', type=str, nargs='+', required=False, help='Identifier for the configuration element to modify.')
     parser_edit_config.add_argument('--new_ID', type=str, nargs='+', required=False, help='New identifier to assign to the configuration element.')
     parser_edit_config.add_argument('--weights', type=float, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--N', default=1, type=int, required=False, help='.')
     parser_edit_config.add_argument('--seed', default=1, type=int, required=False, help='.')
 
@@ -841,15 +915,24 @@
     parser_blender.add_argument('--samples', type=int, default=15, required=False, help='')
     parser_blender.add_argument('--fog', action='store_true', default=False, required=False, help='')
     parser_blender.add_argument('--render', action='store_true', default=False, required=False, help='')
     parser_blender.add_argument('--sigma', type=float, default=1.1, required=False, help='')
     parser_blender.add_argument('--scale', type=float, default=1.0, required=False, help='')
     parser_blender.add_argument('--camera', type=str, nargs='+', default=['x', 'y', 'z'], choices=['x', '-x', 'y', '-y', 'z', '-z'], required=False, help='')
     parser_blender.add_argument('--repeat', type=int, nargs=3, default=[0,0,0], required=False, help='')
-    
+   
+    # ========== EXTRACT ===========
+    parser_extract = subparsers.add_parser('extract', help='')
+    add_arguments(parser_extract)
+    #parser_extract.add_argument('--plot', type=str, choices=['correlation'], default='xyz', required=False, help='')
+    #parser_extract.add_argument('--resolution', type=int, nargs=2, default=[1920, 1920], required=False, help='')
+    parser_extract.add_argument(f'--g', nargs='+', help=f'List of atom indices for group')
+    parser_extract.add_argument(f'--f', type=str, choices=['h5'], help=f'')
+    parser_extract.add_argument('--last', default=False, action='store_true', help='')    
+
     args = parser.parse_args()
 
     # Handle execution based on the specified sub-command
     if args.command == 'defect':
         atom_groups, group_numbers = parse_dynamic_groups(args)
         generate_defects(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             output_path=args.output_path, output_source=args.output_source,
@@ -944,9 +1027,15 @@
     elif args.command == 'blender':
         generate_BLENDER(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             verbose=args.verbose, output_path=args.output_path, 
             plot=args.plot, resolution=args.resolution, samples=args.samples, fog=args.fog, render=args.render,
             scale=args.scale, camera=args.camera, repeat=args.repeat, 
             sigma=args.sigma, )
 
+
+    elif args.command == 'extract':
+        generate_extract(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
+            verbose=args.verbose, output_path=args.output_path, 
+            g=args.g, f=args.f,  last=args.last)
+
 if __name__ == '__main__':
     main()
```

### Comparing `sage_lib-0.1.5.6/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.5.7/sage_lib/master/AtomicProperties.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/master/FileManager.py` & `sage_lib-0.1.5.7/sage_lib/master/FileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.5.7/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/miscellaneous/MD_tools.py` & `sage_lib-0.1.5.7/sage_lib/miscellaneous/MD_tools.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.5.7/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/Partition.py` & `sage_lib-0.1.5.7/sage_lib/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.5.7/sage_lib/partition/PartitionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Blender_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Blender_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Config_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Config_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/CrystalDefect_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/CrystalDefect_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Dataset_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Extract_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Extract_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.5.7/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.5.7/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.5.7/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.5.7/sage_lib/single_run/SingleRunDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.5.7/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.6/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.5.7/sage_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

