# Comparing `tmp/py-adapter-0.0.1.tar.gz` & `tmp/py-adapter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-adapter-0.0.1.tar", last modified: Wed Jul 26 13:34:34 2023, max compression
+gzip compressed data, was "py-adapter-0.0.2.tar", last modified: Fri Jul 28 11:38:31 2023, max compression
```

## Comparing `py-adapter-0.0.1.tar` & `py-adapter-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.091234 py-adapter-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-26 13:34:21.000000 py-adapter-0.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-26 13:34:21.000000 py-adapter-0.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.087234 py-adapter-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.091234 py-adapter-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-26 13:34:21.000000 py-adapter-0.0.1/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-26 13:34:21.000000 py-adapter-0.0.1/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-26 13:34:21.000000 py-adapter-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-26 13:34:21.000000 py-adapter-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-26 13:34:21.000000 py-adapter-0.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-26 13:34:21.000000 py-adapter-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-26 13:34:21.000000 py-adapter-0.0.1/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-26 13:34:34.091234 py-adapter-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-26 13:34:21.000000 py-adapter-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.091234 py-adapter-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-26 13:34:21.000000 py-adapter-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 13:34:21.000000 py-adapter-0.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 13:34:21.000000 py-adapter-0.0.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 13:34:21.000000 py-adapter-0.0.1/docs/py_adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-26 13:34:21.000000 py-adapter-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:34:34.091234 py-adapter-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.087234 py-adapter-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.091234 py-adapter-0.0.1/src/py_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)    21484 2023-07-26 13:34:21.000000 py-adapter-0.0.1/src/py_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-26 13:34:21.000000 py-adapter-0.0.1/src/py_adapter/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 13:34:21.000000 py-adapter-0.0.1/src/py_adapter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.091234 py-adapter-0.0.1/src/py_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-26 13:34:34.000000 py-adapter-0.0.1/src/py_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-26 13:34:34.000000 py-adapter-0.0.1/src/py_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:34:34.000000 py-adapter-0.0.1/src/py_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 13:34:34.000000 py-adapter-0.0.1/src/py_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 13:34:34.000000 py-adapter-0.0.1/src/py_adapter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:34.091234 py-adapter-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-26 13:34:21.000000 py-adapter-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 13:34:21.000000 py-adapter-0.0.1/tests/country.avsc
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 13:34:21.000000 py-adapter-0.0.1/tests/goods_with_country.avsc
--rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-07-26 13:34:21.000000 py-adapter-0.0.1/tests/test_py_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-26 13:34:21.000000 py-adapter-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.406741 py-adapter-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-28 11:38:17.000000 py-adapter-0.0.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-28 11:38:17.000000 py-adapter-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.398740 py-adapter-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.402741 py-adapter-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-28 11:38:17.000000 py-adapter-0.0.2/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-28 11:38:17.000000 py-adapter-0.0.2/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-28 11:38:17.000000 py-adapter-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-28 11:38:17.000000 py-adapter-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-28 11:38:17.000000 py-adapter-0.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-28 11:38:17.000000 py-adapter-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 11:38:17.000000 py-adapter-0.0.2/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-28 11:38:31.406741 py-adapter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-28 11:38:17.000000 py-adapter-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.402741 py-adapter-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-28 11:38:17.000000 py-adapter-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-28 11:38:17.000000 py-adapter-0.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 11:38:17.000000 py-adapter-0.0.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 11:38:17.000000 py-adapter-0.0.2/docs/py_adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-28 11:38:17.000000 py-adapter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:38:31.406741 py-adapter-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.398740 py-adapter-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.406741 py-adapter-0.0.2/src/py_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-07-28 11:38:17.000000 py-adapter-0.0.2/src/py_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-28 11:38:17.000000 py-adapter-0.0.2/src/py_adapter/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 11:38:17.000000 py-adapter-0.0.2/src/py_adapter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.406741 py-adapter-0.0.2/src/py_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-28 11:38:31.000000 py-adapter-0.0.2/src/py_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-28 11:38:31.000000 py-adapter-0.0.2/src/py_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:38:31.000000 py-adapter-0.0.2/src/py_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 11:38:31.000000 py-adapter-0.0.2/src/py_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 11:38:31.000000 py-adapter-0.0.2/src/py_adapter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:38:31.406741 py-adapter-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-28 11:38:17.000000 py-adapter-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-28 11:38:17.000000 py-adapter-0.0.2/tests/country.avsc
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 11:38:17.000000 py-adapter-0.0.2/tests/goods_with_country.avsc
+-rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-07-28 11:38:17.000000 py-adapter-0.0.2/tests/test_py_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-28 11:38:17.000000 py-adapter-0.0.2/tox.ini
```

### Comparing `py-adapter-0.0.1/.flake8` & `py-adapter-0.0.2/.flake8`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/.github/workflows/release-package.yml` & `py-adapter-0.0.2/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/.github/workflows/test-package.yml` & `py-adapter-0.0.2/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/.gitignore` & `py-adapter-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/.pre-commit-config.yaml` & `py-adapter-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/.readthedocs.yaml` & `py-adapter-0.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/LICENSE` & `py-adapter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/LICENSE_HEADER.txt` & `py-adapter-0.0.2/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/PKG-INFO` & `py-adapter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-adapter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Round-trip serialization/deserialization of any Python object to/from any serialization format including Avro and JSON.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-adapter-0.0.1/README.md` & `py-adapter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/docs/conf.py` & `py-adapter-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/pyproject.toml` & `py-adapter-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 requires-python = ">=3.7"
 # All runtime dependencies that must be packaged, pin major version only.
 dependencies = [
     "avro~=1.11",
     "importlib-metadata<4; python_version<'3.8'",
     "memoization~=0.4",
     "orjson~=3.0",
-    "py-avro-schema~=2.1",
+    "py-avro-schema~=2.2",
     "python-dateutil~=2.8",
 ]
 
 
 [project.urls]
 
 "Homepage" = "https://github.com/jpmorganchase/py-adapter"
```

### Comparing `py-adapter-0.0.1/src/py_adapter/__init__.py` & `py-adapter-0.0.2/src/py_adapter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         :param py_type: The Python class to return an object adapter for
         """
         try:
             # TODO: expose options as necessary
             schema = avro.schema.parse(
                 pas.generate(py_type, options=pas.Option.LOGICAL_JSON_STRING | pas.Option.MILLISECONDS).decode("utf-8")
             )
-        except TypeError:
+        except pas.TypeNotSupportedError:
             raise TypeError(f"{py_type} not supported by py-adapter since it is not supported by py-avro-schema")
         return cls(schema)
 
     def adapt(self, data: Basic) -> Any:
         """
         Parse a data structure and return a Python object
```

### Comparing `py-adapter-0.0.1/src/py_adapter/_schema.py` & `py-adapter-0.0.2/src/py_adapter/_schema.py`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/src/py_adapter.egg-info/PKG-INFO` & `py-adapter-0.0.2/src/py_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-adapter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Round-trip serialization/deserialization of any Python object to/from any serialization format including Avro and JSON.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-adapter-0.0.1/src/py_adapter.egg-info/SOURCES.txt` & `py-adapter-0.0.2/src/py_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/tests/conftest.py` & `py-adapter-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/tests/test_py_adapter.py` & `py-adapter-0.0.2/tests/test_py_adapter.py`

 * *Files identical despite different names*

### Comparing `py-adapter-0.0.1/tox.ini` & `py-adapter-0.0.2/tox.ini`

 * *Files identical despite different names*

