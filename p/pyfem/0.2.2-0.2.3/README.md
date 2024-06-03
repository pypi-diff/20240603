# Comparing `tmp/pyfem-0.2.2.tar.gz` & `tmp/pyfem-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.2.2.tar", last modified: Fri May 10 04:00:01 2024, max compression
+gzip compressed data, was "pyfem-0.2.3.tar", last modified: Mon Jun  3 08:33:18 2024, max compression
```

## Comparing `pyfem-0.2.2.tar` & `pyfem-0.2.3.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.688399 pyfem-0.2.2/
--rw-rw-rw-   0        0        0     1190 2024-04-22 05:18:42.000000 pyfem-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     3846 2024-05-10 04:00:01.687426 pyfem-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 04:00:01.688399 pyfem-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1135 2024-05-10 03:47:32.000000 pyfem-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.031399 pyfem-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.059628 pyfem-0.2.2/src/pyfem/
--rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.2.2/src/pyfem/Job.py
--rw-rw-rw-   0        0        0       23 2024-05-10 03:47:11.000000 pyfem-0.2.2/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0     1388 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.113162 pyfem-0.2.2/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.2.2/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.2.2/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.117052 pyfem-0.2.2/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    14827 2024-05-09 08:43:30.000000 pyfem-0.2.2/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.175452 pyfem-0.2.2/src/pyfem/bc/
--rw-rw-rw-   0        0        0     4148 2024-04-15 03:43:05.000000 pyfem-0.2.2/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     3003 2024-04-18 05:44:17.000000 pyfem-0.2.2/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     2984 2024-04-18 05:43:15.000000 pyfem-0.2.2/src/pyfem/bc/NeumannBCConcentrated.py
--rw-rw-rw-   0        0        0    27073 2024-04-18 05:15:08.000000 pyfem-0.2.2/src/pyfem/bc/NeumannBCDistributed.py
--rw-rw-rw-   0        0        0    13067 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/bc/NeumannBCPressure.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/bc/derive_surface_integral.py
--rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.2.2/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.186159 pyfem-0.2.2/src/pyfem/database/
--rw-rw-rw-   0        0        0    11040 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/database/Database.py
--rw-rw-rw-   0        0        0        0 2024-05-06 06:45:32.000000 pyfem-0.2.2/src/pyfem/database/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.263052 pyfem-0.2.2/src/pyfem/elements/
--rw-rw-rw-   0        0        0    20942 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0    10277 2024-05-06 08:03:52.000000 pyfem-0.2.2/src/pyfem/elements/Diffusion.py
--rw-rw-rw-   0        0        0    76454 2024-05-06 08:03:40.000000 pyfem-0.2.2/src/pyfem/elements/SolidFiniteStrain.py
--rw-rw-rw-   0        0        0    18076 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
--rw-rw-rw-   0        0        0    12097 2024-05-06 07:59:24.000000 pyfem-0.2.2/src/pyfem/elements/SolidSmallStrain.py
--rw-rw-rw-   0        0        0    16068 2024-05-06 08:04:12.000000 pyfem-0.2.2/src/pyfem/elements/SolidThermalSmallStrain.py
--rw-rw-rw-   0        0        0     8266 2024-05-06 08:04:41.000000 pyfem-0.2.2/src/pyfem/elements/Thermal.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     3324 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/elements/get_element_data.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.275708 pyfem-0.2.2/src/pyfem/fem/
--rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.2.2/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0      344 2024-04-15 03:43:05.000000 pyfem-0.2.2/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.358439 pyfem-0.2.2/src/pyfem/io/
--rw-rw-rw-   0        0        0     1124 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0     2136 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0     2242 2024-05-10 03:46:13.000000 pyfem-0.2.2/src/pyfem/io/BaseIO.py
--rw-rw-rw-   0        0        0      994 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     3289 2024-05-06 07:17:36.000000 pyfem-0.2.2/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      802 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0     1065 2023-09-21 04:09:47.000000 pyfem-0.2.2/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0      672 2023-10-30 08:41:09.000000 pyfem-0.2.2/src/pyfem/io/Parameter.py
--rw-rw-rw-   0        0        0    13127 2024-05-10 03:41:51.000000 pyfem-0.2.2/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0     2149 2023-09-15 03:47:33.000000 pyfem-0.2.2/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0     1952 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-12-20 04:03:58.000000 pyfem-0.2.2/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     5839 2024-01-15 09:02:18.000000 pyfem-0.2.2/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.402241 pyfem-0.2.2/src/pyfem/isoelements/
--rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/isoelements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    21673 2024-05-06 09:08:36.000000 pyfem-0.2.2/src/pyfem/isoelements/IsoElementShape.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/isoelements/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/isoelements/derive_shape_functions.py
--rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.2.2/src/pyfem/isoelements/get_iso_element_type.py
--rw-rw-rw-   0        0        0    27934 2024-03-28 07:20:41.000000 pyfem-0.2.2/src/pyfem/isoelements/shape_functions.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.501520 pyfem-0.2.2/src/pyfem/materials/
--rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     3177 2024-05-09 08:36:01.000000 pyfem-0.2.2/src/pyfem/materials/DiffusionIsotropic.py
--rw-rw-rw-   0        0        0     8772 2024-05-09 08:28:32.000000 pyfem-0.2.2/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     3177 2024-05-09 08:29:14.000000 pyfem-0.2.2/src/pyfem/materials/MechanicalThermalExpansion.py
--rw-rw-rw-   0        0        0     2211 2024-05-09 08:34:27.000000 pyfem-0.2.2/src/pyfem/materials/PhaseFieldDamage.py
--rw-rw-rw-   0        0        0    80110 2024-05-09 08:51:21.000000 pyfem-0.2.2/src/pyfem/materials/PlasticCrystal.py
--rw-rw-rw-   0        0        0    91328 2024-05-10 03:46:13.000000 pyfem-0.2.2/src/pyfem/materials/PlasticCrystalGNDs.py
--rw-rw-rw-   0        0        0     8446 2024-05-09 08:34:27.000000 pyfem-0.2.2/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     3399 2024-05-09 08:35:00.000000 pyfem-0.2.2/src/pyfem/materials/ThermalIsotropic.py
--rw-rw-rw-   0        0        0    10100 2024-05-09 08:35:55.000000 pyfem-0.2.2/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0    41870 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/materials/crystal_slip_system.py
--rw-rw-rw-   0        0        0     2984 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.511309 pyfem-0.2.2/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     8071 2024-04-18 04:24:18.000000 pyfem-0.2.2/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.604692 pyfem-0.2.2/src/pyfem/quadrature/
--rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/BaseQuadrature.py
--rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/GaussLegendreQuadrature.py
--rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/PyramidQuadrature.py
--rw-rw-rw-   0        0        0    22842 2024-03-28 07:28:06.000000 pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadrature.py
--rw-rw-rw-   0        0        0    27075 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
--rw-rw-rw-   0        0        0    25700 2024-03-28 04:13:23.000000 pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadrature.py
--rw-rw-rw-   0        0        0    31453 2024-03-28 04:11:40.000000 pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadratureBarycentric.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.649466 pyfem-0.2.2/src/pyfem/solvers/
--rw-rw-rw-   0        0        0    15057 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/solvers/ArcLengthSolver.py
--rw-rw-rw-   0        0        0     1633 2024-05-06 06:45:32.000000 pyfem-0.2.2/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     2225 2024-04-18 04:22:23.000000 pyfem-0.2.2/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0    16486 2024-05-06 09:22:48.000000 pyfem-0.2.2/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0    17330 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0     1618 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.685479 pyfem-0.2.2/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      983 2024-05-10 03:46:13.000000 pyfem-0.2.2/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.2.2/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0    28928 2024-05-10 03:46:38.000000 pyfem-0.2.2/src/pyfem/utils/mechanics.py
--rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1183 2024-05-10 03:46:42.000000 pyfem-0.2.2/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.085906 pyfem-0.2.2/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0     3846 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3227 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.792113 pyfem-0.2.3/
+-rw-rw-rw-   0        0        0     1190 2024-04-22 05:18:42.000000 pyfem-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3846 2024-06-03 08:33:18.791117 pyfem-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:33:18.792113 pyfem-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2024-05-10 03:47:32.000000 pyfem-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.683625 pyfem-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.691599 pyfem-0.2.3/src/pyfem/
+-rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.2.3/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0       23 2024-06-03 08:31:31.000000 pyfem-0.2.3/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0     1388 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.701568 pyfem-0.2.3/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.2.3/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.2.3/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.703559 pyfem-0.2.3/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    14823 2024-05-24 05:32:22.000000 pyfem-0.2.3/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.711818 pyfem-0.2.3/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     4148 2024-04-15 03:43:05.000000 pyfem-0.2.3/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     3003 2024-04-18 05:44:17.000000 pyfem-0.2.3/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     2984 2024-04-18 05:43:15.000000 pyfem-0.2.3/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0    27073 2024-04-18 05:15:08.000000 pyfem-0.2.3/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0    13067 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/bc/NeumannBCPressure.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/bc/derive_surface_integral.py
+-rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.2.3/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.713812 pyfem-0.2.3/src/pyfem/database/
+-rw-rw-rw-   0        0        0    11040 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/database/Database.py
+-rw-rw-rw-   0        0        0        0 2024-05-06 06:45:32.000000 pyfem-0.2.3/src/pyfem/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.723249 pyfem-0.2.3/src/pyfem/elements/
+-rw-rw-rw-   0        0        0    20942 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0    10353 2024-05-11 06:39:11.000000 pyfem-0.2.3/src/pyfem/elements/Diffusion.py
+-rw-rw-rw-   0        0        0    76515 2024-05-11 06:36:09.000000 pyfem-0.2.3/src/pyfem/elements/SolidFiniteStrain.py
+-rw-rw-rw-   0        0        0    19087 2024-05-24 04:51:08.000000 pyfem-0.2.3/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
+-rw-rw-rw-   0        0        0    12159 2024-05-11 06:36:51.000000 pyfem-0.2.3/src/pyfem/elements/SolidSmallStrain.py
+-rw-rw-rw-   0        0        0    16134 2024-05-11 06:39:11.000000 pyfem-0.2.3/src/pyfem/elements/SolidThermalSmallStrain.py
+-rw-rw-rw-   0        0        0     8342 2024-05-11 06:39:11.000000 pyfem-0.2.3/src/pyfem/elements/Thermal.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     3324 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/elements/get_element_data.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.725242 pyfem-0.2.3/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.2.3/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-04-15 03:43:05.000000 pyfem-0.2.3/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.738751 pyfem-0.2.3/src/pyfem/io/
+-rw-rw-rw-   0        0        0     1124 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0     2305 2024-05-15 03:57:03.000000 pyfem-0.2.3/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0     2888 2024-05-22 06:29:23.000000 pyfem-0.2.3/src/pyfem/io/BaseIO.py
+-rw-rw-rw-   0        0        0      994 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     3289 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      802 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0     1255 2024-05-15 04:17:58.000000 pyfem-0.2.3/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0      672 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/Parameter.py
+-rw-rw-rw-   0        0        0    13259 2024-05-20 03:25:24.000000 pyfem-0.2.3/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0     2684 2024-05-11 02:55:44.000000 pyfem-0.2.3/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0     2094 2024-05-22 04:58:58.000000 pyfem-0.2.3/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1647 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     5839 2024-05-10 04:11:08.000000 pyfem-0.2.3/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.744838 pyfem-0.2.3/src/pyfem/isoelements/
+-rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/isoelements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    21673 2024-05-06 09:08:36.000000 pyfem-0.2.3/src/pyfem/isoelements/IsoElementShape.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/isoelements/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/isoelements/derive_shape_functions.py
+-rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.2.3/src/pyfem/isoelements/get_iso_element_type.py
+-rw-rw-rw-   0        0        0    27934 2024-03-28 07:20:41.000000 pyfem-0.2.3/src/pyfem/isoelements/shape_functions.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.761216 pyfem-0.2.3/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     3177 2024-05-09 08:36:01.000000 pyfem-0.2.3/src/pyfem/materials/DiffusionIsotropic.py
+-rw-rw-rw-   0        0        0     8772 2024-05-09 08:28:32.000000 pyfem-0.2.3/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     3177 2024-05-09 08:29:14.000000 pyfem-0.2.3/src/pyfem/materials/MechanicalThermalExpansion.py
+-rw-rw-rw-   0        0        0     2211 2024-05-09 08:34:27.000000 pyfem-0.2.3/src/pyfem/materials/PhaseFieldDamage.py
+-rw-rw-rw-   0        0        0    80110 2024-05-09 08:51:21.000000 pyfem-0.2.3/src/pyfem/materials/PlasticCrystal.py
+-rw-rw-rw-   0        0        0    91328 2024-05-10 03:46:13.000000 pyfem-0.2.3/src/pyfem/materials/PlasticCrystalGNDs.py
+-rw-rw-rw-   0        0        0     8446 2024-05-09 08:34:27.000000 pyfem-0.2.3/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     3399 2024-05-09 08:35:00.000000 pyfem-0.2.3/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0    10100 2024-05-09 08:35:55.000000 pyfem-0.2.3/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0    41870 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/materials/crystal_slip_system.py
+-rw-rw-rw-   0        0        0     2984 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.764698 pyfem-0.2.3/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     8071 2024-04-18 04:24:18.000000 pyfem-0.2.3/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.773668 pyfem-0.2.3/src/pyfem/quadrature/
+-rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/quadrature/BaseQuadrature.py
+-rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/quadrature/GaussLegendreQuadrature.py
+-rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/quadrature/PyramidQuadrature.py
+-rw-rw-rw-   0        0        0    22842 2024-03-28 07:28:06.000000 pyfem-0.2.3/src/pyfem/quadrature/TetrahedronQuadrature.py
+-rw-rw-rw-   0        0        0    27075 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0    25700 2024-03-28 04:13:23.000000 pyfem-0.2.3/src/pyfem/quadrature/TriangleQuadrature.py
+-rw-rw-rw-   0        0        0    31453 2024-03-28 04:11:40.000000 pyfem-0.2.3/src/pyfem/quadrature/TriangleQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/quadrature/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.781150 pyfem-0.2.3/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0    15057 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/solvers/ArcLengthSolver.py
+-rw-rw-rw-   0        0        0     1633 2024-05-06 06:45:32.000000 pyfem-0.2.3/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     2225 2024-04-18 04:22:23.000000 pyfem-0.2.3/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0    16659 2024-05-24 05:34:04.000000 pyfem-0.2.3/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0    17330 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1618 2024-05-06 09:04:40.000000 pyfem-0.2.3/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.789124 pyfem-0.2.3/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      983 2024-05-10 03:46:13.000000 pyfem-0.2.3/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.2.3/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0    28928 2024-05-10 03:46:38.000000 pyfem-0.2.3/src/pyfem/utils/mechanics.py
+-rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.2.3/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1183 2024-05-10 03:46:42.000000 pyfem-0.2.3/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:33:18.697579 pyfem-0.2.3/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     3846 2024-06-03 08:33:18.000000 pyfem-0.2.3/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3227 2024-06-03 08:33:18.000000 pyfem-0.2.3/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:33:18.000000 pyfem-0.2.3/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-06-03 08:33:18.000000 pyfem-0.2.3/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-06-03 08:33:18.000000 pyfem-0.2.3/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 08:33:18.000000 pyfem-0.2.3/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.2.2/LICENSE` & `pyfem-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/PKG-INFO` & `pyfem-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Finite Element Method
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.2.2/setup.py` & `pyfem-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/Job.py` & `pyfem-0.2.3/src/pyfem/Job.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/__main__.py` & `pyfem-0.2.3/src/pyfem/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/amplitude/BaseAmplitude.py` & `pyfem-0.2.3/src/pyfem/amplitude/BaseAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.2.3/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/amplitude/get_amplitude_data.py` & `pyfem-0.2.3/src/pyfem/amplitude/get_amplitude_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/assembly/Assembly.py` & `pyfem-0.2.3/src/pyfem/assembly/Assembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
         # 初始化 rhs, fext, fint, dof_solution, ddof_solution
         self.fext = zeros(self.total_dof_number, dtype=DTYPE)
         self.fint = zeros(self.total_dof_number, dtype=DTYPE)
         self.dof_solution = zeros(self.total_dof_number, dtype=DTYPE)
         self.ddof_solution = zeros(self.total_dof_number, dtype=DTYPE)
 
