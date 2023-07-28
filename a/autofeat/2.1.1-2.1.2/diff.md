# Comparing `tmp/autofeat-2.1.1.tar.gz` & `tmp/autofeat-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofeat-2.1.1.tar", last modified: Sun Jun 25 19:03:51 2023, max compression
+gzip compressed data, was "autofeat-2.1.2.tar", max compression
```

## Comparing `autofeat-2.1.1.tar` & `autofeat-2.1.2.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-06-25 19:03:51.533599 autofeat-2.1.1/
--rw-r--r--   0 franzi     (501) staff       (20)     1057 2016-11-03 21:17:21.000000 autofeat-2.1.1/LICENSE
--rw-r--r--   0 franzi     (501) staff       (20)       16 2017-09-06 12:18:36.000000 autofeat-2.1.1/MANIFEST.in
--rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-06-25 19:03:51.533086 autofeat-2.1.1/PKG-INFO
--rw-r--r--   0 franzi     (501) staff       (20)     5190 2023-05-13 14:02:00.000000 autofeat-2.1.1/README.md
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-06-25 19:03:51.530579 autofeat-2.1.1/autofeat/
--rw-r--r--   0 franzi     (501) staff       (20)      282 2023-06-25 19:01:09.000000 autofeat-2.1.1/autofeat/__init__.py
--rw-r--r--   0 franzi     (501) staff       (20)    28722 2023-06-25 19:00:12.000000 autofeat-2.1.1/autofeat/autofeat.py
--rw-r--r--   0 franzi     (501) staff       (20)    12893 2023-06-25 19:00:16.000000 autofeat-2.1.1/autofeat/autofeatlight.py
--rw-r--r--   0 franzi     (501) staff       (20)    19894 2023-06-25 19:00:41.000000 autofeat-2.1.1/autofeat/feateng.py
--rw-r--r--   0 franzi     (501) staff       (20)    17868 2023-06-25 19:00:36.000000 autofeat-2.1.1/autofeat/featsel.py
--rw-r--r--   0 franzi     (501) staff       (20)      866 2023-06-25 19:00:30.000000 autofeat-2.1.1/autofeat/nb_utils.py
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-06-25 19:03:51.532288 autofeat-2.1.1/autofeat.egg-info/
--rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/PKG-INFO
--rw-r--r--   0 franzi     (501) staff       (20)      332 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/SOURCES.txt
--rw-r--r--   0 franzi     (501) staff       (20)        1 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/dependency_links.txt
--rw-r--r--   0 franzi     (501) staff       (20)       72 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/requires.txt
--rw-r--r--   0 franzi     (501) staff       (20)        9 2023-06-25 19:03:51.000000 autofeat-2.1.1/autofeat.egg-info/top_level.txt
--rw-r--r--   0 franzi     (501) staff       (20)      891 2023-06-25 19:03:28.000000 autofeat-2.1.1/pyproject.toml
--rw-r--r--   0 franzi     (501) staff       (20)       38 2023-06-25 19:03:51.533810 autofeat-2.1.1/setup.cfg
+-rw-r--r--   0        0        0     1057 2016-11-03 21:17:21.000000 autofeat-2.1.2/LICENSE
+-rw-r--r--   0        0        0     5190 2023-05-13 14:02:00.144315 autofeat-2.1.2/README.md
+-rw-r--r--   0        0        0      282 2023-07-28 09:04:52.029339 autofeat-2.1.2/autofeat/__init__.py
+-rw-r--r--   0        0        0    29020 2023-07-28 16:29:15.295136 autofeat-2.1.2/autofeat/autofeat.py
+-rw-r--r--   0        0        0    13194 2023-07-28 14:47:13.855557 autofeat-2.1.2/autofeat/autofeatlight.py
+-rw-r--r--   0        0        0    20001 2023-07-28 14:42:04.413663 autofeat-2.1.2/autofeat/feateng.py
+-rw-r--r--   0        0        0    18069 2023-07-28 14:42:04.413055 autofeat-2.1.2/autofeat/featsel.py
+-rw-r--r--   0        0        0      867 2023-07-28 09:24:38.012858 autofeat-2.1.2/autofeat/nb_utils.py
+-rw-r--r--   0        0        0     3779 2023-07-28 16:08:11.384965 autofeat-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 autofeat-2.1.2/PKG-INFO
```

### Comparing `autofeat-2.1.1/LICENSE` & `autofeat-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autofeat-2.1.1/PKG-INFO` & `autofeat-2.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 Metadata-Version: 2.1
 Name: autofeat
-Version: 2.1.1
+Version: 2.1.2
 Summary: Automatic Feature Engineering and Selection Linear Prediction Model
-Author-email: Franziska Horn <cod3licious@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2016 
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/cod3licious/autofeat
+Home-page: https://github.com/cod3licious/autofeat
+License: MIT
 Keywords: automl,feature engineering,feature selection,linear model
+Author: Franziska Horn
+Author-email: cod3licious@gmail.com
+Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
+Requires-Dist: numba (>=0.53.1)
+Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: pandas (>=1.3.5,<3.0.0)
+Requires-Dist: pint (>=0.17,<1.0)
+Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Requires-Dist: scipy (>=1.7.3,<2.0.0)
+Requires-Dist: sympy (>=1.7.1,<2.0.0)
+Project-URL: Repository, https://github.com/cod3licious/autofeat
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # `autofeat` library
 ### Linear Prediction Models with Automated Feature Engineering and Selection
 
 This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
 - `fit()` function to fit the model parameters
 - `predict()` function to predict the target variable given the input
