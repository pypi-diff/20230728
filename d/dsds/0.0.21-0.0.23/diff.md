# Comparing `tmp/dsds-0.0.21.tar.gz` & `tmp/dsds-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.21.tar", last modified: Tue Jul 18 16:14:46 2023, max compression
+gzip compressed data, was "dsds-0.0.23.tar", last modified: Fri Jul 28 04:34:34 2023, max compression
```

## Comparing `dsds-0.0.21.tar` & `dsds-0.0.23.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 16:14:46.431888 dsds-0.0.21/
--rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.21/LICENSE
--rw-rw-rw-   0        0        0     6759 2023-07-18 16:14:46.431888 dsds-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0     4387 2023-07-11 16:38:19.000000 dsds-0.0.21/README.md
--rw-rw-rw-   0        0        0     1398 2023-07-18 16:14:22.000000 dsds-0.0.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 16:14:46.431888 dsds-0.0.21/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 16:14:46.399628 dsds-0.0.21/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 16:14:46.416259 dsds-0.0.21/src/dsds/
--rw-rw-rw-   0        0        0       87 2023-07-18 16:14:32.000000 dsds-0.0.21/src/dsds/__init__.py
--rw-rw-rw-   0        0        0     7663 2023-07-18 15:54:32.000000 dsds-0.0.21/src/dsds/blueprint.py
--rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.21/src/dsds/eda_text.py
--rw-rw-rw-   0        0        0    32902 2023-07-16 03:51:24.000000 dsds-0.0.21/src/dsds/fs.py
--rw-rw-rw-   0        0        0     9077 2023-07-13 03:33:56.000000 dsds-0.0.21/src/dsds/metrics.py
--rw-rw-rw-   0        0        0    30539 2023-07-18 15:20:27.000000 dsds-0.0.21/src/dsds/prescreen.py
--rw-rw-rw-   0        0        0    15697 2023-07-16 03:59:12.000000 dsds-0.0.21/src/dsds/sample.py
--rw-rw-rw-   0        0        0    44312 2023-07-18 15:26:06.000000 dsds-0.0.21/src/dsds/transform.py
--rw-rw-rw-   0        0        0     2988 2023-07-18 16:07:35.000000 dsds-0.0.21/src/dsds/type_alias.py
--rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.21/src/dsds/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:14:46.431888 dsds-0.0.21/src/dsds.egg-info/
--rw-rw-rw-   0        0        0     6759 2023-07-18 16:14:46.000000 dsds-0.0.21/src/dsds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-18 16:14:46.000000 dsds-0.0.21/src/dsds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 16:14:46.000000 dsds-0.0.21/src/dsds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-07-18 16:14:46.000000 dsds-0.0.21/src/dsds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-18 16:14:46.000000 dsds-0.0.21/src/dsds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.077995 dsds-0.0.23/
+-rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.23/LICENSE
+-rw-rw-rw-   0        0        0     9216 2023-07-28 04:34:34.077995 dsds-0.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0     6844 2023-07-27 22:37:38.000000 dsds-0.0.23/README.md
+-rw-rw-rw-   0        0        0     1398 2023-07-24 20:26:15.000000 dsds-0.0.23/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:34:34.077995 dsds-0.0.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.019562 dsds-0.0.23/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.058757 dsds-0.0.23/src/dsds/
+-rw-rw-rw-   0        0        0       87 2023-07-23 18:27:29.000000 dsds-0.0.23/src/dsds/__init__.py
+-rw-rw-rw-   0        0        0    14049 2023-07-27 04:22:14.000000 dsds-0.0.23/src/dsds/blueprint.py
+-rw-rw-rw-   0        0        0      206 2023-07-27 04:58:44.000000 dsds-0.0.23/src/dsds/compare.py
+-rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.23/src/dsds/eda_text.py
+-rw-rw-rw-   0        0        0    26636 2023-07-27 05:09:06.000000 dsds-0.0.23/src/dsds/encoders.py
+-rw-rw-rw-   0        0        0    37634 2023-07-25 05:03:42.000000 dsds-0.0.23/src/dsds/fs.py
+-rw-rw-rw-   0        0        0    11007 2023-07-26 03:13:51.000000 dsds-0.0.23/src/dsds/metrics.py
+-rw-rw-rw-   0        0        0    38259 2023-07-28 04:30:11.000000 dsds-0.0.23/src/dsds/prescreen.py
+-rw-rw-rw-   0        0        0    20414 2023-07-27 15:49:24.000000 dsds-0.0.23/src/dsds/sample.py
+-rw-rw-rw-   0        0        0    28954 2023-07-28 04:16:34.000000 dsds-0.0.23/src/dsds/transform.py
+-rw-rw-rw-   0        0        0     3510 2023-07-28 04:29:38.000000 dsds-0.0.23/src/dsds/type_alias.py
+-rw-rw-rw-   0        0        0    14259 2023-07-27 04:37:24.000000 dsds-0.0.23/src/dsds/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:34:34.075995 dsds-0.0.23/src/dsds.egg-info/
+-rw-rw-rw-   0        0        0     9216 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 04:34:34.000000 dsds-0.0.23/src/dsds.egg-info/top_level.txt
```

### Comparing `dsds-0.0.21/LICENSE` & `dsds-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `dsds-0.0.21/PKG-INFO` & `dsds-0.0.23/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,10 @@
-Metadata-Version: 2.1
-Name: dsds
-Version: 0.0.21
-Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
-Author-email: Tianren Qin <tq9695@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 T.Q
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
-Project-URL: Homepage, https://github.com/abstractqqq/dsds
-Keywords: data pipeline,EDA,feature-screening,feature-selection
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: scikit-learn
-Provides-Extra: xgboost
-Provides-Extra: lightgbm
-Provides-Extra: all
-License-File: LICENSE
-
 # Welcome to the Dark Side of Data Science (DSDS)
 
-This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package.
+This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package. Also see disclaimer in the end.
 
 Welcome to DSDS, a data science package that aims to be an improvement over a subset of sklearn's functionality, primarily in the following areas:
 
 1. Providing practical feature prescreen (immediate detection and removal of useless featuers, data profiling, etc.)
 2. Fast and furious feature selection (significantly faster F-score, MRMR, mutual_info_score, etc.)
 3. Cleaner pipeline construction and management (See examples below.)
 4. Compatible with Polars LazyFrames (Yes! Pipelines can enjoy the benefits of query optimization too!)
@@ -102,15 +54,17 @@
 
 Performance without sacrificing user experience. See ./examples/dsds_comparisons.ipynb
 
 ![Screenshot](./pics/impute.PNG)
 
 ## Dependencies
 
-Python 3.9, 3.10, 3.11+ is recommended. We are forward looking.
+Python 3.9, 3.10, 3.11+ is recommended. We are forward looking. 
+
+It should run on all versions >= 3.9. But I haven't tested 3.9 and 3.10 thoroughly.
 
 pip install polars scipy numpy
 
 pip install dsds[all]
 
 Note: scikit-learn, lightgbm, xgboost are needed for full functionalities. 
 
@@ -134,8 +88,27 @@
 
 You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
 
 # Why not write more functionalities in Rust?
 
 Yes. I will. I am not confident enough with my Rust skill at the moment. I am slowly learning more Rust and hopefully we can delegate more heavy work to Rust. The immediate benefit of using more Rust will be (1) slightly more memory efficient, and (2) slightly faster. I do not expect huge speed boost because most code are written in Polars already. There are some cases when a lot of Python stuff is added (lists and for loops, etc.). But we definitely need to evaluate the gain by using Rust more carefully in the future.
 
-See CONTRIBUTING.md for my contact info.
+# Disclaimer
+
+I do not claim dsds is a superior package to any other traditional machine learning libraries. In fact no one can make this claim. Each package has their own flavor, and there are things that people can disagree with. Disagreements do not translate to contempt or hatred. I primarily set out to make this project because:
+
+1. I want to learn more about machine learning engineering
+2. I want to improve my coding skill
+3. I see opportunies to make things run faster using Polars without relying on bigger machines on the cloud. I want to make this happen for everybody.
+4. I don't think OOP is right for scientific computing.
+
+Everyone has their own bias. I believe in the functional style for scientific computing. I don't like the OOP style adopted by so many other packages, especially the one used in Sklearn pipelines. If you want to discuss, please kindly send me a message on discord. Please do not cherry pick points and claim that my code is **** just because you have never seen functional codebase or projects done in this style. I do not claim to have the best style of code either. OOP elements are still used in this project because it is inevitable in Python.
+
+That said, since performance and functional design are the two major pillars of this project, I will include a lot of benchmarks and code that showcase the style differences. A lot of benchmarks will be done vs. Scikit-learn because Scikit-learn is the de facto "standard" in the tranditional machine learning space. I do this not because I want to prove dsds is superior, but because I want to show the improvement and show people that dsds achieves what it aims to achieve, an improvement over a subset of Scikit-learn's functionalities (in the areas that I set out to improve on, e.g. performance and 'style').
+
+Every few days there is a new javascript framework. Why can't data scientists challenge the design of Scikit-learn? I started learning using Scikit-learn, like 90% of all the data scientists out there. I am free to express my opinions and criticisms. 
+
+No package is perfect and you are free to like/hate it. Just don't be complaining online without ever thinking deeply about machine learning infra and bottlenecks in machine learning pipelines. Don't hate on things because they are different.
+
+# Contribution
+
+See CONTRIBUTING.md for my contact info.
```

### Comparing `dsds-0.0.21/pyproject.toml` & `dsds-0.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "dsds"
-version = "0.0.21"
+version = "0.0.23"
 requires-python = ">=3.9"
 readme = "README.md"
 description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
 authors = [
     {name = "Tianren Qin", email = "tq9695@gmail.com"}
 ]
 license = {file = "LICENSE"}
 dependencies = [
-    "polars >= 0.18.6",
+    "polars >= 0.18.7",
     "scipy >= 1.11.1",
     "pandas",
     "numpy",
     "typing_extensions >= 4.0.1"
 ]
 
 keywords = ["data pipeline", "EDA", "feature-screening", "feature-selection"]
```

### Comparing `dsds-0.0.21/src/dsds/eda_text.py` & `dsds-0.0.23/src/dsds/eda_text.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.21/src/dsds/fs.py` & `dsds-0.0.23/src/dsds/fs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from .prescreen import (
     discrete_inferral
     , check_binary_target
     , get_numeric_cols
     , get_unique_count
     , get_string_cols
     , type_checker
+    , select
 )
 
 from .type_alias import (
     PolarsFrame
     , MRMRStrategy
     , BinaryModels
-    , CPU_COUNT
+    , CPU_M1
     , clean_strategy_str
     , ClassifModel
 )
 from .blueprint import( # Need this for Polars extension to work
     Blueprint
 )
 from .sample import (
@@ -23,25 +24,81 @@
 )
 from .metrics import (
     logloss
     , roc_auc
 )
 import polars as pl
 import numpy as np
-from typing import Any, Optional, Tuple
+from typing import Any, Optional, Tuple, Union
 from scipy.spatial import KDTree
 from scipy.special import fdtrc, psi
 from concurrent.futures import ThreadPoolExecutor, as_completed
 import logging
 from tqdm import tqdm
 import math
 from itertools import combinations
 
 logger = logging.getLogger(__name__)
 
+def corr(
+    df: PolarsFrame
+    , target: str
+    , cols: Optional[list[str]] = None
+) -> pl.DataFrame:
+    '''
+    Returns a dataframe with features and their correlation with target.
+
+    Parameters
+    ----------
+    df 
+        Either an eager or lazy Polars dataframe
+    target
+        The target column
+    cols
+        List of numerical columns. If not provided, will use all numerical columns
+    '''
+    if isinstance(cols, list):
+        _ = type_checker(df, cols, "numeric", "corr_filter")
+        nums = cols
+    else:
+        nums = get_numeric_cols(df)
+
+    return df.lazy().select(pl.corr(c, target).abs() for c in nums)\
+        .collect()\
+        .transpose(include_header=True, column_names=["abs_corr"])
+
+def corr_selector(
+    df: PolarsFrame
+    , target: str
+    , threshold: float
+) -> PolarsFrame:
+    '''
+    Keeps only the columns that have |correlation with target| > threshold and the ones that cannot be 
+    processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or a lazy Polars DataFrame.
+    target
+        The target column
+    threshold
+        The threshold above which the features will be selected
+    '''
+    nums = get_numeric_cols(df, exclude=[target])
+    complement = [f for f in df.columns if f not in nums]
+    # select high corr columns
+    to_select = corr(df, target, nums)\
+                .filter(pl.col("abs_corr") >= threshold)\
+                .get_column("column").to_list()
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the algorithm "
+          "cannot process. They are also returned.")
+    # add the complement set
+    return select(df, to_select + complement, persist=True)
+
 def discrete_ig(
     df:pl.DataFrame
     , target:str
     , cols:Optional[list[str]] = None
 ) -> pl.DataFrame:
 
     if isinstance(cols, list):
@@ -85,43 +142,50 @@
 
 discrete_mi = discrete_ig
 
 def discrete_ig_selector(
     df:PolarsFrame
     , target:str
     , top_k:int
-    , n_threads:int = CPU_COUNT
 ) -> PolarsFrame:
-    
-    discrete_cols = discrete_inferral(df, exclude=[target])
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
+    '''
+    Keeps only the top_k features in terms of discrete_ig and the ones that cannot be processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or lazy dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        Only the top_k features in terms of discrete_ig will be selected 
+    '''
+    if isinstance(df, pl.LazyFrame):
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
-    ig = discrete_ig(input_data, target, discrete_cols, n_threads)\
-            .top_k(by="information_gain", k = top_k)
+    discrete_cols = discrete_inferral(df, exclude=[target])
+    complement = [f for f in df.columns if f not in discrete_cols]
+    to_select = discrete_ig(input_data, target, discrete_cols)\
+        .top_k(by="information_gain", k = top_k)\
+        .get_column("feature").to_list()
+
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
 
-    complement = [f for f in input_data.columns if f not in discrete_cols]
-    selected = ig.get_column("feature").to_list()
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-        "cannot process. They are also returned.")
-
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
+    return select(df, to_select + complement, persist=True)
 
 def mutual_info(
     df:pl.DataFrame
     , target:str
     , conti_cols:list[str]
     , n_neighbors:int=3
     , seed:int=42
-    , n_threads:int=CPU_COUNT
+    , n_threads:int=CPU_M1
 ) -> pl.DataFrame:
     '''
     Approximates mutual information (information gain) between the continuous variables and the target. This
     is essentially the same as sklearn's implementation, except that
 
     1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors
     2. This uses all cores by default
@@ -196,207 +260,223 @@
     return pl.from_records((conti_cols, estimates), schema=["feature", "estimated_mi"])
 
 # Selectors should always return target
 def mutual_info_selector(
     df:PolarsFrame
     , target:str
     , n_neighbors:int=3
-    , seed:int=42
-    , n_threads:int=CPU_COUNT
     , top_k:int = 50
+    , n_threads:int=CPU_M1
+    , seed:int=42
 ) -> PolarsFrame:
     '''
