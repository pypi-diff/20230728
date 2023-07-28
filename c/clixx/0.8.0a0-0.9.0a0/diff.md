# Comparing `tmp/clixx-0.8.0a0.tar.gz` & `tmp/clixx-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clixx-0.8.0a0.tar", last modified: Mon Jun 12 03:12:09 2023, max compression
+gzip compressed data, was "clixx-0.9.0a0.tar", last modified: Fri Jul 28 01:32:32 2023, max compression
```

## Comparing `clixx-0.8.0a0.tar` & `clixx-0.9.0a0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.115541 clixx-0.8.0a0/
--rw-rw-rw-   0        0        0      258 2022-08-20 12:06:12.000000 clixx-0.8.0a0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1087 2023-02-14 02:01:01.000000 clixx-0.8.0a0/LICENSE
--rw-rw-rw-   0        0        0       32 2023-06-01 05:13:09.000000 clixx-0.8.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0     2202 2023-06-12 03:12:09.115541 clixx-0.8.0a0/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-05-14 07:39:38.000000 clixx-0.8.0a0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.078540 clixx-0.8.0a0/docs/
--rw-rw-rw-   0        0        0      638 2022-10-15 01:44:45.000000 clixx-0.8.0a0/docs/Makefile
--rwxrwxrwx   0        0        0      804 2022-10-15 01:44:45.000000 clixx-0.8.0a0/docs/make.bat
--rw-rw-rw-   0        0        0     1476 2023-06-08 11:17:18.000000 clixx-0.8.0a0/docs/release.py
--rw-rw-rw-   0        0        0       69 2023-06-01 07:15:09.000000 clixx-0.8.0a0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.080542 clixx-0.8.0a0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.089541 clixx-0.8.0a0/docs/source/api/
--rw-rw-rw-   0        0        0      457 2023-06-01 09:14:52.000000 clixx-0.8.0a0/docs/source/api/arguments.rst
--rw-rw-rw-   0        0        0      643 2023-06-02 10:51:04.000000 clixx-0.8.0a0/docs/source/api/exceptions.rst
--rw-rw-rw-   0        0        0      462 2023-06-02 10:52:03.000000 clixx-0.8.0a0/docs/source/api/groups.rst
--rw-rw-rw-   0        0        0      134 2023-06-01 07:18:28.000000 clixx-0.8.0a0/docs/source/api/index.rst
--rw-rw-rw-   0        0        0      378 2023-06-02 10:52:28.000000 clixx-0.8.0a0/docs/source/api/printers.rst
--rw-rw-rw-   0        0        0      512 2023-06-01 09:11:06.000000 clixx-0.8.0a0/docs/source/api/types.rst
--rw-rw-rw-   0        0        0     2707 2023-06-03 12:58:19.000000 clixx-0.8.0a0/docs/source/conf.py
--rw-rw-rw-   0        0        0     1274 2023-06-12 02:48:17.000000 clixx-0.8.0a0/pyproject.toml
--rw-rw-rw-   0        0        0     1553 2023-06-12 03:12:09.116540 clixx-0.8.0a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.063539 clixx-0.8.0a0/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.106538 clixx-0.8.0a0/src/clixx/
--rw-rw-rw-   0        0        0     2025 2023-06-12 03:07:22.000000 clixx-0.8.0a0/src/clixx/__init__.py
--rw-rw-rw-   0        0        0     6430 2023-01-07 09:23:51.000000 clixx-0.8.0a0/src/clixx/_rich.py
--rw-rw-rw-   0        0        0    20121 2023-06-12 02:57:15.000000 clixx-0.8.0a0/src/clixx/arguments.py
--rw-rw-rw-   0        0        0    11305 2023-05-21 11:40:40.000000 clixx-0.8.0a0/src/clixx/commands.py
--rw-rw-rw-   0        0        0      412 2023-05-15 03:19:16.000000 clixx-0.8.0a0/src/clixx/constants.py
--rw-rw-rw-   0        0        0    13951 2023-05-17 12:15:48.000000 clixx-0.8.0a0/src/clixx/decorators.py
--rw-rw-rw-   0        0        0     1620 2022-11-13 12:34:28.000000 clixx-0.8.0a0/src/clixx/exceptions.py
--rw-rw-rw-   0        0        0     5325 2023-05-15 08:40:19.000000 clixx-0.8.0a0/src/clixx/groups.py
--rw-rw-rw-   0        0        0    12505 2023-06-01 09:37:06.000000 clixx-0.8.0a0/src/clixx/parsers.py
--rw-rw-rw-   0        0        0     6898 2023-05-14 13:16:46.000000 clixx-0.8.0a0/src/clixx/printers.py
--rw-rw-rw-   0        0        0        0 2022-08-20 08:21:13.000000 clixx-0.8.0a0/src/clixx/py.typed
--rw-rw-rw-   0        0        0    21064 2023-06-12 03:00:46.000000 clixx-0.8.0a0/src/clixx/types.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.114540 clixx-0.8.0a0/src/clixx.egg-info/
--rw-rw-rw-   0        0        0     2202 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-09 02:10:23.000000 clixx-0.8.0a0/src/clixx.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.390154 clixx-0.9.0a0/
+-rw-rw-rw-   0        0        0      258 2022-08-20 12:06:12.000000 clixx-0.9.0a0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1087 2023-02-14 02:01:01.000000 clixx-0.9.0a0/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-06-01 05:13:09.000000 clixx-0.9.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2364 2023-07-28 01:32:32.390663 clixx-0.9.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1082 2023-07-24 03:18:38.000000 clixx-0.9.0a0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.360792 clixx-0.9.0a0/docs/
+-rw-rw-rw-   0        0        0      638 2022-10-15 01:44:45.000000 clixx-0.9.0a0/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2022-10-15 01:44:45.000000 clixx-0.9.0a0/docs/make.bat
+-rw-rw-rw-   0        0        0     1476 2023-06-13 11:28:55.000000 clixx-0.9.0a0/docs/release.py
+-rw-rw-rw-   0        0        0       69 2023-07-28 01:28:41.000000 clixx-0.9.0a0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.361794 clixx-0.9.0a0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.368791 clixx-0.9.0a0/docs/source/api/
+-rw-rw-rw-   0        0        0      457 2023-06-01 09:14:52.000000 clixx-0.9.0a0/docs/source/api/arguments.rst
+-rw-rw-rw-   0        0        0      881 2023-06-14 12:23:59.000000 clixx-0.9.0a0/docs/source/api/exceptions.rst
+-rw-rw-rw-   0        0        0      452 2023-07-02 13:24:01.000000 clixx-0.9.0a0/docs/source/api/groups.rst
+-rw-rw-rw-   0        0        0      150 2023-07-03 06:52:59.000000 clixx-0.9.0a0/docs/source/api/index.rst
+-rw-rw-rw-   0        0        0      240 2023-07-02 13:25:23.000000 clixx-0.9.0a0/docs/source/api/printers.rst
+-rw-rw-rw-   0        0        0      512 2023-06-01 09:11:06.000000 clixx-0.9.0a0/docs/source/api/types.rst
+-rw-rw-rw-   0        0        0     2409 2023-06-30 11:52:53.000000 clixx-0.9.0a0/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1409 2023-07-28 01:24:25.000000 clixx-0.9.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1539 2023-07-28 01:32:32.391670 clixx-0.9.0a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.349793 clixx-0.9.0a0/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.381794 clixx-0.9.0a0/src/clixx/
+-rw-rw-rw-   0        0        0     2801 2023-07-28 01:30:42.000000 clixx-0.9.0a0/src/clixx/__init__.py
+-rw-rw-rw-   0        0        0     4799 2023-07-02 13:31:56.000000 clixx-0.9.0a0/src/clixx/_rich.py
+-rw-rw-rw-   0        0        0    20082 2023-06-13 11:51:55.000000 clixx-0.9.0a0/src/clixx/arguments.py
+-rw-rw-rw-   0        0        0    13941 2023-07-24 03:19:11.000000 clixx-0.9.0a0/src/clixx/commands.py
+-rw-rw-rw-   0        0        0      412 2023-05-15 03:19:16.000000 clixx-0.9.0a0/src/clixx/constants.py
+-rw-rw-rw-   0        0        0    14066 2023-07-02 13:15:16.000000 clixx-0.9.0a0/src/clixx/decorators.py
+-rw-rw-rw-   0        0        0     1729 2023-06-22 11:23:21.000000 clixx-0.9.0a0/src/clixx/exceptions.py
+-rw-rw-rw-   0        0        0     5199 2023-06-27 02:57:35.000000 clixx-0.9.0a0/src/clixx/groups.py
+-rw-rw-rw-   0        0        0    12525 2023-06-22 11:01:40.000000 clixx-0.9.0a0/src/clixx/parsers.py
+-rw-rw-rw-   0        0        0     2817 2023-07-03 06:37:50.000000 clixx-0.9.0a0/src/clixx/printers.py
+-rw-rw-rw-   0        0        0        0 2022-08-20 08:21:13.000000 clixx-0.9.0a0/src/clixx/py.typed
+-rw-rw-rw-   0        0        0    21257 2023-07-02 07:35:21.000000 clixx-0.9.0a0/src/clixx/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.387792 clixx-0.9.0a0/src/clixx.egg-info/
+-rw-rw-rw-   0        0        0     2364 2023-07-28 01:32:32.000000 clixx-0.9.0a0/src/clixx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2023-07-28 01:32:32.000000 clixx-0.9.0a0/src/clixx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 01:32:32.000000 clixx-0.9.0a0/src/clixx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2023-07-28 01:32:32.000000 clixx-0.9.0a0/src/clixx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 01:32:32.000000 clixx-0.9.0a0/src/clixx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-10-09 02:10:23.000000 clixx-0.9.0a0/src/clixx.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-28 01:32:32.388791 clixx-0.9.0a0/tests/
+-rw-rw-rw-   0        0        0      650 2023-06-13 13:18:48.000000 clixx-0.9.0a0/tests/test_decorators.py
```

### Comparing `clixx-0.8.0a0/LICENSE` & `clixx-0.9.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `clixx-0.8.0a0/PKG-INFO` & `clixx-0.9.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clixx
-Version: 0.8.0a0
+Version: 0.9.0a0
 Summary: Command-line interface parser & framework for Python
 Home-page: https://github.com/xymy/clixx
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
@@ -37,14 +37,15 @@
 [![PyPI](https://img.shields.io/pypi/v/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Downloads](https://pepy.tech/badge/clixx/month)](https://pepy.tech/project/clixx)
 [![PyPI - License](https://img.shields.io/pypi/l/clixx)](https://pypi.org/project/clixx/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 CLIXX is a command-line interface parser & framework for Python.
 
 ## Installation
 
 Install from PyPI:
```

