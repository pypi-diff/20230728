# Comparing `tmp/t4gpd-0.7.0.tar.gz` & `tmp/t4gpd-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t4gpd-0.7.0.tar", last modified: Fri Jul 28 08:41:41 2023, max compression
+gzip compressed data, was "t4gpd-0.7.1.tar", last modified: Fri Jul 28 09:25:50 2023, max compression
```

## Comparing `t4gpd-0.7.0.tar` & `t4gpd-0.7.1.tar`

### file list

```diff
@@ -1,362 +1,362 @@
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.379548 t4gpd-0.7.0/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    35149 2020-06-13 17:54:58.000000 t4gpd-0.7.0/LICENSE.txt
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2545 2023-07-28 08:41:41.379548 t4gpd-0.7.0/PKG-INFO
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1490 2023-03-23 21:33:47.000000 t4gpd-0.7.0/README.md
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      107 2023-07-28 08:41:41.379548 t4gpd-0.7.0/setup.cfg
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2141 2022-08-24 08:30:43.000000 t4gpd-0.7.0/setup.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.335548 t4gpd-0.7.0/t4gpd/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      739 2020-11-20 20:32:18.000000 t4gpd-0.7.0/t4gpd/__init__.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      804 2023-07-28 08:34:21.000000 t4gpd-0.7.0/t4gpd/_version.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.335548 t4gpd-0.7.0/t4gpd/comfort/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1492 2022-10-14 15:48:15.000000 t4gpd-0.7.0/t4gpd/comfort/EmpiricalThermalIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-17 12:41:51.000000 t4gpd-0.7.0/t4gpd/comfort/LinearThermalIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2478 2022-10-14 15:47:50.000000 t4gpd-0.7.0/t4gpd/comfort/UniversalThermalIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-02 17:38:35.000000 t4gpd-0.7.0/t4gpd/comfort/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.339548 t4gpd-0.7.0/t4gpd/comfort/algo/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5931 2021-05-12 17:04:21.000000 t4gpd-0.7.0/t4gpd/comfort/algo/CommonsLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4716 2021-05-12 16:38:39.000000 t4gpd-0.7.0/t4gpd/comfort/algo/ConstantsLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7079 2021-05-17 12:10:26.000000 t4gpd-0.7.0/t4gpd/comfort/algo/ETULib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1432 2021-05-12 16:42:17.000000 t4gpd-0.7.0/t4gpd/comfort/algo/PETLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1874 2021-09-02 09:59:31.000000 t4gpd-0.7.0/t4gpd/comfort/algo/PMVLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1714 2021-05-17 13:02:49.000000 t4gpd-0.7.0/t4gpd/comfort/algo/PTLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2066 2021-09-02 10:00:06.000000 t4gpd-0.7.0/t4gpd/comfort/algo/SETLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8302 2021-12-10 17:18:50.000000 t4gpd-0.7.0/t4gpd/comfort/algo/SET_mist.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1380 2021-05-12 08:12:54.000000 t4gpd-0.7.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-12 18:58:48.000000 t4gpd-0.7.0/t4gpd/comfort/algo/TmrtOutLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    17227 2022-10-24 09:23:00.000000 t4gpd-0.7.0/t4gpd/comfort/algo/UTCILib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13633 2021-02-04 21:08:03.000000 t4gpd-0.7.0/t4gpd/comfort/algo/VDI_PET_corrected.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1284 2022-10-24 09:21:44.000000 t4gpd-0.7.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-04 21:08:03.000000 t4gpd-0.7.0/t4gpd/comfort/algo/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.339548 t4gpd-0.7.0/t4gpd/comfort/indices/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2650 2022-10-14 15:46:56.000000 t4gpd-0.7.0/t4gpd/comfort/indices/ASV.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      876 2021-05-12 06:43:03.000000 t4gpd-0.7.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1980 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/DI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3216 2022-10-14 15:46:30.000000 t4gpd-0.7.0/t4gpd/comfort/indices/ETU.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2004 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/H.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2396 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/HI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2202 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/NET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2331 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/OUTSET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2037 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PE.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3895 2023-06-16 15:01:43.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3088 2022-10-24 15:23:58.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PMV.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2232 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/PT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2801 2022-10-24 15:23:09.000000 t4gpd-0.7.0/t4gpd/comfort/indices/SET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3026 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/SETmist.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/THI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2223 2021-05-12 19:36:36.000000 t4gpd-0.7.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2178 2022-10-14 15:45:34.000000 t4gpd-0.7.0/t4gpd/comfort/indices/TmrtOut.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5838 2022-10-14 15:44:45.000000 t4gpd-0.7.0/t4gpd/comfort/indices/TmrtRadiometer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3953 2023-06-16 14:56:42.000000 t4gpd-0.7.0/t4gpd/comfort/indices/UTCI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2660 2022-10-14 14:25:47.000000 t4gpd-0.7.0/t4gpd/comfort/indices/WCT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-05-11 16:27:08.000000 t4gpd-0.7.0/t4gpd/comfort/indices/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1608 2020-10-07 15:28:18.000000 t4gpd-0.7.0/t4gpd/commons/AngleLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1189 2021-01-07 07:59:17.000000 t4gpd-0.7.0/t4gpd/commons/ArrayCoding.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2308 2020-06-19 14:10:50.000000 t4gpd-0.7.0/t4gpd/commons/BoundingBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2366 2020-12-16 13:15:18.000000 t4gpd-0.7.0/t4gpd/commons/CSVLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1675 2021-07-01 09:32:35.000000 t4gpd-0.7.0/t4gpd/commons/CalendarLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7227 2021-06-16 14:25:07.000000 t4gpd-0.7.0/t4gpd/commons/CaliperLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      959 2020-10-02 12:26:10.000000 t4gpd-0.7.0/t4gpd/commons/Checksum.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4541 2020-12-15 16:02:11.000000 t4gpd-0.7.0/t4gpd/commons/ChrystalAlgorithm.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2023-06-24 06:23:57.000000 t4gpd-0.7.0/t4gpd/commons/ColorTemperature.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1637 2022-10-26 07:58:39.000000 t4gpd-0.7.0/t4gpd/commons/DataFrameLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2271 2022-08-24 10:23:43.000000 t4gpd-0.7.0/t4gpd/commons/DateRangeLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4956 2022-05-18 15:38:27.000000 t4gpd-0.7.0/t4gpd/commons/DatetimeLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1770 2022-09-05 10:36:15.000000 t4gpd-0.7.0/t4gpd/commons/DiameterLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5876 2020-06-22 09:32:49.000000 t4gpd-0.7.0/t4gpd/commons/Distances.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2831 2022-01-18 19:42:17.000000 t4gpd-0.7.0/t4gpd/commons/Entropy.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2832 2020-09-11 17:04:11.000000 t4gpd-0.7.0/t4gpd/commons/Epsilon.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1357 2022-10-25 14:40:11.000000 t4gpd-0.7.0/t4gpd/commons/GeoDataFrameLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1907 2021-05-18 08:44:20.000000 t4gpd-0.7.0/t4gpd/commons/GeoProcess.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25373 2023-02-15 21:10:56.000000 t4gpd-0.7.0/t4gpd/commons/GeomLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5407 2022-09-07 15:04:19.000000 t4gpd-0.7.0/t4gpd/commons/GeomLib3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4427 2022-03-28 12:35:37.000000 t4gpd-0.7.0/t4gpd/commons/GridFaceLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1149 2020-06-19 13:58:19.000000 t4gpd-0.7.0/t4gpd/commons/IllegalArgumentTypeException.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5933 2022-11-08 14:40:17.000000 t4gpd-0.7.0/t4gpd/commons/KernelLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3784 2020-10-24 09:49:18.000000 t4gpd-0.7.0/t4gpd/commons/LandoltRingLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2526 2022-03-08 14:24:54.000000 t4gpd-0.7.0/t4gpd/commons/LatLonLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2291 2021-04-12 07:38:42.000000 t4gpd-0.7.0/t4gpd/commons/LineStringCuttingLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1989 2020-10-11 20:51:06.000000 t4gpd-0.7.0/t4gpd/commons/ListUtilities.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5244 2022-06-02 10:16:48.000000 t4gpd-0.7.0/t4gpd/commons/Logos.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2108 2020-06-17 18:58:12.000000 t4gpd-0.7.0/t4gpd/commons/MyEdge.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2709 2020-09-24 09:53:56.000000 t4gpd-0.7.0/t4gpd/commons/MyNode.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8008 2022-06-13 13:36:47.000000 t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3137 2022-09-20 15:59:32.000000 t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2833 2020-06-22 09:34:45.000000 t4gpd-0.7.0/t4gpd/commons/PolarCartesianCoordinates.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13455 2023-01-30 13:37:02.000000 t4gpd-0.7.0/t4gpd/commons/RayCasting2Lib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13317 2023-02-16 10:09:06.000000 t4gpd-0.7.0/t4gpd/commons/RayCasting3Lib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11979 2023-07-27 19:53:59.000000 t4gpd-0.7.0/t4gpd/commons/RayCasting4Lib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11700 2023-02-20 09:15:16.000000 t4gpd-0.7.0/t4gpd/commons/RayCastingLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5638 2022-07-20 08:24:45.000000 t4gpd-0.7.0/t4gpd/commons/RotationLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2201 2022-04-08 14:27:04.000000 t4gpd-0.7.0/t4gpd/commons/SVFLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2307 2021-01-15 15:49:37.000000 t4gpd-0.7.0/t4gpd/commons/ShannonEntropy.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1308 2022-07-19 14:44:29.000000 t4gpd-0.7.0/t4gpd/commons/SphericalCartesianCoordinates.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4937 2022-09-20 16:03:36.000000 t4gpd-0.7.0/t4gpd/commons/SphericalProjectionLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1404 2021-06-08 21:34:17.000000 t4gpd-0.7.0/t4gpd/commons/TestUtils.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1502 2023-05-24 21:14:34.000000 t4gpd-0.7.0/t4gpd/commons/WarnUtils.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 09:59:56.000000 t4gpd-0.7.0/t4gpd/commons/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5464 2023-05-24 14:00:40.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/Sequence.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2722 2023-05-23 14:00:27.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/SequenceRadii.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3626 2022-11-07 10:44:48.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 10:44:48.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_generation/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1860 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/AbstractMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3791 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1070 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FFTMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3228 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FWTMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2953 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1160 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 14:02:08.000000 t4gpd-0.7.0/t4gpd/commons/crossroads_identification/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/ellipse/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2020-08-31 08:21:22.000000 t4gpd-0.7.0/t4gpd/commons/ellipse/EllipseLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25237 2020-06-23 22:05:17.000000 t4gpd-0.7.0/t4gpd/commons/ellipse/EllipticHullLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-23 22:04:55.000000 t4gpd-0.7.0/t4gpd/commons/ellipse/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/graph/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6382 2021-03-24 08:57:48.000000 t4gpd-0.7.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4942 2023-01-27 17:52:06.000000 t4gpd-0.7.0/t4gpd/commons/graph/MCALib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4987 2020-11-23 09:56:15.000000 t4gpd-0.7.0/t4gpd/commons/graph/NeighborhoodLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2883 2020-11-23 09:55:51.000000 t4gpd-0.7.0/t4gpd/commons/graph/ShortestPathLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4289 2020-11-23 10:13:17.000000 t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6322 2021-06-25 08:43:27.000000 t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLibOld.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-21 18:40:43.000000 t4gpd-0.7.0/t4gpd/commons/graph/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/grid/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2298 2023-07-26 09:36:34.000000 t4gpd-0.7.0/t4gpd/commons/grid/AbstractGridLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6264 2023-02-17 15:49:30.000000 t4gpd-0.7.0/t4gpd/commons/grid/GridLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-04-09 08:07:33.000000 t4gpd-0.7.0/t4gpd/commons/grid/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/isovists/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-25 21:42:21.000000 t4gpd-0.7.0/t4gpd/commons/isovists/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.347548 t4gpd-0.7.0/t4gpd/commons/rnd/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4458 2023-05-23 15:30:11.000000 t4gpd-0.7.0/t4gpd/commons/rnd/RandomPointPicking.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2023-01-09 09:57:47.000000 t4gpd-0.7.0/t4gpd/commons/rnd/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.351548 t4gpd-0.7.0/t4gpd/commons/sun/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2774 2021-04-21 15:35:41.000000 t4gpd-0.7.0/t4gpd/commons/sun/AbstractSunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1441 2022-12-08 17:43:59.000000 t4gpd-0.7.0/t4gpd/commons/sun/DaylightLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1897 2021-06-01 20:45:53.000000 t4gpd-0.7.0/t4gpd/commons/sun/PySolarSunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7584 2021-04-22 16:07:47.000000 t4gpd-0.7.0/t4gpd/commons/sun/ShadowLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6719 2021-04-21 15:36:33.000000 t4gpd-0.7.0/t4gpd/commons/sun/SoleneSunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2429 2022-05-18 15:30:31.000000 t4gpd-0.7.0/t4gpd/commons/sun/SunBeamLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8335 2021-12-10 17:17:50.000000 t4gpd-0.7.0/t4gpd/commons/sun/SunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-21 13:30:14.000000 t4gpd-0.7.0/t4gpd/commons/sun/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.355548 t4gpd-0.7.0/t4gpd/demos/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1113 2023-06-08 13:02:08.000000 t4gpd-0.7.0/t4gpd/demos/AbstractGeoDataFrameDemos.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   405923 2023-01-26 09:35:22.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)  1039604 2022-10-25 15:14:06.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   453528 2022-10-25 15:00:19.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos3.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)  2888649 2022-10-25 15:48:49.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos4.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   745426 2022-07-18 15:50:21.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos5.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435846 2022-10-26 14:52:50.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos6.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25686 2022-10-31 17:23:24.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos7.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435537 2022-10-31 17:22:15.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos8.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    87843 2023-03-22 16:19:10.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos9.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   274632 2023-04-27 15:51:16.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosA.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   165333 2023-06-08 13:26:24.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosB.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   193794 2023-06-08 13:03:08.000000 t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosC.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-26 22:34:45.000000 t4gpd-0.7.0/t4gpd/demos/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.359548 t4gpd-0.7.0/t4gpd/energy/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12332 2022-04-28 15:33:51.000000 t4gpd-0.7.0/t4gpd/energy/DirectSolarIrradianceLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3194 2022-07-22 08:39:12.000000 t4gpd-0.7.0/t4gpd/energy/Dogniaux.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3035 2022-07-22 08:20:11.000000 t4gpd-0.7.0/t4gpd/energy/Perez.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1107 2022-07-22 08:20:39.000000 t4gpd-0.7.0/t4gpd/energy/Perraudeau.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3305 2022-07-22 08:21:55.000000 t4gpd-0.7.0/t4gpd/energy/PerrinDeBrichambaut.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3748 2022-07-22 08:40:41.000000 t4gpd-0.7.0/t4gpd/energy/PlotDirectNormalIrradiance.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:57:12.000000 t4gpd-0.7.0/t4gpd/energy/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.359548 t4gpd-0.7.0/t4gpd/energy/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4517 2022-05-18 17:36:24.000000 t4gpd-0.7.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-28 20:49:22.000000 t4gpd-0.7.0/t4gpd/energy/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.359548 t4gpd-0.7.0/t4gpd/graph/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1047 2020-12-31 14:32:10.000000 t4gpd-0.7.0/t4gpd/graph/STBetweennessCentrality.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1043 2020-12-19 20:28:37.000000 t4gpd-0.7.0/t4gpd/graph/STClosenessCentrality.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2657 2020-11-23 10:00:25.000000 t4gpd-0.7.0/t4gpd/graph/STRoadNeighborhood.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2459 2020-11-21 19:04:19.000000 t4gpd-0.7.0/t4gpd/graph/STShortestPath.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1644 2020-11-23 10:45:34.000000 t4gpd-0.7.0/t4gpd/graph/STToRoadsSections.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1474 2020-11-23 10:45:52.000000 t4gpd-0.7.0/t4gpd/graph/STToRoadsSectionsNodes.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 07:51:42.000000 t4gpd-0.7.0/t4gpd/graph/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.363548 t4gpd-0.7.0/t4gpd/io/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1120 2023-04-29 15:30:18.000000 t4gpd-0.7.0/t4gpd/io/AbstractReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4231 2020-09-24 09:56:55.000000 t4gpd-0.7.0/t4gpd/io/CSVInertialSensorReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1889 2020-09-24 09:57:20.000000 t4gpd-0.7.0/t4gpd/io/CSVReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1884 2021-03-10 14:24:32.000000 t4gpd-0.7.0/t4gpd/io/CSVWKTReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2317 2021-03-10 14:24:47.000000 t4gpd-0.7.0/t4gpd/io/CSVWKTWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3373 2022-07-25 09:09:50.000000 t4gpd-0.7.0/t4gpd/io/CirReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1314 2022-07-25 09:34:22.000000 t4gpd-0.7.0/t4gpd/io/CirValReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3331 2021-03-10 21:07:26.000000 t4gpd-0.7.0/t4gpd/io/CirWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5578 2020-10-22 16:39:22.000000 t4gpd-0.7.0/t4gpd/io/CityGMLReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7156 2022-06-24 16:06:01.000000 t4gpd-0.7.0/t4gpd/io/GeoWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1829 2022-11-09 15:42:30.000000 t4gpd-0.7.0/t4gpd/io/GpkgLoader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1818 2022-11-09 15:42:30.000000 t4gpd-0.7.0/t4gpd/io/GpkgWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12097 2021-06-25 08:29:09.000000 t4gpd-0.7.0/t4gpd/io/MshReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3750 2020-08-25 16:50:36.000000 t4gpd-0.7.0/t4gpd/io/ObjReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3541 2021-02-01 10:43:14.000000 t4gpd-0.7.0/t4gpd/io/ObjWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1430 2021-07-19 15:31:30.000000 t4gpd-0.7.0/t4gpd/io/Reloading.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1152 2022-04-26 12:38:58.000000 t4gpd-0.7.0/t4gpd/io/STLoadAndClip.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3086 2020-06-19 14:12:42.000000 t4gpd-0.7.0/t4gpd/io/SVGWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5130 2022-07-26 12:53:22.000000 t4gpd-0.7.0/t4gpd/io/SalomeWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5030 2022-07-26 12:53:22.000000 t4gpd-0.7.0/t4gpd/io/SalomeWriterAndExtruder.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6490 2021-03-10 14:25:07.000000 t4gpd-0.7.0/t4gpd/io/VTUWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2492 2022-07-25 09:33:33.000000 t4gpd-0.7.0/t4gpd/io/ValReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2806 2021-11-08 15:20:17.000000 t4gpd-0.7.0/t4gpd/io/ZipLoader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3559 2021-10-18 16:00:12.000000 t4gpd-0.7.0/t4gpd/io/ZipWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 18:59:50.000000 t4gpd-0.7.0/t4gpd/io/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.363548 t4gpd-0.7.0/t4gpd/isovist/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4347 2022-07-27 15:30:51.000000 t4gpd-0.7.0/t4gpd/isovist/STIsovistField2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4697 2023-07-27 17:24:29.000000 t4gpd-0.7.0/t4gpd/isovist/STIsovistField2D_new.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 09:56:41.000000 t4gpd-0.7.0/t4gpd/isovist/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.363548 t4gpd-0.7.0/t4gpd/misc/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4972 2021-07-20 15:59:02.000000 t4gpd-0.7.0/t4gpd/misc/FrequencyHistogram.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5748 2023-03-23 17:02:07.000000 t4gpd-0.7.0/t4gpd/misc/OptimalNumberOfClusters.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5344 2021-11-14 15:44:04.000000 t4gpd-0.7.0/t4gpd/misc/PlotAMatrixOfDiagrams.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2960 2021-10-01 15:35:34.000000 t4gpd-0.7.0/t4gpd/misc/PopulationPyramid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5500 2023-01-19 10:23:40.000000 t4gpd-0.7.0/t4gpd/misc/RoseMappingTool.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3038 2022-03-15 16:20:31.000000 t4gpd-0.7.0/t4gpd/misc/STCompass.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2311 2023-03-23 14:05:55.000000 t4gpd-0.7.0/t4gpd/misc/STDendrogram.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2023-03-23 16:15:02.000000 t4gpd-0.7.0/t4gpd/misc/STKMeans.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4364 2021-01-25 16:17:15.000000 t4gpd-0.7.0/t4gpd/misc/StreetOrientationHistogram.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4386 2022-12-13 18:08:58.000000 t4gpd-0.7.0/t4gpd/misc/TimelineTool.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2824 2021-03-15 16:13:35.000000 t4gpd-0.7.0/t4gpd/misc/WindRose.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-09-29 10:07:30.000000 t4gpd-0.7.0/t4gpd/misc/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.367548 t4gpd-0.7.0/t4gpd/morph/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2873 2021-08-25 16:19:57.000000 t4gpd-0.7.0/t4gpd/morph/GmshTriangulator.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1413 2023-02-17 18:32:38.000000 t4gpd-0.7.0/t4gpd/morph/STBBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1793 2020-06-30 09:46:17.000000 t4gpd-0.7.0/t4gpd/morph/STClip.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4603 2022-08-24 09:39:40.000000 t4gpd-0.7.0/t4gpd/morph/STCoolscapesTessellation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2723 2023-05-23 14:01:31.000000 t4gpd-0.7.0/t4gpd/morph/STCrossroadsGeneration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2853 2023-02-14 11:31:50.000000 t4gpd-0.7.0/t4gpd/morph/STDilationErosion.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2103 2020-12-14 16:55:46.000000 t4gpd-0.7.0/t4gpd/morph/STExtractOpenSpaces.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3726 2021-04-02 09:43:35.000000 t4gpd-0.7.0/t4gpd/morph/STFacadesAnalysis.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8594 2023-02-20 08:30:55.000000 t4gpd-0.7.0/t4gpd/morph/STGradientOfDistancesToBuildings.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2043 2023-07-26 10:17:45.000000 t4gpd-0.7.0/t4gpd/morph/STGrid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3688 2020-09-17 11:02:43.000000 t4gpd-0.7.0/t4gpd/morph/STIdentifyRowOfTrees.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4480 2021-12-09 14:49:10.000000 t4gpd-0.7.0/t4gpd/morph/STMakeBlocks.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1701 2023-06-07 10:51:36.000000 t4gpd-0.7.0/t4gpd/morph/STMakeGroundSurface.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2812 2020-09-21 14:15:12.000000 t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4550 2023-02-20 08:36:37.000000 t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3134 2022-06-13 13:37:40.000000 t4gpd-0.7.0/t4gpd/morph/STPointsDensifier.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2118 2022-06-13 13:11:05.000000 t4gpd-0.7.0/t4gpd/morph/STPointsDensifier2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1717 2020-12-31 16:03:16.000000 t4gpd-0.7.0/t4gpd/morph/STPolygonize.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3105 2023-02-15 17:59:34.000000 t4gpd-0.7.0/t4gpd/morph/STSkeletonize.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2294 2023-02-15 20:25:15.000000 t4gpd-0.7.0/t4gpd/morph/STSkeletonizeTheVoid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6054 2023-07-27 20:19:56.000000 t4gpd-0.7.0/t4gpd/morph/STSkyMap25D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3196 2020-09-24 10:27:56.000000 t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6567 2022-08-24 09:55:25.000000 t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3217 2021-05-18 08:45:03.000000 t4gpd-0.7.0/t4gpd/morph/STSpatialJoin.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1568 2022-10-14 10:00:03.000000 t4gpd-0.7.0/t4gpd/morph/STSquaredBBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2628 2023-01-31 10:54:56.000000 t4gpd-0.7.0/t4gpd/morph/STVariableWidthBuffer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3729 2020-09-25 16:31:01.000000 t4gpd-0.7.0/t4gpd/morph/STVoronoiPartition.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 10:00:08.000000 t4gpd-0.7.0/t4gpd/morph/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.371548 t4gpd-0.7.0/t4gpd/morph/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      941 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2895 2020-06-19 14:16:30.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AngularAbscissa.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1132 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4153 2023-01-30 15:34:51.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/AspectRatio.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1003 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/BBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1813 2023-02-14 11:19:09.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1996 2020-10-07 15:31:07.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1851 2020-12-18 22:37:53.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CircularityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      946 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexHull.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1917 2020-12-18 22:29:45.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1903 2022-11-07 14:15:37.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4022 2022-11-08 14:46:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5107 2023-02-20 08:57:36.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1136 2020-06-19 14:45:22.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/Diameter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2106 2020-12-30 20:08:51.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/EllipticityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3512 2022-07-22 14:38:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/FootprintExtruder.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1100 2021-06-21 13:53:15.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1227 2022-03-28 12:36:54.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/GridFace.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2283 2023-01-30 16:12:41.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/HMean.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2179 2023-01-30 14:29:24.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2481 2021-02-14 18:01:56.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1564 2023-01-30 13:38:38.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2342 2020-06-23 22:09:00.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABE.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      954 2020-06-18 08:03:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1067 2021-01-10 10:06:31.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1094 2020-12-15 16:02:50.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MBC.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1065 2020-12-15 20:28:55.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/MPBR.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1600 2020-12-30 20:09:13.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectangularityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1374 2022-11-08 14:46:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFFT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1749 2022-11-08 14:46:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFWT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1018 2020-06-19 07:17:45.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RemoveHoles.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1628 2022-06-24 16:06:35.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/RepresentativePoint.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1235 2021-04-26 14:02:10.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/Rotation2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2023-03-15 18:24:43.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/STGeoProcess.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3139 2023-01-30 13:39:08.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyMap2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2996 2023-01-30 15:49:55.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactor.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3657 2021-03-03 16:15:56.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1687 2022-01-18 09:14:29.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/StarShapedIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1898 2023-01-30 14:30:54.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/SurfaceFraction.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1978 2021-04-26 13:48:42.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/Translation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1792 2023-01-30 16:09:52.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/WMean.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-16 15:16:57.000000 t4gpd-0.7.0/t4gpd/morph/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/picoclim/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5476 2023-06-11 13:49:34.000000 t4gpd-0.7.0/t4gpd/picoclim/CampbellSciReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2312 2023-06-11 16:53:22.000000 t4gpd-0.7.0/t4gpd/picoclim/ExtraProcessing.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7497 2023-05-08 20:58:34.000000 t4gpd-0.7.0/t4gpd/picoclim/InertialMeasureReWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5574 2023-06-09 07:25:25.000000 t4gpd-0.7.0/t4gpd/picoclim/InertialMeasureReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3624 2023-03-22 16:43:01.000000 t4gpd-0.7.0/t4gpd/picoclim/JoinByTimeDistance.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6343 2023-06-09 07:11:48.000000 t4gpd-0.7.0/t4gpd/picoclim/KestrelReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2305 2022-10-26 10:49:53.000000 t4gpd-0.7.0/t4gpd/picoclim/MeteoFranceReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15062 2023-03-22 14:23:02.000000 t4gpd-0.7.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8963 2023-06-15 07:06:57.000000 t4gpd-0.7.0/t4gpd/picoclim/MetrologicalCampaignReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3314 2023-06-09 07:21:40.000000 t4gpd-0.7.0/t4gpd/picoclim/SensirionReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6589 2023-05-16 06:56:35.000000 t4gpd-0.7.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7288 2023-06-13 09:00:04.000000 t4gpd-0.7.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3531 2023-05-16 07:41:21.000000 t4gpd-0.7.0/t4gpd/picoclim/TracksWaypointsReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15960 2023-06-13 08:00:50.000000 t4gpd-0.7.0/t4gpd/picoclim/UClimGuidingReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2860 2023-06-13 08:14:48.000000 t4gpd-0.7.0/t4gpd/picoclim/UClimTrackWaypointsReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-09-15 08:50:25.000000 t4gpd-0.7.0/t4gpd/picoclim/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyplot/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4516 2022-11-07 14:14:25.000000 t4gpd-0.7.0/t4gpd/pyplot/MultipleMarkerStyles.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-01-31 17:29:02.000000 t4gpd-0.7.0/t4gpd/pyplot/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyqgis/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3438 2022-07-29 07:32:07.000000 t4gpd-0.7.0/t4gpd/pyqgis/AddMemoryLayer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1629 2022-07-27 20:17:41.000000 t4gpd-0.7.0/t4gpd/pyqgis/Emphasizer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8447 2022-07-10 14:41:36.000000 t4gpd-0.7.0/t4gpd/pyqgis/MapPrinter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5785 2021-09-10 17:42:22.000000 t4gpd-0.7.0/t4gpd/pyqgis/PdfMapWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    10441 2023-04-14 15:51:46.000000 t4gpd-0.7.0/t4gpd/pyqgis/SetSymbolLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1323 2021-09-10 16:28:27.000000 t4gpd-0.7.0/t4gpd/pyqgis/ShowFeatureCount.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1746 2021-09-24 09:47:44.000000 t4gpd-0.7.0/t4gpd/pyqgis/ZoomLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-09-09 16:49:22.000000 t4gpd-0.7.0/t4gpd/pyqgis/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyvista/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3711 2022-09-02 07:34:06.000000 t4gpd-0.7.0/t4gpd/pyvista/GeodeCiel.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4689 2022-09-01 16:13:45.000000 t4gpd-0.7.0/t4gpd/pyvista/Icosahedron.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8601 2023-06-26 13:48:29.000000 t4gpd-0.7.0/t4gpd/pyvista/Plotter3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2043 2022-06-22 15:52:10.000000 t4gpd-0.7.0/t4gpd/pyvista/STRaysToViewFactors.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3916 2022-06-05 15:29:14.000000 t4gpd-0.7.0/t4gpd/pyvista/ToPolyData.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4642 2022-09-25 09:28:13.000000 t4gpd-0.7.0/t4gpd/pyvista/ToUnstructuredGrid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-05 17:09:50.000000 t4gpd-0.7.0/t4gpd/pyvista/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyvista/commons/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1805 2022-09-05 12:42:46.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/Diameter3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8778 2022-09-01 16:15:11.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/RayCasting3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7389 2022-09-05 16:44:01.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8995 2022-09-07 10:57:40.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/SVF3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3683 2022-08-23 11:33:51.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/Triangle3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-05 21:07:30.000000 t4gpd-0.7.0/t4gpd/pyvista/commons/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3127 2022-07-18 15:37:08.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1398 2022-07-18 07:24:52.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1686 2022-06-22 16:23:38.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4679 2022-08-22 15:26:00.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4542 2022-08-24 08:46:07.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6047 2022-09-05 16:44:47.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3951 2022-09-05 16:45:02.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/SVF3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-09 11:51:20.000000 t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.375548 t4gpd-0.7.0/t4gpd/raster/
--rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)     2916 2022-06-01 18:54:37.000000 t4gpd-0.7.0/t4gpd/raster/STToRaster.py
--rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2022-06-01 12:59:39.000000 t4gpd-0.7.0/t4gpd/raster/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.379548 t4gpd-0.7.0/t4gpd/sun/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2021-04-22 15:43:22.000000 t4gpd-0.7.0/t4gpd/sun/AbstractHardShadow.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3176 2022-05-18 15:39:03.000000 t4gpd-0.7.0/t4gpd/sun/STHardShadow.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4002 2022-05-18 15:39:34.000000 t4gpd-0.7.0/t4gpd/sun/STSunMap2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3423 2022-05-18 15:44:21.000000 t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4353 2022-05-18 15:44:39.000000 t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:41:14.000000 t4gpd-0.7.0/t4gpd/sun/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.379548 t4gpd-0.7.0/t4gpd/sun/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2489 2021-04-21 16:17:23.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2218 2021-04-21 16:17:37.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDuration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4779 2021-04-21 16:17:58.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-03 15:05:24.000000 t4gpd-0.7.0/t4gpd/sun/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 08:41:41.335548 t4gpd-0.7.0/t4gpd.egg-info/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2545 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/PKG-INFO
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11205 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/SOURCES.txt
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        1 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/dependency_links.txt
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        6 2023-07-28 08:41:41.000000 t4gpd-0.7.0/t4gpd.egg-info/top_level.txt
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.397163 t4gpd-0.7.1/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    35149 2020-06-13 17:54:58.000000 t4gpd-0.7.1/LICENSE.txt
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2545 2023-07-28 09:25:50.397163 t4gpd-0.7.1/PKG-INFO
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1490 2023-07-28 09:15:27.000000 t4gpd-0.7.1/README.md
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      107 2023-07-28 09:25:50.397163 t4gpd-0.7.1/setup.cfg
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2141 2022-08-24 08:30:43.000000 t4gpd-0.7.1/setup.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.357163 t4gpd-0.7.1/t4gpd/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      739 2020-11-20 20:32:18.000000 t4gpd-0.7.1/t4gpd/__init__.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      804 2023-07-28 09:15:27.000000 t4gpd-0.7.1/t4gpd/_version.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.357163 t4gpd-0.7.1/t4gpd/comfort/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1492 2022-10-14 15:48:15.000000 t4gpd-0.7.1/t4gpd/comfort/EmpiricalThermalIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-17 12:41:51.000000 t4gpd-0.7.1/t4gpd/comfort/LinearThermalIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2478 2022-10-14 15:47:50.000000 t4gpd-0.7.1/t4gpd/comfort/UniversalThermalIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-02 17:38:35.000000 t4gpd-0.7.1/t4gpd/comfort/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.361163 t4gpd-0.7.1/t4gpd/comfort/algo/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5931 2021-05-12 17:04:21.000000 t4gpd-0.7.1/t4gpd/comfort/algo/CommonsLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4716 2021-05-12 16:38:39.000000 t4gpd-0.7.1/t4gpd/comfort/algo/ConstantsLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7079 2021-05-17 12:10:26.000000 t4gpd-0.7.1/t4gpd/comfort/algo/ETULib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1432 2021-05-12 16:42:17.000000 t4gpd-0.7.1/t4gpd/comfort/algo/PETLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1874 2021-09-02 09:59:31.000000 t4gpd-0.7.1/t4gpd/comfort/algo/PMVLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1714 2021-05-17 13:02:49.000000 t4gpd-0.7.1/t4gpd/comfort/algo/PTLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2066 2021-09-02 10:00:06.000000 t4gpd-0.7.1/t4gpd/comfort/algo/SETLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8302 2021-12-10 17:18:50.000000 t4gpd-0.7.1/t4gpd/comfort/algo/SET_mist.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1380 2021-05-12 08:12:54.000000 t4gpd-0.7.1/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-12 18:58:48.000000 t4gpd-0.7.1/t4gpd/comfort/algo/TmrtOutLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    17227 2022-10-24 09:23:00.000000 t4gpd-0.7.1/t4gpd/comfort/algo/UTCILib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13633 2021-02-04 21:08:03.000000 t4gpd-0.7.1/t4gpd/comfort/algo/VDI_PET_corrected.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1284 2022-10-24 09:21:44.000000 t4gpd-0.7.1/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-04 21:08:03.000000 t4gpd-0.7.1/t4gpd/comfort/algo/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.361163 t4gpd-0.7.1/t4gpd/comfort/indices/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2650 2022-10-14 15:46:56.000000 t4gpd-0.7.1/t4gpd/comfort/indices/ASV.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      876 2021-05-12 06:43:03.000000 t4gpd-0.7.1/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1980 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/DI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3216 2022-10-14 15:46:30.000000 t4gpd-0.7.1/t4gpd/comfort/indices/ETU.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2004 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/H.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2396 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/HI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2202 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/NET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2331 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/OUTSET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2037 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/PE.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3895 2023-06-16 15:01:43.000000 t4gpd-0.7.1/t4gpd/comfort/indices/PET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3088 2022-10-24 15:23:58.000000 t4gpd-0.7.1/t4gpd/comfort/indices/PMV.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2232 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/PT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2801 2022-10-24 15:23:09.000000 t4gpd-0.7.1/t4gpd/comfort/indices/SET.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3026 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/SETmist.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/THI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2223 2021-05-12 19:36:36.000000 t4gpd-0.7.1/t4gpd/comfort/indices/TmrtGlobeTemperature.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2178 2022-10-14 15:45:34.000000 t4gpd-0.7.1/t4gpd/comfort/indices/TmrtOut.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5838 2022-10-14 15:44:45.000000 t4gpd-0.7.1/t4gpd/comfort/indices/TmrtRadiometer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3953 2023-06-16 14:56:42.000000 t4gpd-0.7.1/t4gpd/comfort/indices/UTCI.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2660 2022-10-14 14:25:47.000000 t4gpd-0.7.1/t4gpd/comfort/indices/WCT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-05-11 16:27:08.000000 t4gpd-0.7.1/t4gpd/comfort/indices/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1608 2020-10-07 15:28:18.000000 t4gpd-0.7.1/t4gpd/commons/AngleLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1189 2021-01-07 07:59:17.000000 t4gpd-0.7.1/t4gpd/commons/ArrayCoding.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2308 2020-06-19 14:10:50.000000 t4gpd-0.7.1/t4gpd/commons/BoundingBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2366 2020-12-16 13:15:18.000000 t4gpd-0.7.1/t4gpd/commons/CSVLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1675 2021-07-01 09:32:35.000000 t4gpd-0.7.1/t4gpd/commons/CalendarLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7227 2021-06-16 14:25:07.000000 t4gpd-0.7.1/t4gpd/commons/CaliperLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      959 2020-10-02 12:26:10.000000 t4gpd-0.7.1/t4gpd/commons/Checksum.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4541 2020-12-15 16:02:11.000000 t4gpd-0.7.1/t4gpd/commons/ChrystalAlgorithm.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2023-06-24 06:23:57.000000 t4gpd-0.7.1/t4gpd/commons/ColorTemperature.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1637 2022-10-26 07:58:39.000000 t4gpd-0.7.1/t4gpd/commons/DataFrameLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2271 2022-08-24 10:23:43.000000 t4gpd-0.7.1/t4gpd/commons/DateRangeLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4956 2022-05-18 15:38:27.000000 t4gpd-0.7.1/t4gpd/commons/DatetimeLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1770 2022-09-05 10:36:15.000000 t4gpd-0.7.1/t4gpd/commons/DiameterLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5876 2020-06-22 09:32:49.000000 t4gpd-0.7.1/t4gpd/commons/Distances.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2831 2022-01-18 19:42:17.000000 t4gpd-0.7.1/t4gpd/commons/Entropy.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2832 2020-09-11 17:04:11.000000 t4gpd-0.7.1/t4gpd/commons/Epsilon.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1357 2022-10-25 14:40:11.000000 t4gpd-0.7.1/t4gpd/commons/GeoDataFrameLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1907 2021-05-18 08:44:20.000000 t4gpd-0.7.1/t4gpd/commons/GeoProcess.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25373 2023-02-15 21:10:56.000000 t4gpd-0.7.1/t4gpd/commons/GeomLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5407 2022-09-07 15:04:19.000000 t4gpd-0.7.1/t4gpd/commons/GeomLib3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4427 2022-03-28 12:35:37.000000 t4gpd-0.7.1/t4gpd/commons/GridFaceLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1149 2020-06-19 13:58:19.000000 t4gpd-0.7.1/t4gpd/commons/IllegalArgumentTypeException.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5933 2022-11-08 14:40:17.000000 t4gpd-0.7.1/t4gpd/commons/KernelLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3784 2020-10-24 09:49:18.000000 t4gpd-0.7.1/t4gpd/commons/LandoltRingLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2526 2022-03-08 14:24:54.000000 t4gpd-0.7.1/t4gpd/commons/LatLonLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2291 2021-04-12 07:38:42.000000 t4gpd-0.7.1/t4gpd/commons/LineStringCuttingLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1989 2020-10-11 20:51:06.000000 t4gpd-0.7.1/t4gpd/commons/ListUtilities.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5244 2022-06-02 10:16:48.000000 t4gpd-0.7.1/t4gpd/commons/Logos.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2108 2020-06-17 18:58:12.000000 t4gpd-0.7.1/t4gpd/commons/MyEdge.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2709 2020-09-24 09:53:56.000000 t4gpd-0.7.1/t4gpd/commons/MyNode.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8008 2022-06-13 13:36:47.000000 t4gpd-0.7.1/t4gpd/commons/PointsDensifierLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3137 2022-09-20 15:59:32.000000 t4gpd-0.7.1/t4gpd/commons/PointsDensifierLib3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2833 2020-06-22 09:34:45.000000 t4gpd-0.7.1/t4gpd/commons/PolarCartesianCoordinates.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13455 2023-01-30 13:37:02.000000 t4gpd-0.7.1/t4gpd/commons/RayCasting2Lib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13317 2023-02-16 10:09:06.000000 t4gpd-0.7.1/t4gpd/commons/RayCasting3Lib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11979 2023-07-27 19:53:59.000000 t4gpd-0.7.1/t4gpd/commons/RayCasting4Lib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11700 2023-02-20 09:15:16.000000 t4gpd-0.7.1/t4gpd/commons/RayCastingLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5638 2022-07-20 08:24:45.000000 t4gpd-0.7.1/t4gpd/commons/RotationLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2201 2022-04-08 14:27:04.000000 t4gpd-0.7.1/t4gpd/commons/SVFLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2307 2023-07-28 09:19:12.000000 t4gpd-0.7.1/t4gpd/commons/ShannonEntropy.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1308 2022-07-19 14:44:29.000000 t4gpd-0.7.1/t4gpd/commons/SphericalCartesianCoordinates.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4937 2022-09-20 16:03:36.000000 t4gpd-0.7.1/t4gpd/commons/SphericalProjectionLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1404 2021-06-08 21:34:17.000000 t4gpd-0.7.1/t4gpd/commons/TestUtils.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1502 2023-05-24 21:14:34.000000 t4gpd-0.7.1/t4gpd/commons/WarnUtils.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 09:59:56.000000 t4gpd-0.7.1/t4gpd/commons/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/crossroads_generation/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5464 2023-05-24 14:00:40.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_generation/Sequence.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2722 2023-05-23 14:00:27.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_generation/SequenceRadii.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3626 2022-11-07 10:44:48.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_generation/SequencesGeneration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 10:44:48.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_generation/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1860 2022-11-07 14:02:08.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/AbstractMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3791 2022-11-07 14:02:08.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1070 2022-11-07 14:02:08.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/FFTMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3228 2022-11-07 14:02:08.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/FWTMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2953 2022-11-07 14:02:08.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1160 2022-11-07 14:02:08.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 14:02:08.000000 t4gpd-0.7.1/t4gpd/commons/crossroads_identification/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/ellipse/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2020-08-31 08:21:22.000000 t4gpd-0.7.1/t4gpd/commons/ellipse/EllipseLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25237 2020-06-23 22:05:17.000000 t4gpd-0.7.1/t4gpd/commons/ellipse/EllipticHullLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-23 22:04:55.000000 t4gpd-0.7.1/t4gpd/commons/ellipse/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/graph/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6382 2021-03-24 08:57:48.000000 t4gpd-0.7.1/t4gpd/commons/graph/AbstractUrbanGraphLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4942 2023-01-27 17:52:06.000000 t4gpd-0.7.1/t4gpd/commons/graph/MCALib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4987 2020-11-23 09:56:15.000000 t4gpd-0.7.1/t4gpd/commons/graph/NeighborhoodLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2883 2020-11-23 09:55:51.000000 t4gpd-0.7.1/t4gpd/commons/graph/ShortestPathLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4289 2020-11-23 10:13:17.000000 t4gpd-0.7.1/t4gpd/commons/graph/UrbanGraphLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6322 2021-06-25 08:43:27.000000 t4gpd-0.7.1/t4gpd/commons/graph/UrbanGraphLibOld.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-21 18:40:43.000000 t4gpd-0.7.1/t4gpd/commons/graph/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/grid/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2298 2023-07-26 09:36:34.000000 t4gpd-0.7.1/t4gpd/commons/grid/AbstractGridLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6264 2023-02-17 15:49:30.000000 t4gpd-0.7.1/t4gpd/commons/grid/GridLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-04-09 08:07:33.000000 t4gpd-0.7.1/t4gpd/commons/grid/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/isovists/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-25 21:42:21.000000 t4gpd-0.7.1/t4gpd/commons/isovists/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/rnd/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4458 2023-05-23 15:30:11.000000 t4gpd-0.7.1/t4gpd/commons/rnd/RandomPointPicking.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2023-01-09 09:57:47.000000 t4gpd-0.7.1/t4gpd/commons/rnd/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.369162 t4gpd-0.7.1/t4gpd/commons/sun/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2774 2021-04-21 15:35:41.000000 t4gpd-0.7.1/t4gpd/commons/sun/AbstractSunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1441 2022-12-08 17:43:59.000000 t4gpd-0.7.1/t4gpd/commons/sun/DaylightLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1897 2021-06-01 20:45:53.000000 t4gpd-0.7.1/t4gpd/commons/sun/PySolarSunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7584 2021-04-22 16:07:47.000000 t4gpd-0.7.1/t4gpd/commons/sun/ShadowLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6719 2021-04-21 15:36:33.000000 t4gpd-0.7.1/t4gpd/commons/sun/SoleneSunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2429 2022-05-18 15:30:31.000000 t4gpd-0.7.1/t4gpd/commons/sun/SunBeamLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8335 2021-12-10 17:17:50.000000 t4gpd-0.7.1/t4gpd/commons/sun/SunLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-21 13:30:14.000000 t4gpd-0.7.1/t4gpd/commons/sun/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.377163 t4gpd-0.7.1/t4gpd/demos/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1113 2023-06-08 13:02:08.000000 t4gpd-0.7.1/t4gpd/demos/AbstractGeoDataFrameDemos.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   405923 2023-01-26 09:35:22.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)  1039604 2022-10-25 15:14:06.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   453528 2022-10-25 15:00:19.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos3.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)  2888649 2022-10-25 15:48:49.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos4.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   745426 2022-07-18 15:50:21.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos5.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435846 2022-10-26 14:52:50.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos6.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25686 2022-10-31 17:23:24.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos7.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435537 2022-10-31 17:22:15.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos8.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    87843 2023-03-22 16:19:10.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos9.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   274632 2023-04-27 15:51:16.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemosA.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   165333 2023-06-08 13:26:24.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemosB.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   193794 2023-06-08 13:03:08.000000 t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemosC.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-26 22:34:45.000000 t4gpd-0.7.1/t4gpd/demos/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.377163 t4gpd-0.7.1/t4gpd/energy/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12332 2022-04-28 15:33:51.000000 t4gpd-0.7.1/t4gpd/energy/DirectSolarIrradianceLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3194 2022-07-22 08:39:12.000000 t4gpd-0.7.1/t4gpd/energy/Dogniaux.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3035 2022-07-22 08:20:11.000000 t4gpd-0.7.1/t4gpd/energy/Perez.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1107 2022-07-22 08:20:39.000000 t4gpd-0.7.1/t4gpd/energy/Perraudeau.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3305 2022-07-22 08:21:55.000000 t4gpd-0.7.1/t4gpd/energy/PerrinDeBrichambaut.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3748 2022-07-22 08:40:41.000000 t4gpd-0.7.1/t4gpd/energy/PlotDirectNormalIrradiance.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:57:12.000000 t4gpd-0.7.1/t4gpd/energy/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.377163 t4gpd-0.7.1/t4gpd/energy/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4517 2022-05-18 17:36:24.000000 t4gpd-0.7.1/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-28 20:49:22.000000 t4gpd-0.7.1/t4gpd/energy/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.377163 t4gpd-0.7.1/t4gpd/graph/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1047 2020-12-31 14:32:10.000000 t4gpd-0.7.1/t4gpd/graph/STBetweennessCentrality.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1043 2020-12-19 20:28:37.000000 t4gpd-0.7.1/t4gpd/graph/STClosenessCentrality.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2657 2020-11-23 10:00:25.000000 t4gpd-0.7.1/t4gpd/graph/STRoadNeighborhood.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2459 2020-11-21 19:04:19.000000 t4gpd-0.7.1/t4gpd/graph/STShortestPath.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1644 2020-11-23 10:45:34.000000 t4gpd-0.7.1/t4gpd/graph/STToRoadsSections.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1474 2020-11-23 10:45:52.000000 t4gpd-0.7.1/t4gpd/graph/STToRoadsSectionsNodes.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 07:51:42.000000 t4gpd-0.7.1/t4gpd/graph/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.381163 t4gpd-0.7.1/t4gpd/io/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1120 2023-04-29 15:30:18.000000 t4gpd-0.7.1/t4gpd/io/AbstractReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4231 2020-09-24 09:56:55.000000 t4gpd-0.7.1/t4gpd/io/CSVInertialSensorReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1889 2020-09-24 09:57:20.000000 t4gpd-0.7.1/t4gpd/io/CSVReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1884 2021-03-10 14:24:32.000000 t4gpd-0.7.1/t4gpd/io/CSVWKTReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2317 2021-03-10 14:24:47.000000 t4gpd-0.7.1/t4gpd/io/CSVWKTWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3373 2022-07-25 09:09:50.000000 t4gpd-0.7.1/t4gpd/io/CirReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1314 2022-07-25 09:34:22.000000 t4gpd-0.7.1/t4gpd/io/CirValReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3331 2021-03-10 21:07:26.000000 t4gpd-0.7.1/t4gpd/io/CirWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5578 2020-10-22 16:39:22.000000 t4gpd-0.7.1/t4gpd/io/CityGMLReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7156 2022-06-24 16:06:01.000000 t4gpd-0.7.1/t4gpd/io/GeoWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1829 2022-11-09 15:42:30.000000 t4gpd-0.7.1/t4gpd/io/GpkgLoader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1818 2022-11-09 15:42:30.000000 t4gpd-0.7.1/t4gpd/io/GpkgWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12097 2021-06-25 08:29:09.000000 t4gpd-0.7.1/t4gpd/io/MshReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3750 2020-08-25 16:50:36.000000 t4gpd-0.7.1/t4gpd/io/ObjReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3541 2021-02-01 10:43:14.000000 t4gpd-0.7.1/t4gpd/io/ObjWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1430 2021-07-19 15:31:30.000000 t4gpd-0.7.1/t4gpd/io/Reloading.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1152 2022-04-26 12:38:58.000000 t4gpd-0.7.1/t4gpd/io/STLoadAndClip.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3086 2020-06-19 14:12:42.000000 t4gpd-0.7.1/t4gpd/io/SVGWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5130 2022-07-26 12:53:22.000000 t4gpd-0.7.1/t4gpd/io/SalomeWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5030 2022-07-26 12:53:22.000000 t4gpd-0.7.1/t4gpd/io/SalomeWriterAndExtruder.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6490 2021-03-10 14:25:07.000000 t4gpd-0.7.1/t4gpd/io/VTUWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2492 2022-07-25 09:33:33.000000 t4gpd-0.7.1/t4gpd/io/ValReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2806 2021-11-08 15:20:17.000000 t4gpd-0.7.1/t4gpd/io/ZipLoader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3559 2021-10-18 16:00:12.000000 t4gpd-0.7.1/t4gpd/io/ZipWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 18:59:50.000000 t4gpd-0.7.1/t4gpd/io/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.381163 t4gpd-0.7.1/t4gpd/isovist/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4347 2022-07-27 15:30:51.000000 t4gpd-0.7.1/t4gpd/isovist/STIsovistField2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4697 2023-07-27 17:24:29.000000 t4gpd-0.7.1/t4gpd/isovist/STIsovistField2D_new.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 09:56:41.000000 t4gpd-0.7.1/t4gpd/isovist/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.385162 t4gpd-0.7.1/t4gpd/misc/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4972 2021-07-20 15:59:02.000000 t4gpd-0.7.1/t4gpd/misc/FrequencyHistogram.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5748 2023-03-23 17:02:07.000000 t4gpd-0.7.1/t4gpd/misc/OptimalNumberOfClusters.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5344 2021-11-14 15:44:04.000000 t4gpd-0.7.1/t4gpd/misc/PlotAMatrixOfDiagrams.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2960 2021-10-01 15:35:34.000000 t4gpd-0.7.1/t4gpd/misc/PopulationPyramid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5500 2023-01-19 10:23:40.000000 t4gpd-0.7.1/t4gpd/misc/RoseMappingTool.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3038 2022-03-15 16:20:31.000000 t4gpd-0.7.1/t4gpd/misc/STCompass.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2311 2023-03-23 14:05:55.000000 t4gpd-0.7.1/t4gpd/misc/STDendrogram.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2023-03-23 16:15:02.000000 t4gpd-0.7.1/t4gpd/misc/STKMeans.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4364 2021-01-25 16:17:15.000000 t4gpd-0.7.1/t4gpd/misc/StreetOrientationHistogram.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4386 2022-12-13 18:08:58.000000 t4gpd-0.7.1/t4gpd/misc/TimelineTool.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2824 2021-03-15 16:13:35.000000 t4gpd-0.7.1/t4gpd/misc/WindRose.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-09-29 10:07:30.000000 t4gpd-0.7.1/t4gpd/misc/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.385162 t4gpd-0.7.1/t4gpd/morph/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2873 2021-08-25 16:19:57.000000 t4gpd-0.7.1/t4gpd/morph/GmshTriangulator.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1413 2023-02-17 18:32:38.000000 t4gpd-0.7.1/t4gpd/morph/STBBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1793 2020-06-30 09:46:17.000000 t4gpd-0.7.1/t4gpd/morph/STClip.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4603 2022-08-24 09:39:40.000000 t4gpd-0.7.1/t4gpd/morph/STCoolscapesTessellation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2723 2023-05-23 14:01:31.000000 t4gpd-0.7.1/t4gpd/morph/STCrossroadsGeneration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2853 2023-02-14 11:31:50.000000 t4gpd-0.7.1/t4gpd/morph/STDilationErosion.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2103 2020-12-14 16:55:46.000000 t4gpd-0.7.1/t4gpd/morph/STExtractOpenSpaces.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3726 2021-04-02 09:43:35.000000 t4gpd-0.7.1/t4gpd/morph/STFacadesAnalysis.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8594 2023-02-20 08:30:55.000000 t4gpd-0.7.1/t4gpd/morph/STGradientOfDistancesToBuildings.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2043 2023-07-26 10:17:45.000000 t4gpd-0.7.1/t4gpd/morph/STGrid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3688 2020-09-17 11:02:43.000000 t4gpd-0.7.1/t4gpd/morph/STIdentifyRowOfTrees.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4480 2021-12-09 14:49:10.000000 t4gpd-0.7.1/t4gpd/morph/STMakeBlocks.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1701 2023-06-07 10:51:36.000000 t4gpd-0.7.1/t4gpd/morph/STMakeGroundSurface.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2812 2020-09-21 14:15:12.000000 t4gpd-0.7.1/t4gpd/morph/STMultipleOverlaps.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4550 2023-02-20 08:36:37.000000 t4gpd-0.7.1/t4gpd/morph/STMultipleOverlaps2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3134 2022-06-13 13:37:40.000000 t4gpd-0.7.1/t4gpd/morph/STPointsDensifier.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2118 2022-06-13 13:11:05.000000 t4gpd-0.7.1/t4gpd/morph/STPointsDensifier2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1717 2020-12-31 16:03:16.000000 t4gpd-0.7.1/t4gpd/morph/STPolygonize.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3105 2023-02-15 17:59:34.000000 t4gpd-0.7.1/t4gpd/morph/STSkeletonize.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2294 2023-02-15 20:25:15.000000 t4gpd-0.7.1/t4gpd/morph/STSkeletonizeTheVoid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6054 2023-07-27 20:19:56.000000 t4gpd-0.7.1/t4gpd/morph/STSkyMap25D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3196 2020-09-24 10:27:56.000000 t4gpd-0.7.1/t4gpd/morph/STSnappingPointsOnLines.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6567 2022-08-24 09:55:25.000000 t4gpd-0.7.1/t4gpd/morph/STSnappingPointsOnLines2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3217 2021-05-18 08:45:03.000000 t4gpd-0.7.1/t4gpd/morph/STSpatialJoin.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1568 2022-10-14 10:00:03.000000 t4gpd-0.7.1/t4gpd/morph/STSquaredBBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2628 2023-01-31 10:54:56.000000 t4gpd-0.7.1/t4gpd/morph/STVariableWidthBuffer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3729 2020-09-25 16:31:01.000000 t4gpd-0.7.1/t4gpd/morph/STVoronoiPartition.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 10:00:08.000000 t4gpd-0.7.1/t4gpd/morph/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.389162 t4gpd-0.7.1/t4gpd/morph/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      941 2020-06-18 08:03:10.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2895 2020-06-19 14:16:30.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/AngularAbscissa.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1132 2020-06-18 08:03:10.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4153 2023-01-30 15:34:51.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/AspectRatio.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1003 2020-06-18 08:03:10.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/BBox.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1813 2023-02-14 11:19:09.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1996 2020-10-07 15:31:07.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1851 2020-12-18 22:37:53.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/CircularityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      946 2020-06-18 08:03:10.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/ConvexHull.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1917 2020-12-18 22:29:45.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/ConvexityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1903 2022-11-07 14:15:37.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/CrossroadRecognition.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4022 2022-11-08 14:46:29.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5107 2023-02-20 08:57:36.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1136 2020-06-19 14:45:22.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/Diameter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2106 2020-12-30 20:08:51.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/EllipticityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3512 2022-07-22 14:38:29.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/FootprintExtruder.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1100 2021-06-21 13:53:15.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/GetInteriorPoint.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1227 2022-03-28 12:36:54.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/GridFace.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2283 2023-01-30 16:12:41.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/HMean.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2179 2023-01-30 14:29:24.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/HeightOfRoughness.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2481 2021-02-14 18:01:56.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1564 2023-01-30 13:38:38.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2342 2020-06-23 22:09:00.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/MABE.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      954 2020-06-18 08:03:10.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/MABR.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1067 2021-01-10 10:06:31.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/MABR2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1094 2020-12-15 16:02:50.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/MBC.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1065 2020-12-15 20:28:55.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/MPBR.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1600 2020-12-30 20:09:13.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/RectangularityIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1374 2022-11-08 14:46:29.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/RectifyByFFT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1749 2022-11-08 14:46:29.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/RectifyByFWT.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1018 2020-06-19 07:17:45.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/RemoveHoles.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1628 2022-06-24 16:06:35.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/RepresentativePoint.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1235 2021-04-26 14:02:10.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/Rotation2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2023-03-15 18:24:43.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/STGeoProcess.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3139 2023-01-30 13:39:08.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/SkyMap2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2996 2023-01-30 15:49:55.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/SkyViewFactor.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3657 2021-03-03 16:15:56.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1687 2022-01-18 09:14:29.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/StarShapedIndices.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1898 2023-01-30 14:30:54.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/SurfaceFraction.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1978 2021-04-26 13:48:42.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/Translation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1792 2023-01-30 16:09:52.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/WMean.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-16 15:16:57.000000 t4gpd-0.7.1/t4gpd/morph/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.393162 t4gpd-0.7.1/t4gpd/picoclim/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5476 2023-06-11 13:49:34.000000 t4gpd-0.7.1/t4gpd/picoclim/CampbellSciReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2312 2023-06-11 16:53:22.000000 t4gpd-0.7.1/t4gpd/picoclim/ExtraProcessing.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7497 2023-05-08 20:58:34.000000 t4gpd-0.7.1/t4gpd/picoclim/InertialMeasureReWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5574 2023-06-09 07:25:25.000000 t4gpd-0.7.1/t4gpd/picoclim/InertialMeasureReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3624 2023-03-22 16:43:01.000000 t4gpd-0.7.1/t4gpd/picoclim/JoinByTimeDistance.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6343 2023-06-09 07:11:48.000000 t4gpd-0.7.1/t4gpd/picoclim/KestrelReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2305 2022-10-26 10:49:53.000000 t4gpd-0.7.1/t4gpd/picoclim/MeteoFranceReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15062 2023-03-22 14:23:02.000000 t4gpd-0.7.1/t4gpd/picoclim/MetrologicalCampaignPlottings.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8963 2023-06-15 07:06:57.000000 t4gpd-0.7.1/t4gpd/picoclim/MetrologicalCampaignReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3314 2023-06-09 07:21:40.000000 t4gpd-0.7.1/t4gpd/picoclim/SensirionReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6589 2023-05-16 06:56:35.000000 t4gpd-0.7.1/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7288 2023-06-13 09:00:04.000000 t4gpd-0.7.1/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3531 2023-05-16 07:41:21.000000 t4gpd-0.7.1/t4gpd/picoclim/TracksWaypointsReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15960 2023-06-13 08:00:50.000000 t4gpd-0.7.1/t4gpd/picoclim/UClimGuidingReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2860 2023-06-13 08:14:48.000000 t4gpd-0.7.1/t4gpd/picoclim/UClimTrackWaypointsReader.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-09-15 08:50:25.000000 t4gpd-0.7.1/t4gpd/picoclim/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.393162 t4gpd-0.7.1/t4gpd/pyplot/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4516 2022-11-07 14:14:25.000000 t4gpd-0.7.1/t4gpd/pyplot/MultipleMarkerStyles.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-01-31 17:29:02.000000 t4gpd-0.7.1/t4gpd/pyplot/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.393162 t4gpd-0.7.1/t4gpd/pyqgis/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3438 2022-07-29 07:32:07.000000 t4gpd-0.7.1/t4gpd/pyqgis/AddMemoryLayer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1629 2022-07-27 20:17:41.000000 t4gpd-0.7.1/t4gpd/pyqgis/Emphasizer.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8447 2022-07-10 14:41:36.000000 t4gpd-0.7.1/t4gpd/pyqgis/MapPrinter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5785 2023-07-28 09:19:12.000000 t4gpd-0.7.1/t4gpd/pyqgis/PdfMapWriter.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    10441 2023-04-14 15:51:46.000000 t4gpd-0.7.1/t4gpd/pyqgis/SetSymbolLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1323 2021-09-10 16:28:27.000000 t4gpd-0.7.1/t4gpd/pyqgis/ShowFeatureCount.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1746 2021-09-24 09:47:44.000000 t4gpd-0.7.1/t4gpd/pyqgis/ZoomLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-09-09 16:49:22.000000 t4gpd-0.7.1/t4gpd/pyqgis/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.393162 t4gpd-0.7.1/t4gpd/pyvista/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3711 2022-09-02 07:34:06.000000 t4gpd-0.7.1/t4gpd/pyvista/GeodeCiel.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4689 2022-09-01 16:13:45.000000 t4gpd-0.7.1/t4gpd/pyvista/Icosahedron.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8601 2023-06-26 13:48:29.000000 t4gpd-0.7.1/t4gpd/pyvista/Plotter3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2043 2022-06-22 15:52:10.000000 t4gpd-0.7.1/t4gpd/pyvista/STRaysToViewFactors.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3916 2022-06-05 15:29:14.000000 t4gpd-0.7.1/t4gpd/pyvista/ToPolyData.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4642 2022-09-25 09:28:13.000000 t4gpd-0.7.1/t4gpd/pyvista/ToUnstructuredGrid.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-05 17:09:50.000000 t4gpd-0.7.1/t4gpd/pyvista/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.393162 t4gpd-0.7.1/t4gpd/pyvista/commons/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1805 2022-09-05 12:42:46.000000 t4gpd-0.7.1/t4gpd/pyvista/commons/Diameter3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8778 2022-09-01 16:15:11.000000 t4gpd-0.7.1/t4gpd/pyvista/commons/RayCasting3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7389 2022-09-05 16:44:01.000000 t4gpd-0.7.1/t4gpd/pyvista/commons/RayCastingIn3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8995 2022-09-07 10:57:40.000000 t4gpd-0.7.1/t4gpd/pyvista/commons/SVF3DLib.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3683 2022-08-23 11:33:51.000000 t4gpd-0.7.1/t4gpd/pyvista/commons/Triangle3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-05 21:07:30.000000 t4gpd-0.7.1/t4gpd/pyvista/commons/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.397163 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3127 2022-07-18 15:37:08.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1398 2022-07-18 07:24:52.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1686 2022-06-22 16:23:38.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4679 2022-08-22 15:26:00.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4542 2022-08-24 08:46:07.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6047 2022-09-05 16:44:47.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/RayCasting3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3951 2022-09-05 16:45:02.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/SVF3D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-09 11:51:20.000000 t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.397163 t4gpd-0.7.1/t4gpd/raster/
+-rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)     2916 2022-06-01 18:54:37.000000 t4gpd-0.7.1/t4gpd/raster/STToRaster.py
+-rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2022-06-01 12:59:39.000000 t4gpd-0.7.1/t4gpd/raster/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.397163 t4gpd-0.7.1/t4gpd/sun/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2021-04-22 15:43:22.000000 t4gpd-0.7.1/t4gpd/sun/AbstractHardShadow.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3176 2022-05-18 15:39:03.000000 t4gpd-0.7.1/t4gpd/sun/STHardShadow.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4002 2022-05-18 15:39:34.000000 t4gpd-0.7.1/t4gpd/sun/STSunMap2D.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3423 2022-05-18 15:44:21.000000 t4gpd-0.7.1/t4gpd/sun/STTreeHardShadow.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4353 2022-05-18 15:44:39.000000 t4gpd-0.7.1/t4gpd/sun/STTreeHardShadow2.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:41:14.000000 t4gpd-0.7.1/t4gpd/sun/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.397163 t4gpd-0.7.1/t4gpd/sun/geoProcesses/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2489 2021-04-21 16:17:23.000000 t4gpd-0.7.1/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2218 2021-04-21 16:17:37.000000 t4gpd-0.7.1/t4gpd/sun/geoProcesses/SunshineDuration.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4779 2021-04-21 16:17:58.000000 t4gpd-0.7.1/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-03 15:05:24.000000 t4gpd-0.7.1/t4gpd/sun/geoProcesses/__init__.py
+drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-07-28 09:25:50.357163 t4gpd-0.7.1/t4gpd.egg-info/
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2545 2023-07-28 09:25:50.000000 t4gpd-0.7.1/t4gpd.egg-info/PKG-INFO
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11205 2023-07-28 09:25:50.000000 t4gpd-0.7.1/t4gpd.egg-info/SOURCES.txt
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        1 2023-07-28 09:25:50.000000 t4gpd-0.7.1/t4gpd.egg-info/dependency_links.txt
+-rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        6 2023-07-28 09:25:50.000000 t4gpd-0.7.1/t4gpd.egg-info/top_level.txt
```

### Comparing `t4gpd-0.7.0/LICENSE.txt` & `t4gpd-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/PKG-INFO` & `t4gpd-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.7.0
+Version: 0.7.1
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
 Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
