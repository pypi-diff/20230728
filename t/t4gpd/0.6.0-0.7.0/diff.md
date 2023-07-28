# Comparing `tmp/t4gpd-0.6.0.tar.gz` & `tmp/t4gpd-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t4gpd-0.6.0.tar", last modified: Thu Mar 23 21:05:47 2023, max compression
+gzip compressed data, was "t4gpd-0.7.0.tar", last modified: Fri Jul 28 08:41:41 2023, max compression
```

## Comparing `t4gpd-0.6.0.tar` & `t4gpd-0.7.0.tar`

### file list

```diff
@@ -1,349 +1,362 @@
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.539360 t4gpd-0.6.0/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    35149 2020-06-13 17:54:58.000000 t4gpd-0.6.0/LICENSE.txt
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2407 2023-03-23 21:05:47.539360 t4gpd-0.6.0/PKG-INFO
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1352 2023-03-23 20:49:00.000000 t4gpd-0.6.0/README.md
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      107 2023-03-23 21:05:47.539360 t4gpd-0.6.0/setup.cfg
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2141 2022-08-24 08:30:43.000000 t4gpd-0.6.0/setup.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.503359 t4gpd-0.6.0/t4gpd/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      739 2020-11-20 20:32:18.000000 t4gpd-0.6.0/t4gpd/__init__.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      804 2023-03-23 20:47:53.000000 t4gpd-0.6.0/t4gpd/_version.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.503359 t4gpd-0.6.0/t4gpd/comfort/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1492 2022-10-14 15:48:15.000000 t4gpd-0.6.0/t4gpd/comfort/EmpiricalThermalIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1877 2021-05-17 12:41:51.000000 t4gpd-0.6.0/t4gpd/comfort/LinearThermalIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2478 2022-10-14 15:47:50.000000 t4gpd-0.6.0/t4gpd/comfort/UniversalThermalIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-02-02 17:38:35.000000 t4gpd-0.6.0/t4gpd/comfort/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.507359 t4gpd-0.6.0/t4gpd/comfort/algo/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5931 2021-05-12 17:04:21.000000 t4gpd-0.6.0/t4gpd/comfort/algo/CommonsLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4716 2021-05-12 16:38:39.000000 t4gpd-0.6.0/t4gpd/comfort/algo/ConstantsLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     7079 2021-05-17 12:10:26.000000 t4gpd-0.6.0/t4gpd/comfort/algo/ETULib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1432 2021-05-12 16:42:17.000000 t4gpd-0.6.0/t4gpd/comfort/algo/PETLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1874 2021-09-02 09:59:31.000000 t4gpd-0.6.0/t4gpd/comfort/algo/PMVLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1714 2021-05-17 13:02:49.000000 t4gpd-0.6.0/t4gpd/comfort/algo/PTLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2066 2021-09-02 10:00:06.000000 t4gpd-0.6.0/t4gpd/comfort/algo/SETLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     8302 2021-12-10 17:18:50.000000 t4gpd-0.6.0/t4gpd/comfort/algo/SET_mist.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1380 2021-05-12 08:12:54.000000 t4gpd-0.6.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1877 2021-05-12 18:58:48.000000 t4gpd-0.6.0/t4gpd/comfort/algo/TmrtOutLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    17227 2022-10-24 09:23:00.000000 t4gpd-0.6.0/t4gpd/comfort/algo/UTCILib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    13633 2021-02-04 21:08:03.000000 t4gpd-0.6.0/t4gpd/comfort/algo/VDI_PET_corrected.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1284 2022-10-24 09:21:44.000000 t4gpd-0.6.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-02-04 21:08:03.000000 t4gpd-0.6.0/t4gpd/comfort/algo/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.507359 t4gpd-0.6.0/t4gpd/comfort/indices/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2650 2022-10-14 15:46:56.000000 t4gpd-0.6.0/t4gpd/comfort/indices/ASV.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      876 2021-05-12 06:43:03.000000 t4gpd-0.6.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1980 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/DI.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3216 2022-10-14 15:46:30.000000 t4gpd-0.6.0/t4gpd/comfort/indices/ETU.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2004 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/H.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2396 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/HI.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2202 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/NET.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2331 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/OUTSET.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2037 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/PE.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3194 2022-10-24 15:23:58.000000 t4gpd-0.6.0/t4gpd/comfort/indices/PET.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3088 2022-10-24 15:23:58.000000 t4gpd-0.6.0/t4gpd/comfort/indices/PMV.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2232 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/PT.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2801 2022-10-24 15:23:09.000000 t4gpd-0.6.0/t4gpd/comfort/indices/SET.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3026 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/SETmist.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2163 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/THI.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2223 2021-05-12 19:36:36.000000 t4gpd-0.6.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2178 2022-10-14 15:45:34.000000 t4gpd-0.6.0/t4gpd/comfort/indices/TmrtOut.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5838 2022-10-14 15:44:45.000000 t4gpd-0.6.0/t4gpd/comfort/indices/TmrtRadiometer.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3217 2022-10-24 15:23:58.000000 t4gpd-0.6.0/t4gpd/comfort/indices/UTCI.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2660 2022-10-14 14:25:47.000000 t4gpd-0.6.0/t4gpd/comfort/indices/WCT.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-05-11 16:27:08.000000 t4gpd-0.6.0/t4gpd/comfort/indices/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.511359 t4gpd-0.6.0/t4gpd/commons/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1608 2020-10-07 15:28:18.000000 t4gpd-0.6.0/t4gpd/commons/AngleLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1189 2021-01-07 07:59:17.000000 t4gpd-0.6.0/t4gpd/commons/ArrayCoding.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2308 2020-06-19 14:10:50.000000 t4gpd-0.6.0/t4gpd/commons/BoundingBox.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2366 2020-12-16 13:15:18.000000 t4gpd-0.6.0/t4gpd/commons/CSVLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1675 2021-07-01 09:32:35.000000 t4gpd-0.6.0/t4gpd/commons/CalendarLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     7227 2021-06-16 14:25:07.000000 t4gpd-0.6.0/t4gpd/commons/CaliperLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      959 2020-10-02 12:26:10.000000 t4gpd-0.6.0/t4gpd/commons/Checksum.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4541 2020-12-15 16:02:11.000000 t4gpd-0.6.0/t4gpd/commons/ChrystalAlgorithm.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1637 2022-10-26 07:58:39.000000 t4gpd-0.6.0/t4gpd/commons/DataFrameLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2271 2022-08-24 10:23:43.000000 t4gpd-0.6.0/t4gpd/commons/DateRangeLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4956 2022-05-18 15:38:27.000000 t4gpd-0.6.0/t4gpd/commons/DatetimeLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1770 2022-09-05 10:36:15.000000 t4gpd-0.6.0/t4gpd/commons/DiameterLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5876 2020-06-22 09:32:49.000000 t4gpd-0.6.0/t4gpd/commons/Distances.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2831 2022-01-18 19:42:17.000000 t4gpd-0.6.0/t4gpd/commons/Entropy.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2832 2020-09-11 17:04:11.000000 t4gpd-0.6.0/t4gpd/commons/Epsilon.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1357 2022-10-25 14:40:11.000000 t4gpd-0.6.0/t4gpd/commons/GeoDataFrameLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1907 2021-05-18 08:44:20.000000 t4gpd-0.6.0/t4gpd/commons/GeoProcess.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    25373 2023-02-15 21:10:56.000000 t4gpd-0.6.0/t4gpd/commons/GeomLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5407 2022-09-07 15:04:19.000000 t4gpd-0.6.0/t4gpd/commons/GeomLib3D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4427 2022-03-28 12:35:37.000000 t4gpd-0.6.0/t4gpd/commons/GridFaceLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1149 2020-06-19 13:58:19.000000 t4gpd-0.6.0/t4gpd/commons/IllegalArgumentTypeException.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5933 2022-11-08 14:40:17.000000 t4gpd-0.6.0/t4gpd/commons/KernelLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3784 2020-10-24 09:49:18.000000 t4gpd-0.6.0/t4gpd/commons/LandoltRingLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2526 2022-03-08 14:24:54.000000 t4gpd-0.6.0/t4gpd/commons/LatLonLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2291 2021-04-12 07:38:42.000000 t4gpd-0.6.0/t4gpd/commons/LineStringCuttingLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1989 2020-10-11 20:51:06.000000 t4gpd-0.6.0/t4gpd/commons/ListUtilities.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5244 2022-06-02 10:16:48.000000 t4gpd-0.6.0/t4gpd/commons/Logos.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2108 2020-06-17 18:58:12.000000 t4gpd-0.6.0/t4gpd/commons/MyEdge.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2709 2020-09-24 09:53:56.000000 t4gpd-0.6.0/t4gpd/commons/MyNode.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     8008 2022-06-13 13:36:47.000000 t4gpd-0.6.0/t4gpd/commons/PointsDensifierLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3137 2022-09-20 15:59:32.000000 t4gpd-0.6.0/t4gpd/commons/PointsDensifierLib3D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2833 2020-06-22 09:34:45.000000 t4gpd-0.6.0/t4gpd/commons/PolarCartesianCoordinates.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    13455 2023-01-30 13:37:02.000000 t4gpd-0.6.0/t4gpd/commons/RayCasting2Lib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    13317 2023-02-16 10:09:06.000000 t4gpd-0.6.0/t4gpd/commons/RayCasting3Lib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    11700 2023-02-20 09:15:16.000000 t4gpd-0.6.0/t4gpd/commons/RayCastingLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5638 2022-07-20 08:24:45.000000 t4gpd-0.6.0/t4gpd/commons/RotationLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2201 2022-04-08 14:27:04.000000 t4gpd-0.6.0/t4gpd/commons/SVFLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2307 2022-01-04 20:40:30.000000 t4gpd-0.6.0/t4gpd/commons/ShannonEntropy.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1308 2022-07-19 14:44:29.000000 t4gpd-0.6.0/t4gpd/commons/SphericalCartesianCoordinates.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4937 2022-09-20 16:03:36.000000 t4gpd-0.6.0/t4gpd/commons/SphericalProjectionLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1404 2021-06-08 21:34:17.000000 t4gpd-0.6.0/t4gpd/commons/TestUtils.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-03-31 09:59:56.000000 t4gpd-0.6.0/t4gpd/commons/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.511359 t4gpd-0.6.0/t4gpd/commons/crossroads_generation/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5620 2022-11-07 10:44:48.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_generation/Sequence.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2802 2023-02-14 10:49:22.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_generation/SequenceRadii.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3626 2022-11-07 10:44:48.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-11-07 10:44:48.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_generation/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.511359 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1860 2022-11-07 14:02:08.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/AbstractMethod.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3791 2022-11-07 14:02:08.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1070 2022-11-07 14:02:08.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/FFTMethod.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3228 2022-11-07 14:02:08.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/FWTMethod.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2953 2022-11-07 14:02:08.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1160 2022-11-07 14:02:08.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-11-07 14:02:08.000000 t4gpd-0.6.0/t4gpd/commons/crossroads_identification/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.511359 t4gpd-0.6.0/t4gpd/commons/ellipse/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3611 2020-08-31 08:21:22.000000 t4gpd-0.6.0/t4gpd/commons/ellipse/EllipseLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    25237 2020-06-23 22:05:17.000000 t4gpd-0.6.0/t4gpd/commons/ellipse/EllipticHullLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-06-23 22:04:55.000000 t4gpd-0.6.0/t4gpd/commons/ellipse/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.515359 t4gpd-0.6.0/t4gpd/commons/graph/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6382 2021-03-24 08:57:48.000000 t4gpd-0.6.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4942 2023-01-27 17:52:06.000000 t4gpd-0.6.0/t4gpd/commons/graph/MCALib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4987 2020-11-23 09:56:15.000000 t4gpd-0.6.0/t4gpd/commons/graph/NeighborhoodLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2883 2020-11-23 09:55:51.000000 t4gpd-0.6.0/t4gpd/commons/graph/ShortestPathLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4289 2020-11-23 10:13:17.000000 t4gpd-0.6.0/t4gpd/commons/graph/UrbanGraphLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6322 2021-06-25 08:43:27.000000 t4gpd-0.6.0/t4gpd/commons/graph/UrbanGraphLibOld.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-11-21 18:40:43.000000 t4gpd-0.6.0/t4gpd/commons/graph/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.515359 t4gpd-0.6.0/t4gpd/commons/grid/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2179 2023-01-30 13:38:02.000000 t4gpd-0.6.0/t4gpd/commons/grid/AbstractGridLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6264 2023-02-17 15:49:30.000000 t4gpd-0.6.0/t4gpd/commons/grid/GridLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-04-09 08:07:33.000000 t4gpd-0.6.0/t4gpd/commons/grid/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.515359 t4gpd-0.6.0/t4gpd/commons/isovists/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-11-25 21:42:21.000000 t4gpd-0.6.0/t4gpd/commons/isovists/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.515359 t4gpd-0.6.0/t4gpd/commons/rnd/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4259 2023-01-09 10:37:41.000000 t4gpd-0.6.0/t4gpd/commons/rnd/RandomPointPicking.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2023-01-09 09:57:47.000000 t4gpd-0.6.0/t4gpd/commons/rnd/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.515359 t4gpd-0.6.0/t4gpd/commons/sun/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2774 2021-04-21 15:35:41.000000 t4gpd-0.6.0/t4gpd/commons/sun/AbstractSunLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1441 2022-12-08 17:43:59.000000 t4gpd-0.6.0/t4gpd/commons/sun/DaylightLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1897 2021-06-01 20:45:53.000000 t4gpd-0.6.0/t4gpd/commons/sun/PySolarSunLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     7584 2021-04-22 16:07:47.000000 t4gpd-0.6.0/t4gpd/commons/sun/ShadowLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6719 2021-04-21 15:36:33.000000 t4gpd-0.6.0/t4gpd/commons/sun/SoleneSunLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2429 2022-05-18 15:30:31.000000 t4gpd-0.6.0/t4gpd/commons/sun/SunBeamLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     8335 2021-12-10 17:17:50.000000 t4gpd-0.6.0/t4gpd/commons/sun/SunLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-01-21 13:30:14.000000 t4gpd-0.6.0/t4gpd/commons/sun/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.519359 t4gpd-0.6.0/t4gpd/demos/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      879 2022-10-25 16:21:05.000000 t4gpd-0.6.0/t4gpd/demos/AbstractGeoDataFrameDemos.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)   405923 2023-01-26 09:35:22.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)  1039604 2022-10-25 15:14:06.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos2.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)   453528 2022-10-25 15:00:19.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos3.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)  2888649 2022-10-25 15:48:49.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos4.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)   745426 2022-07-18 15:50:21.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos5.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)   435846 2022-10-26 14:52:50.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos6.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    25686 2022-10-31 17:23:24.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos7.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)   435537 2022-10-31 17:22:15.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos8.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    87843 2023-03-22 16:19:10.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos9.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)   258216 2023-03-23 12:09:28.000000 t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemosA.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-01-26 22:34:45.000000 t4gpd-0.6.0/t4gpd/demos/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.523360 t4gpd-0.6.0/t4gpd/energy/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    12332 2022-04-28 15:33:51.000000 t4gpd-0.6.0/t4gpd/energy/DirectSolarIrradianceLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3194 2022-07-22 08:39:12.000000 t4gpd-0.6.0/t4gpd/energy/Dogniaux.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3035 2022-07-22 08:20:11.000000 t4gpd-0.6.0/t4gpd/energy/Perez.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1107 2022-07-22 08:20:39.000000 t4gpd-0.6.0/t4gpd/energy/Perraudeau.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3305 2022-07-22 08:21:55.000000 t4gpd-0.6.0/t4gpd/energy/PerrinDeBrichambaut.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3748 2022-07-22 08:40:41.000000 t4gpd-0.6.0/t4gpd/energy/PlotDirectNormalIrradiance.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-08-25 13:57:12.000000 t4gpd-0.6.0/t4gpd/energy/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.523360 t4gpd-0.6.0/t4gpd/energy/geoProcesses/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4517 2022-05-18 17:36:24.000000 t4gpd-0.6.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-04-28 20:49:22.000000 t4gpd-0.6.0/t4gpd/energy/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.523360 t4gpd-0.6.0/t4gpd/graph/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1047 2020-12-31 14:32:10.000000 t4gpd-0.6.0/t4gpd/graph/STBetweennessCentrality.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1043 2020-12-19 20:28:37.000000 t4gpd-0.6.0/t4gpd/graph/STClosenessCentrality.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2657 2020-11-23 10:00:25.000000 t4gpd-0.6.0/t4gpd/graph/STRoadNeighborhood.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2459 2020-11-21 19:04:19.000000 t4gpd-0.6.0/t4gpd/graph/STShortestPath.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1644 2020-11-23 10:45:34.000000 t4gpd-0.6.0/t4gpd/graph/STToRoadsSections.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1474 2020-11-23 10:45:52.000000 t4gpd-0.6.0/t4gpd/graph/STToRoadsSectionsNodes.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-06-17 07:51:42.000000 t4gpd-0.6.0/t4gpd/graph/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.523360 t4gpd-0.6.0/t4gpd/io/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1018 2022-06-22 07:38:02.000000 t4gpd-0.6.0/t4gpd/io/AbstractReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4231 2020-09-24 09:56:55.000000 t4gpd-0.6.0/t4gpd/io/CSVInertialSensorReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1889 2020-09-24 09:57:20.000000 t4gpd-0.6.0/t4gpd/io/CSVReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1884 2021-03-10 14:24:32.000000 t4gpd-0.6.0/t4gpd/io/CSVWKTReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2317 2021-03-10 14:24:47.000000 t4gpd-0.6.0/t4gpd/io/CSVWKTWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3373 2022-07-25 09:09:50.000000 t4gpd-0.6.0/t4gpd/io/CirReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1314 2022-07-25 09:34:22.000000 t4gpd-0.6.0/t4gpd/io/CirValReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3331 2021-03-10 21:07:26.000000 t4gpd-0.6.0/t4gpd/io/CirWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5578 2020-10-22 16:39:22.000000 t4gpd-0.6.0/t4gpd/io/CityGMLReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     7156 2022-06-24 16:06:01.000000 t4gpd-0.6.0/t4gpd/io/GeoWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1829 2022-11-09 15:42:30.000000 t4gpd-0.6.0/t4gpd/io/GpkgLoader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1818 2022-11-09 15:42:30.000000 t4gpd-0.6.0/t4gpd/io/GpkgWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    12097 2021-06-25 08:29:09.000000 t4gpd-0.6.0/t4gpd/io/MshReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3750 2020-08-25 16:50:36.000000 t4gpd-0.6.0/t4gpd/io/ObjReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3541 2021-02-01 10:43:14.000000 t4gpd-0.6.0/t4gpd/io/ObjWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1430 2021-07-19 15:31:30.000000 t4gpd-0.6.0/t4gpd/io/Reloading.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1152 2022-04-26 12:38:58.000000 t4gpd-0.6.0/t4gpd/io/STLoadAndClip.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3086 2020-06-19 14:12:42.000000 t4gpd-0.6.0/t4gpd/io/SVGWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5130 2022-07-26 12:53:22.000000 t4gpd-0.6.0/t4gpd/io/SalomeWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5030 2022-07-26 12:53:22.000000 t4gpd-0.6.0/t4gpd/io/SalomeWriterAndExtruder.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6490 2021-03-10 14:25:07.000000 t4gpd-0.6.0/t4gpd/io/VTUWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2492 2022-07-25 09:33:33.000000 t4gpd-0.6.0/t4gpd/io/ValReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2806 2021-11-08 15:20:17.000000 t4gpd-0.6.0/t4gpd/io/ZipLoader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3559 2021-10-18 16:00:12.000000 t4gpd-0.6.0/t4gpd/io/ZipWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-06-17 18:59:50.000000 t4gpd-0.6.0/t4gpd/io/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.527360 t4gpd-0.6.0/t4gpd/isovist/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4347 2022-07-27 15:30:51.000000 t4gpd-0.6.0/t4gpd/isovist/STIsovistField2D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-06-17 09:56:41.000000 t4gpd-0.6.0/t4gpd/isovist/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.527360 t4gpd-0.6.0/t4gpd/misc/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4972 2021-07-20 15:59:02.000000 t4gpd-0.6.0/t4gpd/misc/FrequencyHistogram.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5748 2023-03-23 17:02:07.000000 t4gpd-0.6.0/t4gpd/misc/OptimalNumberOfClusters.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5344 2021-11-14 15:44:04.000000 t4gpd-0.6.0/t4gpd/misc/PlotAMatrixOfDiagrams.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2960 2021-10-01 15:35:34.000000 t4gpd-0.6.0/t4gpd/misc/PopulationPyramid.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5500 2023-01-19 10:23:40.000000 t4gpd-0.6.0/t4gpd/misc/RoseMappingTool.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3038 2022-03-15 16:20:31.000000 t4gpd-0.6.0/t4gpd/misc/STCompass.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2311 2023-03-23 14:05:55.000000 t4gpd-0.6.0/t4gpd/misc/STDendrogram.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2041 2023-03-23 16:15:02.000000 t4gpd-0.6.0/t4gpd/misc/STKMeans.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4364 2021-01-25 16:17:15.000000 t4gpd-0.6.0/t4gpd/misc/StreetOrientationHistogram.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4386 2022-12-13 18:08:58.000000 t4gpd-0.6.0/t4gpd/misc/TimelineTool.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2824 2021-03-15 16:13:35.000000 t4gpd-0.6.0/t4gpd/misc/WindRose.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-09-29 10:07:30.000000 t4gpd-0.6.0/t4gpd/misc/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.531360 t4gpd-0.6.0/t4gpd/morph/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2873 2021-08-25 16:19:57.000000 t4gpd-0.6.0/t4gpd/morph/GmshTriangulator.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1413 2023-02-17 18:32:38.000000 t4gpd-0.6.0/t4gpd/morph/STBBox.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1793 2020-06-30 09:46:17.000000 t4gpd-0.6.0/t4gpd/morph/STClip.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4603 2022-08-24 09:39:40.000000 t4gpd-0.6.0/t4gpd/morph/STCoolscapesTessellation.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2459 2022-11-07 10:45:43.000000 t4gpd-0.6.0/t4gpd/morph/STCrossroadsGeneration.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2853 2023-02-14 11:31:50.000000 t4gpd-0.6.0/t4gpd/morph/STDilationErosion.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2103 2020-12-14 16:55:46.000000 t4gpd-0.6.0/t4gpd/morph/STExtractOpenSpaces.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3726 2021-04-02 09:43:35.000000 t4gpd-0.6.0/t4gpd/morph/STFacadesAnalysis.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     8594 2023-02-20 08:30:55.000000 t4gpd-0.6.0/t4gpd/morph/STGradientOfDistancesToBuildings.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2038 2021-04-09 12:28:19.000000 t4gpd-0.6.0/t4gpd/morph/STGrid.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3688 2020-09-17 11:02:43.000000 t4gpd-0.6.0/t4gpd/morph/STIdentifyRowOfTrees.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4480 2021-12-09 14:49:10.000000 t4gpd-0.6.0/t4gpd/morph/STMakeBlocks.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2812 2020-09-21 14:15:12.000000 t4gpd-0.6.0/t4gpd/morph/STMultipleOverlaps.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4550 2023-02-20 08:36:37.000000 t4gpd-0.6.0/t4gpd/morph/STMultipleOverlaps2.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3134 2022-06-13 13:37:40.000000 t4gpd-0.6.0/t4gpd/morph/STPointsDensifier.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2118 2022-06-13 13:11:05.000000 t4gpd-0.6.0/t4gpd/morph/STPointsDensifier2.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1717 2020-12-31 16:03:16.000000 t4gpd-0.6.0/t4gpd/morph/STPolygonize.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3105 2023-02-15 17:59:34.000000 t4gpd-0.6.0/t4gpd/morph/STSkeletonize.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2294 2023-02-15 20:25:15.000000 t4gpd-0.6.0/t4gpd/morph/STSkeletonizeTheVoid.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3196 2020-09-24 10:27:56.000000 t4gpd-0.6.0/t4gpd/morph/STSnappingPointsOnLines.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6567 2022-08-24 09:55:25.000000 t4gpd-0.6.0/t4gpd/morph/STSnappingPointsOnLines2.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3217 2021-05-18 08:45:03.000000 t4gpd-0.6.0/t4gpd/morph/STSpatialJoin.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1568 2022-10-14 10:00:03.000000 t4gpd-0.6.0/t4gpd/morph/STSquaredBBox.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2628 2023-01-31 10:54:56.000000 t4gpd-0.6.0/t4gpd/morph/STVariableWidthBuffer.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3729 2020-09-25 16:31:01.000000 t4gpd-0.6.0/t4gpd/morph/STVoronoiPartition.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-03-31 10:00:08.000000 t4gpd-0.6.0/t4gpd/morph/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.535360 t4gpd-0.6.0/t4gpd/morph/geoProcesses/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      941 2020-06-18 08:03:10.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2895 2020-06-19 14:16:30.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/AngularAbscissa.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1132 2020-06-18 08:03:10.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4153 2023-01-30 15:34:51.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/AspectRatio.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1003 2020-06-18 08:03:10.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/BBox.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1813 2023-02-14 11:19:09.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1996 2020-10-07 15:31:07.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1851 2020-12-18 22:37:53.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/CircularityIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      946 2020-06-18 08:03:10.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/ConvexHull.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1917 2020-12-18 22:29:45.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/ConvexityIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1903 2022-11-07 14:15:37.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4022 2022-11-08 14:46:29.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5107 2023-02-20 08:57:36.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1136 2020-06-19 14:45:22.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/Diameter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2106 2020-12-30 20:08:51.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/EllipticityIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3512 2022-07-22 14:38:29.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/FootprintExtruder.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1100 2021-06-21 13:53:15.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1227 2022-03-28 12:36:54.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/GridFace.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2283 2023-01-30 16:12:41.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/HMean.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2179 2023-01-30 14:29:24.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2481 2021-02-14 18:01:56.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1564 2023-01-30 13:38:38.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2342 2020-06-23 22:09:00.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/MABE.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)      954 2020-06-18 08:03:10.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/MABR.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1067 2021-01-10 10:06:31.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/MABR2.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1094 2020-12-15 16:02:50.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/MBC.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1065 2020-12-15 20:28:55.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/MPBR.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1600 2020-12-30 20:09:13.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/RectangularityIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1374 2022-11-08 14:46:29.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/RectifyByFFT.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1749 2022-11-08 14:46:29.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/RectifyByFWT.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1018 2020-06-19 07:17:45.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/RemoveHoles.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1628 2022-06-24 16:06:35.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/RepresentativePoint.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1235 2021-04-26 14:02:10.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/Rotation2D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3611 2023-03-15 18:24:43.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/STGeoProcess.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3139 2023-01-30 13:39:08.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/SkyMap2D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2996 2023-01-30 15:49:55.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/SkyViewFactor.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3657 2021-03-03 16:15:56.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1687 2022-01-18 09:14:29.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/StarShapedIndices.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1898 2023-01-30 14:30:54.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/SurfaceFraction.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1978 2021-04-26 13:48:42.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/Translation.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1792 2023-01-30 16:09:52.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/WMean.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-06-16 15:16:57.000000 t4gpd-0.6.0/t4gpd/morph/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.535360 t4gpd-0.6.0/t4gpd/picoclim/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5226 2023-03-22 14:14:53.000000 t4gpd-0.6.0/t4gpd/picoclim/CampbellSciReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2546 2023-01-09 14:21:24.000000 t4gpd-0.6.0/t4gpd/picoclim/ExtraProcessing.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2520 2023-03-22 15:24:50.000000 t4gpd-0.6.0/t4gpd/picoclim/InertialMeasureReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3624 2023-03-22 16:43:01.000000 t4gpd-0.6.0/t4gpd/picoclim/JoinByTimeDistance.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2597 2022-09-15 13:20:13.000000 t4gpd-0.6.0/t4gpd/picoclim/KestrelReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2305 2022-10-26 10:49:53.000000 t4gpd-0.6.0/t4gpd/picoclim/MeteoFranceReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    15062 2023-03-22 14:23:02.000000 t4gpd-0.6.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4141 2022-10-26 10:14:02.000000 t4gpd-0.6.0/t4gpd/picoclim/MetrologicalCampaignReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2856 2022-10-26 09:41:11.000000 t4gpd-0.6.0/t4gpd/picoclim/SensirionReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6056 2023-03-22 15:26:59.000000 t4gpd-0.6.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3174 2022-10-26 08:13:12.000000 t4gpd-0.6.0/t4gpd/picoclim/TracksWaypointsReader.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-09-15 08:50:25.000000 t4gpd-0.6.0/t4gpd/picoclim/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.535360 t4gpd-0.6.0/t4gpd/pyplot/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4516 2022-11-07 14:14:25.000000 t4gpd-0.6.0/t4gpd/pyplot/MultipleMarkerStyles.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-01-31 17:29:02.000000 t4gpd-0.6.0/t4gpd/pyplot/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.535360 t4gpd-0.6.0/t4gpd/pyqgis/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3438 2022-07-29 07:32:07.000000 t4gpd-0.6.0/t4gpd/pyqgis/AddMemoryLayer.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1629 2022-07-27 20:17:41.000000 t4gpd-0.6.0/t4gpd/pyqgis/Emphasizer.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     8447 2022-07-10 14:41:36.000000 t4gpd-0.6.0/t4gpd/pyqgis/MapPrinter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     5785 2022-01-04 20:40:30.000000 t4gpd-0.6.0/t4gpd/pyqgis/PdfMapWriter.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     9653 2022-07-29 10:44:37.000000 t4gpd-0.6.0/t4gpd/pyqgis/SetSymbolLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1323 2021-09-10 16:28:27.000000 t4gpd-0.6.0/t4gpd/pyqgis/ShowFeatureCount.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1746 2021-09-24 09:47:44.000000 t4gpd-0.6.0/t4gpd/pyqgis/ZoomLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-09-09 16:49:22.000000 t4gpd-0.6.0/t4gpd/pyqgis/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.535360 t4gpd-0.6.0/t4gpd/pyvista/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3711 2022-09-02 07:34:06.000000 t4gpd-0.6.0/t4gpd/pyvista/GeodeCiel.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4689 2022-09-01 16:13:45.000000 t4gpd-0.6.0/t4gpd/pyvista/Icosahedron.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2043 2022-06-22 15:52:10.000000 t4gpd-0.6.0/t4gpd/pyvista/STRaysToViewFactors.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3916 2022-06-05 15:29:14.000000 t4gpd-0.6.0/t4gpd/pyvista/ToPolyData.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4642 2022-09-25 09:28:13.000000 t4gpd-0.6.0/t4gpd/pyvista/ToUnstructuredGrid.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-04-05 17:09:50.000000 t4gpd-0.6.0/t4gpd/pyvista/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.535360 t4gpd-0.6.0/t4gpd/pyvista/commons/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1805 2022-09-05 12:42:46.000000 t4gpd-0.6.0/t4gpd/pyvista/commons/Diameter3DLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     8778 2022-09-01 16:15:11.000000 t4gpd-0.6.0/t4gpd/pyvista/commons/RayCasting3DLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     7389 2022-09-05 16:44:01.000000 t4gpd-0.6.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     8995 2022-09-07 10:57:40.000000 t4gpd-0.6.0/t4gpd/pyvista/commons/SVF3DLib.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3683 2022-08-23 11:33:51.000000 t4gpd-0.6.0/t4gpd/pyvista/commons/Triangle3D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-06-05 21:07:30.000000 t4gpd-0.6.0/t4gpd/pyvista/commons/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.539360 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3127 2022-07-18 15:37:08.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1398 2022-07-18 07:24:52.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     1686 2022-06-22 16:23:38.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4679 2022-08-22 15:26:00.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4542 2022-08-24 08:46:07.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     6047 2022-09-05 16:44:47.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3951 2022-09-05 16:45:02.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/SVF3D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2022-06-09 11:51:20.000000 t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.539360 t4gpd-0.6.0/t4gpd/raster/
--rwxrwxr-x   0 tleduc    (1000) tleduc    (1000)     2916 2022-06-01 18:54:37.000000 t4gpd-0.6.0/t4gpd/raster/STToRaster.py
--rwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2022-06-01 12:59:39.000000 t4gpd-0.6.0/t4gpd/raster/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.539360 t4gpd-0.6.0/t4gpd/sun/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2041 2021-04-22 15:43:22.000000 t4gpd-0.6.0/t4gpd/sun/AbstractHardShadow.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3176 2022-05-18 15:39:03.000000 t4gpd-0.6.0/t4gpd/sun/STHardShadow.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4002 2022-05-18 15:39:34.000000 t4gpd-0.6.0/t4gpd/sun/STSunMap2D.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     3423 2022-05-18 15:44:21.000000 t4gpd-0.6.0/t4gpd/sun/STTreeHardShadow.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4353 2022-05-18 15:44:39.000000 t4gpd-0.6.0/t4gpd/sun/STTreeHardShadow2.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2020-08-25 13:41:14.000000 t4gpd-0.6.0/t4gpd/sun/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.539360 t4gpd-0.6.0/t4gpd/sun/geoProcesses/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2489 2021-04-21 16:17:23.000000 t4gpd-0.6.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2218 2021-04-21 16:17:37.000000 t4gpd-0.6.0/t4gpd/sun/geoProcesses/SunshineDuration.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     4779 2021-04-21 16:17:58.000000 t4gpd-0.6.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        0 2021-03-03 15:05:24.000000 t4gpd-0.6.0/t4gpd/sun/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1000) tleduc    (1000)        0 2023-03-23 21:05:47.503359 t4gpd-0.6.0/t4gpd.egg-info/
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)     2407 2023-03-23 21:05:47.000000 t4gpd-0.6.0/t4gpd.egg-info/PKG-INFO
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)    10745 2023-03-23 21:05:47.000000 t4gpd-0.6.0/t4gpd.egg-info/SOURCES.txt
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        1 2023-03-23 21:05:47.000000 t4gpd-0.6.0/t4gpd.egg-info/dependency_links.txt
--rw-rw-r--   0 tleduc    (1000) tleduc    (1000)        6 2023-03-23 21:05:47.000000 t4gpd-0.6.0/t4gpd.egg-info/top_level.txt
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.379548 t4gpd-0.7.0/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    35149 2020-06-13 17:54:58.000000 t4gpd-0.7.0/LICENSE.txt
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2545 2023-07-28 08:41:41.379548 t4gpd-0.7.0/PKG-INFO
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1490 2023-03-23 21:33:47.000000 t4gpd-0.7.0/README.md
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      107 2023-07-28 08:41:41.379548 t4gpd-0.7.0/setup.cfg
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2141 2022-08-24 08:30:43.000000 t4gpd-0.7.0/setup.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.335548 t4gpd-0.7.0/t4gpd/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      739 2020-11-20 20:32:18.000000 t4gpd-0.7.0/t4gpd/__init__.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      804 2023-07-28 08:34:21.000000 t4gpd-0.7.0/t4gpd/_version.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.335548 t4gpd-0.7.0/t4gpd/comfort/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1492 2022-10-14 15:48:15.000000 t4gpd-0.7.0/t4gpd/comfort/EmpiricalThermalIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-17 12:41:51.000000 t4gpd-0.7.0/t4gpd/comfort/LinearThermalIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2478 2022-10-14 15:47:50.000000 t4gpd-0.7.0/t4gpd/comfort/UniversalThermalIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-02 17:38:35.000000 t4gpd-0.7.0/t4gpd/comfort/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.339548 t4gpd-0.7.0/t4gpd/comfort/algo/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5931 2021-05-12 17:04:21.000000 t4gpd-0.7.0/t4gpd/comfort/algo/CommonsLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4716 2021-05-12 16:38:39.000000 t4gpd-0.7.0/t4gpd/comfort/algo/ConstantsLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7079 2021-05-17 12:10:26.000000 t4gpd-0.7.0/t4gpd/comfort/algo/ETULib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1432 2021-05-12 16:42:17.000000 t4gpd-0.7.0/t4gpd/comfort/algo/PETLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1874 2021-09-02 09:59:31.000000 t4gpd-0.7.0/t4gpd/comfort/algo/PMVLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1714 2021-05-17 13:02:49.000000 t4gpd-0.7.0/t4gpd/comfort/algo/PTLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2066 2021-09-02 10:00:06.000000 t4gpd-0.7.0/t4gpd/comfort/algo/SETLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8302 2021-12-10 17:18:50.000000 t4gpd-0.7.0/t4gpd/comfort/algo/SET_mist.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1380 2021-05-12 08:12:54.000000 t4gpd-0.7.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-12 18:58:48.000000 t4gpd-0.7.0/t4gpd/comfort/algo/TmrtOutLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    17227 2022-10-24 09:23:00.000000 t4gpd-0.7.0/t4gpd/comfort/algo/UTCILib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13633 2021-02-04 21:08:03.000000 t4gpd-0.7.0/t4gpd/comfort/algo/VDI_PET_corrected.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1284 2022-10-24 09:21:44.000000 t4gpd-0.7.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-04 21:08:03.000000 t4gpd-0.7.0/t4gpd/comfort/algo/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.339548 t4gpd-0.7.0/t4gpd/comfort/indices/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2650 2022-10-14 15:46:56.000000 t4gpd-0.7.0/t4gpd/comfort/indices/ASV.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      876 2021-05-12 06:43:03.000000 t4gpd-0.7.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1980 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/DI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3216 2022-10-14 15:46:30.000000 t4gpd-0.7.0/t4gpd/comfort/indices/ETU.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2004 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/H.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2396 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/HI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2202 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/NET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2331 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/OUTSET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2037 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PE.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3895 2023-06-16 15:01:43.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3088 2022-10-24 15:23:58.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PMV.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2232 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2801 2022-10-24 15:23:09.000000 t4gpd-0.7.0/t4gpd/comfort/indices/SET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3026 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/SETmist.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/THI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2223 2021-05-12 19:36:36.000000 t4gpd-0.7.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2178 2022-10-14 15:45:34.000000 t4gpd-0.7.0/t4gpd/comfort/indices/TmrtOut.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5838 2022-10-14 15:44:45.000000 t4gpd-0.7.0/t4gpd/comfort/indices/TmrtRadiometer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3953 2023-06-16 14:56:42.000000 t4gpd-0.7.0/t4gpd/comfort/indices/UTCI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2660 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/WCT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-05-11 16:27:08.000000 t4gpd-0.7.0/t4gpd/comfort/indices/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1608 2020-10-07 15:28:18.000000 t4gpd-0.7.0/t4gpd/commons/AngleLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1189 2021-01-07 07:59:17.000000 t4gpd-0.7.0/t4gpd/commons/ArrayCoding.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2308 2020-06-19 14:10:50.000000 t4gpd-0.7.0/t4gpd/commons/BoundingBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2366 2020-12-16 13:15:18.000000 t4gpd-0.7.0/t4gpd/commons/CSVLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1675 2021-07-01 09:32:35.000000 t4gpd-0.7.0/t4gpd/commons/CalendarLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7227 2021-06-16 14:25:07.000000 t4gpd-0.7.0/t4gpd/commons/CaliperLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      959 2020-10-02 12:26:10.000000 t4gpd-0.7.0/t4gpd/commons/Checksum.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4541 2020-12-15 16:02:11.000000 t4gpd-0.7.0/t4gpd/commons/ChrystalAlgorithm.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2023-06-24 06:23:57.000000 t4gpd-0.7.0/t4gpd/commons/ColorTemperature.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1637 2022-10-26 07:58:39.000000 t4gpd-0.7.0/t4gpd/commons/DataFrameLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2271 2022-08-24 10:23:43.000000 t4gpd-0.7.0/t4gpd/commons/DateRangeLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4956 2022-05-18 15:38:27.000000 t4gpd-0.7.0/t4gpd/commons/DatetimeLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1770 2022-09-05 10:36:15.000000 t4gpd-0.7.0/t4gpd/commons/DiameterLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5876 2020-06-22 09:32:49.000000 t4gpd-0.7.0/t4gpd/commons/Distances.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2831 2022-01-18 19:42:17.000000 t4gpd-0.7.0/t4gpd/commons/Entropy.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2832 2020-09-11 17:04:11.000000 t4gpd-0.7.0/t4gpd/commons/Epsilon.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1357 2022-10-25 14:40:11.000000 t4gpd-0.7.0/t4gpd/commons/GeoDataFrameLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1907 2021-05-18 08:44:20.000000 t4gpd-0.7.0/t4gpd/commons/GeoProcess.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25373 2023-02-15 21:10:56.000000 t4gpd-0.7.0/t4gpd/commons/GeomLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5407 2022-09-07 15:04:19.000000 t4gpd-0.7.0/t4gpd/commons/GeomLib3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4427 2022-03-28 12:35:37.000000 t4gpd-0.7.0/t4gpd/commons/GridFaceLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1149 2020-06-19 13:58:19.000000 t4gpd-0.7.0/t4gpd/commons/IllegalArgumentTypeException.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5933 2022-11-08 14:40:17.000000 t4gpd-0.7.0/t4gpd/commons/KernelLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3784 2020-10-24 09:49:18.000000 t4gpd-0.7.0/t4gpd/commons/LandoltRingLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2526 2022-03-08 14:24:54.000000 t4gpd-0.7.0/t4gpd/commons/LatLonLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2291 2021-04-12 07:38:42.000000 t4gpd-0.7.0/t4gpd/commons/LineStringCuttingLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1989 2020-10-11 20:51:06.000000 t4gpd-0.7.0/t4gpd/commons/ListUtilities.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5244 2022-06-02 10:16:48.000000 t4gpd-0.7.0/t4gpd/commons/Logos.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2108 2020-06-17 18:58:12.000000 t4gpd-0.7.0/t4gpd/commons/MyEdge.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2709 2020-09-24 09:53:56.000000 t4gpd-0.7.0/t4gpd/commons/MyNode.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8008 2022-06-13 13:36:47.000000 t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3137 2022-09-20 15:59:32.000000 t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2833 2020-06-22 09:34:45.000000 t4gpd-0.7.0/t4gpd/commons/PolarCartesianCoordinates.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13455 2023-01-30 13:37:02.000000 t4gpd-0.7.0/t4gpd/commons/RayCasting2Lib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13317 2023-02-16 10:09:06.000000 t4gpd-0.7.0/t4gpd/commons/RayCasting3Lib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11979 2023-07-27 19:53:59.000000 t4gpd-0.7.0/t4gpd/commons/RayCasting4Lib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11700 2023-02-20 09:15:16.000000 t4gpd-0.7.0/t4gpd/commons/RayCastingLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5638 2022-07-20 08:24:45.000000 t4gpd-0.7.0/t4gpd/commons/RotationLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2201 2022-04-08 14:27:04.000000 t4gpd-0.7.0/t4gpd/commons/SVFLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2307 2021-01-15 15:49:37.000000 t4gpd-0.7.0/t4gpd/commons/ShannonEntropy.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1308 2022-07-19 14:44:29.000000 t4gpd-0.7.0/t4gpd/commons/SphericalCartesianCoordinates.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4937 2022-09-20 16:03:36.000000 t4gpd-0.7.0/t4gpd/commons/SphericalProjectionLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1404 2021-06-08 21:34:17.000000 t4gpd-0.7.0/t4gpd/commons/TestUtils.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1502 2023-05-24 21:14:34.000000 t4gpd-0.7.0/t4gpd/commons/WarnUtils.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 09:59:56.000000 t4gpd-0.7.0/t4gpd/commons/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5464 2023-05-24 14:00:40.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/Sequence.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2722 2023-05-23 14:00:27.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/SequenceRadii.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3626 2022-11-07 10:44:48.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 10:44:48.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1860 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/AbstractMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3791 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1070 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FFTMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3228 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FWTMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2953 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1160 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/ellipse/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2020-08-31 08:21:22.000000 t4gpd-0.7.0/t4gpd/commons/ellipse/EllipseLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25237 2020-06-23 22:05:17.000000 t4gpd-0.7.0/t4gpd/commons/ellipse/EllipticHullLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-23 22:04:55.000000 t4gpd-0.7.0/t4gpd/commons/ellipse/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/graph/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6382 2021-03-24 08:57:48.000000 t4gpd-0.7.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4942 2023-01-27 17:52:06.000000 t4gpd-0.7.0/t4gpd/commons/graph/MCALib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4987 2020-11-23 09:56:15.000000 t4gpd-0.7.0/t4gpd/commons/graph/NeighborhoodLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2883 2020-11-23 09:55:51.000000 t4gpd-0.7.0/t4gpd/commons/graph/ShortestPathLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4289 2020-11-23 10:13:17.000000 t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6322 2021-06-25 08:43:27.000000 t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLibOld.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-21 18:40:43.000000 t4gpd-0.7.0/t4gpd/commons/graph/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/grid/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2298 2023-07-26 09:36:34.000000 t4gpd-0.7.0/t4gpd/commons/grid/AbstractGridLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6264 2023-02-17 15:49:30.000000 t4gpd-0.7.0/t4gpd/commons/grid/GridLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-04-09 08:07:33.000000 t4gpd-0.7.0/t4gpd/commons/grid/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/isovists/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-25 21:42:21.000000 t4gpd-0.7.0/t4gpd/commons/isovists/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/rnd/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4458 2023-05-23 15:30:11.000000 t4gpd-0.7.0/t4gpd/commons/rnd/RandomPointPicking.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2023-01-09 09:57:47.000000 t4gpd-0.7.0/t4gpd/commons/rnd/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.351548 t4gpd-0.7.0/t4gpd/commons/sun/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2774 2021-04-21 15:35:41.000000 t4gpd-0.7.0/t4gpd/commons/sun/AbstractSunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1441 2022-12-08 17:43:59.000000 t4gpd-0.7.0/t4gpd/commons/sun/DaylightLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1897 2021-06-01 20:45:53.000000 t4gpd-0.7.0/t4gpd/commons/sun/PySolarSunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7584 2021-04-22 16:07:47.000000 t4gpd-0.7.0/t4gpd/commons/sun/ShadowLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6719 2021-04-21 15:36:33.000000 t4gpd-0.7.0/t4gpd/commons/sun/SoleneSunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2429 2022-05-18 15:30:31.000000 t4gpd-0.7.0/t4gpd/commons/sun/SunBeamLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8335 2021-12-10 17:17:50.000000 t4gpd-0.7.0/t4gpd/commons/sun/SunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-21 13:30:14.000000 t4gpd-0.7.0/t4gpd/commons/sun/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.355548 t4gpd-0.7.0/t4gpd/demos/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1113 2023-06-08 13:02:08.000000 t4gpd-0.7.0/t4gpd/demos/AbstractGeoDataFrameDemos.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   405923 2023-01-26 09:35:22.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)  1039604 2022-10-25 15:14:06.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   453528 2022-10-25 15:00:19.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos3.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)  2888649 2022-10-25 15:48:49.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos4.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   745426 2022-07-18 15:50:21.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos5.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435846 2022-10-26 14:52:50.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos6.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25686 2022-10-31 17:23:24.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos7.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435537 2022-10-31 17:22:15.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos8.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    87843 2023-03-22 16:19:10.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos9.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   274632 2023-04-27 15:51:16.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosA.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   165333 2023-06-08 13:26:24.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosB.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   193794 2023-06-08 13:03:08.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosC.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-26 22:34:45.000000 t4gpd-0.7.0/t4gpd/demos/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.359548 t4gpd-0.7.0/t4gpd/energy/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12332 2022-04-28 15:33:51.000000 t4gpd-0.7.0/t4gpd/energy/DirectSolarIrradianceLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3194 2022-07-22 08:39:12.000000 t4gpd-0.7.0/t4gpd/energy/Dogniaux.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3035 2022-07-22 08:20:11.000000 t4gpd-0.7.0/t4gpd/energy/Perez.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1107 2022-07-22 08:20:39.000000 t4gpd-0.7.0/t4gpd/energy/Perraudeau.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3305 2022-07-22 08:21:55.000000 t4gpd-0.7.0/t4gpd/energy/PerrinDeBrichambaut.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3748 2022-07-22 08:40:41.000000 t4gpd-0.7.0/t4gpd/energy/PlotDirectNormalIrradiance.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:57:12.000000 t4gpd-0.7.0/t4gpd/energy/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.359548 t4gpd-0.7.0/t4gpd/energy/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4517 2022-05-18 17:36:24.000000 t4gpd-0.7.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-28 20:49:22.000000 t4gpd-0.7.0/t4gpd/energy/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.359548 t4gpd-0.7.0/t4gpd/graph/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1047 2020-12-31 14:32:10.000000 t4gpd-0.7.0/t4gpd/graph/STBetweennessCentrality.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1043 2020-12-19 20:28:37.000000 t4gpd-0.7.0/t4gpd/graph/STClosenessCentrality.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2657 2020-11-23 10:00:25.000000 t4gpd-0.7.0/t4gpd/graph/STRoadNeighborhood.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2459 2020-11-21 19:04:19.000000 t4gpd-0.7.0/t4gpd/graph/STShortestPath.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1644 2020-11-23 10:45:34.000000 t4gpd-0.7.0/t4gpd/graph/STToRoadsSections.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1474 2020-11-23 10:45:52.000000 t4gpd-0.7.0/t4gpd/graph/STToRoadsSectionsNodes.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 07:51:42.000000 t4gpd-0.7.0/t4gpd/graph/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.363548 t4gpd-0.7.0/t4gpd/io/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1120 2023-04-29 15:30:18.000000 t4gpd-0.7.0/t4gpd/io/AbstractReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4231 2020-09-24 09:56:55.000000 t4gpd-0.7.0/t4gpd/io/CSVInertialSensorReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1889 2020-09-24 09:57:20.000000 t4gpd-0.7.0/t4gpd/io/CSVReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1884 2021-03-10 14:24:32.000000 t4gpd-0.7.0/t4gpd/io/CSVWKTReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2317 2021-03-10 14:24:47.000000 t4gpd-0.7.0/t4gpd/io/CSVWKTWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3373 2022-07-25 09:09:50.000000 t4gpd-0.7.0/t4gpd/io/CirReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1314 2022-07-25 09:34:22.000000 t4gpd-0.7.0/t4gpd/io/CirValReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3331 2021-03-10 21:07:26.000000 t4gpd-0.7.0/t4gpd/io/CirWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5578 2020-10-22 16:39:22.000000 t4gpd-0.7.0/t4gpd/io/CityGMLReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7156 2022-06-24 16:06:01.000000 t4gpd-0.7.0/t4gpd/io/GeoWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1829 2022-11-09 15:42:30.000000 t4gpd-0.7.0/t4gpd/io/GpkgLoader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1818 2022-11-09 15:42:30.000000 t4gpd-0.7.0/t4gpd/io/GpkgWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12097 2021-06-25 08:29:09.000000 t4gpd-0.7.0/t4gpd/io/MshReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3750 2020-08-25 16:50:36.000000 t4gpd-0.7.0/t4gpd/io/ObjReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3541 2021-02-01 10:43:14.000000 t4gpd-0.7.0/t4gpd/io/ObjWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1430 2021-07-19 15:31:30.000000 t4gpd-0.7.0/t4gpd/io/Reloading.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1152 2022-04-26 12:38:58.000000 t4gpd-0.7.0/t4gpd/io/STLoadAndClip.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3086 2020-06-19 14:12:42.000000 t4gpd-0.7.0/t4gpd/io/SVGWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5130 2022-07-26 12:53:22.000000 t4gpd-0.7.0/t4gpd/io/SalomeWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5030 2022-07-26 12:53:22.000000 t4gpd-0.7.0/t4gpd/io/SalomeWriterAndExtruder.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6490 2021-03-10 14:25:07.000000 t4gpd-0.7.0/t4gpd/io/VTUWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2492 2022-07-25 09:33:33.000000 t4gpd-0.7.0/t4gpd/io/ValReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2806 2021-11-08 15:20:17.000000 t4gpd-0.7.0/t4gpd/io/ZipLoader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3559 2021-10-18 16:00:12.000000 t4gpd-0.7.0/t4gpd/io/ZipWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 18:59:50.000000 t4gpd-0.7.0/t4gpd/io/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.363548 t4gpd-0.7.0/t4gpd/isovist/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4347 2022-07-27 15:30:51.000000 t4gpd-0.7.0/t4gpd/isovist/STIsovistField2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4697 2023-07-27 17:24:29.000000 t4gpd-0.7.0/t4gpd/isovist/STIsovistField2D_new.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 09:56:41.000000 t4gpd-0.7.0/t4gpd/isovist/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.363548 t4gpd-0.7.0/t4gpd/misc/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4972 2021-07-20 15:59:02.000000 t4gpd-0.7.0/t4gpd/misc/FrequencyHistogram.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5748 2023-03-23 17:02:07.000000 t4gpd-0.7.0/t4gpd/misc/OptimalNumberOfClusters.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5344 2021-11-14 15:44:04.000000 t4gpd-0.7.0/t4gpd/misc/PlotAMatrixOfDiagrams.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2960 2021-10-01 15:35:34.000000 t4gpd-0.7.0/t4gpd/misc/PopulationPyramid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5500 2023-01-19 10:23:40.000000 t4gpd-0.7.0/t4gpd/misc/RoseMappingTool.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3038 2022-03-15 16:20:31.000000 t4gpd-0.7.0/t4gpd/misc/STCompass.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2311 2023-03-23 14:05:55.000000 t4gpd-0.7.0/t4gpd/misc/STDendrogram.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2023-03-23 16:15:02.000000 t4gpd-0.7.0/t4gpd/misc/STKMeans.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4364 2021-01-25 16:17:15.000000 t4gpd-0.7.0/t4gpd/misc/StreetOrientationHistogram.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4386 2022-12-13 18:08:58.000000 t4gpd-0.7.0/t4gpd/misc/TimelineTool.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2824 2021-03-15 16:13:35.000000 t4gpd-0.7.0/t4gpd/misc/WindRose.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-09-29 10:07:30.000000 t4gpd-0.7.0/t4gpd/misc/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.367548 t4gpd-0.7.0/t4gpd/morph/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2873 2021-08-25 16:19:57.000000 t4gpd-0.7.0/t4gpd/morph/GmshTriangulator.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1413 2023-02-17 18:32:38.000000 t4gpd-0.7.0/t4gpd/morph/STBBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1793 2020-06-30 09:46:17.000000 t4gpd-0.7.0/t4gpd/morph/STClip.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4603 2022-08-24 09:39:40.000000 t4gpd-0.7.0/t4gpd/morph/STCoolscapesTessellation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2723 2023-05-23 14:01:31.000000 t4gpd-0.7.0/t4gpd/morph/STCrossroadsGeneration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2853 2023-02-14 11:31:50.000000 t4gpd-0.7.0/t4gpd/morph/STDilationErosion.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2103 2020-12-14 16:55:46.000000 t4gpd-0.7.0/t4gpd/morph/STExtractOpenSpaces.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3726 2021-04-02 09:43:35.000000 t4gpd-0.7.0/t4gpd/morph/STFacadesAnalysis.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8594 2023-02-20 08:30:55.000000 t4gpd-0.7.0/t4gpd/morph/STGradientOfDistancesToBuildings.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2043 2023-07-26 10:17:45.000000 t4gpd-0.7.0/t4gpd/morph/STGrid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3688 2020-09-17 11:02:43.000000 t4gpd-0.7.0/t4gpd/morph/STIdentifyRowOfTrees.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4480 2021-12-09 14:49:10.000000 t4gpd-0.7.0/t4gpd/morph/STMakeBlocks.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1701 2023-06-07 10:51:36.000000 t4gpd-0.7.0/t4gpd/morph/STMakeGroundSurface.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2812 2020-09-21 14:15:12.000000 t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4550 2023-02-20 08:36:37.000000 t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3134 2022-06-13 13:37:40.000000 t4gpd-0.7.0/t4gpd/morph/STPointsDensifier.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2118 2022-06-13 13:11:05.000000 t4gpd-0.7.0/t4gpd/morph/STPointsDensifier2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1717 2020-12-31 16:03:16.000000 t4gpd-0.7.0/t4gpd/morph/STPolygonize.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3105 2023-02-15 17:59:34.000000 t4gpd-0.7.0/t4gpd/morph/STSkeletonize.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2294 2023-02-15 20:25:15.000000 t4gpd-0.7.0/t4gpd/morph/STSkeletonizeTheVoid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6054 2023-07-27 20:19:56.000000 t4gpd-0.7.0/t4gpd/morph/STSkyMap25D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3196 2020-09-24 10:27:56.000000 t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6567 2022-08-24 09:55:25.000000 t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3217 2021-05-18 08:45:03.000000 t4gpd-0.7.0/t4gpd/morph/STSpatialJoin.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1568 2022-10-14 10:00:03.000000 t4gpd-0.7.0/t4gpd/morph/STSquaredBBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2628 2023-01-31 10:54:56.000000 t4gpd-0.7.0/t4gpd/morph/STVariableWidthBuffer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3729 2020-09-25 16:31:01.000000 t4gpd-0.7.0/t4gpd/morph/STVoronoiPartition.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 10:00:08.000000 t4gpd-0.7.0/t4gpd/morph/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.371548 t4gpd-0.7.0/t4gpd/morph/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      941 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2895 2020-06-19 14:16:30.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AngularAbscissa.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1132 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4153 2023-01-30 15:34:51.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AspectRatio.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1003 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/BBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1813 2023-02-14 11:19:09.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1996 2020-10-07 15:31:07.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1851 2020-12-18 22:37:53.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CircularityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      946 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexHull.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1917 2020-12-18 22:29:45.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1903 2022-11-07 14:15:37.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4022 2022-11-08 14:46:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5107 2023-02-20 08:57:36.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1136 2020-06-19 14:45:22.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/Diameter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2106 2020-12-30 20:08:51.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/EllipticityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3512 2022-07-22 14:38:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/FootprintExtruder.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1100 2021-06-21 13:53:15.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1227 2022-03-28 12:36:54.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/GridFace.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2283 2023-01-30 16:12:41.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/HMean.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2179 2023-01-30 14:29:24.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2481 2021-02-14 18:01:56.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1564 2023-01-30 13:38:38.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2342 2020-06-23 22:09:00.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABE.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      954 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1067 2021-01-10 10:06:31.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1094 2020-12-15 16:02:50.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MBC.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1065 2020-12-15 20:28:55.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MPBR.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1600 2020-12-30 20:09:13.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectangularityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1374 2022-11-08 14:46:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFFT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1749 2022-11-08 14:46:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFWT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1018 2020-06-19 07:17:45.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RemoveHoles.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1628 2022-06-24 16:06:35.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RepresentativePoint.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1235 2021-04-26 14:02:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/Rotation2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2023-03-15 18:24:43.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/STGeoProcess.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3139 2023-01-30 13:39:08.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyMap2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2996 2023-01-30 15:49:55.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactor.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3657 2021-03-03 16:15:56.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1687 2022-01-18 09:14:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/StarShapedIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1898 2023-01-30 14:30:54.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SurfaceFraction.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1978 2021-04-26 13:48:42.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/Translation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1792 2023-01-30 16:09:52.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/WMean.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-16 15:16:57.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/picoclim/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5476 2023-06-11 13:49:34.000000 t4gpd-0.7.0/t4gpd/picoclim/CampbellSciReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2312 2023-06-11 16:53:22.000000 t4gpd-0.7.0/t4gpd/picoclim/ExtraProcessing.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7497 2023-05-08 20:58:34.000000 t4gpd-0.7.0/t4gpd/picoclim/InertialMeasureReWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5574 2023-06-09 07:25:25.000000 t4gpd-0.7.0/t4gpd/picoclim/InertialMeasureReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3624 2023-03-22 16:43:01.000000 t4gpd-0.7.0/t4gpd/picoclim/JoinByTimeDistance.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6343 2023-06-09 07:11:48.000000 t4gpd-0.7.0/t4gpd/picoclim/KestrelReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2305 2022-10-26 10:49:53.000000 t4gpd-0.7.0/t4gpd/picoclim/MeteoFranceReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15062 2023-03-22 14:23:02.000000 t4gpd-0.7.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8963 2023-06-15 07:06:57.000000 t4gpd-0.7.0/t4gpd/picoclim/MetrologicalCampaignReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3314 2023-06-09 07:21:40.000000 t4gpd-0.7.0/t4gpd/picoclim/SensirionReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6589 2023-05-16 06:56:35.000000 t4gpd-0.7.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7288 2023-06-13 09:00:04.000000 t4gpd-0.7.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3531 2023-05-16 07:41:21.000000 t4gpd-0.7.0/t4gpd/picoclim/TracksWaypointsReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15960 2023-06-13 08:00:50.000000 t4gpd-0.7.0/t4gpd/picoclim/UClimGuidingReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2860 2023-06-13 08:14:48.000000 t4gpd-0.7.0/t4gpd/picoclim/UClimTrackWaypointsReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-09-15 08:50:25.000000 t4gpd-0.7.0/t4gpd/picoclim/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyplot/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4516 2022-11-07 14:14:25.000000 t4gpd-0.7.0/t4gpd/pyplot/MultipleMarkerStyles.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-01-31 17:29:02.000000 t4gpd-0.7.0/t4gpd/pyplot/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyqgis/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3438 2022-07-29 07:32:07.000000 t4gpd-0.7.0/t4gpd/pyqgis/AddMemoryLayer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1629 2022-07-27 20:17:41.000000 t4gpd-0.7.0/t4gpd/pyqgis/Emphasizer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8447 2022-07-10 14:41:36.000000 t4gpd-0.7.0/t4gpd/pyqgis/MapPrinter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5785 2021-09-10 17:42:22.000000 t4gpd-0.7.0/t4gpd/pyqgis/PdfMapWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    10441 2023-04-14 15:51:46.000000 t4gpd-0.7.0/t4gpd/pyqgis/SetSymbolLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1323 2021-09-10 16:28:27.000000 t4gpd-0.7.0/t4gpd/pyqgis/ShowFeatureCount.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1746 2021-09-24 09:47:44.000000 t4gpd-0.7.0/t4gpd/pyqgis/ZoomLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-09-09 16:49:22.000000 t4gpd-0.7.0/t4gpd/pyqgis/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyvista/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3711 2022-09-02 07:34:06.000000 t4gpd-0.7.0/t4gpd/pyvista/GeodeCiel.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4689 2022-09-01 16:13:45.000000 t4gpd-0.7.0/t4gpd/pyvista/Icosahedron.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8601 2023-06-26 13:48:29.000000 t4gpd-0.7.0/t4gpd/pyvista/Plotter3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2043 2022-06-22 15:52:10.000000 t4gpd-0.7.0/t4gpd/pyvista/STRaysToViewFactors.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3916 2022-06-05 15:29:14.000000 t4gpd-0.7.0/t4gpd/pyvista/ToPolyData.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4642 2022-09-25 09:28:13.000000 t4gpd-0.7.0/t4gpd/pyvista/ToUnstructuredGrid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-05 17:09:50.000000 t4gpd-0.7.0/t4gpd/pyvista/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyvista/commons/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1805 2022-09-05 12:42:46.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/Diameter3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8778 2022-09-01 16:15:11.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/RayCasting3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7389 2022-09-05 16:44:01.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8995 2022-09-07 10:57:40.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/SVF3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3683 2022-08-23 11:33:51.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/Triangle3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-05 21:07:30.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3127 2022-07-18 15:37:08.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1398 2022-07-18 07:24:52.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1686 2022-06-22 16:23:38.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4679 2022-08-22 15:26:00.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4542 2022-08-24 08:46:07.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6047 2022-09-05 16:44:47.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3951 2022-09-05 16:45:02.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/SVF3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-09 11:51:20.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/raster/
+-rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)     2916 2022-06-01 18:54:37.000000 t4gpd-0.7.0/t4gpd/raster/STToRaster.py
+-rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2022-06-01 12:59:39.000000 t4gpd-0.7.0/t4gpd/raster/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.379548 t4gpd-0.7.0/t4gpd/sun/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2021-04-22 15:43:22.000000 t4gpd-0.7.0/t4gpd/sun/AbstractHardShadow.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3176 2022-05-18 15:39:03.000000 t4gpd-0.7.0/t4gpd/sun/STHardShadow.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4002 2022-05-18 15:39:34.000000 t4gpd-0.7.0/t4gpd/sun/STSunMap2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3423 2022-05-18 15:44:21.000000 t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4353 2022-05-18 15:44:39.000000 t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:41:14.000000 t4gpd-0.7.0/t4gpd/sun/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.379548 t4gpd-0.7.0/t4gpd/sun/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2489 2021-04-21 16:17:23.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2218 2021-04-21 16:17:37.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDuration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4779 2021-04-21 16:17:58.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-03 15:05:24.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.335548 t4gpd-0.7.0/t4gpd.egg-info/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2545 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/PKG-INFO
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11205 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/SOURCES.txt
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        1 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/dependency_links.txt
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        6 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/top_level.txt
```

### Comparing `t4gpd-0.6.0/LICENSE.txt` & `t4gpd-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/PKG-INFO` & `t4gpd-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.6.0
+Version: 0.7.0
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
 Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
