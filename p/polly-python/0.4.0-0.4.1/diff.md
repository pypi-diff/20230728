# Comparing `tmp/polly-python-0.4.0.tar.gz` & `tmp/polly-python-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polly-python-0.4.0.tar", last modified: Fri Jul 21 07:08:24 2023, max compression
+gzip compressed data, was "polly-python-0.4.1.tar", last modified: Fri Jul 28 09:18:58 2023, max compression
```

## Comparing `polly-python-0.4.0.tar` & `polly-python-0.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-21 07:07:10.000000 polly-python-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-21 07:07:10.000000 polly-python-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 07:08:24.615474 polly-python-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-21 07:07:10.000000 polly-python-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/polly/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/application_error_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/bridge_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/core_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    35626 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/http_response_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/index_schema_level_conversion_const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)   198377 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    74348 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/omixatlas_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/validation_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-07-21 07:07:10.000000 polly-python-0.4.0/polly/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/polly_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:08:24.000000 polly-python-0.4.0/polly_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 07:07:10.000000 polly-python-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-21 07:08:24.615474 polly-python-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:07:10.000000 polly-python-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:08:24.615474 polly-python-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98539 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_schema_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-21 07:07:10.000000 polly-python-0.4.0/tests/test_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:18:58.047489 polly-python-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-28 09:17:23.000000 polly-python-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 09:17:23.000000 polly-python-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-28 09:18:58.047489 polly-python-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-28 09:17:23.000000 polly-python-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:18:58.047489 polly-python-0.4.1/polly/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/application_error_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/bridge_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/core_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35626 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/http_response_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/index_schema_level_conversion_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198377 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74348 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/omixatlas_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/validation_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-07-28 09:17:23.000000 polly-python-0.4.1/polly/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:18:58.047489 polly-python-0.4.1/polly_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-28 09:18:58.000000 polly-python-0.4.1/polly_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 09:18:58.000000 polly-python-0.4.1/polly_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:18:58.000000 polly-python-0.4.1/polly_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-28 09:18:58.000000 polly-python-0.4.1/polly_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 09:18:58.000000 polly-python-0.4.1/polly_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 09:17:23.000000 polly-python-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-28 09:18:58.051489 polly-python-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:17:23.000000 polly-python-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:18:58.047489 polly-python-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98529 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_schema_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-28 09:17:23.000000 polly-python-0.4.1/tests/test_workspaces.py
```

### Comparing `polly-python-0.4.0/LICENSE.md` & `polly-python-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/PKG-INFO` & `polly-python-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.4.0
+Version: 0.4.1
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `polly-python-0.4.0/README.md` & `polly-python-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/analyze.py` & `polly-python-0.4.1/polly/analyze.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from polly.errors import paramException
 from polly.tracking import Track
 from polly import omixatlas_hlpr
 from polly.constants import (
     COHORT_SUPPORTED_DATATYPES,
     COHORT_SUPPORTED_DATASOURCES,
     COHORT_LIST_COLS_TO_DROP,
+    MA_SUPPORTED_REPO,
 )
 
 import pandas as pd
 import plotly.express as px
 import json
 import numpy as np
 
@@ -50,31 +51,26 @@
         """
         This function is used to get the cohorts that can be created from samples in a GEO dataset.
         Please note: Currently only Bulk RNASeq datasets from GEO source are supported.
         If results are generated for other datatypes or datasource, they may be inaccurate.
         If you want to use this functionality for any other data type and source,
         please reach out to polly.support@elucidata.io
 
-        If you want to plot a sunburst on specific columns of interest, please use the following code:
-        ` import plotly.express as px`
-        ` metadata = identify_cohorts(repo_key, dataset_id)`
-        ` fig = px.sunburst(metadata, path=['column_1','column_2','column_n'])`
-        ` fig.show()`
-
         Args:
             repo_key (int/str): repo_id or repo_name in str or int format
             dataset_id (str): dataset_id of the GEO dataset. eg. "GSE132270_GPL11154_raw"
         Returns:
             Dataframe showing values of samples across factors/cohorts.
         """
         # param checks
         omixatlas_hlpr.parameter_check_for_dataset_id(dataset_id)
         omixatlas_hlpr.parameter_check_for_repo_id(repo_key)
         repo_key = omixatlas_hlpr.make_repo_id_string(repo_key)
 
+        # TO DO: get_metadata() for dataset level in omixatlas.py and call that here
         # Get dataset level metadata and check if datatype is supported
         response_omixatlas = self.omixatlas_obj.omixatlas_summary(repo_key)
         data = response_omixatlas.get("data", "")
         index_name = data.get("indexes", {}).get("files", "")
         if index_name is None:
             raise paramException(
                 title="Param Error", detail="Repo entered is not an omixatlas."
@@ -207,14 +203,26 @@
             design_formula (dict): design_formula_control or design_formula_perturbation
 
         Returns:
             list: list of sample_ids that are either control or perturbation
         """
         sample_ids = []
         for column, value in design_formula.items():
+            # Check if the user-provided column exists in the DataFrame
+            if column not in col_metadata_df.columns:
+                raise paramException(
+                    title="Param Error",
+                    detail=f"Column '{column}' does not exist in the DataFrame.",
+                )
+            # Check if the user-provided value exists in the given column
+            if value not in col_metadata_df[column].values:
+                raise paramException(
+                    title="Param Error",
+                    detail=f"Value '{value}' does not exist in column '{column}'",
+                )
             # Boolean values list for samples in df if column == value
             sample_filter = col_metadata_df[column] == value
             # Add sublists to list with boolean values for each condition
             sample_ids.append([sample_filter])
         # Logical AND of all bool values in sublist
         sample_ids = np.all(sample_ids, axis=0)
         # Get sample IDs corresponding to logical AND indices
@@ -234,14 +242,23 @@
 
         Returns:
             DataFrame: cohort df with three columns ['dataset_id', 'sample_id', 'kw_condition']\
             'kw_condition' has value 'control' or 'perturbation' based on the design formula.
         """
         col_metadata = self.omixatlas_obj.get_metadata(repo_key, dataset_id, "samples")
 
+        # Convert curated columns to string so that input values can be compared directly
+        for column in col_metadata.columns:
+            # Check if column contains lists (curated columns do)
+            if col_metadata[column].apply(lambda x: isinstance(x, list)).any():
+                # Convert lists to strings
+                col_metadata[column] = col_metadata[column].apply(
+                    lambda x: "[" + ", ".join(x) + "]" if isinstance(x, list) else x
+                )
+
         # Create design formula dataframe for this dataset ID
         cohort_df = pd.DataFrame(columns=["dataset_id", "sample_id", "kw_condition"])
         cohort_df["sample_id"] = col_metadata["geo_accession"]
         cohort_df["dataset_id"] = dataset_id
 
         # Extract control and perturbation sample IDs
         control_ids = self._get_control_perturbation_ids(
@@ -268,40 +285,83 @@
         workspace_id: int,
         analysis_name: str,
         design_formulas: dict,
         samples_to_remove=[],
     ):
         """
         Use this function to execute the Polly DIY Meta-Analysis Pipeline.
+        Only the 'geo_transcriptomics_omixatlas' omixatlas is supported currently.
         Args:
             repo_key (int/str): repo_id or repo_name in str or int format
             workspace_id (int): the workspace in which the datasets and results should be stored
             analysis_name (str): name of your analysis, eg. "MA_BRCA_run1".\
             The reports, datasets, and results will be stored in a folder with this name.
-            design_formulas (dict): key:value pair of atleast 5 dataset ids and a list of design formulas.\
+            design_formulas (dict): key:value pair of atleast 2 dataset ids and a list of design formulas.\
             eg. dataset_id:[design formula control, design formula perturbation]
             samples_to_remove (list, optional): List of samples to omit, if any. Defaults to [].
         """
         dataset_ids = list(design_formulas.keys())
 
         # param checks
         omixatlas_hlpr.parameter_check_for_list_dataset_ids(dataset_ids)
+        if len(dataset_ids) < 2:
+            raise paramException(
+                title="Param Error",
+                detail="Design formula should contain atleast two datasets.",
+            )
         omixatlas_hlpr.parameter_check_for_repo_id(repo_key)
         repo_key = omixatlas_hlpr.make_repo_id_string(repo_key)
+        if repo_key not in MA_SUPPORTED_REPO:
+            raise paramException(
+                title="Param Error",
+                detail="Only the 'geo_transcriptomics_omixatlas' omixatlas is supported currently.",
+            )
         omixatlas_hlpr.str_params_check([analysis_name])
 
         # parse design formula to get cohort df
         cohort_dfs = []
         for dataset, design_formula in design_formulas.items():
+            # Check if user has specified both control and perturbation in the list
+            if len(design_formula) != 2:
+                raise paramException(
+                    title="Param Error",
+                    detail=f"""Design formula for dataset_id '{dataset}' should have length
+                    two with one dictionary for control and perturbation each.""",
+                )
+            # Check if user has specified both control and perturbation in the list
+            if design_formula[0] == design_formula[1]:
+                raise paramException(
+                    title="Param Error",
+                    detail=f"Control and perturbation dictionaries for dataset_id '{dataset}' cannot be the same.",
+                )
             df = self._parse_design_formula(repo_key, dataset, design_formula)
             cohort_dfs.append(df)
         cohort_df = pd.concat(cohort_dfs)
 
-        # remove samples from above df if any
-        cohort_df = cohort_df[~cohort_df["sample_id"].isin(samples_to_remove)]
+        if samples_to_remove:
+            # Check if samples_to_remove is not a list
+            if not (samples_to_remove and isinstance(samples_to_remove, list)):
+                raise paramException(
+                    title="Param Error",
+                    detail="'samples_to_remove' should be list of strings",
+                )
+            # Check if any samples in 'samples_to_remove' are not present in the DataFrame's index
+            invalid_samples = [
+                sample
+                for sample in samples_to_remove
+                if sample not in cohort_df["sample_id"].tolist()
+            ]
+            if invalid_samples:
+                raise paramException(
+                    title="Param Error",
+                    detail=f"The following samples are not present in the DataFrame: {invalid_samples}",
+                )
+            # remove samples from above df if any
+            cohort_df = cohort_df[~cohort_df["sample_id"].isin(samples_to_remove)]
+
         print("Cohort csv file created from the design formulae.")
 
         # save cohort df as csv to workspace
         cohort_csv_path = analysis_name + "_cohorts.csv"
         cohort_df.to_csv(cohort_csv_path, sep="\t")
         self.workspace_obj.upload_to_workspaces(
             workspace_id, cohort_csv_path, cohort_csv_path
```