-    # @show_running_time
+    @show_running_time
     def assembly_global_stiffness(self) -> None:
         if IS_PETSC:
             self.A.createAIJ((self.total_dof_number, self.total_dof_number))
             for element_data in self.element_data_list:
                 element_dof_ids = element_data.element_dof_ids
                 self.A.setValues(element_dof_ids, element_dof_ids, element_data.element_stiffness, addv=True)
             self.A.assemble()
@@ -261,15 +261,15 @@
             self.fint[element_data.element_dof_ids] += element_data.element_fint
 
     def assembly_ftime(self) -> None:
         self.ftime = zeros(self.total_dof_number, dtype=DTYPE)
         for element_data in self.element_data_list:
             self.ftime[element_data.element_dof_ids] += element_data.element_ftime
 
-    # @show_running_time
+    @show_running_time
     def update_element_data(self) -> None:
         dof_solution = self.dof_solution
         ddof_solution = self.ddof_solution
         for element_data in self.element_data_list:
             element_data.update_element_dof_values(dof_solution)
             element_data.update_element_ddof_values(ddof_solution)
             element_data.update_element_material_stiffness_fint()
```

### Comparing `pyfem-0.2.2/src/pyfem/bc/BaseBC.py` & `pyfem-0.2.3/src/pyfem/bc/BaseBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/bc/DirichletBC.py` & `pyfem-0.2.3/src/pyfem/bc/DirichletBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/bc/NeumannBCConcentrated.py` & `pyfem-0.2.3/src/pyfem/bc/NeumannBCConcentrated.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/bc/NeumannBCDistributed.py` & `pyfem-0.2.3/src/pyfem/bc/NeumannBCDistributed.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/bc/NeumannBCPressure.py` & `pyfem-0.2.3/src/pyfem/bc/NeumannBCPressure.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/bc/derive_surface_integral.py` & `pyfem-0.2.3/src/pyfem/bc/derive_surface_integral.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/bc/get_bc_data.py` & `pyfem-0.2.3/src/pyfem/bc/get_bc_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/database/Database.py` & `pyfem-0.2.3/src/pyfem/database/Database.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/elements/BaseElement.py` & `pyfem-0.2.3/src/pyfem/elements/BaseElement.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/elements/Diffusion.py` & `pyfem-0.2.3/src/pyfem/elements/Diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,29 @@
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量'),
     }
 
     __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __allowed_material_data_list__ = [('DiffusionIsotropic', 'User')]