@@ -42,14 +42,14 @@
 > pip install Dijkstar suntimes pythermalcomfort
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-> pip install t4gpd-0.6.0.tar.gz
+> pip install t4gpd-0.7.1.tar.gz
 
 ## Read the documentation
 Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
```

### Comparing `t4gpd-0.7.0/README.md` & `t4gpd-0.7.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 > pip install Dijkstar suntimes pythermalcomfort
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-> pip install t4gpd-0.6.0.tar.gz
+> pip install t4gpd-0.7.1.tar.gz
 
 ## Read the documentation
 Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
```

### Comparing `t4gpd-0.7.0/setup.py` & `t4gpd-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/__init__.py` & `t4gpd-0.7.1/t4gpd/__init__.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/_version.py` & `t4gpd-0.7.1/t4gpd/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 # The following line *must* be the last in the module, exactly as formatted:
-__version__ = '0.7.0'
+__version__ = '0.7.1'
```

### Comparing `t4gpd-0.7.0/t4gpd/comfort/EmpiricalThermalIndices.py` & `t4gpd-0.7.1/t4gpd/comfort/EmpiricalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/LinearThermalIndices.py` & `t4gpd-0.7.1/t4gpd/comfort/LinearThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/UniversalThermalIndices.py` & `t4gpd-0.7.1/t4gpd/comfort/UniversalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/CommonsLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/CommonsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/ConstantsLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/ConstantsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/ETULib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/ETULib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/PETLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/PETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/PMVLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/PMVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/PTLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/PTLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/SETLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/SETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/SET_mist.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/SET_mist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/TmrtOutLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/TmrtOutLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/UTCILib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/UTCILib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/VDI_PET_corrected.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/VDI_PET_corrected.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py` & `t4gpd-0.7.1/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/ASV.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/ASV.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/AbstractThermalComfortIndice.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/DI.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/DI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/ETU.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/ETU.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/H.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/H.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/HI.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/HI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/NET.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/NET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/OUTSET.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/OUTSET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/PE.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/PE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/PET.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/PET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/PMV.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/PMV.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/PT.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/PT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/SET.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/SET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/SETmist.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/SETmist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/THI.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/THI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/TmrtGlobeTemperature.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/TmrtOut.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/TmrtOut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/TmrtRadiometer.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/TmrtRadiometer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/UTCI.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/UTCI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/comfort/indices/WCT.py` & `t4gpd-0.7.1/t4gpd/comfort/indices/WCT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/AngleLib.py` & `t4gpd-0.7.1/t4gpd/commons/AngleLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/ArrayCoding.py` & `t4gpd-0.7.1/t4gpd/commons/ArrayCoding.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/BoundingBox.py` & `t4gpd-0.7.1/t4gpd/commons/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/CSVLib.py` & `t4gpd-0.7.1/t4gpd/commons/CSVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/CalendarLib.py` & `t4gpd-0.7.1/t4gpd/commons/CalendarLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/CaliperLib.py` & `t4gpd-0.7.1/t4gpd/commons/CaliperLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/Checksum.py` & `t4gpd-0.7.1/t4gpd/commons/Checksum.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/ChrystalAlgorithm.py` & `t4gpd-0.7.1/t4gpd/commons/ChrystalAlgorithm.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/ColorTemperature.py` & `t4gpd-0.7.1/t4gpd/commons/ColorTemperature.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/DataFrameLib.py` & `t4gpd-0.7.1/t4gpd/commons/DataFrameLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/DateRangeLib.py` & `t4gpd-0.7.1/t4gpd/commons/DateRangeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/DatetimeLib.py` & `t4gpd-0.7.1/t4gpd/commons/DatetimeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/DiameterLib.py` & `t4gpd-0.7.1/t4gpd/commons/DiameterLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/Distances.py` & `t4gpd-0.7.1/t4gpd/commons/Distances.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/Entropy.py` & `t4gpd-0.7.1/t4gpd/commons/Entropy.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/Epsilon.py` & `t4gpd-0.7.1/t4gpd/commons/Epsilon.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/GeoDataFrameLib.py` & `t4gpd-0.7.1/t4gpd/commons/GeoDataFrameLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/GeoProcess.py` & `t4gpd-0.7.1/t4gpd/commons/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/GeomLib.py` & `t4gpd-0.7.1/t4gpd/commons/GeomLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/GeomLib3D.py` & `t4gpd-0.7.1/t4gpd/commons/GeomLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/GridFaceLib.py` & `t4gpd-0.7.1/t4gpd/commons/GridFaceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/IllegalArgumentTypeException.py` & `t4gpd-0.7.1/t4gpd/commons/IllegalArgumentTypeException.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/KernelLib.py` & `t4gpd-0.7.1/t4gpd/commons/KernelLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/LandoltRingLib.py` & `t4gpd-0.7.1/t4gpd/commons/LandoltRingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/LatLonLib.py` & `t4gpd-0.7.1/t4gpd/commons/LatLonLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/LineStringCuttingLib.py` & `t4gpd-0.7.1/t4gpd/commons/LineStringCuttingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/ListUtilities.py` & `t4gpd-0.7.1/t4gpd/commons/ListUtilities.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/Logos.py` & `t4gpd-0.7.1/t4gpd/commons/Logos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/MyEdge.py` & `t4gpd-0.7.1/t4gpd/commons/MyEdge.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/MyNode.py` & `t4gpd-0.7.1/t4gpd/commons/MyNode.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib.py` & `t4gpd-0.7.1/t4gpd/commons/PointsDensifierLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/PointsDensifierLib3D.py` & `t4gpd-0.7.1/t4gpd/commons/PointsDensifierLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/PolarCartesianCoordinates.py` & `t4gpd-0.7.1/t4gpd/commons/PolarCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/RayCasting2Lib.py` & `t4gpd-0.7.1/t4gpd/commons/RayCasting2Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/RayCasting3Lib.py` & `t4gpd-0.7.1/t4gpd/commons/RayCasting3Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/RayCasting4Lib.py` & `t4gpd-0.7.1/t4gpd/commons/RayCasting4Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/RayCastingLib.py` & `t4gpd-0.7.1/t4gpd/commons/RayCastingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/RotationLib.py` & `t4gpd-0.7.1/t4gpd/commons/RotationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/SVFLib.py` & `t4gpd-0.7.1/t4gpd/commons/SVFLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/ShannonEntropy.py` & `t4gpd-0.7.1/t4gpd/commons/ShannonEntropy.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/SphericalCartesianCoordinates.py` & `t4gpd-0.7.1/t4gpd/commons/SphericalCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/SphericalProjectionLib.py` & `t4gpd-0.7.1/t4gpd/commons/SphericalProjectionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/TestUtils.py` & `t4gpd-0.7.1/t4gpd/commons/TestUtils.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/WarnUtils.py` & `t4gpd-0.7.1/t4gpd/commons/WarnUtils.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_generation/Sequence.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_generation/Sequence.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_generation/SequenceRadii.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_generation/SequenceRadii.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_generation/SequencesGeneration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/AbstractMethod.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_identification/AbstractMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FFTMethod.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_identification/FFTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/FWTMethod.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_identification/FWTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py` & `t4gpd-0.7.1/t4gpd/commons/crossroads_identification/MeanVectorMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/ellipse/EllipseLib.py` & `t4gpd-0.7.1/t4gpd/commons/ellipse/EllipseLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/ellipse/EllipticHullLib.py` & `t4gpd-0.7.1/t4gpd/commons/ellipse/EllipticHullLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py` & `t4gpd-0.7.1/t4gpd/commons/graph/AbstractUrbanGraphLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/graph/MCALib.py` & `t4gpd-0.7.1/t4gpd/commons/graph/MCALib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/graph/NeighborhoodLib.py` & `t4gpd-0.7.1/t4gpd/commons/graph/NeighborhoodLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/graph/ShortestPathLib.py` & `t4gpd-0.7.1/t4gpd/commons/graph/ShortestPathLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLib.py` & `t4gpd-0.7.1/t4gpd/commons/graph/UrbanGraphLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/graph/UrbanGraphLibOld.py` & `t4gpd-0.7.1/t4gpd/commons/graph/UrbanGraphLibOld.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/grid/AbstractGridLib.py` & `t4gpd-0.7.1/t4gpd/commons/grid/AbstractGridLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/grid/GridLib.py` & `t4gpd-0.7.1/t4gpd/commons/grid/GridLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/rnd/RandomPointPicking.py` & `t4gpd-0.7.1/t4gpd/commons/rnd/RandomPointPicking.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/sun/AbstractSunLib.py` & `t4gpd-0.7.1/t4gpd/commons/sun/AbstractSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/sun/DaylightLib.py` & `t4gpd-0.7.1/t4gpd/commons/sun/DaylightLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/sun/PySolarSunLib.py` & `t4gpd-0.7.1/t4gpd/commons/sun/PySolarSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/sun/ShadowLib.py` & `t4gpd-0.7.1/t4gpd/commons/sun/ShadowLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/sun/SoleneSunLib.py` & `t4gpd-0.7.1/t4gpd/commons/sun/SoleneSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/sun/SunBeamLib.py` & `t4gpd-0.7.1/t4gpd/commons/sun/SunBeamLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/commons/sun/SunLib.py` & `t4gpd-0.7.1/t4gpd/commons/sun/SunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/AbstractGeoDataFrameDemos.py` & `t4gpd-0.7.1/t4gpd/demos/AbstractGeoDataFrameDemos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos2.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos3.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos4.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos4.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos5.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos5.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos6.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos6.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos7.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos7.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos8.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos8.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemos9.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemos9.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosA.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemosA.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosB.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemosB.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/demos/GeoDataFrameDemosC.py` & `t4gpd-0.7.1/t4gpd/demos/GeoDataFrameDemosC.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/energy/DirectSolarIrradianceLib.py` & `t4gpd-0.7.1/t4gpd/energy/DirectSolarIrradianceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/energy/Dogniaux.py` & `t4gpd-0.7.1/t4gpd/energy/Dogniaux.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/energy/Perez.py` & `t4gpd-0.7.1/t4gpd/energy/Perez.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/energy/Perraudeau.py` & `t4gpd-0.7.1/t4gpd/energy/Perraudeau.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/energy/PerrinDeBrichambaut.py` & `t4gpd-0.7.1/t4gpd/energy/PerrinDeBrichambaut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/energy/PlotDirectNormalIrradiance.py` & `t4gpd-0.7.1/t4gpd/energy/PlotDirectNormalIrradiance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py` & `t4gpd-0.7.1/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/graph/STBetweennessCentrality.py` & `t4gpd-0.7.1/t4gpd/graph/STBetweennessCentrality.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/graph/STClosenessCentrality.py` & `t4gpd-0.7.1/t4gpd/graph/STClosenessCentrality.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/graph/STRoadNeighborhood.py` & `t4gpd-0.7.1/t4gpd/graph/STRoadNeighborhood.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/graph/STShortestPath.py` & `t4gpd-0.7.1/t4gpd/graph/STShortestPath.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/graph/STToRoadsSections.py` & `t4gpd-0.7.1/t4gpd/graph/STToRoadsSections.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/graph/STToRoadsSectionsNodes.py` & `t4gpd-0.7.1/t4gpd/graph/STToRoadsSectionsNodes.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/AbstractReader.py` & `t4gpd-0.7.1/t4gpd/io/AbstractReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CSVInertialSensorReader.py` & `t4gpd-0.7.1/t4gpd/io/CSVInertialSensorReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CSVReader.py` & `t4gpd-0.7.1/t4gpd/io/CSVReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CSVWKTReader.py` & `t4gpd-0.7.1/t4gpd/io/CSVWKTReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CSVWKTWriter.py` & `t4gpd-0.7.1/t4gpd/io/CSVWKTWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CirReader.py` & `t4gpd-0.7.1/t4gpd/io/CirReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CirValReader.py` & `t4gpd-0.7.1/t4gpd/io/CirValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CirWriter.py` & `t4gpd-0.7.1/t4gpd/io/CirWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/CityGMLReader.py` & `t4gpd-0.7.1/t4gpd/io/CityGMLReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/GeoWriter.py` & `t4gpd-0.7.1/t4gpd/io/GeoWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/GpkgLoader.py` & `t4gpd-0.7.1/t4gpd/io/GpkgLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/GpkgWriter.py` & `t4gpd-0.7.1/t4gpd/io/GpkgWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/MshReader.py` & `t4gpd-0.7.1/t4gpd/io/MshReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/ObjReader.py` & `t4gpd-0.7.1/t4gpd/io/ObjReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/ObjWriter.py` & `t4gpd-0.7.1/t4gpd/io/ObjWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/Reloading.py` & `t4gpd-0.7.1/t4gpd/io/Reloading.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/STLoadAndClip.py` & `t4gpd-0.7.1/t4gpd/io/STLoadAndClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/SVGWriter.py` & `t4gpd-0.7.1/t4gpd/io/SVGWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/SalomeWriter.py` & `t4gpd-0.7.1/t4gpd/io/SalomeWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/SalomeWriterAndExtruder.py` & `t4gpd-0.7.1/t4gpd/io/SalomeWriterAndExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/VTUWriter.py` & `t4gpd-0.7.1/t4gpd/io/VTUWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/ValReader.py` & `t4gpd-0.7.1/t4gpd/io/ValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/ZipLoader.py` & `t4gpd-0.7.1/t4gpd/io/ZipLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/io/ZipWriter.py` & `t4gpd-0.7.1/t4gpd/io/ZipWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/isovist/STIsovistField2D.py` & `t4gpd-0.7.1/t4gpd/isovist/STIsovistField2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/isovist/STIsovistField2D_new.py` & `t4gpd-0.7.1/t4gpd/isovist/STIsovistField2D_new.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/FrequencyHistogram.py` & `t4gpd-0.7.1/t4gpd/misc/FrequencyHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/OptimalNumberOfClusters.py` & `t4gpd-0.7.1/t4gpd/misc/OptimalNumberOfClusters.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/PlotAMatrixOfDiagrams.py` & `t4gpd-0.7.1/t4gpd/misc/PlotAMatrixOfDiagrams.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/PopulationPyramid.py` & `t4gpd-0.7.1/t4gpd/misc/PopulationPyramid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/RoseMappingTool.py` & `t4gpd-0.7.1/t4gpd/misc/RoseMappingTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/STCompass.py` & `t4gpd-0.7.1/t4gpd/misc/STCompass.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/STDendrogram.py` & `t4gpd-0.7.1/t4gpd/misc/STDendrogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/STKMeans.py` & `t4gpd-0.7.1/t4gpd/misc/STKMeans.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/StreetOrientationHistogram.py` & `t4gpd-0.7.1/t4gpd/misc/StreetOrientationHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/TimelineTool.py` & `t4gpd-0.7.1/t4gpd/misc/TimelineTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/misc/WindRose.py` & `t4gpd-0.7.1/t4gpd/misc/WindRose.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/GmshTriangulator.py` & `t4gpd-0.7.1/t4gpd/morph/GmshTriangulator.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STBBox.py` & `t4gpd-0.7.1/t4gpd/morph/STBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STClip.py` & `t4gpd-0.7.1/t4gpd/morph/STClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STCoolscapesTessellation.py` & `t4gpd-0.7.1/t4gpd/morph/STCoolscapesTessellation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STCrossroadsGeneration.py` & `t4gpd-0.7.1/t4gpd/morph/STCrossroadsGeneration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STDilationErosion.py` & `t4gpd-0.7.1/t4gpd/morph/STDilationErosion.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STExtractOpenSpaces.py` & `t4gpd-0.7.1/t4gpd/morph/STExtractOpenSpaces.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STFacadesAnalysis.py` & `t4gpd-0.7.1/t4gpd/morph/STFacadesAnalysis.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STGradientOfDistancesToBuildings.py` & `t4gpd-0.7.1/t4gpd/morph/STGradientOfDistancesToBuildings.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STGrid.py` & `t4gpd-0.7.1/t4gpd/morph/STGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STIdentifyRowOfTrees.py` & `t4gpd-0.7.1/t4gpd/morph/STIdentifyRowOfTrees.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STMakeBlocks.py` & `t4gpd-0.7.1/t4gpd/morph/STMakeBlocks.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STMakeGroundSurface.py` & `t4gpd-0.7.1/t4gpd/morph/STMakeGroundSurface.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps.py` & `t4gpd-0.7.1/t4gpd/morph/STMultipleOverlaps.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STMultipleOverlaps2.py` & `t4gpd-0.7.1/t4gpd/morph/STMultipleOverlaps2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STPointsDensifier.py` & `t4gpd-0.7.1/t4gpd/morph/STPointsDensifier.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STPointsDensifier2.py` & `t4gpd-0.7.1/t4gpd/morph/STPointsDensifier2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STPolygonize.py` & `t4gpd-0.7.1/t4gpd/morph/STPolygonize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STSkeletonize.py` & `t4gpd-0.7.1/t4gpd/morph/STSkeletonize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STSkeletonizeTheVoid.py` & `t4gpd-0.7.1/t4gpd/morph/STSkeletonizeTheVoid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STSkyMap25D.py` & `t4gpd-0.7.1/t4gpd/morph/STSkyMap25D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines.py` & `t4gpd-0.7.1/t4gpd/morph/STSnappingPointsOnLines.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STSnappingPointsOnLines2.py` & `t4gpd-0.7.1/t4gpd/morph/STSnappingPointsOnLines2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STSpatialJoin.py` & `t4gpd-0.7.1/t4gpd/morph/STSpatialJoin.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STSquaredBBox.py` & `t4gpd-0.7.1/t4gpd/morph/STSquaredBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STVariableWidthBuffer.py` & `t4gpd-0.7.1/t4gpd/morph/STVariableWidthBuffer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/STVoronoiPartition.py` & `t4gpd-0.7.1/t4gpd/morph/STVoronoiPartition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/AbstractGeoprocess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AngularAbscissa.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/AngularAbscissa.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/AreaConvexityDefect.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/AspectRatio.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/AspectRatio.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/BBox.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/BBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CircularityIndices.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/CircularityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexHull.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/ConvexityIndices.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/ConvexityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/CrossroadRecognition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/CrossroadsAngularity.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/Diameter.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/Diameter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/EllipticityIndices.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/EllipticityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/FootprintExtruder.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/FootprintExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/GetInteriorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/GridFace.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/GridFace.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/HMean.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/HMean.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/HeightOfRoughness.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABE.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/MABE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/MABR.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MABR2.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/MABR2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MBC.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/MBC.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/MPBR.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/MPBR.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectangularityIndices.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/RectangularityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFFT.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/RectifyByFFT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RectifyByFWT.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/RectifyByFWT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RemoveHoles.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/RemoveHoles.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/RepresentativePoint.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/RepresentativePoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/Rotation2D.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/Rotation2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/STGeoProcess.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/STGeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyMap2D.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/SkyMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactor.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/SkyViewFactor.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/StarShapedIndices.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/StarShapedIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/SurfaceFraction.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/SurfaceFraction.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/Translation.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/Translation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/morph/geoProcesses/WMean.py` & `t4gpd-0.7.1/t4gpd/morph/geoProcesses/WMean.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/CampbellSciReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/CampbellSciReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/ExtraProcessing.py` & `t4gpd-0.7.1/t4gpd/picoclim/ExtraProcessing.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/InertialMeasureReWriter.py` & `t4gpd-0.7.1/t4gpd/picoclim/InertialMeasureReWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/InertialMeasureReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/InertialMeasureReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/JoinByTimeDistance.py` & `t4gpd-0.7.1/t4gpd/picoclim/JoinByTimeDistance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/KestrelReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/KestrelReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/MeteoFranceReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/MeteoFranceReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py` & `t4gpd-0.7.1/t4gpd/picoclim/MetrologicalCampaignPlottings.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/MetrologicalCampaignReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/MetrologicalCampaignReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/SensirionReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/SensirionReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py` & `t4gpd-0.7.1/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py` & `t4gpd-0.7.1/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/TracksWaypointsReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/TracksWaypointsReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/UClimGuidingReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/UClimGuidingReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/picoclim/UClimTrackWaypointsReader.py` & `t4gpd-0.7.1/t4gpd/picoclim/UClimTrackWaypointsReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyplot/MultipleMarkerStyles.py` & `t4gpd-0.7.1/t4gpd/pyplot/MultipleMarkerStyles.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyqgis/AddMemoryLayer.py` & `t4gpd-0.7.1/t4gpd/pyqgis/AddMemoryLayer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyqgis/Emphasizer.py` & `t4gpd-0.7.1/t4gpd/pyqgis/Emphasizer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyqgis/MapPrinter.py` & `t4gpd-0.7.1/t4gpd/pyqgis/MapPrinter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyqgis/PdfMapWriter.py` & `t4gpd-0.7.1/t4gpd/pyqgis/PdfMapWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyqgis/SetSymbolLib.py` & `t4gpd-0.7.1/t4gpd/pyqgis/SetSymbolLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyqgis/ShowFeatureCount.py` & `t4gpd-0.7.1/t4gpd/pyqgis/ShowFeatureCount.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyqgis/ZoomLib.py` & `t4gpd-0.7.1/t4gpd/pyqgis/ZoomLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/GeodeCiel.py` & `t4gpd-0.7.1/t4gpd/pyvista/GeodeCiel.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/Icosahedron.py` & `t4gpd-0.7.1/t4gpd/pyvista/Icosahedron.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/Plotter3D.py` & `t4gpd-0.7.1/t4gpd/pyvista/Plotter3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/STRaysToViewFactors.py` & `t4gpd-0.7.1/t4gpd/pyvista/STRaysToViewFactors.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/ToPolyData.py` & `t4gpd-0.7.1/t4gpd/pyvista/ToPolyData.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/ToUnstructuredGrid.py` & `t4gpd-0.7.1/t4gpd/pyvista/ToUnstructuredGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/commons/Diameter3DLib.py` & `t4gpd-0.7.1/t4gpd/pyvista/commons/Diameter3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/commons/RayCasting3DLib.py` & `t4gpd-0.7.1/t4gpd/pyvista/commons/RayCasting3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py` & `t4gpd-0.7.1/t4gpd/pyvista/commons/RayCastingIn3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/commons/SVF3DLib.py` & `t4gpd-0.7.1/t4gpd/pyvista/commons/SVF3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/commons/Triangle3D.py` & `t4gpd-0.7.1/t4gpd/pyvista/commons/Triangle3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py` & `t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py` & `t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py` & `t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py` & `t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py` & `t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py` & `t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/RayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/pyvista/geoProcesses/SVF3D.py` & `t4gpd-0.7.1/t4gpd/pyvista/geoProcesses/SVF3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/raster/STToRaster.py` & `t4gpd-0.7.1/t4gpd/raster/STToRaster.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/AbstractHardShadow.py` & `t4gpd-0.7.1/t4gpd/sun/AbstractHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/STHardShadow.py` & `t4gpd-0.7.1/t4gpd/sun/STHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/STSunMap2D.py` & `t4gpd-0.7.1/t4gpd/sun/STSunMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow.py` & `t4gpd-0.7.1/t4gpd/sun/STTreeHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/STTreeHardShadow2.py` & `t4gpd-0.7.1/t4gpd/sun/STTreeHardShadow2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py` & `t4gpd-0.7.1/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDuration.py` & `t4gpd-0.7.1/t4gpd/sun/geoProcesses/SunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py` & `t4gpd-0.7.1/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.7.0/t4gpd.egg-info/PKG-INFO` & `t4gpd-0.7.1/t4gpd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.7.0
+Version: 0.7.1
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
 Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
@@ -42,14 +42,14 @@
 > pip install Dijkstar suntimes pythermalcomfort
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-> pip install t4gpd-0.6.0.tar.gz
+> pip install t4gpd-0.7.1.tar.gz
 
 ## Read the documentation
 Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
```

### Comparing `t4gpd-0.7.0/t4gpd.egg-info/SOURCES.txt` & `t4gpd-0.7.1/t4gpd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