@@ -33,17 +33,17 @@
 
 > conda activate gpd
 
 > conda config --env --add channels conda-forge
 
 > conda config --env --set channel_priority strict
 
-> conda install geopandas descartes matplotlib networkx notebook numpy pysolar plotly
+> conda install python=3.10 geopandas=0.12.2 jupyterlab matplotlib notebook scikit-learn xlrd openpyxl imageio rasterio networkx PyWavelets pysolar windrose geocube mapclassify seaborn plotly matplotlib-scalebar pyvista contextily xlwt
 
-> pip install matplotlib-scalebar Dijkstar suntimes windrose
+> pip install Dijkstar suntimes pythermalcomfort
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
 > pip install t4gpd-0.6.0.tar.gz
```

### Comparing `t4gpd-0.6.0/setup.py` & `t4gpd-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/__init__.py` & `t4gpd-0.7.0/t4gpd/__init__.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/_version.py` & `t4gpd-0.7.0/t4gpd/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 # The following line *must* be the last in the module, exactly as formatted:
-__version__ = '0.6.0'
+__version__ = '0.7.0'
```

### Comparing `t4gpd-0.6.0/t4gpd/comfort/EmpiricalThermalIndices.py` & `t4gpd-0.7.0/t4gpd/comfort/EmpiricalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/LinearThermalIndices.py` & `t4gpd-0.7.0/t4gpd/comfort/LinearThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/UniversalThermalIndices.py` & `t4gpd-0.7.0/t4gpd/comfort/UniversalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/CommonsLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/CommonsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/ConstantsLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/ConstantsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/ETULib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/ETULib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/PETLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/PETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/PMVLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/PMVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/PTLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/PTLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/SETLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/SETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/SET_mist.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/SET_mist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/TmrtOutLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/TmrtOutLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/UTCILib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/UTCILib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/VDI_PET_corrected.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/VDI_PET_corrected.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py` & `t4gpd-0.7.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/ASV.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/ASV.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/DI.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/DI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/ETU.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/ETU.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/H.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/H.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/HI.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/HI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/NET.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/NET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/OUTSET.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/OUTSET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/PE.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/PE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/PET.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/PMV.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-'''
-Created on 11 mai 2021
-
-@author: tleduc
-
-Copyright 2020-2021 Thomas Leduc
-
-This file is part of t4gpd.
-
-t4gpd is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-t4gpd is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
-'''
-from numpy import isnan
-from pandas import DataFrame
-from t4gpd.comfort.algo.PETLib import PETLib
-from t4gpd.comfort.indices.AbstractThermalComfortIndice import AbstractThermalComfortIndice
-from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-
-
-class PET(AbstractThermalComfortIndice):
-    '''
-    classdocs
-    '''
-
-    def __init__(self, sensorsGdf, AirTC='AirTC_Avg', RH='RH_Avg', WS_ms='WS_ms_Avg',
-                 T_mrt='T_mrt'):
-        '''
-        Constructor
-
-        AirTC: air temperature [C]
-        RH: relative humidity [%]
-        Ws_ms: wind speed recorded at pedestrian level (at height 1.1 m) [m.s-1]
-        T_mrt: Mean radiant temperature [C]
-        
-        PET: Physiologically Equivalent Temperature
-        '''
-        if not isinstance(sensorsGdf, DataFrame):
-            raise IllegalArgumentTypeException(sensorsGdf, 'DataFrame')
-
-        for fieldname in (AirTC, RH, WS_ms, T_mrt):
-            if fieldname not in sensorsGdf:
-                raise Exception('%s is not a relevant field name!' % fieldname)
-
-        self.AirTC = AirTC
-        self.RH = RH
-        self.WS_ms = WS_ms
-        self.T_mrt = T_mrt
-
-    @staticmethod
-    def thermalPerceptionRanges():
-        # Excerpt from https://doi.org/10.1016/j.wace.2018.01.004
-        return {
-            'Extreme cold': { 'min':-float('inf'), 'max':4, 'color': '#003075' },
-            'Strong cold': { 'min':4, 'max':8, 'color': '#00c2f7' },
-            'Moderate cold': { 'min':8, 'max': 13, 'color': '#91c1e1' },
-            'Slight cold': { 'min': 13, 'max': 18, 'color': '#dbebf5' },
-            'Comfortable': { 'min': 18, 'max': 23, 'color': '#ffffff' },
-            'Slight heat': { 'min': 23, 'max': 29, 'color': '#ffdabd' },
-            'Moderate heat': { 'min': 29, 'max': 35, 'color': '#fffa00' },
-            'Strong heat': { 'min': 35, 'max': 41, 'color': '#ff7900' },
-            'Extreme heat': { 'min': 41, 'max': float('inf'), 'color': '#ff0000' }
-            }
-
-    def runWithArgs(self, row):
-        AirTC = row[self.AirTC]
-        RH = row[self.RH]
-        WS_ms = row[self.WS_ms]
-        T_mrt = row[self.T_mrt]
-
-        PET = None
-        if not (isnan(AirTC) or isnan(RH) or isnan(WS_ms) or isnan(T_mrt)):
-            # PET: Physiologically Equivalent Temperature
-            _, _, _, PET = PETLib.assess_pet(AirTC, RH, WS_ms, T_mrt) 
-
-        return { 'PET': PET }
+'''
+Created on 12 mai 2021
+
+@author: tleduc
+
+Copyright 2020-2021 Thomas Leduc
+
+This file is part of t4gpd.
+
+t4gpd is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+t4gpd is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
+'''
+from numpy import isnan
+from pandas.core.frame import DataFrame
+from t4gpd.comfort.algo.PMVLib import PMVLib
+from t4gpd.comfort.indices.AbstractThermalComfortIndice import AbstractThermalComfortIndice
+from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
+
+
+class PMV(AbstractThermalComfortIndice):
+    '''
+    classdocs
+    '''
+
+    def __init__(self, sensorsGdf, AirTC='AirTC_Avg', RH='RH_Avg', WS_ms='WS_ms_Avg',
+                 T_mrt='T_mrt'):
+        '''
+        Constructor
+
+        AirTC: air temperature [C]
+        RH: relative humidity [%]
+        Ws_ms: wind speed recorded at pedestrian level (at height 1.1 m) [m.s-1]
+        T_mrt: Mean radiant temperature [C]
+        
+        PMV: Predicted Mean Vote
+        '''
+        if not isinstance(sensorsGdf, DataFrame):
+            raise IllegalArgumentTypeException(sensorsGdf, 'DataFrame')
+
+        for fieldname in (AirTC, RH, WS_ms, T_mrt):
+            if fieldname not in sensorsGdf:
+                raise Exception('%s is not a relevant field name!' % fieldname)
+
+        self.AirTC = AirTC
+        self.RH = RH
+        self.WS_ms = WS_ms
+        self.T_mrt = T_mrt
+
+    @staticmethod
+    def thermalPerceptionRanges():
+        # Excerpt from https://doi.org/10.1016/j.wace.2018.01.004
+        return {
+            'Extreme cold': { 'min':-float('inf'), 'max':-3, 'color': '#003075' },
+            'Strong cold': { 'min':-3, 'max':-2.5, 'color': '#00c2f7' },
+            'Moderate cold': { 'min':-2.5, 'max':-1.5, 'color': '#91c1e1' },
+            'Slight cold': { 'min':-1.5, 'max':-0.5, 'color': '#dbebf5' },
+            'Comfortable': { 'min':-0.5, 'max': 0, 'color': '#ffffff' },
+            'Slight heat': { 'min': 0, 'max': 0.5, 'color': '#ffdabd' },
+            'Moderate heat': { 'min': 0.5, 'max': 1.5, 'color': '#fffa00' },
+            'Strong heat': { 'min': 1.5, 'max': 2.5, 'color': '#ff7900' },
+            'Extreme heat': { 'min': 2.5, 'max': float('inf'), 'color': '#ff0000' }
+            }
+
+    def runWithArgs(self, row):
+        AirTC = row[self.AirTC]
+        RH = row[self.RH]
+        WS_ms = row[self.WS_ms]
+        T_mrt = row[self.T_mrt]
+
+        PMV = None
+        if not (isnan(AirTC) or isnan(RH) or isnan(WS_ms) or isnan(T_mrt)):
+            # PMV: Predicted Mean Vote
+            PMV = PMVLib.assess_pmv(AirTC, RH, WS_ms, T_mrt)
+
+        return { 'PMV': PMV }
```

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/PMV.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/SET.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,35 +18,35 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from numpy import isnan
 from pandas.core.frame import DataFrame
-from t4gpd.comfort.algo.PMVLib import PMVLib
+from t4gpd.comfort.algo.SETLib import SETLib
 from t4gpd.comfort.indices.AbstractThermalComfortIndice import AbstractThermalComfortIndice
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
-class PMV(AbstractThermalComfortIndice):
+class SET(AbstractThermalComfortIndice):
     '''
     classdocs
     '''
 
     def __init__(self, sensorsGdf, AirTC='AirTC_Avg', RH='RH_Avg', WS_ms='WS_ms_Avg',
                  T_mrt='T_mrt'):
         '''
         Constructor
 
         AirTC: air temperature [C]
         RH: relative humidity [%]
         Ws_ms: wind speed recorded at pedestrian level (at height 1.1 m) [m.s-1]
         T_mrt: Mean radiant temperature [C]
-        
-        PMV: Predicted Mean Vote
+
+        SET: Standard Effective Temperature
         '''
         if not isinstance(sensorsGdf, DataFrame):
             raise IllegalArgumentTypeException(sensorsGdf, 'DataFrame')
 
         for fieldname in (AirTC, RH, WS_ms, T_mrt):
             if fieldname not in sensorsGdf:
                 raise Exception('%s is not a relevant field name!' % fieldname)
@@ -56,30 +56,26 @@
         self.WS_ms = WS_ms
         self.T_mrt = T_mrt
 
     @staticmethod
     def thermalPerceptionRanges():
         # Excerpt from https://doi.org/10.1016/j.wace.2018.01.004
         return {
-            'Extreme cold': { 'min':-float('inf'), 'max':-3, 'color': '#003075' },
-            'Strong cold': { 'min':-3, 'max':-2.5, 'color': '#00c2f7' },
-            'Moderate cold': { 'min':-2.5, 'max':-1.5, 'color': '#91c1e1' },
-            'Slight cold': { 'min':-1.5, 'max':-0.5, 'color': '#dbebf5' },
-            'Comfortable': { 'min':-0.5, 'max': 0, 'color': '#ffffff' },
-            'Slight heat': { 'min': 0, 'max': 0.5, 'color': '#ffdabd' },
-            'Moderate heat': { 'min': 0.5, 'max': 1.5, 'color': '#fffa00' },
-            'Strong heat': { 'min': 1.5, 'max': 2.5, 'color': '#ff7900' },
-            'Extreme heat': { 'min': 2.5, 'max': float('inf'), 'color': '#ff0000' }
+            'Moderate cold': { 'min':-float('inf'), 'max': 17, 'color': '#91c1e1' },
+            'Comfortable': { 'min': 17, 'max': 30, 'color': '#ffffff' },
+            'Moderate heat': { 'min': 30, 'max': 34, 'color': '#fffa00' },
+            'Strong heat': { 'min': 34, 'max': 37, 'color': '#ff7900' },
+            'Extreme heat': { 'min': 37, 'max': float('inf'), 'color': '#ff0000' }
             }
 
     def runWithArgs(self, row):
         AirTC = row[self.AirTC]
         RH = row[self.RH]
         WS_ms = row[self.WS_ms]
         T_mrt = row[self.T_mrt]
 
-        PMV = None
+        SET = None
         if not (isnan(AirTC) or isnan(RH) or isnan(WS_ms) or isnan(T_mrt)):
-            # PMV: Predicted Mean Vote
-            PMV = PMVLib.assess_pmv(AirTC, RH, WS_ms, T_mrt)
+            # SET: Standard Effective Temperature
+            SET = SETLib.assess_set(AirTC, RH, WS_ms, T_mrt)
 
-        return { 'PMV': PMV }
+        return { 'SET': SET }
```

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/PT.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/PT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/SET.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/THI.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,64 +18,49 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from numpy import isnan
 from pandas.core.frame import DataFrame