+
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('DiffusionIsotropic', 'User')]
+        self.allowed_material_data_list = self.__allowed_material_data_list__
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.2/src/pyfem/elements/SolidFiniteStrain.py` & `pyfem-0.2.3/src/pyfem/elements/SolidFiniteStrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,28 +72,29 @@
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量')
     }
 
     __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __allowed_material_data_list__ = [('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell', 'User')]
+
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [
-            ('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell', 'User')]
+        self.allowed_material_data_list = self.__allowed_material_data_list__
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.2/src/pyfem/elements/SolidPhaseDamageSmallStrain.py` & `pyfem-0.2.3/src/pyfem/elements/SolidPhaseDamageSmallStrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from numpy import array, zeros, dot, ndarray, average, ix_, outer
+from numpy import array, zeros, dot, ndarray, average, ix_, outer, abs
+from numpy.linalg import norm
 
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
@@ -76,29 +77,30 @@
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量')
     }
 
     __slots__ = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __allowed_material_data_list__ = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell', 'PlasticCrystal', 'PlasticCrystalGNDs', 'User'),
+                                      ('PhaseFieldDamage', 'User')]
+
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [
-            ('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell', 'PlasticCrystal', 'PlasticCrystalGNDs', 'User'),
-            ('PhaseFieldDamage', 'User')]
+        self.allowed_material_data_list = self.__allowed_material_data_list__
         self.allowed_material_number = len(self.allowed_material_data_list)
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
@@ -297,34 +299,58 @@
                 energy_positive = qp_state_variables[i]['history_energy'][0]
 
             if energy_positive < qp_state_variables_new[i]['history_energy'][0]:
                 energy_positive = qp_state_variables_new[i]['history_energy'][0]
 
             qp_state_variables_new[i]['history_energy'][0] = energy_positive
 