-    A selector based on the mutual_info feature selection method.
+    Keeps only the top_k features in terms of mutual_info_score and the ones that cannot be processed by the algorithm.
 
-    This 
-    
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    n_neighbors
+        The n_neighbors parameter in the approximation method
+    top_k
+        The top_k features will ke kept
+    n_threads
+        The max number of workers for multithreading
+    seed
+        Random seed used in approximation to generate noise
     '''
-    
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
+    if isinstance(df, pl.LazyFrame):
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
-    nums = get_numeric_cols(input_data, exclude=[target])
-    complement = [f for f in input_data.columns if f not in nums]
+    nums = get_numeric_cols(df, exclude=[target])
+    complement = [f for f in df.columns if f not in nums]
+    to_select = mutual_info(input_data, target, nums, n_neighbors, seed, n_threads)\
+                .top_k(by="estimated_mi", k = top_k)\
+                .get_column("feature").to_list()
 
-    mi_scores = mutual_info(input_data, target, nums, n_neighbors, seed, n_threads)\
-                .top_k(by="estimated_mi", k = top_k)
+    logger.info(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
 
-    selected = mi_scores.get_column("feature").to_list()
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-        "cannot process. They are also returned.")
-
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
+    return select(df, to_select + complement, persist=True)
 
 def _f_score(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , num_list:list[str]
 ) -> np.ndarray:
-    '''Same as f_classif, but returns a numpy array of f scores only.'''
+    '''
+    This is the same as what is in f_classif to compute f_score. Except that this only 
+    returns a numpy array of f scores and this does not error check.
+    '''
     
-    # See comments in f_classif
-    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")]
+    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] 
     step_two_expr:list[pl.Expr] = []
-    step_three_expr:list[pl.Expr] = []
     for n in num_list:
-        n_avg:str = n + "_avg"
-        n_tavg:str = n + "_tavg"
-        n_var:str = n + "_var"
+        n_sum:str = n + "_sum" # sum of class
+        n_var:str = n + "_var" # var within class
         step_one_expr.append(
-            pl.col(n).mean().alias(n_avg)
+            pl.col(n).sum().alias(n_sum)
         )
         step_one_expr.append(
-            pl.col(n).var(ddof=0).alias(n_var)
+            pl.col(n).var(ddof=0).alias(n_var) 
         )
         step_two_expr.append(
-            (pl.col(n_avg).dot(pl.col("cnt")) / len(df)).alias(n_tavg)
-        )
-        step_three_expr.append(
-            (pl.col(n_avg) - pl.col(n_tavg)).pow(2).dot(pl.col("cnt"))/ pl.col(n_var).dot(pl.col("cnt"))
+            (pl.col(n_sum)/pl.col("cnt") - pl.col(n_sum).sum()/pl.col("cnt").sum()).pow(2).dot(pl.col("cnt")) 
+            / pl.col(n_var).dot(pl.col("cnt"))
         )
 
-    ref = df.groupby(target).agg(step_one_expr)
-    n_samples = len(df)
-    n_classes = len(ref)
+    ref = (
+        df.lazy().groupby(target).agg(step_one_expr)
+        .select(
+            pl.col("cnt").sum().alias("n_samples")
+            , pl.col(target).len().alias("n_classes")
+            , *step_two_expr
+        ).collect()
+    )
+    
+    n_samples = ref.drop_in_place("n_samples")[0]
+    n_classes = ref.drop_in_place("n_classes")[0]
     df_btw_class = n_classes - 1 
     df_in_class = n_samples - n_classes
-    # This is f-score, score in the order of num_list
-    return ref.with_columns(step_two_expr).select(step_three_expr)\
-            .to_numpy().ravel() * (df_in_class / df_btw_class)
+
+    return ref.to_numpy().ravel() * (df_in_class / df_btw_class)
 
 def f_classif(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , cols:Optional[list[str]]=None
 ) -> pl.DataFrame:
-    '''Computes ANOVA one way test, the f value/score and the p value. 
-        Equivalent to f_classif in sklearn.feature_selection, but is more dataframe-friendly, 
-        and performs better on bigger data.
-
-        Arguments:
-            df: input Polars dataframe.
-            target: the target column.
-            cols: if provided, will run the ANOVA one way test for each column in num_cols. If none,
-                will try to infer from df according to data types. Note that num_cols should be numeric!
+    '''
+    Computes ANOVA one way test, the f value/score and the p value. Equivalent to f_classif in sklearn.feature_selection
+    , but is more dataframe-friendly and faster. 
 
-        Returns:
-            a polars dataframe with f score and p value.
-    
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars DataFrame
+    target
+        The target column
+    cols
+        If not provided, will use all inferred numeric columns
     '''
     if isinstance(cols, list):
         nums = cols
     else:
         nums = get_numeric_cols(df, exclude=[target])
 
-    # Get average within group and sample variance within group.
-    ## Could potentially replace this with generators instead of lists. Not sure how impactful that would be... Probably no diff.
-    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] # get cnt, and avg within classes
-    step_two_expr:list[pl.Expr] = [] # Get average for each column
-    step_three_expr:list[pl.Expr] = [] # Get "f score" (without some normalizer, see below)
-    # Minimize the amount of looping and str concating in Python. Use Exprs as much as possible.
+    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] 
+    step_two_expr:list[pl.Expr] = []
     for n in nums:
-        n_avg:str = n + "_avg" # avg within class
-        n_tavg:str = n + "_tavg" # true avg / overall average
+        n_sum:str = n + "_sum" # sum of class
         n_var:str = n + "_var" # var within class
         step_one_expr.append(
-            pl.col(n).mean().alias(n_avg)
+            pl.col(n).sum().alias(n_sum)
         )
         step_one_expr.append(
-            pl.col(n).var(ddof=0).alias(n_var) # ddof = 0 so that we don't need to compute pl.col("cnt") - 1
-        )
-        step_two_expr.append( # True average of this column, reduce the amount of repeated computation.
-            # by using n_avg column dotted with cnt
-            (pl.col(n_avg).dot(pl.col("cnt")) / len(df)).alias(n_tavg)
+            pl.col(n).var(ddof=0).alias(n_var) 
         )
-        step_three_expr.append(
-            # Between class var (without diving by df_btw_class) / Within class var (without dividng by df_in_class) 
-            (pl.col(n_avg) - pl.col(n_tavg)).pow(2).dot(pl.col("cnt"))/ pl.col(n_var).dot(pl.col("cnt"))
+        step_two_expr.append(
+            (pl.col(n_sum)/pl.col("cnt") - pl.col(n_sum).sum()/pl.col("cnt").sum()).pow(2).dot(pl.col("cnt")) 
+            / pl.col(n_var).dot(pl.col("cnt"))
         )
 
-    # Get in class average and var
-    ref = df.groupby(target).agg(step_one_expr)
-    n_samples = len(df)
-    n_classes = len(ref)
+    ref = (
+        df.lazy().groupby(target).agg(step_one_expr)
+        .select(
+            pl.col("cnt").sum().alias("n_samples")
+            , pl.col(target).len().alias("n_classes")
+            , *step_two_expr
+        ).collect()
+    )
+    n_samples = ref.drop_in_place("n_samples")[0]
+    n_classes = ref.drop_in_place("n_classes")[0]
     df_btw_class = n_classes - 1 
     df_in_class = n_samples - n_classes
+
+    if df_btw_class == 0:
+        raise ZeroDivisionError("Target has only one class.")
     
-    f_values = ref.with_columns(step_two_expr).select(step_three_expr)\
-            .to_numpy().ravel() * (df_in_class / df_btw_class)
+    f_values = ref.to_numpy().ravel() * (df_in_class / df_btw_class)
     # We should scale this by (df_in_class / df_btw_class) because we did not do this earlier
     # At this point, f_values should be a pretty small dataframe. 
     # Cast to numpy, so that fdtrc can process it properly.
 
     p_values = fdtrc(df_btw_class, df_in_class, f_values) # get p values 
     return pl.from_records((nums, f_values, p_values), schema=["feature","f_value","p_value"])
 
 def f_score_selector(
     df:PolarsFrame
     , target:str
     , top_k:int
 ) -> PolarsFrame:
+    '''
+    Keeps only the top_k features in terms of f-score and the ones that cannot be processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        The top_k features will ke kept
+    '''
     
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
+    if isinstance(df, pl.LazyFrame):
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
     nums = get_numeric_cols(input_data, exclude=[target])
-    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in input_data.columns if f not in nums]
-
+    complement = [f for f in df.columns if f not in nums]
     scores = _f_score(input_data, target, nums)
-    temp_df = pl.DataFrame({"feature":nums, "fscore":scores}).top_k(
-        by = "fscore", k = top_k
-    )
-    selected = temp_df.get_column("feature").to_list()
-    
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-    "cannot process. They are also returned.")
+    to_select = pl.DataFrame({"feature":nums, "fscore":scores})\
+        .top_k(by = "fscore", k = top_k)\
+        .get_column("feature").to_list()
 
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
+
+    return select(df, to_select + complement, persist=True)
 
 def _mrmr_underlying_score(
     df:pl.DataFrame
     , target:str
-    , num_list:list[str]
+    , nums:list[str]
     , strategy:MRMRStrategy
     , params:dict[str,Any]
 ) -> np.ndarray:
     
-    print(f"Running {strategy} to determine feature relevance...")
+    logger.info(f"Running {strategy} to determine feature relevance...")
     s = clean_strategy_str(strategy)
     if s in ("fscore", "f", "f_score"):
-        scores = _f_score(df, target, num_list)
+        scores = _f_score(df, target, nums)
     elif s in ("rf", "random_forest"):
         from sklearn.ensemble import RandomForestClassifier
         print("Random forest is not deterministic by default. Results may vary.")
         rf = RandomForestClassifier(**params)
-        rf.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
+        rf.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
         scores = rf.feature_importances_
     elif s in ("xgb", "xgboost"):
         from xgboost import XGBClassifier
         print("XGB is not deterministic by default. Results may vary.")
         xgb = XGBClassifier(**params)
-        xgb.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
+        xgb.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
         scores = xgb.feature_importances_
     elif s in ("mis", "mutual_info_score"):
-        scores = mutual_info(df, conti_cols=num_list, target=target).get_column("estimated_mi").to_numpy().ravel()
+        scores = mutual_info(df, conti_cols=nums, target=target).get_column("estimated_mi").to_numpy().ravel()
     elif s in ("lgbm", "lightgbm"):
         from lightgbm import LGBMClassifier
         print("LightGBM is not deterministic by default. Results may vary.")
         lgbm = LGBMClassifier(**params)
-        lgbm.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
+        lgbm.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
         scores = lgbm.feature_importances_
     else: # Pythonic nonsense
         raise ValueError(f"The strategy {strategy} is not a valid MRMR Strategy.")
     
     return scores
 
 def mrmr(
@@ -428,29 +508,24 @@
         MRMR strategy. By default, `fscore` will be used.
     params
         Optional. If a model strategy is selected (`rf`, `xgb`, `lgbm`), params is a dict of 
         parameters for the model.
     low_memory
         Whether to do some computation all at once, which uses more memory at once, or do some 
         computation when needed, which uses less memory at any given time.
-
-    Returns
-    -------
-        A list of top k features
-    
     '''
     if isinstance(cols, list):
         nums = cols
     else:
         nums = get_numeric_cols(df, exclude=[target])
 
     s = clean_strategy_str(strategy)
     scores = _mrmr_underlying_score(df
         , target = target
-        , num_list = nums
+        , nums = nums
         , strategy = s
         , params = {} if params is None else params
     )
 
     if low_memory:
         df_local = df.select(nums)
     else: # this could potentially double memory usage. so I provided a low_memory flag.
@@ -501,81 +576,105 @@
     , target:str
     , top_k:int
     , strategy:MRMRStrategy = "fscore"
     , params:Optional[dict[str,Any]] = None
     , low_memory:bool=False
 ) -> PolarsFrame:
     '''
-    '''
+    Keeps only the top_k (first k) features selected by MRMR and the ones that cannot be processed by the algorithm.
 
-    is_lazy = isinstance(df, pl.LazyFrame)
-    if is_lazy:
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        The top_k features will ke kept
+    strategy
+        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
+    params
+        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
+    low_memory
+        If true, use less memory. But the computation will take longer
+    '''
+    if isinstance(df, pl.LazyFrame):
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
     nums = get_numeric_cols(input_data, exclude=[target])
-    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in input_data.columns if f not in nums]
     s = clean_strategy_str(strategy)
-    selected = mrmr(input_data, target, top_k, nums, s, params, low_memory)
-
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-          "cannot process. They are also returned.")
-    
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
+    to_select = mrmr(input_data, target, top_k, nums, s, params, low_memory)
+    logger.info(f"Selected {len(to_select)} features. There are {len(df.columns) - len(to_select)} columns the "
+          "algorithm cannot process. They are also returned.")
+    to_select.extend(f for f in df.columns if f not in nums)
+    return select(df, to_select, persist=True)
 
 def knock_out_mrmr(
     df:pl.DataFrame
     , target:str
     , k:int 
-    , num_cols:Optional[list[str]] = None
-    , strategy:MRMRStrategy = "fscore"
+    , cols:Optional[list[str]] = None
     , corr_threshold:float = 0.7
+    , strategy:MRMRStrategy = "fscore"
     , params:Optional[dict[str,Any]] = None
 ) -> list[str]:
     '''
     Essentially the same as vanilla MRMR. Instead of using sum(abs(corr)) to "weigh down" correlated 
     variables, here we use a simpler knock out rule based on absolute correlation. We go down the list
     according to importance, take top one, knock out all other features that are highly correlated with
     it, take the next top feature that has not been knocked out, continue, until we pick enough features
     or there is no feature left.
 
     Inspired by the package Featurewiz and its creator.
 
-
-    
+    Parameters
+    ----------
+    df
+        An eager Polars Dataframe
+    target
+        The target column
+    k
+        The top k features to return
+    cols
+        Numerical columns to select from. If not provided, all numeric columns will be used
+    corr_threshold
+        The threshold above which correlation is considered too high. This means if A has high correlation to B, then
+        B will not be selected if A is
+    strategy
+        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
+    params
+        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
     '''
-    if isinstance(num_cols, list):
-        num_list = num_cols
+    if isinstance(cols, list):
+        nums = cols
     else:
-        num_list = get_numeric_cols(df, exclude=[target])
+        nums = get_numeric_cols(df, exclude=[target])
 
     s = clean_strategy_str(strategy)
     scores = _mrmr_underlying_score(df
         , target = target
-        , num_list = num_list
+        , nums = nums
         , strategy = s
         , params = {} if params is None else params
     )
 
     # Set up
-    low_corr = np.abs(df[num_list].corr().to_numpy()) < corr_threshold
-    surviving_indices = np.full(shape=len(num_list), fill_value=True) # an array of booleans
+    low_corr = np.abs(df[nums].corr().to_numpy()) < corr_threshold
+    surviving_indices = np.full(shape=len(nums), fill_value=True) # an array of booleans
     scores = sorted(enumerate(scores), key=lambda x:x[1], reverse=True)
     selected = []
     count = 0
-    output_size = min(k, len(num_list))
+    output_size = min(k, len(nums))
     pbar = tqdm(total=output_size)
     # Run the knock outs
     for i, _ in scores:
         if surviving_indices[i]:
-            selected.append(num_list[i])
+            selected.append(nums[i])
             surviving_indices = surviving_indices & low_corr[:,i]
             count += 1
             pbar.update(1)
         if count >= output_size:
             break
 
     pbar.close()
@@ -586,54 +685,63 @@
     print("Output is sorted in order of selection (max relevance min redundancy).")
     return selected
 
 def knock_out_mrmr_selector(
     df:PolarsFrame
     , target:str
     , top_k:int 
-    , strategy:MRMRStrategy = "fscore"
     , corr_threshold:float = 0.7
+    , strategy:MRMRStrategy = "fscore"
     , params:Optional[dict[str,Any]] = None
 ) -> PolarsFrame:
     '''
-    Performs knock out MRMR
-    '''
+    Keeps only the top_k (first k) features selected by MRMR and the ones that cannot be processed by the algorithm.
 
-    is_lazy = isinstance(df, pl.LazyFrame)
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        The top_k features will ke kept
+    corr_threshold
+        The threshold above which correlation is considered too high. This means if A has high correlation to B, then
+        B will not be selected if A is
+    strategy
+        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
+    params
+        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
+    '''
     if isinstance(df, pl.LazyFrame):
         input_data:pl.DataFrame = df.collect()
     else:
         input_data:pl.DataFrame = df
 
-    num_cols = get_numeric_cols(df, exclude=[target])
-    # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in df.columns if f not in num_cols]
-
+    nums = get_numeric_cols(df, exclude=[target])
+    complement = [f for f in df.columns if f not in nums]
     s = clean_strategy_str(strategy)
-    selected = knock_out_mrmr(input_data, target, top_k, num_cols, s, corr_threshold, params)
-    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
-        "cannot process. They are also returned.")
+    to_select = knock_out_mrmr(input_data, target, top_k, nums, s, corr_threshold, params)
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
     
-    if is_lazy:
-        return df.blueprint.select(selected + complement)
-    return df.select(selected + complement)
+    return select(df, to_select + complement, persist=True)
 
 # Selectors for the methods below are not yet implemented
 
-# Create a numeric + string version of woe_iv in the future
-def woe_iv_cat(
+def woe_iv(
     df:PolarsFrame
     , target:str
     , cols:Optional[list[str]]=None
     , min_count:float = 1.
     , check_binary:bool = True
 ) -> pl.DataFrame:
     '''
-    Computes information values for categorical variables. Notice that by using binning methods provided, you can turn
-    numerical values into categorical bins.
+    Computes information values for categorical variables. Notice that by using binning methods provided in 
+    dsds.transform, you can turn numerical values into categorical bins.
 
     Parameters
     ----------
     df
         Either a lazy or eager Polars Dataframe
     target
         The target column
@@ -642,15 +750,15 @@
     min_count
         A regularization term that prevents ln(0). This is the same as category_encoders package's 
         regularization parameter.
     check_binary
         Whether to check if target is binary or not
     '''
     if isinstance(cols, list):
-        _ = type_checker(df, cols, "string", "woe_iv_cat")
+        _ = type_checker(df, cols, "string", "woe_iv")
         input_cols = cols
     else:
         input_cols = get_string_cols(df)
 
     if check_binary:
         if not check_binary_target(df, target):
             raise ValueError("Target is not binary or not properly encoded.")
@@ -675,15 +783,22 @@
     return pl.concat(results).collect()
 
 def _binary_model_init(
     model_str:BinaryModels
     , params: dict[str, Any]
 ) -> ClassifModel:
     '''
-    Creates the binary classification model given by the model_str and the params dict
+    Returns a classification model. If n_job parameter is not specified, it will default to -1.
+
+    Parameters
+    ----------
+    model_str
+        One of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        The parameters for the model specified
     '''
     if "n_jobs" not in params:
         params["n_jobs"] = -1
 
     if model_str in ("logistic", "lr"):
         from sklearn.linear_model import LogisticRegression
         model = LogisticRegression(**params)
@@ -701,19 +816,38 @@
     
     return model
 
 def _fc_fi(
     model_str:str
     , params:dict[str, Any]
     , target:str
-    , features: Tuple | list
+    , features: Union[Tuple,list[str]]
     , train: pl.DataFrame
     , test: pl.DataFrame
 )-> Tuple[Tuple[Tuple, float, float], np.ndarray]:
-    
+    '''
+    Creates a classification model, evaluations model with log loss and roc_auc for each feature combination
+    (fc) and feature importance (fi). It will return a tuple of the following structure: 
+    ( (feature combination, log loss, roc_auc), feature_importance array) 
+
+    Parameters
+    ----------
+    model_str
+        One of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        The parameters for the model specified
+    target
+        The target column
+    features
+        Either a tuple or a list which represents the current feature combination
+    train
+        The training dataset. Must be eager
+    test
+        The testing dataset on which log loss and roc_auc will be evaluation. Must be eager
+    '''
     estimator = _binary_model_init(model_str, params)
     _ = estimator.fit(train.select(features), train[target])
     y_pred = estimator.predict_proba(test.select(features))[:,1]
     y_test = test[target].to_numpy()
     fc_rec = (
         features,
         logloss(y_test, y_pred, check_binary=False),
@@ -748,14 +882,16 @@
 
     This method will be extremely slow if (n choose n_comb) is a big number. All numerical columns 
     will be taken as potential features. Please encode the string columns if you want to use them
     as features here.
 
     If n_jobs is not provided in params, it will be defaulted to -1.
 
+    This will return a feature combination (fc) summary and a feature importance (fi) summary. 
+
     Parameters
     ----------
     df
         An eager Polars DataFrame
     target
         The target column
     model_str
@@ -806,32 +942,45 @@
     return fc.filter(
         (pl.col("logloss") <= logloss_threshold)
         & (pl.col("roc_auc") >= roc_auc_threshold)
     ).get_column("combination").explode().unique().to_list()
 
 def _permute_importance(
     model:ClassifModel
-    , df:pl.DataFrame
+    , X:pl.DataFrame
     , y: np.ndarray
-    , features: Tuple | list
-    , index: int
+    , index:int
     , k: int
 ) -> Tuple[float, int]:
+    '''
+    Computes permutation importance for a single feature.
+
+    Parameters
+    ----------
+    model
+        A trained classification model
+    X
+        An eager dataframe on which we shuffle the column at the given index and train the model
+    y
+        The target column turned into np.ndarray
+    index
+        The index of the column in X to shuffle
+    k
+        The number of times to repeat the shuffling
+    '''
     test_score = 0.
+    c = X.columns[index] # column to shuffle
     for _ in range(k):
-        shuffled_df = df.with_columns(
-            pl.col(features[index]).shuffle(seed=42)
+        shuffled_df = X.with_columns(
+            pl.col(c).shuffle(seed=42)
         )
-        pred = model.predict_proba(shuffled_df[features])[:, -1]
-        test_score += roc_auc(y, pred)
+        test_score += roc_auc(y, model.predict_proba(shuffled_df)[:, -1])
 
     return test_score, index
 
-# Can extend this for n_comb as well, as 
-
 def permutation_importance(
     df:pl.DataFrame
     , target:str
     , model_str:BinaryModels
     , params:dict[str, Any]
     , k:int = 5
 ) -> pl.DataFrame:
@@ -852,30 +1001,29 @@
     params
         Parameters for the model
     k
         Permute the same feature k times
     '''
     features = df.columns
     features.remove(target)
-    
+    _ = type_checker(df, features, "numeric", "permutation_importance")
     estimator = _binary_model_init(model_str, params)
     estimator.fit(df[features], df[target])
+    X = df[features]
     y = df[target].to_numpy()
-    pred = estimator.predict_proba(df[features])[:, -1]
-    score = roc_auc(y, pred)
+    score = roc_auc(y, estimator.predict_proba(X)[:, -1])
     pbar = tqdm(total=len(features), desc="Analyzing Features")
     imp = np.zeros(shape=len(features))
-    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
+    with ThreadPoolExecutor(max_workers=CPU_M1) as ex:
         futures = (
             ex.submit(
                 _permute_importance,
                 estimator,
-                df,
+                X,
                 y,
-                features, 
                 j,
                 k
             )
             for j in range(len(features))
         )
         for f in as_completed(futures):
             test_score, i = f.result()
```

### Comparing `dsds-0.0.21/src/dsds/metrics.py` & `dsds-0.0.23/src/dsds/metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np 
 import polars as pl
-from typing import Tuple, Optional
 import logging
+from typing import Tuple, Optional, Union
 
 logger = logging.getLogger(__name__)
 
 # No need to do length checking (len(y_1) == len(y_2)) because NumPy / Polars will complain for us.
 # Everything here is essentially fun stuff.
 # Ideally speaking, you should never convert things to dataframes when you compute these metrics.
 # But using only NumPy means we loss parallelism, and using Python concurrent module will not help
@@ -96,32 +96,31 @@
     return float(-np.trapz(tpr, fpr))
 
 def logloss(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , sample_weights:Optional[np.ndarray]=None
     , min_prob:float = 1e-12
-    , check_binary:bool = True
+    , check_binary:bool = False
 ) -> float:
     '''
-    Return the logloss of the binary classification.
+    Return the logloss of the binary classification. This only works for binary target.
 
     Parameters
     ----------
     y_actual
         Actual binary labels
     y_predicted
         Predicted probabilities
     sample_weights
         An array of size (n_sample, ) which provides weights to each sample
     min_prob
         Minimum probability to clip so that we can prevent illegal computations like 
         log(0). If p < min_prob, log(min_prob) will be computed instead.
     '''
-
     # Takes about 1/3 time of sklearn's log_loss because we parallelized some computations
     y_a, y_p = _flatten_input(y_actual, y_predicted)
     if check_binary:
         uniques = np.unique(y_a)
         if uniques.size != 2:
             raise ValueError("Currently this only supports binary classification.")
         if not (0 in uniques and 1 in uniques):
@@ -129,29 +128,80 @@
 
     if sample_weights is None:
         return pl.from_records((y_a, y_p), schema=["y", "p"]).with_columns(
             l = pl.col("p").clip_min(min_prob).log(),
             o = (1- pl.col("p")).clip_min(min_prob).log(),
             ny = 1 - pl.col("y")
         ).select(
-            pl.lit(-1, dtype=pl.Float64) * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o")).mean()
-        ).row(0)[0]
+            pl.lit(-1, dtype=pl.Float64) 
+            * (pl.col("y").dot(pl.col("l")) + pl.col("ny").dot(pl.col("o"))) / len(y_a)
+        ).item(0,0)
     else:
         s = sample_weights.ravel()
         return pl.from_records((y_a, y_p, s), schema=["y", "p", "s"]).with_columns(
             l = pl.col("p").clip_min(min_prob).log(),
             o = (1- pl.col("p")).clip_min(min_prob).log(),
             ny = 1 - pl.col("y")
         ).select(
             pl.lit(-1, dtype=pl.Float64)
-            * pl.col("s") 
-            * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o")).mean()
-        ).row(0)[0]
+            * (pl.col("s") * (pl.col("y") * pl.col("l") + pl.col("ny") * pl.col("o"))).mean()
+        ).item(0,0)
+    
+def binary_psi(
+    new_score: Union[pl.Series, np.ndarray]
+    , old_score: Union[pl.Series, np.ndarray]
+    , n_bins: int = 10
+) -> pl.DataFrame:
+    '''
+    Computes the Population Stability Index of a binary model by binning the new score into n_bins using quantiles.
+
+    Parameters
+    ----------
+    new_score
+        Either a Polars Series or a NumPy array that contains the new probabilites
+    old_score
+        Either a Polars Series or a NumPy array that contains the old probabilites
+    n_bins
+        The number of bins used in the computation. By default it is 10, which means we are using deciles
+    '''
+    if isinstance(new_score, np.ndarray):
+        s1 = pl.Series(new_score)
+    else:
+        s1 = new_score
+    
+    if isinstance(old_score, np.ndarray):
+        s2 = pl.Series(old_score)
+    else:
+        s2 = old_score
+
+    qcuts = np.arange(start=1/n_bins, stop=1.0, step = 1/n_bins)
+    s1_cuts:pl.DataFrame = s1.qcut(quantiles=qcuts, series=False)
+    s1_summary = s1_cuts.lazy().groupby(pl.col("category").cast(pl.Utf8)).agg(
+        a = pl.count()
+    )
+
+    s2_base:pl.DataFrame = s2.cut(bins = s1_cuts.get_column("break_point").unique().sort().head(len(qcuts)), 
+                                  series = False)
+
+    s2_summary:pl.DataFrame = s2_base.lazy().groupby(
+        pl.col("category").cast(pl.Utf8)
+    ).agg(
+        b = pl.count()
+    )
+    return s1_summary.join(s2_summary, on="category").with_columns(
+        a = pl.max(pl.col("a"), 0.00001)/len(s1),
+        b = pl.max(pl.col("b"), 0.00001)/len(s2)
+    ).with_columns(
+        a_minus_b = pl.col("a") - pl.col("b"),
+        ln_a_on_b = (pl.col("a")/pl.col("b")).log()
+    ).with_columns(
+        psi = pl.col("a_minus_b") * pl.col("ln_a_on_b")
+    ).sort("category").rename({"category":"score_range"}).collect()
 
