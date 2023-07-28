# Comparing `tmp/code_data_science-1.0.1.1.tar.gz` & `tmp/code_data_science-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_data_science-1.0.1.1.tar", last modified: Tue Jul 25 01:56:28 2023, max compression
+gzip compressed data, was "code_data_science-1.1.0.tar", last modified: Fri Jul 28 18:19:35 2023, max compression
```

## Comparing `code_data_science-1.0.1.1.tar` & `code_data_science-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:28.416926 code_data_science-1.0.1.1/code_data_science/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/index_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/moderne_data_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/moderne_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/scm_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/sort_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/code_data_science.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.742563 code_data_science-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 18:19:35.742563 code_data_science-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-28 18:19:16.000000 code_data_science-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.734562 code_data_science-1.1.0/code_data_science/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.742563 code_data_science-1.1.0/code_data_science/clustering_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/datasets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/hf_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/clustering_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/data_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/index_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/moderne_data_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/moderne_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/scm_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-28 18:19:16.000000 code_data_science-1.1.0/code_data_science/sort_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:35.738563 code_data_science-1.1.0/code_data_science.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 18:19:35.000000 code_data_science-1.1.0/code_data_science.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-28 18:19:16.000000 code_data_science-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:19:35.742563 code_data_science-1.1.0/setup.cfg
```

### Comparing `code_data_science-1.0.1.1/code_data_science/moderne_data_grid.py` & `code_data_science-1.1.0/code_data_science/moderne_data_grid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from enum import Enum
 from pandas import DataFrame
 from IPython.display import display
 
+
 class ColumnType(str, Enum):
     """
     Enum for the column types supported by the moderne data grid
     """
     LINK = "link"
 
-def moderne_data_grid(df: DataFrame, columnTypes = None):
+
+def moderne_data_grid(df: DataFrame, column_types=None):
     """
     Converts the dataframe to a format that can be consumed by the moderne data grid.
     Calling this will result in the data frame passed being rendered as a moderne data grid on the dashboard
 
     You can also pass a dictionary where the keys are the column names and the values are the column types.
     To have greater control of how the data grid is rendered.
     """
@@ -21,12 +23,12 @@
     # Remove empty lines (likely to always be one at the end)
     csv_data = list(filter(None, csv_data))
 
     # Create the output dictionary
     output_data = {
         "application/vnd.moderne.datagrid+json": {
             "rows": csv_data,
-            "columnTypes": columnTypes
+            "columnTypes": column_types
         }
     }
 
-    display(output_data, raw=True)
+    display(output_data, raw=True)
```

### Comparing `code_data_science-1.0.1.1/code_data_science/moderne_palette.py` & `code_data_science-1.1.0/code_data_science/moderne_palette.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     'black': {
         100: '#1e1e1e',
         800: '#121212'
     }
 }
 
 