@@ -85,7 +75,8 @@
 The code is intended for research purposes.
 
 If you have any questions please don't hesitate to send me an [email](mailto:cod3licious@gmail.com) and of course if you should find any bugs or want to contribute other improvements, pull requests are very welcome!
 
 ### Acknowledgments
 
 This project was made possible thanks to support by [BASF](https://www.basf.com).
+
```

### Comparing `autofeat-2.1.1/README.md` & `autofeat-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `autofeat-2.1.1/autofeat/autofeat.py` & `autofeat-2.1.2/autofeat/autofeat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
 from __future__ import annotations
+
+import logging
 import warnings
+
 import numba as nb
 import numpy as np
 import pandas as pd
+import pint
 import sklearn.linear_model as lm
+from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin
 from sklearn.preprocessing import OneHotEncoder
-from sklearn.base import BaseEstimator, RegressorMixin, ClassifierMixin
-from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
+from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 from sympy.utilities.lambdify import lambdify
-import pint
 
-from .feateng import engineer_features, n_cols_generated, colnames2symbols
-from .featsel import select_features
+from autofeat.feateng import colnames2symbols, engineer_features, n_cols_generated
+from autofeat.featsel import select_features
+
+logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=logging.INFO)
 
 
 def _parse_units(units: dict, ureg: pint.UnitRegistry | None = None, verbose: int = 0):
     """
     Convert a dict with string units to pint quantities.
 
     Inputs:
         - units: dict with {"variable_name": "unit"}
         - ureg: optional: a pint UnitRegistry
         - verbose: verbosity level (int; default: 0)
 
-    Returns
+    Returns:
         - parsed_units: dict with {"variable_name": pint Quantity}
     """
     parsed_units = {}
     if units:
         if ureg is None:
             ureg = pint.UnitRegistry(auto_reduce_dimensions=True, autoconvert_offset_to_baseunit=True)
         for c in units:
             try:
                 parsed_units[c] = ureg.parse_expression(units[c])
             except pint.UndefinedUnitError:
                 if verbose > 0:
-                    print(f"[AutoFeat] WARNING: unit {units[c]} of column {c} was not recognized and will be ignored!")
+                    logging.warning(f"[AutoFeat] unit {units[c]} of column {c} was not recognized and will be ignored!")
                 parsed_units[c] = ureg.parse_expression("")
             parsed_units[c].__dict__["_magnitude"] = 1.0
     return parsed_units
 
 
 class AutoFeatModel(BaseEstimator):
     def __init__(
@@ -115,17 +120,15 @@
         self.transformations = transformations
         self.apply_pi_theorem = apply_pi_theorem
         self.always_return_numpy = always_return_numpy
         self.n_jobs = n_jobs
         self.verbose = verbose
 
     def __getstate__(self):
-        """
-        get dict for pickling without feature_functions as they are not pickleable
-        """
+        """Get dict for pickling without feature_functions as they are not pickleable"""
         return {k: self.__dict__[k] if k != "feature_functions_" else {} for k in self.__dict__}
 
     def _transform_categorical_cols(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transform categorical features into 0/1 encoding.
 
         Inputs:
@@ -140,29 +143,30 @@
                 if c not in df.columns:
                     raise ValueError(f"[AutoFeat] categorical_col {c} not in df.columns")
                 ohe = e.fit_transform(df[c].to_numpy()[:, None])
                 new_cat_cols = [f"cat_{c}_{i}" for i in e.categories_[0]]
                 self.categorical_cols_map_[c] = new_cat_cols
                 df = df.join(pd.DataFrame(ohe, columns=new_cat_cols, index=df.index))
             # remove the categorical column from our columns to consider
-            df.drop(columns=self.categorical_cols, inplace=True)
+            df = df.drop(columns=self.categorical_cols)
         return df
 
     def _apply_pi_theorem(self, df: pd.DataFrame) -> pd.DataFrame:
         if self.apply_pi_theorem and self.units:
             ureg = pint.UnitRegistry(auto_reduce_dimensions=True, autoconvert_offset_to_baseunit=True)
             parsed_units = _parse_units(self.units, ureg, self.verbose)
             # use only original features
             parsed_units = {c: parsed_units[c] for c in self.feateng_cols_ if not parsed_units[c].dimensionless}
             if self.verbose:
-                print("[AutoFeat] Applying the Pi Theorem")
+                logging.info("[AutoFeat] Applying the Pi Theorem")
             pi_theorem_results = ureg.pi_theorem(parsed_units)
             for i, r in enumerate(pi_theorem_results, 1):
                 if self.verbose:
-                    print(f"[AutoFeat] Pi Theorem {i}: ", pint.formatter(r.items()))
+                    logging.info(f"[AutoFeat] Pi Theorem {i}: ")
+                    logging.info(pint.formatter(r.items()))
                 # compute the final result by multiplying and taking the power of
                 cols = sorted(r)
                 # only use data points where non of the affected columns are NaNs
                 not_na_idx = df[cols].notna().all(axis=1)
                 ptr = df[cols[0]].to_numpy()[not_na_idx] ** r[cols[0]]
                 for c in cols[1:]:
                     ptr *= df[c].to_numpy()[not_na_idx] ** r[c]
@@ -173,24 +177,25 @@
         """
         Generate additional features based on the feature formulas for all data points in the df.
         Only works after the model was fitted.
 
         Inputs:
             - df: pandas dataframe with original features
             - new_feat_cols: names of new features that should be generated (keys of self.feature_formulas_)
+
         Returns:
             - df: dataframe with the additional feature columns added
         """
         check_is_fitted(self, ["feature_formulas_"])
         if not new_feat_cols:
             return df
-        if not new_feat_cols[0] in self.feature_formulas_:
+        if new_feat_cols[0] not in self.feature_formulas_:
             raise RuntimeError("[AutoFeat] First call fit or fit_transform to generate the features!")
         if self.verbose:
-            print(f"[AutoFeat] Computing {len(new_feat_cols)} new features.")
+            logging.info(f"[AutoFeat] Computing {len(new_feat_cols)} new features.")
         # generate all good feature; unscaled this time
         feat_array = np.zeros((len(df), len(new_feat_cols)))
         for i, expr in enumerate(new_feat_cols):
             if self.verbose:
                 print(f"[AutoFeat] {i:5}/{len(new_feat_cols):5} new features", end="\r")
             if expr not in self.feature_functions_:
                 # generate a substitution expression based on all the original symbols of the original features
@@ -203,62 +208,62 @@
                     f = None
                     f_jit = None
                 else:
                     try:
                         f = lambdify([self.feature_formulas_[c] for c in cols], self.feature_formulas_[expr])
                         f_jit = nb.njit(f)
                     except Exception:
-                        print(f"[AutoFeat] Error while processing expression: {expr}")
+                        logging.exception(f"[AutoFeat] Error while processing expression: {expr}")
                         raise
                 self.feature_functions_[expr] = (cols, f, f_jit)
             else:
                 cols, f, f_jit = self.feature_functions_[expr]
-            if f is not None:
+            if f is not None and f_jit is not None:
                 # only generate features for completely not-nan rows
                 not_na_idx = df[cols].notna().all(axis=1)
                 try:
                     try:
                         feat = f_jit(*(df[c].to_numpy(dtype=float)[not_na_idx] for c in cols))
                     except nb.TypingError:
                         # lambified abs fn with non trivial inputs doesn't jit compile with numba, yet
                         # fallback on the non jitted version of the function
                         feat = f(*(df[c].to_numpy(dtype=float)[not_na_idx] for c in cols))
                         # henceforth, always use the non jitted version of the function
                         self.feature_functions_[expr] = (cols, f, f)
                     feat_array[not_na_idx, i] = feat
                     feat_array[~not_na_idx, i] = np.nan
                 except RuntimeWarning:
-                    print(
-                        f"[AutoFeat] WARNING: Problem while evaluating expression: {expr} with columns {cols}",
+                    logging.warning(
+                        f"[AutoFeat] Problem while evaluating expression: {expr} with columns {cols}",
                         " - is the data in a different range then when calling .fit()? Are maybe some values 0 that shouldn't be?",
                     )
                     raise
         if self.verbose:
-            print(f"[AutoFeat] {len(new_feat_cols):5}/{len(new_feat_cols):5} new features ...done.")
-        df = df.join(pd.DataFrame(feat_array, columns=new_feat_cols, index=df.index))
-        return df
+            logging.info(f"[AutoFeat] {len(new_feat_cols):5}/{len(new_feat_cols):5} new features ...done.")
+        return df.join(pd.DataFrame(feat_array, columns=new_feat_cols, index=df.index))
 
     def _X2df(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Helper function that ensures correctness of the input data for classification tasks.
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+
         Returns:
             - df: transformed dataframe
         """
         # store column names as they'll be lost in the other check
         cols = [str(c) for c in X.columns] if isinstance(X, pd.DataFrame) else []
         # check input variables
         X = check_array(X, dtype=None)
         if not cols:
             cols = [f"x{i:03}" for i in range(X.shape[1])]
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=cols)
         # do we need to call transform?
-        if not list(df.columns) == self.all_columns_:
+        if list(df.columns) != self.all_columns_:
             temp = self.always_return_numpy
             self.always_return_numpy = False
             df = self.transform(df)
             self.always_return_numpy = temp
         return df
 
     def fit_transform(self, X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
@@ -313,123 +318,128 @@
             # apply pi-theorem -- additional columns are not used for regular feature engineering (for now)!
             df = self._apply_pi_theorem(df)
         # subsample data points and targets in case we'll generate too many features
         # (n_rows * n_cols * 32/8)/1000000000 <= max_gb
         n_cols = n_cols_generated(len(self.feateng_cols_), self.feateng_steps, len(self.transformations))
         n_gb = (len(df) * n_cols) / 250000000
         if self.verbose:
-            print(
-                f"[AutoFeat] The {self.feateng_steps} step feature engineering process could generate up to {n_cols} features."
+            logging.info(
+                f"[AutoFeat] The {self.feateng_steps} step feature engineering process could generate up to {n_cols} features.",
+            )
+            logging.info(
+                f"[AutoFeat] With {len(df)} data points this new feature matrix would use about {n_gb:.2f} gb of space.",
             )
-            print(f"[AutoFeat] With {len(df)} data points this new feature matrix would use about {n_gb:.2f} gb of space.")
         if self.max_gb and n_gb > self.max_gb:
             n_rows = int(self.max_gb * 250000000 / n_cols)
             if self.verbose:
-                print(
-                    f"[AutoFeat] As you specified a limit of {self.max_gb:.1f} gb, the number of data points is subsampled to {n_rows}"
+                logging.info(
+                    f"[AutoFeat] As you specified a limit of {self.max_gb:.1f} gb, the number of data points is subsampled to {n_rows}",
                 )
             subsample_idx = np.random.permutation(list(df.index))[:n_rows]
             df_subs = df.iloc[subsample_idx]
-            df_subs.reset_index(drop=True, inplace=True)
+            df_subs = df_subs.reset_index(drop=True)
             target_sub = target[subsample_idx]
         else:
             df_subs = df.copy()
             target_sub = target.copy()
         # generate features
         df_subs, self.feature_formulas_ = engineer_features(
             df_subs,
             self.feateng_cols_,
-            _parse_units(self.units, verbose=self.verbose),
+            _parse_units(self.units, verbose=self.verbose),  # type: ignore
             self.feateng_steps,
             self.transformations,
             self.verbose,
         )
         # select predictive features
         if self.featsel_runs <= 0:
             if self.verbose:
-                print("[AutoFeat] WARNING: Not performing feature selection.")
+                logging.warning("[AutoFeat] Not performing feature selection.")
             good_cols = df_subs.columns
+        elif self.problem_type in ("regression", "classification"):
+            good_cols = select_features(
+                df_subs,
+                target_sub,
+                self.featsel_runs,
+                None,
+                self.problem_type,
+                self.n_jobs,
+                self.verbose,
+            )
+            # if no features were selected, take the original features
+            if not good_cols:
+                good_cols = list(df.columns)
         else:
-            if self.problem_type in ("regression", "classification"):
-                good_cols = select_features(
-                    df_subs, target_sub, self.featsel_runs, None, self.problem_type, self.n_jobs, self.verbose
-                )
-                # if no features were selected, take the original features
-                if not good_cols:
-                    good_cols = list(df.columns)
-            else:
-                print(f"[AutoFeat] WARNING: Unknown problem_type {self.problem_type} - not performing feature selection.")
-                good_cols = df_subs.columns
+            logging.warning(f"[AutoFeat] Unknown problem_type {self.problem_type} - not performing feature selection.")
+            good_cols = df_subs.columns
         # filter out those columns that were original features or generated otherwise
         self.new_feat_cols_ = [c for c in good_cols if c not in list(df.columns)]
         self.good_cols_ = good_cols
         # re-generate all good feature again; for all data points this time
-        self.feature_functions_ = {}
+        self.feature_functions_ = {}  # type: ignore
         df = self._generate_features(df, self.new_feat_cols_)
         # to prevent an error because sometimes the column names are numpy.str_ instead of normal str
         df.columns = [str(c) for c in df.columns]
         # filter out unnecessary junk from self.feature_formulas_
         self.feature_formulas_ = {f: self.feature_formulas_[f] for f in self.new_feat_cols_ + self.feateng_cols_}
         self.feature_functions_ = {f: self.feature_functions_[f] for f in self.new_feat_cols_}
         self.all_columns_ = list(df.columns)
         # train final prediction model on all selected features
         if self.verbose:
             # final dataframe contains original columns and good additional columns
-            print(
-                f"[AutoFeat] Final dataframe with {len(df.columns)} feature columns ({len(df.columns) - len(self.original_columns_)} new)."
+            logging.info(
+                f"[AutoFeat] Final dataframe with {len(df.columns)} feature columns ({len(df.columns) - len(self.original_columns_)} new).",
             )
 
         # train final prediction model
         if self.problem_type == "regression":
             model = lm.LassoLarsCV(cv=5)
         elif self.problem_type == "classification":
             model = lm.LogisticRegressionCV(cv=5, class_weight="balanced")
         else:
-            print(f"[AutoFeat] WARNING: Unknown problem_type {self.problem_type} - not fitting a prediction model.")
+            logging.warning(f"[AutoFeat] Unknown problem_type {self.problem_type} - not fitting a prediction model.")
             model = None
         if model is not None:
             if self.verbose:
-                print(f"[AutoFeat] Training final {self.problem_type} model.")
+                logging.info(f"[AutoFeat] Training final {self.problem_type} model.")
             X = df[self.good_cols_].to_numpy()
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 model.fit(X, target)
             self.prediction_model_ = model
             # sklearn requires a "classes_" attribute
             if self.problem_type == "classification":
                 self.classes_ = model.classes_
             if self.verbose:
-                if self.problem_type == "regression":
-                    coefs = model.coef_
-                else:
-                    # model.coefs_ is n_classes x n_features, but we need n_features
-                    coefs = np.max(np.abs(model.coef_), axis=0)
+                # for classification, model.coefs_ is n_classes x n_features, but we need n_features
+                coefs = model.coef_ if self.problem_type == "regression" else np.max(np.abs(model.coef_), axis=0)
                 weights = dict(zip(self.good_cols_, coefs))
-                print("[AutoFeat] Trained model: largest coefficients:")
-                print(model.intercept_)
+                logging.info("[AutoFeat] Trained model: largest coefficients:")
+                logging.info(model.intercept_)
                 for c in sorted(weights, key=lambda x: abs(weights[x]), reverse=True):
                     if abs(weights[c]) < 1e-5:
                         break
-                    print(f"{weights[c]:.6f} * {c}")
-                print(f"[AutoFeat] Final score: {model.score(X, target):.4f}")
+                    logging.info(f"{weights[c]:.6f} * {c}")
+                logging.info(f"[AutoFeat] Final score: {model.score(X, target):.4f}")
         if self.always_return_numpy:
             return df.to_numpy()
         return df
 
     def fit(self, X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame):
         if self.verbose:
-            print("[AutoFeat] Warning: This just calls fit_transform() but does not return the transformed dataframe.")
-            print("[AutoFeat] It is much more efficient to call fit_transform() instead of fit() and transform()!")
-        _ = self.fit_transform(X, y)  # noqa
+            logging.warning("[AutoFeat] This just calls fit_transform() but does not return the transformed dataframe.")
+            logging.info("[AutoFeat] It is much more efficient to call fit_transform() instead of fit() and transform()!")
+        _ = self.fit_transform(X, y)
         return self
 
     def transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+
         Returns:
             - new_df: new pandas dataframe with all the original features (except categorical features transformed
                       into multiple 0/1 columns) and the most promising engineered features. This df can then be
                       used to train your final model.
         """
         check_is_fitted(self, ["feature_formulas_"])
         # store column names as they'll be lost in the other check
@@ -454,14 +464,15 @@
             return df.to_numpy()
         return df
 
     def predict(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+
         Returns:
             - y_pred: predicted targets returned by prediction_model.predict()
         """
         check_is_fitted(self, ["prediction_model_"])
         df = self._X2df(X)
         return self.prediction_model_.predict(df[self.good_cols_].to_numpy())
 
@@ -479,15 +490,15 @@
         # check input variables
         X, target = check_X_y(X, y, y_numeric=self.problem_type == "regression", dtype=None)
         if not cols:
             cols = [f"x{i:03}" for i in range(X.shape[1])]
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=cols)
         # do we need to call transform?
-        if not list(df.columns) == self.all_columns_:
+        if list(df.columns) != self.all_columns_:
             temp = self.always_return_numpy
             self.always_return_numpy = False
             df = self.transform(df)
             self.always_return_numpy = temp
         return self.prediction_model_.score(df[self.good_cols_].to_numpy(), target)
 
     @property
@@ -560,13 +571,14 @@
             verbose,
         )
 
     def predict_proba(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+
         Returns:
             - y_pred: predicted targets probabilities returned by prediction_model.predict_proba()
         """
         check_is_fitted(self, ["prediction_model_"])
         df = self._X2df(X)
         return self.prediction_model_.predict_proba(df[self.good_cols_].to_numpy())
```

### Comparing `autofeat-2.1.1/autofeat/autofeatlight.py` & `autofeat-2.1.2/autofeat/autofeatlight.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,103 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
 from __future__ import annotations
+
+import logging
 import sys
+from collections import defaultdict
+
 import numpy as np
 import pandas as pd
-from collections import defaultdict
-from typing import Tuple
 from sklearn.base import BaseEstimator
+from sklearn.preprocessing import PowerTransformer, StandardScaler
 from sklearn.utils.validation import check_array, check_is_fitted
-from sklearn.preprocessing import StandardScaler, PowerTransformer
+
+logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=logging.INFO)
 
 
 def _check_features(df: pd.DataFrame, corrthr: float = 0.995, verbose: int = 0) -> list:
     """
     Identify features with zeros variance or a correlation of (almost) 1 to other features, i.e., useless features.
 
     Inputs:
         - df: pd.DataFrame with all features
         - corrthr: threshold for correlations: if a feature has a higher pearson correlation to another feature it's
                    considered as redundant and ignored (float; default: 0.995)
         - verbose: verbosity level (int; default: 0)
+
     Returns:
         - list of column names representing 'ok' features (numeric, non-zero variance, not redundant)
     """
     # make sure all data is numeric
     df = df.select_dtypes(include=np.number)
     useless_cols = set()
     # 1. identify features with zero variance
     for c, v in df.var().items():
         if pd.isna(v) or v <= sys.float_info.epsilon:
             useless_cols.add(c)
     # 2. identify redundant features (that have a correlation of ~1 with other features)
     correlated_cols = defaultdict(set)
     corrmat = pd.DataFrame(np.abs(np.corrcoef(df.values, rowvar=False)), columns=df.columns, index=df.columns)
     np.fill_diagonal(corrmat.values, 0)