### Comparing `polly-python-0.4.0/polly/application_error_info.py` & `polly-python-0.4.1/polly/application_error_info.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/auth.py` & `polly-python-0.4.1/polly/auth.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/bridge_cohort.py` & `polly-python-0.4.1/polly/bridge_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/cohort.py` & `polly-python-0.4.1/polly/cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/constants.py` & `polly-python-0.4.1/polly/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "curated_cohort_id",
     "curated_cohort_name",
     "curated_is_control",
     "curated_max_age",
     "curated_min_age",
     "curated_age_unit",
 ]
+MA_SUPPORTED_REPO = ["geo_transcriptomics_omixatlas"]
 
 # validation flow files url github
 VALIDATION_FLOW_FILES_URL = (
     "https://raw.githubusercontent.com/ElucidataInc/PublicAssets/master/"
     + "internal-user/validation_full_flow_files"
 )
```

### Comparing `polly-python-0.4.0/polly/core_cohort.py` & `polly-python-0.4.1/polly/core_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/curation.py` & `polly-python-0.4.1/polly/curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/errors.py` & `polly-python-0.4.1/polly/errors.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/help.py` & `polly-python-0.4.1/polly/help.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/helpers.py` & `polly-python-0.4.1/polly/helpers.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/http_response_codes.py` & `polly-python-0.4.1/polly/http_response_codes.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/jobs.py` & `polly-python-0.4.1/polly/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 class jobs:
 
     """
     The polly_jobs class contains functions which can be used to create, cancel and monitor polly jobs.
     Polly CLI jobs can now be initiated, managed and have a status-checked for from Polly Python.
     This lets users run jobs on the Polly cloud infrastructure by scaling computation resources as per need.
     Users can start and stop tasks and even monitor jobs.
+
+    Note:- User must use TOKEN instead of KEYS to work with the job module of polly-python.
+
     Args:
         token (str): token copy from polly.
     Usage:
         from polly.jobs import jobs
 
         jobs = jobs(token)
     """
