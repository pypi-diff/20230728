# Comparing `tmp/autoray-0.6.5.tar.gz` & `tmp/autoray-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoray-0.6.5.tar", last modified: Tue Jul 25 23:31:39 2023, max compression
+gzip compressed data, was "autoray-0.6.6.tar", last modified: Thu Jul 27 23:00:32 2023, max compression
```

## Comparing `autoray-0.6.5.tar` & `autoray-0.6.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 23:31:18.000000 autoray-0.6.5/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 23:31:18.000000 autoray-0.6.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.157408 autoray-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-25 23:31:18.000000 autoray-0.6.5/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 23:31:18.000000 autoray-0.6.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-25 23:31:18.000000 autoray-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 23:31:18.000000 autoray-0.6.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-25 23:31:18.000000 autoray-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 23:31:18.000000 autoray-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 23:31:39.169408 autoray-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-07-25 23:31:18.000000 autoray-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/autoray/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    60207 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/autoray.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/autoray/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/experimental/complexity_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)  1265159 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/experimental/complexity_tracing_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/autoray/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48582 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/autoray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.157408 autoray-0.6.5/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-jax.yml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-tensorflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-torch.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/docs/_pygments/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_pygments/_pygments_dark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_pygments/_pygments_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_static/autoray-header.png
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_static/my-styles.css
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/automatic_dispatch.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/compilation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57965 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/images/autoray-readme-pic-0.png
--rw-r--r--   0 runner    (1001) docker     (123)    99582 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/images/autoray-readme-pic-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)   608532 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/lazy_computation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 23:31:18.000000 autoray-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:31:39.169408 autoray-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-25 23:31:18.000000 autoray-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/test_autocompile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/test_autoray.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/test_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.245405 autoray-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 23:00:11.000000 autoray-0.6.6/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 23:00:11.000000 autoray-0.6.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.229404 autoray-0.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.233404 autoray-0.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-27 23:00:11.000000 autoray-0.6.6/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-27 23:00:11.000000 autoray-0.6.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-27 23:00:11.000000 autoray-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 23:00:11.000000 autoray-0.6.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-27 23:00:11.000000 autoray-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 23:00:11.000000 autoray-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18398 2023-07-27 23:00:32.245405 autoray-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-07-27 23:00:11.000000 autoray-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.237404 autoray-0.6.6/autoray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 23:00:32.000000 autoray-0.6.6/autoray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60212 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/autoray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.237404 autoray-0.6.6/autoray/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/experimental/complexity_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1265159 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/experimental/complexity_tracing_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.237404 autoray-0.6.6/autoray/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49489 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/lazy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25851 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/lazy/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-27 23:00:11.000000 autoray-0.6.6/autoray/lazy/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.237404 autoray-0.6.6/autoray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18398 2023-07-27 23:00:32.000000 autoray-0.6.6/autoray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-27 23:00:32.000000 autoray-0.6.6/autoray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:00:32.000000 autoray-0.6.6/autoray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 23:00:32.000000 autoray-0.6.6/autoray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 23:00:32.000000 autoray-0.6.6/autoray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.233404 autoray-0.6.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.241405 autoray-0.6.6/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-27 23:00:11.000000 autoray-0.6.6/ci/requirements/py-base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 23:00:11.000000 autoray-0.6.6/ci/requirements/py-jax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 23:00:11.000000 autoray-0.6.6/ci/requirements/py-tensorflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-27 23:00:11.000000 autoray-0.6.6/ci/requirements/py-torch.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.241405 autoray-0.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.241405 autoray-0.6.6/docs/_pygments/
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/_pygments/_pygments_dark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/_pygments/_pygments_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.241405 autoray-0.6.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/_static/autoray-header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/_static/my-styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/automatic_dispatch.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/compilation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.241405 autoray-0.6.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57965 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/images/autoray-readme-pic-0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99582 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/images/autoray-readme-pic-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)   782774 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/lazy_computation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-27 23:00:11.000000 autoray-0.6.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-27 23:00:11.000000 autoray-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:00:32.245405 autoray-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-27 23:00:11.000000 autoray-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:32.245405 autoray-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:11.000000 autoray-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-27 23:00:11.000000 autoray-0.6.6/tests/test_autocompile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-07-27 23:00:11.000000 autoray-0.6.6/tests/test_autoray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-27 23:00:11.000000 autoray-0.6.6/tests/test_lazy.py
```

### Comparing `autoray-0.6.5/.github/workflows/pypi-release.yml` & `autoray-0.6.6/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/.github/workflows/tests.yml` & `autoray-0.6.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/.gitignore` & `autoray-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/LICENSE` & `autoray-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/PKG-INFO` & `autoray-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoray
-Version: 0.6.5
+Version: 0.6.6
 Summary: Abstract your array operations.
 Home-page: http://github.com/jcmgray/autoray
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/autoray/issues
 Project-URL: Source, https://github.com/jcmgray/autoray/