-from t4gpd.comfort.algo.SETLib import SETLib
 from t4gpd.comfort.indices.AbstractThermalComfortIndice import AbstractThermalComfortIndice
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
-class SET(AbstractThermalComfortIndice):
+class THI(AbstractThermalComfortIndice):
     '''
     classdocs
     '''
 
-    def __init__(self, sensorsGdf, AirTC='AirTC_Avg', RH='RH_Avg', WS_ms='WS_ms_Avg',
-                 T_mrt='T_mrt'):
+    def __init__(self, sensorsGdf, AirTC='AirTC_Avg', RH='RH_Avg'):
         '''
         Constructor
 
         AirTC: air temperature [C]
         RH: relative humidity [%]
-        Ws_ms: wind speed recorded at pedestrian level (at height 1.1 m) [m.s-1]
-        T_mrt: Mean radiant temperature [C]
 
-        SET: Standard Effective Temperature
+        THI: Temperature-Humidity Index (THI) stated in Grosdemouge (2020) 
+        after (Emmanuel et al., 2016) in humid and hot environment
+        *** 21-24: 100% des personnes en situation de confort
+        *** 24-26: 50% des personnes en situation de confort
+        *** > 26: 100% des personnes en situation d'inconfort lie a la chaleur
         '''
         if not isinstance(sensorsGdf, DataFrame):
             raise IllegalArgumentTypeException(sensorsGdf, 'DataFrame')
 
