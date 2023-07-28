# Comparing `tmp/example_package_kian-0.0.2.tar.gz` & `tmp/example_package_kian-0.0.3.tar.gz`

## Comparing `example_package_kian-0.0.2.tar` & `example_package_kian-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/src/example_package_kian/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/src/example_package_kian/example.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/README.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 example_package_kian-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_kian-0.0.3/src/example_package_kian/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 example_package_kian-0.0.3/src/example_package_kian/example.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 example_package_kian-0.0.3/LICENSE
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 example_package_kian-0.0.3/README.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 example_package_kian-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 example_package_kian-0.0.3/PKG-INFO
```

### Comparing `example_package_kian-0.0.2/LICENSE` & `example_package_kian-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_kian-0.0.2/pyproject.toml` & `example_package_kian-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "example_package_kian"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="kian kyars", email="kiankyars@gmail.com" },
 ]
 maintainers = [
-    {name="andrej karpathy", email="andrej.karpathy@gmail.com"}
+    {name="andrej karpathy", email="andrej.karpathy@gmail.com"},
+    {name="leo gao", email="leogao31@gmail.com"},
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `example_package_kian-0.0.2/PKG-INFO` & `example_package_kian-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: example_package_kian
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: kian kyars <kiankyars@gmail.com>
-Maintainer-email: andrej karpathy <andrej.karpathy@gmail.com>
+Maintainer-email: andrej karpathy <andrej.karpathy@gmail.com>, leo gao <leogao31@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+to write your content.
+I also completely lacked on my internship.
```