@@ -271,15 +271,15 @@
 #  'conj': 10}
 
 # --> the largest array encountered
 ly.history_max_size()
 # 25
 
 # --> traverse the unique computational nodes, e.g. to estimate FLOP cost
-len([node for node in ly])
+len([node for node in ly.descend()])
 # 57
 
 # --> traverse in topological/computational order
 len([node for node in ly.ascend()])
 # 57
 
 # --> plot the full computation as a circuit
@@ -313,15 +313,15 @@
 If the computation might involve repeated computations then you can call it in a ``shared_intermediates`` context:
 
 ```python
 with lazy.shared_intermediates():
     ly = modified_gram_schmidt(lx)
 
 # --> a few nodes can be reused here (c.f. 57 previously)
-len(tuple(ly))
+ly.history_num_nodes()
 # 51
 ```
 this caches the computational nodes as they are created based on a hash of their input arguments (note this uses ``id`` for array like things, i.e. assumes they are immutable). Unlike eagerly caching function calls in real time, which might consume large amounts of memory, now when the computation runs (i.e. ``ly.compute()`` is called) data is only kept as long as its needed.
 
 **Why not use e.g. ``dask``?**
 
  There are many reasons to use [dask](https://dask.org/), but it incurs a pretty large overhead for big computational graphs with comparatively small operations. Calling and computing the ``modified_gram_schmidt`` function for a 100x100 matrix (20,102 computational nodes) with ``dask.array`` takes ~25sec whereas with ``lazy.array`` it takes ~0.25sec:
```

### Comparing `autoray-0.6.5/README.md` & `autoray-0.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 #  'conj': 10}
 
 # --> the largest array encountered
 ly.history_max_size()
 # 25
 
 # --> traverse the unique computational nodes, e.g. to estimate FLOP cost
-len([node for node in ly])
+len([node for node in ly.descend()])
 # 57
 
 # --> traverse in topological/computational order
 len([node for node in ly.ascend()])
 # 57
 
 # --> plot the full computation as a circuit
@@ -289,15 +289,15 @@
 If the computation might involve repeated computations then you can call it in a ``shared_intermediates`` context:
 
 ```python
 with lazy.shared_intermediates():
     ly = modified_gram_schmidt(lx)
 
 # --> a few nodes can be reused here (c.f. 57 previously)
-len(tuple(ly))
+ly.history_num_nodes()
 # 51
 ```
 this caches the computational nodes as they are created based on a hash of their input arguments (note this uses ``id`` for array like things, i.e. assumes they are immutable). Unlike eagerly caching function calls in real time, which might consume large amounts of memory, now when the computation runs (i.e. ``ly.compute()`` is called) data is only kept as long as its needed.
 
 **Why not use e.g. ``dask``?**
 
  There are many reasons to use [dask](https://dask.org/), but it incurs a pretty large overhead for big computational graphs with comparatively small operations. Calling and computing the ``modified_gram_schmidt`` function for a 100x100 matrix (20,102 computational nodes) with ``dask.array`` takes ~25sec whereas with ``lazy.array`` it takes ~0.25sec:
```

### Comparing `autoray-0.6.5/autoray/__init__.py` & `autoray-0.6.6/autoray/__init__.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/autoray/autoray.py` & `autoray-0.6.6/autoray/autoray.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,15 +692,15 @@
     ----------
     tree : pytree
         A nested sequence of tuples, lists, dicts and other objects.
     is_leaf : callable
         A function to determine if an object is a leaf, only objects for which
         ``is_leaf(x)`` returns ``True`` are returned in the flattened list.
     get_ref : bool
-        If ``True``, a reference tree is returned which can be used to
+        If ``True``, a reference tree is also returned which can be used to
         reconstruct the original tree from a flattened list.
 
     Returns
     -------
     objs : list
         The flattened list of leaf objects.
     (ref_tree) : pytree
```

### Comparing `autoray-0.6.5/autoray/compiler.py` & `autoray-0.6.6/autoray/compiler.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/autoray/experimental/complexity_tracing.py` & `autoray-0.6.6/autoray/experimental/complexity_tracing.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/autoray/experimental/complexity_tracing_example.ipynb` & `autoray-0.6.6/autoray/experimental/complexity_tracing_example.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/autoray/lazy/__init__.py` & `autoray-0.6.6/autoray/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/autoray/lazy/core.py` & `autoray-0.6.6/autoray/lazy/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,49 +10,67 @@
     astype,
     get_dtype_name,
     get_lib_fn,
     infer_backend,
     multi_class_priorities,
     register_backend,
     register_function,
+    tree_flatten,
+    tree_map,
+    tree_iter,
+    tree_unflatten,
 )
 from .draw import (
     plot_graph,
     plot_circuit,
     plot_history_size_footprint,
     plot_history_functions,
     plot_history_stats,
 )
 
 
 _EMPTY_DICT = {}
 get_depth = operator.attrgetter("_depth")
+get_data = operator.attrgetter("_data")
 
 
 # ------------------------ traversal and computation ------------------------ #
 
 
+def is_lazy_array(x):
+    """Check if ``x`` is a lazy array."""
+    return isinstance(x, LazyArray)
+
+
+def to_queue(lz):
+    """Parse a pytree of lazy arrays into a queue of nodes, sorted by depth.
+    This is useful for traversing the computational graph of multiple outputs
+    in topological order.
+    """
+    if isinstance(lz, LazyArray):
+        return [lz]
+    queue = tree_flatten(lz, is_lazy_array)
+    queue.sort(key=get_depth)
+    return queue
+
+
 def descend(lz):
     """Generate each unique computational node. Use ``ascend`` if you need to
     visit children before parents.
 
     Parameters
     ----------
-    lz : LazyArray or sequence of LazyArray
+    lz : pytree of LazyArray
         The output node(s) of the computational graph to descend.
 
     Yields
     ------
     LazyArray
     """
-    if isinstance(lz, LazyArray):
-        queue = [lz]
-    else:
-        queue = sorted(lz, key=get_depth)
-
+    queue = to_queue(lz)
     seen = set()
     while queue:
         node = queue.pop()
         nid = id(node)
         if nid not in seen:
             yield node
             queue.extend(node._deps)
@@ -62,26 +80,22 @@
 def ascend(lz):
     """Generate each unique computational node, from leaves to root. I.e. a
     topological ordering of the computational graph. Moreover, the nodes
     are visited 'deepest first'.
 
     Parameters
     ----------
-    lz : LazyArray or sequence of LazyArray
+    lz : pytree of LazyArray
         The output node(s) of the computational graph to ascend to.
 
     Yields
     ------
     LazyArray
     """
-    if isinstance(lz, LazyArray):
-        queue = [lz]
-    else:
-        queue = sorted(lz, key=get_depth)
-
+    queue = to_queue(lz)
     seen = set()
     ready = set()
     while queue:
         node = queue[-1]
         need_to_visit = [c for c in node._deps if id(c) not in ready]
         if need_to_visit:
             need_to_visit.sort(key=get_depth)
@@ -98,47 +112,40 @@
 def compute(lz):
     """Compute the value of one or more lazy arrays. All nodes that are
     computed clear any references to their function, arguments and
     dependencies, and store the result in their ``_data`` attribute.
 
     Parameters
     ----------
-    lz : LazyArray or sequence of LazyArray
+    lz : pytree of LazyArray
         The output node(s) of the computational graph to compute.
 
     Returns
     -------
     array or tuple of array
         The computed value(s) of the lazy array(s).
     """
     for node in ascend(lz):
         node._materialize()
-
-    if isinstance(lz, LazyArray):
-        return lz._data
-
-    return tuple(node._data for node in lz)
+    return tree_map(get_data, lz, is_lazy_array)
 
 
 def compute_constants(lz, variables):
     """Fold constant arrays - everything not dependent on ``variables`` -
     into the graph.
 
     Parameters
     ----------
-    lz : LazyArray or sequence of LazyArray
+    lz : pytree of LazyArray
         The output node(s) of the computational graph.
-    variables : LazyArray or sequence of LazyArray
+    variables : pytree of LazyArray
         Nodes that should be treated as variable. I.e. any descendants will
         not be folded into the graph.
     """
-    if isinstance(variables, LazyArray):
-        variables = {variables}
-    else:
-        variables = set(variables)
+    variables = set(tree_iter(variables, is_lazy_array))
 
     # must ascend
     for node in ascend(lz):
         if not any(c in variables for c in node._deps):
             # can fold
             node._materialize()
         else:
@@ -197,117 +204,94 @@
     computational graph corresponding to ``inputs`` -> ``outputs``. The
     signature of the function is ``func(input_arrays) -> output_arrays``. As an
     intermediate step, the computational graph is traced to a flattened source
     code string.
 
     Parameters
     ----------
-    inputs : LazyArray or sequence of LazyArray
+    inputs : pytree of LazyArray
         The input node(s) of the computational graph.
-    outputs : LazyArray or sequence of LazyArray
+    outputs : pytree of LazyArray
         The output node(s) of the computational graph.
     fold_constants : bool, optional
         If True, fold constant arrays (those with no dependence on ``inputs``)
         into the graph ahead of compile.
 
     See Also
     --------
     get_source, compute
     """
 
     __slots__ = (
         "_in_names",
         "_out_names",
+        "_out_tree",
         "_source",
         "_code",
-        "_params",
-        "_is_single_in",
-        "_is_single_out",
+        "_locals",
     )
 
     def __init__(self, inputs, outputs, fold_constants=True):
         if fold_constants:
             # compute everything not dependent on inputs
             compute_constants(outputs, variables=inputs)
 
-        # write source and populate locals mapping that function will run under
-        # params will include the functions and other constant objects
-        self._params = {}
-        self._source = get_source(outputs, params=self._params)
+        # write source and populate locals mapping that function will run
+        # under, locals will include the functions and other constant objects
+        self._locals = {}
+        self._source = get_source(outputs, params=self._locals)
 
         # compile source
         self._code = compile(
             source=self._source,
             filename="<string>",
             mode="exec",
             optimize=1,
         )
 
         # get names to inject and extract arrays into and from locals
-        self._is_single_in = isinstance(inputs, LazyArray)
-        if self._is_single_in:
-            self._in_names = f"x{id(inputs)}"
-        else:
-            self._in_names = tuple(f"x{id(v)}" for v in inputs)
-
-        self._is_single_out = isinstance(outputs, LazyArray)
-        if self._is_single_out:
-            self._out_names = f"x{id(outputs)}"
-        else:
-            self._out_names = tuple(f"x{id(v)}" for v in outputs)
-
-    def __call__(self, arrays, *args):
-
-        # allow fn(arrays) or fn(*arrays)
-        if args:
-            arrays = (arrays,) + args
-
-        # inject the new array(s)
-        if self._is_single_in:
-            self._params[self._in_names] = arrays
-        else:
-            for name, array in zip(self._in_names, arrays):
-                self._params[name] = array
+        self._in_names = tuple(f"x{id(v)}" for v in tree_iter(inputs))
+        outs_flat, self._out_tree = tree_flatten(outputs, get_ref=True)
+        self._out_names = tuple(f"x{id(v)}" for v in outs_flat)
+
+    def __call__(self, *args):
+        # this allows any matching zipped tree
+        for name, array in zip(self._in_names, tree_iter(args)):
+            self._locals[name] = array
 
         # run the byte-compiled function with the updated locals
-        exec(self._code, None, self._params)
+        exec(self._code, None, self._locals)
 
-        if self._is_single_in:
-            # remove the input array(s) from the locals
-            del self._params[self._in_names]
-        else:
-            for name in self._in_names:
-                del self._params[name]
+        # remove inputs from locals
+        for name in self._in_names:
+            del self._locals[name]
 
-        if self._is_single_out:
-            # return the result, whilst removing it from the locals
-            return self._params.pop(self._out_names)
+        # pop outputs from locals
+        outs = tuple(self._locals.pop(name) for name in self._out_names)
 
-        # return the results, whilst removing them from the locals
-        return tuple(self._params.pop(name) for name in self._out_names)
+        # return the outputs in the original tree structure
+        return tree_unflatten(outs, self._out_tree)
 
     def __getstate__(self):
         # can't pickle the code object -> recompile in setstate
         return (
             self._in_names,
             self._out_names,
+            self._out_tree,
             self._source,
-            self._params,
-            self._is_single_in,
-            self._is_single_out,
+            self._locals,
         )
 
     def __setstate__(self, state):
         (
             self._in_names,
             self._out_names,
+            self._out_tree,
             self._source,
-            self._params,
-            self._is_single_in,
-            self._is_single_out,
+            self._locals,
         ) = state
 
         # recompile the source
         self._code = compile(
             source=self._source,
             filename="<string>",
             mode="exec",
@@ -315,33 +299,24 @@
         )
 
     def print_source(self):
         """Print the source code of the compiled function."""
         print(self._source)
 
     def __repr__(self):
-        if self._is_single_in:
-            insig = "array_like"
-        else:
-            insig = "Sequence[array_like]"
-
-        if self._is_single_out:
-            outsig = "array_like"
-        else:
-            outsig = "Tuple[array_like]"
-
+        insig = f"{len(self._in_names)} input(s)"
+        outsig = f"{len(self._out_names)} output(s) "
         return f"<Function({insig}) -> {outsig}>"
 
 
 # --------------------------- computational nodes --------------------------- #
 
 
 class Placeholder:
-    """A singleton object to use as a placeholder in a LazyArray.
-    """
+    """A singleton object to use as a placeholder in a LazyArray."""
 
     __slots__ = ()
 
     def __repr__(self):
         return "Placeholder"
 
 
@@ -484,15 +459,15 @@
 
             # free any references to deps
             self._fn = self._args = self._kwargs = None
             self._deps = ()
 
         return self._data
 
-    __iter__ = descend = descend
+    descend = descend
     ascend = ascend
 
     def compute(self):
         """Compute the value of this lazy array, clearing any references to the
         function, arguments and dependencies, and storing the result in the
         ``_data`` attribute as well as returning it.
 
@@ -594,49 +569,78 @@
 
             if len(columns) < max_depth:
                 deps = sorted(t.deps, key=get_depth, reverse=True)
                 islasts = [True] + [False] * (len(deps) - 1)
                 for islast, d in zip(islasts, deps):
                     queue.append((d, columns + (islast,)))
 
+    def history_num_nodes(self):
+        """Return the number of unique computational nodes in the history of
+        this ``LazyArray``.
+        """
+        num_nodes = 0
+        for _ in self.descend():
+            num_nodes += 1
+        return num_nodes
+
     def history_max_size(self):
         """Get the largest single tensor size appearing in this computation."""
-        return max(node.size for node in self)
+        return max(node.size for node in self.descend())
 
-    def history_size_footprint(self):
+    def history_size_footprint(self, include_inputs=True):
         """Get the combined size of intermediates at each step of the
         computation. Note this assumes that intermediates are immediately
         garbage collected when they are no longer required.
+
+        Parameters
+        ----------
+        include_inputs : bool, optional
+            Whether to include the size of the inputs in the computation. If
+            ``True`` It is assumed they can be garbage collected once used but
+            are all present at the beginning of the computation.
         """
         delete_checked = set()
         sizes = []
+        input_size = 0
         for node in reversed(tuple(self.ascend())):
             for c in node._deps:
                 if c not in delete_checked:
                     # last time a dependency is seen, subtract the size
-                    if c._deps:
+                    if include_inputs or c._deps:
                         sizes.append(-c.size)
                     delete_checked.add(c)
 
             if node._data is None:
                 # this is a new intermediate, add the size
                 sizes.append(+node.size)
+            elif include_inputs:
+                # this is an input, size is added at beginning
+                input_size += node.size
 
+        sizes.append(input_size)
         sizes.reverse()
         return list(itertools.accumulate(sizes))
 
-    def history_peak_size(self):
-        """Get the peak combined intermediate size of this computation."""
-        return max(self.history_size_footprint())
+    def history_peak_size(self, include_inputs=True):
+        """Get the peak combined intermediate size of this computation.
+
+        Parameters
+        ----------
+        include_inputs : bool, optional
+            Whether to include the size of the inputs in the computation. If
+            ``True`` It is assumed they can be garbage collected once used but
+            are all present at the beginning of the computation.
+        """
+        return max(self.history_size_footprint(include_inputs=include_inputs))
 
     def history_total_size(self):
         """The the total size of all unique arrays in the computational graph,
         possibly relevant e.g. for back-propagation algorithms.
         """
-        return sum(node.size for node in self)
+        return sum(node.size for node in self.descend())
 
     def history_stats(self, fn):
         """Compute aggregate statistics about the computational graph.
 
         Parameters
         ----------
         fn : callable or str
@@ -663,15 +667,15 @@
 
             elif fn == "sizeout":
 
                 def fn(node):
                     return node.size
 
         stats = collections.defaultdict(int)
-        for node in self:
+        for node in self.descend():
             node_cost = fn(node)
             if node_cost is not None:
                 stats[node.fn_name] += fn(node)
 
         return dict(stats)
 
     def history_fn_frequencies(self):
@@ -754,14 +758,28 @@
         """
         return self._kwargs
 
     @property
     def shape(self):
         return self._shape
 
+    def __len__(self):
+        return self.shape[0]
+
+    def __iter__(self):
+        import warnings
+
+        warnings.warn(
+            "Iterating over LazyArray to get the computational graph nodes is "
+            "deprecated - use `LazyArray.descend()` instead. Eventually "
+            "`iter(lz)` will iterate over first axis slices."
+        )
+
+        return self.descend()
+
     @property
     def ndim(self):
         return len(self._shape)
 
     @property
     def size(self):
         return functools.reduce(operator.mul, self.shape, 1)
@@ -1285,29 +1303,27 @@
 
     adv_idx_shape = adv_idx_loc = None
     adv_idx_locs = []
 
     shape = iter(a.shape)
     newshape = []
     for i, k in enumerate(key):
-
         if k is None:
             # (newaxis) -> new dimension of size 1
             newshape.append(1)
             # don't want to iterate shape
             continue
 
         d = next(shape)
 
         if isinstance(k, slice):
             # range of values
             newshape.append(get_sliced_size(d, k.start, k.stop, k.step))
 
         elif hasattr(k, "shape") or isinstance(k, (tuple, list)):
-
             if adv_idx_shape is None:
                 # first advanced index
                 adv_idx_shape = _get_py_shape(k)
                 adv_idx_loc = len(newshape)
                 adv_idx_locs.append(i)
             else:
                 # check if broadcast shape matches
@@ -1333,15 +1349,15 @@
             # 'move to front' advanced indexing
             newshape = (*adv_idx_shape, *newshape)
         else:
             # 'keep in place' advanced indexing
             newshape = (
                 *newshape[:adv_idx_loc],
                 *adv_idx_shape,
-                *newshape[adv_idx_loc:]
+                *newshape[adv_idx_loc:],
             )
     else:
         newshape = tuple(newshape)
 
     return a.to(operator.getitem, (a, key), shape=newshape, deps=deps)
 
 
@@ -1429,36 +1445,38 @@
     backend = find_common_backend(x1, x2)
 
     shape1 = shape(x1)
     shape2 = shape(x2)
     if len(shape2) == 1:
         if shape1[-1] != shape2[-1]:
             raise ValueError(
-                'matmul: Input operand 1 has a mismatch in its core dimension 0, '
-                'with gufunc signature (n?,k),(k,m?)->(n?,m?)'
+                "matmul: Input operand 1 has a mismatch in its core dimension "
+                "0, with gufunc signature (n?,k),(k,m?)->(n?,m?)"
             )
         newshape = shape1[:-1]
     elif len(shape1) == 1:
         if len(shape2) > 2 or shape1[-1] != shape2[-2]:
             raise ValueError(
-                'matmul: Input operand 1 has a mismatch in its core dimension 0, '
-                'with gufunc signature (n?,k),(k,m?)->(n?,m?)'
+                "matmul: Input operand 1 has a mismatch in its core dimension "
+                "0, with gufunc signature (n?,k),(k,m?)->(n?,m?)"
             )
         newshape = shape2[-1:]
     else:
         if shape2[:-2] != shape1[:-2]:
             raise ValueError(
-                'operands could not be broadcast together with remapped shapes '
-                f'[original->remapped]: {shape1}->({shape1[:-2]},newaxis,newaxis) '
-                f'{shape2}->({shape2[:-2]},newaxis,newaxis)  and requested shape ({shape1[-2], shape2[-1]})'
+                "operands could not be broadcast together with remapped "
+                f"shapes [original->remapped]: {shape1}->({shape1[:-2]},"
+                "newaxis,newaxis) "
+                f"{shape2}->({shape2[:-2]},newaxis,newaxis)  and requested "
+                f"shape ({shape1[-2], shape2[-1]})"
             )
         if shape1[-1] != shape2[-2]:
             raise ValueError(
-                'matmul: Input operand 1 has a mismatch in its core dimension 0, '
-                'with gufunc signature (n?,k),(k,m?)->(n?,m?)'
+                "matmul: Input operand 1 has a mismatch in its core dimension "
+                "0, with gufunc signature (n?,k),(k,m?)->(n?,m?)"
             )
         newshape = (*shape1[:-1], shape2[-1])
 
     return LazyArray(
         backend=backend,
         fn=operator.matmul,
         args=(x1, x2),
```

### Comparing `autoray-0.6.5/autoray/lazy/draw.py` & `autoray-0.6.6/autoray/lazy/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Visualizations for ``LazyArray`` computational graphs.
 """
 
 import itertools
 import functools
-import importlib
+import importlib.util
 
 
 COLORING_SEED = 1  # 8, 10
 
 
 def set_coloring_seed(seed):
     """Set the seed for the random color generator.
```

### Comparing `autoray-0.6.5/autoray/lazy/linalg.py` & `autoray-0.6.6/autoray/lazy/linalg.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/autoray.egg-info/PKG-INFO` & `autoray-0.6.6/autoray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoray
-Version: 0.6.5
+Version: 0.6.6
 Summary: Abstract your array operations.
 Home-page: http://github.com/jcmgray/autoray
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/autoray/issues
 Project-URL: Source, https://github.com/jcmgray/autoray/
@@ -271,15 +271,15 @@
 #  'conj': 10}
 
 # --> the largest array encountered
 ly.history_max_size()
 # 25
 
 # --> traverse the unique computational nodes, e.g. to estimate FLOP cost
-len([node for node in ly])
+len([node for node in ly.descend()])
 # 57
 
 # --> traverse in topological/computational order
 len([node for node in ly.ascend()])
 # 57
 
 # --> plot the full computation as a circuit
@@ -313,15 +313,15 @@
 If the computation might involve repeated computations then you can call it in a ``shared_intermediates`` context:
 
 ```python
 with lazy.shared_intermediates():
     ly = modified_gram_schmidt(lx)
 
 # --> a few nodes can be reused here (c.f. 57 previously)
-len(tuple(ly))
+ly.history_num_nodes()
 # 51
 ```
 this caches the computational nodes as they are created based on a hash of their input arguments (note this uses ``id`` for array like things, i.e. assumes they are immutable). Unlike eagerly caching function calls in real time, which might consume large amounts of memory, now when the computation runs (i.e. ``ly.compute()`` is called) data is only kept as long as its needed.
 
 **Why not use e.g. ``dask``?**
 
  There are many reasons to use [dask](https://dask.org/), but it incurs a pretty large overhead for big computational graphs with comparatively small operations. Calling and computing the ``modified_gram_schmidt`` function for a 100x100 matrix (20,102 computational nodes) with ``dask.array`` takes ~25sec whereas with ``lazy.array`` it takes ~0.25sec:
```

### Comparing `autoray-0.6.5/autoray.egg-info/SOURCES.txt` & `autoray-0.6.6/autoray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/Makefile` & `autoray-0.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/_pygments/_pygments_dark.py` & `autoray-0.6.6/docs/_pygments/_pygments_dark.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/_pygments/_pygments_light.py` & `autoray-0.6.6/docs/_pygments/_pygments_light.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/_static/autoray-header.png` & `autoray-0.6.6/docs/_static/autoray-header.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/_static/my-styles.css` & `autoray-0.6.6/docs/_static/my-styles.css`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/automatic_dispatch.md` & `autoray-0.6.6/docs/automatic_dispatch.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/compilation.ipynb` & `autoray-0.6.6/docs/compilation.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/conf.py` & `autoray-0.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/images/autoray-readme-pic-0.png` & `autoray-0.6.6/docs/images/autoray-readme-pic-0.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/images/autoray-readme-pic-1.png` & `autoray-0.6.6/docs/images/autoray-readme-pic-1.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/index.md` & `autoray-0.6.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/installation.md` & `autoray-0.6.6/docs/installation.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/docs/make.bat` & `autoray-0.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/pyproject.toml` & `autoray-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/setup.py` & `autoray-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/tests/test_autocompile.py` & `autoray-0.6.6/tests/test_autocompile.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.5/tests/test_autoray.py` & `autoray-0.6.6/tests/test_autoray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import importlib
+import importlib.util
 
 import pytest
 
 import autoray as ar
 from autoray import shape
```

### Comparing `autoray-0.6.5/tests/test_lazy.py` & `autoray-0.6.6/tests/test_lazy.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         assert infer_backend(data) == larray.backend
         return data
 
     return checked
 
 
 def make_strict(larray):
-    for node in larray:
+    for node in larray.descend():
         larray._fn = wrap_strict_check(larray)
 
 
 @pytest.mark.parametrize("backend", BACKENDS)
 def test_lazy_mgs(backend):
     if backend == "sparse":
         pytest.xfail("Sparse doesn't support 'linalg.norm' yet...")
@@ -84,22 +84,22 @@
     )
     assert isinstance(ly, lazy.LazyArray)
     hmax = ly.history_max_size()
     hpeak = ly.history_peak_size()
     htot = ly.history_total_size()
     assert hmax == 25
     assert 25 < hpeak < htot
-    assert len(tuple(ly)) == 57
-    assert len({node.fn_name for node in ly}) == 9
+    assert ly.history_num_nodes() == 57
+    assert len(ly.history_fn_frequencies()) == 9
     assert_allclose(to_numpy(ly.compute()), to_numpy(modified_gram_schmidt(x)))
     with lazy.shared_intermediates():
         ly = modified_gram_schmidt(lx)
         make_strict(ly)
-    assert len(tuple(ly)) == 51
-    assert len({node.fn_name for node in ly}) == 9
+    assert ly.history_num_nodes() == 51
+    assert len(ly.history_fn_frequencies()) == 9
     assert_allclose(to_numpy(ly.compute()), to_numpy(modified_gram_schmidt(x)))
 
 
 def test_partial_evaluation():
     la = lazy.array(gen_rand((10, 10), "numpy"))
     lb = lazy.array(gen_rand((10, 10), "numpy"))
     lc = lazy.array(gen_rand((10, 10), "numpy"))
@@ -107,18 +107,18 @@
     lab = do("tanh", la @ lb)
     lcd = lc @ ld
     ls = lab + lcd
     ld = do("abs", lab / lcd)
     le = do("einsum", "ab,ba->a", ls, ld)
     lf = do("sum", le)
     make_strict(lf)
-    assert len(tuple(lf)) == 12
+    assert lf.history_num_nodes() == 12
     lf.compute_constants(variables=[lc, ld])  # constants = [la, lb]
-    assert len(tuple(lf)) == 9
-    assert "tanh" not in {node.fn_name for node in lf}
+    assert lf.history_num_nodes() == 9
+    assert "tanh" not in {node.fn_name for node in lf.descend()}
     lf.compute()
 
 
 def test_history_fn_frequencies():
     la = lazy.array(gen_rand((10, 10), "numpy"))
     lb = lazy.array(gen_rand((10, 10), "numpy"))
     lc = lazy.array(gen_rand((10, 10), "numpy"))
@@ -168,52 +168,52 @@
 
 def test_share_intermediates():
     la = lazy.array(gen_rand((10, 10), "numpy"))
     lb = lazy.array(gen_rand((10, 10), "numpy"))
     l1 = do("tanh", la @ lb)
     l2 = do("tanh", la @ lb)
     ly = l1 + l2
-    assert len(tuple(ly)) == 7
+    assert ly.history_num_nodes() == 7
     y1 = ly.compute()
     with lazy.shared_intermediates():
         l1 = do("tanh", la @ lb)
         l2 = do("tanh", la @ lb)
         ly = l1 + l2
-    assert len(tuple(ly)) == 5
+    assert ly.history_num_nodes() == 5
     y2 = ly.compute()
     assert_allclose(y1, y2)
 
 
 @pytest.mark.parametrize("backend", BACKENDS)
 def test_transpose_chain(backend):
     lx = lazy.array(gen_rand((2, 3, 4, 5, 6), backend))
     l1 = do("transpose", lx, (1, 0, 3, 2, 4))
     l2 = do("transpose", l1, (1, 0, 3, 2, 4))
     assert l2.args[0] is lx
     assert l2.deps == (lx,)
-    assert len(tuple(l1)) == 2
-    assert len(tuple(l2)) == 2
+    assert l1.history_num_nodes() == 2
+    assert l2.history_num_nodes() == 2
     assert_allclose(
         to_numpy(lx.compute()),
         to_numpy(l2.compute()),
     )
 
 
 @pytest.mark.parametrize("backend", BACKENDS)
 def test_reshape_chain(backend):
     lx = lazy.array(gen_rand((2, 3, 4, 5, 6), backend))
     l1 = do("reshape", lx, (6, 4, 30))
     l2 = do("reshape", l1, (-1,))
-    assert len(tuple(l1)) == 2
-    assert len(tuple(l2)) == 2
+    assert l1.history_num_nodes() == 2
+    assert l2.history_num_nodes() == 2
     assert l2.args[0] is lx
     assert l2.deps == (lx,)
     assert_allclose(
         to_numpy(lx.compute()).flatten(),
-        to_numpy(l2.compute()),
+        to_numpy(l2.compute()), atol=1e-6,
     )
 
 
 @pytest.mark.parametrize("backend", BACKENDS)
 @pytest.mark.parametrize("dtype", ["float64", "complex128"])
 def test_svd(backend, dtype):
     if backend == "sparse":
@@ -484,18 +484,39 @@
 def test_where():
     a = lazy.Variable(shape=(4,), backend="numpy")
     b = lazy.Variable(shape=(4,), backend="numpy")
     c = do("where", *(a > 0, b, 1))
     f = c.get_function([a, b])
     x = do("asarray", [-0.5, -0.5, 1, 2], like="numpy")
     y = do("asarray", [1, 2, 3, 4], like="numpy")
-    z = f([x, y])
+    z = f(x, y)
     assert_allclose(z, [1, 1, 3, 4])
 
 
+def test_lazy_function_pytree_input_and_output():
+    inputs = {
+        'a': lazy.Variable(shape=(2, 3), backend="numpy"),
+        'b': lazy.Variable(shape=(3, 4), backend="numpy"),
+    }
+    outputs = {
+        'outa': do("tanh", inputs['a'] @ inputs['b']),
+        'outb': [inputs['a'] - 1, inputs['b'] - 1],
+    }
+    f = lazy.Function(inputs, outputs)
+
+    a = do("random.uniform", size=(2, 3), like="numpy")
+    b = do("random.uniform", size=(3, 4), like="numpy")
+
+    outs = f({'a': a, 'b': b})
+
+    assert_allclose(outs['outa'], do("tanh", a @ b))
+    assert_allclose(outs['outb'][0], a - 1)
+    assert_allclose(outs['outb'][1], b - 1)
+
+
 @pytest.mark.parametrize(
     "indices",
     [
         [0, 1],
         [[0, 1], [1, 2]],
         [[[0, 1], [1, 2]], [[1, 1], [2, 2]]],
         [[[[0, 1, 2, 3]]]],
```

