# Comparing `tmp/pyfem-0.1.3.tar.gz` & `tmp/pyfem-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.1.3.tar", last modified: Mon Jul 24 07:11:46 2023, max compression
+gzip compressed data, was "pyfem-0.1.4.tar", last modified: Tue Aug  1 07:08:18 2023, max compression
```

## Comparing `pyfem-0.1.3.tar` & `pyfem-0.1.4.tar`

### file list

```diff
@@ -1,96 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.650114 pyfem-0.1.3/
--rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     5000 2023-07-24 07:11:46.649121 pyfem-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4477 2023-07-21 05:51:34.000000 pyfem-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 07:11:46.650114 pyfem-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-07-24 07:11:34.000000 pyfem-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.565120 pyfem-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.577113 pyfem-0.1.3/src/pyfem/
--rw-rw-rw-   0        0        0     2370 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/Job.py
--rw-rw-rw-   0        0        0       23 2023-07-24 07:09:24.000000 pyfem-0.1.3/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.3/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.587120 pyfem-0.1.3/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0     1403 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1892 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.589113 pyfem-0.1.3/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    13349 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.597120 pyfem-0.1.3/src/pyfem/bc/
--rw-rw-rw-   0        0        0     3725 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2250 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     2222 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/NeumannBCConcentrated.py
--rw-rw-rw-   0        0        0     8556 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/NeumannBCDistributed.py
--rw-rw-rw-   0        0        0     8667 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/NeumannBCPressure.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1965 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.604120 pyfem-0.1.3/src/pyfem/elements/
--rw-rw-rw-   0        0        0    15918 2023-07-24 05:03:33.000000 pyfem-0.1.3/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0    15924 2023-07-24 06:41:10.000000 pyfem-0.1.3/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
--rw-rw-rw-   0        0        0    11522 2023-07-24 06:42:53.000000 pyfem-0.1.3/src/pyfem/elements/SolidSmallStrain.py
--rw-rw-rw-   0        0        0    16417 2023-07-24 06:30:08.000000 pyfem-0.1.3/src/pyfem/elements/SolidThermalSmallStrain.py
--rw-rw-rw-   0        0        0     8363 2023-07-24 06:42:11.000000 pyfem-0.1.3/src/pyfem/elements/Thermal.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     3127 2023-07-24 06:54:28.000000 pyfem-0.1.3/src/pyfem/elements/get_element_data.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.606122 pyfem-0.1.3/src/pyfem/fem/
--rw-rw-rw-   0        0        0     1866 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.3/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.619113 pyfem-0.1.3/src/pyfem/io/
--rw-rw-rw-   0        0        0     1124 2023-07-21 09:01:29.000000 pyfem-0.1.3/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0     2136 2023-07-21 02:42:25.000000 pyfem-0.1.3/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0     1781 2023-07-24 05:11:05.000000 pyfem-0.1.3/src/pyfem/io/BaseIO.py
--rw-rw-rw-   0        0        0      994 2023-07-21 02:42:25.000000 pyfem-0.1.3/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     2795 2023-07-21 04:25:39.000000 pyfem-0.1.3/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      802 2023-07-21 04:30:08.000000 pyfem-0.1.3/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0     1073 2023-07-21 07:53:54.000000 pyfem-0.1.3/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0     9316 2023-07-24 05:11:05.000000 pyfem-0.1.3/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0     1939 2023-07-21 05:12:54.000000 pyfem-0.1.3/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0     1952 2023-07-21 05:18:19.000000 pyfem-0.1.3/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     5230 2023-07-21 05:45:16.000000 pyfem-0.1.3/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.625120 pyfem-0.1.3/src/pyfem/isoelements/
--rw-rw-rw-   0        0        0     2320 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    19943 2023-07-24 06:39:32.000000 pyfem-0.1.3/src/pyfem/isoelements/IsoElementShape.py
--rw-rw-rw-   0        0        0        0 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/derive_shape_functions.py
--rw-rw-rw-   0        0        0     2153 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/get_iso_element_type.py
--rw-rw-rw-   0        0        0    23677 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/shape_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.634113 pyfem-0.1.3/src/pyfem/materials/
--rw-rw-rw-   0        0        0     3385 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     7734 2023-07-24 06:56:36.000000 pyfem-0.1.3/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     3135 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/MechanicalThermalExpansion.py
--rw-rw-rw-   0        0        0     2174 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/PhaseFieldDamage.py
--rw-rw-rw-   0        0        0     8629 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     2773 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/ThermalIsotropic.py
--rw-rw-rw-   0        0        0     7283 2023-07-24 06:57:39.000000 pyfem-0.1.3/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0     7188 2023-07-24 06:57:39.000000 pyfem-0.1.3/src/pyfem/materials/ViscoElasticMaxwellUMAT.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0     2266 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.636124 pyfem-0.1.3/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     7874 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.641120 pyfem-0.1.3/src/pyfem/solvers/
--rw-rw-rw-   0        0        0     1450 2023-07-21 08:11:51.000000 pyfem-0.1.3/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     2168 2023-07-21 08:28:00.000000 pyfem-0.1.3/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0     9830 2023-07-21 08:32:14.000000 pyfem-0.1.3/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-07-21 08:57:15.000000 pyfem-0.1.3/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.648112 pyfem-0.1.3/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2443 2023-07-24 05:11:05.000000 pyfem-0.1.3/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.3/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     2672 2023-07-21 08:55:34.000000 pyfem-0.1.3/src/pyfem/utils/derive.py
--rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.3/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     5032 2023-07-14 05:55:14.000000 pyfem-0.1.3/src/pyfem/utils/mechanics.py
--rw-rw-rw-   0        0        0     3941 2023-07-20 05:58:39.000000 pyfem-0.1.3/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.3/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.583125 pyfem-0.1.3/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0     5000 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2487 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.571073 pyfem-0.1.4/
+-rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4994 2023-08-01 07:08:18.570073 pyfem-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4471 2023-08-01 06:57:01.000000 pyfem-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 07:08:18.571073 pyfem-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-08-01 07:07:43.000000 pyfem-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.471073 pyfem-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.482073 pyfem-0.1.4/src/pyfem/
+-rw-rw-rw-   0        0        0     2370 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0       23 2023-08-01 07:06:03.000000 pyfem-0.1.4/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.4/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.493073 pyfem-0.1.4/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0     1403 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1892 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.495073 pyfem-0.1.4/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    13329 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.504078 pyfem-0.1.4/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     3725 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2250 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     2222 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0    25209 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0     8667 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/bc/NeumannBCPressure.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1067 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/bc/derive_surface_integral.py
+-rw-rw-rw-   0        0        0     1965 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.512077 pyfem-0.1.4/src/pyfem/elements/
+-rw-rw-rw-   0        0        0    15861 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0    18114 2023-07-28 00:07:08.000000 pyfem-0.1.4/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
+-rw-rw-rw-   0        0        0    11596 2023-07-26 07:04:19.000000 pyfem-0.1.4/src/pyfem/elements/SolidSmallStrain.py
+-rw-rw-rw-   0        0        0    16473 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/elements/SolidThermalSmallStrain.py
+-rw-rw-rw-   0        0        0     8419 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/elements/Thermal.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     3127 2023-07-24 06:54:28.000000 pyfem-0.1.4/src/pyfem/elements/get_element_data.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.515074 pyfem-0.1.4/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     1866 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.4/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.529081 pyfem-0.1.4/src/pyfem/io/
+-rw-rw-rw-   0        0        0     1124 2023-07-21 09:01:29.000000 pyfem-0.1.4/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0     2136 2023-07-21 02:42:25.000000 pyfem-0.1.4/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0     1781 2023-07-24 05:11:05.000000 pyfem-0.1.4/src/pyfem/io/BaseIO.py
+-rw-rw-rw-   0        0        0      994 2023-07-21 02:42:25.000000 pyfem-0.1.4/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2806 2023-07-24 08:07:34.000000 pyfem-0.1.4/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      802 2023-07-21 04:30:08.000000 pyfem-0.1.4/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0     1073 2023-07-21 07:53:54.000000 pyfem-0.1.4/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0     9316 2023-07-24 05:11:05.000000 pyfem-0.1.4/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0     1939 2023-07-21 05:12:54.000000 pyfem-0.1.4/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0     1952 2023-07-21 05:18:19.000000 pyfem-0.1.4/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     5230 2023-07-21 05:45:16.000000 pyfem-0.1.4/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.535079 pyfem-0.1.4/src/pyfem/isoelements/
+-rw-rw-rw-   0        0        0     2320 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/isoelements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    21358 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/isoelements/IsoElementShape.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/isoelements/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/isoelements/derive_shape_functions.py
+-rw-rw-rw-   0        0        0     2153 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/isoelements/get_iso_element_type.py
+-rw-rw-rw-   0        0        0    23677 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/isoelements/shape_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.546073 pyfem-0.1.4/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     3385 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     8212 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     3135 2023-07-24 06:57:15.000000 pyfem-0.1.4/src/pyfem/materials/MechanicalThermalExpansion.py
+-rw-rw-rw-   0        0        0     2174 2023-07-24 06:57:15.000000 pyfem-0.1.4/src/pyfem/materials/PhaseFieldDamage.py
+-rw-rw-rw-   0        0        0     6895 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/materials/PlasticCrystal.py
+-rw-rw-rw-   0        0        0     8742 2023-07-28 00:07:08.000000 pyfem-0.1.4/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     2773 2023-07-24 06:57:15.000000 pyfem-0.1.4/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0    10049 2023-07-28 00:07:08.000000 pyfem-0.1.4/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 08:08:28.000000 pyfem-0.1.4/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.548072 pyfem-0.1.4/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     7874 2023-07-24 03:15:19.000000 pyfem-0.1.4/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.554081 pyfem-0.1.4/src/pyfem/quadrature/
+-rw-rw-rw-   0        0        0     1657 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/quadrature/BaseQuadrature.py
+-rw-rw-rw-   0        0        0     1628 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/quadrature/GaussLegendreQuadrature.py
+-rw-rw-rw-   0        0        0     1122 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/quadrature/TetrahedronQuadrature.py
+-rw-rw-rw-   0        0        0     1702 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/quadrature/TriangleQuadrature.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/quadrature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.558082 pyfem-0.1.4/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0     1450 2023-07-21 08:11:51.000000 pyfem-0.1.4/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     2168 2023-07-26 07:13:41.000000 pyfem-0.1.4/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0    10760 2023-08-01 03:33:40.000000 pyfem-0.1.4/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-07-21 08:57:15.000000 pyfem-0.1.4/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.569073 pyfem-0.1.4/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2443 2023-07-24 05:11:05.000000 pyfem-0.1.4/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.4/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.4/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     2672 2023-07-21 08:55:34.000000 pyfem-0.1.4/src/pyfem/utils/derive.py
+-rw-rw-rw-   0        0        0     2848 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/utils/derive_CPFEM.py
+-rw-rw-rw-   0        0        0     4108 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/utils/derive_CPFEM2.py
+-rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.4/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     5191 2023-07-26 03:21:35.000000 pyfem-0.1.4/src/pyfem/utils/mechanics.py
+-rw-rw-rw-   0        0        0     3941 2023-07-20 05:58:39.000000 pyfem-0.1.4/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.4/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:08:18.489073 pyfem-0.1.4/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-08-01 07:08:18.000000 pyfem-0.1.4/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2792 2023-08-01 07:08:18.000000 pyfem-0.1.4/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:08:18.000000 pyfem-0.1.4/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-01 07:08:18.000000 pyfem-0.1.4/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 07:08:18.000000 pyfem-0.1.4/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 07:08:18.000000 pyfem-0.1.4/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.1.3/LICENSE` & `pyfem-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/PKG-INFO` & `pyfem-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.1.3
+Version: 0.1.4
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -129,15 +129,15 @@
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
 #### 采用abaqus格式的网格文件 hex8.inp:
 
-```abaqus
+```
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
 *Part, name=Part-1
 *Node
```

### Comparing `pyfem-0.1.3/README.md` & `pyfem-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
 #### 采用abaqus格式的网格文件 hex8.inp:
 
-```abaqus
+```
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
 *Part, name=Part-1
 *Node
```

### Comparing `pyfem-0.1.3/setup.py` & `pyfem-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,10 +30,11 @@
         ]
     },
     install_requires=[
         'numpy',
         'scipy',
         'meshio',
         'tomli',
-        'colorlog'
+        'colorlog',
+        'sympy'
     ],
 )
