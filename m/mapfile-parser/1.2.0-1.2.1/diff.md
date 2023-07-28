# Comparing `tmp/mapfile_parser-1.2.0.tar.gz` & `tmp/mapfile_parser-1.2.1.tar.gz`

## Comparing `mapfile_parser-1.2.0.tar` & `mapfile_parser-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.gitattributes
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/mypy.ini
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/requirements.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.github/workflows/upload_pypi.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/__main__.py
--rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/mapfile.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/progress_stats.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/utils.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/__init__.py
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/first_diff.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/pj64_syms.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/progress.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/sym_info.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/symbol_sizes_csv.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/upload_frogress.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/LICENSE
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.gitattributes
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/mypy.ini
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/requirements.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.github/workflows/upload_pypi.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/__main__.py
+-rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/mapfile.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/progress_stats.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/utils.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/__init__.py
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/first_diff.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/pj64_syms.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/progress.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/sym_info.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/symbol_sizes_csv.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/src/mapfile_parser/frontends/upload_frogress.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 mapfile_parser-1.2.1/PKG-INFO
```

### Comparing `mapfile_parser-1.2.0/.github/workflows/mypy.yml` & `mapfile_parser-1.2.1/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/.github/workflows/upload_pypi.yml` & `mapfile_parser-1.2.1/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/__main__.py` & `mapfile_parser-1.2.1/src/mapfile_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/mapfile.py` & `mapfile_parser-1.2.1/src/mapfile_parser/mapfile.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/progress_stats.py` & `mapfile_parser-1.2.1/src/mapfile_parser/progress_stats.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/utils.py` & `mapfile_parser-1.2.1/src/mapfile_parser/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return bytearray(0)
     with filepath.open(mode="rb") as f:
         return bytearray(f.read())
 
 def hexbytes(bs: bytes, addColons: bool=True) -> str:
     glue = ""
     if addColons:
-        glue = ""
+        glue = ":"
     return glue.join("{:02X}".format(c) for c in bs)
 
 def getGitCommitTimestamp() -> int:
     return int(subprocess.check_output(['git', 'show', '-s', '--format=%ct']).decode('ascii').rstrip())
 
 def getGitCommitHash() -> str:
     return subprocess.check_output(['git', 'rev-parse', 'HEAD']).decode('ascii').strip()
```

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/frontends/first_diff.py` & `mapfile_parser-1.2.1/src/mapfile_parser/frontends/first_diff.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/frontends/pj64_syms.py` & `mapfile_parser-1.2.1/src/mapfile_parser/frontends/pj64_syms.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/frontends/progress.py` & `mapfile_parser-1.2.1/src/mapfile_parser/frontends/progress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/frontends/sym_info.py` & `mapfile_parser-1.2.1/src/mapfile_parser/frontends/sym_info.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/frontends/symbol_sizes_csv.py` & `mapfile_parser-1.2.1/src/mapfile_parser/frontends/symbol_sizes_csv.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/src/mapfile_parser/frontends/upload_frogress.py` & `mapfile_parser-1.2.1/src/mapfile_parser/frontends/upload_frogress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/.gitignore` & `mapfile_parser-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/LICENSE` & `mapfile_parser-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/README.md` & `mapfile_parser-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.2.0/pyproject.toml` & `mapfile_parser-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: © 2022 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "mapfile_parser"
-version = "1.2.0"
+version = "1.2.1"
 description = "Map file parser library focusing decompilation projects"
 readme = "README.md"
 requires-python = ">=3.7"
 dynamic = ["dependencies"]
 
 [project.urls]
 "Homepage" = "https://github.com/Decompollaborate/mapfile_parser"
```

### Comparing `mapfile_parser-1.2.0/PKG-INFO` & `mapfile_parser-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfile_parser
-Version: 1.2.0
+Version: 1.2.1
 Summary: Map file parser library focusing decompilation projects
 Project-URL: Homepage, https://github.com/Decompollaborate/mapfile_parser
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/mapfile_parser/issues
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: requests
 Description-Content-Type: text/markdown
```

