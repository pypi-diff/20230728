# Comparing `tmp/az_image-converter-0.0.1.tar.gz` & `tmp/az_image-converter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "az_image-converter-0.0.1.tar", last modified: Fri Jul 28 11:30:57 2023, max compression
+gzip compressed data, was "az_image-converter-0.0.2.tar", last modified: Fri Jul 28 11:41:59 2023, max compression
```

## Comparing `az_image-converter-0.0.1.tar` & `az_image-converter-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:30:57.019621 az_image-converter-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-28 11:06:18.000000 az_image-converter-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      850 2023-07-28 11:30:57.003986 az_image-converter-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2954 2023-07-28 09:48:45.000000 az_image-converter-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 11:30:57.003986 az_image-converter-0.0.1/az_image_converter.egg-info/
--rw-rw-rw-   0        0        0      850 2023-07-28 11:30:56.000000 az_image-converter-0.0.1/az_image_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-28 11:30:56.000000 az_image-converter-0.0.1/az_image_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:30:56.000000 az_image-converter-0.0.1/az_image_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 11:30:56.000000 az_image-converter-0.0.1/az_image_converter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:30:56.000000 az_image-converter-0.0.1/az_image_converter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 11:30:57.019621 az_image-converter-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-07-28 11:30:52.000000 az_image-converter-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:41:59.831100 az_image-converter-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-28 11:06:18.000000 az_image-converter-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3742 2023-07-28 11:41:59.831100 az_image-converter-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2954 2023-07-28 09:48:45.000000 az_image-converter-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 11:41:59.831100 az_image-converter-0.0.2/az_image_converter.egg-info/
+-rw-rw-rw-   0        0        0     3742 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:41:59.846726 az_image-converter-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4080 2023-07-28 11:39:32.000000 az_image-converter-0.0.2/setup.py
```

### Comparing `az_image-converter-0.0.1/LICENSE` & `az_image-converter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `az_image-converter-0.0.1/README.md` & `az_image-converter-0.0.2/README.md`

 * *Files identical despite different names*