### Comparing `clixx-0.8.0a0/README.md` & `clixx-0.9.0a0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![PyPI](https://img.shields.io/pypi/v/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Downloads](https://pepy.tech/badge/clixx/month)](https://pepy.tech/project/clixx)
 [![PyPI - License](https://img.shields.io/pypi/l/clixx)](https://pypi.org/project/clixx/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 CLIXX is a command-line interface parser & framework for Python.
 
 ## Installation
 
 Install from PyPI:
```

### Comparing `clixx-0.8.0a0/docs/Makefile` & `clixx-0.9.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clixx-0.8.0a0/docs/make.bat` & `clixx-0.9.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clixx-0.8.0a0/docs/release.py` & `clixx-0.9.0a0/docs/release.py`

 * *Files identical despite different names*

### Comparing `clixx-0.8.0a0/docs/source/api/exceptions.rst` & `clixx-0.9.0a0/docs/source/api/exceptions.rst`

 * *Files 14% similar despite different names*

```diff
@@ -8,28 +8,44 @@
 
 .. autoexception:: DefinitionError
 
 .. autoexception:: ParserContextError
 
 .. autoexception:: TypeConversionError
 
+Exceptions for parsing
+----------------------
+
 .. autoexception:: CLIXXException
 
+.. autoexception:: ArgumentError
+
 .. autoexception:: TooFewArguments
 
 .. autoexception:: TooManyArguments
 
+.. autoexception:: InvalidArgument
+
+.. autoexception:: OptionError
+
 .. autoexception:: MissingOption
 
 .. autoexception:: UnknownOption
 
 .. autoexception:: TooFewOptionValues
 
 .. autoexception:: TooManyOptionValues
 
-.. autoexception:: InvalidArgumentValue
-
 .. autoexception:: InvalidOptionValue
 
+.. autoexception:: GroupError
+
 .. autoexception:: CommandError
 
-.. autoexception:: GroupError
+Signals
+-------
+
+.. autoexception:: CLIXXSignal
+
+.. autoexception:: HelpSignal
+
+.. autoexception:: VersionSignal
```

### Comparing `clixx-0.8.0a0/docs/source/api/types.rst` & `clixx-0.9.0a0/docs/source/api/types.rst`

 * *Files identical despite different names*

### Comparing `clixx-0.8.0a0/docs/source/conf.py` & `clixx-0.9.0a0/docs/source/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "myst_parser",
     "sphinx_copybutton",
 ]
 templates_path = ["_templates"]
 exclude_patterns = ["**/.DS_Store"]
@@ -49,23 +48,18 @@
 autodoc_default_options = {"members": True, "member-order": "bysource", "show-inheritance": True}
 
 # -- Options for intersphinx -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html#module-sphinx.ext.intersphinx
 
 intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
 
-# -- Options for mathjax -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/extensions/math.html#module-sphinx.ext.mathjax
-
-# mathjax_path = "https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"
-
 # -- Options for myst-parser -------------------------------------------------
 # https://myst-parser.readthedocs.io/en/latest/
 
-myst_enable_extensions = ["deflist", "dollarmath", "tasklist"]
+myst_enable_extensions = ["deflist", "tasklist"]
 myst_heading_anchors = 3
 
 # -- Options for sphinx-copybutton -------------------------------------------
 # https://sphinx-copybutton.readthedocs.io/en/latest/
 
 copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
 copybutton_prompt_is_regexp = True
```

### Comparing `clixx-0.8.0a0/pyproject.toml` & `clixx-0.9.0a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,46 +2,48 @@
 requires = ["setuptools>=51.0", "wheel>=0.36"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 target-version = ["py38", "py39", "py310"]
 
-[tool.isort]
-profile = "black"
-line_length = 120
-
 [tool.ruff]
 line-length = 120
 target-version = "py38"
 show-fixes = true
 show-source = true
 select = [
     "F",      # pyflakes
     "E",      # pycodestyle error
     "W",      # pycodestyle warning
     "D3",     # pydocstyle
     "YTT",    # flake8-2020
     "B",      # flake8-bugbear
     "C4",     # flake8-comprehensions
     "ISC",    # flake8-implicit-str-concat
+    "PIE",    # flake8-pie
     "SIM",    # flake8-simplify
-    "INT",    # flake8-gettext
+    "TCH",    # flake8-type-checking
+    "I",      # isort
+    "RUF010",
     "RUF100",
 ]
 ignore = [
     # Module level import not at top of file
     "E402",
     # Line too long ({width} > {limit} characters)
     "E501",
 ]
 
 [tool.ruff.flake8-comprehensions]
 allow-dict-calls-with-keyword-arguments = true
 
+[tool.ruff.flake8-type-checking]
+exempt-modules = ["typing", "typing_extensions", "enum", "datetime", "pathlib"]
+
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 check_untyped_defs = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
```

### Comparing `clixx-0.8.0a0/setup.cfg` & `clixx-0.9.0a0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -80,19 +80,18 @@
 000004f0: 6963 683e 3d31 332e 300d 0a09 7479 7069  ich>=13.0...typi
 00000500: 6e67 2d65 7874 656e 7369 6f6e 733e 3d34  ng-extensions>=4
 00000510: 2e34 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .4....[options.p
 00000520: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
 00000530: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
 00000540: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
 00000550: 7175 6972 655d 0d0a 6c69 6e74 203d 200d  quire]..lint = .
-00000560: 0a09 626c 6163 6b3e 3d32 332e 330d 0a09  ..black>=23.3...
-00000570: 6973 6f72 743e 3d35 2e31 320d 0a09 7275  isort>=5.12...ru
-00000580: 6666 3e3d 302e 302e 3237 300d 0a09 6d79  ff>=0.0.270...my
-00000590: 7079 3e3d 312e 330d 0a74 6573 7420 3d20  py>=1.3..test = 
-000005a0: 0d0a 0963 6f76 6572 6167 653e 3d37 2e32  ...coverage>=7.2
-000005b0: 0d0a 0968 7970 6f74 6865 7369 733e 3d36  ...hypothesis>=6
-000005c0: 2e37 300d 0a09 7079 7465 7374 3e3d 372e  .70...pytest>=7.
-000005d0: 330d 0a09 7079 7465 7374 2d63 6f76 3e3d  3...pytest-cov>=
-000005e0: 342e 310d 0a0d 0a5b 6567 675f 696e 666f  4.1....[egg_info
-000005f0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000600: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000610: 0a                                       .
+00000560: 0a09 626c 6163 6b3e 3d32 332e 370d 0a09  ..black>=23.7...
+00000570: 7275 6666 3e3d 302e 302e 3238 300d 0a09  ruff>=0.0.280...
+00000580: 6d79 7079 3e3d 312e 340d 0a74 6573 7420  mypy>=1.4..test 
+00000590: 3d20 0d0a 0963 6f76 6572 6167 653e 3d37  = ...coverage>=7
+000005a0: 2e32 0d0a 0968 7970 6f74 6865 7369 733e  .2...hypothesis>
+000005b0: 3d36 2e38 300d 0a09 7079 7465 7374 3e3d  =6.80...pytest>=
+000005c0: 372e 340d 0a09 7079 7465 7374 2d63 6f76  7.4...pytest-cov
+000005d0: 3e3d 342e 310d 0a0d 0a5b 6567 675f 696e  >=4.1....[egg_in
+000005e0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+000005f0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000600: 0a0d 0a                                  ...
```

### Comparing `clixx-0.8.0a0/src/clixx/__init__.py` & `clixx-0.9.0a0/src/clixx/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,16 +21,36 @@
     flag_option,
     help_option,
     option,
     option_group,
     simple_super_command,
     version_option,
 )
+from .exceptions import (
+    ArgumentError,
+    CLIXXException,
+    CLIXXSignal,
+    CommandError,
+    DefinitionError,
+    GroupError,
+    HelpSignal,
+    InvalidArgument,
+    InvalidOptionValue,
+    MissingOption,
+    OptionError,
+    ParserContextError,
+    TooFewArguments,
+    TooFewOptionValues,
+    TooManyArguments,
+    TooManyOptionValues,
+    TypeConversionError,
+    UnknownOption,
+    VersionSignal,
+)
 from .groups import ALL, ANY, AT_LEAST_ONE, AT_MOST_ONE, EXACTLY_ONE, NONE, ArgumentGroup, GroupType, OptionGroup
-from .printers import PrinterHelper, SuperPrinterHelper
 from .types import (
     Bool,
     Choice,
     DateTime,
     DirPath,
     Enum,
     File,
@@ -69,27 +89,44 @@
     "count_option",
     "help_option",
     "version_option",
     "argument_group",
     "option_group",
     "command",
     "simple_super_command",
+    # exceptions
+    "DefinitionError",
+    "ParserContextError",
+    "TypeConversionError",
+    "CLIXXException",
+    "ArgumentError",
+    "TooFewArguments",
+    "TooManyArguments",
+    "InvalidArgument",
+    "OptionError",
+    "MissingOption",
+    "UnknownOption",
+    "TooFewOptionValues",
+    "TooManyOptionValues",
+    "InvalidOptionValue",
+    "GroupError",
+    "CommandError",
+    "CLIXXSignal",
+    "HelpSignal",
+    "VersionSignal",
     # groups
     "GroupType",
     "ANY",
     "ALL",
     "NONE",
     "AT_LEAST_ONE",
     "AT_MOST_ONE",
     "EXACTLY_ONE",
     "ArgumentGroup",
     "OptionGroup",
-    # printers
-    "PrinterHelper",
-    "SuperPrinterHelper",
     # types
     "Type",
     "Str",
     "Bool",
     "Int",
     "Float",
     "Choice",
@@ -101,10 +138,10 @@
     "Path",
     "DirPath",
     "FilePath",
     "resolve_type",
 ]
 
 __title__ = "clixx"
-__version__ = "0.8.0a"
+__version__ = "0.9.0a"
 __author__ = "xymy"
 __email__ = "thyfan@163.com"
```

### Comparing `clixx-0.8.0a0/src/clixx/_rich.py` & `clixx-0.9.0a0/src/clixx/_rich.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from rich.console import Console
 from rich.style import Style
 from rich.table import Table
 from rich.text import Text
 
-from .commands import Command, SuperCommand
-from .exceptions import CLIXXException
+from .commands import Command, SuperCommand, _Command
+
+if TYPE_CHECKING:
+    from .exceptions import CLIXXException
 
 
 def _get_console_params(config: dict[str, Any]) -> dict[str, Any]:
     params = {}
     for param in ["markup", "emoji", "highlight", "highlighter"]:
         if param in config:
             params[param] = config.pop(param)
@@ -28,140 +30,91 @@
 
 
 class RichPrinter:
     def __init__(self, config: dict[str, Any]) -> None:
         self.config = config
         self.console_params = _get_console_params(config)
 
-    def _print_usage(self, console: Console, cmd: Command) -> None:
-        text = Text("Usage: " + cmd.get_prog())
+    def _print_usage(self, console: Console, cmd: _Command) -> None:
+        text = Text("Usage: " + cmd.get_cmd_path())
 
-        if cmd.option_groups:
-            text.append(" [OPTIONS]...")
+        if isinstance(cmd, (Command, SuperCommand)):  # noqa
+            if cmd.option_groups:
+                text.append(" [OPTIONS]...")
+
+        if isinstance(cmd, Command):
+            for argument_group in cmd.argument_groups:
+                for argument in argument_group:
+                    if metavar := argument.resolve_metavar():
+                        if not argument.required:
+                            metavar = "[" + metavar + "]"
+                        if argument.nargs == -1:
+                            metavar += "..."
+                        text.append(" " + metavar)
+        elif isinstance(cmd, SuperCommand):
+            text.append(" COMMAND")
+            text.append(" [ARGS]...")
 
-        for argument_group in cmd.argument_groups:
-            for argument in argument_group:
-                if metavar := argument.resolve_metavar():
-                    if not argument.required:
-                        metavar = "[" + metavar + "]"
-                    if argument.nargs == -1:
-                        metavar += "..."
-                    text.append(" " + metavar)
         console.print(text, soft_wrap=True)
 
-    def _print_try_help(self, console: Console, cmd: Command) -> None:
-        prog = cmd.get_prog()
+    def _print_try_help(self, console: Console, cmd: _Command) -> None:
         option = self.config.get("try_help_option", "--help")
-        text = Text("Try " + repr(prog + " " + option) + " for help.")
+        text = Text("Try " + repr(cmd.get_cmd_path() + " " + option) + " for help.")
         console.print(text, soft_wrap=True)
 
-    def print_error(self, cmd: Command, exc: CLIXXException) -> None:
+    def print_error(self, cmd: _Command, exc: CLIXXException) -> None:
         console = Console(stderr=True, **self.console_params)
         self._print_usage(console, cmd)
         self._print_try_help(console, cmd)
         console.print()
         _print_error(console, exc)
 
-    def print_help(self, cmd: Command) -> None:
+    def print_help(self, cmd: _Command) -> None:
         console = Console(**self.console_params)
         self._print_usage(console, cmd)
 
-        for argument_group in cmd.argument_groups:
-            if argument_group.hidden:
-                continue
-            console.print(f"\n{argument_group.title}:")
-            table = Table(box=None, padding=(0, 0, 0, 2), show_header=False, show_edge=False)
-            table.add_column("Arguments")
-            table.add_column("Descriptions")
-            for argument in argument_group:
-                if argument.hidden:
+        if isinstance(cmd, Command):
+            for argument_group in cmd.argument_groups:
+                if argument_group.hidden:
                     continue
-                table.add_row(argument.argument, argument.help)
-            console.print(table)
-
-        for option_group in cmd.option_groups:
-            if option_group.hidden:
-                continue
-            console.print(f"\n{option_group.title}:")
-            table = Table(box=None, padding=(0, 0, 0, 2), show_header=False, show_edge=False)
-            table.add_column("Options")
-            table.add_column("Descriptions")
-            for option in option_group:
-                if option.hidden:
+                console.print(f"\n{argument_group.title}:")
+                table = Table(box=None, padding=(0, 0, 0, 2), show_header=False, show_edge=False)
+                table.add_column("Arguments")
+                table.add_column("Descriptions")
+                for argument in argument_group:
+                    if argument.hidden:
+                        continue
+                    table.add_row(argument.argument, argument.help)
+                console.print(table)
+        elif isinstance(cmd, SuperCommand):
+            for command_group in cmd.iter_command_group():
+                if command_group.hidden:
                     continue
-                opts = ", ".join(option.short_options + option.long_options)
-                if metavar := option.resolve_metavar():
-                    opts += " " + metavar
-                table.add_row(opts, option.help)
-            console.print(table)
-
-    def print_version(self, cmd: Command) -> None:
-        console = Console(**self.console_params)
-        name = cmd.get_name()
-        version = cmd.get_version()
-        version_info = f"{name} {version}"
-        console.print(version_info, highlight=False)
-
-
-class RichSuperPrinter:
-    def __init__(self, config: dict[str, Any]) -> None:
-        self.config = config
-        self.console_params = _get_console_params(config)
-
-    def _print_usage(self, console: Console, cmd: SuperCommand) -> None:
-        text = Text("Usage: " + cmd.get_prog())
-
-        if cmd.option_groups:
-            text.append(" [OPTIONS]...")
-
-        text.append(" COMMAND")
-        text.append(" [ARGS]...")
-        console.print(text, soft_wrap=True)
-
-    def _print_try_help(self, console: Console, cmd: SuperCommand) -> None:
-        prog = cmd.get_prog()
-        option = self.config.get("try_help_option", "--help")
-        text = Text("Try " + repr(prog + " " + option) + " for help.")
-        console.print(text, soft_wrap=True)
-
-    def print_error(self, cmd: SuperCommand, exc: CLIXXException) -> None:
-        console = Console(stderr=True, **self.console_params)
-        self._print_usage(console, cmd)
-        self._print_try_help(console, cmd)
-        console.print()
-        _print_error(console, exc)
-
-    def print_help(self, cmd: SuperCommand) -> None:
-        console = Console(**self.console_params)
-        self._print_usage(console, cmd)
+                console.print(f"\n{command_group.title}:")
 
-        for command_group in cmd.iter_command_group():
-            if command_group.hidden:
-                continue
-            console.print(f"\n{command_group.title}:")
-
-            # TODO
-            for cmd_name in command_group:
-                console.print(f"  {cmd_name}")
-
-        for option_group in cmd.option_groups:
-            if option_group.hidden:
-                continue
-            console.print(f"\n{option_group.title}:")
-            table = Table(box=None, padding=(0, 0, 0, 2), show_header=False, show_edge=False)
-            table.add_column("Options")
-            table.add_column("Descriptions")
-            for option in option_group:
-                if option.hidden:
+                # TODO
+                for cmd_name in command_group:
+                    console.print(f"  {cmd_name}")
+
+        if isinstance(cmd, (Command, SuperCommand)):
+            for option_group in cmd.option_groups:
+                if option_group.hidden:
                     continue
-                opts = ", ".join(option.short_options + option.long_options)
-                if metavar := option.resolve_metavar():
-                    opts += " " + metavar
-                table.add_row(opts, option.help)
-            console.print(table)
+                console.print(f"\n{option_group.title}:")
+                table = Table(box=None, padding=(0, 0, 0, 2), show_header=False, show_edge=False)
+                table.add_column("Options")
+                table.add_column("Descriptions")
+                for option in option_group:
+                    if option.hidden:
+                        continue
+                    opts = ", ".join(option.short_options + option.long_options)
+                    if metavar := option.resolve_metavar():
+                        opts += " " + metavar
+                    table.add_row(opts, option.help)
+                console.print(table)
 
-    def print_version(self, cmd: SuperCommand) -> None:
+    def print_version(self, cmd: _Command) -> None:
         console = Console(**self.console_params)
         name = cmd.get_name()
         version = cmd.get_version()
         version_info = f"{name} {version}"
         console.print(version_info, highlight=False)
```

### Comparing `clixx-0.8.0a0/src/clixx/arguments.py` & `clixx-0.9.0a0/src/clixx/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 raise DefinitionError("For nargs == -1, the default value must be None.")
         self._default = value
 
     def _verify(self, value: Any) -> Any:
         try:
             return self.type.safe_convert(value)
         except TypeConversionError as e:
-            raise DefinitionError(f"Invalid default value for argument {self.format_decl()}. {str(e)}") from e
+            raise DefinitionError(f"Invalid default value for argument {self.format_decl()}. {e}") from e
 
 
 class Option:
     """The option, aka optional argument.
 
     Parameters:
         decls (tuple[str, ...]):
@@ -292,15 +292,15 @@
         return " / ".join(map(repr, self.short_options + self.long_options))
 
     def resolve_metavar(self) -> str:
         """Resolve metavar."""
 
         if self.metavar is not None:
             return self.metavar
-        elif (metavar := self.type.suggest_metavar()) is not None:
+        elif metavar := self.type.metavar:
             return metavar
         elif self.long_options:
             return _norm_metavar(self.long_options[0][LONG_PREFIX_LEN:])
         else:
             return _norm_metavar(self.short_options[0][SHORT_PREFIX_LEN:])
 
     @property
@@ -319,15 +319,15 @@
 
     @default.setter
     def default(self, value: Any) -> None:
         if value is not None:
             try:
                 value = self.type.safe_convert(value)
             except TypeConversionError as e:
-                raise DefinitionError(f"Invalid default value for option {self.format_decls()}. {str(e)}") from e
+                raise DefinitionError(f"Invalid default value for option {self.format_decls()}. {e}") from e
         self._default = value
 
 
 class FlagOption(Option):
     """The flag option.
 
     Parameters:
@@ -396,15 +396,15 @@
 
     @const.setter
     def const(self, value: Any) -> None:
         if value is not None:
             try:
                 value = self.type.safe_convert(value)
             except TypeConversionError as e:
-                raise DefinitionError(f"Invalid constant value for option {self.format_decls()}. {str(e)}") from e
+                raise DefinitionError(f"Invalid constant value for option {self.format_decls()}. {e}") from e
         self._const = value
 
 
 class AppendOption(Option):
     """The append option.
 
     Parameters:
```

### Comparing `clixx-0.8.0a0/src/clixx/commands.py` & `clixx-0.9.0a0/src/clixx/commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import sys
 from contextlib import suppress
-from typing import Any, Callable, Iterator, Literal, Optional, TypeVar, Union, overload
+from importlib import import_module
+from typing import Any, Callable, Iterator, Optional, TypeVar, Union
 
-from typing_extensions import Never, Self, TypeAlias
+from typing_extensions import Self, TypeAlias
 
 from .constants import DEST_COMMAND_NAME
-from .exceptions import CommandError
+from .exceptions import CommandError, ParserContextError
 from .groups import ArgumentGroup, CommandGroup, OptionGroup
 from .parsers import Parser, SuperParser
-from .printers import PrinterFactory, PrinterHelper, SuperPrinterFactory, SuperPrinterHelper
+from .printers import PrinterFactory, PrinterHelper
 
 CommandFunction: TypeAlias = Callable[..., Optional[int]]
 SuperCommandFunction: TypeAlias = Callable[..., Optional["dict[str, Any]"]]
 
 
 def _print_args(*args: Any, **kwargs: Any) -> None:
     from rich.console import Console
@@ -24,42 +25,23 @@
         if len(args) == 1:
             console.print(args[0])
         else:
             raise AssertionError
     console.print(kwargs)
 
 
-def _interpret_standalone(standalone: bool) -> dict[str, bool]:
-    return {"is_exit": standalone, "is_raise": not standalone}
-
-
-@overload
-def _exit_command(exit_code: int | None, standalone: Literal[False]) -> int:
-    ...
-
-
-@overload
-def _exit_command(exit_code: int | None, standalone: Literal[True]) -> Never:
-    ...
-
-
-@overload
-def _exit_command(exit_code: int | None, standalone: bool) -> int | Never:
-    ...
-
-
-def _exit_command(exit_code: int | None, standalone: bool) -> int | Never:
+def _exit_command(exit_code: int | None, standalone: bool) -> int:
     if standalone:
         sys.exit(exit_code)
     return exit_code if exit_code is not None else 0
 
 
 class _Command:
     parent: SuperCommand | None = None
-    prog: str | None = None
+    _prog: str | None = None
     _args: dict[str, Any] | None = None
     _argv: list[str] | None = None
 
     def __init__(
         self,
         name: str | None = None,
         version: str | None = None,
@@ -85,40 +67,61 @@
     def get_version(self) -> str:
         if self.version is not None:
             return self.version
         if self.parent is not None:
             return self.parent.get_version()
         return "Unknown Version"
 
-    def get_prog(self) -> str:
-        prog = sys.argv[0] if self.prog is None else self.prog
+    def get_cmd_path(self) -> str:
         if self.parent is None:
-            return prog
-        return f"{self.parent.get_prog()} {prog}"
+            return self.prog
+        return f"{self.parent.get_cmd_path()} {self.prog}"
+
+    @property
+    def prog(self) -> str:
+        if self._prog is None:
+            raise ParserContextError("This command is not running.")
+        return self._prog
+
+    @prog.setter
+    def prog(self, value: str) -> None:
+        self._prog = value
 
     @property
     def args(self) -> dict[str, Any]:
         if self._args is None:
-            raise RuntimeError("This command is not running.")
+            raise ParserContextError("This command is not running.")
         return self._args
 
     @args.setter
     def args(self, value: dict[str, Any]) -> None:
         self._args = value
 
     @property
     def argv(self) -> list[str]:
         if self._argv is None:
-            raise RuntimeError("This command is not running.")
+            raise ParserContextError("This command is not running.")
         return self._argv
 
     @argv.setter
     def argv(self, value: list[str]) -> None:
         self._argv = value
 
+    @staticmethod
+    def _check_parent_args(
+        parent: SuperCommand | None, prog: str | None, args: dict[str, Any] | None, argv: list[str] | None
+    ) -> None:
+        if parent is not None:
+            if prog is None:
+                raise ParserContextError("Parent command must provide prog.")
+            if args is None:
+                raise ParserContextError("Parent command must provide args.")
+            if argv is None:
+                raise ParserContextError("Parent command must provide argv.")
+
 
 class Command(_Command):
     """The command.
 
     Parameters:
         name (str | None, default=None):
             The name to display in the version information.
@@ -143,24 +146,30 @@
         description: str = "",
         epilog: str = "",
         *,
         pass_cmd: bool = False,
         printer_factory: PrinterFactory | None = None,
         printer_config: dict[str, Any] | None = None,
     ) -> None:
-        super().__init__(name, version, description, epilog, pass_cmd=pass_cmd)
+        super().__init__(
+            name,
+            version,
+            description,
+            epilog,
+            pass_cmd=pass_cmd,
+        )
+
+        self.printer_factory = printer_factory
+        self.printer_config = printer_config
 
         self.function = _print_args
 
         self.argument_groups: list[ArgumentGroup] = []
         self.option_groups: list[OptionGroup] = []
 
-        self.printer_factory = printer_factory
-        self.printer_config = printer_config
-
     @property
     def function(self) -> CommandFunction:
         """The command function."""
 
         return self._function
 
     @function.setter
@@ -179,21 +188,24 @@
         self,
         args: dict[str, Any] | None = None,
         argv: list[str] | None = None,
         *,
         parent: SuperCommand | None = None,
         prog: str | None = None,
         standalone: bool = True,
-    ) -> int | Never:
-        with PrinterHelper(self, self.printer_factory, self.printer_config, **_interpret_standalone(standalone)):
-            self.parent = parent
-            self.prog = prog
-            self.args = args = args if args is not None else {}
-            self.argv = argv = argv if argv is not None else sys.argv[1:]
+    ) -> int:
+        """Invoke this command."""
 
