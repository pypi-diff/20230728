# Comparing `tmp/mordredcommunity-2.0.1rc1.tar.gz` & `tmp/mordredcommunity-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mordredcommunity-2.0.1rc1.tar", last modified: Thu Jul 27 21:07:14 2023, max compression
+gzip compressed data, was "mordredcommunity-2.0.2.tar", last modified: Fri Jul 28 13:34:43 2023, max compression
```

## Comparing `mordredcommunity-2.0.1rc1.tar` & `mordredcommunity-2.0.2.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1493 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/LICENSE
--rw-rw-r--   0 jackson   (1000) jackson   (1000)     5756 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/PKG-INFO
--rw-r--r--   0 jackson   (1000) jackson   (1000)     5144 2023-07-21 16:14:04.000000 mordredcommunity-2.0.1rc1/README.md
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.183553 mordredcommunity-2.0.1rc1/mordred/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1954 2023-07-21 14:50:39.000000 mordredcommunity-2.0.1rc1/mordred/ABCIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1810 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/AcidBase.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1394 2023-07-21 16:05:36.000000 mordredcommunity-2.0.1rc1/mordred/AdjacencyMatrix.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      947 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Aromatic.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2949 2023-07-21 14:53:32.000000 mordredcommunity-2.0.1rc1/mordred/AtomCount.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     7796 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Autocorrelation.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3003 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BCUT.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      733 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BalabanJ.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2410 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BaryszMatrix.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      711 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BertzCT.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2711 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/BondCount.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     9304 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/CPSA.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3502 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/CarbonTypes.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     6216 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Chi.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1882 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Constitutional.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     5927 2023-07-21 14:55:24.000000 mordredcommunity-2.0.1rc1/mordred/DetourMatrix.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1273 2023-07-21 14:53:32.000000 mordredcommunity-2.0.1rc1/mordred/DistanceMatrix.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3679 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/EState.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      957 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/EccentricConnectivityIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)    20747 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/ExtendedTopochemicalAtom.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      978 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/FragmentComplexity.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1873 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Framework.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2504 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/GeometricalIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1459 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/GravitationalIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1041 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/HydrogenBond.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     7355 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/InformationContent.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2177 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/KappaShapeIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1448 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Lipinski.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1540 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/LogS.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      667 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/McGowanVolume.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2224 2023-07-21 15:02:23.000000 mordredcommunity-2.0.1rc1/mordred/MoRSE.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2718 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/MoeType.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2728 2023-07-21 15:07:03.000000 mordredcommunity-2.0.1rc1/mordred/MolecularDistanceEdge.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4271 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/MolecularId.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1655 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/MomentOfInertia.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      543 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/PBF.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4030 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/PathCount.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1565 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Polarizability.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4512 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/RingCount.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1368 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/RotatableBond.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      990 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/SLogP.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3438 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/TopoPSA.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2607 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/TopologicalCharge.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2414 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/TopologicalIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1602 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/VdwVolumeABC.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      943 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/VertexAdjacencyInformation.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2156 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/WalkCount.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1141 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/Weight.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      995 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/WienerIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2111 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/ZagrebIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      268 2023-07-21 15:05:05.000000 mordredcommunity-2.0.1rc1/mordred/__init__.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     6462 2023-07-21 16:05:30.000000 mordredcommunity-2.0.1rc1/mordred/__main__.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     8724 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_atomic_property.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/_base/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2193 2023-07-21 15:06:36.000000 mordredcommunity-2.0.1rc1/mordred/_base/__init__.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)    12279 2023-07-21 16:05:54.000000 mordredcommunity-2.0.1rc1/mordred/_base/calculator.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2430 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/context.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     9681 2023-07-21 14:52:55.000000 mordredcommunity-2.0.1rc1/mordred/_base/descriptor.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      400 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/pandas_module.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2169 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/parallel.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4323 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/result.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      435 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_base/util.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3336 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_graph_matrix.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     6191 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_matrix_attributes.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2230 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/_util.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/data/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1291 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/allred_rocow_electron_negativity.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2220 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/ionization_potential.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2553 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/mass.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1602 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/mc_gowan_volume.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1612 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/pauling_electron_negativity.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2046 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/polarizalibity78.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2510 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/polarizalibity94.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1472 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/sanderson_electron_negativity.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1569 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/data/van_der_waals_radii.txt
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/descriptors/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1044 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/descriptors/__init__.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/error/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2045 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/error/__init__.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.187553 mordredcommunity-2.0.1rc1/mordred/surface_area/
--rw-r--r--   0 jackson   (1000) jackson   (1000)      519 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/__init__.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1422 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/__main__.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2392 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/_mesh.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3433 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/surface_area/_sasa.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.191553 mordredcommunity-2.0.1rc1/mordred/tests/
--rw-r--r--   0 jackson   (1000) jackson   (1000)      633 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/Dummy.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)       28 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/__init__.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.199553 mordredcommunity-2.0.1rc1/mordred/tests/references/
--rw-r--r--   0 jackson   (1000) jackson   (1000)      349 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Aromatic.yaml
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.199553 mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/
--rw-r--r--   0 jackson   (1000) jackson   (1000)      884 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/AtomCount.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      948 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/CarbonTypes.yaml
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     9836 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/AATS.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)    10241 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/AATSC.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     9554 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/ATS.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)    10102 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/ATSC.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     8768 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/GATS.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     9170 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/MATS.yaml
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1062 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/BondTypes.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      345 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/HBond.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      577 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/Rotatable.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1525 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/CPSA.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     8654 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Chi.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2049 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Constitutional.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1546 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/DistanceEdge.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      318 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/EState.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)    10580 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/ExtendedTopochemicalAtom.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      296 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/FragmentComplexity.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      310 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Framework.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1356 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/GeometricalIndex.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2177 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/GravitationalIndex.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2546 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Indices.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4713 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/InformationContent.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      416 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Lipinski.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      861 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/LogS.yaml
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/
--rw-r--r--   0 jackson   (1000) jackson   (1000)      544 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/BCUT.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1346 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/barysz.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1072 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/detour.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1725 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/distance.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      518 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/MoRSE.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      926 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/MolecularId.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1802 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/MomentOfInertia.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3549 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/PathCount.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      532 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Polarizability.yaml
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.203553 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/
--rw-r--r--   0 jackson   (1000) jackson   (1000)      311 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/McGowanVolume.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      380 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/Vabc.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      556 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Property/Weight.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      508 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Ring.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      507 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Smarts.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      922 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/TopoPSA.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3340 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/TopologicalCharge.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)      601 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/VAdjMat.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3663 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/Walk.yaml
--rw-r--r--   0 jackson   (1000) jackson   (1000)    64187 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/structures.sdf
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1262 2023-07-21 14:36:40.000000 mordredcommunity-2.0.1rc1/mordred/tests/references/structures.smi
--rw-r--r--   0 jackson   (1000) jackson   (1000)      605 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_ABCIndex.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4227 2023-07-21 14:44:01.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_ETA.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1554 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_SASA.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      444 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_SLogP.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4732 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_VEA.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     3171 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_atomic_property.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      811 2023-07-21 16:08:22.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_attributes.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2024 2023-07-21 15:24:13.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_by_references.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      615 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_compose_descriptor.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      587 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_exceptions.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      346 2023-07-21 15:07:33.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_import_all_descriptors.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      243 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_json.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     4905 2023-07-21 16:06:00.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_mordred_main.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      565 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_pandas.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)      842 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_parallel.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1013 2023-07-21 14:36:46.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_pickle.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     2326 2023-07-21 16:12:42.000000 mordredcommunity-2.0.1rc1/mordred/tests/test_result_type.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/
--rw-rw-r--   0 jackson   (1000) jackson   (1000)     5756 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/PKG-INFO
--rw-rw-r--   0 jackson   (1000) jackson   (1000)     4880 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/SOURCES.txt
--rw-rw-r--   0 jackson   (1000) jackson   (1000)        1 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/dependency_links.txt
--rw-rw-r--   0 jackson   (1000) jackson   (1000)       98 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/requires.txt
--rw-rw-r--   0 jackson   (1000) jackson   (1000)        8 2023-07-27 21:07:14.000000 mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/top_level.txt
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1168 2023-07-27 21:06:38.000000 mordredcommunity-2.0.1rc1/pyproject.toml
--rw-rw-r--   0 jackson   (1000) jackson   (1000)       38 2023-07-27 21:07:14.207553 mordredcommunity-2.0.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.884570 mordredcommunity-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-28 13:34:43.884570 mordredcommunity-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.872570 mordredcommunity-2.0.2/mordred/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/ABCIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/AcidBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/AdjacencyMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Aromatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/AtomCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/BCUT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/BalabanJ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/BaryszMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/BertzCT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/BondCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/CPSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/CarbonTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Chi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Constitutional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/DetourMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/DistanceMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/EState.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/EccentricConnectivityIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/ExtendedTopochemicalAtom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/FragmentComplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/GeometricalIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/GravitationalIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/HydrogenBond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/InformationContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/KappaShapeIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Lipinski.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/LogS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/McGowanVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/MoRSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/MoeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/MolecularDistanceEdge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/MolecularId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/MomentOfInertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/PBF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/PathCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Polarizability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/RingCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/RotatableBond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/SLogP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/TopoPSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/TopologicalCharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/TopologicalIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/VdwVolumeABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/VertexAdjacencyInformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/WalkCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/Weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/WienerIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/ZagrebIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_atomic_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.872570 mordredcommunity-2.0.2/mordred/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/pandas_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_base/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_graph_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_matrix_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.876570 mordredcommunity-2.0.2/mordred/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/allred_rocow_electron_negativity.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/ionization_potential.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/mass.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/mc_gowan_volume.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/pauling_electron_negativity.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/polarizalibity78.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/polarizalibity94.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/sanderson_electron_negativity.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/data/van_der_waals_radii.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.876570 mordredcommunity-2.0.2/mordred/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/descriptors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.876570 mordredcommunity-2.0.2/mordred/error/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.876570 mordredcommunity-2.0.2/mordred/surface_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/surface_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/surface_area/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/surface_area/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/surface_area/_sasa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.876570 mordredcommunity-2.0.2/mordred/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/Dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.880570 mordredcommunity-2.0.2/mordred/tests/references/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Aromatic.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.880570 mordredcommunity-2.0.2/mordred/tests/references/Atom/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Atom/AtomCount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Atom/CarbonTypes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.880570 mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/AATS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/AATSC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/ATS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/ATSC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/GATS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/MATS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.880570 mordredcommunity-2.0.2/mordred/tests/references/Bond/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Bond/BondTypes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Bond/HBond.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Bond/Rotatable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/CPSA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Chi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Constitutional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/DistanceEdge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/EState.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/ExtendedTopochemicalAtom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/FragmentComplexity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Framework.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/GeometricalIndex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/GravitationalIndex.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Indices.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/InformationContent.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Lipinski.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/LogS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.880570 mordredcommunity-2.0.2/mordred/tests/references/Matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Matrix/BCUT.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Matrix/barysz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Matrix/detour.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Matrix/distance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/MoRSE.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/MolecularId.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/MomentOfInertia.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/PathCount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Polarizability.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.884570 mordredcommunity-2.0.2/mordred/tests/references/Property/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Property/McGowanVolume.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Property/Vabc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Property/Weight.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Ring.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Smarts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/TopoPSA.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/TopologicalCharge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/VAdjMat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/Walk.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    64187 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/structures.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/references/structures.smi
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_ABCIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_ETA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_SASA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_SLogP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_VEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_atomic_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_by_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_compose_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_import_all_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_mordred_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/mordred/tests/test_result_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:34:43.884570 mordredcommunity-2.0.2/mordredcommunity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-28 13:34:43.000000 mordredcommunity-2.0.2/mordredcommunity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-28 13:34:43.000000 mordredcommunity-2.0.2/mordredcommunity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:34:43.000000 mordredcommunity-2.0.2/mordredcommunity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 13:34:43.000000 mordredcommunity-2.0.2/mordredcommunity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 13:34:43.000000 mordredcommunity-2.0.2/mordredcommunity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-28 13:34:31.000000 mordredcommunity-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:34:43.884570 mordredcommunity-2.0.2/setup.cfg
```

### Comparing `mordredcommunity-2.0.1rc1/LICENSE` & `mordredcommunity-2.0.2/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2017, Hirotomo Moriwaki
+Copyright (c) 2023, Jackson Burns and the mordredcommunity Team
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `mordredcommunity-2.0.1rc1/PKG-INFO` & `mordredcommunity-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mordredcommunity
-Version: 2.0.1rc1
+Version: 2.0.2
 Summary: Community-Maintained Version of mordred
 Author-email: Jackson Burns <jwburns@mit.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/JacksonBurns/mordred-community
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
 
 # mordred-community
 Community maintained version of the [mordred molecular descriptor calculator](https://github.com/mordred-descriptor/mordred) which is no longer maintained.
```

