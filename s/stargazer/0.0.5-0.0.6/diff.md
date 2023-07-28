# Comparing `tmp/stargazer-0.0.5.tar.gz` & `tmp/stargazer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stargazer-0.0.5.tar", last modified: Tue Jul 14 01:16:49 2020, max compression
+gzip compressed data, was "stargazer-0.0.6.tar", last modified: Fri Jul 28 11:54:51 2023, max compression
```

## Comparing `stargazer-0.0.5.tar` & `stargazer-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0 mwburke   (1000) mwburke   (1000)        0 2020-07-14 01:16:49.000000 stargazer-0.0.5/
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)     6807 2020-07-14 01:16:49.000000 stargazer-0.0.5/PKG-INFO
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)     5786 2020-07-14 00:56:29.000000 stargazer-0.0.5/README.md
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)       38 2020-07-14 01:16:49.000000 stargazer-0.0.5/setup.cfg
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)      605 2020-07-14 00:56:29.000000 stargazer-0.0.5/setup.py
-drwxrwxrwx   0 mwburke   (1000) mwburke   (1000)        0 2020-07-14 01:16:49.000000 stargazer-0.0.5/stargazer/
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)       19 2018-06-21 19:57:44.000000 stargazer-0.0.5/stargazer/__init__.py
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)    27855 2020-07-14 00:56:29.000000 stargazer-0.0.5/stargazer/stargazer.py
-drwxrwxrwx   0 mwburke   (1000) mwburke   (1000)        0 2020-07-14 01:16:49.000000 stargazer-0.0.5/stargazer.egg-info/
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)     6807 2020-07-14 01:16:49.000000 stargazer-0.0.5/stargazer.egg-info/PKG-INFO
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)      195 2020-07-14 01:16:49.000000 stargazer-0.0.5/stargazer.egg-info/SOURCES.txt
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)        1 2020-07-14 01:16:49.000000 stargazer-0.0.5/stargazer.egg-info/dependency_links.txt
--rwxrwxrwx   0 mwburke   (1000) mwburke   (1000)       10 2020-07-14 01:16:49.000000 stargazer-0.0.5/stargazer.egg-info/top_level.txt
+drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2023-07-28 11:54:51.036068 stargazer-0.0.6/
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      509 2019-10-12 15:25:47.000000 stargazer-0.0.6/LICENSE
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     6304 2023-07-28 11:54:51.036068 stargazer-0.0.6/PKG-INFO
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     5868 2023-07-24 22:39:27.000000 stargazer-0.0.6/README.md
+-rw-r--r--   0 pietro    (1000) pietro    (1000)       38 2023-07-28 11:54:51.036068 stargazer-0.0.6/setup.cfg
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      653 2023-07-28 06:14:43.000000 stargazer-0.0.6/setup.py
+drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2023-07-28 11:54:51.036068 stargazer-0.0.6/stargazer/
+-rw-r--r--   0 pietro    (1000) pietro    (1000)       19 2019-10-12 15:25:47.000000 stargazer-0.0.6/stargazer/__init__.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)    31325 2023-07-22 22:42:06.000000 stargazer-0.0.6/stargazer/stargazer.py
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     1107 2021-10-12 16:00:48.000000 stargazer-0.0.6/stargazer/utils.py
+drwxr-xr-x   0 pietro    (1000) pietro    (1000)        0 2023-07-28 11:54:51.036068 stargazer-0.0.6/stargazer.egg-info/
+-rw-r--r--   0 pietro    (1000) pietro    (1000)     6304 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/PKG-INFO
+-rw-r--r--   0 pietro    (1000) pietro    (1000)      222 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/SOURCES.txt
+-rw-r--r--   0 pietro    (1000) pietro    (1000)        1 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/dependency_links.txt
+-rw-r--r--   0 pietro    (1000) pietro    (1000)       10 2023-07-28 11:54:51.000000 stargazer-0.0.6/stargazer.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stargazer-0.0.5/PKG-INFO` & `stargazer-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,110 @@
 Metadata-Version: 2.1
 Name: stargazer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Nicely formatted regression reporting
-Home-page: https://github.com/mwburke/stargazer
-Author: Matthew Burke
-Author-email: matthew.wesley.burke@gmail.com
+Home-page: https://github.com/StatsReporting/stargazer
+Author: Pietro Battiston, Matthew Burke
+Author-email: me@pietrobattiston.it, matthew.wesley.burke@gmail.com
 License: GPLv2
