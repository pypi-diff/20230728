# Comparing `tmp/saiph-1.4.4.tar.gz` & `tmp/saiph-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saiph-1.4.4.tar", max compression
+gzip compressed data, was "saiph-1.4.5.tar", max compression
```

## Comparing `saiph-1.4.4.tar` & `saiph-1.4.5.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     9861 2023-01-26 13:33:30.598429 saiph-1.4.4/LICENSE
--rw-r--r--   0        0        0     2270 2023-01-26 13:33:30.602429 saiph-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      286 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/__init__.py
--rw-r--r--   0        0        0     4441 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/conftest.py
--rw-r--r--   0        0        0     1195 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/contribution.py
--rw-r--r--   0        0        0     1384 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/contribution_test.py
--rw-r--r--   0        0        0      119 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/exception.py
--rw-r--r--   0        0        0     6789 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/inverse_transform.py
--rw-r--r--   0        0        0     8613 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/inverse_transform_test.py
--rw-r--r--   0        0        0      410 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/lib/size.py
--rw-r--r--   0        0        0     2479 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/models.py
--rw-r--r--   0        0        0     8300 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/projection.py
--rw-r--r--   0        0        0    11890 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/projection_test.py
--rw-r--r--   0        0        0       27 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/__init__.py
--rw-r--r--   0        0        0    15243 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/famd.py
--rw-r--r--   0        0        0     4560 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/famd_sparse.py
--rw-r--r--   0        0        0     4888 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/famd_sparse_test.py
--rw-r--r--   0        0        0     8519 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/famd_test.py
--rw-r--r--   0        0        0     9228 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/mca.py
--rw-r--r--   0        0        0     6875 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/mca_test.py
--rw-r--r--   0        0        0     4251 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/pca.py
--rw-r--r--   0        0        0     3829 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/pca_test.py
--rw-r--r--   0        0        0        0 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/utils/__init__.py
--rw-r--r--   0        0        0     3825 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/utils/common.py
--rw-r--r--   0        0        0     2457 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/utils/common_test.py
--rw-r--r--   0        0        0     4642 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/utils/svd.py
--rw-r--r--   0        0        0     5005 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/reduction/utils/svd_test.py
--rw-r--r--   0        0        0     5172 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/serializer.py
--rw-r--r--   0        0        0     1919 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/serializer_test.py
--rw-r--r--   0        0        0        0 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/tests/__init_.py
--rw-r--r--   0        0        0     1402 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/tests/benchmark_test.py
--rw-r--r--   0        0        0      521 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/tests/profile_cpu.py
--rw-r--r--   0        0        0      983 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/tests/profile_memory.py
--rw-r--r--   0        0        0     5405 2023-01-26 13:33:30.602429 saiph-1.4.4/saiph/visualization.py
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 saiph-1.4.4/setup.py
--rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 saiph-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     9861 2023-07-28 13:33:05.156053 saiph-1.4.5/LICENSE
+-rw-r--r--   0        0        0     2194 2023-07-28 13:33:05.156053 saiph-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/__init__.py
+-rw-r--r--   0        0        0     4441 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/conftest.py
+-rw-r--r--   0        0        0     1195 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/contribution.py
+-rw-r--r--   0        0        0     1384 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/contribution_test.py
+-rw-r--r--   0        0        0      119 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/exception.py
+-rw-r--r--   0        0        0     6908 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/inverse_transform.py
+-rw-r--r--   0        0        0     9030 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/inverse_transform_test.py
+-rw-r--r--   0        0        0      410 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/lib/size.py
+-rw-r--r--   0        0        0     2479 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/models.py
+-rw-r--r--   0        0        0     8300 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/projection.py
+-rw-r--r--   0        0        0    11890 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/projection_test.py
+-rw-r--r--   0        0        0       27 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/reduction/__init__.py
+-rw-r--r--   0        0        0    15367 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/reduction/famd.py
+-rw-r--r--   0        0        0     4560 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/reduction/famd_sparse.py
+-rw-r--r--   0        0        0     4888 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/reduction/famd_sparse_test.py
+-rw-r--r--   0        0        0     8519 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/reduction/famd_test.py
+-rw-r--r--   0        0        0     9228 2023-07-28 13:33:05.156053 saiph-1.4.5/saiph/reduction/mca.py
+-rw-r--r--   0        0        0     6875 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/mca_test.py
+-rw-r--r--   0        0        0     4251 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/pca.py
+-rw-r--r--   0        0        0     3829 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/pca_test.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/utils/__init__.py
+-rw-r--r--   0        0        0     3825 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/utils/common.py
+-rw-r--r--   0        0        0     2457 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/utils/common_test.py
+-rw-r--r--   0        0        0     4642 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/utils/svd.py
+-rw-r--r--   0        0        0     5005 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/reduction/utils/svd_test.py
+-rw-r--r--   0        0        0     5172 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/serializer.py
+-rw-r--r--   0        0        0     1919 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/serializer_test.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/tests/__init_.py
+-rw-r--r--   0        0        0     1402 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/tests/benchmark_test.py
+-rw-r--r--   0        0        0      521 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/tests/profile_cpu.py
+-rw-r--r--   0        0        0      983 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/tests/profile_memory.py
+-rw-r--r--   0        0        0     5405 2023-07-28 13:33:05.160053 saiph-1.4.5/saiph/visualization.py
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 saiph-1.4.5/PKG-INFO
```

### Comparing `saiph-1.4.4/LICENSE` & `saiph-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/pyproject.toml` & `saiph-1.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "saiph"
 # Also modify in saiph/__init__.py