```

### Comparing `pyfem-0.1.3/src/pyfem/Job.py` & `pyfem-0.1.4/src/pyfem/Job.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/amplitude/BaseAmplitude.py` & `pyfem-0.1.4/src/pyfem/amplitude/BaseAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.1.4/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/amplitude/get_amplitude_data.py` & `pyfem-0.1.4/src/pyfem/amplitude/get_amplitude_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/assembly/Assembly.py` & `pyfem-0.1.4/src/pyfem/assembly/Assembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,33 +242,31 @@
         ddof_solution = self.ddof_solution
         for element_data in self.element_data_list:
             element_data.update_element_dof_values(dof_solution)
             element_data.update_element_ddof_values(ddof_solution)
             element_data.update_element_material_stiffness_fint()
 
     # @show_running_time
-    def update_element_stiffness(self) -> None:
-        for element_data in self.element_data_list:
-            element_data.update_element_stiffness()
-
-    # @show_running_time
     def update_element_data_without_stiffness(self) -> None:
         dof_solution = self.dof_solution
         ddof_solution = self.ddof_solution
         for element_data in self.element_data_list:
             element_data.update_element_dof_values(dof_solution)
             element_data.update_element_ddof_values(ddof_solution)
-            element_data.update_material_state()
-            element_data.update_element_fint()
+            element_data.update_element_material_stiffness_fint(is_update_stiffness=False)
 
     # @show_running_time
     def update_element_state_variables(self) -> None:
         for element_data in self.element_data_list:
             element_data.update_element_state_variables()
 
+    def goback_element_state_variables(self) -> None:
+        for element_data in self.element_data_list:
+            element_data.goback_element_state_variables()
+
     # @show_running_time
     def update_element_field_variables(self) -> None:
         for element_data in self.element_data_list:
             element_data.update_element_field_variables()
 
     def assembly_field_variables(self) -> None:
         nodes_number = len(self.props.mesh_data.nodes)
```

### Comparing `pyfem-0.1.3/src/pyfem/bc/BaseBC.py` & `pyfem-0.1.4/src/pyfem/bc/BaseBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/bc/DirichletBC.py` & `pyfem-0.1.4/src/pyfem/bc/DirichletBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/bc/NeumannBCConcentrated.py` & `pyfem-0.1.4/src/pyfem/bc/NeumannBCConcentrated.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/bc/NeumannBCDistributed.py` & `pyfem-0.1.4/src/pyfem/bc/NeumannBCPressure.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.isoelements.IsoElementShape import iso_element_shape_dict
 from pyfem.isoelements.get_iso_element_type import get_iso_element_type
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
-from pyfem.utils.wrappers import show_running_time
 
 
-class NeumannBCDistributed(BaseBC):
+class NeumannBCPressure(BaseBC):
     """
-    Neumann边界条件：分布力。
+    Neumann边界条件：压力。
     """
 
     __slots__ = BaseBC.__slots__ + []
 
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
-    @show_running_time
     def get_surface_from_bc_element(self, bc_element_id: int, bc_element: ndarray) -> list[tuple[int, str]]:
         nodes = self.mesh_data.nodes
         elements = self.mesh_data.elements
         element_surface = []
         for element_id, element in enumerate(elements):
             is_element_surface = all(in1d(bc_element, element))
             if is_element_surface:
@@ -132,30 +130,33 @@
             for node_index in surface_nodes:
                 for _, bc_dof_name in enumerate(bc_dof_names):
                     surface_dof_id = node_index * len(dof_names) + dof_names.index(bc_dof_name)
                     surface_dof_ids.append(surface_dof_id)
 
             dof_ids += surface_dof_ids
 
-            element_fext = zeros(nodes_number)
+            element_fext = zeros(nodes_number * len(self.bc.dof))
 
             for i in range(bc_gp_number):
                 bc_gp_jacobi = dot(bc_gp_shape_gradients[i], node_coords).transpose()
                 bc_gp_jacobi_sub = delete(bc_gp_jacobi, bc_surface_coord[0], axis=1)
-                surface_weight = bc_surface_coord[3]
                 if dimension == 2:
-                    s = sum(bc_gp_jacobi_sub ** 2)
-                    element_fext += bc_gp_shape_values[i].transpose() * bc_gp_weights[i] * bc_value * sqrt(s) * \
-                                    surface_weight
+                    pressure = -array([[0, bc_value], [-bc_value, 0]])
+                    pressure_times_jacobi = (dot(pressure, bc_gp_jacobi_sub)).transpose()
+                    element_fext += (dot(bc_gp_shape_values[i].transpose().reshape(4, -1), pressure_times_jacobi) *
+                                     bc_gp_weights[i] * bc_surface_coord[2]).reshape(-1)
+
                 elif dimension == 3:
                     s = 0
                     for row in range(bc_gp_jacobi_sub.shape[0]):
                         s += det(delete(bc_gp_jacobi_sub, row, axis=0)) ** 2
                     element_fext += bc_gp_shape_values[i].transpose() * bc_gp_weights[i] * bc_value * sqrt(s) * \
-                                    surface_weight
+                                    bc_surface_coord[2]
+
+            print(element_fext)
 
             surface_fext = []
             for fext in element_fext[surface_local_nodes]:
                 for _ in range(len(bc_dof_names)):
                     surface_fext.append(fext)
 
             bc_fext += list(surface_fext)
@@ -163,21 +164,23 @@
         self.dof_ids = array(dof_ids)
         self.bc_fext = array(bc_fext)
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
-    # props = Properties()
-    # props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-    # bc_data = NeumannBCDistributed(props.bcs[3], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
-    # bc_data.show()
+    props = Properties()
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    bc_data = NeumannBCPressure(props.bcs[3], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
+    bc_data.show()
+
+    print(props.mesh_data.bc_element_sets)
 
     # props = Properties()
     # props.read_file(r'F:\Github\pyfem\examples\hex\hex.toml')
     # bc_data = NeumannBCDistributed(props.bcs[4], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
     # bc_data.show()
 
-    props = Properties()
-    props.read_file(r'..\..\..\examples\mechanical\quad8\Job-1.toml')
-    bc_data = NeumannBCDistributed(props.bcs[2], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
-    bc_data.show()
+    # props = Properties()
+    # props.read_file(r'F:\Github\pyfem\examples\quad8\quad8.toml')
+    # bc_data = NeumannBCDistributed(props.bcs[2], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
+    # bc_data.show()
```

### Comparing `pyfem-0.1.3/src/pyfem/bc/get_bc_data.py` & `pyfem-0.1.4/src/pyfem/bc/get_bc_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/elements/BaseElement.py` & `pyfem-0.1.4/src/pyfem/elements/BaseElement.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,29 +279,23 @@
 
     def update_element_ddof_values(self, global_ddof_values: ndarray) -> None:
         self.element_ddof_values = global_ddof_values[self.element_dof_ids]
 
     def update_element_state_variables(self) -> None:
         self.gp_state_variables = deepcopy(self.gp_state_variables_new)
 
+    def goback_element_state_variables(self) -> None:
+        self.gp_state_variables_new = deepcopy(self.gp_state_variables)
+
     def update_element_material_stiffness_fint(self,
                                                is_update_material: bool = True,
                                                is_update_stiffness: bool = True,
                                                is_update_fint: bool = True, ) -> None:
         pass
 
-    def update_material_state(self) -> None:
-        pass
-
-    def update_element_stiffness(self) -> None:
-        pass
-
-    def update_element_fint(self) -> None:
-        pass
-
     def update_element_field_variables(self) -> None:
         pass
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
```

### Comparing `pyfem-0.1.3/src/pyfem/elements/SolidPhaseDamageSmallStrain.py` & `pyfem-0.1.4/src/pyfem/elements/SolidThermalSmallStrain.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,48 +9,32 @@
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import IsoElementShape
 from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
-from pyfem.utils.mechanics import get_decompose_energy
 
 
-class SolidPhaseDamageSmallStrain(BaseElement):
+class SolidThermalSmallStrain(BaseElement):
     """
-    固体相场断裂单元。
+    固体变形-温度场耦合单元。
 
     :ivar gp_b_matrices: 积分点处的B矩阵列表
     :vartype gp_b_matrices: ndarray
 
     :ivar gp_b_matrices_transpose: 积分点处的B矩阵转置列表
     :vartype gp_b_matrices_transpose: ndarray
 
     :ivar gp_strains: 积分点处的应变列表
     :vartype gp_strains: list[ndarray]
 
     :ivar gp_stresses: 积分点处的应力列表
     :vartype gp_stresses: list[ndarray]
 
-    :ivar gp_phases: 积分点处的相场变量列表
-    :vartype gp_phases: list[ndarray]
-
-    :ivar gp_phase_fluxes: 积分点处的相场变量通量列表
-    :vartype gp_phase_fluxes: list[ndarray]
-
-    :ivar gp_ddsddps: 积分点处的相场刚度矩阵列表
-    :vartype gp_ddsddps: list[ndarray]
-
-    :ivar dof_u: 单元位移自由度列表
-    :vartype dof_u: list[int]
-
-    :ivar dof_p: 单元相场自由度列表
-    :vartype dof_p: list[int]
-
     :ivar ntens: 总应力数量
     :vartype ntens: int
 
     :ivar ndi: 轴向应力数量
     :vartype ndi: int
 
     :ivar nshr: 剪切应力数量
@@ -58,56 +42,57 @@
     """
 
     __slots_dict__: dict = {
         'gp_b_matrices': ('ndarray', '积分点处的B矩阵列表'),
         'gp_b_matrices_transpose': ('ndarray', '积分点处的B矩阵转置列表'),
         'gp_strains': ('list[ndarray]', '积分点处的应变列表'),
         'gp_stresses': ('list[ndarray]', '积分点处的应力列表'),
-        'gp_phases': ('list[ndarray]', '积分点处的相场变量列表'),
-        'gp_phase_fluxes': ('list[ndarray]', '积分点处的相场变量通量列表'),
-        'gp_ddsddps': ('list[ndarray]', '积分点处的相场刚度矩阵列表'),
+        'gp_temperatures': ('ndarray', '积分点处的温度列表'),
+        'gp_heat_fluxes': ('ndarray', '积分点处的热流密度列表'),
+        'gp_ddsddts': ('list[ndarray]', '积分点处的材料热传导系数矩阵列表'),
         'dof_u': ('list[int]', '单元位移自由度列表'),
-        'dof_p': ('list[int]', '单元相场自由度列表'),
+        'dof_T': ('list[int]', '单元温度自由度列表'),
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量')
     }
 
-    __slots__ = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
+    __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
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
 
         self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell'),
-                                           ('PhaseFieldDamage',)]
+                                           ('ThermalIsotropic',),
+                                           ('MechanicalThermalExpansion',)]
         self.allowed_material_number = len(self.allowed_material_data_list)
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
         self.timer = timer
 
         if self.dimension == 2:
-            self.dof_names = ['u1', 'u2', 'phi']
+            self.dof_names = ['u1', 'u2', 'T']
             self.ntens = 4
             self.ndi = 3
             self.nshr = 1
         elif self.dimension == 3:
-            self.dof_names = ['u1', 'u2', 'u3', 'phi']
+            self.dof_names = ['u1', 'u2', 'u3', 'T']
             self.ntens = 6
             self.ndi = 3
             self.nshr = 3
         else:
             error_msg = f'{self.dimension} is not the supported dimension'
             raise NotImplementedError(error_style(error_msg))
 
@@ -116,33 +101,29 @@
             raise NotImplementedError(error_style(error_msg))
 
         element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
         self.element_dof_number = element_dof_number
         self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_ddof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_fint = zeros(element_dof_number, dtype=DTYPE)
-        self.element_stiffness = None  # type: ignore
+        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
         self.gp_b_matrices: ndarray = None  # type: ignore
         self.gp_b_matrices_transpose: ndarray = None  # type: ignore
         self.gp_strains: list[ndarray] = None  # type: ignore
         self.gp_stresses: list[ndarray] = None  # type: ignore