-    for c, v in corrmat.unstack().sort_values(ascending=False).items():
+    for c, v in corrmat.unstack().sort_values(ascending=False).items():  # noqa PD010
         if v < corrthr:
             break
         if (c[0] != c[1]) and (c[0] not in useless_cols):
             correlated_cols[c[0]].add(c[1])
     # keep the columns that eliminate the most correlated columns
     for c in sorted(correlated_cols, key=lambda x: len(correlated_cols[x]), reverse=True):
         # the first variable that is correlated with others adds its correlated variables to the set of useless cols
         # since we check if a variable is in useless_cols, the correlated variables can't add the original variable
         if c not in useless_cols:
             useless_cols.update(correlated_cols[c])
     # return list of columns that should be kept
     if verbose:
-        print(f"[AutoFeatLight] {len(useless_cols)} columns identified as useless:")
-        print(sorted(useless_cols))
+        logging.info(f"[AutoFeatLight] {len(useless_cols)} columns identified as useless:")
+        logging.info(sorted(useless_cols))
     return [c for c in df.columns if c not in useless_cols]
 
 
 def _compute_additional_features(
-    X: np.ndarray, feature_names: list | None = None, compute_ratio: bool = True, compute_product: bool = True, verbose: int = 0
-) -> Tuple[np.ndarray, list]:
+    X: np.ndarray,
+    feature_names: list | None = None,
+    compute_ratio: bool = True,
+    compute_product: bool = True,
+    verbose: int = 0,
+) -> tuple[np.ndarray | None, list]:
     """
     Compute additional non-linear features from the original features (ratio or product of two features).
 
     Inputs:
         - X: np.array with data (n_datapoints x n_features)
         - feature_names: optional list of column names to identify the features in X
         - compute_ratio: bool (default: True), whether to compute ratios of features
         - compute_product: bool (default: True), whether to compute products of features
         - verbose: verbosity level (int; default: 0)
+
     Returns:
         - np.array (n_datapoints x n_additional_features) with newly computed features
         - list with n_additional_features names describing the newly computed features
     """
     # check how many new features we will compute
     d = X.shape[1]
     n = 0
     if compute_ratio:
         n += d * d - d
     if compute_product:
         n += (d * d - d) // 2
     if not n:
-        print("ERROR: call _compute_additional_features with compute_ratio and/or compute_product set to True")
+        logging.error("[AutoFeatLight] call _compute_additional_features with compute_ratio and/or compute_product set to True")
         return None, []
     if not feature_names:
         feature_names = [f"x{i}" for i in range(1, d + 1)]
     # compute new features
     if verbose:
-        print(f"[AutoFeatLight] computing {n} additional features from {d} original features")
+        logging.info(f"[AutoFeatLight] computing {n} additional features from {d} original features")
     new_features = []
     X_new = np.zeros((X.shape[0], n))
     new_i = 0
     if compute_ratio:
         for i in range(d):
             # compute 1/x1
             with np.errstate(divide="ignore"):
@@ -158,30 +168,31 @@
         """
         WARNING: call fit_transform instead!
 
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
         """
         if self.verbose:
-            print("[AutoFeatLight] Warning: This just calls fit_transform() but does not return the transformed dataframe.")
-            print("[AutoFeatLight] It is much more efficient to call fit_transform() instead of fit() and transform()!")
-        _ = self.fit_transform(X)  # noqa
+            logging.warning("[AutoFeatLight] This just calls fit_transform() but does not return the transformed dataframe.")
+            logging.info("[AutoFeatLight] It is much more efficient to call fit_transform() instead of fit() and transform()!")
+        _ = self.fit_transform(X)
         return self
 
     def transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+
         Returns:
             - new_X: new pandas dataframe or numpy array with additional/transformed features
         """
         check_is_fitted(self, ["good_cols_org_"])
         if not self.good_cols_org_:
             if self.verbose > 0:
-                print("[AutoFeatLight] WARNING: No good features found; returning data unchanged.")
+                logging.warning("[AutoFeatLight] No good features found; returning data unchanged.")
             return X
         if isinstance(X, pd.DataFrame):
             # make sure all data is numeric or we'll get an error when checking X
             X = X.select_dtypes(include=np.number)
             df_index = X.index
         else:
             df_index = None
@@ -191,15 +202,19 @@
         if not cols == self.original_columns_:
             raise ValueError("[AutoFeatLight] Not the same features as when calling fit.")
         # sort out useless original columns
         df = pd.DataFrame(X, columns=cols, index=df_index)[self.good_cols_org_]
         if self.compute_ratio or self.compute_product:
             # compute additional useful features
             X_new, new_features = _compute_additional_features(
-                df.to_numpy(), self.good_cols_org_, self.compute_ratio, self.compute_product, self.verbose
+                df.to_numpy(),
+                self.good_cols_org_,
+                self.compute_ratio,
+                self.compute_product,
+                self.verbose,
             )
             df = pd.concat([df, pd.DataFrame(X_new, columns=new_features)], axis=1)
             df = df[self.features_]
         # scale/transform
         if self.scale or self.power_transform:
             X_new = self.scaler_.transform(df.to_numpy())
             if self.power_transform:
@@ -208,14 +223,15 @@
         # return either dataframe or array
         return df if self.return_df_ else df.to_numpy()
 
     def fit_transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+
         Returns:
             - new_X: new pandas dataframe or numpy array with additional/transformed features
         """
         self.return_df_ = isinstance(X, pd.DataFrame)
         if isinstance(X, pd.DataFrame):
             # make sure all data is numeric or we'll get an error when checking X
             X = X.select_dtypes(include=np.number)