-def moderne_qualitative_palette(number=0):
+def moderne_qualitative_palette(number: int = 0):
     if number == 500:
         return [
             __moderneColorMap['blue'][500],
             __moderneColorMap['red'][500],
             __moderneColorMap['yellow'][500],
             __moderneColorMap['green'][500],
             __moderneColorMap['indigo'][500],
```

### Comparing `code_data_science-1.0.1.1/code_data_science/scm_link.py` & `code_data_science-1.1.0/code_data_science/scm_link.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-def _base_scm_link(scm_dictionary, origin, organization, repository) -> str:
+def _base_scm_link(scm_dictionary, origin: str, organization: str, repository: str) -> str:
     if origin in scm_dictionary and scm_dictionary[origin] == 'BitbucketConfiguration':
         return f"{origin}/projects/{organization}/repos/{repository}"
     else:
         return f"{origin}/{organization}/{repository}"
-    
 
-def scm_link(scm_dictionary, origin, organization, repository, committish, sourcePath, line):
+
+def scm_link(scm_dictionary, origin: str, organization: str, repository: str,
+             committish: str, source_path: str, line) -> str:
     """
     Generates a link to a repository's landing page specific to the SCM system it originated from
     """
     scheme = "https://"
     pathname = _base_scm_link(scm_dictionary, origin, organization, repository)
-    searchParams = ""
-    hash = ""
+    search_params = ""
+    url_hash = ""
 
     if origin in scm_dictionary and committish:
         if scm_dictionary[origin] == "GithubConfiguration":
-            pathname = '/'.join(filter(lambda x: bool(x), [pathname, 'blob' if sourcePath else 'tree', committish, sourcePath]))
+            pathname = '/'.join(
+                filter(lambda x: bool(x), [pathname, 'blob' if source_path else 'tree', committish, source_path]))
             if line:
-                hash = f"L{line}"
+                url_hash = f"L{line}"
         elif scm_dictionary[origin] == "BitbucketConfiguration":
-            pathname = '/'.join(filter(lambda x: bool(x), [pathname, 'browse', sourcePath]))
-            searchParams = f"?at={committish}"
+            pathname = '/'.join(filter(lambda x: bool(x), [pathname, 'browse', source_path]))
+            search_params = f"?at={committish}"
             if line:
-                hash = line
+                url_hash = line
         elif scm_dictionary[origin] == "BitbucketCloudConfiguration":
-            pathname = '/'.join(filter(lambda x: bool(x), [pathname, 'src', committish, sourcePath]))
+            pathname = '/'.join(filter(lambda x: bool(x), [pathname, 'src', committish, source_path]))
             if line:
-                hash = f"lines-{line}"
+                url_hash = f"lines-{line}"
         elif scm_dictionary[origin] == "GitLabConfiguration":
-            pathname = '/'.join(filter(lambda x: bool(x), [pathname, '-', 'blob', committish, sourcePath]))
+            pathname = '/'.join(filter(lambda x: bool(x), [pathname, '-', 'blob', committish, source_path]))
             if line:
-                hash = f"L{line}"
-    
-    return f"{scheme}{pathname}{searchParams}{'#' if hash else ''}{hash}"
+                url_hash = f"L{line}"
+
+    return f"{scheme}{pathname}{search_params}{'#' if url_hash else ''}{url_hash}"
```

### Comparing `code_data_science-1.0.1.1/code_data_science/sort_versions.py` & `code_data_science-1.1.0/code_data_science/sort_versions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import re
 
 
-def sort_versions(versions, metadata_pattern=None):
+def sort_versions(versions: [str], metadata_pattern: str = None) -> [str]:
     """
         Sort the versions in order from oldest to newest. Not every version must strictly adhere to Semver.
         :param versions: a list of versions to sort
         :param metadata_pattern: optionally, a metadata pattern like '-jre' in Google Guava versions
         :rtype array:
         >>> sort_versions(['1.1.1.1', '1.1.1.2'])
         ['1.1.1.1', '1.1.1.2']
@@ -18,55 +18,55 @@
 
     def metadata_compare(v1, v2):
         return compare_versions(v1, v2, metadata_pattern)
 
     return sorted(versions, key=functools.cmp_to_key(metadata_compare))
 
 
-def compare_versions(v1, v2, metadata_pattern=None):
+def compare_versions(v1: str, v2: str, metadata_pattern: str = None) -> int:
     nv1 = v1
     nv2 = v2
 
     vp1 = __count_version_parts(nv1)
     vp2 = __count_version_parts(nv2)
     len_diff = abs(vp1 - vp2)
     if v1 > v2:
         for i in range(1, len_diff):
             nv2 += ".0"
     elif v2 > v1:
         for i in range(1, len_diff):
             nv1 += ".0"
 
-    releasePattern = re.compile(r"(\d+)(?:\.(\d+))?(?:\.(\d+))?(?:\.(\d+))?(?:\.(\d+))?([-+].*)?")
-    v1Gav = releasePattern.match(nv1)
-    v2Gav = releasePattern.match(nv2)
+    release_pattern = re.compile(r"(\d+)(?:\.(\d+))?(?:\.(\d+))?(?:\.(\d+))?(?:\.(\d+))?([-+].*)?")
+    v1_gav = release_pattern.match(nv1)
+    v2_gav = release_pattern.match(nv2)
 
     normalized1 = nv1 if metadata_pattern is None else nv1.replace(metadata_pattern, "")
     normalized2 = nv2 if metadata_pattern is None else nv2.replace(metadata_pattern, "")
 
     for i in range(1, max(vp1, vp2)):
-        v1Part = v1Gav.group(i)
-        v2Part = v2Gav.group(i)
-        if v1Part is None:
-            return normalized1.compareTo(normalized2) if v2Part is None else -1
-        elif v2Part is None:
+        v1_part = v1_gav.group(i)
+        v2_part = v2_gav.group(i)
+        if v1_part is None:
+            return compare_versions(normalized1, normalized2) if v2_part is None else -1
+        elif v2_part is None:
             return 1
-        diff = int(v1Part) - int(v2Part)
+        diff = int(v1_part) - int(v2_part)
         if diff != 0:
             return diff
 
     if normalized1 == normalized2:
         return 0
     elif normalized1 > normalized2:
         return 1
     else:
         return -1
 
 
-def __normalize_version(v) -> str:
+def __normalize_version(v: str) -> str:
     """
     Remove RELEASE and FINAL suffixes and make sure there are at least three parts to the version.
     :param v:
     :return: str:
     >>> __normalize_version("1.5.1.2.RELEASE")
     '1.5.1.2'
     >>> __normalize_version("1.5.1.RELEASE")
@@ -94,14 +94,14 @@
             version_and_metadata[0] += ".0"
             version_parts += 1
         return version_and_metadata[0] + (version_and_metadata[1] if len(version_and_metadata) > 1 else "")
 
     return v
 
 
-def __count_version_parts(v) -> int:
+def __count_version_parts(v: str) -> int:
     count = 0
     for part in re.split(r"[.\-$]", v):
         if len(part) == 0 or not (part[0].isdigit()):
             break
         count += 1
     return count
```

### Comparing `code_data_science-1.0.1.1/pyproject.toml` & `code_data_science-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "code_data_science"
-version = "1.0.1.1"
+version = "1.1.0"
 description = "A python implementation of various tools used in code data science."
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io"},
     { name = "Kyle Scully", email = "kyle@moderne.io"}
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
```

