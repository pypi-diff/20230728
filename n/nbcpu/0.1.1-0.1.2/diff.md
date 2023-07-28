# Comparing `tmp/nbcpu-0.1.1.tar.gz` & `tmp/nbcpu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbcpu-0.1.1.tar", max compression
+gzip compressed data, was "nbcpu-0.1.2.tar", max compression
```

## Comparing `nbcpu-0.1.1.tar` & `nbcpu-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-06-28 05:12:47.521733 nbcpu-0.1.1/LICENSE
--rw-r--r--   0        0        0     3320 2023-06-28 05:12:47.521733 nbcpu-0.1.1/README.md
--rw-r--r--   0        0        0     2997 2023-06-28 05:13:13.625833 nbcpu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      286 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/__cli__.py
--rw-r--r--   0        0        0      379 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/__init__.py
--rw-r--r--   0        0        0       22 2023-06-28 05:13:13.585832 nbcpu-0.1.1/src/nbcpu/_version.py
--rw-r--r--   0        0        0        0 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/__init__.py
--rw-r--r--   0        0        0      325 2023-06-28 05:13:13.585832 nbcpu-0.1.1/src/nbcpu/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/path/__init__.yaml
--rw-r--r--   0        0        0      412 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/path/__task__.yaml
--rw-r--r--   0        0        0       76 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       72 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       74 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0      119 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      237 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      242 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       92 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       19 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      742 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/project/__init__.yaml
--rw-r--r--   0        0        0      168 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/project/__test__.yaml
--rw-r--r--   0        0        0       36 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/running/__init__.yaml
--rw-r--r--   0        0        0      176 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      319 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/task/__init__.yaml
--rw-r--r--   0        0        0      311 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/task/__test__.yaml
--rw-r--r--   0        0        0       97 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       97 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-06-28 05:12:47.525733 nbcpu-0.1.1/src/nbcpu/py.typed
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 nbcpu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-28 08:30:10.267032 nbcpu-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-28 08:30:10.267032 nbcpu-0.1.2/README.md
+-rw-r--r--   0        0        0     2921 2023-07-28 08:30:44.039374 nbcpu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-07-28 08:30:10.267032 nbcpu-0.1.2/src/nbcpu/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-28 08:30:10.267032 nbcpu-0.1.2/src/nbcpu/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-28 08:30:43.971373 nbcpu-0.1.2/src/nbcpu/_version.py
+-rw-r--r--   0        0        0        0 2023-07-28 08:30:10.267032 nbcpu-0.1.2/src/nbcpu/conf/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-28 08:30:10.267032 nbcpu-0.1.2/src/nbcpu/conf/about/nbcpu.yaml
+-rw-r--r--   0        0        0        0 2023-07-28 08:30:10.267032 nbcpu-0.1.2/src/nbcpu/py.typed
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 nbcpu-0.1.2/PKG-INFO
```

### Comparing `nbcpu-0.1.1/LICENSE` & `nbcpu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nbcpu-0.1.1/README.md` & `nbcpu-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 [version-image]: https://img.shields.io/github/v/release/entelecheia/nbcpu?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/nbcpu
 [release-url]: https://github.com/entelecheia/nbcpu/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
 
 [repo-url]: https://github.com/entelecheia/nbcpu
 [pypi-url]: https://pypi.org/project/nbcpu
-[docs-url]: https://entelecheia.github.io/nbcpu
+[docs-url]: https://nbcpu.entelecheia.ai
 [changelog]: https://github.com/entelecheia/nbcpu/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/nbcpu/blob/main/CONTRIBUTING.md
 <!-- Links: -->
 
 Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach
 
-- Documentation: [https://entelecheia.github.io/nbcpu][docs-url]
+- Documentation: [https://nbcpu.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/nbcpu][repo-url]
 - PyPI: [https://pypi.org/project/nbcpu][pypi-url]
 
 Understanding and measuring central bank policy uncertainty are fundamental to predicting economic outcomes, particularly in economies like Cambodia where the monetary policy tools are underdeveloped and the economy is heavily dollarized. This study aims to develop and evaluate topic-based measures of policy uncertainty in the Cambodian context, using narrative text data derived from major news media outlets. Leveraging Latent Dirichlet Allocation (LDA), a widely-used generative model for text data, we estimate the document-topic and topic-word distributions from a corpus of news articles, thereby deriving measures of policy uncertainty.
 
 Our methodology involves applying two topic models: one classifies articles into four categories of interest - Exchange Rate Policy Uncertainty, Currency Stabilization Policy Uncertainty, De-dollarization Policy Uncertainty, and International Monetary Policy Impact Uncertainty; the other quantifies the intensity of uncertainty within these articles. We use a seed word approach to guide the LDA in determining relevant topics and the level of associated uncertainty.
```

### Comparing `nbcpu-0.1.1/pyproject.toml` & `nbcpu-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nbcpu"
-version = "0.1.1"
+version = "0.1.2"
 description = "Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/nbcpu"
 repository = "https://github.com/entelecheia/nbcpu"
 readme = "README.md"
 packages = [{ include = "nbcpu", from = "src" }]
 
 [tool.poetry.scripts]
 nbcpu = 'nbcpu.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^0.15.0"
+hyfi = "^1.12.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
@@ -83,15 +83,14 @@
 name = "cz_conventional_commits"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/nbcpu/_version.py:__version__"
-version_pattern = 'src/nbcpu/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
```

### Comparing `nbcpu-0.1.1/PKG-INFO` & `nbcpu-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nbcpu
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach
 Home-page: https://entelecheia.github.io/nbcpu
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=0.15.0,<0.16.0)
+Requires-Dist: hyfi (>=1.12.1,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/nbcpu
 Description-Content-Type: text/markdown
 
 # Measuring Central Bank Policy Uncertainty
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
@@ -35,22 +35,22 @@
 [version-image]: https://img.shields.io/github/v/release/entelecheia/nbcpu?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/nbcpu
 [release-url]: https://github.com/entelecheia/nbcpu/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
 
 [repo-url]: https://github.com/entelecheia/nbcpu
 [pypi-url]: https://pypi.org/project/nbcpu
-[docs-url]: https://entelecheia.github.io/nbcpu
+[docs-url]: https://nbcpu.entelecheia.ai
 [changelog]: https://github.com/entelecheia/nbcpu/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/nbcpu/blob/main/CONTRIBUTING.md
 <!-- Links: -->
 
 Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach
 
-- Documentation: [https://entelecheia.github.io/nbcpu][docs-url]
+- Documentation: [https://nbcpu.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/nbcpu][repo-url]
 - PyPI: [https://pypi.org/project/nbcpu][pypi-url]
 
 Understanding and measuring central bank policy uncertainty are fundamental to predicting economic outcomes, particularly in economies like Cambodia where the monetary policy tools are underdeveloped and the economy is heavily dollarized. This study aims to develop and evaluate topic-based measures of policy uncertainty in the Cambodian context, using narrative text data derived from major news media outlets. Leveraging Latent Dirichlet Allocation (LDA), a widely-used generative model for text data, we estimate the document-topic and topic-word distributions from a corpus of news articles, thereby deriving measures of policy uncertainty.
 
 Our methodology involves applying two topic models: one classifies articles into four categories of interest - Exchange Rate Policy Uncertainty, Currency Stabilization Policy Uncertainty, De-dollarization Policy Uncertainty, and International Monetary Policy Impact Uncertainty; the other quantifies the intensity of uncertainty within these articles. We use a seed word approach to guide the LDA in determining relevant topics and the level of associated uncertainty.
```