+        self._check_parent_args(parent, prog, args, argv)
+        self.parent = parent
+        self.prog = prog if prog is not None else sys.argv[0]
+        self.args = args = args if args is not None else {}
+        self.argv = argv = argv if argv is not None else sys.argv[1:]
+
+        with PrinterHelper(self, self.printer_factory, self.printer_config, standalone=standalone):
             parser = Parser(self.argument_groups, self.option_groups)
             parser.parse_args(args, argv)
 
             if self.pass_cmd:  # noqa
                 exit_code = self.function(self, **args)
             else:
                 exit_code = self.function(**args)
@@ -211,42 +223,48 @@
         description (str, default=''):
             The description to display before the main help.
         epilog (str, default=''):
             The epilog to display after the main help.
         pass_cmd (bool, default=False):
             If ``True``, pass this command instance to the command function.
         printer_factory (SuperPrinterFactory | None, default=None):
-            The super printer factory.
+            The printer factory.
         printer_config (dict[str, Any] | None, default=None):
-            The super printer config.
+            The printer config.
     """
 
     def __init__(
         self,
         name: str | None = None,
         version: str | None = None,
         description: str = "",
         epilog: str = "",
         *,
         pass_cmd: bool = False,
-        printer_factory: SuperPrinterFactory | None = None,
+        printer_factory: PrinterFactory | None = None,
         printer_config: dict[str, Any] | None = None,
     ) -> None:
-        super().__init__(name, version, description, epilog, pass_cmd=pass_cmd)
+        super().__init__(
+            name,
+            version,
+            description,
+            epilog,
+            pass_cmd=pass_cmd,
+        )
+
+        self.printer_factory = printer_factory
+        self.printer_config = printer_config
 
         self.function = _print_args
 
         self.option_groups: list[OptionGroup] = []
 
-        self.printer_factory = printer_factory
-        self.printer_config = printer_config
-
     @property
     def function(self) -> SuperCommandFunction:
-        """The super command function."""
+        """The command function."""
 
         return self._function
 
     @function.setter
     def function(self, value: SuperCommandFunction) -> None:
         self._function = value
 
@@ -264,21 +282,24 @@
         self,
         args: dict[str, Any] | None = None,
         argv: list[str] | None = None,
         *,
         parent: SuperCommand | None = None,
         prog: str | None = None,
         standalone: bool = True,
-    ) -> int | Never:
-        with SuperPrinterHelper(self, self.printer_factory, self.printer_config, **_interpret_standalone(standalone)):
-            self.parent = parent
-            self.prog = prog
-            self.args = args = args if args is not None else {}
-            self.argv = argv = argv if argv is not None else sys.argv[1:]
+    ) -> int:
+        """Invoke this command."""
+
+        self._check_parent_args(parent, prog, args, argv)
+        self.parent = parent
+        self.prog = prog if prog is not None else sys.argv[0]
+        self.args = args = args if args is not None else {}
+        self.argv = argv = argv if argv is not None else sys.argv[1:]
 
+        with PrinterHelper(self, self.printer_factory, self.printer_config, standalone=standalone):
             parser = SuperParser(self.option_groups)
             ctx = parser.parse_args(args, argv)
 
             if (cmd_name := args.pop(DEST_COMMAND_NAME, None)) is None:
                 raise CommandError("Missing command.")
 
             if (cmd := self.load_command(cmd_name)) is None:
@@ -286,15 +307,15 @@
 
             if self.pass_cmd:  # noqa
                 args = self.function(self, **args)
             else:
                 args = self.function(**args)
 
             args = args if args is not None else {}
-            exit_code = cmd(args, ctx.argv_remained, parent=self, standalone=standalone)
+            exit_code = cmd(args, ctx.argv_remained, parent=self, prog=cmd_name, standalone=standalone)
         return _exit_command(exit_code, standalone)
 
 
 AnyCommand = TypeVar("AnyCommand", bound=Union[Command, SuperCommand])
 
 
 class SimpleSuperCommand(SuperCommand):
@@ -302,26 +323,27 @@
         self,
         name: str | None = None,
         version: str | None = None,
         description: str = "",
         epilog: str = "",
         *,
         pass_cmd: bool = False,
-        printer_factory: SuperPrinterFactory | None = None,
+        printer_factory: PrinterFactory | None = None,
         printer_config: dict[str, Any] | None = None,
     ) -> None:
         super().__init__(
             name,
             version,
             description,
             epilog,
             pass_cmd=pass_cmd,
             printer_factory=printer_factory,
             printer_config=printer_config,
         )
+
         self.commands: dict[str, dict[str, Command | SuperCommand]] = {}
 
     def add_command(self, group_name: str, cmd_name: str, cmd: Command | SuperCommand) -> Self:
         group_dict = self.commands.setdefault(group_name, {})
         group_dict[cmd_name] = cmd
         return self
 
@@ -340,7 +362,66 @@
             yield group
 
     def load_command(self, name: str) -> Command | SuperCommand | None:
         for group_dict in self.commands.values():
             with suppress(KeyError):
                 return group_dict[name]
         return None
+
+
+class DynamicSuperCommand(SuperCommand):
+    def __init__(
+        self,
+        name: str | None = None,
+        version: str | None = None,
+        description: str = "",
+        epilog: str = "",
+        *,
+        pass_cmd: bool = False,
+        printer_factory: PrinterFactory | None = None,
+        printer_config: dict[str, Any] | None = None,
+    ) -> None:
+        super().__init__(
+            name,
+            version,
+            description,
+            epilog,
+            pass_cmd=pass_cmd,
+            printer_factory=printer_factory,
+            printer_config=printer_config,
+        )
+
+        self.entry_points: dict[str, dict[str, str]] = {}
+
+    def add_entry_point(self, group_name: str, cmd_name: str, ep: str) -> Self:
+        group_dict = self.entry_points.setdefault(group_name, {})
+        group_dict[cmd_name] = ep
+        return self
+
+    def extend_entry_points(self, entry_points: dict[str, dict[str, str]]) -> Self:
+        self.entry_points.update(entry_points)
+        return self
+
+    def iter_command_group(self) -> Iterator[CommandGroup]:
+        for group_name, group_dict in self.entry_points.items():
+            group = CommandGroup(group_name)
+            for cmd_name in group_dict:
+                group.add(cmd_name)
+            yield group
+
+    def load_entry_point(self, name: str) -> str | None:
+        for group_dict in self.entry_points.values():
+            with suppress(KeyError):
+                return group_dict[name]
+        return None
+
+    def load_command(self, name: str) -> Command | SuperCommand | None:
+        ep = self.load_entry_point(name)
+        if ep is not None:
+            split_result = ep.split(":", maxsplit=1)
+            if len(split_result) != 2:
+                return None
+            mod_name, cmd_obj_name = split_result
+            mod = import_module(mod_name)
+            cmd = getattr(mod, cmd_obj_name)
+            return cmd
+        return None
```

### Comparing `clixx-0.8.0a0/src/clixx/decorators.py` & `clixx-0.9.0a0/src/clixx/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 from contextlib import suppress
-from typing import Any, Callable, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, TypeVar, Union
 
 from .arguments import AppendOption, Argument, CountOption, FlagOption, HelpOption, Option, VersionOption
 from .commands import Command, CommandFunction, SimpleSuperCommand, SuperCommandFunction
 from .exceptions import DefinitionError
 from .groups import ANY, ArgumentGroup, GroupType, OptionGroup
-from .printers import PrinterFactory, SuperPrinterFactory
-from .types import Type
+
+if TYPE_CHECKING:
+    from .printers import PrinterFactory
+    from .types import Type
 
 CF = TypeVar("CF", bound=CommandFunction)
 SCF = TypeVar("SCF", bound=SuperCommandFunction)
 F = TypeVar("F", bound=Union[CommandFunction, SuperCommandFunction])
 
 
 def _prepare_definition(func: F, obj: Argument | Option | ArgumentGroup | OptionGroup) -> None:
@@ -36,23 +38,22 @@
 ) -> Callable[[CF], CF]:
     """The argument, aka positional argument.
 
     Parameters:
         decl (str):
             The declaration for this argument.
         dest (str | None, default=None):
