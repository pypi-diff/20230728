# Comparing `tmp/rxn-utils-1.1.9.tar.gz` & `tmp/rxn-utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-utils-1.1.9.tar", last modified: Fri Feb 10 13:01:39 2023, max compression
+gzip compressed data, was "rxn-utils-1.2.0.tar", last modified: Fri Jul 28 13:29:26 2023, max compression
```

## Comparing `rxn-utils-1.1.9.tar` & `rxn-utils-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.685262 rxn-utils-1.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.685262 rxn-utils-1.1.9/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.685262 rxn-utils-1.1.9/src/rxn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/src/rxn/utilities/databases/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/databases/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/src/rxn/utilities/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/scripts/stable_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/src/rxn/utilities/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/src/rxn_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-10 13:01:39.000000 rxn-utils-1.1.9/src/rxn_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:01:39.689262 rxn-utils-1.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_databases_pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-10 13:01:29.000000 rxn-utils-1.1.9/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.737385 rxn-utils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-28 13:29:26.737385 rxn-utils-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-28 13:29:26.737385 rxn-utils-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.729385 rxn-utils-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.729385 rxn-utils-1.2.0/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.733385 rxn-utils-1.2.0/src/rxn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.733385 rxn-utils-1.2.0/src/rxn/utilities/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/databases/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.733385 rxn-utils-1.2.0/src/rxn/utilities/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/scripts/extract_csv_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/scripts/stable_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/src/rxn/utilities/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.733385 rxn-utils-1.2.0/src/rxn_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-28 13:29:26.000000 rxn-utils-1.2.0/src/rxn_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-28 13:29:26.000000 rxn-utils-1.2.0/src/rxn_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:29:26.000000 rxn-utils-1.2.0/src/rxn_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-28 13:29:26.000000 rxn-utils-1.2.0/src/rxn_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:29:26.000000 rxn-utils-1.2.0/src/rxn_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 13:29:26.000000 rxn-utils-1.2.0/src/rxn_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-28 13:29:26.000000 rxn-utils-1.2.0/src/rxn_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:29:26.737385 rxn-utils-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_databases_pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 13:29:16.000000 rxn-utils-1.2.0/tests/test_types.py
```

### Comparing `rxn-utils-1.1.9/LICENSE` & `rxn-utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/PKG-INFO` & `rxn-utils-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-utils
-Version: 1.1.9
+Version: 1.2.0
 Summary: General utilities (not related to chemistry)
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `rxn-utils-1.1.9/README.md` & `rxn-utils-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/setup.cfg` & `rxn-utils-1.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 	mypy>=0.910
 	pytest-cov>=2.8.1
 	pytest>=7.0.1
 	types-setuptools>=57.4.14
 
 [options.entry_points]
 console_scripts = 
+	rxn-extract-csv-column = rxn.utilities.scripts.extract_csv_column:main
 	rxn-stable-shuffle = rxn.utilities.scripts.stable_shuffle:main
 
 [flake8]
 extend-ignore = E203, E501
 
 [egg_info]
 tag_build =
```

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/attrs.py` & `rxn-utils-1.2.0/src/rxn/utilities/attrs.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/basic.py` & `rxn-utils-1.2.0/src/rxn/utilities/basic.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/caching.py` & `rxn-utils-1.2.0/src/rxn/utilities/caching.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/containers.py` & `rxn-utils-1.2.0/src/rxn/utilities/containers.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/databases/pymongo.py` & `rxn-utils-1.2.0/src/rxn/utilities/databases/pymongo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """PyMongo-related utilities."""
 import os
 from functools import lru_cache
 from typing import Any, Dict, Optional
 
 import pymongo
-from pydantic import BaseSettings, Extra
+from pydantic import Extra
 
+try:
+    # pydantic >= 2, requires the pydantic_settings package
+    from pydantic_settings import BaseSettings  # type: ignore[import,unused-ignore]
+except ImportError:
+    # pydantic < 2
+    from pydantic import BaseSettings  # type: ignore[no-redef,unused-ignore]
 
-class PyMongoSettings(BaseSettings):
+
+class PyMongoSettings(BaseSettings):  # type: ignore[misc,unused-ignore]
     """Settings for connecting to a MongoDB via pymongo."""
 
     mongo_uri: Optional[str] = None
     tls_ca_certificate_path: Optional[str] = None
 
     class Config:
         env_prefix = "RXN_"  # prefix for env vars to override defaults