### Comparing `mordredcommunity-2.0.1rc1/README.md` & `mordredcommunity-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/ABCIndex.py` & `mordredcommunity-2.0.2/mordred/ABCIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/AcidBase.py` & `mordredcommunity-2.0.2/mordred/AcidBase.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/AdjacencyMatrix.py` & `mordredcommunity-2.0.2/mordred/AdjacencyMatrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 
 from ._base import Descriptor
 from ._graph_matrix import AdjacencyMatrix as A
 from ._matrix_attributes import SM1, methods, get_method
 
 __all__ = ("AdjacencyMatrix",)
 
-try:
-    from importlib.metadata import version
-except ImportError:
-    from importlib_metadata import version
-
 _version_remove_SM1_A = StrictVersion("1.1.0")
 
 
 class AdjacencyMatrix(Descriptor):
     r"""adjacency matrix descriptor.
 
     :type type: :py:class:`str`
@@ -41,17 +36,13 @@
     def parameters(self):
         return (self._type,)
 
     def __init__(self, type="SpMax"):
         self._type = get_method(type)
 
     def dependencies(self):
-        return {
-            "result": self._type(
-                A(self.explicit_hydrogens), self.explicit_hydrogens, self.kekulize
-            )
-        }
+        return {"result": self._type(A(self.explicit_hydrogens), self.explicit_hydrogens, self.kekulize)}
 
     def calculate(self, result):
         return result
 
     rtype = float
```

### Comparing `mordredcommunity-2.0.1rc1/mordred/Aromatic.py` & `mordredcommunity-2.0.2/mordred/Aromatic.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/AtomCount.py` & `mordredcommunity-2.0.2/mordred/AtomCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/Autocorrelation.py` & `mordredcommunity-2.0.2/mordred/Autocorrelation.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/BCUT.py` & `mordredcommunity-2.0.2/mordred/BCUT.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/BalabanJ.py` & `mordredcommunity-2.0.2/mordred/BalabanJ.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/BaryszMatrix.py` & `mordredcommunity-2.0.2/mordred/BaryszMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/BertzCT.py` & `mordredcommunity-2.0.2/mordred/BertzCT.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/BondCount.py` & `mordredcommunity-2.0.2/mordred/BondCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/CPSA.py` & `mordredcommunity-2.0.2/mordred/CPSA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/CarbonTypes.py` & `mordredcommunity-2.0.2/mordred/CarbonTypes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/Chi.py` & `mordredcommunity-2.0.2/mordred/Chi.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/Constitutional.py` & `mordredcommunity-2.0.2/mordred/Constitutional.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/DetourMatrix.py` & `mordredcommunity-2.0.2/mordred/DetourMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/DistanceMatrix.py` & `mordredcommunity-2.0.2/mordred/DistanceMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/EState.py` & `mordredcommunity-2.0.2/mordred/EState.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/EccentricConnectivityIndex.py` & `mordredcommunity-2.0.2/mordred/EccentricConnectivityIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/ExtendedTopochemicalAtom.py` & `mordredcommunity-2.0.2/mordred/ExtendedTopochemicalAtom.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/FragmentComplexity.py` & `mordredcommunity-2.0.2/mordred/FragmentComplexity.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/Framework.py` & `mordredcommunity-2.0.2/mordred/Framework.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/GeometricalIndex.py` & `mordredcommunity-2.0.2/mordred/GeometricalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/GravitationalIndex.py` & `mordredcommunity-2.0.2/mordred/GravitationalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/HydrogenBond.py` & `mordredcommunity-2.0.2/mordred/HydrogenBond.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/InformationContent.py` & `mordredcommunity-2.0.2/mordred/InformationContent.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/KappaShapeIndex.py` & `mordredcommunity-2.0.2/mordred/KappaShapeIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/Lipinski.py` & `mordredcommunity-2.0.2/mordred/Lipinski.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/LogS.py` & `mordredcommunity-2.0.2/mordred/LogS.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/McGowanVolume.py` & `mordredcommunity-2.0.2/mordred/McGowanVolume.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/MoRSE.py` & `mordredcommunity-2.0.2/mordred/MoRSE.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/MoeType.py` & `mordredcommunity-2.0.2/mordred/MoeType.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/MolecularDistanceEdge.py` & `mordredcommunity-2.0.2/mordred/MolecularDistanceEdge.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/MolecularId.py` & `mordredcommunity-2.0.2/mordred/MolecularId.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/MomentOfInertia.py` & `mordredcommunity-2.0.2/mordred/MomentOfInertia.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/PBF.py` & `mordredcommunity-2.0.2/mordred/PBF.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/PathCount.py` & `mordredcommunity-2.0.2/mordred/PathCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/Polarizability.py` & `mordredcommunity-2.0.2/mordred/Polarizability.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/RingCount.py` & `mordredcommunity-2.0.2/mordred/RingCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/RotatableBond.py` & `mordredcommunity-2.0.2/mordred/RotatableBond.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/SLogP.py` & `mordredcommunity-2.0.2/mordred/SLogP.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/TopoPSA.py` & `mordredcommunity-2.0.2/mordred/TopoPSA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/TopologicalCharge.py` & `mordredcommunity-2.0.2/mordred/TopologicalCharge.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/TopologicalIndex.py` & `mordredcommunity-2.0.2/mordred/TopologicalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/VdwVolumeABC.py` & `mordredcommunity-2.0.2/mordred/VdwVolumeABC.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/VertexAdjacencyInformation.py` & `mordredcommunity-2.0.2/mordred/VertexAdjacencyInformation.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/WalkCount.py` & `mordredcommunity-2.0.2/mordred/WalkCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/Weight.py` & `mordredcommunity-2.0.2/mordred/Weight.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/WienerIndex.py` & `mordredcommunity-2.0.2/mordred/WienerIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/ZagrebIndex.py` & `mordredcommunity-2.0.2/mordred/ZagrebIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/__main__.py` & `mordredcommunity-2.0.2/mordred/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 from rdkit import Chem
 
 from . import Calculator, descriptors
 from ._base import get_descriptors_in_module
 from ._util import PathType, module_prog
 from .error import Missing, MissingValueBase
 
-try:
-    from importlib.metadata import version
-except ImportError:
-    from importlib_metadata import version
+from importlib.metadata import version
 
 __version__ = version("mordredcommunity")
 
 
 def smiles_parser(path):
     with open(path) as file:
         for line in file:
@@ -99,17 +96,15 @@
     parser.add_argument(
         "--version",
         action="version",
         help="input molecular file",
         version="{}-{}".format(__package__, __version__),
     )
     parser.add_argument("input", type=PathType, nargs="+", metavar="INPUT")
-    parser.add_argument(
-        "-t", "--type", action=ParserAction, help="input filetype (default: auto)"
-    )
+    parser.add_argument("-t", "--type", action=ParserAction, help="input filetype (default: auto)")
     parser.add_argument(
         "-o",
         "--output",
         default="-",
         type=argparse.FileType("w"),
         help="output file path (default: stdout)",
     )
@@ -134,24 +129,20 @@
     parser.add_argument(
         "-3",
         "--3D",
         action="store_true",
         dest="with3D",
         help="use 3D descriptors (require sdf or mol file)",
     )
-    parser.add_argument(
-        "-v", "--verbosity", action="count", default=0, help="verbosity"
-    )
+    parser.add_argument("-v", "--verbosity", action="count", default=0, help="verbosity")
 
     return parser
 
 
-def main_process(
-    input, parser, output, nproc, quiet, stream, descriptor, with3D, verbosity
-):
+def main_process(input, parser, output, nproc, quiet, stream, descriptor, with3D, verbosity):
     mols = (m for i in input for m in parser(i))
 
     if output.isatty():
         quiet = True
 
     if stream:
         N = None
@@ -165,21 +156,15 @@
     if verbosity >= 2:
         calc._debug = True
 
     if len(descriptor) == 0:
         calc.register(descriptors, ignore_3D=not with3D)
     else:
         calc.register(
-            (
-                d
-                for m in descriptor
-                for d in get_descriptors_in_module(
-                    import_module("." + m, __package__), False
-                )
-            ),
+            (d for m in descriptor for d in get_descriptors_in_module(import_module("." + m, __package__), False)),
             ignore_3D=not with3D,
         )
 
     with output:
         write_row(output, ["name"] + [str(d) for d in calc.descriptors])
 
         def warning(name, v, err_set):
@@ -215,19 +200,15 @@
             else:
                 name = Chem.MolToSmiles(result.mol)
 
             write_row(output, [name] + [pretty(name, v, err_set) for v in result])
 
 
 def write_row(file, data):
-    file.write(
-        ",".join(
-            str(v).replace('"', '""').replace("\n", "").replace("\r", "") for v in data
-        )
-    )
+    file.write(",".join(str(v).replace('"', '""').replace("\n", "").replace("\r", "") for v in data))
     file.write("\n")
 
 
 def main(args=None):
     parser = make_parser()
     p = parser.parse_args(args)
     return main_process(
```

### Comparing `mordredcommunity-2.0.1rc1/mordred/_atomic_property.py` & `mordredcommunity-2.0.2/mordred/_atomic_property.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_base/__init__.py` & `mordredcommunity-2.0.2/mordred/_base/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_base/calculator.py` & `mordredcommunity-2.0.2/mordred/_base/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 
 from .._util import Capture, DummyBar
 from ..error import Error, Missing, MultipleFragments, DuplicatedDescriptorName
 from .result import Result
 from .context import Context
 from .descriptor import Descriptor, MissingValueException, is_descriptor_class
 
-try:
-    from importlib.metadata import version as importlib_version
-except ImportError:
-    from importlib_metadata import version as importlib_version
+from importlib.metadata import version as importlib_version
 
 __version__ = importlib_version("mordredcommunity")
 
 try:
     from tqdm import tqdm
     from .._util import NotebookWrapper
 except ImportError:
@@ -288,28 +285,24 @@
 
         :type id: int
         :param id: conformer id
 
         :rtype: Result[scalar or Error]
         :returns: iterator of descriptor and value
         """