-            The destination used to store/forward the argument value. If ``None``,
-            infer from declaration. If empty string, disable store/forward.
+            The destination used to store the argument value. If ``None``, infer
+            from declaration. If empty string, disable the store action.
         nargs (int, default=1):
-            The number of argument values. Valid values are ``nargs == 1`` or
-            ``nargs == -1``.
+            The number of argument values. Valid values are ``1`` or ``-1``.
         required (bool, default=False):
             Whether this argument is required or optional.
         type (Type | type | None, default=None):
-            The type converter. If ``None``, use ``Str()``.
+            The type converter. If ``None``, use :class:`clixx.types.Str()`.
         default (Any, default=None):
             The default value used if argument omitted.
         hidden (bool, default=False):
             If ``True``, hide this argument from help information.
         show_default (bool, default=False):
             If ``True``, show the default value in help information.
         metavar (str | None, default=None):
@@ -94,20 +95,20 @@
 ) -> Callable[[F], F]:
     """The option, aka optional argument.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
         required (bool, default=False):
             Whether this option is required or optional.
         type (Type | type | None, default=None):
-            The type converter. If ``None``, use ``Str()``.
+            The type converter. If ``None``, use :class:`clixx.types.Str()`.
         default (Any, default=None):
             The default value used if option omitted.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         show_default (bool, default=False):
             If ``True``, show the default value in help information.
         metavar (str | None, default=None):
@@ -145,16 +146,16 @@
 ) -> Callable[[F], F]:
     """The flag option.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
         const (Any, default=True):
             The constant value used if option occurred.
         default (Any, default=False):
             The default value used if option omitted.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         help (str, default=''):
