# Comparing `tmp/mscales-1.3.6.tar.gz` & `tmp/mscales-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscales-1.3.6.tar", last modified: Wed Jul 12 11:03:35 2023, max compression
+gzip compressed data, was "mscales-1.4.0.tar", last modified: Fri Jul 28 16:49:54 2023, max compression
```

## Comparing `mscales-1.3.6.tar` & `mscales-1.4.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.6/AUTHORS.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.6/CONTRIBUTING.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.6/LICENSE
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.6/MANIFEST.in
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 11:03:35.284790 mscales-1.3.6/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      953 2023-07-05 10:34:36.000000 mscales-1.3.6/README.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/docs/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/Makefile
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/make.bat
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/docs/source/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-07-05 10:34:36.000000 mscales-1.3.6/docs/source/conf.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/index.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/pcsets.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/quickstart.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1422 2023-07-12 11:01:23.000000 mscales-1.3.6/docs/source/release-history.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.6/docs/source/scales.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales/_version.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/concepts.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    10724 2023-07-12 11:00:53.000000 mscales-1.3.6/mscales/pcsets.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/plots.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/scales.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/sound.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales/tests/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/tests/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/tests/conftest.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/tests/test_examples.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.6/mscales/utils.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-12 11:03:35.284790 mscales-1.3.6/mscales.egg-info/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1408 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/SOURCES.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/dependency_links.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/requires.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-12 11:03:35.000000 mscales-1.3.6/mscales.egg-info/top_level.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.6/pyproject.toml
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.6/requirements.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-12 11:03:35.284790 mscales-1.3.6/setup.cfg
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.3.6/setup.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.6/versioneer.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.4.0/AUTHORS.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.4.0/LICENSE
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.4.0/MANIFEST.in
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1430 2023-07-28 16:49:54.902812 mscales-1.4.0/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      975 2023-07-28 16:41:27.000000 mscales-1.4.0/README.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.898811 mscales-1.4.0/docs/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      655 2023-07-12 14:02:42.000000 mscales-1.4.0/docs/Makefile
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      779 2023-07-12 14:02:42.000000 mscales-1.4.0/docs/make.bat
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.898811 mscales-1.4.0/docs/source/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3574 2023-07-28 16:23:15.000000 mscales-1.4.0/docs/source/basic.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7379 2023-07-13 12:17:47.000000 mscales-1.4.0/docs/source/conf.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      418 2023-07-12 14:46:17.000000 mscales-1.4.0/docs/source/index.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-07-28 16:23:15.000000 mscales-1.4.0/docs/source/quickstart.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1624 2023-07-28 16:47:57.000000 mscales-1.4.0/docs/source/release-history.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.4.0/docs/source/scales.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      229 2023-07-12 14:46:22.000000 mscales-1.4.0/mscales/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales/_version.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    15496 2023-07-28 16:23:20.000000 mscales-1.4.0/mscales/basic.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/concepts.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/plots.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-07-12 14:56:49.000000 mscales-1.4.0/mscales/scales.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/sound.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales/tests/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/tests/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/tests/conftest.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/tests/test_examples.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3138 2023-07-28 16:23:20.000000 mscales-1.4.0/mscales/utils.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales.egg-info/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1430 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      666 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       29 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/requires.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/top_level.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       81 2023-07-13 16:14:25.000000 mscales-1.4.0/requirements.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-28 16:49:54.902812 mscales-1.4.0/setup.cfg
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.4.0/setup.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.4.0/versioneer.py
```

### Comparing `mscales-1.3.6/CONTRIBUTING.rst` & `mscales-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/LICENSE` & `mscales-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/PKG-INFO` & `mscales-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.6
+Version: 1.4.0
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -31,14 +31,15 @@
 
 Python package to generate, visualize, and sonify musical scales.
 
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
 
+---------------------
 Notes for development
 ---------------------
 
 - `python3 -m pip install -e .`
 - `python3 -m pip install --upgrade -r requirements-dev.txt`
 
 Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.6/README.rst` & `mscales-1.4.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 Python package to generate, visualize, and sonify musical scales.
 
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
 
+---------------------
 Notes for development
 ---------------------
 
 - `python3 -m pip install -e .`
 - `python3 -m pip install --upgrade -r requirements-dev.txt`
 
 Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.6/docs/Makefile` & `mscales-1.4.0/docs/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    = "-W"  # This flag turns warnings into errors.
 SPHINXBUILD   = sphinx-build