+            if dimension == 2:
+                gi = array([1.0 * gc, 1.0 * gc])
+                qp_stress_tensor = array([[qp_stress[0], qp_stress[2]], [qp_stress[2], qp_stress[1]]])
+
+            stress_on_crack = abs(dot(qp_stress_tensor, qp_phase_gradient))
+            if norm(stress_on_crack) < 1e-16:
+                gn = array([0.5, 0.5])
+            else:
+                gn = stress_on_crack / sum(stress_on_crack)
+            gc_eff = float(dot(gn, gi))
+
+            # a = dot(qp_stress_tensor, qp_phase_gradient)
+            # b = norm(a)
+            # if b < 1e-16:
+            #     gn = array([1, 1]) / sum(array([1, 1]))
+            # else:
+            #     gn = abs(a) / b
+            # gc_eff = float(dot(gn, gi))
+
+            # gc_eff = gc
+            #
+            # if element_id == 0:
+            #     print(gn, gi, gc_eff)
+
             self.qp_energies.append(energy_positive)
 
             if is_update_stiffness:
                 self.element_stiffness[ix_(self.dof_u, self.dof_u)] += qp_weight_times_jacobi_det * \
                                                                        dot(qp_b_matrix_transpose, dot(qp_ddsdde * qp_degradation, qp_b_matrix))
 
                 self.element_stiffness[ix_(self.dof_p, self.dof_p)] += qp_weight_times_jacobi_det * \
