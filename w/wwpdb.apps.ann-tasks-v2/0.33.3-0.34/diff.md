# Comparing `tmp/wwpdb.apps.ann_tasks_v2-0.33.3.tar.gz` & `tmp/wwpdb.apps.ann_tasks_v2-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ann_tasks_v2-0.33.3.tar", last modified: Wed Jul 26 01:10:21 2023, max compression
+gzip compressed data, was "wwpdb.apps.ann_tasks_v2-0.34.tar", last modified: Fri Jul 28 11:32:33 2023, max compression
```

## Comparing `wwpdb.apps.ann_tasks_v2-0.33.3.tar` & `wwpdb.apps.ann_tasks_v2-0.34.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.357967 wwpdb.apps.ann_tasks_v2-0.33.3/
--rw-r--r--   0 vsts      (1001) docker     (123)      786 2023-07-26 01:10:21.357967 wwpdb.apps.ann_tasks_v2-0.33.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-26 01:10:21.357967 wwpdb.apps.ann_tasks_v2-0.33.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2540 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.337966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.341966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.341966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/
--rw-r--r--   0 vsts      (1001) docker     (123)      152 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.341966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/assembly/
--rw-r--r--   0 vsts      (1001) docker     (123)    39726 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
--rw-r--r--   0 vsts      (1001) docker     (123)    46849 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.341966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/
--rw-r--r--   0 vsts      (1001) docker     (123)     5712 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/Check.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7768 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4947 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4344 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3727 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3138 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6865 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.341966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33685 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16936 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.345966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/density/
--rw-r--r--   0 vsts      (1001) docker     (123)      998 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/density/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.345966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.345966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/
--rw-r--r--   0 vsts      (1001) docker     (123)     2573 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4448 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3981 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19613 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5646 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.345966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/
--rw-r--r--   0 vsts      (1001) docker     (123)     6295 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14499 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12364 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12679 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.345966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/
--rw-r--r--   0 vsts      (1001) docker     (123)    10620 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12969 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18806 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11248 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.345966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    15912 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9923 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.345966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/link/
--rw-r--r--   0 vsts      (1001) docker     (123)     3057 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/link/Link.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/link/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.349966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/
--rw-r--r--   0 vsts      (1001) docker     (123)     3231 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4323 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3336 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4763 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5394 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4764 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3305 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3716 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3561 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.349966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nafeatures/
--rw-r--r--   0 vsts      (1001) docker     (123)     2610 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.349966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/
--rw-r--r--   0 vsts      (1001) docker     (123)    16217 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6954 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8475 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3526 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.349966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/
--rw-r--r--   0 vsts      (1001) docker     (123)     1540 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2010 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/Related.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.349966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/
--rw-r--r--   0 vsts      (1001) docker     (123)     8209 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24814 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/
--rw-r--r--   0 vsts      (1001) docker     (123)     8612 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    80925 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33069 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/secstruct/
--rw-r--r--   0 vsts      (1001) docker     (123)     3406 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/site/
--rw-r--r--   0 vsts      (1001) docker     (123)     3094 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/site/Site.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/site/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/solvent/
--rw-r--r--   0 vsts      (1001) docker     (123)     3037 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/status/
--rw-r--r--   0 vsts      (1001) docker     (123)    32859 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/status/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/transformCoord/
--rw-r--r--   0 vsts      (1001) docker     (123)     3759 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     6454 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3600 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1509 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3451 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4026 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8388 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3396 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4790 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3021 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4071 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/validate/
--rw-r--r--   0 vsts      (1001) docker     (123)    10304 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/validate/Validate.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/validate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.353967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/view3d/
--rw-r--r--   0 vsts      (1001) docker     (123)     5085 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.357967 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)     5627 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    40112 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)   177046 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15293 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    73514 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16955 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-26 01:07:01.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-26 01:10:21.341966 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      786 2023-07-26 01:10:21.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5436 2023-07-26 01:10:21.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-26 01:10:21.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-26 01:09:25.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      323 2023-07-26 01:10:21.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-26 01:10:21.000000 wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.553663 wwpdb.apps.ann_tasks_v2-0.34/
+-rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-07-28 11:32:33.553663 wwpdb.apps.ann_tasks_v2-0.34/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-28 11:32:33.553663 wwpdb.apps.ann_tasks_v2-0.34/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2540 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.521663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.525663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.525663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.525663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/assembly/
+-rw-r--r--   0 vsts      (1001) docker     (123)    39726 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    46849 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.529663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5712 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/Check.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7768 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4947 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4344 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3727 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3138 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6865 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.529663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33814 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16936 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.529663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/density/
+-rw-r--r--   0 vsts      (1001) docker     (123)      998 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/density/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.529663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.533663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2573 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4448 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3981 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19613 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5646 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.533663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6295 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14499 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12364 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12679 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.537663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10620 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12969 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18806 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11248 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.537663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    15912 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9923 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.537663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/link/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3057 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/link/Link.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/link/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.541663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3231 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4323 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3336 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4763 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5394 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4764 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3305 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3716 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3561 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.541663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nafeatures/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2610 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.541663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    16217 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6954 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8475 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3526 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.541663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1540 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2010 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/Related.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.545663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8209 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24814 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.545663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8612 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    80925 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33069 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.545663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/secstruct/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3406 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.545663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/site/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3094 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/site/Site.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/site/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.545663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/solvent/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3037 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.549663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/status/
+-rw-r--r--   0 vsts      (1001) docker     (123)    32859 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/status/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.549663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/transformCoord/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3759 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.549663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6454 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3600 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1509 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3451 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4026 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8388 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3396 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4790 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3021 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4071 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.553663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/validate/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10304 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/validate/Validate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/validate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.553663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/view3d/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5085 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.553663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5627 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    40112 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   177046 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15293 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    73514 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16955 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 11:30:22.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 11:32:33.525663 wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-07-28 11:32:33.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5436 2023-07-28 11:32:33.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 11:32:33.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 11:31:52.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      323 2023-07-28 11:32:33.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-28 11:32:33.000000 wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/PKG-INFO` & `wwpdb.apps.ann_tasks_v2-0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.33.3
+Version: 0.34
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/setup.py` & `wwpdb.apps.ann_tasks_v2-0.34/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/Check.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/Check.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         for item in self.__corres_items:
             self.__corresInfo[item] = cifObj.GetSingleValue("correspondence_information", item)
         #
         self.__corresInfo["values"] = self.__getMissingAndInsistentValues(cifObj)
         self.__ligandInfo = cifObj.GetValue("ligand_information")
         #
         self.__EmFsc143CutOff = (cifObj.GetSingleValue("correspondence_information", "fsc_143_cut_off") == "yes")