@@ -228,21 +244,25 @@
         X = check_array(X, force_all_finite="allow-nan")
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=self.original_columns_, index=df_index)
         # see which of the original features are not completely useless
         self.good_cols_org_ = _check_features(df, self.corrthr_init, self.verbose)
         if not self.good_cols_org_:
             if self.verbose > 0:
-                print("[AutoFeatLight] WARNING: No good features found; returning original features.")
+                logging.warning("[AutoFeatLight] No good features found; returning original features.")
             return df if self.return_df_ else X
         # compute additional features
         df = df[self.good_cols_org_]
         if self.compute_ratio or self.compute_product:
             X_new, new_features = _compute_additional_features(
-                df.to_numpy(), self.good_cols_org_, self.compute_ratio, self.compute_product, self.verbose
+                df.to_numpy(),
+                self.good_cols_org_,
+                self.compute_ratio,
+                self.compute_product,
+                self.verbose,
             )
             # add new features to original dataframe
             df = pd.concat([df, pd.DataFrame(X_new, columns=new_features, index=df_index)], axis=1)
             # check again which of the features we should keep
             self.features_ = _check_features(df, self.corrthr, self.verbose)
             df = df[self.features_]
         else:
@@ -252,11 +272,11 @@
             self.scaler_ = StandardScaler(with_mean=False)
             X_new = self.scaler_.fit_transform(df.to_numpy())
             if self.power_transform:
                 self.power_transformer_ = PowerTransformer(method="yeo-johnson", standardize=True)
                 X_new = self.power_transformer_.fit_transform(X_new)
             df = pd.DataFrame(X_new, columns=df.columns, index=df.index)
         if self.verbose > 0:
-            print(f"[AutoFeatLight] New data shape: {df.shape[0]} x {df.shape[1]}")
+            logging.info(f"[AutoFeatLight] New data shape: {df.shape[0]} x {df.shape[1]}")
         self.n_features_in_ = len(self.original_columns_)
         # return either dataframe or array
         return df if self.return_df_ else df.to_numpy()
```

### Comparing `autofeat-2.1.1/autofeat/feateng.py` & `autofeat-2.1.2/autofeat/feateng.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
 from __future__ import annotations
-import re
+
+import logging
 import operator as op
+import re
 from functools import reduce
 from itertools import combinations, product
-from typing import Callable, Tuple
+from typing import Callable
 
 import numba as nb
 import numpy as np
 import pandas as pd
+import pint
 import sympy
-from sympy.utilities.lambdify import lambdify
 from sklearn.preprocessing import StandardScaler
-import pint
+from sympy.utilities.lambdify import lambdify
+
+logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=logging.INFO)
 
 
 def colnames2symbols(c: str | int, i: int = 0) -> str:
     # take a messy column name and transform it to something sympy can handle
     # worst case: i is the number of the features
     # has to be a string
     c = str(c)
@@ -92,15 +96,15 @@
 def engineer_features(
     df_org: pd.DataFrame,
     start_features: list | None = None,
     units: dict | None = None,
     max_steps: int = 3,
     transformations: list | tuple = ("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
     verbose: int = 0,
-) -> Tuple[pd.DataFrame, dict]:
+) -> tuple[pd.DataFrame, dict]:
     """
     Given a DataFrame with original features, perform the feature engineering routine for max_steps.
     It starts with a transformation of the original features (applying log, ^2, sqrt, etc.),
     then in the next step, the features are combined (x+y, x*y, ...), and in further steps, the resulting
     features are again transformed and combinations of the resulting features are computed.
 
     Inputs:
@@ -116,54 +120,49 @@
             Step 3: transformation of new features
             (Step 4: combination of old and new features)
             --> with 3 original features, after 4 steps you will already end up with around 200k features!
         - transformations: list of transformations that should be applied; possible elements:
                            "1/", "exp", "log", "abs", "sqrt", "^2", "^3", "1+", "1-", "sin", "cos", "exp-", "2^"
                            (first 7, i.e., up to ^3, are applied by default)
         - verbose: verbosity level (int; default: 0)
+
     Returns:
         - df: new DataFrame with all features in columns
         - feature_pool: dict with {col: sympy formula} formulas to generate each feature
     """
     # initialize the feature pool with columns from the dataframe
     if not start_features:
         start_features = df_org.columns
     else:
         for c in start_features:
             if c not in df_org.columns:
                 raise ValueError(f"[feateng] start feature {c} not in df_org.columns")
-    feature_pool = {c: sympy.symbols(colnames2symbols(c, i), real=True) for i, c in enumerate(start_features)}
+    feature_pool = {c: sympy.symbols(colnames2symbols(c, i), real=True) for i, c in enumerate(start_features)}  # type: ignore
     if max_steps < 1:
         if verbose > 0:
-            print("[feateng] Warning: no features generated for max_steps < 1.")
+            logging.warning("[feateng] no features generated for max_steps < 1.")
         return df_org, feature_pool
     # get a copy of the dataframe - this is where all the features will be added
     df = pd.DataFrame(df_org.copy(), dtype=np.float32)
 
     compiled_func_transformations = None
     compiled_func_transforms_cond = None
     compiled_func_combinations = None
 
     def compile_func_transform(name: str, ft: Callable, plus_1: bool = False):
         def _abs(x):
             return np.abs(x)
 
         # create temporary variable expression and apply it to precomputed feature
         t = sympy.symbols("t")
-        if plus_1:
-            expr_temp = ft(t + 1)
-        else:
-            expr_temp = ft(t)
-        if name == "abs":
-            fn = _abs
-        else:
-            fn = lambdify(t, expr_temp)
+        expr_temp = ft(t + 1) if plus_1 else ft(t)
+        fn = _abs if name == "abs" else lambdify(t, expr_temp)
         return nb.njit(fn)
 