@@ -179,18 +180,18 @@
 ) -> Callable[[F], F]:
     """The append option.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
         type (Type | type | None, default=None):
-            The type converter. If ``None``, use ``Str()``.
+            The type converter. If ``None``, use :class:`clixx.types.Str()`.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         metavar (str | None, default=None):
             The option value name used in usage. If ``None``, infer from
             declarations. If empty string, disable metavar.
         help (str, default=''):
             The help information.
@@ -209,17 +210,17 @@
 ) -> Callable[[F], F]:
     """The count option.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
-        default (Any, default=0):
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
+        default (int, default=0):
             The default value used if option omitted.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         help (str, default=''):
             The help information.
     """
 
@@ -311,24 +312,26 @@
     return decorator
 
 
 def command(
     name: str | None = None,
     version: str | None = None,
     description: str = "",
+    epilog: str = "",
     *,
     pass_cmd: bool = False,
     printer_factory: PrinterFactory | None = None,
     printer_config: dict[str, Any] | None = None,
 ) -> Callable[[CF], Command]:
     def decorator(func: CF) -> Command:
         cmd = Command(
             name,
             version,
             description,
+            epilog=epilog,
             pass_cmd=pass_cmd,
             printer_factory=printer_factory,
             printer_config=printer_config,
         )
 
         if hasattr(func, "__clixx_definition__"):
             it = reversed(func.__clixx_definition__)
@@ -357,24 +360,26 @@
     return decorator
 
 
 def simple_super_command(
     name: str | None = None,
     version: str | None = None,
     description: str = "",
+    epilog: str = "",
     *,
     pass_cmd: bool = False,
-    printer_factory: SuperPrinterFactory | None = None,
+    printer_factory: PrinterFactory | None = None,
     printer_config: dict[str, Any] | None = None,
 ) -> Callable[[SCF], SimpleSuperCommand]:
     def decorator(func: SCF) -> SimpleSuperCommand:
         cmd = SimpleSuperCommand(
             name,
             version,
             description,
+            epilog=epilog,
             pass_cmd=pass_cmd,
             printer_factory=printer_factory,
             printer_config=printer_config,
         )
 
         if hasattr(func, "__clixx_definition__"):
             it = reversed(func.__clixx_definition__)
```

### Comparing `clixx-0.8.0a0/src/clixx/exceptions.py` & `clixx-0.9.0a0/src/clixx/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-class DefinitionError(Exception):
+class DefinitionError(ValueError):
     """Define a bad command, group, argument, option, type, etc."""
 
 
-class ParserContextError(Exception):
+class ParserContextError(RuntimeError):
     """Parser context error."""
 
 
-class TypeConversionError(Exception):
+class TypeConversionError(TypeError):
     """Type conversion error."""
 
 
 class CLIXXException(Exception):
     """The base class for all CLIXX exceptions."""
 
     exit_code = 128
@@ -19,54 +19,62 @@
         super().__init__(message)
         self.message = message
 
     def __str__(self) -> str:
         return self.message
 
 
-class TooFewArguments(CLIXXException):
+class ArgumentError(CLIXXException):
+    """Argument error."""
+
+
+class TooFewArguments(ArgumentError):
     """Too few arguments given."""
 
 
-class TooManyArguments(CLIXXException):
+class TooManyArguments(ArgumentError):
     """Too many arguments given."""
 
 
-class MissingOption(CLIXXException):
+class InvalidArgument(ArgumentError):
+    """Invalid argument given."""
+
+
+class OptionError(CLIXXException):
+    """Option error."""
+
+
+class MissingOption(OptionError):
     """Missing option."""
 
 
-class UnknownOption(CLIXXException):
+class UnknownOption(OptionError):
     """Unknown option."""
 
 
-class TooFewOptionValues(CLIXXException):
+class TooFewOptionValues(OptionError):
     """Too few option values given."""
 
 
-class TooManyOptionValues(CLIXXException):
+class TooManyOptionValues(OptionError):
     """Too many option values given."""
 
 
-class InvalidArgumentValue(CLIXXException):
-    """Invalid argument value given."""
+class InvalidOptionValue(OptionError):
+    """Invalid option value given."""
 
 
-class InvalidOptionValue(CLIXXException):
-    """Invalid option value given."""
+class GroupError(CLIXXException):
+    """Group error."""
 
 
 class CommandError(CLIXXException):
     """Command error."""
 
 
-class GroupError(CLIXXException):
-    """Group error."""
-
-
 class CLIXXSignal(BaseException):
     """The base class for all CLIXX signals."""
 
     exit_code = 0
 
 
 class HelpSignal(CLIXXSignal):
```

### Comparing `clixx-0.8.0a0/src/clixx/groups.py` & `clixx-0.9.0a0/src/clixx/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,23 +57,18 @@
         return len(self.members)
 
     def __iter__(self) -> Iterator[T]:
         """Iterate members."""
 
         yield from self.members
 
-    def __iadd__(self, member: T) -> Self:
-        """Add the member to this group."""
+    def add(self, *members: T) -> Self:
+        """Add members to this group."""
 
-        return self.add(member)
-
-    def add(self, member: T) -> Self:
-        """Add the member to this group."""
-
-        self.members.append(member)
+        self.members.extend(members)
         return self
 
 
 class ArgumentGroup(_Group[Argument]):
     """The argument group.
 
     Parameters:
```

### Comparing `clixx-0.8.0a0/src/clixx/parsers.py` & `clixx-0.9.0a0/src/clixx/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from __future__ import annotations
 
 import weakref
 from contextlib import contextmanager
-from typing import Any, Callable, Generator, cast
+from typing import TYPE_CHECKING, Any, Callable, Generator, cast
 
 from .arguments import Argument, Option, is_long_option, is_separator, is_short_option
 from .constants import DEST_COMMAND_NAME, SHORT_PREFIX_LEN
 from .exceptions import (
-    InvalidArgumentValue,
+    InvalidArgument,
     InvalidOptionValue,
     MissingOption,
     ParserContextError,
     TooFewArguments,
     TooFewOptionValues,
     TooManyArguments,
     TooManyOptionValues,
     TypeConversionError,
     UnknownOption,
 )
-from .groups import ArgumentGroup, OptionGroup
+
+if TYPE_CHECKING:
+    from .groups import ArgumentGroup, OptionGroup
 
 
 @contextmanager
 def _raise_invalid_argument_value(format_decl: Callable[[], str]) -> Generator[None, None, None]:
     try:
         yield
     except TypeConversionError as e:
         name = format_decl()
-        raise InvalidArgumentValue(f"Invalid value for argument {name}. {str(e)}") from e
+        raise InvalidArgument(f"Invalid value for argument {name}. {e}") from e
 
 
 @contextmanager
 def _raise_invalid_option_value(format_decls: Callable[[], str]) -> Generator[None, None, None]:
     try:
         yield
     except TypeConversionError as e:
         name = format_decls()