```

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/files.py` & `rxn-utils-1.2.0/src/rxn/utilities/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import csv
 import errno
 import os
 import random
 import shutil
 import sys
 import tempfile
 from contextlib import ExitStack, contextmanager
@@ -135,14 +136,37 @@
         if delete and temporary_path.exists():
             if temporary_path.is_file():
                 temporary_path.unlink()
             else:
                 shutil.rmtree(temporary_path)
 
 
+@contextmanager
+def named_temporary_directory(delete: bool = True) -> Iterator[Path]:
+    """
+    Get the path for a temporary directory and create it.
+
+    Relies on ``named_temporary_path`` to provide a context manager that will
+    automatically delete the directory when leaving the context.
+
+    Args:
+        delete: whether to delete the file when exiting the context
+
+    Examples:
+        >>> with named_temporary_directory() as temporary_directory:
+        ...     # do something with the temporary directory.
+        ...     # The directory will be deleted at the
+        ...     # end of the context, except if delete=False.
+    """
+
+    with named_temporary_path(delete=delete) as path:
+        path.mkdir()
+        yield path
+
+
 def is_pathname_valid(pathname: PathLike) -> bool:
     """
     `True` if the passed pathname is a valid pathname for the current OS;
     `False` otherwise.
 
     Copied from https://stackoverflow.com/a/34102855. More details there.
     """
@@ -226,7 +250,42 @@
 
 def ensure_directory_exists_and_is_empty(directory: Path) -> None:
     """Create a directory if it does not exist already, and raise if not empty."""
     directory.mkdir(parents=True, exist_ok=True)
     directory_contains_files = any(directory.iterdir())
     if directory_contains_files:
         raise RuntimeError(f'The directory "{directory}" is required to be empty.')
+
+
+def iterate_csv_column(
+    csv_file: PathLike, column: str, delimiter: str = ","
+) -> Iterator[str]:
+    """
+    Iterate through a specific column of a CSV file.
+
+    The CSV file is iterated through one line at a time, so that the memory footprint
+    remains very small, even for large files.
+
+    Args:
+        csv_file: CSV file.
+        column: Column to iterate through.
+        delimiter: CSV delimiter.
+
+    Raises:
+        FileNotFoundError: if the file does not exist. Note: the exception is raised not
+            raised if the iterator is not consumed.
+        RuntimeError: if the column is not valid. Note: the exception is raised not
+            raised if the iterator is not consumed.
+
+    Returns:
+        iterator through the values in the selected column.
+    """
+    with open(csv_file, "rt") as f:
+        reader = csv.reader(f, delimiter=delimiter)
+
+        header = next(reader)
+        try:
+            column_index = header.index(column)
+        except ValueError:
+            raise RuntimeError(f'"{csv_file}" has no column "{column}".')
+
+        yield from (row[column_index] for row in reader)
```

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/logging.py` & `rxn-utils-1.2.0/src/rxn/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/misc.py` & `rxn-utils-1.2.0/src/rxn/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/regex.py` & `rxn-utils-1.2.0/src/rxn/utilities/regex.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/scripts/stable_shuffle.py` & `rxn-utils-1.2.0/src/rxn/utilities/scripts/stable_shuffle.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/strings.py` & `rxn-utils-1.2.0/src/rxn/utilities/strings.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn/utilities/types.py` & `rxn-utils-1.2.0/src/rxn/utilities/types.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/src/rxn_utils.egg-info/PKG-INFO` & `rxn-utils-1.2.0/src/rxn_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-utils
-Version: 1.1.9
+Version: 1.2.0
 Summary: General utilities (not related to chemistry)
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `rxn-utils-1.1.9/src/rxn_utils.egg-info/SOURCES.txt` & `rxn-utils-1.2.0/src/rxn_utils.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/rxn/utilities/py.typed
 src/rxn/utilities/regex.py
 src/rxn/utilities/strings.py
 src/rxn/utilities/types.py
 src/rxn/utilities/databases/__init__.py
 src/rxn/utilities/databases/pymongo.py
 src/rxn/utilities/scripts/__init__.py
+src/rxn/utilities/scripts/extract_csv_column.py
 src/rxn/utilities/scripts/stable_shuffle.py
 src/rxn_utils.egg-info/PKG-INFO
 src/rxn_utils.egg-info/SOURCES.txt
 src/rxn_utils.egg-info/dependency_links.txt
 src/rxn_utils.egg-info/entry_points.txt
 src/rxn_utils.egg-info/not-zip-safe
 src/rxn_utils.egg-info/requires.txt
```

### Comparing `rxn-utils-1.1.9/tests/test_attrs.py` & `rxn-utils-1.2.0/tests/test_attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     ]
 
 
 def test_get_variables_and_type_names() -> None:
     assert get_variables_and_type_names(DummyClass) == [
         ("variable_1", "float"),
         ("variable_2", "str"),
-        ("variable_3", "typing.Union[int, NoneType]"),
+        ("variable_3", "typing.Optional[int]"),
     ]