-def l2_loss(
+def mse(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , sample_weights:Optional[np.ndarray]=None
 ) -> float:
     '''
     Computes average L2 loss of some regression model
 
@@ -166,17 +216,18 @@
     '''
     diff = y_actual - y_predicted
     if sample_weights is None:
         return np.mean(diff.dot(diff))
     else:
         return (sample_weights/(len(diff))).dot(diff.dot(diff))
     
-mse = l2_loss
+l2_loss = mse
+brier_loss = mse
 
-def l1_loss(
+def mae(
     y_actual:np.ndarray
     , y_predicted:np.ndarray
     , sample_weights:Optional[np.ndarray]=None
 ) -> float:
     '''
     Computes average L1 loss of some regression model
 
@@ -191,15 +242,15 @@
     '''
     diff = np.abs(y_actual - y_predicted)
     if sample_weights is None:
         return np.mean(diff)
     else:
         return (sample_weights/(len(diff))).dot(diff)
 
-mae = l1_loss 
+l1_loss = mae
 
 def r2(y_actual:np.ndarray, y_predicted:np.ndarray) -> float:
     '''
     Computes R square metric for some regression model
 
     Parameters
     ----------
```

### Comparing `dsds-0.0.21/src/dsds/prescreen.py` & `dsds-0.0.23/src/dsds/prescreen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from .type_alias import (
     PolarsFrame
-    , KSAlternatives
-    , CommonContinuousDist
+    , Alternatives
+    , CommonContiDist
     , SimpleDtypes
     , CPU_COUNT
     , POLARS_DATETIME_TYPES
     , POLARS_NUMERICAL_TYPES
 )
 from .sample import (
     lazy_sample
 )
 from .blueprint import(
-    Blueprint
+    Blueprint  # noqa: F401
 )
-import re
-import polars.selectors as cs
-import polars as pl
-import logging  
 from datetime import datetime 
-from typing import Any, Optional, Tuple
+from typing import Any, Optional, Tuple, Union
 from itertools import combinations
 from scipy.stats import (
     ks_2samp
     , kstest
 )
 from concurrent.futures import as_completed, ThreadPoolExecutor
 from tqdm import tqdm
 from math import comb
+import re
+import polars.selectors as cs
+import polars as pl
+import logging  
 
 logger = logging.getLogger(__name__)
 
 #----------------------------------------------------------------------------------------------#
 # Generic columns checks | Only works with Polars because Pandas's data types suck!            #
 #----------------------------------------------------------------------------------------------#
 
@@ -54,66 +54,70 @@
     '''Returns only datetime columns. This will not try to infer date from strings.'''
     return df.select(cs.datetime()).columns
 
 def get_bool_cols(df:PolarsFrame) -> list[str]:
     '''Returns boolean columns.'''
     return df.select(cs.by_dtype(pl.Boolean)).columns
 
-def get_cols_regex(df:PolarsFrame, pattern:str) -> list[str]:
-    '''Returns columns that have names matching the regex pattern.'''
-    return df.select(cs.matches(pattern=pattern)).columns
-
-def lowercase(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+def get_cols_regex(df:PolarsFrame, pattern:str, lowercase:bool=False) -> list[str]:
     '''
-    Lowercases all column names.
-
-    Set persist = True if this needs to be remembered by the blueprint.
+    Returns columns that have names matching the regex pattern.
+    
+    
     '''
-    output = df.rename({c: c.lower() for c in df.columns})
-    if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.add_func(df, lowercase, kwargs = {})
-    return output
+    if lowercase:
+        return (
+            df.rename({c:c.lower() for c in df.columns})
+            .select(cs.matches(pattern=pattern)).columns
+        )
+    else:
+        return df.select(cs.matches(pattern=pattern)).columns
+
 
 def rename(df:PolarsFrame, rename_dict:dict[str, str], persist:bool=False) -> PolarsFrame:
     '''
     A wrapper function for df.rename() so that it works with pipeline.
 
     Set persist = True if this needs to be remembered by the blueprint.
     '''
     output = df.rename(rename_dict)
     if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.add_func(df, rename, kwargs = {"rename_dict", rename_dict})
+        return output.blueprint.add_func(df, rename, kwargs = {"rename_dict": rename_dict})
     return output
 
+def lowercase(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+    '''
+    Lowercases all column names.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    return rename(df, {c: c.lower() for c in df.columns}, persist)
+
 def snake_case(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
     '''
     Turn all camel case column names into snake case.
 
     Set persist = True if this needs to be remembered by the blueprint.
     '''
     pat = re.compile(r"(?<!^)(?=[A-Z])")
     return rename(df, {c: pat.sub('_', c).lower() for c in df.columns}, persist)
 
 def select(
     df:PolarsFrame
-    , selector: list[str] | cs._selector_proxy_
+    , selector: Union[list[str], cs._selector_proxy_]
     , persist:bool=False
 ) -> PolarsFrame:
     '''
-    A select wrapper that makes it pipeline compatible
+    A select wrapper that makes it pipeline compatible.
 
     Set persist = True if this needs to be remembered by the blueprint.
     '''
-    if cs.is_selector(selector):
-        if isinstance(df, pl.LazyFrame) and persist:
-            return df.blueprint.select(selector)
-        else:
-            return df.select(selector)
-    else:
-        raise TypeError("The selector is not a valid selector.")
+    if isinstance(df, pl.LazyFrame) and persist:
+        return df.blueprint.select(selector)
+    return df.select(selector)
 
 def drop_nulls(
     df:PolarsFrame
     , subset:Optional[list[str]] = None
     , persist:bool=False
 ) -> PolarsFrame:
     '''
@@ -122,106 +126,146 @@
     Set persist = True if this needs to be remembered by the blueprint.
     '''
     if subset is None:
         by = df.columns
     else:
         by = subset
 
-    if isinstance(df, pl.LazyFrame):
-        cond = pl.lit(True)
-        for c in by:
-            cond = cond & pl.col(c).is_not_null()
-        
-        if persist:
-            return df.blueprint.filter(cond)
-        return df.filter(cond)
-    else:
-        return df.drop_nulls(subset=by)
+    output = df.drop_nulls(subset=by)
+    if isinstance(df, pl.LazyFrame) and persist:
+        return output.blueprint.add_func(df, drop_nulls, {"subset":subset})
+    return output
 
 def filter(
     df:PolarsFrame
     , condition: pl.Expr
     , persist: bool = False
 ) -> PolarsFrame:
     ''' 
     A wrapper function for Polars' filter so that it can be used in pipeline.
 
     Set persist = True if this needs to be remembered by the blueprint.
     '''
-    if isinstance(df, pl.LazyFrame):
-        if persist:
-            return df.blueprint.filter(condition)
+    if isinstance(df, pl.LazyFrame) and persist:
+        return df.blueprint.filter(condition)
     return df.filter(condition)
 
+def order_by(
+    df: PolarsFrame
+    , by: Union[str, list[str]]
+    , descending:bool = False
+    , nulls_last:bool = False
+    , persist: bool = False
+) -> PolarsFrame:
+    ''' 
+    A wrapper function for Polars' sort so that it can be used in pipeline.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    output = df.sort(by=by, descending=descending, nulls_last=nulls_last)
+    if isinstance(df, pl.LazyFrame) and persist:
+        return output.blueprint.add_func(df, order_by, {"by":by,"descending":descending, "nulls_last":nulls_last})
+    return output
+
 def check_binary_target(df:PolarsFrame, target:str) -> bool:
     '''Checks if target is binary or not. Only binary targets with 0s and 1s will pass.'''
     target_uniques = df.lazy().select(pl.col(target).unique()).collect().get_column(target)
     if len(target_uniques) != 2:
         logger.error("Target is not binary.")
         return False
     elif not (0 in target_uniques and 1 in target_uniques):
         logger.error("The binary target is not encoded as 0s and 1s.")
         return False
     return True
     
-def check_target_cardinality(df:PolarsFrame, target:str) -> pl.DataFrame:
-    '''Returns a dataframe showing the cardinality of different target values.'''
-    return df.lazy().groupby(target).count().sort(target).collect()
+def check_target_cardinality(df:PolarsFrame, target:str, raise_null:bool=True) -> pl.DataFrame:
+    '''
+    Returns a dataframe showing the cardinality of different target values. If raise_null = True, raise 
+    an exception if target column has any null values.
+    '''
+    output = df.lazy().groupby(target).count().sort(target).with_columns(
+        pct = pl.col("count")/pl.col("count").sum()
+    ).collect()
+    if raise_null and output.get_column(target).null_count() > 0:
+        raise ValueError("Target contains null.")
+    return output
 
 def check_columns_types(df:PolarsFrame, cols:Optional[list[str]]=None) -> str:
-    '''Returns the unique types of given columns in a single string. If multiple types are present
-    they are joined by a |. If cols is not given, automatically uses all columns.'''
+    '''
+    Returns the unique types of given columns in a single string. If multiple types are present
+    they are joined by a |. If cols is not given, automatically uses all columns.
+    '''
     if cols is None:
         check_cols:list[str] = df.columns
     else:
         check_cols:list[str] = cols 
 
-    types = set(dtype_mapping(t) for t in df.select(check_cols).dtypes)
-    return "|".join(types) if len(types) > 0 else "unknown"
+    types = sorted(set(dtype_mapping(t) for t in df.select(check_cols).dtypes))
+    return "|".join(types) if len(types) > 0 else "other/unknown"
 
 def type_checker(df:PolarsFrame, cols:list[str], expected_type:SimpleDtypes, caller_name:str) -> bool:
     types = check_columns_types(df, cols)
     if types != expected_type:
-        raise ValueError(f"The call `{caller_name}` can only be used on {expected_type} columns, not {types} types.")    
+        raise ValueError(f"The call `{caller_name}` can only be used on {expected_type} columns, not {types} types.")
     return True
 
 # dtype can be a "pl.datatype" or just some random data for which we want to infer a generic type.
 def dtype_mapping(d: Any) -> SimpleDtypes:
     if isinstance(d, str) or d == pl.Utf8:
         return "string"
     elif isinstance(d, bool) or d == pl.Boolean:
         return "bool"
     elif isinstance(d, (int,float)) or d in POLARS_NUMERICAL_TYPES:
         return "numeric"
+    elif isinstance(d, pl.List):
+        return "list" # Too many possibilities. Keep it to list for now.
     elif isinstance(d, datetime) or d in POLARS_DATETIME_TYPES:
         return "datetime"
     else:
         return "other/unknown"
 
 #----------------------------------------------------------------------------------------------#
 # Prescreen Inferral, Removal Methods                                                          #
 #----------------------------------------------------------------------------------------------#
 
 # Add a slim option that returns fewer stats? This is generic describe.
-# Separate str and numeric?
 def describe(
     df:PolarsFrame
-    , sample_frac:float = 0.75
+    , sample_frac:float = 1.0
+    , percentiles: list[float] = [0.25, 0.75]
+    , exclude: Optional[list[str]] = None
 ) -> pl.DataFrame:
     '''
-    Profile the data.
-
-    '''
+    A more detailed profile the data than Polars' default. This is an expensive function. Please sample 
+    and exclude some columns if runtime is important.
 
-    if isinstance(df, pl.LazyFrame):
-        df_local = lazy_sample(df, sample_frac=sample_frac)
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    sample_frac
+        If > 0 and < 1, will run profiling on a sample. This is recommended for bigger dataframes
+    percentiles
+        Percentile cuts that will be returned
+    exclude
+        List of columns to exclude
+    '''
+    selector = cs.all()
+    if exclude is not None:
+        selector = selector & ~cs.by_name(exclude)
+        
+    if sample_frac > 0 and sample_frac < 1:
+        if isinstance(df, pl.LazyFrame):
+            df_local = lazy_sample(df.select(selector), sample_frac=sample_frac).collect()
+        else:
+            df_local = df.select(selector).sample(fraction=sample_frac)
     else:
-        df_local = df
-    
-    temp = df_local.describe()
+        df_local = df.lazy().select(selector).collect()
+
+    temp = df_local.describe(percentiles)
     desc = temp.drop_in_place("describe")
     # Get unique
     unique_counts = get_unique_count(df_local).with_columns(
         unique_pct = pl.col("n_unique") / len(df_local)
     )
     # Skew and Kurtosis
     skew_and_kt_data = df_local.lazy().select(
@@ -231,40 +275,46 @@
 
     n_cols = len(df_local.columns)
     skew_and_kt = pl.from_records((df_local.columns, skew_and_kt_data[:n_cols], skew_and_kt_data[n_cols:])
                                   , schema=["column", "skew", "kurtosis"])
 
     # Get a basic string description of the data type.
     dtypes_dict = dict(zip(df_local.columns, map(dtype_mapping, df_local.dtypes)))
+    # Get all percentiles
+    pat = re.compile("^\d+%$")
+    pctls = [d for d in desc if pat.search(d)]
+    # Numerical stuff
+    nums = ["null_count", "mean", "std", "median"] + pctls
     # Combine all
-    nums = ("count", "null_count", "mean", "std", "median", "25%", "75%")
     final = temp.transpose(include_header=True, column_names=desc).with_columns(
         pl.col(c).cast(pl.Float64) for c in nums
     ).with_columns(
         null_pct = pl.col("null_count")/pl.col("count")
+        , non_null_count = pl.col("count") - pl.col("null_count")
         , CoV = pl.col("std") / pl.col("mean")
         , dtype = pl.col("column").map_dict(dtypes_dict)
     ).join(unique_counts, on="column").join(skew_and_kt, on="column")
-    
-    return final.select('column','count','null_count','null_pct','n_unique'
-                        , 'unique_pct','mean','std', 'CoV','min','max','25%'
-                        , 'median','75%', "skew", "kurtosis",'dtype')
+    # select only the stuff we need
+    return final.select('column', 'dtype', "non_null_count", 'null_count','null_pct','n_unique'
+                        , 'unique_pct','mean','std', 'CoV','min','max','median',"skew", "kurtosis"
+                        , *pctls)
 
 # Numeric only describe. Be more detailed.
 
 # String only describe. Be more detailed about interesting string stats.
 
-def describe_str(df:PolarsFrame
+def describe_str(
+    df:PolarsFrame
     , words_to_count:Optional[list[str]]=None
     , sample_frac:float = 0.75
 ) -> pl.DataFrame:
-    '''Gives some statistics about the string columns. Optionally you may pass a list
-    of strings to compute the total occurrances of each of the words in the string columns. If input is a LazyFrame, 
+    '''
+    Computes some statistics about the string columns. Optionally you may pass a list
+    of strings to compute the total occurrences of each of the words in the string columns. If input is a LazyFrame, 
     a sample of sample_pct will be used, and sample_pct will only be used in the lazy case. 
-
     '''
     strs = get_string_cols(df)
     df_str = df.select(strs)
     if isinstance(df, pl.LazyFrame):
         df_str = lazy_sample(df_str, sample_frac=sample_frac).collect()
 
     nstrs = len(strs)
@@ -303,21 +353,26 @@
             t = df_str.select(pl.all().str.count_match(w).sum().prefix("wc:")).row(0)
             output["total_"+ w + "_count"] = t
 
     return pl.from_dict(output)
 
 # -----------------------------------------------------------------------------------------------
 def drop(df:PolarsFrame, to_drop:list[str]) -> PolarsFrame:
+    '''
+    A pipeline compatible way to drop the given columns, which will be remembered by the blueprint
+    by default.
+    '''
     if isinstance(df, pl.LazyFrame):
         return df.blueprint.drop(to_drop)
     return df.drop(to_drop)
 
-def non_numeric_removal(df:PolarsFrame, include_bools:bool=True) -> PolarsFrame:
-    '''Removes all non-numeric columns. If include_bools = True, then keep boolean columns.'''
-    
+def non_numeric_removal(df:PolarsFrame, include_bools:bool=False) -> PolarsFrame:
+    '''
+    Removes all non-numeric columns. If include_bools = True, then keep boolean columns.
+    '''
     if include_bools:
         selector = ~(cs.numeric()|cs.by_dtype(pl.Boolean))
     else:
         selector = ~cs.numeric()
 
     non_nums = df.select(selector).columns
     logger.info(f"The following columns are dropped because they are not numeric: {non_nums}.\n"
@@ -342,40 +397,48 @@
     , threshold:float = 0.9
     , count_null:bool = True
 ) -> list[str]:
     '''
     Find all string columns whose elements reasonably match the given pattern. The match logic can 
     be tuned using the all the parameters.
 
-    Arguments:
-        sample_frac: the pct of the total dataframe to use as basis
-        sample_count: from the basis, how many rows to sample for each round 
-        sample_rounds: how many rounds of sampling we are doing
-        threhold: For each round, what is the match% that is needed to be a counted as a success. For instance, 
+    Parameters
+    ----------
+    sample_frac
+        The pct of the total dataframe to use as pool
+    sample_count
+        From the pool, how many rows to sample for each round 
+    sample_rounds
+        How many rounds of sampling we are doing
+    threshold
+        For each round, what is the match% that is needed to be a counted as a success. For instance, 
         in round 1, for column x, we have 92% match rate, and threshold = 0.9. We count column x as a match for 
         this round. In the end, the column must match for every round to be considered a real match.
-        count_null: for individual matches, do we want to count null as a match or not? If the column has high null pct,
+    count_null
+        For individual matches, do we want to count null as a match or not? If the column has high null pct,
         the non-null values might mostly match the pattern. In this case, using count_null = True will match the column, 
         while count_null = False will most likely exclude the column.
 
     Returns:
         a list of columns that pass the matching test
     
     '''
-    
     strs = get_string_cols(df)
     df_local = lazy_sample(df.lazy(), sample_frac=sample_frac).collect()    
     matches:set[str] = set(strs)
     sample_size = min(sample_count, len(df_local))
     for _ in range(sample_rounds):
         df_sample = df_local.sample(n = sample_size)
         fail = df_sample.select(
-            (pl.when(pl.col(s).is_null()).then(count_null).otherwise(
-                pl.col(s).str.contains(pattern)
-            ).sum()/sample_size).alias(s) for s in strs
+            (
+                pl.when(pl.col(s).is_null()).then(count_null).otherwise(
+                    pl.col(s).str.contains(pattern)
+                ).sum()/sample_size
+            ).alias(s) 
+            for s in strs
         ).transpose(include_header=True, column_names=["pattern_match_pct"])\
         .filter(pl.col("pattern_match_pct") < threshold).get_column("column")
         # If the match failes in this round, remove the column.
         matches.difference_update(fail)
 
     return list(matches)
 
@@ -480,23 +543,90 @@
     '''Removes all date columns from dataframe. This algorithm will try to infer if string column is date.'''
 
     remove_cols = date_inferral(df) 
     logger.info(f"The following columns are dropped because they are dates. {remove_cols}.\n"
                 f"Removed a total of {len(remove_cols)} columns.")
     return drop(df, remove_cols)
 
+def invalid_inferral(df:PolarsFrame, threshold:float=0.5, include_null:bool=False) -> list[str]:
+    '''
+    Infers numeric columns that have more than threshold pct of invalid (NaN) values.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    include_null
+        If true, then null values will also be counted as invalid.
+    '''
+    nums = get_numeric_cols(df)
+    df_local = df.lazy().select(nums).with_row_count(offset=1).set_sorted("row_nr")
+    if include_null:
+        expr = (pl.all().is_nan().sum() + pl.all().is_null().sum())/pl.col("row_nr").max()
+    else:
+        expr = pl.all().is_nan().sum()/pl.col("row_nr").max()
+    
+    return (
+        df_local.select(
+            expr
+        ).select(~cs.by_name(["row_nr"]))
+        .collect()
+        .transpose(include_header=True, column_names=["nan_pct"])
+        .filter(pl.col("nan_pct") >= threshold)
+        .get_column("column")
+        .to_list()
+    )
+
+def invalid_removal(df:PolarsFrame, threshold:float=0.5, include_null:bool=False) -> PolarsFrame:
+    '''
+    Removes numeric columns that have more than threshold pct of invalid (NaN) values.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    include_null
+        If true, then null values will also be counted as invalid.
+    '''
+    remove_cols = invalid_inferral(df, threshold, include_null) 
+    logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
+                f" not valid values. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
 def null_inferral(df:PolarsFrame, threshold:float=0.5) -> list[str]:
-    '''Infers columns that have more than threshold pct of null values. Threshold should be between 0 and 1.'''
+    '''
+    Infers columns that have more than threshold pct of null values.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    '''
     return (df.lazy().null_count().collect()/len(df)).transpose(include_header=True, column_names=["null_pct"])\
                     .filter(pl.col("null_pct") >= threshold)\
                     .get_column("column").to_list()
 
 def null_removal(df:PolarsFrame, threshold:float=0.5) -> PolarsFrame:
-    '''Removes columns with more than threshold pct of null values. Threshold should be between 0 and 1.'''
+    '''
+    Removes columns with more than threshold pct of null values.
 
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    '''
     remove_cols = null_inferral(df, threshold) 
     logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
                 f" null values. {remove_cols}.\n"
                 f"Removed a total of {len(remove_cols)} columns.")
     return drop(df, remove_cols)
 
 def var_inferral(df:PolarsFrame, threshold:float, target:str) -> list[str]:
@@ -515,233 +645,332 @@
                 f"Removed a total of {len(remove_cols)} columns.")
     return drop(df, remove_cols)
 
 # Really this is just an alias
 regex_inferral = get_cols_regex
 
 def regex_removal(df:PolarsFrame, pattern:str, lowercase:bool=False) -> PolarsFrame:
-    '''Remove columns if they satisfy some regex rules.'''
+    '''
+    Remove columns if their names satisfy the given regex rules. This is common when you want to remove columns 
+    with certain prefixes that may not be allowed to use in models.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    pattern
+        The regex pattern
+    lowercase
+        Whether to lowercase everything and then match
+    '''
     remove_cols = get_cols_regex(df, pattern, lowercase)
     logger.info(f"The following columns are dropped because their names satisfy the regex rule: {pattern}."
                 f" {remove_cols}.\n"
                 f"Removed a total of {len(remove_cols)} columns.")
     
     return drop(df, remove_cols)
 
-def get_unique_count(df:PolarsFrame) -> pl.DataFrame:
-    '''Gets unique counts for columns.'''
-    return df.lazy().select(
-        pl.col(x).n_unique() for x in df.columns
-    ).collect().transpose(include_header=True, column_names=["n_unique"])
+def get_unique_count(df:PolarsFrame, include_null_count:bool=False) -> pl.DataFrame:
+    '''
+    Gets unique counts for columns and returns a dataframe with schema = ["column", "n_unique"]. Null count
+    is useful in knowing if null is one of the unique values and thus is included as an option. Note that
+    null != NaN.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    include_null_count
+        If true, this will return a dataframe with schema = ["column", "n_unique", "null_count"]
+    '''
+    if include_null_count:
+        temp = df.lazy().select(
+            pl.all().n_unique().suffix("_n_unique"),
+            pl.all().null_count().suffix("_null_count")
+        ).collect().row(0)
+        n = len(df.columns)
+        return pl.from_records((df.columns, temp[:n], temp[n:]), schema=["column", "n_unique", "null_count"])
+    else:
+        return df.lazy().select(
+            pl.all().n_unique()
+        ).collect().transpose(include_header=True, column_names=["n_unique"])
 
 # Really this is just an alias
 def unique_inferral(df:PolarsFrame, threshold:float=0.9) -> list[str]:
-    '''Infers columns that have higher than threshold pct of unique values.'''
-    return get_unique_count(df).with_columns(
-        (pl.col("n_unique")/len(df)).alias("unique_pct")
-    ).filter(pl.col("unique_pct") >= threshold)\
-    .get_column("column").to_list()
+    '''
+    Infers columns that have higher than threshold unique pct.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Every column with unique pct higher than this threshold will be returned. Note that 
+        threshold will be clipped between 0.01 and 0.99.
+    '''
+    clipped_threshold = min(0.99, max(threshold, 0.01))
+    temp = get_unique_count(df.with_row_count(offset=1))
+    len_df:int = temp.filter(pl.col("column") == "row_nr").item(0,1)
+    return (
+        temp.with_columns(
+            (pl.col("n_unique")/len_df).alias("unique_pct")
+        ).filter((pl.col("unique_pct") >= clipped_threshold) & (pl.col("column") != "row_nr"))\
+        .get_column("column")
+        .to_list()
+    )
 
 def unique_removal(df:PolarsFrame, threshold:float=0.9) -> PolarsFrame:
-    '''Remove columns that have higher than threshold pct of unique values.'''
+    '''
+    Remove columns that have higher than threshold pct of unique values. Usually this is done to filter
+    out id-like columns
 
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    threshold
+        The threshold for unique pct. Columns with higher than this threshold unique pct will be removed 
+    '''
     remove_cols = unique_inferral(df, threshold)
     logger.info(f"The following columns are dropped because more than {threshold*100:.2f}% of unique values."
                 f" {remove_cols}.\n"
                 f"Removed a total of {len(remove_cols)} columns.")
     return drop(df, remove_cols)
 
-# Is this a good definition?
+# Once there is a config, add a discrete criterion config
 def discrete_inferral(df:PolarsFrame
     , threshold:float=0.1
     , max_n_unique:int=100
     , exclude:Optional[list[str]]=None
 ) -> list[str]:
     '''
-        A column that satisfies either n_unique < max_n_unique or unique_pct < threshold 
-        will be considered discrete.
+    A column that satisfies either n_unique < max_n_unique or unique_pct < threshold 
+    will be considered discrete. E.g. threshold = 0.1 and max_n_unique = 100 means if a 
+    column has < 100 unique values, or the unique pct is < 10%, then it will be considered
+    as discrete.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    threshold
+        The threshold for unique pct
+    max_n_unique
+        The maximum number of unique values allowed for a column to be considered discrete
+    exclude
+        List of columns to exclude
     '''
     exclude_list = [] if exclude is None else exclude
-    return get_unique_count(df).filter(
-        ((pl.col("n_unique") < max_n_unique) | (pl.col("n_unique")/len(df) < threshold)) 
+    exclude_list.append("row_nr")
+    temp = get_unique_count(df.with_row_count(offset=1).set_sorted("row_nr"))
+    len_df = temp.filter(pl.col("column") == "row_nr").item(0,1)
+    return temp.filter(
+        ((pl.col("n_unique") < max_n_unique) | (pl.col("n_unique")/len_df < threshold)) 
         & (~pl.col("column").is_in(exclude_list)) # is not in
     ).get_column("column").to_list()
 
 def conti_inferral(
     df:PolarsFrame
     , discrete_threshold:float = 0.1
     , discrete_max_n_unique:int = 100
     , exclude:Optional[list[str]]=None
 ) -> list[str]:
+    '''
+    Returns everything that is not considered discrete.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    discrete_threshold
+        The threshold for unique pct in discrete inferral
+    discrete_max_n_unique
+        The maximum number of unique values allowed for a column to be considered discrete
+    exclude
+        List of columns to exclude
+    '''
     exclude_list = [] if exclude is None else exclude
     discrete = discrete_inferral(df, discrete_threshold, discrete_max_n_unique)
     return df.select(cs.numeric() & ~cs.by_name(exclude_list) & ~cs.by_name(discrete)).columns
 
 def constant_inferral(df:PolarsFrame, include_null:bool=True) -> list[str]:
-    temp = get_unique_count(df).filter(pl.col("n_unique") <= 2)
-    remove_cols = temp.filter(pl.col("n_unique") == 1).get_column("column").to_list() 
-    if include_null: # This step is kind of inefficient right now.
-        binary = temp.filter(pl.col("n_unique") == 2).get_column("column")
-        nc = df.lazy().select(binary).null_count().collect().row(0)
-        remove_cols.extend(
-            binary[i] for i in range(len(nc)) if nc[i] > 0
-        )
-
-    return remove_cols
+    '''
+    Returns a list of inferred constant columns.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    include_null
+        If true, then columns with two distinct values like [value_1, null] will be considered a 
+        constant column
+    '''
+    if include_null:
+        return get_unique_count(df, include_null_count=True).filter(
+            ((pl.col("n_unique") == 1) | ((pl.col("n_unique") == 2) & (pl.col("null_count") > 0)))
+        ).get_column("column").to_list()
+    else:
+        return get_unique_count(df).filter(pl.col("n_unique") == 1).get_column("column").to_list()
 
 def constant_removal(df:PolarsFrame, include_null:bool=True) -> PolarsFrame:
-    '''Removes all constant columns from dataframe.
+    '''
+    Removes all constant columns from dataframe.
     
-        Arguments:
-            df:
-            include_null: if true, then columns with two distinct values like [value_1, null] will be considered a 
-                constant column.
-
-        Returns: 
-            the df without constant columns
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    include_null
+        If true, then columns with two distinct values like [value_1, null] will be considered a 
+        constant column
     '''
     remove_cols = constant_inferral(df, include_null)
     logger.info(f"The following columns are dropped because they are constants. {remove_cols}.\n"
                 f"Removed a total of {len(remove_cols)} columns.")
     return drop(df, remove_cols)
 
 def remove_if_exists(df:PolarsFrame, cols:list[str]) -> PolarsFrame:
     '''Removes the given columns if they exist in the dataframe.'''
-    remove_cols = list(set(cols).intersection(set(df.columns)))
+    remove_cols = list(set(cols).intersection(df.columns))
     logger.info(f"The following columns are dropped. {remove_cols}.\nRemoved a total of {len(remove_cols)} columns.")
     return drop(df, remove_cols)
 
 #----------------------------------------------------------------------------------------------#
-# More advanced Methods
+# More statistical Methods
 #----------------------------------------------------------------------------------------------#
 
 def _ks_compare(
     df:pl.DataFrame
     , pair:Tuple[str, str]
-    , alt:KSAlternatives="two-sided"
+    , alt:Alternatives="two-sided"
 ) -> Tuple[Tuple[str, str], float, float]:
-    
     res = ks_2samp(df.get_column(pair[0]), df.get_column(pair[1]), alt)
     return (pair, res.statistic, res.pvalue)
 
 def ks_compare(
     df:PolarsFrame
     , target:Optional[str] = None
     , smaple_frac:float = 0.75
     , test_cols:Optional[list[str]] = None
-    , alt: KSAlternatives = "two-sided"
+    , alt: Alternatives = "two-sided"
     , skip:int = 0
     , max_comp:int = 1000
 ) -> pl.DataFrame:
-    '''Run ks-stats on all non-discrete columns in the dataframe. If test_cols is None, it will infer non-discrete 
+    '''
+    Run ks-stats on all non-discrete columns in the dataframe. If test_cols is None, it will infer non-discrete 
     continuous columns. See docstring of discrete_inferral to see what is considered discrete. Provide the target 
     so that it will not be included in the comparisons. Since ks 2 sample comparison is relatively expensive, we will
     always sample 75% of the dataset, unless the user specifies a different sample_frac.
 
-    Note: this will only run on all 2 combinations of columns, starting from skip and end at 
-    skip + max_comp.
+    Note: this will only run on all 2 combinations of columns, starting from skip and end at skip + max_comp.
 
     Note: The null hypothesis is that the two columns come from the same distribution. Therefore a small p-value means
     that they do not come from the same distribution. Having p-value > threshold does not mean they have the same 
     distribution automatically, and it requires more examination to reach the conclusion.
     '''
     if test_cols is None:
         nums = [f for f in get_numeric_cols(df) if f not in discrete_inferral(df)]
     else:
         nums = test_cols
 
     if target in nums:
         nums.remove(target)
-    sorted(nums)
+
+    nums.sort()
     if isinstance(df, pl.LazyFrame):
         df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
     else:
         df_test = df.select(nums).sample(fraction=smaple_frac)
 
     n_c2 = comb(len(nums), 2)
-    last_index = min(skip + max_comp, n_c2)
+    last = min(skip + max_comp, n_c2)
     results = []
-    to_test = enumerate(combinations(nums, 2), start=skip)
+    to_test = enumerate(combinations(nums, 2))
     pbar = tqdm(total=min(max_comp, n_c2 - skip), desc="Comparisons")
     with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
-        for f in as_completed(ex.submit(_ks_compare, df_test, p, alt) for i, p in to_test if i < last_index):
+        for f in as_completed(ex.submit(_ks_compare, df_test, pair, alt) 
+                              for i, pair in to_test if i < last and i > skip):
             results.append(f.result())
             pbar.update(1)
 
     pbar.close()
     return pl.from_records(results, schema=["combination", "ks-stats", "p-value"])
 
-def _dist_inferral(df:pl.DataFrame, c:str, dist:CommonContinuousDist) -> Tuple[str, float, float]:
+def _dist_inferral(df:pl.DataFrame, c:str, dist:CommonContiDist) -> Tuple[str, float, float]:
     res = kstest(df[c], dist)
     return (c, res.statistic, res.pvalue)
 
 def dist_test(
     df: PolarsFrame
-    , which_dist:CommonContinuousDist
+    , which_dist:CommonContiDist
     , smaple_frac:float = 0.75
     , target: Optional[str] = None
 ) -> pl.DataFrame:
-    '''Tests if the numeric columns follow the given distribution by using the KS test. If
+    '''
+    Tests if the numeric columns follow the given distribution by using the KS test. If
     target is provided it will be excluded. The null hypothesis is that the columns follow the given distribution. 
     We sample 75% of data because ks test is relatively expensive.
     '''
-    
     nums = get_numeric_cols(df, exclude=[target])
     if isinstance(df, pl.LazyFrame):
         df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
     else:
         df_test = df.select(nums).sample(fraction=smaple_frac)
 
     results = []
     pbar = tqdm(total=len(nums), desc="Comparisons")
     with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
         for f in as_completed(ex.submit(_dist_inferral, df_test, c, which_dist) for c in nums):
             results.append(f.result())
             pbar.update(1)
 
     pbar.close()
-    return pl.from_records(results, schema=["feature", "ks-stats", "p-value"])
+    return pl.from_records(results, schema=["feature", "ks-stats", "p_value"])
 
 def suggest_normal(
     df:PolarsFrame
     , target: Optional[str] = None
     , threshold:float = 0.05
 ) -> list[str]:
-    '''Suggests which columns are normally distributed. This takes the columns for which the null hypothesis
+    '''
+    Suggests which columns are normally distributed. This takes the columns for which the null hypothesis
     cannot be rejected in the dist_test (KS test).
     '''
-    return dist_test(df, "norm", target=target).filter(pl.col("p-value") > threshold)\
+    return dist_test(df, "norm", target=target).filter(pl.col("p_value") > threshold)\
         .get_column("feature").to_list()
 
 def suggest_uniform(
     df:PolarsFrame
     , target: Optional[str] = None
     , threshold:float = 0.05
 ) -> list[str]:
-    '''Suggests which columns are uniformly distributed. This takes the columns for which the null hypothesis
+    '''
+    Suggests which columns are uniformly distributed. This takes the columns for which the null hypothesis
     cannot be rejected in the dist_test (KS test).
     '''
-    return dist_test(df, "uniform", target=target).filter(pl.col("p-value") > threshold)\
+    return dist_test(df, "uniform", target=target).filter(pl.col("p_value") > threshold)\
         .get_column("feature").to_list()
 
 def suggest_lognormal(
     df:PolarsFrame
     , target: Optional[str] = None
     , threshold:float = 0.05
 ) -> list[str]:
-    '''Suggests which columns are log-normally distributed. This takes the columns which the null hypothesis
+    '''
+    Suggests which columns are log-normally distributed. This takes the columns which the null hypothesis
     cannot be rejected in the dist_test (KS test).
     '''
-    return dist_test(df, "lognorm", target=target).filter(pl.col("p-value") > threshold)\
+    return dist_test(df, "lognorm", target=target).filter(pl.col("p_value") > threshold)\
         .get_column("feature").to_list()
 
 def suggest_dist(
     df:PolarsFrame
     , target: Optional[str] = None
     , threshold:float = 0.05
-    , dist: CommonContinuousDist = "norm"
+    , dist: CommonContiDist = "norm"
 ) -> list[str]:
-    '''Suggests which columns follow the given distribution. This returns the columns which the null hypothesis
+    '''
+    Suggests which columns follow the given distribution. This returns the columns which the null hypothesis
     cannot be rejected in the dist_test (KS test).
     '''
-    return dist_test(df, dist, target=target).filter(pl.col("p-value") > threshold)\
+    return dist_test(df, dist, target=target).filter(pl.col("p_value") > threshold)\
         .get_column("feature").to_list()
```

### Comparing `dsds-0.0.21/src/dsds/transform.py` & `dsds-0.0.23/src/dsds/encoders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,136 +1,32 @@
 from __future__ import annotations
 
 from .type_alias import (
     PolarsFrame
-    , ImputationStrategy
-    , ScalingStrategy
-    , PowerTransformStrategy
-    , DateExtract
-    , clean_strategy_str
-    , CPU_COUNT
 )
 from .prescreen import (
     get_bool_cols
     , get_string_cols
     , get_unique_count
     , check_binary_target
-    , check_columns_types
     , type_checker
 )
 from .blueprint import( # Need this for Polars extension to work
-    Blueprint
+    Blueprint  # noqa: F401
 )
+from typing import Optional, Union, Any
 import logging
-import math
 import numpy as np
 import polars as pl
-from typing import Optional, Tuple, Any
-from scipy.stats._morestats import (
-    yeojohnson_normmax
-    , boxcox_normmax
-)
-from concurrent.futures import as_completed, ThreadPoolExecutor
-from tqdm import tqdm
-
-# A lot of companies are still using Python < 3.10
-# So I am not using match statements
 
 logger = logging.getLogger(__name__)
 
-def impute(
-    df:PolarsFrame
-    , cols:list[str]
-    , strategy:ImputationStrategy = 'median'
-    , const:float = 1.
-) -> PolarsFrame:
+def boolean_encode(df:PolarsFrame, keep_null:bool=True) -> PolarsFrame:
     '''
-    Impute the given columns with the given strategy.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        The columns to impute
-    strategy
-        One of 'median', 'mean', 'const' or 'mode'. If 'const', the const argument should be provided. Note that
-        if strategy is mode and if two values occur the same number of times, a random one will be picked.
-    const
-        The constant value to impute by if strategy = 'const'    
-    '''
-    s = clean_strategy_str(strategy)
-    if s == "median":
-        all_medians = df.lazy().select(cols).median().collect().row(0)
-        exprs = (pl.col(c).fill_null(all_medians[i]) for i,c in enumerate(cols))
-    elif s in ("mean", "avg", "average"):
-        all_means = df.lazy().select(cols).mean().collect().row(0)
-        exprs = (pl.col(c).fill_null(all_means[i]) for i,c in enumerate(cols))
-    elif s in ("const", "constant"):
-        exprs = (pl.col(c).fill_null(const) for c in cols)
-    elif s in ("mode", "most_frequent"):
-        all_modes = df.lazy().select(cols).select(pl.all().mode().first()).collect().row(0)
-        exprs = (pl.col(c).fill_null(all_modes[i]) for i,c in enumerate(cols))
-    else:
-        raise TypeError(f"Unknown imputation strategy: {strategy}")
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def scale(
-    df:PolarsFrame
-    , cols:list[str]
-    , strategy:ScalingStrategy="standard"
-    , const:float = 1.0
-) -> PolarsFrame:
-    '''
-    Scale the given columns with the given strategy.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        The columns to scale
-    strategy
-        One of 'standard', 'min_max', 'const'. If 'const', the const argument should be provided
-    const
-        The constant value to scale by if strategy = 'const'    
-    '''
-    _ = type_checker(df, cols, "numeric", "scale")
-    s = clean_strategy_str(strategy)
-    if s == "standard":
-        mean_std = df.lazy().select(cols).select(
-            pl.all().mean().prefix("mean:")
-            , pl.all().std().prefix("std:")
-        ).collect().row(0)
-        exprs = ( (pl.col(c) - mean_std[i])/(mean_std[i + len(cols)]) for i,c in enumerate(cols) )
-    elif s == "min_max":
-        min_max = df.lazy().select(cols).select(
-            pl.all().min().prefix("min:"),
-            pl.all().max().prefix("max:")
-        ).collect().row(0) # All mins come first, then maxs
-        exprs = ( (pl.col(c) - min_max[i])/((min_max[i + len(cols)] - min_max[i])) for i,c in enumerate(cols) )
-    elif s in ("const", "constant"):
-        exprs = (pl.col(c)/const for c in cols)
-    else:
-        raise TypeError(f"Unknown scaling strategy: {strategy}")
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def boolean_transform(df:PolarsFrame, keep_null:bool=True) -> PolarsFrame:
-    '''
-    Converts all boolean columns into binary columns.
+    Converts all boolean columns into binary 0, 1 columns.
 
     This will be remembered by blueprint by default.
 
     Parameters
     ----------
     df
         Either a lazy or eager Polars DataFrame
@@ -173,106 +69,14 @@
     one = pl.lit(1, dtype=pl.UInt8)
     zero = pl.lit(0, dtype=pl.UInt8)
     exprs = (pl.when(pl.col(c).is_null()).then(one).otherwise(zero).suffix(suffix) for c in to_add)
     if isinstance(df, pl.LazyFrame):
         return df.blueprint.with_columns(list(exprs))
     return df.with_columns(exprs)
 
-def merge_infreq_values(
-    df: PolarsFrame
-    , cols: list[str]
-    , min_count: int | None = 10
-    , min_frac: float | None = None
-    , separator: str = '|'
-) -> PolarsFrame:
-    '''
-    Combines infrequent categories in string columns together.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        List of string columns to perform this operation
-    min_count
-        Define a category to be infrequent if it occurs less than min_count. This defaults to 10 if both min_count and 
-        min_frac are None.
-    min_frac
-        Define category to be infrequent if it occurs less than this percentage of times. If both min_count and min_frac
-        are set, min_frac takes priority
-    separator
-        The separator for the new value representing the combined categories
-
-    Example
-    -------
-    >>> import dsds.transform as t
-    ... df = pl.DataFrame({
-    ...     "a":["a", "b", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c"],
-    ...     "b":["a", "b", "c", "d", "d", "d", "d", "d", "d", "d", "d", "d", "d", "d"]
-    ... })
-    >>> df
-    shape: (14, 2)
-    ┌─────┬─────┐
-    │ a   ┆ b   │
-    │ --- ┆ --- │
-    │ str ┆ str │
-    ╞═════╪═════╡
-    │ a   ┆ a   │
-    │ b   ┆ b   │
-    │ c   ┆ c   │
-    │ c   ┆ d   │
-    │ …   ┆ …   │
-    │ c   ┆ d   │
-    │ c   ┆ d   │
-    │ c   ┆ d   │
-    │ c   ┆ d   │
-    └─────┴─────┘
-    >>> t.merge_infreq_values(df, ["a", "b"], min_count=3)
-    shape: (14, 2)
-    ┌─────┬───────┐
-    │ a   ┆ b     │
-    │ --- ┆ ---   │
-    │ str ┆ str   │
-    ╞═════╪═══════╡
-    │ a|b ┆ a|c|b │
-    │ a|b ┆ a|c|b │
-    │ c   ┆ a|c|b │
-    │ c   ┆ d     │
-    │ …   ┆ …     │
-    │ c   ┆ d     │
-    │ c   ┆ d     │
-    │ c   ┆ d     │
-    │ c   ┆ d     │
-    └─────┴───────┘
-    '''
-    _ = type_checker(df, cols, "string", "merge_infreq_values")
-    if min_frac is None:
-        if min_count is None:
-            comp = pl.col("count") < 10
-        else:
-            comp = pl.col("count") < min_count
-    else:
-        comp = pl.col("count")/pl.col("count").sum() < min_frac
-
-    exprs = []
-    for c in cols:
-        infreq = df.lazy().groupby(c).count().filter(
-            comp
-        ).collect().get_column(c)
-        value = separator.join(infreq)
-        exprs.append(
-            pl.when(pl.col(c).is_in(infreq)).then(value).otherwise(pl.col(c)).alias(c)
-        )
-    
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
 def one_hot_encode(
     df:PolarsFrame
     , cols:Optional[list[str]]=None
     , separator:str="_"
     , drop_first:bool=False
 ) -> PolarsFrame:
     '''
@@ -289,15 +93,14 @@
     separator
         The separator used in the names of the new columns
     drop_first
         If true, the first category in the each column will be dropped. E.g. if column "D" has 3 distinct values, 
         say 'A', 'B', 'C', then only two binary indicators 'D_B' and 'D_C' will be created. This is useful for
         reducing dimensions and also good for optimization methods that require data to be non-degenerate.
     '''
-    
     if isinstance(cols, list):
         _ = type_checker(df, cols, "string", "one_hot_encode")
         str_cols = cols
     else:
         str_cols = get_string_cols(df)
 
     if isinstance(df, pl.LazyFrame):
@@ -340,57 +143,79 @@
     df
         Either a lazy or eager Polars DataFrame
     cols
         If not provided, will use all string columns
     separator
         The separator used in the names of the new columns
     '''
-
     if cols is None:
         str_cols = get_string_cols(df)
         exclude = [] if exclude is None else exclude
         binary_list = get_unique_count(df)\
             .filter( # Binary + Not Exclude + Only String
                 (pl.col("n_unique") == 2) & (~pl.col("column").is_in(exclude)) & (pl.col("column").is_in(str_cols))
             ).get_column("column").to_list()
     else:
         binary_list = cols
     
     return one_hot_encode(df, cols=binary_list, drop_first=True, separator=separator)
 
+def force_binary(df:PolarsFrame) -> PolarsFrame:
+    '''
+    Force every binary column, no matter what data type, to be turned into 0s and 1s according to the order of the 
+    elements. If a column has two unique values like [null, "haha"], then null will be mapped to 0 and "haha" to 1.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    '''
+    binary_list = get_unique_count(df).filter(pl.col("n_unique") == 2).get_column("column")
+    temp = df.lazy().select(binary_list).groupby(1).agg(
+            pl.all().unique().sort()
+        ).select(binary_list)
+    exprs:list[pl.Expr] = []
+    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+    for t in temp.collect().get_columns():
+        u:pl.List = t[0] # t is a Series which contains a single list which contains the 2 unique values 
+        exprs.append(
+            pl.when(pl.col(t.name) == u[0]).then(zero).otherwise(one).alias(t.name)
+        )
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
 def multicat_one_hot_encode(
     df:PolarsFrame
     , cols: list[str]
     , delimiter: str
     , drop_first: bool = False
 ) -> PolarsFrame:
     '''
     Expands multicategorical columns into several one-hot-encoded columns respectively. A multicategorical column is a 
-    column with strings like `aaa|bbb|ccc`, where it means this row belongs to categories aaa, bbb, and ccc. Typically, 
+    column with strings like `aaa|bbb|ccc`, which means this row belongs to categories aaa, bbb, and ccc. Typically, 
     such a column will contain strings separated by a delimiter. This method will collect all unique strings separated 
     by the delimiter and one hot encode the corresponding column.
 
     This will be remembered by blueprint by default.
 
     Parameters
     ----------
     df
         Either a lazy or eager Polars DataFrame
     cols
         If not provided, will use all string columns
     separator
         The separator used in the names of the new columns
     drop_first
-        If true, the first category in the each column will be dropped. E.g. if column "D" has 3 distinct values, 
-        say 'A', 'B', 'C', then only two binary indicators 'D_B' and 'D_C' will be created. This is useful for
-        reducing dimensions and also good for optimization methods that require data to be non-degenerate.
-
-    Returns
-    -------
-        A lazy/eager dataframe with multicategorical columns one-hot-encoded
+        If true, the first category in the each column will be dropped.
 
     Example
     -------
     >>> df = pl.DataFrame({
     ... "text1":["abc|ggg", "abc|sss", "ccc|abc"],
     ... "text2":["aaa|bbb", "ccc|aaa", "bbb|ccc"]
     ... })
@@ -416,16 +241,16 @@
     │ 1         ┆ 0         ┆ 0         ┆ 1         ┆ 1         ┆ 0         ┆ 1         │
     │ 1         ┆ 1         ┆ 0         ┆ 0         ┆ 0         ┆ 1         ┆ 1         │
     └───────────┴───────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
     '''
     _ = type_checker(df, cols, "string", "multicat_one_hot_encode")
     temp = df.lazy().select(cols).groupby(1).agg(
         pl.all().str.split(delimiter).explode().unique().sort()
-    ).select(cols) 
-    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+    ).select(cols)
+    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting
     zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
     exprs = []
     start_index = int(drop_first)
     for c in temp.collect().get_columns():
         u = c[0]
         if len(u) > 1:
             exprs.extend(
@@ -435,52 +260,25 @@
         else:
             logger.info(f"The multicategorical column {c.name} seems to have only 1 unique value. Dropped.")
 
     if isinstance(df, pl.LazyFrame):
         return df.blueprint.with_columns(exprs).blueprint.drop(cols)
     return df.with_columns(exprs).drop(cols)
 
-def force_binary(df:PolarsFrame) -> PolarsFrame:
-    '''
-    Force every binary column, no matter what data type, to be turned into 0s and 1s according to the order of the 
-    elements. If a column has two unique values like [null, "haha"], then null will be mapped to 0 and "haha" to 1.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    '''
-    binary_list = get_unique_count(df).filter(pl.col("n_unique") == 2).get_column("column")
-    temp = df.lazy().select(binary_list).groupby(1).agg(
-            pl.all().unique().sort()
-        ).select(binary_list)
-    exprs:list[pl.Expr] = []
-    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
-    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
-    for t in temp.collect().get_columns():
-        u:pl.List = t[0] # t is a Series which contains a single list which contains the 2 unique values 
-        exprs.append(
-            pl.when(pl.col(t.name) == u[0]).then(zero).otherwise(one).alias(t.name)
-        )
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
 
 def ordinal_auto_encode(
     df:PolarsFrame
     , cols:Optional[list[str]]=None
     , descending:bool = False
     , exclude:Optional[list[str]]=None
 ) -> PolarsFrame:
     '''
     Automatically applies ordinal encoding to the provided columns by the order of the elements. This method is 
-    great for string columns like age ranges, with values like ["10-20", "20-30"], etc.
+    great for string columns like age ranges, with values like ["10-20", "20-30"], etc. (Beware of string lengths,
+    e.g. if "100-110" exists in age range, then it may mess up the natural order.)
 
     This will be remembered by blueprint by default.
         
     Parameters
     ----------
     df
         Either a lazy or eager Polars DataFrame
@@ -493,67 +291,62 @@
     '''
     if isinstance(cols, list):
         _ = type_checker(df, cols, "string", "ordinal_auto_encode")
         ordinal_list = cols
     else:
         ordinal_list = get_string_cols(df, exclude=exclude)
 
-    temp = df.lazy().groupby(1).agg(
-        pl.col(c).unique().sort(descending=descending) for c in ordinal_list
+    temp = df.lazy().select(ordinal_list).groupby(1).agg(
+        pl.all().unique().sort(descending=descending) 
     ).select(ordinal_list)
     for t in temp.collect().get_columns():
         uniques:pl.Series = t[0]
-        mapping = {t.name: uniques, "to": list(range(len(uniques)))} 
+        mapping = {t.name: uniques, "to": list(range(len(uniques)))}
         if isinstance(df, pl.LazyFrame):
-            # Use a list here because Python cannot pickle a generator
             df = df.blueprint.map_dict(t.name, mapping, "to", None)
         else:
             map_tb = pl.DataFrame(mapping)
             df = df.join(map_tb, on = t.name).with_columns(
                 pl.col("to").alias(t.name)
             ).drop("to")
     return df
 
 def ordinal_encode(
     df:PolarsFrame
     , ordinal_mapping:dict[str, dict[str,int]]
-    , default:int|None=None
+    , default:Optional[int] = None
 ) -> PolarsFrame:
     '''
-    Ordinal encode the columns in the ordinal_mapping dictionary. The ordinal_mapping dict should look like:
-    {"a":{"a1":1, "a2":2}, ...}, which means for column a, a1 should be mapped to 1, a2 mapped to 2. Values 
-    not mentioned in the dict will be mapped to default.
+    Ordinal encode the columns in the ordinal_mapping dictionary.
 
     This will be remembered by blueprint by default.
         
     Parameters
     ----------
     df
         Either a lazy or eager Polars DataFrame
     ordinal_mapping
         A dictionary that looks like {"a":{"a1":1, "a2":2}, ...}
     default
-        Default value for values not mentioned in the dict.
+        Default value for values not mentioned in the ordinal_mapping dict.
     '''
-
     for c in ordinal_mapping:
         if c in df.columns:
             mapping = ordinal_mapping[c]
             if isinstance(df, pl.LazyFrame):
                 # This relies on the fact that dicts in Python is ordered
                 mapping = {c: mapping.keys(), "to": mapping.values()}
                 df = df.blueprint.map_dict(c, mapping, "to", default)
             else:
                 mapping = pl.DataFrame((mapping.keys(), mapping.values()), schema=[c, "to"])
                 df = df.join(mapping, on = c, how="left").with_columns(
                     pl.col("to").fill_null(default).alias(c)
                 ).drop("to")
         else:
             logger.warning(f"Found that column {c} is not in df. Skipped.")
-
     return df
 
 def smooth_target_encode(
     df:PolarsFrame
     , target:str
     , cols:list[str]
     , min_samples_leaf:int
@@ -591,25 +384,25 @@
     # Only works for binary target for now. There is a non-binary ver of target encode, but I
     # am just delaying the implementation...
     if check_binary:
         if not check_binary_target(df, target):
             raise ValueError("Target is not binary or not properly encoded.")
 
     # probability of target = 1
-    p = df.lazy().select(pl.col(target).mean()).collect().row(0)[0]
+    p = df.lazy().select(pl.col(target).mean()).collect().item(0,0)
     is_lazy = isinstance(df, pl.LazyFrame)
     # If c has null, null will become a group when we group by.
     for c in str_cols:
         ref = df.groupby(c).agg(
             pl.count().alias("cnt"),
             pl.col(target).mean().alias("cond_p")
         ).with_columns(
             (1./(1. + ((-(pl.col("cnt").cast(pl.Float64) - min_samples_leaf))/smoothing).exp())).alias("alpha")
         ).select(
-            pl.col(c).alias(c),
+            pl.col(c),
             to = pl.col("alpha") * pl.col("cond_p") + (pl.lit(1) - pl.col("alpha")) * pl.lit(p)
         ) # If df is lazy, ref is lazy. If df is eager, ref is eager
         if is_lazy:
             df = df.blueprint.map_dict(c, ref.collect().to_dict(), "to", None)
         else: # It is ok to do inner join because all values of c are present in ref.
             df = df.join(ref, on = c).with_columns(
                 pl.col("to").alias(c)
@@ -621,15 +414,15 @@
     for og, repl in repl_map.items():
         expr = pl.when(pl.col(c).eq(og)).then(repl).otherwise(expr)
     
     return expr.alias(c)
 
 def feature_mapping(
     df:PolarsFrame
-    , mapping: dict[str, dict[Any, Any]] | list[pl.Expr] | pl.Expr
+    , mapping: Union[dict[str, dict[Any, Any]], list[pl.Expr] , pl.Expr]
 ) -> PolarsFrame:
     '''
     Maps specific values of a feature into values provided. This is a common task when the feature columns come with 
     error codes.
 
     This will be remembered by blueprint by default.
 
@@ -912,238 +705,8 @@
         if is_lazy:
             df = df.blueprint.map_dict(s, ref.to_dict(), "woe", default)
         else:
             df = df.join(ref, on = s, how="left").with_columns(
                 pl.col("woe").fill_null(default).alias(s)
             ).drop("woe")
 
-    return df
-
-def _lmax_estimate_step(df:PolarsFrame, c:str, s:PowerTransformStrategy) -> Tuple[str, float]:
-    np_col = df.lazy().select(pl.col(c).cast(pl.Float64)).collect().get_column(c).view()
-    if s in ("yeo_johnson", "yeojohnson"):
-        lmax:float = yeojohnson_normmax(np_col)
-    else:
-        lmax:float = boxcox_normmax(np_col, method="mle")
-    
-    return (c, lmax)
-
-def power_transform(
-    df: PolarsFrame
-    , cols: list[str]
-    , strategy: PowerTransformStrategy = "yeo_johnson"
-    , n_threads:int = CPU_COUNT
-    # , lmbda: Optional[float] = None
-) -> PolarsFrame:
-    '''
-    Performs power transform on the numerical columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and must all be numerical
-    strategy
-        Either 'yeo_johnson' or 'box_cox'
-    n_threads
-        The max number of worker threads to use in Python
-    '''
-    _ = type_checker(df, cols, "numeric", "power_transform")
-    s = clean_strategy_str(strategy)
-    exprs:list[pl.Expr] = []
-    # Ensure columns do not have missing values
-    exclude_columns_w_nulls = df.lazy().select(cols).null_count().collect().transpose(
-        include_header=True, column_names=["null_count"]
-    ).filter(pl.col("null_count") > 0).get_column("column").to_list()
-
-    if len(exclude_columns_w_nulls) > 0:
-        logger.info("The following columns will not be processed by power_transform because they contain missing "
-                    f"values. Please impute them:\n{exclude_columns_w_nulls}")
-        
-    non_null_list = [c for c in cols if c not in exclude_columns_w_nulls]
-    pbar = tqdm(non_null_list, desc = "Inferring best paramters")
-    if s in ("yeo_johnson", "yeojohnson"):
-        with ThreadPoolExecutor(max_workers=n_threads) as ex:
-            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
-                c, lmax = future.result()
-                if lmax == 0: # log(x + 1)
-                    x_ge_0_sub_expr = (pl.col(c).add(1)).log()
-                else: # ((x + 1)**lmbda - 1) / lmbda
-                    x_ge_0_sub_expr = ((pl.col(c).add(1)).pow(lmax) - 1) / lmax
-
-                if lmax == 2: # -log(-x + 1)
-                    x_lt_0_sub_expr = pl.lit(-1) * (1 - pl.col(c)).log()
-                else: #  -((-x + 1)**(2 - lmbda) - 1) / (2 - lmbda)
-                    t = 2 - lmax
-                    x_lt_0_sub_expr = pl.lit(-1/t) * ((1 - pl.col(c)).pow(t) - 1)
-
-                exprs.append(
-                    pl.when(pl.col(c).ge(0)).then(x_ge_0_sub_expr).otherwise(x_lt_0_sub_expr).alias(c)
-                )
-                pbar.update(1)
-
-    elif s in ("box_cox", "boxcox"):
-        with ThreadPoolExecutor(max_workers=n_threads) as ex:
-            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
-                c, lmax = future.result()
-                if lmax == 0: # log(x)
-                    exprs.append(pl.col(c).log())
-                else: # (x**lmbda - 1) / lmbda
-                    exprs.append(
-                        (pl.col(c).pow(lmax) - 1) / lmax
-                    )
-                pbar.update(1)
-    else:
-        raise TypeError(f"The input strategy {strategy} is not a valid strategy. Valid strategies are: yeo_johnson "
-                        "or box_cox")
-    pbar.close()
-    if isinstance(df, pl.LazyFrame):
-        return df.lazy().blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-
-# Should feature engineering spin off to its own module? Or stay in transform?
-# First, I need to wait until I have more feature engineering stuff..
-
-def normalize(
-    df: PolarsFrame
-    , cols:list[str]
-) -> PolarsFrame:
-    '''
-    Normalize the given columns by dividing them with the respective column sum.
-
-    !!!Note this will not be remember by the pipeline!!!
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be numeric columns
-    '''
-    
-    types = check_columns_types(df, cols)
-    if types != "numeric":
-        raise ValueError(f"normalize can only be used on numeric columns, not {types} types.")
-
-    return df.with_columns(pl.col(c)/pl.col(c).sum() for c in cols)
-
-def log_transform(
-    df: PolarsFrame
-    , cols:list[str]
-    , base:float = math.e
-    , cast_non_positive: None | float = None
-) -> PolarsFrame:
-    '''
-    Performs classical log transform on the given columns
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be numeric columns
-    base
-        Base of log. Default is math.e
-    cast_non_positive
-        How to deal with non positive values (<=0). None means turn them into null
-    '''
-    _ = type_checker(df, cols, "numeric", "log_transform")
-    exprs = [
-        pl.when(pl.col(c) <= 0).then(cast_non_positive).otherwise(pl.col(c).log(base)).suffix("_log") for c in cols
-    ]
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-def extract_dt_features(
-    df: PolarsFrame
-    , cols: list[str]
-    , extract: DateExtract | list[DateExtract] = ["year", "quarter", "month"]
-    , sunday_first: bool = False
-) -> PolarsFrame:
-    '''
-    Extracts additional date related features from existing date/datetime columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be date/datetime columns
-    extract
-        One of "year", "quarter", "month", "week", "day_of_week", "day_of_year", or a list of these values
-        such as ["year", "quarter"], which means extract year and quarter from all the columns provided 
-    sunday_first
-        For day_of_week, by default, Monday maps to 1, and so on. If sunday_first = True, then Sunday will be
-        mapped to 1 and so on
-
-    Example
-    -------
-    >>> import dsds.transform as t
-    ... df = pl.DataFrame({
-    ...     "date1":["2021-01-01", "2022-02-03", "2023-11-23"]
-    ...     , "date2":["2021-01-01", "2022-02-03", "2023-11-23"]
-    ... }).with_columns(
-    ...     pl.col(c).str.to_date() for c in ["date1", "date2"]
-    ... )
-    >>> print(df)
-    shape: (3, 2)
-    ┌────────────┬────────────┐
-    │ date1      ┆ date2      │
-    │ ---        ┆ ---        │
-    │ date       ┆ date       │
-    ╞════════════╪════════════╡
-    │ 2021-01-01 ┆ 2021-01-01 │
-    │ 2022-02-03 ┆ 2022-02-03 │
-    │ 2023-11-23 ┆ 2023-11-23 │
-    └────────────┴────────────┘
-    >>> cols = ["date1", "date2"]
-    >>> print(t.extract_dt_features(df, cols=cols))
-    shape: (3, 8)
-    ┌────────────┬────────────┬────────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
-    │ date1      ┆ date2      ┆ date1_year ┆ date2_yea ┆ date1_qua ┆ date2_qua ┆ date1_mon ┆ date2_mon │
-    │ ---        ┆ ---        ┆ ---        ┆ r         ┆ rter      ┆ rter      ┆ th        ┆ th        │
-    │ date       ┆ date       ┆ u16        ┆ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       │
-    │            ┆            ┆            ┆ u16       ┆ u8        ┆ u8        ┆ u8        ┆ u8        │
-    ╞════════════╪════════════╪════════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
-    │ 2021-01-01 ┆ 2021-01-01 ┆ 2021       ┆ 2021      ┆ 1         ┆ 1         ┆ 1         ┆ 1         │
-    │ 2022-02-03 ┆ 2022-02-03 ┆ 2022       ┆ 2022      ┆ 1         ┆ 1         ┆ 2         ┆ 2         │
-    │ 2023-11-23 ┆ 2023-11-23 ┆ 2023       ┆ 2023      ┆ 4         ┆ 4         ┆ 11        ┆ 11        │
-    └────────────┴────────────┴────────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
-    '''
-    _ = type_checker(df, cols, "datetime", "extract_dt_features")
-    exprs = []
-    if isinstance(extract, list):
-        to_extract = extract
-    else:
-        to_extract = [extract]
-    
-    for e in to_extract:
-        if e == "month":
-            exprs.extend(pl.col(c).dt.month().cast(pl.UInt8).suffix("_month") for c in cols)
-        elif e == "year":
-            exprs.extend(pl.col(c).dt.year().cast(pl.UInt16).suffix("_year") for c in cols)
-        elif e == "quarter":
-            exprs.extend(pl.col(c).dt.quarter().cast(pl.UInt8).suffix("_quarter") for c in cols)
-        elif e == "week":
-            exprs.extend(pl.col(c).dt.week().cast(pl.UInt8).suffix("_week") for c in cols)
-        elif e == "day_of_week":
-            if sunday_first:
-                exprs.extend(((pl.col(c).dt.weekday()+1)%7).cast(pl.UInt8).suffix("_day_of_week") for c in cols)
-            else:
-                exprs.extend(pl.col(c).dt.weekday().cast(pl.UInt8).suffix("_day_of_week") for c in cols)
-        elif e == "day_of_year":
-            exprs.extend(pl.col(c).dt.ordinal_day().cast(pl.UInt8).suffix("_day_of_year") for c in cols)
-        else:
-            logger.error(f"Found {e} in extract, but is not a valid DateExtract value. Ignored.")
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
+    return df
```

### Comparing `dsds-0.0.21/src/dsds/type_alias.py` & `dsds-0.0.23/src/dsds/type_alias.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,85 @@
 from typing import (
     Literal
     , Final
     , Tuple
+    , Union
 )
-
+from abc import ABC, abstractmethod
 import polars as pl
 import sys
 if sys.version_info >= (3, 10):
     from typing import TypeAlias, Concatenate, ParamSpec, Callable
     P = ParamSpec('P')
-    PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
+    PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
     PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
 else:
     from typing_extensions import TypeAlias
-    PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
+    PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
     PipeFunction = Callable
 
 import os
 import numpy as np
-from abc import ABC, abstractmethod
-
 
+# --- Constants ---
 CPU_COUNT:Final[int] = os.cpu_count()
-POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64, pl.Int8, pl.Int16, pl.Int32, pl.Int64)  # noqa: E501
+CPU_M1: Final[int] = CPU_COUNT - 1
+POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64
+                                                    , pl.Int8, pl.Int16, pl.Int32, pl.Int64)
 POLARS_DATETIME_TYPES:Final[Tuple[pl.DataType]] = (pl.Datetime, pl.Date)
 
-ActionType:TypeAlias = Literal["with_columns", "map_dict", "drop", "select", "add_func", "filter"]
+# --- Strategies ---
 MRMRStrategy:TypeAlias = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
-                       , "mutual_info_score", "lgbm", "lightgbm"]
+                                , "mutual_info_score", "lgbm", "lightgbm"]
 ScalingStrategy:TypeAlias = Literal["standard", "min_max", "const", "constant"]
 ImputationStrategy:TypeAlias = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
 PowerTransformStrategy:TypeAlias = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
-KSAlternatives = Literal["two-sided", "greater", "less"]
 
-SimpleDtypes:TypeAlias = Literal["numeric", "datetime", "bool", "string", "other/unknown"]
+# --- Models ---
 BinaryModels:TypeAlias = Literal["logistic", "lr", "lightgbm", "lgbm", "xgboost", "xgb", "random_forest", "rf"]
+
+# --- Extracts ---
 DateExtract:TypeAlias = Literal["year", "quarter", "month", "week", "day_of_week", "day_of_year"]
-# ArithmeticTransforms = Literal["log", "exp", "sqrt", "fourier"]
-# This is just a subset of Scipy.stats's distributions which can be named by strings. All scipy.stats's string-name-able
-# distributions should work when the arguments asks for a CommonContinuousDist.
-CommonContinuousDist:TypeAlias = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
+ListExtract:TypeAlias = Literal["min", "max", "mean", "len", "first", "last"]
+HorizontalExtract:TypeAlias = Literal["min", "max", "sum", "any", "all"]
+
+# --- Stats Related ---
+Alternatives = Literal["two-sided", "greater", "less"]
+# This is just a subset of Scipy.stats's distributions which can be named by strings. 
+# All scipy.stats's string-name-able distributions should work when the arguments asks 
+# for a CommonContinuousDist.
+CommonContiDist:TypeAlias = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
+
+# --- Other ---
+ZeroOneCombineRules = Literal["union", "intersection", "same"]
+SimpleDtypes:TypeAlias = Literal["numeric", "datetime", "bool", "string", "other/unknown"]
+ActionType:TypeAlias = Literal["with_columns", "map_dict", "drop", "select", "add_func", "filter", "classif"
+                               , "regression"]
 
+# --- Utils ---
 def clean_strategy_str(s:str):
     '''Strategy strings will only have _, no -, and all lowercase.'''
     return s.strip().replace("-", "_").lower()
 
+# --- ABC ---
 class ClassifModel(ABC):
 
     @abstractmethod
-    def predict(self, X:np.ndarray|pl.DataFrame) -> np.ndarray:
+    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
         ...
 
     @abstractmethod
-    def predict_proba(self, X: np.ndarray|pl.DataFrame) -> np.ndarray:
+    def predict_proba(self, X: Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
         ...
 
     @abstractmethod
-    def fit(self, X:np.ndarray|pl.DataFrame, y:np.ndarray|pl.Series|pl.DataFrame): # Should return self
+    def fit(self, X:Union[np.ndarray,pl.DataFrame], y:Union[np.ndarray,pl.Series,pl.DataFrame]): # Should return self
         ...
     
 class RegressionModel(ABC):
     @abstractmethod
-    def predict(self, X: np.ndarray|pl.DataFrame) -> np.ndarray:
+    def predict(self, X: Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
         ...
 
     @abstractmethod
-    def fit(self, X:np.ndarray|pl.DataFrame, y:np.ndarray|pl.Series|pl.DataFrame): # Should return self
+    def fit(self, X:Union[np.ndarray,pl.DataFrame], y:Union[np.ndarray,pl.Series,pl.DataFrame]): # Should return self
         ...
```

### Comparing `dsds-0.0.21/src/dsds.egg-info/PKG-INFO` & `dsds-0.0.23/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.21
+Version: 0.0.23
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,15 +44,15 @@
 Provides-Extra: xgboost
 Provides-Extra: lightgbm
 Provides-Extra: all
 License-File: LICENSE
 
 # Welcome to the Dark Side of Data Science (DSDS)
 
-This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package.
+This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package. Also see disclaimer in the end.
 
 Welcome to DSDS, a data science package that aims to be an improvement over a subset of sklearn's functionality, primarily in the following areas:
 
 1. Providing practical feature prescreen (immediate detection and removal of useless featuers, data profiling, etc.)
 2. Fast and furious feature selection (significantly faster F-score, MRMR, mutual_info_score, etc.)
 3. Cleaner pipeline construction and management (See examples below.)
 4. Compatible with Polars LazyFrames (Yes! Pipelines can enjoy the benefits of query optimization too!)
@@ -102,15 +102,17 @@
 
 Performance without sacrificing user experience. See ./examples/dsds_comparisons.ipynb
 
 ![Screenshot](./pics/impute.PNG)
 
 ## Dependencies
 
-Python 3.9, 3.10, 3.11+ is recommended. We are forward looking.
+Python 3.9, 3.10, 3.11+ is recommended. We are forward looking. 
+
+It should run on all versions >= 3.9. But I haven't tested 3.9 and 3.10 thoroughly.
 
 pip install polars scipy numpy
 
 pip install dsds[all]
 
 Note: scikit-learn, lightgbm, xgboost are needed for full functionalities. 
 
@@ -134,8 +136,27 @@
 
 You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
 
 # Why not write more functionalities in Rust?
 
 Yes. I will. I am not confident enough with my Rust skill at the moment. I am slowly learning more Rust and hopefully we can delegate more heavy work to Rust. The immediate benefit of using more Rust will be (1) slightly more memory efficient, and (2) slightly faster. I do not expect huge speed boost because most code are written in Polars already. There are some cases when a lot of Python stuff is added (lists and for loops, etc.). But we definitely need to evaluate the gain by using Rust more carefully in the future.
 
+# Disclaimer
+
+I do not claim dsds is a superior package to any other traditional machine learning libraries. In fact no one can make this claim. Each package has their own flavor, and there are things that people can disagree with. Disagreements do not translate to contempt or hatred. I primarily set out to make this project because:
+
+1. I want to learn more about machine learning engineering
+2. I want to improve my coding skill
+3. I see opportunies to make things run faster using Polars without relying on bigger machines on the cloud. I want to make this happen for everybody.
+4. I don't think OOP is right for scientific computing.
+
+Everyone has their own bias. I believe in the functional style for scientific computing. I don't like the OOP style adopted by so many other packages, especially the one used in Sklearn pipelines. If you want to discuss, please kindly send me a message on discord. Please do not cherry pick points and claim that my code is **** just because you have never seen functional codebase or projects done in this style. I do not claim to have the best style of code either. OOP elements are still used in this project because it is inevitable in Python.
+
+That said, since performance and functional design are the two major pillars of this project, I will include a lot of benchmarks and code that showcase the style differences. A lot of benchmarks will be done vs. Scikit-learn because Scikit-learn is the de facto "standard" in the tranditional machine learning space. I do this not because I want to prove dsds is superior, but because I want to show the improvement and show people that dsds achieves what it aims to achieve, an improvement over a subset of Scikit-learn's functionalities (in the areas that I set out to improve on, e.g. performance and 'style').
+
+Every few days there is a new javascript framework. Why can't data scientists challenge the design of Scikit-learn? I started learning using Scikit-learn, like 90% of all the data scientists out there. I am free to express my opinions and criticisms. 
+
+No package is perfect and you are free to like/hate it. Just don't be complaining online without ever thinking deeply about machine learning infra and bottlenecks in machine learning pipelines. Don't hate on things because they are different.
+
+# Contribution
+
 See CONTRIBUTING.md for my contact info.
```