-        for fieldname in (AirTC, RH, WS_ms, T_mrt):
+        for fieldname in (AirTC, RH):
             if fieldname not in sensorsGdf:
                 raise Exception('%s is not a relevant field name!' % fieldname)
 
         self.AirTC = AirTC
         self.RH = RH
-        self.WS_ms = WS_ms
-        self.T_mrt = T_mrt
-
-    @staticmethod
-    def thermalPerceptionRanges():
-        # Excerpt from https://doi.org/10.1016/j.wace.2018.01.004
-        return {
-            'Moderate cold': { 'min':-float('inf'), 'max': 17, 'color': '#91c1e1' },
-            'Comfortable': { 'min': 17, 'max': 30, 'color': '#ffffff' },
-            'Moderate heat': { 'min': 30, 'max': 34, 'color': '#fffa00' },
-            'Strong heat': { 'min': 34, 'max': 37, 'color': '#ff7900' },
-            'Extreme heat': { 'min': 37, 'max': float('inf'), 'color': '#ff0000' }
-            }
 
     def runWithArgs(self, row):
         AirTC = row[self.AirTC]
         RH = row[self.RH]
-        WS_ms = row[self.WS_ms]
-        T_mrt = row[self.T_mrt]
 
-        SET = None
-        if not (isnan(AirTC) or isnan(RH) or isnan(WS_ms) or isnan(T_mrt)):
-            # SET: Standard Effective Temperature
-            SET = SETLib.assess_set(AirTC, RH, WS_ms, T_mrt)
+        THI = None
+        if not (isnan(AirTC) or isnan(RH)):
+            # THI: Temperature-Humidity Index
+            THI = 0.8 * AirTC + (AirTC * RH) / 500
 
-        return { 'SET': SET }
+        return { 'THI': THI }
```

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/SETmist.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/SETmist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/TmrtOut.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/TmrtOut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/TmrtRadiometer.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/TmrtRadiometer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/comfort/indices/WCT.py` & `t4gpd-0.7.0/t4gpd/comfort/indices/WCT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/AngleLib.py` & `t4gpd-0.7.0/t4gpd/commons/AngleLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/ArrayCoding.py` & `t4gpd-0.7.0/t4gpd/commons/ArrayCoding.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/BoundingBox.py` & `t4gpd-0.7.0/t4gpd/commons/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/CSVLib.py` & `t4gpd-0.7.0/t4gpd/commons/CSVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/CalendarLib.py` & `t4gpd-0.7.0/t4gpd/commons/CalendarLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/CaliperLib.py` & `t4gpd-0.7.0/t4gpd/commons/CaliperLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/Checksum.py` & `t4gpd-0.7.0/t4gpd/commons/Checksum.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/ChrystalAlgorithm.py` & `t4gpd-0.7.0/t4gpd/commons/ChrystalAlgorithm.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/DataFrameLib.py` & `t4gpd-0.7.0/t4gpd/commons/DataFrameLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/DateRangeLib.py` & `t4gpd-0.7.0/t4gpd/commons/DateRangeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/DatetimeLib.py` & `t4gpd-0.7.0/t4gpd/commons/DatetimeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/DiameterLib.py` & `t4gpd-0.7.0/t4gpd/commons/DiameterLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/Distances.py` & `t4gpd-0.7.0/t4gpd/commons/Distances.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/Entropy.py` & `t4gpd-0.7.0/t4gpd/commons/Entropy.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/Epsilon.py` & `t4gpd-0.7.0/t4gpd/commons/Epsilon.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/GeoDataFrameLib.py` & `t4gpd-0.7.0/t4gpd/commons/GeoDataFrameLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/GeoProcess.py` & `t4gpd-0.7.0/t4gpd/commons/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/GeomLib.py` & `t4gpd-0.7.0/t4gpd/commons/GeomLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/GeomLib3D.py` & `t4gpd-0.7.0/t4gpd/commons/GeomLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/GridFaceLib.py` & `t4gpd-0.7.0/t4gpd/commons/GridFaceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/IllegalArgumentTypeException.py` & `t4gpd-0.7.0/t4gpd/commons/IllegalArgumentTypeException.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/KernelLib.py` & `t4gpd-0.7.0/t4gpd/commons/KernelLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/LandoltRingLib.py` & `t4gpd-0.7.0/t4gpd/commons/LandoltRingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/LatLonLib.py` & `t4gpd-0.7.0/t4gpd/commons/LatLonLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/LineStringCuttingLib.py` & `t4gpd-0.7.0/t4gpd/commons/LineStringCuttingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/ListUtilities.py` & `t4gpd-0.7.0/t4gpd/commons/ListUtilities.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/Logos.py` & `t4gpd-0.7.0/t4gpd/commons/Logos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/MyEdge.py` & `t4gpd-0.7.0/t4gpd/commons/MyEdge.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/MyNode.py` & `t4gpd-0.7.0/t4gpd/commons/MyNode.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/PointsDensifierLib.py` & `t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/PointsDensifierLib3D.py` & `t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/PolarCartesianCoordinates.py` & `t4gpd-0.7.0/t4gpd/commons/PolarCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/RayCasting2Lib.py` & `t4gpd-0.7.0/t4gpd/commons/RayCasting2Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/RayCasting3Lib.py` & `t4gpd-0.7.0/t4gpd/commons/RayCasting3Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/RayCastingLib.py` & `t4gpd-0.7.0/t4gpd/commons/RayCastingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/RotationLib.py` & `t4gpd-0.7.0/t4gpd/commons/RotationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/SVFLib.py` & `t4gpd-0.7.0/t4gpd/commons/SVFLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/ShannonEntropy.py` & `t4gpd-0.7.0/t4gpd/commons/ShannonEntropy.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/SphericalCartesianCoordinates.py` & `t4gpd-0.7.0/t4gpd/commons/SphericalCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/SphericalProjectionLib.py` & `t4gpd-0.7.0/t4gpd/commons/SphericalProjectionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/TestUtils.py` & `t4gpd-0.7.0/t4gpd/commons/TestUtils.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_generation/Sequence.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_generation/Sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from shapely.geometry import Point
 from shapely.ops import unary_union
 
 
 class Sequence(object):
     '''
     classdocs
     '''
@@ -74,15 +73,15 @@
             return True
         for i in range(1, self.nbranchs):
             if (self.__strictEquality(otherSequence.rotate(i))):
                 return True
         return False
 
     def __isContinuousItem(self, item):
-        return (isinstance(item, list) or isinstance(item, tuple))
+        return isinstance(item, (list, tuple))
 
     def __isValidItem(self, item):
         if self.__isContinuousItem(item):
             return (((0 == item[0]) and (self.nbranchs == item[1])) or 
                     ((item[0] in range(self.nbranchs)) and (item[1] in range(self.nbranchs)))) 
         return (item in range(self.nbranchs))
 
@@ -116,26 +115,24 @@
                         item, self.nbranchs - 1, self.nbranchs - 1, self.nbranchs - 1))
         # A CONTINUER
 
     def rotate(self, offset=1):
         newseq = [self.__plus(item, offset) for item in self.seq]
         return Sequence(self.nbranchs, newseq, self.__mirror)
 
-    def asPolygon(self, sequenceRadii, width, centre=[0, 0]):
-        polygons = list()
-        polygon = Point(centre).buffer(0.5 * width, -1)
-        polygons.append(polygon)
+    def asPolygon(self, sequenceRadii, centre=[0, 0]):
+        geoms = []
 
         for item in self.seq:
             if self.__isContinuousItem(item):
-                polygon = sequenceRadii.getSector(item, centre)
+                geoms.append(sequenceRadii.getSector(item, centre))
             else:
-                polygon = sequenceRadii.getBranch(item, centre)
-            polygons.append(polygon)
-        result = unary_union(polygons)
+                geoms.append(sequenceRadii.getBranch(item, centre))
+
+        result = unary_union(geoms).buffer(sequenceRadii.getWidth())
         return result
 
     def getMinModel(self):
         if (4 == self.nbranchs):
             return 4
 
         if (0 == (self.nbranchs % 4)):
```

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_identification/AbstractMethod.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/AbstractMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_identification/FFTMethod.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FFTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_identification/FWTMethod.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FWTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py` & `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/ellipse/EllipseLib.py` & `t4gpd-0.7.0/t4gpd/commons/ellipse/EllipseLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/ellipse/EllipticHullLib.py` & `t4gpd-0.7.0/t4gpd/commons/ellipse/EllipticHullLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py` & `t4gpd-0.7.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/graph/MCALib.py` & `t4gpd-0.7.0/t4gpd/commons/graph/MCALib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/graph/NeighborhoodLib.py` & `t4gpd-0.7.0/t4gpd/commons/graph/NeighborhoodLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/graph/ShortestPathLib.py` & `t4gpd-0.7.0/t4gpd/commons/graph/ShortestPathLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/graph/UrbanGraphLib.py` & `t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/graph/UrbanGraphLibOld.py` & `t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLibOld.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/grid/AbstractGridLib.py` & `t4gpd-0.7.0/t4gpd/commons/grid/AbstractGridLib.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
+from geopandas import GeoDataFrame, overlay
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
 class AbstractGridLib(object):
     '''
     classdocs
@@ -40,30 +40,32 @@
         self.dx = dx
         self.dy = dx if (dy is None) else dy
         self.encode = encode
 
     def grid(self):
         raise NotImplementedError('grid() must be overridden!')
 
+    def __overlayWithGrid(self, grid, how="difference"):
+        _result = grid.loc[:, ["gid", "geometry"]]
+        _result.geometry = _result.geometry.apply(lambda geom: geom.centroid)
+        _result = overlay(_result, self.gdf, how)
+        _result = set(_result.gid.to_list())
+        return _result
+
     def indoorGrid(self):
         _grid = self.indoorOutdoorGrid()
-        _grid = _grid.loc[ _grid[_grid.indoor == 1].index ]
+        _grid = _grid.loc[_grid[_grid.indoor == 1].index]
         _grid.reset_index(drop=True, inplace=True)
         return _grid
 
     def indoorOutdoorGrid(self):
         _grid = self.grid()
-        rows = []
-        for _, row in _grid.iterrows():
-            _row = dict(row)
-            _centroid = row['geometry'].centroid
-            _indoor = 1 if (GeomLib.isAnIndoorPoint(_centroid, self.gdf)) else 0
-            _row['indoor'] = _indoor
-            rows.append(_row)
-        _grid = GeoDataFrame(rows, crs=self.gdf.crs)
+        _gids = self.__overlayWithGrid(_grid, how="difference")
+        _grid["indoor"] = _grid.gid.apply(
+            lambda gid: 0 if (gid in _gids) else 1)
         return _grid
 
     def outdoorGrid(self):
         _grid = self.indoorOutdoorGrid()
-        _grid = _grid.loc[ _grid[_grid.indoor == 0].index ]
+        _grid = _grid.loc[_grid[_grid.indoor == 0].index]
         _grid.reset_index(drop=True, inplace=True)
         return _grid
```

### Comparing `t4gpd-0.6.0/t4gpd/commons/grid/GridLib.py` & `t4gpd-0.7.0/t4gpd/commons/grid/GridLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/rnd/RandomPointPicking.py` & `t4gpd-0.7.0/t4gpd/commons/rnd/RandomPointPicking.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas.geodataframe import GeoDataFrame
-from numpy import arcsin, asarray, cos, pi, sin, sqrt, vstack, where
-from numpy.random import uniform
+from numpy import arcsin, asarray, cos, pi, round, sin, sqrt, vstack, where
+from numpy.random import default_rng, uniform
 from shapely.geometry import Point, Polygon
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.GeomLib3D import GeomLib3D
 
 
 class RandomPointPicking(object):
     '''
@@ -40,23 +40,28 @@
         resultat = []
         for i, ipp in zip(range(1, n - 1), range(2, n)):
             resultat.append(Polygon([coords[0], coords[i], coords[ipp]]))
         return resultat
     
     @staticmethod
     def convexPolygonPointPicking(ngon, npts):
+        rng = default_rng()
         # INSPIRED BY:
         # https://blogs.sas.com/content/iml/2020/10/21/random-points-in-polygon.html
         assert isinstance(ngon, Polygon), 'ngon is expected to be a Shapely Polygon!'
         assert GeomLib.isConvex(ngon), 'ngon is expected to be convex!'
         tris = RandomPointPicking._simpleTriangulation(ngon)
         # areas = [tri.area for tri in tris]
         areas = asarray([GeomLib3D.getArea(tri) for tri in tris])
         ratios = areas / areas.sum() 
-        listOfNpts = (npts * ratios).astype(int)
+        listOfNpts = round(npts * ratios).astype(int)
+
+        choices = [0] * len(tris) + [1] * npts
+        listOfNpts[listOfNpts == 0] = rng.choice(choices, size=len(listOfNpts[listOfNpts == 0]))
+
         resultat = []
         for tri, _npts in zip(tris, listOfNpts):
             resultat.append(RandomPointPicking.trianglePointPicking(tri, _npts))
         return vstack(resultat)
 
     @staticmethod
     def trianglePointPicking(tri, npts):
```

### Comparing `t4gpd-0.6.0/t4gpd/commons/sun/AbstractSunLib.py` & `t4gpd-0.7.0/t4gpd/commons/sun/AbstractSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/sun/DaylightLib.py` & `t4gpd-0.7.0/t4gpd/commons/sun/DaylightLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/sun/PySolarSunLib.py` & `t4gpd-0.7.0/t4gpd/commons/sun/PySolarSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/sun/ShadowLib.py` & `t4gpd-0.7.0/t4gpd/commons/sun/ShadowLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/sun/SoleneSunLib.py` & `t4gpd-0.7.0/t4gpd/commons/sun/SoleneSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/sun/SunBeamLib.py` & `t4gpd-0.7.0/t4gpd/commons/sun/SunBeamLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/commons/sun/SunLib.py` & `t4gpd-0.7.0/t4gpd/commons/sun/SunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/AbstractGeoDataFrameDemos.py` & `t4gpd-0.7.0/t4gpd/io/AbstractReader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 17 feb. 2022
+Created on 22 juin 2022
 
 @author: tleduc
 
 Copyright 2020-2022 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,17 +16,24 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
+from io import StringIO
 
+from t4gpd.commons.GeoProcess import GeoProcess
 
-class AbstractGeoDataFrameDemos(object):
+
+class AbstractReader(GeoProcess):
     '''
     classdocs
     '''
 
     @staticmethod