-        raise InvalidOptionValue(f"Invalid value for option {name}. {str(e)}") from e
+        raise InvalidOptionValue(f"Invalid value for option {name}. {e}") from e
 
 
 class ArgumentNode:
     """The stateful argument node."""
 
     def __init__(self, argument: Argument, parent: ArgumentGroupNode) -> None:
         self._argument = argument
```

### Comparing `clixx-0.8.0a0/src/clixx/types.py` & `clixx-0.9.0a0/src/clixx/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def _force_decode(filename: Any) -> str:
     fname = cast(Union[str, bytes], os.fspath(filename))
     if isinstance(fname, str):
         return fname
     return fname.decode(sys.getfilesystemencoding(), "backslashreplace")
 
 
-def _resolve_norm(case_sensitive: bool) -> Callable[[str], str]:
+def _resolve_normcase(case_sensitive: bool) -> Callable[[str], str]:
     if case_sensitive:
         return str
     return str.casefold
 
 
 class Type:
     """The base class for all CLIXX type converters.
@@ -53,33 +53,34 @@
 
         This is used to verify and preprocess the *constant*/*default* values.
         """
 
         return self(value)
 
     def release(self, value: Any) -> None:
-        """Release the resource.
+        """Release resource held by value.
 
-        This is used to release the resource for the previous parsed values
+        This is used to release resource held by the previous parsed values
         which are overrided by the current value.
         """
 
     def format(self, value: Any) -> str:
-        """Format value.
+        """Format value to pretty string.
 
         The ``value`` must be compatible with this type, usually the return
         value of :meth:`~clixx.types.Type.safe_convert`.
         """
 
         return str(value)
 
-    def suggest_metavar(self) -> str | None:
-        """Suggest metavar for help information."""
+    @property
+    def metavar(self) -> str:
+        """The metavar suitable for this type. Empty string means inavailable."""
 
-        return None
+        return ""
 
 
 class Str(Type):
     """The class used to convert command-line arguments to string.
 
     Target type: :class:`str`.
     """
@@ -105,26 +106,27 @@
 
     def convert(self, value: Any) -> Any:
         if isinstance(value, bool):
             return value
         raise TypeConversionError(f"{value!r} is not a valid boolean.")
 
     def convert_str(self, value: str) -> Any:
-        v = value.lower()
-        if v in {"t", "true", "y", "yes", "on", "1"}:
+        value_norm = value.lower()
+        if value_norm in {"t", "true", "y", "yes", "on", "1"}:
             return True
-        if v in {"f", "false", "n", "no", "off", "0"}:
+        if value_norm in {"f", "false", "n", "no", "off", "0"}:
             return False
         raise TypeConversionError(f"{value!r} is not a valid boolean.")
 
     def format(self, value: Any) -> str:
         assert isinstance(value, bool)
         return "true" if value else "false"
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "BOOLEAN"
 
 
 class Int(Type):
     """The class used to convert command-line arguments to integer.
 
     Target type: :class:`int`.
@@ -159,15 +161,16 @@
             elif self.base == 8:
                 raise TypeConversionError(f"{value!r} is not a valid octal integer.") from e
             elif self.base == 2:
                 raise TypeConversionError(f"{value!r} is not a valid binary integer.") from e
             else:
                 raise TypeConversionError(f"{value!r} is not a valid integer with base {self.base!r}.") from e
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "INTEGER"
 
 
 class Float(Type):
     """The class used to convert command-line arguments to floating point number.
 
     Target type: :class:`float`.
