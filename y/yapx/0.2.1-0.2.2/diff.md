# Comparing `tmp/yapx-0.2.1.tar.gz` & `tmp/yapx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapx-0.2.1.tar", last modified: Tue Jul 25 04:05:50 2023, max compression
+gzip compressed data, was "yapx-0.2.2.tar", last modified: Fri Jul 28 04:52:45 2023, max compression
```

## Comparing `yapx-0.2.1.tar` & `yapx-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.599640 yapx-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-25 04:01:15.000000 yapx-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5869 2023-07-25 04:05:50.599640 yapx-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4124 2023-07-25 04:01:15.000000 yapx-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)     4887 2023-07-25 04:01:15.000000 yapx-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 04:05:50.599640 yapx-0.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.591640 yapx-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.595640 yapx-0.2.1/src/yapx/
--rw-r--r--   0 root         (0) root         (0)     5155 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.599640 yapx-0.2.1/src/yapx/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-25 04:05:29.000000 yapx-0.2.1/src/yapx/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7098 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/actions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7626 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/arg.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    27701 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/argument_parser.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      784 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/namespace.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/types.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4278 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-25 04:05:29.000000 yapx-0.2.1/src/yapx/__version__.py
--rw-r--r--   0 root         (0) root         (0)     9750 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/actions.py
--rw-r--r--   0 root         (0) root         (0)     9642 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/arg.py
--rw-r--r--   0 root         (0) root         (0)    44458 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/argument_parser.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/namespace.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/py.typed
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/types.py
--rw-r--r--   0 root         (0) root         (0)     4211 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.595640 yapx-0.2.1/src/yapx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5869 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.599640 yapx-0.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)     5205 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_actions.py
--rw-r--r--   0 root         (0) root         (0)    11974 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_add_arguments.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_add_arguments_future.py
--rw-r--r--   0 root         (0) root         (0)     1260 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_add_command.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_arg.py
--rw-r--r--   0 root         (0) root         (0)    25200 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_run.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.706005 yapx-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-28 04:48:20.000000 yapx-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-07-28 04:52:45.706005 yapx-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-07-28 04:48:20.000000 yapx-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     4885 2023-07-28 04:48:20.000000 yapx-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 04:52:45.706005 yapx-0.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.694005 yapx-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.698005 yapx-0.2.2/src/yapx/
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.702005 yapx-0.2.2/src/yapx/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-28 04:52:24.000000 yapx-0.2.2/src/yapx/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-28 04:49:01.000000 yapx-0.2.2/src/yapx/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/arg.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    27963 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/argument_parser.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      784 2023-07-28 04:49:01.000000 yapx-0.2.2/src/yapx/__pycache__/namespace.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-28 04:49:00.000000 yapx-0.2.2/src/yapx/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4278 2023-07-28 04:49:01.000000 yapx-0.2.2/src/yapx/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 04:52:24.000000 yapx-0.2.2/src/yapx/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     9750 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/actions.py
+-rw-r--r--   0 root         (0) root         (0)     9642 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/arg.py
+-rw-r--r--   0 root         (0) root         (0)    44793 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/namespace.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/types.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-07-28 04:48:20.000000 yapx-0.2.2/src/yapx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.702005 yapx-0.2.2/src/yapx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      770 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-28 04:52:45.000000 yapx-0.2.2/src/yapx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:52:45.706005 yapx-0.2.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_actions.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_add_arguments.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_add_arguments_future.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_add_command.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)    25200 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_run.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-28 04:48:20.000000 yapx-0.2.2/tests/test_utils.py
```

### Comparing `yapx-0.2.1/LICENSE` & `yapx-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/README.md` & `yapx-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,74 @@
+Metadata-Version: 2.1
+Name: yapx
+Version: 0.2.2
+Summary: The next generation of Python's Argparse.
+Author-email: Donald Mellenbruch <hello@f2dv.com>
+License: Copyright 2023 Donald Mellenbruch
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: Homepage, https://www.f2dv.com/r/yapx
+Project-URL: Repository, https://www.github.com/fresh2dev/yapx
+Project-URL: Funding, https://www.f2dv.com/fund
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: tests
+Provides-Extra: pydantic
+Provides-Extra: shtab
+Provides-Extra: rich
+Provides-Extra: tui
+Provides-Extra: extras
+License-File: LICENSE
+
 # yapx
 
-> Build awesome Python CLIs with ease.
+> The next generation of Python's Argparse.
 
-| Links         |                                              |
-|---------------|----------------------------------------------|
-| Code Repo     | https://www.github.com/fresh2dev/yapx        |
-| Mirror Repo   | https://www.f2dv.com/code/r/yapx             |
-| Documentation | https://www.f2dv.com/code/r/yapx/i           |
-| Changelog     | https://www.f2dv.com/code/r/yapx/i/changelog |
-| License       | https://www.f2dv.com/code/r/yapx/i/license   |
-| Funding       | https://www.f2dv.com/fund                    |
-
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
-[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
-[![License](https://img.shields.io/github/license/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/yapx/i/license)
+| Links         |                                       |
+|---------------|---------------------------------------|
+| Code Repo     | https://www.github.com/fresh2dev/yapx |
+| Mirror Repo   | https://www.f2dv.com/r/yapx           |
+| Documentation | https://www.f2dv.com/r/yapx           |
+| Changelog     | https://www.f2dv.com/r/yapx/changelog |
+| License       | https://www.f2dv.com/r/yapx/license   |
+| Funding       | https://www.f2dv.com/fund             |
+
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/changelog)
+[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/changelog)
+[![License](https://img.shields.io/github/license/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/license)
+[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/yapx?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/yapx&Date)
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/pulls)
-[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/yapx?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/yapx&Date)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/yapx?color=blue&style=for-the-badge)](https://pypi.org/project/yapx)
 [![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/yapx?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/yapx)
-[![Docs Website](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/yapx/i)](https://www.f2dv.com/code/r/yapx/i)
-[![Coverage Website](https://img.shields.io/website?down_message=unavailable&label=coverage&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/yapx/i/tests/coverage)](https://www.f2dv.com/code/r/yapx/i/tests/coverage)
+[![Changelog](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/yapx/changelog)](https://www.f2dv.com/r/yapx/changelog)
 [![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.f2dv.com/fund)
 
-## Overview
-
-Yapx is "yeah, another argparse extension" for building Python CLIs with the utmost simplicity.
-
-It works by reading type hints of Python functions and dataclasses, and uses them to construct an argparse `ArgumentParser`.
+---
 
-Yapx features:
+## Overview
 
-- Support for subcommands
-- Support for lists in various forms: (positional) `1 2 3`, (multiple) `-x 1 -x 2 -x 3`, (multi-value) `-x 1 2 3`, (comma-separated), `-x 1, 2, 3`, (string) `-x '[1, 2, 3]'`
-- Support for dictionaries / key-value mappings such as `--values one=1 two=2 three=3`
-- Support for optional booleans: `--flag` / `--no-flag`
-- Support for feature flags: `--dev` / `--test` / `--prod`
-- Support for counting parameters: `-vvv`
-- Automatic "helpful" arguments: `--help`, `--help-all`, `--version`, etc.
-- Support for setting values from environment variables
+...
 
 ## Install
 
-Yapx has no 3rd-party dependencies out-of-the-box:
-
-```sh
-pip install yapx
-```
-
-Extras are available to unlock additional functionality:
-
-- `yapx[pydantic]`: enables support for additional types
-- `yapx[shtab]`: enables shell-completion
-- `yapx[rich]`: enables prettier help and error messages
-- `yapx[tui]`: enables experimental TUI support
-- `yapx[extras]`: enables each of the above
+...
 
 ## Use
 
-See notebooks of examples here:
-
-https://www.f2dv.com/code/r/yapx/i/page/overview
-
-Read more about yapx @ https://www.f2dv.com/code/r/yapx/i
+...
 
 ## Support
 
 If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/yapx/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
 
-See all of my projects @ https://www.f2dv.com/code/r
-
 *Brought to you by...*
 
 <a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

#### html2text {}

```diff
@@ -1,53 +1,54 @@
-# yapx > Build awesome Python CLIs with ease. | Links | | |---------------|----
-------------------------------------------| | Code Repo | https://
-www.github.com/fresh2dev/yapx | | Mirror Repo | https://www.f2dv.com/code/r/
-yapx | | Documentation | https://www.f2dv.com/code/r/yapx/i | | Changelog |
-https://www.f2dv.com/code/r/yapx/i/changelog | | License | https://
-www.f2dv.com/code/r/yapx/i/license | | Funding | https://www.f2dv.com/fund | [!
-[GitHub release (latest SemVer)](https://img.shields.io/github/v/release/
+Metadata-Version: 2.1 Name: yapx Version: 0.2.2 Summary: The next generation of
+Python's Argparse. Author-email: Donald Mellenbruch
+f2dv.com> License: Copyright 2023 Donald Mellenbruch Permission is hereby
+granted, free of charge, to any person obtaining a copy of this software and
+associated documentation files (the "Software"), to deal in the Software
+without restriction, including without limitation the rights to use, copy,
+modify, merge, publish, distribute, sublicense, and/or sell copies of the
+Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://www.f2dv.com/r/yapx
+Project-URL: Repository, https://www.github.com/fresh2dev/yapx Project-URL:
+Funding, https://www.f2dv.com/fund Classifier: Programming Language :: Python
+:: 3 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
+Extra: dev Provides-Extra: docs Provides-Extra: tests Provides-Extra: pydantic
+Provides-Extra: shtab Provides-Extra: rich Provides-Extra: tui Provides-Extra:
+extras License-File: LICENSE # yapx > The next generation of Python's Argparse.
+| Links | | |---------------|---------------------------------------| | Code
+Repo | https://www.github.com/fresh2dev/yapx | | Mirror Repo | https://
+www.f2dv.com/r/yapx | | Documentation | https://www.f2dv.com/r/yapx | |
+Changelog | https://www.f2dv.com/r/yapx/changelog | | License | https://
+www.f2dv.com/r/yapx/license | | Funding | https://www.f2dv.com/fund | [![GitHub
+release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/
+yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/changelog) [!
+[GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/
+yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/changelog) [!
+[License](https://img.shields.io/github/license/fresh2dev/
+yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/r/yapx/license) [!
+[GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/
+yapx?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/
+yapx&Date) [![GitHub issues](https://img.shields.io/github/issues-raw/
 fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/
-fresh2dev/yapx/releases) [![GitHub Release Date](https://img.shields.io/github/
-release-date/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
-www.github.com/fresh2dev/yapx/releases) [![License](https://img.shields.io/
-github/license/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
-www.f2dv.com/code/r/yapx/i/license) [![GitHub issues](https://img.shields.io/
-github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
-www.github.com/fresh2dev/yapx/issues) [![GitHub pull requests](https://
-img.shields.io/github/issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-
-badge)](https://www.github.com/fresh2dev/yapx/pulls) [![GitHub Repo stars]
-(https://img.shields.io/github/stars/fresh2dev/yapx?color=blue&style=for-the-
-badge)](https://star-history.com/#fresh2dev/yapx&Date) [![PyPI - Downloads]
-(https://img.shields.io/pypi/dm/yapx?color=blue&style=for-the-badge)](https://
-pypi.org/project/yapx) [![Docker Pulls](https://img.shields.io/docker/pulls/
-fresh2dev/yapx?color=blue&style=for-the-badge)](https://hub.docker.com/r/
-fresh2dev/yapx) [![Docs Website](https://img.shields.io/
+fresh2dev/yapx/issues) [![GitHub pull requests](https://img.shields.io/github/
+issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
+www.github.com/fresh2dev/yapx/pulls) [![PyPI - Downloads](https://
+img.shields.io/pypi/dm/yapx?color=blue&style=for-the-badge)](https://pypi.org/
+project/yapx) [![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/
+yapx?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/yapx)
+[![Changelog](https://img.shields.io/
 website?down_message=unavailable&label=docs&style=for-the-
-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/yapx/
-i)](https://www.f2dv.com/code/r/yapx/i) [![Coverage Website](https://
-img.shields.io/website?down_message=unavailable&label=coverage&style=for-the-
-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/yapx/
-i/tests/coverage)](https://www.f2dv.com/code/r/yapx/i/tests/coverage) [!
-[Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-
-badge)](https://www.f2dv.com/fund) ## Overview Yapx is "yeah, another argparse
-extension" for building Python CLIs with the utmost simplicity. It works by
-reading type hints of Python functions and dataclasses, and uses them to
-construct an argparse `ArgumentParser`. Yapx features: - Support for
-subcommands - Support for lists in various forms: (positional) `1 2 3`,
-(multiple) `-x 1 -x 2 -x 3`, (multi-value) `-x 1 2 3`, (comma-separated), `-
-x 1, 2, 3`, (string) `-x '[1, 2, 3]'` - Support for dictionaries / key-value
-mappings such as `--values one=1 two=2 three=3` - Support for optional
-booleans: `--flag` / `--no-flag` - Support for feature flags: `--dev` / `--
-test` / `--prod` - Support for counting parameters: `-vvv` - Automatic
-"helpful" arguments: `--help`, `--help-all`, `--version`, etc. - Support for
-setting values from environment variables ## Install Yapx has no 3rd-party
-dependencies out-of-the-box: ```sh pip install yapx ``` Extras are available to
-unlock additional functionality: - `yapx[pydantic]`: enables support for
-additional types - `yapx[shtab]`: enables shell-completion - `yapx[rich]`:
-enables prettier help and error messages - `yapx[tui]`: enables experimental
-TUI support - `yapx[extras]`: enables each of the above ## Use See notebooks of
-examples here: https://www.f2dv.com/code/r/yapx/i/page/overview Read more about
-yapx @ https://www.f2dv.com/code/r/yapx/i ## Support If this project delivers
-value to you, please [provide feedback](https://www.github.com/fresh2dev/yapx/
-issues), code contributions, and/or [funding](https://www.f2dv.com/fund). See
-all of my projects @ https://www.f2dv.com/code/r *Brought to you by...* [https:
-//img.fresh2.dev/fresh2dev.svg]
+badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/yapx/
+changelog)](https://www.f2dv.com/r/yapx/changelog) [![Funding](https://
+img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://
+www.f2dv.com/fund) --- ## Overview ... ## Install ... ## Use ... ## Support If
+this project delivers value to you, please [provide feedback](https://
+www.github.com/fresh2dev/yapx/issues), code contributions, and/or [funding]
+(https://www.f2dv.com/fund). *Brought to you by...* [https://img.fresh2.dev/
+fresh2dev.svg]
```

### Comparing `yapx-0.2.1/pyproject.toml` & `yapx-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yapx"
 authors = [
     {name = "Donald Mellenbruch", email = "hello@f2dv.com"},
 ]
-description = "Build awesome Python CLIs with ease."
+description = "The next generation of Python's Argparse."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["version"]
@@ -72,15 +72,15 @@
     "pydantic>=1.10.3,<3",
     "shtab==1.6.2",
     "rich-argparse==1.*",
     "argparse-tui>=0.1.2,<1",
 ]
 
 [project.urls]
-Homepage = "https://www.f2dv.com/code/r/yapx/i"
+Homepage = "https://www.f2dv.com/r/yapx"
 Repository = "https://www.github.com/fresh2dev/yapx"
 Funding = "https://www.f2dv.com/fund"
 
 [tool.setuptools.package-data]
 "*" = ["**"]
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `yapx-0.2.1/src/yapx/__init__.py` & `yapx-0.2.2/src/yapx/__init__.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/src/yapx/__pycache__/__init__.cpython-310.pyc` & `yapx-0.2.2/src/yapx/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 25 04:01:15 2023 UTC, .py size: 5155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b49 bf64 2314 0000  o........I.d#...
+00000000: 6f0d 0d0a 0000 0000 9448 c364 2314 0000  o........H.d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 1402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6403 6404 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6403 6405 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6403 6406 6c0d 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `yapx-0.2.1/src/yapx/__pycache__/actions.cpython-310.pyc` & `yapx-0.2.2/src/yapx/__pycache__/actions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 25 04:01:15 2023 UTC, .py size: 9750 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b49 bf64 1626 0000  o........I.d.&..
+00000000: 6f0d 0d0a 0000 0000 9448 c364 1626 0000  o........H.d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 7201 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c03 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
```

### Comparing `yapx-0.2.1/src/yapx/__pycache__/arg.cpython-310.pyc` & `yapx-0.2.2/src/yapx/__pycache__/arg.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 25 04:01:15 2023 UTC, .py size: 9642 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b49 bf64 aa25 0000  o........I.d.%..
+00000000: 6f0d 0d0a 0000 0000 9448 c364 aa25 0000  o........H.d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 3c02 0000 5500  .....@...s<...U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6402 6c02 6d03 5a03 0100 6400 6403  d.d.l.m.Z...d.d.
 00000050: 6c04 6d05 5a05 0100 6400 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 6d0e  Z...d.d.l.m.Z.m.
```

### Comparing `yapx-0.2.1/src/yapx/__pycache__/argument_parser.cpython-310.pyc` & `yapx-0.2.2/src/yapx/__pycache__/argument_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 25 04:01:15 2023 UTC, .py size: 44458 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b49 bf64 aaad 0000  o........I.d....
+00000000: 6f0d 0d0a 0000 0000 9448 c364 f9ae 0000  o........H.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c02 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -84,1649 +84,1665 @@
 00000530: 5f69 7369 6e73 7461 6e63 65da 0e74 7279  _isinstance..try
 00000540: 5f69 7373 7562 636c 6173 7329 02e9 0300  _issubclass)....
 00000550: 0000 e909 0000 0029 01da 0f5f 416e 6e6f  .......)..._Anno
 00000560: 7461 7465 6441 6c69 6173 a902 723a 0000  tatedAlias..r:..
 00000570: 00e9 0a00 0000 2901 da09 556e 696f 6e54  ......)...UnionT
 00000580: 7970 65da 0154 6300 0000 0000 0000 0000  ype..Tc.........
 00000590: 0000 0000 0000 0017 0000 0000 0000 0073  ...............s
-000005a0: 2805 0000 6500 5a01 6400 5a02 5500 6401  (...e.Z.d.Z.U.d.
+000005a0: 3c05 0000 6500 5a01 6400 5a02 5500 6401  <...e.Z.d.Z.U.d.
 000005b0: 5a03 6504 6505 6402 3c00 6403 5a06 6504  Z.e.e.d.<.d.Z.e.
 000005c0: 6505 6404 3c00 6405 5a07 6504 6505 6406  e.d.<.d.Z.e.e.d.
 000005d0: 3c00 6407 5a08 6504 6505 6408 3c00 6409  <.d.Z.e.e.d.<.d.
 000005e0: 5a09 6504 6505 640a 3c00 640b 640b 640b  Z.e.e.d.<.d.d.d.
 000005f0: 640b 640b 640b 640b 650a 640c 640d 9c09  d.d.d.d.e.d.d...
 00000600: 640e 650b 640f 650c 6504 1900 6410 650c  d.e.d.e.e...d.e.
 00000610: 6504 1900 6411 650c 6504 1900 6412 650c  e...d.e.e...d.e.
 00000620: 650d 6504 1900 1900 6413 650c 650d 6504  e.e.....d.e.e.e.
 00000630: 1900 1900 6414 650c 650d 6504 1900 1900  ....d.e.e.e.....
 00000640: 6415 650c 650d 6504 1900 1900 6416 650e  d.e.e.e.....d.e.
 00000650: 650b 1900 6417 650f 6418 650b 6616 8700  e...d.e.d.e.f...
 00000660: 6601 6419 641a 840e 5a10 641b 6504 6602  f.d.d...Z.d.e.f.
-00000670: 641c 641d 8404 5a11 090b 090c 6468 641e  d.d...Z.....dhd.
+00000670: 641c 641d 8404 5a11 090b 090c 646a 641e  d.d...Z.....djd.
 00000680: 650c 6512 6504 1900 1900 641f 650f 6420  e.e.e.....d.e.d 
 00000690: 640b 6606 8700 6601 6421 6422 840d 5a13  d.f...f.d!d"..Z.
 000006a0: 6423 6514 6515 6424 650b 6602 1900 650e  d#e.e.d$e.f...e.
 000006b0: 6516 1900 6602 1900 6420 640b 6604 6425  e...f...d d.f.d%
-000006c0: 6426 8404 5a17 090b 6469 6423 6514 6515  d&..Z...did#e.e.
+000006c0: 6426 8404 5a17 090b 646b 6423 6514 6515  d&..Z...dkd#e.e.
 000006d0: 6424 650b 6602 1900 650e 6516 1900 6602  d$e.f...e.e...f.
 000006e0: 1900 6427 650c 6504 1900 6418 650b 6420  ..d'e.e...d.e.d 
 000006f0: 6518 6a19 6608 6428 6429 8405 5a1a 090b  e.j.f.d(d)..Z...
-00000700: 6469 642a 6515 6424 650b 6602 1900 6427  did*e.d$e.f...d'
+00000700: 646b 642a 6515 6424 650b 6602 1900 6427  dkd*e.d$e.f...d'
 00000710: 650c 6504 1900 6418 650b 6420 640b 6608  e.e...d.e.d d.f.
 00000720: 642b 642c 8405 5a1b 651c 642d 650e 6516  d+d,..Z.e.d-e.e.
 00000730: 1900 642e 6504 6420 650f 6606 642f 6430  ..d.e.d e.f.d/d0
 00000740: 8404 8301 5a1d 651e 6431 6518 6a19 6423  ....Z.e.d1e.j.d#
 00000750: 6514 6515 6424 650b 6602 1900 650e 6516  e.e.d$e.f...e.e.
 00000760: 1900 6602 1900 6420 650d 651f 1900 6606  ..f...d e.e...f.
 00000770: 6432 6433 8404 8301 5a20 651c 6434 650e  d2d3....Z e.d4e.
 00000780: 650b 1900 6420 650c 650e 650b 1900 1900  e...d e.e.e.....
 00000790: 6604 6435 6436 8404 8301 5a21 651c 6434  f.d5d6....Z!e.d4
 000007a0: 650e 650b 1900 6420 6522 650e 650b 1900  e.e...d e"e.e...
 000007b0: 6424 6602 1900 6604 6437 6438 8404 8301  d$f...f.d7d8....
 000007c0: 5a23 651c 6434 650e 650b 1900 6420 6522  Z#e.d4e.e...d e"
 000007d0: 650e 650b 1900 6424 6602 1900 6604 6439  e.e...d$f...f.d9
-000007e0: 643a 8404 8301 5a24 651e 090c 090c 646a  d:....Z$e.....dj
+000007e0: 643a 8404 8301 5a24 651e 090c 090c 646c  d:....Z$e.....dl
 000007f0: 643b 650e 650b 1900 643c 650f 643d 650f  d;e.e...d<e.d=e.
 00000800: 6420 650e 650b 1900 6608 643e 643f 8405  d e.e...f.d>d?..
-00000810: 8301 5a25 6420 650c 6518 6a26 1900 6602  ..Z%d e.e.j&..f.
-00000820: 6440 6441 8404 5a27 6420 6518 6a26 6602  d@dA..Z'd e.j&f.
-00000830: 6442 6443 8404 5a28 6444 6518 6a29 6420  dBdC..Z(dDe.j)d 
-00000840: 6529 6604 6445 6446 8404 5a2a 090b 090b  e)f.dEdF..Z*....
-00000850: 646b 640e 650c 652b 6504 1900 1900 6444  dkd.e.e+e.....dD
-00000860: 650c 6518 6a29 1900 6420 6529 6606 8700  e.e.j)..d e)f...
-00000870: 6601 6447 6448 840d 5a2c 090b 090b 646b  f.dGdH..Z,....dk
-00000880: 640e 650c 652b 6504 1900 1900 6444 650c  d.e.e+e.....dDe.
-00000890: 6518 6a29 1900 6420 6522 6529 650d 6504  e.j)..d e"e)e.e.
-000008a0: 1900 6602 1900 6606 8700 6601 6449 644a  ..f...f...f.dIdJ
-000008b0: 840d 5a2d 090b 090b 090c 646c 640e 650c  ..Z-......dld.e.
-000008c0: 652b 6504 1900 1900 6423 650c 650e 6516  e+e.....d#e.e.e.
-000008d0: 1900 1900 644b 650f 6420 6522 6516 650d  ....dKe.d e"e.e.
-000008e0: 6504 1900 6602 1900 6608 644c 644d 8405  e...f...f.dLdM..
-000008f0: 5a2e 090b 090b 090c 646c 640e 650c 652b  Z.......dld.e.e+
-00000900: 6504 1900 1900 6423 650c 650e 6516 1900  e.....d#e.e.e...
-00000910: 1900 644b 650f 6420 6516 6608 644e 644f  ..dKe.d e.f.dNdO
-00000920: 8405 5a2f 090b 090c 6468 640e 6518 6a29  ..Z/....dhd.e.j)
-00000930: 6423 650c 650e 6516 1900 1900 644b 650f  d#e.e.e.....dKe.
-00000940: 6420 6516 6608 6450 6451 8405 5a30 651c  d e.f.dPdQ..Z0e.
-00000950: 6452 6531 6504 650b 6602 1900 6423 650e  dRe1e.e.f...d#e.
-00000960: 6516 1900 6420 6531 6504 650b 6602 1900  e...d e1e.e.f...
-00000970: 6606 6453 6454 8404 8301 5a32 651e 6423  f.dSdT....Z2e.d#
-00000980: 6514 6515 6424 650b 6602 1900 650e 6516  e.e.d$e.f...e.e.
-00000990: 1900 6602 1900 6420 650c 6504 1900 6604  ..f...d e.e...f.
-000009a0: 6455 6456 8404 8301 5a33 651e 6431 6518  dUdV....Z3e.d1e.
-000009b0: 6a19 6423 6514 6515 6424 650b 6602 1900  j.d#e.e.d$e.f...
-000009c0: 650e 6516 1900 6602 1900 6420 640b 6606  e.e...f...d d.f.
-000009d0: 6457 6458 8404 8301 5a34 651e 090b 090b  dWdX....Z4e.....
-000009e0: 090b 646d 6431 6400 642a 6515 6424 650b  ..dmd1d.d*e.d$e.
-000009f0: 6602 1900 640e 650d 6504 1900 6423 650c  f...d.e.e...d#e.
-00000a00: 650e 650b 1900 1900 6459 650c 6515 6424  e.e.....dYe.e.d$
-00000a10: 650b 6602 1900 1900 645a 650c 650b 1900  e.f.....dZe.e...
-00000a20: 6420 650b 660e 645b 645c 8405 8301 5a35  d e.f.d[d\....Z5
-00000a30: 651e 090b 090b 090b 646d 645d 650c 6515  e.......dmd]e.e.
-00000a40: 6424 650b 6602 1900 1900 645e 650c 652b  d$e.f.....d^e.e+
-00000a50: 6515 6424 650b 6602 1900 1900 1900 645f  e.d$e.f.......d_
-00000a60: 650c 6531 6504 6515 6424 650b 6602 1900  e.e1e.e.d$e.f...
-00000a70: 6602 1900 1900 6418 650b 6420 6400 660a  f.....d.e.d d.f.
-00000a80: 6460 6461 8405 8301 5a36 651e 640b 640b  d`da....Z6e.d.d.
-00000a90: 6462 9c02 6463 650b 640e 650c 650d 6504  db..dce.d.e.e.e.
-00000aa0: 1900 1900 6464 650c 650d 6504 1900 1900  ....dde.e.e.....
-00000ab0: 6465 650b 6420 650b 660a 6466 6467 8406  dee.d e.f.dfdg..
-00000ac0: 8301 5a37 8700 0400 5a38 5300 296e da0e  ..Z7....Z8S.)n..
-00000ad0: 4172 6775 6d65 6e74 5061 7273 6572 5a0a  ArgumentParserZ.
-00000ae0: 5f72 6f6f 745f 6675 6e63 da13 524f 4f54  _root_func..ROOT
-00000af0: 5f46 554e 435f 4154 5452 5f4e 414d 455a  _FUNC_ATTR_NAMEZ
-00000b00: 155f 726f 6f74 5f66 756e 635f 6172 6773  ._root_func_args
-00000b10: 5f6d 6f64 656c da18 524f 4f54 5f46 554e  _model..ROOT_FUN
-00000b20: 435f 4152 4753 5f41 5454 525f 4e41 4d45  C_ARGS_ATTR_NAME
-00000b30: 5a08 5f63 6f6d 6d61 6e64 da0d 434d 445f  Z._command..CMD_
-00000b40: 4154 5452 5f4e 414d 455a 0d5f 636f 6d6d  ATTR_NAMEZ._comm
-00000b50: 616e 645f 6675 6e63 da12 434d 445f 4655  and_func..CMD_FU
-00000b60: 4e43 5f41 5454 525f 4e41 4d45 5a18 5f63  NC_ATTR_NAMEZ._c
-00000b70: 6f6d 6d61 6e64 5f66 756e 635f 6172 6773  ommand_func_args
-00000b80: 5f6d 6f64 656c da17 434d 445f 4655 4e43  _model..CMD_FUNC
-00000b90: 5f41 5247 535f 4154 5452 5f4e 414d 454e  _ARGS_ATTR_NAMEN
-00000ba0: 4629 09da 0470 726f 67da 0c70 726f 675f  F)...prog..prog_
-00000bb0: 7665 7273 696f 6eda 0b64 6573 6372 6970  version..descrip
-00000bc0: 7469 6f6e da0a 6865 6c70 5f66 6c61 6773  tion..help_flags
-00000bd0: da0d 7665 7273 696f 6e5f 666c 6167 73da  ..version_flags.
-00000be0: 0974 7569 5f66 6c61 6773 da10 636f 6d70  .tui_flags..comp
-00000bf0: 6c65 7469 6f6e 5f66 6c61 6773 da0f 666f  letion_flags..fo
-00000c00: 726d 6174 7465 725f 636c 6173 73da 0d5f  rmatter_class.._
-00000c10: 6973 5f73 7562 7061 7273 6572 da04 6172  is_subparser..ar
-00000c20: 6773 7247 0000 0072 4800 0000 7249 0000  gsrG...rH...rI..
-00000c30: 0072 4a00 0000 724b 0000 0072 4c00 0000  .rJ...rK...rL...
-00000c40: 724d 0000 0072 4e00 0000 724f 0000 00da  rM...rN...rO....
-00000c50: 066b 7761 7267 7363 0100 0000 0000 0000  .kwargsc........
-00000c60: 0900 0000 0d00 0000 0800 0000 0f00 0000  ................
-00000c70: 73ee 0100 0074 0083 006a 017c 0a7c 017c  s....t...j.|.|.|
-00000c80: 0972 0964 006e 017c 0364 017c 0864 029c  .r.d.n.|.d.|.d..
-00000c90: 047c 0ba4 018e 0101 0064 007c 005f 0264  .|.......d.|._.d
-00000ca0: 037c 006a 035f 047c 0464 0075 0072 2164  .|.j._.|.d.u.r!d
-00000cb0: 0464 0567 027d 047c 0472 3974 057c 0474  .d.g.}.|.r9t.|.t
-00000cc0: 0683 0272 2b7c 0467 017d 047c 006a 0764  ...r+|.g.}.|.j.d
-00000cd0: 0664 0784 007c 0444 0083 0174 0864 0864  .d...|.D...t.d.d
-00000ce0: 099c 028e 0101 0064 0a7c 005f 0974 0a64  .......d.|._.t.d
-00000cf0: 0b64 0c84 0083 017c 005f 0b69 007c 005f  .d.....|._.i.|._
-00000d00: 0c7c 0973 f17c 0472 5a64 0d64 0784 007c  .|.s.|.rZd.d...|
-00000d10: 0444 0083 017d 0c7c 006a 077c 0c74 0d64  .D...}.|.j.|.t.d
-00000d20: 0e64 099c 028e 0101 007c 0564 0075 0072  .d.......|.d.u.r
-00000d30: 6164 0f67 017d 057c 0572 9974 057c 0574  ad.g.}.|.r.t.|.t
-00000d40: 0683 0272 6b7c 0567 017d 057c 006a 0e72  ...rk|.g.}.|.j.r
-00000d50: 8a7c 0273 8a74 0f74 1083 018f 0e01 0074  .|.s.t.t.......t
-00000d60: 117c 006a 0e83 016a 127d 0257 0064 0004  .|.j...j.}.W.d..
-00000d70: 0004 0083 0301 006e 0831 0073 8577 0101  .......n.1.s.w..
-00000d80: 0001 0001 0059 0001 007c 0272 997c 006a  .....Y...|.r.|.j
-00000d90: 077c 0564 1064 117c 029b 009d 0264 1264  .|.d.d.|.....d.d
-00000da0: 139c 038e 0101 007c 0764 0075 0072 a064  .......|.d.u.r.d
-00000db0: 1467 017d 0774 1372 b97c 0772 b974 057c  .g.}.t.r.|.r.t.|
-00000dc0: 0774 0683 0272 ac7c 0767 017d 077c 006a  .t...r.|.g.}.|.j
-00000dd0: 077c 0774 1483 0074 156a 1674 1764 1564  .|.t...t.j.t.d.d
-00000de0: 169c 048e 0101 007c 0664 0075 0072 c064  .......|.d.u.r.d
-00000df0: 1767 017d 067c 0672 f374 1872 f574 057c  .g.}.|.r.t.r.t.|
-00000e00: 0674 0683 0272 cc7c 0667 017d 0674 197c  .t...r.|.g.}.t.|
-00000e10: 0683 0164 186b 0272 e87c 0664 1919 00a0  ...d.k.r.|.d....
-00000e20: 1a64 1aa1 0173 e87c 00a0 1ba1 0001 0074  .d...s.|.......t
-00000e30: 1c7c 007c 0664 1919 0064 1b64 1c8d 0301  .|.|.d...d.d....
-00000e40: 0064 0053 0074 1d7c 007c 0664 1b64 1c8d  .d.S.t.|.|.d.d..
-00000e50: 0301 0064 0053 0064 0053 0064 0053 0064  ...d.S.d.S.d.S.d
-00000e60: 0053 0029 1d4e 4629 0472 4700 0000 7249  .S.).NF).rG...rI
-00000e70: 0000 00da 0861 6464 5f68 656c 7072 4e00  .....add_helprN.
-00000e80: 0000 7a12 6865 6c70 6675 6c20 7061 7261  ..z.helpful para
-00000e90: 6d65 7465 7273 7a02 2d68 7a06 2d2d 6865  metersz.-hz.--he
-00000ea0: 6c70 6301 0000 0000 0000 0000 0000 0002  lpc.............
-00000eb0: 0000 0003 0000 0053 0000 0073 1400 0000  .......S...s....
-00000ec0: 6700 7c00 5d06 7d01 7c01 7202 7c01 9102  g.|.].}.|.r.|...
-00000ed0: 7102 5300 a900 7253 0000 00a9 02da 022e  q.S...rS........
-00000ee0: 30da 0178 7253 0000 0072 5300 0000 fa26  0..xrS...rS....&
-00000ef0: 2f64 726f 6e65 2f73 7263 2f73 7263 2f79  /drone/src/src/y
-00000f00: 6170 782f 6172 6775 6d65 6e74 5f70 6172  apx/argument_par
-00000f10: 7365 722e 7079 da0a 3c6c 6973 7463 6f6d  ser.py..<listcom
-00000f20: 703e 7600 0000 7302 0000 0014 007a 2b41  p>v...s......z+A
-00000f30: 7267 756d 656e 7450 6172 7365 722e 5f5f  rgumentParser.__
-00000f40: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-00000f50: 3c6c 6973 7463 6f6d 703e 7a17 5368 6f77  <listcomp>z.Show
-00000f60: 2074 6869 7320 6865 6c70 206d 6573 7361   this help messa
-00000f70: 6765 2e29 02da 0661 6374 696f 6eda 0468  ge.)...action..h
-00000f80: 656c 70fa 013d 6300 0000 0000 0000 0000  elp..=c.........
-00000f90: 0000 0000 0000 0002 0000 0053 0000 0073  ...........S...s
-00000fa0: 0800 0000 7400 7401 8301 5300 a901 4e29  ....t.t...S...N)
-00000fb0: 0272 0200 0000 da04 6c69 7374 7253 0000  .r......listrS..
-00000fc0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
-00000fd0: da08 3c6c 616d 6264 613e 8000 0000 7302  ..<lambda>....s.
-00000fe0: 0000 0008 007a 2941 7267 756d 656e 7450  .....z)ArgumentP
-00000ff0: 6172 7365 722e 5f5f 696e 6974 5f5f 2e3c  arser.__init__.<
-00001000: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00001010: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001020: 0005 0000 0053 0000 0073 2000 0000 6700  .....S...s ...g.
-00001030: 7c00 5d0c 7d01 7c01 a000 6400 a101 7202  |.].}.|...d...r.
-00001040: 7c01 9b00 6401 9d02 9102 7102 5300 2902  |...d.....q.S.).
-00001050: 7a02 2d2d 7a04 2d61 6c6c a901 da0a 7374  z.--z.-all....st
-00001060: 6172 7473 7769 7468 7254 0000 0072 5300  artswithrT...rS.
-00001070: 0000 7253 0000 0072 5700 0000 7258 0000  ..rS...rW...rX..
-00001080: 0086 0000 00f3 0200 0000 2000 7a1b 5368  .......... .z.Sh
-00001090: 6f77 2068 656c 7020 666f 7220 616c 6c20  ow help for all 
-000010a0: 636f 6d6d 616e 6473 2e7a 092d 2d76 6572  commands.z.--ver
-000010b0: 7369 6f6e da07 7665 7273 696f 6e7a 0925  sion..versionz.%
-000010c0: 2870 726f 6729 7320 7a20 5368 6f77 2074  (prog)s z Show t
-000010d0: 6865 2070 726f 6772 616d 2076 6572 7369  he program versi
-000010e0: 6f6e 206e 756d 6265 722e 2903 7259 0000  on number.).rY..
-000010f0: 0072 6200 0000 725a 0000 007a 182d 2d70  .rb...rZ...z.--p
-00001100: 7269 6e74 2d73 6865 6c6c 2d63 6f6d 706c  rint-shell-compl
-00001110: 6574 696f 6e7a 1e50 7269 6e74 2073 6865  etionz.Print she
-00001120: 6c6c 2063 6f6d 706c 6574 696f 6e20 7363  ll completion sc
-00001130: 7269 7074 2e29 0472 5900 0000 da07 6465  ript.).rY.....de
-00001140: 6661 756c 74da 0763 686f 6963 6573 725a  fault..choicesrZ
-00001150: 0000 007a 052d 2d74 7569 7217 0000 0072  ...z.--tuir....r
-00001160: 0100 0000 fa01 2d7a 2253 686f 7720 5465  ......-z"Show Te
-00001170: 7874 7561 6c20 5573 6572 2049 6e74 6572  xtual User Inter
-00001180: 6661 6365 2028 5455 4929 2e29 03da 0670  face (TUI).)...p
-00001190: 6172 7365 72da 0e6f 7074 696f 6e5f 7374  arser..option_st
-000011a0: 7269 6e67 7372 5a00 0000 291e da05 7375  ringsrZ...)...su
-000011b0: 7065 72da 085f 5f69 6e69 745f 5fda 125f  per..__init__.._
-000011c0: 7375 6270 6172 7365 7273 5f61 6374 696f  subparsers_actio
-000011d0: 6eda 0a5f 6f70 7469 6f6e 616c 73da 0574  n.._optionals..t
-000011e0: 6974 6c65 da0a 6973 696e 7374 616e 6365  itle..isinstance
-000011f0: da03 7374 72da 0c61 6464 5f61 7267 756d  ..str..add_argum
-00001200: 656e 7472 1b00 0000 da0c 6b76 5f73 6570  entr......kv_sep
-00001210: 6172 6174 6f72 7202 0000 00da 185f 6d75  aratorr......_mu
-00001220: 7475 616c 6c79 5f65 7863 6c75 7369 7665  tually_exclusive
-00001230: 5f61 7267 73da 0a5f 6465 7374 5f74 7970  _args.._dest_typ
-00001240: 6572 1c00 0000 7247 0000 0072 0300 0000  er....rG...r....
-00001250: da09 4578 6365 7074 696f 6e72 1600 0000  ..Exceptionr....
-00001260: 7262 0000 0072 3600 0000 7232 0000 00da  rb...r6...r2....
-00001270: 0861 7267 7061 7273 65da 0853 5550 5052  .argparse..SUPPR
-00001280: 4553 5372 2c00 0000 7237 0000 00da 036c  ESSr,...r7.....l
-00001290: 656e 7260 0000 00da 165f 6765 745f 6f72  enr`....._get_or
-000012a0: 5f61 6464 5f73 7562 7061 7273 6572 7372  _add_subparsersr
-000012b0: 3000 0000 722f 0000 0029 0dda 0473 656c  0...r/...)...sel
-000012c0: 6672 4700 0000 7248 0000 0072 4900 0000  frG...rH...rI...
-000012d0: 724a 0000 0072 4b00 0000 724c 0000 0072  rJ...rK...rL...r
-000012e0: 4d00 0000 724e 0000 0072 4f00 0000 7250  M...rN...rO...rP
-000012f0: 0000 0072 5100 0000 5a0e 6865 6c70 5f61  ...rQ...Z.help_a
-00001300: 6c6c 5f66 6c61 6773 a901 da09 5f5f 636c  ll_flags....__cl
-00001310: 6173 735f 5f72 5300 0000 7257 0000 0072  ass__rS...rW...r
-00001320: 6900 0000 5300 0000 73a0 0000 0006 0e02  i...S...s.......
-00001330: 0102 010a 0102 0102 0104 fb02 0606 fa06  ................
-00001340: 0908 0308 0208 0104 020a 0106 0104 010c  ................
-00001350: 0102 0102 0108 fd06 060a 0504 fd06 0504  ................
-00001360: 0204 010e 0104 0102 0102 0102 0108 fd08  ................
-00001370: 0606 0104 020a 0106 010a 020a 010e 011c  ................
-00001380: ff04 0304 0102 0102 0108 0102 0108 fc08  ................
-00001390: 0706 0108 020a 0106 0104 0202 0104 0104  ................
-000013a0: 0102 0102 0108 fb08 0806 0108 020a 0106  ................
-000013b0: 011a 0208 0102 0102 0106 0102 010a fd02  ................
-000013c0: 0602 0102 0102 010a fd04 c608 2e7a 1741  .............z.A
-000013d0: 7267 756d 656e 7450 6172 7365 722e 5f5f  rgumentParser.__
-000013e0: 696e 6974 5f5f da07 6d65 7373 6167 6563  init__..messagec
-000013f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001400: 0600 0000 4300 0000 7324 0000 007c 00a0  ....C...s$...|..
-00001410: 0074 016a 02a1 0101 007c 00a0 0364 0164  .t.j.....|...d.d
-00001420: 027c 019b 0064 039d 03a1 0201 0064 0053  .|...d.......d.S
-00001430: 0029 044e e902 0000 007a 0765 7272 6f72  .).N.....z.error
-00001440: 3a20 da01 0a29 04da 0b70 7269 6e74 5f75  : ...)...print_u
-00001450: 7361 6765 da03 7379 73da 0673 7464 6572  sage..sys..stder
-00001460: 72da 0465 7869 7429 0272 7800 0000 727b  r..exit).rx...r{
-00001470: 0000 0072 5300 0000 7253 0000 0072 5700  ...rS...rS...rW.
-00001480: 0000 da05 6572 726f 72c4 0000 0073 0400  ....error....s..
-00001490: 0000 0c01 1801 7a14 4172 6775 6d65 6e74  ......z.Argument
-000014a0: 5061 7273 6572 2e65 7272 6f72 da04 6669  Parser.error..fi
-000014b0: 6c65 da10 696e 636c 7564 655f 636f 6d6d  le..include_comm
-000014c0: 616e 6473 da06 7265 7475 726e 6303 0000  ands..returnc...
-000014d0: 0000 0000 0000 0000 0008 0000 0005 0000  ................
-000014e0: 0003 0000 0073 9c00 0000 6401 7d03 7c03  .....s....d.}.|.
-000014f0: 6402 1400 6403 1700 7d04 7400 8300 0100  d...d...}.t.....
-00001500: 7400 7c04 8301 0100 7400 6404 7c00 6a01  t.|.....t.d.|.j.
-00001510: 9b00 9d02 8301 0100 7400 7c04 8301 0100  ........t.|.....
-00001520: 7c00 6a02 7d05 7403 6a04 7c00 5f02 7405  |.j.}.t.j.|._.t.
-00001530: 8300 a006 7c01 a101 0100 7c02 7249 7c00  ....|.....|.rI|.
-00001540: 6a07 7249 7c00 6a08 6405 7500 7237 7c00  j.rI|.j.d.u.r7|.
-00001550: a009 a100 7c00 5f08 7c00 6a08 6a0a a00b  ....|._.|.j.j...
-00001560: a100 4400 5d0b 5c02 7d06 7d07 7c07 6a06  ..D.].\.}.}.|.j.
-00001570: 7c01 7c02 6406 8d02 0100 713d 7c05 7c00  |.|.d.....q=|.|.
-00001580: 5f02 6405 5300 2907 6118 0200 0050 7269  _.d.S.).a....Pri
-00001590: 6e74 2043 4c49 2068 656c 702e 0a0a 2020  nt CLI help...  
-000015a0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-000015b0: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-000015c0: 636f 6d6d 616e 6473 3a20 6966 2054 7275  commands: if Tru
-000015d0: 652c 2061 6c73 6f20 7072 696e 7420 6865  e, also print he
-000015e0: 6c70 2066 6f72 2065 6163 6820 636f 6d6d  lp for each comm
-000015f0: 616e 642e 0a0a 2020 2020 2020 2020 4578  and...        Ex
-00001600: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00001610: 2020 2020 3e3e 3e20 696d 706f 7274 2079      >>> import y
-00001620: 6170 780a 2020 2020 2020 2020 2020 2020  apx.            
-00001630: 3e3e 3e20 6672 6f6d 2064 6174 6163 6c61  >>> from datacla
-00001640: 7373 6573 2069 6d70 6f72 7420 6461 7461  sses import data
-00001650: 636c 6173 730a 2020 2020 2020 2020 2020  class.          
-00001660: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00001670: 2020 3e3e 3e20 4064 6174 6163 6c61 7373    >>> @dataclass
-00001680: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00001690: 2063 6c61 7373 2041 6464 4e75 6d73 3a0a   class AddNums:.
-000016a0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
-000016b0: 2020 2020 783a 2069 6e74 0a20 2020 2020      x: int.     
-000016c0: 2020 2020 2020 202e 2e2e 2020 2020 2079         ...     y
-000016d0: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
-000016e0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-000016f0: 2020 3e3e 3e20 7061 7273 6572 203d 2079    >>> parser = y
-00001700: 6170 782e 4172 6775 6d65 6e74 5061 7273  apx.ArgumentPars
-00001710: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-00001720: 203e 3e3e 2070 6172 7365 722e 6164 645f   >>> parser.add_
-00001730: 6172 6775 6d65 6e74 7328 4164 644e 756d  arguments(AddNum
-00001740: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
-00001750: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
-00001760: 3e3e 2070 6172 7365 722e 7072 696e 745f  >> parser.print_
-00001770: 6865 6c70 2869 6e63 6c75 6465 5f63 6f6d  help(include_com
-00001780: 6d61 6e64 733d 5472 7565 2920 2023 646f  mands=True)  #do
-00001790: 6374 6573 743a 202b 534b 4950 0a20 2020  ctest: +SKIP.   
-000017a0: 2020 2020 20da 015f e950 0000 0072 7d00       .._.P...r}.
-000017b0: 0000 7a02 2420 4e29 0172 8400 0000 290c  ..z.$ N).r....).
-000017c0: da05 7072 696e 7472 4700 0000 da05 7573  ..printrG.....us
-000017d0: 6167 6572 7400 0000 7275 0000 0072 6800  agert...ru...rh.
-000017e0: 0000 da0a 7072 696e 745f 6865 6c70 da0b  ....print_help..
-000017f0: 5f73 7562 7061 7273 6572 7372 6a00 0000  _subparsersrj...
-00001800: da17 5f66 696e 645f 7375 6270 6172 7365  .._find_subparse
-00001810: 7273 5f61 6374 696f 6e72 6400 0000 da05  rs_actionrd.....
-00001820: 6974 656d 7329 0872 7800 0000 7283 0000  items).rx...r...
-00001830: 0072 8400 0000 5a08 7365 705f 6368 6172  .r....Z.sep_char
-00001840: da09 7365 7061 7261 746f 7272 8900 0000  ..separatorr....
-00001850: 5a07 5f63 686f 6963 655a 0973 7562 7061  Z._choiceZ.subpa
-00001860: 7273 6572 7279 0000 0072 5300 0000 7257  rserry...rS...rW
-00001870: 0000 0072 8a00 0000 c800 0000 731e 0000  ...r........s...
-00001880: 0004 180c 0106 0108 0110 0108 0106 0308  ................
-00001890: 010c 020a 020a 010a 0114 0210 010a 027a  ...............z
-000018a0: 1941 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
-000018b0: 7072 696e 745f 6865 6c70 da0a 6172 6773  print_help..args
-000018c0: 5f6d 6f64 656c 2e63 0200 0000 0000 0000  _model.c........
-000018d0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-000018e0: 7310 0000 007c 00a0 007c 007c 01a1 0201  s....|...|.|....
-000018f0: 0064 0153 0029 0261 d605 0000 4164 6420  .d.S.).a....Add 
-00001900: 6172 6775 6d65 6e74 7320 6672 6f6d 2074  arguments from t
-00001910: 6865 2067 6976 656e 2066 756e 6374 696f  he given functio
-00001920: 6e20 6f72 2064 6174 6166 7261 6d65 2e0a  n or dataframe..
-00001930: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00001940: 2020 2020 2020 2020 2020 2061 7267 735f             args_
-00001950: 6d6f 6465 6c3a 2061 2066 756e 6374 696f  model: a functio
-00001960: 6e20 6f72 2064 6174 6163 6c61 7373 2066  n or dataclass f
-00001970: 726f 6d20 7768 6963 6820 746f 2064 6572  rom which to der
-00001980: 6976 6520 6172 6775 6d65 6e74 732e 0a0a  ive arguments...
-00001990: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-000019a0: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
-000019b0: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
-000019c0: 2020 2020 2020 2020 2020 3e3e 3e20 6672            >>> fr
-000019d0: 6f6d 2064 6174 6163 6c61 7373 6573 2069  om dataclasses i
-000019e0: 6d70 6f72 7420 6461 7461 636c 6173 730a  mport dataclass.
-000019f0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00001a00: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00001a10: 4064 6174 6163 6c61 7373 0a20 2020 2020  @dataclass.     
-00001a20: 2020 2020 2020 202e 2e2e 2063 6c61 7373         ... class
-00001a30: 2041 6464 4e75 6d73 3a0a 2020 2020 2020   AddNums:.      
-00001a40: 2020 2020 2020 2e2e 2e20 2020 2020 783a        ...     x:
-00001a50: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-00001a60: 202e 2e2e 2020 2020 2079 3a20 696e 740a   ...     y: int.
-00001a70: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00001a80: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00001a90: 7061 7273 6572 203d 2079 6170 782e 4172  parser = yapx.Ar
-00001aa0: 6775 6d65 6e74 5061 7273 6572 2829 0a20  gumentParser(). 
-00001ab0: 2020 2020 2020 2020 2020 203e 3e3e 2070             >>> p
-00001ac0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00001ad0: 6e74 7328 4164 644e 756d 7329 0a20 2020  nts(AddNums).   
-00001ae0: 2020 2020 2020 2020 203e 3e3e 2070 6172           >>> par
-00001af0: 7365 722e 7365 745f 6465 6661 756c 7473  ser.set_defaults
-00001b00: 285f 636f 6d6d 616e 645f 6675 6e63 3d6c  (_command_func=l
-00001b10: 616d 6264 6120 782c 2079 3a20 782b 7929  ambda x, y: x+y)
-00001b20: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00001b30: 2070 6172 7365 6420 3d20 7061 7273 6572   parsed = parser
-00001b40: 2e70 6172 7365 5f61 7267 7328 5b27 2d78  .parse_args(['-x
-00001b50: 272c 2027 3127 2c20 272d 7927 2c20 2732  ', '1', '-y', '2
-00001b60: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
-00001b70: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00001b80: 3e3e 3e20 2870 6172 7365 642e 782c 2070  >>> (parsed.x, p
-00001b90: 6172 7365 642e 7929 0a20 2020 2020 2020  arsed.y).       
-00001ba0: 2020 2020 2028 312c 2032 290a 2020 2020       (1, 2).    
-00001bb0: 2020 2020 2020 2020 3e3e 3e20 7061 7273          >>> pars
-00001bc0: 6564 2e5f 636f 6d6d 616e 645f 6675 6e63  ed._command_func
-00001bd0: 5f61 7267 735f 6d6f 6465 6c28 783d 7061  _args_model(x=pa
-00001be0: 7273 6564 2e78 2c20 793d 7061 7273 6564  rsed.x, y=parsed
-00001bf0: 2e79 290a 2020 2020 2020 2020 2020 2020  .y).            
-00001c00: 4164 644e 756d 7328 783d 312c 2079 3d32  AddNums(x=1, y=2
-00001c10: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-00001c20: 3e20 7061 7273 6564 2e5f 636f 6d6d 616e  > parsed._comman
-00001c30: 645f 6675 6e63 2878 3d70 6172 7365 642e  d_func(x=parsed.
-00001c40: 782c 2079 3d70 6172 7365 642e 7929 0a20  x, y=parsed.y). 
-00001c50: 2020 2020 2020 2020 2020 2033 0a0a 2020             3..  
-00001c60: 2020 2020 2020 2020 2020 3e3e 3e20 696d            >>> im
-00001c70: 706f 7274 2079 6170 780a 2020 2020 2020  port yapx.      
-00001c80: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00001c90: 2020 2020 2020 3e3e 3e20 6465 6620 6164        >>> def ad
-00001ca0: 645f 6e75 6d73 2878 3a20 696e 742c 2079  d_nums(x: int, y
-00001cb0: 3a20 696e 7429 3a0a 2020 2020 2020 2020  : int):.        
-00001cc0: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
-00001cd0: 726e 2078 202b 2079 0a20 2020 2020 2020  rn x + y.       
-00001ce0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00001cf0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
-00001d00: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
-00001d10: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
-00001d20: 2020 2020 3e3e 3e20 7061 7273 6572 2e61      >>> parser.a
-00001d30: 6464 5f61 7267 756d 656e 7473 2861 6464  dd_arguments(add
-00001d40: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
-00001d50: 2020 203e 3e3e 2070 6172 7365 722e 7365     >>> parser.se
-00001d60: 745f 6465 6661 756c 7473 285f 636f 6d6d  t_defaults(_comm
-00001d70: 616e 645f 6675 6e63 3d61 6464 5f6e 756d  and_func=add_num
-00001d80: 7329 0a20 2020 2020 2020 2020 2020 203e  s).            >
-00001d90: 3e3e 2070 6172 7365 6420 3d20 7061 7273  >> parsed = pars
-00001da0: 6572 2e70 6172 7365 5f61 7267 7328 5b27  er.parse_args(['
-00001db0: 2d78 272c 2027 3127 2c20 272d 7927 2c20  -x', '1', '-y', 
-00001dc0: 2732 275d 290a 2020 2020 2020 2020 2020  '2']).          
-00001dd0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00001de0: 2020 3e3e 3e20 2870 6172 7365 642e 782c    >>> (parsed.x,
-00001df0: 2070 6172 7365 642e 7929 0a20 2020 2020   parsed.y).     
-00001e00: 2020 2020 2020 2028 312c 2032 290a 2020         (1, 2).  
-00001e10: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
-00001e20: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
-00001e30: 6e63 5f61 7267 735f 6d6f 6465 6c28 783d  nc_args_model(x=
-00001e40: 7061 7273 6564 2e78 2c20 793d 7061 7273  parsed.x, y=pars
-00001e50: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
-00001e60: 2020 4461 7461 636c 6173 735f 6164 645f    Dataclass_add_
-00001e70: 6e75 6d73 2878 3d31 2c20 793d 3229 0a20  nums(x=1, y=2). 
-00001e80: 2020 2020 2020 2020 2020 203e 3e3e 2070             >>> p
-00001e90: 6172 7365 642e 5f63 6f6d 6d61 6e64 5f66  arsed._command_f
-00001ea0: 756e 6328 783d 7061 7273 6564 2e78 2c20  unc(x=parsed.x, 
-00001eb0: 793d 7061 7273 6564 2e79 290a 2020 2020  y=parsed.y).    
-00001ec0: 2020 2020 2020 2020 330a 2020 2020 2020          3.      
-00001ed0: 2020 4e29 01da 0e5f 6164 645f 6172 6775    N)..._add_argu
-00001ee0: 6d65 6e74 7329 0272 7800 0000 728f 0000  ments).rx...r...
-00001ef0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
-00001f00: da0d 6164 645f 6172 6775 6d65 6e74 73f6  ..add_arguments.
-00001f10: 0000 0073 0200 0000 102f 7a1c 4172 6775  ...s...../z.Argu
-00001f20: 6d65 6e74 5061 7273 6572 2e61 6464 5f61  mentParser.add_a
-00001f30: 7267 756d 656e 7473 da04 6e61 6d65 6303  rguments..namec.
-00001f40: 0000 0000 0000 0000 0000 0009 0000 0005  ................
-00001f50: 0000 004b 0000 0073 9800 0000 7c00 a000  ...K...s....|...
-00001f60: a100 7d04 7c02 730b 7401 7c01 6a02 8301  ..}.|.s.t.|.j...
-00001f70: 7d02 7403 7c04 7404 6a05 8302 7313 4a00  }.t.|.t.j...s.J.
-00001f80: 8201 7c03 a006 6401 6402 a102 7d05 7c05  ..|...d.d...}.|.
-00001f90: 7221 7c05 6403 7c02 1700 3700 7d05 7c00  r!|.d.|...7.}.|.
-00001fa0: 6a07 7c01 6404 8d01 7d06 6402 7d07 7c06  j.|.d...}.d.}.|.
-00001fb0: 7231 7c06 a008 a100 6405 1900 7d07 7c04  r1|.....d...}.|.
-00001fc0: 6a09 7c02 6601 7c05 7c07 6406 9c02 7c03  j.|.f.|.|.d...|.
-00001fd0: a401 8e01 7d08 7c06 7242 7c06 7c08 5f0a  ....}.|.rB|.|._.
-00001fe0: 7c01 724a 7c00 a00b 7c08 7c01 a102 0100  |.rJ|...|.|.....
-00001ff0: 7c08 5300 2907 6159 0800 0043 7265 6174  |.S.).aY...Creat
-00002000: 6520 6120 6e65 7720 7375 6263 6f6d 6d61  e a new subcomma
-00002010: 6e64 2061 6e64 2061 6464 2061 7267 756d  nd and add argum
-00002020: 656e 7473 2066 726f 6d20 7468 6520 6769  ents from the gi
-00002030: 7665 6e20 6675 6e63 7469 6f6e 206f 7220  ven function or 
-00002040: 6461 7461 6672 616d 6520 746f 2069 742e  dataframe to it.
-00002050: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00002060: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00002070: 5f6d 6f64 656c 3a20 6120 6675 6e63 7469  _model: a functi
-00002080: 6f6e 206f 7220 6461 7461 636c 6173 7320  on or dataclass 
-00002090: 6672 6f6d 2077 6869 6368 2074 6f20 6465  from which to de
-000020a0: 7269 7665 2061 7267 756d 656e 7473 2e0a  rive arguments..
-000020b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-000020c0: 3a20 6e61 6d65 206f 6620 7468 6520 636f  : name of the co
-000020d0: 6d6d 616e 640a 0a20 2020 2020 2020 2052  mmand..        R
-000020e0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000020f0: 2020 2020 7468 6520 6e65 7720 6172 6770      the new argp
-00002100: 6172 7365 2073 7562 7061 7273 6572 0a0a  arse subparser..
-00002110: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-00002120: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
-00002130: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
-00002140: 2020 2020 2020 2020 2020 3e3e 3e20 6672            >>> fr
-00002150: 6f6d 2064 6174 6163 6c61 7373 6573 2069  om dataclasses i
-00002160: 6d70 6f72 7420 6461 7461 636c 6173 730a  mport dataclass.
-00002170: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00002180: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00002190: 4064 6174 6163 6c61 7373 0a20 2020 2020  @dataclass.     
-000021a0: 2020 2020 2020 202e 2e2e 2063 6c61 7373         ... class
-000021b0: 2041 6464 4e75 6d73 3a0a 2020 2020 2020   AddNums:.      
-000021c0: 2020 2020 2020 2e2e 2e20 2020 2020 783a        ...     x:
-000021d0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-000021e0: 202e 2e2e 2020 2020 2079 3a20 696e 740a   ...     y: int.
-000021f0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00002200: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00002210: 7061 7273 6572 203d 2079 6170 782e 4172  parser = yapx.Ar
-00002220: 6775 6d65 6e74 5061 7273 6572 2829 0a20  gumentParser(). 
-00002230: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
-00002240: 7562 7061 7273 6572 5f31 203d 2070 6172  ubparser_1 = par
-00002250: 7365 722e 6164 645f 636f 6d6d 616e 6428  ser.add_command(
-00002260: 4164 644e 756d 732c 206e 616d 653d 2761  AddNums, name='a
-00002270: 6464 2729 0a20 2020 2020 2020 2020 2020  dd').           
-00002280: 203e 3e3e 2073 7562 7061 7273 6572 5f31   >>> subparser_1
-00002290: 2e73 6574 5f64 6566 6175 6c74 7328 5f63  .set_defaults(_c
-000022a0: 6f6d 6d61 6e64 5f66 756e 633d 6c61 6d62  ommand_func=lamb
-000022b0: 6461 2078 2c20 793a 2078 2b79 290a 2020  da x, y: x+y).  
-000022c0: 2020 2020 2020 2020 2020 3e3e 3e20 7375            >>> su
-000022d0: 6270 6172 7365 725f 3220 3d20 7061 7273  bparser_2 = pars
-000022e0: 6572 2e61 6464 5f63 6f6d 6d61 6e64 2841  er.add_command(A
-000022f0: 6464 4e75 6d73 2c20 6e61 6d65 3d27 7375  ddNums, name='su
-00002300: 6274 7261 6374 2729 0a20 2020 2020 2020  btract').       
-00002310: 2020 2020 203e 3e3e 2073 7562 7061 7273       >>> subpars
-00002320: 6572 5f32 2e73 6574 5f64 6566 6175 6c74  er_2.set_default
-00002330: 7328 5f63 6f6d 6d61 6e64 5f66 756e 633d  s(_command_func=
-00002340: 6c61 6d62 6461 2078 2c20 793a 2078 2d79  lambda x, y: x-y
-00002350: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
-00002360: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00002370: 3e20 7061 7273 6564 203d 2070 6172 7365  > parsed = parse
-00002380: 722e 7061 7273 655f 6172 6773 285b 2761  r.parse_args(['a
-00002390: 6464 272c 2027 2d78 272c 2027 3127 2c20  dd', '-x', '1', 
-000023a0: 272d 7927 2c20 2732 275d 290a 2020 2020  '-y', '2']).    
-000023b0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-000023c0: 2020 2020 2020 2020 3e3e 3e20 2870 6172          >>> (par
-000023d0: 7365 642e 782c 2070 6172 7365 642e 7929  sed.x, parsed.y)
-000023e0: 0a20 2020 2020 2020 2020 2020 2028 312c  .            (1,
-000023f0: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
-00002400: 3e3e 3e20 7061 7273 6564 2e5f 636f 6d6d  >>> parsed._comm
-00002410: 616e 645f 6675 6e63 5f61 7267 735f 6d6f  and_func_args_mo
-00002420: 6465 6c28 783d 7061 7273 6564 2e78 2c20  del(x=parsed.x, 
-00002430: 793d 7061 7273 6564 2e79 290a 2020 2020  y=parsed.y).    
-00002440: 2020 2020 2020 2020 4164 644e 756d 7328          AddNums(
-00002450: 783d 312c 2079 3d32 290a 2020 2020 2020  x=1, y=2).      
-00002460: 2020 2020 2020 3e3e 3e20 7061 7273 6564        >>> parsed
-00002470: 2e5f 636f 6d6d 616e 645f 6675 6e63 2878  ._command_func(x
-00002480: 3d70 6172 7365 642e 782c 2079 3d70 6172  =parsed.x, y=par
-00002490: 7365 642e 7929 0a20 2020 2020 2020 2020  sed.y).         
-000024a0: 2020 2033 0a0a 2020 2020 2020 2020 2020     3..          
-000024b0: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
-000024c0: 780a 2020 2020 2020 2020 2020 2020 2e2e  x.            ..
-000024d0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-000024e0: 3e20 6465 6620 6164 645f 6e75 6d73 2878  > def add_nums(x
-000024f0: 3a20 696e 742c 2079 3a20 696e 7429 3a0a  : int, y: int):.
-00002500: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
-00002510: 2020 2020 7265 7475 726e 2078 202b 2079      return x + y
-00002520: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00002530: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00002540: 2064 6566 2073 7562 7472 6163 745f 6e75   def subtract_nu
-00002550: 6d73 2878 3a20 696e 742c 2079 3a20 696e  ms(x: int, y: in
-00002560: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00002570: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
-00002580: 202d 2079 0a20 2020 2020 2020 2020 2020   - y.           
-00002590: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-000025a0: 203e 3e3e 2070 6172 7365 7220 3d20 7961   >>> parser = ya
-000025b0: 7078 2e41 7267 756d 656e 7450 6172 7365  px.ArgumentParse
-000025c0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-000025d0: 3e3e 3e20 7375 6270 6172 7365 725f 3120  >>> subparser_1 
-000025e0: 3d20 7061 7273 6572 2e61 6464 5f63 6f6d  = parser.add_com
-000025f0: 6d61 6e64 2861 6464 5f6e 756d 732c 206e  mand(add_nums, n
-00002600: 616d 653d 2761 6464 2729 0a20 2020 2020  ame='add').     
-00002610: 2020 2020 2020 203e 3e3e 2073 7562 7061         >>> subpa
-00002620: 7273 6572 5f31 2e73 6574 5f64 6566 6175  rser_1.set_defau
-00002630: 6c74 7328 5f63 6f6d 6d61 6e64 5f66 756e  lts(_command_fun
-00002640: 633d 6164 645f 6e75 6d73 290a 2020 2020  c=add_nums).    
-00002650: 2020 2020 2020 2020 3e3e 3e20 7375 6270          >>> subp
-00002660: 6172 7365 725f 3220 3d20 7061 7273 6572  arser_2 = parser
-00002670: 2e61 6464 5f63 6f6d 6d61 6e64 2873 7562  .add_command(sub
-00002680: 7472 6163 745f 6e75 6d73 2c20 6e61 6d65  tract_nums, name
-00002690: 3d27 7375 6274 7261 6374 2729 0a20 2020  ='subtract').   
-000026a0: 2020 2020 2020 2020 203e 3e3e 2073 7562           >>> sub
-000026b0: 7061 7273 6572 5f32 2e73 6574 5f64 6566  parser_2.set_def
-000026c0: 6175 6c74 7328 5f63 6f6d 6d61 6e64 5f66  aults(_command_f
-000026d0: 756e 633d 7375 6274 7261 6374 5f6e 756d  unc=subtract_num
-000026e0: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
-000026f0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
-00002700: 3e3e 2070 6172 7365 6420 3d20 7061 7273  >> parsed = pars
-00002710: 6572 2e70 6172 7365 5f61 7267 7328 5b27  er.parse_args(['
-00002720: 7375 6274 7261 6374 272c 2027 2d78 272c  subtract', '-x',
-00002730: 2027 3127 2c20 272d 7927 2c20 2732 275d   '1', '-y', '2']
-00002740: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
-00002750: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00002760: 3e20 2870 6172 7365 642e 782c 2070 6172  > (parsed.x, par
-00002770: 7365 642e 7929 0a20 2020 2020 2020 2020  sed.y).         
-00002780: 2020 2028 312c 2032 290a 2020 2020 2020     (1, 2).      
-00002790: 2020 2020 2020 3e3e 3e20 7061 7273 6564        >>> parsed
-000027a0: 2e5f 636f 6d6d 616e 645f 6675 6e63 5f61  ._command_func_a
-000027b0: 7267 735f 6d6f 6465 6c28 783d 7061 7273  rgs_model(x=pars
-000027c0: 6564 2e78 2c20 793d 7061 7273 6564 2e79  ed.x, y=parsed.y
-000027d0: 290a 2020 2020 2020 2020 2020 2020 4461  ).            Da
-000027e0: 7461 636c 6173 735f 7375 6274 7261 6374  taclass_subtract
-000027f0: 5f6e 756d 7328 783d 312c 2079 3d32 290a  _nums(x=1, y=2).
-00002800: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00002810: 7061 7273 6564 2e5f 636f 6d6d 616e 645f  parsed._command_
-00002820: 6675 6e63 2878 3d70 6172 7365 642e 782c  func(x=parsed.x,
-00002830: 2079 3d70 6172 7365 642e 7929 0a20 2020   y=parsed.y).   
-00002840: 2020 2020 2020 2020 202d 310a 2020 2020           -1.    
-00002850: 2020 2020 7247 0000 004e fa01 20a9 0172      rG...N.. ..r
-00002860: 8f00 0000 7201 0000 0029 0272 4700 0000  ....r....).rG...
-00002870: 725a 0000 0029 0c72 7700 0000 7224 0000  rZ...).rw...r$..
-00002880: 00da 085f 5f6e 616d 655f 5f72 6d00 0000  ...__name__rm...
-00002890: 7274 0000 00da 115f 5375 6250 6172 7365  rt....._SubParse
-000028a0: 7273 4163 7469 6f6e da03 706f 70da 1f5f  rsAction..pop.._
-000028b0: 6765 745f 6465 7363 7269 7074 696f 6e5f  get_description_
-000028c0: 6672 6f6d 5f64 6f63 7374 7269 6e67 da0a  from_docstring..
-000028d0: 7370 6c69 746c 696e 6573 da0a 6164 645f  splitlines..add_
-000028e0: 7061 7273 6572 7249 0000 0072 9000 0000  parserrI...r....
-000028f0: 2909 7278 0000 0072 8f00 0000 7292 0000  ).rx...r....r...
-00002900: 0072 5100 0000 5a0a 7375 6270 6172 7365  .rQ...Z.subparse
-00002910: 7273 7247 0000 005a 0f64 6573 6372 6970  rsrG...Z.descrip
-00002920: 7469 6f6e 5f74 7874 5a08 6865 6c70 5f74  tion_txtZ.help_t
-00002930: 7874 7266 0000 0072 5300 0000 7253 0000  xtrf...rS...rS..
-00002940: 0072 5700 0000 da0b 6164 645f 636f 6d6d  .rW.....add_comm
-00002950: 616e 6427 0100 0073 3400 0000 083e 0402  and'...s4....>..
-00002960: 0a01 1003 0c01 0401 0c01 0404 0201 06ff  ................
-00002970: 0403 0401 0c01 0402 0201 02ff 0202 0201  ................
-00002980: 04fd 0204 06fc 0406 0601 0402 0c01 0402  ................
-00002990: 7a1a 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
-000029a0: 2e61 6464 5f63 6f6d 6d61 6e64 da04 6675  .add_command..fu
-000029b0: 6e63 6303 0000 0000 0000 0000 0000 0005  ncc.............
-000029c0: 0000 0005 0000 004b 0000 0073 4200 0000  .......K...sB...
-000029d0: 7400 7c02 7205 7c02 6e02 7c01 6a01 8301  t.|.r.|.n.|.j...
-000029e0: 7d02 7c00 6a02 7c01 6601 6401 7c02 6901  }.|.j.|.f.d.|.i.
-000029f0: 7c03 a401 8e01 7d04 7c04 6a03 6402 6900  |.....}.|.j.d.i.
-00002a00: 7c00 6a04 7c01 6901 a401 8e01 0100 6400  |.j.|.i.......d.
-00002a10: 5300 2903 4e72 9200 0000 7253 0000 0029  S.).Nr....rS...)
-00002a20: 0572 2400 0000 7295 0000 0072 9b00 0000  .r$...r....r....
-00002a30: da0c 7365 745f 6465 6661 756c 7473 7245  ..set_defaultsrE
-00002a40: 0000 0029 0572 7800 0000 729c 0000 0072  ...).rx...r....r
-00002a50: 9200 0000 7251 0000 0072 6600 0000 7253  ....rQ...rf...rS
-00002a60: 0000 0072 5300 0000 7257 0000 00da 115f  ...rS...rW....._
-00002a70: 7265 6769 7374 6572 5f63 6f6d 6d61 6e64  register_command
-00002a80: 8701 0000 7312 0000 0012 0604 0102 0104  ....s...........
-00002a90: ff02 0202 fe02 0306 fd1a 057a 2041 7267  ...........z Arg
-00002aa0: 756d 656e 7450 6172 7365 722e 5f72 6567  umentParser._reg
-00002ab0: 6973 7465 725f 636f 6d6d 616e 64da 0464  ister_command..d
-00002ac0: 636c 73da 0461 7474 7263 0200 0000 0000  cls..attrc......
-00002ad0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00002ae0: 0000 730a 0000 007c 017c 006a 0076 0153  ..s....|.|.j.v.S
-00002af0: 0072 5c00 0000 a901 da0f 5f5f 616e 6e6f  .r\.......__anno
-00002b00: 7461 7469 6f6e 735f 5fa9 0272 9f00 0000  tations__..r....
-00002b10: 72a0 0000 0072 5300 0000 7253 0000 0072  r....rS...rS...r
-00002b20: 5700 0000 da17 5f69 735f 6174 7472 6962  W....._is_attrib
-00002b30: 7574 655f 696e 6865 7269 7465 6495 0100  ute_inherited...
-00002b40: 0073 0200 0000 0a02 7a26 4172 6775 6d65  .s......z&Argume
-00002b50: 6e74 5061 7273 6572 2e5f 6973 5f61 7474  ntParser._is_att
-00002b60: 7269 6275 7465 5f69 6e68 6572 6974 6564  ribute_inherited
-00002b70: 7266 0000 0063 0300 0000 0000 0000 0000  rf...c..........
-00002b80: 0000 1900 0000 0900 0000 0300 0000 73f2  ..............s.
-00002b90: 0600 0074 007c 0283 0172 077c 0289 016e  ...t.|...r.|...n
-00002ba0: 0474 017c 0283 0189 017c 01a0 0288 006a  .t.|.....|.....j
-00002bb0: 03a1 0172 1864 017d 037c 01a0 047c 03a1  ...r.d.}.|...|..
-00002bc0: 0101 007c 016a 0564 2269 0088 006a 0388  ...|.j.d"i...j..
-00002bd0: 0169 01a4 018e 0101 0069 007d 0474 0674  .i.......i.}.t.t
-00002be0: 0787 0087 0166 0264 0264 0384 0874 0888  .....f.d.d...t..
-00002bf0: 0183 0183 0283 017d 0564 0464 0584 007c  .......}.d.d...|
-00002c00: 0544 0083 017d 0667 007d 077c 0644 0090  .D...}.g.}.|.D..
-00002c10: 035d 375c 027d 087d 097c 086a 097d 0a74  .]7\.}.}.|.j.}.t
-00002c20: 0a7c 0a74 0b83 0272 4f74 0c7c 0a83 017d  .|.t...rOt.|...}
-00002c30: 0a74 0a7c 0a74 0b83 0272 564a 0082 0174  .t.|.t...rVJ...t
-00002c40: 0d6a 0e64 066b 0572 6074 0a7c 0a74 0f83  .j.d.k.r`t.|.t..
-00002c50: 0273 6788 00a0 107c 0aa1 0174 1175 0072  .sg....|...t.u.r
-00002c60: 6e88 006a 127c 0a64 0764 088d 027d 0a74  n..j.|.d.d...}.t
-00002c70: 0a7c 0a74 1383 0272 a988 00a0 147c 0aa1  .|.t...r.....|..
-00002c80: 0144 005d 137d 0b74 157c 0b74 1683 0272  .D.].}.t.|.t...r
-00002c90: 8b74 177c 0b6a 1876 0072 8b7c 0b6a 1874  .t.|.j.v.r.|.j.t
-00002ca0: 1719 007d 0901 006e 0171 7888 00a0 107c  ...}...n.qx....|
-00002cb0: 0aa1 017d 0a74 0d6a 0e64 066b 0572 9b74  ...}.t.j.d.k.r.t
-00002cc0: 0a7c 0a74 0f83 0273 a288 00a0 107c 0aa1  .|.t...s.....|..
-00002cd0: 0174 1175 0072 a988 006a 127c 0a64 0764  .t.u.r...j.|.d.d
-00002ce0: 088d 027d 0a74 0a7c 0a74 0983 0272 b17c  ...}.t.|.t...r.|
-00002cf0: 0a6a 196e 0a74 0b7c 0a83 016a 1a64 0964  .j.n.t.|...j.d.d
-00002d00: 0a64 0b8d 0264 0c19 007d 0c7c 09a0 1b7c  .d...d...}.|...|
-00002d10: 086a 1ca1 0101 007c 096a 1d72 df7c 086a  .j.....|.j.r.|.j
-00002d20: 1e74 1f75 0172 d27c 086a 1e7c 095f 1e64  .t.u.r.|.j.|._.d
-00002d30: 0d7c 095f 1d6e 0d7c 086a 2074 1f75 0172  .|._.n.|.j t.u.r
-00002d40: df7c 08a0 20a1 007c 095f 1e64 0d7c 095f  .|.. ..|._.d.|._
-00002d50: 1d88 00a0 107c 0aa1 017d 0d7c 0d90 0172  .....|...}.|...r
-00002d60: 6f7c 0d90 0172 037c 0d74 2175 0090 0172  o|...r.|.t!u...r
-00002d70: 0374 0688 00a0 227c 0aa1 0183 017c 095f  .t...."|.....|._
-00002d80: 237c 096a 2390 0172 0274 097c 096a 2364  #|.j#..r.t.|.j#d
-00002d90: 0e19 0083 017d 0a6e 7774 247c 0d74 256a  .....}.nwt$|.t%j
-00002da0: 266a 2783 0290 0172 1a88 006a 127c 0a64  &j'....r...j.|.d
-00002db0: 0764 0f8d 027d 0a7c 096a 2890 0173 1974  .d...}.|.j(..s.t
-00002dc0: 297c 095f 286e 3574 247c 0d74 256a 266a  )|._(n5t$|.t%j&j
-00002dd0: 2a83 0290 0173 277c 0d74 2b75 0090 0172  *....s'|.t+u...r
-00002de0: 4888 006a 127c 0a64 0764 0f8d 027d 0a7c  H..j.|.d.d...}.|
-00002df0: 096a 2890 0173 477c 0d74 2b75 0090 0172  .j(..sG|.t+u...r
-00002e00: 3b74 2c7c 095f 286e 147c 0d74 2d75 0090  ;t,|._(n.|.t-u..
-00002e10: 0172 4474 2e7c 095f 286e 0b74 2f7c 095f  .rDt.|._(n.t/|._
-00002e20: 286e 0774 3090 0173 4f74 317c 0a83 0101  (n.t0..sOt1|....
-00002e30: 0074 247c 0a74 3283 0290 0172 5d64 1064  .t$|.t2....r]d.d
-00002e40: 0584 007c 0a44 0083 017c 095f 2374 157c  ...|.D...|._#t.|
-00002e50: 0188 0083 0290 0172 6c74 3374 347c 0a83  .......rlt3t4|..
-00002e60: 027c 016a 357c 096a 363c 0074 0b7d 0a6e  .|.j5|.j6<.t.}.n
-00002e70: 0b74 247c 0a74 3283 0290 0172 7a74 067c  .t$|.t2....rzt.|
-00002e80: 0a83 017c 095f 237c 0a7c 095f 097c 09a0  ...|._#|.|._.|..
-00002e90: 37a1 007d 0e7c 0e64 113d 007c 0ea0 3864  7..}.|.d.=.|..8d
-00002ea0: 12a1 017d 0f7c 0f90 0173 8e67 006e 0664  ...}.|...s.g.n.d
-00002eb0: 1364 0584 007c 0f44 0083 017d 107c 0e64  .d...|.D...}.|.d
-00002ec0: 1419 0090 0173 b17c 0ea0 3964 15a1 0190  .....s.|..9d....
-00002ed0: 0173 b17c 1090 0173 ad64 167c 0e64 1719  .s.|...s.d.|.d..
-00002ee0: 00a0 3aa1 009b 0064 189d 036e 0164 197c  ..:....d...n.d.|
-00002ef0: 0e64 143c 007c 0e64 1a19 007d 117c 1090  .d.<.|.d...}.|..
-00002f00: 0173 d27c 0e64 1a3d 007c 1190 0173 ca7c  .s.|.d.=.|...s.|
-00002f10: 0ea0 3964 1ba1 0164 0075 0090 0172 ca64  ..9d...d.u...r.d
-00002f20: 1c7c 0e64 1b3c 0074 3374 347c 0a83 027c  .|.d.<.t3t4|...|
-00002f30: 0e64 1d3c 006e 4c7c 096a 0974 3b75 0090  .d.<.nL|.j.t;u..
-00002f40: 0172 fd74 157c 0188 0083 0290 0172 e774  .r.t.|.......r.t
-00002f50: 3374 347c 0a83 027c 016a 357c 096a 363c  3t4|...|.j5|.j6<
-00002f60: 0064 1e44 005d 097d 127c 0ea0 387c 1264  .d.D.].}.|..8|.d
-00002f70: 00a1 0201 0090 0171 e97c 0e64 1f19 0090  .......q.|.d....
-00002f80: 0173 fc74 3c7c 0e64 1f3c 006e 217c 096a  .s.t<|.d.<.n!|.j
-00002f90: 3d64 0e6b 0390 0272 0b74 3374 347c 0a83  =d.k...r.t3t4|..
-00002fa0: 027c 0e64 1d3c 006e 137c 0a74 3e75 0090  .|.d.<.n.|.t>u..
-00002fb0: 0272 1574 3f7c 0e64 1f3c 006e 097c 0a74  .r.t?|.d.<.n.|.t
-00002fc0: 0b75 0090 0272 1e74 407c 0e64 1f3c 007c  .u...r.t@|.d.<.|
-00002fd0: 086a 1e74 1f75 0190 0273 327c 086a 2074  .j.t.u...s2|.j t
-00002fe0: 1f75 0190 0273 327c 0ea0 3964 20a1 0164  .u...s2|..9d ..d
-00002ff0: 0075 0190 0272 c97c 0ea0 3964 1fa1 0190  .u...r.|..9d....
-00003000: 0272 6574 247c 0e64 1f19 0074 416a 4274  .ret$|.d...tAjBt
-00003010: 3c66 0283 0290 0272 6574 0964 2164 2269  <f.....ret.d!d"i
-00003020: 0083 0383 007d 137c 0e64 1f19 007c 107c  .....}.|.d...|.|
-00003030: 0e64 1719 0064 238d 027c 017c 137c 0e64  .d...d#..|.|.|.d
-00003040: 2019 0064 248d 0301 0074 437c 137c 0e64   ..d$....tC|.|.d
-00003050: 1719 0083 027c 0e64 203c 006e 0f64 1d7c  .....|.d <.n.d.|
-00003060: 0e76 0090 0272 747c 0e64 1d19 007c 0e64  .v...rt|.d...|.d
-00003070: 2019 0083 017c 0e64 203c 007c 0ea0 3964   ....|.d <.|..9d
-00003080: 15a1 0190 0272 c97c 0e64 2019 007d 1474  .....r.|.d ..}.t
-00003090: 0a7c 1474 0b83 0290 0273 8c74 0a7c 1474  .|.t.....s.t.|.t
-000030a0: 256a 266a 2a83 0290 0273 8f7c 1467 017d  %j&j*....s.|.g.}
-000030b0: 147c 1444 005d 377d 0b7c 0b7c 0e64 1519  .|.D.]7}.|.|.d..
-000030c0: 0076 0190 0272 c774 0a7c 0b74 3283 0290  .v...r.t.|.t2...
-000030d0: 0272 a87c 0b6a 1c7c 0e64 1519 0076 0190  .r.|.j.|.d...v..
-000030e0: 0272 c77c 0ea0 3964 1aa1 0190 0273 b37c  .r.|..9d.....s.|
-000030f0: 0b64 0075 0090 0273 c764 257c 0b9b 0064  .d.u...s.d%|...d
-00003100: 267c 0e64 1719 009b 0064 277c 0e64 1519  &|.d.....d'|.d..
-00003110: 009b 009d 067d 037c 01a0 047c 03a1 0101  .....}.|...|....
-00003120: 0090 0271 9164 287c 0c9b 009d 0267 017d  ...q.d(|.....g.}
-00003130: 157c 1190 0273 e674 157c 0ea0 3964 20a1  .|...s.t.|..9d .
-00003140: 0174 0b83 0290 0272 e17c 15a0 4464 29a1  .t.....r.|..Dd).
-00003150: 0101 006e 057c 15a0 4464 2aa1 0101 007c  ...n.|..Dd*....|
-00003160: 0ea0 3864 2b64 0da1 0290 0272 f27c 15a0  ..8d+d.....r.|..
-00003170: 4464 2ca1 0101 007c 096a 4590 0272 ff7c  Dd,....|.jE..r.|
-00003180: 15a0 4464 2d7c 096a 459b 009d 02a1 0101  ..Dd-|.jE.......
-00003190: 0064 2e64 2fa0 467c 15a1 019b 009d 027d  .d.d/.F|.......}
-000031a0: 167c 0ea0 3964 30a1 0190 0372 187c 0e64  .|..9d0....r.|.d
-000031b0: 3005 0019 0064 317c 1617 0037 0003 003c  0....d1|...7...<
-000031c0: 006e 047c 167c 0e64 303c 007c 0ea0 3864  .n.|.|.d0<.|..8d
-000031d0: 3264 00a1 027d 177c 1790 0373 2c7c 1190  2d...}.|...s,|..
-000031e0: 0372 2a64 336e 0164 347d 177c 04a0 397c  .r*d3n.d4}.|..9|
-000031f0: 1764 00a1 027d 187c 1890 0373 3e7c 01a0  .d...}.|...s>|..
-00003200: 477c 17a1 017d 187c 187c 047c 173c 007c  G|...}.|.|.|.<.|
-00003210: 096a 4890 0372 697c 1190 0372 5064 357c  .jH..ri|...rPd5|
-00003220: 096a 369b 009d 027d 037c 01a0 047c 03a1  .j6....}.|...|..
-00003230: 0101 007c 016a 497c 016a 4aa0 3988 006a  ...|.jI|.jJ.9..j
-00003240: 4ba1 0119 007c 1719 00a0 447c 096a 367c  K....|....D|.j6|
-00003250: 1090 0372 657c 1064 0c19 006e 0164 0066  ...re|.d...n.d.f
-00003260: 02a1 0101 007c 186a 4c7c 1069 007c 0ea4  .....|.jL|.i.|..
-00003270: 018e 0101 007c 07a0 447c 09a1 0101 0071  .....|..D|.....q
-00003280: 3e7c 0753 0029 364e 7a3e 5468 6973 2070  >|.S.)6Nz>This p
-00003290: 6172 7365 7220 616c 7265 6164 7920 636f  arser already co
-000032a0: 6e74 6169 6e73 2061 7267 756d 656e 7473  ntains arguments
-000032b0: 2066 726f 6d20 616e 6f74 6865 7220 6461   from another da
-000032c0: 7461 636c 6173 732e 6301 0000 0000 0000  taclass.c.......
-000032d0: 0000 0000 0001 0000 0004 0000 0013 0000  ................
-000032e0: 0073 1200 0000 8800 6a00 8801 7c00 6a01  .s......j...|.j.
-000032f0: 6401 8d02 0c00 5300 2902 4e72 a300 0000  d.....S.).Nr....
-00003300: 2902 72a4 0000 0072 9200 0000 2901 da01  ).r....r....)...
-00003310: 66a9 02da 0363 6c73 5a05 6d6f 6465 6c72  f....clsZ.modelr
-00003320: 5300 0000 7257 0000 0072 5e00 0000 b201  S...rW...r^.....
-00003330: 0000 f302 0000 0012 007a 2f41 7267 756d  .........z/Argum
-00003340: 656e 7450 6172 7365 722e 5f61 6464 5f61  entParser._add_a
-00003350: 7267 756d 656e 7473 2e3c 6c6f 6361 6c73  rguments.<locals
-00003360: 3e2e 3c6c 616d 6264 613e 6301 0000 0000  >.<lambda>c.....
-00003370: 0000 0000 0000 0002 0000 0007 0000 0053  ...............S
-00003380: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
-00003390: 7c01 7c01 6a00 a001 7402 7403 8300 a102  |.|.j...t.t.....
-000033a0: 6602 9102 7102 5300 7253 0000 0029 04da  f...q.S.rS...)..
-000033b0: 086d 6574 6164 6174 61da 0367 6574 7221  .metadata..getr!
-000033c0: 0000 0072 2200 0000 7254 0000 0072 5300  ...r"...rT...rS.
-000033d0: 0000 7253 0000 0072 5700 0000 7258 0000  ..rS...rW...rX..
-000033e0: 00b7 0100 0073 0800 0000 0600 0202 12ff  .....s..........
-000033f0: 06ff 7a31 4172 6775 6d65 6e74 5061 7273  ..z1ArgumentPars
-00003400: 6572 2e5f 6164 645f 6172 6775 6d65 6e74  er._add_argument
-00003410: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-00003420: 636f 6d70 3e72 3d00 0000 5429 01da 0d69  comp>r=...T)...i
-00003430: 735f 756e 696f 6e5f 7479 7065 da01 2e72  s_union_type...r
-00003440: 1700 0000 a901 da08 6d61 7873 706c 6974  ........maxsplit
-00003450: e9ff ffff ff46 7201 0000 0029 01da 1061  .....Fr....)...a
-00003460: 7373 6572 745f 7072 696d 6974 6976 6563  ssert_primitivec
-00003470: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00003480: 0300 0000 5300 0000 7312 0000 0067 007c  ....S...s....g.|
-00003490: 005d 057d 017c 016a 0091 0271 0253 0072  .].}.|.j...q.S.r
-000034a0: 5300 0000 a901 7292 0000 0072 5400 0000  S.....r....rT...
-000034b0: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-000034c0: 5800 0000 1302 0000 72a8 0000 00da 0370  X.......r......p
-000034d0: 6f73 7267 0000 0063 0100 0000 0000 0000  osrg...c........
-000034e0: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-000034f0: 731a 0000 0067 007c 005d 097d 017c 01a0  s....g.|.].}.|..
-00003500: 0064 00a1 0172 027c 0191 0271 0253 0029  .d...r.|...q.S.)
-00003510: 0172 6500 0000 725f 0000 0072 5400 0000  .re...r_...rT...
-00003520: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-00003530: 5800 0000 2d02 0000 7302 0000 001a 00da  X...-...s.......
-00003540: 076d 6574 6176 6172 7264 0000 00fa 013c  .metavarrd.....<
-00003550: da04 6465 7374 fa01 3e7a 073c 7661 6c75  ..dest..>z.<valu
-00003560: 653e da08 7265 7175 6972 6564 da05 6e61  e>..required..na
-00003570: 7267 73fa 013f da04 7479 7065 2905 72ba  rgs..?..type).r.
-00003580: 0000 0072 b800 0000 da05 636f 6e73 7472  ...r......constr
-00003590: 6400 0000 72b3 0000 0072 5900 0000 7263  d...r....rY...rc
-000035a0: 0000 00da 0072 5300 0000 2902 7267 0000  .....rS...).rg..
-000035b0: 0072 b500 0000 2903 7266 0000 00da 096e  .r....).rf.....n
-000035c0: 616d 6573 7061 6365 da06 7661 6c75 6573  amespace..values
-000035d0: 7a0f 496e 7661 6c69 6420 7661 6c75 6520  z.Invalid value 
-000035e0: 277a 1027 2066 6f72 2061 7267 756d 656e  'z.' for argumen
-000035f0: 7420 277a 1327 3b20 6d75 7374 2062 6520  t 'z.'; must be 
-00003600: 6f6e 6520 6f66 3a20 7a06 5479 7065 3a20  one of: z.Type: 
-00003610: 7a16 4465 6661 756c 743a 2022 2528 6465  z.Default: "%(de
-00003620: 6661 756c 7429 7322 7a14 4465 6661 756c  fault)s"z.Defaul
-00003630: 743a 2025 2864 6566 6175 6c74 2973 da09  t: %(default)s..
-00003640: 6578 636c 7573 6976 657a 044d 2e58 2e7a  exclusivez.M.X.z
-00003650: 0545 6e76 3a20 7a02 3e20 fa02 2c20 725a  .Env: z.> .., rZ
-00003660: 0000 0072 7d00 0000 da05 6772 6f75 707a  ...r}.....groupz
-00003670: 1372 6571 7569 7265 6420 7061 7261 6d65  .required parame
-00003680: 7465 7273 7a13 6f70 7469 6f6e 616c 2070  tersz.optional p
-00003690: 6172 616d 6574 6572 737a 3341 206d 7574  arametersz3A mut
-000036a0: 7561 6c6c 792d 6578 636c 7573 6976 6520  ually-exclusive 
-000036b0: 7061 7261 6d65 7465 7220 6361 6e6e 6f74  parameter cannot
-000036c0: 2062 6520 7265 7175 6972 6564 3a20 294d   be required: )M
-000036d0: 7234 0000 0072 2500 0000 da0b 6765 745f  r4...r%.....get_
-000036e0: 6465 6661 756c 7472 4600 0000 7282 0000  defaultrF...r...
-000036f0: 0072 9d00 0000 725d 0000 00da 0666 696c  .r....r].....fil
-00003700: 7465 7272 0600 0000 72ba 0000 0072 3800  terr....r....r8.
-00003710: 0000 726e 0000 0072 2300 0000 727f 0000  ..rn...r#...r...
-00003720: 00da 0c76 6572 7369 6f6e 5f69 6e66 6f72  ...version_infor
-00003730: 3f00 0000 da10 5f67 6574 5f74 7970 655f  ?....._get_type_
-00003740: 6f72 6967 696e 7215 0000 00da 1c5f 6578  originr......_ex
-00003750: 7472 6163 745f 7479 7065 5f66 726f 6d5f  tract_type_from_
-00003760: 636f 6e74 6169 6e65 7272 3c00 0000 da12  containerr<.....
-00003770: 5f67 6574 5f74 7970 655f 6d65 7461 6461  _get_type_metada
-00003780: 7461 726d 0000 0072 0500 0000 7221 0000  tarm...r....r!..
-00003790: 0072 a900 0000 7295 0000 00da 0672 7370  .r....r......rsp
-000037a0: 6c69 74da 0873 6574 5f64 6573 7472 9200  lit..set_destr..
-000037b0: 0000 72b7 0000 0072 6300 0000 7204 0000  ..r....rc...r...
-000037c0: 00da 0f64 6566 6175 6c74 5f66 6163 746f  ...default_facto
-000037d0: 7279 722a 0000 00da 0e5f 6765 745f 7479  ryr*....._get_ty
-000037e0: 7065 5f61 7267 7372 6400 0000 7239 0000  pe_argsrd...r9..
-000037f0: 00da 0b63 6f6c 6c65 6374 696f 6e73 da03  ...collections..
-00003800: 6162 63da 074d 6170 7069 6e67 7259 0000  abc..MappingrY..
-00003810: 0072 1d00 0000 da08 4974 6572 6162 6c65  .r......Iterable
-00003820: da03 7365 7472 1f00 0000 da05 7475 706c  ..setr......tupl
-00003830: 6572 2000 0000 721e 0000 0072 3500 0000  er ...r....r5...
-00003840: 7227 0000 0072 0700 0000 7208 0000 0072  r'...r....r....r
-00003850: 3100 0000 7272 0000 0072 b500 0000 da06  1...rr...r......
-00003860: 6173 6469 6374 7297 0000 0072 aa00 0000  asdictr....r....
-00003870: da05 7570 7065 72da 0462 6f6f 6c72 1800  ..upper..boolr..
-00003880: 0000 72b8 0000 00da 0369 6e74 7219 0000  ..r......intr...
-00003890: 0072 1a00 0000 7274 0000 00da 0641 6374  .r....rt.....Act
-000038a0: 696f 6eda 0767 6574 6174 7472 da06 6170  ion..getattr..ap
-000038b0: 7065 6e64 da08 5f65 6e76 5f76 6172 da04  pend.._env_var..
-000038c0: 6a6f 696e da12 6164 645f 6172 6775 6d65  join..add_argume
-000038d0: 6e74 5f67 726f 7570 72bf 0000 0072 7100  nt_groupr....rq.
-000038e0: 0000 da09 5f64 6566 6175 6c74 7372 4500  ...._defaultsrE.
-000038f0: 0000 726f 0000 0029 1972 a700 0000 7266  ..ro...).r....rf
-00003900: 0000 0072 8f00 0000 da03 6572 725a 1170  ...r......errZ.p
-00003910: 6172 7365 725f 6172 675f 6772 6f75 7073  arser_arg_groups
-00003920: 5a0c 6e6f 7665 6c5f 6669 656c 6473 5a10  Z.novel_fieldsZ.
-00003930: 6e6f 7665 6c5f 6669 656c 645f 6172 6773  novel_field_args
-00003940: 5a0a 6164 6465 645f 6172 6773 5a03 666c  Z.added_argsZ.fl
-00003950: 645a 1161 7267 7061 7273 655f 6172 6775  dZ.argparse_argu
-00003960: 6d65 6e74 da08 666c 645f 7479 7065 7256  ment..fld_typerV
-00003970: 0000 005a 0968 656c 705f 7479 7065 5a0f  ...Z.help_typeZ.
-00003980: 666c 645f 7479 7065 5f6f 7269 6769 6e72  fld_type_originr
-00003990: 5100 0000 7267 0000 0072 5000 0000 72b7  Q...rg...rP...r.
-000039a0: 0000 00da 016b 5a0f 6475 6d6d 795f 6e61  .....kZ.dummy_na
-000039b0: 6d65 7370 6163 65da 0164 5a0e 6865 6c70  mespace..dZ.help
-000039c0: 5f6d 7367 5f70 6172 7473 5a08 6865 6c70  _msg_partsZ.help
-000039d0: 5f6d 7367 72c1 0000 005a 0961 7267 5f67  _msgr....Z.arg_g
-000039e0: 726f 7570 7253 0000 0072 a600 0000 7257  rouprS...r....rW
-000039f0: 0000 0072 9000 0000 9901 0000 739c 0100  ...r........s...
-00003a00: 0008 0a06 0108 020c 0204 010a 0116 0204  ................
-00003a10: 0202 0202 010c 0106 0102 fe04 ff06 0702  ................
-00003a20: 0206 fe04 050e 0206 010a 0408 010e 0114  ................
-00003a30: 030e 0104 0102 0102 0106 fe0a 050e 0114  ................
-00003a40: 010a 0104 0102 800a 0214 030e 0104 0102  ................
-00003a50: 0102 0106 fe08 0708 ff14 0202 fd0c 0606  ................
-00003a60: 020a 0108 0108 010a 010a 0106 010a 0206  ................
-00003a70: 0110 0110 0108 010e 0102 8010 0304 0102  ................
-00003a80: 0102 0106 fe08 0406 0102 800c 0304 ff0a  ................
-00003a90: 0204 0202 0102 0106 fe08 040a 0108 010a  ................
-00003aa0: 0108 0106 0202 8006 0208 010c 0210 010c  ................
-00003ab0: 0202 0302 0102 010c fe06 070c 020a 0106  ................
-00003ac0: 0208 0206 010a 0202 0308 ff0c 0202 fd16  ................
-00003ad0: 061c 0206 ff08 0406 0206 0216 0108 0110  ................
-00003ae0: 010c 010c 0102 0302 0102 010c fe08 0510  ................
-00003af0: 010a 0108 0102 800c 0210 010a 010a 020a  ................
-00003b00: 0108 020c 040c 0110 010e 0206 0108 0106  ................
-00003b10: fe0e 0512 0102 0102 0106 0106 fd14 050a  ................
-00003b20: 0114 010c 0308 010e 0102 0106 0106 fe06  ................
-00003b30: 0408 020e 0208 0204 fe10 0308 0304 fd0a  ................
-00003b40: 0312 0306 0104 ff02 ff0a 0404 800c 0206  ................
-00003b50: 0312 010c 010a 020e 020a 0108 0212 0110  ................
-00003b60: 020c 0216 0108 020c 0206 020e 010c 0206  ................
-00003b70: 020a 0108 0108 0206 0102 0204 0104 ff02  ................
-00003b80: ff0a 0404 020c 0102 ff02 0202 fe02 0204  ................
-00003b90: 0210 0102 fe04 ff10 070c 0204 027a 1d41  .............z.A
-00003ba0: 7267 756d 656e 7450 6172 7365 722e 5f61  rgumentParser._a
-00003bb0: 6464 5f61 7267 756d 656e 7473 da01 7463  dd_arguments..tc
-00003bc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00003bd0: 0400 0000 4300 0000 730c 0000 0074 007c  ....C...s....t.|
-00003be0: 0064 0164 0083 0353 0029 024e da0a 5f5f  .d.d...S.).N..__
-00003bf0: 6f72 6967 696e 5f5f a901 72d7 0000 00a9  origin__..r.....
-00003c00: 0172 e100 0000 7253 0000 0072 5300 0000  .r....rS...rS...
-00003c10: 7257 0000 0072 c500 0000 ba02 0000 f302  rW...r..........
-00003c20: 0000 000c 027a 1f41 7267 756d 656e 7450  .....z.ArgumentP
-00003c30: 6172 7365 722e 5f67 6574 5f74 7970 655f  arser._get_type_
-00003c40: 6f72 6967 696e 6301 0000 0000 0000 0000  originc.........
-00003c50: 0000 0001 0000 0004 0000 0043 0000 00f3  ...........C....
-00003c60: 0c00 0000 7400 7c00 6401 6402 8303 5300  ....t.|.d.d...S.
-00003c70: 2903 4eda 085f 5f61 7267 735f 5f72 5300  ).N..__args__rS.
-00003c80: 0000 72e3 0000 0072 e400 0000 7253 0000  ..r....r....rS..
-00003c90: 0072 5300 0000 7257 0000 0072 cb00 0000  .rS...rW...r....
-00003ca0: be02 0000 72e5 0000 007a 1d41 7267 756d  ....r....z.Argum
-00003cb0: 656e 7450 6172 7365 722e 5f67 6574 5f74  entParser._get_t
-00003cc0: 7970 655f 6172 6773 6301 0000 0000 0000  ype_argsc.......
-00003cd0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00003ce0: 0072 e600 0000 2903 4eda 0c5f 5f6d 6574  .r....).N..__met
-00003cf0: 6164 6174 615f 5f72 5300 0000 72e3 0000  adata__rS...r...
-00003d00: 0072 e400 0000 7253 0000 0072 5300 0000  .r....rS...rS...
-00003d10: 7257 0000 0072 c700 0000 c202 0000 72e5  rW...r........r.
-00003d20: 0000 007a 2141 7267 756d 656e 7450 6172  ...z!ArgumentPar
-00003d30: 7365 722e 5f67 6574 5f74 7970 655f 6d65  ser._get_type_me
-00003d40: 7461 6461 7461 da0e 7479 7065 5f63 6f6e  tadata..type_con
-00003d50: 7461 696e 6572 72b0 0000 0072 ab00 0000  tainerr....r....
-00003d60: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
-00003d70: 0003 0000 0043 0000 0073 1801 0000 7c03  .....C...s....|.
-00003d80: 7204 7400 6e04 7c00 a001 7c01 a101 7d04  r.t.n.|...|...}.
-00003d90: 7c04 6400 7500 7215 7402 6401 7c01 6a03  |.d.u.r.t.d.|.j.
-00003da0: 9b00 9d02 8301 8201 7c00 a004 7c01 a101  ........|...|...
-00003db0: 7d05 6402 6403 8400 7c05 4400 8301 7d06  }.d.d...|.D...}.
-00003dc0: 7c04 7400 7500 7330 7405 7c04 7406 6a07  |.t.u.s0t.|.t.j.
-00003dd0: 6a08 8302 7330 7c04 7409 7500 7240 740a  j...s0|.t.u.r@t.
-00003de0: 7c06 8301 6404 6b03 723b 7c06 a00b a100  |...d.k.r;|.....
-00003df0: 0100 6e2c 7c06 6405 1900 7d07 6e27 7405  ..n,|.d...}.n't.
-00003e00: 7c04 7406 6a07 6a0c 8302 7261 740a 7c06  |.t.j.j...rat.|.
-00003e10: 8301 6406 6b03 7252 7c06 a00b a100 0100  ..d.k.rR|.......
-00003e20: 6e15 7c06 5c02 7d08 7d09 7c08 740d 7501  n.|.\.}.}.|.t.u.
-00003e30: 725e 7402 6407 8301 8201 7c09 7d07 6e06  r^t.d.....|.}.n.
-00003e40: 740e 7367 740f 7c01 8301 0100 7c06 736d  t.sgt.|.....|.sm
-00003e50: 7402 6408 8301 8201 7c00 a001 7c07 a101  t.d.....|...|...
-00003e60: 7d0a 7c0a 7400 7500 7280 7c00 a010 7c07  }.|.t.u.r.|...|.
-00003e70: a101 7d07 7c00 a001 7c07 a101 7d0a 7c02  ..}.|...|...}.|.
-00003e80: 728a 7c0a 728a 740e 738a 740f 7c0a 8301  r.|.r.t.s.t.|...
-00003e90: 0100 7c07 5300 2909 4e7a 1f47 6976 656e  ..|.S.).Nz.Given
-00003ea0: 2074 7970 6520 6973 206e 6f74 2061 2063   type is not a c
-00003eb0: 6f6e 7461 696e 6572 3a20 6301 0000 0000  ontainer: c.....
-00003ec0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00003ed0: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
-00003ee0: 7c01 6400 7501 7202 7c01 7400 7501 7202  |.d.u.r.|.t.u.r.
-00003ef0: 7c01 9102 7102 5300 2901 2e29 0172 2b00  |...q.S.)..).r+.
-00003f00: 0000 2902 7255 0000 00da 0161 7253 0000  ..).rU.....arS..
-00003f10: 0072 5300 0000 7257 0000 0072 5800 0000  .rS...rW...rX...
-00003f20: d802 0000 7304 0000 0006 001a 017a 3f41  ....s........z?A
-00003f30: 7267 756d 656e 7450 6172 7365 722e 5f65  rgumentParser._e
-00003f40: 7874 7261 6374 5f74 7970 655f 6672 6f6d  xtract_type_from
-00003f50: 5f63 6f6e 7461 696e 6572 2e3c 6c6f 6361  _container.<loca
-00003f60: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7217  ls>.<listcomp>r.
-00003f70: 0000 0072 0100 0000 727c 0000 007a 2244  ...r....r|...z"D
-00003f80: 6963 7469 6f6e 6172 7920 6b65 7973 206d  ictionary keys m
-00003f90: 7573 7420 6265 2074 7970 6520 6073 7472  ust be type `str
-00003fa0: 607a 1b54 6f6f 206d 616e 7920 7479 7065  `z.Too many type
-00003fb0: 7320 696e 2063 6f6e 7461 696e 6572 2911  s in container).
-00003fc0: 7215 0000 0072 c500 0000 da09 5479 7065  r....r......Type
-00003fd0: 4572 726f 7272 9500 0000 72cb 0000 0072  Errorr....r....r
-00003fe0: 3900 0000 72cc 0000 0072 cd00 0000 7211  9...r....r....r.
-00003ff0: 0000 0072 d000 0000 7276 0000 00da 0563  ...r....rv.....c
-00004000: 6c65 6172 72ce 0000 0072 6e00 0000 7235  learr....rn...r5
-00004010: 0000 0072 2700 0000 72c6 0000 0029 0b72  ...r'...r....).r
-00004020: a700 0000 72e9 0000 0072 b000 0000 72ab  ....r....r....r.
-00004030: 0000 005a 1574 7970 655f 636f 6e74 6169  ...Z.type_contai
-00004040: 6e65 725f 6f72 6967 696e 5a13 7479 7065  ner_originZ.type
-00004050: 5f63 6f6e 7461 696e 6572 5f61 7267 73da  _container_args.
-00004060: 0772 6573 756c 7473 5a16 7479 7065 5f63  .resultsZ.type_c
-00004070: 6f6e 7461 696e 6572 5f73 7562 7479 7065  ontainer_subtype
-00004080: 5a08 6b65 795f 7479 7065 5a0a 7661 6c75  Z.key_typeZ.valu
-00004090: 655f 7479 7065 5a1d 7479 7065 5f63 6f6e  e_typeZ.type_con
-000040a0: 7461 696e 6572 5f73 7562 7479 7065 5f6f  tainer_subtype_o
-000040b0: 7269 6769 6e72 5300 0000 7253 0000 0072  riginrS...rS...r
-000040c0: 5700 0000 72c6 0000 00c6 0200 0073 5400  W...r........sT.
-000040d0: 0000 1008 02ff 0804 0201 0a01 04ff 0a04  ................
-000040e0: 0602 0201 06ff 0807 0c01 02ff 0802 0c02  ................
-000040f0: 0a01 0a02 0e01 0c01 0a01 0802 0801 0801  ................
-00004100: 0601 0401 0801 0402 0801 0a02 0802 0401  ................
-00004110: 0201 04ff 0a03 0203 02ff 0202 02fe 0203  ................
-00004120: 02fd 0805 0402 7a2b 4172 6775 6d65 6e74  ......z+Argument
-00004130: 5061 7273 6572 2e5f 6578 7472 6163 745f  Parser._extract_
-00004140: 7479 7065 5f66 726f 6d5f 636f 6e74 6169  type_from_contai
-00004150: 6e65 7263 0100 0000 0000 0000 0000 0000  nerc............
-00004160: 0200 0000 0400 0000 4300 0000 7324 0000  ........C...s$..
-00004170: 007c 006a 0044 005d 0c7d 0174 017c 0174  .|.j.D.].}.t.|.t
-00004180: 026a 0383 0272 0f7c 0102 0001 0053 0071  .j...r.|.....S.q
-00004190: 0364 0053 0072 5c00 0000 2904 da08 5f61  .d.S.r\...)..._a
-000041a0: 6374 696f 6e73 726d 0000 0072 7400 0000  ctionsrm...rt...
-000041b0: 7296 0000 0029 0272 7800 0000 72ea 0000  r....).rx...r...
-000041c0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
-000041d0: 728c 0000 0006 0300 0073 1000 0000 0a01  r........s......
-000041e0: 0201 0201 0401 04fe 0804 02fc 0405 7a26  ..............z&
-000041f0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-00004200: 6669 6e64 5f73 7562 7061 7273 6572 735f  find_subparsers_
-00004210: 6163 7469 6f6e 6301 0000 0000 0000 0000  actionc.........
-00004220: 0000 0001 0000 0007 0000 0003 0000 0073  ...............s
-00004230: 4400 0000 8800 6a00 6400 7500 721f 8800  D.....j.d.u.r...
-00004240: 6a01 7210 8800 a002 a100 8800 5f00 8800  j.r........._...
-00004250: 6a00 5300 8800 6a03 6401 6402 8800 6a04  j.S...j.d.d...j.
-00004260: 8700 6601 6403 6404 8408 6405 8d04 8800  ..f.d.d...d.....
-00004270: 5f00 8800 6a00 5300 2906 4e5a 0863 6f6d  _...j.S.).NZ.com
-00004280: 6d61 6e64 737a 093c 434f 4d4d 414e 443e  mandsz.<COMMAND>
-00004290: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-000042a0: 0006 0000 001b 0000 0073 1e00 0000 7400  .........s....t.
-000042b0: 8800 8301 6403 6900 7c00 a401 6401 8800  ....d.i.|...d...
-000042c0: 6a01 6402 9c02 a401 8e01 5300 2904 4e54  j.d.......S.).NT
-000042d0: 2902 724f 0000 0072 4e00 0000 7253 0000  ).rO...rN...rS..
-000042e0: 0029 0272 ba00 0000 724e 0000 0029 0172  .).r....rN...).r
-000042f0: df00 0000 a901 7278 0000 0072 5300 0000  ......rx...rS...
-00004300: 7257 0000 0072 5e00 0000 1803 0000 730c  rW...r^.......s.
-00004310: 0000 000a 0002 0102 ff02 0204 010a fd7a  ...............z
-00004320: 3741 7267 756d 656e 7450 6172 7365 722e  7ArgumentParser.
-00004330: 5f67 6574 5f6f 725f 6164 645f 7375 6270  _get_or_add_subp
-00004340: 6172 7365 7273 2e3c 6c6f 6361 6c73 3e2e  arsers.<locals>.
-00004350: 3c6c 616d 6264 613e 2904 726c 0000 0072  <lambda>).rl...r
-00004360: b300 0000 72b5 0000 00da 0c70 6172 7365  ....r......parse
-00004370: 725f 636c 6173 7329 0572 6a00 0000 728b  r_class).rj...r.
-00004380: 0000 0072 8c00 0000 da0e 6164 645f 7375  ...r......add_su
-00004390: 6270 6172 7365 7273 7244 0000 0072 ef00  bparsersrD...r..
-000043a0: 0000 7253 0000 0072 ef00 0000 7257 0000  ..rS...r....rW..
-000043b0: 0072 7700 0000 0f03 0000 7316 0000 000a  .rw.......s.....
-000043c0: 0106 010a 0106 0d04 f502 0102 0104 010a  ................
-000043d0: 0108 fc06 0b7a 2541 7267 756d 656e 7450  .....z%ArgumentP
-000043e0: 6172 7365 722e 5f67 6574 5f6f 725f 6164  arser._get_or_ad
-000043f0: 645f 7375 6270 6172 7365 7273 72bd 0000  d_subparsersr...
-00004400: 0063 0200 0000 0000 0000 0000 0000 0600  .c..............
-00004410: 0000 0600 0000 0300 0000 736e 0000 007c  ..........sn...|
-00004420: 006a 00a0 0174 0288 007c 006a 0364 0083  .j...t...|.j.d..
-00004430: 0369 00a1 027d 027c 02a0 04a1 0044 005d  .i...}.|.....D.]
-00004440: 1d7d 0387 0066 0164 0164 0284 087c 0344  .}...f.d.d...|.D
-00004450: 0083 017d 0474 057c 0483 0164 036b 0472  ...}.t.|...d.k.r
-00004460: 2d64 0464 05a0 067c 04a1 0117 007d 057c  -d.d...|.....}.|
-00004470: 00a0 077c 05a1 0101 0071 1074 0864 0669  ...|.....q.t.d.i
-00004480: 0074 0988 0083 01a4 018e 0153 0029 074e  .t.........S.).N
-00004490: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-000044a0: 0005 0000 0013 0000 0073 6c00 0000 6700  .........sl...g.
-000044b0: 7c00 5d32 5c02 7d01 7d02 7400 8800 7c01  |.]2\.}.}.t...|.
-000044c0: 8302 7234 7401 8800 7c01 8302 7d03 7402  ..r4t...|...}.t.
-000044d0: 7c03 7403 8302 731c 7402 7c03 7404 6a05  |.t...s.t.|.t.j.
-000044e0: 6a06 8302 7320 7c03 6400 7501 732e 7402  j...s |.d.u.s.t.
-000044f0: 7c03 7403 8302 7302 7402 7c03 7404 6a05  |.t...s.t.|.t.j.
-00004500: 6a06 8302 7202 7c03 7202 7c02 7232 7c02  j...r.|.r.|.r2|.
-00004510: 6e01 7c01 9102 7102 5300 725c 0000 0029  n.|...q.S.r\...)
-00004520: 07da 0768 6173 6174 7472 72d7 0000 0072  ...hasattrr....r
-00004530: 3800 0000 726e 0000 0072 cc00 0000 72cd  8...rn...r....r.
-00004540: 0000 0072 cf00 0000 2904 7255 0000 0072  ...r....).rU...r
-00004550: b500 0000 da04 666c 6167 5a0a 6174 7472  ......flagZ.attr
-00004560: 5f76 616c 7565 a901 72bd 0000 0072 5300  _value..r....rS.
-00004570: 0000 7257 0000 0072 5800 0000 3003 0000  ..rW...rX...0...
-00004580: 7330 0000 0006 0006 0208 0102 fd0a 0408  s0..............
-00004590: 0302 f902 0802 0106 0102 fe02 f808 0d08  ................
-000045a0: 0302 fd02 0402 0106 0102 fe02 fc02 0802  ................
-000045b0: f80a f406 0c7a 3341 7267 756d 656e 7450  .....z3ArgumentP
-000045c0: 6172 7365 722e 5f70 6f73 745f 7061 7273  arser._post_pars
-000045d0: 655f 6172 6773 2e3c 6c6f 6361 6c73 3e2e  e_args.<locals>.
-000045e0: 3c6c 6973 7463 6f6d 703e 7217 0000 007a  <listcomp>r....z
-000045f0: 2854 6865 7365 2061 7267 756d 656e 7473  (These arguments
-00004600: 2061 7265 206d 7574 7561 6c6c 7920 6578   are mutually ex
-00004610: 636c 7573 6976 653a 2072 c000 0000 7253  clusive: r....rS
-00004620: 0000 0029 0a72 7100 0000 72aa 0000 0072  ...).rq...r....r
-00004630: d700 0000 7245 0000 0072 be00 0000 7276  ....rE...r....rv
-00004640: 0000 0072 da00 0000 7282 0000 0072 2800  ...r....r....r(.
-00004650: 0000 da04 7661 7273 2906 7278 0000 0072  ....vars).rx...r
-00004660: bd00 0000 5a12 6675 6e63 5f6d 785f 6172  ....Z.func_mx_ar
-00004670: 675f 6772 6f75 7073 5a06 675f 6172 6773  g_groupsZ.g_args
-00004680: 5a0e 6d78 5f66 6c61 6773 5f66 6f75 6e64  Z.mx_flags_found
-00004690: 72dd 0000 0072 5300 0000 72f4 0000 0072  r....rS...r....r
-000046a0: 5700 0000 da10 5f70 6f73 745f 7061 7273  W....._post_pars
-000046b0: 655f 6172 6773 2103 0000 7320 0000 0006  e_args!...s ....
-000046c0: 070c 0102 0102 fe02 fd0c 070a 0402 0206  ................
-000046d0: fe0c 1906 0102 0106 ff0a 0302 8012 027a  ...............z
-000046e0: 1f41 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
-000046f0: 5f70 6f73 745f 7061 7273 655f 6172 6773  _post_parse_args
-00004700: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
-00004710: 000a 0000 0003 0000 0073 5200 0000 7a0e  .........sR...z.
-00004720: 7400 8300 6a01 7c01 7c02 6401 8d02 7d03  t...j.|.|.d...}.
-00004730: 7c00 a002 7c03 a101 5700 5300 0400 7403  |...|...W.S...t.
-00004740: 7928 0100 7d04 0100 7a0e 7c00 a004 7405  y(..}...z.|...t.
-00004750: 7c04 8301 a101 0100 5700 5900 6400 7d04  |.......W.Y.d.}.
-00004760: 7e04 6400 5300 6400 7d04 7e04 7701 7700  ~.d.S.d.}.~.w.w.
-00004770: a902 4e29 0272 5000 0000 72bd 0000 0029  ..N).rP...r....)
-00004780: 0672 6800 0000 da0a 7061 7273 655f 6172  .rh.....parse_ar
-00004790: 6773 72f6 0000 00da 0a56 616c 7565 4572  gsr......ValueEr
-000047a0: 726f 7272 8200 0000 726e 0000 0029 0572  rorr....rn...).r
-000047b0: 7800 0000 7250 0000 0072 bd00 0000 da06  x...rP...r......
-000047c0: 7061 7273 6564 da01 6572 7900 0000 7253  parsed..ery...rS
-000047d0: 0000 0072 5700 0000 72f8 0000 0051 0300  ...rW...r....Q..
-000047e0: 0073 1400 0000 0205 0601 0201 0201 06fe  .s..............
-000047f0: 0c04 0e01 1c01 0880 02ff 7a19 4172 6775  ..........z.Argu
-00004800: 6d65 6e74 5061 7273 6572 2e70 6172 7365  mentParser.parse
-00004810: 5f61 7267 7363 0300 0000 0000 0000 0000  _argsc..........
-00004820: 0000 0600 0000 0a00 0000 0300 0000 735a  ..............sZ
-00004830: 0000 007a 1274 0083 006a 017c 017c 0264  ...z.t...j.|.|.d
-00004840: 018d 025c 027d 037d 047c 00a0 027c 03a1  ...\.}.}.|...|..
-00004850: 017c 0466 0257 0053 0004 0074 0379 2c01  .|.f.W.S...t.y,.
-00004860: 007d 0501 007a 0e7c 00a0 0474 057c 0583  .}...z.|...t.|..
-00004870: 01a1 0101 0057 0059 0064 007d 057e 0564  .....W.Y.d.}.~.d
-00004880: 0053 0064 007d 057e 0577 0177 0072 f700  .S.d.}.~.w.w.r..
-00004890: 0000 2906 7268 0000 00da 1070 6172 7365  ..).rh.....parse
-000048a0: 5f6b 6e6f 776e 5f61 7267 7372 f600 0000  _known_argsr....
-000048b0: 72f9 0000 0072 8200 0000 726e 0000 0029  r....r....rn...)
-000048c0: 0672 7800 0000 7250 0000 0072 bd00 0000  .rx...rP...r....
-000048d0: 72fa 0000 00da 0775 6e6b 6e6f 776e 72fb  r......unknownr.
-000048e0: 0000 0072 7900 0000 7253 0000 0072 5700  ...ry...rS...rW.
-000048f0: 0000 72fc 0000 005f 0300 0073 0e00 0000  ..r...._...s....
-00004900: 0207 1401 1001 0e01 1c01 0880 02ff 7a1f  ..............z.
-00004910: 4172 6775 6d65 6e74 5061 7273 6572 2e70  ArgumentParser.p
-00004920: 6172 7365 5f6b 6e6f 776e 5f61 7267 73da  arse_known_args.
-00004930: 1873 6b69 705f 7079 6461 6e74 6963 5f76  .skip_pydantic_v
-00004940: 616c 6964 6174 696f 6e63 0400 0000 0000  alidationc......
-00004950: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
-00004960: 0000 7322 0000 007c 00a0 007c 01a1 015c  ..s"...|...|...\
-00004970: 027d 047d 057c 006a 017c 047c 027c 0364  .}.}.|.j.|.|.|.d
-00004980: 018d 037c 0566 0253 0029 0261 c902 0000  ...|.f.S.).a....
-00004990: 5573 6520 7061 7273 6564 2061 7267 7320  Use parsed args 
-000049a0: 746f 2069 6e73 7461 6e74 6961 7465 2074  to instantiate t
-000049b0: 6865 2067 6976 656e 2064 6174 6120 6d6f  he given data mo
-000049c0: 6465 6c2e 0a0a 2020 2020 2020 2020 4172  del...        Ar
-000049d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000049e0: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
-000049f0: 2020 6172 6773 5f6d 6f64 656c 3a0a 2020    args_model:.  
-00004a00: 2020 2020 2020 2020 2020 736b 6970 5f70            skip_p
-00004a10: 7964 616e 7469 635f 7661 6c69 6461 7469  ydantic_validati
-00004a20: 6f6e 3a0a 0a20 2020 2020 2020 2045 7861  on:..        Exa
-00004a30: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
-00004a40: 2020 203e 3e3e 2069 6d70 6f72 7420 7961     >>> import ya
-00004a50: 7078 0a20 2020 2020 2020 2020 2020 203e  px.            >
-00004a60: 3e3e 2066 726f 6d20 6461 7461 636c 6173  >> from dataclas
-00004a70: 7365 7320 696d 706f 7274 2064 6174 6163  ses import datac
-00004a80: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
-00004a90: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00004aa0: 203e 3e3e 2040 6461 7461 636c 6173 730a   >>> @dataclass.
-00004ab0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
-00004ac0: 636c 6173 7320 4164 644e 756d 733a 0a20  class AddNums:. 
-00004ad0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-00004ae0: 2020 2078 3a20 696e 740a 2020 2020 2020     x: int.      
-00004af0: 2020 2020 2020 2e2e 2e20 2020 2020 793a        ...     y:
-00004b00: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-00004b10: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00004b20: 203e 3e3e 2070 6172 7365 7220 3d20 7961   >>> parser = ya
-00004b30: 7078 2e41 7267 756d 656e 7450 6172 7365  px.ArgumentParse
-00004b40: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-00004b50: 3e3e 3e20 7061 7273 6572 2e61 6464 5f61  >>> parser.add_a
-00004b60: 7267 756d 656e 7473 2841 6464 4e75 6d73  rguments(AddNums
-00004b70: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-00004b80: 3e20 7061 7273 6564 2c20 756e 6b6e 6f77  > parsed, unknow
-00004b90: 6e20 3d20 7061 7273 6572 2e70 6172 7365  n = parser.parse
-00004ba0: 5f6b 6e6f 776e 5f61 7267 735f 746f 5f6d  _known_args_to_m
-00004bb0: 6f64 656c 285b 272d 7827 2c20 2731 272c  odel(['-x', '1',
-00004bc0: 2027 2d79 272c 2027 3227 2c20 272d 7a27   '-y', '2', '-z'
-00004bd0: 2c20 2733 275d 290a 2020 2020 2020 2020  , '3']).        
-00004be0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00004bf0: 2020 2020 3e3e 3e20 2870 6172 7365 642e      >>> (parsed.
-00004c00: 782c 2070 6172 7365 642e 7929 0a20 2020  x, parsed.y).   
-00004c10: 2020 2020 2020 2020 2028 312c 2032 290a           (1, 2).
-00004c20: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00004c30: 756e 6b6e 6f77 6e0a 2020 2020 2020 2020  unknown.        
-00004c40: 2020 2020 5b27 2d7a 272c 2027 3327 5d0a      ['-z', '3'].
-00004c50: 0a20 2020 2020 2020 20a9 0372 5000 0000  .        ..rP...
-00004c60: 728f 0000 0072 fe00 0000 2902 72fc 0000  r....r....).r...
-00004c70: 00da 145f 7061 7273 655f 6172 6773 5f74  ..._parse_args_t
-00004c80: 6f5f 6d6f 6465 6c29 0672 7800 0000 7250  o_model).rx...rP
-00004c90: 0000 0072 8f00 0000 72fe 0000 00da 0b70  ...r....r......p
-00004ca0: 6172 7365 645f 6172 6773 da0c 756e 6b6e  arsed_args..unkn
-00004cb0: 6f77 6e5f 6172 6773 7253 0000 0072 5300  own_argsrS...rS.
-00004cc0: 0000 7257 0000 00da 1970 6172 7365 5f6b  ..rW.....parse_k
-00004cd0: 6e6f 776e 5f61 7267 735f 746f 5f6d 6f64  nown_args_to_mod
-00004ce0: 656c 6c03 0000 7310 0000 000e 2304 0302  ell...s.....#...
-00004cf0: 0102 0102 0104 fd02 0504 fa7a 2841 7267  ...........z(Arg
-00004d00: 756d 656e 7450 6172 7365 722e 7061 7273  umentParser.pars
-00004d10: 655f 6b6e 6f77 6e5f 6172 6773 5f74 6f5f  e_known_args_to_
-00004d20: 6d6f 6465 6c63 0400 0000 0000 0000 0000  modelc..........
-00004d30: 0000 0500 0000 0500 0000 4300 0000 731a  ..........C...s.
-00004d40: 0000 007c 00a0 007c 01a1 017d 047c 006a  ...|...|...}.|.j
-00004d50: 017c 047c 027c 0364 018d 0353 0029 0261  .|.|.|.d...S.).a
-00004d60: 7f02 0000 5573 6520 7061 7273 6564 2061  ....Use parsed a
-00004d70: 7267 7320 746f 2069 6e73 7461 6e74 6961  rgs to instantia
-00004d80: 7465 2074 6865 2067 6976 656e 2064 6174  te the given dat
-00004d90: 6120 6d6f 6465 6c2e 0a0a 2020 2020 2020  a model...      
-00004da0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00004db0: 2020 2020 6172 6773 3a0a 2020 2020 2020      args:.      
-00004dc0: 2020 2020 2020 6172 6773 5f6d 6f64 656c        args_model
-00004dd0: 3a0a 2020 2020 2020 2020 2020 2020 736b  :.            sk
-00004de0: 6970 5f70 7964 616e 7469 635f 7661 6c69  ip_pydantic_vali
-00004df0: 6461 7469 6f6e 3a0a 0a20 2020 2020 2020  dation:..       
-00004e00: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-00004e10: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00004e20: 7420 7961 7078 0a20 2020 2020 2020 2020  t yapx.         
-00004e30: 2020 203e 3e3e 2066 726f 6d20 6461 7461     >>> from data
-00004e40: 636c 6173 7365 7320 696d 706f 7274 2064  classes import d
-00004e50: 6174 6163 6c61 7373 0a20 2020 2020 2020  ataclass.       
-00004e60: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00004e70: 2020 2020 203e 3e3e 2040 6461 7461 636c       >>> @datacl
-00004e80: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00004e90: 2e2e 2e20 636c 6173 7320 4164 644e 756d  ... class AddNum
-00004ea0: 733a 0a20 2020 2020 2020 2020 2020 202e  s:.            .
-00004eb0: 2e2e 2020 2020 2078 3a20 696e 740a 2020  ..     x: int.  
-00004ec0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00004ed0: 2020 793a 2069 6e74 0a20 2020 2020 2020    y: int.       
-00004ee0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00004ef0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
-00004f00: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
-00004f10: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
-00004f20: 2020 2020 3e3e 3e20 7061 7273 6572 2e61      >>> parser.a
-00004f30: 6464 5f61 7267 756d 656e 7473 2841 6464  dd_arguments(Add
-00004f40: 4e75 6d73 290a 2020 2020 2020 2020 2020  Nums).          
-00004f50: 2020 3e3e 3e20 7061 7273 6564 203d 2070    >>> parsed = p
-00004f60: 6172 7365 722e 7061 7273 655f 6172 6773  arser.parse_args
-00004f70: 5f74 6f5f 6d6f 6465 6c28 5b27 2d78 272c  _to_model(['-x',
-00004f80: 2027 3127 2c20 272d 7927 2c20 2732 275d   '1', '-y', '2']
-00004f90: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
-00004fa0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00004fb0: 3e20 2870 6172 7365 642e 782c 2070 6172  > (parsed.x, par
-00004fc0: 7365 642e 7929 0a20 2020 2020 2020 2020  sed.y).         
-00004fd0: 2020 2028 312c 2032 290a 0a20 2020 2020     (1, 2)..     
-00004fe0: 2020 2072 ff00 0000 2902 72f8 0000 0072     r....).r....r
-00004ff0: 0001 0000 2905 7278 0000 0072 5000 0000  ....).rx...rP...
-00005000: 728f 0000 0072 fe00 0000 7201 0100 0072  r....r....r....r
-00005010: 5300 0000 7253 0000 0072 5700 0000 da13  S...rS...rW.....
-00005020: 7061 7273 655f 6172 6773 5f74 6f5f 6d6f  parse_args_to_mo
-00005030: 6465 6c9a 0300 0073 0c00 0000 0a1e 0401  del....s........
-00005040: 0201 0201 0201 06fd 7a22 4172 6775 6d65  ........z"Argume
-00005050: 6e74 5061 7273 6572 2e70 6172 7365 5f61  ntParser.parse_a
-00005060: 7267 735f 746f 5f6d 6f64 656c 6304 0000  rgs_to_modelc...
-00005070: 0000 0000 0000 0000 0008 0000 000a 0000  ................
-00005080: 0043 0000 0073 aa00 0000 7400 7c01 8301  .C...s....t.|...
-00005090: 7d04 7c02 7310 7c04 a001 7c00 6a02 a101  }.|.s.|...|.j...
-000050a0: 7d02 7c02 7310 7403 8201 7c00 6a04 7c04  }.|.s.t...|.j.|.
-000050b0: 7c02 6401 8d02 7d05 7405 724e 7c03 734e  |.d...}.t.rN|.sN
-000050c0: 7a0d 7400 7406 7c02 8301 6405 6900 7c05  z.t.t.|...d.i.|.
-000050d0: a401 8e01 8301 7d05 5700 6e25 0400 7407  ......}.W.n%..t.
-000050e0: 794d 0100 7d06 0100 7a19 6402 6402 a008  yM..}...z.d.d...
-000050f0: 6403 6404 8400 7c06 a009 a100 4400 8301  d.d...|.....D...
-00005100: a101 1700 7d07 7c00 a00a 7c07 a101 0100  ....}.|...|.....
-00005110: 5700 5900 6400 7d06 7e06 6e05 6400 7d06  W.Y.d.}.~.n.d.}.
-00005120: 7e06 7701 7700 7c02 6405 6900 7c05 a401  ~.w.w.|.d.i.|...
-00005130: 8e01 5300 2906 4ea9 02da 0961 7267 735f  ..S.).N....args_
-00005140: 6469 6374 728f 0000 0072 7d00 0000 6301  dictr....r}...c.
-00005150: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00005160: 0000 0073 0000 0073 2e00 0000 8100 7c00  ...s...s......|.
-00005170: 5d12 7d01 6400 7c01 6401 1900 6402 1900  ].}.d.|.d...d...
-00005180: 9b00 6403 7c01 6404 1900 9b00 6405 9d05  ..d.|.d.....d...
-00005190: 5600 0100 7102 6406 5300 2907 7a18 4572  V...q.d.S.).z.Er
-000051a0: 726f 7220 7061 7273 696e 6720 6172 6775  ror parsing argu
-000051b0: 6d65 6e74 2060 da03 6c6f 6372 0100 0000  ment `..locr....
-000051c0: 7a03 603b 20da 036d 7367 72ac 0000 004e  z.`; ..msgr....N
-000051d0: 7253 0000 0072 5400 0000 7253 0000 0072  rS...rT...rS...r
-000051e0: 5300 0000 7257 0000 00da 093c 6765 6e65  S...rW.....<gene
-000051f0: 7870 723e d803 0000 730a 0000 0002 8004  xpr>....s.......
-00005200: 0002 021c ff0a ff7a 3641 7267 756d 656e  .......z6Argumen
-00005210: 7450 6172 7365 722e 5f70 6172 7365 5f61  tParser._parse_a
-00005220: 7267 735f 746f 5f6d 6f64 656c 2e3c 6c6f  rgs_to_model.<lo
-00005230: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
-00005240: 5300 0000 290b 72f5 0000 0072 aa00 0000  S...).r....r....
-00005250: 7246 0000 0072 2600 0000 da16 5f75 6e69  rF...r&....._uni
-00005260: 6f6e 5f61 7267 735f 7769 7468 5f6d 6f64  on_args_with_mod
-00005270: 656c 7235 0000 0072 3300 0000 722e 0000  elr5...r3...r...
-00005280: 0072 da00 0000 da06 6572 726f 7273 7282  .r......errorsr.
-00005290: 0000 0029 0872 7800 0000 7250 0000 0072  ...).rx...rP...r
-000052a0: 8f00 0000 72fe 0000 0072 0101 0000 5a0a  ....r....r....Z.
-000052b0: 6172 6773 5f75 6e69 6f6e 72fb 0000 0072  args_unionr....r
-000052c0: dd00 0000 7253 0000 0072 5300 0000 7257  ....rS...rS...rW
-000052d0: 0000 0072 0001 0000 bf03 0000 732c 0000  ...r........s,..
-000052e0: 0008 0604 020c 0104 0104 0104 0202 0102  ................
-000052f0: 0106 fe08 0502 0202 0110 0108 ff0e 030c  ................
-00005300: 0106 020a fe16 0408 8002 fb0e 077a 2341  .............z#A
-00005310: 7267 756d 656e 7450 6172 7365 722e 5f70  rgumentParser._p
-00005320: 6172 7365 5f61 7267 735f 746f 5f6d 6f64  arse_args_to_mod
-00005330: 656c 7206 0100 0063 0200 0000 0000 0000  elr....c........
-00005340: 0000 0000 0200 0000 0300 0000 0300 0000  ................
-00005350: 7316 0000 0087 0066 0164 0164 0284 087c  s......f.d.d...|
-00005360: 00a0 00a1 0044 0083 0153 0029 034e 6301  .....D...S.).Nc.
-00005370: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00005380: 0000 0013 0000 0073 2000 0000 6900 7c00  .......s ...i.|.
-00005390: 5d0c 5c02 7d01 7d02 7c01 8800 6a00 7600  ].\.}.}.|...j.v.
-000053a0: 7202 7c01 7c02 9302 7102 5300 7253 0000  r.|.|...q.S.rS..
-000053b0: 0072 a100 0000 a903 7255 0000 0072 df00  .r......rU...r..
-000053c0: 0000 da01 7672 9400 0000 7253 0000 0072  ....vr....rS...r
-000053d0: 5700 0000 da0a 3c64 6963 7463 6f6d 703e  W.....<dictcomp>
-000053e0: e503 0000 7261 0000 007a 3941 7267 756d  ....ra...z9Argum
-000053f0: 656e 7450 6172 7365 722e 5f75 6e69 6f6e  entParser._union
-00005400: 5f61 7267 735f 7769 7468 5f6d 6f64 656c  _args_with_model
-00005410: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00005420: 6f6d 703e 2901 728d 0000 0072 0501 0000  omp>).r....r....
-00005430: 7253 0000 0072 9400 0000 7257 0000 0072  rS...r....rW...r
-00005440: 0a01 0000 e003 0000 7302 0000 0016 057a  ........s......z
-00005450: 2541 7267 756d 656e 7450 6172 7365 722e  %ArgumentParser.
-00005460: 5f75 6e69 6f6e 5f61 7267 735f 7769 7468  _union_args_with
-00005470: 5f6d 6f64 656c 6302 0000 0000 0000 0000  _modelc.........
-00005480: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
-00005490: 8000 0000 6400 7d02 7c01 6a00 7215 7c01  ....d.}.|.j.r.|.
-000054a0: 6a00 a001 7c01 6a02 6401 1700 a101 7315  j...|.j.d.....s.
-000054b0: 7c01 6a00 a003 a100 a004 a100 7d02 7c02  |.j.........}.|.
-000054c0: 7319 6400 5300 6402 7d03 7405 7c02 8301  s.d.S.d.}.t.|...
-000054d0: 4400 5d0c 5c02 7d04 7d05 7c05 a003 a100  D.].\.}.}.|.....
-000054e0: 732b 7c04 7d03 0100 6e01 711f 7c03 6402  s+|.}...n.q.|.d.
-000054f0: 6b04 7236 7c02 6400 7c03 8502 1900 7d02  k.r6|.d.|.....}.
-00005500: 6403 a006 6404 6405 8400 7c02 4400 8301  d...d.d...|.D...
-00005510: a101 5300 2906 4efa 0128 7201 0000 0072  ..S.).N..(r....r
-00005520: 7d00 0000 6301 0000 0000 0000 0000 0000  }...c...........
-00005530: 0002 0000 0003 0000 0073 0000 0073 1800  .........s...s..
-00005540: 0000 8100 7c00 5d07 7d01 7c01 a000 a100  ....|.].}.|.....
-00005550: 5600 0100 7102 6400 5300 725c 0000 0029  V...q.d.S.r\...)
-00005560: 01da 0573 7472 6970 7254 0000 0072 5300  ...striprT...rS.
-00005570: 0000 7253 0000 0072 5700 0000 7209 0100  ..rS...rW...r...
-00005580: 00ff 0300 0073 0400 0000 0280 1600 7a41  .....s........zA
-00005590: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-000055a0: 6765 745f 6465 7363 7269 7074 696f 6e5f  get_description_
-000055b0: 6672 6f6d 5f64 6f63 7374 7269 6e67 2e3c  from_docstring.<
-000055c0: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-000055d0: 3e29 07da 075f 5f64 6f63 5f5f 7260 0000  >)...__doc__r`..
-000055e0: 0072 9500 0000 7210 0100 0072 9900 0000  .r....r....r....
-000055f0: da09 656e 756d 6572 6174 6572 da00 0000  ..enumerater....
-00005600: 2906 72a7 0000 0072 8f00 0000 5a11 6465  ).r....r....Z.de
-00005610: 7363 7269 7074 696f 6e5f 6c69 6e65 735a  scription_linesZ
-00005620: 1274 6578 745f 626c 6f63 6b5f 656e 6473  .text_block_ends
-00005630: 5f61 74da 0169 da04 6c69 6e65 7253 0000  _at..i..linerS..
-00005640: 0072 5300 0000 7257 0000 0072 9800 0000  .rS...rW...r....
-00005650: e703 0000 7320 0000 0004 050c 0208 0104  ....s ..........
-00005660: ff0e 0304 0204 0104 0210 0108 0104 0104  ................
-00005670: 0102 fe08 040c 0114 027a 2e41 7267 756d  .........z.Argum
-00005680: 656e 7450 6172 7365 722e 5f67 6574 5f64  entParser._get_d
-00005690: 6573 6372 6970 7469 6f6e 5f66 726f 6d5f  escription_from_
-000056a0: 646f 6373 7472 696e 6763 0300 0000 0000  docstringc......
-000056b0: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
-000056c0: 0000 731c 0000 007c 00a0 007c 02a1 017d  ..s....|...|...}
-000056d0: 037c 0372 0c7c 037c 015f 0164 0053 0064  .|.r.|.|._.d.S.d
-000056e0: 0053 0072 5c00 0000 2902 7298 0000 0072  .S.r\...).r....r
-000056f0: 4900 0000 2904 72a7 0000 0072 6600 0000  I...).r....rf...
-00005700: 728f 0000 0072 4900 0000 7253 0000 0072  r....rI...rS...r
-00005710: 5300 0000 7257 0000 00da 1f5f 7365 745f  S...rW....._set_
-00005720: 6465 7363 7269 7074 696f 6e5f 6672 6f6d  description_from
-00005730: 5f64 6f63 7374 7269 6e67 0104 0000 7308  _docstring....s.
-00005740: 0000 000a 0604 020a 0104 ff7a 2e41 7267  ...........z.Arg
-00005750: 756d 656e 7450 6172 7365 722e 5f73 6574  umentParser._set
-00005760: 5f64 6573 6372 6970 7469 6f6e 5f66 726f  _description_fro
-00005770: 6d5f 646f 6373 7472 696e 67da 0b6c 696e  m_docstring..lin
-00005780: 6b65 645f 6675 6e63 da0b 7265 6c61 795f  ked_func..relay_
-00005790: 7661 6c75 6563 0700 0000 0000 0000 0000  valuec..........
-000057a0: 0000 1700 0000 0700 0000 0300 0000 73e6  ..............s.
-000057b0: 0100 0067 007d 0769 007d 0864 017d 0964  ...g.}.i.}.d.}.d
-000057c0: 017d 0a64 017d 0b64 017d 0c64 017d 0d74  .}.d.}.d.}.d.}.t
-000057d0: 007c 0283 016a 01a0 02a1 0044 005d 437d  .|...j.....D.]C}
-000057e0: 0e74 037c 0e83 01a0 0464 02a1 0172 2164  .t.|.....d...r!d
-000057f0: 037d 0c71 1574 037c 0e83 01a0 0464 04a1  .}.q.t.|.....d..
-00005800: 0172 2b64 037d 0a71 157c 0e6a 0564 056b  .r+d.}.q.|.j.d.k
-00005810: 0272 3364 037d 0b71 157c 0e6a 0564 066b  .r3d.}.q.|.j.d.k
-00005820: 0272 3b64 037d 0d71 157c 0e6a 0564 076b  .r;d.}.q.|.j.d.k
-00005830: 0272 457c 037c 0864 073c 0071 157c 0e6a  .rE|.|.d.<.q.|.j
-00005840: 0564 086b 0272 4f7c 067c 0864 083c 0071  .d.k.rO|.|.d.<.q
-00005850: 157c 0e6a 0564 096b 0272 5864 037c 0864  .|.j.d.k.rXd.|.d
-00005860: 093c 0071 157c 0a70 607c 0c70 607c 0b70  .<.q.|.p`|.p`|.p
-00005870: 607c 0d7d 097c 0973 737c 0572 7374 0664  `|.}.|.ss|.rst.d
-00005880: 0a64 0b84 0074 007c 0583 016a 01a0 02a1  .d...t.|...j....
-00005890: 0044 0083 0183 017d 097c 0473 7974 077c  .D.....}.|.syt.|
-000058a0: 0283 017d 047c 0972 e17c 016a 087c 037c  ...}.|.r.|.j.|.|
-000058b0: 0464 0c8d 025c 027d 0f7d 107c 0c73 887c  .d...\.}.}.|.s.|
-000058c0: 0d72 d669 0089 007c 0083 007d 117c 1044  .r.i...|...}.|.D
-000058d0: 005d 247d 127c 12a0 0464 0da1 0172 b37c  .]$}.|...d...r.|
-000058e0: 126a 0964 0e64 0f64 108d 0264 1119 007d  .j.d.d.d...d...}
-000058f0: 137c 13a0 0a64 0da1 017d 147c 1472 b37c  .|...d...}.|.r.|
-00005900: 116a 0b7c 1364 1264 0064 0164 138d 0401  .j.|.d.d.d.d....
-00005910: 007c 1388 007c 143c 0071 8f7c 116a 0c7c  .|...|.<.q.|.j.|
-00005920: 1064 148d 015c 027d 157d 1087 0066 0164  .d...\.}.}...f.d
-00005930: 1564 1684 0874 0d7c 1583 01a0 0ea1 0044  .d...t.|.......D
-00005940: 0083 017d 167c 0c72 d07c 08a0 0f7c 16a1  ...}.|.r.|...|..
-00005950: 0101 007c 0d72 d67c 167c 0864 063c 007c  ...|.r.|.|.d.<.|
-00005960: 0a72 da7c 107d 077c 0b72 e07c 107c 0864  .r.|.}.|.r.|.|.d
-00005970: 053c 006e 077c 016a 107c 037c 0464 0c8d  .<.n.|.j.|.|.d..
-00005980: 027d 0f7c 027c 0769 0074 0d7c 0f83 01a4  .}.|.|.i.t.|....
-00005990: 017c 08a4 018e 0153 0029 174e 467a 022a  .|.....S.).NFz.*
-000059a0: 2a54 da01 2ada 0b5f 6578 7472 615f 6172  *T..*.._extra_ar
-000059b0: 6773 da0d 5f65 7874 7261 5f6b 7761 7267  gs.._extra_kwarg
-000059c0: 735a 095f 616c 6c5f 6172 6773 5a0c 5f72  sZ._all_argsZ._r
-000059d0: 656c 6179 5f76 616c 7565 5a10 5f63 616c  elay_valueZ._cal
-000059e0: 6c65 645f 6672 6f6d 5f63 6c69 6301 0000  led_from_clic...
-000059f0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00005a00: 0073 0000 0073 2800 0000 8100 7c00 5d0f  .s...s(.....|.].
-00005a10: 7d01 7400 7c01 8301 a001 6400 a101 700f  }.t.|.....d...p.
-00005a20: 7c01 6a02 6401 7600 5600 0100 7102 6402  |.j.d.v.V...q.d.
-00005a30: 5300 2903 7218 0100 0029 0272 1901 0000  S.).r....).r....
-00005a40: 721a 0100 004e 2903 726e 0000 0072 6000  r....N).rn...r`.
-00005a50: 0000 7292 0000 0029 0272 5500 0000 da01  ..r....).rU.....
-00005a60: 7072 5300 0000 7253 0000 0072 5700 0000  prS...rS...rW...
-00005a70: 7209 0100 0036 0400 0073 0a00 0000 0280  r....6...s......
-00005a80: 0400 0202 16ff 0aff 7a2b 4172 6775 6d65  ........z+Argume
-00005a90: 6e74 5061 7273 6572 2e5f 7275 6e5f 6675  ntParser._run_fu
-00005aa0: 6e63 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  nc.<locals>.<gen
-00005ab0: 6578 7072 3e29 0272 5000 0000 728f 0000  expr>).rP...r...
-00005ac0: 0072 6500 0000 725b 0000 0072 1700 0000  .re...r[...r....
-00005ad0: 72ad 0000 0072 0100 0000 72b9 0000 0029  r....r....r....)
-00005ae0: 0372 b800 0000 7263 0000 0072 b700 0000  .r....rc...r....
-00005af0: 2901 7250 0000 0063 0100 0000 0000 0000  ).rP...c........
-00005b00: 0000 0000 0300 0000 0400 0000 1300 0000  ................
-00005b10: 731a 0000 0069 007c 005d 095c 027d 017d  s....i.|.].\.}.}
-00005b20: 0288 007c 0119 007c 0293 0271 0253 0072  ...|...|...q.S.r
-00005b30: 5300 0000 7253 0000 0072 0c01 0000 a901  S...rS...r......
-00005b40: 5a10 756e 6b6e 6f77 6e5f 6e61 6d65 5f6d  Z.unknown_name_m
-00005b50: 6170 7253 0000 0072 5700 0000 720e 0100  aprS...rW...r...
-00005b60: 005a 0400 0073 0600 0000 0600 0e01 06ff  .Z...s..........
-00005b70: 7a2c 4172 6775 6d65 6e74 5061 7273 6572  z,ArgumentParser
-00005b80: 2e5f 7275 6e5f 6675 6e63 2e3c 6c6f 6361  ._run_func.<loca
-00005b90: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2911  ls>.<dictcomp>).
-00005ba0: 7209 0000 00da 0a70 6172 616d 6574 6572  r......parameter
-00005bb0: 7372 be00 0000 726e 0000 0072 6000 0000  sr....rn...r`...
-00005bc0: 7292 0000 00da 0361 6e79 7225 0000 0072  r......anyr%...r
-00005bd0: 0301 0000 da05 7370 6c69 74da 066c 7374  ......split..lst
-00005be0: 7269 7072 6f00 0000 72fc 0000 0072 f500  ripro...r....r..
-00005bf0: 0000 728d 0000 00da 0675 7064 6174 6572  ..r......updater
-00005c00: 0401 0000 2917 72a7 0000 0072 6600 0000  ....).r....rf...
-00005c10: 729c 0000 0072 5000 0000 728f 0000 0072  r....rP...r....r
-00005c20: 1601 0000 7217 0100 005a 0966 756e 635f  ....r....Z.func_
-00005c30: 6172 6773 5a0b 6675 6e63 5f6b 7761 7267  argsZ.func_kwarg
-00005c40: 735a 0d65 7874 7261 5f61 7267 735f 6f6b  sZ.extra_args_ok
-00005c50: 5a0c 6163 6365 7074 735f 6172 6773 5a12  Z.accepts_argsZ.
-00005c60: 6163 6365 7074 735f 6578 7472 615f 6172  accepts_extra_ar
-00005c70: 6773 5a0e 6163 6365 7074 735f 6b77 6172  gsZ.accepts_kwar
-00005c80: 6773 5a14 6163 6365 7074 735f 6578 7472  gsZ.accepts_extr
-00005c90: 615f 6b77 6172 6773 721b 0100 005a 0a6d  a_kwargsr....Z.m
-00005ca0: 6f64 656c 5f69 6e73 7472 0201 0000 5a0e  odel_instr....Z.
-00005cb0: 756e 6b6e 6f77 6e5f 7061 7273 6572 7256  unknown_parserrV
-00005cc0: 0000 005a 0678 5f66 6c61 675a 0b78 5f66  ...Z.x_flagZ.x_f
-00005cd0: 6c61 675f 6261 7265 5a0e 7061 7273 6564  lag_bareZ.parsed
-00005ce0: 5f75 6e6b 6e6f 776e 5a0c 6578 7472 615f  _unknownZ.extra_
-00005cf0: 6b77 6172 6773 7253 0000 0072 1c01 0000  kwargsrS...r....
-00005d00: 7257 0000 00da 095f 7275 6e5f 6675 6e63  rW....._run_func
-00005d10: 0c04 0000 7390 0000 0004 0a04 0104 0204  ....s...........
-00005d20: 0204 0104 0204 0112 020e 0106 010e 0106  ................
-00005d30: 010a 0106 010a 0106 010a 010a 010a 010a  ................
-00005d40: 010a 0108 0102 800e 0302 ff08 0408 010c  ................
-00005d50: 0208 fe04 0508 0104 0304 0202 0102 010a  ................
-00005d60: fe08 0504 0106 0108 010a 0112 010a 0104  ................
-00005d70: 0104 0102 0102 0102 0102 0106 fc08 0602  ................
-00005d80: 8004 0202 010a ff0a 040a 0106 ff04 030a  ................
-00005d90: 0104 0108 0104 0204 0104 0208 0102 8004  ................
-00005da0: 0302 0102 0106 fe16 057a 1841 7267 756d  .........z.Argum
-00005db0: 656e 7450 6172 7365 722e 5f72 756e 5f66  entParser._run_f
-00005dc0: 756e 63da 0763 6f6d 6d61 6e64 da0b 7375  unc..command..su
-00005dd0: 6263 6f6d 6d61 6e64 73da 116e 616d 6564  bcommands..named
-00005de0: 5f73 7562 636f 6d6d 616e 6473 6304 0000  _subcommandsc...
-00005df0: 0000 0000 0000 0000 0009 0000 000b 0000  ................
-00005e00: 004b 0000 0073 d200 0000 7c00 6403 6900  .K...s....|.d.i.
-00005e10: 7c04 a401 8e01 7d05 7c01 722e 7400 7c01  |.....}.|.r.t.|.
-00005e20: 8301 7d06 7c00 6a01 7c05 7c06 6401 8d02  ..}.|.j.|.|.d...
-00005e30: 0100 7c05 a002 7c06 a101 0100 7c05 6a03  ..|...|.....|.j.
-00005e40: 6403 6900 7c00 6a04 7c01 7c00 6a05 7c06  d.i.|.j.|.|.j.|.
-00005e50: 7c00 6a06 7c01 7c00 6a07 7c06 6904 a401  |.j.|.|.j.|.i...
-00005e60: 8e01 0100 6e14 7c05 6a03 6403 6900 7c00  ....n.|.j.d.i.|.
-00005e70: 6a05 6400 7c00 6a04 6400 7c00 6a07 6400  j.d.|.j.d.|.j.d.
-00005e80: 7c00 6a06 6400 6904 a401 8e01 0100 7c02  |.j.d.i.......|.
-00005e90: 7255 7408 7c02 8301 724b 7c02 6701 7d02  rUt.|...rK|.g.}.
-00005ea0: 7c02 4400 5d07 7d07 7c05 a009 7c07 a101  |.D.].}.|...|...
-00005eb0: 0100 714d 7c03 7267 7c03 a00a a100 4400  ..qM|.rg|.....D.
-00005ec0: 5d0b 5c02 7d08 7d07 7c05 6a09 7c07 7c08  ].\.}.}.|.j.|.|.
-00005ed0: 6402 8d02 0100 715b 7c05 5300 2904 4e29  d.....q[|.S.).N)
-00005ee0: 0272 6600 0000 728f 0000 0072 b100 0000  .rf...r....r....
-00005ef0: 7253 0000 0029 0b72 2500 0000 7215 0100  rS...).r%...r...
-00005f00: 0072 9100 0000 729d 0000 0072 4200 0000  .r....r....rB...
-00005f10: 7243 0000 0072 4500 0000 7246 0000 00da  rC...rE...rF....
-00005f20: 0863 616c 6c61 626c 6572 9e00 0000 728d  .callabler....r.
-00005f30: 0000 0029 0972 a700 0000 7223 0100 0072  ...).r....r#...r
-00005f40: 2401 0000 7225 0100 0072 5100 0000 7266  $...r%...rQ...rf
-00005f50: 0000 005a 0e72 6f6f 745f 6172 675f 6d6f  ...Z.root_arg_mo
-00005f60: 6465 6c72 5600 0000 7292 0000 0072 5300  delrV...r....rS.
-00005f70: 0000 7253 0000 0072 5700 0000 da0d 5f62  ..rS...rW....._b
-00005f80: 7569 6c64 5f70 6172 7365 7270 0400 0073  uild_parserp...s
-00005f90: 3e00 0000 0e08 0402 0801 0401 0201 0201  >...............
-00005fa0: 06fe 0a04 0801 0602 0601 0601 0601 02fc  ................
-00005fb0: 08ff 0809 0602 0601 0601 0601 02fc 06ff  ................
-00005fc0: 0409 0801 0601 0801 0c01 0402 1001 1001  ................
-00005fd0: 0402 7a1c 4172 6775 6d65 6e74 5061 7273  ..z.ArgumentPars
-00005fe0: 6572 2e5f 6275 696c 645f 7061 7273 6572  er._build_parser
-00005ff0: 2902 7250 0000 00da 0c64 6566 6175 6c74  ).rP.....default
-00006000: 5f61 7267 73da 0b70 6172 7365 725f 6172  _args..parser_ar
-00006010: 6773 7228 0100 00da 0d70 6172 7365 725f  gsr(.....parser_
-00006020: 6b77 6172 6773 6301 0000 0000 0000 0002  kwargsc.........
-00006030: 0000 0011 0000 0009 0000 004f 0000 0073  ...........O...s
-00006040: 3801 0000 7c00 6a00 7c03 6900 7c04 a401  8...|.j.|.i.|...
-00006050: 8e01 7d05 7c01 6401 7500 7213 7401 6a02  ..}.|.d.u.r.t.j.
-00006060: 6402 6401 8502 1900 7d01 7c01 7319 7c02  d.d.....}.|.s.|.
-00006070: 7219 7c02 7d01 7c05 a003 7c01 a101 5c02  r.|.}.|...|...\.
-00006080: 7d06 7d07 7404 7c06 8301 7d08 7c08 a005  }.}.t.|...}.|...
-00006090: 7c00 6a06 a101 7d09 7c08 a005 7c00 6a07  |.j...}.|...|.j.
-000060a0: a101 7d0a 7c08 a005 7c00 6a08 a101 7d0b  ..}.|...|.j...}.
-000060b0: 7c08 a005 7c00 6a09 a101 7d0c 7c08 a005  |...|.j...}.|...
-000060c0: 7c00 6a0a a101 7d0d 6401 7d0e 6401 7d0f  |.j...}.d.}.d.}.
-000060d0: 7c09 7252 7c00 6a0b 7c05 7c09 7c0a 7c0c  |.rR|.j.|.|.|.|.
-000060e0: 7c01 6403 8d05 7d0f 740c 7c0f 740d 8302  |.d...}.t.|.t...
-000060f0: 7269 7a06 740e 7c0f 8301 7d0e 5700 6e0d  riz.t.|...}.W.n.
-00006100: 0400 740f 7968 0100 0100 0100 7c0f 7d0e  ..t.yh......|.}.
-00006110: 5900 6e03 7700 7c0f 7d0e 7a20 7c0b 727b  Y.n.w.|.}.z |.r{
-00006120: 7c0c 727b 7c00 6a0b 7c05 7c0c 7c0d 7c01  |.r{|.j.|.|.|.|.
-00006130: 7c09 7c0e 6404 8d06 7d0e 5700 740c 7c0f  |.|.d...}.W.t.|.
-00006140: 740d 8302 728a 7c0f 4400 5d06 7d10 7c0c  t...r.|.D.].}.|.
-00006150: 7389 7c10 7d0e 7183 7c0e 5300 740c 7c0f  s.|.}.q.|.S.t.|.
-00006160: 740d 8302 729a 7c0f 4400 5d07 7d10 7c0c  t...r.|.D.].}.|.
-00006170: 7399 7c10 7d0e 7193 7700 7700 2905 612d  s.|.}.q.w.w.).a-
-00006180: 0300 0055 7365 2067 6976 656e 2066 756e  ...Use given fun
-00006190: 6374 696f 6e73 2074 6f20 636f 6e73 7472  ctions to constr
-000061a0: 7563 7420 6120 434c 492c 2070 6172 7365  uct a CLI, parse
-000061b0: 2074 6865 2061 7267 732c 2061 6e64 2069   the args, and i
-000061c0: 6e76 6f6b 6520 7468 6520 6170 7072 6f70  nvoke the approp
-000061d0: 7269 6174 6520 636f 6d6d 616e 642e 0a0a  riate command...
-000061e0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000061f0: 2020 2020 2020 2020 2020 2a70 6172 7365            *parse
-00006200: 725f 6172 6773 3a0a 2020 2020 2020 2020  r_args:.        
-00006210: 2020 2020 6172 6773 3a0a 2020 2020 2020      args:.      
-00006220: 2020 2020 2020 6465 6661 756c 745f 6172        default_ar
-00006230: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00006240: 2a2a 7061 7273 6572 5f6b 7761 7267 733a  **parser_kwargs:
-00006250: 0a0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-00006260: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
-00006270: 203e 3e3e 2069 6d70 6f72 7420 7961 7078   >>> import yapx
-00006280: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00006290: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-000062a0: 2064 6566 2070 7269 6e74 5f6e 756d 7328   def print_nums(
-000062b0: 2a61 7267 7329 3a0a 2020 2020 2020 2020  *args):.        
-000062c0: 2020 2020 2e2e 2e20 2020 2020 7072 696e      ...     prin
-000062d0: 7428 2741 7267 733a 2027 2c20 2a61 7267  t('Args: ', *arg
-000062e0: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
-000062f0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
-00006300: 3e3e 2064 6566 2066 696e 645f 6576 656e  >> def find_even
-00006310: 7328 2a61 7267 7329 3a0a 2020 2020 2020  s(*args):.      
-00006320: 2020 2020 2020 2e2e 2e20 2020 2020 7265        ...     re
-00006330: 7475 726e 205b 7820 666f 7220 7820 696e  turn [x for x in
-00006340: 2061 7267 7320 6966 2069 6e74 2878 2920   args if int(x) 
-00006350: 2520 3220 3d3d 2030 5d0a 2020 2020 2020  % 2 == 0].      
-00006360: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00006370: 2020 2020 2020 3e3e 3e20 6465 6620 6669        >>> def fi
-00006380: 6e64 5f6f 6464 7328 2a61 7267 7329 3a0a  nd_odds(*args):.
-00006390: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
-000063a0: 2020 2020 7265 7475 726e 205b 7820 666f      return [x fo
-000063b0: 7220 7820 696e 2061 7267 7320 6966 2069  r x in args if i
-000063c0: 6e74 2878 2920 2520 3220 213d 2030 5d0a  nt(x) % 2 != 0].
-000063d0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-000063e0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-000063f0: 636c 695f 6172 6773 203d 205b 2766 696e  cli_args = ['fin
-00006400: 642d 6f64 6473 272c 2027 3127 2c20 2732  d-odds', '1', '2
-00006410: 272c 2027 3327 2c20 2734 272c 2027 3527  ', '3', '4', '5'
-00006420: 5d0a 2020 2020 2020 2020 2020 2020 3e3e  ].            >>
-00006430: 3e20 7961 7078 2e72 756e 2870 7269 6e74  > yapx.run(print
-00006440: 5f6e 756d 732c 205b 6669 6e64 5f65 7665  _nums, [find_eve
-00006450: 6e73 2c20 6669 6e64 5f6f 6464 735d 2c20  ns, find_odds], 
-00006460: 6172 6773 3d63 6c69 5f61 7267 7329 0a20  args=cli_args). 
-00006470: 2020 2020 2020 2020 2020 2041 7267 733a             Args:
-00006480: 2020 3120 3220 3320 3420 350a 2020 2020    1 2 3 4 5.    
-00006490: 2020 2020 2020 2020 5b27 3127 2c20 2733          ['1', '3
-000064a0: 272c 2027 3527 5d0a 2020 2020 2020 2020  ', '5'].        
-000064b0: 4e72 1700 0000 2905 7266 0000 0072 9c00  Nr....).rf...r..
-000064c0: 0000 728f 0000 0072 1601 0000 7250 0000  ..r....r....rP..
-000064d0: 0029 0672 6600 0000 729c 0000 0072 8f00  .).rf...r....r..
-000064e0: 0000 7250 0000 0072 1601 0000 7217 0100  ..rP...r....r...
-000064f0: 0029 1072 2701 0000 727f 0000 00da 0461  .).r'...r......a
-00006500: 7267 7672 fc00 0000 72f5 0000 0072 aa00  rgvr....r....r..
-00006510: 0000 7242 0000 0072 4300 0000 7244 0000  ..rB...rC...rD..
-00006520: 0072 4500 0000 7246 0000 0072 2201 0000  .rE...rF...r"...
-00006530: 7238 0000 0072 0a00 0000 da04 6e65 7874  r8...r......next
-00006540: da0d 5374 6f70 4974 6572 6174 696f 6e29  ..StopIteration)
-00006550: 1172 a700 0000 7250 0000 0072 2801 0000  .r....rP...r(...
-00006560: 7229 0100 0072 2a01 0000 7266 0000 005a  r)...r*...rf...Z
-00006570: 0a6b 6e6f 776e 5f61 7267 7372 8600 0000  .known_argsr....
-00006580: 7201 0100 005a 0972 6f6f 745f 6675 6e63  r....Z.root_func
-00006590: 5a14 726f 6f74 5f66 756e 635f 6172 6773  Z.root_func_args
-000065a0: 5f6d 6f64 656c 5a0c 636f 6d6d 616e 645f  _modelZ.command_
-000065b0: 6e61 6d65 5a0c 636f 6d6d 616e 645f 6675  nameZ.command_fu
-000065c0: 6e63 5a17 636f 6d6d 616e 645f 6675 6e63  ncZ.command_func
-000065d0: 5f61 7267 735f 6d6f 6465 6c72 1701 0000  _args_modelr....
-000065e0: 5a0b 726f 6f74 5f72 6573 756c 745a 0a67  Z.root_resultZ.g
-000065f0: 656e 5f72 6573 756c 7472 5300 0000 7253  en_resultrS...rS
-00006600: 0000 0072 5700 0000 da04 5f72 756e 9f04  ...rW....._run..
-00006610: 0000 737a 0000 0010 2308 020e 0108 0204  ..sz....#.......
-00006620: 010e 0308 0104 0204 0104 ff04 0304 0104  ................
-00006630: ff0c 0304 0104 0104 ff04 0304 0104 ff04  ................
-00006640: 0404 0104 0204 0102 0102 0102 0102 0102  ................
-00006650: 0106 fb0a 0802 010c 010c 0108 0102 ff04  ................
-00006660: 0302 0208 0104 0102 0102 0102 0102 0102  ................
-00006670: 0102 0106 fa02 800a 0908 0104 0104 0102  ................
-00006680: 8004 020a fb08 0104 0104 0102 8002 fd02  ................
-00006690: 017a 1341 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
-000066a0: 722e 5f72 756e 2902 4e46 725c 0000 0029  r._run).NFr\...)
-000066b0: 0246 4629 024e 4e29 034e 4e46 2903 4e4e  .FF).NN).NNF).NN
-000066c0: 4e29 3972 9500 0000 da0a 5f5f 6d6f 6475  N)9r......__modu
-000066d0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000066e0: 5f5f 7242 0000 0072 6e00 0000 72a2 0000  __rB...rn...r...
-000066f0: 0072 4300 0000 7244 0000 0072 4500 0000  .rC...rD...rE...
-00006700: 7246 0000 0072 2d00 0000 720c 0000 0072  rF...r-...r....r
-00006710: 1000 0000 720f 0000 0072 1300 0000 72d4  ....r....r....r.
-00006720: 0000 0072 6900 0000 7282 0000 0072 0b00  ...ri...r....r..
-00006730: 0000 728a 0000 0072 1500 0000 720d 0000  ..r....r....r...
-00006740: 0072 2900 0000 7291 0000 0072 7400 0000  .r)...r....rt...
-00006750: 7241 0000 0072 9b00 0000 729e 0000 00da  rA...r....r.....
-00006760: 0c73 7461 7469 636d 6574 686f 6472 a400  .staticmethodr..
-00006770: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
-00006780: 2200 0000 7290 0000 0072 c500 0000 7212  "...r....r....r.
-00006790: 0000 0072 cb00 0000 72c7 0000 0072 c600  ...r....r....r..
-000067a0: 0000 7296 0000 0072 8c00 0000 7277 0000  ..r....r....rw..
-000067b0: 0072 2800 0000 72f6 0000 0072 1100 0000  .r(...r....r....
-000067c0: 72f8 0000 0072 fc00 0000 7203 0100 0072  r....r....r....r
-000067d0: 0401 0000 7200 0100 0072 0e00 0000 720a  ....r....r....r.
-000067e0: 0100 0072 9800 0000 7215 0100 0072 2201  ...r....r....r".
-000067f0: 0000 7227 0100 0072 2e01 0000 da0d 5f5f  ..r'...r......__
-00006800: 636c 6173 7363 656c 6c5f 5f72 5300 0000  classcell__rS...
-00006810: 7253 0000 0072 7900 0000 7257 0000 0072  rS...ry...rW...r
-00006820: 4100 0000 4c00 0000 73d2 0100 000a 000c  A...L...s.......
-00006830: 010c 010c 010c 010c 0102 0502 0102 0102  ................
-00006840: 0102 0102 0102 0102 0102 0106 f502 0202  ................
-00006850: fe06 0302 fd06 0402 fc06 0502 fb0a 0602  ................
-00006860: fa0a 0702 f90a 0802 f80a 0902 f706 0a02  ................
-00006870: f602 0b02 f502 0c0e f40e 7102 0602 0104  ..........q.....
-00006880: fd0a 0202 fe02 0302 fd02 040e fc02 2e16  ................
-00006890: 0202 fe02 030a fd02 3404 fd16 0202 fe06  ........4.......
-000068a0: 0302 fd02 0402 fc04 050a fb02 6304 fd0a  ............c...
-000068b0: 0202 fe06 0302 fd02 0402 fc02 050a fb02  ................
-000068c0: 0e1c 0102 0302 0104 0202 fe16 0302 fd06  ................
-000068d0: 040c fc00 7f00 7f02 2220 0102 0324 0102  ........" ...$..
-000068e0: 0324 0102 0302 0402 0104 fc06 0202 fe02  .$..............
-000068f0: 0302 fd02 0402 fc06 050c fb14 3f10 0902  ............?...
-00006900: 1204 0202 fe02 030a fd02 3202 0104 fd0a  ..........2.....
-00006910: 0202 fe08 0302 fd02 040e fc02 1002 0104  ................
-00006920: fd0a 0202 fe08 0302 fd0e 040e fc02 0f02  ................
-00006930: 0102 0104 fc0a 0202 fe0a 0302 fd02 0402  ................
-00006940: fc0e 050a fb02 3002 0102 0104 fc0a 0202  ......0.........
-00006950: fe0a 0302 fd02 0402 fc02 050a fb02 2802  ..............(.
-00006960: 0104 fc04 0202 fe0a 0302 fd02 0402 fc02  ................
-00006970: 050a fb02 2102 010a 0102 ff06 0202 fe0a  ....!...........
-00006980: 030c fd02 0602 0116 0202 fe06 030c fd02  ................
-00006990: 1902 0104 0202 fe16 0302 fd02 040c fc02  ................
-000069a0: 0a02 0602 0102 0104 f902 0202 fe0a 0302  ................
-000069b0: fd06 0402 fc0a 0502 fb0e 0602 fa06 0702  ................
-000069c0: f902 080c f802 6302 0302 0102 0104 fc0e  ......c.........
-000069d0: 0202 fe12 0302 fd16 0402 fc02 0502 fb02  ................
-000069e0: 060c fa02 2e02 0402 0106 fc02 0202 fe0a  ................
-000069f0: 0302 fd0a 0402 fc02 0502 fb02 0614 fa72  ...............r
-00006a00: 4100 0000 294e 7274 0000 00da 0f63 6f6c  A...)Nrt.....col
-00006a10: 6c65 6374 696f 6e73 2e61 6263 72cc 0000  lections.abcr...
-00006a20: 0072 7f00 0000 7202 0000 00da 0a63 6f6e  .r....r......con
-00006a30: 7465 7874 6c69 6272 0300 0000 da0b 6461  textlibr......da
-00006a40: 7461 636c 6173 7365 7372 0400 0000 7205  taclassesr....r.
-00006a50: 0000 0072 0600 0000 da04 656e 756d 7207  ...r......enumr.
-00006a60: 0000 00da 0966 756e 6374 6f6f 6c73 7208  .....functoolsr.
-00006a70: 0000 00da 0769 6e73 7065 6374 7209 0000  .....inspectr...
-00006a80: 00da 0574 7970 6573 720a 0000 00da 0674  ...typesr......t
-00006a90: 7970 696e 6772 0b00 0000 720c 0000 0072  ypingr....r....r
-00006aa0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00006ab0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00006ac0: 0000 7214 0000 0072 1500 0000 5a0d 706b  ..r....r....Z.pk
-00006ad0: 675f 7265 736f 7572 6365 7372 1600 0000  g_resourcesr....
-00006ae0: da07 6163 7469 6f6e 7372 1800 0000 7219  ..actionsr....r.
-00006af0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00006b00: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00006b10: 0072 2000 0000 da03 6172 6772 2100 0000  .r .....argr!...
-00006b20: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
-00006b30: 2500 0000 da0a 6578 6365 7074 696f 6e73  %.....exceptions
-00006b40: 7226 0000 0072 2700 0000 72bd 0000 0072  r&...r'...r....r
-00006b50: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
-00006b60: 0000 00da 0575 7469 6c73 722c 0000 0072  .....utilsr,...r
-00006b70: 2d00 0000 722e 0000 0072 2f00 0000 7230  -...r....r/...r0
-00006b80: 0000 0072 3100 0000 7232 0000 0072 3300  ...r1...r2...r3.
-00006b90: 0000 7234 0000 0072 3500 0000 7236 0000  ..r4...r5...r6..
-00006ba0: 0072 3700 0000 7238 0000 0072 3900 0000  .r7...r8...r9...
-00006bb0: 72c4 0000 0072 3c00 0000 5a11 7479 7069  r....r<...Z.typi
-00006bc0: 6e67 5f65 7874 656e 7369 6f6e 7372 3f00  ng_extensionsr?.
-00006bd0: 0000 7240 0000 0072 4100 0000 7253 0000  ..r@...rA...rS..
-00006be0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
-00006bf0: da08 3c6d 6f64 756c 653e 0100 0000 7332  ..<module>....s2
-00006c00: 0000 0008 0008 0108 010c 010c 0114 010c  ................
-00006c10: 010c 010c 010c 0134 010c 0e2c 021c 0b10  .......4...,....
-00006c20: 070c 0114 0140 010a 110e 010c 020a 020c  .....@..........
-00006c30: 0108 0216 03                             .....
+00000810: 8301 5a25 6420 6518 6a26 6602 8700 6601  ..Z%d e.j&f...f.
+00000820: 6440 6441 840c 5a27 6420 650c 6518 6a26  d@dA..Z'd e.e.j&
+00000830: 1900 6602 6442 6443 8404 5a28 6420 6518  ..f.dBdC..Z(d e.
+00000840: 6a26 6602 6444 6445 8404 5a29 6446 6518  j&f.dDdE..Z)dFe.
+00000850: 6a2a 6420 652a 6604 6447 6448 8404 5a2b  j*d e*f.dGdH..Z+
+00000860: 090b 090b 646d 640e 650c 652c 6504 1900  ....dmd.e.e,e...
+00000870: 1900 6446 650c 6518 6a2a 1900 6420 652a  ..dFe.e.j*..d e*
+00000880: 6606 8700 6601 6449 644a 840d 5a2d 090b  f...f.dIdJ..Z-..
+00000890: 090b 646d 640e 650c 652c 6504 1900 1900  ..dmd.e.e,e.....
+000008a0: 6446 650c 6518 6a2a 1900 6420 6522 652a  dFe.e.j*..d e"e*
+000008b0: 650d 6504 1900 6602 1900 6606 8700 6601  e.e...f...f...f.
+000008c0: 644b 644c 840d 5a2e 090b 090b 090c 646e  dKdL..Z.......dn
+000008d0: 640e 650c 652c 6504 1900 1900 6423 650c  d.e.e,e.....d#e.
+000008e0: 650e 6516 1900 1900 644d 650f 6420 6522  e.e.....dMe.d e"
+000008f0: 6516 650d 6504 1900 6602 1900 6608 644e  e.e.e...f...f.dN
+00000900: 644f 8405 5a2f 090b 090b 090c 646e 640e  dO..Z/......dnd.
+00000910: 650c 652c 6504 1900 1900 6423 650c 650e  e.e,e.....d#e.e.
+00000920: 6516 1900 1900 644d 650f 6420 6516 6608  e.....dMe.d e.f.
+00000930: 6450 6451 8405 5a30 090b 090c 646a 640e  dPdQ..Z0....djd.
+00000940: 6518 6a2a 6423 650c 650e 6516 1900 1900  e.j*d#e.e.e.....
+00000950: 644d 650f 6420 6516 6608 6452 6453 8405  dMe.d e.f.dRdS..
+00000960: 5a31 651c 6454 6532 6504 650b 6602 1900  Z1e.dTe2e.e.f...
+00000970: 6423 650e 6516 1900 6420 6532 6504 650b  d#e.e...d e2e.e.
+00000980: 6602 1900 6606 6455 6456 8404 8301 5a33  f...f.dUdV....Z3
+00000990: 651e 6423 6514 6515 6424 650b 6602 1900  e.d#e.e.d$e.f...
+000009a0: 650e 6516 1900 6602 1900 6420 650c 6504  e.e...f...d e.e.
+000009b0: 1900 6604 6457 6458 8404 8301 5a34 651e  ..f.dWdX....Z4e.
+000009c0: 6431 6518 6a19 6423 6514 6515 6424 650b  d1e.j.d#e.e.d$e.
+000009d0: 6602 1900 650e 6516 1900 6602 1900 6420  f...e.e...f...d 
+000009e0: 640b 6606 6459 645a 8404 8301 5a35 651e  d.f.dYdZ....Z5e.
+000009f0: 090b 090b 090b 646f 6431 6400 642a 6515  ......dod1d.d*e.
+00000a00: 6424 650b 6602 1900 640e 650d 6504 1900  d$e.f...d.e.e...
+00000a10: 6423 650c 650e 650b 1900 1900 645b 650c  d#e.e.e.....d[e.
+00000a20: 6515 6424 650b 6602 1900 1900 645c 650c  e.d$e.f.....d\e.
+00000a30: 650b 1900 6420 650b 660e 645d 645e 8405  e...d e.f.d]d^..
+00000a40: 8301 5a36 651e 090b 090b 090b 646f 645f  ..Z6e.......dod_
+00000a50: 650c 6515 6424 650b 6602 1900 1900 6460  e.e.d$e.f.....d`
+00000a60: 650c 652c 6515 6424 650b 6602 1900 1900  e.e,e.d$e.f.....
+00000a70: 1900 6461 650c 6532 6504 6515 6424 650b  ..dae.e2e.e.d$e.
+00000a80: 6602 1900 6602 1900 1900 6418 650b 6420  f...f.....d.e.d 
+00000a90: 6400 660a 6462 6463 8405 8301 5a37 651e  d.f.dbdc....Z7e.
+00000aa0: 640b 640b 6464 9c02 6465 650b 640e 650c  d.d.dd..dee.d.e.
+00000ab0: 650d 6504 1900 1900 6466 650c 650d 6504  e.e.....dfe.e.e.
+00000ac0: 1900 1900 6467 650b 6420 650b 660a 6468  ....dge.d e.f.dh
+00000ad0: 6469 8406 8301 5a38 8700 0400 5a39 5300  di....Z8....Z9S.
+00000ae0: 2970 da0e 4172 6775 6d65 6e74 5061 7273  )p..ArgumentPars
+00000af0: 6572 5a0a 5f72 6f6f 745f 6675 6e63 da13  erZ._root_func..
+00000b00: 524f 4f54 5f46 554e 435f 4154 5452 5f4e  ROOT_FUNC_ATTR_N
+00000b10: 414d 455a 155f 726f 6f74 5f66 756e 635f  AMEZ._root_func_
+00000b20: 6172 6773 5f6d 6f64 656c da18 524f 4f54  args_model..ROOT
+00000b30: 5f46 554e 435f 4152 4753 5f41 5454 525f  _FUNC_ARGS_ATTR_
+00000b40: 4e41 4d45 5a08 5f63 6f6d 6d61 6e64 da0d  NAMEZ._command..
+00000b50: 434d 445f 4154 5452 5f4e 414d 455a 0d5f  CMD_ATTR_NAMEZ._
+00000b60: 636f 6d6d 616e 645f 6675 6e63 da12 434d  command_func..CM
+00000b70: 445f 4655 4e43 5f41 5454 525f 4e41 4d45  D_FUNC_ATTR_NAME
+00000b80: 5a18 5f63 6f6d 6d61 6e64 5f66 756e 635f  Z._command_func_
+00000b90: 6172 6773 5f6d 6f64 656c da17 434d 445f  args_model..CMD_
+00000ba0: 4655 4e43 5f41 5247 535f 4154 5452 5f4e  FUNC_ARGS_ATTR_N
+00000bb0: 414d 454e 4629 09da 0470 726f 67da 0c70  AMENF)...prog..p
+00000bc0: 726f 675f 7665 7273 696f 6eda 0b64 6573  rog_version..des
+00000bd0: 6372 6970 7469 6f6e da0a 6865 6c70 5f66  cription..help_f
+00000be0: 6c61 6773 da0d 7665 7273 696f 6e5f 666c  lags..version_fl
+00000bf0: 6167 73da 0974 7569 5f66 6c61 6773 da10  ags..tui_flags..
+00000c00: 636f 6d70 6c65 7469 6f6e 5f66 6c61 6773  completion_flags
+00000c10: da0f 666f 726d 6174 7465 725f 636c 6173  ..formatter_clas
+00000c20: 73da 0d5f 6973 5f73 7562 7061 7273 6572  s.._is_subparser
+00000c30: da04 6172 6773 7247 0000 0072 4800 0000  ..argsrG...rH...
+00000c40: 7249 0000 0072 4a00 0000 724b 0000 0072  rI...rJ...rK...r
+00000c50: 4c00 0000 724d 0000 0072 4e00 0000 724f  L...rM...rN...rO
+00000c60: 0000 00da 066b 7761 7267 7363 0100 0000  .....kwargsc....
+00000c70: 0000 0000 0900 0000 0d00 0000 0800 0000  ................
+00000c80: 0f00 0000 73ee 0100 0074 0083 006a 017c  ....s....t...j.|
+00000c90: 0a7c 017c 0972 0964 006e 017c 0364 017c  .|.|.r.d.n.|.d.|
+00000ca0: 0864 029c 047c 0ba4 018e 0101 0064 007c  .d...|.......d.|
+00000cb0: 005f 0264 037c 006a 035f 047c 0464 0075  ._.d.|.j._.|.d.u
+00000cc0: 0072 2164 0464 0567 027d 047c 0472 3974  .r!d.d.g.}.|.r9t
+00000cd0: 057c 0474 0683 0272 2b7c 0467 017d 047c  .|.t...r+|.g.}.|
+00000ce0: 006a 0764 0664 0784 007c 0444 0083 0174  .j.d.d...|.D...t
+00000cf0: 0864 0864 099c 028e 0101 0064 0a7c 005f  .d.d.......d.|._
+00000d00: 0974 0a64 0b64 0c84 0083 017c 005f 0b69  .t.d.d.....|._.i
+00000d10: 007c 005f 0c7c 0973 f17c 0472 5a64 0d64  .|._.|.s.|.rZd.d
+00000d20: 0784 007c 0444 0083 017d 0c7c 006a 077c  ...|.D...}.|.j.|
+00000d30: 0c74 0d64 0e64 099c 028e 0101 007c 0564  .t.d.d.......|.d
+00000d40: 0075 0072 6164 0f67 017d 057c 0572 9974  .u.rad.g.}.|.r.t
+00000d50: 057c 0574 0683 0272 6b7c 0567 017d 057c  .|.t...rk|.g.}.|
+00000d60: 006a 0e72 8a7c 0273 8a74 0f74 1083 018f  .j.r.|.s.t.t....
+00000d70: 0e01 0074 117c 006a 0e83 016a 127d 0257  ...t.|.j...j.}.W
+00000d80: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00000d90: 8577 0101 0001 0001 0059 0001 007c 0272  .w.......Y...|.r
+00000da0: 997c 006a 077c 0564 1064 117c 029b 009d  .|.j.|.d.d.|....
+00000db0: 0264 1264 139c 038e 0101 007c 0764 0075  .d.d.......|.d.u
+00000dc0: 0072 a064 1467 017d 0774 1372 b97c 0772  .r.d.g.}.t.r.|.r
+00000dd0: b974 057c 0774 0683 0272 ac7c 0767 017d  .t.|.t...r.|.g.}
+00000de0: 077c 006a 077c 0774 1483 0074 156a 1674  .|.j.|.t...t.j.t
+00000df0: 1764 1564 169c 048e 0101 007c 0664 0075  .d.d.......|.d.u
+00000e00: 0072 c064 1767 017d 067c 0672 f374 1872  .r.d.g.}.|.r.t.r
+00000e10: f574 057c 0674 0683 0272 cc7c 0667 017d  .t.|.t...r.|.g.}
+00000e20: 0674 197c 0683 0164 186b 0272 e87c 0664  .t.|...d.k.r.|.d
+00000e30: 1919 00a0 1a64 1aa1 0173 e87c 00a0 1ba1  .....d...s.|....
+00000e40: 0001 0074 1c7c 007c 0664 1919 0064 1b64  ...t.|.|.d...d.d
+00000e50: 1c8d 0301 0064 0053 0074 1d7c 007c 0664  .....d.S.t.|.|.d
+00000e60: 1b64 1c8d 0301 0064 0053 0064 0053 0064  .d.....d.S.d.S.d
+00000e70: 0053 0064 0053 0029 1d4e 4629 0472 4700  .S.d.S.).NF).rG.
+00000e80: 0000 7249 0000 00da 0861 6464 5f68 656c  ..rI.....add_hel
+00000e90: 7072 4e00 0000 7a12 6865 6c70 6675 6c20  prN...z.helpful 
+00000ea0: 7061 7261 6d65 7465 7273 7a02 2d68 7a06  parametersz.-hz.
+00000eb0: 2d2d 6865 6c70 6301 0000 0000 0000 0000  --helpc.........
+00000ec0: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00000ed0: 1400 0000 6700 7c00 5d06 7d01 7c01 7202  ....g.|.].}.|.r.
+00000ee0: 7c01 9102 7102 5300 a900 7253 0000 00a9  |...q.S...rS....
+00000ef0: 02da 022e 30da 0178 7253 0000 0072 5300  ....0..xrS...rS.
+00000f00: 0000 fa26 2f64 726f 6e65 2f73 7263 2f73  ...&/drone/src/s
+00000f10: 7263 2f79 6170 782f 6172 6775 6d65 6e74  rc/yapx/argument
+00000f20: 5f70 6172 7365 722e 7079 da0a 3c6c 6973  _parser.py..<lis
+00000f30: 7463 6f6d 703e 7600 0000 7302 0000 0014  tcomp>v...s.....
+00000f40: 007a 2b41 7267 756d 656e 7450 6172 7365  .z+ArgumentParse
+00000f50: 722e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  r.__init__.<loca
+00000f60: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a17  ls>.<listcomp>z.
+00000f70: 5368 6f77 2074 6869 7320 6865 6c70 206d  Show this help m
+00000f80: 6573 7361 6765 2e29 02da 0661 6374 696f  essage.)...actio
+00000f90: 6eda 0468 656c 70fa 013d 6300 0000 0000  n..help..=c.....
+00000fa0: 0000 0000 0000 0000 0000 0002 0000 0053  ...............S
+00000fb0: 0000 0073 0800 0000 7400 7401 8301 5300  ...s....t.t...S.
+00000fc0: a901 4e29 0272 0200 0000 da04 6c69 7374  ..N).r......list
+00000fd0: 7253 0000 0072 5300 0000 7253 0000 0072  rS...rS...rS...r
+00000fe0: 5700 0000 da08 3c6c 616d 6264 613e 8000  W.....<lambda>..
+00000ff0: 0000 7302 0000 0008 007a 2941 7267 756d  ..s......z)Argum
+00001000: 656e 7450 6172 7365 722e 5f5f 696e 6974  entParser.__init
+00001010: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  __.<locals>.<lam
+00001020: 6264 613e 6301 0000 0000 0000 0000 0000  bda>c...........
+00001030: 0002 0000 0005 0000 0053 0000 0073 2000  .........S...s .
+00001040: 0000 6700 7c00 5d0c 7d01 7c01 a000 6400  ..g.|.].}.|...d.
+00001050: a101 7202 7c01 9b00 6401 9d02 9102 7102  ..r.|...d.....q.
+00001060: 5300 2902 7a02 2d2d 7a04 2d61 6c6c a901  S.).z.--z.-all..
+00001070: da0a 7374 6172 7473 7769 7468 7254 0000  ..startswithrT..
+00001080: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
+00001090: 7258 0000 0086 0000 00f3 0200 0000 2000  rX............ .
+000010a0: 7a1b 5368 6f77 2068 656c 7020 666f 7220  z.Show help for 
+000010b0: 616c 6c20 636f 6d6d 616e 6473 2e7a 092d  all commands.z.-
+000010c0: 2d76 6572 7369 6f6e da07 7665 7273 696f  -version..versio
+000010d0: 6e7a 0925 2870 726f 6729 7320 7a20 5368  nz.%(prog)s z Sh
+000010e0: 6f77 2074 6865 2070 726f 6772 616d 2076  ow the program v
+000010f0: 6572 7369 6f6e 206e 756d 6265 722e 2903  ersion number.).
+00001100: 7259 0000 0072 6200 0000 725a 0000 007a  rY...rb...rZ...z
+00001110: 182d 2d70 7269 6e74 2d73 6865 6c6c 2d63  .--print-shell-c
+00001120: 6f6d 706c 6574 696f 6e7a 1e50 7269 6e74  ompletionz.Print
+00001130: 2073 6865 6c6c 2063 6f6d 706c 6574 696f   shell completio
+00001140: 6e20 7363 7269 7074 2e29 0472 5900 0000  n script.).rY...
+00001150: da07 6465 6661 756c 74da 0763 686f 6963  ..default..choic
+00001160: 6573 725a 0000 007a 052d 2d74 7569 7217  esrZ...z.--tuir.
+00001170: 0000 0072 0100 0000 fa01 2d7a 2253 686f  ...r......-z"Sho
+00001180: 7720 5465 7874 7561 6c20 5573 6572 2049  w Textual User I
+00001190: 6e74 6572 6661 6365 2028 5455 4929 2e29  nterface (TUI).)
+000011a0: 03da 0670 6172 7365 72da 0e6f 7074 696f  ...parser..optio
+000011b0: 6e5f 7374 7269 6e67 7372 5a00 0000 291e  n_stringsrZ...).
+000011c0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+000011d0: 5fda 125f 7375 6270 6172 7365 7273 5f61  _.._subparsers_a
+000011e0: 6374 696f 6eda 0a5f 6f70 7469 6f6e 616c  ction.._optional
+000011f0: 73da 0574 6974 6c65 da0a 6973 696e 7374  s..title..isinst
+00001200: 616e 6365 da03 7374 72da 0c61 6464 5f61  ance..str..add_a
+00001210: 7267 756d 656e 7472 1b00 0000 da0c 6b76  rgumentr......kv
+00001220: 5f73 6570 6172 6174 6f72 7202 0000 00da  _separatorr.....
+00001230: 185f 6d75 7475 616c 6c79 5f65 7863 6c75  ._mutually_exclu
+00001240: 7369 7665 5f61 7267 73da 0a5f 6465 7374  sive_args.._dest
+00001250: 5f74 7970 6572 1c00 0000 7247 0000 0072  _typer....rG...r
+00001260: 0300 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
+00001270: 1600 0000 7262 0000 0072 3600 0000 7232  ....rb...r6...r2
+00001280: 0000 00da 0861 7267 7061 7273 65da 0853  .....argparse..S
+00001290: 5550 5052 4553 5372 2c00 0000 7237 0000  UPPRESSr,...r7..
+000012a0: 00da 036c 656e 7260 0000 00da 165f 6765  ...lenr`....._ge
+000012b0: 745f 6f72 5f61 6464 5f73 7562 7061 7273  t_or_add_subpars
+000012c0: 6572 7372 3000 0000 722f 0000 0029 0dda  ersr0...r/...)..
+000012d0: 0473 656c 6672 4700 0000 7248 0000 0072  .selfrG...rH...r
+000012e0: 4900 0000 724a 0000 0072 4b00 0000 724c  I...rJ...rK...rL
+000012f0: 0000 0072 4d00 0000 724e 0000 0072 4f00  ...rM...rN...rO.
+00001300: 0000 7250 0000 0072 5100 0000 5a0e 6865  ..rP...rQ...Z.he
+00001310: 6c70 5f61 6c6c 5f66 6c61 6773 a901 da09  lp_all_flags....
+00001320: 5f5f 636c 6173 735f 5f72 5300 0000 7257  __class__rS...rW
+00001330: 0000 0072 6900 0000 5300 0000 73a0 0000  ...ri...S...s...
+00001340: 0006 0e02 0102 010a 0102 0102 0104 fb02  ................
+00001350: 0606 fa06 0908 0308 0208 0104 020a 0106  ................
+00001360: 0104 010c 0102 0102 0108 fd06 060a 0504  ................
+00001370: fd06 0504 0204 010e 0104 0102 0102 0102  ................
+00001380: 0108 fd08 0606 0104 020a 0106 010a 020a  ................
+00001390: 010e 011c ff04 0304 0102 0102 0108 0102  ................
+000013a0: 0108 fc08 0706 0108 020a 0106 0104 0202  ................
+000013b0: 0104 0104 0102 0102 0108 fb08 0806 0108  ................
+000013c0: 020a 0106 011a 0208 0102 0102 0106 0102  ................
+000013d0: 010a fd02 0602 0102 0102 010a fd04 c608  ................
+000013e0: 2e7a 1741 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
+000013f0: 722e 5f5f 696e 6974 5f5f da07 6d65 7373  r.__init__..mess
+00001400: 6167 6563 0200 0000 0000 0000 0000 0000  agec............
+00001410: 0200 0000 0600 0000 4300 0000 7324 0000  ........C...s$..
+00001420: 007c 00a0 0074 016a 02a1 0101 007c 00a0  .|...t.j.....|..
+00001430: 0364 0164 027c 019b 0064 039d 03a1 0201  .d.d.|...d......
+00001440: 0064 0053 0029 044e e902 0000 007a 0765  .d.S.).N.....z.e
+00001450: 7272 6f72 3a20 da01 0a29 04da 0b70 7269  rror: ...)...pri
+00001460: 6e74 5f75 7361 6765 da03 7379 73da 0673  nt_usage..sys..s
+00001470: 7464 6572 72da 0465 7869 7429 0272 7800  tderr..exit).rx.
+00001480: 0000 727b 0000 0072 5300 0000 7253 0000  ..r{...rS...rS..
+00001490: 0072 5700 0000 da05 6572 726f 72c4 0000  .rW.....error...
+000014a0: 0073 0400 0000 0c01 1801 7a14 4172 6775  .s........z.Argu
+000014b0: 6d65 6e74 5061 7273 6572 2e65 7272 6f72  mentParser.error
+000014c0: da04 6669 6c65 da10 696e 636c 7564 655f  ..file..include_
+000014d0: 636f 6d6d 616e 6473 da06 7265 7475 726e  commands..return
+000014e0: 6303 0000 0000 0000 0000 0000 0008 0000  c...............
+000014f0: 0005 0000 0003 0000 0073 9c00 0000 6401  .........s....d.
+00001500: 7d03 7c03 6402 1400 6403 1700 7d04 7400  }.|.d...d...}.t.
+00001510: 8300 0100 7400 7c04 8301 0100 7400 6404  ....t.|.....t.d.
+00001520: 7c00 6a01 9b00 9d02 8301 0100 7400 7c04  |.j.........t.|.
+00001530: 8301 0100 7c00 6a02 7d05 7403 6a04 7c00  ....|.j.}.t.j.|.
+00001540: 5f02 7405 8300 a006 7c01 a101 0100 7c02  _.t.....|.....|.
+00001550: 7249 7c00 6a07 7249 7c00 6a08 6405 7500  rI|.j.rI|.j.d.u.
+00001560: 7237 7c00 a009 a100 7c00 5f08 7c00 6a08  r7|.....|._.|.j.
+00001570: 6a0a a00b a100 4400 5d0b 5c02 7d06 7d07  j.....D.].\.}.}.
+00001580: 7c07 6a06 7c01 7c02 6406 8d02 0100 713d  |.j.|.|.d.....q=
+00001590: 7c05 7c00 5f02 6405 5300 2907 6118 0200  |.|._.d.S.).a...
+000015a0: 0050 7269 6e74 2043 4c49 2068 656c 702e  .Print CLI help.
+000015b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000015c0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+000015d0: 7564 655f 636f 6d6d 616e 6473 3a20 6966  ude_commands: if
+000015e0: 2054 7275 652c 2061 6c73 6f20 7072 696e   True, also prin
+000015f0: 7420 6865 6c70 2066 6f72 2065 6163 6820  t help for each 
+00001600: 636f 6d6d 616e 642e 0a0a 2020 2020 2020  command...      
+00001610: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+00001620: 2020 2020 2020 2020 3e3e 3e20 696d 706f          >>> impo
+00001630: 7274 2079 6170 780a 2020 2020 2020 2020  rt yapx.        
+00001640: 2020 2020 3e3e 3e20 6672 6f6d 2064 6174      >>> from dat
+00001650: 6163 6c61 7373 6573 2069 6d70 6f72 7420  aclasses import 
+00001660: 6461 7461 636c 6173 730a 2020 2020 2020  dataclass.      
+00001670: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00001680: 2020 2020 2020 3e3e 3e20 4064 6174 6163        >>> @datac
+00001690: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
+000016a0: 202e 2e2e 2063 6c61 7373 2041 6464 4e75   ... class AddNu
+000016b0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+000016c0: 2e2e 2e20 2020 2020 783a 2069 6e74 0a20  ...     x: int. 
+000016d0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+000016e0: 2020 2079 3a20 696e 740a 2020 2020 2020     y: int.      
+000016f0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00001700: 2020 2020 2020 3e3e 3e20 7061 7273 6572        >>> parser
+00001710: 203d 2079 6170 782e 4172 6775 6d65 6e74   = yapx.Argument
+00001720: 5061 7273 6572 2829 0a20 2020 2020 2020  Parser().       
+00001730: 2020 2020 203e 3e3e 2070 6172 7365 722e       >>> parser.
+00001740: 6164 645f 6172 6775 6d65 6e74 7328 4164  add_arguments(Ad
+00001750: 644e 756d 7329 0a20 2020 2020 2020 2020  dNums).         
+00001760: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00001770: 2020 203e 3e3e 2070 6172 7365 722e 7072     >>> parser.pr
+00001780: 696e 745f 6865 6c70 2869 6e63 6c75 6465  int_help(include
+00001790: 5f63 6f6d 6d61 6e64 733d 5472 7565 2920  _commands=True) 
+000017a0: 2023 646f 6374 6573 743a 202b 534b 4950   #doctest: +SKIP
+000017b0: 0a20 2020 2020 2020 20da 015f e950 0000  .        .._.P..
+000017c0: 0072 7d00 0000 7a02 2420 4e29 0172 8400  .r}...z.$ N).r..
+000017d0: 0000 290c da05 7072 696e 7472 4700 0000  ..)...printrG...
+000017e0: da05 7573 6167 6572 7400 0000 7275 0000  ..usagert...ru..
+000017f0: 0072 6800 0000 da0a 7072 696e 745f 6865  .rh.....print_he
+00001800: 6c70 da0b 5f73 7562 7061 7273 6572 7372  lp.._subparsersr
+00001810: 6a00 0000 da17 5f66 696e 645f 7375 6270  j....._find_subp
+00001820: 6172 7365 7273 5f61 6374 696f 6e72 6400  arsers_actionrd.
+00001830: 0000 da05 6974 656d 7329 0872 7800 0000  ....items).rx...
+00001840: 7283 0000 0072 8400 0000 5a08 7365 705f  r....r....Z.sep_
+00001850: 6368 6172 da09 7365 7061 7261 746f 7272  char..separatorr
+00001860: 8900 0000 5a07 5f63 686f 6963 655a 0973  ....Z._choiceZ.s
+00001870: 7562 7061 7273 6572 7279 0000 0072 5300  ubparserry...rS.
+00001880: 0000 7257 0000 0072 8a00 0000 c800 0000  ..rW...r........
+00001890: 731e 0000 0004 180c 0106 0108 0110 0108  s...............
+000018a0: 0106 0308 010c 020a 020a 010a 0114 0210  ................
+000018b0: 010a 027a 1941 7267 756d 656e 7450 6172  ...z.ArgumentPar
+000018c0: 7365 722e 7072 696e 745f 6865 6c70 da0a  ser.print_help..
+000018d0: 6172 6773 5f6d 6f64 656c 2e63 0200 0000  args_model.c....
+000018e0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000018f0: 4300 0000 7310 0000 007c 00a0 007c 007c  C...s....|...|.|
+00001900: 01a1 0201 0064 0153 0029 0261 d605 0000  .....d.S.).a....
+00001910: 4164 6420 6172 6775 6d65 6e74 7320 6672  Add arguments fr
+00001920: 6f6d 2074 6865 2067 6976 656e 2066 756e  om the given fun
+00001930: 6374 696f 6e20 6f72 2064 6174 6166 7261  ction or datafra
+00001940: 6d65 2e0a 0a20 2020 2020 2020 2041 7267  me...        Arg
+00001950: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00001960: 7267 735f 6d6f 6465 6c3a 2061 2066 756e  rgs_model: a fun
+00001970: 6374 696f 6e20 6f72 2064 6174 6163 6c61  ction or datacla
+00001980: 7373 2066 726f 6d20 7768 6963 6820 746f  ss from which to
+00001990: 2064 6572 6976 6520 6172 6775 6d65 6e74   derive argument
+000019a0: 732e 0a0a 2020 2020 2020 2020 4578 616d  s...        Exam
+000019b0: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
+000019c0: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
+000019d0: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
+000019e0: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
+000019f0: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00001a00: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+00001a10: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00001a20: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
+00001a30: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
+00001a40: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
+00001a50: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00001a60: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
+00001a70: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
+00001a80: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00001a90: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00001aa0: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
+00001ab0: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
+00001ac0: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
+00001ad0: 3e3e 2070 6172 7365 722e 6164 645f 6172  >> parser.add_ar
+00001ae0: 6775 6d65 6e74 7328 4164 644e 756d 7329  guments(AddNums)
+00001af0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00001b00: 2070 6172 7365 722e 7365 745f 6465 6661   parser.set_defa
+00001b10: 756c 7473 285f 636f 6d6d 616e 645f 6675  ults(_command_fu
+00001b20: 6e63 3d6c 616d 6264 6120 782c 2079 3a20  nc=lambda x, y: 
+00001b30: 782b 7929 0a20 2020 2020 2020 2020 2020  x+y).           
+00001b40: 203e 3e3e 2070 6172 7365 6420 3d20 7061   >>> parsed = pa
+00001b50: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
+00001b60: 5b27 2d78 272c 2027 3127 2c20 272d 7927  ['-x', '1', '-y'
+00001b70: 2c20 2732 275d 290a 2020 2020 2020 2020  , '2']).        
+00001b80: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00001b90: 2020 2020 3e3e 3e20 2870 6172 7365 642e      >>> (parsed.
+00001ba0: 782c 2070 6172 7365 642e 7929 0a20 2020  x, parsed.y).   
+00001bb0: 2020 2020 2020 2020 2028 312c 2032 290a           (1, 2).
+00001bc0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00001bd0: 7061 7273 6564 2e5f 636f 6d6d 616e 645f  parsed._command_
+00001be0: 6675 6e63 5f61 7267 735f 6d6f 6465 6c28  func_args_model(
+00001bf0: 783d 7061 7273 6564 2e78 2c20 793d 7061  x=parsed.x, y=pa
+00001c00: 7273 6564 2e79 290a 2020 2020 2020 2020  rsed.y).        
+00001c10: 2020 2020 4164 644e 756d 7328 783d 312c      AddNums(x=1,
+00001c20: 2079 3d32 290a 2020 2020 2020 2020 2020   y=2).          
+00001c30: 2020 3e3e 3e20 7061 7273 6564 2e5f 636f    >>> parsed._co
+00001c40: 6d6d 616e 645f 6675 6e63 2878 3d70 6172  mmand_func(x=par
+00001c50: 7365 642e 782c 2079 3d70 6172 7365 642e  sed.x, y=parsed.
+00001c60: 7929 0a20 2020 2020 2020 2020 2020 2033  y).            3
+00001c70: 0a0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+00001c80: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
+00001c90: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
+00001ca0: 2020 2020 2020 2020 2020 3e3e 3e20 6465            >>> de
+00001cb0: 6620 6164 645f 6e75 6d73 2878 3a20 696e  f add_nums(x: in
+00001cc0: 742c 2079 3a20 696e 7429 3a0a 2020 2020  t, y: int):.    
+00001cd0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00001ce0: 7265 7475 726e 2078 202b 2079 0a20 2020  return x + y.   
+00001cf0: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
+00001d00: 2020 2020 2020 2020 203e 3e3e 2070 6172           >>> par
+00001d10: 7365 7220 3d20 7961 7078 2e41 7267 756d  ser = yapx.Argum
+00001d20: 656e 7450 6172 7365 7228 290a 2020 2020  entParser().    
+00001d30: 2020 2020 2020 2020 3e3e 3e20 7061 7273          >>> pars
+00001d40: 6572 2e61 6464 5f61 7267 756d 656e 7473  er.add_arguments
+00001d50: 2861 6464 5f6e 756d 7329 0a20 2020 2020  (add_nums).     
+00001d60: 2020 2020 2020 203e 3e3e 2070 6172 7365         >>> parse
+00001d70: 722e 7365 745f 6465 6661 756c 7473 285f  r.set_defaults(_
+00001d80: 636f 6d6d 616e 645f 6675 6e63 3d61 6464  command_func=add
+00001d90: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
+00001da0: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
+00001db0: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
+00001dc0: 7328 5b27 2d78 272c 2027 3127 2c20 272d  s(['-x', '1', '-
+00001dd0: 7927 2c20 2732 275d 290a 2020 2020 2020  y', '2']).      
+00001de0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00001df0: 2020 2020 2020 3e3e 3e20 2870 6172 7365        >>> (parse
+00001e00: 642e 782c 2070 6172 7365 642e 7929 0a20  d.x, parsed.y). 
+00001e10: 2020 2020 2020 2020 2020 2028 312c 2032             (1, 2
+00001e20: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00001e30: 3e20 7061 7273 6564 2e5f 636f 6d6d 616e  > parsed._comman
+00001e40: 645f 6675 6e63 5f61 7267 735f 6d6f 6465  d_func_args_mode
+00001e50: 6c28 783d 7061 7273 6564 2e78 2c20 793d  l(x=parsed.x, y=
+00001e60: 7061 7273 6564 2e79 290a 2020 2020 2020  parsed.y).      
+00001e70: 2020 2020 2020 4461 7461 636c 6173 735f        Dataclass_
+00001e80: 6164 645f 6e75 6d73 2878 3d31 2c20 793d  add_nums(x=1, y=
+00001e90: 3229 0a20 2020 2020 2020 2020 2020 203e  2).            >
+00001ea0: 3e3e 2070 6172 7365 642e 5f63 6f6d 6d61  >> parsed._comma
+00001eb0: 6e64 5f66 756e 6328 783d 7061 7273 6564  nd_func(x=parsed
+00001ec0: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
+00001ed0: 2020 2020 2020 2020 2020 2020 330a 2020              3.  
+00001ee0: 2020 2020 2020 4e29 01da 0e5f 6164 645f        N)..._add_
+00001ef0: 6172 6775 6d65 6e74 7329 0272 7800 0000  arguments).rx...
+00001f00: 728f 0000 0072 5300 0000 7253 0000 0072  r....rS...rS...r
+00001f10: 5700 0000 da0d 6164 645f 6172 6775 6d65  W.....add_argume
+00001f20: 6e74 73f6 0000 0073 0200 0000 102f 7a1c  nts....s...../z.
+00001f30: 4172 6775 6d65 6e74 5061 7273 6572 2e61  ArgumentParser.a
+00001f40: 6464 5f61 7267 756d 656e 7473 da04 6e61  dd_arguments..na
+00001f50: 6d65 6303 0000 0000 0000 0000 0000 0009  mec.............
+00001f60: 0000 0005 0000 004b 0000 0073 9800 0000  .......K...s....
+00001f70: 7c00 a000 a100 7d04 7c02 730b 7401 7c01  |.....}.|.s.t.|.
+00001f80: 6a02 8301 7d02 7403 7c04 7404 6a05 8302  j...}.t.|.t.j...
+00001f90: 7313 4a00 8201 7c03 a006 6401 6402 a102  s.J...|...d.d...
+00001fa0: 7d05 7c05 7221 7c05 6403 7c02 1700 3700  }.|.r!|.d.|...7.
+00001fb0: 7d05 7c00 6a07 7c01 6404 8d01 7d06 6402  }.|.j.|.d...}.d.
+00001fc0: 7d07 7c06 7231 7c06 a008 a100 6405 1900  }.|.r1|.....d...
+00001fd0: 7d07 7c04 6a09 7c02 6601 7c05 7c07 6406  }.|.j.|.f.|.|.d.
+00001fe0: 9c02 7c03 a401 8e01 7d08 7c06 7242 7c06  ..|.....}.|.rB|.
+00001ff0: 7c08 5f0a 7c01 724a 7c00 a00b 7c08 7c01  |._.|.rJ|...|.|.
+00002000: a102 0100 7c08 5300 2907 6159 0800 0043  ....|.S.).aY...C
+00002010: 7265 6174 6520 6120 6e65 7720 7375 6263  reate a new subc
+00002020: 6f6d 6d61 6e64 2061 6e64 2061 6464 2061  ommand and add a
+00002030: 7267 756d 656e 7473 2066 726f 6d20 7468  rguments from th
+00002040: 6520 6769 7665 6e20 6675 6e63 7469 6f6e  e given function
+00002050: 206f 7220 6461 7461 6672 616d 6520 746f   or dataframe to
+00002060: 2069 742e 0a0a 2020 2020 2020 2020 4172   it...        Ar
+00002070: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00002080: 6172 6773 5f6d 6f64 656c 3a20 6120 6675  args_model: a fu
+00002090: 6e63 7469 6f6e 206f 7220 6461 7461 636c  nction or datacl
+000020a0: 6173 7320 6672 6f6d 2077 6869 6368 2074  ass from which t
+000020b0: 6f20 6465 7269 7665 2061 7267 756d 656e  o derive argumen
+000020c0: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+000020d0: 6e61 6d65 3a20 6e61 6d65 206f 6620 7468  name: name of th
+000020e0: 6520 636f 6d6d 616e 640a 0a20 2020 2020  e command..     
+000020f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00002100: 2020 2020 2020 2020 7468 6520 6e65 7720          the new 
+00002110: 6172 6770 6172 7365 2073 7562 7061 7273  argparse subpars
+00002120: 6572 0a0a 2020 2020 2020 2020 4578 616d  er..        Exam
+00002130: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
+00002140: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
+00002150: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
+00002160: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
+00002170: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00002180: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+00002190: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+000021a0: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
+000021b0: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
+000021c0: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
+000021d0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+000021e0: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
+000021f0: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
+00002200: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00002210: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00002220: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
+00002230: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
+00002240: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
+00002250: 3e3e 2073 7562 7061 7273 6572 5f31 203d  >> subparser_1 =
+00002260: 2070 6172 7365 722e 6164 645f 636f 6d6d   parser.add_comm
+00002270: 616e 6428 4164 644e 756d 732c 206e 616d  and(AddNums, nam
+00002280: 653d 2761 6464 2729 0a20 2020 2020 2020  e='add').       
+00002290: 2020 2020 203e 3e3e 2073 7562 7061 7273       >>> subpars
+000022a0: 6572 5f31 2e73 6574 5f64 6566 6175 6c74  er_1.set_default
+000022b0: 7328 5f63 6f6d 6d61 6e64 5f66 756e 633d  s(_command_func=
+000022c0: 6c61 6d62 6461 2078 2c20 793a 2078 2b79  lambda x, y: x+y
+000022d0: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+000022e0: 3e20 7375 6270 6172 7365 725f 3220 3d20  > subparser_2 = 
+000022f0: 7061 7273 6572 2e61 6464 5f63 6f6d 6d61  parser.add_comma
+00002300: 6e64 2841 6464 4e75 6d73 2c20 6e61 6d65  nd(AddNums, name
+00002310: 3d27 7375 6274 7261 6374 2729 0a20 2020  ='subtract').   
+00002320: 2020 2020 2020 2020 203e 3e3e 2073 7562           >>> sub
+00002330: 7061 7273 6572 5f32 2e73 6574 5f64 6566  parser_2.set_def
+00002340: 6175 6c74 7328 5f63 6f6d 6d61 6e64 5f66  aults(_command_f
+00002350: 756e 633d 6c61 6d62 6461 2078 2c20 793a  unc=lambda x, y:
+00002360: 2078 2d79 290a 2020 2020 2020 2020 2020   x-y).          
+00002370: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+00002380: 2020 3e3e 3e20 7061 7273 6564 203d 2070    >>> parsed = p
+00002390: 6172 7365 722e 7061 7273 655f 6172 6773  arser.parse_args
+000023a0: 285b 2761 6464 272c 2027 2d78 272c 2027  (['add', '-x', '
+000023b0: 3127 2c20 272d 7927 2c20 2732 275d 290a  1', '-y', '2']).
+000023c0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+000023d0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+000023e0: 2870 6172 7365 642e 782c 2070 6172 7365  (parsed.x, parse
+000023f0: 642e 7929 0a20 2020 2020 2020 2020 2020  d.y).           
+00002400: 2028 312c 2032 290a 2020 2020 2020 2020   (1, 2).        
+00002410: 2020 2020 3e3e 3e20 7061 7273 6564 2e5f      >>> parsed._
+00002420: 636f 6d6d 616e 645f 6675 6e63 5f61 7267  command_func_arg
+00002430: 735f 6d6f 6465 6c28 783d 7061 7273 6564  s_model(x=parsed
+00002440: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
+00002450: 2020 2020 2020 2020 2020 2020 4164 644e              AddN
+00002460: 756d 7328 783d 312c 2079 3d32 290a 2020  ums(x=1, y=2).  
+00002470: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
+00002480: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
+00002490: 6e63 2878 3d70 6172 7365 642e 782c 2079  nc(x=parsed.x, y
+000024a0: 3d70 6172 7365 642e 7929 0a20 2020 2020  =parsed.y).     
+000024b0: 2020 2020 2020 2033 0a0a 2020 2020 2020         3..      
+000024c0: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
+000024d0: 2079 6170 780a 2020 2020 2020 2020 2020   yapx.          
+000024e0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+000024f0: 2020 3e3e 3e20 6465 6620 6164 645f 6e75    >>> def add_nu
+00002500: 6d73 2878 3a20 696e 742c 2079 3a20 696e  ms(x: int, y: in
+00002510: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00002520: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
+00002530: 202b 2079 0a20 2020 2020 2020 2020 2020   + y.           
+00002540: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00002550: 203e 3e3e 2064 6566 2073 7562 7472 6163   >>> def subtrac
+00002560: 745f 6e75 6d73 2878 3a20 696e 742c 2079  t_nums(x: int, y
+00002570: 3a20 696e 7429 3a0a 2020 2020 2020 2020  : int):.        
+00002580: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
+00002590: 726e 2078 202d 2079 0a20 2020 2020 2020  rn x - y.       
+000025a0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+000025b0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
+000025c0: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
+000025d0: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
+000025e0: 2020 2020 3e3e 3e20 7375 6270 6172 7365      >>> subparse
+000025f0: 725f 3120 3d20 7061 7273 6572 2e61 6464  r_1 = parser.add
+00002600: 5f63 6f6d 6d61 6e64 2861 6464 5f6e 756d  _command(add_num
+00002610: 732c 206e 616d 653d 2761 6464 2729 0a20  s, name='add'). 
+00002620: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
+00002630: 7562 7061 7273 6572 5f31 2e73 6574 5f64  ubparser_1.set_d
+00002640: 6566 6175 6c74 7328 5f63 6f6d 6d61 6e64  efaults(_command
+00002650: 5f66 756e 633d 6164 645f 6e75 6d73 290a  _func=add_nums).
+00002660: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00002670: 7375 6270 6172 7365 725f 3220 3d20 7061  subparser_2 = pa
+00002680: 7273 6572 2e61 6464 5f63 6f6d 6d61 6e64  rser.add_command
+00002690: 2873 7562 7472 6163 745f 6e75 6d73 2c20  (subtract_nums, 
+000026a0: 6e61 6d65 3d27 7375 6274 7261 6374 2729  name='subtract')
+000026b0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+000026c0: 2073 7562 7061 7273 6572 5f32 2e73 6574   subparser_2.set
+000026d0: 5f64 6566 6175 6c74 7328 5f63 6f6d 6d61  _defaults(_comma
+000026e0: 6e64 5f66 756e 633d 7375 6274 7261 6374  nd_func=subtract
+000026f0: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
+00002700: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00002710: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
+00002720: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
+00002730: 7328 5b27 7375 6274 7261 6374 272c 2027  s(['subtract', '
+00002740: 2d78 272c 2027 3127 2c20 272d 7927 2c20  -x', '1', '-y', 
+00002750: 2732 275d 290a 2020 2020 2020 2020 2020  '2']).          
+00002760: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+00002770: 2020 3e3e 3e20 2870 6172 7365 642e 782c    >>> (parsed.x,
+00002780: 2070 6172 7365 642e 7929 0a20 2020 2020   parsed.y).     
+00002790: 2020 2020 2020 2028 312c 2032 290a 2020         (1, 2).  
+000027a0: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
+000027b0: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
+000027c0: 6e63 5f61 7267 735f 6d6f 6465 6c28 783d  nc_args_model(x=
+000027d0: 7061 7273 6564 2e78 2c20 793d 7061 7273  parsed.x, y=pars
+000027e0: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
+000027f0: 2020 4461 7461 636c 6173 735f 7375 6274    Dataclass_subt
+00002800: 7261 6374 5f6e 756d 7328 783d 312c 2079  ract_nums(x=1, y
+00002810: 3d32 290a 2020 2020 2020 2020 2020 2020  =2).            
+00002820: 3e3e 3e20 7061 7273 6564 2e5f 636f 6d6d  >>> parsed._comm
+00002830: 616e 645f 6675 6e63 2878 3d70 6172 7365  and_func(x=parse
+00002840: 642e 782c 2079 3d70 6172 7365 642e 7929  d.x, y=parsed.y)
+00002850: 0a20 2020 2020 2020 2020 2020 202d 310a  .            -1.
+00002860: 2020 2020 2020 2020 7247 0000 004e fa01          rG...N..
+00002870: 20a9 0172 8f00 0000 7201 0000 0029 0272   ..r....r....).r
+00002880: 4700 0000 725a 0000 0029 0c72 7700 0000  G...rZ...).rw...
+00002890: 7224 0000 00da 085f 5f6e 616d 655f 5f72  r$.....__name__r
+000028a0: 6d00 0000 7274 0000 00da 115f 5375 6250  m...rt....._SubP
+000028b0: 6172 7365 7273 4163 7469 6f6e da03 706f  arsersAction..po
+000028c0: 70da 1f5f 6765 745f 6465 7363 7269 7074  p.._get_descript
+000028d0: 696f 6e5f 6672 6f6d 5f64 6f63 7374 7269  ion_from_docstri
+000028e0: 6e67 da0a 7370 6c69 746c 696e 6573 da0a  ng..splitlines..
+000028f0: 6164 645f 7061 7273 6572 7249 0000 0072  add_parserrI...r
+00002900: 9000 0000 2909 7278 0000 0072 8f00 0000  ....).rx...r....
+00002910: 7292 0000 0072 5100 0000 5a0a 7375 6270  r....rQ...Z.subp
+00002920: 6172 7365 7273 7247 0000 005a 0f64 6573  arsersrG...Z.des
+00002930: 6372 6970 7469 6f6e 5f74 7874 5a08 6865  cription_txtZ.he
+00002940: 6c70 5f74 7874 7266 0000 0072 5300 0000  lp_txtrf...rS...
+00002950: 7253 0000 0072 5700 0000 da0b 6164 645f  rS...rW.....add_
+00002960: 636f 6d6d 616e 6427 0100 0073 3400 0000  command'...s4...
+00002970: 083e 0402 0a01 1003 0c01 0401 0c01 0404  .>..............
+00002980: 0201 06ff 0403 0401 0c01 0402 0201 02ff  ................
+00002990: 0202 0201 04fd 0204 06fc 0406 0601 0402  ................
+000029a0: 0c01 0402 7a1a 4172 6775 6d65 6e74 5061  ....z.ArgumentPa
+000029b0: 7273 6572 2e61 6464 5f63 6f6d 6d61 6e64  rser.add_command
+000029c0: da04 6675 6e63 6303 0000 0000 0000 0000  ..funcc.........
+000029d0: 0000 0005 0000 0005 0000 004b 0000 0073  ...........K...s
+000029e0: 4200 0000 7400 7c02 7205 7c02 6e02 7c01  B...t.|.r.|.n.|.
+000029f0: 6a01 8301 7d02 7c00 6a02 7c01 6601 6401  j...}.|.j.|.f.d.
+00002a00: 7c02 6901 7c03 a401 8e01 7d04 7c04 6a03  |.i.|.....}.|.j.
+00002a10: 6402 6900 7c00 6a04 7c01 6901 a401 8e01  d.i.|.j.|.i.....
+00002a20: 0100 6400 5300 2903 4e72 9200 0000 7253  ..d.S.).Nr....rS
+00002a30: 0000 0029 0572 2400 0000 7295 0000 0072  ...).r$...r....r
+00002a40: 9b00 0000 da0c 7365 745f 6465 6661 756c  ......set_defaul
+00002a50: 7473 7245 0000 0029 0572 7800 0000 729c  tsrE...).rx...r.
+00002a60: 0000 0072 9200 0000 7251 0000 0072 6600  ...r....rQ...rf.
+00002a70: 0000 7253 0000 0072 5300 0000 7257 0000  ..rS...rS...rW..
+00002a80: 00da 115f 7265 6769 7374 6572 5f63 6f6d  ..._register_com
+00002a90: 6d61 6e64 8701 0000 7312 0000 0012 0604  mand....s.......
+00002aa0: 0102 0104 ff02 0202 fe02 0306 fd1a 057a  ...............z
+00002ab0: 2041 7267 756d 656e 7450 6172 7365 722e   ArgumentParser.
+00002ac0: 5f72 6567 6973 7465 725f 636f 6d6d 616e  _register_comman
+00002ad0: 64da 0464 636c 73da 0461 7474 7263 0200  d..dcls..attrc..
+00002ae0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00002af0: 0000 4300 0000 730a 0000 007c 017c 006a  ..C...s....|.|.j
+00002b00: 0076 0153 0072 5c00 0000 a901 da0f 5f5f  .v.S.r\.......__
+00002b10: 616e 6e6f 7461 7469 6f6e 735f 5fa9 0272  annotations__..r
+00002b20: 9f00 0000 72a0 0000 0072 5300 0000 7253  ....r....rS...rS
+00002b30: 0000 0072 5700 0000 da17 5f69 735f 6174  ...rW....._is_at
+00002b40: 7472 6962 7574 655f 696e 6865 7269 7465  tribute_inherite
+00002b50: 6495 0100 0073 0200 0000 0a02 7a26 4172  d....s......z&Ar
+00002b60: 6775 6d65 6e74 5061 7273 6572 2e5f 6973  gumentParser._is
+00002b70: 5f61 7474 7269 6275 7465 5f69 6e68 6572  _attribute_inher
+00002b80: 6974 6564 7266 0000 0063 0300 0000 0000  itedrf...c......
+00002b90: 0000 0000 0000 1900 0000 0900 0000 0300  ................
+00002ba0: 0000 73f2 0600 0074 007c 0283 0172 077c  ..s....t.|...r.|
+00002bb0: 0289 016e 0474 017c 0283 0189 017c 01a0  ...n.t.|.....|..
+00002bc0: 0288 006a 03a1 0172 1864 017d 037c 01a0  ...j...r.d.}.|..
+00002bd0: 047c 03a1 0101 007c 016a 0564 2269 0088  .|.....|.j.d"i..
+00002be0: 006a 0388 0169 01a4 018e 0101 0069 007d  .j...i.......i.}
+00002bf0: 0474 0674 0787 0087 0166 0264 0264 0384  .t.t.....f.d.d..
+00002c00: 0874 0888 0183 0183 0283 017d 0564 0464  .t.........}.d.d
+00002c10: 0584 007c 0544 0083 017d 0667 007d 077c  ...|.D...}.g.}.|
+00002c20: 0644 0090 035d 375c 027d 087d 097c 086a  .D...]7\.}.}.|.j
+00002c30: 097d 0a74 0a7c 0a74 0b83 0272 4f74 0c7c  .}.t.|.t...rOt.|
+00002c40: 0a83 017d 0a74 0a7c 0a74 0b83 0272 564a  ...}.t.|.t...rVJ
+00002c50: 0082 0174 0d6a 0e64 066b 0572 6074 0a7c  ...t.j.d.k.r`t.|
+00002c60: 0a74 0f83 0273 6788 00a0 107c 0aa1 0174  .t...sg....|...t
+00002c70: 1175 0072 6e88 006a 127c 0a64 0764 088d  .u.rn..j.|.d.d..
+00002c80: 027d 0a74 0a7c 0a74 1383 0272 a988 00a0  .}.t.|.t...r....
+00002c90: 147c 0aa1 0144 005d 137d 0b74 157c 0b74  .|...D.].}.t.|.t
+00002ca0: 1683 0272 8b74 177c 0b6a 1876 0072 8b7c  ...r.t.|.j.v.r.|
+00002cb0: 0b6a 1874 1719 007d 0901 006e 0171 7888  .j.t...}...n.qx.
+00002cc0: 00a0 107c 0aa1 017d 0a74 0d6a 0e64 066b  ...|...}.t.j.d.k
+00002cd0: 0572 9b74 0a7c 0a74 0f83 0273 a288 00a0  .r.t.|.t...s....
+00002ce0: 107c 0aa1 0174 1175 0072 a988 006a 127c  .|...t.u.r...j.|
+00002cf0: 0a64 0764 088d 027d 0a74 0a7c 0a74 0983  .d.d...}.t.|.t..
+00002d00: 0272 b17c 0a6a 196e 0a74 0b7c 0a83 016a  .r.|.j.n.t.|...j
+00002d10: 1a64 0964 0a64 0b8d 0264 0c19 007d 0c7c  .d.d.d...d...}.|
+00002d20: 09a0 1b7c 086a 1ca1 0101 007c 096a 1d72  ...|.j.....|.j.r
+00002d30: df7c 086a 1e74 1f75 0172 d27c 086a 1e7c  .|.j.t.u.r.|.j.|
+00002d40: 095f 1e64 0d7c 095f 1d6e 0d7c 086a 2074  ._.d.|._.n.|.j t
+00002d50: 1f75 0172 df7c 08a0 20a1 007c 095f 1e64  .u.r.|.. ..|._.d
+00002d60: 0d7c 095f 1d88 00a0 107c 0aa1 017d 0d7c  .|._.....|...}.|
+00002d70: 0d90 0172 6f7c 0d90 0172 037c 0d74 2175  ...ro|...r.|.t!u
+00002d80: 0090 0172 0374 0688 00a0 227c 0aa1 0183  ...r.t...."|....
+00002d90: 017c 095f 237c 096a 2390 0172 0274 097c  .|._#|.j#..r.t.|
+00002da0: 096a 2364 0e19 0083 017d 0a6e 7774 247c  .j#d.....}.nwt$|
+00002db0: 0d74 256a 266a 2783 0290 0172 1a88 006a  .t%j&j'....r...j
+00002dc0: 127c 0a64 0764 0f8d 027d 0a7c 096a 2890  .|.d.d...}.|.j(.
+00002dd0: 0173 1974 297c 095f 286e 3574 247c 0d74  .s.t)|._(n5t$|.t
+00002de0: 256a 266a 2a83 0290 0173 277c 0d74 2b75  %j&j*....s'|.t+u
+00002df0: 0090 0172 4888 006a 127c 0a64 0764 0f8d  ...rH..j.|.d.d..
+00002e00: 027d 0a7c 096a 2890 0173 477c 0d74 2b75  .}.|.j(..sG|.t+u
+00002e10: 0090 0172 3b74 2c7c 095f 286e 147c 0d74  ...r;t,|._(n.|.t
+00002e20: 2d75 0090 0172 4474 2e7c 095f 286e 0b74  -u...rDt.|._(n.t
+00002e30: 2f7c 095f 286e 0774 3090 0173 4f74 317c  /|._(n.t0..sOt1|
+00002e40: 0a83 0101 0074 247c 0a74 3283 0290 0172  .....t$|.t2....r
+00002e50: 5d64 1064 0584 007c 0a44 0083 017c 095f  ]d.d...|.D...|._
+00002e60: 2374 157c 0188 0083 0290 0172 6c74 3374  #t.|.......rlt3t
+00002e70: 347c 0a83 027c 016a 357c 096a 363c 0074  4|...|.j5|.j6<.t
+00002e80: 0b7d 0a6e 0b74 247c 0a74 3283 0290 0172  .}.n.t$|.t2....r
+00002e90: 7a74 067c 0a83 017c 095f 237c 0a7c 095f  zt.|...|._#|.|._
+00002ea0: 097c 09a0 37a1 007d 0e7c 0e64 113d 007c  .|..7..}.|.d.=.|
+00002eb0: 0ea0 3864 12a1 017d 0f7c 0f90 0173 8e67  ..8d...}.|...s.g
+00002ec0: 006e 0664 1364 0584 007c 0f44 0083 017d  .n.d.d...|.D...}
+00002ed0: 107c 0e64 1419 0090 0173 b17c 0ea0 3964  .|.d.....s.|..9d
+00002ee0: 15a1 0190 0173 b17c 1090 0173 ad64 167c  .....s.|...s.d.|
+00002ef0: 0e64 1719 00a0 3aa1 009b 0064 189d 036e  .d....:....d...n
+00002f00: 0164 197c 0e64 143c 007c 0e64 1a19 007d  .d.|.d.<.|.d...}
+00002f10: 117c 1090 0173 d27c 0e64 1a3d 007c 1190  .|...s.|.d.=.|..
+00002f20: 0173 ca7c 0ea0 3964 1ba1 0164 0075 0090  .s.|..9d...d.u..
+00002f30: 0172 ca64 1c7c 0e64 1b3c 0074 3374 347c  .r.d.|.d.<.t3t4|
+00002f40: 0a83 027c 0e64 1d3c 006e 4c7c 096a 0974  ...|.d.<.nL|.j.t
+00002f50: 3b75 0090 0172 fd74 157c 0188 0083 0290  ;u...r.t.|......
+00002f60: 0172 e774 3374 347c 0a83 027c 016a 357c  .r.t3t4|...|.j5|
+00002f70: 096a 363c 0064 1e44 005d 097d 127c 0ea0  .j6<.d.D.].}.|..
+00002f80: 387c 1264 00a1 0201 0090 0171 e97c 0e64  8|.d.......q.|.d
+00002f90: 1f19 0090 0173 fc74 3c7c 0e64 1f3c 006e  .....s.t<|.d.<.n
+00002fa0: 217c 096a 3d64 0e6b 0390 0272 0b74 3374  !|.j=d.k...r.t3t
+00002fb0: 347c 0a83 027c 0e64 1d3c 006e 137c 0a74  4|...|.d.<.n.|.t
+00002fc0: 3e75 0090 0272 1574 3f7c 0e64 1f3c 006e  >u...r.t?|.d.<.n
+00002fd0: 097c 0a74 0b75 0090 0272 1e74 407c 0e64  .|.t.u...r.t@|.d
+00002fe0: 1f3c 007c 086a 1e74 1f75 0190 0273 327c  .<.|.j.t.u...s2|
+00002ff0: 086a 2074 1f75 0190 0273 327c 0ea0 3964  .j t.u...s2|..9d
+00003000: 20a1 0164 0075 0190 0272 c97c 0ea0 3964   ..d.u...r.|..9d
+00003010: 1fa1 0190 0272 6574 247c 0e64 1f19 0074  .....ret$|.d...t
+00003020: 416a 4274 3c66 0283 0290 0272 6574 0964  AjBt<f.....ret.d
+00003030: 2164 2269 0083 0383 007d 137c 0e64 1f19  !d"i.....}.|.d..
+00003040: 007c 107c 0e64 1719 0064 238d 027c 017c  .|.|.d...d#..|.|
+00003050: 137c 0e64 2019 0064 248d 0301 0074 437c  .|.d ..d$....tC|
+00003060: 137c 0e64 1719 0083 027c 0e64 203c 006e  .|.d.....|.d <.n
+00003070: 0f64 1d7c 0e76 0090 0272 747c 0e64 1d19  .d.|.v...rt|.d..
+00003080: 007c 0e64 2019 0083 017c 0e64 203c 007c  .|.d ....|.d <.|
+00003090: 0ea0 3964 15a1 0190 0272 c97c 0e64 2019  ..9d.....r.|.d .
+000030a0: 007d 1474 0a7c 1474 0b83 0290 0273 8c74  .}.t.|.t.....s.t
+000030b0: 0a7c 1474 256a 266a 2a83 0290 0273 8f7c  .|.t%j&j*....s.|
+000030c0: 1467 017d 147c 1444 005d 377d 0b7c 0b7c  .g.}.|.D.]7}.|.|
+000030d0: 0e64 1519 0076 0190 0272 c774 0a7c 0b74  .d...v...r.t.|.t
+000030e0: 3283 0290 0272 a87c 0b6a 1c7c 0e64 1519  2....r.|.j.|.d..
+000030f0: 0076 0190 0272 c77c 0ea0 3964 1aa1 0190  .v...r.|..9d....
+00003100: 0273 b37c 0b64 0075 0090 0273 c764 257c  .s.|.d.u...s.d%|
+00003110: 0b9b 0064 267c 0e64 1719 009b 0064 277c  ...d&|.d.....d'|
+00003120: 0e64 1519 009b 009d 067d 037c 01a0 047c  .d.......}.|...|
+00003130: 03a1 0101 0090 0271 9164 287c 0c9b 009d  .......q.d(|....
+00003140: 0267 017d 157c 1190 0273 e674 157c 0ea0  .g.}.|...s.t.|..
+00003150: 3964 20a1 0174 0b83 0290 0272 e17c 15a0  9d ..t.....r.|..
+00003160: 4464 29a1 0101 006e 057c 15a0 4464 2aa1  Dd)....n.|..Dd*.
+00003170: 0101 007c 0ea0 3864 2b64 0da1 0290 0272  ...|..8d+d.....r
+00003180: f27c 15a0 4464 2ca1 0101 007c 096a 4590  .|..Dd,....|.jE.
+00003190: 0272 ff7c 15a0 4464 2d7c 096a 459b 009d  .r.|..Dd-|.jE...
+000031a0: 02a1 0101 0064 2e64 2fa0 467c 15a1 019b  .....d.d/.F|....
+000031b0: 009d 027d 167c 0ea0 3964 30a1 0190 0372  ...}.|..9d0....r
+000031c0: 187c 0e64 3005 0019 0064 317c 1617 0037  .|.d0....d1|...7
+000031d0: 0003 003c 006e 047c 167c 0e64 303c 007c  ...<.n.|.|.d0<.|
+000031e0: 0ea0 3864 3264 00a1 027d 177c 1790 0373  ..8d2d...}.|...s
+000031f0: 2c7c 1190 0372 2a64 336e 0164 347d 177c  ,|...r*d3n.d4}.|
+00003200: 04a0 397c 1764 00a1 027d 187c 1890 0373  ..9|.d...}.|...s
+00003210: 3e7c 01a0 477c 17a1 017d 187c 187c 047c  >|..G|...}.|.|.|
+00003220: 173c 007c 096a 4890 0372 697c 1190 0372  .<.|.jH..ri|...r
+00003230: 5064 357c 096a 369b 009d 027d 037c 01a0  Pd5|.j6....}.|..
+00003240: 047c 03a1 0101 007c 016a 497c 016a 4aa0  .|.....|.jI|.jJ.
+00003250: 3988 006a 4ba1 0119 007c 1719 00a0 447c  9..jK....|....D|
+00003260: 096a 367c 1090 0372 657c 1064 0c19 006e  .j6|...re|.d...n
+00003270: 0164 0066 02a1 0101 007c 186a 4c7c 1069  .d.f.....|.jL|.i
+00003280: 007c 0ea4 018e 0101 007c 07a0 447c 09a1  .|.......|..D|..
+00003290: 0101 0071 3e7c 0753 0029 364e 7a3e 5468  ...q>|.S.)6Nz>Th
+000032a0: 6973 2070 6172 7365 7220 616c 7265 6164  is parser alread
+000032b0: 7920 636f 6e74 6169 6e73 2061 7267 756d  y contains argum
+000032c0: 656e 7473 2066 726f 6d20 616e 6f74 6865  ents from anothe
+000032d0: 7220 6461 7461 636c 6173 732e 6301 0000  r dataclass.c...
+000032e0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+000032f0: 0013 0000 0073 1200 0000 8800 6a00 8801  .....s......j...
+00003300: 7c00 6a01 6401 8d02 0c00 5300 2902 4e72  |.j.d.....S.).Nr
+00003310: a300 0000 2902 72a4 0000 0072 9200 0000  ....).r....r....
+00003320: 2901 da01 66a9 02da 0363 6c73 5a05 6d6f  )...f....clsZ.mo
+00003330: 6465 6c72 5300 0000 7257 0000 0072 5e00  delrS...rW...r^.
+00003340: 0000 b201 0000 f302 0000 0012 007a 2f41  .............z/A
+00003350: 7267 756d 656e 7450 6172 7365 722e 5f61  rgumentParser._a
+00003360: 6464 5f61 7267 756d 656e 7473 2e3c 6c6f  dd_arguments.<lo
+00003370: 6361 6c73 3e2e 3c6c 616d 6264 613e 6301  cals>.<lambda>c.
+00003380: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00003390: 0000 0053 0000 0073 2000 0000 6700 7c00  ...S...s ...g.|.
+000033a0: 5d0c 7d01 7c01 7c01 6a00 a001 7402 7403  ].}.|.|.j...t.t.
+000033b0: 8300 a102 6602 9102 7102 5300 7253 0000  ....f...q.S.rS..
+000033c0: 0029 04da 086d 6574 6164 6174 61da 0367  .)...metadata..g
+000033d0: 6574 7221 0000 0072 2200 0000 7254 0000  etr!...r"...rT..
+000033e0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
+000033f0: 7258 0000 00b7 0100 0073 0800 0000 0600  rX.......s......
+00003400: 0202 12ff 06ff 7a31 4172 6775 6d65 6e74  ......z1Argument
+00003410: 5061 7273 6572 2e5f 6164 645f 6172 6775  Parser._add_argu
+00003420: 6d65 6e74 732e 3c6c 6f63 616c 733e 2e3c  ments.<locals>.<
+00003430: 6c69 7374 636f 6d70 3e72 3d00 0000 5429  listcomp>r=...T)
+00003440: 01da 0d69 735f 756e 696f 6e5f 7479 7065  ...is_union_type
+00003450: da01 2e72 1700 0000 a901 da08 6d61 7873  ...r........maxs
+00003460: 706c 6974 e9ff ffff ff46 7201 0000 0029  plit.....Fr....)
+00003470: 01da 1061 7373 6572 745f 7072 696d 6974  ...assert_primit
+00003480: 6976 6563 0100 0000 0000 0000 0000 0000  ivec............
+00003490: 0200 0000 0300 0000 5300 0000 7312 0000  ........S...s...
+000034a0: 0067 007c 005d 057d 017c 016a 0091 0271  .g.|.].}.|.j...q
+000034b0: 0253 0072 5300 0000 a901 7292 0000 0072  .S.rS.....r....r
+000034c0: 5400 0000 7253 0000 0072 5300 0000 7257  T...rS...rS...rW
+000034d0: 0000 0072 5800 0000 1302 0000 72a8 0000  ...rX.......r...
+000034e0: 00da 0370 6f73 7267 0000 0063 0100 0000  ...posrg...c....
+000034f0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00003500: 5300 0000 731a 0000 0067 007c 005d 097d  S...s....g.|.].}
+00003510: 017c 01a0 0064 00a1 0172 027c 0191 0271  .|...d...r.|...q
+00003520: 0253 0029 0172 6500 0000 725f 0000 0072  .S.).re...r_...r
+00003530: 5400 0000 7253 0000 0072 5300 0000 7257  T...rS...rS...rW
+00003540: 0000 0072 5800 0000 2d02 0000 7302 0000  ...rX...-...s...
+00003550: 001a 00da 076d 6574 6176 6172 7264 0000  .....metavarrd..
+00003560: 00fa 013c da04 6465 7374 fa01 3e7a 073c  ...<..dest..>z.<
+00003570: 7661 6c75 653e da08 7265 7175 6972 6564  value>..required
+00003580: da05 6e61 7267 73fa 013f da04 7479 7065  ..nargs..?..type
+00003590: 2905 72ba 0000 0072 b800 0000 da05 636f  ).r....r......co
+000035a0: 6e73 7472 6400 0000 72b3 0000 0072 5900  nstrd...r....rY.
+000035b0: 0000 7263 0000 00da 0072 5300 0000 2902  ..rc.....rS...).
+000035c0: 7267 0000 0072 b500 0000 2903 7266 0000  rg...r....).rf..
+000035d0: 00da 096e 616d 6573 7061 6365 da06 7661  ...namespace..va
+000035e0: 6c75 6573 7a0f 496e 7661 6c69 6420 7661  luesz.Invalid va
+000035f0: 6c75 6520 277a 1027 2066 6f72 2061 7267  lue 'z.' for arg
+00003600: 756d 656e 7420 277a 1327 3b20 6d75 7374  ument 'z.'; must
+00003610: 2062 6520 6f6e 6520 6f66 3a20 7a06 5479   be one of: z.Ty
+00003620: 7065 3a20 7a16 4465 6661 756c 743a 2022  pe: z.Default: "
+00003630: 2528 6465 6661 756c 7429 7322 7a14 4465  %(default)s"z.De
+00003640: 6661 756c 743a 2025 2864 6566 6175 6c74  fault: %(default
+00003650: 2973 da09 6578 636c 7573 6976 657a 044d  )s..exclusivez.M
+00003660: 2e58 2e7a 0545 6e76 3a20 7a02 3e20 fa02  .X.z.Env: z.> ..
+00003670: 2c20 725a 0000 0072 7d00 0000 da05 6772  , rZ...r}.....gr
+00003680: 6f75 707a 1372 6571 7569 7265 6420 7061  oupz.required pa
+00003690: 7261 6d65 7465 7273 7a13 6f70 7469 6f6e  rametersz.option
+000036a0: 616c 2070 6172 616d 6574 6572 737a 3341  al parametersz3A
+000036b0: 206d 7574 7561 6c6c 792d 6578 636c 7573   mutually-exclus
+000036c0: 6976 6520 7061 7261 6d65 7465 7220 6361  ive parameter ca
+000036d0: 6e6e 6f74 2062 6520 7265 7175 6972 6564  nnot be required
+000036e0: 3a20 294d 7234 0000 0072 2500 0000 da0b  : )Mr4...r%.....
+000036f0: 6765 745f 6465 6661 756c 7472 4600 0000  get_defaultrF...
+00003700: 7282 0000 0072 9d00 0000 725d 0000 00da  r....r....r]....
+00003710: 0666 696c 7465 7272 0600 0000 72ba 0000  .filterr....r...
+00003720: 0072 3800 0000 726e 0000 0072 2300 0000  .r8...rn...r#...
+00003730: 727f 0000 00da 0c76 6572 7369 6f6e 5f69  r......version_i
+00003740: 6e66 6f72 3f00 0000 da10 5f67 6574 5f74  nfor?....._get_t
+00003750: 7970 655f 6f72 6967 696e 7215 0000 00da  ype_originr.....
+00003760: 1c5f 6578 7472 6163 745f 7479 7065 5f66  ._extract_type_f
+00003770: 726f 6d5f 636f 6e74 6169 6e65 7272 3c00  rom_containerr<.
+00003780: 0000 da12 5f67 6574 5f74 7970 655f 6d65  ...._get_type_me
+00003790: 7461 6461 7461 726d 0000 0072 0500 0000  tadatarm...r....
+000037a0: 7221 0000 0072 a900 0000 7295 0000 00da  r!...r....r.....
+000037b0: 0672 7370 6c69 74da 0873 6574 5f64 6573  .rsplit..set_des
+000037c0: 7472 9200 0000 72b7 0000 0072 6300 0000  tr....r....rc...
+000037d0: 7204 0000 00da 0f64 6566 6175 6c74 5f66  r......default_f
+000037e0: 6163 746f 7279 722a 0000 00da 0e5f 6765  actoryr*....._ge
+000037f0: 745f 7479 7065 5f61 7267 7372 6400 0000  t_type_argsrd...
+00003800: 7239 0000 00da 0b63 6f6c 6c65 6374 696f  r9.....collectio
+00003810: 6e73 da03 6162 63da 074d 6170 7069 6e67  ns..abc..Mapping
+00003820: 7259 0000 0072 1d00 0000 da08 4974 6572  rY...r......Iter
+00003830: 6162 6c65 da03 7365 7472 1f00 0000 da05  able..setr......
+00003840: 7475 706c 6572 2000 0000 721e 0000 0072  tupler ...r....r
+00003850: 3500 0000 7227 0000 0072 0700 0000 7208  5...r'...r....r.
+00003860: 0000 0072 3100 0000 7272 0000 0072 b500  ...r1...rr...r..
+00003870: 0000 da06 6173 6469 6374 7297 0000 0072  ....asdictr....r
+00003880: aa00 0000 da05 7570 7065 72da 0462 6f6f  ......upper..boo
+00003890: 6c72 1800 0000 72b8 0000 00da 0369 6e74  lr....r......int
+000038a0: 7219 0000 0072 1a00 0000 7274 0000 00da  r....r....rt....
+000038b0: 0641 6374 696f 6eda 0767 6574 6174 7472  .Action..getattr
+000038c0: da06 6170 7065 6e64 da08 5f65 6e76 5f76  ..append.._env_v
+000038d0: 6172 da04 6a6f 696e da12 6164 645f 6172  ar..join..add_ar
+000038e0: 6775 6d65 6e74 5f67 726f 7570 72bf 0000  gument_groupr...
+000038f0: 0072 7100 0000 da09 5f64 6566 6175 6c74  .rq....._default
+00003900: 7372 4500 0000 726f 0000 0029 1972 a700  srE...ro...).r..
+00003910: 0000 7266 0000 0072 8f00 0000 da03 6572  ..rf...r......er
+00003920: 725a 1170 6172 7365 725f 6172 675f 6772  rZ.parser_arg_gr
+00003930: 6f75 7073 5a0c 6e6f 7665 6c5f 6669 656c  oupsZ.novel_fiel
+00003940: 6473 5a10 6e6f 7665 6c5f 6669 656c 645f  dsZ.novel_field_
+00003950: 6172 6773 5a0a 6164 6465 645f 6172 6773  argsZ.added_args
+00003960: 5a03 666c 645a 1161 7267 7061 7273 655f  Z.fldZ.argparse_
+00003970: 6172 6775 6d65 6e74 da08 666c 645f 7479  argument..fld_ty
+00003980: 7065 7256 0000 005a 0968 656c 705f 7479  perV...Z.help_ty
+00003990: 7065 5a0f 666c 645f 7479 7065 5f6f 7269  peZ.fld_type_ori
+000039a0: 6769 6e72 5100 0000 7267 0000 0072 5000  ginrQ...rg...rP.
+000039b0: 0000 72b7 0000 00da 016b 5a0f 6475 6d6d  ..r......kZ.dumm
+000039c0: 795f 6e61 6d65 7370 6163 65da 0164 5a0e  y_namespace..dZ.
+000039d0: 6865 6c70 5f6d 7367 5f70 6172 7473 5a08  help_msg_partsZ.
+000039e0: 6865 6c70 5f6d 7367 72c1 0000 005a 0961  help_msgr....Z.a
+000039f0: 7267 5f67 726f 7570 7253 0000 0072 a600  rg_grouprS...r..
+00003a00: 0000 7257 0000 0072 9000 0000 9901 0000  ..rW...r........
+00003a10: 739c 0100 0008 0a06 0108 020c 0204 010a  s...............
+00003a20: 0116 0204 0202 0202 010c 0106 0102 fe04  ................
+00003a30: ff06 0702 0206 fe04 050e 0206 010a 0408  ................
+00003a40: 010e 0114 030e 0104 0102 0102 0106 fe0a  ................
+00003a50: 050e 0114 010a 0104 0102 800a 0214 030e  ................
+00003a60: 0104 0102 0102 0106 fe08 0708 ff14 0202  ................
+00003a70: fd0c 0606 020a 0108 0108 010a 010a 0106  ................
+00003a80: 010a 0206 0110 0110 0108 010e 0102 8010  ................
+00003a90: 0304 0102 0102 0106 fe08 0406 0102 800c  ................
+00003aa0: 0304 ff0a 0204 0202 0102 0106 fe08 040a  ................
+00003ab0: 0108 010a 0108 0106 0202 8006 0208 010c  ................
+00003ac0: 0210 010c 0202 0302 0102 010c fe06 070c  ................
+00003ad0: 020a 0106 0208 0206 010a 0202 0308 ff0c  ................
+00003ae0: 0202 fd16 061c 0206 ff08 0406 0206 0216  ................
+00003af0: 0108 0110 010c 010c 0102 0302 0102 010c  ................
+00003b00: fe08 0510 010a 0108 0102 800c 0210 010a  ................
+00003b10: 010a 020a 0108 020c 040c 0110 010e 0206  ................
+00003b20: 0108 0106 fe0e 0512 0102 0102 0106 0106  ................
+00003b30: fd14 050a 0114 010c 0308 010e 0102 0106  ................
+00003b40: 0106 fe06 0408 020e 0208 0204 fe10 0308  ................
+00003b50: 0304 fd0a 0312 0306 0104 ff02 ff0a 0404  ................
+00003b60: 800c 0206 0312 010c 010a 020e 020a 0108  ................
+00003b70: 0212 0110 020c 0216 0108 020c 0206 020e  ................
+00003b80: 010c 0206 020a 0108 0108 0206 0102 0204  ................
+00003b90: 0104 ff02 ff0a 0404 020c 0102 ff02 0202  ................
+00003ba0: fe02 0204 0210 0102 fe04 ff10 070c 0204  ................
+00003bb0: 027a 1d41 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
+00003bc0: 722e 5f61 6464 5f61 7267 756d 656e 7473  r._add_arguments
+00003bd0: da01 7463 0100 0000 0000 0000 0000 0000  ..tc............
+00003be0: 0100 0000 0400 0000 4300 0000 730c 0000  ........C...s...
+00003bf0: 0074 007c 0064 0164 0083 0353 0029 024e  .t.|.d.d...S.).N
+00003c00: da0a 5f5f 6f72 6967 696e 5f5f a901 72d7  ..__origin__..r.
+00003c10: 0000 00a9 0172 e100 0000 7253 0000 0072  .....r....rS...r
+00003c20: 5300 0000 7257 0000 0072 c500 0000 ba02  S...rW...r......
+00003c30: 0000 f302 0000 000c 027a 1f41 7267 756d  .........z.Argum
+00003c40: 656e 7450 6172 7365 722e 5f67 6574 5f74  entParser._get_t
+00003c50: 7970 655f 6f72 6967 696e 6301 0000 0000  ype_originc.....
+00003c60: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00003c70: 0000 00f3 0c00 0000 7400 7c00 6401 6402  ........t.|.d.d.
+00003c80: 8303 5300 2903 4eda 085f 5f61 7267 735f  ..S.).N..__args_
+00003c90: 5f72 5300 0000 72e3 0000 0072 e400 0000  _rS...r....r....
+00003ca0: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
+00003cb0: cb00 0000 be02 0000 72e5 0000 007a 1d41  ........r....z.A
+00003cc0: 7267 756d 656e 7450 6172 7365 722e 5f67  rgumentParser._g
+00003cd0: 6574 5f74 7970 655f 6172 6773 6301 0000  et_type_argsc...
+00003ce0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00003cf0: 0043 0000 0072 e600 0000 2903 4eda 0c5f  .C...r....).N.._
+00003d00: 5f6d 6574 6164 6174 615f 5f72 5300 0000  _metadata__rS...
+00003d10: 72e3 0000 0072 e400 0000 7253 0000 0072  r....r....rS...r
+00003d20: 5300 0000 7257 0000 0072 c700 0000 c202  S...rW...r......
+00003d30: 0000 72e5 0000 007a 2141 7267 756d 656e  ..r....z!Argumen
+00003d40: 7450 6172 7365 722e 5f67 6574 5f74 7970  tParser._get_typ
+00003d50: 655f 6d65 7461 6461 7461 da0e 7479 7065  e_metadata..type
+00003d60: 5f63 6f6e 7461 696e 6572 72b0 0000 0072  _containerr....r
+00003d70: ab00 0000 6304 0000 0000 0000 0000 0000  ....c...........
+00003d80: 000b 0000 0003 0000 0043 0000 0073 1801  .........C...s..
+00003d90: 0000 7c03 7204 7400 6e04 7c00 a001 7c01  ..|.r.t.n.|...|.
+00003da0: a101 7d04 7c04 6400 7500 7215 7402 6401  ..}.|.d.u.r.t.d.
+00003db0: 7c01 6a03 9b00 9d02 8301 8201 7c00 a004  |.j.........|...
+00003dc0: 7c01 a101 7d05 6402 6403 8400 7c05 4400  |...}.d.d...|.D.
+00003dd0: 8301 7d06 7c04 7400 7500 7330 7405 7c04  ..}.|.t.u.s0t.|.
+00003de0: 7406 6a07 6a08 8302 7330 7c04 7409 7500  t.j.j...s0|.t.u.
+00003df0: 7240 740a 7c06 8301 6404 6b03 723b 7c06  r@t.|...d.k.r;|.
+00003e00: a00b a100 0100 6e2c 7c06 6405 1900 7d07  ......n,|.d...}.
+00003e10: 6e27 7405 7c04 7406 6a07 6a0c 8302 7261  n't.|.t.j.j...ra
+00003e20: 740a 7c06 8301 6406 6b03 7252 7c06 a00b  t.|...d.k.rR|...
+00003e30: a100 0100 6e15 7c06 5c02 7d08 7d09 7c08  ....n.|.\.}.}.|.
+00003e40: 740d 7501 725e 7402 6407 8301 8201 7c09  t.u.r^t.d.....|.
+00003e50: 7d07 6e06 740e 7367 740f 7c01 8301 0100  }.n.t.sgt.|.....
+00003e60: 7c06 736d 7402 6408 8301 8201 7c00 a001  |.smt.d.....|...
+00003e70: 7c07 a101 7d0a 7c0a 7400 7500 7280 7c00  |...}.|.t.u.r.|.
+00003e80: a010 7c07 a101 7d07 7c00 a001 7c07 a101  ..|...}.|...|...
+00003e90: 7d0a 7c02 728a 7c0a 728a 740e 738a 740f  }.|.r.|.r.t.s.t.
+00003ea0: 7c0a 8301 0100 7c07 5300 2909 4e7a 1f47  |.....|.S.).Nz.G
+00003eb0: 6976 656e 2074 7970 6520 6973 206e 6f74  iven type is not
+00003ec0: 2061 2063 6f6e 7461 696e 6572 3a20 6301   a container: c.
+00003ed0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00003ee0: 0000 0053 0000 0073 2000 0000 6700 7c00  ...S...s ...g.|.
+00003ef0: 5d0c 7d01 7c01 6400 7501 7202 7c01 7400  ].}.|.d.u.r.|.t.
+00003f00: 7501 7202 7c01 9102 7102 5300 2901 2e29  u.r.|...q.S.)..)
+00003f10: 0172 2b00 0000 2902 7255 0000 00da 0161  .r+...).rU.....a
+00003f20: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
+00003f30: 5800 0000 d802 0000 7304 0000 0006 001a  X.......s.......
+00003f40: 017a 3f41 7267 756d 656e 7450 6172 7365  .z?ArgumentParse
+00003f50: 722e 5f65 7874 7261 6374 5f74 7970 655f  r._extract_type_
+00003f60: 6672 6f6d 5f63 6f6e 7461 696e 6572 2e3c  from_container.<
+00003f70: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00003f80: 703e 7217 0000 0072 0100 0000 727c 0000  p>r....r....r|..
+00003f90: 007a 2244 6963 7469 6f6e 6172 7920 6b65  .z"Dictionary ke
+00003fa0: 7973 206d 7573 7420 6265 2074 7970 6520  ys must be type 
+00003fb0: 6073 7472 607a 1b54 6f6f 206d 616e 7920  `str`z.Too many 
+00003fc0: 7479 7065 7320 696e 2063 6f6e 7461 696e  types in contain
+00003fd0: 6572 2911 7215 0000 0072 c500 0000 da09  er).r....r......
+00003fe0: 5479 7065 4572 726f 7272 9500 0000 72cb  TypeErrorr....r.
+00003ff0: 0000 0072 3900 0000 72cc 0000 0072 cd00  ...r9...r....r..
+00004000: 0000 7211 0000 0072 d000 0000 7276 0000  ..r....r....rv..
+00004010: 00da 0563 6c65 6172 72ce 0000 0072 6e00  ...clearr....rn.
+00004020: 0000 7235 0000 0072 2700 0000 72c6 0000  ..r5...r'...r...
+00004030: 0029 0b72 a700 0000 72e9 0000 0072 b000  .).r....r....r..
+00004040: 0000 72ab 0000 005a 1574 7970 655f 636f  ..r....Z.type_co
+00004050: 6e74 6169 6e65 725f 6f72 6967 696e 5a13  ntainer_originZ.
+00004060: 7479 7065 5f63 6f6e 7461 696e 6572 5f61  type_container_a
+00004070: 7267 73da 0772 6573 756c 7473 5a16 7479  rgs..resultsZ.ty
+00004080: 7065 5f63 6f6e 7461 696e 6572 5f73 7562  pe_container_sub
+00004090: 7479 7065 5a08 6b65 795f 7479 7065 5a0a  typeZ.key_typeZ.
+000040a0: 7661 6c75 655f 7479 7065 5a1d 7479 7065  value_typeZ.type
+000040b0: 5f63 6f6e 7461 696e 6572 5f73 7562 7479  _container_subty
+000040c0: 7065 5f6f 7269 6769 6e72 5300 0000 7253  pe_originrS...rS
+000040d0: 0000 0072 5700 0000 72c6 0000 00c6 0200  ...rW...r.......
+000040e0: 0073 5400 0000 1008 02ff 0804 0201 0a01  .sT.............
+000040f0: 04ff 0a04 0602 0201 06ff 0807 0c01 02ff  ................
+00004100: 0802 0c02 0a01 0a02 0e01 0c01 0a01 0802  ................
+00004110: 0801 0801 0601 0401 0801 0402 0801 0a02  ................
+00004120: 0802 0401 0201 04ff 0a03 0203 02ff 0202  ................
+00004130: 02fe 0203 02fd 0805 0402 7a2b 4172 6775  ..........z+Argu
+00004140: 6d65 6e74 5061 7273 6572 2e5f 6578 7472  mentParser._extr
+00004150: 6163 745f 7479 7065 5f66 726f 6d5f 636f  act_type_from_co
+00004160: 6e74 6169 6e65 7263 0100 0000 0000 0000  ntainerc........
+00004170: 0000 0000 0200 0000 0600 0000 0b00 0000  ................
+00004180: 7364 0000 007c 01a0 0064 0164 02a1 027c  sd...|...d.d...|
+00004190: 0164 013c 007c 01a0 0064 0364 04a1 027c  .d.<.|...d.d...|
+000041a0: 0164 033c 007c 01a0 0064 0588 006a 01a1  .d.<.|...d...j..
+000041b0: 027c 0164 053c 007c 01a0 0064 0687 0066  .|.d.<.|...d...f
+000041c0: 0164 0764 0884 08a1 027c 0164 063c 0074  .d.d.....|.d.<.t
+000041d0: 0283 006a 0364 0969 007c 01a4 018e 0188  ...j.d.i.|......
+000041e0: 005f 0488 006a 0453 0029 0a4e 726c 0000  ._...j.S.).Nrl..
+000041f0: 005a 0863 6f6d 6d61 6e64 7372 b300 0000  .Z.commandsr....
+00004200: 7a09 3c43 4f4d 4d41 4e44 3e72 b500 0000  z.<COMMAND>r....
+00004210: da0c 7061 7273 6572 5f63 6c61 7373 6300  ..parser_classc.
+00004220: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+00004230: 0000 001b 0000 0073 1e00 0000 7400 8800  .......s....t...
+00004240: 8301 6403 6900 7c00 a401 6401 8800 6a01  ..d.i.|...d...j.
+00004250: 6402 9c02 a401 8e01 5300 2904 4e54 2902  d.......S.).NT).
+00004260: 724f 0000 0072 4e00 0000 7253 0000 0029  rO...rN...rS...)
+00004270: 0272 ba00 0000 724e 0000 0029 0172 df00  .r....rN...).r..
+00004280: 0000 a901 7278 0000 0072 5300 0000 7257  ....rx...rS...rW
+00004290: 0000 0072 5e00 0000 0c03 0000 730c 0000  ...r^.......s...
+000042a0: 000a 0002 0102 ff02 0204 010a fd7a 2f41  .............z/A
+000042b0: 7267 756d 656e 7450 6172 7365 722e 6164  rgumentParser.ad
+000042c0: 645f 7375 6270 6172 7365 7273 2e3c 6c6f  d_subparsers.<lo
+000042d0: 6361 6c73 3e2e 3c6c 616d 6264 613e 7253  cals>.<lambda>rS
+000042e0: 0000 0029 0572 aa00 0000 7244 0000 0072  ...).r....rD...r
+000042f0: 6800 0000 da0e 6164 645f 7375 6270 6172  h.....add_subpar
+00004300: 7365 7273 726a 0000 0029 0272 7800 0000  sersrj...).rx...
+00004310: 7251 0000 0072 7900 0000 72ef 0000 0072  rQ...ry...r....r
+00004320: 5700 0000 72f0 0000 0006 0300 0073 1200  W...r........s..
+00004330: 0000 1001 1001 1201 0401 0201 0a01 08fe  ................
+00004340: 1409 0602 7a1d 4172 6775 6d65 6e74 5061  ....z.ArgumentPa
+00004350: 7273 6572 2e61 6464 5f73 7562 7061 7273  rser.add_subpars
+00004360: 6572 7363 0100 0000 0000 0000 0000 0000  ersc............
+00004370: 0200 0000 0400 0000 4300 0000 732c 0000  ........C...s,..
+00004380: 007c 006a 0044 005d 107d 0174 017c 0174  .|.j.D.].}.t.|.t
+00004390: 026a 0383 0272 137c 017c 005f 047c 006a  .j...r.|.|._.|.j
+000043a0: 0402 0001 0053 0071 0364 0053 0072 5c00  .....S.q.d.S.r\.
+000043b0: 0000 2905 da08 5f61 6374 696f 6e73 726d  ..)..._actionsrm
+000043c0: 0000 0072 7400 0000 7296 0000 0072 6a00  ...rt...r....rj.
+000043d0: 0000 2902 7278 0000 0072 ea00 0000 7253  ..).rx...r....rS
+000043e0: 0000 0072 5300 0000 7257 0000 0072 8c00  ...rS...rW...r..
+000043f0: 0000 1703 0000 7312 0000 000a 0102 0102  ......s.........
+00004400: 0104 0104 fe06 040a 0102 fb04 067a 2641  .............z&A
+00004410: 7267 756d 656e 7450 6172 7365 722e 5f66  rgumentParser._f
+00004420: 696e 645f 7375 6270 6172 7365 7273 5f61  ind_subparsers_a
+00004430: 6374 696f 6e63 0100 0000 0000 0000 0000  ctionc..........
+00004440: 0000 0100 0000 0200 0000 4300 0000 7336  ..........C...s6
+00004450: 0000 007c 006a 0064 0075 0172 087c 006a  ...|.j.d.u.r.|.j
+00004460: 0053 007c 006a 0172 177c 00a0 02a1 0001  .S.|.j.r.|......
+00004470: 007c 006a 0073 144a 0082 017c 006a 0053  .|.j.s.J...|.j.S
+00004480: 007c 00a0 03a1 0053 0072 5c00 0000 2904  .|.....S.r\...).
+00004490: 726a 0000 0072 8b00 0000 728c 0000 0072  rj...r....r....r
+000044a0: f000 0000 72ef 0000 0072 5300 0000 7253  ....r....rS...rS
+000044b0: 0000 0072 5700 0000 7277 0000 0021 0300  ...rW...rw...!..
+000044c0: 0073 0e00 0000 0a01 0601 0602 0801 0a01  .s..............
+000044d0: 0601 0802 7a25 4172 6775 6d65 6e74 5061  ....z%ArgumentPa
+000044e0: 7273 6572 2e5f 6765 745f 6f72 5f61 6464  rser._get_or_add
+000044f0: 5f73 7562 7061 7273 6572 7372 bd00 0000  _subparsersr....
+00004500: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
+00004510: 0006 0000 0003 0000 0073 6e00 0000 7c00  .........sn...|.
+00004520: 6a00 a001 7402 8800 7c00 6a03 6400 8303  j...t...|.j.d...
+00004530: 6900 a102 7d02 7c02 a004 a100 4400 5d1d  i...}.|.....D.].
+00004540: 7d03 8700 6601 6401 6402 8408 7c03 4400  }...f.d.d...|.D.
+00004550: 8301 7d04 7405 7c04 8301 6403 6b04 722d  ..}.t.|...d.k.r-
+00004560: 6404 6405 a006 7c04 a101 1700 7d05 7c00  d.d...|.....}.|.
+00004570: a007 7c05 a101 0100 7110 7408 6406 6900  ..|.....q.t.d.i.
+00004580: 7409 8800 8301 a401 8e01 5300 2907 4e63  t.........S.).Nc
+00004590: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000045a0: 0500 0000 1300 0000 736c 0000 0067 007c  ........sl...g.|
+000045b0: 005d 325c 027d 017d 0274 0088 007c 0183  .]2\.}.}.t...|..
+000045c0: 0272 3474 0188 007c 0183 027d 0374 027c  .r4t...|...}.t.|
+000045d0: 0374 0383 0273 1c74 027c 0374 046a 056a  .t...s.t.|.t.j.j
+000045e0: 0683 0273 207c 0364 0075 0173 2e74 027c  ...s |.d.u.s.t.|
+000045f0: 0374 0383 0273 0274 027c 0374 046a 056a  .t...s.t.|.t.j.j
+00004600: 0683 0272 027c 0372 027c 0272 327c 026e  ...r.|.r.|.r2|.n
+00004610: 017c 0191 0271 0253 0072 5c00 0000 2907  .|...q.S.r\...).
+00004620: da07 6861 7361 7474 7272 d700 0000 7238  ..hasattrr....r8
+00004630: 0000 0072 6e00 0000 72cc 0000 0072 cd00  ...rn...r....r..
+00004640: 0000 72cf 0000 0029 0472 5500 0000 72b5  ..r....).rU...r.
+00004650: 0000 00da 0466 6c61 675a 0a61 7474 725f  .....flagZ.attr_
+00004660: 7661 6c75 65a9 0172 bd00 0000 7253 0000  value..r....rS..
+00004670: 0072 5700 0000 7258 0000 003b 0300 0073  .rW...rX...;...s
+00004680: 3000 0000 0600 0602 0801 02fd 0a04 0803  0...............
+00004690: 02f9 0208 0201 0601 02fe 02f8 080d 0803  ................
+000046a0: 02fd 0204 0201 0601 02fe 02fc 0208 02f8  ................
+000046b0: 0af4 060c 7a33 4172 6775 6d65 6e74 5061  ....z3ArgumentPa
+000046c0: 7273 6572 2e5f 706f 7374 5f70 6172 7365  rser._post_parse
+000046d0: 5f61 7267 732e 3c6c 6f63 616c 733e 2e3c  _args.<locals>.<
+000046e0: 6c69 7374 636f 6d70 3e72 1700 0000 7a28  listcomp>r....z(
+000046f0: 5468 6573 6520 6172 6775 6d65 6e74 7320  These arguments 
+00004700: 6172 6520 6d75 7475 616c 6c79 2065 7863  are mutually exc
+00004710: 6c75 7369 7665 3a20 72c0 0000 0072 5300  lusive: r....rS.
+00004720: 0000 290a 7271 0000 0072 aa00 0000 72d7  ..).rq...r....r.
+00004730: 0000 0072 4500 0000 72be 0000 0072 7600  ...rE...r....rv.
+00004740: 0000 72da 0000 0072 8200 0000 7228 0000  ..r....r....r(..
+00004750: 00da 0476 6172 7329 0672 7800 0000 72bd  ...vars).rx...r.
+00004760: 0000 005a 1266 756e 635f 6d78 5f61 7267  ...Z.func_mx_arg
+00004770: 5f67 726f 7570 735a 0667 5f61 7267 735a  _groupsZ.g_argsZ
+00004780: 0e6d 785f 666c 6167 735f 666f 756e 6472  .mx_flags_foundr
+00004790: dd00 0000 7253 0000 0072 f400 0000 7257  ....rS...r....rW
+000047a0: 0000 00da 105f 706f 7374 5f70 6172 7365  ....._post_parse
+000047b0: 5f61 7267 732c 0300 0073 2000 0000 0607  _args,...s .....
+000047c0: 0c01 0201 02fe 02fd 0c07 0a04 0202 06fe  ................
+000047d0: 0c19 0601 0201 06ff 0a03 0280 1202 7a1f  ..............z.
+000047e0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+000047f0: 706f 7374 5f70 6172 7365 5f61 7267 7363  post_parse_argsc
+00004800: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00004810: 0a00 0000 0300 0000 7352 0000 007a 0e74  ........sR...z.t
+00004820: 0083 006a 017c 017c 0264 018d 027d 037c  ...j.|.|.d...}.|
+00004830: 00a0 027c 03a1 0157 0053 0004 0074 0379  ...|...W.S...t.y
+00004840: 2801 007d 0401 007a 0e7c 00a0 0474 057c  (..}...z.|...t.|
+00004850: 0483 01a1 0101 0057 0059 0064 007d 047e  .......W.Y.d.}.~
+00004860: 0464 0053 0064 007d 047e 0477 0177 00a9  .d.S.d.}.~.w.w..
+00004870: 024e 2902 7250 0000 0072 bd00 0000 2906  .N).rP...r....).
+00004880: 7268 0000 00da 0a70 6172 7365 5f61 7267  rh.....parse_arg
+00004890: 7372 f600 0000 da0a 5661 6c75 6545 7272  sr......ValueErr
+000048a0: 6f72 7282 0000 0072 6e00 0000 2905 7278  orr....rn...).rx
+000048b0: 0000 0072 5000 0000 72bd 0000 00da 0670  ...rP...r......p
+000048c0: 6172 7365 64da 0165 7279 0000 0072 5300  arsed..ery...rS.
+000048d0: 0000 7257 0000 0072 f800 0000 5c03 0000  ..rW...r....\...
+000048e0: 7314 0000 0002 0506 0102 0102 0106 fe0c  s...............
+000048f0: 040e 011c 0108 8002 ff7a 1941 7267 756d  .........z.Argum
+00004900: 656e 7450 6172 7365 722e 7061 7273 655f  entParser.parse_
+00004910: 6172 6773 6303 0000 0000 0000 0000 0000  argsc...........
+00004920: 0006 0000 000a 0000 0003 0000 0073 5a00  .............sZ.
+00004930: 0000 7a12 7400 8300 6a01 7c01 7c02 6401  ..z.t...j.|.|.d.
+00004940: 8d02 5c02 7d03 7d04 7c00 a002 7c03 a101  ..\.}.}.|...|...
+00004950: 7c04 6602 5700 5300 0400 7403 792c 0100  |.f.W.S...t.y,..
+00004960: 7d05 0100 7a0e 7c00 a004 7405 7c05 8301  }...z.|...t.|...
+00004970: a101 0100 5700 5900 6400 7d05 7e05 6400  ....W.Y.d.}.~.d.
+00004980: 5300 6400 7d05 7e05 7701 7700 72f7 0000  S.d.}.~.w.w.r...
+00004990: 0029 0672 6800 0000 da10 7061 7273 655f  .).rh.....parse_
+000049a0: 6b6e 6f77 6e5f 6172 6773 72f6 0000 0072  known_argsr....r
+000049b0: f900 0000 7282 0000 0072 6e00 0000 2906  ....r....rn...).
+000049c0: 7278 0000 0072 5000 0000 72bd 0000 0072  rx...rP...r....r
+000049d0: fa00 0000 da07 756e 6b6e 6f77 6e72 fb00  ......unknownr..
+000049e0: 0000 7279 0000 0072 5300 0000 7257 0000  ..ry...rS...rW..
+000049f0: 0072 fc00 0000 6a03 0000 730e 0000 0002  .r....j...s.....
+00004a00: 0714 0110 010e 011c 0108 8002 ff7a 1f41  .............z.A
+00004a10: 7267 756d 656e 7450 6172 7365 722e 7061  rgumentParser.pa
+00004a20: 7273 655f 6b6e 6f77 6e5f 6172 6773 da18  rse_known_args..
+00004a30: 736b 6970 5f70 7964 616e 7469 635f 7661  skip_pydantic_va
+00004a40: 6c69 6461 7469 6f6e 6304 0000 0000 0000  lidationc.......
+00004a50: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
+00004a60: 0073 2200 0000 7c00 a000 7c01 a101 5c02  .s"...|...|...\.
+00004a70: 7d04 7d05 7c00 6a01 7c04 7c02 7c03 6401  }.}.|.j.|.|.|.d.
+00004a80: 8d03 7c05 6602 5300 2902 61c9 0200 0055  ..|.f.S.).a....U
+00004a90: 7365 2070 6172 7365 6420 6172 6773 2074  se parsed args t
+00004aa0: 6f20 696e 7374 616e 7469 6174 6520 7468  o instantiate th
+00004ab0: 6520 6769 7665 6e20 6461 7461 206d 6f64  e given data mod
+00004ac0: 656c 2e0a 0a20 2020 2020 2020 2041 7267  el...        Arg
+00004ad0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+00004ae0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00004af0: 2061 7267 735f 6d6f 6465 6c3a 0a20 2020   args_model:.   
+00004b00: 2020 2020 2020 2020 2073 6b69 705f 7079           skip_py
+00004b10: 6461 6e74 6963 5f76 616c 6964 6174 696f  dantic_validatio
+00004b20: 6e3a 0a0a 2020 2020 2020 2020 4578 616d  n:..        Exam
+00004b30: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
+00004b40: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
+00004b50: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
+00004b60: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
+00004b70: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00004b80: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+00004b90: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00004ba0: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
+00004bb0: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
+00004bc0: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
+00004bd0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00004be0: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
+00004bf0: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
+00004c00: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00004c10: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00004c20: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
+00004c30: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
+00004c40: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
+00004c50: 3e3e 2070 6172 7365 722e 6164 645f 6172  >> parser.add_ar
+00004c60: 6775 6d65 6e74 7328 4164 644e 756d 7329  guments(AddNums)
+00004c70: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00004c80: 2070 6172 7365 642c 2075 6e6b 6e6f 776e   parsed, unknown
+00004c90: 203d 2070 6172 7365 722e 7061 7273 655f   = parser.parse_
+00004ca0: 6b6e 6f77 6e5f 6172 6773 5f74 6f5f 6d6f  known_args_to_mo
+00004cb0: 6465 6c28 5b27 2d78 272c 2027 3127 2c20  del(['-x', '1', 
+00004cc0: 272d 7927 2c20 2732 272c 2027 2d7a 272c  '-y', '2', '-z',
+00004cd0: 2027 3327 5d29 0a20 2020 2020 2020 2020   '3']).         
+00004ce0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00004cf0: 2020 203e 3e3e 2028 7061 7273 6564 2e78     >>> (parsed.x
+00004d00: 2c20 7061 7273 6564 2e79 290a 2020 2020  , parsed.y).    
+00004d10: 2020 2020 2020 2020 2831 2c20 3229 0a20          (1, 2). 
+00004d20: 2020 2020 2020 2020 2020 203e 3e3e 2075             >>> u
+00004d30: 6e6b 6e6f 776e 0a20 2020 2020 2020 2020  nknown.         
+00004d40: 2020 205b 272d 7a27 2c20 2733 275d 0a0a     ['-z', '3']..
+00004d50: 2020 2020 2020 2020 a903 7250 0000 0072          ..rP...r
+00004d60: 8f00 0000 72fe 0000 0029 0272 fc00 0000  ....r....).r....
+00004d70: da14 5f70 6172 7365 5f61 7267 735f 746f  .._parse_args_to
+00004d80: 5f6d 6f64 656c 2906 7278 0000 0072 5000  _model).rx...rP.
+00004d90: 0000 728f 0000 0072 fe00 0000 da0b 7061  ..r....r......pa
+00004da0: 7273 6564 5f61 7267 73da 0c75 6e6b 6e6f  rsed_args..unkno
+00004db0: 776e 5f61 7267 7372 5300 0000 7253 0000  wn_argsrS...rS..
+00004dc0: 0072 5700 0000 da19 7061 7273 655f 6b6e  .rW.....parse_kn
+00004dd0: 6f77 6e5f 6172 6773 5f74 6f5f 6d6f 6465  own_args_to_mode
+00004de0: 6c77 0300 0073 1000 0000 0e23 0403 0201  lw...s.....#....
+00004df0: 0201 0201 04fd 0205 04fa 7a28 4172 6775  ..........z(Argu
+00004e00: 6d65 6e74 5061 7273 6572 2e70 6172 7365  mentParser.parse
+00004e10: 5f6b 6e6f 776e 5f61 7267 735f 746f 5f6d  _known_args_to_m
+00004e20: 6f64 656c 6304 0000 0000 0000 0000 0000  odelc...........
+00004e30: 0005 0000 0005 0000 0043 0000 0073 1a00  .........C...s..
+00004e40: 0000 7c00 a000 7c01 a101 7d04 7c00 6a01  ..|...|...}.|.j.
+00004e50: 7c04 7c02 7c03 6401 8d03 5300 2902 617f  |.|.|.d...S.).a.
+00004e60: 0200 0055 7365 2070 6172 7365 6420 6172  ...Use parsed ar
+00004e70: 6773 2074 6f20 696e 7374 616e 7469 6174  gs to instantiat
+00004e80: 6520 7468 6520 6769 7665 6e20 6461 7461  e the given data
+00004e90: 206d 6f64 656c 2e0a 0a20 2020 2020 2020   model...       
+00004ea0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00004eb0: 2020 2061 7267 733a 0a20 2020 2020 2020     args:.       
+00004ec0: 2020 2020 2061 7267 735f 6d6f 6465 6c3a       args_model:
+00004ed0: 0a20 2020 2020 2020 2020 2020 2073 6b69  .            ski
+00004ee0: 705f 7079 6461 6e74 6963 5f76 616c 6964  p_pydantic_valid
+00004ef0: 6174 696f 6e3a 0a0a 2020 2020 2020 2020  ation:..        
+00004f00: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+00004f10: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
+00004f20: 2079 6170 780a 2020 2020 2020 2020 2020   yapx.          
+00004f30: 2020 3e3e 3e20 6672 6f6d 2064 6174 6163    >>> from datac
+00004f40: 6c61 7373 6573 2069 6d70 6f72 7420 6461  lasses import da
+00004f50: 7461 636c 6173 730a 2020 2020 2020 2020  taclass.        
+00004f60: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00004f70: 2020 2020 3e3e 3e20 4064 6174 6163 6c61      >>> @datacla
+00004f80: 7373 0a20 2020 2020 2020 2020 2020 202e  ss.            .
+00004f90: 2e2e 2063 6c61 7373 2041 6464 4e75 6d73  .. class AddNums
+00004fa0: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
+00004fb0: 2e20 2020 2020 783a 2069 6e74 0a20 2020  .     x: int.   
+00004fc0: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
+00004fd0: 2079 3a20 696e 740a 2020 2020 2020 2020   y: int.        
+00004fe0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00004ff0: 2020 2020 3e3e 3e20 7061 7273 6572 203d      >>> parser =
+00005000: 2079 6170 782e 4172 6775 6d65 6e74 5061   yapx.ArgumentPa
+00005010: 7273 6572 2829 0a20 2020 2020 2020 2020  rser().         
+00005020: 2020 203e 3e3e 2070 6172 7365 722e 6164     >>> parser.ad
+00005030: 645f 6172 6775 6d65 6e74 7328 4164 644e  d_arguments(AddN
+00005040: 756d 7329 0a20 2020 2020 2020 2020 2020  ums).           
+00005050: 203e 3e3e 2070 6172 7365 6420 3d20 7061   >>> parsed = pa
+00005060: 7273 6572 2e70 6172 7365 5f61 7267 735f  rser.parse_args_
+00005070: 746f 5f6d 6f64 656c 285b 272d 7827 2c20  to_model(['-x', 
+00005080: 2731 272c 2027 2d79 272c 2027 3227 5d29  '1', '-y', '2'])
+00005090: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+000050a0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+000050b0: 2028 7061 7273 6564 2e78 2c20 7061 7273   (parsed.x, pars
+000050c0: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
+000050d0: 2020 2831 2c20 3229 0a0a 2020 2020 2020    (1, 2)..      
+000050e0: 2020 72ff 0000 0029 0272 f800 0000 7200    r....).r....r.
+000050f0: 0100 0029 0572 7800 0000 7250 0000 0072  ...).rx...rP...r
+00005100: 8f00 0000 72fe 0000 0072 0101 0000 7253  ....r....r....rS
+00005110: 0000 0072 5300 0000 7257 0000 00da 1370  ...rS...rW.....p
+00005120: 6172 7365 5f61 7267 735f 746f 5f6d 6f64  arse_args_to_mod
+00005130: 656c a503 0000 730c 0000 000a 1e04 0102  el....s.........
+00005140: 0102 0102 0106 fd7a 2241 7267 756d 656e  .......z"Argumen
+00005150: 7450 6172 7365 722e 7061 7273 655f 6172  tParser.parse_ar
+00005160: 6773 5f74 6f5f 6d6f 6465 6c63 0400 0000  gs_to_modelc....
+00005170: 0000 0000 0000 0000 0800 0000 0a00 0000  ................
+00005180: 4300 0000 73aa 0000 0074 007c 0183 017d  C...s....t.|...}
+00005190: 047c 0273 107c 04a0 017c 006a 02a1 017d  .|.s.|...|.j...}
+000051a0: 027c 0273 1074 0382 017c 006a 047c 047c  .|.s.t...|.j.|.|
+000051b0: 0264 018d 027d 0574 0572 4e7c 0373 4e7a  .d...}.t.rN|.sNz
+000051c0: 0d74 0074 067c 0283 0164 0569 007c 05a4  .t.t.|...d.i.|..
+000051d0: 018e 0183 017d 0557 006e 2504 0074 0779  .....}.W.n%..t.y
+000051e0: 4d01 007d 0601 007a 1964 0264 02a0 0864  M..}...z.d.d...d
+000051f0: 0364 0484 007c 06a0 09a1 0044 0083 01a1  .d...|.....D....
+00005200: 0117 007d 077c 00a0 0a7c 07a1 0101 0057  ...}.|...|.....W
+00005210: 0059 0064 007d 067e 066e 0564 007d 067e  .Y.d.}.~.n.d.}.~
+00005220: 0677 0177 007c 0264 0569 007c 05a4 018e  .w.w.|.d.i.|....
+00005230: 0153 0029 064e a902 da09 6172 6773 5f64  .S.).N....args_d
+00005240: 6963 7472 8f00 0000 727d 0000 0063 0100  ictr....r}...c..
+00005250: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00005260: 0000 7300 0000 732e 0000 0081 007c 005d  ..s...s......|.]
+00005270: 127d 0164 007c 0164 0119 0064 0219 009b  .}.d.|.d...d....
+00005280: 0064 037c 0164 0419 009b 0064 059d 0556  .d.|.d.....d...V
+00005290: 0001 0071 0264 0653 0029 077a 1845 7272  ...q.d.S.).z.Err
+000052a0: 6f72 2070 6172 7369 6e67 2061 7267 756d  or parsing argum
+000052b0: 656e 7420 60da 036c 6f63 7201 0000 007a  ent `..locr....z
+000052c0: 0360 3b20 da03 6d73 6772 ac00 0000 4e72  .`; ..msgr....Nr
+000052d0: 5300 0000 7254 0000 0072 5300 0000 7253  S...rT...rS...rS
+000052e0: 0000 0072 5700 0000 da09 3c67 656e 6578  ...rW.....<genex
+000052f0: 7072 3ee3 0300 0073 0a00 0000 0280 0400  pr>....s........
+00005300: 0202 1cff 0aff 7a36 4172 6775 6d65 6e74  ......z6Argument
+00005310: 5061 7273 6572 2e5f 7061 7273 655f 6172  Parser._parse_ar
+00005320: 6773 5f74 6f5f 6d6f 6465 6c2e 3c6c 6f63  gs_to_model.<loc
+00005330: 616c 733e 2e3c 6765 6e65 7870 723e 7253  als>.<genexpr>rS
+00005340: 0000 0029 0b72 f500 0000 72aa 0000 0072  ...).r....r....r
+00005350: 4600 0000 7226 0000 00da 165f 756e 696f  F...r&....._unio
+00005360: 6e5f 6172 6773 5f77 6974 685f 6d6f 6465  n_args_with_mode
+00005370: 6c72 3500 0000 7233 0000 0072 2e00 0000  lr5...r3...r....
+00005380: 72da 0000 00da 0665 7272 6f72 7372 8200  r......errorsr..
+00005390: 0000 2908 7278 0000 0072 5000 0000 728f  ..).rx...rP...r.
+000053a0: 0000 0072 fe00 0000 7201 0100 005a 0a61  ...r....r....Z.a
+000053b0: 7267 735f 756e 696f 6e72 fb00 0000 72dd  rgs_unionr....r.
+000053c0: 0000 0072 5300 0000 7253 0000 0072 5700  ...rS...rS...rW.
+000053d0: 0000 7200 0100 00ca 0300 0073 2c00 0000  ..r........s,...
+000053e0: 0806 0402 0c01 0401 0401 0402 0201 0201  ................
+000053f0: 06fe 0805 0202 0201 1001 08ff 0e03 0c01  ................
+00005400: 0602 0afe 1604 0880 02fb 0e07 7a23 4172  ............z#Ar
+00005410: 6775 6d65 6e74 5061 7273 6572 2e5f 7061  gumentParser._pa
+00005420: 7273 655f 6172 6773 5f74 6f5f 6d6f 6465  rse_args_to_mode
+00005430: 6c72 0601 0000 6302 0000 0000 0000 0000  lr....c.........
+00005440: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
+00005450: 1600 0000 8700 6601 6401 6402 8408 7c00  ......f.d.d...|.
+00005460: a000 a100 4400 8301 5300 2903 4e63 0100  ....D...S.).Nc..
+00005470: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00005480: 0000 1300 0000 7320 0000 0069 007c 005d  ......s ...i.|.]
+00005490: 0c5c 027d 017d 027c 0188 006a 0076 0072  .\.}.}.|...j.v.r
+000054a0: 027c 017c 0293 0271 0253 0072 5300 0000  .|.|...q.S.rS...
+000054b0: 72a1 0000 00a9 0372 5500 0000 72df 0000  r......rU...r...
+000054c0: 00da 0176 7294 0000 0072 5300 0000 7257  ...vr....rS...rW
+000054d0: 0000 00da 0a3c 6469 6374 636f 6d70 3ef0  .....<dictcomp>.
+000054e0: 0300 0072 6100 0000 7a39 4172 6775 6d65  ...ra...z9Argume
+000054f0: 6e74 5061 7273 6572 2e5f 756e 696f 6e5f  ntParser._union_
+00005500: 6172 6773 5f77 6974 685f 6d6f 6465 6c2e  args_with_model.
+00005510: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+00005520: 6d70 3e29 0172 8d00 0000 7205 0100 0072  mp>).r....r....r
+00005530: 5300 0000 7294 0000 0072 5700 0000 720a  S...r....rW...r.
+00005540: 0100 00eb 0300 0073 0200 0000 1605 7a25  .......s......z%
+00005550: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00005560: 756e 696f 6e5f 6172 6773 5f77 6974 685f  union_args_with_
+00005570: 6d6f 6465 6c63 0200 0000 0000 0000 0000  modelc..........
+00005580: 0000 0600 0000 0400 0000 4300 0000 7380  ..........C...s.
+00005590: 0000 0064 007d 027c 016a 0072 157c 016a  ...d.}.|.j.r.|.j
+000055a0: 00a0 017c 016a 0264 0117 00a1 0173 157c  ...|.j.d.....s.|
+000055b0: 016a 00a0 03a1 00a0 04a1 007d 027c 0273  .j.........}.|.s
+000055c0: 1964 0053 0064 027d 0374 057c 0283 0144  .d.S.d.}.t.|...D
+000055d0: 005d 0c5c 027d 047d 057c 05a0 03a1 0073  .].\.}.}.|.....s
+000055e0: 2b7c 047d 0301 006e 0171 1f7c 0364 026b  +|.}...n.q.|.d.k
+000055f0: 0472 367c 0264 007c 0385 0219 007d 0264  .r6|.d.|.....}.d
+00005600: 03a0 0664 0464 0584 007c 0244 0083 01a1  ...d.d...|.D....
+00005610: 0153 0029 064e fa01 2872 0100 0000 727d  .S.).N..(r....r}
+00005620: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00005630: 0200 0000 0300 0000 7300 0000 7318 0000  ........s...s...
+00005640: 0081 007c 005d 077d 017c 01a0 00a1 0056  ...|.].}.|.....V
+00005650: 0001 0071 0264 0053 0072 5c00 0000 2901  ...q.d.S.r\...).
+00005660: da05 7374 7269 7072 5400 0000 7253 0000  ..striprT...rS..
+00005670: 0072 5300 0000 7257 0000 0072 0901 0000  .rS...rW...r....
+00005680: 0a04 0000 7304 0000 0002 8016 007a 4141  ....s........zAA
+00005690: 7267 756d 656e 7450 6172 7365 722e 5f67  rgumentParser._g
+000056a0: 6574 5f64 6573 6372 6970 7469 6f6e 5f66  et_description_f
+000056b0: 726f 6d5f 646f 6373 7472 696e 672e 3c6c  rom_docstring.<l
+000056c0: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+000056d0: 2907 da07 5f5f 646f 635f 5f72 6000 0000  )...__doc__r`...
+000056e0: 7295 0000 0072 1001 0000 7299 0000 00da  r....r....r.....
+000056f0: 0965 6e75 6d65 7261 7465 72da 0000 0029  .enumerater....)
+00005700: 0672 a700 0000 728f 0000 005a 1164 6573  .r....r....Z.des
+00005710: 6372 6970 7469 6f6e 5f6c 696e 6573 5a12  cription_linesZ.
+00005720: 7465 7874 5f62 6c6f 636b 5f65 6e64 735f  text_block_ends_
+00005730: 6174 da01 69da 046c 696e 6572 5300 0000  at..i..linerS...
+00005740: 7253 0000 0072 5700 0000 7298 0000 00f2  rS...rW...r.....
+00005750: 0300 0073 2000 0000 0405 0c02 0801 04ff  ...s ...........
+00005760: 0e03 0402 0401 0402 1001 0801 0401 0401  ................
+00005770: 02fe 0804 0c01 1402 7a2e 4172 6775 6d65  ........z.Argume
+00005780: 6e74 5061 7273 6572 2e5f 6765 745f 6465  ntParser._get_de
+00005790: 7363 7269 7074 696f 6e5f 6672 6f6d 5f64  scription_from_d
+000057a0: 6f63 7374 7269 6e67 6303 0000 0000 0000  ocstringc.......
+000057b0: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
+000057c0: 0073 1c00 0000 7c00 a000 7c02 a101 7d03  .s....|...|...}.
+000057d0: 7c03 720c 7c03 7c01 5f01 6400 5300 6400  |.r.|.|._.d.S.d.
+000057e0: 5300 725c 0000 0029 0272 9800 0000 7249  S.r\...).r....rI
+000057f0: 0000 0029 0472 a700 0000 7266 0000 0072  ...).r....rf...r
+00005800: 8f00 0000 7249 0000 0072 5300 0000 7253  ....rI...rS...rS
+00005810: 0000 0072 5700 0000 da1f 5f73 6574 5f64  ...rW....._set_d
+00005820: 6573 6372 6970 7469 6f6e 5f66 726f 6d5f  escription_from_
+00005830: 646f 6373 7472 696e 670c 0400 0073 0800  docstring....s..
+00005840: 0000 0a06 0402 0a01 04ff 7a2e 4172 6775  ..........z.Argu
+00005850: 6d65 6e74 5061 7273 6572 2e5f 7365 745f  mentParser._set_
+00005860: 6465 7363 7269 7074 696f 6e5f 6672 6f6d  description_from
+00005870: 5f64 6f63 7374 7269 6e67 da0b 6c69 6e6b  _docstring..link
+00005880: 6564 5f66 756e 63da 0b72 656c 6179 5f76  ed_func..relay_v
+00005890: 616c 7565 6307 0000 0000 0000 0000 0000  aluec...........
+000058a0: 0017 0000 0007 0000 0003 0000 0073 e601  .............s..
+000058b0: 0000 6700 7d07 6900 7d08 6401 7d09 6401  ..g.}.i.}.d.}.d.
+000058c0: 7d0a 6401 7d0b 6401 7d0c 6401 7d0d 7400  }.d.}.d.}.d.}.t.
+000058d0: 7c02 8301 6a01 a002 a100 4400 5d43 7d0e  |...j.....D.]C}.
+000058e0: 7403 7c0e 8301 a004 6402 a101 7221 6403  t.|.....d...r!d.
+000058f0: 7d0c 7115 7403 7c0e 8301 a004 6404 a101  }.q.t.|.....d...
+00005900: 722b 6403 7d0a 7115 7c0e 6a05 6405 6b02  r+d.}.q.|.j.d.k.
+00005910: 7233 6403 7d0b 7115 7c0e 6a05 6406 6b02  r3d.}.q.|.j.d.k.
+00005920: 723b 6403 7d0d 7115 7c0e 6a05 6407 6b02  r;d.}.q.|.j.d.k.
+00005930: 7245 7c03 7c08 6407 3c00 7115 7c0e 6a05  rE|.|.d.<.q.|.j.
+00005940: 6408 6b02 724f 7c06 7c08 6408 3c00 7115  d.k.rO|.|.d.<.q.
+00005950: 7c0e 6a05 6409 6b02 7258 6403 7c08 6409  |.j.d.k.rXd.|.d.
+00005960: 3c00 7115 7c0a 7060 7c0c 7060 7c0b 7060  <.q.|.p`|.p`|.p`
+00005970: 7c0d 7d09 7c09 7373 7c05 7273 7406 640a  |.}.|.ss|.rst.d.
+00005980: 640b 8400 7400 7c05 8301 6a01 a002 a100  d...t.|...j.....
+00005990: 4400 8301 8301 7d09 7c04 7379 7407 7c02  D.....}.|.syt.|.
+000059a0: 8301 7d04 7c09 72e1 7c01 6a08 7c03 7c04  ..}.|.r.|.j.|.|.
+000059b0: 640c 8d02 5c02 7d0f 7d10 7c0c 7388 7c0d  d...\.}.}.|.s.|.
+000059c0: 72d6 6900 8900 7c00 8300 7d11 7c10 4400  r.i...|...}.|.D.
+000059d0: 5d24 7d12 7c12 a004 640d a101 72b3 7c12  ]$}.|...d...r.|.
+000059e0: 6a09 640e 640f 6410 8d02 6411 1900 7d13  j.d.d.d...d...}.
+000059f0: 7c13 a00a 640d a101 7d14 7c14 72b3 7c11  |...d...}.|.r.|.
+00005a00: 6a0b 7c13 6412 6400 6401 6413 8d04 0100  j.|.d.d.d.d.....
+00005a10: 7c13 8800 7c14 3c00 718f 7c11 6a0c 7c10  |...|.<.q.|.j.|.
+00005a20: 6414 8d01 5c02 7d15 7d10 8700 6601 6415  d...\.}.}...f.d.
+00005a30: 6416 8408 740d 7c15 8301 a00e a100 4400  d...t.|.......D.
+00005a40: 8301 7d16 7c0c 72d0 7c08 a00f 7c16 a101  ..}.|.r.|...|...
+00005a50: 0100 7c0d 72d6 7c16 7c08 6406 3c00 7c0a  ..|.r.|.|.d.<.|.
+00005a60: 72da 7c10 7d07 7c0b 72e0 7c10 7c08 6405  r.|.}.|.r.|.|.d.
+00005a70: 3c00 6e07 7c01 6a10 7c03 7c04 640c 8d02  <.n.|.j.|.|.d...
+00005a80: 7d0f 7c02 7c07 6900 740d 7c0f 8301 a401  }.|.|.i.t.|.....
+00005a90: 7c08 a401 8e01 5300 2917 4e46 7a02 2a2a  |.....S.).NFz.**
+00005aa0: 54da 012a da0b 5f65 7874 7261 5f61 7267  T..*.._extra_arg
+00005ab0: 73da 0d5f 6578 7472 615f 6b77 6172 6773  s.._extra_kwargs
+00005ac0: 5a09 5f61 6c6c 5f61 7267 735a 0c5f 7265  Z._all_argsZ._re
+00005ad0: 6c61 795f 7661 6c75 655a 105f 6361 6c6c  lay_valueZ._call
+00005ae0: 6564 5f66 726f 6d5f 636c 6963 0100 0000  ed_from_clic....
+00005af0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00005b00: 7300 0000 7328 0000 0081 007c 005d 0f7d  s...s(.....|.].}
+00005b10: 0174 007c 0183 01a0 0164 00a1 0170 0f7c  .t.|.....d...p.|
+00005b20: 016a 0264 0176 0056 0001 0071 0264 0253  .j.d.v.V...q.d.S
+00005b30: 0029 0372 1801 0000 2902 7219 0100 0072  .).r....).r....r
+00005b40: 1a01 0000 4e29 0372 6e00 0000 7260 0000  ....N).rn...r`..
+00005b50: 0072 9200 0000 2902 7255 0000 00da 0170  .r....).rU.....p
+00005b60: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
+00005b70: 0901 0000 4104 0000 730a 0000 0002 8004  ....A...s.......
+00005b80: 0002 0216 ff0a ff7a 2b41 7267 756d 656e  .......z+Argumen
+00005b90: 7450 6172 7365 722e 5f72 756e 5f66 756e  tParser._run_fun
+00005ba0: 632e 3c6c 6f63 616c 733e 2e3c 6765 6e65  c.<locals>.<gene
+00005bb0: 7870 723e 2902 7250 0000 0072 8f00 0000  xpr>).rP...r....
+00005bc0: 7265 0000 0072 5b00 0000 7217 0000 0072  re...r[...r....r
+00005bd0: ad00 0000 7201 0000 0072 b900 0000 2903  ....r....r....).
+00005be0: 72b8 0000 0072 6300 0000 72b7 0000 0029  r....rc...r....)
+00005bf0: 0172 5000 0000 6301 0000 0000 0000 0000  .rP...c.........
+00005c00: 0000 0003 0000 0004 0000 0013 0000 0073  ...............s
+00005c10: 1a00 0000 6900 7c00 5d09 5c02 7d01 7d02  ....i.|.].\.}.}.
+00005c20: 8800 7c01 1900 7c02 9302 7102 5300 7253  ..|...|...q.S.rS
+00005c30: 0000 0072 5300 0000 720c 0100 00a9 015a  ...rS...r......Z
+00005c40: 1075 6e6b 6e6f 776e 5f6e 616d 655f 6d61  .unknown_name_ma
+00005c50: 7072 5300 0000 7257 0000 0072 0e01 0000  prS...rW...r....
+00005c60: 6504 0000 7306 0000 0006 000e 0106 ff7a  e...s..........z
+00005c70: 2c41 7267 756d 656e 7450 6172 7365 722e  ,ArgumentParser.
+00005c80: 5f72 756e 5f66 756e 632e 3c6c 6f63 616c  _run_func.<local
+00005c90: 733e 2e3c 6469 6374 636f 6d70 3e29 1172  s>.<dictcomp>).r
+00005ca0: 0900 0000 da0a 7061 7261 6d65 7465 7273  ......parameters
+00005cb0: 72be 0000 0072 6e00 0000 7260 0000 0072  r....rn...r`...r
+00005cc0: 9200 0000 da03 616e 7972 2500 0000 7203  ......anyr%...r.
+00005cd0: 0100 00da 0573 706c 6974 da06 6c73 7472  .....split..lstr
+00005ce0: 6970 726f 0000 0072 fc00 0000 72f5 0000  ipro...r....r...
+00005cf0: 0072 8d00 0000 da06 7570 6461 7465 7204  .r......updater.
+00005d00: 0100 0029 1772 a700 0000 7266 0000 0072  ...).r....rf...r
+00005d10: 9c00 0000 7250 0000 0072 8f00 0000 7216  ....rP...r....r.
+00005d20: 0100 0072 1701 0000 5a09 6675 6e63 5f61  ...r....Z.func_a
+00005d30: 7267 735a 0b66 756e 635f 6b77 6172 6773  rgsZ.func_kwargs
+00005d40: 5a0d 6578 7472 615f 6172 6773 5f6f 6b5a  Z.extra_args_okZ
+00005d50: 0c61 6363 6570 7473 5f61 7267 735a 1261  .accepts_argsZ.a
+00005d60: 6363 6570 7473 5f65 7874 7261 5f61 7267  ccepts_extra_arg
+00005d70: 735a 0e61 6363 6570 7473 5f6b 7761 7267  sZ.accepts_kwarg
+00005d80: 735a 1461 6363 6570 7473 5f65 7874 7261  sZ.accepts_extra
+00005d90: 5f6b 7761 7267 7372 1b01 0000 5a0a 6d6f  _kwargsr....Z.mo
+00005da0: 6465 6c5f 696e 7374 7202 0100 005a 0e75  del_instr....Z.u
+00005db0: 6e6b 6e6f 776e 5f70 6172 7365 7272 5600  nknown_parserrV.
+00005dc0: 0000 5a06 785f 666c 6167 5a0b 785f 666c  ..Z.x_flagZ.x_fl
+00005dd0: 6167 5f62 6172 655a 0e70 6172 7365 645f  ag_bareZ.parsed_
+00005de0: 756e 6b6e 6f77 6e5a 0c65 7874 7261 5f6b  unknownZ.extra_k
+00005df0: 7761 7267 7372 5300 0000 721c 0100 0072  wargsrS...r....r
+00005e00: 5700 0000 da09 5f72 756e 5f66 756e 6317  W....._run_func.
+00005e10: 0400 0073 9000 0000 040a 0401 0402 0402  ...s............
+00005e20: 0401 0402 0401 1202 0e01 0601 0e01 0601  ................
+00005e30: 0a01 0601 0a01 0601 0a01 0a01 0a01 0a01  ................
+00005e40: 0a01 0801 0280 0e03 02ff 0804 0801 0c02  ................
+00005e50: 08fe 0405 0801 0403 0402 0201 0201 0afe  ................
+00005e60: 0805 0401 0601 0801 0a01 1201 0a01 0401  ................
+00005e70: 0401 0201 0201 0201 0201 06fc 0806 0280  ................
+00005e80: 0402 0201 0aff 0a04 0a01 06ff 0403 0a01  ................
+00005e90: 0401 0801 0402 0401 0402 0801 0280 0403  ................
+00005ea0: 0201 0201 06fe 1605 7a18 4172 6775 6d65  ........z.Argume
+00005eb0: 6e74 5061 7273 6572 2e5f 7275 6e5f 6675  ntParser._run_fu
+00005ec0: 6e63 da07 636f 6d6d 616e 64da 0b73 7562  nc..command..sub
+00005ed0: 636f 6d6d 616e 6473 da11 6e61 6d65 645f  commands..named_
+00005ee0: 7375 6263 6f6d 6d61 6e64 7363 0400 0000  subcommandsc....
+00005ef0: 0000 0000 0000 0000 0900 0000 0b00 0000  ................
+00005f00: 4b00 0000 73d2 0000 007c 0064 0369 007c  K...s....|.d.i.|
+00005f10: 04a4 018e 017d 057c 0172 2e74 007c 0183  .....}.|.r.t.|..
+00005f20: 017d 067c 006a 017c 057c 0664 018d 0201  .}.|.j.|.|.d....
+00005f30: 007c 05a0 027c 06a1 0101 007c 056a 0364  .|...|.....|.j.d
+00005f40: 0369 007c 006a 047c 017c 006a 057c 067c  .i.|.j.|.|.j.|.|
+00005f50: 006a 067c 017c 006a 077c 0669 04a4 018e  .j.|.|.j.|.i....
+00005f60: 0101 006e 147c 056a 0364 0369 007c 006a  ...n.|.j.d.i.|.j
+00005f70: 0564 007c 006a 0464 007c 006a 0764 007c  .d.|.j.d.|.j.d.|
+00005f80: 006a 0664 0069 04a4 018e 0101 007c 0272  .j.d.i.......|.r
+00005f90: 5574 087c 0283 0172 4b7c 0267 017d 027c  Ut.|...rK|.g.}.|
+00005fa0: 0244 005d 077d 077c 05a0 097c 07a1 0101  .D.].}.|...|....
+00005fb0: 0071 4d7c 0372 677c 03a0 0aa1 0044 005d  .qM|.rg|.....D.]
+00005fc0: 0b5c 027d 087d 077c 056a 097c 077c 0864  .\.}.}.|.j.|.|.d
+00005fd0: 028d 0201 0071 5b7c 0553 0029 044e 2902  .....q[|.S.).N).
+00005fe0: 7266 0000 0072 8f00 0000 72b1 0000 0072  rf...r....r....r
+00005ff0: 5300 0000 290b 7225 0000 0072 1501 0000  S...).r%...r....
+00006000: 7291 0000 0072 9d00 0000 7242 0000 0072  r....r....rB...r
+00006010: 4300 0000 7245 0000 0072 4600 0000 da08  C...rE...rF.....
+00006020: 6361 6c6c 6162 6c65 729e 0000 0072 8d00  callabler....r..
+00006030: 0000 2909 72a7 0000 0072 2301 0000 7224  ..).r....r#...r$
+00006040: 0100 0072 2501 0000 7251 0000 0072 6600  ...r%...rQ...rf.
+00006050: 0000 5a0e 726f 6f74 5f61 7267 5f6d 6f64  ..Z.root_arg_mod
+00006060: 656c 7256 0000 0072 9200 0000 7253 0000  elrV...r....rS..
+00006070: 0072 5300 0000 7257 0000 00da 0d5f 6275  .rS...rW....._bu
+00006080: 696c 645f 7061 7273 6572 7b04 0000 733e  ild_parser{...s>
+00006090: 0000 000e 0804 0208 0104 0102 0102 0106  ................
+000060a0: fe0a 0408 0106 0206 0106 0106 0102 fc08  ................
+000060b0: ff08 0906 0206 0106 0106 0102 fc06 ff04  ................
+000060c0: 0908 0106 0108 010c 0104 0210 0110 0104  ................
+000060d0: 027a 1c41 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
+000060e0: 722e 5f62 7569 6c64 5f70 6172 7365 7229  r._build_parser)
+000060f0: 0272 5000 0000 da0c 6465 6661 756c 745f  .rP.....default_
+00006100: 6172 6773 da0b 7061 7273 6572 5f61 7267  args..parser_arg
+00006110: 7372 2801 0000 da0d 7061 7273 6572 5f6b  sr(.....parser_k
+00006120: 7761 7267 7363 0100 0000 0000 0000 0200  wargsc..........
+00006130: 0000 1100 0000 0900 0000 4f00 0000 7338  ..........O...s8
+00006140: 0100 007c 006a 007c 0369 007c 04a4 018e  ...|.j.|.i.|....
+00006150: 017d 057c 0164 0175 0072 1374 016a 0264  .}.|.d.u.r.t.j.d
+00006160: 0264 0185 0219 007d 017c 0173 197c 0272  .d.....}.|.s.|.r
+00006170: 197c 027d 017c 05a0 037c 01a1 015c 027d  .|.}.|...|...\.}
+00006180: 067d 0774 047c 0683 017d 087c 08a0 057c  .}.t.|...}.|...|
+00006190: 006a 06a1 017d 097c 08a0 057c 006a 07a1  .j...}.|...|.j..
+000061a0: 017d 0a7c 08a0 057c 006a 08a1 017d 0b7c  .}.|...|.j...}.|
+000061b0: 08a0 057c 006a 09a1 017d 0c7c 08a0 057c  ...|.j...}.|...|
+000061c0: 006a 0aa1 017d 0d64 017d 0e64 017d 0f7c  .j...}.d.}.d.}.|
+000061d0: 0972 527c 006a 0b7c 057c 097c 0a7c 0c7c  .rR|.j.|.|.|.|.|
+000061e0: 0164 038d 057d 0f74 0c7c 0f74 0d83 0272  .d...}.t.|.t...r
+000061f0: 697a 0674 0e7c 0f83 017d 0e57 006e 0d04  iz.t.|...}.W.n..
+00006200: 0074 0f79 6801 0001 0001 007c 0f7d 0e59  .t.yh......|.}.Y
+00006210: 006e 0377 007c 0f7d 0e7a 207c 0b72 7b7c  .n.w.|.}.z |.r{|
+00006220: 0c72 7b7c 006a 0b7c 057c 0c7c 0d7c 017c  .r{|.j.|.|.|.|.|
+00006230: 097c 0e64 048d 067d 0e57 0074 0c7c 0f74  .|.d...}.W.t.|.t
+00006240: 0d83 0272 8a7c 0f44 005d 067d 107c 0c73  ...r.|.D.].}.|.s
+00006250: 897c 107d 0e71 837c 0e53 0074 0c7c 0f74  .|.}.q.|.S.t.|.t
+00006260: 0d83 0272 9a7c 0f44 005d 077d 107c 0c73  ...r.|.D.].}.|.s
+00006270: 997c 107d 0e71 9377 0077 0029 0561 2d03  .|.}.q.w.w.).a-.
+00006280: 0000 5573 6520 6769 7665 6e20 6675 6e63  ..Use given func
+00006290: 7469 6f6e 7320 746f 2063 6f6e 7374 7275  tions to constru
+000062a0: 6374 2061 2043 4c49 2c20 7061 7273 6520  ct a CLI, parse 
+000062b0: 7468 6520 6172 6773 2c20 616e 6420 696e  the args, and in
+000062c0: 766f 6b65 2074 6865 2061 7070 726f 7072  voke the appropr
+000062d0: 6961 7465 2063 6f6d 6d61 6e64 2e0a 0a20  iate command... 
+000062e0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000062f0: 2020 2020 2020 2020 202a 7061 7273 6572           *parser
+00006300: 5f61 7267 733a 0a20 2020 2020 2020 2020  _args:.         
+00006310: 2020 2061 7267 733a 0a20 2020 2020 2020     args:.       
+00006320: 2020 2020 2064 6566 6175 6c74 5f61 7267       default_arg
+00006330: 733a 0a20 2020 2020 2020 2020 2020 202a  s:.            *
+00006340: 2a70 6172 7365 725f 6b77 6172 6773 3a0a  *parser_kwargs:.
+00006350: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+00006360: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00006370: 3e3e 3e20 696d 706f 7274 2079 6170 780a  >>> import yapx.
+00006380: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+00006390: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+000063a0: 6465 6620 7072 696e 745f 6e75 6d73 282a  def print_nums(*
+000063b0: 6172 6773 293a 0a20 2020 2020 2020 2020  args):.         
+000063c0: 2020 202e 2e2e 2020 2020 2070 7269 6e74     ...     print
+000063d0: 2827 4172 6773 3a20 272c 202a 6172 6773  ('Args: ', *args
+000063e0: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
+000063f0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+00006400: 3e20 6465 6620 6669 6e64 5f65 7665 6e73  > def find_evens
+00006410: 282a 6172 6773 293a 0a20 2020 2020 2020  (*args):.       
+00006420: 2020 2020 202e 2e2e 2020 2020 2072 6574       ...     ret
+00006430: 7572 6e20 5b78 2066 6f72 2078 2069 6e20  urn [x for x in 
+00006440: 6172 6773 2069 6620 696e 7428 7829 2025  args if int(x) %
+00006450: 2032 203d 3d20 305d 0a20 2020 2020 2020   2 == 0].       
+00006460: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00006470: 2020 2020 203e 3e3e 2064 6566 2066 696e       >>> def fin
+00006480: 645f 6f64 6473 282a 6172 6773 293a 0a20  d_odds(*args):. 
+00006490: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+000064a0: 2020 2072 6574 7572 6e20 5b78 2066 6f72     return [x for
+000064b0: 2078 2069 6e20 6172 6773 2069 6620 696e   x in args if in
+000064c0: 7428 7829 2025 2032 2021 3d20 305d 0a20  t(x) % 2 != 0]. 
+000064d0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
+000064e0: 2020 2020 2020 2020 2020 203e 3e3e 2063             >>> c
+000064f0: 6c69 5f61 7267 7320 3d20 5b27 6669 6e64  li_args = ['find
+00006500: 2d6f 6464 7327 2c20 2731 272c 2027 3227  -odds', '1', '2'
+00006510: 2c20 2733 272c 2027 3427 2c20 2735 275d  , '3', '4', '5']
+00006520: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00006530: 2079 6170 782e 7275 6e28 7072 696e 745f   yapx.run(print_
+00006540: 6e75 6d73 2c20 5b66 696e 645f 6576 656e  nums, [find_even
+00006550: 732c 2066 696e 645f 6f64 6473 5d2c 2061  s, find_odds], a
+00006560: 7267 733d 636c 695f 6172 6773 290a 2020  rgs=cli_args).  
+00006570: 2020 2020 2020 2020 2020 4172 6773 3a20            Args: 
+00006580: 2031 2032 2033 2034 2035 0a20 2020 2020   1 2 3 4 5.     
+00006590: 2020 2020 2020 205b 2731 272c 2027 3327         ['1', '3'
+000065a0: 2c20 2735 275d 0a20 2020 2020 2020 204e  , '5'].        N
+000065b0: 7217 0000 0029 0572 6600 0000 729c 0000  r....).rf...r...
+000065c0: 0072 8f00 0000 7216 0100 0072 5000 0000  .r....r....rP...
+000065d0: 2906 7266 0000 0072 9c00 0000 728f 0000  ).rf...r....r...
+000065e0: 0072 5000 0000 7216 0100 0072 1701 0000  .rP...r....r....
+000065f0: 2910 7227 0100 0072 7f00 0000 da04 6172  ).r'...r......ar
+00006600: 6776 72fc 0000 0072 f500 0000 72aa 0000  gvr....r....r...
+00006610: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
+00006620: 7245 0000 0072 4600 0000 7222 0100 0072  rE...rF...r"...r
+00006630: 3800 0000 720a 0000 00da 046e 6578 74da  8...r......next.
+00006640: 0d53 746f 7049 7465 7261 7469 6f6e 2911  .StopIteration).
+00006650: 72a7 0000 0072 5000 0000 7228 0100 0072  r....rP...r(...r
+00006660: 2901 0000 722a 0100 0072 6600 0000 5a0a  )...r*...rf...Z.
+00006670: 6b6e 6f77 6e5f 6172 6773 7286 0000 0072  known_argsr....r
+00006680: 0101 0000 5a09 726f 6f74 5f66 756e 635a  ....Z.root_funcZ
+00006690: 1472 6f6f 745f 6675 6e63 5f61 7267 735f  .root_func_args_
+000066a0: 6d6f 6465 6c5a 0c63 6f6d 6d61 6e64 5f6e  modelZ.command_n
+000066b0: 616d 655a 0c63 6f6d 6d61 6e64 5f66 756e  ameZ.command_fun
+000066c0: 635a 1763 6f6d 6d61 6e64 5f66 756e 635f  cZ.command_func_
+000066d0: 6172 6773 5f6d 6f64 656c 7217 0100 005a  args_modelr....Z
+000066e0: 0b72 6f6f 745f 7265 7375 6c74 5a0a 6765  .root_resultZ.ge
+000066f0: 6e5f 7265 7375 6c74 7253 0000 0072 5300  n_resultrS...rS.
+00006700: 0000 7257 0000 00da 045f 7275 6eaa 0400  ..rW....._run...
+00006710: 0073 7a00 0000 1023 0802 0e01 0802 0401  .sz....#........
+00006720: 0e03 0801 0402 0401 04ff 0403 0401 04ff  ................
+00006730: 0c03 0401 0401 04ff 0403 0401 04ff 0404  ................
+00006740: 0401 0402 0401 0201 0201 0201 0201 0201  ................
+00006750: 06fb 0a08 0201 0c01 0c01 0801 02ff 0403  ................
+00006760: 0202 0801 0401 0201 0201 0201 0201 0201  ................
+00006770: 0201 06fa 0280 0a09 0801 0401 0401 0280  ................
+00006780: 0402 0afb 0801 0401 0401 0280 02fd 0201  ................
+00006790: 7a13 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
+000067a0: 2e5f 7275 6e29 024e 4672 5c00 0000 2902  ._run).NFr\...).
+000067b0: 4646 2902 4e4e 2903 4e4e 4629 034e 4e4e  FF).NN).NNF).NNN
+000067c0: 293a 7295 0000 00da 0a5f 5f6d 6f64 756c  ):r......__modul
+000067d0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000067e0: 5f72 4200 0000 726e 0000 0072 a200 0000  _rB...rn...r....
+000067f0: 7243 0000 0072 4400 0000 7245 0000 0072  rC...rD...rE...r
+00006800: 4600 0000 722d 0000 0072 0c00 0000 7210  F...r-...r....r.
+00006810: 0000 0072 0f00 0000 7213 0000 0072 d400  ...r....r....r..
+00006820: 0000 7269 0000 0072 8200 0000 720b 0000  ..ri...r....r...
+00006830: 0072 8a00 0000 7215 0000 0072 0d00 0000  .r....r....r....
+00006840: 7229 0000 0072 9100 0000 7274 0000 0072  r)...r....rt...r
+00006850: 4100 0000 729b 0000 0072 9e00 0000 da0c  A...r....r......
+00006860: 7374 6174 6963 6d65 7468 6f64 72a4 0000  staticmethodr...
+00006870: 00da 0b63 6c61 7373 6d65 7468 6f64 7222  ...classmethodr"
+00006880: 0000 0072 9000 0000 72c5 0000 0072 1200  ...r....r....r..
+00006890: 0000 72cb 0000 0072 c700 0000 72c6 0000  ..r....r....r...
+000068a0: 0072 9600 0000 72f0 0000 0072 8c00 0000  .r....r....r....
+000068b0: 7277 0000 0072 2800 0000 72f6 0000 0072  rw...r(...r....r
+000068c0: 1100 0000 72f8 0000 0072 fc00 0000 7203  ....r....r....r.
+000068d0: 0100 0072 0401 0000 7200 0100 0072 0e00  ...r....r....r..
+000068e0: 0000 720a 0100 0072 9800 0000 7215 0100  ..r....r....r...
+000068f0: 0072 2201 0000 7227 0100 0072 2e01 0000  .r"...r'...r....
+00006900: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00006910: 5300 0000 7253 0000 0072 7900 0000 7257  S...rS...ry...rW
+00006920: 0000 0072 4100 0000 4c00 0000 73d4 0100  ...rA...L...s...
+00006930: 000a 000c 010c 010c 010c 010c 0102 0502  ................
+00006940: 0102 0102 0102 0102 0102 0102 0102 0106  ................
+00006950: f502 0202 fe06 0302 fd06 0402 fc06 0502  ................
+00006960: fb0a 0602 fa0a 0702 f90a 0802 f80a 0902  ................
+00006970: f706 0a02 f602 0b02 f502 0c0e f40e 7102  ..............q.
+00006980: 0602 0104 fd0a 0202 fe02 0302 fd02 040e  ................
+00006990: fc02 2e16 0202 fe02 030a fd02 3404 fd16  ............4...
+000069a0: 0202 fe06 0302 fd02 0402 fc04 050a fb02  ................
+000069b0: 6304 fd0a 0202 fe06 0302 fd02 0402 fc02  c...............
+000069c0: 050a fb02 0e1c 0102 0302 0104 0202 fe16  ................
+000069d0: 0302 fd06 040c fc00 7f00 7f02 2220 0102  ............" ..
+000069e0: 0324 0102 0324 0102 0302 0402 0104 fc06  .$...$..........
+000069f0: 0202 fe02 0302 fd02 0402 fc06 050c fb14  ................
+00006a00: 3f14 1110 0a02 0b04 0202 fe02 030a fd02  ?...............
+00006a10: 3202 0104 fd0a 0202 fe08 0302 fd02 040e  2...............
+00006a20: fc02 1002 0104 fd0a 0202 fe08 0302 fd0e  ................
+00006a30: 040e fc02 0f02 0102 0104 fc0a 0202 fe0a  ................
+00006a40: 0302 fd02 0402 fc0e 050a fb02 3002 0102  ............0...
+00006a50: 0104 fc0a 0202 fe0a 0302 fd02 0402 fc02  ................
+00006a60: 050a fb02 2802 0104 fc04 0202 fe0a 0302  ....(...........
+00006a70: fd02 0402 fc02 050a fb02 2102 010a 0102  ..........!.....
+00006a80: ff06 0202 fe0a 030c fd02 0602 0116 0202  ................
+00006a90: fe06 030c fd02 1902 0104 0202 fe16 0302  ................
+00006aa0: fd02 040c fc02 0a02 0602 0102 0104 f902  ................
+00006ab0: 0202 fe0a 0302 fd06 0402 fc0a 0502 fb0e  ................
+00006ac0: 0602 fa06 0702 f902 080c f802 6302 0302  ............c...
+00006ad0: 0102 0104 fc0e 0202 fe12 0302 fd16 0402  ................
+00006ae0: fc02 0502 fb02 060c fa02 2e02 0402 0106  ................
+00006af0: fc02 0202 fe0a 0302 fd0a 0402 fc02 0502  ................
+00006b00: fb02 0614 fa72 4100 0000 294e 7274 0000  .....rA...)Nrt..
+00006b10: 00da 0f63 6f6c 6c65 6374 696f 6e73 2e61  ...collections.a
+00006b20: 6263 72cc 0000 0072 7f00 0000 7202 0000  bcr....r....r...
+00006b30: 00da 0a63 6f6e 7465 7874 6c69 6272 0300  ...contextlibr..
+00006b40: 0000 da0b 6461 7461 636c 6173 7365 7372  ....dataclassesr
+00006b50: 0400 0000 7205 0000 0072 0600 0000 da04  ....r....r......
+00006b60: 656e 756d 7207 0000 00da 0966 756e 6374  enumr......funct
+00006b70: 6f6f 6c73 7208 0000 00da 0769 6e73 7065  oolsr......inspe
+00006b80: 6374 7209 0000 00da 0574 7970 6573 720a  ctr......typesr.
+00006b90: 0000 00da 0674 7970 696e 6772 0b00 0000  .....typingr....
+00006ba0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00006bb0: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
+00006bc0: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+00006bd0: 0000 5a0d 706b 675f 7265 736f 7572 6365  ..Z.pkg_resource
+00006be0: 7372 1600 0000 da07 6163 7469 6f6e 7372  sr......actionsr
+00006bf0: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
+00006c00: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00006c10: 0000 721f 0000 0072 2000 0000 da03 6172  ..r....r .....ar
+00006c20: 6772 2100 0000 7222 0000 0072 2300 0000  gr!...r"...r#...
+00006c30: 7224 0000 0072 2500 0000 da0a 6578 6365  r$...r%.....exce
+00006c40: 7074 696f 6e73 7226 0000 0072 2700 0000  ptionsr&...r'...
+00006c50: 72bd 0000 0072 2800 0000 7229 0000 0072  r....r(...r)...r
+00006c60: 2a00 0000 722b 0000 00da 0575 7469 6c73  *...r+.....utils
+00006c70: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
+00006c80: 2f00 0000 7230 0000 0072 3100 0000 7232  /...r0...r1...r2
+00006c90: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
+00006ca0: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
+00006cb0: 0072 3900 0000 72c4 0000 0072 3c00 0000  .r9...r....r<...
+00006cc0: 5a11 7479 7069 6e67 5f65 7874 656e 7369  Z.typing_extensi
+00006cd0: 6f6e 7372 3f00 0000 7240 0000 0072 4100  onsr?...r@...rA.
+00006ce0: 0000 7253 0000 0072 5300 0000 7253 0000  ..rS...rS...rS..
+00006cf0: 0072 5700 0000 da08 3c6d 6f64 756c 653e  .rW.....<module>
+00006d00: 0100 0000 7332 0000 0008 0008 0108 010c  ....s2..........
+00006d10: 010c 0114 010c 010c 010c 010c 0134 010c  .............4..
+00006d20: 0e2c 021c 0b10 070c 0114 0140 010a 110e  .,.........@....
+00006d30: 010c 020a 020c 0108 0216 03              ...........
```

### Comparing `yapx-0.2.1/src/yapx/__pycache__/exceptions.cpython-310.pyc` & `yapx-0.2.2/src/yapx/__pycache__/exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 25 04:01:15 2023 UTC, .py size: 633 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b49 bf64 7902 0000  o........I.dy...
+00000000: 6f0d 0d0a 0000 0000 9448 c364 7902 0000  o........H.dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 4700  m.Z.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6506 8303 5a07 4700  d.d...d.e...Z.G.
 00000060: 6405 6406 8400 6406 6501 8303 5a08 0907  d.d...d.e...Z...
 00000070: 640c 6408 6505 6503 1900 6409 6504 6506  d.d.e.e...d.e.e.
```

### Comparing `yapx-0.2.1/src/yapx/__pycache__/types.cpython-310.pyc` & `yapx-0.2.2/src/yapx/__pycache__/types.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 25 04:01:15 2023 UTC, .py size: 1300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b49 bf64 1405 0000  o........I.d....
+00000000: 6f0d 0d0a 0000 0000 9448 c364 1405 0000  o........H.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6500 6a0a 6404 6b05 7226 6400 6405  ..e.j.d.k.r&d.d.
 00000070: 6c03 6d0b 5a0b 0100 6e06 6400 6405 6c0c  l.m.Z...n.d.d.l.
```

### Comparing `yapx-0.2.1/src/yapx/__pycache__/utils.cpython-310.pyc` & `yapx-0.2.2/src/yapx/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 25 04:01:15 2023 UTC, .py size: 4211 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0b49 bf64 7310 0000  o........I.ds...
+00000000: 6f0d 0d0a 0000 0000 9448 c364 7310 0000  o........H.ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 2803 0000 5500  .....@...s(...U.
 00000030: 6400 6401 6c00 5a00 6400 6402 6c01 6d02  d.d.l.Z.d.d.l.m.
 00000040: 5a02 0100 6400 6403 6c03 6d04 5a04 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c05 6d06 5a06 0100 6400 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 6400 6406 6c09 6d0a  l.m.Z...d.d.l.m.
 00000070: 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  Z.m.Z.m.Z.m.Z.m.
```

### Comparing `yapx-0.2.1/src/yapx/actions.py` & `yapx-0.2.2/src/yapx/actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/src/yapx/arg.py` & `yapx-0.2.2/src/yapx/arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/src/yapx/argument_parser.py` & `yapx-0.2.2/src/yapx/argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -767,40 +767,51 @@
             and type_container_subtype_origin
             and not is_pydantic_available
         ):
             raise_unsupported_type_error(type_container_subtype_origin)
 
         return type_container_subtype
 
+    def add_subparsers(self, **kwargs) -> argparse._SubParsersAction:
+        kwargs["title"] = kwargs.get("title", "commands")
+        kwargs["metavar"] = kwargs.get("metavar", "<COMMAND>")
+        kwargs["dest"] = kwargs.get("dest", self.CMD_ATTR_NAME)
+        kwargs["parser_class"] = kwargs.get(
+            "parser_class",
+            lambda **k: type(self)(
+                **k,
+                _is_subparser=True,
+                formatter_class=self.formatter_class,
+            ),
+        )
+
+        self._subparsers_action = super().add_subparsers(**kwargs)
+
+        return self._subparsers_action
+
     def _find_subparsers_action(self) -> Optional[argparse._SubParsersAction]:
         for a in self._actions:
             if isinstance(
                 a,
                 argparse._SubParsersAction,  # pylint: disable=protected-access
             ):
-                return a
+                self._subparsers_action = a
+                return self._subparsers_action
         return None
 
     def _get_or_add_subparsers(self) -> argparse._SubParsersAction:
-        if self._subparsers_action is None:
-            if self._subparsers:
-                self._subparsers_action = self._find_subparsers_action()
-            else:
-                self._subparsers_action = self.add_subparsers(
-                    title="commands",
-                    metavar="<COMMAND>",
-                    dest=self.CMD_ATTR_NAME,
-                    parser_class=lambda **k: type(self)(
-                        **k,
-                        _is_subparser=True,
-                        formatter_class=self.formatter_class,
-                    ),
-                )
+        if self._subparsers_action is not None:
+            return self._subparsers_action
 
-        return self._subparsers_action
+        if self._subparsers:
+            self._find_subparsers_action()
+            assert self._subparsers_action
+            return self._subparsers_action
+
+        return self.add_subparsers()
 
     def _post_parse_args(  # type: ignore[override]
         self,
         namespace: argparse.Namespace,
     ) -> Namespace:
         func_mx_arg_groups: Dict[
             str,
```

### Comparing `yapx-0.2.1/src/yapx/exceptions.py` & `yapx-0.2.2/src/yapx/exceptions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/src/yapx/types.py` & `yapx-0.2.2/src/yapx/types.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/src/yapx/utils.py` & `yapx-0.2.2/src/yapx/utils.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/src/yapx.egg-info/SOURCES.txt` & `yapx-0.2.2/src/yapx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/src/yapx.egg-info/requires.txt` & `yapx-0.2.2/src/yapx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/tests/test_actions.py` & `yapx-0.2.2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/tests/test_add_arguments.py` & `yapx-0.2.2/tests/test_add_arguments.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/tests/test_add_arguments_future.py` & `yapx-0.2.2/tests/test_add_arguments_future.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/tests/test_add_command.py` & `yapx-0.2.2/tests/test_add_command.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/tests/test_arg.py` & `yapx-0.2.2/tests/test_arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/tests/test_run.py` & `yapx-0.2.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.1/tests/test_utils.py` & `yapx-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