-        self.gp_phases: list[ndarray] = None  # type: ignore
-        self.gp_phase_fluxes: list[ndarray] = None  # type: ignore
-        self.gp_ddsddps: list[ndarray] = None  # type: ignore
-
-        # for i in range(self.gp_number):
-        #     self.gp_state_variables[i]['history_energy'] = array([0.0])
-        #     self.gp_state_variables_new[i]['history_energy'] = array([0.0])
+        self.gp_temperatures: list[ndarray] = None  # type: ignore
+        self.gp_heat_fluxes: list[ndarray] = None  # type: ignore
+        self.gp_ddsddts: list[ndarray] = None  # type: ignore
 
         self.dof_u: list[int] = list()
-        self.dof_p: list[int] = list()
+        self.dof_T: list[int] = list()
         for i in range(self.iso_element_shape.nodes_number):
             self.dof_u += [len(self.dof_names) * i + 0, len(self.dof_names) * i + 1]
-            self.dof_p += [len(self.dof_names) * i + 2]
+            self.dof_T += [len(self.dof_names) * i + 2]
 
         self.create_gp_b_matrices()
 
     def create_gp_b_matrices(self) -> None:
         if self.dimension == 2:
             self.gp_b_matrices = zeros(shape=(self.gp_number, 3, len(self.dof_u)), dtype=DTYPE)
             for igp, (gp_shape_gradient, gp_jacobi_inv) in \
@@ -178,125 +159,140 @@
                                                is_update_fint: bool = True, ) -> None:
         element_id = self.element_id
         timer = self.timer
         ntens = self.ntens
         ndi = self.ndi
         nshr = self.nshr
 
-        dimension = self.iso_element_shape.dimension
-
         gp_number = self.gp_number
         gp_shape_values = self.iso_element_shape.gp_shape_values
         gp_shape_gradients = self.iso_element_shape.gp_shape_gradients
         gp_b_matrices = self.gp_b_matrices
         gp_b_matrices_transpose = self.gp_b_matrices_transpose
         gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
 
         gp_state_variables = self.gp_state_variables
         gp_state_variables_new = self.gp_state_variables_new
 
         element_dof_values = self.element_dof_values
         element_ddof_values = self.element_ddof_values
 
         u = element_dof_values[self.dof_u]
-        phi = element_dof_values[self.dof_p]
+        T = element_dof_values[self.dof_T]
 
         du = element_ddof_values[self.dof_u]
-        dphi = element_ddof_values[self.dof_p]
+        dT = element_ddof_values[self.dof_T]
 
         solid_material_data = self.material_data_list[0]
-        phase_material_data = self.material_data_list[1]
+        thermal_material_data = self.material_data_list[1]
+        solid_thermal_material_data = self.material_data_list[2]
 
-        gc = phase_material_data.gc  # type: ignore
-        lc = phase_material_data.lc  # type: ignore
+        alpha = solid_thermal_material_data.tangent
 
         if is_update_stiffness:
             self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
         if is_update_fint:
             self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
 
         if is_update_material:
             self.gp_ddsddes = list()
             self.gp_strains = list()
             self.gp_stresses = list()
-            self.gp_ddsddps = list()
-            self.gp_phases = list()
-            self.gp_phase_fluxes = list()
 
         for i in range(gp_number):
             if is_update_material:
                 gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
                 gp_shape_value = gp_shape_values[i]
-                gp_shape_gradient = gp_shape_gradients[i]
                 gp_b_matrix_transpose = gp_b_matrices_transpose[i]
                 gp_b_matrix = gp_b_matrices[i]
                 gp_strain = dot(gp_b_matrix, u)
                 gp_dstrain = dot(gp_b_matrix, du)
-                gp_phase = dot(gp_shape_value, phi)
-                gp_dphase = dot(gp_shape_value, dphi)
-                gp_phase_gradient = dot(gp_shape_gradient, phi)
-                gp_dphase_gradient = dot(gp_shape_gradient, dphi)
-
-                degradation = min((1.0 - gp_phase) ** 2 + 1.0e-7, 1.0)
-
+                gp_temperature = dot(gp_shape_value, T)
+                gp_dtemperature = dot(gp_shape_value, dT)
+                gp_strain += (-alpha * gp_temperature)
+                gp_dstrain += (-alpha * gp_dtemperature)
                 variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
                 gp_ddsdde, gp_output = solid_material_data.get_tangent(variable=variable,
                                                                        state_variable=gp_state_variables[i],
                                                                        state_variable_new=gp_state_variables_new[i],
                                                                        element_id=element_id,
                                                                        igp=i,
                                                                        ntens=ntens,
                                                                        ndi=ndi,
                                                                        nshr=nshr,
                                                                        timer=timer)
-                gp_stress = gp_output['stress'] * degradation
+                gp_stress = gp_output['stress']
                 self.gp_ddsddes.append(gp_ddsdde)
                 self.gp_strains.append(gp_strain)
                 self.gp_stresses.append(gp_stress)
-                self.gp_phases.append(gp_phase)
-
             else:
                 gp_b_matrix_transpose = gp_b_matrices_transpose[i]
                 gp_b_matrix = gp_b_matrices[i]
                 gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
                 gp_shape_value = gp_shape_values[i]
-                gp_shape_gradient = gp_shape_gradients[i]
                 gp_ddsdde = self.gp_ddsddes[i]
                 gp_stress = self.gp_stresses[i]
-                gp_strain = dot(gp_b_matrix, u)
-                gp_dstrain = dot(gp_b_matrix, du)
-                gp_phase = dot(gp_shape_value, phi)
-                gp_dphase = dot(gp_shape_value, dphi)
-                gp_phase_gradient = dot(gp_shape_gradient, phi)
-
-            energy_positive, energy_negative = get_decompose_energy(gp_strain + gp_dstrain, gp_stress, dimension)
-
-            # if energy_positive > gp_state_variables_new[i]['history_energy'][0]:
-            #     gp_state_variables_new[i]['history_energy'][0] = energy_positive
-            # else:
-            #     energy_positive = gp_state_variables_new[i]['history_energy'][0]
 
             if is_update_stiffness:
                 self.element_stiffness[ix_(self.dof_u, self.dof_u)] += \
-                    dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * gp_weight_times_jacobi_det * degradation
-
-                self.element_stiffness[ix_(self.dof_p, self.dof_p)] += \
-                    ((gc / lc + 2.0 * energy_positive) * outer(gp_shape_value, gp_shape_value) +
-                     gc * lc * dot((gp_phase + gp_dphase),
-                                   (gp_phase + gp_dphase).transpose())) * gp_weight_times_jacobi_det
+                    dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * gp_weight_times_jacobi_det
 
             if is_update_fint:
+                dsdt = -1.0 * dot(gp_ddsdde, alpha)
+                self.element_stiffness[ix_(self.dof_u, self.dof_T)] += \
+                    dot(gp_b_matrix_transpose, outer(dsdt, gp_shape_value)) * gp_weight_times_jacobi_det
+
                 self.element_fint[self.dof_u] += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
 
-                self.element_fint[self.dof_p] += \
-                    (gc * lc * dot(gp_shape_gradient.transpose(), gp_phase_gradient) +
-                     gc / lc * gp_shape_value * (gp_phase + gp_dphase) +
-                     2.0 * ((gp_phase + gp_dphase) - 1.0) * gp_shape_value * energy_positive) \
-                    * gp_weight_times_jacobi_det
+        if is_update_material:
+            self.gp_ddsddts = list()
+            self.gp_temperatures = list()
+            self.gp_heat_fluxes = list()
+
+        for i in range(gp_number):
+            if is_update_material:
+                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
+                gp_shape_value = gp_shape_values[i]
+                gp_shape_gradient = gp_shape_gradients[i]
+                gp_temperature = dot(gp_shape_value, T)
+                gp_dtemperature = dot(gp_shape_value, dT)
+                gp_temperature_gradient = dot(gp_shape_gradient, T)
+                gp_dtemperature_gradient = dot(gp_shape_gradient, dT)
+
+                variable = {'temperature': gp_temperature,
+                            'dtemperature': gp_dtemperature,
+                            'temperature_gradient': gp_temperature_gradient,
+                            'dtemperature_gradient': gp_dtemperature_gradient}
+                gp_ddsddt, gp_output = thermal_material_data.get_tangent(variable=variable,
+                                                                         state_variable=gp_state_variables[i],
+                                                                         state_variable_new=gp_state_variables_new[i],
+                                                                         element_id=element_id,
+                                                                         igp=i,
+                                                                         ntens=ntens,
+                                                                         ndi=ndi,
+                                                                         nshr=nshr,
+                                                                         timer=timer)
+                gp_heat_flux = gp_output['heat_flux']
+                self.gp_ddsddts.append(gp_ddsddt)
+                self.gp_temperatures.append(gp_temperature)
+                self.gp_heat_fluxes.append(gp_heat_flux)
+            else:
+                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
+                gp_shape_gradient = gp_shape_gradients[i]
+                gp_ddsddt = self.gp_ddsddts[i]
+                gp_heat_flux = self.gp_heat_fluxes[i]
+
+            if is_update_stiffness:
+                self.element_stiffness[ix_(self.dof_T, self.dof_T)] += \
+                    dot(gp_shape_gradient.transpose(), dot(gp_ddsddt, gp_shape_gradient)) * gp_weight_times_jacobi_det
+
+            if is_update_fint:
+                self.element_fint[self.dof_T] += \
+                    dot(gp_shape_gradient.transpose(), gp_heat_flux) * gp_weight_times_jacobi_det
 
     def update_element_field_variables(self) -> None:
         gp_stresses = self.gp_stresses
         gp_strains = self.gp_strains
 
         average_strain = average(gp_strains, axis=0)
         average_stress = average(gp_stresses, axis=0)
@@ -326,14 +322,14 @@
             self.element_average_field_variables['S13'] = average_stress[4]
             self.element_average_field_variables['S23'] = average_stress[5]
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
-    print_slots_dict(SolidPhaseDamageSmallStrain.__slots_dict__)
-
-    from pyfem.Job import Job
-
-    job = Job(r'..\..\..\examples\mechanical_phase\rectangle\Job-1.toml')
+    print_slots_dict(SolidThermalSmallStrain.__slots_dict__)
 
-    job.assembly.element_data_list[0].show()
+    # from pyfem.Job import Job
+    #
+    # job = Job(r'..\..\..\examples\mechanical_thermal\rectangle\Job-1.toml')
+    #
+    # job.assembly.element_data_list[0].show()
```

### Comparing `pyfem-0.1.3/src/pyfem/elements/SolidSmallStrain.py` & `pyfem-0.1.4/src/pyfem/elements/SolidSmallStrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell')]
+        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'ViscoElasticMaxwell')]
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
@@ -94,15 +94,15 @@
             raise NotImplementedError(error_style(error_msg))
 
         element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
         self.element_dof_number = element_dof_number
         self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_ddof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_fint = zeros(element_dof_number, dtype=DTYPE)
-        self.element_stiffness = None  # type: ignore
+        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
         self.gp_b_matrices: ndarray = None  # type: ignore
         self.gp_b_matrices_transpose: ndarray = None  # type: ignore
         self.gp_strains: list[ndarray] = None  # type: ignore
         self.gp_stresses: list[ndarray] = None  # type: ignore
 
         self.create_gp_b_matrices()
```

### Comparing `pyfem-0.1.3/src/pyfem/elements/SolidThermalSmallStrain.py` & `pyfem-0.1.4/src/pyfem/elements/SolidPhaseDamageSmallStrain.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,90 +9,112 @@
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import IsoElementShape
 from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
+from pyfem.utils.mechanics import get_decompose_energy
 
 
-class SolidThermalSmallStrain(BaseElement):
-    """
-    固体变形-温度场耦合单元。
+class SolidPhaseDamageSmallStrain(BaseElement):
+    r"""
+    固体相场断裂单元。
 
     :ivar gp_b_matrices: 积分点处的B矩阵列表
     :vartype gp_b_matrices: ndarray
 
     :ivar gp_b_matrices_transpose: 积分点处的B矩阵转置列表
     :vartype gp_b_matrices_transpose: ndarray
 
     :ivar gp_strains: 积分点处的应变列表
     :vartype gp_strains: list[ndarray]
 
     :ivar gp_stresses: 积分点处的应力列表
     :vartype gp_stresses: list[ndarray]
 
