# Comparing `tmp/irsdev_pycolor-1.0.2.tar.gz` & `tmp/irsdev_pycolor-1.0.3.tar.gz`

## Comparing `irsdev_pycolor-1.0.2.tar` & `irsdev_pycolor-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.2/irs-pycolor/PyColor/Colors.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.2/irs-pycolor/PyColor/Palettes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.2/irs-pycolor/PyColor/__init__.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.2/LICENSE
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.2/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.3/irsdev-pycolor/Colors.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.3/irsdev-pycolor/Palettes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.3/irsdev-pycolor/__init__.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.3/LICENSE
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.3/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 irsdev_pycolor-1.0.3/PKG-INFO
```

### Comparing `irsdev_pycolor-1.0.2/irs-pycolor/PyColor/Colors.py` & `irsdev_pycolor-1.0.3/irsdev-pycolor/Colors.py`

 * *Files identical despite different names*

### Comparing `irsdev_pycolor-1.0.2/irs-pycolor/PyColor/Palettes.py` & `irsdev_pycolor-1.0.3/irsdev-pycolor/Palettes.py`

 * *Files identical despite different names*

### Comparing `irsdev_pycolor-1.0.2/LICENSE` & `irsdev_pycolor-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `irsdev_pycolor-1.0.2/README.md` & `irsdev_pycolor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `irsdev_pycolor-1.0.2/pyproject.toml` & `irsdev_pycolor-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "irsdev-pycolor"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
 description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `irsdev_pycolor-1.0.2/PKG-INFO` & `irsdev_pycolor-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irsdev-pycolor
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Author-email: Irtsa <irtsa.development@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