-SPHINXPROJ    = PackagingScientificPython
+SPHINXPROJ    = mscales
 SOURCEDIR     = source
 BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `mscales-1.3.6/docs/make.bat` & `mscales-1.4.0/docs/make.bat`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
 set SOURCEDIR=source
 set BUILDDIR=build
-set SPHINXPROJ=PackagingScientificPython
+set SPHINXPROJ=mscales
 
 if "%1" == "" goto help
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
```

### Comparing `mscales-1.3.6/docs/source/conf.py` & `mscales-1.4.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,38 +17,39 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath("../../mscales/"))
-import sphinx_material
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
+import sphinx_material
+
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx_material",
     "sphinx.ext.autodoc",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.githubpages",
-    "sphinx.ext.intersphinx",
-    "sphinx.ext.mathjax",
-    "sphinx.ext.viewcode",
-    "IPython.sphinxext.ipython_directive",
-    "IPython.sphinxext.ipython_console_highlighting",
+    # "sphinx.ext.autosummary",
+    # "sphinx.ext.githubpages",
+    # "sphinx.ext.intersphinx",
+    # "sphinx.ext.mathjax",
+    # "sphinx.ext.viewcode",
+    # "IPython.sphinxext.ipython_directive",
+    # "IPython.sphinxext.ipython_console_highlighting",
     "matplotlib.sphinxext.plot_directive",
-    "numpydoc",
-    "sphinx_copybutton",
+    # "numpydoc",
+    # "sphinx_copybutton",
 ]
 
 # Configuration options for plot_directive. See:
 # https://github.com/matplotlib/matplotlib/blob/f3ed922d935751e08494e5fb5311d3050a3b637b/lib/matplotlib/sphinxext/plot_directive.py#L81
 plot_html_show_source_link = False
 plot_html_show_formats = False
 