-                                                                       ((gc / lc + 2.0 * energy_positive) * outer(qp_shape_value, qp_shape_value) +
-                                                                        gc * lc * dot(qp_dhdx.transpose(), qp_dhdx))
+                                                                       ((gc_eff / lc + 2.0 * energy_positive) * outer(qp_shape_value, qp_shape_value) +
+                                                                        gc_eff * lc * dot(qp_dhdx.transpose(), qp_dhdx))
 
                 # vecu = -2.0 * (1.0 - (qp_phase + qp_dphase)) * dot(qp_b_matrix_transpose, qp_stress * qp_degradation) * qp_weight_times_jacobi_det
                 # self.element_stiffness[ix_(self.dof_u, self.dof_p)] += outer(vecu, qp_shape_value)
                 # self.element_stiffness[ix_(self.dof_p, self.dof_u)] += outer(qp_shape_value, vecu)
 
             if is_update_fint:
                 self.element_fint[self.dof_u] += dot(qp_b_matrix_transpose, qp_stress * qp_degradation) * qp_weight_times_jacobi_det
 
                 self.element_fint[self.dof_p] += qp_weight_times_jacobi_det * \
-                                                 (gc * lc * dot(qp_dhdx.transpose(), (qp_phase_gradient + qp_dphase_gradient)) +
-                                                  gc / lc * (qp_phase + qp_dphase) * qp_shape_value +
+                                                 (gc_eff * lc * dot(qp_dhdx.transpose(), (qp_phase_gradient + qp_dphase_gradient)) +
+                                                  gc_eff / lc * (qp_phase + qp_dphase) * qp_shape_value +
                                                   2.0 * ((qp_phase + qp_dphase) - 1.0) * energy_positive * qp_shape_value)
 
     def update_element_field_variables(self) -> None:
         qp_stresses = self.qp_stresses
         qp_strains = self.qp_strains
         qp_energies = self.qp_energies
```

### Comparing `pyfem-0.2.2/src/pyfem/elements/SolidSmallStrain.py` & `pyfem-0.2.3/src/pyfem/elements/SolidSmallStrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,28 +58,29 @@
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量')
     }
 
     __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __allowed_material_data_list__ = [('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell', 'User')]
