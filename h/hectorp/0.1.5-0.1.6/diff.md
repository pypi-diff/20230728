# Comparing `tmp/hectorp-0.1.5.tar.gz` & `tmp/hectorp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hectorp-0.1.5.tar", last modified: Sun Jun 18 08:48:13 2023, max compression
+gzip compressed data, was "hectorp-0.1.6.tar", last modified: Fri Jul 28 17:34:43 2023, max compression
```

## Comparing `hectorp-0.1.5.tar` & `hectorp-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-18 08:48:13.359206 hectorp-0.1.5/
--rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.5/LICENSE
--rw-r--r--   0 msbos      (501) staff       (20)     7909 2023-06-18 08:48:13.358921 hectorp-0.1.5/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     7344 2023-06-17 17:50:05.000000 hectorp-0.1.5/README.md
--rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.5/pyproject.toml
--rw-r--r--   0 msbos      (501) staff       (20)       38 2023-06-18 08:48:13.359285 hectorp-0.1.5/setup.cfg
--rw-r--r--   0 msbos      (501) staff       (20)     1841 2023-06-18 08:48:04.000000 hectorp-0.1.5/setup.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-18 08:48:13.339906 hectorp-0.1.5/src/
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-18 08:48:13.356823 hectorp-0.1.5/src/hectorp/
--rw-r--r--   0 msbos      (501) staff       (20)        0 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/__init__.py
--rw-r--r--   0 msbos      (501) staff       (20)     7125 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/ammargrag.py
--rw-r--r--   0 msbos      (501) staff       (20)    10305 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/apply_WF.py
--rw-r--r--   0 msbos      (501) staff       (20)     4453 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/ar1.py
--rw-r--r--   0 msbos      (501) staff       (20)     3888 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/control.py
--rw-r--r--   0 msbos      (501) staff       (20)     2217 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/convert_rlrdata2mom.py
--rw-r--r--   0 msbos      (501) staff       (20)     7568 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/covariance.py
--rw-r--r--   0 msbos      (501) staff       (20)     3395 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/datasnooping.py
--rw-r--r--   0 msbos      (501) staff       (20)     1817 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/date2mjd.py
--rw-r--r--   0 msbos      (501) staff       (20)    14416 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/designmatrix.py
--rw-r--r--   0 msbos      (501) staff       (20)     8101 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/estimate_all_trends.py
--rw-r--r--   0 msbos      (501) staff       (20)    12518 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/estimatespectrum.py
--rw-r--r--   0 msbos      (501) staff       (20)     5702 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/estimatetrend.py
--rw-r--r--   0 msbos      (501) staff       (20)     8136 2023-06-18 08:35:30.000000 hectorp-0.1.5/src/hectorp/findoffsets.py
--rw-r--r--   0 msbos      (501) staff       (20)     3082 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/fullcov.py
--rw-r--r--   0 msbos      (501) staff       (20)     9744 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/ggm.py
--rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/levinson.py
--rw-r--r--   0 msbos      (501) staff       (20)     7625 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/matern.py
--rw-r--r--   0 msbos      (501) staff       (20)     1617 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/mjd2date.py
--rw-r--r--   0 msbos      (501) staff       (20)     9677 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/mle.py
--rw-r--r--   0 msbos      (501) staff       (20)     4205 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/msf.py
--rw-r--r--   0 msbos      (501) staff       (20)     3923 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/msfdump.py
--rw-r--r--   0 msbos      (501) staff       (20)     3527 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/msfgen.py
--rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/mycalendar.py
--rw-r--r--   0 msbos      (501) staff       (20)    16821 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/observations.py
--rw-r--r--   0 msbos      (501) staff       (20)     2574 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/ols.py
--rw-r--r--   0 msbos      (501) staff       (20)     4682 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/powerlaw.py
--rw-r--r--   0 msbos      (501) staff       (20)     8520 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/predicttrenderror.py
--rw-r--r--   0 msbos      (501) staff       (20)     1102 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/pyfftw_ex1.py
--rw-r--r--   0 msbos      (501) staff       (20)     4866 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/removeoutliers.py
--rw-r--r--   0 msbos      (501) staff       (20)       55 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/run_schur.py
--rw-r--r--   0 msbos      (501) staff       (20)     8995 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/schur.py
--rw-r--r--   0 msbos      (501) staff       (20)    11670 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/simulatenoise.py
--rw-r--r--   0 msbos      (501) staff       (20)     9805 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/test_Schur.py
--rw-r--r--   0 msbos      (501) staff       (20)     1050 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/test_opencl.py
--rw-r--r--   0 msbos      (501) staff       (20)     1852 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/test_reikna.py
--rw-r--r--   0 msbos      (501) staff       (20)     5265 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/varyingannual.py
--rw-r--r--   0 msbos      (501) staff       (20)     3067 2023-06-18 08:21:37.000000 hectorp-0.1.5/src/hectorp/white.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-18 08:48:13.358548 hectorp-0.1.5/src/hectorp.egg-info/
--rw-r--r--   0 msbos      (501) staff       (20)     7909 2023-06-18 08:48:13.000000 hectorp-0.1.5/src/hectorp.egg-info/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     1218 2023-06-18 08:48:13.000000 hectorp-0.1.5/src/hectorp.egg-info/SOURCES.txt
--rw-r--r--   0 msbos      (501) staff       (20)        1 2023-06-18 08:48:13.000000 hectorp-0.1.5/src/hectorp.egg-info/dependency_links.txt
--rw-r--r--   0 msbos      (501) staff       (20)      596 2023-06-18 08:48:13.000000 hectorp-0.1.5/src/hectorp.egg-info/entry_points.txt
--rw-r--r--   0 msbos      (501) staff       (20)       37 2023-06-18 08:48:13.000000 hectorp-0.1.5/src/hectorp.egg-info/requires.txt
--rw-r--r--   0 msbos      (501) staff       (20)        8 2023-06-18 08:48:13.000000 hectorp-0.1.5/src/hectorp.egg-info/top_level.txt
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-07-28 17:34:43.045880 hectorp-0.1.6/
+-rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.6/LICENSE
+-rw-r--r--   0 msbos      (501) staff       (20)     7908 2023-07-28 17:34:43.045318 hectorp-0.1.6/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     7343 2023-07-20 15:14:52.000000 hectorp-0.1.6/README.md
+-rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.6/pyproject.toml
+-rw-r--r--   0 msbos      (501) staff       (20)       38 2023-07-28 17:34:43.046056 hectorp-0.1.6/setup.cfg
+-rw-r--r--   0 msbos      (501) staff       (20)     1841 2023-07-28 17:33:15.000000 hectorp-0.1.6/setup.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-07-28 17:34:43.002440 hectorp-0.1.6/src/
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-07-28 17:34:43.040524 hectorp-0.1.6/src/hectorp/
+-rw-r--r--   0 msbos      (501) staff       (20)        0 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/__init__.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7125 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/ammargrag.py
+-rw-r--r--   0 msbos      (501) staff       (20)    10305 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/apply_WF.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4453 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/ar1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/calendar.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3888 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/control.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2217 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/convert_rlrdata2mom.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7568 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/covariance.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3395 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/datasnooping.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1817 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/date2mjd.py
+-rw-r--r--   0 msbos      (501) staff       (20)    14416 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/designmatrix.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8101 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/estimate_all_trends.py
+-rw-r--r--   0 msbos      (501) staff       (20)    12518 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/estimatespectrum.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5702 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/estimatetrend.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8136 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/findoffsets.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3082 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/fullcov.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9744 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/ggm.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/levinson.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7625 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/matern.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1617 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/mjd2date.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9677 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/mle.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4205 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/msf.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3923 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/msfdump.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3527 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/msfgen.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/mycalendar.py
+-rw-r--r--   0 msbos      (501) staff       (20)    16821 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/observations.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2574 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/ols.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4682 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/powerlaw.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8520 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/predicttrenderror.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1102 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/pyfftw_ex1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4866 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/removeoutliers.py
+-rw-r--r--   0 msbos      (501) staff       (20)       55 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/run_schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8995 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)    11670 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/simulatenoise.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9805 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/test_Schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1050 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/test_opencl.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1852 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/test_reikna.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5265 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/varyingannual.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3067 2023-07-28 17:29:55.000000 hectorp-0.1.6/src/hectorp/white.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-07-28 17:34:43.044659 hectorp-0.1.6/src/hectorp.egg-info/
+-rw-r--r--   0 msbos      (501) staff       (20)     7908 2023-07-28 17:34:42.000000 hectorp-0.1.6/src/hectorp.egg-info/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     1242 2023-07-28 17:34:43.000000 hectorp-0.1.6/src/hectorp.egg-info/SOURCES.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        1 2023-07-28 17:34:42.000000 hectorp-0.1.6/src/hectorp.egg-info/dependency_links.txt
+-rw-r--r--   0 msbos      (501) staff       (20)      596 2023-07-28 17:34:42.000000 hectorp-0.1.6/src/hectorp.egg-info/entry_points.txt
+-rw-r--r--   0 msbos      (501) staff       (20)       37 2023-07-28 17:34:42.000000 hectorp-0.1.6/src/hectorp.egg-info/requires.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        8 2023-07-28 17:34:42.000000 hectorp-0.1.6/src/hectorp.egg-info/top_level.txt
```

### Comparing `hectorp-0.1.5/LICENSE` & `hectorp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/PKG-INFO` & `hectorp-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 ### HectorP
 
 ### Table of Contents
 
 1. [Introduction](#introduction)
 2. [Code Description](#code)
     1. [Installation](#installation)
@@ -45,15 +44,15 @@
 
 | Name              | Description                                              |
 |:---               |:---                                                      |
 | estimatetrend | Main program to estimate a linear trend.                 |
 | estimatespectrum  | Program to estimate the power spectral density from the data or residuals using the Welch periodogram method.  |
 | modelspectrum     | Given a noise model and values of the noise parameters,  this program computed the associated power spectral density for given frequency range.                       |
 | removeoutliers | Program to remove outliers from the data.                |
-| findoffset        | Program to find the epoch of a possible offset in the time series.                                             |
+| findoffsets       | Program to find the epoch of a possible offset in the time series.                                             |
 | simulatenoise     | Program to files with synthetic coloured noise.          |
 | date2mjd | Small program to convert calendar date into Modified  Julian Date.                                      |
 | mjd2date | The inverse of date2mjd.      |
 | msfgen | MSF: MJD - SOD - Format. Small program to combine a json file with metadata and a text file with data in columns into a single binary file.      |
 | msfdump | Inverse of msfgen. Small program that reads a msf-file and creates  a json file with metadata and a text file with data in columns.      |
```

### Comparing `hectorp-0.1.5/README.md` & `hectorp-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 ### HectorP
 
 ### Table of Contents
 
 1. [Introduction](#introduction)
 2. [Code Description](#code)
     1. [Installation](#installation)
@@ -30,15 +29,15 @@
 
 | Name              | Description                                              |
 |:---               |:---                                                      |
 | estimatetrend | Main program to estimate a linear trend.                 |
 | estimatespectrum  | Program to estimate the power spectral density from the data or residuals using the Welch periodogram method.  |
 | modelspectrum     | Given a noise model and values of the noise parameters,  this program computed the associated power spectral density for given frequency range.                       |
 | removeoutliers | Program to remove outliers from the data.                |
-| findoffset        | Program to find the epoch of a possible offset in the time series.                                             |
+| findoffsets       | Program to find the epoch of a possible offset in the time series.                                             |
 | simulatenoise     | Program to files with synthetic coloured noise.          |
 | date2mjd | Small program to convert calendar date into Modified  Julian Date.                                      |
 | mjd2date | The inverse of date2mjd.      |
 | msfgen | MSF: MJD - SOD - Format. Small program to combine a json file with metadata and a text file with data in columns into a single binary file.      |
 | msfdump | Inverse of msfgen. Small program that reads a msf-file and creates  a json file with metadata and a text file with data in columns.      |
```

### Comparing `hectorp-0.1.5/setup.py` & `hectorp-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hectorp",
-    version="0.1.5",
+    version="0.1.6",
     author="Machiel Bos",
     author_email="machielbos@protonmail.com",
     description="A collection of programs to analyse geodetic time series",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/machielsimonbos/hectorp",
     project_urls={
```

### Comparing `hectorp-0.1.5/src/hectorp/ammargrag.py` & `hectorp-0.1.6/src/hectorp/ammargrag.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # for Toeplitz Systems", By Michael K. Ng  (page 28-29)
 #
 # Equations are taken from Bos et al. (2013), "Fast error analysis of 
 # continuous GNSS observations with missing data", Journal of Geodesy,
 # DOI 10.1007/s00190-012-0605-0.
 #
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/apply_WF.py` & `hectorp-0.1.6/src/hectorp/apply_WF.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp/ar1.py` & `hectorp-0.1.6/src/hectorp/ar1.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp/control.py` & `hectorp-0.1.6/src/hectorp/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # control.py
 #
-# This file is part of HectorP 0.1.5
+# This file is part of HectorP 0.1.6
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/convert_rlrdata2mom.py` & `hectorp-0.1.6/src/hectorp/convert_rlrdata2mom.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp/covariance.py` & `hectorp-0.1.6/src/hectorp/covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  1) power-law noise using Eq. (7) of Bos et al. (2008).
 #  2) white noise
 #
 # Bos, MS, Fernandes, RMS, Williams, SDP & Bastos, L (2008). "Fast error 
 # analysis of continuous GPS observations". Journal of Geodesy, 82(3), 157-166.
 #
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/datasnooping.py` & `hectorp-0.1.6/src/hectorp/datasnooping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # datasnooping.py
 #
 # Class which computes residuals and removes outliers
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/date2mjd.py` & `hectorp-0.1.6/src/hectorp/date2mjd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This small program computes the Modified Julian Date (MJD).
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.5/src/hectorp/designmatrix.py` & `hectorp-0.1.6/src/hectorp/designmatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # designmatrix.py
 #
 # Create design matrix
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/estimate_all_trends.py` & `hectorp-0.1.6/src/hectorp/estimate_all_trends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program find all files in ./obs_files and estimate all trends.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -153,15 +153,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n*******************************************")
-    print("    estimate_all_trends, version 0.1.5")
+    print("    estimate_all_trends, version 0.1.6")
     print("*******************************************\n")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Estimate all trends')
 
     #--- List arguments that can be given 
     parser.add_argument('-n', dest='noisemodels', action='store',default='PLWN',
```

### Comparing `hectorp-0.1.5/src/hectorp/estimatespectrum.py` & `hectorp-0.1.6/src/hectorp/estimatespectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program uses the Welch method of scipy to compute the power spectral 
 # density (one-sided).
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -185,15 +185,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    estimatespectrum, version 0.1.5")
+        print("    estimatespectrum, version 0.1.6")
         print("***************************************")
 
     #--- Get Classes
     observations = Observations()
 
     #--- Sampling frequency (change daily period into number of seconds)
     DeltaT = observations.sampling_period
```

### Comparing `hectorp-0.1.5/src/hectorp/estimatetrend.py` & `hectorp-0.1.6/src/hectorp/estimatetrend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program estimates a trend from the observations.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -67,15 +67,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    estimatetrend, version 0.1.5")
+        print("    estimatetrend, version 0.1.6")
         print("***************************************")
 
    
     #--- Get basename of filename
     datafile = control.params['DataFile']
     unit = control.params['PhysicalUnit']
     try:
```

### Comparing `hectorp-0.1.5/src/hectorp/findoffsets.py` & `hectorp-0.1.6/src/hectorp/findoffsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # Perform cycles of offset detection for a single station [optionally 3D]
 #  1) Compute noise and SLT model parameters
 #  2) Compute for each epoch the new log-likelihood when an offset is added
 #     but maintaining the noise parameters constant.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -86,15 +86,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n***************************************")
-    print("    findoffsets, version 0.1.5")
+    print("    findoffsets, version 0.1.6")
     print("***************************************")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Find offsets in time series')
 
     #--- List arguments that can be given 
     parser.add_argument('-s', dest='station', action='store', required=True,
```

### Comparing `hectorp-0.1.5/src/hectorp/fullcov.py` & `hectorp-0.1.6/src/hectorp/fullcov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # fullcov.py
 # 
 # Python3 implemenation of FullCov.cpp. 
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/ggm.py` & `hectorp-0.1.6/src/hectorp/ggm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ggm.py
 #
 # Create the first row of the covariance matrix for Generalised Gauss Markov
 # noise.
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/levinson.py` & `hectorp-0.1.6/src/hectorp/levinson.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # for Toeplitz Systems", By Michael K. Ng  (page 28-29)
 #
 # Equations are taken from Bos et al. (2013), "Fast error analysis of 
 # continuous GNSS observations with missing data", Journal of Geodesy,
 # DOI 10.1007/s00190-012-0605-0.
 #
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/matern.py` & `hectorp-0.1.6/src/hectorp/matern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # This class implements the Matérn noise model. Eqs. are taken from
 # Lilly et al. (2017) "Fractional Brownian motion, the Matérn process, and 
 # stochastic modeling of turbulent dispersion", Nonlinear Processes in 
 # Geophysics, 24: 481-514 
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/mjd2date.py` & `hectorp-0.1.6/src/hectorp/mjd2date.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # Simple MJD to date converter.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.5/src/hectorp/mle.py` & `hectorp-0.1.6/src/hectorp/mle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # mle.py
 #
 # Class which computes the log-likelihood and searches for the maximum value.
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/msf.py` & `hectorp-0.1.6/src/hectorp/msf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # msf.py
 #
 # A simple class that helps to read and write msf-files
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/msfdump.py` & `hectorp-0.1.6/src/hectorp/msfdump.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Create text file from msf-json file
 #
 # Example:
 # --------
 # msfdump -i drone_flight1.msf -o data.txt
 #
-# This program is part of HectorP 0.1.5
+# This program is part of HectorP 0.1.6
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/msfgen.py` & `hectorp-0.1.6/src/hectorp/msfgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Create msf-json files
 #
 # Example:
 # --------
 # msfgen -ji meta.json -di imu.dat -o drone_flight1.msf
 #
-# This program is part of HectorP 0.1.5
+# This program is part of HectorP 0.1.6
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/mycalendar.py` & `hectorp-0.1.6/src/hectorp/calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# This file is part of HectorP 0.1.5
+# This file is part of HectorP 0.1.6
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/observations.py` & `hectorp-0.1.6/src/hectorp/observations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # observations.py
 #
 # A simple interface that reads and writes mom-files and stores
 # them into a Python class 'observations'.
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/ols.py` & `hectorp-0.1.6/src/hectorp/ols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ols.py
 # 
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/powerlaw.py` & `hectorp-0.1.6/src/hectorp/powerlaw.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Create the first row of the covariance matrix for power-law noise models
 # using Eq. (7) of Bos et al. (2008).
 #
 # Bos, MS, Fernandes, RMS, Williams, SDP & Bastos, L (2008). "Fast error 
 # analysis of continuous GPS observations". Journal of Geodesy, 82(3), 157-166.
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/predicttrenderror.py` & `hectorp-0.1.6/src/hectorp/predicttrenderror.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program uses the estimated noise models parameters to predict the 
 # trend error for given number of observations.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -113,15 +113,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    predict error, version 0.1.5")
+        print("    predict error, version 0.1.6")
         print("***************************************")
 
     #--- Get Classes
     white = White()
     powerlaw = Powerlaw()
     ggm = GGM()
     varyingannual = VaryingAnnual()
```

### Comparing `hectorp-0.1.5/src/hectorp/pyfftw_ex1.py` & `hectorp-0.1.6/src/hectorp/pyfftw_ex1.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp/removeoutliers.py` & `hectorp-0.1.6/src/hectorp/removeoutliers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program removes outliers from the observations.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -71,15 +71,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    removeoutliers, version 0.1.5")
+        print("    removeoutliers, version 0.1.6")
         print("***************************************")
 
     #--- Get Classes
     datasnooping = DataSnooping()
     observations = Observations()
 
     #--- Get data
```

### Comparing `hectorp-0.1.5/src/hectorp/schur.py` & `hectorp-0.1.6/src/hectorp/schur.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # the first column of the Toeplitz covariance matrix C.
 #
 # Equations are taken from Bos et al. (2013), "Fast error analysis of 
 # continuous GNSS observations with missing data", Journal of Geodesy,
 # DOI 10.1007/s00190-012-0605-0.
 #
 #
-# This file is part of HectorP 0.1.5.
+# This file is part of HectorP 0.1.6.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.5/src/hectorp/simulatenoise.py` & `hectorp-0.1.6/src/hectorp/simulatenoise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program creates synthetic noise.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -242,15 +242,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n***************************************")
-    print("    simulatenoise, version 0.1.5")
+    print("    simulatenoise, version 0.1.6")
     print("***************************************")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Simulate noise time series')
 
     #--- List arguments that can be given 
     parser.add_argument('-i', required=False, default='simulatenoise.ctl', \
```

### Comparing `hectorp-0.1.5/src/hectorp/test_Schur.py` & `hectorp-0.1.6/src/hectorp/test_Schur.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program tests the generalised Schur algorithm to find the 
 # Cholesky decomposition of the inverse covariance matrix.
 #
-#  This script is part of HectorP 0.1.5
+#  This script is part of HectorP 0.1.6
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.5/src/hectorp/test_opencl.py` & `hectorp-0.1.6/src/hectorp/test_opencl.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp/test_reikna.py` & `hectorp-0.1.6/src/hectorp/test_reikna.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp/varyingannual.py` & `hectorp-0.1.6/src/hectorp/varyingannual.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp/white.py` & `hectorp-0.1.6/src/hectorp/white.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.5/src/hectorp.egg-info/PKG-INFO` & `hectorp-0.1.6/src/hectorp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 ### HectorP
 
 ### Table of Contents
 
 1. [Introduction](#introduction)
 2. [Code Description](#code)
     1. [Installation](#installation)
@@ -45,15 +44,15 @@
 
 | Name              | Description                                              |
 |:---               |:---                                                      |
 | estimatetrend | Main program to estimate a linear trend.                 |
 | estimatespectrum  | Program to estimate the power spectral density from the data or residuals using the Welch periodogram method.  |
 | modelspectrum     | Given a noise model and values of the noise parameters,  this program computed the associated power spectral density for given frequency range.                       |
 | removeoutliers | Program to remove outliers from the data.                |
-| findoffset        | Program to find the epoch of a possible offset in the time series.                                             |
+| findoffsets       | Program to find the epoch of a possible offset in the time series.                                             |
 | simulatenoise     | Program to files with synthetic coloured noise.          |
 | date2mjd | Small program to convert calendar date into Modified  Julian Date.                                      |
 | mjd2date | The inverse of date2mjd.      |
 | msfgen | MSF: MJD - SOD - Format. Small program to combine a json file with metadata and a text file with data in columns into a single binary file.      |
 | msfdump | Inverse of msfgen. Small program that reads a msf-file and creates  a json file with metadata and a text file with data in columns.      |
```

### Comparing `hectorp-0.1.5/src/hectorp.egg-info/SOURCES.txt` & `hectorp-0.1.6/src/hectorp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.py
 src/hectorp/__init__.py
 src/hectorp/ammargrag.py
 src/hectorp/apply_WF.py
 src/hectorp/ar1.py
+src/hectorp/calendar.py
 src/hectorp/control.py
 src/hectorp/convert_rlrdata2mom.py
 src/hectorp/covariance.py
 src/hectorp/datasnooping.py
 src/hectorp/date2mjd.py
 src/hectorp/designmatrix.py
 src/hectorp/estimate_all_trends.py
```

### Comparing `hectorp-0.1.5/src/hectorp.egg-info/entry_points.txt` & `hectorp-0.1.6/src/hectorp.egg-info/entry_points.txt`

 * *Files identical despite different names*