-version = "1.4.4"
+version = "1.4.5"
 description = "A projection package"
 authors = ["Octopize <help@octopize.io>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pandas = "^1.3"
 numpy = "^1.21"
 scipy = "^1.7"
 scikit-learn = "^1.0"
 toolz = "^0.11.2"
 matplotlib = {version = "^3.5.2", optional = true}
-pydantic = "^1.10.4"
+pydantic = "^2"
 
 [tool.poetry.extras]
 matplotlib = ["matplotlib"]
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.4"
@@ -34,15 +34,14 @@
 flake8-black = "^0.3.2"
 flake8-isort = "^4.1.1"
 flake8-tidy-imports = "^4.6.0"
 flake8-eradicate = "^1.2.0"
 flake8-printf-formatting = "^1.1.2"
 flake8-use-fstring = "^1.3"
 flake8-print = "^4.0.0"
-filprofiler = {git = "https://github.com/pythonspeed/filprofiler.git"}
 py-spy = "^0.3.11"
 typer = "^0.4.1"
 Faker = "^13.6.0"
 tqdm = "^4.64.0"
 pytest-benchmark = "^3.4.1"
 doubles = "^1.5.3"
 ipdb = "^0.13.9"
```

### Comparing `saiph-1.4.4/saiph/conftest.py` & `saiph-1.4.5/saiph/conftest.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/contribution.py` & `saiph-1.4.5/saiph/contribution.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/contribution_test.py` & `saiph-1.4.5/saiph/contribution_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/inverse_transform.py` & `saiph-1.4.5/saiph/inverse_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
     # Descale regarding projection type
     # FAMD
     if model.type == "famd":
         model.prop = cast(pd.Series, model.prop)
         descaled_values_quanti = (scaled_values_quanti * model.std) + model.mean
         descaled_values_quali = (scaled_values_quali * np.sqrt(model.prop)) + model.prop
+
         del scaled_values_quali
         del scaled_values_quanti
         undummy = undummify(
             descaled_values_quali,
             get_dummies_mapping(model.original_categorical, model.dummy_categorical),
             use_max_modalities=use_max_modalities,
             seed=seed,
@@ -163,13 +164,16 @@
         df : dataframe containing proportions
         random_gen: random generator
 
     Returns:
         column_labels: selected column labels
     """
     # Example for 1 row:  [0.1, 0.3, 0.6] --> [0.1, 0.4, 1.0]
-    cum_probability = df.cumsum(axis=1)
+    # probabilities needs to be normalized before draw
+    normalized_df = df.div(df.sum(axis=1), axis=0)
+    cum_probability = normalized_df.cumsum(axis=1)
     random_probability = random_gen.random((cum_probability.shape[0], 1))
+
     # [0.342] < [0.1, 0.4, 1.0] --> [False, True, True] --> idx: 1
     column_labels = (random_probability < cum_probability).idxmax(axis=1)
 
     return column_labels
```

### Comparing `saiph-1.4.4/saiph/inverse_transform_test.py` & `saiph-1.4.5/saiph/inverse_transform_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,26 @@
 def test_get_random_weighted_columns(weights: List[float], expected_index: int) -> None:
     """Verify that get_random_weighted_columns returns the correct column."""
     df = pd.DataFrame(data=[weights])
     result = get_random_weighted_columns(df, np.random.default_rng(1))
     assert result.values[0] == expected_index
 
 
+def test_normalization() -> None:
+    """Verify that the last modality can be sampled when its cumulated sum is greater than 1.
+
+    This test will fail if the values are not normalized first because the last modality would
+    have no chance to be drawn.
+
+    """
+    df = pd.DataFrame(data=[[0.5, 0.5, 0.5]])
+    result = get_random_weighted_columns(df, np.random.default_rng(4))
+    assert result.values[0] == 2
+
+
 @pytest.mark.parametrize(
     "use_max_modalities, expected",
     [
         (
             True,
             pd.DataFrame(
                 [["wrench", "orange"], ["hammer", "apple"]], columns=["tool", "fruit"]
```

### Comparing `saiph-1.4.4/saiph/models.py` & `saiph-1.4.5/saiph/models.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/projection.py` & `saiph-1.4.5/saiph/projection.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/projection_test.py` & `saiph-1.4.5/saiph/projection_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/famd.py` & `saiph-1.4.5/saiph/reduction/famd.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,16 @@
     df_quanti = df[model.original_continuous]
     df_quanti = (df_quanti - model.mean) / model.std
 
     # scale
     df_quali = pd.get_dummies(
         df[model.original_categorical].astype("category"), prefix_sep=DUMMIES_PREFIX_SEP
     )
+    # Here we add a column with 0 if the modality is not present in the dataset but
+    # was used to train the saiph model
     if model._modalities is not None:
         for mod in model._modalities:
             if mod not in df_quali:
                 df_quali[mod] = 0
     df_quali = df_quali[model._modalities]
     df_quali = (df_quali - model.prop) / np.sqrt(model.prop)
```

### Comparing `saiph-1.4.4/saiph/reduction/famd_sparse.py` & `saiph-1.4.5/saiph/reduction/famd_sparse.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/famd_sparse_test.py` & `saiph-1.4.5/saiph/reduction/famd_sparse_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/famd_test.py` & `saiph-1.4.5/saiph/reduction/famd_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/mca.py` & `saiph-1.4.5/saiph/reduction/mca.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/mca_test.py` & `saiph-1.4.5/saiph/reduction/mca_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/pca.py` & `saiph-1.4.5/saiph/reduction/pca.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/pca_test.py` & `saiph-1.4.5/saiph/reduction/pca_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/utils/common.py` & `saiph-1.4.5/saiph/reduction/utils/common.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/utils/common_test.py` & `saiph-1.4.5/saiph/reduction/utils/common_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/utils/svd.py` & `saiph-1.4.5/saiph/reduction/utils/svd.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/reduction/utils/svd_test.py` & `saiph-1.4.5/saiph/reduction/utils/svd_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/serializer.py` & `saiph-1.4.5/saiph/serializer.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/serializer_test.py` & `saiph-1.4.5/saiph/serializer_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/tests/benchmark_test.py` & `saiph-1.4.5/saiph/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/tests/profile_cpu.py` & `saiph-1.4.5/saiph/tests/profile_cpu.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/tests/profile_memory.py` & `saiph-1.4.5/saiph/tests/profile_memory.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/saiph/visualization.py` & `saiph-1.4.5/saiph/visualization.py`

 * *Files identical despite different names*

### Comparing `saiph-1.4.4/PKG-INFO` & `saiph-1.4.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saiph
-Version: 1.4.4
+Version: 1.4.5
 Summary: A projection package
 License: Apache-2.0
 Author: Octopize
 Author-email: help@octopize.io
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,11 +12,11 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: matplotlib
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0) ; extra == "matplotlib"
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pandas (>=1.3,<2.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: scipy (>=1.7,<2.0)
 Requires-Dist: toolz (>=0.11.2,<0.12.0)
```