```

### Comparing `rxn-utils-1.1.9/tests/test_basic.py` & `rxn-utils-1.2.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/tests/test_caching.py` & `rxn-utils-1.2.0/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/tests/test_containers.py` & `rxn-utils-1.2.0/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/tests/test_databases_pymongo.py` & `rxn-utils-1.2.0/tests/test_databases_pymongo.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/tests/test_files.py` & `rxn-utils-1.2.0/tests/test_files.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 from rxn.utilities.files import (
     count_lines,
     dump_list_to_file,
     dump_tuples_to_files,
     ensure_directory_exists_and_is_empty,
     is_path_creatable,
+    iterate_csv_column,
     iterate_tuples_from_files,
     load_list_from_file,
+    named_temporary_directory,
     named_temporary_path,
     paths_are_identical,
     raise_if_paths_are_identical,
     stable_shuffle,
 )
 
 
@@ -57,14 +59,45 @@
         (path / "foo").mkdir()
         (path / "foo" / "bar").touch()
         (path / "foo.bar").touch()
         assert set(path.iterdir()) == {path / "foo", path / "foo.bar"}
     assert set(path.iterdir()) == {path / "foo", path / "foo.bar"}
 
 
+def test_named_temporary_directory() -> None:
+    # Basic checks - empty directory, deleted automatically
+    with named_temporary_directory() as path:
+        assert path.exists()
+        assert path.is_dir()
+        is_empty = not any(path.iterdir())
+        assert is_empty
+    assert not path.exists()
+
+    # create directory, without deleting it
+    with named_temporary_directory(delete=False) as path:
+        pass
+    assert path.exists()
+
+    # create directory with files and directories, make sure it is deleted
+    with named_temporary_directory() as path:
+        (path / "foo").mkdir()
+        (path / "foo" / "bar").touch()
+        (path / "foo.bar").touch()
+        assert set(path.iterdir()) == {path / "foo", path / "foo.bar"}
+    assert not path.exists()
+
+    # create directory with files and directories, without deleting
+    with named_temporary_directory(delete=False) as path:
+        (path / "foo").mkdir()
+        (path / "foo" / "bar").touch()
+        (path / "foo.bar").touch()
+        assert set(path.iterdir()) == {path / "foo", path / "foo.bar"}
+    assert set(path.iterdir()) == {path / "foo", path / "foo.bar"}
+
+
 def test_dump_and_load_list() -> None:
     original_list = ["some", "random", "words", " with", "    ", "spaces  "]
 
     with named_temporary_path() as tmp_path:
         dump_list_to_file(original_list, tmp_path)
         loaded_list = load_list_from_file(tmp_path)
 
@@ -203,7 +236,50 @@
         # Calling it a second time does nothing
         ensure_directory_exists_and_is_empty(path)
 
         # Creating a file inside it and calling it again -> will fail
         (path / "foo").touch()
         with pytest.raises(RuntimeError):
             ensure_directory_exists_and_is_empty(path)
+
+
+def test_iterate_csv_column() -> None:
+    path: Path
+    with named_temporary_path() as path:
+        # put the content of a CSV into path; five columns A, B, C, D:DD, and E.
+        dump_list_to_file(
+            [
+                "A,B,C,D:DD,E",
+                "a1,b1,c1,d1:41,1",
+                "a2,,c2,d2:42,2",
+                "a3,b3,,d3:43,3",
+                ",b4,c4,d4:44,4",
+            ],
+            path,
+        )
+
+        assert list(iterate_csv_column(path, "A")) == ["a1", "a2", "a3", ""]
+        assert list(iterate_csv_column(path, "B")) == ["b1", "", "b3", "b4"]
+        assert list(iterate_csv_column(path, "C")) == ["c1", "c2", "", "c4"]
+        assert list(iterate_csv_column(path, "D:DD")) == [
+            "d1:41",
+            "d2:42",
+            "d3:43",
+            "d4:44",
+        ]
+        assert list(iterate_csv_column(path, "E")) == ["1", "2", "3", "4"]
+
+        with pytest.raises(RuntimeError):
+            _ = list(iterate_csv_column(path, "F"))
+
+        with pytest.raises(FileNotFoundError):
+            _ = list(iterate_csv_column("invalid_file.csv", "A"))
+
+        # Use ":" as delimiter instead of ",". Now the columns are "A,B,C,D" and "DD,E".
+        with pytest.raises(RuntimeError):
+            _ = list(iterate_csv_column(path, "A", delimiter=":"))
+        assert list(iterate_csv_column(path, "DD,E", delimiter=":")) == [
+            "41,1",
+            "42,2",
+            "43,3",
+            "44,4",
+        ]
```

### Comparing `rxn-utils-1.1.9/tests/test_misc.py` & `rxn-utils-1.2.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/tests/test_regex.py` & `rxn-utils-1.2.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/tests/test_strings.py` & `rxn-utils-1.2.0/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `rxn-utils-1.1.9/tests/test_types.py` & `rxn-utils-1.2.0/tests/test_types.py`

 * *Files identical despite different names*