-    def postprocess(sio, crs='epsg:2154'):
-        raise Exception('Deprecated!')
+    def opener(inputFile):
+        if isinstance(inputFile, StringIO):
+            # There is no way to re-open a StringIO object, so let's duplicate it
+            return StringIO(inputFile.getvalue())
+        else:
+            return open(inputFile, 'r')
```

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos2.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos3.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos4.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos4.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos5.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos5.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos6.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos6.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos7.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos7.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos8.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos8.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemos9.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos9.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/demos/GeoDataFrameDemosA.py` & `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosA.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,30 +98,39 @@
     def intraPeripheriqueNantes():
         _sio = StringIO("""geometry
 POLYGON ((356389.5 6683116.3, 356362.5 6683112.6, 356312.1 6683108.2, 356264.2 6683103.7, 356223 6683101.6, 356179.4 6683100.9, 356134.6 6683100.3, 356101.6 6683100.6, 356094.5 6683100.6, 356083.5 6683100.9, 356083.2 6683100.9, 356078.1 6683101, 356068.6 6683101.1, 356040.8 6683101.9, 356008 6683103.9, 355961.4 6683107.3, 355918 6683111.1, 355877.8 6683115.9, 355843.7 6683120, 355813.7 6683123.8, 355784.5 6683128.5, 355761.8 6683132.2, 355747.3 6683134.9, 355737.8 6683136.7, 355688 6683146.5, 355622.1 6683161.4, 355562.8 6683176.3, 355513.8 6683190.3, 355466.6 6683204.7, 355429.5 6683217.1, 355394.3 6683228.2, 355379.5 6683233.3, 355289.5 6683266.9, 355136.9 6683332.1, 355081.3 6683355.9, 355081.1 6683356, 355078.1 6683357.4, 354813.9 6683472.1, 354799.9 6683478.4, 354708.8 6683519.8, 354664.6 6683539.8, 354618.8 6683561.4, 354505.2 6683616.6, 354423.1 6683659.7, 354383.2 6683681.6, 354282.7 6683738.2, 354213 6683781.3, 354076.5 6683870.4, 353968.5 6683944.3, 353881.6 6684005.1, 353830.5 6684043.2, 353822.4 6684048.3, 353815.2 6684054.2, 353615 6684194.6, 353565.2 6684229.5, 353500.5 6684274.5, 353486.5 6684283.5, 353454.5 6684304.3, 353416.4 6684328.1, 353379.7 6684349.3, 353379.2 6684349.5, 353379 6684349.6, 353328.4 6684377, 353284.1 6684398.5, 353283.5 6684398.8, 353283 6684399.1, 353249.6 6684414.1, 353194.9 6684437.1, 353126.7 6684462, 353048.3 6684487.9, 353043.3 6684489.7, 353017.7 6684497.9, 352939.4 6684521.8, 352886.7 6684539.8, 352835.2 6684560, 352794.4 6684576.6, 352746.5 6684597.3, 352714.2 6684612.8, 352688 6684625.7, 352651.9 6684645.3, 352614.4 6684666.7, 352568.9 6684694.5, 352529.8 6684719.5, 352501 6684738.9, 352470.5 6684760.7, 352452.3 6684774.8, 352427.8 6684794.1, 352370.6 6684845, 352323.2 6684888.8, 352304.1 6684909.4, 352221.1 6684991.4, 352192.1 6685019.8, 352155.8 6685055.4, 352088.6 6685121.9, 352010.8 6685198.9, 351884.6 6685321.8, 351826.8 6685373.6, 351769.1 6685422.2, 351738.7 6685445.7, 351737 6685447.2, 351716.1 6685463.6, 351669.5 6685497.9, 351624.4 6685528.6, 351568.2 6685565.2, 351530.4 6685588.5, 351488.7 6685612, 351444.7 6685636.4, 351400.5 6685659.1, 351398.7 6685659.9, 351374 6685672.4, 351323.5 6685695.4, 351277.6 6685714.9, 351266 6685721.1, 351241.21984726447 6685734.764484223, 351238.73263200646 6685730.522026966, 351228.1 6685734.8, 351227 6685735.3, 351107.2 6685781.4, 351070.4 6685796.4, 351028.5 6685817.5, 350981.6 6685848.5, 350969.1 6685858.9, 350948.3 6685876.2, 350937 6685889.5, 350916.1 6685913.7, 350892.7 6685944.3, 350870.9 6685981.2, 350858.7 6686006.1, 350850.9 6686022.4, 350847.8 6686031.1, 350838.8 6686056, 350837.6 6686059.6, 350831.7 6686086, 350826.4 6686118.4, 350824.5 6686141.4, 350823.9 6686149.3, 350822.9 6686174.6, 350822.9 6686180.9, 350823.2 6686193.1, 350823.7 6686206.4, 350824.3 6686219.6, 350824.7 6686232.3, 350825.6 6686245.8, 350828.3 6686287.6, 350830.9 6686324, 350833.9 6686361.5, 350834.7 6686374.1, 350835.5 6686388.9, 350837.6 6686426.5, 350840.1 6686464, 350842.8 6686502.5, 350845.4 6686541, 350847.8 6686579.6, 350850.5 6686618.1, 350852.8 6686656.7, 350855.3 6686695, 350858 6686736.8, 350861.5 6686784.8, 350864.5 6686832.2, 350867 6686871.2, 350869.2 6686909.4, 350871.9 6686948.3, 350874.7 6686987.6, 350876.9 6687024.5, 350879.5 6687062.3, 350881 6687087.6, 350882.8 6687114, 350885.5 6687154.2, 350888.4 6687192.5, 350891.6 6687243.4, 350893.3 6687280, 350895.8 6687310.2, 350895.2 6687343.6, 350894.2 6687358.2, 350893.8 6687361.4, 350893.7 6687363.2, 350893.4 6687368.1, 350893.3 6687369.8, 350893.1 6687371.2, 350892.6 6687377.2, 350892.5 6687379.3, 350892.4 6687380.2, 350891.8 6687387.4, 350891.7 6687388.9, 350891.7 6687389.2, 350891.1 6687398, 350888.9 6687413.2, 350885.3 6687438, 350884.9 6687441.1, 350883.7 6687450, 350881.7 6687463.9, 350874.5 6687498.4, 350873.3 6687504, 350872.4 6687508.4, 350871.1 6687515.1, 350870.9 6687515.7, 350870.2 6687519.2, 350869.9 6687520.6, 350864.1 6687540.4, 350849.3 6687591.6, 350824.9 6687655.6, 350824.8 6687656.3, 350823.4 6687659.2, 350800.1 6687710.2, 350780.3 6687748.9, 350780 6687749.3, 350779.1 6687751.3, 350778.3 6687752.8, 350757.1 6687788.9, 350754.4 6687793, 350748.5 6687801.7, 350747.7 6687802.9, 350733.5 6687821.2, 350697.3 6687871.7, 350659.8 6687914.4, 350639.7 6687935.3, 350618.8 6687957.1, 350592.3 6687981.6, 350537.6 6688026.6, 350518.1 6688043, 350483.6 6688074.7, 350459.9 6688100.4, 350459.3 6688101, 350455.6 6688105.1, 350435.9 6688125.8, 350403.5 6688162.8, 350399.8 6688168, 350376.3 6688199.8, 350352.9 6688234.3, 350345 6688245.9, 350317 6688294.4, 350314.9 6688298.2, 350312.3 6688302.5, 350312.2 6688302.9, 350308.4 6688309.9, 350233.2 6688456.9, 350158.1 6688604, 350083 6688751, 350060.2 6688800.6, 350042.9 6688843.4, 350038.4 6688856, 350029.1 6688882.4, 350016.2 6688926.6, 350009.3 6688958.5, 350002.1 6688996.6, 350001.3 6689002.4, 349996.7 6689037.2, 349992.5 6689089.9, 349991.6 6689125.6, 349992 6689152.3, 349995.8 6689202.1, 349996.1 6689205.6, 350000.8 6689241.4, 350009.1 6689287.8, 350013.4 6689308.2, 350025 6689355.1, 350029.9 6689371.7, 350032.8 6689381.7, 350036.1 6689393, 350094.2 6689589.5, 350098.2 6689604.8, 350101.4 6689617.8, 350102 6689619.9, 350102.7 6689623.5, 350104.3 6689630.1, 350110.4 6689646.3, 350142.3 6689744.4, 350159.3 6689792.1, 350184.5 6689855, 350201.8 6689895.7, 350207.9 6689907.9, 350222.1 6689938.5, 350229.5 6689953.9, 350315.8 6690129.4, 350327.1 6690154.4, 350327.6 6690155.5, 350329.2 6690158.9, 350331.3 6690163.2, 350331.5 6690163.6, 350358.2 6690217.6, 350379.7 6690265.5, 350388.5 6690288.1, 350414.9 6690363.4, 350417 6690367.3, 350429.9 6690403.8, 350441.3 6690436.4, 350449.5 6690466, 350459.6 6690501.1, 350474.9 6690549.7, 350490.3 6690592.9, 350497.5 6690616.4, 350504.2 6690641.9, 350506.2 6690662.8, 350505.8 6690681.6, 350502.5 6690698.6, 350499.9 6690708.4, 350499.6 6690709.7, 350498.8 6690717.5, 350499.7 6690726.8, 350501.7 6690736.3, 350509.8 6690742, 350515.1 6690747.5, 350522.4 6690757.5, 350526.8 6690767.9, 350528.4 6690773.6, 350529.5 6690783.4, 350529.2 6690787.9, 350528.8 6690789.5, 350525.8 6690802.4, 350524.1 6690807.3, 350519.6 6690814.5, 350511.8 6690824.2, 350510.1 6690826.3, 350505.8 6690830.1, 350505.5 6690839.7, 350505.3 6690857.7, 350506.3 6690882.4, 350506 6690907.8, 350504.8 6690929.5, 350502.7 6690948.4, 350499.9 6690966, 350497.7 6690990.6, 350495.9 6691020.1, 350495.9 6691021.9, 350495.8 6691032.1, 350495.8 6691041, 350495.7 6691046.9, 350496.1 6691137, 350493.9 6691164.6, 350491.8 6691187.2, 350489.4 6691197, 350488 6691203.9, 350484.7 6691221.3, 350478.6 6691252.8, 350469.1 6691288.1, 350454.6 6691332.4, 350438.9 6691371.6, 350425 6691400.7, 350401.4 6691443.5, 350363.7 6691510.1, 350357.4 6691521.2, 350339.7 6691552.9, 350320.5 6691592.2, 350308 6691622.2, 350295.6 6691654.7, 350288.1 6691680.4, 350282.7 6691700.2, 350278.4 6691718.5, 350275.7 6691735.2, 350272.7 6691753.3, 350271.9 6691758.7, 350269.6 6691777.4, 350267.7 6691800, 350267.6 6691802.2, 350266.3 6691824.1, 350266.6 6691845.3, 350267.2 6691867.6, 350268.4 6691892.4, 350270.6 6691910.9, 350273.6 6691931, 350277.3 6691953.3, 350282.6 6691975.6, 350289.1 6692002.3, 350295.4 6692023, 350306.6 6692054.7, 350321.2 6692089.9, 350329.6 6692109.5, 350338.5 6692130.5, 350353.1 6692164.6, 350365.3 6692195.4, 350375.9 6692223.6, 350387.1 6692255.6, 350399.3 6692292.1, 350408 6692317.8, 350420 6692355.9, 350431.5 6692393.4, 350439.3 6692420, 350443.8 6692436.3, 350447.3 6692449.4, 350458.5 6692490.1, 350469 6692530.9, 350479.6 6692567.7, 350488.2 6692600.4, 350500.9 6692643.4, 350507.7 6692668.4, 350525.8 6692734.7, 350541.7 6692789.5, 350558.8 6692850.5, 350568 6692881.9, 350578.3 6692916.7, 350591.3 6692962.8, 350598.9 6692989.7, 350611 6693031.9, 350617.2 6693053.2, 350634.6 6693120.5, 350659.2 6693204.2, 350679.1 6693275.6, 350694.4 6693328.5, 350706.7 6693382.3, 350716.5 6693437.6, 350721.6 6693493.8, 350721.7 6693494.7, 350725.2 6693555.4, 350724.3 6693609.8, 350723.5 6693621.6, 350721.3 6693653.4, 350718.6 6693674.1, 350715.4 6693698.3, 350710.7 6693723.4, 350709.8 6693728.3, 350706.1 6693748.3, 350697.7 6693785.5, 350694.5 6693799.4, 350681.6 6693847.2, 350662 6693922.2, 350651 6693962.5, 350649.6 6693968, 350640.2 6694017.5, 350634.7 6694063.1, 350632.9 6694108.9, 350634.6 6694157.3, 350639.6 6694203.3, 350650.1 6694255.4, 350663.3 6694300.8, 350669.2 6694316.3, 350672.5 6694324.9, 350682.1 6694350.3, 350684.7 6694355.6, 350703.8 6694394.2, 350711.1 6694406.4, 350727.1 6694433, 350752 6694469, 350779.2 6694502.5, 350810.2 6694535.5, 350845.8 6694568.5, 350871.3 6694588.2, 350881.9 6694589.1, 350918 6694596.1, 350929.2 6694598.2, 350931.8 6694598.8, 350968.4 6694606.7, 350986.8 6694613.4, 351004.7 6694620, 351051.4 6694639.5, 351090.6 6694658.7, 351129.5 6694679, 351168.6 6694697.6, 351213.8 6694716.3, 351253 6694729.5, 351284.2 6694747.5, 351288 6694748.6, 351411 6694790.6, 351491 6694819.2, 351500.1 6694822.8, 351521.5 6694831.1, 351595.9 6694860, 351672.4 6694888.2, 351716.9 6694903.6, 351792.2 6694926.8, 351841.2 6694939.1, 351855.7 6694942.8, 351862.5 6694944.4, 351864 6694944.7, 351865.6 6694945.1, 351867.9 6694945.7, 351892.5 6694951.3, 351926.6 6694958, 351974.3 6694965.7, 351974.6 6694965.7, 351999.4 6694968.7, 352026.4 6694973.2, 352106.8 6694981.2, 352189.5 6694986.8, 352274.7 6694991.1, 352364.3 6694993.1, 352393.6 6694993.7, 352498.9 6694996.2, 352534.7 6694997.1, 352548.3 6694997.4, 352594.6 6694998.5, 352645 6695000.3, 352692.2 6695002.8, 352745.9 6695006.5, 352807 6695010.6, 352849.2 6695014.2, 352936 6695016.7, 352985.3 6695023.9, 353001.4 6695026.3, 353042.6 6695034, 353101.5 6695045.7, 353173 6695062.7, 353304.5 6695098.7, 353333.33387808467 6695107.3180748485, 353343.3098948428 6695110.299777791, 353367.4 6695117.5, 353417.3 6695132.9, 353486.7 6695153.5, 353534.1 6695166.5, 353582.4 6695179, 353676.7 6695205.4, 353751.9 6695224.7, 353799.9 6695236.6, 353831.1 6695243.9, 353920.8 6695269.2, 353946.8 6695274.6, 353991.6 6695285.5, 354045.7 6695292.3, 354105.4 6695298.6, 354165.7 6695303.3, 354237.6 6695305.2, 354303.8 6695305.9, 354360.1 6695303, 354386 6695301.9, 354432.7 6695298.2, 354459.2 6695295.7, 354482.7 6695293.8, 354493.7 6695292.7, 354562.3 6695283.2, 354592.5 6695278.1, 354621.2 6695273.7, 354653.9 6695268.5, 354683.3 6695263.8, 354719.7 6695256.8, 354805.4 6695242.9, 354875.3 6695234.7, 354895 6695231.5, 354946.5 6695228.1, 355012.2 6695228.9, 355073.3 6695235.5, 355090.3 6695238.2, 355105.8 6695241.6, 355121 6695243.7, 355167.5 6695252.9, 355192.3 6695258.5, 355199.8 6695261, 355213.1 6695261, 355241.7 6695257.8, 355250.9 6695256.8, 355259.8 6695254.7, 355270.5 6695250.6, 355288.1 6695241, 355304.9 6695226.1, 355322.2 6695204.8, 355337.1 6695174.9, 355345.1 6695154.8, 355361.9 6695109.6, 355362.5 6695107.9, 355368.4 6695088.4, 355375.7 6695064.4, 355382.1 6695046.1, 355387.7 6695025.2, 355388.3 6695023.6, 355399.8 6694989.5, 355410.4 6694961.7, 355422 6694927.1, 355430.7 6694906.8, 355439.5 6694881.4, 355458.6 6694836.7, 355465.3 6694823.3, 355472.7 6694805, 355478.8 6694792.4, 355489.6 6694770.7, 355506.2 6694736.1, 355518.9 6694709.4, 355532.2 6694683.6, 355548.3 6694651.6, 355566.5 6694609.5, 355578.5 6694585.7, 355583.7 6694570.6, 355591.5 6694542.7, 355597.8 6694498.6, 355598.6 6694485.8, 355596.9 6694469.5, 355594.8 6694427.8, 355593.9 6694391.3, 355593.9 6694389.7, 355593.7 6694375, 355597 6694347.2, 355599.4 6694331.7, 355603.8 6694311.8, 355608.1 6694296.4, 355614.1 6694279.9, 355624.9 6694255.4, 355638.3 6694231.9, 355656.4 6694206.6, 355657.7 6694204.9, 355663.8 6694197.1, 355664.9 6694195.7, 355674.3 6694184, 355688.2 6694170.1, 355710.8 6694149.5, 355720.9 6694142.1, 355726.9 6694137.8, 355732 6694134.7, 355742.1 6694128.7, 355743.7 6694127.9, 355755.8 6694122, 355767.3 6694114.8, 355784.6 6694107.1, 355801.2 6694100.7, 355819 6694095.3, 355828 6694093.1, 355859.8 6694086.5, 355890.3 6694080.3, 355890.8 6694080.2, 355892 6694080.1, 355910.5 6694075.9, 355918.5 6694074.4, 355927.6 6694073.2, 355952.3 6694068.5, 356005.2 6694055.5, 356011 6694054, 356048.7 6694045.4, 356132.2 6694026.4, 356179.6 6694017.2, 356251.5 6694004.7, 356267.8 6694002, 356268.5 6694001.9, 356345.3 6693988, 356363.8 6693985.2, 356382.1 6693982.4, 356390.7 6693981.3, 356419.3 6693975.5, 356456.4 6693968.2, 356465 6693966.5, 356502 6693960.3, 356533 6693955, 356552.4 6693950.6, 356567.4 6693945.7, 356590.4 6693938.3, 356603.5 6693934.8, 356615.3 6693932.1, 356629.7 6693929.6, 356654.1 6693925.3, 356705.6 6693916.4, 356729.7 6693911.9, 356753.4 6693906.1, 356766.4 6693901.8, 356787.9 6693894.3, 356802.7 6693888.3, 356835.9 6693873.4, 356886.2 6693850.4, 356931.9 6693829.5, 356986.8 6693804.7, 357026.7 6693786.4, 357041.5 6693781.1, 357069.5 6693769.3, 357102.7 6693758.1, 357157.8 6693743.5, 357196.1 6693735.7, 357210.4 6693733.2, 357345 6693714.7, 357492.6 6693697.5, 357544.2 6693689.5, 357580.5 6693683.4, 357625.2 6693675.7, 357679.4 6693666.2, 357766.9 6693651.9, 357846.1 6693638.3, 357857.6 6693634.6, 357865.8 6693633.3, 358001.7 6693610.4, 358030.8 6693605, 358060.2 6693598.7, 358093.3 6693591, 358122.5 6693581.7, 358162.1 6693565.1, 358223.1 6693536.1, 358292.3 6693502.1, 358308.8 6693494, 358375.4 6693459.9, 358384.8 6693455.9, 358418.2 6693437.5, 358454.8 6693423.5, 358467.7 6693419.9, 358486.2 6693415.8, 358494.6 6693414.1, 358522.3 6693411.2, 358524.6 6693411, 358528 6693410.5, 358531.2 6693410.3, 358550.4 6693409.3, 358573.2 6693408.3, 358589.3 6693407.5, 358597.6 6693406.9, 358616.3 6693405.5, 358636.2 6693403.5, 358658.1 6693399.8, 358664.2 6693398.6, 358669.5 6693397, 358681.2 6693393.5, 358689.5 6693391.1, 358711.4 6693384.4, 358729.2 6693376.6, 358743.5 6693368.5, 358754.7 6693362, 358768.7 6693352.9, 358784.4 6693339.9, 358837.4 6693296.9, 358899.1 6693253.6, 358909.7 6693251.9, 358918.3 6693245.2, 358919.4 6693244.3, 358964.5 6693207.3, 359038.7 6693152, 359098.2 6693105.6, 359137 6693075.3, 359219.6 6693010.7, 359232.1 6693000.9, 359233.4 6692999.8, 359234.4 6692999, 359240.6 6692994.4, 359346.4 6692911.4, 359386.6 6692880.2, 359402 6692868.2, 359488.1 6692799.6, 359540.4 6692760.2, 359552.9 6692751.1, 359634 6692693.2, 359713 6692641, 359738.4 6692624.2, 359743.5 6692620.8, 359749.8 6692616.6, 359750.5 6692616.2, 359756.2 6692612.5, 359762.3 6692608.4, 359765.6 6692606.3, 359767.6 6692605.1, 359858.5 6692545.3, 359913.8 6692508.7, 359983.7 6692459.7, 360035 6692421.9, 360109.1 6692364.1, 360128.9 6692347.5, 360144.3 6692334.8, 360145.8 6692333.6, 360149.9 6692330, 360152.6 6692327.9, 360156.7 6692324.4, 360181.9 6692304, 360198.1 6692290.6, 360205.6 6692284.4, 360249.1 6692248.5, 360284.7 6692217.8, 360326.2 6692182.2, 360369.2 6692146, 360410.3 6692111.1, 360446.9 6692080, 360484.9 6692047.2, 360516.6 6692019.9, 360549.8 6691992.3, 360588.9 6691958.9, 360626.5 6691926.7, 360667.1 6691892.2, 360717.9 6691849.1, 360779.4 6691796.6, 360786.5 6691787.7, 360811 6691767, 360867.2 6691719.8, 360878.6 6691710.3, 360895.3 6691696.2, 360908 6691685.5, 360929.8 6691666.8, 360931.4 6691665.4, 360942.2 6691656.2, 360958.2 6691642.6, 361011.9 6691597.1, 361085.6 6691537.8, 361123 6691507.8, 361175.5 6691461.9, 361186.8 6691451.6, 361204.5 6691435.1, 361225.5 6691414.7, 361308.3 6691334.2, 361366.1 6691277.6, 361421.3 6691224.1, 361432.8 6691213, 361550.4 6691100.7, 361558.3 6691093.1, 361612.2 6691041.5, 361621.2 6691032.8, 361622.5 6691031.4, 361623.7 6691030.3, 361640.6 6691016.7, 361657.7 6691001.8, 361686.6 6690972.9, 361784.6 6690881.1, 361797.6 6690866.9, 361808.5 6690856.5, 361819.3 6690846.2, 361830.1 6690835.9, 361841 6690825.5, 361851.6 6690815.3, 361862.1 6690805.2, 361872.3 6690795.4, 361882.3 6690786, 361891.6 6690777.1, 361902.1 6690766.8, 361911.9 6690756.8, 361921 6690746, 361929.5 6690735.5, 361937.8 6690725.5, 361948.5 6690709.4, 361956 6690697.2, 361962.6 6690684.9, 361968.2 6690672.2, 361973.1 6690659.1, 361977.1 6690645.7, 361980 6690632, 361982.1 6690618.1, 361983.3 6690603.8, 361983.6 6690589.3, 361983.1 6690574.6, 361983.1 6690560.1, 361983.9 6690546, 361985 6690537.5, 361985.9 6690532.1, 361989 6690518.4, 361993.9 6690504.9, 362000.2 6690491.6, 362008.2 6690478.8, 362017.8 6690466.8, 362028.2 6690454.5, 362037.2 6690448.7, 362041.6068047337 6690446.251775148, 362041.6 6690446, 362041.6 6690436.1, 362041.7 6690432.8, 362041.4 6690419.2, 362040.6 6690405.6, 362039.2 6690391.6, 362037.3 6690377.4, 362034.9 6690363.2, 362031.8 6690348.9, 362028.4 6690334.5, 362024.6 6690320.1, 362020.4 6690305.5, 362015.4 6690291, 362009.9 6690276.6, 362003.8 6690262.2, 361997.1 6690247.6, 361989.9 6690233.2, 361982 6690218.8, 361977.3 6690210.9, 361973.6 6690204.8, 361969.4 6690198.1, 361920.1 6690196.7, 361908.4 6690192, 361897.9 6690185, 361888.9 6690177.2, 361880.9 6690167.2, 361873.9 6690155.9, 361868.1 6690142.5, 361862.8 6690128.3, 361857.1 6690113.4, 361851.4 6690097.6, 361845.3 6690081.3, 361838.5 6690064.7, 361830.4 6690048.1, 361820.5 6690031.7, 361808.6 6690015.3, 361795.6 6689998.5, 361782.1 6689981.4, 361768.9 6689964, 361755.6 6689945.9, 361742.3 6689926.9, 361729.1 6689906.9, 361715.8 6689886.2, 361683.4 6689834.4, 361615.2 6689727.9, 361527.3 6689595.5, 361446.1 6689482.8, 361370.2 6689376.2, 361316.2 6689298.7, 361315.8 6689298.1, 361311.5 6689292, 361309.6 6689289.3, 361303.6 6689280.6, 361300.8 6689276.6, 361298.8 6689273.8, 361298.5 6689273.4, 361222.9 6689168.4, 361217.8 6689161.4, 361211.4 6689152.6, 361206.6 6689145.9, 361203.1 6689140.7, 361175.6 6689100.4, 361121.4 6689026.3, 361074.7 6688968.5, 361031.7 6688931.2, 361021.8 6688922.7, 360961.5 6688883.6, 360891.8 6688845.2, 360845.2 6688807.5, 360835.4 6688799.7, 360834.8 6688799.1, 360798.6 6688760.5, 360792.9 6688754.4, 360780.1 6688737.9, 360779 6688736.6, 360769.2 6688724, 360765.8 6688719.3, 360749.5 6688687.3, 360730.4 6688649.9, 360706.2 6688586.5, 360693.3 6688540.7, 360689.3 6688521.3, 360687.8 6688507.5, 360687 6688495, 360685.4 6688466.9, 360684.5 6688448, 360684.9 6688442.9, 360685.2 6688438.8, 360689 6688398.3, 360690.1 6688384.9, 360696.6 6688352.2, 360707.1 6688313.4, 360712.3 6688293.2, 360722.9 6688246.1, 360730.3 6688217.5, 360739 6688179, 360746 6688144.1, 360752.1 6688109.3, 360755.5 6688086.9, 360758.4 6688064.7, 360760.9 6688036.5, 360763.6 6687991.6, 360763.9 6687970.5, 360762.2 6687913, 360757.5 6687849.9, 360751.5 6687787.2, 360750.5 6687778.9, 360745.4 6687725.1, 360743.3 6687702.7, 360736.7 6687641.2, 360730 6687583.8, 360724 6687540, 360714 6687478.4, 360705.1 6687431.4, 360690.1 6687366.3, 360689.7 6687364.7, 360684.5 6687344, 360664.5 6687270, 360642.2 6687200.1, 360611.5 6687114.8, 360586.5 6687053.6, 360557 6686987.7, 360532.1 6686936.6, 360510.4 6686895.4, 360498.9 6686874, 360483.5 6686846.8, 360461.9 6686809.1, 360439.3 6686771.8, 360415.9 6686732, 360393.6 6686699.5, 360351.8 6686642.8, 360320.2 6686602.7, 360318.1 6686600.1, 360306.7 6686585.7, 360287.5 6686562.3, 360284.7 6686558.8, 360276.2 6686548.6, 360258.1 6686525.6, 360250 6686515.5, 360205 6686459.8, 360183.1 6686432.6, 360176.4 6686424.1, 360172.3 6686420.7, 360168.6 6686416.7, 360163.8 6686409.9, 360159.6 6686403.6, 360156.9 6686400.8, 360154.2 6686397.1, 360142.4 6686385.5, 360116.8 6686356.4, 360084.4 6686316.7, 360072.7 6686302.4, 360014.6 6686232, 359977.2 6686186.2, 359974.6 6686183.1, 359959.7 6686164.6, 359954.7 6686158.5, 359936.3 6686135.8, 359934.3 6686133.3, 359926.8 6686124.7, 359919.9 6686116.8, 359915.7 6686111.8, 359907.7 6686102.6, 359891.5 6686083.7, 359889.4 6686081.3, 359886.9 6686078.5, 359869.9 6686058.9, 359863.9 6686052, 359850.1 6686037.1, 359848.5 6686035.3, 359844.7 6686031.1, 359838.6 6686024.7, 359819.8 6686005.1, 359790.6 6685974, 359753.7 6685938, 359740.4 6685925.3, 359720.4 6685906.2, 359715.6 6685901.8, 359709.4 6685896.1, 359690.5 6685878.5, 359661 6685852.3, 359620.9 6685816.6, 359569.8 6685771.5, 359545.3 6685749.6, 359524.5 6685730.9, 359496.1 6685705.2, 359478 6685688.7, 359451.2 6685663.5, 359420.5 6685633.2, 359390.3 6685601.7, 359370 6685580.2, 359355.9 6685565.3, 359346 6685554.6, 359337.8 6685544.5, 359333.9 6685539.6, 359325 6685528.7, 359295.5 6685492.5, 359267.3 6685454.7, 359265.4 6685452.1, 359233.3 6685408.2, 359198.9 6685358.1, 359170 6685316.1, 359153.6 6685292, 359130.9 6685260.1, 359115.1 6685237.7, 359076.4 6685185, 359058.3 6685161.9, 359025.7 6685122.1, 358992.6 6685085.7, 358974 6685066.9, 358962 6685053.9, 358960.7 6685052.7, 358916.3 6685009.5, 358879.3 6684977.9, 358846.7 6684950.7, 358815 6684926.1, 358787.2 6684906.4, 358766 6684891.2, 358763.5 6684889.3, 358758.2 6684886.3, 358749.4 6684880.1, 358736.7 6684871.5, 358726.6 6684864.6, 358692.8 6684843.4, 358662.9 6684823.7, 358659.9 6684821.7, 358628.4 6684801.9, 358598.9 6684784.7, 358568.5 6684765.8, 358539.6 6684750.7, 358523 6684741.3, 358490.3 6684722.6, 358450.9 6684699.8, 358431.6 6684688.4, 358371 6684649.1, 358361 6684642.4, 358332.3 6684622.6, 358327.3 6684619.1, 358272.7 6684581.5, 358254.4 6684566.7, 358240.3 6684556.4, 358235 6684552.4, 358233.9 6684551.5, 358231.7 6684549.9, 358228.3 6684547.5, 358223.2 6684543.9, 358211.6 6684535, 358168.3 6684500.8, 358139.2 6684475.9, 358110.2 6684449.9, 358060.3 6684402.8, 358057.6 6684400.3, 358042.3 6684384.9, 358021.1 6684363.8, 357976.8 6684315.7, 357948.4 6684284.5, 357917.4 6684248, 357870.7 6684188.7, 357853.7 6684165.9, 357840.8 6684147.8, 357827.9 6684130.2, 357800.5 6684089.6, 357757.6 6684028.7, 357737.7 6684001.1, 357708 6683954.6, 357690.6 6683932.5, 357676 6683910.1, 357671.5 6683903.1, 357642.3 6683862.2, 357626.8 6683840.6, 357563 6683760.1, 357562 6683758.9, 357555.9 6683751.3, 357498.7 6683687.7, 357498.3 6683687.2, 357465.8 6683653.1, 357426.8 6683614.9, 357394.4 6683584.2, 357364.9 6683557.6, 357327.3 6683525.6, 357279.6 6683487, 357277.1 6683485.2, 357222.9 6683444.4, 357215.4 6683438.9, 357175.9 6683412, 357122.5 6683377.9, 357096.1 6683361.7, 357047.1 6683333.2, 356995.6 6683306, 356935.1 6683276, 356872.8 6683248.2, 356816.2 6683224.5, 356756.8 6683203, 356706 6683185.5, 356634.6 6683164.6, 356607.7 6683158.3, 356596.2 6683155.4, 356582.2 6683151.9, 356567.3 6683148.2, 356511.3 6683136.3, 356461.5 6683126.9, 356408.4 6683118.8, 356389.5 6683116.3))
 """)
         return GeoDataFrameLib.read_csv(_sio)
 
     @staticmethod
+    def psmv():
+        _sio = StringIO("""geometry
+POLYGON ((355953.13724598865 6690121.022695063, 355991.1256333038 6690062.449445751, 355995.75711670384 6690055.308554656, 355995.7600164053 6690055.304159484, 355996.28986012575 6690054.506037854, 356019.7988701737 6690019.075525806, 356022.0712293572 6690015.65089435, 356022.0748289555 6690015.645500298, 356022.11022520554 6690015.592158997, 356005.985362746 6689995.958908279, 356002.6832348582 6689991.938297648, 355962.89210702555 6689942.005637332, 355962.894106764 6689942.002740554, 355962.897706324 6689941.99744642, 355984.89499625727 6689909.888801831, 355985.29254512186 6689909.3092456395, 356012.4964337797 6689862.034169074, 356012.4921380284 6689862.032368538, 356012.4830474187 6689862.027668118, 356007.94509280287 6689859.778880569, 356002.49607080274 6689857.0787351625, 356002.504371832 6689857.062052253, 356046.2009743332 6689769.714360653, 356046.7752141979 6689769.938345243, 356055.5130873548 6689774.446056351, 356055.5128968025 6689774.425772427, 356055.511193729 6689774.217137876, 356057.4397012718 6689775.212428277, 356057.6953370728 6689775.344540122, 356057.6994330783 6689775.346140717, 356058.34251309576 6689775.581048133, 356060.4513796609 6689776.352099802, 356063.600528829 6689769.457335752, 356063.6752366606 6689769.310287133, 356067.8813765881 6689761.033608357, 356074.59787897783 6689747.816915635, 356074.6421836203 6689747.729705418, 356074.33539691987 6689747.579384667, 356068.94060576195 6689744.937018979, 356068.89495240117 6689744.914615918, 356069.1851697178 6689744.371981219, 356073.90165051847 6689735.5544673735, 356074.98401494115 6689733.530975475, 356076.4493402314 6689730.271743638, 356082.58920300467 6689716.615437525, 356082.62981205876 6689716.5250281645, 356077.9174980815 6689714.273863539, 356087.15411484987 6689695.766741474, 356087.1553150887 6689695.764144097, 356097.72068848537 6689671.982134404, 356103.5819750972 6689646.747828164, 356105.2342129853 6689647.283657878, 356105.30374726193 6689647.306171785, 356120.10596658516 6689651.421071826, 356120.1080667015 6689651.417175893, 356120.3314973611 6689650.961441398, 356120.33469742077 6689650.955747401, 356133.8810361542 6689627.9538819995, 356136.75696858263 6689629.64754931, 356136.97754332947 6689629.75556424, 356136.9869337415 6689629.760164871, 356136.9894339425 6689629.755369838, 356137.0994492473 6689629.5304994285, 356137.10545008944 6689629.518211971, 356138.1128891933 6689627.461312558, 356156.81139568595 6689590.1015497865, 356090.89526863064 6689551.372629867, 356096.76962981635 6689537.30433357, 356104.1729489059 6689519.574756076, 356115.9346736425 6689491.407594926, 356152.6563903446 6689402.55304465, 356154.1037400987 6689399.050999388, 356154.868172348 6689397.212914834, 356156.3492222055 6689393.651932012, 356156.34452755324 6689393.648432655, 356156.2811993762 6689393.601840799, 356155.8885450072 6689393.312291839, 356150.5736251839 6689391.253299587, 356148.65179828776 6689390.508813091, 356088.2305832188 6689365.588211044, 356055.0987467865 6689346.053511086, 356051.3025082173 6689343.794773176, 356051.0458820438 6689343.643676103, 356050.7273219714 6689343.456079762, 356033.33460281853 6689330.54720554, 355997.5291990086 6689305.996878781, 355884.3568540695 6689228.501521939, 355848.1188011855 6689203.741860638, 355833.66265734896 6689193.864612579, 355833.0774073696 6689193.464763239, 355823.74167659937 6689187.086071666, 355793.290599759 6689166.280408039, 355683.6851686518 6689090.930761163, 355636.65132815146 6689065.327617719, 355616.41543021175 6689054.731690446, 355616.2991275425 6689054.503718975, 355608.8150849961 6689049.298639054, 355608.80989065464 6689049.295339303, 355584.2258060896 6689033.807419972, 355542.1869925586 6689007.321668036, 355541.7247948669 6689007.030488332, 355539.78706092876 6689008.0766648445, 355537.25645306625 6689006.6090749, 355537.2522559076 6689006.610172102, 355423.00897567946 6689032.381399032, 355420.3544187758 6689032.980003403, 355343.3786302797 6689013.803976844, 355314.41056831443 6688998.93084721, 355314.40697205457 6688998.928947073, 355247.7142494402 6688962.841824844, 355247.71065318043 6688962.839924705, 355210.8879659003 6688939.900822326, 355204.5314136748 6688934.290980047, 355198.5491112956 6688929.011346115, 355152.5158863203 6688899.736768604, 355134.0119835535 6688890.9581764545, 355114.6184520325 6688881.176076219, 355070.4606209468 6688858.902869763, 355048.0228260048 6688847.58519552, 355038.2485613102 6688842.284635904, 355028.4784307177 6688837.556021644, 355018.7058598738 6688832.4841801, 355018.7025632895 6688832.482479939, 355009.3928189595 6688827.637569818, 355000.6605053792 6688823.246562634, 355000.65610989806 6688823.244362369, 354991.8020521226 6688818.508274596, 354984.0207884285 6688814.751298184, 354983.6413754219 6688814.568070106, 354976.75112047064 6688811.421016211, 354976.7465250999 6688811.418915774, 354976.4882902891 6688811.290299782, 354969.7344257684 6688807.927280868, 354961.8027673912 6688803.985182945, 354959.6556384986 6688802.989591037, 354957.4357831941 6688801.960192694, 354955.90353433567 6688801.245858818, 354955.02242631116 6688800.835081833, 354951.5808150143 6688799.220489185, 354949.506018216 6688798.247112769, 354946.6526068306 6688796.916863421, 354945.70316796476 6688796.474280417, 354942.2708426019 6688794.874280358, 354942.26584768883 6688794.871879981, 354936.9347171086 6688792.01121363, 354936.1714145495 6688791.601589836, 354935.0598519163 6688791.057113658, 354934.553469962 6688790.809278786, 354933.4127372281 6688790.250400696, 354933.4091396399 6688790.25139825, 354929.7824740037 6688791.253032369, 354913.0623970145 6688795.8709636, 354892.40556223143 6688801.57621754, 354892.40106536075 6688801.577214675, 354847.83540585096 6688811.213542309, 354846.1366433227 6688811.471056014, 354846.07298967964 6688811.480719048, 354807.9542569724 6688817.25938628, 354805.9532146112 6688817.562724379, 354805.52842401894 6688817.62717768, 354793.4098505944 6688817.7261281395, 354789.61636398773 6688817.757159576, 354773.22753523407 6688815.601446227, 354729.3837709283 6688798.107951934, 354720.2505360865 6688794.463861299, 354719.24382444494 6688794.061819328, 354719.2498283393 6688794.042937161, 354721.25272341433 6688787.749181466, 354721.24403187144 6688787.745880109, 354708.5064599406 6688783.045075638, 354708.47721989715 6688782.965425771, 354707.92116184725 6688781.447082, 354707.9197646155 6688781.443484232, 354705.3775255957 6688775.5020576455, 354705.23648971657 6688775.172455879, 354697.2994944921 6688772.193783992, 354694.7863342977 6688771.250281518, 354673.730745119 6688763.411656471, 354659.12010875036 6688757.972079754, 354607.19234983117 6688738.638831105, 354593.38773314375 6688733.499184632, 354591.55977480765 6688733.972066406, 354584.7053307435 6688735.745298257, 354584.36180365516 6688735.748137985, 354563.39597909705 6688728.053037063, 354563.0035586203 6688727.908971557, 354558.28776917275 6688725.199864944, 354558.2539054499 6688725.17976541, 354558.19057348405 6688725.141766613, 354556.21669390355 6688723.957504003, 354544.3941872231 6688719.7056598095, 354544.3899914043 6688719.70385932, 354544.2754823749 6688719.704805885, 354524.9232934976 6688712.612065528, 354474.004327562 6688693.949837616, 354474.0003313959 6688693.948436898, 354392.92014754575 6688662.899115741, 354392.91265693004 6688662.8917182, 354392.8048916831 6688662.785853127, 354392.6904825856 6688662.78679972, 354391.53139943694 6688662.370698504, 354391.4753535246 6688662.350388927, 354390.50878496474 6688662.003221275, 354388.53184264543 6688663.134508303, 354372.70241115935 6688672.193091418, 354356.2096341773 6688681.631265939, 354353.0142146553 6688683.522685258, 354344.246625395 6688688.712506702, 354339.55280764506 6688691.460752295, 354335.59060294955 6688693.780676543, 354334.43271527684 6688694.458602393, 354261.7551447005 6688737.011876769, 354261.413510715 6688737.243634488, 354260.10441406595 6688745.153717488, 354254.3913872626 6688780.096294945, 354251.783826016 6688796.044764371, 354244.61045158206 6688839.919142923, 354242.22373557964 6688854.516693421, 354242.0610550558 6688855.190780527, 354242.0022898072 6688855.434359067, 354242.01877039723 6688855.447955802, 354242.0260618129 6688855.453954371, 354242.1543108457 6688855.559529159, 354358.9922710264 6688951.788519611, 354545.1834786871 6689033.127693225, 354726.0821138283 6689112.154842791, 354716.86998442875 6689133.638369244, 354716.88813985174 6689133.703825379, 354742.4663373369 6689225.702503903, 354743.00250127964 6689263.782579436, 354743.0127596541 6689264.507805766, 354743.0096582687 6689264.516197647, 354740.7272248794 6689270.722798302, 354740.441895666 6689271.498748279, 354740.4368934056 6689271.512335141, 354663.67480631097 6689320.4517083615, 354628.9555880234 6689342.4233192885, 354627.57018952793 6689343.3000829285, 354600.79275573633 6689358.055300244, 354600.78705884865 6689358.0583951585, 354649.9853156427 6689368.303454132, 354681.86545568635 6689374.911446362, 354779.344402945 6689493.291383237, 354780.9385118068 6689492.247947974, 354786.5208087882 6689488.882297588, 354791.85852329346 6689489.600379052, 354792.13668433955 6689489.63777712, 354799.1272165261 6689490.49650626, 354799.3562348153 6689490.494613051, 354945.0492182174 6689521.977479444, 354945.35294572264 6689522.0435663285, 354947.97943026596 6689521.220329543, 354948.0938394981 6689521.219382871, 354956.65900109056 6689518.630782313, 354996.5195014726 6689465.141739691, 354999.5774488811 6689461.038316127, 355001.3424326292 6689461.493464186, 355003.0189971275 6689461.92628942, 355007.8344977712 6689463.145629769, 355007.8375949802 6689463.146330634, 355011.1630408685 6689463.805632857, 355017.2303265431 6689463.7560599055, 355017.232423492 6689463.759058476, 355082.66546648956 6689555.608996896, 355119.96092603303 6689595.477349134, 355119.9658197001 6689595.482647159, 355119.9702139478 6689595.487545273, 355099.7531367539 6689614.191751013, 355099.74763880007 6689614.196844421, 355099.7450397714 6689614.199241322, 355112.5729179315 6689626.385920353, 355119.9368351429 6689633.382526283, 355125.8390640913 6689638.971282929, 355126.5637713295 6689639.657468894, 355159.9689207045 6689671.288401958, 355159.97291586845 6689671.292000928, 355174.2608777798 6689682.508823414, 355190.46953606186 6689690.61910353, 355206.51604209165 6689693.4633055935, 355206.5206378733 6689693.464506744, 355206.7331366991 6689695.058234246, 355207.61838215607 6689701.698249203, 355207.62442305987 6689701.816457777, 355209.9203796513 6689745.183053925, 355212.77956293477 6689800.798551418, 355214.86822945526 6689804.2159875855, 355217.6304811209 6689806.061485546, 355217.74605358904 6689806.138677108, 355221.6380674128 6689806.1062900815, 355221.97671728925 6689806.063379776, 355222.3314547998 6689806.019477647, 355225.5267936207 6689805.617065524, 355232.9574791674 6689804.297029285, 355233.37161302404 6689804.158030192, 355244.14618840703 6689800.542058598, 355258.1089256575 6689799.970425003, 355269.8756611278 6689796.8972760765, 355290.4015512362 6689786.99788737, 355295.0773415491 6689784.784897274, 355295.1233533151 6689784.897228889, 355295.1966128673 6689785.076020065, 355295.5446453817 6689785.925902658, 355297.0052651077 6689789.229141215, 355297.4110205679 6689790.146696393, 355297.877877469 6689791.1728930585, 355300.43280138815 6689795.617324726, 355301.01276857004 6689796.6426739935, 355303.91057337873 6689800.969356914, 355304.49099263165 6689801.880497398, 355305.61240999924 6689803.599442607, 355307.2681258114 6689806.1370807905, 355307.37636331376 6689806.303198124, 355307.38884483714 6689806.321789038, 355307.69471721386 6689806.722410254, 355308.0832737874 6689807.231782778, 355311.3213665108 6689811.212197841, 355311.7451737976 6689811.767749758, 355312.01569545653 6689812.122391379, 355312.49456785835 6689812.658384161, 355315.3665039378 6689815.872941346, 355315.9582320969 6689816.745118078, 355316.0617795735 6689816.897644084, 355316.97188679274 6689817.916350225, 355319.4124881737 6689820.64819401, 355320.2203796585 6689821.442931676, 355322.0862342775 6689823.531524133, 355322.11309905455 6689823.561612494, 355323.57108830684 6689825.193481606, 355324.3742377973 6689825.870111193, 355324.3782329628 6689825.873710162, 355327.9577601546 6689829.622466572, 355328.7656515738 6689830.417404074, 355328.7684479644 6689830.42040297, 355332.3456782281 6689834.166560394, 355332.4150961724 6689834.224845823, 355333.1523235356 6689834.846289118, 355336.2962282116 6689837.657592456, 355336.9577295966 6689838.249224743, 355337.09126295435 6689838.380481461, 355337.7660205705 6689839.04446219, 355341.5718261789 6689842.447797678, 355342.2402350069 6689843.011255581, 355342.3715795135 6689843.12202762, 355342.3790707918 6689843.128026276, 355342.38226700836 6689843.130725594, 355346.2996327952 6689846.6451238, 355347.7148827825 6689848.001193039, 355350.8002671572 6689850.958553145, 355351.60371613805 6689851.6358823115, 355351.6070122309 6689851.638681598, 355355.30040183075 6689855.272282024, 355355.3028986003 6689855.274981021, 355355.9938841504 6689856.067866499, 355359.6870740941 6689859.70116708, 355360.00617578725 6689860.0150634665, 355360.49496566335 6689860.4959047455, 355364.1875085375 6689864.015095934, 355364.88069125346 6689864.810380513, 355368.410934499 6689868.174820499, 355368.4165276166 6689868.180118844, 355368.57043764106 6689868.326872573, 355368.57293454825 6689868.329271807, 355369.3761319891 6689869.119410984, 355369.38072616846 6689869.124109349, 355372.8446980738 6689872.759103375, 355373.76824531663 6689873.6676035, 355373.7707421778 6689873.670102648, 355377.2317701771 6689877.1880885465, 355377.48208604765 6689877.3726563975, 355378.15322425956 6689877.867470236, 355381.8458671325 6689881.38686132, 355382.6525125282 6689882.066590041, 355386.3466494651 6689885.814299916, 355390.6178661375 6689890.129722388, 355391.6556229237 6689891.037175763, 355395.2325105338 6689894.442404667, 355395.92599288566 6689895.2380890725, 355399.6168903306 6689898.64197138, 355399.7609198928 6689898.763340796, 355400.42423475 6689899.322699624, 355403.3698153922 6689902.31386864, 355403.70009831 6689902.649352965, 355404.00301582675 6689902.956946952, 355404.81090748956 6689903.751684621, 355404.81380394025 6689903.7543838015, 355408.50315120834 6689907.270476003, 355412.4426874242 6689911.24801543, 355412.8899239563 6689911.699461056, 355412.89292014594 6689911.702559964, 355447.75409019727 6689947.133234532, 355449.01717882836 6689947.580457912, 355449.02027594834 6689947.581358616, 355450.27912056475 6689947.913971343, 355482.466907219 6689936.087961677, 355519.2198613167 6689922.507442904, 355519.6407552395 6689922.443786717, 355520.02027923753 6689922.386406552, 355520.0233762201 6689922.387607016, 355521.05380242306 6689922.721014182, 355523.1867696119 6689923.884266139, 355539.4073925535 6689932.7248655865, 355618.11102403374 6689975.620500225, 355630.3928373908 6689983.914227398, 355647.9271406827 6689995.754938324, 355647.9309365101 6689995.757438076, 355678.43116130005 6690015.997904905, 355730.1374122277 6690039.043960542, 355748.233415961 6690047.079158462, 355791.1506996402 6690066.135858302, 355791.15529598214 6690066.135860408, 355791.26510896144 6690066.134911507, 355793.8711703274 6690067.363427874, 355794.29064556846 6690067.561262632, 355794.3687671722 6690067.596570327, 355798.4210855724 6690059.208108546, 355801.80379120953 6690052.88309652, 355801.8768670317 6690052.808889123, 355801.91705425957 6690052.766940952, 355826.99410669087 6690067.331037997, 355827.2127834421 6690067.438152935, 355827.22397200594 6690067.44365368, 355827.75542942365 6690067.703989975, 355827.91366788157 6690067.781500787, 355828.60326387367 6690068.119247923, 355840.67386254395 6690074.202736244, 355851.0190013822 6690079.269842946, 355872.16357248236 6690089.284559427, 355872.16616986325 6690089.285759664, 355882.5083687467 6690094.009737957, 355899.96488461696 6690100.7362820115, 355900.07949391817 6690100.735035528, 355953.0209430607 6690120.794723303, 355953.13494983065 6690121.018297514, 355953.13724598865 6690121.022695063))
+""")
+        return GeoDataFrameLib.read_csv(_sio)
+
+    @staticmethod
     def plot(oFile=None):
         nm = GeoDataFrameDemosA.nantesMetropole()
         nantes = GeoDataFrameDemosA.villeDeNantes()
         ileDeNantes = GeoDataFrameDemosA.ileDeNantes()
         intraBoulevardsNantes = GeoDataFrameDemosA.intraBoulevardsNantes()
         intraPeripheriqueNantes = GeoDataFrameDemosA.intraPeripheriqueNantes()
+        psmv = GeoDataFrameDemosA.psmv()
 
         # MAPPING
         minx, miny, maxx, maxy = nm.total_bounds
 
         fig, basemap = plt.subplots(figsize=(0.7 * 8.26, 1 * 8.26))
         nm.boundary.plot(ax=basemap, color='red')
         nantes.boundary.plot(ax=basemap, color='blue')
         ileDeNantes.boundary.plot(ax=basemap, color='green')
         intraBoulevardsNantes.boundary.plot(ax=basemap, color='orange')
         intraPeripheriqueNantes.boundary.plot(ax=basemap, color='brown')
+        psmv.boundary.plot(ax=basemap, color='magenta')
         basemap.axis('off')
         basemap.axis([minx, maxx, miny, maxy])
         if oFile is None:
             plt.show()
         else:
             plt.savefig(oFile, bbox_inches='tight')
         plt.close(fig)
```