-    def apply_transformations(features_list: list) -> Tuple[list, set]:
+    def apply_transformations(features_list: list) -> tuple[list, set]:
         # feature transformations
         func_transform = {
             "exp": lambda x: sympy.exp(x),
             "exp-": lambda x: sympy.exp(-x),
             "log": lambda x: sympy.log(x),
             "abs": lambda x: sympy.Abs(x),
             "sqrt": lambda x: sympy.sqrt(x),
@@ -215,15 +214,15 @@
         if compiled_func_transformations is None:
             compiled_func_transformations = {k: compile_func_transform(k, v) for k, v in func_transform.items()}
             compiled_func_transformations["log_plus_1"] = compile_func_transform("log", func_transform["log"], plus_1=True)
 
             compiled_func_transforms_cond = {x[0]: nb.njit(x[1]) for x in func_transform_cond.items()}
 
         # returns a list of new features that were generated
-        new_features = []
+        new_features: list[str] = []
         uncorr_features = set()
         # store all new features in a preallocated numpy array before adding it to the dataframe
         feat_array = np.zeros((df.shape[0], len(features_list) * len(transformations)), dtype=np.float32)
         cat_features = {feat for feat in features_list if len(df[feat].unique()) <= 2}
         func_transform_cond_cache = {}  # Cache for compiled_func_transforms_cond checks
         for i, feat in enumerate(features_list):
             if verbose and not i % 100:
@@ -262,31 +261,31 @@
                                 feat_array[:, len(new_features)] = new_feat
                                 new_features.append(expr_name)
                                 # correlation test: don't include features that are basically the same as the original features
                                 # but we only filter them out at the end, since they still might help in other steps!
                                 if corr < 0.95:
                                     uncorr_features.add(expr_name)
         if verbose > 0:
-            print(
-                f"[feateng] Generated {len(new_features)} transformed features from {len(features_list)} original features - done."
+            logging.info(
+                f"[feateng] Generated {len(new_features)} transformed features from {len(features_list)} original features - done.",
             )
         df = df.join(pd.DataFrame(feat_array[:, : len(new_features)], columns=new_features, index=df.index, dtype=np.float32))
         return new_features, uncorr_features
 
     def compile_func_combinations(func_combinations: dict) -> dict:
         d = {}
         for fc in func_combinations:
             s, t = sympy.symbols("s t")
             expr_temp = func_combinations[fc](s, t)
             fn = lambdify((s, t), expr_temp)
             vect = nb.vectorize(["float32(float32, float32)"], nopython=True)
             d[fc] = vect(fn)
         return d
 
-    def get_feature_combinations(feature_tuples: list) -> Tuple[list, set]:
+    def get_feature_combinations(feature_tuples: list) -> tuple[list, set]:
         # new features as combinations of two other features
         func_combinations = {
             "x+y": lambda x, y: x + y,
             "x*y": lambda x, y: x * y,
             "x-y": lambda x, y: x - y,
             "y-x": lambda x, y: y - x,
         }
@@ -295,20 +294,17 @@
         nonlocal df, feature_pool, units, compiled_func_combinations
 
         if compiled_func_combinations is None:
             compiled_func_combinations = compile_func_combinations(func_combinations)
 
         # only compute all combinations if there are more transformations applied afterwards
         # additions at the highest level are sorted out later anyways
-        if steps == max_steps:
-            combinations = ["x*y"]
-        else:
-            combinations = list(func_combinations.keys())
+        combinations = ["x*y"] if steps == max_steps else list(func_combinations.keys())
         # returns a list of new features that were generated
-        new_features = []
+        new_features: list[str] = []
         uncorr_features = set()
         # store all new features in a preallocated numpy array before adding it to the dataframe
         feat_array = np.zeros((df.shape[0], len(feature_tuples) * len(combinations)), dtype=np.float32)
         for i, (feat1, feat2) in enumerate(feature_tuples):
             if verbose and not i % 100:
                 print(f"[feateng] {i:15}/{len(feature_tuples):15} feature tuples combined", end="\r")
             for fc in combinations:
@@ -332,86 +328,86 @@
                             feat_array[:, len(new_features)] = new_feat
                             new_features.append(expr_name)
                             # correlation test: don't include features that are basically the same as the original features
                             # but we only filter them out at the end, since they still might help in other steps!
                             if corr < 0.95:
                                 uncorr_features.add(expr_name)
         if verbose > 0:
-            print(
-                f"[feateng] Generated {len(new_features)} feature combinations from {len(feature_tuples)} original feature tuples - done."
+            logging.info(
+                f"[feateng] Generated {len(new_features)} feature combinations from {len(feature_tuples)} original feature tuples - done.",
             )
         df = df.join(pd.DataFrame(feat_array[:, : len(new_features)], columns=new_features, index=df.index, dtype=np.float32))
         return new_features, uncorr_features
 
     # get transformations of initial features
     steps = 1
     if verbose > 0:
-        print("[feateng] Step 1: transformation of original features")
+        logging.info("[feateng] Step 1: transformation of original features")
     original_features = list(feature_pool.keys())
     uncorr_features = set(feature_pool.keys())
     temp_new, temp_uncorr = apply_transformations(original_features)
     original_features.extend(temp_new)
     uncorr_features.update(temp_uncorr)
     steps += 1
     # get combinations of first feature set
     if steps <= max_steps:
         if verbose > 0:
-            print("[feateng] Step 2: first combination of features")
+            logging.info("[feateng] Step 2: first combination of features")
         new_features, temp_uncorr = get_feature_combinations(list(combinations(original_features, 2)))
         uncorr_features.update(temp_uncorr)
         steps += 1
     while steps <= max_steps:
         # apply transformations on these new features
         if verbose > 0:
-            print(f"[feateng] Step {steps}: transformation of new features")
+            logging.info(f"[feateng] Step {steps}: transformation of new features")
         temp_new, temp_uncorr = apply_transformations(new_features)
         new_features.extend(temp_new)
         uncorr_features.update(temp_uncorr)
         steps += 1
         # get combinations of old and new features
         if steps <= max_steps:
             if verbose > 0:
-                print(f"[feateng] Step {steps}: combining old and new features")
+                logging.info(f"[feateng] Step {steps}: combining old and new features")
             new_new_features, temp_uncorr = get_feature_combinations(list(product(original_features, new_features)))
             uncorr_features.update(temp_uncorr)
             steps += 1
         # and combinations of new features within themselves
         if steps <= max_steps:
             if verbose > 0:
-                print(f"[feateng] Step {steps}: combining new features")
+                logging.info(f"[feateng] Step {steps}: combining new features")
             temp_new, temp_uncorr = get_feature_combinations(list(combinations(new_features, 2)))
             new_new_features.extend(temp_new)
             uncorr_features.update(temp_uncorr)
             steps += 1
             # update old and new features and repeat
             original_features.extend(new_features)
             new_features = new_new_features
 
     # sort out all features that are just additions on the highest level or correlated with more basic features
     if verbose > 0:
-        print(f"[feateng] Generated altogether {len(feature_pool) - len(start_features)} new features in {max_steps} steps")
-        print("[feateng] Removing correlated features, as well as additions at the highest level")
+        logging.info(f"[feateng] Generated altogether {len(feature_pool) - len(start_features)} new features in {max_steps} steps")  # type: ignore
+        logging.info("[feateng] Removing correlated features, as well as additions at the highest level")
     feature_pool = {
-        c: feature_pool[c] for c in feature_pool if c in uncorr_features and not feature_pool[c].func == sympy.core.add.Add
+        c: feature_pool[c] for c in feature_pool if c in uncorr_features and feature_pool[c].func != sympy.core.add.Add
     }
     cols = [
         c for c in list(df.columns) if c in feature_pool and c not in df_org.columns
     ]  # categorical cols not in feature_pool
     if cols:
         # check for correlated features again; this time with the start features
         corrs = dict(
             zip(
                 cols,
                 np.max(
                     np.abs(
                         np.dot(StandardScaler().fit_transform(df[cols]).T, StandardScaler().fit_transform(df_org))
-                        / df_org.shape[0]
+                        / df_org.shape[0],
                     ),
                     axis=1,
                 ),
-            )
+            ),
         )
         cols = [c for c in cols if corrs[c] < 0.9]
     cols = list(df_org.columns) + cols
     if verbose > 0:
-        print(f"[feateng] Generated a total of {len(feature_pool) - len(start_features)} additional features")
+        logging.info(f"[feateng] Generated a total of {len(feature_pool) - len(start_features)} additional features")  # type: ignore
     return df[cols], feature_pool
```

### Comparing `autofeat-2.1.1/autofeat/featsel.py` & `autofeat-2.1.2/autofeat/featsel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
 from __future__ import annotations
+
+import logging
 import warnings
+from collections import Counter
+
 import numpy as np
 import pandas as pd
-from collections import Counter
+import sklearn.linear_model as lm
 from joblib import Parallel, delayed
 from sklearn.base import BaseEstimator
-from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
-import sklearn.linear_model as lm
-from .nb_utils import nb_standard_scale
+from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
+
+from autofeat.nb_utils import nb_standard_scale
+
+logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=logging.INFO)
 
 
 def _add_noise_features(X: np.ndarray):
     """
     Adds 3-1.5*d additional noise features to X.
 
     Inputs:
@@ -25,61 +31,61 @@
     n_feat = X.shape[1]
     if X.shape[0] > 50 and n_feat > 1:
         # shuffled features
         rand_noise = nb_standard_scale(np.random.permutation(X.flatten()).reshape(X.shape))
         X = np.hstack([X, rand_noise])
     # normally distributed noise
     rand_noise = np.random.randn(X.shape[0], max(3, int(0.5 * n_feat)))
-    X = np.hstack([X, rand_noise])
-    return X
+    return np.hstack([X, rand_noise])
 
 
 def _noise_filtering(
-    X: np.ndarray, target: np.ndarray, good_cols: list | None = None, problem_type: str = "regression"
+    X: np.ndarray,
+    target: np.ndarray,
+    good_cols: list | None = None,
+    problem_type: str = "regression",
 ) -> list:
     """
     Trains a prediction model with additional noise features and selects only those of the
     original features that have a higher coefficient than any of the noise features.
 
     Inputs:
         - X: n x d numpy array with d features
         - target: n dimensional array with targets corresponding to the data points in X
         - good_cols: list of column names for the features in X
         - problem_type: str, either "regression" or "classification" (default: "regression")
+
     Returns:
         - good_cols: list of noise filtered column names
     """
     n_feat = X.shape[1]
     if good_cols is None or not len(good_cols):
         good_cols = list(range(n_feat))
     assert len(good_cols) == n_feat, "fewer column names provided than features in X."
     # perform noise filtering on these features
     if problem_type == "regression":
         model = lm.LassoLarsCV(cv=5, eps=1e-8)
     elif problem_type == "classification":
         model = lm.LogisticRegressionCV(cv=5, penalty="l1", solver="saga", class_weight="balanced")
     else:
-        print(f"[featsel] WARNING: Unknown problem_type {problem_type} - not performing noise filtering.")
+        logging.warning(f"[featsel] Unknown problem_type {problem_type} - not performing noise filtering.")
         model = None
     if model is not None:
         X = _add_noise_features(X)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             # TODO: remove if sklearn least_angle issue is fixed
             try:
                 model.fit(X, target)
             except ValueError:
                 rand_idx = np.random.permutation(X.shape[0])
                 model.fit(X[rand_idx], target[rand_idx])
             # model.fit(X, target)
-        if problem_type == "regression":
-            coefs = np.abs(model.coef_)
-        else:
-            # model.coefs_ is n_classes x n_features, but we need n_features
-            coefs = np.max(np.abs(model.coef_), axis=0)
+        # for classification, model.coefs_ is n_classes x n_features, but we need n_features
+        coefs = np.abs(model.coef_) if problem_type == "regression" else np.max(np.abs(model.coef_), axis=0)
         weights = dict(zip(good_cols, coefs[: len(good_cols)]))
         # only include features that are more important than our known noise features
         noise_w_thr = np.max(coefs[n_feat:])
         good_cols = [c for c in good_cols if weights[c] > noise_w_thr]
     return good_cols
 
 
@@ -89,50 +95,48 @@
 
     Inputs:
         - df: nxp pandas DataFrame with n data points and p features; to avoid overfitting, only provide data belonging
               to the n training data points. The variables have to be scaled to have 0 mean and unit variance.
         - target: n dimensional array with targets corresponding to the data points in df
         - problem_type: str, either "regression" or "classification" (default: "regression")
         - verbose: verbosity level (int; default: 0)
+
     Returns:
         - good_cols: list of column names for df with which a prediction model can be trained
     """
     if df.shape[0] <= 1:
         raise ValueError(f"n_samples = {df.shape[0]}")
     # initial selection of too few but (hopefully) relevant features
     if problem_type == "regression":
         model = lm.LassoLarsCV(cv=5, eps=1e-8)
     elif problem_type == "classification":
         model = lm.LogisticRegressionCV(cv=5, penalty="l1", solver="saga", class_weight="balanced")
     else:
-        print(f"[featsel] WARNING: Unknown problem_type {problem_type} - not performing feature selection!")
+        logging.warning(f"[featsel] Unknown problem_type {problem_type} - not performing feature selection!")
         return []
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         # TODO: remove if sklearn least_angle issue is fixed
         try:
             model.fit(df, target)
         except ValueError:
             # try once more with shuffled data, if it still doesn't work, give up
             rand_idx = np.random.permutation(df.shape[0])
             model.fit(df.iloc[rand_idx], target[rand_idx])
         # model.fit(df, target)
-    if problem_type == "regression":
-        coefs = np.abs(model.coef_)
-    else:
-        # model.coefs_ is n_classes x n_features, but we need n_features
-        coefs = np.max(np.abs(model.coef_), axis=0)
+    # for classification, model.coefs_ is n_classes x n_features, but we need n_features
+    coefs = np.abs(model.coef_) if problem_type == "regression" else np.max(np.abs(model.coef_), axis=0)
     # weight threshold: select at most 0.2*n_train initial features
     thr = sorted(coefs, reverse=True)[min(df.shape[1] - 1, df.shape[0] // 5)]
     initial_cols = list(df.columns[coefs > thr])
     # noise filter
     initial_cols = _noise_filtering(df[initial_cols].to_numpy(), target, initial_cols, problem_type)
     good_cols_set = set(initial_cols)
     if verbose > 0:
-        print(f"[featsel]\t {len(initial_cols)} initial features.")
+        logging.info(f"[featsel]\t {len(initial_cols)} initial features.")
     # add noise features
     X_w_noise = _add_noise_features(df[initial_cols].to_numpy())
     # go through all remaining features in splits of n_feat <= 0.5*n_train
     other_cols = list(np.random.permutation(list(set(df.columns).difference(initial_cols))))
     if other_cols:
         n_splits = int(np.ceil(len(other_cols) / max(10, 0.5 * df.shape[0] - len(initial_cols))))
         split_size = int(np.ceil(len(other_cols) / n_splits))
@@ -149,32 +153,30 @@
                 try:
                     model.fit(X, target)
                 except ValueError:
                     rand_idx = np.random.permutation(X.shape[0])
                     model.fit(X[rand_idx], target[rand_idx])
                 # model.fit(X, target)
             current_cols.extend(initial_cols)
-            if problem_type == "regression":
-                coefs = np.abs(model.coef_)
-            else:
-                # model.coefs_ is n_classes x n_features, but we need n_features
-                coefs = np.max(np.abs(model.coef_), axis=0)
+            # for classification, model.coefs_ is n_classes x n_features, but we need n_features
+            coefs = np.abs(model.coef_) if problem_type == "regression" else np.max(np.abs(model.coef_), axis=0)
             weights = dict(zip(current_cols, coefs[: len(current_cols)]))
             # only include features that are more important than our known noise features
             noise_w_thr = np.max(coefs[len(current_cols) :])
             good_cols_set.update([c for c in weights if abs(weights[c]) > noise_w_thr])
             if verbose > 0:
                 print(
-                    f"[featsel]\t Split {i + 1:2}/{n_splits}: {len(good_cols_set):3} candidate features identified.", end="\r"
+                    f"[featsel]\t Split {i + 1:2}/{n_splits}: {len(good_cols_set):3} candidate features identified.",
+                    end="\r",
                 )
     # noise filtering on the combination of features
     good_cols = list(good_cols_set)
     good_cols = _noise_filtering(df[good_cols].to_numpy(), target, good_cols, problem_type)
     if verbose > 0:
-        print(f"\n[featsel]\t Selected {len(good_cols):3} features after noise filtering.")
+        logging.info(f"\n[featsel]\t Selected {len(good_cols):3} features after noise filtering.")
     return good_cols
 
 
 def select_features(
     df: pd.DataFrame,
     target: np.ndarray,
     featsel_runs: int = 5,
@@ -191,45 +193,43 @@
               to the n training data points.
         - target: n dimensional array with targets corresponding to the data points in df
         - featsel_runs: number of times to perform in the feature selection part with a random fraction of data points (int; default: 5)
         - keep: list of features that should be kept no matter what
         - problem_type: str, either "regression" or "classification" (default: "regression")
         - n_jobs: how many jobs to run when selecting the features in parallel (int; default: 1)
         - verbose: verbosity level (int; default: 0)
+
     Returns:
         - good_cols: list of column names for df with which a regression model can be trained
     """
     if not (len(df) == len(target)):
         raise ValueError("[featsel] df and target dimension mismatch.")
     if keep is None:
         keep = []
     # check that keep columns are actually in df (- the columns might have been transformed to strings!)
-    keep = [c for c in keep if c in df.columns and not str(c) in df.columns] + [str(c) for c in keep if str(c) in df.columns]
+    keep = [c for c in keep if c in df.columns and str(c) not in df.columns] + [str(c) for c in keep if str(c) in df.columns]
     # scale features to have 0 mean and unit std
     if verbose > 0:
         if featsel_runs > df.shape[0]:
-            print("[featsel] WARNING: Less data points than featsel runs!!")
+            logging.warning("[featsel] Less data points than featsel runs!!")
         print("[featsel] Scaling data...", end="")
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         df_scaled = pd.DataFrame(nb_standard_scale(df.to_numpy()), columns=df.columns, dtype=np.float32)
-        if problem_type == "regression":
-            target_scaled = nb_standard_scale(target.reshape(-1, 1)).ravel()
-        else:
-            target_scaled = target
+        target_scaled = nb_standard_scale(target.reshape(-1, 1)).ravel() if problem_type == "regression" else target
     if verbose > 0:
         print("done.")
 
     good_cols = list(df.columns)
 
     # select good features in k runs in parallel
     # by doing sort of a cross-validation (i.e., randomly subsample data points)
     def run_select_features(i: int):
         if verbose > 0:
-            print(f"[featsel] Feature selection run {i + 1}/{featsel_runs}")
+            logging.info(f"[featsel] Feature selection run {i + 1}/{featsel_runs}")
         np.random.seed(i)
         rand_idx = np.random.permutation(df_scaled.index)[: max(10, int(0.85 * len(df_scaled)))]
         return _select_features_1run(df_scaled.iloc[rand_idx], target_scaled[rand_idx], problem_type, verbose=verbose - 1)
 
     if featsel_runs >= 1 and problem_type in ("regression", "classification"):
         if n_jobs == 1 or featsel_runs == 1:
             # only use parallelization code if you actually parallelize
@@ -238,25 +238,27 @@
                 selected_columns.extend(run_select_features(i))
         else:
 
             def flatten_lists(l: list):
                 return [item for sublist in l for item in sublist]
 
             selected_columns = flatten_lists(
-                Parallel(n_jobs=n_jobs, verbose=100 * verbose)(delayed(run_select_features)(i) for i in range(featsel_runs))
+                Parallel(n_jobs=n_jobs, verbose=100 * verbose)(delayed(run_select_features)(i) for i in range(featsel_runs)),
             )
 
         if selected_columns:
-            selected_columns = Counter(selected_columns)
+            selected_columns_counter = Counter(selected_columns)
             # sort by frequency, but down weight longer formulas to break ties
             selected_columns = sorted(
-                selected_columns, key=lambda x: selected_columns[x] - 0.000001 * len(str(x)), reverse=True
+                selected_columns_counter,
+                key=lambda x: selected_columns_counter[x] - 0.000001 * len(str(x)),
+                reverse=True,
             )
             if verbose > 0:
-                print(f"[featsel] {len(selected_columns)} features after {featsel_runs} feature selection runs")
+                logging.info(f"[featsel] {len(selected_columns)} features after {featsel_runs} feature selection runs")
             # correlation filtering
             selected_columns = keep + [c for c in selected_columns if c not in keep]
             if not keep:
                 good_cols = [selected_columns[0]]
                 k = 1
             else:
                 good_cols = keep
@@ -264,27 +266,27 @@
             if len(selected_columns) > k:
                 correlations = df_scaled[selected_columns].corr()
                 for i, c in enumerate(selected_columns[k:], k):
                     # only take features that are somewhat uncorrelated with the rest
                     if np.max(np.abs(correlations[c].ravel()[:i])) < 0.9:
                         good_cols.append(c)
             if verbose > 0:
-                print(f"[featsel] {len(good_cols)} features after correlation filtering")
+                logging.info(f"[featsel] {len(good_cols)} features after correlation filtering")
 
     # perform noise filtering on these features
     good_cols = _noise_filtering(df_scaled[good_cols].to_numpy(), target_scaled, good_cols, problem_type)
     if verbose > 0:
-        print(f"[featsel] {len(good_cols)} features after noise filtering")
+        logging.info(f"[featsel] {len(good_cols)} features after noise filtering")
         if not good_cols:
-            print("[featsel] WARNING: Not a single good features was found...")
+            logging.warning("[featsel] Not a single good features was found...")
 
     # add keep columns back in
     good_cols = keep + [c for c in good_cols if c not in keep]
     if verbose > 0 and keep:
-        print(f"[featsel] {len(good_cols)} final features selected (including {len(keep)} original keep features).")
+        logging.info(f"[featsel] {len(good_cols)} final features selected (including {len(keep)} original keep features).")
     return good_cols
 
 
 class FeatureSelector(BaseEstimator):
     def __init__(
         self,
         problem_type: str = "regression",
@@ -333,30 +335,37 @@
         if not cols:
             cols = [f"x{i}" for i in range(X.shape[1])]
         self.original_columns_ = cols
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=cols)
         # do the feature selection
         self.good_cols_ = select_features(
-            df, target, self.featsel_runs, self.keep, self.problem_type, self.n_jobs, self.verbose
+            df,
+            target,
+            self.featsel_runs,
+            self.keep,
+            self.problem_type,
+            self.n_jobs,
+            self.verbose,
         )
         self.n_features_in_ = X.shape[1]
         return self
 
     def transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+
         Returns:
             - new_X: new pandas dataframe or numpy array with only the good features
         """
         check_is_fitted(self, ["good_cols_"])
         if not self.good_cols_:
             if self.verbose > 0:
-                print("[FeatureSelector] WARNING: No good features found; returning data unchanged.")
+                logging.warning("[FeatureSelector] No good features found; returning data unchanged.")
             return X
         # store column names as they'll be lost in the other check
         # first calling np.array assures that all the column names have the same dtype
         # as otherwise we get problems when calling np.random.permutation on the columns
         cols = list(np.array(list(X.columns))) if isinstance(X, pd.DataFrame) else []
         # check input variables
         X = check_array(X, force_all_finite="allow-nan")
```

### Comparing `autofeat-2.1.1/autofeat/nb_utils.py` & `autofeat-2.1.2/autofeat/nb_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Author: Jeethu Rao <jboloor@acm.org>
 # License: MIT
 
 from __future__ import annotations
+
 import numba as nb
 import numpy as np
 
 
 @nb.njit(inline="always")
 def nb_apply_along_axis(func1d, axis, arr):
     assert arr.ndim == 2
```