@@ -120,15 +121,15 @@
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 
 # Material theme options (see theme.conf for more information)
 html_theme_options = {
     # Set the name of the project to appear in the navigation.
-    "nav_title": "mscales",
+    "nav_title": "mscales - music theory in Python",
     # Set you GA account ID to enable tracking
     # 'google_analytics_account': 'UA-XXXXX',
     # Specify a base_url used to generate sitemap.xml. If not
     # specified, then no sitemap will be built.
     "base_url": "https://mscales.readthedocs.io/en/latest/",
     # Set the color and the accent color
     "color_primary": "teal",
@@ -138,15 +139,14 @@
     "repo_name": "mscales",
     # Visible levels of the global TOC; -1 means unlimited
     "globaltoc_depth": 1,
     # If False, expand all TOC entries
     "globaltoc_collapse": False,
     # If True, show hidden TOC entries
     "globaltoc_includehidden": False,
-    "nav_title": "mscales - music theory in Python",
     "logo_icon": "&#xE405;",  # Material music note
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static/"]
```

### Comparing `mscales-1.3.6/docs/source/pcsets.rst` & `mscales-1.4.0/docs/source/basic.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Basic objects
 =============
 
 .. note::
     Apart from the ``scales`` module discussed
-    in Quickstart, ``mscales`` also contains the ``pcsets`` module.
+    in Quickstart, ``mscales`` also contains the ``basic`` module.
     At the moment, they are alternatives with partially overlapping
     functionalities but they will be merged in the futured.
     
     As a rule of thumb, use the ``scales`` module whenever possible
-    and only revert to ``pcsets`` when you need very specific things.
+    and only revert to ``basic`` when you need very specific things.
 
-The ``pcsets`` module implements classic definitions of
+The ``basic`` module implements classic definitions of
 and transformations on pitch-class sets known from
 `Set Theory <https://en.wikipedia.org/wiki/Set_theory_(music)>`_.
 
 Pitch classes
 -------------
 
 The fundamental objects of set theory are `pitch classes`.
@@ -119,10 +119,10 @@
     """
 
 
 .. rubric:: API
 
 All methods currently implemented are:
 
-.. automodule:: pcsets
+.. automodule:: basic
     :members:
     :undoc-members:
```

### Comparing `mscales-1.3.6/docs/source/quickstart.rst` & `mscales-1.4.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/docs/source/release-history.rst` & `mscales-1.4.0/docs/source/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Release History
 ===============
 
+v1.4.0 (2023-07-28)
+-------------------
+
+- add several scale properties to PitchClassSet type
+
+v1.3.7 (2023-07-21)
+-------------------
+
+- fix build of documentation
+- rename `pcsets` module to `basic`
+
 v1.3.6 (2023-07-12)
 -------------------
 
 - fix normal form bugs
 - add plotting functionality for PitchClassSets
 
 v1.3.5 (2023-07-12)
```

### Comparing `mscales-1.3.6/mscales/concepts.py` & `mscales-1.4.0/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/mscales/pcsets.py` & `mscales-1.4.0/mscales/basic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import numpy as np
 from itertools import combinations
 from collections.abc import Iterable
 import matplotlib.pyplot as plt
+import pretty_midi as pm
+from utils import find_ngrams
+from collections import Counter
+
+rng = np.random.default_rng()
 
 
 class PitchClass:
-    """Basic pitch-class representation as integers."""
+    """
+    Basic pitch-class representation as integers.
+    """
 
     def __init__(self, p, c: int = 12):
         self.c = c
         self.p = p % self.c
 
     def __repr__(self):
         return f"PitchClass({self.p})"
@@ -33,15 +40,17 @@
             raise TypeError(f"Can't subtract type {type(other)} from pitch class {self.p}.")
 
     def __eq__(self, other):
         return self.p == other.p
 
 
 class PitchClassInterval:
-    """Interval between two pitch classes (mod c)."""
+    """
+    Interval between two pitch classes.
+    """
 
     def __init__(self, i: int, c: int = 12):
         self.c = c
         self.i = i
 
     def __repr__(self):
         return f"PitchClassInterval({self.i})"
@@ -64,35 +73,37 @@
             raise TypeError(f"Can't subtract type {type(other)} from interval {self.i}.")
 
     def __eq__(self, other):
         return self.i == other.i
 
 
 class PitchClassSet:
-    """Set of pitch classes."""
+    """
+    Set of pitch classes.
+    """
 
     def __init__(self, pcset, c: int = 12):
         self.c = c
         self.d = len(pcset)
 
         if isinstance(pcset, str):
             assert all(
                 x in [str(i) for i in range(10)] + ["T"] + ["E"] for x in list(pcset)
             ), "Some pitch classes are not valid."
             self.pcs = np.array([10 if p == "T" else 11 if p == "E" else int(p) for p in list(pcset)])
         elif isinstance(pcset, (Iterable, PitchClassSet)):
             self.pcs = np.array([int(p) for p in pcset])
         else:
-            raise TypeError(f"I don't recognize the pitch-class input {type(pcset)}.")
+            raise TypeError(f"I don't recognize the pitch-class input {type(pcset)}.")        
 
     def __repr__(self):
         return f"PitchClassSet({self.pcs})"
 
-    # def __str__(self):
-    #     return str(self.pcs)
+    def __str__(self):
+        return str(set(self.pcs))
 
     def __len__(self):
         return len(self.pcs)
 
     def __eq__(self, other) -> bool:
         if isinstance(other, PitchClassSet):
             return np.array_equal(self.pcs, other.pcs)
@@ -197,122 +208,249 @@
 
         iv = np.zeros(half, dtype=int)
         for i in interval_classes:
             iv[i - 1] += 1
 
         return iv
 
+    def maximally_even(self):
+        """
+        Calculates all maximally even sets for chromatic cardinality c 
+        and diatonic cardinality d.
+        """
+
+        D = [ [ np.floor((self.c * k + m) / self.d).astype(int) for k in range(self.d) ] for m in range(self.c) ]
+        D = [ np.array(s) for s in set(tuple(i) for i in D) ]
+
+        for s in D:
+            if set(s) == set(self.pcs):
+                return True
+            else:
+                return False
+
+    def spectrum(self, i):
+        """
+        Returns the spectrum of generic interval i,
+        given chromatic cardinality c and diatonic cardinality d.
+        """
+
+        assert i in range(self.d), f"Generic interval i={i} has to be between 0 and {self.d-1}."
+
+        return { (k - j) % self.c for j, k in zip(self.pcs, np.roll(self.pcs, -i)) }
+
+    def myhill(self):
+        """
+        Returns whether pitch-class set has Myhill's property.
+        """
+
+        specs = set([ len(self.spectrum(i=i)) for i in range(1,self.d) ])
+        
+        return True if specs == {2} else False
+
+    def cardinality_equals_variety(self):
+        """
+        Tests if cardinality equals variety holds for PCSet.
+        See: https://en.wikipedia.org/wiki/Cardinality_equals_variety
+        """
+        cev = True
+        for n in range(2,self.d + 1):
+            s = np.append(self.pcs, self.pcs[:n-1])
+            ngrams = find_ngrams(s, n=n)
+            intervals = [ "".join([str((gram[i] - gram[i-1]) % 12) for i in range(1, len(gram))]) for gram in ngrams ]
+            if n != len(Counter(intervals)):
+                return False
+        return True
+
     def sum(self) -> int:
         return sum(self.pcs)
 
     def retrograde(self):
         return PitchClassSet(np.flip(self.pcs))
 
     def inversion(self):
         """This is different from `self.invert` !!"""
         return self.invert(self.pcs[0]).transpose(self.pcs[0])
 
     def matrix(self):
         return np.asarray([self.transpose(-i).pcs for i in self.pcs])
 
-    def plot(self, kind="lollipop", save=False):
+    def plot(self, kind: str = "area", save: bool = False):
+        """This function offers various means for visualizing pitch-class sets.
 
-        if kind == "lollipop":
-            # c = s.shape[0]
+        Args:
+            kind (str, optional): What kind of visualization, see documentation for examples. Defaults to "area".
+            save (bool/str, optional): Given a file path, will try to save the figure at this location. Defaults to False.
 
-            # figure and axis settings
-            _, ax = plt.subplots(subplot_kw={"projection": "polar", "clip_on": False})
-            ax.set_theta_direction(-1)
-            ax.set_theta_zero_location("N")
-            ax.set_yticklabels([])
-            ax.set_ylim(0, 1)
-            plt.thetagrids(np.linspace(0, 360, self.c, endpoint=False), np.arange(self.c))
-
-            # data
-            thetas = [k / self.c * 2 * np.pi for k in np.flatnonzero(self.to_vector())]
-            radii = np.ones(len(thetas))
+        Returns:
+            plt.axis: _matplotlib_ axis object
+        """
 
+        if kind == "bar":
+            _, ax = plt.subplots()
+            ax.bar(np.arange(self.c), self.to_vector(), color="k")
+            ax.set(xlabel="Pitch class", yticks=[], ylim=(0, 1))
+            return ax
+
+        _, ax = plt.subplots(subplot_kw={"projection": "polar", "clip_on": False})
+        ax.set_theta_direction(-1)
+        ax.set_theta_zero_location("N")
+        ax.set_yticklabels([])
+        ax.set_ylim(0, 1)
+        plt.thetagrids(np.linspace(0, 360, self.c, endpoint=False), np.arange(self.c))
+
+        # data
+        thetas = [k / self.c * 2 * np.pi for k in np.flatnonzero(self.to_vector())]
+        radii = [1 for _ in range(len(thetas))]
+
+        if kind == "lollipop":
             stems = ax.stem(thetas, radii, linefmt="k", markerfmt="ok")
             for st in stems:
                 st.set_clip_on(False)
             plt.setp(stems, "linewidth", 3)
             plt.setp(stems[0], "markersize", 10)
-        if kind == "area":
-            # c = s.shape[0]
-
-            # figure and axis settings
-            _, ax = plt.subplots(subplot_kw={"projection": "polar", "clip_on": False})
-            ax.set_theta_direction(-1)
-            ax.set_theta_zero_location("N")
-            ax.set_yticklabels([])
-            ax.set_ylim(0, 1)
-            plt.thetagrids(np.linspace(0, 360, self.c, endpoint=False), np.arange(self.c))
-
-            # data
-            thetas = [k / self.c * 2 * np.pi for k in np.flatnonzero(self.to_vector())]
-            radii = [1 for _ in range(len(thetas))]
-
+            return ax
+        elif kind == "area":
             thetas += thetas[:1]
             radii += radii[:1]
-
             ax.plot(thetas, radii, c="k", zorder=5)
             ax.fill(thetas, radii, alpha=0.75, zorder=4)
-
-        elif kind == "bar":
-            _, ax = plt.subplots()
-            ax.bar(np.arange(self.c), self.to_vector(), color="k")
-            ax.set(xlabel="Pitch class", yticks=[], ylim=(0, 1))
-
         else:
             print("I don't recognize the plot kind." "Valid values are 'polar' and 'bar'.")
-
         if save:
             plt.savefig(save)
-        plt.show()
+
+    def play(
+        self,
+        mode: str = "cloud",
+        n_notes: int = 100,
+        note_duration: float = 0.15,
+        velocity: int = 100,
+        instrument_name: str = "Acoustic Grand Piano",
+        save_as: str = None,
+    ):
+
+        if mode == "cloud":
+            starts = np.arange(n_notes) * note_duration  # onsets
+            ends = starts + note_duration  # offsets
+
+            pitches = [x for x in rng.choice(np.nonzero(self.to_vector())[0], size=n_notes)]
+            octaves = rng.choice(np.arange(3, 7), size=n_notes)
+            midi_pitches = [(p + 12 * o) for p, o in list(zip(pitches, octaves))]
+        elif mode == "chord":
+            pitches = self.pcs
+            octaves = [4] * pitches.shape[0]
+            midi_pitches = [(p + 12 * o) for p, o in list(zip(pitches, octaves))]
+
+            starts = [0] * pitches.shape[0]
+            ends = [note_duration] * pitches.shape[0]
+
+        # Create a PrettyMIDI object
+        midi = pm.PrettyMIDI()
+
+        # Create an Instrument instance for an instrument
+        assert (
+            instrument_name in pm.constants.INSTRUMENT_MAP
+        ), f"Instrument must be in {pm.constants.INSTRUMENT_MAP}"
+        # instrument_code = pm.constants.INSTRUMENT_MAP.index(instrument_name)
+
+        program = pm.instrument_name_to_program(instrument_name)
+        instrument = pm.Instrument(program=program)
+
+        for mp, s, e in zip(midi_pitches, starts, ends):
+            # Create a Note instance for this note, starting at `s` and ending at `e`.
+            note = pm.Note(pitch=mp, velocity=velocity, start=s, end=e)
+            # Add it to instrument
+            instrument.notes.append(note)
+
+        # Add the instrument to the PrettyMIDI object
+        midi.instruments.append(instrument)
+
+        if save_as is not None:
+            midi.write(save_as)
+        else:
+            return midi
 
     def info(self):
-        print("=" * len(repr(self)))
-        print(repr(self))
-        print("=" * len(repr(self)))
-        print()
-        print("Set Theory")
-        print("==========")
-        print("cardin. (d, c)\t:", self.d, self.c)
-        print("pc vector\t:", self.to_vector())
-        print("complement\t:", self.complement())
-        print("transposed\t:", self.transpose(2))
-        print("inverted\t:", self.invert())
-        print("T2I\t\t:", self.invert(2))
-        print("normal form\t:", self.normal_form())
-        print("prime form\t:", self.prime_form())
-        print("interval vector\t:", self.interval_vector())
-        print()
-        print("Serialism")
-        print("=========")
-        print("original\t:", self)
-        print("retrograde\t:", self.retrograde())
-        print("inversion\t:", self.inversion())
-        print("retro.-inv.\t:", self.inversion().retrograde())
-        print("matrix\t\t:", str(self.matrix()).replace("\n", "\n\t\t"))
+        """Returns all sorts of information on the PitchClassSet."""
+        tab = "\n\t\t  "
+        s = "=" * len(repr(self)) + "\n"
+        s += repr(self) + "\n"
+        s += "=" * len(repr(self)) + "\n\n"
+
+        s += "Set Theory" + "\n"
+        s += "==========" + "\n"
+        s += f"cardin. (d, c)\t: {self.d}, {self.c}" + "\n"
+        s += f"pc vector\t: {self.to_vector()}" + "\n"
+        s += f"complement\t: {self.complement()}" + "\n"
+        s += f"transposed\t: {self.transpose(2)}" + "\n"
+        s += f"inverted\t: {self.invert()}" + "\n"
+        s += f"T2I\t\t: {self.invert(2)}" + "\n"
+        s += f"normal form\t: {self.normal_form()}" + "\n"
+        s += f"prime form\t: {self.prime_form()}" + "\n"
+        s += f"interval vector\t: {self.interval_vector()}" + "\n\n"
+
+        s += "Diatonic Scale Theory" + "\n"
+        s += "====================="  + "\n"
+        s += f"Maximally even: {str(self.maximally_even())}" + "\n" 
+        s += f"Spectrum (step): {str(self.spectrum(i=1))}" + "\n"
+        s += f"Myhill's property: {str(self.myhill())}" + "\n"
+        s += f"Cardinality equals variety: {str(self.cardinality_equals_variety())}" + "\n\n" 
+
+        s += "Serialism" + "\n"
+        s += "=========" + "\n"
+        s += f"original\t: {self}" + "\n"
+        s += f"retrograde\t: {self.retrograde()}" + "\n"
+        s += f"inversion\t: {self.inversion()}" + "\n"
+        s += f"retro.-inv.\t: {self.inversion().retrograde()}" + "\n"
+        s += f"matrix\t\t: {str(self.matrix()).replace(chr(10), tab)}"
+
+        return s
 
 
 if __name__ == "__main__":
 
     # test cases from https://musictheory.pugetsound.edu/mt21c/PrimeForm.html
     s = {3, 11, 2}
-    s = {8, 0, 9}
-    s = "123E"
-    s = "17TE"
-    s = "941"
+    # s = {8, 0, 9}
+    # s = "123E"
+    # s = "17TE"
+    # s = "941"
     # s = {11,2,3,7,2}
     # s = {2,3,8,9}
     # s = {0, 2, 4}
-    # s = {0, 1, 4, 6}  # all-interval tetrachord
+    s = {0, 1, 4, 6}  # all-interval tetrachord
     # s = {1,5,6,7} # from Straus, p. 58
     # s = {0, 2, 4, 5, 7, 9, 11}
     # s = {0,1,2}
-    # s = {6,9,2}
+    # s = "147T"
+    # s = "02479"
+    # s = {6, 9, 2}
     # s = {7, 10, 1, 5}
     # s = [0, 1, 6, 7, 5, 2, 4, 3, 10, 9, 11, 8]  # 12-tone row
 
     pcset = PitchClassSet(s)
-    pcset.info()
+    print(pcset.pcs)
+    print(pcset.info())
+    # ax = pcset.plot(kind="area")
+    # plt.show()
+
+    # pcset.play(save_as="test.mid", mode="cloud")
+
+    ## maximally even test
+    # t = PitchClassSet("1234")
+    # dia = PitchClassSet("024579E")
+    p = PitchClassSet("1368T")
+    # oct = PitchClassSet("0134679T")
+    print(p.info())
+    # hex = PitchClassSet("E03478")
+    # ten = PitchClassSet("02468", c=10)
+    # chr = PitchClassSet("1023456789TE")
+
+    # print(oct.maximally_even)
+    # print(hex.maximally_even)
+    # print(ten.maximally_even)
+    # print(p.maximally_even())
+    # print(pcset.myhill())
+
+    # for p in (oct, hex, ten, r):
+    #     p.plot(kind="area")
+    #     plt.show()
```

### Comparing `mscales-1.3.6/mscales/plots.py` & `mscales-1.4.0/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/mscales/scales.py` & `mscales-1.4.0/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/mscales/sound.py` & `mscales-1.4.0/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/mscales/utils.py` & `mscales-1.4.0/mscales/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,9 +155,11 @@
     np.ndarray
         _description_
     """
     z = np.zeros(c).astype(int)
     z[pcset] += 1
     return z
 
+def find_ngrams(input_list, n):
+  return zip(*[input_list[i:] for i in range(n)])
 
 print(transpose(1, 2))
```

### Comparing `mscales-1.3.6/mscales.egg-info/PKG-INFO` & `mscales-1.4.0/mscales.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.6
+Version: 1.4.0
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -31,14 +31,15 @@
 
 Python package to generate, visualize, and sonify musical scales.
 
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
 
+---------------------
 Notes for development
 ---------------------
 
 - `python3 -m pip install -e .`
 - `python3 -m pip install --upgrade -r requirements-dev.txt`
 
 Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.6/mscales.egg-info/SOURCES.txt` & `mscales-1.4.0/mscales.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
-pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 docs/Makefile
 docs/make.bat
+docs/source/basic.rst
 docs/source/conf.py
 docs/source/index.rst
-docs/source/pcsets.rst
 docs/source/quickstart.rst
 docs/source/release-history.rst
 docs/source/scales.rst
 mscales/__init__.py
 mscales/_version.py
+mscales/basic.py
 mscales/concepts.py
-mscales/pcsets.py
 mscales/plots.py
 mscales/scales.py
 mscales/sound.py
 mscales/utils.py
 mscales.egg-info/PKG-INFO
 mscales.egg-info/SOURCES.txt
 mscales.egg-info/dependency_links.txt
```

### Comparing `mscales-1.3.6/setup.py` & `mscales-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.6/versioneer.py` & `mscales-1.4.0/versioneer.py`

 * *Files identical despite different names*