### Comparing `t4gpd-0.6.0/t4gpd/energy/DirectSolarIrradianceLib.py` & `t4gpd-0.7.0/t4gpd/energy/DirectSolarIrradianceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/energy/Dogniaux.py` & `t4gpd-0.7.0/t4gpd/energy/Dogniaux.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/energy/Perez.py` & `t4gpd-0.7.0/t4gpd/energy/Perez.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/energy/Perraudeau.py` & `t4gpd-0.7.0/t4gpd/energy/Perraudeau.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/energy/PerrinDeBrichambaut.py` & `t4gpd-0.7.0/t4gpd/energy/PerrinDeBrichambaut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/energy/PlotDirectNormalIrradiance.py` & `t4gpd-0.7.0/t4gpd/energy/PlotDirectNormalIrradiance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py` & `t4gpd-0.7.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/graph/STBetweennessCentrality.py` & `t4gpd-0.7.0/t4gpd/graph/STBetweennessCentrality.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/graph/STClosenessCentrality.py` & `t4gpd-0.7.0/t4gpd/graph/STClosenessCentrality.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/graph/STRoadNeighborhood.py` & `t4gpd-0.7.0/t4gpd/graph/STRoadNeighborhood.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/graph/STShortestPath.py` & `t4gpd-0.7.0/t4gpd/graph/STShortestPath.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/graph/STToRoadsSections.py` & `t4gpd-0.7.0/t4gpd/graph/STToRoadsSections.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/graph/STToRoadsSectionsNodes.py` & `t4gpd-0.7.0/t4gpd/graph/STToRoadsSectionsNodes.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/AbstractReader.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 22 juin 2022
+Created on 16 juin 2020
 
 @author: tleduc
 
-Copyright 2020-2022 Thomas Leduc
+Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,23 +16,18 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from _io import StringIO
+from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
-from t4gpd.commons.GeoProcess import GeoProcess
 
-
-class AbstractReader(GeoProcess):
+class MABR(AbstractGeoprocess):
     '''
     classdocs
     '''
 
     @staticmethod
-    def opener(inputFile):
-        if isinstance(inputFile, StringIO):
-            return inputFile
-        else:
-            return open(inputFile, 'r')
+    def runWithArgs(row):
+        return { 'geometry': row.geometry.minimum_rotated_rectangle }
```

### Comparing `t4gpd-0.6.0/t4gpd/io/CSVInertialSensorReader.py` & `t4gpd-0.7.0/t4gpd/io/CSVInertialSensorReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/CSVReader.py` & `t4gpd-0.7.0/t4gpd/io/CSVReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/CSVWKTReader.py` & `t4gpd-0.7.0/t4gpd/io/CSVWKTReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/CSVWKTWriter.py` & `t4gpd-0.7.0/t4gpd/io/CSVWKTWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/CirReader.py` & `t4gpd-0.7.0/t4gpd/io/CirReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/CirValReader.py` & `t4gpd-0.7.0/t4gpd/io/CirValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/CirWriter.py` & `t4gpd-0.7.0/t4gpd/io/CirWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/CityGMLReader.py` & `t4gpd-0.7.0/t4gpd/io/CityGMLReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/GeoWriter.py` & `t4gpd-0.7.0/t4gpd/io/GeoWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/GpkgLoader.py` & `t4gpd-0.7.0/t4gpd/io/GpkgLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/GpkgWriter.py` & `t4gpd-0.7.0/t4gpd/io/GpkgWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/MshReader.py` & `t4gpd-0.7.0/t4gpd/io/MshReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/ObjReader.py` & `t4gpd-0.7.0/t4gpd/io/ObjReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/ObjWriter.py` & `t4gpd-0.7.0/t4gpd/io/ObjWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/Reloading.py` & `t4gpd-0.7.0/t4gpd/io/Reloading.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/STLoadAndClip.py` & `t4gpd-0.7.0/t4gpd/io/STLoadAndClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/SVGWriter.py` & `t4gpd-0.7.0/t4gpd/io/SVGWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/SalomeWriter.py` & `t4gpd-0.7.0/t4gpd/io/SalomeWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/SalomeWriterAndExtruder.py` & `t4gpd-0.7.0/t4gpd/io/SalomeWriterAndExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/VTUWriter.py` & `t4gpd-0.7.0/t4gpd/io/VTUWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/ValReader.py` & `t4gpd-0.7.0/t4gpd/io/ValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/ZipLoader.py` & `t4gpd-0.7.0/t4gpd/io/ZipLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/io/ZipWriter.py` & `t4gpd-0.7.0/t4gpd/io/ZipWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/isovist/STIsovistField2D.py` & `t4gpd-0.7.0/t4gpd/isovist/STIsovistField2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/FrequencyHistogram.py` & `t4gpd-0.7.0/t4gpd/misc/FrequencyHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/OptimalNumberOfClusters.py` & `t4gpd-0.7.0/t4gpd/misc/OptimalNumberOfClusters.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/PlotAMatrixOfDiagrams.py` & `t4gpd-0.7.0/t4gpd/misc/PlotAMatrixOfDiagrams.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/PopulationPyramid.py` & `t4gpd-0.7.0/t4gpd/misc/PopulationPyramid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/RoseMappingTool.py` & `t4gpd-0.7.0/t4gpd/misc/RoseMappingTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/STCompass.py` & `t4gpd-0.7.0/t4gpd/misc/STCompass.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/STDendrogram.py` & `t4gpd-0.7.0/t4gpd/misc/STDendrogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/STKMeans.py` & `t4gpd-0.7.0/t4gpd/misc/STKMeans.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/StreetOrientationHistogram.py` & `t4gpd-0.7.0/t4gpd/misc/StreetOrientationHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/TimelineTool.py` & `t4gpd-0.7.0/t4gpd/misc/TimelineTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/misc/WindRose.py` & `t4gpd-0.7.0/t4gpd/misc/WindRose.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/GmshTriangulator.py` & `t4gpd-0.7.0/t4gpd/morph/GmshTriangulator.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STBBox.py` & `t4gpd-0.7.0/t4gpd/morph/STBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STClip.py` & `t4gpd-0.7.0/t4gpd/morph/STClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STCoolscapesTessellation.py` & `t4gpd-0.7.0/t4gpd/morph/STCoolscapesTessellation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STCrossroadsGeneration.py` & `t4gpd-0.7.0/t4gpd/morph/STCrossroadsGeneration.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,31 +19,34 @@
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas.geodataframe import GeoDataFrame
 from numpy import sqrt
 from t4gpd.commons.GeoProcess import GeoProcess
-
+from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 from t4gpd.commons.crossroads_generation.SequenceRadii import SequenceRadii
 from t4gpd.commons.crossroads_generation.SequencesGeneration import SequencesGeneration
 
 
 class STCrossroadsGeneration(GeoProcess):
     '''
     classdocs
     '''
 
     def __init__(self, nbranchs, length, width, mirror=False, withBranchs=True, withSectors=True,
-                 crs='EPSG:2154', magnitude=2.5):
+                 crs='EPSG:2154', magnitude=2.5, varLength=None):
         '''
         Constructor
         '''
+        if not((varLength is None) or (0 <= varLength <= 1.0)):
+            raise IllegalArgumentTypeException(varLength, "Float value between 0.0 and 1.0 or None")
+
         self.nbranchs = nbranchs
-        self.sequenceRadii = SequenceRadii(nbranchs, width, length)
+        self.sequenceRadii = SequenceRadii(nbranchs, width, length, varLength)
         self.dictOfSequences = SequencesGeneration(nbranchs, mirror, withBranchs, withSectors).run()
         self.width = width
         self.offset = magnitude * length
 
         nseq = len(self.dictOfSequences)
         sqrt_nseq = int(sqrt(nseq))
         if (abs(nseq - sqrt_nseq * sqrt_nseq) < abs(nseq - (sqrt_nseq + 1) * (sqrt_nseq + 1))):
@@ -54,15 +57,15 @@
         self.crs = crs
 
     def run(self):
         rows = list()
         for i, (gid, seq) in enumerate(self.dictOfSequences.items()):
             xoffset = self.offset * (i % self.ncols)
             yoffset = -self.offset * int(i / self.ncols)
-            geom = seq.asPolygon(self.sequenceRadii, self.width, [xoffset, yoffset])
+            geom = seq.asPolygon(self.sequenceRadii, [xoffset, yoffset])
             row = dict({'gid': gid,
                         'vpoint_x': xoffset,
                         'vpoint_y': yoffset,
                         'model': seq.getMinModel(),
                         'sequence': str(seq),
                         'geometry': geom})
             rows.append(row)