-        if ("emdbid" in self.__corresInfo) and self.__corresInfo["emdbid"]and ("pdbid" in self.__corresInfo) and self.__corresInfo["pdbid"]:
+        if ("emdbid" in self.__corresInfo) and self.__corresInfo["emdbid"] and ("pdbid" in self.__corresInfo) and self.__corresInfo["pdbid"]:
             self.__EmMapwithModel = True
         #
 
     def __getMissingAndInsistentValues(self, cifObj):
         """ """
         text = self.__getConcatText(cifObj, "missing_value_items")
         txt = self.__getComparisonText(cifObj)
@@ -260,38 +260,38 @@
             if self.__EmMapwithModel:
                 atom_inclusion_all_atoms = cifObj.GetSingleValue("pdbx_vrpt_summary_em", "atom_inclusion_all_atoms")
                 atom_inclusion_backbone = cifObj.GetSingleValue("pdbx_vrpt_summary_em", "atom_inclusion_backbone")
                 if atom_inclusion_all_atoms and atom_inclusion_backbone:
                     try:
                         self.__corresInfo["atom_inclusion_all_atoms"] = "%.2f" % (float(atom_inclusion_all_atoms) * 100)
                         self.__corresInfo["atom_inclusion_backbone"] = "%.2f" % (float(atom_inclusion_backbone) * 100)
-                    except:
+                    except:  # noqa: E722 pylint: disable=bare-except
                         self.__lfh.write("_pdbx_vrpt_summary_em.atom_inclusion_all_atoms=%r _pdbx_vrpt_summary_em.atom_inclusion_backbone=%r\n" %
-                                        (atom_inclusion_all_atoms, atom_inclusion_backbone))
+                                         (atom_inclusion_all_atoms, atom_inclusion_backbone))
                     #
                 #
             #
             if self.__EmFsc143CutOff:
                 author_fsc_cutoff = cifObj.GetSingleValue("pdbx_vrpt_summary_em", "author_provided_fsc_resolution_by_cutoff_pt_143")
                 EMDB_resolution = cifObj.GetSingleValue("pdbx_vrpt_summary_em", "EMDB_resolution")
                 if author_fsc_cutoff and EMDB_resolution:
                     try:
                         lower_bound = 0.9 * float(author_fsc_cutoff)
                         upper_bound = 1.1 * float(author_fsc_cutoff)
                         resolution = float(EMDB_resolution)
                         if (resolution < lower_bound) or (resolution > upper_bound):
                             self.__corresInfo["fsc_curve"] = "yes"
                         #
-                    except:
+                    except:  # noqa: E722 pylint: disable=bare-except
                         self.__lfh.write("_pdbx_vrpt_summary_em.author_provided_fsc_resolution_by_cutoff_pt_143=%r _pdbx_vrpt_summary_em.EMDB_resolution=%r\n" %
-                                        (author_fsc_cutoff, EMDB_resolution))
+                                         (author_fsc_cutoff, EMDB_resolution))
                     #
                 #
             #
-        except:
+        except:  # noqa: E722 pylint: disable=bare-except
             self.__lfh.write("Read %s failed.\n" % cifPath)
         #
 
     # def __getPolymerBondOutlier(self, vobj):
     #     """ """
     #     list = vobj.getOutlier("bond-outlier")
     #     if not list:
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/io/PisaReader.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/io/PisaReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/link/Link.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/link/Link.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/Related.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/Related.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/site/Site.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/site/Site.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/validate/Validate.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/validate/Validate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann-tasks-v2
-Version: 0.33.3
+Version: 0.34
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33.3/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt` & `wwpdb.apps.ann_tasks_v2-0.34/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