+    :ivar gp_phases: 积分点处的相场变量列表
+    :vartype gp_phases: list[ndarray]
+
+    :ivar gp_phase_fluxes: 积分点处的相场变量通量列表
+    :vartype gp_phase_fluxes: list[ndarray]
+
+    :ivar gp_ddsddps: 积分点处的相场刚度矩阵列表
+    :vartype gp_ddsddps: list[ndarray]
+
+    :ivar dof_u: 单元位移自由度列表
+    :vartype dof_u: list[int]
+
+    :ivar dof_p: 单元相场自由度列表
+    :vartype dof_p: list[int]
+
     :ivar ntens: 总应力数量
     :vartype ntens: int
 
     :ivar ndi: 轴向应力数量
     :vartype ndi: int
 
     :ivar nshr: 剪切应力数量
     :vartype nshr: int
+
+    .. math::
+        K_{ij}^\varphi  = \int_V {\left[ {{g_c}{l_c}{{\left( {\nabla {N_i}} \right)}^T}\nabla {N_j} + \left( {\frac{{{g_c}}}{{{l_c}}} + 2H} \right){N_i}{N_j}} \right]{\text{d}}V}
+
+    .. math::
+        RHS_i^\varphi  = \int_V {\left[ {{g_c}{l_c}{{\left( {\nabla {N_i}} \right)}^T}\nabla \varphi  - \left( {2\left( {1 - \varphi } \right)H - \frac{{{g_c}}}{{{l_c}}}\varphi } \right){N_i}} \right]{\text{d}}V}
     """
 
     __slots_dict__: dict = {
         'gp_b_matrices': ('ndarray', '积分点处的B矩阵列表'),
         'gp_b_matrices_transpose': ('ndarray', '积分点处的B矩阵转置列表'),
         'gp_strains': ('list[ndarray]', '积分点处的应变列表'),
         'gp_stresses': ('list[ndarray]', '积分点处的应力列表'),
-        'gp_temperatures': ('ndarray', '积分点处的温度列表'),
-        'gp_heat_fluxes': ('ndarray', '积分点处的热流密度列表'),
-        'gp_ddsddts': ('list[ndarray]', '积分点处的材料热传导系数矩阵列表'),
+        'gp_phases': ('list[ndarray]', '积分点处的相场变量列表'),
+        'gp_phase_fluxes': ('list[ndarray]', '积分点处的相场变量通量列表'),
+        'gp_ddsddps': ('list[ndarray]', '积分点处的相场刚度矩阵列表'),
+        'gp_energies': ('list[ndarray]', '积分点处的相场刚度矩阵列表'),
         'dof_u': ('list[int]', '单元位移自由度列表'),
-        'dof_T': ('list[int]', '单元温度自由度列表'),
+        'dof_p': ('list[int]', '单元相场自由度列表'),
         'ntens': ('int', '总应力数量'),
         'ndi': ('int', '轴向应力数量'),
         'nshr': ('int', '剪切应力数量')
     }
 
-    __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
+    __slots__ = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
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
 
         self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell'),
-                                           ('ThermalIsotropic',),
-                                           ('MechanicalThermalExpansion',)]
+                                           ('PhaseFieldDamage',)]
         self.allowed_material_number = len(self.allowed_material_data_list)
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
         self.timer = timer
 
         if self.dimension == 2:
-            self.dof_names = ['u1', 'u2', 'T']
+            self.dof_names = ['u1', 'u2', 'phi']
             self.ntens = 4
             self.ndi = 3
             self.nshr = 1
         elif self.dimension == 3:
-            self.dof_names = ['u1', 'u2', 'u3', 'T']
+            self.dof_names = ['u1', 'u2', 'u3', 'phi']
             self.ntens = 6
             self.ndi = 3
             self.nshr = 3
         else:
             error_msg = f'{self.dimension} is not the supported dimension'
             raise NotImplementedError(error_style(error_msg))
 
@@ -101,29 +123,34 @@
             raise NotImplementedError(error_style(error_msg))
 
         element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
         self.element_dof_number = element_dof_number
         self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_ddof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_fint = zeros(element_dof_number, dtype=DTYPE)
-        self.element_stiffness = None  # type: ignore
+        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
         self.gp_b_matrices: ndarray = None  # type: ignore
         self.gp_b_matrices_transpose: ndarray = None  # type: ignore
         self.gp_strains: list[ndarray] = None  # type: ignore
         self.gp_stresses: list[ndarray] = None  # type: ignore
-        self.gp_temperatures: list[ndarray] = None  # type: ignore
-        self.gp_heat_fluxes: list[ndarray] = None  # type: ignore
-        self.gp_ddsddts: list[ndarray] = None  # type: ignore
+        self.gp_phases: list[ndarray] = None  # type: ignore
+        self.gp_phase_fluxes: list[ndarray] = None  # type: ignore
+        self.gp_ddsddps: list[ndarray] = None  # type: ignore
+        self.gp_energies: list[ndarray] = None  # type: ignore
+
+        for i in range(self.gp_number):
+            self.gp_state_variables[i]['history_energy'] = array([0.0])
+            self.gp_state_variables_new[i]['history_energy'] = array([0.0])
 
         self.dof_u: list[int] = list()
-        self.dof_T: list[int] = list()
+        self.dof_p: list[int] = list()
         for i in range(self.iso_element_shape.nodes_number):
             self.dof_u += [len(self.dof_names) * i + 0, len(self.dof_names) * i + 1]
-            self.dof_T += [len(self.dof_names) * i + 2]
+            self.dof_p += [len(self.dof_names) * i + 2]
 
         self.create_gp_b_matrices()
 
     def create_gp_b_matrices(self) -> None:
         if self.dimension == 2:
             self.gp_b_matrices = zeros(shape=(self.gp_number, 3, len(self.dof_u)), dtype=DTYPE)
             for igp, (gp_shape_gradient, gp_jacobi_inv) in \
@@ -159,158 +186,173 @@
                                                is_update_fint: bool = True, ) -> None:
         element_id = self.element_id
         timer = self.timer
         ntens = self.ntens
         ndi = self.ndi
         nshr = self.nshr
 
+        dimension = self.iso_element_shape.dimension
+
         gp_number = self.gp_number
         gp_shape_values = self.iso_element_shape.gp_shape_values
         gp_shape_gradients = self.iso_element_shape.gp_shape_gradients
         gp_b_matrices = self.gp_b_matrices
         gp_b_matrices_transpose = self.gp_b_matrices_transpose
+        gp_jacobi_invs = self.gp_jacobi_invs
         gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
 
         gp_state_variables = self.gp_state_variables
         gp_state_variables_new = self.gp_state_variables_new
 
         element_dof_values = self.element_dof_values
         element_ddof_values = self.element_ddof_values
 
         u = element_dof_values[self.dof_u]
-        T = element_dof_values[self.dof_T]
+        phi = element_dof_values[self.dof_p]
 
         du = element_ddof_values[self.dof_u]
-        dT = element_ddof_values[self.dof_T]
+        dphi = element_ddof_values[self.dof_p]
 
         solid_material_data = self.material_data_list[0]
-        thermal_material_data = self.material_data_list[1]
-        solid_thermal_material_data = self.material_data_list[2]
+        phase_material_data = self.material_data_list[1]
 
-        alpha = solid_thermal_material_data.tangent
+        gc = phase_material_data.gc  # type: ignore
+        lc = phase_material_data.lc  # type: ignore
 
         if is_update_stiffness:
             self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
         if is_update_fint:
             self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
 
         if is_update_material:
             self.gp_ddsddes = list()
             self.gp_strains = list()
             self.gp_stresses = list()
+            self.gp_ddsddps = list()
+            self.gp_phases = list()
+            self.gp_phase_fluxes = list()
+            self.gp_energies = list()
 
         for i in range(gp_number):
             if is_update_material:
                 gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
                 gp_shape_value = gp_shape_values[i]
+                gp_shape_gradient = gp_shape_gradients[i]
                 gp_b_matrix_transpose = gp_b_matrices_transpose[i]
                 gp_b_matrix = gp_b_matrices[i]
                 gp_strain = dot(gp_b_matrix, u)
                 gp_dstrain = dot(gp_b_matrix, du)
-                gp_temperature = dot(gp_shape_value, T)
-                gp_dtemperature = dot(gp_shape_value, dT)
-                gp_strain += (-alpha * gp_temperature)
-                gp_dstrain += (-alpha * gp_dtemperature)
+                gp_phase = dot(gp_shape_value, phi)
+                gp_dphase = dot(gp_shape_value, dphi)
+                gp_phase_gradient = dot(gp_shape_gradient, phi)
+                gp_dphase_gradient = dot(gp_shape_gradient, dphi)
+                gp_jacobi_inv = gp_jacobi_invs[i]
+                gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
+
+                degradation = (1.0 - gp_phase) ** 2 + 1.0e-7
+                degradation = min(degradation, 1.0)
+                degradation = max(degradation, 0.0)
+
                 variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
                 gp_ddsdde, gp_output = solid_material_data.get_tangent(variable=variable,
                                                                        state_variable=gp_state_variables[i],
                                                                        state_variable_new=gp_state_variables_new[i],
                                                                        element_id=element_id,
                                                                        igp=i,
                                                                        ntens=ntens,
                                                                        ndi=ndi,
                                                                        nshr=nshr,
                                                                        timer=timer)
                 gp_stress = gp_output['stress']
+                gp_plastic_energy = gp_output['plastic_energy']
                 self.gp_ddsddes.append(gp_ddsdde)
                 self.gp_strains.append(gp_strain)
-                self.gp_stresses.append(gp_stress)
+                self.gp_stresses.append(gp_stress * degradation)
+                self.gp_phases.append(gp_phase)
+
             else:
                 gp_b_matrix_transpose = gp_b_matrices_transpose[i]
                 gp_b_matrix = gp_b_matrices[i]
                 gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
                 gp_shape_value = gp_shape_values[i]
+                gp_shape_gradient = gp_shape_gradients[i]
                 gp_ddsdde = self.gp_ddsddes[i]
                 gp_stress = self.gp_stresses[i]
+                gp_strain = dot(gp_b_matrix, u)
+                gp_dstrain = dot(gp_b_matrix, du)
+                gp_phase = dot(gp_shape_value, phi)
+                gp_dphase = dot(gp_shape_value, dphi)
+                gp_phase_gradient = dot(gp_shape_gradient, phi)
+                gp_dphase_gradient = dot(gp_shape_gradient, dphi)
+                gp_jacobi_inv = gp_jacobi_invs[i]
+                gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
 
-            if is_update_stiffness:
-                self.element_stiffness[ix_(self.dof_u, self.dof_u)] += \
-                    dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * gp_weight_times_jacobi_det
+                degradation = (1.0 - gp_phase) ** 2 + 1.0e-7
+                degradation = min(degradation, 1.0)
+                degradation = max(degradation, 0.0)
 
-            if is_update_fint:
-                dsdt = -1.0 * dot(gp_ddsdde, alpha)
-                self.element_stiffness[ix_(self.dof_u, self.dof_T)] += \
-                    dot(gp_b_matrix_transpose, outer(dsdt, gp_shape_value)) * gp_weight_times_jacobi_det
+            energy_positive, energy_negative = get_decompose_energy(gp_strain + gp_dstrain, gp_stress, dimension)
 
-                self.element_fint[self.dof_u] += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
+            energy_positive += gp_plastic_energy
 
-        if is_update_material:
-            self.gp_ddsddts = list()
-            self.gp_temperatures = list()
-            self.gp_heat_fluxes = list()
+            if energy_positive < gp_state_variables[i]['history_energy'][0]:
+                energy_positive = gp_state_variables[i]['history_energy'][0]
 
-        for i in range(gp_number):
-            if is_update_material:
-                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
-                gp_shape_value = gp_shape_values[i]
-                gp_shape_gradient = gp_shape_gradients[i]
-                gp_temperature = dot(gp_shape_value, T)
-                gp_dtemperature = dot(gp_shape_value, dT)
-                gp_temperature_gradient = dot(gp_shape_gradient, T)
-                gp_dtemperature_gradient = dot(gp_shape_gradient, dT)
-
-                variable = {'temperature': gp_temperature,
-                            'dtemperature': gp_dtemperature,
-                            'temperature_gradient': gp_temperature_gradient,
-                            'dtemperature_gradient': gp_dtemperature_gradient}
-                gp_ddsddt, gp_output = thermal_material_data.get_tangent(variable=variable,
-                                                                         state_variable=gp_state_variables[i],
-                                                                         state_variable_new=gp_state_variables_new[i],
-                                                                         element_id=element_id,
-                                                                         igp=i,
-                                                                         ntens=ntens,
-                                                                         ndi=ndi,
-                                                                         nshr=nshr,
-                                                                         timer=timer)
-                gp_heat_flux = gp_output['heat_flux']
-                self.gp_ddsddts.append(gp_ddsddt)
-                self.gp_temperatures.append(gp_temperature)
-                self.gp_heat_fluxes.append(gp_heat_flux)
-            else:
-                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
-                gp_shape_gradient = gp_shape_gradients[i]
-                gp_ddsddt = self.gp_ddsddts[i]
-                gp_heat_flux = self.gp_heat_fluxes[i]
+            gp_state_variables_new[i]['history_energy'][0] = energy_positive
+
+            self.gp_energies.append(energy_positive)
+
+            # if element_id == 59 and i == 0:
+            #     print(gp_phase, degradation, energy_positive)
+
+            # if element_id == 3310:
+            #     print((gp_strain + gp_dstrain), gp_stress, energy_positive)
+            # degradation = 1.0
 
             if is_update_stiffness:
-                self.element_stiffness[ix_(self.dof_T, self.dof_T)] += \
-                    dot(gp_shape_gradient.transpose(), dot(gp_ddsddt, gp_shape_gradient)) * gp_weight_times_jacobi_det
+                self.element_stiffness[ix_(self.dof_u, self.dof_u)] += gp_weight_times_jacobi_det * \
+                    dot(gp_b_matrix_transpose, dot(gp_ddsdde * degradation, gp_b_matrix))
+
+                self.element_stiffness[ix_(self.dof_p, self.dof_p)] += gp_weight_times_jacobi_det * \
+                ((gc / lc + 2.0 * energy_positive) * outer(gp_shape_value, gp_shape_value) +
+                 gc * lc * dot(gp_shape_gradient.transpose(), gp_shape_gradient))
+
+                # vecu = -2.0 * (1.0 - (gp_phase + gp_dphase)) * dot(gp_b_matrix_transpose, gp_stress * degradation) * gp_weight_times_jacobi_det
+                # self.element_stiffness[ix_(self.dof_u, self.dof_p)] += outer(vecu, gp_shape_value)
+                # self.element_stiffness[ix_(self.dof_p, self.dof_u)] += outer(gp_shape_value, vecu)
 
             if is_update_fint:
-                self.element_fint[self.dof_T] += \
-                    dot(gp_shape_gradient.transpose(), gp_heat_flux) * gp_weight_times_jacobi_det
+                self.element_fint[self.dof_u] += dot(gp_b_matrix_transpose, gp_stress * degradation) * gp_weight_times_jacobi_det
+
+                self.element_fint[self.dof_p] += gp_weight_times_jacobi_det * \
+                    (gc * lc * dot(gp_shape_gradient.transpose(), (gp_phase_gradient + gp_dphase_gradient)) +
+                     gc / lc * (gp_phase + gp_dphase) * gp_shape_value +
+                     2.0 * ((gp_phase + gp_dphase) - 1.0) * energy_positive * gp_shape_value)
 
     def update_element_field_variables(self) -> None:
         gp_stresses = self.gp_stresses
         gp_strains = self.gp_strains
+        gp_energies = self.gp_energies
 
         average_strain = average(gp_strains, axis=0)
         average_stress = average(gp_stresses, axis=0)
+        average_energy = average(gp_energies, axis=0)
 
         self.gp_field_variables['strain'] = array(gp_strains, dtype=DTYPE)
         self.gp_field_variables['stress'] = array(gp_stresses, dtype=DTYPE)
 
         if self.dimension == 2:
             self.element_average_field_variables['E11'] = average_strain[0]
             self.element_average_field_variables['E22'] = average_strain[1]
             self.element_average_field_variables['E12'] = average_strain[2]
             self.element_average_field_variables['S11'] = average_stress[0]
             self.element_average_field_variables['S22'] = average_stress[1]
             self.element_average_field_variables['S12'] = average_stress[2]
+            self.element_average_field_variables['ENERGY'] = average_energy
 
         elif self.dimension == 3:
             self.element_average_field_variables['E11'] = average_strain[0]
             self.element_average_field_variables['E22'] = average_strain[1]
             self.element_average_field_variables['E33'] = average_strain[2]
             self.element_average_field_variables['E12'] = average_strain[3]
             self.element_average_field_variables['E13'] = average_strain[4]
@@ -322,14 +364,14 @@
             self.element_average_field_variables['S13'] = average_stress[4]
             self.element_average_field_variables['S23'] = average_stress[5]
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
-    print_slots_dict(SolidThermalSmallStrain.__slots_dict__)
+    print_slots_dict(SolidPhaseDamageSmallStrain.__slots_dict__)
+
+    from pyfem.Job import Job
+
+    job = Job(r'..\..\..\examples\mechanical_phase\rectangle\Job-1.toml')
 
-    # from pyfem.Job import Job
-    #
-    # job = Job(r'..\..\..\examples\mechanical_thermal\rectangle\Job-1.toml')
-    #
-    # job.assembly.element_data_list[0].show()
+    job.assembly.element_data_list[0].show()
```

### Comparing `pyfem-0.1.3/src/pyfem/elements/Thermal.py` & `pyfem-0.1.4/src/pyfem/elements/Thermal.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
 
         self.element_dof_number = element_dof_number
         self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_ddof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_fint = zeros(element_dof_number, dtype=DTYPE)
-        self.element_stiffness = None  # type: ignore
+        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
         self.gp_temperatures: list[ndarray] = None  # type: ignore
         self.gp_heat_fluxes: list[ndarray] = None  # type: ignore
         self.gp_ddsddts: list[ndarray] = None  # type: ignore
 
     def update_element_material_stiffness_fint(self,
                                                is_update_material: bool = True,
```

### Comparing `pyfem-0.1.3/src/pyfem/elements/get_element_data.py` & `pyfem-0.1.4/src/pyfem/elements/get_element_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/fem/Timer.py` & `pyfem-0.1.4/src/pyfem/fem/Timer.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/Amplitude.py` & `pyfem-0.1.4/src/pyfem/io/Amplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/BC.py` & `pyfem-0.1.4/src/pyfem/io/BC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/BaseIO.py` & `pyfem-0.1.4/src/pyfem/io/BaseIO.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/Dof.py` & `pyfem-0.1.4/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/Material.py` & `pyfem-0.1.4/src/pyfem/io/Material.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     allowed_categories_types: dict = {
         None: [None],
         'Elastic': ['Isotropic'],
-        'Plastic': ['KinematicHardening'],
+        'Plastic': ['KinematicHardening', 'Crystal'],
         'ViscoElastic': ['Maxwell'],
         'Thermal': ['Isotropic'],
         'PhaseField': ['Damage'],
         'MechanicalThermal': ['Expansion']
     }
 
     allowed_keys_values: dict = {
```

### Comparing `pyfem-0.1.3/src/pyfem/io/Mesh.py` & `pyfem-0.1.4/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/Output.py` & `pyfem-0.1.4/src/pyfem/io/Output.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/Properties.py` & `pyfem-0.1.4/src/pyfem/io/Properties.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/Section.py` & `pyfem-0.1.4/src/pyfem/io/Section.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/Solver.py` & `pyfem-0.1.4/src/pyfem/io/Solver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/arguments.py` & `pyfem-0.1.4/src/pyfem/io/arguments.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/io/write_vtk.py` & `pyfem-0.1.4/src/pyfem/io/write_vtk.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/isoelements/IsoElementDiagram.py` & `pyfem-0.1.4/src/pyfem/isoelements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/isoelements/IsoElementShape.py` & `pyfem-0.1.4/src/pyfem/isoelements/IsoElementShape.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         self.shape_function = get_shape_hex8
 
         self.bc_surface_number = 6
         bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
         self.bc_surface_nodes_dict = {'s1': (0, 3, 7, 4),
                                       's2': (1, 2, 6, 5),
                                       's3': (0, 1, 5, 4),
-                                      's4': (2, 3, 6, 7),
+                                      's4': (3, 2, 6, 7),
                                       's5': (0, 1, 2, 3),
                                       's6': (4, 5, 6, 7)}
         self.bc_surface_coord_dict = {'s1': (0, -1, 1, 1),
                                       's2': (0, 1, 1, 1),
                                       's3': (1, -1, 1, 1),
                                       's4': (1, 1, 1, 1),
                                       's5': (2, -1, 1, 1),
@@ -316,14 +316,35 @@
     def set_hex20(self) -> None:
         self.dimension = 3
         self.topological_dimension = 3
         self.nodes_number = 20
         self.order = 3
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
         self.shape_function = get_shape_hex20
+
+        self.bc_surface_number = 6
+        bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
+        self.bc_surface_nodes_dict = {'s1': (0, 11, 3, 19, 7, 15, 4, 16),
+                                      's2': (1, 9, 2, 18, 6, 13, 5, 17),
+                                      's3': (0, 8, 1, 17, 5, 12, 4, 16),
+                                      's4': (3, 10, 2, 18, 6, 14, 7, 19),
+                                      's5': (0, 8, 1, 9, 2, 10, 3, 11),
+                                      's6': (4, 12, 5, 13, 6, 14, 7, 15)}
+        self.bc_surface_coord_dict = {'s1': (0, -1, 1, 1),
+                                      's2': (0, 1, 1, 1),
+                                      's3': (1, -1, 1, 1),
+                                      's4': (1, 1, 1, 1),
+                                      's5': (2, -1, 1, 1),
+                                      's6': (2, 1, 1, 1)}
+        self.bc_gp_coords_dict = {'s1': insert(bc_gp_coords, 0, -1, axis=1),
+                                  's2': insert(bc_gp_coords, 0, 1, axis=1),
+                                  's3': insert(bc_gp_coords, 1, -1, axis=1),
+                                  's4': insert(bc_gp_coords, 1, 1, axis=1),
+                                  's5': insert(bc_gp_coords, 2, -1, axis=1),
+                                  's6': insert(bc_gp_coords, 2, 1, axis=1)}
         self.diagram = IsoElementDiagram.hex20
 
 
 def get_gauss_points(dimension: int, order: int) -> tuple[ndarray, ndarray]:
     xi, weight = leggauss(order)
     if dimension == 1:
         xi = xi.reshape(len(xi), -1)
```

### Comparing `pyfem-0.1.3/src/pyfem/isoelements/derive_shape_functions.py` & `pyfem-0.1.4/src/pyfem/isoelements/derive_shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/isoelements/get_iso_element_type.py` & `pyfem-0.1.4/src/pyfem/isoelements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/isoelements/shape_functions.py` & `pyfem-0.1.4/src/pyfem/isoelements/shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.1.4/src/pyfem/materials/BaseMaterial.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.1.4/src/pyfem/materials/ElasticIsotropic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from numpy import array, outer, diag, ndarray, dot
+from numpy import array, ndarray, dot
 
 from pyfem.fem.Timer import Timer
-from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class ElasticIsotropic(BaseMaterial):
@@ -67,15 +66,15 @@
         strain = variable['strain']
         dstrain = variable['dstrain']
         stress = dot(self.tangent, strain + dstrain)
         output = {'stress': stress}
         return self.tangent, output
 
 
-def get_lame_from_young_poisson(young: float, poisson: float, plane: str) -> tuple[float, float]:
+def get_lame_from_young_poisson(E: float, nu: float, plane: str) -> tuple[float, float]:
     r"""
     Compute Lamé parameters from Young's modulus and Poisson's ratio.
 
     The relationship between Lamé parameters and Young's modulus, Poisson's
     ratio (see [1],[2]):
 
     .. math::