```

### Comparing `t4gpd-0.6.0/t4gpd/morph/STDilationErosion.py` & `t4gpd-0.7.0/t4gpd/morph/STDilationErosion.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STExtractOpenSpaces.py` & `t4gpd-0.7.0/t4gpd/morph/STExtractOpenSpaces.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STFacadesAnalysis.py` & `t4gpd-0.7.0/t4gpd/morph/STFacadesAnalysis.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STGradientOfDistancesToBuildings.py` & `t4gpd-0.7.0/t4gpd/morph/STGradientOfDistancesToBuildings.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STGrid.py` & `t4gpd-0.7.0/t4gpd/morph/STGrid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 11 juin 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -32,32 +32,32 @@
     '''
 
     def __init__(self, inputGdf, dx, dy=None, indoor=None, intoPoint=True, encode=True):
         '''
         Constructor
         '''
         if not isinstance(inputGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(inputGdf, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(inputGdf, "GeoDataFrame")
 
         self.inputGdf = inputGdf
         self.dx = dx
         self.dy = dy
-        if indoor in [None, True, False, 'both']:
+        if indoor in [None, True, False, "both"]:
             self.indoor = indoor
         else:
-            raise Exception('Illegal argument: indoor must be chosen in [None, True, False, "both"]!')
+            raise Exception("Illegal argument: indoor must be chosen in [None, True, False, 'both']!")
         self.intoPoint = intoPoint
         self.encode = encode
 
     def run(self):
         gridLib = GridLib(self.inputGdf, self.dx, self.dy, self.encode)
 
         if self.indoor is None:
             grid = gridLib.grid()
-        elif ('both' == self.indoor):
+        elif ("both" == self.indoor):
             grid = gridLib.indoorOutdoorGrid()
         elif self.indoor:
             grid = gridLib.indoorGrid()
         else:
             grid = gridLib.outdoorGrid()
 
         if self.intoPoint:
```

### Comparing `t4gpd-0.6.0/t4gpd/morph/STIdentifyRowOfTrees.py` & `t4gpd-0.7.0/t4gpd/morph/STIdentifyRowOfTrees.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STMakeBlocks.py` & `t4gpd-0.7.0/t4gpd/morph/STMakeBlocks.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STMultipleOverlaps.py` & `t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STMultipleOverlaps2.py` & `t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STPointsDensifier.py` & `t4gpd-0.7.0/t4gpd/morph/STPointsDensifier.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STPointsDensifier2.py` & `t4gpd-0.7.0/t4gpd/morph/STPointsDensifier2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STPolygonize.py` & `t4gpd-0.7.0/t4gpd/morph/STPolygonize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STSkeletonize.py` & `t4gpd-0.7.0/t4gpd/morph/STSkeletonize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STSkeletonizeTheVoid.py` & `t4gpd-0.7.0/t4gpd/morph/STSkeletonizeTheVoid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STSnappingPointsOnLines.py` & `t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STSnappingPointsOnLines2.py` & `t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STSpatialJoin.py` & `t4gpd-0.7.0/t4gpd/morph/STSpatialJoin.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STSquaredBBox.py` & `t4gpd-0.7.0/t4gpd/morph/STSquaredBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STVariableWidthBuffer.py` & `t4gpd-0.7.0/t4gpd/morph/STVariableWidthBuffer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/STVoronoiPartition.py` & `t4gpd-0.7.0/t4gpd/morph/STVoronoiPartition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/AngularAbscissa.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AngularAbscissa.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/AspectRatio.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AspectRatio.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/BBox.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/BBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/CircularityIndices.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CircularityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/ConvexHull.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/ConvexityIndices.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/Diameter.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/Diameter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/EllipticityIndices.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/EllipticityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/FootprintExtruder.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/FootprintExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/GridFace.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/GridFace.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/HMean.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/HMean.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/MABE.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/MABR.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RemoveHoles.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
+from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class MABR(AbstractGeoprocess):
+class RemoveHoles(AbstractGeoprocess):
     '''
     classdocs
     '''
 
     @staticmethod
     def runWithArgs(row):
-        return { 'geometry': row.geometry.minimum_rotated_rectangle }
+        geom = row.geometry
+        return { 'geometry': GeomLib.removeHoles(geom) }
```

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/MABR2.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/MBC.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MBC.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/MPBR.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MPBR.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/RectangularityIndices.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectangularityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/RectifyByFFT.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFFT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/RectifyByFWT.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFWT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/RemoveHoles.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/Rotation2D.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 16 juin 2020
+Created on 11 sept. 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,20 +16,27 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from t4gpd.commons.GeomLib import GeomLib
+from shapely.affinity import rotate
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class RemoveHoles(AbstractGeoprocess):
+class Rotation2D(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    @staticmethod
-    def runWithArgs(row):
-        geom = row.geometry
-        return { 'geometry': GeomLib.removeHoles(geom) }
+    def __init__(self, angle, origin='center', use_radians=False):
+        '''
+        Constructor
+        '''
+        self.angle = angle
+        self.origin = origin
+        self.use_radians = use_radians
+
+    def runWithArgs(self, row):
+        return { 'geometry': rotate(
+            row.geometry, self.angle, origin='center', use_radians=False) }
```

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/RepresentativePoint.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RepresentativePoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/Rotation2D.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/WMean.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 11 sept. 2020
+Created on 28 sept. 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,27 +16,40 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from shapely.affinity import rotate
+from geopandas.geodataframe import GeoDataFrame
+from numpy import mean
+from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
+from t4gpd.commons.RayCasting3Lib import RayCasting3Lib
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class Rotation2D(AbstractGeoprocess):
+class WMean(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    def __init__(self, angle, origin='center', use_radians=False):
+    def __init__(self, buildingsGdf, nRays=64, maxRayLen=100.0):
         '''
         Constructor
         '''
-        self.angle = angle
-        self.origin = origin
-        self.use_radians = use_radians
+        if not isinstance(buildingsGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(buildingsGdf, 'GeoDataFrame')
+        self.buildingsGdf = buildingsGdf
+
+        self.shootingDirs = RayCasting3Lib.preparePanopticRays(nRays)
+        self.maxRayLen = maxRayLen
 
     def runWithArgs(self, row):
-        return { 'geometry': rotate(
-            row.geometry, self.angle, origin='center', use_radians=False) }
+        viewPoint = row.geometry.centroid
+
+        _, _, hitDists = RayCasting3Lib.outdoorMultipleRayCast2D(
+            self.buildingsGdf, viewPoint, self.shootingDirs, self.maxRayLen)
+
+        return {
+            # 'hit_dists': ArrayCoding.encode(hitDists),
+            'wmean': float(mean(hitDists))
+            }
```

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/STGeoProcess.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/STGeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/SkyMap2D.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/SkyViewFactor.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactor.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/StarShapedIndices.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/StarShapedIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/SurfaceFraction.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SurfaceFraction.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/Translation.py` & `t4gpd-0.7.0/t4gpd/morph/geoProcesses/Translation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/morph/geoProcesses/WMean.py` & `t4gpd-0.7.0/t4gpd/morph/STMakeGroundSurface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 28 sept. 2020
+Created on 7 juin 2023
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -17,39 +17,37 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas.geodataframe import GeoDataFrame
-from numpy import mean
+from shapely import union_all
+from shapely.geometry import box, JOIN_STYLE
+from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.RayCasting3Lib import RayCasting3Lib
-from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
+from t4gpd.commons.GeomLib import GeomLib
 
 
-class WMean(AbstractGeoprocess):
+class STMakeGroundSurface(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, buildingsGdf, nRays=64, maxRayLen=100.0):
+    def __init__(self, gdf, buffDist=10.0, holed=False):
         '''
         Constructor
         '''
-        if not isinstance(buildingsGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(buildingsGdf, 'GeoDataFrame')
-        self.buildingsGdf = buildingsGdf
-
-        self.shootingDirs = RayCasting3Lib.preparePanopticRays(nRays)
-        self.maxRayLen = maxRayLen
-
-    def runWithArgs(self, row):
-        viewPoint = row.geometry.centroid
-
-        _, _, hitDists = RayCasting3Lib.outdoorMultipleRayCast2D(
-            self.buildingsGdf, viewPoint, self.shootingDirs, self.maxRayLen)
-
-        return {
-            # 'hit_dists': ArrayCoding.encode(hitDists),
-            'wmean': float(mean(hitDists))
-            }
+        if not isinstance(gdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(gdf, "GeoDataFrame")
+        self.gdf = gdf
+        self.buffDist = buffDist
+        self.holed = holed
+
+    def run(self):
+        bbox = box(*self.gdf.total_bounds).buffer(self.buffDist, join_style=JOIN_STYLE.mitre)
+
+        if self.holed:
+            bbox = bbox.difference(union_all(self.gdf.geometry))
+
+        bbox = GeomLib.forceZCoordinateToZ0(bbox, z0=0.0)
+        return GeoDataFrame([{'geometry': bbox}], crs=self.gdf.crs)
```

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/ExtraProcessing.py` & `t4gpd-0.7.0/t4gpd/picoclim/ExtraProcessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,57 +16,50 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from datetime import timezone
-
 from geopandas import GeoDataFrame
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 from t4gpd.commons.sun.PySolarSunLib import PySolarSunLib
 
 
 class ExtraProcessing(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, dfImuMob, inplace=False, tz=timezone.utc):
+    def __init__(self, dfImuMob, inplace=False):
         '''
         Constructor
         '''
         if not isinstance(dfImuMob, GeoDataFrame):
-            raise IllegalArgumentTypeException(dfImuMob, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(dfImuMob, "GeoDataFrame")
         if inplace:
             self.dfImuMob = dfImuMob
         else:
             self.dfImuMob = dfImuMob.copy(deep=True)
         self.crs = dfImuMob.crs
 
         self.sunLib = PySolarSunLib(dfImuMob)
-        self.tz = tz
 
-        assert dfImuMob.timestamp.is_monotonic_increasing, f'dfImu.timestamp is not monotonic increasing!'
+        assert dfImuMob.timestamp.is_monotonic_increasing, f"dfImu.timestamp is not monotonic increasing!"
 
     def run(self):
-        self.dfImuMob.to_crs('epsg:4326', inplace=True)
-        self.dfImuMob['lat_cor'] = self.dfImuMob.geometry.apply(lambda geom: geom.y)
-        self.dfImuMob['lon_cor'] = self.dfImuMob.geometry.apply(lambda geom: geom.x)
+        self.dfImuMob.to_crs("epsg:4326", inplace=True)
+        self.dfImuMob["lat_cor"] = self.dfImuMob.geometry.apply(lambda geom: geom.y)
+        self.dfImuMob["lon_cor"] = self.dfImuMob.geometry.apply(lambda geom: geom.x)
         self.dfImuMob.to_crs(self.crs, inplace=True)
 
-        self.dfImuMob['epoch'] = self.dfImuMob.timestamp.apply(
+        self.dfImuMob["epoch"] = self.dfImuMob.timestamp.apply(
             lambda dt: dt.timestamp())
-            # lambda dt: int(dt.strftime('%s')))
+            # lambda dt: int(dt.strftime("%s")))
         self.dfImuMob.epoch = self.dfImuMob.epoch.astype(int)
 
-        self.dfImuMob['sun_alti'] = self.dfImuMob.timestamp.apply(
-            lambda dt: self.sunLib.getSolarAnglesInDegrees(
-                dt.to_pydatetime().replace(tzinfo=self.tz)))
-        self.dfImuMob['sun_azim'] = self.dfImuMob.sun_alti.apply(
-            lambda altiazim: altiazim[1]) 
-        self.dfImuMob['sun_alti'] = self.dfImuMob.sun_alti.apply(
-            lambda altiazim: altiazim[0]) 
+        self.dfImuMob["sun_alti"], self.dfImuMob["sun_azim"] = self.dfImuMob.apply(
+            lambda row: self.sunLib.getSolarAnglesInDegrees(row.timestamp.to_pydatetime()),
+            axis=1, result_type="expand").to_numpy().transpose()
 
         return self.dfImuMob
```

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/InertialMeasureReader.py` & `t4gpd-0.7.0/t4gpd/picoclim/UClimTrackWaypointsReader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 15 sept. 2022
+Created on 8 juin 2023
 
 @author: tleduc
 
 Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,63 +16,71 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from os.path import basename
+import warnings
 
-from dateutil.parser import parse
 from geopandas import GeoDataFrame
-from numpy.random import choice
 from pandas import read_csv
-from shapely.geometry import Point
-from t4gpd.commons.GeoProcess import GeoProcess
+from shapely.geometry import LineString, Point
+from t4gpd.commons.WarnUtils import WarnUtils
+from t4gpd.io.AbstractReader import AbstractReader
 
 
-class InertialMeasureReader(GeoProcess):
+class UClimTrackWaypointsReader(AbstractReader):
     '''
     classdocs
     '''
-    FIELD_NAMES = [
-        "timestamp", "step_count", "X", "Y", "Z", "Distance", "degree",
-        "latitude", "longitude", "GpsAccuracy", "indoor_outdoor_flag", "TagName"
-    ]
 
-    def __init__(self, inputFile, outputCrs=None):
+    def __init__(self, inputFile, icrs="epsg:4326", ocrs="epsg:2154"):
         '''
         Constructor
         '''
+        warnings.formatwarning = WarnUtils.format_Warning_alt
         self.inputFile = inputFile
-        self.outputCrs = outputCrs
+        self.icrs = icrs
+        self.ocrs = ocrs
 
-    def __extract_YYYYMMDD_from_filename(self):
-        yyyymmdd = basename(self.inputFile)[9:17]
-        year, month, day = yyyymmdd[0:4], yyyymmdd[4:6], yyyymmdd[6:8]
-        return year, month, day
+    def __getVersion(self):
+        return 1
 
-    def __getRndSubtrackId(self):
-        return "".join(choice([str(i) for i in range(10)], size=10))
+    def __postpcs(self, df):
+        df["geometry"] = df.apply(lambda row: Point((row.long, row.lat)), axis=1)
+        gdf = GeoDataFrame(df, crs=self.icrs).to_crs(self.ocrs)
+        assert gdf.ptid.is_monotonic_increasing, "ptid must be monotonic increasing!"
+
+        track_geom = LineString(gdf.geometry.apply(lambda g: g.coords[0:2][0]))
+        tracks = GeoDataFrame([{"length": track_geom.length, "geometry": track_geom}], crs=self.ocrs)
+
+        waypoints = gdf.loc[gdf.waypoint == 1 , ["ptid", "geometry"]]
+        waypoints.reset_index(drop=True, inplace=True)
+        waypoints["curv_absc"] = waypoints.geometry.apply(lambda g: track_geom.project(g, normalized=False))
+        waypoints["sect_len"] = waypoints.curv_absc.diff(periods=-1).abs()
+        waypoints.rename(columns={"ptid": "id"}, inplace=True)
+
+        return tracks, waypoints
+
+    def __readV1(self):
+        df = read_csv(UClimTrackWaypointsReader.opener(self.inputFile), sep=";")
+        return self.__postpcs(df)
 
     def run(self):
-        df = read_csv(self.inputFile, decimal=",", header=None,
-                      names=self.FIELD_NAMES, sep="\s+",
-                      skip_blank_lines=True, skiprows=2)
+        version = self.__getVersion()
+        if (1 == version):
+            warnings.warn("UClimTrackWaypointsReader (v1)")
+            return self.__readV1()
+        raise Exception("Unreachable instruction!")
+
+"""
+import matplotlib.pyplot as plt
 
-        year, month, day = self.__extract_YYYYMMDD_from_filename()
-        df.timestamp = df.timestamp.apply(lambda t: parse(f"{year}-{month}-{day}T{t}"))
+ifile = "/home/tleduc/prj/uclim/data/nantes_commerce_feydeau/nantes_commerce_feydeau_track1.csv"
+tracks, waypoints = UClimTrackWaypointsReader(ifile).run()
 
-        df["subtrack"] = self.__getRndSubtrackId()
+gdf.to_csv("/tmp/a.csv", index=False, sep=";")
+print(gdf.head(3))
 
-        df["geometry"] = df.apply(lambda row: Point(row.longitude, row.latitude), axis=1)
-        df = GeoDataFrame(df, geometry="geometry", crs="epsg:4326")
-
-        if self.outputCrs is None:
-            return df
-        return df.to_crs(self.outputCrs)
-
-'''
-inputFile = "/home/tleduc/prj/nm-ilots-frais/terrain/220711/LOG_FILE_20220711_172000.txt"
-df = InertialMeasureReader(inputFile, outputCrs="epsg:2154").run()
-print(df.head(5))
-'''
+ax=waypoints.plot(); tracks.plot(ax=ax); plt.show()
+"""
```

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/JoinByTimeDistance.py` & `t4gpd-0.7.0/t4gpd/picoclim/JoinByTimeDistance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/MeteoFranceReader.py` & `t4gpd-0.7.0/t4gpd/picoclim/MeteoFranceReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py` & `t4gpd-0.7.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/SensirionReader.py` & `t4gpd-0.7.0/t4gpd/picoclim/SensirionReader.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,68 +16,77 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from _warnings import warn
-from datetime import datetime
 import re
+import warnings
+from zoneinfo import ZoneInfo
 
 from pandas import read_csv
-from t4gpd.commons.GeoProcess import GeoProcess
+from t4gpd.commons.WarnUtils import WarnUtils
+from t4gpd.io.AbstractReader import AbstractReader
 
 
-class SensirionReader(GeoProcess):
+class SensirionReader(AbstractReader):
     '''
     classdocs
+
+    https://sensirion.com/products/catalog/SHT40/
     '''
     FIELD_NAMES = ['local_datetime', 'Tair', 'RH'] 
 
     RE1 = re.compile(r'^# EdfVersion=(\d\.\d)$')
     RE2 = re.compile(r'^# SensorFamily=(\w*).*$')
     RE3 = re.compile(r'^# SensorId=(.*)$')
 
-    def __init__(self, inputFile):
+    def __init__(self, inputFile, tzinfo="Europe/Paris"):
         '''
         Constructor
         '''
+        warnings.formatwarning = WarnUtils.format_Warning
         self.inputFile = inputFile
+        self.tzinfo = ZoneInfo(tzinfo)
 
     def __getEdfVersionAndSensorSpecs(self):
-        with open(self.inputFile, 'r') as f:
+        with SensirionReader.opener(self.inputFile) as f:
             for nline, line in enumerate(f, start=1):
                 line = line.strip()
                 if (1 == nline):
                     version = float(self.RE1.search(line).group(1))
                 elif (6 == nline):
                     sensorFamily = self.RE2.search(line).group(1)
                 elif (7 == nline):
                     sensorId = self.RE3.search(line).group(1)
                     sensorId = sensorId.replace(':', '')
                     return version, sensorFamily, sensorId
 
     def run(self):
-        # https://sensirion.com/products/catalog/SHT40/
         version, sensorFamily, sensorId = self.__getEdfVersionAndSensorSpecs()
 
         if (4.0 != version):
-            warn('EdfVersion is expected to be equal to 4.0!')
+            warnings.warn('EdfVersion is expected to be equal to 4.0!')
 
         # https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
-        df = read_csv(self.inputFile, header=None, names=self.FIELD_NAMES,
-                      parse_dates=['local_datetime'], sep='\s+',
-                      skiprows=10, usecols=range(1, 4))
+        df = read_csv(SensirionReader.opener(self.inputFile), header=None,
+                      names=self.FIELD_NAMES, parse_dates=['local_datetime'],
+                      sep='\s+', skiprows=10, usecols=range(1, 4))
         # df.Epoch_UTC = df.Epoch_UTC.apply(lambda v: datetime.fromtimestamp(v))
         df.rename(columns={'local_datetime': 'timestamp'}, inplace=True)
         df['sensorFamily'] = sensorFamily
         df['sensorId'] = sensorId
         df['station'] = f'{sensorFamily}-{sensorId}'
 
+        df.timestamp = df.timestamp.apply(lambda dt: dt.replace(tzinfo=self.tzinfo))
+        if not df.timestamp.is_monotonic_increasing:
+            msg = f"Timestamps in {self.inputFile} are not monotonically increasing"
+            warnings.warn(msg)
+
         return df
 
 '''
 inputFile = '/home/tleduc/prj/nm-ilots-frais/terrain/220711/Sensirion_MyAmbience_SHT40_Gadget_0F0E_2022-07-11T18-49-50.435746.edf'
 df = SensirionReader(inputFile).run()
 print(df.head(5))
 '''
```

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py` & `t4gpd-0.7.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 11 oct. 2022
 
 @author: tleduc
 
-Copyright 2020-2022 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -33,36 +33,46 @@
     '''
 
     def __init__(self, dfImu, tracks, waypoints):
         '''
         Constructor
         '''
         if not isinstance(dfImu, GeoDataFrame):