+
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [
-            ('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell', 'User')]
+        self.allowed_material_data_list = self.__allowed_material_data_list__
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.2/src/pyfem/elements/SolidThermalSmallStrain.py` & `pyfem-0.2.3/src/pyfem/elements/SolidThermalSmallStrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,29 +54,31 @@
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量')
     }
 
     __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __allowed_material_data_list__ = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell', 'User'),
+                                      ('ThermalIsotropic', 'User'),
+                                      ('MechanicalThermalExpansion', 'User')]
+
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell', 'User'),
-                                           ('ThermalIsotropic', 'User'),
-                                           ('MechanicalThermalExpansion', 'User')]
+        self.allowed_material_data_list = self.__allowed_material_data_list__
         self.allowed_material_number = len(self.allowed_material_data_list)
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.2/src/pyfem/elements/Thermal.py` & `pyfem-0.2.3/src/pyfem/elements/Thermal.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,27 +45,29 @@
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量')
     }
 
     __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __allowed_material_data_list__ = [('ThermalIsotropic', 'User')]
+
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ThermalIsotropic', 'User')]
+        self.allowed_material_data_list = self.__allowed_material_data_list__
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.2/src/pyfem/elements/get_element_data.py` & `pyfem-0.2.3/src/pyfem/elements/get_element_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/fem/Timer.py` & `pyfem-0.2.3/src/pyfem/fem/Timer.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/io/Amplitude.py` & `pyfem-0.2.3/src/pyfem/io/Amplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/io/BC.py` & `pyfem-0.2.3/src/pyfem/io/BC.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,20 @@
         'bc_element_sets': ('list[str]', '边界单元集合列表'),
         'value': ('float', '边界条件数值'),
         'amplitude_name': ('str', '边界条件幅值名称')
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
+    allowed_categories_types: dict = {
+        None: [None],
+        'DirichletBC': [''],
+        'NeumannBC': ['Concentrated', 'Distributed', 'Pressure'],
+    }
+
     def __init__(self) -> None:
         super().__init__()
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.dof: list[str] = None  # type: ignore
         self.node_sets: list[str] = None  # type: ignore
```

### Comparing `pyfem-0.2.2/src/pyfem/io/BaseIO.py` & `pyfem-0.2.3/src/pyfem/io/BaseIO.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,22 +55,39 @@
     def show(self) -> None:
         print(self.to_string())
 
     def set_io_values(self, io_dict: Dict) -> None:
         for key, item in io_dict.items():
             self.__setattr__(key, item)
 
+    def set_io_values_from_toml(self, io_toml: str) -> None:
+        self.set_io_values(tomllib.loads(io_toml))
+
     def to_dict(self) -> dict:
         object_dict = {}
         for key in self.__slots__:
             item = self.__getattribute__(key)
             if item is not None:
                 object_dict[key] = item
         return object_dict
 
+    def remove_none_values(self, object_dict: dict) -> dict:
+        if not isinstance(object_dict, dict):
+            return object_dict
+
+        for key, value in list(object_dict.items()):
+            if value is None:
+                del object_dict[key]
+            elif isinstance(value, dict):
+                self.remove_none_values(value)
+                if not value:  # 如果子字典为空，则删除该键
+                    del object_dict[key]
+
+        return object_dict
+
     def to_toml(self) -> str:
-        return tomli_w.dumps(self.to_dict())
+        return tomli_w.dumps(self.remove_none_values(self.to_dict()))
 
 
 if __name__ == "__main__":
     io = BaseIO()
     io.show()
