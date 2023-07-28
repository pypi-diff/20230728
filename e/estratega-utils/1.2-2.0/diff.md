# Comparing `tmp/estratega-utils-1.2.tar.gz` & `tmp/estratega-utils-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estratega-utils-1.2.tar", last modified: Mon Jul 10 18:06:06 2023, max compression
+gzip compressed data, was "estratega-utils-2.0.tar", last modified: Fri Jul 28 14:27:11 2023, max compression
```

## Comparing `estratega-utils-1.2.tar` & `estratega-utils-2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.041013 estratega-utils-1.2/
--rw-rw-rw-   0        0        0      479 2023-07-10 18:06:06.037979 estratega-utils-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-07 15:48:13.000000 estratega-utils-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.027671 estratega-utils-1.2/estratega_utils.egg-info/
--rw-rw-rw-   0        0        0      479 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 18:06:06.041968 estratega-utils-1.2/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-07-10 13:20:00.000000 estratega-utils-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.033991 estratega-utils-1.2/utils/
--rw-rw-rw-   0        0        0      202 2023-07-07 17:18:39.000000 estratega-utils-1.2/utils/PRUEBAS.py
--rw-rw-rw-   0        0        0      228 2023-07-07 18:48:55.000000 estratega-utils-1.2/utils/__init__.py
--rw-rw-rw-   0        0        0     1188 2023-07-07 17:18:39.000000 estratega-utils-1.2/utils/dicts.py
--rw-rw-rw-   0        0        0      160 2023-07-07 18:48:27.000000 estratega-utils-1.2/utils/lists.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.035985 estratega-utils-1.2/utils/query_builder/
--rw-rw-rw-   0        0        0      119 2023-07-07 18:40:39.000000 estratega-utils-1.2/utils/query_builder/__init__.py
--rw-rw-rw-   0        0        0     7836 2023-07-10 18:03:44.000000 estratega-utils-1.2/utils/query_builder/mysql.py
--rw-rw-rw-   0        0        0      403 2023-07-06 14:57:10.000000 estratega-utils-1.2/utils/strings.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:27:11.223924 estratega-utils-2.0/
+-rw-rw-rw-   0        0        0      479 2023-07-28 14:27:11.222927 estratega-utils-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-26 20:22:24.000000 estratega-utils-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 14:27:11.210960 estratega-utils-2.0/estratega_utils.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-07-28 14:27:11.000000 estratega-utils-2.0/estratega_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-28 14:27:11.000000 estratega-utils-2.0/estratega_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 14:27:11.000000 estratega-utils-2.0/estratega_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 14:27:11.000000 estratega-utils-2.0/estratega_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 14:27:11.000000 estratega-utils-2.0/estratega_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 14:27:11.223924 estratega-utils-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-28 13:53:09.000000 estratega-utils-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:27:11.217945 estratega-utils-2.0/utils/
+-rw-rw-rw-   0        0        0      202 2023-07-07 17:18:39.000000 estratega-utils-2.0/utils/PRUEBAS.py
+-rw-rw-rw-   0        0        0      228 2023-07-07 18:48:55.000000 estratega-utils-2.0/utils/__init__.py
+-rw-rw-rw-   0        0        0     1188 2023-07-07 17:18:39.000000 estratega-utils-2.0/utils/dicts.py
+-rw-rw-rw-   0        0        0      160 2023-07-07 18:48:27.000000 estratega-utils-2.0/utils/lists.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:27:11.221931 estratega-utils-2.0/utils/query_builder/
+-rw-rw-rw-   0        0        0      119 2023-07-07 18:40:39.000000 estratega-utils-2.0/utils/query_builder/__init__.py
+-rw-rw-rw-   0        0        0    11731 2023-07-27 13:22:15.000000 estratega-utils-2.0/utils/query_builder/mysql.py
+-rw-rw-rw-   0        0        0      394 2023-07-27 13:04:09.000000 estratega-utils-2.0/utils/strings.py
```

### Comparing `estratega-utils-1.2/setup.py` & `estratega-utils-2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2'
+VERSION = '2.0'
 DESCRIPTION = 'Utilidades varias'
-LONG_DESCRIPTION = 'Funciones y clases con utiliddades para agilizar y optimizar la escritura de código'
+LONG_DESCRIPTION = 'Funciones y clases con utilidades para agilizar y optimizar la escritura de código.'
 
 # Configurando
 setup(
     # el nombre debe coincidir con el nombre de la carpeta
     # 'modulomuysimple'
     name="estratega-utils",
     version=VERSION,
```

### Comparing `estratega-utils-1.2/utils/dicts.py` & `estratega-utils-2.0/utils/dicts.py`

 * *Files identical despite different names*