-            raise IllegalArgumentTypeException(dfImu, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(dfImu, "GeoDataFrame")
+        for fieldname in ["timestamp", "TagName"]:
+            if fieldname not in dfImu:
+                raise Exception(f"{fieldname} is not a relevant field name!")
+        assert dfImu.timestamp.is_monotonic_increasing, "dfImu.timestamp must be increasing!"
+        assert dfImu.timestamp.is_unique, "dfImu.timestamp must be strictly increasing!"
         self.dfImu = dfImu
 
         if not isinstance(tracks, GeoDataFrame):
-            raise IllegalArgumentTypeException(tracks, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(tracks, "GeoDataFrame")
+        if "id" not in tracks:
+            raise Exception(f"'id' is not a relevant field name!")
         self.tracks = tracks
 
         if not isinstance(waypoints, GeoDataFrame):
-            raise IllegalArgumentTypeException(waypoints, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(waypoints, "GeoDataFrame")
+        if "id" not in waypoints:
+            raise Exception(f"'id' is not a relevant field name!")
         self.waypoints = waypoints
 
-        assert GeoDataFrameLib.shareTheSameCrs(dfImu, tracks), 'dfImu and tracks must share the same crs!'
-        assert GeoDataFrameLib.shareTheSameCrs(tracks, waypoints), 'tracks and waypoints must share the same crs!'
+        assert GeoDataFrameLib.shareTheSameCrs(dfImu, tracks), "dfImu and tracks must share the same crs!"
+        assert GeoDataFrameLib.shareTheSameCrs(tracks, waypoints), "tracks and waypoints must share the same crs!"
+        self.crs = tracks.crs
 
     def run(self):
         maxTagNames = self.waypoints.maxTagName.unique()
         imu = self.dfImu.copy(deep=True)
-        imu.to_crs(self.tracks.crs, inplace=True)
+        imu.to_crs(self.crs, inplace=True)
 
         # ==============================================================
         # 1st STEP: IDENTIFY THE TRACK TO PROJECT ON
-        imu['track'], imu['curv_absc'], imu['n_curv_absc'] = None, None, None
+        imu["track"], imu["curv_absc"], imu["n_curv_absc"] = None, None, None
 
         prev, cnt1, rows, cnts = nan, nan, [], []
         for cnt2, (_, row) in enumerate(imu.iterrows()):
             curr = row.TagName
             if isnan(prev):
                 prev, cnt1 = (nan, nan) if isnan(curr) else (curr, 0)
                 row.track, row.curv_absc = prev, cnt1
@@ -84,74 +94,67 @@
 
                     if curr in maxTagNames:
                         prev, cnt1 = nan, nan
                     else:
                         prev, cnt1 = curr, 0
 
             rows.append(row)
-        imu = GeoDataFrame(rows, crs=imu.crs)
-
-        imu.curv_absc = list(zip(imu.track, imu.curv_absc, imu.n_curv_absc))
-        imu.track = imu.track.apply(lambda v: v if isnan(v) else int(v // 100))
+        imu = GeoDataFrame(rows, crs=self.crs)
 
         # ==============================================================
         # 2nd STEP: ASSESS THE CURVILINEAR ABSCISSA OF THE PROJECTED POINT
-        wpDict = self.waypoints.set_index('id').to_dict(orient='index')
-
-        foo = lambda t: (None if isnan(t[0]) else (
-            wpDict[t[0]]['curv_absc'] + (t[1] * wpDict[t[0]]['delta_curv_absc']) / t[2]))
-        imu.curv_absc = imu.curv_absc.apply(lambda t: foo(t))
+        wpDict = self.waypoints.set_index("id").to_dict(orient="index")
 
+        imu.curv_absc = imu.apply(lambda row: None
+                                  if isnan(row.track)
+                                  else wpDict[row.track]["curv_absc"] + (row.curv_absc * wpDict[row.track]["delta_curv_absc"]) / row.n_curv_absc,
+                                  axis=1)
         for tn in maxTagNames:
-            imu.loc[ imu[imu.TagName == tn].index, 'curv_absc' ] = 1.0
+            imu.loc[ imu[imu.TagName == tn].index, "curv_absc" ] = 1.0
 
         # ==============================================================
         # 3rd STEP: ASSESS THE COORDINATES OF THE PROJECTED POINT
-        trDict = self.tracks.set_index('id').to_dict(orient='index')
-
-        imu['snap_geometry'] = list(zip(imu.track, imu.curv_absc))
-
-        foo = lambda t: (None if isnan(t[0]) else (
-            trDict[t[0]]['geometry'].interpolate(t[1], normalized=True)
-            ))
-        imu.snap_geometry = imu.snap_geometry.apply(lambda t: foo(t))
+        trDict = {row.id: row.geometry for _, row in self.tracks.iterrows()}
 
+        imu.track = imu.track.apply(lambda v: v if isnan(v) else int(v // 100))
+        imu["snap_geometry"] = imu.apply(lambda row: None
+                                         if isnan(row.track)
+                                         else trDict[row.track].interpolate(row.curv_absc, normalized=True),
+                                         axis=1)
+ 
         # ==============================================================
         # 4th STEP: ASSESS THE DISTANCE (DRIFT) BETWEEN THE GNSS POINT AND 
         # ITS CORRESPONDING PROJECTED POINT
-        imu.rename(columns={'geometry': 'gnss_geom', 'snap_geometry': 'geometry'}, inplace=True)
-        imu.drop(columns=['n_curv_absc'], inplace=True)
-
-        imu['drift'] = list(zip(imu.gnss_geom, imu.geometry))
-        imu.drift = imu.drift.apply(lambda t:
-                                    nan if ((t[0] is None) or (t[1] is None))
-                                    else t[0].distance(t[1]))
+        imu.rename(columns={"geometry": "gnss_geom", "snap_geometry": "geometry"}, inplace=True)
+        imu.drop(columns=["n_curv_absc"], inplace=True)
 
+        imu["drift"] = imu.apply(lambda row: nan 
+                                 if ((row.gnss_geom is None) or (row.geometry is None))
+                                 else row.gnss_geom.distance(row.geometry),
+                                 axis=1)
         imu.gnss_geom = imu.gnss_geom.apply(lambda g: g.wkt)
-        imu.set_crs(self.tracks.crs, inplace=True)
-
-        # imu.drop(columns=['n_curv_absc'], inplace=True)
+        imu.set_crs(self.crs, inplace=True)
 
         imu.drop(index=imu[imu.geometry.isna()].index, inplace=True)
         imu.reset_index(drop=True, inplace=True)
 
         return imu
 
 '''
 import matplotlib.pyplot as plt
 from t4gpd.picoclim.MetrologicalCampaignReader import MetrologicalCampaignReader
 
-# dirName = '/home/tleduc/prj/nm-ilots-frais/terrain/220711'
-dirName = '/home/tleduc/prj/nm-ilots-frais/terrain/220713'
+# dirName = "/home/tleduc/prj/nm-ilots-frais/terrain/220711"
+dirName = "/home/tleduc/prj/nm-ilots-frais/terrain/220713"
 static, tracks, waypoints, dfImu, dfMob, dfStat1, dfStat2, dfMeteoFr = MetrologicalCampaignReader(dirName).run()
 dfImu.to_crs(crs=tracks.crs, inplace=True)
 
 imu = SnapImuOnTrackUsingWaypoints(dfImu, tracks, waypoints).run()
 
-# imu.drop(columns=['timestamp', 'X', 'Y', 'Z', 'Distance', 'degree', 'latitude',
-#                   'longitude', 'GpsAccuracy', 'indoor_outdoor_flag'], inplace=True)
-# imu.to_csv('/home/tleduc/prj/nm-ilots-frais/a.csv', index=False)
-# imu.to_file('/tmp/imu.gpkg')
+# imu.drop(columns=["timestamp", "X", "Y", "Z", "Distance", "degree", "latitude",
+#                   "longitude", "GpsAccuracy", "indoor_outdoor_flag"], inplace=True)
+# imu.to_csv("/home/tleduc/prj/nm-ilots-frais/a.csv", index=False)
+# imu.to_file("/tmp/imu.gpkg")
 imu.plot()
 plt.show()
 
 '''
```

### Comparing `t4gpd-0.6.0/t4gpd/picoclim/TracksWaypointsReader.py` & `t4gpd-0.7.0/t4gpd/picoclim/TracksWaypointsReader.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 import re
 
 from fiona import listlayers
 from geopandas import read_file
 from pandas import concat
+from t4gpd.commons.Epsilon import Epsilon
 from t4gpd.commons.GeoProcess import GeoProcess
 
 
 class TracksWaypointsReader(GeoProcess):
     '''
     classdocs
     '''
@@ -61,22 +62,29 @@
                 df = df[['id', 'geometry']].copy(deep=True)
                 idMin, idMax = df.id.min(), df.id.max()
                 df['minTagName'], df['maxTagName'] = idMin, idMax
                 assert (num == idMin // 100) and (num == idMax // 100), f'inconsistent ids in the waypoints{num} layer'
                 df.sort_values(by='id', inplace=True)
                 waypoints.append(df)
 
-        assert len(tracks) == len(waypoints), 'The number of tracks does not equal the number of waypoints layers!'
+        if (len(tracks) != len(waypoints)):
+            raise Exception("The number of tracks does not equal the number of waypoints layers!")
 
         for i in range(len(tracks)):
             _trackId, _trackGeom, _waypoints = tracks[i].id.squeeze(), tracks[i].geometry.squeeze(), waypoints[i]
             _waypoints['curv_absc'] = _waypoints.geometry.apply(
                 lambda g: _trackGeom.project(g, normalized=True))
+
+            if not _waypoints.curv_absc.is_monotonic_increasing:
+                raise Exception(f"The abscissa of the \
+waypoints should be increasing. Check the direction of track #{_trackId}, which should \
+be consistent with the direction of the waypoints.")
+
             _waypoints['delta_curv_absc'] = _waypoints.curv_absc.diff(periods=1)
             _waypoints.delta_curv_absc = _waypoints.delta_curv_absc.shift(periods=-1)
 
-        assert 0.0 == _waypoints.curv_absc.min(), f'Track {_trackId}: The min. curv. absc. must be equal to 0'
-        assert 1.0 == _waypoints.curv_absc.max(), f'Track {_trackId}: The max. curv. absc. must be equal to 1'
+        assert Epsilon.isZero(_waypoints.curv_absc.min()), f'Track {_trackId}: The min. curv. absc. must be equal to 0'
+        assert Epsilon.equals(1.0, _waypoints.curv_absc.max()), f'Track {_trackId}: The max. curv. absc. must be equal to 1'
 
         tracks = concat(tracks, ignore_index=True)
         waypoints = concat(waypoints, ignore_index=True)
         return static, tracks, waypoints
```

### Comparing `t4gpd-0.6.0/t4gpd/pyplot/MultipleMarkerStyles.py` & `t4gpd-0.7.0/t4gpd/pyplot/MultipleMarkerStyles.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyqgis/AddMemoryLayer.py` & `t4gpd-0.7.0/t4gpd/pyqgis/AddMemoryLayer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyqgis/Emphasizer.py` & `t4gpd-0.7.0/t4gpd/pyqgis/Emphasizer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyqgis/MapPrinter.py` & `t4gpd-0.7.0/t4gpd/pyqgis/MapPrinter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyqgis/PdfMapWriter.py` & `t4gpd-0.7.0/t4gpd/pyqgis/PdfMapWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyqgis/SetSymbolLib.py` & `t4gpd-0.7.0/t4gpd/pyqgis/SetSymbolLib.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                        QgsFillSymbol, QgsHeatmapRenderer,
                        QgsLineSymbol, QgsMarkerSymbol,
                        QgsPalLayerSettings, QgsLinePatternFillSymbolLayer,
                        QgsPointPatternFillSymbolLayer, QgsProperty,
                        QgsRendererCategory, QgsSimpleFillSymbolLayer,
                        QgsSimpleLineSymbolLayer, QgsStyle,
                        QgsSvgMarkerSymbolLayer, QgsSymbol, QgsSymbolLayer,
-                       QgsTextFormat, QgsVectorLayerSimpleLabeling)
+                       QgsTextFormat, QgsUnitTypes, QgsVectorLayerSimpleLabeling)
 from qgis.PyQt.QtGui import QColor
 from qgis.utils import iface
 
 
 class SetSymbolLib(object):
     '''
     classdocs
@@ -56,44 +56,44 @@
     def __otherAltSetSymbol(layer, renderer):
         if layer is not None:
             layer.setRenderer(renderer)
             iface.layerTreeView().refreshLayerSymbology(layer.id())
             layer.triggerRepaint()
 
     @staticmethod
-    def setAlternateFillSymbol(layer, color='black', patternDistance=1.0,
-                               lineAngle=45, penstyle='solid', width='0.35'):
+    def setAlternateFillSymbol(layer, color="black", patternDistance=1.0,
+                               lineAngle=45, penstyle="solid", width="0.35"):
         lineSymbol = QgsLineSymbol.createSimple({
-            'penstyle': penstyle, 'width': width, 'color': color})
+            "penstyle": penstyle, "width": width, "color": color})
         filled_pattern = QgsLinePatternFillSymbolLayer()
         filled_pattern.setLineAngle(lineAngle)
         filled_pattern.setDistance(patternDistance)
         filled_pattern.setSubSymbol(lineSymbol)
         SetSymbolLib.__altSetSymbol(layer, filled_pattern)
 
     @staticmethod
-    def setAlternateFillSymbol2(layer, color='red', color_border='black',
-                                name='diamond', size='3.0'):
+    def setAlternateFillSymbol2(layer, color="red", color_border="black",
+                                name="diamond", size="3.0"):
         markerSymbol = QgsMarkerSymbol.createSimple({
-            'color':color, 'color_border':color_border, 'name':name, 'size':size})
+            "color":color, "color_border":color_border, "name":name, "size":size})
         filled_pattern = QgsPointPatternFillSymbolLayer()
         filled_pattern.setDistanceX(4.0)
         filled_pattern.setDistanceY(4.0)
         filled_pattern.setSubSymbol(markerSymbol)
         SetSymbolLib.__altSetSymbol(layer, filled_pattern)
 
     @staticmethod
-    def setAlternateFillSymbol3(layer, color='black', style='b_diagonal'):
-        # style = ['cross', 'b_diagonal', 'diagonal_x', 'f_diagonal', 
-        # 'horizontal', 'solid', 'vertical']
-        symbol_layer = QgsSimpleFillSymbolLayer.create({'color':color, 'style': style})
+    def setAlternateFillSymbol3(layer, color="black", style="b_diagonal"):
+        # style = ["cross", "b_diagonal", "diagonal_x", "f_diagonal", 
+        # "horizontal", "solid", "vertical"]
+        symbol_layer = QgsSimpleFillSymbolLayer.create({"color":color, "style": style})
         SetSymbolLib.__altSetSymbol(layer, symbol_layer)
 
     @staticmethod
-    def setArrowSymbol(layer, color='black', headType=QgsArrowSymbolLayer.HeadSingle,
+    def setArrowSymbol(layer, color="black", headType=QgsArrowSymbolLayer.HeadSingle,
                        width=0.60, headLength=2.05, headThickness=1.55,
                        arrowType=QgsArrowSymbolLayer.ArrowPlain):
         # headType = {QgsArrowSymbolLayer.HeadDouble, QgsArrowSymbolLayer.HeadReversed, QgsArrowSymbolLayer.HeadSingle}
         # arrowType = {QgsArrowSymbolLayer.ArrowPlain, QgsArrowSymbolLayer.ArrowLeftHalf, QgsArrowSymbolLayer.ArrowRightHalf}
 
         arrowSymbol = QgsArrowSymbolLayer()
         arrowSymbol.setColor(QColor(color))
@@ -112,18 +112,18 @@
 
         SetSymbolLib.__altSetSymbol(layer, arrowSymbol)
 
     @staticmethod
     def setCategorizedSymbol(layer, fieldName, listOfValueColorLabels):
         '''
         listOfValueColorLabels = (
-            ('cat', 'red'),
-            ('dog', 'blue', 'Big dog'),
-            ('sheep', 'green'),
-            ('', 'yellow', 'Unknown')
+            ("cat", "red"),
+            ("dog", "blue", "Big dog"),
+            ("sheep", "green"),
+            ("", "yellow", "Unknown")
         )
         '''
         # CREATE A CATEGORY FOR EACH ITEM IN 'fieldLookupTable'
         categories = []
         for item in listOfValueColorLabels:
             value, color, label = item if 3 == len(item) else [item[0], item[1], item[0]]
             symbol = QgsSymbol.defaultSymbol(layer.geometryType())
@@ -131,88 +131,101 @@
             categories.append(QgsRendererCategory(value, symbol, label))
 
         # CREATE THE RENDERER AND ASSIGN IT TO THE GIVEN LAYER
         renderer = QgsCategorizedSymbolRenderer(fieldName, categories)
         SetSymbolLib.__otherAltSetSymbol(layer, renderer)
 
     @staticmethod
-    def setFillSymbol(layer, color='lightgrey', outline_color='darkgrey',
-                      style_border='solid', width_border='0.75'):
+    def setFillSymbol(layer, color="lightgrey", outline_color="darkgrey",
+                      style_border="solid", width_border="0.75"):
         fillSymbol = QgsFillSymbol.createSimple({
-            'color': color,
-            'outline_color': outline_color,
-            'width_border': width_border,
-            'style_border': style_border})
+            "color": color,
+            "outline_color": outline_color,
+            "width_border": width_border,
+            "style_border": style_border})
         SetSymbolLib.__setSymbol(layer, fillSymbol)
 
     @staticmethod
-    def setHeatMap(layer, radius=20, rampName='Blues'):
+    def setHeatMap(layer, expr, radius=20, rampName="Blues", maxValue=0,
+                   color1=QColor(255, 255, 255, 0),
+                   unit=QgsUnitTypes.RenderUnit.MetersInMapUnits):
         # To get a list of available color ramp names, use:
         # QgsStyle().defaultStyle().colorRampNames()
+        # ["Blues", "BrBG", "BuGn", "BuPu", "GnBu", "Greens", "Greys", "Inferno", "Magma", 
+        # "OrRd", "Oranges", "PRGn", "PiYG", "Plasma", "PuBu", "PuBuGn", "PuOr", "PuRd", 
+        # "Purples", "RdBu", "RdGy", "RdPu", "RdYlBu", "RdYlGn", "Reds", "Spectral", 
+        # "Viridis", "YlGn", "YlGnBu", "YlOrBr", "YlOrRd"]
         ramp = QgsStyle().defaultStyle().colorRamp(rampName)
+        ramp.setColor1(color1)
+
         heatmap = QgsHeatmapRenderer()
-        heatmap.setRadius(radius)
         heatmap.setColorRamp(ramp)
+        heatmap.setMaximumValue(maxValue) # Set to 0 for automatic calculation of max value
+        heatmap.setRadius(radius)
+        heatmap.setRadiusUnit(unit)
+        heatmap.setRenderQuality(1) # A value of 1 indicates maximum quality
+        heatmap.setWeightExpression(expr) # expr: fieldname
+
         SetSymbolLib.__otherAltSetSymbol(layer, heatmap)
 
     @staticmethod
-    def setLabelSymbol(layer, fieldName, overPoint=True, size='14',
-                       color='black', positionX=None, positionY=None,
+    def setLabelSymbol(layer, fieldName, overPoint=True, size="14",
+                       color="black", positionX=None, positionY=None,
                        offsetX=None, offsetY=None):
         label = QgsPalLayerSettings()
         label.fieldName = fieldName
     
         textFormat = QgsTextFormat()
         # bgColor = QgsTextBackgroundSettings()
-        # bgColor.setFillColor(QColor('white'))
+        # bgColor.setFillColor(QColor("white"))
         # bgColor.setEnabled(True)
         # textFormat.setBackground(bgColor )
         textFormat.setColor(QColor(color))
         textFormat.setSize(int(size))
         label.setFormat(textFormat)
         label.isExpression = True
     
         layer.setLabeling(QgsVectorLayerSimpleLabeling(label))
         layer.setLabelsEnabled(True)
         iface.layerTreeView().refreshLayerSymbology(layer.id())
         layer.triggerRepaint()
 
     @staticmethod
-    def setLineSymbol(layer, color='black', penstyle='solid', width='0.55'):
+    def setLineSymbol(layer, color="black", penstyle="solid", width="0.55"):
         # dash, dash dot, dash dot dot, dot, solid
         lineSymbol = QgsLineSymbol.createSimple({
-            'color': color, 'penstyle': penstyle, 'width': width})
+            "color": color, "penstyle": penstyle, "width": width})
         SetSymbolLib.__setSymbol(layer, lineSymbol)
 
     @staticmethod
-    def setMarkerSymbol(layer, color='black', size='3.6', name='circle'):
+    def setMarkerSymbol(layer, color="black", size="3.6", name="circle"):
         # circle, square, rectangle, diamond, pentagon, triangle, 
         # equilateral_triangle, star, regular_star, arrow 
         nodesSymbol = QgsMarkerSymbol.createSimple({
-            'color': color, 'name': name, 'size': size, 'width_border': '0'})
+            "color": color, "name": name, "size": size, "width_border": "0"})
         SetSymbolLib.__setSymbol(layer, nodesSymbol)
 
     @staticmethod
-    def setSimpleOutlineFillSymbol(layer, color='red', width='1.1', penstyle='dot'):
+    def setSimpleOutlineFillSymbol(layer, color="red", width="1.1", penstyle="dot"):
         symbol_layer = QgsSimpleLineSymbolLayer.create(
-            {'color': color, 'width': width, 'penstyle': penstyle})
+            {"color": color, "width": width, "penstyle": penstyle})
         SetSymbolLib.__altSetSymbol(layer, symbol_layer)
 
     @staticmethod
     def setSvgSymbol(markerLayer, fieldName, svgSymbolDirname,
-                     size='6', rotationFieldName=None):
+                     size="6", rotationFieldName=None):
         if markerLayer is not None:
             fni = markerLayer.dataProvider().fieldNameIndex(fieldName)
             uniqValues = markerLayer.dataProvider().uniqueValues(fni)
 
             categories = []
             for value in uniqValues:
                 mySymbol = QgsSymbol.defaultSymbol(markerLayer.geometryType())
 
-                svgStyle = { 'name': f'{svgSymbolDirname}/{value}.svg', 'size': size }
+                svgStyle = { "name": f"{svgSymbolDirname}/{value}.svg", "size": size }
                 svgSymbol = QgsSvgMarkerSymbolLayer.create(svgStyle)
                 if rotationFieldName is not None:
                     svgSymbol.dataDefinedProperties().setProperty(
                         QgsSymbolLayer.PropertyAngle, QgsProperty.fromField(rotationFieldName))
 
                 mySymbol.changeSymbolLayer(0, svgSymbol)
```

### Comparing `t4gpd-0.6.0/t4gpd/pyqgis/ShowFeatureCount.py` & `t4gpd-0.7.0/t4gpd/pyqgis/ShowFeatureCount.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyqgis/ZoomLib.py` & `t4gpd-0.7.0/t4gpd/pyqgis/ZoomLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/GeodeCiel.py` & `t4gpd-0.7.0/t4gpd/pyvista/GeodeCiel.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/Icosahedron.py` & `t4gpd-0.7.0/t4gpd/pyvista/Icosahedron.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/STRaysToViewFactors.py` & `t4gpd-0.7.0/t4gpd/pyvista/STRaysToViewFactors.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/ToPolyData.py` & `t4gpd-0.7.0/t4gpd/pyvista/ToPolyData.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/ToUnstructuredGrid.py` & `t4gpd-0.7.0/t4gpd/pyvista/ToUnstructuredGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/commons/Diameter3DLib.py` & `t4gpd-0.7.0/t4gpd/pyvista/commons/Diameter3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/commons/RayCasting3DLib.py` & `t4gpd-0.7.0/t4gpd/pyvista/commons/RayCasting3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py` & `t4gpd-0.7.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/commons/SVF3DLib.py` & `t4gpd-0.7.0/t4gpd/pyvista/commons/SVF3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/commons/Triangle3D.py` & `t4gpd-0.7.0/t4gpd/pyvista/commons/Triangle3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py` & `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py` & `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py` & `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py` & `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py` & `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py` & `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/pyvista/geoProcesses/SVF3D.py` & `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/SVF3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/raster/STToRaster.py` & `t4gpd-0.7.0/t4gpd/raster/STToRaster.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/AbstractHardShadow.py` & `t4gpd-0.7.0/t4gpd/sun/AbstractHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/STHardShadow.py` & `t4gpd-0.7.0/t4gpd/sun/STHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/STSunMap2D.py` & `t4gpd-0.7.0/t4gpd/sun/STSunMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/STTreeHardShadow.py` & `t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/STTreeHardShadow2.py` & `t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py` & `t4gpd-0.7.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/geoProcesses/SunshineDuration.py` & `t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py` & `t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.6.0/t4gpd.egg-info/PKG-INFO` & `t4gpd-0.7.0/t4gpd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.6.0
+Version: 0.7.0
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
 Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
@@ -33,17 +33,17 @@
 
 > conda activate gpd
 
 > conda config --env --add channels conda-forge
 
 > conda config --env --set channel_priority strict
 
-> conda install geopandas descartes matplotlib networkx notebook numpy pysolar plotly
+> conda install python=3.10 geopandas=0.12.2 jupyterlab matplotlib notebook scikit-learn xlrd openpyxl imageio rasterio networkx PyWavelets pysolar windrose geocube mapclassify seaborn plotly matplotlib-scalebar pyvista contextily xlwt
 
-> pip install matplotlib-scalebar Dijkstar suntimes windrose
+> pip install Dijkstar suntimes pythermalcomfort
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
 > pip install t4gpd-0.6.0.tar.gz
```

### Comparing `t4gpd-0.6.0/t4gpd.egg-info/SOURCES.txt` & `t4gpd-0.7.0/t4gpd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 t4gpd/commons/ArrayCoding.py
 t4gpd/commons/BoundingBox.py
 t4gpd/commons/CSVLib.py
 t4gpd/commons/CalendarLib.py
 t4gpd/commons/CaliperLib.py
 t4gpd/commons/Checksum.py
 t4gpd/commons/ChrystalAlgorithm.py
+t4gpd/commons/ColorTemperature.py
 t4gpd/commons/DataFrameLib.py
 t4gpd/commons/DateRangeLib.py
 t4gpd/commons/DatetimeLib.py
 t4gpd/commons/DiameterLib.py
 t4gpd/commons/Distances.py
 t4gpd/commons/Entropy.py
 t4gpd/commons/Epsilon.py
@@ -77,21 +78,23 @@
 t4gpd/commons/MyEdge.py
 t4gpd/commons/MyNode.py
 t4gpd/commons/PointsDensifierLib.py
 t4gpd/commons/PointsDensifierLib3D.py
 t4gpd/commons/PolarCartesianCoordinates.py
 t4gpd/commons/RayCasting2Lib.py
 t4gpd/commons/RayCasting3Lib.py
+t4gpd/commons/RayCasting4Lib.py
 t4gpd/commons/RayCastingLib.py
 t4gpd/commons/RotationLib.py
 t4gpd/commons/SVFLib.py
 t4gpd/commons/ShannonEntropy.py
 t4gpd/commons/SphericalCartesianCoordinates.py
 t4gpd/commons/SphericalProjectionLib.py
 t4gpd/commons/TestUtils.py
+t4gpd/commons/WarnUtils.py
 t4gpd/commons/__init__.py
 t4gpd/commons/crossroads_generation/Sequence.py
 t4gpd/commons/crossroads_generation/SequenceRadii.py
 t4gpd/commons/crossroads_generation/SequencesGeneration.py
 t4gpd/commons/crossroads_generation/__init__.py
 t4gpd/commons/crossroads_identification/AbstractMethod.py
 t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
@@ -131,14 +134,16 @@
 t4gpd/demos/GeoDataFrameDemos4.py
 t4gpd/demos/GeoDataFrameDemos5.py
 t4gpd/demos/GeoDataFrameDemos6.py
 t4gpd/demos/GeoDataFrameDemos7.py
 t4gpd/demos/GeoDataFrameDemos8.py
 t4gpd/demos/GeoDataFrameDemos9.py
 t4gpd/demos/GeoDataFrameDemosA.py
+t4gpd/demos/GeoDataFrameDemosB.py
+t4gpd/demos/GeoDataFrameDemosC.py
 t4gpd/demos/__init__.py
 t4gpd/energy/DirectSolarIrradianceLib.py
 t4gpd/energy/Dogniaux.py
 t4gpd/energy/Perez.py
 t4gpd/energy/Perraudeau.py
 t4gpd/energy/PerrinDeBrichambaut.py
 t4gpd/energy/PlotDirectNormalIrradiance.py
@@ -174,14 +179,15 @@
 t4gpd/io/SalomeWriterAndExtruder.py
 t4gpd/io/VTUWriter.py
 t4gpd/io/ValReader.py
 t4gpd/io/ZipLoader.py
 t4gpd/io/ZipWriter.py
 t4gpd/io/__init__.py
 t4gpd/isovist/STIsovistField2D.py
+t4gpd/isovist/STIsovistField2D_new.py
 t4gpd/isovist/__init__.py
 t4gpd/misc/FrequencyHistogram.py
 t4gpd/misc/OptimalNumberOfClusters.py
 t4gpd/misc/PlotAMatrixOfDiagrams.py
 t4gpd/misc/PopulationPyramid.py
 t4gpd/misc/RoseMappingTool.py
 t4gpd/misc/STCompass.py
@@ -199,21 +205,23 @@
 t4gpd/morph/STDilationErosion.py
 t4gpd/morph/STExtractOpenSpaces.py
 t4gpd/morph/STFacadesAnalysis.py
 t4gpd/morph/STGradientOfDistancesToBuildings.py
 t4gpd/morph/STGrid.py
 t4gpd/morph/STIdentifyRowOfTrees.py
 t4gpd/morph/STMakeBlocks.py
+t4gpd/morph/STMakeGroundSurface.py
 t4gpd/morph/STMultipleOverlaps.py
 t4gpd/morph/STMultipleOverlaps2.py
 t4gpd/morph/STPointsDensifier.py
 t4gpd/morph/STPointsDensifier2.py
 t4gpd/morph/STPolygonize.py
 t4gpd/morph/STSkeletonize.py
 t4gpd/morph/STSkeletonizeTheVoid.py
+t4gpd/morph/STSkyMap25D.py
 t4gpd/morph/STSnappingPointsOnLines.py
 t4gpd/morph/STSnappingPointsOnLines2.py
 t4gpd/morph/STSpatialJoin.py
 t4gpd/morph/STSquaredBBox.py
 t4gpd/morph/STVariableWidthBuffer.py
 t4gpd/morph/STVoronoiPartition.py
 t4gpd/morph/__init__.py
@@ -257,36 +265,41 @@
 t4gpd/morph/geoProcesses/StarShapedIndices.py
 t4gpd/morph/geoProcesses/SurfaceFraction.py
 t4gpd/morph/geoProcesses/Translation.py
 t4gpd/morph/geoProcesses/WMean.py
 t4gpd/morph/geoProcesses/__init__.py
 t4gpd/picoclim/CampbellSciReader.py
 t4gpd/picoclim/ExtraProcessing.py
+t4gpd/picoclim/InertialMeasureReWriter.py
 t4gpd/picoclim/InertialMeasureReader.py
 t4gpd/picoclim/JoinByTimeDistance.py
 t4gpd/picoclim/KestrelReader.py
 t4gpd/picoclim/MeteoFranceReader.py
 t4gpd/picoclim/MetrologicalCampaignPlottings.py
 t4gpd/picoclim/MetrologicalCampaignReader.py
 t4gpd/picoclim/SensirionReader.py
 t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
+t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
 t4gpd/picoclim/TracksWaypointsReader.py
+t4gpd/picoclim/UClimGuidingReader.py
+t4gpd/picoclim/UClimTrackWaypointsReader.py
 t4gpd/picoclim/__init__.py
 t4gpd/pyplot/MultipleMarkerStyles.py
 t4gpd/pyplot/__init__.py
 t4gpd/pyqgis/AddMemoryLayer.py
 t4gpd/pyqgis/Emphasizer.py
 t4gpd/pyqgis/MapPrinter.py
 t4gpd/pyqgis/PdfMapWriter.py
 t4gpd/pyqgis/SetSymbolLib.py
 t4gpd/pyqgis/ShowFeatureCount.py
 t4gpd/pyqgis/ZoomLib.py
 t4gpd/pyqgis/__init__.py
 t4gpd/pyvista/GeodeCiel.py
 t4gpd/pyvista/Icosahedron.py
+t4gpd/pyvista/Plotter3D.py
 t4gpd/pyvista/STRaysToViewFactors.py
 t4gpd/pyvista/ToPolyData.py
 t4gpd/pyvista/ToUnstructuredGrid.py
 t4gpd/pyvista/__init__.py
 t4gpd/pyvista/commons/Diameter3DLib.py
 t4gpd/pyvista/commons/RayCasting3DLib.py
 t4gpd/pyvista/commons/RayCastingIn3DLib.py
```