-Description: # Stargazer
-        
-        This is a python port of the R stargazer package that can be found [on CRAN](https://CRAN.R-project.org/package=stargazer). I was disappointed that there wasn't equivalent functionality in any python packages I was aware of so I'm re-implementing it here.
-        
-        There is an experimental function in the [statsmodels.regression.linear_model.OLSResults.summary2](http://www.statsmodels.org/dev/generated/statsmodels.regression.linear_model.OLSResults.summary2.html) that can report single regression model results in HTML/CSV/LaTeX/etc, but it still didn't quite fulfill what I was looking for.
-        
-        The python package is object oriented now with chained commands to make changes to the rendering parameters, which is hopefully more pythonic and the user doesn't have to put a bunch of arguments in a single function.
-        
-        ## Installation
-        
-        You can install this package through PyPi with `pip install stargazer` or just clone the repo and take the `stargazer.py` file since it's the only one in the package.
-        
-        ### Dependencies
-        
-        It depends on `statsmodels`, which in turn depends on several other libraries like `pandas`, `numpy`, etc
-        
-        ## Editing Features
-        
-        This library implements many of the customization features found in the original package. Examples of most can be found [in the examples jupyter notebook](https://github.com/mwburke/stargazer/blob/master/examples.ipynb) and a full list of the methods/features is here below:
-        
-        * `title`: custom title
-        * `show_header`: display or hide model header data
-        * `show_model_numbers`: display or hide model numbers
-        * `custom_columns`: custom model names and model groupings
-        * `significance_levels`: change statistical significance thresholds
-        * `significant_digits`: change number of significant digits
-        * `show_confidence_intervals`: display confidence intervals instead of variance
-        * `dependent_variable_name`: rename dependent variable
-        * `rename_covariates`: rename covariates
-        * `covariate_order`: reorder covariates
-        * `reset_covariate_order`: reset covariate order to original ordering
-        * `show_degrees_of_freedom`: display or hide degrees of freedom
-        * `custom_note_label`: label notes section at bottom of table
-        * `add_custom_notes`: add custom notes to section at bottom of the table
-        * `add_line`: add a custom line to the table
-        * `append_notes`: display or hide statistical significance thresholds
-        
-        These features are agnostic of the rendering type and will be applied whether the user outputs in HTML, LaTeX, etc
-        
-        ## Example
-        
-        Here is an examples of how to quickly get started with the library. More examples can be found in the `examples.ipynb` file in the github repo. The examples all use the scikit-learn diabetes dataset, but it is not a dependency for the package.
-        
-        ### OLS Models Preparation
-        
-        ```python
-        import pandas as pd
-        from sklearn import datasets
-        import statsmodels.api as sm
-        from stargazer.stargazer import Stargazer
-        
-        diabetes = datasets.load_diabetes()
-        df = pd.DataFrame(diabetes.data)
-        df.columns = ['Age', 'Sex', 'BMI', 'ABP', 'S1', 'S2', 'S3', 'S4', 'S5', 'S6']
-        df['target'] = diabetes.target
-        
-        est = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:4]])).fit()
-        est2 = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:6]])).fit()
-        
-        
-        stargazer = Stargazer([est, est2])
-        ```
-        
-        ### HTML Example
-        
-        ```python
-        stargazer.render_html()
-        ```
-        
-        <table style="text-align:center"><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><td style="text-align:left"></td><td colspan="2"><em>Dependent variable:</em></td></tr><tr><td style="text-align:left"><tr><td style="text-align:left"></td><td>(1)</td><td>(2)</td></tr><td colspan="3" style="border-bottom: 1px solid black"><tr><td style="text-align:left">ABP</td><td>416.674<sup>***</sup></td><td>397.583<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(69.495)</td><td>(70.87)</td></tr><tr><td style="text-align:left">Age</td><td>37.241<sup></sup></td><td>24.704<sup></sup></td></tr><tr><td style="text-align:left"></td><td>(64.117)</td><td>(65.411)</td></tr><tr><td style="text-align:left">BMI</td><td>787.179<sup>***</sup></td><td>789.742<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(65.424)</td><td>(66.887)</td></tr><tr><td style="text-align:left">S1</td><td></td><td>197.852<sup></sup></td></tr><tr><td style="text-align:left"></td><td></td><td>(143.812)</td></tr><tr><td style="text-align:left">S2</td><td></td><td>-169.251<sup></sup></td></tr><tr><td style="text-align:left"></td><td></td><td>(142.744)</td></tr><tr><td style="text-align:left">Sex</td><td>-106.578<sup>*</sup></td><td>-82.862<sup></sup></td></tr><tr><td style="text-align:left"></td><td>(62.125)</td><td>(64.851)</td></tr><tr><td style="text-align:left">const</td><td>152.133<sup>***</sup></td><td>152.133<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(2.853)</td><td>(2.853)</td></tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Observations</td><td>442.0</td><td>442.0</td></tr><tr><td style="text-align: left">R<sup>2</sup></td><td>0.4</td><td>0.403</td></tr><tr><td style="text-align: left">Adjusted R<sup>2</sup></td><td>0.395</td><td>0.395</td></tr><tr><td style="text-align: left">Residual Std. Error</td><td>59.976(df = 437.0)</td><td>59.982(df = 435.0)</td></tr><tr><td style="text-align: left">F Statistic</td><td>72.913<sup>***</sup>(df = 4.0; 437.0)</td><td>48.915<sup>***</sup>(df = 6.0; 435.0)</td></tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Note:</td><td colspan="2" style="text-align: right"><em>p<0.1</em>; <b>p<0.05</b>; p<0.01</td></tr></table>
-        
-        ### LaTeX Example
-        
-        ```python
-        stargazer.render_latex()
-        ```
-        
-        ![](https://raw.githubusercontent.com/mwburke/stargazer/master/latex_example.png)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Stargazer
+
+This is a python port of the R stargazer package that can be found [on CRAN](https://CRAN.R-project.org/package=stargazer). I was disappointed that there wasn't equivalent functionality in any python packages I was aware of so I'm re-implementing it here.
+
+There is an experimental function in the [statsmodels.regression.linear_model.OLSResults.summary2](http://www.statsmodels.org/dev/generated/statsmodels.regression.linear_model.OLSResults.summary2.html) that can report single regression model results in HTML/CSV/LaTeX/etc, but it still didn't quite fulfill what I was looking for.
+
+The python package is object oriented now with chained commands to make changes to the rendering parameters, which is hopefully more pythonic and the user doesn't have to put a bunch of arguments in a single function.
+
+## Installation
+
+You can install this package through PyPi with `pip install stargazer` or just clone the repo and take the `stargazer.py` file since it's the only one in the package.
+
+### Dependencies
+
+It depends on `statsmodels`, which in turn depends on several other libraries like `pandas`, `numpy`, etc
+
+## Editing Features
+
+This library implements many of the customization features found in the original package. Examples of most can be found [in the examples jupyter notebook](https://github.com/StatsReporting/stargazer/blob/master/examples.ipynb) and a full list of the methods/features is here below:
+
+* `title`: custom title
+* `show_header`: display or hide model header data
+* `show_model_numbers`: display or hide model numbers
+* `custom_columns`: custom model names and model groupings
+* `significance_levels`: change statistical significance thresholds
+* `significant_digits`: change number of significant digits
+* `show_confidence_intervals`: display confidence intervals instead of variance
+* `dependent_variable_name`: rename dependent variable
+* `rename_covariates`: rename covariates
+* `covariate_order`: reorder covariates
+* `reset_covariate_order`: reset covariate order to original ordering
+* `show_degrees_of_freedom`: display or hide degrees of freedom
+* `custom_note_label`: label notes section at bottom of table
+* `add_custom_notes`: add custom notes to section at bottom of the table
+* `add_line`: add a custom line to the table
+* `append_notes`: display or hide statistical significance thresholds
+
+These features are agnostic of the rendering type and will be applied whether the user outputs in HTML, LaTeX, etc
+
+## Example
+
+Here is an examples of how to quickly get started with the library. More examples can be found in the `examples.ipynb` file in the github repo. The examples all use the scikit-learn diabetes dataset, but it is not a dependency for the package.
+
+### OLS Models Preparation
+
+```python
+import pandas as pd
+from sklearn import datasets
+import statsmodels.api as sm
+from stargazer.stargazer import Stargazer
+
+diabetes = datasets.load_diabetes()
+df = pd.DataFrame(diabetes.data)
+df.columns = ['Age', 'Sex', 'BMI', 'ABP', 'S1', 'S2', 'S3', 'S4', 'S5', 'S6']
+df['target'] = diabetes.target
+
+est = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:4]])).fit()
+est2 = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:6]])).fit()
+
+
+stargazer = Stargazer([est, est2])
+```
+
+### HTML Example
+
+```python
+stargazer.render_html()
+```
+
+<table style="text-align:center"><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left"></td><td colspan="2"><em>Dependent variable: target</em></td></tr><tr><td style="text-align:left"></td><tr><td style="text-align:left"></td><td>(1)</td><td>(2)</td></tr><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr>
+
+<tr><td style="text-align:left">ABP</td><td>416.674<sup>***</sup></td><td>397.583<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(69.495)</td><td>(70.870)</td></tr>
+<tr><td style="text-align:left">Age</td><td>37.241<sup></sup></td><td>24.704<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td>(64.117)</td><td>(65.411)</td></tr>
+<tr><td style="text-align:left">BMI</td><td>787.179<sup>***</sup></td><td>789.742<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(65.424)</td><td>(66.887)</td></tr>
+<tr><td style="text-align:left">S1</td><td></td><td>197.852<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td></td><td>(143.812)</td></tr>
+<tr><td style="text-align:left">S2</td><td></td><td>-169.251<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td></td><td>(142.744)</td></tr>
+<tr><td style="text-align:left">Sex</td><td>-106.578<sup>*</sup></td><td>-82.862<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td>(62.125)</td><td>(64.851)</td></tr>
+<tr><td style="text-align:left">const</td><td>152.133<sup>***</sup></td><td>152.133<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(2.853)</td><td>(2.853)</td></tr>
+
+<td colspan="3" style="border-bottom: 1px solid black"></td></tr>
+<tr><td style="text-align: left">Observations</td><td>442</td><td>442</td></tr><tr><td style="text-align: left">R<sup>2</sup></td><td>0.400</td><td>0.403</td></tr><tr><td style="text-align: left">Adjusted R<sup>2</sup></td><td>0.395</td><td>0.395</td></tr><tr><td style="text-align: left">Residual Std. Error</td><td>59.976 (df=437)</td><td>59.982 (df=435)</td></tr><tr><td style="text-align: left">F Statistic</td><td>72.913<sup>***</sup> (df=4; 437)</td><td>48.915<sup>***</sup> (df=6; 435)</td></tr>
+<tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Note:</td><td colspan="2" style="text-align: right"><sup>*</sup>p&lt;0.1; <sup>**</sup>p&lt;0.05; <sup>***</sup>p&lt;0.01</td></tr></table>
+
+### LaTeX Example
+
+```python
+stargazer.render_latex()
+```
+
+![](https://raw.githubusercontent.com/StatsReporting/stargazer/master/latex_example.png)
```

### Comparing `stargazer-0.0.5/README.md` & `stargazer-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ### Dependencies
 
 It depends on `statsmodels`, which in turn depends on several other libraries like `pandas`, `numpy`, etc
 
 ## Editing Features
 
-This library implements many of the customization features found in the original package. Examples of most can be found [in the examples jupyter notebook](https://github.com/mwburke/stargazer/blob/master/examples.ipynb) and a full list of the methods/features is here below:
+This library implements many of the customization features found in the original package. Examples of most can be found [in the examples jupyter notebook](https://github.com/StatsReporting/stargazer/blob/master/examples.ipynb) and a full list of the methods/features is here below:
 
 * `title`: custom title
 * `show_header`: display or hide model header data
 * `show_model_numbers`: display or hide model numbers
 * `custom_columns`: custom model names and model groupings
 * `significance_levels`: change statistical significance thresholds
 * `significant_digits`: change number of significant digits
@@ -63,16 +63,35 @@
 
 ### HTML Example
 
 ```python
 stargazer.render_html()
 ```
 
-<table style="text-align:center"><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><td style="text-align:left"></td><td colspan="2"><em>Dependent variable:</em></td></tr><tr><td style="text-align:left"><tr><td style="text-align:left"></td><td>(1)</td><td>(2)</td></tr><td colspan="3" style="border-bottom: 1px solid black"><tr><td style="text-align:left">ABP</td><td>416.674<sup>***</sup></td><td>397.583<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(69.495)</td><td>(70.87)</td></tr><tr><td style="text-align:left">Age</td><td>37.241<sup></sup></td><td>24.704<sup></sup></td></tr><tr><td style="text-align:left"></td><td>(64.117)</td><td>(65.411)</td></tr><tr><td style="text-align:left">BMI</td><td>787.179<sup>***</sup></td><td>789.742<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(65.424)</td><td>(66.887)</td></tr><tr><td style="text-align:left">S1</td><td></td><td>197.852<sup></sup></td></tr><tr><td style="text-align:left"></td><td></td><td>(143.812)</td></tr><tr><td style="text-align:left">S2</td><td></td><td>-169.251<sup></sup></td></tr><tr><td style="text-align:left"></td><td></td><td>(142.744)</td></tr><tr><td style="text-align:left">Sex</td><td>-106.578<sup>*</sup></td><td>-82.862<sup></sup></td></tr><tr><td style="text-align:left"></td><td>(62.125)</td><td>(64.851)</td></tr><tr><td style="text-align:left">const</td><td>152.133<sup>***</sup></td><td>152.133<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(2.853)</td><td>(2.853)</td></tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Observations</td><td>442.0</td><td>442.0</td></tr><tr><td style="text-align: left">R<sup>2</sup></td><td>0.4</td><td>0.403</td></tr><tr><td style="text-align: left">Adjusted R<sup>2</sup></td><td>0.395</td><td>0.395</td></tr><tr><td style="text-align: left">Residual Std. Error</td><td>59.976(df = 437.0)</td><td>59.982(df = 435.0)</td></tr><tr><td style="text-align: left">F Statistic</td><td>72.913<sup>***</sup>(df = 4.0; 437.0)</td><td>48.915<sup>***</sup>(df = 6.0; 435.0)</td></tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Note:</td><td colspan="2" style="text-align: right"><em>p<0.1</em>; <b>p<0.05</b>; p<0.01</td></tr></table>
+<table style="text-align:center"><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left"></td><td colspan="2"><em>Dependent variable: target</em></td></tr><tr><td style="text-align:left"></td><tr><td style="text-align:left"></td><td>(1)</td><td>(2)</td></tr><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr>
+
+<tr><td style="text-align:left">ABP</td><td>416.674<sup>***</sup></td><td>397.583<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(69.495)</td><td>(70.870)</td></tr>
+<tr><td style="text-align:left">Age</td><td>37.241<sup></sup></td><td>24.704<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td>(64.117)</td><td>(65.411)</td></tr>
+<tr><td style="text-align:left">BMI</td><td>787.179<sup>***</sup></td><td>789.742<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(65.424)</td><td>(66.887)</td></tr>
+<tr><td style="text-align:left">S1</td><td></td><td>197.852<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td></td><td>(143.812)</td></tr>
+<tr><td style="text-align:left">S2</td><td></td><td>-169.251<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td></td><td>(142.744)</td></tr>
+<tr><td style="text-align:left">Sex</td><td>-106.578<sup>*</sup></td><td>-82.862<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td>(62.125)</td><td>(64.851)</td></tr>
+<tr><td style="text-align:left">const</td><td>152.133<sup>***</sup></td><td>152.133<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(2.853)</td><td>(2.853)</td></tr>
+
+<td colspan="3" style="border-bottom: 1px solid black"></td></tr>
+<tr><td style="text-align: left">Observations</td><td>442</td><td>442</td></tr><tr><td style="text-align: left">R<sup>2</sup></td><td>0.400</td><td>0.403</td></tr><tr><td style="text-align: left">Adjusted R<sup>2</sup></td><td>0.395</td><td>0.395</td></tr><tr><td style="text-align: left">Residual Std. Error</td><td>59.976 (df=437)</td><td>59.982 (df=435)</td></tr><tr><td style="text-align: left">F Statistic</td><td>72.913<sup>***</sup> (df=4; 437)</td><td>48.915<sup>***</sup> (df=6; 435)</td></tr>
+<tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Note:</td><td colspan="2" style="text-align: right"><sup>*</sup>p&lt;0.1; <sup>**</sup>p&lt;0.05; <sup>***</sup>p&lt;0.01</td></tr></table>
 
 ### LaTeX Example
 
 ```python
 stargazer.render_latex()
 ```
 
-![](https://raw.githubusercontent.com/mwburke/stargazer/master/latex_example.png)
+![](https://raw.githubusercontent.com/StatsReporting/stargazer/master/latex_example.png)
```

### Comparing `stargazer-0.0.5/setup.py` & `stargazer-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stargazer",
-    version="0.0.5",
-    author="Matthew Burke",
-    author_email="matthew.wesley.burke@gmail.com",
+    version="0.0.6",
+    author="Pietro Battiston, Matthew Burke",
+    author_email="me@pietrobattiston.it, matthew.wesley.burke@gmail.com",
     description="Nicely formatted regression reporting",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/mwburke/stargazer",
+    url="https://github.com/StatsReporting/stargazer",
     packages=setuptools.find_packages(),
     license='GPLv2',
     classifiers=(
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ),
 )
```

### Comparing `stargazer-0.0.5/stargazer/stargazer.py` & `stargazer-0.0.6/stargazer/stargazer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 """
 This is a python package to generate nicely formatted
 regression results similar to the style of the R
 package of the same name:
 https://CRAN.R-project.org/package=stargazer
 
 @authors:
+    Pietro Battiston
+        me@pietrobattiston.it
+        https://pietrobattiston.it
     Matthew Burke:
         matthew.wesley.burke@gmail.com
         github.com/mwburke
 """
 
-from statsmodels.regression.linear_model import RegressionResultsWrapper
+from statsmodels.base.wrapper import ResultsWrapper
+from statsmodels.regression.linear_model import RegressionResults
 from math import sqrt
 from collections import defaultdict
 from enum import Enum
-
+import numbers
+import pandas as pd
 
 class LineLocation(Enum):
+    HEADER_TOP = 'ht'
+    HEADER_BOTTOM = 'hb'
     BODY_TOP = 'bt'
     BODY_BOTTOM = 'bb'
     FOOTER_TOP = 'ft'
-    FOOTER_BOOTM = 'fb'
+    FOOTER_BOTTOM = 'fb'
 
 
 class Stargazer:
     """
     Class that is constructed with one or more trained
     OLS models from the statsmodels package.
 
     The user then can change the rendering options by
     chaining different methods to the Stargazer object
     and then render the results in either HTML or LaTeX.
     """
 
+    # This is a mapping from 'show_*' attribute to name of generating method
+    # "_generate_{LABEL}" (if present) and to name of stat in data store
+    # otherwise.
+    # Stats will be automatically formatted. Order matters!
+    _auto_stats = [('n', 'nobs'),
+                   ('r2', 'r2'),
+                   ('adj_r2', 'r2_adj'),
+                   ('residual_std_err', 'resid_std_err'),
+                   ('f_statistic', 'f_statistic')]
+
     def __init__(self, models):
         self.models = models
         self.num_models = len(models)
         self.reset_params()
         self.extract_data()
 
     def validate_input(self):
@@ -45,15 +62,16 @@
         cause any problems further down the line.
 
         Any future checking will be added here.
         """
         targets = []
 
         for m in self.models:
-            if not isinstance(m, RegressionResultsWrapper):
+            if not isinstance(m, (ResultsWrapper,
+                                  RegressionResults)):
                 raise ValueError('Please use trained OLS models as inputs')
             targets.append(m.model.endog_names)
 
         if targets.count(targets[0]) != len(targets):
             self.dependent_variable = ''
             self.dep_var_name = None
         else:
@@ -65,20 +83,21 @@
         Run upon initialization but also allows the user to reset
         if they have made several changes and want to start fresh.
 
         Does not effect any of the underlying model data.
         """
         self.title_text = None
         self.show_header = True
-        self.dep_var_name = 'Dependent variable:'
+        self.dep_var_name = 'Dependent variable: '
         self.column_labels = None
         self.column_separators = None
         self.show_model_nums = True
         self.original_cov_names = None
         self.cov_map = None
+        self.cov_spacing = None
         self.show_precision = True
         self.show_sig = True
         self.sig_levels = [0.1, 0.05, 0.01]
         self.sig_digits = 3
         self.confidence_intervals = False
         self.show_footer = True
         self.custom_lines = defaultdict(list)
@@ -135,18 +154,30 @@
                            'f_statistic' : 'fvalue'
                            }
 
         data = {}
         for key, val in statsmodels_map.items():
             data[key] = self._extract_feature(model, val)
 
-        data['cov_names'] = model.params.index.values
+        if isinstance(model, ResultsWrapper):
+            data['cov_names'] = model.params.index.values
+        else:
+            # Simple RegressionResults, for instance as a result of
+            # get_robustcov_results():
+            data['cov_names'] = model.model.data.orig_exog.columns
+
+            # These are simple arrays, not Series:
+            for what in 'cov_values', 'p_values', 'cov_std_err':
+                data[what] = pd.Series(data[what],
+                                       index=data['cov_names'])
+
         data['conf_int_low_values'] = model.conf_int()[0]
         data['conf_int_high_values'] = model.conf_int()[1]
-        data['resid_std_err'] = sqrt(model.scale)
+        data['resid_std_err'] = (sqrt(sum(model.resid**2) / model.df_resid)
+                                 if hasattr(model, 'resid') else None)
 
         # Workaround for
         # https://github.com/statsmodels/statsmodels/issues/6778:
         if 'f_statistic' in data:
             data['f_statistic'] = (lambda x : x[0, 0] if getattr(x, 'ndim', 0)
                                    else x)(data['f_statistic'])
 
@@ -161,22 +192,37 @@
         self.header = show
 
     def show_model_numbers(self, show):
         assert type(show) == bool, 'Please input True/False'
         self.show_model_nums = show
 
     def custom_columns(self, labels, separators=None):
-        if separators is not None:
-            assert type(labels) == list, 'Please input a list of labels or a single label string'
-            assert type(separators) == list, 'Please input a list of column separators'
-            assert len(labels) == len(separators), 'Number of labels must match number of columns'
-            assert sum([int(type(s) != int) for s in separators]) == 0, 'Columns must be ints'
-            assert sum(separators) == self.num_models, 'Please set number of columns to number of models'
+        """
+        "labels": list of labels, or single label string.
+        "separators" (optional): list of integers, of same length of "labels",
+        indicating how many columns each header covers (default is 1).
+        """
+        if isinstance(labels, list):
+            if separators is None:
+                assert(len(labels) == self.num_models), ('If separators are '
+                'not provided, custom headers must be the same number as '
+                'models,')
+                separators = [1] * self.num_models
+            else:
+                assert type(separators) == list, ('Please input a list of '
+                                                  'column separators.')
+                assert len(labels) == len(separators), ('Number of labels '
+                                               'must match number of columns.')
+                assert(all(isinstance(s, int) for s in separators)), ('Column '
+                                                   'numbers must be integers.')
+                assert sum(separators) == self.num_models, ('Please set total '
+                                      'number of columns to number of models.')
         else:
-            assert type(labels) == str, 'Please input a single string label if no columns specified'
+            assert isinstance(labels, str), ('Please input a single string '
+                                             'label, or a list of strings.')
 
         self.column_labels = labels
         self.column_separators = separators
 
     def significance_levels(self, levels):
         assert len(levels) == 3, 'Please input 3 significance levels'
         assert sum([int(type(l) != float) for l in levels]) == 0, 'Please input floating point values as significance levels'
@@ -189,15 +235,15 @@
 
     def show_confidence_intervals(self, show):
         assert type(show) == bool, 'Please input True/False'
         self.confidence_intervals = show
 
     def dependent_variable_name(self, name):
         assert type(name) == str, 'Please input a string to use as the depedent variable name'
-        self.dep_var_name = name
+        self.dependent_variable = name
 
     def covariate_order(self, cov_names):
         missing = set(cov_names).difference(set(self.cov_names))
         assert not missing, ('Covariate order must contain subset of existing '
                              'covariates: {} are not.'.format(missing))
         self.original_cov_names = self.cov_names
         self.cov_names = cov_names
@@ -250,30 +296,48 @@
 
     def render_html(self, *args, **kwargs):
         return HTMLRenderer(self).render(*args, **kwargs)
 
     def _repr_html_(self):
         return self.render_html()
 
-    def render_latex(self, *args, **kwargs):
-        return LaTeXRenderer(self).render(*args, **kwargs)
+    def render_latex(self, *args, escape=False, **kwargs):
+        """
+        Render as LaTeX code.
+
+        Parameters
+        ----------
+        escape : bool
+            Escape special characters.
+
+        Returns
+        -------
+        str
+            The LaTeX code.
+        """
+        return LaTeXRenderer(self, escape=escape).render(*args, **kwargs)
 
 
 class Renderer:
     """
     Base class for renderers to specific formats. Only meant to be subclassed.
     """
-    def __init__(self, table):
+
+    # Formatters for stats which are not formatted via Renderer._float_format()
+    _formatters = {'nobs' : lambda x : str(int(x))}
+
+    def __init__(self, table, **kwargs):
         """
         Initialize a new renderer.
         
         "table": Stargazer object to render
         """
 
         self.table = table
+        self.kwargs = kwargs
 
     def __getattribute__(self, key):
         """
         Temporary fix while we better organize how a Stargazer table stores
         parameters: just retrieve them transparently as attributes of the
         Stargazer table object.
         """
@@ -294,27 +358,72 @@
         elif p_value >= self.sig_levels[1]:
             return sig_char
         elif p_value >= self.sig_levels[2]:
             return sig_char * 2
         else:
             return sig_char * 3
 
+    def _generate_cov_spacing(self):
+        if self.cov_spacing is None:
+            return None
+        if isinstance(self.cov_spacing, numbers.Number):
+            # A number is interpreted in "em" by default:
+            return f'{self.cov_spacing}em'
+        else:
+            return self.cov_spacing
+
     def _float_format(self, value):
         """
         Format value to string, using the precision set by the user.
         """
         if value is None:
             return ''
 
         return '{{:.{prec}f}}'.format(prec=self.sig_digits).format(value)
 
+    def _generate_resid_std_err(self, md):
+        rse = md['resid_std_err']
+        if rse is None:
+            return None
+
+        rse_text = self._float_format(rse)
+        if self.show_dof:
+            rse_text += ' (df={degree_freedom_resid:.0f})'.format(**md)
+        return rse_text
+
+    def _generate_f_statistic(self, md):
+        f_stat = md['f_statistic']
+        if f_stat is None:
+            return None
+
+        f_stars = self._format_sig_icon(md['f_p_value'])
+        f_text = f'{self._float_format(f_stat)}{f_stars}'
+        if self.show_dof:
+            f_text += (' (df={degree_freedom:.0f}; '
+                       '{degree_freedom_resid:.0f})').format(**md)
+
+        return f_text
+
+    def _generate_stat_values(self, stat):
+        if hasattr(self, f'_generate_{stat}'):
+            generator = getattr(self, f'_generate_{stat}')
+            return [generator(md) for md in self.model_data]
+        else:
+            return [md[stat] for md in self.model_data]
 
 class HTMLRenderer(Renderer):
     fmt = 'html'
 
+    # Labels for stats in Stargazer._auto_stats:
+    _stats_labels = {'n' : 'Observations',
+                     'r2' : 'R<sup>2</sup>',
+                     'adj_r2' : 'Adjusted R<sup>2</sup>',
+                     'residual_std_err' : 'Residual Std. Error',
+                     'f_statistic' : 'F Statistic'}
+
     def render(self):
         html = self.generate_header()
         html += self.generate_body()
         html += self.generate_footer()
         return html
 
     def generate_header(self):
@@ -323,14 +432,16 @@
             return header
 
         if self.title_text is not None:
             header += self.title_text + '<br>'
 
         header += '<table style="text-align:center"><tr><td colspan="'
         header += str(self.num_models + 1) + '" style="border-bottom: 1px solid black"></td></tr>'
+        header += self.generate_custom_lines(LineLocation.HEADER_TOP)
+
         if self.dep_var_name is not None:
             header += '<tr><td style="text-align:left"></td><td colspan="' + str(self.num_models)
             header += '"><em>' + self.dep_var_name + self.dependent_variable + '</em></td></tr>'
 
         header += '<tr><td style="text-align:left"></td>'
         if self.column_labels is not None:
             if type(self.column_labels) == str:
@@ -346,194 +457,204 @@
 
         if self.show_model_nums:
             header += '<tr><td style="text-align:left"></td>'
             for num in range(1, self.num_models + 1):
                 header += '<td>(' + str(num) + ')</td>'
             header += '</tr>'
 
+        header += self.generate_custom_lines(LineLocation.HEADER_BOTTOM)
+
         header += '<tr><td colspan="' + str(self.num_models + 1)
-        header += '" style="border-bottom: 1px solid black"></td></tr>'
+        header += '" style="border-bottom: 1px solid black"></td></tr>\n'
 
         return header
 
+    def _generate_cov_style(self):
+        if self.cov_spacing is None:
+            return ''
+        spacing = self._generate_cov_spacing()
+        return f' style="padding-bottom:{spacing}"'
+
+    def _format_sig_icon(self, pvalue):
+        return '<sup>' + str(self.get_sig_icon(pvalue)) + '</sup>'
+
     def generate_body(self):
         """
         Generate the body of the results where the
         covariate reporting is.
         """
+
+        spacing = self._generate_cov_style()
+
         body = ''
         body += self.generate_custom_lines(LineLocation.BODY_TOP)
         for cov_name in self.cov_names:
-            body += self.generate_cov_rows(cov_name)
+            body += self.generate_cov_rows(cov_name, spacing)
         body += self.generate_custom_lines(LineLocation.BODY_BOTTOM)
 
         return body
 
-    def generate_cov_rows(self, cov_name):
+    def generate_cov_rows(self, cov_name, spacing):
         cov_text = ''
-        cov_text += self.generate_cov_main(cov_name)
+        main_spacing = spacing if not self.show_precision else ''
+        cov_text += self.generate_cov_main(cov_name, spacing=main_spacing)
         if self.show_precision:
-            cov_text += self.generate_cov_precision(cov_name)
+            cov_text += self.generate_cov_precision(cov_name, spacing=spacing)
         else:
             cov_text += '<tr></tr>'
 
         return cov_text
 
-    def generate_cov_main(self, cov_name):
+    def generate_cov_main(self, cov_name, spacing):
         cov_print_name = cov_name
         if self.cov_map is not None:
             cov_print_name = self.cov_map.get(cov_print_name, cov_name)
-        cov_text = '<tr><td style="text-align:left">' + cov_print_name + '</td>'
+        cov_text = (f'<tr><td style="text-align:left">'
+                    f'{cov_print_name}</td>')
         for md in self.model_data:
             if cov_name in md['cov_names']:
-                cov_text += '<td>'
+                cov_text += f'<td{spacing}>'
                 cov_text += self._float_format(md['cov_values'][cov_name])
                 if self.show_sig:
-                    cov_text += '<sup>' + str(self.get_sig_icon(md['p_values'][cov_name])) + '</sup>'
+                    cov_text += self._format_sig_icon(md['p_values'][cov_name])
                 cov_text += '</td>'
             else:
-                cov_text += '<td></td>'
-        cov_text += '</tr>'
+                cov_text += f'<td{spacing}></td>'
+        cov_text += '</tr>\n'
 
         return cov_text
 
-    def generate_cov_precision(self, cov_name):
-        cov_text = '<tr><td style="text-align:left"></td>'
+    def generate_cov_precision(self, cov_name, spacing):
+        # This is the only place where we need to add spacing and there's a
+        # "style" already:
+        space_style = (f';padding-bottom:{self._generate_cov_spacing()}'
+                       if self.cov_spacing else '')
+        cov_text = f'<tr><td style="text-align:left{space_style}"></td>'
         for md in self.model_data:
             if cov_name in md['cov_names']:
-                cov_text += '<td>('
+                cov_text += f'<td{spacing}>('
                 if self.confidence_intervals:
                     cov_text += self._float_format(md['conf_int_low_values'][cov_name]) + ' , '
                     cov_text += self._float_format(md['conf_int_high_values'][cov_name])
                 else:
                     cov_text += self._float_format(md['cov_std_err'][cov_name])
                 cov_text += ')</td>'
             else:
-                cov_text += '<td></td>'
-        cov_text += '</tr>'
+                cov_text += f'<td{spacing}></td>'
+        cov_text += '</tr>\n'
 
         return cov_text
 
     def generate_footer(self):
         """
         Generate the footer of the table where
         model summary section is.
         """
         footer = '<td colspan="' + str(self.num_models + 1) + '" style="border-bottom: 1px solid black"></td></tr>'
 
         if not self.show_footer:
             return footer
         footer += self.generate_custom_lines(LineLocation.FOOTER_TOP)
-        if self.show_n:
-            footer += self.generate_observations()
-        if self.show_r2:
-            footer += self.generate_r2()
-        if self.show_adj_r2:
-            footer += self.generate_r2_adj()
-        if self.show_residual_std_err:
-            footer += self.generate_resid_std_err()
-        if self.show_f_statistic:
-            footer += self.generate_f_statistic()
-        footer += self.generate_custom_lines(LineLocation.FOOTER_BOOTM)
+
+        for attr, stat in Stargazer._auto_stats:
+            if getattr(self, f'show_{attr}'):
+                footer += self.generate_stat(stat, self._stats_labels[attr])
+
+        footer += self.generate_custom_lines(LineLocation.FOOTER_BOTTOM)
         footer += '<tr><td colspan="' + str(self.num_models + 1) + '" style="border-bottom: 1px solid black"></td></tr>'
         if self.show_notes:
             footer += self.generate_notes()
         footer += '</table>'
 
         return footer
 
     def generate_custom_lines(self, location):
-        custom_text = ''
+        custom_text = '\n'
         for custom_row in self.custom_lines[location]:
             custom_text += '<tr><td style="text-align: left">' + str(custom_row[0]) + '</td>'
             for custom_column in custom_row[1:]:
                 custom_text += '<td>' + str(custom_column) + '</td>'
             custom_text += '</tr>'
         return custom_text
 
-    def generate_observations(self):
-        obs_text = ''
-        obs_text += '<tr><td style="text-align: left">Observations</td>'
-        for md in self.model_data:
-            obs_text += '<td>{:,}</td>'.format(int(md['nobs']))
-        obs_text += '</tr>'
-        return obs_text
-
-    def generate_r2(self):
-        r2_text = ''
-        r2_text += '<tr><td style="text-align: left">R<sup>2</sup></td>'
-        for md in self.model_data:
-            r2_text += '<td>' + self._float_format(md['r2']) + '</td>'
-        r2_text += '</tr>'
-        return r2_text
-
-    def generate_r2_adj(self):
-        r2_text = ''
-        r2_text += '<tr><td style="text-align: left">Adjusted R<sup>2</sup></td>'
-        for md in self.model_data:
-            r2_text += '<td>' + self._float_format(md['r2_adj']) + '</td>'
-        r2_text += '</tr>'
-        return r2_text
-
-    def generate_resid_std_err(self):
-        rse_text = ''
-        rse_text += '<tr><td style="text-align: left">Residual Std. Error</td>'
-        for md in self.model_data:
-            rse_text += '<td>' + self._float_format(md['resid_std_err'])
-            if self.show_dof:
-                rse_text += ' (df={degree_freedom_resid:.0f})'.format(**md)
-            rse_text += '</td>'
-        rse_text += '</tr>'
-        return rse_text
+    def generate_stat(self, stat, label):
+        values = self._generate_stat_values(stat)
+        if not any(values):
+            return ''
 
-    def generate_f_statistic(self):
-        f_text = ''
-        f_text += '<tr><td style="text-align: left">F Statistic</td>'
-        for md in self.model_data:
-            f_text += '<td>' + self._float_format(md['f_statistic'])
-            f_text += '<sup>' + self.get_sig_icon(md['f_p_value']) + '</sup>'
-            if self.show_dof:
-                f_text += ' (df={degree_freedom:.0f}; {degree_freedom_resid:.0f})'.format(**md)
-            f_text += '</td>'
-        f_text += '</tr>'
-        return f_text
+        formatter = self._formatters.get(stat, self._float_format)
+
+        text = f'<tr><td style="text-align: left">{label}</td>'
+        for value in values:
+            if not isinstance(value, str):
+                value = formatter(value)
+            text += f'<td>{value}</td>'
+        text += '</tr>'
+        return text
 
     def generate_notes(self):
         notes_text = ''
         notes_text += '<tr><td style="text-align: left">' + self.notes_label + '</td>'
         if self.notes_append and self.show_stars:
             notes_text += self.generate_p_value_section()
         notes_text += '</tr>'
         notes_text += self.generate_additional_notes()
         return notes_text
 
     def generate_p_value_section(self):
-        notes_text = """
- <td colspan="{}" style="text-align: right">
-  <sup>*</sup>p&lt;{};
-  <sup>**</sup>p&lt;{};
-  <sup>***</sup>p&lt;{}
- </td>""".format(self.num_models, *self.sig_levels)
+        notes_text = f'<td colspan="{self.num_models}" style="text-align: right">'
+        pval_cells = [self._format_sig_icon(self.sig_levels[idx] - 0.001)
+                      + 'p&lt;' + str(self.sig_levels[idx]) for idx in range(3)]
+        notes_text += '; '.join(pval_cells)
+        notes_text += '</td>'
         return notes_text
 
     def generate_additional_notes(self):
         notes_text = ''
         if len(self.custom_notes) == 0:
             return notes_text
         i = 0
         for i, note in enumerate(self.custom_notes):
             if (i != 0) | (self.notes_append):
                 notes_text += '<tr>'
-            notes_text += '<td></td><td colspan="' + str(self.num_models) + '" style="text-align: right">' + note + '</td></tr>'
+            notes_text += '<td colspan="' + str(self.num_models+1) + '" style="text-align: right">' + note + '</td></tr>'
 
         return notes_text
 
 class LaTeXRenderer(Renderer):
     fmt = 'LaTeX'
 
+    # Labels for stats in Stargazer._auto_stats:
+    _stats_labels = {'n' : 'Observations',
+                     'r2' : '$R^2$',
+                     'adj_r2' : 'Adjusted $R^2$',
+                     'residual_std_err' : 'Residual Std. Error',
+                     'f_statistic' : 'F Statistic'}
+
+    # LaTeX escape characters, borrowed from pandas.io.formats.latex
+    _ESCAPE_CHARS = [
+        ('\\', r'\textbackslash '),
+        ('_', r'\_'),
+        ('%', r'\%'),
+        ('$', r'\$'),
+        ('#', r'\#'),
+        ('{', r'\{'),
+        ('}', r'\}'),
+        ('~', r'\textasciitilde '),
+        ('^', r'\textasciicircum '),
+        ('&', r'\&')
+    ]
+
+    def _escape(self, text):
+        """Escape LaTeX special characters"""
+        if self.kwargs.get('escape', False):
+            for orig_char, escape_char in LaTeXRenderer._ESCAPE_CHARS:
+                text = text.replace(orig_char, escape_char)
+        return text
+
     def render(self, only_tabular=False, insert_empty_rows=False):
         latex = self.generate_header(only_tabular=only_tabular)
         latex += self.generate_body(insert_empty_rows=insert_empty_rows)
         latex += self.generate_footer(only_tabular=only_tabular)
 
         return latex
 
@@ -550,50 +671,67 @@
             if self.table_label is not None:
                 header += '  \\label{' + self.table_label + '}\n'
 
         content_columns = 'c' * self.num_models
         header += '\\begin{tabular}{@{\\extracolsep{5pt}}l' + content_columns + '}\n'
         header += '\\\\[-1.8ex]\\hline\n'
         header += '\\hline \\\\[-1.8ex]\n'
+        header += self.generate_custom_lines(LineLocation.HEADER_TOP)
+
         if self.dep_var_name is not None:
             header += '& \\multicolumn{' + str(self.num_models) + '}{c}'
-            header += '{\\textit{' + self.dep_var_name + '}} \\\n'
-            header += '\\cr \\cline{' + str(self.num_models) + '-' + str(self.num_models + 1) + '}\n'
+            header += '{\\textit{' + self.dep_var_name + self.dependent_variable + '}} \\\n'
+            header += '\\cr \\cline{2-' + str(self.num_models + 1) + '}\n'
 
         if self.column_labels is not None:
             if type(self.column_labels) == str:
-                header += '\\\\[-1.8ex] & \\multicolumn{' + str(self.num_models) + '}{c}{' + self.column_labels + '} \\\\'
+                header += '\\\\[-1.8ex] & \\multicolumn{' + str(self.num_models) + '}{c}{' + self._escape(self.column_labels) + '} \\\\'
             else:
                 header += '\\\\[-1.8ex] '
                 for i, label in enumerate(self.column_labels):
                     header += '& \\multicolumn{' + str(self.column_separators[i])
-                    header += '}{c}{' + label + '} '
+                    header += '}{c}{' + self._escape(label) + '} '
                 header += ' \\\\\n'
 
         if self.show_model_nums:
             header += '\\\\[-1.8ex] '
             for num in range(1, self.num_models + 1):
                 header += '& (' + str(num) + ') '
             header += '\\\\\n'
 
+        header += self.generate_custom_lines(LineLocation.HEADER_BOTTOM)
+
         header += '\\hline \\\\[-1.8ex]\n'
 
         return header
 
+    def _generate_cov_end(self):
+        if self.cov_spacing is None:
+            return '\\\\\n'
+        spacing = self._generate_cov_spacing()
+        return f'\\\\[{spacing}]\n'
+
+    def _format_sig_icon(self, pvalue):
+        return '$^{' + str(self.get_sig_icon(pvalue)) + '}$'
+
     def generate_body(self, insert_empty_rows=False):
         """
         Generate the body of the results where the
         covariate reporting is.
         """
         body = ''
         body += self.generate_custom_lines(LineLocation.BODY_TOP)
+
+        cov_end = self._generate_cov_end()
+
         for cov_name in self.cov_names:
             body += self.generate_cov_rows(cov_name)
             if insert_empty_rows:
-                body += '  ' + '& '*len(self.num_models) + '\\\\\n'
+                body += '\\\\\n  ' + '& '*len(self.num_models)
+            body += cov_end
         body += self.generate_custom_lines(LineLocation.BODY_BOTTOM)
 
         return body
 
     def generate_cov_rows(self, cov_name):
         cov_text = ''
         cov_text += self.generate_cov_main(cov_name)
@@ -607,67 +745,60 @@
     def generate_cov_main(self, cov_name):
         cov_print_name = cov_name
 
         if self.cov_map is not None:
             if cov_name in self.cov_map:
                 cov_print_name = self.cov_map[cov_name]
 
-        cov_text = ' ' + cov_print_name + ' '
+        cov_text = ' ' + self._escape(cov_print_name) + ' '
         for md in self.model_data:
             if cov_name in md['cov_names']:
                 cov_text += '& ' + self._float_format(md['cov_values'][cov_name])
                 if self.show_sig:
-                    cov_text += '$^{' + str(self.get_sig_icon(md['p_values'][cov_name])) + '}$'
+                    cov_text += self._format_sig_icon(md['p_values'][cov_name])
                 cov_text += ' '
             else:
                 cov_text += '& '
-        cov_text += '\\\\\n'
 
         return cov_text
 
     def generate_cov_precision(self, cov_name):
-        cov_text = '  '
+        cov_text = '\\\\\n'
 
         for md in self.model_data:
             if cov_name in md['cov_names']:
                 cov_text += '& ('
                 if self.confidence_intervals:
                     cov_text += self._float_format(md['conf_int_low_values'][cov_name]) + ' , '
                     cov_text += self._float_format(md['conf_int_high_values'][cov_name])
                 else:
                     cov_text += self._float_format(md['cov_std_err'][cov_name])
                 cov_text += ') '
             else:
                 cov_text += '& '
-        cov_text += '\\\\\n'
 
         return cov_text
 
     def generate_footer(self, only_tabular=False):
         """
         Generate the footer of the table where
         model summary section is.
         """
 
         footer = '\\hline \\\\[-1.8ex]\n'
 
         if not self.show_footer:
             return footer
         footer += self.generate_custom_lines(LineLocation.FOOTER_TOP)
-        if self.show_n:
-            footer += self.generate_observations()
-        if self.show_r2:
-            footer += self.generate_r2()
-        if self.show_adj_r2:
-            footer += self.generate_r2_adj()
-        if self.show_residual_std_err:
-            footer += self.generate_resid_std_err()
-        if self.show_f_statistic:
-            footer += self.generate_f_statistic()
-        footer += self.generate_custom_lines(LineLocation.FOOTER_BOOTM)
+
+        for attr, stat in Stargazer._auto_stats:
+            if getattr(self, f'show_{attr}'):
+                footer += self.generate_stat(stat, self._stats_labels[attr])
+
+        footer += self.generate_custom_lines(LineLocation.FOOTER_BOTTOM)
         footer += '\\hline\n\\hline \\\\[-1.8ex]\n'
         if self.show_notes:
             footer += self.generate_notes()
         footer += '\\end{tabular}'
 
         if not only_tabular:
             footer += '\n\\end{table}'
@@ -679,79 +810,50 @@
         for custom_row in self.custom_lines[location]:
             custom_text += ' ' + str(custom_row[0]) + ' '
             for custom_column in custom_row[1:]:
                 custom_text += '& ' + str(custom_column) + ' '
             custom_text += '\\\\\n'
         return custom_text
 
-    def generate_observations(self):
-        obs_text = ''
-        obs_text += ' Observations '
-        for md in self.model_data:
-            obs_text += '& {:,} '.format(int(md['nobs']))
-        obs_text += '\\\\\n'
-        return obs_text
-
-    def generate_r2(self):
-        r2_text = ' $R^2$ '
-        for md in self.model_data:
-            r2_text += '& ' + self._float_format(md['r2']) + ' '
-        r2_text += '\\\\\n'
-        return r2_text
+    def generate_stat(self, stat, label):
+        values = self._generate_stat_values(stat)
+        if not any(values):
+            return ''
 
-    def generate_r2_adj(self):
-        r2_text = ' Adjusted $R^2$ '
-        for md in self.model_data:
-            r2_text += '& ' + self._float_format(md['r2_adj']) + ' '
-        r2_text += '\\\\\n'
-        return r2_text
-
-    def generate_resid_std_err(self):
-        rse_text = ''
-        rse_text += ' Residual Std. Error '
-        for md in self.model_data:
-            rse_text += '& ' + self._float_format(md['resid_std_err'])
-            if self.show_dof:
-                rse_text += '(df = {:d})'.format(int(md['degree_freedom_resid']))
-            rse_text += ' '
-        rse_text += ' \\\\\n'
-        return rse_text
+        formatter = self._formatters.get(stat, self._float_format)
 
-    def generate_f_statistic(self):
-        f_text = ''
-        f_text += ' F Statistic '
-        for md in self.model_data:
-            f_text += '& ' + self._float_format(md['f_statistic'])
-            f_text += '$^{' + self.get_sig_icon(md['f_p_value']) + '}$ '
-            if self.show_dof:
-                f_text += '(df = ' + str(md['degree_freedom']) + '; ' + str(md['degree_freedom_resid']) + ')'
-            f_text += ' '
-        f_text += '\\\\\n'
-        return f_text
+        text = f' {label} '
+        for value in values:
+            if not isinstance(value, str):
+                value = formatter(value)
+            text += f'& {value} '
+        text += '\\\\\n'
+        return text
 
     def generate_notes(self):
         notes_text = ''
         notes_text += '\\textit{' + self.notes_label + '}'
         if self.notes_append and self.show_stars:
             notes_text += self.generate_p_value_section()
         notes_text += self.generate_additional_notes()
         return notes_text
 
     def generate_p_value_section(self):
-        notes_text = ''
-        notes_text += ' & \\multicolumn{' + str(self.num_models) + '}{r}{$^{' + self.get_sig_icon(self.sig_levels[0] - 0.001) + '}$p$<$' + str(self.sig_levels[0]) + '; '
-        notes_text += '$^{' + self.get_sig_icon(self.sig_levels[1] - 0.001) + '}$p$<$' + str(self.sig_levels[1]) + '; '
-        notes_text += '$^{' + self.get_sig_icon(self.sig_levels[2] - 0.001) + '}$p$<$' + str(self.sig_levels[2]) + '} \\\\\n'
+        notes_text = ' & \\multicolumn{' + str(self.num_models) + '}{r}{'
+        pval_cells = [self._format_sig_icon(self.sig_levels[idx] - 0.001)
+                      + 'p$<$' + str(self.sig_levels[idx]) for idx in range(3)]
+        notes_text += '; '.join(pval_cells)
+        notes_text += '} \\\\\n'
         return notes_text
 
     def generate_additional_notes(self):
         notes_text = ''
         # if len(self.custom_notes) == 0:
         #     return notes_text
         for note in self.custom_notes:
             # if (i != 0) | (self.notes_append):
             #     notes_text += '\\multicolumn{' + str(self.num_models) + '}{r}\\textit{' + note + '} \\\\\n'
             # else:
             #     notes_text += ' & \\multicolumn{' + str(self.num_models) + '}{r}\\textit{' + note + '} \\\\\n'
-            notes_text += ' & \\multicolumn{' + str(self.num_models) + '}{r}\\textit{' + note + '} \\\\\n'
+            notes_text += '\\multicolumn{' + str(self.num_models+1) + '}{r}\\textit{' + self._escape(note) + '} \\\\\n'
 
         return notes_text
```

### Comparing `stargazer-0.0.5/stargazer.egg-info/PKG-INFO` & `stargazer-0.0.6/stargazer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,110 @@
 Metadata-Version: 2.1
 Name: stargazer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Nicely formatted regression reporting
-Home-page: https://github.com/mwburke/stargazer
-Author: Matthew Burke
-Author-email: matthew.wesley.burke@gmail.com
+Home-page: https://github.com/StatsReporting/stargazer
+Author: Pietro Battiston, Matthew Burke
+Author-email: me@pietrobattiston.it, matthew.wesley.burke@gmail.com
 License: GPLv2
-Description: # Stargazer
-        
-        This is a python port of the R stargazer package that can be found [on CRAN](https://CRAN.R-project.org/package=stargazer). I was disappointed that there wasn't equivalent functionality in any python packages I was aware of so I'm re-implementing it here.
-        
-        There is an experimental function in the [statsmodels.regression.linear_model.OLSResults.summary2](http://www.statsmodels.org/dev/generated/statsmodels.regression.linear_model.OLSResults.summary2.html) that can report single regression model results in HTML/CSV/LaTeX/etc, but it still didn't quite fulfill what I was looking for.
-        
-        The python package is object oriented now with chained commands to make changes to the rendering parameters, which is hopefully more pythonic and the user doesn't have to put a bunch of arguments in a single function.
-        
-        ## Installation
-        
-        You can install this package through PyPi with `pip install stargazer` or just clone the repo and take the `stargazer.py` file since it's the only one in the package.
-        
-        ### Dependencies
-        
-        It depends on `statsmodels`, which in turn depends on several other libraries like `pandas`, `numpy`, etc
-        
-        ## Editing Features
-        
-        This library implements many of the customization features found in the original package. Examples of most can be found [in the examples jupyter notebook](https://github.com/mwburke/stargazer/blob/master/examples.ipynb) and a full list of the methods/features is here below:
-        
-        * `title`: custom title
-        * `show_header`: display or hide model header data
-        * `show_model_numbers`: display or hide model numbers
-        * `custom_columns`: custom model names and model groupings
-        * `significance_levels`: change statistical significance thresholds
-        * `significant_digits`: change number of significant digits
-        * `show_confidence_intervals`: display confidence intervals instead of variance
-        * `dependent_variable_name`: rename dependent variable
-        * `rename_covariates`: rename covariates
-        * `covariate_order`: reorder covariates
-        * `reset_covariate_order`: reset covariate order to original ordering
-        * `show_degrees_of_freedom`: display or hide degrees of freedom
-        * `custom_note_label`: label notes section at bottom of table
-        * `add_custom_notes`: add custom notes to section at bottom of the table
-        * `add_line`: add a custom line to the table
-        * `append_notes`: display or hide statistical significance thresholds
-        
-        These features are agnostic of the rendering type and will be applied whether the user outputs in HTML, LaTeX, etc
-        
-        ## Example
-        
-        Here is an examples of how to quickly get started with the library. More examples can be found in the `examples.ipynb` file in the github repo. The examples all use the scikit-learn diabetes dataset, but it is not a dependency for the package.
-        
-        ### OLS Models Preparation
-        
-        ```python
-        import pandas as pd
-        from sklearn import datasets
-        import statsmodels.api as sm
-        from stargazer.stargazer import Stargazer
-        
-        diabetes = datasets.load_diabetes()
-        df = pd.DataFrame(diabetes.data)
-        df.columns = ['Age', 'Sex', 'BMI', 'ABP', 'S1', 'S2', 'S3', 'S4', 'S5', 'S6']
-        df['target'] = diabetes.target
-        
-        est = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:4]])).fit()
-        est2 = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:6]])).fit()
-        
-        
-        stargazer = Stargazer([est, est2])
-        ```
-        
-        ### HTML Example
-        
-        ```python
-        stargazer.render_html()
-        ```
-        
-        <table style="text-align:center"><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><td style="text-align:left"></td><td colspan="2"><em>Dependent variable:</em></td></tr><tr><td style="text-align:left"><tr><td style="text-align:left"></td><td>(1)</td><td>(2)</td></tr><td colspan="3" style="border-bottom: 1px solid black"><tr><td style="text-align:left">ABP</td><td>416.674<sup>***</sup></td><td>397.583<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(69.495)</td><td>(70.87)</td></tr><tr><td style="text-align:left">Age</td><td>37.241<sup></sup></td><td>24.704<sup></sup></td></tr><tr><td style="text-align:left"></td><td>(64.117)</td><td>(65.411)</td></tr><tr><td style="text-align:left">BMI</td><td>787.179<sup>***</sup></td><td>789.742<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(65.424)</td><td>(66.887)</td></tr><tr><td style="text-align:left">S1</td><td></td><td>197.852<sup></sup></td></tr><tr><td style="text-align:left"></td><td></td><td>(143.812)</td></tr><tr><td style="text-align:left">S2</td><td></td><td>-169.251<sup></sup></td></tr><tr><td style="text-align:left"></td><td></td><td>(142.744)</td></tr><tr><td style="text-align:left">Sex</td><td>-106.578<sup>*</sup></td><td>-82.862<sup></sup></td></tr><tr><td style="text-align:left"></td><td>(62.125)</td><td>(64.851)</td></tr><tr><td style="text-align:left">const</td><td>152.133<sup>***</sup></td><td>152.133<sup>***</sup></td></tr><tr><td style="text-align:left"></td><td>(2.853)</td><td>(2.853)</td></tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Observations</td><td>442.0</td><td>442.0</td></tr><tr><td style="text-align: left">R<sup>2</sup></td><td>0.4</td><td>0.403</td></tr><tr><td style="text-align: left">Adjusted R<sup>2</sup></td><td>0.395</td><td>0.395</td></tr><tr><td style="text-align: left">Residual Std. Error</td><td>59.976(df = 437.0)</td><td>59.982(df = 435.0)</td></tr><tr><td style="text-align: left">F Statistic</td><td>72.913<sup>***</sup>(df = 4.0; 437.0)</td><td>48.915<sup>***</sup>(df = 6.0; 435.0)</td></tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Note:</td><td colspan="2" style="text-align: right"><em>p<0.1</em>; <b>p<0.05</b>; p<0.01</td></tr></table>
-        
-        ### LaTeX Example
-        
-        ```python
-        stargazer.render_latex()
-        ```
-        
-        ![](https://raw.githubusercontent.com/mwburke/stargazer/master/latex_example.png)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Stargazer
+
+This is a python port of the R stargazer package that can be found [on CRAN](https://CRAN.R-project.org/package=stargazer). I was disappointed that there wasn't equivalent functionality in any python packages I was aware of so I'm re-implementing it here.
+
+There is an experimental function in the [statsmodels.regression.linear_model.OLSResults.summary2](http://www.statsmodels.org/dev/generated/statsmodels.regression.linear_model.OLSResults.summary2.html) that can report single regression model results in HTML/CSV/LaTeX/etc, but it still didn't quite fulfill what I was looking for.
+
+The python package is object oriented now with chained commands to make changes to the rendering parameters, which is hopefully more pythonic and the user doesn't have to put a bunch of arguments in a single function.
+
+## Installation
+
+You can install this package through PyPi with `pip install stargazer` or just clone the repo and take the `stargazer.py` file since it's the only one in the package.
+
+### Dependencies
+
+It depends on `statsmodels`, which in turn depends on several other libraries like `pandas`, `numpy`, etc
+
+## Editing Features
+
+This library implements many of the customization features found in the original package. Examples of most can be found [in the examples jupyter notebook](https://github.com/StatsReporting/stargazer/blob/master/examples.ipynb) and a full list of the methods/features is here below:
+
+* `title`: custom title
+* `show_header`: display or hide model header data
+* `show_model_numbers`: display or hide model numbers
+* `custom_columns`: custom model names and model groupings
+* `significance_levels`: change statistical significance thresholds
+* `significant_digits`: change number of significant digits
+* `show_confidence_intervals`: display confidence intervals instead of variance
+* `dependent_variable_name`: rename dependent variable
+* `rename_covariates`: rename covariates
+* `covariate_order`: reorder covariates
+* `reset_covariate_order`: reset covariate order to original ordering
+* `show_degrees_of_freedom`: display or hide degrees of freedom
+* `custom_note_label`: label notes section at bottom of table
+* `add_custom_notes`: add custom notes to section at bottom of the table
+* `add_line`: add a custom line to the table
+* `append_notes`: display or hide statistical significance thresholds
+
+These features are agnostic of the rendering type and will be applied whether the user outputs in HTML, LaTeX, etc
+
+## Example
+
+Here is an examples of how to quickly get started with the library. More examples can be found in the `examples.ipynb` file in the github repo. The examples all use the scikit-learn diabetes dataset, but it is not a dependency for the package.
+
+### OLS Models Preparation
+
+```python
+import pandas as pd
+from sklearn import datasets
+import statsmodels.api as sm
+from stargazer.stargazer import Stargazer
+
+diabetes = datasets.load_diabetes()
+df = pd.DataFrame(diabetes.data)
+df.columns = ['Age', 'Sex', 'BMI', 'ABP', 'S1', 'S2', 'S3', 'S4', 'S5', 'S6']
+df['target'] = diabetes.target
+
+est = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:4]])).fit()
+est2 = sm.OLS(endog=df['target'], exog=sm.add_constant(df[df.columns[0:6]])).fit()
+
+
+stargazer = Stargazer([est, est2])
+```
+
+### HTML Example
+
+```python
+stargazer.render_html()
+```
+
+<table style="text-align:center"><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left"></td><td colspan="2"><em>Dependent variable: target</em></td></tr><tr><td style="text-align:left"></td><tr><td style="text-align:left"></td><td>(1)</td><td>(2)</td></tr><tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr>
+
+<tr><td style="text-align:left">ABP</td><td>416.674<sup>***</sup></td><td>397.583<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(69.495)</td><td>(70.870)</td></tr>
+<tr><td style="text-align:left">Age</td><td>37.241<sup></sup></td><td>24.704<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td>(64.117)</td><td>(65.411)</td></tr>
+<tr><td style="text-align:left">BMI</td><td>787.179<sup>***</sup></td><td>789.742<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(65.424)</td><td>(66.887)</td></tr>
+<tr><td style="text-align:left">S1</td><td></td><td>197.852<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td></td><td>(143.812)</td></tr>
+<tr><td style="text-align:left">S2</td><td></td><td>-169.251<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td></td><td>(142.744)</td></tr>
+<tr><td style="text-align:left">Sex</td><td>-106.578<sup>*</sup></td><td>-82.862<sup></sup></td></tr>
+<tr><td style="text-align:left"></td><td>(62.125)</td><td>(64.851)</td></tr>
+<tr><td style="text-align:left">const</td><td>152.133<sup>***</sup></td><td>152.133<sup>***</sup></td></tr>
+<tr><td style="text-align:left"></td><td>(2.853)</td><td>(2.853)</td></tr>
+
+<td colspan="3" style="border-bottom: 1px solid black"></td></tr>
+<tr><td style="text-align: left">Observations</td><td>442</td><td>442</td></tr><tr><td style="text-align: left">R<sup>2</sup></td><td>0.400</td><td>0.403</td></tr><tr><td style="text-align: left">Adjusted R<sup>2</sup></td><td>0.395</td><td>0.395</td></tr><tr><td style="text-align: left">Residual Std. Error</td><td>59.976 (df=437)</td><td>59.982 (df=435)</td></tr><tr><td style="text-align: left">F Statistic</td><td>72.913<sup>***</sup> (df=4; 437)</td><td>48.915<sup>***</sup> (df=6; 435)</td></tr>
+<tr><td colspan="3" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align: left">Note:</td><td colspan="2" style="text-align: right"><sup>*</sup>p&lt;0.1; <sup>**</sup>p&lt;0.05; <sup>***</sup>p&lt;0.01</td></tr></table>
+
+### LaTeX Example
+
+```python
+stargazer.render_latex()
+```
+
+![](https://raw.githubusercontent.com/StatsReporting/stargazer/master/latex_example.png)
```

