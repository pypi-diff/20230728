# Comparing `tmp/example_package_kian-0.0.1.tar.gz` & `tmp/example_package_kian-0.0.2.tar.gz`

## Comparing `example_package_kian-0.0.1.tar` & `example_package_kian-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_kian-0.0.1/src/example_package_kian/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_kian-0.0.1/src/example_package_kian/example.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 example_package_kian-0.0.1/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 example_package_kian-0.0.1/README.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 example_package_kian-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 example_package_kian-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/src/example_package_kian/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/src/example_package_kian/example.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/README.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/PKG-INFO
```

### Comparing `example_package_kian-0.0.1/LICENSE` & `example_package_kian-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_kian-0.0.1/pyproject.toml` & `example_package_kian-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "example_package_kian"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="kian kyars", email="kiankyars@gmail.com" },
 ]
 maintainers = [
     {name="andrej karpathy", email="andrej.karpathy@gmail.com"}
 ]
 description = "A small example package"
```

### Comparing `example_package_kian-0.0.1/PKG-INFO` & `example_package_kian-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_kian
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: kian kyars <kiankyars@gmail.com>
 Maintainer-email: andrej karpathy <andrej.karpathy@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

