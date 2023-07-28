# Comparing `tmp/irdev_pycolor-1.0.0.tar.gz` & `tmp/irdev_pycolor-1.0.1.tar.gz`

## Comparing `irdev_pycolor-1.0.0.tar` & `irdev_pycolor-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.0/src/PyColor/Colors.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.0/src/PyColor/Palettes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.0/src/PyColor/__init__.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.0/LICENSE
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.0/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.1/src/PyColor/Colors.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.1/src/PyColor/Palettes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.1/src/PyColor/__init__.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.1/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 irdev_pycolor-1.0.1/PKG-INFO
```

### Comparing `irdev_pycolor-1.0.0/src/PyColor/Colors.py` & `irdev_pycolor-1.0.1/src/PyColor/Colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,17 +926,17 @@
     def rgb(self) -> tuple:
         if not self.__valid: return None
 
         r = int(round((self.y * 1.1643835616 + self.cr * 1.7927410714 - 248.100994), 3))
         g = int(round((self.y * 1.1643835616 + self.cb * -0.2132486143 + self.cr * -0.5329093286 + 76.878080), 3))
         b = int(round((self.y * 1.1643835616 + self.cb * 2.1124017857 - 289.017566), 3))
 
-	r = max(0, min(255, r))
-	g = max(0, min(255, g))
-	b = max(0, min(255, b))
+        r = max(0, min(255, r))
+        g = max(0, min(255, g))
+        b = max(0, min(255, b))
         
         return (r, g, b)
     
 
     @property
     def hexidecimal(self) -> tuple:
         if not self.__valid: return None
```

### Comparing `irdev_pycolor-1.0.0/src/PyColor/Palettes.py` & `irdev_pycolor-1.0.1/src/PyColor/Palettes.py`

 * *Files identical despite different names*

### Comparing `irdev_pycolor-1.0.0/LICENSE` & `irdev_pycolor-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `irdev_pycolor-1.0.0/README.md` & `irdev_pycolor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `irdev_pycolor-1.0.0/pyproject.toml` & `irdev_pycolor-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "irdev-pycolor"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
 description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `irdev_pycolor-1.0.0/PKG-INFO` & `irdev_pycolor-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irdev-pycolor
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Author-email: Irtsa <irtsa.development@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