@@ -87,59 +86,77 @@
        \bar\lambda = {2\lambda\mu \over \lambda + 2\mu}
 
     [1] I.S. Sokolnikoff: Mathematical Theory of Elasticity. New York, 1956.
 
     [2] T.J.R. Hughes: The Finite Element Method, Linear Static and Dynamic
     Finite Element Analysis. New Jersey, 1987.
     """
-    mu = young / (2.0 * (1.0 + poisson))
-    lam = young * poisson / ((1.0 + poisson) * (1.0 - 2.0 * poisson))
+    mu = E / (2.0 * (1.0 + nu))
+    lam = E * nu / ((1.0 + nu) * (1.0 - 2.0 * nu))
 
     if plane == 'PlaneStress':
         lam = 2 * lam * mu / (lam + 2 * mu)
 
     return lam, mu
 
 
-def get_stiffness_from_lame(dim: int, lam: float, mu: float) -> ndarray:
+def get_stiffness_from_lame(dimension: int, lam: float, mu: float) -> ndarray:
     r"""
     Compute stiffness tensor corresponding to Lamé parameters.
 
     .. math::
         {\bf D}_{(2D)} = \begin{bmatrix} \lambda + 2\mu & \lambda & 0\\
         \lambda & \lambda + 2\mu & 0\\ 0 & 0 & \mu \end{bmatrix}
 
     .. math::
         {\bf D}_{(3D)} = \begin{bmatrix} \lambda + 2\mu & \lambda &
         \lambda & 0 & 0 & 0\\ \lambda & \lambda + 2\mu & \lambda & 0 & 0 & 0 \\
         \lambda & \lambda & \lambda + 2\mu & 0 & 0 & 0 \\ 0 & 0 & 0 & \mu & 0 &
         0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 & 0 & 0 & 0 & \mu\\ \end{bmatrix}
     """
-    sym = (dim + 1) * dim // 2
-    o = array([1.] * dim + [0.] * (sym - dim), dtype=DTYPE)
-    oot = outer(o, o)
-    do1 = diag(o + 1.0)
 
-    lam_array = array(lam, dtype=DTYPE)[..., None, None]
-    mu_array = array(mu, dtype=DTYPE)[..., None, None]
-    return lam_array * oot + mu_array * do1
+    # sym = (dimension + 1) * dimension // 2
+    # o = array([1.] * dimension + [0.] * (sym - dimension), dtype=DTYPE)
+    # oot = outer(o, o)
+    # do1 = diag(o + 1.0)
+    #
+    # lam_array = array(lam, dtype=DTYPE)[..., None, None]
+    # mu_array = array(mu, dtype=DTYPE)[..., None, None]
+    #
+    # D = lam_array * oot + mu_array * do1
+
+    assert dimension == 2 or dimension == 3, "Invalid dimension. Must be 2 or 3."
+
+    if dimension == 2:
+        D = array([[lam + 2 * mu, lam, 0],
+                   [lam, lam + 2 * mu, 0],
+                   [0, 0, mu]])
+    else:
+        D = array([[lam + 2 * mu, lam, lam, 0, 0, 0],
+                   [lam, lam + 2 * mu, lam, 0, 0, 0],
+                   [lam, lam, lam + 2 * mu, 0, 0, 0],
+                   [0, 0, 0, mu, 0, 0],
+                   [0, 0, 0, 0, mu, 0],
+                   [0, 0, 0, 0, 0, mu]])
 
+    return D
 
-def get_stiffness_from_young_poisson(dim: int, young: float, poisson: float, plane: str) -> ndarray:
+
+def get_stiffness_from_young_poisson(dimension: int, E: float, nu: float, plane: str) -> ndarray:
     """
     Compute stiffness tensor corresponding to Young's modulus and Poisson's
     ratio.
     """
 
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+    lam, mu = get_lame_from_young_poisson(E, nu, plane)
 
-    return get_stiffness_from_lame(dim, lam, mu)
+    return get_stiffness_from_lame(dimension, lam, mu)
 
 
-def get_stiffness_from_lame_mixed(dim: int, lam: float, mu: float) -> ndarray:
+def get_stiffness_from_lame_mixed(dimension: int, lam: float, mu: float) -> ndarray:
     r"""
     Compute stiffness tensor corresponding to Lamé parameters for mixed
     formulation.
 
     .. math::
         {\bf D}_{(2D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
         \widetilde\lambda & 0\\ \widetilde\lambda & \widetilde\lambda + 2\mu &
@@ -156,42 +173,42 @@
     where
 
     .. math::
        \widetilde\lambda = -{2\over 3} \mu
     """
     lam = - 2.0 / 3.0 * mu
 
-    return get_stiffness_from_lame(dim, lam, mu)
+    return get_stiffness_from_lame(dimension, lam, mu)
 
 
-def get_stiffness_from_young_poisson_mixed(dim: int, young: float, poisson: float, plane) -> ndarray:
+def get_stiffness_from_young_poisson_mixed(dimension: int, E: float, nu: float, plane) -> ndarray:
     """
     Compute stiffness tensor corresponding to Young's modulus and Poisson's
     ratio for mixed formulation.
     """
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+    lam, mu = get_lame_from_young_poisson(E, nu, plane)
 
-    return get_stiffness_from_lame_mixed(dim, lam, mu)
+    return get_stiffness_from_lame_mixed(dimension, lam, mu)
 
 
 def get_bulk_from_lame(lam: float, mu: float) -> float:
     r"""
     Compute bulk modulus from Lamé parameters.
 
     .. math::
         \gamma = \lambda + {2 \over 3} \mu
     """
     return lam + 2.0 * mu / 3.0
 
 
-def get_bulk_from_young_poisson(young: float, poisson: float, plane: str) -> float:
+def get_bulk_from_young_poisson(E: float, nu: float, plane: str) -> float:
     """
     Compute bulk modulus corresponding to Young's modulus and Poisson's ratio.
     """
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+    lam, mu = get_lame_from_young_poisson(E, nu, plane)
 
     return get_bulk_from_lame(lam, mu)
 
 
 def get_lame_from_stiffness(stiffness: ndarray, plane: str) -> tuple[float, float]:
     """
     Compute Lamé parameters from an isotropic stiffness tensor.
@@ -206,18 +223,18 @@
 
 def get_young_poisson_from_stiffness(stiffness: ndarray, plane: str) -> tuple[float, float]:
     """
     Compute Young's modulus and Poisson's ratio from an isotropic stiffness
     tensor.
     """
     lam, mu = get_lame_from_stiffness(stiffness, plane)
-    young = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
-    poisson = lam / (2 * lam + 2 * mu)
+    E = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
+    nu = lam / (2 * lam + 2 * mu)
 
-    return young, poisson
+    return E, nu
 
 
 if __name__ == "__main__":
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(ElasticIsotropic.__slots_dict__)
```

### Comparing `pyfem-0.1.3/src/pyfem/materials/MechanicalThermalExpansion.py` & `pyfem-0.1.4/src/pyfem/materials/MechanicalThermalExpansion.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/materials/PhaseFieldDamage.py` & `pyfem-0.1.4/src/pyfem/materials/PhaseFieldDamage.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.1.4/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
                     timer: Timer) -> tuple[ndarray, dict[str, ndarray]]:
 
-        if state_variable == {}:
+        if state_variable == {} or timer.time0 == 0.0:
             state_variable['elastic_strain'] = zeros(ntens, dtype=DTYPE)
             state_variable['plastic_strain'] = zeros(ntens, dtype=DTYPE)
             state_variable['back_stress'] = zeros(ntens, dtype=DTYPE)
             state_variable['stress'] = zeros(ntens, dtype=DTYPE)
 
         elastic_strain = deepcopy(state_variable['elastic_strain'])
         plastic_strain = deepcopy(state_variable['plastic_strain'])
@@ -195,26 +195,28 @@
         #     print(stress)
 
         state_variable_new['elastic_strain'] = elastic_strain
         state_variable_new['plastic_strain'] = plastic_strain
         state_variable_new['back_stress'] = back_stress
         state_variable_new['stress'] = stress
 
+        plastic_energy = sum(plastic_strain * stress)
+
         if self.section.type == 'PlaneStrain':
             ddsdde = delete(delete(ddsdde, 2, axis=0), 2, axis=1)
             stress = delete(stress, 2)
         elif self.section.type == 'PlaneStress':
             ddsdde = delete(delete(ddsdde, 2, axis=0), 2, axis=1)
             ddsdde[0, 0] -= lam * lam / (lam + 2 * mu)
             ddsdde[0, 1] -= lam * lam / (lam + 2 * mu)
             ddsdde[1, 0] -= lam * lam / (lam + 2 * mu)
             ddsdde[1, 1] -= lam * lam / (lam + 2 * mu)
             stress = delete(stress, 2)
 
-        output = {'stress': stress}
+        output = {'stress': stress, 'plastic_energy': plastic_energy}
 
         return ddsdde, output
 
 
 def get_smises(s: ndarray) -> float:
     if len(s) == 3:
         smises = sqrt(s[0] ** 2 + s[1] ** 2 - s[0] * s[1] + 3 * s[2] ** 2)
```

### Comparing `pyfem-0.1.3/src/pyfem/materials/ThermalIsotropic.py` & `pyfem-0.1.4/src/pyfem/materials/ThermalIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/materials/ViscoElasticMaxwell.py` & `pyfem-0.1.4/src/pyfem/materials/PlasticCrystal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,198 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
 
-from numpy import zeros, ndarray, exp, inner
+from numpy import zeros, ndarray, dot, sqrt, outer, insert, delete, ones
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
 from pyfem.utils.colors import error_style
 
 
-class ViscoElasticMaxwell(BaseMaterial):
-    """
-    广义Maxwell粘弹性材料。
+class PlasticCrystal(BaseMaterial):
+    r"""
+    晶体塑性材料。
 
     支持的截面属性：('Volume', 'PlaneStress', 'PlaneStrain')
 
-    :ivar E0: 弹性单元的弹性模量
-    :vartype E0: float
+    :ivar E: Young's modulus E
+    :vartype E: float
+
+    :ivar nu: Poisson's ratio nu
+    :vartype nu: float
+
+    :ivar yield_stress: Yield stress
+    :vartype yield_stress: float
+
+    :ivar hard: Hardening coefficient
+    :vartype hard: float
 
-    :ivar E1: 第1个粘弹性单元的弹性模量
-    :vartype E1: float
+    :ivar EBULK3: 3倍体积模量
+    :vartype EBULK3: float
 
-    :ivar E2: 第2个粘弹性单元的弹性模量
-    :vartype E2: float
+    :ivar EG: 剪切模量
+    :vartype EG: float
 
-    :ivar E3: 第3个粘弹性单元的弹性模量
-    :vartype E3: float
+    :ivar EG2: 2倍剪切模量
+    :vartype EG2: float
 
-    :ivar TAU1: 第1个粘弹性单元的时间系数
-    :vartype TAU1: float
+    :ivar EG3: 3倍剪切模量
+    :vartype EG3: float
 
-    :ivar TAU2: 第2个粘弹性单元的时间系数
-    :vartype TAU2: float
+    :ivar ELAM: 拉梅常数
+    :vartype ELAM: float
 
-    :ivar TAU3: 第3个粘弹性单元的时间系数
-    :vartype TAU3: float
+    :ivar tolerance: 判断屈服的误差容限
+    :vartype tolerance: float
+
+    :ivar total_number_of_slips: 总的滑移系数量
+    :vartype total_number_of_slips: int
+
+    :ivar h_matrix: 硬化系数矩阵
+    :vartype h_matrix: ndarray
 
-    :ivar POISSON: 泊松比
-    :vartype POISSON: float
     """
 
     __slots_dict__: dict = {
-        'E0': ('float', '弹性单元的弹性模量'),
-        'E1': ('float', '第1个粘弹性单元的弹性模量'),
-        'E2': ('float', '第2个粘弹性单元的弹性模量'),
-        'E3': ('float', '第3个粘弹性单元的弹性模量'),
-        'TAU1': ('float', '第1个粘弹性单元的时间系数'),
-        'TAU2': ('float', '第2个粘弹性单元的时间系数'),
-        'TAU3': ('float', '第3个粘弹性单元的时间系数'),
-        'POISSON': ('float', '泊松比')
+        'E': ('float', 'Young\'s modulus E'),
+        'nu': ('float', 'Poisson\'s ratio nu'),
+        'yield_stress': ('float', 'Yield stress'),
+        'hard': ('float', 'Hardening coefficient'),
+        'EBULK3': ('float', '3倍体积模量'),
+        'EG': ('float', '剪切模量'),
+        'EG2': ('float', '2倍剪切模量'),
+        'EG3': ('float', '3倍剪切模量'),
+        'ELAM': ('float', '拉梅常数'),
+        'tolerance': ('float', '判断屈服的误差容限'),
+        'total_number_of_slips': ('int', '总的滑移系数量'),
+        'h_matrix': ('ndarray', '硬化系数矩阵')
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
-        self.data_keys = ['E0', 'Poisson\'s ratio nu', 'E1', 'TAU1', 'E2', 'TAU2', 'E3', 'TAU3']
+        self.data_keys = ['Young\'s modulus E', 'Poisson\'s ratio nu', 'Yield stress', 'Hardening coefficient']
 
         if len(self.material.data) != len(self.data_keys):
             raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
             for i, key in enumerate(self.data_keys):
                 self.data_dict[key] = material.data[i]
 
-        self.E0: float = self.data_dict['E0']
-        self.E1: float = self.data_dict['E1']
-        self.E2: float = self.data_dict['E2']
-        self.E3: float = self.data_dict['E3']
-        self.TAU1: float = self.data_dict['TAU1']
-        self.TAU2: float = self.data_dict['TAU2']
-        self.TAU3: float = self.data_dict['TAU3']
-        self.POISSON: float = self.data_dict['Poisson\'s ratio nu']
+        self.E: float = self.data_dict['Young\'s modulus E']
+        self.nu: float = self.data_dict['Poisson\'s ratio nu']
+        self.yield_stress: float = self.data_dict['Yield stress']
+        self.hard: float = self.data_dict['Hardening coefficient']
+
+        self.EBULK3: float = self.E / (1.0 - 2.0 * self.nu)
+        self.EG2: float = self.E / (1.0 + self.nu)
+        self.EG: float = self.EG2 / 2.0
+        self.EG3: float = 3.0 * self.EG
+        self.ELAM: float = (self.EBULK3 - self.EG2) / 3.0
+        self.tolerance: float = 1.0e-10
+
+        self.total_number_of_slips: int = 12
+        self.h_matrix: ndarray = ones((self.total_number_of_slips, self.total_number_of_slips))
 
         self.create_tangent()
 
     def create_tangent(self):
         if self.section.type in self.allowed_section_types:
-            self.tangent = get_stiffness_from_young_poisson(self.dimension, self.E0, self.POISSON, self.section.type)
+            self.tangent = get_stiffness_from_young_poisson(self.dimension, self.E, self.nu, self.section.type)
         else:
             raise NotImplementedError(error_style(self.get_section_type_error_msg()))
 
     def get_tangent(self, variable: dict[str, ndarray],
                     state_variable: dict[str, ndarray],
                     state_variable_new: dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
                     timer: Timer) -> tuple[ndarray, dict[str, ndarray]]:
 
-        if state_variable == {}:
-            state_variable['SM1'] = zeros(ntens, dtype=DTYPE)
-            state_variable['SM2'] = zeros(ntens, dtype=DTYPE)
-            state_variable['SM3'] = zeros(ntens, dtype=DTYPE)
-
-        SM1OLD = deepcopy(state_variable['SM1'])
-        SM2OLD = deepcopy(state_variable['SM2'])
-        SM3OLD = deepcopy(state_variable['SM3'])
-
-        # if element_id == 0 and igp == 0:
-        #     print(state_variable)
-
-        dtime = timer.dtime
-        dstrain = variable['dstrain']
         strain = variable['strain']
+        dstrain = variable['dstrain']
 
-        E0 = self.E0
-        E1 = self.E1
-        E2 = self.E2
-        E3 = self.E3
-        TAU1 = self.TAU1
-        TAU2 = self.TAU2
-        TAU3 = self.TAU3
-        POISSON = self.POISSON
-
-        mu0 = 0.5 * E0 / (1.0 + POISSON)
-        mu1 = 0.5 * E1 / (1.0 + POISSON)
-        mu2 = 0.5 * E2 / (1.0 + POISSON)
-        mu3 = 0.5 * E3 / (1.0 + POISSON)
-
-        BULK = E0 / 3 / (1.0 - 2 * POISSON)
-
-        term1 = BULK + (4.0 * mu0) / 3.0
-        term2 = BULK - (2.0 * mu0) / 3.0
-
-        g = zeros((ntens, ntens), dtype=DTYPE)
+        if state_variable == {}:
+            state_variable['rho_m'] = zeros(self.total_number_of_slips, dtype=DTYPE)
+            state_variable['rho_di'] = zeros(self.total_number_of_slips, dtype=DTYPE)
+            state_variable['m_e'] = zeros((self.total_number_of_slips, 3), dtype=DTYPE)
+            state_variable['n_e'] = zeros((self.total_number_of_slips, 3), dtype=DTYPE)
+            state_variable['gamma'] = zeros(self.total_number_of_slips, dtype=DTYPE)
+
+        rho_m = deepcopy(state_variable['rho_m'])
+        rho_di = deepcopy(state_variable['rho_di'])
+        m_e = deepcopy(state_variable['m_e'])
+        n_e = deepcopy(state_variable['n_e'])
+        gamma = deepcopy(state_variable['gamma'])
+
+        rho_m = rho_m + sum(dstrain)
+
+        ddsdde = zeros((ntens, ntens), dtype=DTYPE)
+        E = self.E
+        nu = self.nu
+        lam = E * nu / ((1.0 + nu) * (1.0 - 2.0 * nu))
+        mu = E / (2.0 * (1.0 + nu))
+
+        if element_id == 0 and igp == 0:
+            print(E, nu)
+            print(rho_m)
 
+        ddsdde[:ndi, :ndi] += lam
         for i in range(ndi):
-            g[i, i] = term1
-        for i in range(1, ndi):
-            for j in range(0, i):
-                g[i, j] = term2
-                g[j, i] = term2
+            ddsdde[i, i] += 2 * mu
         for i in range(ndi, ntens):
-            g[i, i] = mu0
-
-        stress = zeros(ntens, dtype=DTYPE)
-
-        m1 = (TAU1 * mu1 - TAU1 * mu1 * exp(-dtime / TAU1)) / (mu0 * dtime)
-        m2 = (TAU2 * mu2 - TAU2 * mu2 * exp(-dtime / TAU2)) / (mu0 * dtime)
-        m3 = (TAU3 * mu3 - TAU3 * mu3 * exp(-dtime / TAU3)) / (mu0 * dtime)
-
-        term3 = 1 + m1 + m2 + m3
+            ddsdde[i, i] += mu
 
-        for i in range(ndi):
-            stress[i] = inner(g[i, 0:ndi], strain[0:ndi]) + term3 * inner(g[i, 0:ndi], dstrain[0:ndi]) + SM1OLD[i] + \
-                        SM2OLD[i] + SM3OLD[i]
-
-        for i in range(ndi, ntens):
-            stress[i] = g[i, i] * strain[i] + SM1OLD[i] + SM2OLD[i] + SM3OLD[i] + term3 * (g[i, i] * dstrain[i])
+        # dstrain = variable['dstrain']
 
-        # if element_id == 0 and igp == 0:
-        #     print(stress)
+        stress = ddsdde.dot(strain + dstrain) + sum(rho_m) * 100
 
-        SM1 = zeros(ntens, dtype=DTYPE)
-        SM2 = zeros(ntens, dtype=DTYPE)
-        SM3 = zeros(ntens, dtype=DTYPE)
+        state_variable_new['rho_m'] = rho_m
+        state_variable_new['rho_di'] = rho_di
+        state_variable_new['m_e'] = m_e
+        state_variable_new['n_e'] = n_e
+        state_variable_new['gamma'] = gamma
+        output = {'stress': stress}
 
-        for i in range(ndi):
-            SM1[i] = SM1OLD[i] + m1 * (inner(g[i, 0:ndi], dstrain[0:ndi]))
-            SM2[i] = SM2OLD[i] + m2 * (inner(g[i, 0:ndi], dstrain[0:ndi]))
-            SM3[i] = SM3OLD[i] + m3 * (inner(g[i, 0:ndi], dstrain[0:ndi]))
+        return ddsdde, output
 
-        for i in range(ndi, ntens):
-            SM1[i] = SM1OLD[i] + m1 * (g[i, i] * dstrain[i])
-            SM2[i] = SM2OLD[i] + m2 * (g[i, i] * dstrain[i])
-            SM3[i] = SM3OLD[i] + m3 * (g[i, i] * dstrain[i])
-
-        for i in range(ntens):
-            SM1[i] = exp(-dtime / TAU1) * SM1[i]
-            SM2[i] = exp(-dtime / TAU2) * SM2[i]
-            SM3[i] = exp(-dtime / TAU3) * SM3[i]
-
-        # if element_id == 0 and igp == 0:
-        #     print(SM1)
-
-        state_variable_new['SM1'] = SM1
-        state_variable_new['SM2'] = SM2
-        state_variable_new['SM3'] = SM3
 
-        ddsdde = (1 + m1 + m2 + m3) * g
+def get_smises(s: ndarray) -> float:
+    if len(s) == 3:
+        smises = sqrt(s[0] ** 2 + s[1] ** 2 - s[0] * s[1] + 3 * s[2] ** 2)
+        return float(smises)
+    elif len(s) >= 3:
+        smises = (s[0] - s[1]) ** 2 + (s[1] - s[2]) ** 2 + (s[2] - s[0]) ** 2
+        smises += 6 * sum([i ** 2 for i in s[3:]])
+        smises = sqrt(0.5 * smises)
+        return float(smises)
+    else:
+        raise NotImplementedError(error_style(f'unsupported stress dimension {len(s)}'))
 
-        output = {'stress': stress}
 
-        return ddsdde, output
+if __name__ == "__main__":
+    # from pyfem.utils.visualization import print_slots_dict
+    #
+    # print_slots_dict(PlasticCrystal.__slots_dict__)
 
+    from pyfem.Job import Job
 
-if __name__ == "__main__":
-    from pyfem.utils.visualization import print_slots_dict
+    job = Job(r'..\..\..\examples\mechanical\1element\hex8_crystal\Job-1.toml')
 
-    print_slots_dict(ViscoElasticMaxwell.__slots_dict__)
+    # job.assembly.element_data_list[0].material_data_list[0].show()
 
-    from pyfem.io.Properties import Properties
+    print(job.assembly.element_data_list[0].gp_state_variables[0]['n_e'])
 
-    props = Properties()
-    props.read_file(r'..\..\..\examples\mechanical\1element\hex8\Job-1.toml')
-    material_data = ViscoElasticMaxwell(props.materials[2], 3, props.sections[0])
-    material_data.show()
+    # job.run()
```

### Comparing `pyfem-0.1.3/src/pyfem/materials/get_material_data.py` & `pyfem-0.1.4/src/pyfem/materials/get_material_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import ElasticIsotropic
 from pyfem.materials.MechanicalThermalExpansion import MechanicalThermalExpansion
 from pyfem.materials.PhaseFieldDamage import PhaseFieldDamage
 from pyfem.materials.PlasticKinematicHardening import PlasticKinematicHardening
+from pyfem.materials.PlasticCrystal import PlasticCrystal
 from pyfem.materials.ThermalIsotropic import ThermalIsotropic
 from pyfem.materials.ViscoElasticMaxwell import ViscoElasticMaxwell
 from pyfem.utils.colors import error_style
 
 MaterialData = Union[
     BaseMaterial, MechanicalThermalExpansion, PhaseFieldDamage, PlasticKinematicHardening, ThermalIsotropic, ViscoElasticMaxwell, ElasticIsotropic]
 
 material_data_dict = {
     'ElasticIsotropic': ElasticIsotropic,
     'PlasticKinematicHardening': PlasticKinematicHardening,
+    'PlasticCrystal': PlasticCrystal,
     'ViscoElasticMaxwell': ViscoElasticMaxwell,
     'ThermalIsotropic': ThermalIsotropic,
     'MechanicalThermalExpansion': MechanicalThermalExpansion,
     'PhaseFieldDamage': PhaseFieldDamage
 }
```

### Comparing `pyfem-0.1.3/src/pyfem/mesh/MeshData.py` & `pyfem-0.1.4/src/pyfem/mesh/MeshData.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.1.4/src/pyfem/solvers/BaseSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.1.4/src/pyfem/solvers/LinearSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.1.4/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
         self.assembly = assembly
         self.solver = solver
         self.dof_solution = zeros(self.assembly.total_dof_number)
         self.PENALTY: float = 1.0e16
         self.FORCE_TOL: float = 1.0e-6
-        self.MAX_NITER: int = 32
+        self.MAX_NITER: int = 8
 
     def run(self) -> int:
         if self.assembly.props.solver.option in [None, '', 'NR', 'NewtonRaphson']:
             return self.Newton_Raphson_solve()
         elif self.assembly.props.solver.option in ['IT', 'InitialTangent']:
             return self.initial_tangent_solve()
         else:
@@ -65,24 +65,27 @@
         timer.increment = 0
         timer.frame_ids.append(0)
 
         self.assembly.update_element_field_variables()
         self.assembly.assembly_field_variables()
         write_vtk(self.assembly)
 
-        for increment in range(1, self.solver.max_increment):
+        increment = 1
+
+        for i in range(1, self.solver.max_increment):
 
             timer.time1 = timer.time0 + timer.dtime
             timer.increment = increment
 
-            print(info_style(f'increment = {increment}, time = {timer.time1}'))
+            print(info_style(f'increment = {increment}, time = {timer.time1}, dtime = {timer.dtime}'))
 
             self.assembly.ddof_solution = zeros(self.assembly.total_dof_number, dtype=DTYPE)
 
             is_convergence = False
+
             for niter in range(self.MAX_NITER):
                 self.assembly.assembly_global_stiffness()
                 fint = self.assembly.fint
                 rhs = deepcopy(self.assembly.fext)
                 if niter == 0:
                     for bc_data in self.assembly.bc_data_list:
                         amplitude_increment = bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(timer.time0)
@@ -120,21 +123,32 @@
 
             if is_convergence:
                 self.assembly.dof_solution += self.assembly.ddof_solution
                 self.assembly.update_element_data()
                 self.assembly.update_element_state_variables()
                 self.assembly.update_element_field_variables()
                 self.assembly.assembly_field_variables()
-            else:
-                raise NotImplementedError(error_style('the iteration is not convergence'))
-
-            write_vtk(self.assembly)
 
-            timer.time0 = timer.time1
-            timer.frame_ids.append(increment)
+                write_vtk(self.assembly)
+                timer.time0 = timer.time1
+                timer.frame_ids.append(increment)
+                increment += 1
+                timer.dtime *= 1.5
+                if timer.dtime >= self.solver.max_dtime:
+                    timer.dtime = self.solver.max_dtime
+                if timer.time0 + timer.dtime >= self.solver.total_time:
+                    timer.dtime = self.solver.total_time - timer.time0
+            else:
+                timer.dtime *= 0.5
+                if timer.dtime <= self.assembly.props.solver.min_dtime:
+                    raise NotImplementedError(error_style('the iteration is not convergence'))
+                self.assembly.ddof_solution = zeros(self.assembly.total_dof_number, dtype=DTYPE)
+                self.assembly.goback_element_state_variables()
+                self.assembly.update_element_data()
+                self.assembly.assembly_fint()
 
             if timer.is_done():
                 write_pvd(self.assembly)
                 break
 
         if not timer.is_done():
             print((error_style('maximum increment is reached')))
@@ -208,21 +222,24 @@
 
             if is_convergence:
                 self.assembly.dof_solution += self.assembly.ddof_solution
                 self.assembly.update_element_data()
                 self.assembly.update_element_state_variables()
                 self.assembly.update_element_field_variables()
                 self.assembly.assembly_field_variables()
-            else:
-                raise NotImplementedError(error_style('the iteration is not convergence'))
-
-            write_vtk(self.assembly)
 
-            timer.time0 = timer.time1
-            timer.frame_ids.append(increment)
+                write_vtk(self.assembly)
+                timer.time0 = timer.time1
+                timer.frame_ids.append(increment)
+                increment += 1
+            else:
+                increment -= 1
+                timer.dtime *= 0.5
+                self.assembly.goback_element_state_variables()
+                # raise NotImplementedError(error_style('the iteration is not convergence'))
 
             if timer.is_done():
                 write_pvd(self.assembly)
                 break
 
         if not timer.is_done():
             print((error_style('maximum increment is reached')))
```

### Comparing `pyfem-0.1.3/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.1.4/src/pyfem/solvers/get_solver_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.1.4/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/utils/colors.py` & `pyfem-0.1.4/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/utils/derive.py` & `pyfem-0.1.4/src/pyfem/utils/derive.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/utils/logger.py` & `pyfem-0.1.4/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/utils/mechanics.py` & `pyfem-0.1.4/src/pyfem/utils/mechanics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from numpy import zeros, ndarray, tensordot, array
+from numpy import zeros, ndarray, tensordot, array, sum
 from numpy.linalg import eig, inv
 
 from pyfem.utils.colors import error_style
 
 
 def inverse(gp_jacobis: ndarray, gp_jacobi_dets: ndarray) -> ndarray:
     """
@@ -76,45 +76,47 @@
         tensor[1, 0] = array[5]
     else:
         raise NotImplementedError(error_style(f'unsupported dimension {dimension}'))
     return tensor
 
 
 def get_decompose_energy(strain: ndarray, stress: ndarray, dimension: int):
-    strain = array_to_tensor_order_2(strain, dimension)
-    # stress = array_to_tensor_order_2(stress, dimension)
+    # strain = array_to_tensor_order_2(strain, dimension)
+    # # stress = array_to_tensor_order_2(stress, dimension)
+    #
+    # principle_strain_value, principle_strain_vector = eig(strain)
+    # # principle_stress_value, principle_stress_vector = eig(stress)
+    #
+    # strain_positive = zeros(shape=(dimension, dimension))
+    # strain_negative = zeros(shape=(dimension, dimension))
+    #
+    # # stress_positive = zeros(shape=(dimension, dimension))
+    # # stress_negative = zeros(shape=(dimension, dimension))
+    #
+    # for i in range(dimension):
+    #     strain_positive += 0.5 * (principle_strain_value[i] + abs(principle_strain_value[i])) * \
+    #                        tensordot(principle_strain_vector[:, i], principle_strain_vector[:, i], 0)
+    #
+    #     strain_negative += 0.5 * (principle_strain_value[i] - abs(principle_strain_value[i])) * \
+    #                        tensordot(principle_strain_vector[:, i], principle_strain_vector[:, i], 0)
+    #
+    #     # stress_positive += 0.5 * (principle_stress_value[i] + abs(principle_stress_value[i])) * \
+    #     #                    tensordot(principle_stress_vector[:, i], principle_stress_vector[:, i], 0)
+    #     #
+    #     # stress_negative += 0.5 * (principle_stress_value[i] - abs(principle_stress_value[i])) * \
+    #     #                    tensordot(principle_stress_vector[:, i], principle_stress_vector[:, i], 0)
+    #
+    # E = 1.0e5
+    # nu = 0.25
+    #
+    # mu = E / (2 * (1 + nu))
+    # lame = (E * nu) / ((1 + nu) * (1 - 2 * nu))
+    #
+    # energy_positive = 0.5 * lame * (0.5 * (strain.trace() + abs(strain.trace()))) ** 2 + \
+    #                   mu * (strain_positive * strain_positive).trace()
+    #
+    # energy_negative = 0.5 * lame * (0.5 * (strain.trace() - abs(strain.trace()))) ** 2 + \
+    #                   mu * (strain_negative * strain_negative).trace()
 
-    principle_strain_value, principle_strain_vector = eig(strain)
-    # principle_stress_value, principle_stress_vector = eig(stress)
+    energy_positive = 0.5 * sum(stress * strain)
 
-    strain_positive = zeros(shape=(dimension, dimension))
-    strain_negative = zeros(shape=(dimension, dimension))
-
-    # stress_positive = zeros(shape=(dimension, dimension))
-    # stress_negative = zeros(shape=(dimension, dimension))
-
-    for i in range(dimension):
-        strain_positive += 0.5 * (principle_strain_value[i] + abs(principle_strain_value[i])) * \
-                           tensordot(principle_strain_vector[:, i], principle_strain_vector[:, i], 0)
-
-        strain_negative += 0.5 * (principle_strain_value[i] - abs(principle_strain_value[i])) * \
-                           tensordot(principle_strain_vector[:, i], principle_strain_vector[:, i], 0)
-
-        # stress_positive += 0.5 * (principle_stress_value[i] + abs(principle_stress_value[i])) * \
-        #                    tensordot(principle_stress_vector[:, i], principle_stress_vector[:, i], 0)
-        #
-        # stress_negative += 0.5 * (principle_stress_value[i] - abs(principle_stress_value[i])) * \
-        #                    tensordot(principle_stress_vector[:, i], principle_stress_vector[:, i], 0)
-
-    E = 1.0e5
-    nu = 0.25
-
-    mu = E / (2 * (1 + nu))
-    lame = (E * nu) / ((1 + nu) * (1 - 2 * nu))
-
-    energy_positive = 0.5 * lame * (0.5 * (strain.trace() + abs(strain.trace()))) ** 2 + \
-                      mu * (strain_positive * strain_positive).trace()
-
-    energy_negative = 0.5 * lame * (0.5 * (strain.trace() - abs(strain.trace()))) ** 2 + \
-                      mu * (strain_negative * strain_negative).trace()
-
-    return energy_positive, energy_negative
+    return energy_positive, energy_positive
```

### Comparing `pyfem-0.1.3/src/pyfem/utils/visualization.py` & `pyfem-0.1.4/src/pyfem/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem/utils/wrappers.py` & `pyfem-0.1.4/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.3/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.1.4/src/pyfem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.1.3
+Version: 0.1.4
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -129,15 +129,15 @@
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
 #### 采用abaqus格式的网格文件 hex8.inp:
 
-```abaqus
+```
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
 *Part, name=Part-1
 *Node
```

### Comparing `pyfem-0.1.3/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.1.4/src/pyfem.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/pyfem/assembly/__init__.py
 src/pyfem/bc/BaseBC.py
 src/pyfem/bc/DirichletBC.py
 src/pyfem/bc/NeumannBCConcentrated.py
 src/pyfem/bc/NeumannBCDistributed.py
 src/pyfem/bc/NeumannBCPressure.py
 src/pyfem/bc/__init__.py
+src/pyfem/bc/derive_surface_integral.py
 src/pyfem/bc/get_bc_data.py
 src/pyfem/elements/BaseElement.py
 src/pyfem/elements/SolidPhaseDamageSmallStrain.py
 src/pyfem/elements/SolidSmallStrain.py
 src/pyfem/elements/SolidThermalSmallStrain.py
 src/pyfem/elements/Thermal.py
 src/pyfem/elements/__init__.py
@@ -52,28 +53,35 @@
 src/pyfem/isoelements/derive_shape_functions.py
 src/pyfem/isoelements/get_iso_element_type.py
 src/pyfem/isoelements/shape_functions.py
 src/pyfem/materials/BaseMaterial.py
 src/pyfem/materials/ElasticIsotropic.py
 src/pyfem/materials/MechanicalThermalExpansion.py
 src/pyfem/materials/PhaseFieldDamage.py
+src/pyfem/materials/PlasticCrystal.py
 src/pyfem/materials/PlasticKinematicHardening.py
 src/pyfem/materials/ThermalIsotropic.py
 src/pyfem/materials/ViscoElasticMaxwell.py
-src/pyfem/materials/ViscoElasticMaxwellUMAT.py
 src/pyfem/materials/__init__.py
 src/pyfem/materials/get_material_data.py
 src/pyfem/mesh/MeshData.py
 src/pyfem/mesh/__init__.py
+src/pyfem/quadrature/BaseQuadrature.py
+src/pyfem/quadrature/GaussLegendreQuadrature.py
+src/pyfem/quadrature/TetrahedronQuadrature.py
+src/pyfem/quadrature/TriangleQuadrature.py
+src/pyfem/quadrature/__init__.py
 src/pyfem/solvers/BaseSolver.py
 src/pyfem/solvers/LinearSolver.py
 src/pyfem/solvers/NonlinearSolver.py
 src/pyfem/solvers/__init__.py
 src/pyfem/solvers/get_solver_data.py
 src/pyfem/utils/IntKeyDict.py
 src/pyfem/utils/__init__.py
 src/pyfem/utils/colors.py
 src/pyfem/utils/derive.py
+src/pyfem/utils/derive_CPFEM.py
+src/pyfem/utils/derive_CPFEM2.py
 src/pyfem/utils/logger.py
 src/pyfem/utils/mechanics.py
 src/pyfem/utils/visualization.py
 src/pyfem/utils/wrappers.py
```