@@ -57,34 +60,53 @@
         self.session = Polly.get_session(token, env=env)
         self.base_url = f"https://v2.api.{self.session.env}.elucidata.io"
         self.discover_url = f"https://api.discover.{self.session.env}.elucidata.io"
 
     # project_id -> workspace_id
     # job_file -> json file
     @Track.track_decorator
-    def submit_job(self, project_id: str, job_file: str) -> pd.DataFrame:
+    def submit_job(self, project_id: str, job_file=None, job_dict=None) -> pd.DataFrame:
         """
         Submits  a polly cli job in the given workspace.
         A message will be displayed on the status of the operation.
+        Job configuration can be provided either as a json file using job_file parameter or
+        as a dictionary using job_dict parameter
 
         Args:
             project_id (str):  workspace id
-            job_file (str): required configuration json file path
+            job_file (str, optional) : job configuration json file path, defaults to None
+            job_dict (dict, optional) : job configuration dictionary, defaults to None
         """
         parameter_check_dict = {}
+
         parameter_check_dict["project_id"] = project_id
-        parameter_check_dict["job_file"] = job_file
+        # neither both job_file and job_dict should be provided, nor both should not be provided.
+        # only one of the two should be provided
+        if (job_file is None and job_dict is None) or (job_file and job_dict):
+            raise InvalidParameterException(
+                "One of json_file or json_dict required for the function."
+                + "Either both or none have been provided.Please check"
+            )
+        if job_file:
+            parameter_check_dict["job_file"] = job_file
+        if job_dict:
+            parameter_check_dict["job_dict"] = job_dict
+
         self._parameter_check_for_jobs(parameter_check_dict)
         if isinstance(project_id, int):
             project_id = str(project_id)
 
         try:
-            with open(job_file, "r") as jobfile:
-                jobData = json.load(jobfile)
-                # self._validate_job_json(jobData)
+            if job_file:
+                with open(job_file, "r") as jobfile:
+                    jobData = json.load(jobfile)
+                    # self._validate_job_json(jobData)
+            else:
+                jobData_json_string = json.dumps(job_dict)
+                jobData = json.loads(jobData_json_string)
         except Exception as err:
             raise err
 
         # TODO: add file validation for json
         jobData = self._add_secret_env_keys_to_jobData(jobData, project_id)
         job_post_data = self._submit_job_to_polly(project_id, jobData)
         submittedProject_df = ""
@@ -570,28 +592,38 @@
             if keys == "project_id":
                 project_id = values
                 if not (
                     project_id
                     and (isinstance(project_id, str) or isinstance(project_id, int))
                 ):
                     raise InvalidParameterException("project id/workspace id")
-            elif keys == "job_file":
-                job_file = values
-                if not (job_file):
-                    raise InvalidParameterException("job_file")
-                if not os.path.exists(job_file):
-                    raise InvalidPathException(job_file)
+            elif keys in ["job_file", "job_dict"]:
+                self._check_job_configuration_parameter(keys, values)
             elif keys == "job_id":
                 job_id = values
                 self._check_job_id(job_id, project_id)
             elif keys == "mode":
                 mode = values
                 if mode not in DATA_LOG_MODES:
                     raise InvalidParameterException(
                         f"valid mode values are : {DATA_LOG_MODES}"
                     )
 
+    def _check_job_configuration_parameter(
+        self, job_config_param_key, job_config_param_value
+    ):
+        if job_config_param_key == "job_file":
+            job_file = job_config_param_value
+            if not os.path.exists(job_file):
+                raise InvalidPathException(job_file)
+        elif job_config_param_key == "job_dict":
+            job_dict = job_config_param_value
+            if not (isinstance(job_dict, dict)):
+                raise InvalidParameterException(
+                    "job_dict should be a dictionary datatype"
+                )
+
     def _check_job_id(self, job_id, project_id):
         if not (job_id and (isinstance(job_id, str))):
             raise InvalidParameterException("Missing/invalid datatype for job id")
         if not self._is_valid_job_id(project_id, job_id):
             raise InvalidJobFunctionParameterException("Job id")
```

### Comparing `polly-python-0.4.0/polly/omixatlas.py` & `polly-python-0.4.1/polly/omixatlas.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/omixatlas_hlpr.py` & `polly-python-0.4.1/polly/omixatlas_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/schema.py` & `polly-python-0.4.1/polly/schema.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/session.py` & `polly-python-0.4.1/polly/session.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/tracking.py` & `polly-python-0.4.1/polly/tracking.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/validation.py` & `polly-python-0.4.1/polly/validation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/validation_hlpr.py` & `polly-python-0.4.1/polly/validation_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly/workspaces.py` & `polly-python-0.4.1/polly/workspaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
     This class contains functions to interact with workspaces on Polly. Users can create a workspace, fetch list\
  of workspaces, upload data to workspace and download data from workspace. To get started, users need to \
 initialize a object that can use all function and methods of Workspaces class.
     Args:
         token (str): Authentication token from polly
     Usage:
-        from polly.Workspaces import Workspaces
+        from polly.workspaces import Workspaces
 
         workspaces = Workspaces(token)
     """
 
     example = classmethod(example)
 
     def __init__(self, token=None, env="", default_env="polly") -> None:
```

### Comparing `polly-python-0.4.0/polly_python.egg-info/PKG-INFO` & `polly-python-0.4.1/polly_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.4.0
+Version: 0.4.1
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `polly-python-0.4.0/polly_python.egg-info/SOURCES.txt` & `polly-python-0.4.1/polly_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/polly_python.egg-info/requires.txt` & `polly-python-0.4.1/polly_python.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/setup.cfg` & `polly-python-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/tests/test_cohort.py` & `polly-python-0.4.1/tests/test_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/tests/test_constants.py` & `polly-python-0.4.1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/tests/test_curation.py` & `polly-python-0.4.1/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/tests/test_jobs.py` & `polly-python-0.4.1/tests/test_jobs.py`

 * *Files 16% similar despite different names*

```diff
@@ -112,22 +112,29 @@
         TypeError,
         match=r"path should be string, bytes, os.PathLike or integer, not list",
     ):
         jobs_obj.submit_job(valid_workspace_id, invalid_file_path_type)
 
 
 # @pytest.mark.skip(reason="no way of currently testing this")
-def test_submit_job_invalid_json(mocker, get_job_submission_json_file, capsys):
+def test_submit_job_invalid_json(
+    mocker, get_job_submission_json_file, get_jobData_with_secret_env_keys, capsys
+):
     # valid_input_json_file = "/Users/shilpanair/workspace/dev_test_files/jobs_work/test_job.json"
     valid_input_json_file = get_job_submission_json_file
     valid_workspace_id = 12345
     # internally called fuction _submit_job_to_polly returns a response object - creating a mock of the response object
     # patching the mock response object when _submit_job_to_polly is called
 
     mocker.patch(
+        polly.jobs.__name__ + ".jobs._add_secret_env_keys_to_jobData",
+        return_value=get_jobData_with_secret_env_keys,
+    )
+
+    mocker.patch(
         polly.jobs.__name__ + ".jobs._submit_job_to_polly",
         side_effect=Exception(
             "Either cpu and memory or machineType should be specified', "
             + "'Server could not understand the request due to invalid syntax"
         ),
     )
     # calling the function under test
@@ -139,23 +146,32 @@
     ):
         jobs_obj.submit_job(valid_workspace_id, valid_input_json_file)
         captured = capsys.readouterr()
         assert "Not able to submit job" in captured.out
 
 
 # @pytest.mark.skip(reason="no way of currently testing this")
-def test_submit_job_invalid_workspace_id(mocker, get_job_submission_json_file, capsys):
+def test_submit_job_invalid_workspace_id(
+    mocker, get_job_submission_json_file, get_jobData_with_secret_env_keys, capsys
+):
     Polly.auth(testpolly_token, env="testpolly")
     jobs_obj = jobs.jobs()
     valid_input_json_file = get_job_submission_json_file
     invalid_workspace_id_1 = "abcdwef"
     invalid_workspace_id_2 = "00000000"
+
+    mocker.patch(
+        polly.jobs.__name__ + ".jobs._add_secret_env_keys_to_jobData",
+        return_value=get_jobData_with_secret_env_keys,
+    )
+
     # case 1: where the project_id/workspace_id is not of valid type (should be numeric)
     Polly.auth(testpolly_token, env="testpolly")
     jobs_obj = jobs.jobs()
+
     mocker.patch(
         polly.jobs.__name__ + ".jobs._submit_job_to_polly",
         side_effect=Exception("Bad Request', 'Project ID - abcdwef should be numeric"),
     )
     # calling the function under test
     with pytest.raises(
         Exception,
@@ -253,7 +269,101 @@
 
     jobs_obj.cancel_job(valid_workspace_id, invalid_job_id)
     captured = capsys.readouterr()
     assert (
         "Failed to cancel the job.: Cannot cancel a job in CANCELLED state"
         in captured.out
     )
+
+
+def test_job_status(mocker, get_jobData_with_secret_env_keys):
+    valid_workspace_id = 12345
+    valid_job_id = f"{random.randrange(16**32):032x}"
+    Polly.auth(testpolly_token, env="testpolly")
+    jobs_obj = jobs.jobs()
+    # internally called fuction _submit_job_to_polly returns a response object - creating a mock of the response object
+    mocker.patch(
+        polly.jobs.__name__ + ".jobs._add_secret_env_keys_to_jobData",
+        return_value=get_jobData_with_secret_env_keys,
+    )
+    mocker.patch(
+        polly.jobs.__name__ + ".jobs._parameter_check_for_jobs",
+        return_value=None,
+    )
+    mock_response = MagicMock()
+    mock_response.status_code = 200
+    mock_response.json.return_value = {
+        "data": [
+            {
+                "type": "jobs",
+                "id": valid_job_id,
+                "attributes": {
+                    "job_name": "This is a job for testing bust mode",
+                    "started_ts": 1666346315947,
+                    "creator_id": 1663209871,
+                    "log_ids": ["random_log_id"],
+                    "project_id": valid_workspace_id,
+                    "config_json": {
+                        "cpu": "1",
+                        "memory": "1Gi",
+                        "image": "ubuntu",
+                        "tag": "latest",
+                        "machineType": "null",
+                        "cloud_provider": "aws",
+                        "timelimit": 12,
+                        "command": [
+                            "/bin/bash",
+                            "-c",
+                            "TERM=xterm free -h; echo '\nnumber of vCPU';nproc;sleep 30",
+                        ],
+                    },
+                    "job_id": "valid_job_id",
+                    "ended_ts": 1666346361960,
+                    "session_info": [
+                        {
+                            "log_id": "14832-20c139ae6925438ba670fdac6175b4c4-776133615_compute-test_main",
+                            "ended_ts": 1666346361960,
+                            "state": "Success",
+                            "started_ts": 1666346315947,
+                        }
+                    ],
+                    "created_ts": 1666346311500,
+                    "state": "Success",
+                },
+            }
+        ]
+    }
+    # patching the mock response object when _submit_job_to_polly is called
+    mocker.patch(
+        polly.jobs.__name__ + ".jobs._get_data_for_job_id",
+        return_value=mock_response,
+    )
+    Polly.auth(testpolly_token, env="testpolly")
+    jobs_obj = jobs.jobs()
+    output = jobs_obj.job_status(valid_workspace_id, valid_job_id)
+    assert type(output) is pd.DataFrame
+    assert output.iloc[0]["Job State"] == "Success"
+
+
+def test_job_status_invalid_job_id(mocker, get_jobData_with_secret_env_keys):
+    valid_workspace_id = 12345
+    Polly.auth(testpolly_token, env="testpolly")
+    jobs_obj = jobs.jobs()
+    # internally called fuction _submit_job_to_polly returns a response object - creating a mock of the response object
+    mocker.patch(
+        polly.jobs.__name__ + ".jobs._add_secret_env_keys_to_jobData",
+        return_value=get_jobData_with_secret_env_keys,
+    )
+    invalid_job_id = "1234"
+    valid_workspace_id = 12345
+    mocker.patch(
+        polly.jobs.__name__ + ".jobs._check_job_id",
+        side_effect=InvalidJobFunctionParameterException(
+            "The specified  job_id could not be found. Inspect and try again."
+        ),
+    )
+    with pytest.raises(
+        InvalidJobFunctionParameterException,
+        match=r"The specified The specified  job_id could not be found."
+        + " Inspect and try again. could not be found. Inspect and try again.",
+    ):
+        jobs_obj.job_status(valid_workspace_id, invalid_job_id)
```

### Comparing `polly-python-0.4.0/tests/test_omixatlas.py` & `polly-python-0.4.1/tests/test_omixatlas.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     assert nobj._get_omixatlas(key)["data"] is not None
 
 
 def test_omixatlas_summary():
     Polly.auth(token)
     nobj1 = omixatlas.OmixAtlas()
     obj1 = omixatlas.OmixAtlas(token)
-    key = "elucidata.liveromix_atlas"
+    key = "liveromix_atlas"
     assert obj1.omixatlas_summary(key)["data"] is not None
     assert nobj1.omixatlas_summary(key)["data"] is not None
 
 
 def test_download_data(mocker):
     # mocking session response of {self.resource_url}/{repo_name}/download api call -> positive scenario
     obj = omixatlas.OmixAtlas(testpolly_token, env="testpolly")
```

### Comparing `polly-python-0.4.0/tests/test_schema_ux.py` & `polly-python-0.4.1/tests/test_schema_ux.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.4.0/tests/test_workspaces.py` & `polly-python-0.4.1/tests/test_workspaces.py`

 * *Files identical despite different names*