-        return self._wrap_result(
-            mol, self._calculate(Context.from_calculator(self, mol, id))
-        )
+        return self._wrap_result(mol, self._calculate(Context.from_calculator(self, mol, id)))
 
     def _wrap_result(self, mol, r):
         return Result(mol, r, self._descriptors)
 
     def _serial(self, mols, nmols, quiet, ipynb, id):
         with self._progress(quiet, nmols, ipynb) as bar:
             for m in mols:
                 with Capture() as capture:
-                    r = self._wrap_result(
-                        m, self._calculate(Context.from_calculator(self, m, id))
-                    )
+                    r = self._wrap_result(m, self._calculate(Context.from_calculator(self, m, id)))
 
                 for e in capture.result:
                     e = e.rstrip()
                     if not e:
                         continue
 
                     bar.write(e, file=capture.orig)
@@ -379,17 +372,15 @@
 
         if hasattr(mols, "__len__"):
             nmols = len(mols)
 
         if nproc == 1:
             return self._serial(mols, nmols=nmols, quiet=quiet, ipynb=ipynb, id=id)
         else:
-            return self._parallel(
-                mols, nproc, nmols=nmols, quiet=quiet, ipynb=ipynb, id=id
-            )
+            return self._parallel(mols, nproc, nmols=nmols, quiet=quiet, ipynb=ipynb, id=id)
 
     def pandas(self, mols, nproc=None, nmols=None, quiet=False, ipynb=False, id=-1):
         r"""Calculate descriptors over mols.
 
         Returns:
             pandas.DataFrame
```

### Comparing `mordredcommunity-2.0.1rc1/mordred/_base/context.py` & `mordredcommunity-2.0.2/mordred/_base/context.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_base/descriptor.py` & `mordredcommunity-2.0.2/mordred/_base/descriptor.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_base/parallel.py` & `mordredcommunity-2.0.2/mordred/_base/parallel.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_base/result.py` & `mordredcommunity-2.0.2/mordred/_base/result.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_graph_matrix.py` & `mordredcommunity-2.0.2/mordred/_graph_matrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_matrix_attributes.py` & `mordredcommunity-2.0.2/mordred/_matrix_attributes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/_util.py` & `mordredcommunity-2.0.2/mordred/_util.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/allred_rocow_electron_negativity.txt` & `mordredcommunity-2.0.2/mordred/data/allred_rocow_electron_negativity.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/ionization_potential.txt` & `mordredcommunity-2.0.2/mordred/data/ionization_potential.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/mass.txt` & `mordredcommunity-2.0.2/mordred/data/mass.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/mc_gowan_volume.txt` & `mordredcommunity-2.0.2/mordred/data/mc_gowan_volume.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/pauling_electron_negativity.txt` & `mordredcommunity-2.0.2/mordred/data/pauling_electron_negativity.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/polarizalibity78.txt` & `mordredcommunity-2.0.2/mordred/data/polarizalibity78.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/polarizalibity94.txt` & `mordredcommunity-2.0.2/mordred/data/polarizalibity94.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/sanderson_electron_negativity.txt` & `mordredcommunity-2.0.2/mordred/data/sanderson_electron_negativity.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/data/van_der_waals_radii.txt` & `mordredcommunity-2.0.2/mordred/data/van_der_waals_radii.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/descriptors/__init__.py` & `mordredcommunity-2.0.2/mordred/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/error/__init__.py` & `mordredcommunity-2.0.2/mordred/error/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/surface_area/__init__.py` & `mordredcommunity-2.0.2/mordred/surface_area/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/surface_area/__main__.py` & `mordredcommunity-2.0.2/mordred/surface_area/__main__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/surface_area/_mesh.py` & `mordredcommunity-2.0.2/mordred/surface_area/_mesh.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/surface_area/_sasa.py` & `mordredcommunity-2.0.2/mordred/surface_area/_sasa.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/Dummy.py` & `mordredcommunity-2.0.2/mordred/tests/Dummy.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/AtomCount.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Atom/AtomCount.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Atom/CarbonTypes.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Atom/CarbonTypes.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/AATS.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/AATS.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/AATSC.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/AATSC.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/ATS.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/ATS.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/ATSC.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/ATSC.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/GATS.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/GATS.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Autocorrelation/MATS.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Autocorrelation/MATS.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/BondTypes.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Bond/BondTypes.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Bond/Rotatable.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Bond/Rotatable.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/CPSA.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/CPSA.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Chi.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Chi.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Constitutional.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Constitutional.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/DistanceEdge.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/DistanceEdge.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/ExtendedTopochemicalAtom.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/ExtendedTopochemicalAtom.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/GeometricalIndex.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/GeometricalIndex.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/GravitationalIndex.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/GravitationalIndex.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Indices.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Indices.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/InformationContent.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/InformationContent.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/LogS.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/LogS.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/BCUT.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Matrix/BCUT.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/barysz.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Matrix/barysz.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/detour.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Matrix/detour.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Matrix/distance.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Matrix/distance.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/MoRSE.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/MoRSE.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/MolecularId.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/MolecularId.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/MomentOfInertia.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/MomentOfInertia.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/PathCount.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/PathCount.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Polarizability.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Polarizability.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Property/Weight.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Property/Weight.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/TopoPSA.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/TopoPSA.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/TopologicalCharge.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/TopologicalCharge.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/VAdjMat.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/VAdjMat.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/Walk.yaml` & `mordredcommunity-2.0.2/mordred/tests/references/Walk.yaml`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/structures.sdf` & `mordredcommunity-2.0.2/mordred/tests/references/structures.sdf`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/references/structures.smi` & `mordredcommunity-2.0.2/mordred/tests/references/structures.smi`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_ABCIndex.py` & `mordredcommunity-2.0.2/mordred/tests/test_ABCIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_ETA.py` & `mordredcommunity-2.0.2/mordred/tests/test_ETA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_SASA.py` & `mordredcommunity-2.0.2/mordred/tests/test_SASA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_VEA.py` & `mordredcommunity-2.0.2/mordred/tests/test_VEA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_atomic_property.py` & `mordredcommunity-2.0.2/mordred/tests/test_atomic_property.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_attributes.py` & `mordredcommunity-2.0.2/mordred/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_by_references.py` & `mordredcommunity-2.0.2/mordred/tests/test_by_references.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_compose_descriptor.py` & `mordredcommunity-2.0.2/mordred/tests/test_compose_descriptor.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_exceptions.py` & `mordredcommunity-2.0.2/mordred/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_mordred_main.py` & `mordredcommunity-2.0.2/mordred/tests/test_mordred_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 
 from .. import Calculator, descriptors
 from ..__main__ import main as mordred
 
 Nd2D = len(Calculator(descriptors, ignore_3D=True).descriptors)
 Nd3D = len(Calculator(descriptors, ignore_3D=False).descriptors)
 
-try:
-    from importlib.metadata import version
-except ImportError:
-    from importlib_metadata import version
+from importlib.metadata import version
 
 __version__ = version("mordredcommunity")
 
 
 def in_(a, s):
     assert a in s, "{!r} not in {!r}".format(a, s)
 
@@ -79,18 +76,15 @@
 
 def test_no_args():
     stdout, stderr, exitcode = command(mordred)
     assert exitcode == 2
     assert stdout == ""
     in_("usage:", stderr)
     # python3 or python2
-    assert (
-        "the following arguments are required: INPUT" in stderr
-        or "too few arguments" in stderr
-    )
+    assert "the following arguments are required: INPUT" in stderr or "too few arguments" in stderr
 
 
 def test_help():
     stdout, stderr, exitcode = command(mordred, "-h")
     assert exitcode == 0
     assert stderr == ""
     in_("usage:", stdout)
@@ -147,17 +141,15 @@
 
 def test_sdf():
     with isolate():
         mol = Chem.MolFromSmiles("c1ccccc1")
         mol.SetProp("_Name", "Benzene")
         Chem.MolToMolFile(mol, "input.sdf")
 
-        stdout, stderr, exitcode = command(
-            mordred, "input.sdf", "-q", "-o", "output.csv"
-        )
+        stdout, stderr, exitcode = command(mordred, "input.sdf", "-q", "-o", "output.csv")
 
         assert exitcode == 0
         assert stdout == ""
         assert stderr == ""
         output = open("output.csv").read()
         assert number_of_field(output) == Nd2D
         assert output.split("\n")[1].split(",")[0] == "Benzene"
@@ -166,17 +158,15 @@
 def test_sdf_3D():
     with isolate():
         mol = Chem.MolFromSmiles("c1ccccc1")
         Chem.EmbedMolecule(mol)
         mol.SetProp("_Name", "Benzene")
         Chem.MolToMolFile(mol, "input.sdf")
 
-        stdout, stderr, exitcode = command(
-            mordred, "input.sdf", "-q", "-o", "output.csv", "-3"
-        )
+        stdout, stderr, exitcode = command(mordred, "input.sdf", "-q", "-o", "output.csv", "-3")
 
         assert exitcode == 0
         assert stdout == ""
         assert stderr == ""
         output = open("output.csv").read()
         assert number_of_field(output) == Nd3D
         assert output.split("\n")[1].split(",")[0] == "Benzene"
```

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_pandas.py` & `mordredcommunity-2.0.2/mordred/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_parallel.py` & `mordredcommunity-2.0.2/mordred/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_pickle.py` & `mordredcommunity-2.0.2/mordred/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordred/tests/test_result_type.py` & `mordredcommunity-2.0.2/mordred/tests/test_result_type.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/PKG-INFO` & `mordredcommunity-2.0.2/mordredcommunity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mordredcommunity
-Version: 2.0.1rc1
+Version: 2.0.2
 Summary: Community-Maintained Version of mordred
 Author-email: Jackson Burns <jwburns@mit.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/JacksonBurns/mordred-community
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE
 
 # mordred-community
 Community maintained version of the [mordred molecular descriptor calculator](https://github.com/mordred-descriptor/mordred) which is no longer maintained.
```

### Comparing `mordredcommunity-2.0.1rc1/mordredcommunity.egg-info/SOURCES.txt` & `mordredcommunity-2.0.2/mordredcommunity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mordredcommunity-2.0.1rc1/pyproject.toml` & `mordredcommunity-2.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mordredcommunity"
-version = "2.0.1rc1"
+version = "2.0.2"
 authors = [{ name = "Jackson Burns", email = "jwburns@mit.edu" }]
 license = { text = "BSD-3-Clause" }
 description = "Community-Maintained Version of mordred"
 classifiers = [
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 urls = { Homepage = "https://github.com/JacksonBurns/mordred-community" }
-requires-python = ">=3.7"
-dependencies = [
-    "rdkit",
-    "six",
-    "numpy",
-    "networkx",
-    "importlib-metadata ; python_version < '3.8'",
-]
+requires-python = ">=3.8"
+dependencies = ["rdkit", "six", "numpy", "networkx"]
 
 [project.optional-dependencies]
 full = ["pandas", "tqdm", "pyyaml"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