```

### Comparing `pyfem-0.2.2/src/pyfem/io/Dof.py` & `pyfem-0.2.3/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/io/Material.py` & `pyfem-0.2.3/src/pyfem/io/Material.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/io/Mesh.py` & `pyfem-0.2.3/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/io/Output.py` & `pyfem-0.2.3/src/pyfem/io/Output.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,34 +5,41 @@
 from pyfem.io.BaseIO import BaseIO
 
 
 class Output(BaseIO):
     """
     定义输出文件的格式和详细信息。
 
+    :ivar name: 输出名称
+    :vartype name: str
+
     :ivar type: 输出类型
     :vartype type: str
 
     :ivar field_outputs: 输出场变量列表
     :vartype field_outputs: list[str]
 
     :ivar is_save: 是否保存结果文件
     :vartype is_save: bool
     """
 
     __slots_dict__: dict = {
+        'name': ('str', '输出名称'),
         'type': ('str', '输出类型'),
         'field_outputs': ('list[str]', '输出场变量列表'),
         'is_save': ('bool', '是否保存结果文件')
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
+    allowed_types: list = ['hdf5', 'vtk']
+
     def __init__(self) -> None:
         super().__init__()
+        self.name: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.field_outputs: list[str] = None  # type: ignore
         self.is_save: bool = None  # type: ignore
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
```

### Comparing `pyfem-0.2.2/src/pyfem/io/Parameter.py` & `pyfem-0.2.3/src/pyfem/io/Parameter.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/io/Properties.py` & `pyfem-0.2.3/src/pyfem/io/Properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,16 +297,18 @@
         prop_dict['dof'] = self.__getattribute__('dof').to_dict()
         prop_dict['materials'] = [material.to_dict() for material in self.__getattribute__('materials')]
         prop_dict['sections'] = [material.to_dict() for material in self.__getattribute__('sections')]
         prop_dict['amplitudes'] = [material.to_dict() for material in self.__getattribute__('amplitudes')]
         prop_dict['bcs'] = [material.to_dict() for material in self.__getattribute__('bcs')]
         prop_dict['solver'] = self.__getattribute__('solver').to_dict()
         prop_dict['outputs'] = [material.to_dict() for material in self.__getattribute__('outputs')]
-        prop_dict['parameter_filename'] = self.__getattribute__('parameter_filename')
-        prop_dict['parameters'] = self.__getattribute__('parameters')
+        if self.__getattribute__('parameter_filename') is not None:
+            prop_dict['parameter_filename'] = self.__getattribute__('parameter_filename')
+        if self.__getattribute__('parameters') != {}:
+            prop_dict['parameters'] = self.__getattribute__('parameters')
         return prop_dict
 
 
 def extract_parameter_label(string: str) -> str:
     """
     从带有<>的字符串中提取参数标签
     """
```

### Comparing `pyfem-0.2.2/src/pyfem/io/Section.py` & `pyfem-0.2.3/src/pyfem/io/Section.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,14 +44,30 @@
         'material_names': ('list[str]', '材料列表，一个截面可以包含多个材料属性，例如热传导系数+弹性模量'),
         'data': ('list[float]', '截面数据'),
         'data_dict': ('dict[str, any]', '截面数据字典')
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
+    allowed_categories_types: dict = {
+        None: [None],
+        'Solid': ['Volume', 'PlaneStress', 'PlaneStrain'],
+        'SolidThermal': ['Volume', 'PlaneStress', 'PlaneStrain'],
+        'SolidPhaseDamage': ['Volume', 'PlaneStress', 'PlaneStrain'],
+        'Thermal': [''],
+    }
+
+    allowed_categories_options: dict = {
+        None: [None],
+        'Solid': ['SmallStrain', 'FiniteStrain'],
+        'SolidThermal': ['SmallStrain'],
+        'SolidPhaseDamage': ['SmallStrain'],
+        'Thermal': [''],
+    }
+
     def __init__(self) -> None:
         super().__init__()
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.option: str = None  # type: ignore
         self.element_sets: list[str] = None  # type: ignore
```

### Comparing `pyfem-0.2.2/src/pyfem/io/Solver.py` & `pyfem-0.2.3/src/pyfem/io/Solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,19 @@
         'initial_dtime': ('float', '初始时间增量步长'),
         'max_dtime': ('float', '最大时间增量步长'),
         'min_dtime': ('float', '最小时间增量步长')
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
+    allowed_types_options: dict = {
+        'NonlinearSolver': ['NewtonRaphson', 'InitialTangent'],
+        'LinearSolver': [''],
+    }
+
     def __init__(self) -> None:
         super().__init__()
         self.type: str = None  # type: ignore
         self.option: str = None  # type: ignore
         self.total_time: float = None  # type: ignore
         self.start_time: float = None  # type: ignore
         self.max_increment: int = None  # type: ignore
```

### Comparing `pyfem-0.2.2/src/pyfem/io/arguments.py` & `pyfem-0.2.3/src/pyfem/io/arguments.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/io/write_vtk.py` & `pyfem-0.2.3/src/pyfem/io/write_vtk.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/isoelements/IsoElementDiagram.py` & `pyfem-0.2.3/src/pyfem/isoelements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/isoelements/IsoElementShape.py` & `pyfem-0.2.3/src/pyfem/isoelements/IsoElementShape.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/isoelements/derive_shape_functions.py` & `pyfem-0.2.3/src/pyfem/isoelements/derive_shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/isoelements/get_iso_element_type.py` & `pyfem-0.2.3/src/pyfem/isoelements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/isoelements/shape_functions.py` & `pyfem-0.2.3/src/pyfem/isoelements/shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.2.3/src/pyfem/materials/BaseMaterial.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/DiffusionIsotropic.py` & `pyfem-0.2.3/src/pyfem/materials/DiffusionIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.2.3/src/pyfem/materials/ElasticIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/MechanicalThermalExpansion.py` & `pyfem-0.2.3/src/pyfem/materials/MechanicalThermalExpansion.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/PhaseFieldDamage.py` & `pyfem-0.2.3/src/pyfem/materials/PhaseFieldDamage.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/PlasticCrystal.py` & `pyfem-0.2.3/src/pyfem/materials/PlasticCrystal.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/PlasticCrystalGNDs.py` & `pyfem-0.2.3/src/pyfem/materials/PlasticCrystalGNDs.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.2.3/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/ThermalIsotropic.py` & `pyfem-0.2.3/src/pyfem/materials/ThermalIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/ViscoElasticMaxwell.py` & `pyfem-0.2.3/src/pyfem/materials/ViscoElasticMaxwell.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/crystal_slip_system.py` & `pyfem-0.2.3/src/pyfem/materials/crystal_slip_system.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/materials/get_material_data.py` & `pyfem-0.2.3/src/pyfem/materials/get_material_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/mesh/MeshData.py` & `pyfem-0.2.3/src/pyfem/mesh/MeshData.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/quadrature/BaseQuadrature.py` & `pyfem-0.2.3/src/pyfem/quadrature/BaseQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/quadrature/GaussLegendreQuadrature.py` & `pyfem-0.2.3/src/pyfem/quadrature/GaussLegendreQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/quadrature/PyramidQuadrature.py` & `pyfem-0.2.3/src/pyfem/quadrature/PyramidQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadrature.py` & `pyfem-0.2.3/src/pyfem/quadrature/TetrahedronQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py` & `pyfem-0.2.3/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadrature.py` & `pyfem-0.2.3/src/pyfem/quadrature/TriangleQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadratureBarycentric.py` & `pyfem-0.2.3/src/pyfem/quadrature/TriangleQuadratureBarycentric.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/solvers/ArcLengthSolver.py` & `pyfem-0.2.3/src/pyfem/solvers/ArcLengthSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.2.3/src/pyfem/solvers/BaseSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.2.3/src/pyfem/solvers/LinearSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.2.3/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,20 @@
                         # ksp.getPC().setType('lu')
                         ksp.setType('bcgs')
                         ksp.setConvergenceHistory()
                         ksp.getPC().setType('sor')
                         ksp.solve(b, x)
                         da = x.array[:]
                     else:
+                        import time
                         self.assembly.global_stiffness = self.assembly.global_stiffness.tocsc()
+                        time0 = time.time()
                         LU = splu(self.assembly.global_stiffness)
+                        time1 = time.time()
+                        print(time1 - time0)
                         da = LU.solve(rhs - fint)
 
                 except RuntimeError as e:
                     is_convergence = False
                     print(error_style(f"Catch RuntimeError exception: {e}"))
                     break
```

### Comparing `pyfem-0.2.2/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py` & `pyfem-0.2.3/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.2.3/src/pyfem/solvers/get_solver_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.2.3/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/utils/colors.py` & `pyfem-0.2.3/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/utils/logger.py` & `pyfem-0.2.3/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/utils/mechanics.py` & `pyfem-0.2.3/src/pyfem/utils/mechanics.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/utils/visualization.py` & `pyfem-0.2.3/src/pyfem/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem/utils/wrappers.py` & `pyfem-0.2.3/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.2/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.2.3/src/pyfem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Finite Element Method
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.2.2/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.2.3/src/pyfem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