@@ -183,15 +186,16 @@
 
     def convert_str(self, value: str) -> Any:
         try:
             return float(value)
         except ValueError as e:
             raise TypeConversionError(f"{value!r} is not a valid floating point number.") from e
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "FLOAT"
 
 
 class Choice(Type):
     """The class used to convert command-line arguments to string in choices.
 
     Target type: :class:`str`.
@@ -210,24 +214,25 @@
         self.case_sensitive = case_sensitive
 
     def convert(self, value: Any) -> Any:
         choices_str = ", ".join(map(repr, self.choices))
         raise TypeConversionError(f"{value!r} is not one of {choices_str}.")
 
     def convert_str(self, value: str) -> Any:
-        norm = _resolve_norm(self.case_sensitive)
-        v = norm(value)
+        normcase = _resolve_normcase(self.case_sensitive)
+        value_norm = normcase(value)
         for choice in self.choices:
-            if v == norm(choice):
+            if value_norm == normcase(choice):
                 return choice
 
         choices_str = ", ".join(map(repr, self.choices))
         raise TypeConversionError(f"{value!r} is not one of {choices_str}.")
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "[" + "|".join(self.choices) + "]"
 
 
 class IntChoice(Type):
     """The class used to convert command-line arguments to integer in choices.
 
     Target type: :class:`int`.
@@ -255,15 +260,16 @@
         for choice in self.choices:
             if value == choice:
                 return choice
 
         choices_str = ", ".join(map(repr, self.choices))
         raise TypeConversionError(f"{value!r} is not one of {choices_str}.")
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "[" + "|".join(map(str, self.choices)) + "]"
 
 
 class Enum(Type):
     """The class used to convert command-line arguments to enumeration.
 
     Target type: :class:`enum.Enum`.
@@ -283,28 +289,29 @@
 
     def convert(self, value: Any) -> Any:
         if isinstance(value, self.enum_type):
             return value
         raise TypeConversionError(f"{value!r} is not a valid enumeration member of {self.enum_type!r}.")
 
     def convert_str(self, value: str) -> Any:
-        norm = _resolve_norm(self.case_sensitive)
-        v = norm(value)
+        normcase = _resolve_normcase(self.case_sensitive)
+        value_norm = normcase(value)
         for name, member in self.enum_type.__members__.items():
-            if v == norm(name):
+            if value_norm == normcase(name):
                 return member
 
         enum_str = ", ".join(map(repr, self.enum_type.__members__))
         raise TypeConversionError(f"{value!r} is not one of {enum_str}.")
 
     def format(self, value: Any) -> str:
         assert isinstance(value, self.enum_type)
         return value.name
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "[" + "|".join(self.enum_type.__members__) + "]"
 
 
 class IntEnum(Type):
     """The class used to convert command-line arguments to integer enumeration.
 
     Target type: :class:`enum.IntEnum`.
@@ -337,15 +344,16 @@
         enum_str = ", ".join(repr(m.value) for m in self.enum_type)
         raise TypeConversionError(f"{value!r} is not one of {enum_str}.")
 
     def format(self, value: Any) -> str:
         assert isinstance(value, self.enum_type)
         return str(value.value)
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "[" + "|".join(str(m.value) for m in self.enum_type) + "]"
 
 
 class DateTime(Type):
     """The class used to convert command-line arguments to datetime.
 
     Target type: :class:`datetime.datetime`.
@@ -380,15 +388,16 @@
         formats_str = ", ".join(map(repr, self.formats))
         if len(self.formats) == 1:  # noqa
             hint = f"Valid format is {formats_str}."
         else:
             hint = f"Valid formats are {formats_str}."
         raise TypeConversionError(f"{value!r} is not a valid datetime. {hint}")
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "DATETIME"
 
 
 class File(Type):
     """The class used to convert command-line arguments to file.
 
     Target type: :class:`typing.IO`.
@@ -461,39 +470,41 @@
 
     def safe_convert(self, value: Any) -> Any:
         if isinstance(value, (str, bytes, pathlib.Path)) or hasattr(value, "read") or hasattr(value, "write"):
             return value
         raise TypeConversionError(f"{value!r} is not a valid file.")
 
     def release(self, value: Any) -> None:
-        cast(IO, value).close()
+        with suppress(AttributeError):
+            if value.fileno() > 2:  # skip stdin/stdout/stderr
+                value.close()
 
     def format(self, value: Any) -> str:
         # These types can be decoded anyway.
         if isinstance(value, (str, bytes, pathlib.Path)):
             return _force_decode(value)
         # The file object may know its filename.
-        if (name := getattr(value, "name", None)) is not None:
-            with suppress(TypeError):
-                return _force_decode(name)
+        with suppress(AttributeError, TypeError):
+            return _force_decode(value.name)
         # This file does not have a pretty string representation. Just return a rough string.
         return str(value)
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "FILE"
 
 
 class Path(Type):
     """The class used to convert command-line arguments to path.
 
     Target type: :class:`pathlib.Path`.
 
     Parameters:
         resolve (bool, default=False):
-            If ``True``, make the path absolute, resolve all symlinks, and normalize it.
+            If ``True``, resolve the path via :meth:`pathlib.Path.resolve`.
         exists (bool, default=False):
             If ``True``, check whether the path exists.
         readable (bool, default=False):
             If ``True``, check whether the path is readable.
         writable (bool, default=False):
             If ``True``, check whether the path is writable.
         executable (bool, default=False):
@@ -556,41 +567,44 @@
         if isinstance(value, (str, bytes, pathlib.Path)):
             return value
         raise TypeConversionError(f"{value!r} is not a valid path.")
 
     def format(self, value: Any) -> str:
         return _force_decode(value)
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "PATH"
 
 
 class DirPath(Path):
     """Similar to :class:`clixx.types.Path`, but check whether the path is a
     directory if it exists."""
 
     @staticmethod
     def _check_path_stat(path: pathlib.Path, st: os.stat_result) -> None:
         if not stat.S_ISDIR(st.st_mode):
             raise TypeConversionError(f"{str(path)!r} is not a directory.")
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "DIRECTORY"
 
 
 class FilePath(Path):
     """Similar to :class:`clixx.types.Path`, but check whether the path is a
     file if it exists."""
 
     @staticmethod
     def _check_path_stat(path: pathlib.Path, st: os.stat_result) -> None:
         if not stat.S_ISREG(st.st_mode):
             raise TypeConversionError(f"{str(path)!r} is not a file.")
 
-    def suggest_metavar(self) -> str | None:
+    @property
+    def metavar(self) -> str:
         return "FILE"
 
 
 def resolve_type(type: Type | type) -> Type:
     """Convert Python's builtin type to CLIXX's type. Return as is if ``type``
     is already an instance of :class:`clixx.types.Type`.
```

### Comparing `clixx-0.8.0a0/src/clixx.egg-info/PKG-INFO` & `clixx-0.9.0a0/src/clixx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clixx
-Version: 0.8.0a0
+Version: 0.9.0a0
 Summary: Command-line interface parser & framework for Python
 Home-page: https://github.com/xymy/clixx
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
@@ -37,14 +37,15 @@
 [![PyPI](https://img.shields.io/pypi/v/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Downloads](https://pepy.tech/badge/clixx/month)](https://pepy.tech/project/clixx)
 [![PyPI - License](https://img.shields.io/pypi/l/clixx)](https://pypi.org/project/clixx/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 CLIXX is a command-line interface parser & framework for Python.
 
 ## Installation
 
 Install from PyPI:
```

### Comparing `clixx-0.8.0a0/src/clixx.egg-info/SOURCES.txt` & `clixx-0.9.0a0/src/clixx.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 src/clixx/py.typed
 src/clixx/types.py
 src/clixx.egg-info/PKG-INFO
 src/clixx.egg-info/SOURCES.txt
 src/clixx.egg-info/dependency_links.txt
 src/clixx.egg-info/requires.txt
 src/clixx.egg-info/top_level.txt
-src/clixx.egg-info/zip-safe
+src/clixx.egg-info/zip-safe
+tests/test_decorators.py
```

