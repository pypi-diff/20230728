# Comparing `tmp/argparse-tui-0.1.2.tar.gz` & `tmp/argparse-tui-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-tui-0.1.2.tar", last modified: Mon Jul 24 22:10:24 2023, max compression
+gzip compressed data, was "argparse-tui-0.1.3.tar", last modified: Fri Jul 28 04:41:11 2023, max compression
```

## Comparing `argparse-tui-0.1.2.tar` & `argparse-tui-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.970949 argparse-tui-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5487 2023-07-24 22:10:24.970949 argparse-tui-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3823 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)     4714 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 22:10:24.970949 argparse-tui-0.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.958949 argparse-tui-0.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.962949 argparse-tui-0.1.2/src/argparse_tui/
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.966949 argparse-tui-0.1.2/src/argparse_tui/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      325 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-24 22:10:04.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7517 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/argparse.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7012 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/run_command.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4197 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/schemas.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    11772 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/__pycache__/tui.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-24 22:10:04.000000 argparse-tui-0.1.2/src/argparse_tui/__version__.py
--rw-r--r--   0 root         (0) root         (0)    10860 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/argparse.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/constants.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/detect_run_string.py
--rw-r--r--   0 root         (0) root         (0)    10938 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/run_command.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/schemas.py
--rw-r--r--   0 root         (0) root         (0)    12743 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/tui.py
--rw-r--r--   0 root         (0) root         (0)     3859 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/tui.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.966949 argparse-tui-0.1.2/src/argparse_tui/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.970949 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3449 2023-07-24 22:07:12.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4146 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2573 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     6957 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3854 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    11469 2023-07-24 22:07:10.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2647 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/about.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/command_info.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/command_tree.py
--rw-r--r--   0 root         (0) root         (0)     8067 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/form.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/multiple_choice.py
--rw-r--r--   0 root         (0) root         (0)    16529 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/src/argparse_tui/widgets/parameter_controls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.962949 argparse-tui-0.1.2/src/argparse_tui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5487 2023-07-24 22:10:24.000000 argparse-tui-0.1.2/src/argparse_tui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1724 2023-07-24 22:10:24.000000 argparse-tui-0.1.2/src/argparse_tui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 22:10:24.000000 argparse-tui-0.1.2/src/argparse_tui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-24 22:10:24.000000 argparse-tui-0.1.2/src/argparse_tui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 22:10:24.000000 argparse-tui-0.1.2/src/argparse_tui.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:10:24.970949 argparse-tui-0.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)     1611 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/tests/test_help_argparse.py
--rw-r--r--   0 root         (0) root         (0)     3897 2023-07-24 22:05:59.000000 argparse-tui-0.1.2/tests/test_run_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.475588 argparse-tui-0.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.479588 argparse-tui-0.1.3/src/argparse_tui/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.483588 argparse-tui-0.1.3/src/argparse_tui/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      325 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-28 04:40:50.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7696 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/argparse.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/run_command.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4197 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/schemas.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    11857 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/__pycache__/tui.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 04:40:50.000000 argparse-tui-0.1.3/src/argparse_tui/__version__.py
+-rw-r--r--   0 root         (0) root         (0)    11067 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/argparse.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/detect_run_string.py
+-rw-r--r--   0 root         (0) root         (0)    10938 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/run_command.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12871 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/tui.py
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/tui.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.487588 argparse-tui-0.1.3/src/argparse_tui/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.487588 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-07-28 04:38:02.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    11469 2023-07-28 04:38:01.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/about.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/command_info.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/command_tree.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/form.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/multiple_choice.py
+-rw-r--r--   0 root         (0) root         (0)    16529 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/src/argparse_tui/widgets/parameter_controls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.483588 argparse-tui-0.1.3/src/argparse_tui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 04:41:11.000000 argparse-tui-0.1.3/src/argparse_tui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:41:11.491588 argparse-tui-0.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/tests/test_help_argparse.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-07-28 04:37:17.000000 argparse-tui-0.1.3/tests/test_run_command.py
```

### Comparing `argparse-tui-0.1.2/LICENSE` & `argparse-tui-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/PKG-INFO` & `argparse-tui-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: argparse-tui
-Version: 0.1.2
-Summary: Display your Python argparse CLI as a TUI.
+Version: 0.1.3
+Summary: Display your Python argparse parser as a TUI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-Project-URL: Homepage, https://www.f2dv.com/code/r/argparse-tui/i
+Project-URL: Homepage, https://www.f2dv.com/r/argparse-tui
 Project-URL: Repository, https://www.github.com/fresh2dev/argparse-tui
 Project-URL: Funding, https://www.f2dv.com/fund
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 # argparse-tui
 
-> Display your Python argparse CLI as a TUI.
+> Display your Python argparse parser as a TUI.
 
-| Links         |                                                      |
-|---------------|------------------------------------------------------|
-| Code Repo     | https://www.github.com/fresh2dev/argparse-tui        |
-| Mirror Repo   | https://www.f2dv.com/code/r/argparse-tui             |
-| Documentation | https://www.f2dv.com/code/r/argparse-tui/i           |
-| Changelog     | https://www.f2dv.com/code/r/argparse-tui/i/changelog |
-| License       | https://www.f2dv.com/code/r/argparse-tui/i/license   |
-| Funding       | https://www.f2dv.com/fund                            |
-
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/releases)
-[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/releases)
-[![License](https://img.shields.io/github/license/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/argparse-tui/i/license)
+| Links         |                                               |
+|---------------|-----------------------------------------------|
+| Code Repo     | https://www.github.com/fresh2dev/argparse-tui |
+| Mirror Repo   | https://www.f2dv.com/r/argparse-tui           |
+| Documentation | https://www.f2dv.com/r/argparse-tui           |
+| Changelog     | https://www.f2dv.com/r/argparse-tui/changelog |
+| License       | https://www.f2dv.com/r/argparse-tui/license   |
+| Funding       | https://www.f2dv.com/fund                     |
+
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/r/argparse-tui/changelog)
+[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/r/argparse-tui/changelog)
+[![License](https://img.shields.io/github/license/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/r/argparse-tui/license)
+[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/argparse-tui&Date)
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/pulls)
-[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/argparse-tui&Date)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/argparse-tui?color=blue&style=for-the-badge)](https://pypi.org/project/argparse-tui)
-[![Docs Website](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/argparse-tui/i)](https://www.f2dv.com/code/r/argparse-tui/i)
-[![Coverage Website](https://img.shields.io/website?down_message=unavailable&label=coverage&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/argparse-tui/i/tests/coverage)](https://www.f2dv.com/code/r/argparse-tui/i/tests/coverage)
+[![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/argparse-tui)
+[![Changelog](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/argparse-tui/changelog)](https://www.f2dv.com/r/argparse-tui/changelog)
 [![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.f2dv.com/fund)
 
 ---
 
 ## Overview
 
 This is a fork of the Textualize [Trogon TUI library](https://github.com/Textualize/trogon.git) that introduces these features:
 
 - add support for Python's argparse parsers
+    - add `--tui` flag as an argument
+    - or, add `tui` command to your subparser
+    - or, invoke the TUI with `invoke_tui(parser)`
 - remove support for Click
 - add ability for TUI parameter to filter subcommands
 - support for manually constructing schemas
 - support for argparse
 - add examples for yapx, myke, and sys.argv
 - support ommission of hidden parameters and subcommands from the TUI
 - support the redaction of sensitive "secret" values
@@ -85,17 +88,47 @@
 
 # Or, add tui command (my-cli tui)
 add_tui_command(parser, command="tui", help="Open Textual UI")
 
 parser.print_help()
 ```
 
+### `invoke_tui`
+
+argparse-tui offers this function to display a TUI based on the arguments of the given parser:
+
+```python
+import argparse
+
+from argparse_tui import invoke_tui
+
+parser = argparse.ArgumentParser(prog="echo")
+
+parser.add_argument("STRING", nargs="*")
+
+parser.add_argument(
+    "-n",
+    action="store_true",
+    help="do not output the trailing newline",
+)
+
+invoke_tui(parser)
+```
+
+In this way, `argparse` is not actually serving as an argument parser, but instead as the specification language for the TUI. Whoa.
+
+### ChatGPT and TUIview
+
+Given the structured help text output of some CLI program, it turns out ChatGPT is decent at implementing an equivalent CLI using a Python argparse parser. Whoaaa.
+
+Coupled with `invoke_tui`, this means that argparse-tui is capable of producing a TUI for any CLI. This is the idea behind a tool built using argparse-tui: [TUIview](https://github.com/fresh2dev/tuiview). It does not use ChatGPT itself, but I used ChatGPT to generate equivalent-enough argparse parsers for `git`, `rsync`, `grep`.
+
 ## Docs
 
-See more examples in the [reference docs](https://www.f2dv.com/code/r/argparse-tui/i/reference/).
+See more examples in the [reference docs](https://www.f2dv.com/r/argparse-tui/reference).
 
 
 ## Support
 
 *Brought to you by...*
 
 <a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

### Comparing `argparse-tui-0.1.2/README.md` & `argparse-tui-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,239 +1,301 @@
 00000000: 2320 6172 6770 6172 7365 2d74 7569 0a0a  # argparse-tui..
 00000010: 3e20 4469 7370 6c61 7920 796f 7572 2050  > Display your P
-00000020: 7974 686f 6e20 6172 6770 6172 7365 2043  ython argparse C
-00000030: 4c49 2061 7320 6120 5455 492e 0a0a 7c20  LI as a TUI...| 
-00000040: 4c69 6e6b 7320 2020 2020 2020 2020 7c20  Links         | 
-00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000020: 7974 686f 6e20 6172 6770 6172 7365 2070  ython argparse p
+00000030: 6172 7365 7220 6173 2061 2054 5549 2e0a  arser as a TUI..
+00000040: 0a7c 204c 696e 6b73 2020 2020 2020 2020  .| Links        
+00000050: 207c 2020 2020 2020 2020 2020 2020 2020   |              
 00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000080: 2020 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d       |.|--------
-00000090: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00000080: 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|------------
+00000090: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
 000000a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000000b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000000c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
-000000d0: 7c20 436f 6465 2052 6570 6f20 2020 2020  | Code Repo     
-000000e0: 7c20 6874 7470 733a 2f2f 7777 772e 6769  | https://www.gi
-000000f0: 7468 7562 2e63 6f6d 2f66 7265 7368 3264  thub.com/fresh2d
-00000100: 6576 2f61 7267 7061 7273 652d 7475 6920  ev/argparse-tui 
-00000110: 2020 2020 2020 207c 0a7c 204d 6972 726f         |.| Mirro
-00000120: 7220 5265 706f 2020 207c 2068 7474 7073  r Repo   | https
-00000130: 3a2f 2f77 7777 2e66 3264 762e 636f 6d2f  ://www.f2dv.com/
-00000140: 636f 6465 2f72 2f61 7267 7061 7273 652d  code/r/argparse-
-00000150: 7475 6920 2020 2020 2020 2020 2020 2020  tui             
-00000160: 7c0a 7c20 446f 6375 6d65 6e74 6174 696f  |.| Documentatio
-00000170: 6e20 7c20 6874 7470 733a 2f2f 7777 772e  n | https://www.
-00000180: 6632 6476 2e63 6f6d 2f63 6f64 652f 722f  f2dv.com/code/r/
-00000190: 6172 6770 6172 7365 2d74 7569 2f69 2020  argparse-tui/i  
-000001a0: 2020 2020 2020 2020 207c 0a7c 2043 6861           |.| Cha
-000001b0: 6e67 656c 6f67 2020 2020 207c 2068 7474  ngelog     | htt
-000001c0: 7073 3a2f 2f77 7777 2e66 3264 762e 636f  ps://www.f2dv.co
-000001d0: 6d2f 636f 6465 2f72 2f61 7267 7061 7273  m/code/r/argpars
-000001e0: 652d 7475 692f 692f 6368 616e 6765 6c6f  e-tui/i/changelo
-000001f0: 6720 7c0a 7c20 4c69 6365 6e73 6520 2020  g |.| License   
-00000200: 2020 2020 7c20 6874 7470 733a 2f2f 7777      | https://ww
-00000210: 772e 6632 6476 2e63 6f6d 2f63 6f64 652f  w.f2dv.com/code/
-00000220: 722f 6172 6770 6172 7365 2d74 7569 2f69  r/argparse-tui/i
-00000230: 2f6c 6963 656e 7365 2020 207c 0a7c 2046  /license   |.| F
-00000240: 756e 6469 6e67 2020 2020 2020 207c 2068  unding       | h
-00000250: 7474 7073 3a2f 2f77 7777 2e66 3264 762e  ttps://www.f2dv.
-00000260: 636f 6d2f 6675 6e64 2020 2020 2020 2020  com/fund        
-00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000280: 2020 2020 7c0a 0a5b 215b 4769 7448 7562      |..[![GitHub
-00000290: 2072 656c 6561 7365 2028 6c61 7465 7374   release (latest
-000002a0: 2053 656d 5665 7229 5d28 6874 7470 733a   SemVer)](https:
-000002b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000002c0: 2f67 6974 6875 622f 762f 7265 6c65 6173  /github/v/releas
-000002d0: 652f 6672 6573 6832 6465 762f 6172 6770  e/fresh2dev/argp
-000002e0: 6172 7365 2d74 7569 3f63 6f6c 6f72 3d62  arse-tui?color=b
-000002f0: 6c75 6526 7374 796c 653d 666f 722d 7468  lue&style=for-th
-00000300: 652d 6261 6467 6529 5d28 6874 7470 733a  e-badge)](https:
-00000310: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
-00000320: 2f66 7265 7368 3264 6576 2f61 7267 7061  /fresh2dev/argpa
-00000330: 7273 652d 7475 692f 7265 6c65 6173 6573  rse-tui/releases
-00000340: 290a 5b21 5b47 6974 4875 6220 5265 6c65  ).[![GitHub Rele
-00000350: 6173 6520 4461 7465 5d28 6874 7470 733a  ase Date](https:
-00000360: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000370: 2f67 6974 6875 622f 7265 6c65 6173 652d  /github/release-
-00000380: 6461 7465 2f66 7265 7368 3264 6576 2f61  date/fresh2dev/a
-00000390: 7267 7061 7273 652d 7475 693f 636f 6c6f  rgparse-tui?colo
-000003a0: 723d 626c 7565 2673 7479 6c65 3d66 6f72  r=blue&style=for
-000003b0: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
-000003c0: 7073 3a2f 2f77 7777 2e67 6974 6875 622e  ps://www.github.
-000003d0: 636f 6d2f 6672 6573 6832 6465 762f 6172  com/fresh2dev/ar
-000003e0: 6770 6172 7365 2d74 7569 2f72 656c 6561  gparse-tui/relea
-000003f0: 7365 7329 0a5b 215b 4c69 6365 6e73 655d  ses).[![License]
-00000400: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000410: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
-00000420: 6963 656e 7365 2f66 7265 7368 3264 6576  icense/fresh2dev
-00000430: 2f61 7267 7061 7273 652d 7475 693f 636f  /argparse-tui?co
-00000440: 6c6f 723d 626c 7565 2673 7479 6c65 3d66  lor=blue&style=f
-00000450: 6f72 2d74 6865 2d62 6164 6765 295d 2868  or-the-badge)](h
-00000460: 7474 7073 3a2f 2f77 7777 2e66 3264 762e  ttps://www.f2dv.
-00000470: 636f 6d2f 636f 6465 2f72 2f61 7267 7061  com/code/r/argpa
-00000480: 7273 652d 7475 692f 692f 6c69 6365 6e73  rse-tui/i/licens
-00000490: 6529 0a5b 215b 4769 7448 7562 2069 7373  e).[![GitHub iss
-000004a0: 7565 735d 2868 7474 7073 3a2f 2f69 6d67  ues](https://img
-000004b0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-000004c0: 7562 2f69 7373 7565 732d 7261 772f 6672  ub/issues-raw/fr
-000004d0: 6573 6832 6465 762f 6172 6770 6172 7365  esh2dev/argparse
-000004e0: 2d74 7569 3f63 6f6c 6f72 3d62 6c75 6526  -tui?color=blue&
-000004f0: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-00000500: 6467 6529 5d28 6874 7470 733a 2f2f 7777  dge)](https://ww
-00000510: 772e 6769 7468 7562 2e63 6f6d 2f66 7265  w.github.com/fre
-00000520: 7368 3264 6576 2f61 7267 7061 7273 652d  sh2dev/argparse-
-00000530: 7475 692f 6973 7375 6573 290a 5b21 5b47  tui/issues).[![G
-00000540: 6974 4875 6220 7075 6c6c 2072 6571 7565  itHub pull reque
-00000550: 7374 735d 2868 7474 7073 3a2f 2f69 6d67  sts](https://img
-00000560: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000570: 7562 2f69 7373 7565 732d 7072 2d72 6177  ub/issues-pr-raw
-00000580: 2f66 7265 7368 3264 6576 2f61 7267 7061  /fresh2dev/argpa
-00000590: 7273 652d 7475 693f 636f 6c6f 723d 626c  rse-tui?color=bl
-000005a0: 7565 2673 7479 6c65 3d66 6f72 2d74 6865  ue&style=for-the
-000005b0: 2d62 6164 6765 295d 2868 7474 7073 3a2f  -badge)](https:/
-000005c0: 2f77 7777 2e67 6974 6875 622e 636f 6d2f  /www.github.com/
-000005d0: 6672 6573 6832 6465 762f 6172 6770 6172  fresh2dev/argpar
-000005e0: 7365 2d74 7569 2f70 756c 6c73 290a 5b21  se-tui/pulls).[!
-000005f0: 5b47 6974 4875 6220 5265 706f 2073 7461  [GitHub Repo sta
-00000600: 7273 5d28 6874 7470 733a 2f2f 696d 672e  rs](https://img.
-00000610: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000620: 622f 7374 6172 732f 6672 6573 6832 6465  b/stars/fresh2de
-00000630: 762f 6172 6770 6172 7365 2d74 7569 3f63  v/argparse-tui?c
-00000640: 6f6c 6f72 3d62 6c75 6526 7374 796c 653d  olor=blue&style=
-00000650: 666f 722d 7468 652d 6261 6467 6529 5d28  for-the-badge)](
-00000660: 6874 7470 733a 2f2f 7374 6172 2d68 6973  https://star-his
-00000670: 746f 7279 2e63 6f6d 2f23 6672 6573 6832  tory.com/#fresh2
-00000680: 6465 762f 6172 6770 6172 7365 2d74 7569  dev/argparse-tui
-00000690: 2644 6174 6529 0a5b 215b 5079 5049 202d  &Date).[![PyPI -
-000006a0: 2044 6f77 6e6c 6f61 6473 5d28 6874 7470   Downloads](http
-000006b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000006c0: 696f 2f70 7970 692f 646d 2f61 7267 7061  io/pypi/dm/argpa
-000006d0: 7273 652d 7475 693f 636f 6c6f 723d 626c  rse-tui?color=bl
-000006e0: 7565 2673 7479 6c65 3d66 6f72 2d74 6865  ue&style=for-the
-000006f0: 2d62 6164 6765 295d 2868 7474 7073 3a2f  -badge)](https:/
-00000700: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000710: 742f 6172 6770 6172 7365 2d74 7569 290a  t/argparse-tui).
-00000720: 5b21 5b44 6f63 7320 5765 6273 6974 655d  [![Docs Website]
-00000730: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000740: 656c 6473 2e69 6f2f 7765 6273 6974 653f  elds.io/website?
-00000750: 646f 776e 5f6d 6573 7361 6765 3d75 6e61  down_message=una
-00000760: 7661 696c 6162 6c65 266c 6162 656c 3d64  vailable&label=d
-00000770: 6f63 7326 7374 796c 653d 666f 722d 7468  ocs&style=for-th
-00000780: 652d 6261 6467 6526 7570 5f63 6f6c 6f72  e-badge&up_color
-00000790: 3d62 6c75 6526 7570 5f6d 6573 7361 6765  =blue&up_message
-000007a0: 3d61 7661 696c 6162 6c65 2675 726c 3d68  =available&url=h
-000007b0: 7474 7073 3a2f 2f77 7777 2e66 3264 762e  ttps://www.f2dv.
-000007c0: 636f 6d2f 636f 6465 2f72 2f61 7267 7061  com/code/r/argpa
-000007d0: 7273 652d 7475 692f 6929 5d28 6874 7470  rse-tui/i)](http
-000007e0: 733a 2f2f 7777 772e 6632 6476 2e63 6f6d  s://www.f2dv.com
-000007f0: 2f63 6f64 652f 722f 6172 6770 6172 7365  /code/r/argparse
-00000800: 2d74 7569 2f69 290a 5b21 5b43 6f76 6572  -tui/i).[![Cover
-00000810: 6167 6520 5765 6273 6974 655d 2868 7474  age Website](htt
-00000820: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000830: 2e69 6f2f 7765 6273 6974 653f 646f 776e  .io/website?down
-00000840: 5f6d 6573 7361 6765 3d75 6e61 7661 696c  _message=unavail
-00000850: 6162 6c65 266c 6162 656c 3d63 6f76 6572  able&label=cover
-00000860: 6167 6526 7374 796c 653d 666f 722d 7468  age&style=for-th
-00000870: 652d 6261 6467 6526 7570 5f63 6f6c 6f72  e-badge&up_color
-00000880: 3d62 6c75 6526 7570 5f6d 6573 7361 6765  =blue&up_message
-00000890: 3d61 7661 696c 6162 6c65 2675 726c 3d68  =available&url=h
-000008a0: 7474 7073 3a2f 2f77 7777 2e66 3264 762e  ttps://www.f2dv.
-000008b0: 636f 6d2f 636f 6465 2f72 2f61 7267 7061  com/code/r/argpa
-000008c0: 7273 652d 7475 692f 692f 7465 7374 732f  rse-tui/i/tests/
-000008d0: 636f 7665 7261 6765 295d 2868 7474 7073  coverage)](https
-000008e0: 3a2f 2f77 7777 2e66 3264 762e 636f 6d2f  ://www.f2dv.com/
-000008f0: 636f 6465 2f72 2f61 7267 7061 7273 652d  code/r/argparse-
-00000900: 7475 692f 692f 7465 7374 732f 636f 7665  tui/i/tests/cove
-00000910: 7261 6765 290a 5b21 5b46 756e 6469 6e67  rage).[![Funding
-00000920: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000930: 6965 6c64 732e 696f 2f62 6164 6765 2f66  ields.io/badge/f
-00000940: 756e 6469 6e67 2d25 3234 2532 3425 3234  unding-%24%24%24
-00000950: 2d62 6c75 653f 7374 796c 653d 666f 722d  -blue?style=for-
-00000960: 7468 652d 6261 6467 6529 5d28 6874 7470  the-badge)](http
-00000970: 733a 2f2f 7777 772e 6632 6476 2e63 6f6d  s://www.f2dv.com
-00000980: 2f66 756e 6429 0a0a 2d2d 2d0a 0a23 2320  /fund)..---..## 
-00000990: 4f76 6572 7669 6577 0a0a 5468 6973 2069  Overview..This i
-000009a0: 7320 6120 666f 726b 206f 6620 7468 6520  s a fork of the 
-000009b0: 5465 7874 7561 6c69 7a65 205b 5472 6f67  Textualize [Trog
-000009c0: 6f6e 2054 5549 206c 6962 7261 7279 5d28  on TUI library](
-000009d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000009e0: 6f6d 2f54 6578 7475 616c 697a 652f 7472  om/Textualize/tr
-000009f0: 6f67 6f6e 2e67 6974 2920 7468 6174 2069  ogon.git) that i
-00000a00: 6e74 726f 6475 6365 7320 7468 6573 6520  ntroduces these 
-00000a10: 6665 6174 7572 6573 3a0a 0a2d 2061 6464  features:..- add
-00000a20: 2073 7570 706f 7274 2066 6f72 2050 7974   support for Pyt
-00000a30: 686f 6e27 7320 6172 6770 6172 7365 2070  hon's argparse p
-00000a40: 6172 7365 7273 0a2d 2072 656d 6f76 6520  arsers.- remove 
-00000a50: 7375 7070 6f72 7420 666f 7220 436c 6963  support for Clic
-00000a60: 6b0a 2d20 6164 6420 6162 696c 6974 7920  k.- add ability 
-00000a70: 666f 7220 5455 4920 7061 7261 6d65 7465  for TUI paramete
-00000a80: 7220 746f 2066 696c 7465 7220 7375 6263  r to filter subc
-00000a90: 6f6d 6d61 6e64 730a 2d20 7375 7070 6f72  ommands.- suppor
-00000aa0: 7420 666f 7220 6d61 6e75 616c 6c79 2063  t for manually c
-00000ab0: 6f6e 7374 7275 6374 696e 6720 7363 6865  onstructing sche
-00000ac0: 6d61 730a 2d20 7375 7070 6f72 7420 666f  mas.- support fo
-00000ad0: 7220 6172 6770 6172 7365 0a2d 2061 6464  r argparse.- add
-00000ae0: 2065 7861 6d70 6c65 7320 666f 7220 7961   examples for ya
-00000af0: 7078 2c20 6d79 6b65 2c20 616e 6420 7379  px, myke, and sy
-00000b00: 732e 6172 6776 0a2d 2073 7570 706f 7274  s.argv.- support
-00000b10: 206f 6d6d 6973 7369 6f6e 206f 6620 6869   ommission of hi
-00000b20: 6464 656e 2070 6172 616d 6574 6572 7320  dden parameters 
-00000b30: 616e 6420 7375 6263 6f6d 6d61 6e64 7320  and subcommands 
-00000b40: 6672 6f6d 2074 6865 2054 5549 0a2d 2073  from the TUI.- s
-00000b50: 7570 706f 7274 2074 6865 2072 6564 6163  upport the redac
-00000b60: 7469 6f6e 206f 6620 7365 6e73 6974 6976  tion of sensitiv
-00000b70: 6520 2273 6563 7265 7422 2076 616c 7565  e "secret" value
-00000b80: 730a 2d20 7375 7070 6f72 7420 666f 7220  s.- support for 
-00000b90: 7368 6f77 696e 6720 7265 7175 6972 6564  showing required
-00000ba0: 2070 726f 6d70 7473 2061 7320 7265 6164   prompts as read
-00000bb0: 2d6f 6e6c 790a 2d20 6162 696c 6974 7920  -only.- ability 
-00000bc0: 746f 206a 6f69 6e20 6c69 7374 2061 7267  to join list arg
-00000bd0: 756d 656e 7473 2076 616c 7565 7320 6c69  uments values li
-00000be0: 6b65 2074 6869 733a 2060 2d78 2031 202d  ke this: `-x 1 -
-00000bf0: 7820 3220 2d78 2033 6020 2864 6566 6175  x 2 -x 3` (defau
-00000c00: 6c74 292c 206f 7220 6c69 6b65 2074 6869  lt), or like thi
-00000c10: 733a 2060 2d78 2031 2032 2033 600a 2d20  s: `-x 1 2 3`.- 
-00000c20: 7669 6d2d 6672 6965 6e64 6c79 206b 6579  vim-friendly key
-00000c30: 6269 6e64 696e 6773 0a0a 2323 2049 6e73  bindings..## Ins
-00000c40: 7461 6c6c 0a0a 496e 7374 616c 6c20 6672  tall..Install fr
-00000c50: 6f6d 2050 7950 493a 0a0a 6060 600a 7069  om PyPI:..```.pi
-00000c60: 7020 696e 7374 616c 6c20 6172 6770 6172  p install argpar
-00000c70: 7365 2d74 7569 0a60 6060 0a0a 2323 2055  se-tui.```..## U
-00000c80: 7365 0a0a 6060 6070 7974 686f 6e0a 696d  se..```python.im
-00000c90: 706f 7274 2061 7270 6172 7365 0a66 726f  port arparse.fro
-00000ca0: 6d20 6172 6770 6172 7365 5f74 7569 2069  m argparse_tui i
-00000cb0: 6d70 6f72 7420 6164 645f 7475 695f 6172  mport add_tui_ar
-00000cc0: 6775 6d65 6e74 2c20 6164 645f 7475 695f  gument, add_tui_
-00000cd0: 636f 6d6d 616e 640a 0a70 6172 7365 7220  command..parser 
-00000ce0: 3d20 6172 6770 6172 7365 2e41 7267 756d  = argparse.Argum
-00000cf0: 656e 7450 6172 7365 7228 290a 0a23 2041  entParser()..# A
-00000d00: 6464 2074 7569 2061 7267 756d 656e 7420  dd tui argument 
-00000d10: 286d 792d 636c 6920 2d2d 7475 6929 0a61  (my-cli --tui).a
-00000d20: 6464 5f74 7569 5f61 7267 756d 656e 7428  dd_tui_argument(
-00000d30: 7061 7273 6572 2c20 6f70 7469 6f6e 5f73  parser, option_s
-00000d40: 7472 696e 6773 3d5b 222d 2d74 7569 225d  trings=["--tui"]
-00000d50: 2c20 6865 6c70 3d22 4f70 656e 2054 6578  , help="Open Tex
-00000d60: 7475 616c 2055 4922 290a 0a23 204f 722c  tual UI")..# Or,
-00000d70: 2061 6464 2074 7569 2063 6f6d 6d61 6e64   add tui command
-00000d80: 2028 6d79 2d63 6c69 2074 7569 290a 6164   (my-cli tui).ad
-00000d90: 645f 7475 695f 636f 6d6d 616e 6428 7061  d_tui_command(pa
-00000da0: 7273 6572 2c20 636f 6d6d 616e 643d 2274  rser, command="t
-00000db0: 7569 222c 2068 656c 703d 224f 7065 6e20  ui", help="Open 
-00000dc0: 5465 7874 7561 6c20 5549 2229 0a0a 7061  Textual UI")..pa
-00000dd0: 7273 6572 2e70 7269 6e74 5f68 656c 7028  rser.print_help(
-00000de0: 290a 6060 600a 0a23 2320 446f 6373 0a0a  ).```..## Docs..
-00000df0: 5365 6520 6d6f 7265 2065 7861 6d70 6c65  See more example
-00000e00: 7320 696e 2074 6865 205b 7265 6665 7265  s in the [refere
-00000e10: 6e63 6520 646f 6373 5d28 6874 7470 733a  nce docs](https:
-00000e20: 2f2f 7777 772e 6632 6476 2e63 6f6d 2f63  //www.f2dv.com/c
-00000e30: 6f64 652f 722f 6172 6770 6172 7365 2d74  ode/r/argparse-t
-00000e40: 7569 2f69 2f72 6566 6572 656e 6365 2f29  ui/i/reference/)
-00000e50: 2e0a 0a0a 2323 2053 7570 706f 7274 0a0a  ....## Support..
-00000e60: 2a42 726f 7567 6874 2074 6f20 796f 7520  *Brought to you 
-00000e70: 6279 2e2e 2e2a 0a0a 3c61 2068 7265 663d  by...*..<a href=
-00000e80: 2268 7474 7073 3a2f 2f77 7777 2e66 3264  "https://www.f2d
-00000e90: 762e 636f 6d22 3e3c 696d 6720 7372 633d  v.com"><img src=
-00000ea0: 2268 7474 7073 3a2f 2f69 6d67 2e66 7265  "https://img.fre
-00000eb0: 7368 322e 6465 762f 6672 6573 6832 6465  sh2.dev/fresh2de
-00000ec0: 762e 7376 6722 2073 7479 6c65 3d22 6669  v.svg" style="fi
-00000ed0: 6c74 6572 3a20 696e 7665 7274 2835 3025  lter: invert(50%
-00000ee0: 293b 223e 3c2f 696d 673e 3c2f 613e 0a    );"></img></a>.
+000000c0: 2d2d 2d7c 0a7c 2043 6f64 6520 5265 706f  ---|.| Code Repo
+000000d0: 2020 2020 207c 2068 7474 7073 3a2f 2f77       | https://w
+000000e0: 7777 2e67 6974 6875 622e 636f 6d2f 6672  ww.github.com/fr
+000000f0: 6573 6832 6465 762f 6172 6770 6172 7365  esh2dev/argparse
+00000100: 2d74 7569 207c 0a7c 204d 6972 726f 7220  -tui |.| Mirror 
+00000110: 5265 706f 2020 207c 2068 7474 7073 3a2f  Repo   | https:/
+00000120: 2f77 7777 2e66 3264 762e 636f 6d2f 722f  /www.f2dv.com/r/
+00000130: 6172 6770 6172 7365 2d74 7569 2020 2020  argparse-tui    
+00000140: 2020 2020 2020 207c 0a7c 2044 6f63 756d         |.| Docum
+00000150: 656e 7461 7469 6f6e 207c 2068 7474 7073  entation | https
+00000160: 3a2f 2f77 7777 2e66 3264 762e 636f 6d2f  ://www.f2dv.com/
+00000170: 722f 6172 6770 6172 7365 2d74 7569 2020  r/argparse-tui  
+00000180: 2020 2020 2020 2020 207c 0a7c 2043 6861           |.| Cha
+00000190: 6e67 656c 6f67 2020 2020 207c 2068 7474  ngelog     | htt
+000001a0: 7073 3a2f 2f77 7777 2e66 3264 762e 636f  ps://www.f2dv.co
+000001b0: 6d2f 722f 6172 6770 6172 7365 2d74 7569  m/r/argparse-tui
+000001c0: 2f63 6861 6e67 656c 6f67 207c 0a7c 204c  /changelog |.| L
+000001d0: 6963 656e 7365 2020 2020 2020 207c 2068  icense       | h
+000001e0: 7474 7073 3a2f 2f77 7777 2e66 3264 762e  ttps://www.f2dv.
+000001f0: 636f 6d2f 722f 6172 6770 6172 7365 2d74  com/r/argparse-t
+00000200: 7569 2f6c 6963 656e 7365 2020 207c 0a7c  ui/license   |.|
+00000210: 2046 756e 6469 6e67 2020 2020 2020 207c   Funding       |
+00000220: 2068 7474 7073 3a2f 2f77 7777 2e66 3264   https://www.f2d
+00000230: 762e 636f 6d2f 6675 6e64 2020 2020 2020  v.com/fund      
+00000240: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000250: 0a0a 5b21 5b47 6974 4875 6220 7265 6c65  ..[![GitHub rele
+00000260: 6173 6520 286c 6174 6573 7420 5365 6d56  ase (latest SemV
+00000270: 6572 295d 2868 7474 7073 3a2f 2f69 6d67  er)](https://img
+00000280: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000290: 7562 2f76 2f72 656c 6561 7365 2f66 7265  ub/v/release/fre
+000002a0: 7368 3264 6576 2f61 7267 7061 7273 652d  sh2dev/argparse-
+000002b0: 7475 693f 636f 6c6f 723d 626c 7565 2673  tui?color=blue&s
+000002c0: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
+000002d0: 6765 295d 2868 7474 7073 3a2f 2f77 7777  ge)](https://www
+000002e0: 2e66 3264 762e 636f 6d2f 722f 6172 6770  .f2dv.com/r/argp
+000002f0: 6172 7365 2d74 7569 2f63 6861 6e67 656c  arse-tui/changel
+00000300: 6f67 290a 5b21 5b47 6974 4875 6220 5265  og).[![GitHub Re
+00000310: 6c65 6173 6520 4461 7465 5d28 6874 7470  lease Date](http
+00000320: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000330: 696f 2f67 6974 6875 622f 7265 6c65 6173  io/github/releas
+00000340: 652d 6461 7465 2f66 7265 7368 3264 6576  e-date/fresh2dev
+00000350: 2f61 7267 7061 7273 652d 7475 693f 636f  /argparse-tui?co
+00000360: 6c6f 723d 626c 7565 2673 7479 6c65 3d66  lor=blue&style=f
+00000370: 6f72 2d74 6865 2d62 6164 6765 295d 2868  or-the-badge)](h
+00000380: 7474 7073 3a2f 2f77 7777 2e66 3264 762e  ttps://www.f2dv.
+00000390: 636f 6d2f 722f 6172 6770 6172 7365 2d74  com/r/argparse-t
+000003a0: 7569 2f63 6861 6e67 656c 6f67 290a 5b21  ui/changelog).[!
+000003b0: 5b4c 6963 656e 7365 5d28 6874 7470 733a  [License](https:
+000003c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000003d0: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+000003e0: 6672 6573 6832 6465 762f 6172 6770 6172  fresh2dev/argpar
+000003f0: 7365 2d74 7569 3f63 6f6c 6f72 3d62 6c75  se-tui?color=blu
+00000400: 6526 7374 796c 653d 666f 722d 7468 652d  e&style=for-the-
+00000410: 6261 6467 6529 5d28 6874 7470 733a 2f2f  badge)](https://
+00000420: 7777 772e 6632 6476 2e63 6f6d 2f72 2f61  www.f2dv.com/r/a
+00000430: 7267 7061 7273 652d 7475 692f 6c69 6365  rgparse-tui/lice
+00000440: 6e73 6529 0a5b 215b 4769 7448 7562 2052  nse).[![GitHub R
+00000450: 6570 6f20 7374 6172 735d 2868 7474 7073  epo stars](https
+00000460: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000470: 6f2f 6769 7468 7562 2f73 7461 7273 2f66  o/github/stars/f
+00000480: 7265 7368 3264 6576 2f61 7267 7061 7273  resh2dev/argpars
+00000490: 652d 7475 693f 636f 6c6f 723d 626c 7565  e-tui?color=blue
+000004a0: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
+000004b0: 6164 6765 295d 2868 7474 7073 3a2f 2f73  adge)](https://s
+000004c0: 7461 722d 6869 7374 6f72 792e 636f 6d2f  tar-history.com/
+000004d0: 2366 7265 7368 3264 6576 2f61 7267 7061  #fresh2dev/argpa
+000004e0: 7273 652d 7475 6926 4461 7465 290a 5b21  rse-tui&Date).[!
+000004f0: 5b47 6974 4875 6220 6973 7375 6573 5d28  [GitHub issues](
+00000500: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000510: 6c64 732e 696f 2f67 6974 6875 622f 6973  lds.io/github/is
+00000520: 7375 6573 2d72 6177 2f66 7265 7368 3264  sues-raw/fresh2d
+00000530: 6576 2f61 7267 7061 7273 652d 7475 693f  ev/argparse-tui?
+00000540: 636f 6c6f 723d 626c 7565 2673 7479 6c65  color=blue&style
+00000550: 3d66 6f72 2d74 6865 2d62 6164 6765 295d  =for-the-badge)]
+00000560: 2868 7474 7073 3a2f 2f77 7777 2e67 6974  (https://www.git
+00000570: 6875 622e 636f 6d2f 6672 6573 6832 6465  hub.com/fresh2de
+00000580: 762f 6172 6770 6172 7365 2d74 7569 2f69  v/argparse-tui/i
+00000590: 7373 7565 7329 0a5b 215b 4769 7448 7562  ssues).[![GitHub
+000005a0: 2070 756c 6c20 7265 7175 6573 7473 5d28   pull requests](
+000005b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000005c0: 6c64 732e 696f 2f67 6974 6875 622f 6973  lds.io/github/is
+000005d0: 7375 6573 2d70 722d 7261 772f 6672 6573  sues-pr-raw/fres
+000005e0: 6832 6465 762f 6172 6770 6172 7365 2d74  h2dev/argparse-t
+000005f0: 7569 3f63 6f6c 6f72 3d62 6c75 6526 7374  ui?color=blue&st
+00000600: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00000610: 6529 5d28 6874 7470 733a 2f2f 7777 772e  e)](https://www.
+00000620: 6769 7468 7562 2e63 6f6d 2f66 7265 7368  github.com/fresh
+00000630: 3264 6576 2f61 7267 7061 7273 652d 7475  2dev/argparse-tu
+00000640: 692f 7075 6c6c 7329 0a5b 215b 5079 5049  i/pulls).[![PyPI
+00000650: 202d 2044 6f77 6e6c 6f61 6473 5d28 6874   - Downloads](ht
+00000660: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000670: 732e 696f 2f70 7970 692f 646d 2f61 7267  s.io/pypi/dm/arg
+00000680: 7061 7273 652d 7475 693f 636f 6c6f 723d  parse-tui?color=
+00000690: 626c 7565 2673 7479 6c65 3d66 6f72 2d74  blue&style=for-t
+000006a0: 6865 2d62 6164 6765 295d 2868 7474 7073  he-badge)](https
+000006b0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000006c0: 6563 742f 6172 6770 6172 7365 2d74 7569  ect/argparse-tui
+000006d0: 290a 5b21 5b44 6f63 6b65 7220 5075 6c6c  ).[![Docker Pull
+000006e0: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+000006f0: 6869 656c 6473 2e69 6f2f 646f 636b 6572  hields.io/docker
+00000700: 2f70 756c 6c73 2f66 7265 7368 3264 6576  /pulls/fresh2dev
+00000710: 2f61 7267 7061 7273 652d 7475 693f 636f  /argparse-tui?co
+00000720: 6c6f 723d 626c 7565 2673 7479 6c65 3d66  lor=blue&style=f
+00000730: 6f72 2d74 6865 2d62 6164 6765 295d 2868  or-the-badge)](h
+00000740: 7474 7073 3a2f 2f68 7562 2e64 6f63 6b65  ttps://hub.docke
+00000750: 722e 636f 6d2f 722f 6672 6573 6832 6465  r.com/r/fresh2de
+00000760: 762f 6172 6770 6172 7365 2d74 7569 290a  v/argparse-tui).
+00000770: 5b21 5b43 6861 6e67 656c 6f67 5d28 6874  [![Changelog](ht
+00000780: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000790: 732e 696f 2f77 6562 7369 7465 3f64 6f77  s.io/website?dow
+000007a0: 6e5f 6d65 7373 6167 653d 756e 6176 6169  n_message=unavai
+000007b0: 6c61 626c 6526 6c61 6265 6c3d 646f 6373  lable&label=docs
+000007c0: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
+000007d0: 6164 6765 2675 705f 636f 6c6f 723d 626c  adge&up_color=bl
+000007e0: 7565 2675 705f 6d65 7373 6167 653d 6176  ue&up_message=av
+000007f0: 6169 6c61 626c 6526 7572 6c3d 6874 7470  ailable&url=http
+00000800: 733a 2f2f 7777 772e 6632 6476 2e63 6f6d  s://www.f2dv.com
+00000810: 2f72 2f61 7267 7061 7273 652d 7475 692f  /r/argparse-tui/
+00000820: 6368 616e 6765 6c6f 6729 5d28 6874 7470  changelog)](http
+00000830: 733a 2f2f 7777 772e 6632 6476 2e63 6f6d  s://www.f2dv.com
+00000840: 2f72 2f61 7267 7061 7273 652d 7475 692f  /r/argparse-tui/
+00000850: 6368 616e 6765 6c6f 6729 0a5b 215b 4675  changelog).[![Fu
+00000860: 6e64 696e 675d 2868 7474 7073 3a2f 2f69  nding](https://i
+00000870: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000880: 6467 652f 6675 6e64 696e 672d 2532 3425  dge/funding-%24%
+00000890: 3234 2532 342d 626c 7565 3f73 7479 6c65  24%24-blue?style
+000008a0: 3d66 6f72 2d74 6865 2d62 6164 6765 295d  =for-the-badge)]
+000008b0: 2868 7474 7073 3a2f 2f77 7777 2e66 3264  (https://www.f2d
+000008c0: 762e 636f 6d2f 6675 6e64 290a 0a2d 2d2d  v.com/fund)..---
+000008d0: 0a0a 2323 204f 7665 7276 6965 770a 0a54  ..## Overview..T
+000008e0: 6869 7320 6973 2061 2066 6f72 6b20 6f66  his is a fork of
+000008f0: 2074 6865 2054 6578 7475 616c 697a 6520   the Textualize 
+00000900: 5b54 726f 676f 6e20 5455 4920 6c69 6272  [Trogon TUI libr
+00000910: 6172 795d 2868 7474 7073 3a2f 2f67 6974  ary](https://git
+00000920: 6875 622e 636f 6d2f 5465 7874 7561 6c69  hub.com/Textuali
+00000930: 7a65 2f74 726f 676f 6e2e 6769 7429 2074  ze/trogon.git) t
+00000940: 6861 7420 696e 7472 6f64 7563 6573 2074  hat introduces t
+00000950: 6865 7365 2066 6561 7475 7265 733a 0a0a  hese features:..
+00000960: 2d20 6164 6420 7375 7070 6f72 7420 666f  - add support fo
+00000970: 7220 5079 7468 6f6e 2773 2061 7267 7061  r Python's argpa
+00000980: 7273 6520 7061 7273 6572 730a 2020 2020  rse parsers.    
+00000990: 2d20 6164 6420 602d 2d74 7569 6020 666c  - add `--tui` fl
+000009a0: 6167 2061 7320 616e 2061 7267 756d 656e  ag as an argumen
+000009b0: 740a 2020 2020 2d20 6f72 2c20 6164 6420  t.    - or, add 
+000009c0: 6074 7569 6020 636f 6d6d 616e 6420 746f  `tui` command to
+000009d0: 2079 6f75 7220 7375 6270 6172 7365 720a   your subparser.
+000009e0: 2020 2020 2d20 6f72 2c20 696e 766f 6b65      - or, invoke
+000009f0: 2074 6865 2054 5549 2077 6974 6820 6069   the TUI with `i
+00000a00: 6e76 6f6b 655f 7475 6928 7061 7273 6572  nvoke_tui(parser
+00000a10: 2960 0a2d 2072 656d 6f76 6520 7375 7070  )`.- remove supp
+00000a20: 6f72 7420 666f 7220 436c 6963 6b0a 2d20  ort for Click.- 
+00000a30: 6164 6420 6162 696c 6974 7920 666f 7220  add ability for 
+00000a40: 5455 4920 7061 7261 6d65 7465 7220 746f  TUI parameter to
+00000a50: 2066 696c 7465 7220 7375 6263 6f6d 6d61   filter subcomma
+00000a60: 6e64 730a 2d20 7375 7070 6f72 7420 666f  nds.- support fo
+00000a70: 7220 6d61 6e75 616c 6c79 2063 6f6e 7374  r manually const
+00000a80: 7275 6374 696e 6720 7363 6865 6d61 730a  ructing schemas.
+00000a90: 2d20 7375 7070 6f72 7420 666f 7220 6172  - support for ar
+00000aa0: 6770 6172 7365 0a2d 2061 6464 2065 7861  gparse.- add exa
+00000ab0: 6d70 6c65 7320 666f 7220 7961 7078 2c20  mples for yapx, 
+00000ac0: 6d79 6b65 2c20 616e 6420 7379 732e 6172  myke, and sys.ar
+00000ad0: 6776 0a2d 2073 7570 706f 7274 206f 6d6d  gv.- support omm
+00000ae0: 6973 7369 6f6e 206f 6620 6869 6464 656e  ission of hidden
+00000af0: 2070 6172 616d 6574 6572 7320 616e 6420   parameters and 
+00000b00: 7375 6263 6f6d 6d61 6e64 7320 6672 6f6d  subcommands from
+00000b10: 2074 6865 2054 5549 0a2d 2073 7570 706f   the TUI.- suppo
+00000b20: 7274 2074 6865 2072 6564 6163 7469 6f6e  rt the redaction
+00000b30: 206f 6620 7365 6e73 6974 6976 6520 2273   of sensitive "s
+00000b40: 6563 7265 7422 2076 616c 7565 730a 2d20  ecret" values.- 
+00000b50: 7375 7070 6f72 7420 666f 7220 7368 6f77  support for show
+00000b60: 696e 6720 7265 7175 6972 6564 2070 726f  ing required pro
+00000b70: 6d70 7473 2061 7320 7265 6164 2d6f 6e6c  mpts as read-onl
+00000b80: 790a 2d20 6162 696c 6974 7920 746f 206a  y.- ability to j
+00000b90: 6f69 6e20 6c69 7374 2061 7267 756d 656e  oin list argumen
+00000ba0: 7473 2076 616c 7565 7320 6c69 6b65 2074  ts values like t
+00000bb0: 6869 733a 2060 2d78 2031 202d 7820 3220  his: `-x 1 -x 2 
+00000bc0: 2d78 2033 6020 2864 6566 6175 6c74 292c  -x 3` (default),
+00000bd0: 206f 7220 6c69 6b65 2074 6869 733a 2060   or like this: `
+00000be0: 2d78 2031 2032 2033 600a 2d20 7669 6d2d  -x 1 2 3`.- vim-
+00000bf0: 6672 6965 6e64 6c79 206b 6579 6269 6e64  friendly keybind
+00000c00: 696e 6773 0a0a 2323 2049 6e73 7461 6c6c  ings..## Install
+00000c10: 0a0a 496e 7374 616c 6c20 6672 6f6d 2050  ..Install from P
+00000c20: 7950 493a 0a0a 6060 600a 7069 7020 696e  yPI:..```.pip in
+00000c30: 7374 616c 6c20 6172 6770 6172 7365 2d74  stall argparse-t
+00000c40: 7569 0a60 6060 0a0a 2323 2055 7365 0a0a  ui.```..## Use..
+00000c50: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000c60: 2061 7270 6172 7365 0a66 726f 6d20 6172   arparse.from ar
+00000c70: 6770 6172 7365 5f74 7569 2069 6d70 6f72  gparse_tui impor
+00000c80: 7420 6164 645f 7475 695f 6172 6775 6d65  t add_tui_argume
+00000c90: 6e74 2c20 6164 645f 7475 695f 636f 6d6d  nt, add_tui_comm
+00000ca0: 616e 640a 0a70 6172 7365 7220 3d20 6172  and..parser = ar
+00000cb0: 6770 6172 7365 2e41 7267 756d 656e 7450  gparse.ArgumentP
+00000cc0: 6172 7365 7228 290a 0a23 2041 6464 2074  arser()..# Add t
+00000cd0: 7569 2061 7267 756d 656e 7420 286d 792d  ui argument (my-
+00000ce0: 636c 6920 2d2d 7475 6929 0a61 6464 5f74  cli --tui).add_t
+00000cf0: 7569 5f61 7267 756d 656e 7428 7061 7273  ui_argument(pars
+00000d00: 6572 2c20 6f70 7469 6f6e 5f73 7472 696e  er, option_strin
+00000d10: 6773 3d5b 222d 2d74 7569 225d 2c20 6865  gs=["--tui"], he
+00000d20: 6c70 3d22 4f70 656e 2054 6578 7475 616c  lp="Open Textual
+00000d30: 2055 4922 290a 0a23 204f 722c 2061 6464   UI")..# Or, add
+00000d40: 2074 7569 2063 6f6d 6d61 6e64 2028 6d79   tui command (my
+00000d50: 2d63 6c69 2074 7569 290a 6164 645f 7475  -cli tui).add_tu
+00000d60: 695f 636f 6d6d 616e 6428 7061 7273 6572  i_command(parser
+00000d70: 2c20 636f 6d6d 616e 643d 2274 7569 222c  , command="tui",
+00000d80: 2068 656c 703d 224f 7065 6e20 5465 7874   help="Open Text
+00000d90: 7561 6c20 5549 2229 0a0a 7061 7273 6572  ual UI")..parser
+00000da0: 2e70 7269 6e74 5f68 656c 7028 290a 6060  .print_help().``
+00000db0: 600a 0a23 2323 2060 696e 766f 6b65 5f74  `..### `invoke_t
+00000dc0: 7569 600a 0a61 7267 7061 7273 652d 7475  ui`..argparse-tu
+00000dd0: 6920 6f66 6665 7273 2074 6869 7320 6675  i offers this fu
+00000de0: 6e63 7469 6f6e 2074 6f20 6469 7370 6c61  nction to displa
+00000df0: 7920 6120 5455 4920 6261 7365 6420 6f6e  y a TUI based on
+00000e00: 2074 6865 2061 7267 756d 656e 7473 206f   the arguments o
+00000e10: 6620 7468 6520 6769 7665 6e20 7061 7273  f the given pars
+00000e20: 6572 3a0a 0a60 6060 7079 7468 6f6e 0a69  er:..```python.i
+00000e30: 6d70 6f72 7420 6172 6770 6172 7365 0a0a  mport argparse..
+00000e40: 6672 6f6d 2061 7267 7061 7273 655f 7475  from argparse_tu
+00000e50: 6920 696d 706f 7274 2069 6e76 6f6b 655f  i import invoke_
+00000e60: 7475 690a 0a70 6172 7365 7220 3d20 6172  tui..parser = ar
+00000e70: 6770 6172 7365 2e41 7267 756d 656e 7450  gparse.ArgumentP
+00000e80: 6172 7365 7228 7072 6f67 3d22 6563 686f  arser(prog="echo
+00000e90: 2229 0a0a 7061 7273 6572 2e61 6464 5f61  ")..parser.add_a
+00000ea0: 7267 756d 656e 7428 2253 5452 494e 4722  rgument("STRING"
+00000eb0: 2c20 6e61 7267 733d 222a 2229 0a0a 7061  , nargs="*")..pa
+00000ec0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00000ed0: 7428 0a20 2020 2022 2d6e 222c 0a20 2020  t(.    "-n",.   
+00000ee0: 2061 6374 696f 6e3d 2273 746f 7265 5f74   action="store_t
+00000ef0: 7275 6522 2c0a 2020 2020 6865 6c70 3d22  rue",.    help="
+00000f00: 646f 206e 6f74 206f 7574 7075 7420 7468  do not output th
+00000f10: 6520 7472 6169 6c69 6e67 206e 6577 6c69  e trailing newli
+00000f20: 6e65 222c 0a29 0a0a 696e 766f 6b65 5f74  ne",.)..invoke_t
+00000f30: 7569 2870 6172 7365 7229 0a60 6060 0a0a  ui(parser).```..
+00000f40: 496e 2074 6869 7320 7761 792c 2060 6172  In this way, `ar
+00000f50: 6770 6172 7365 6020 6973 206e 6f74 2061  gparse` is not a
+00000f60: 6374 7561 6c6c 7920 7365 7276 696e 6720  ctually serving 
+00000f70: 6173 2061 6e20 6172 6775 6d65 6e74 2070  as an argument p
+00000f80: 6172 7365 722c 2062 7574 2069 6e73 7465  arser, but inste
+00000f90: 6164 2061 7320 7468 6520 7370 6563 6966  ad as the specif
+00000fa0: 6963 6174 696f 6e20 6c61 6e67 7561 6765  ication language
+00000fb0: 2066 6f72 2074 6865 2054 5549 2e20 5768   for the TUI. Wh
+00000fc0: 6f61 2e0a 0a23 2323 2043 6861 7447 5054  oa...### ChatGPT
+00000fd0: 2061 6e64 2054 5549 7669 6577 0a0a 4769   and TUIview..Gi
+00000fe0: 7665 6e20 7468 6520 7374 7275 6374 7572  ven the structur
+00000ff0: 6564 2068 656c 7020 7465 7874 206f 7574  ed help text out
+00001000: 7075 7420 6f66 2073 6f6d 6520 434c 4920  put of some CLI 
+00001010: 7072 6f67 7261 6d2c 2069 7420 7475 726e  program, it turn
+00001020: 7320 6f75 7420 4368 6174 4750 5420 6973  s out ChatGPT is
+00001030: 2064 6563 656e 7420 6174 2069 6d70 6c65   decent at imple
+00001040: 6d65 6e74 696e 6720 616e 2065 7175 6976  menting an equiv
+00001050: 616c 656e 7420 434c 4920 7573 696e 6720  alent CLI using 
+00001060: 6120 5079 7468 6f6e 2061 7267 7061 7273  a Python argpars
+00001070: 6520 7061 7273 6572 2e20 5768 6f61 6161  e parser. Whoaaa
+00001080: 2e0a 0a43 6f75 706c 6564 2077 6974 6820  ...Coupled with 
+00001090: 6069 6e76 6f6b 655f 7475 6960 2c20 7468  `invoke_tui`, th
+000010a0: 6973 206d 6561 6e73 2074 6861 7420 6172  is means that ar
+000010b0: 6770 6172 7365 2d74 7569 2069 7320 6361  gparse-tui is ca
+000010c0: 7061 626c 6520 6f66 2070 726f 6475 6369  pable of produci
+000010d0: 6e67 2061 2054 5549 2066 6f72 2061 6e79  ng a TUI for any
+000010e0: 2043 4c49 2e20 5468 6973 2069 7320 7468   CLI. This is th
+000010f0: 6520 6964 6561 2062 6568 696e 6420 6120  e idea behind a 
+00001100: 746f 6f6c 2062 7569 6c74 2075 7369 6e67  tool built using
+00001110: 2061 7267 7061 7273 652d 7475 693a 205b   argparse-tui: [
+00001120: 5455 4976 6965 775d 2868 7474 7073 3a2f  TUIview](https:/
+00001130: 2f67 6974 6875 622e 636f 6d2f 6672 6573  /github.com/fres
+00001140: 6832 6465 762f 7475 6976 6965 7729 2e20  h2dev/tuiview). 
+00001150: 4974 2064 6f65 7320 6e6f 7420 7573 6520  It does not use 
+00001160: 4368 6174 4750 5420 6974 7365 6c66 2c20  ChatGPT itself, 
+00001170: 6275 7420 4920 7573 6564 2043 6861 7447  but I used ChatG
+00001180: 5054 2074 6f20 6765 6e65 7261 7465 2065  PT to generate e
+00001190: 7175 6976 616c 656e 742d 656e 6f75 6768  quivalent-enough
+000011a0: 2061 7267 7061 7273 6520 7061 7273 6572   argparse parser
+000011b0: 7320 666f 7220 6067 6974 602c 2060 7273  s for `git`, `rs
+000011c0: 796e 6360 2c20 6067 7265 7060 2e0a 0a23  ync`, `grep`...#
+000011d0: 2320 446f 6373 0a0a 5365 6520 6d6f 7265  # Docs..See more
+000011e0: 2065 7861 6d70 6c65 7320 696e 2074 6865   examples in the
+000011f0: 205b 7265 6665 7265 6e63 6520 646f 6373   [reference docs
+00001200: 5d28 6874 7470 733a 2f2f 7777 772e 6632  ](https://www.f2
+00001210: 6476 2e63 6f6d 2f72 2f61 7267 7061 7273  dv.com/r/argpars
+00001220: 652d 7475 692f 7265 6665 7265 6e63 6529  e-tui/reference)
+00001230: 2e0a 0a0a 2323 2053 7570 706f 7274 0a0a  ....## Support..
+00001240: 2a42 726f 7567 6874 2074 6f20 796f 7520  *Brought to you 
+00001250: 6279 2e2e 2e2a 0a0a 3c61 2068 7265 663d  by...*..<a href=
+00001260: 2268 7474 7073 3a2f 2f77 7777 2e66 3264  "https://www.f2d
+00001270: 762e 636f 6d22 3e3c 696d 6720 7372 633d  v.com"><img src=
+00001280: 2268 7474 7073 3a2f 2f69 6d67 2e66 7265  "https://img.fre
+00001290: 7368 322e 6465 762f 6672 6573 6832 6465  sh2.dev/fresh2de
+000012a0: 762e 7376 6722 2073 7479 6c65 3d22 6669  v.svg" style="fi
+000012b0: 6c74 6572 3a20 696e 7665 7274 2835 3025  lter: invert(50%
+000012c0: 293b 223e 3c2f 696d 673e 3c2f 613e 0a    );"></img></a>.
```

### Comparing `argparse-tui-0.1.2/pyproject.toml` & `argparse-tui-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "argparse-tui"
 authors = [
     {name = "Donald Mellenbruch", email = "hello@f2dv.com"},
 ]
-description = "Display your Python argparse CLI as a TUI."
+description = "Display your Python argparse parser as a TUI."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["version"]
@@ -53,15 +53,15 @@
     "pylint==2.*",
     "pylint-pytest==1.*",
     "packaging==23.*",
     "mockish>=0.1.1,<2",
 ]
 
 [project.urls]
-Homepage = "https://www.f2dv.com/code/r/argparse-tui/i"
+Homepage = "https://www.f2dv.com/r/argparse-tui"
 Repository = "https://www.github.com/fresh2dev/argparse-tui"
 Funding = "https://www.f2dv.com/fund"
 
 [tool.setuptools.package-data]
 "*" = ["**"]
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/__pycache__/argparse.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/__pycache__/argparse.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 10860 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 6c2a 0000  o..........dl*..
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 3b2b 0000  o........E.d;+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6404 6407 6c0d  m.Z.m.Z...d.d.l.
-00000080: 6d0e 5a0e 0100 0902 6422 6423 640e 640f  m.Z.....d"d#d.d.
-00000090: 8405 5a0f 0902 0902 6424 6425 6413 6414  ..Z.....d$d%d.d.
+00000080: 6d0e 5a0e 0100 0902 6425 6426 640e 640f  m.Z.....d%d&d.d.
+00000090: 8405 5a0f 0902 0902 6427 6428 6413 6414  ..Z.....d'd(d.d.
 000000a0: 8405 5a10 4700 6415 6416 8400 6416 6502  ..Z.G.d.d...d.e.
 000000b0: 6a11 8303 5a12 6402 6417 6502 6a13 6603  j...Z.d.d.e.j.f.
-000000c0: 6426 641d 641e 8405 5a14 6507 6417 6602  d&d.d...Z.e.d.f.
-000000d0: 6427 6420 6421 8405 5a15 6402 5300 2928  d'd d!..Z.d.S.)(
+000000c0: 6429 641d 641e 8405 5a14 6507 6417 6602  d)d.d...Z.e.d.f.
+000000d0: 642a 6423 6424 8405 5a15 6402 5300 292b  d*d#d$..Z.d.S.)+
 000000e0: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
 000000f0: 696f 6e73 4e29 01da 0341 6e79 e901 0000  ionsN)...Any....
 00000100: 0029 01da 1444 4546 4155 4c54 5f43 4f4d  .)...DEFAULT_COM
 00000110: 4d41 4e44 5f4e 414d 4529 04da 0e41 7267  MAND_NAME)...Arg
 00000120: 756d 656e 7453 6368 656d 61da 0b43 6f6d  umentSchema..Com
 00000130: 6d61 6e64 4e61 6d65 da0d 436f 6d6d 616e  mandName..Comman
 00000140: 6453 6368 656d 61da 0c4f 7074 696f 6e53  dSchema..OptionS
@@ -383,88 +383,99 @@
 000017e0: 7472 4200 0000 2905 720b 0000 0072 4900  trB...).r....rI.
 000017f0: 0000 7237 0000 0072 3600 0000 da06 6b77  ..r7...r6.....kw
 00001800: 6172 6773 721d 0000 0072 1d00 0000 7222  argsr....r....r"
 00001810: 0000 00da 1061 6464 5f74 7569 5f61 7267  .....add_tui_arg
 00001820: 756d 656e 74f7 0000 0073 1a00 0000 0419  ument....s......
 00001830: 1c01 0a01 0601 0402 0201 0201 0201 0201  ................
 00001840: 0201 04fb 0206 0afa 7285 0000 00da 0763  ........r......c
-00001850: 6f6d 6d61 6e64 6303 0000 0000 0000 0000  ommandc.........
-00001860: 0000 0006 0000 0006 0000 0043 0000 0173  ...........C...s
-00001870: 5c00 0000 7c00 6a00 4400 5d0c 7d03 7401  \...|.j.D.].}.t.
-00001880: 7c03 7402 6a03 8302 720f 7c03 7d04 0100  |.t.j...r.|.}...
-00001890: 6e05 7103 7c00 a004 a100 7d04 7c04 6a05  n.q.|.....}.|.j.
-000018a0: 7c01 7402 6a06 7c02 6401 8d03 7d05 7c05  |.t.j.|.d...}.|.
-000018b0: 6a07 7c00 6402 8d01 0100 7408 7c05 6403  j.|.d.....t.|.d.
-000018c0: 6701 6404 6405 6406 8d04 0100 6404 5300  g.d.d.d.....d.S.
-000018d0: 2907 6106 0200 000a 0a20 2020 2041 7267  ).a......    Arg
-000018e0: 733a 0a20 2020 2020 2020 2070 6172 7365  s:.        parse
-000018f0: 723a 2074 6865 2061 7267 7061 7273 6520  r: the argparse 
-00001900: 7061 7273 6572 0a20 2020 2020 2020 2063  parser.        c
-00001910: 6f6d 6d61 6e64 3a20 6e61 6d65 206f 6620  ommand: name of 
-00001920: 7468 6520 434c 4920 636f 6d6d 616e 6420  the CLI command 
-00001930: 7468 6174 2077 696c 6c20 696e 766f 6b65  that will invoke
-00001940: 2074 6865 2054 5549 2028 6465 6661 756c   the TUI (defaul
-00001950: 743d 6074 7569 6029 0a20 2020 2020 2020  t=`tui`).       
-00001960: 2068 656c 703a 2068 656c 7020 6d65 7373   help: help mess
-00001970: 6167 6520 666f 7220 7468 6520 6172 6775  age for the argu
-00001980: 6d65 6e74 0a0a 2020 2020 4578 616d 706c  ment..    Exampl
-00001990: 6573 3a0a 2020 2020 2020 2020 3e3e 3e20  es:.        >>> 
-000019a0: 696d 706f 7274 2061 7267 7061 7273 650a  import argparse.
-000019b0: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
-000019c0: 2061 7267 7061 7273 655f 7475 6920 696d   argparse_tui im
-000019d0: 706f 7274 2061 6464 5f74 7569 5f61 7267  port add_tui_arg
-000019e0: 756d 656e 740a 2020 2020 2020 2020 2e2e  ument.        ..
-000019f0: 2e0a 2020 2020 2020 2020 3e3e 3e20 7061  ..        >>> pa
-00001a00: 7273 6572 203d 2061 7267 7061 7273 652e  rser = argparse.
-00001a10: 4172 6775 6d65 6e74 5061 7273 6572 2829  ArgumentParser()
-00001a20: 0a20 2020 2020 2020 203e 3e3e 2073 7562  .        >>> sub
-00001a30: 7061 7273 6572 7320 3d20 7061 7273 6572  parsers = parser
-00001a40: 2e61 6464 5f73 7562 7061 7273 6572 7328  .add_subparsers(
-00001a50: 290a 2020 2020 2020 2020 2e2e 2e0a 2020  ).        ....  
-00001a60: 2020 2020 2020 3e3e 3e20 6164 645f 7475        >>> add_tu
-00001a70: 695f 636f 6d6d 616e 6428 7061 7273 6572  i_command(parser
-00001a80: 290a 2020 2020 2020 2020 2e2e 2e0a 2020  ).        ....  
-00001a90: 2020 2020 2020 3e3e 3e20 7061 7273 6572        >>> parser
-00001aa0: 2e70 7269 6e74 5f75 7361 6765 2829 0a20  .print_usage(). 
-00001ab0: 2020 2020 2020 2075 7361 6765 3a20 5f5f         usage: __
-00001ac0: 6d61 696e 5f5f 2e70 7920 5b2d 685d 207b  main__.py [-h] {
-00001ad0: 7475 697d 202e 2e2e 0a20 2020 2029 0272  tui} ....    ).r
-00001ae0: 3e00 0000 7237 0000 0029 0172 7300 0000  >...r7...).rs...
-00001af0: 5a0a 636d 645f 6669 6c74 6572 4e7a 0e43  Z.cmd_filterNz.C
-00001b00: 6f6d 6d61 6e64 2066 696c 7465 7229 0372  ommand filter).r
-00001b10: 4900 0000 7236 0000 0072 3700 0000 2909  I...r6...r7...).
-00001b20: 7240 0000 0072 4100 0000 7243 0000 0072  r@...rA...rC...r
-00001b30: 4500 0000 da0e 6164 645f 7375 6270 6172  E.....add_subpar
-00001b40: 7365 7273 da0a 6164 645f 7061 7273 6572  sers..add_parser
-00001b50: 7244 0000 00da 0c73 6574 5f64 6566 6175  rD.....set_defau
-00001b60: 6c74 7372 8500 0000 2906 720b 0000 0072  ltsr....).r....r
-00001b70: 8600 0000 7237 0000 0072 8100 0000 5a0a  ....r7...r....Z.
-00001b80: 7375 6270 6172 7365 7273 5a0a 7475 695f  subparsersZ.tui_
-00001b90: 7061 7273 6572 721d 0000 0072 1d00 0000  parserr....r....
-00001ba0: 7222 0000 00da 0f61 6464 5f74 7569 5f63  r".....add_tui_c
-00001bb0: 6f6d 6d61 6e64 1f01 0000 7324 0000 000a  ommand....s$....
-00001bc0: 1a0c 0104 0104 0102 fe08 0404 0202 0104  ................
-00001bd0: 0102 0106 fd0c 0502 0202 0104 0102 0102  ................
-00001be0: 010a fc72 8a00 0000 725f 0000 0029 0672  ...r....r_...).r
-00001bf0: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
-00001c00: 0000 0072 0f00 0000 7210 0000 0029 024e  ...r....r....).N
-00001c10: 4e29 0672 0b00 0000 720c 0000 0072 0d00  N).r....r....r..
-00001c20: 0000 7262 0000 0072 6300 0000 7264 0000  ..rb...rc...rd..
-00001c30: 0029 0872 0b00 0000 720c 0000 0072 4900  .).r....r....rI.
-00001c40: 0000 727d 0000 0072 3700 0000 7253 0000  ..r}...r7...rS..
-00001c50: 0072 0f00 0000 727e 0000 0029 0872 0b00  .r....r~...).r..
-00001c60: 0000 720c 0000 0072 8600 0000 7253 0000  ..r....r....rS..
-00001c70: 0072 3700 0000 7253 0000 0072 0f00 0000  .r7...rS...r....
-00001c80: 727e 0000 0029 16da 0a5f 5f66 7574 7572  r~...)...__futur
-00001c90: 655f 5f72 0200 0000 7243 0000 0072 4d00  e__r....rC...rM.
-00001ca0: 0000 da06 7479 7069 6e67 7203 0000 00da  ....typingr.....
-00001cb0: 0963 6f6e 7374 616e 7473 7205 0000 005a  .constantsr....Z
-00001cc0: 0773 6368 656d 6173 7206 0000 0072 0700  .schemasr....r..
-00001cd0: 0000 7208 0000 0072 0900 0000 da03 7475  ..r....r......tu
-00001ce0: 6972 0a00 0000 7261 0000 0072 6700 0000  ir....ra...rg...
-00001cf0: da06 4163 7469 6f6e 7242 0000 0072 4400  ..ActionrB...rD.
-00001d00: 0000 7285 0000 0072 8a00 0000 721d 0000  ..r....r....r...
-00001d10: 0072 1d00 0000 721d 0000 0072 2200 0000  .r....r....r"...
-00001d20: da08 3c6d 6f64 756c 653e 0100 0000 732a  ..<module>....s*
-00001d30: 0000 000c 0008 0208 010c 010c 0218 010c  ................
-00001d40: 0102 050c fe00 7f02 2502 010c fd12 1a02  ........%.......
-00001d50: 3102 0104 010c fc02 2a02 0110 fd         1.......*....
+00001850: 6f6d 6d61 6e64 7284 0000 0072 0300 0000  ommandr....r....
+00001860: fa1a 6172 6770 6172 7365 2e5f 5375 6250  ..argparse._SubP
+00001870: 6172 7365 7273 4163 7469 6f6e 6303 0000  arsersActionc...
+00001880: 0000 0000 0000 0000 0007 0000 0006 0000  ................
+00001890: 004b 0000 0173 7000 0000 7c00 6a00 6401  .K...sp...|.j.d.
+000018a0: 7500 720e 7c00 6a01 6407 6900 7c03 a401  u.r.|.j.d.i.|...
+000018b0: 8e01 7d04 6e10 7c00 6a02 4400 5d0c 7d05  ..}.n.|.j.D.].}.
+000018c0: 7403 7c05 7404 6a05 8302 721d 7c05 7d04  t.|.t.j...r.|.}.
+000018d0: 0100 6e01 7111 7c04 6a06 7c01 7404 6a07  ..n.q.|.j.|.t.j.
+000018e0: 7c02 6402 8d03 7d06 7c06 6a08 7c00 6403  |.d...}.|.j.|.d.
+000018f0: 8d01 0100 7409 7c06 6404 6701 6401 6405  ....t.|.d.g.d.d.
+00001900: 6406 8d04 0100 7c04 5300 2908 615a 0200  d.....|.S.).aZ..
+00001910: 000a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00001920: 2020 2020 2070 6172 7365 723a 2074 6865       parser: the
+00001930: 2061 7267 7061 7273 6520 7061 7273 6572   argparse parser
+00001940: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+00001950: 3a20 6e61 6d65 206f 6620 7468 6520 434c  : name of the CL
+00001960: 4920 636f 6d6d 616e 6420 7468 6174 2077  I command that w
+00001970: 696c 6c20 696e 766f 6b65 2074 6865 2054  ill invoke the T
+00001980: 5549 2028 6465 6661 756c 743d 6074 7569  UI (default=`tui
+00001990: 6029 0a20 2020 2020 2020 2068 656c 703a  `).        help:
+000019a0: 2068 656c 7020 6d65 7373 6167 6520 666f   help message fo
+000019b0: 7220 7468 6520 6172 6775 6d65 6e74 0a20  r the argument. 
+000019c0: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+000019d0: 2069 6620 7375 6270 6172 7365 7273 2064   if subparsers d
+000019e0: 6f20 6e6f 7420 616c 7265 6164 7920 6578  o not already ex
+000019f0: 6973 742c 2063 7265 6174 6520 7769 7468  ist, create with
+00001a00: 2074 6865 7365 206b 7761 7267 732e 0a0a   these kwargs...
+00001a10: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
+00001a20: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
+00001a30: 2061 7267 7061 7273 650a 2020 2020 2020   argparse.      
+00001a40: 2020 3e3e 3e20 6672 6f6d 2061 7267 7061    >>> from argpa
+00001a50: 7273 655f 7475 6920 696d 706f 7274 2061  rse_tui import a
+00001a60: 6464 5f74 7569 5f61 7267 756d 656e 740a  dd_tui_argument.
+00001a70: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00001a80: 2020 2020 3e3e 3e20 7061 7273 6572 203d      >>> parser =
+00001a90: 2061 7267 7061 7273 652e 4172 6775 6d65   argparse.Argume
+00001aa0: 6e74 5061 7273 6572 2829 0a20 2020 2020  ntParser().     
+00001ab0: 2020 203e 3e3e 2073 7562 7061 7273 6572     >>> subparser
+00001ac0: 7320 3d20 7061 7273 6572 2e61 6464 5f73  s = parser.add_s
+00001ad0: 7562 7061 7273 6572 7328 290a 2020 2020  ubparsers().    
+00001ae0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00001af0: 3e3e 3e20 5f20 3d20 6164 645f 7475 695f  >>> _ = add_tui_
+00001b00: 636f 6d6d 616e 6428 7061 7273 6572 290a  command(parser).
+00001b10: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00001b20: 2020 2020 3e3e 3e20 7061 7273 6572 2e70      >>> parser.p
+00001b30: 7269 6e74 5f75 7361 6765 2829 0a20 2020  rint_usage().   
+00001b40: 2020 2020 2075 7361 6765 3a20 5f5f 6d61       usage: __ma
+00001b50: 696e 5f5f 2e70 7920 5b2d 685d 207b 7475  in__.py [-h] {tu
+00001b60: 697d 202e 2e2e 0a20 2020 204e 2902 723e  i} ....    N).r>
+00001b70: 0000 0072 3700 0000 2901 7273 0000 005a  ...r7...).rs...Z
+00001b80: 0a63 6d64 5f66 696c 7465 727a 0e43 6f6d  .cmd_filterz.Com
+00001b90: 6d61 6e64 2066 696c 7465 7229 0372 4900  mand filter).rI.
+00001ba0: 0000 7236 0000 0072 3700 0000 721d 0000  ..r6...r7...r...
+00001bb0: 0029 0ada 0b5f 7375 6270 6172 7365 7273  .)..._subparsers
+00001bc0: da0e 6164 645f 7375 6270 6172 7365 7273  ..add_subparsers
+00001bd0: 7240 0000 0072 4100 0000 7243 0000 0072  r@...rA...rC...r
+00001be0: 4500 0000 da0a 6164 645f 7061 7273 6572  E.....add_parser
+00001bf0: 7244 0000 00da 0c73 6574 5f64 6566 6175  rD.....set_defau
+00001c00: 6c74 7372 8500 0000 2907 720b 0000 0072  ltsr....).r....r
+00001c10: 8600 0000 7237 0000 0072 8400 0000 5a0a  ....r7...r....Z.
+00001c20: 7375 6270 6172 7365 7273 7281 0000 005a  subparsersr....Z
+00001c30: 0a74 7569 5f70 6172 7365 7272 1d00 0000  .tui_parserr....
+00001c40: 721d 0000 0072 2200 0000 da0f 6164 645f  r....r".....add_
+00001c50: 7475 695f 636f 6d6d 616e 641f 0100 0073  tui_command....s
+00001c60: 2800 0000 0a1c 1201 0a02 0c01 0401 0401  (...............
+00001c70: 02fe 0404 0201 0401 0201 06fd 0c05 0202  ................
+00001c80: 0201 0401 0201 0201 06fc 0407 728c 0000  ............r...
+00001c90: 0072 5f00 0000 2906 720b 0000 0072 0c00  .r_...).r....r..
+00001ca0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00001cb0: 0072 1000 0000 2902 4e4e 2906 720b 0000  .r....).NN).r...
+00001cc0: 0072 0c00 0000 720d 0000 0072 6200 0000  .r....r....rb...
+00001cd0: 7263 0000 0072 6400 0000 2908 720b 0000  rc...rd...).r...
+00001ce0: 0072 0c00 0000 7249 0000 0072 7d00 0000  .r....rI...r}...
+00001cf0: 7237 0000 0072 5300 0000 720f 0000 0072  r7...rS...r....r
+00001d00: 7e00 0000 290a 720b 0000 0072 0c00 0000  ~...).r....r....
+00001d10: 7286 0000 0072 5300 0000 7237 0000 0072  r....rS...r7...r
+00001d20: 5300 0000 7284 0000 0072 0300 0000 720f  S...r....r....r.
+00001d30: 0000 0072 8700 0000 2916 da0a 5f5f 6675  ...r....)...__fu
+00001d40: 7475 7265 5f5f 7202 0000 0072 4300 0000  ture__r....rC...
+00001d50: 724d 0000 00da 0674 7970 696e 6772 0300  rM.....typingr..
+00001d60: 0000 da09 636f 6e73 7461 6e74 7372 0500  ....constantsr..
+00001d70: 0000 5a07 7363 6865 6d61 7372 0600 0000  ..Z.schemasr....
+00001d80: 7207 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
+00001d90: 0374 7569 720a 0000 0072 6100 0000 7267  .tuir....ra...rg
+00001da0: 0000 00da 0641 6374 696f 6e72 4200 0000  .....ActionrB...
+00001db0: 7244 0000 0072 8500 0000 728c 0000 0072  rD...r....r....r
+00001dc0: 1d00 0000 721d 0000 0072 1d00 0000 7222  ....r....r....r"
+00001dd0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001de0: 0073 2a00 0000 0c00 0802 0801 0c01 0c02  .s*.............
+00001df0: 1801 0c01 0205 0cfe 007f 0225 0201 0cfd  ...........%....
+00001e00: 121a 0231 0201 0401 0cfc 022a 0201 10fd  ...1.......*....
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 1740 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 cc06 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 cc06 0000  o........E.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 640b 6405 6406 8404 5a05 6402 6504  Z.d.d.d...Z.d.e.
 00000060: 6a06 6407 1900 6602 640c 6409 640a 8405  j.d...f.d.d.d...
 00000070: 5a07 6402 5300 290d e900 0000 0029 01da  Z.d.S.)......)..
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/__pycache__/run_command.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/__pycache__/run_command.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 10938 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 ba2a 0000  o..........d.*..
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 ba2a 0000  o........E.d.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 c400 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 5a02 6400 6402 6c03 5a03 6400 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 6d05 5a05 0100 6400 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 0100 6400 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 0100 6400 6406 6c0c 6d0d  Z.m.Z...d.d.l.m.
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/__pycache__/schemas.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/__pycache__/schemas.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 3736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 980e 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 980e 0000  o........E.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6406 6407 8400 5a0d 6504  m.Z...d.d...Z.e.
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/__pycache__/tui.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/__pycache__/tui.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 12743 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 c731 0000  o..........d.1..
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 4732 0000  o........E.dG2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 a401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
@@ -181,556 +181,562 @@
 00000b40: 800c 0110 0206 010a 011a 010a 0202 020a  ................
 00000b50: 0102 0102 0106 fd06 050a 0306 0406 020c  ................
 00000b60: 020c 0106 0116 011c fe02 0406 0102 0106  ................
 00000b70: fe06 0406 0102 0102 010a 0102 0104 fe02  ................
 00000b80: 080a f71c f50c 177a 1643 6f6d 6d61 6e64  .......z.Command
 00000b90: 4275 696c 6465 722e 636f 6d70 6f73 65da  Builder.compose.
 00000ba0: 044e 6f6e 6563 0100 0000 0000 0000 0000  .Nonec..........
-00000bb0: 0000 0100 0000 0200 0000 4300 0001 7332  ..........C...s2
-00000bc0: 0000 007c 006a 00a0 01a1 007c 006a 025f  ...|.j.....|.j._
-00000bd0: 037c 006a 00a0 04a1 007c 006a 025f 0564  .|.j.....|.j._.d
-00000be0: 017c 006a 025f 067c 006a 02a0 07a1 0001  .|.j._.|.j......
-00000bf0: 0064 0053 00a9 024e 5429 0872 4200 0000  .d.S...NT).rB...
-00000c00: da0d 746f 5f63 6c69 5f73 7472 696e 67da  ..to_cli_string.
-00000c10: 0361 7070 da19 706f 7374 5f72 756e 5f63  .app..post_run_c
-00000c20: 6f6d 6d61 6e64 5f72 6564 6163 7465 64da  ommand_redacted.
-00000c30: 0b74 6f5f 636c 695f 6172 6773 da10 706f  .to_cli_args..po
-00000c40: 7374 5f72 756e 5f63 6f6d 6d61 6e64 da0f  st_run_command..
-00000c50: 6578 6563 7574 655f 6f6e 5f65 7869 7472  execute_on_exitr
-00000c60: 3200 0000 a901 7245 0000 0072 4800 0000  2.....rE...rH...
-00000c70: 7248 0000 0072 4900 0000 da14 6163 7469  rH...rI.....acti
-00000c80: 6f6e 5f63 6c6f 7365 5f61 6e64 5f72 756e  on_close_and_run
-00000c90: 7e00 0000 7308 0000 000e 010e 0108 010e  ~...s...........
-00000ca0: 017a 2343 6f6d 6d61 6e64 4275 696c 6465  .z#CommandBuilde
-00000cb0: 722e 6163 7469 6f6e 5f63 6c6f 7365 5f61  r.action_close_a
-00000cc0: 6e64 5f72 756e 6301 0000 0000 0000 0000  nd_runc.........
-00000cd0: 0000 0002 0000 0009 0000 0043 0000 0173  ...........C...s
-00000ce0: 6000 0000 7400 6a01 6401 6b02 7208 6402  `...t.j.d.k.r.d.
-00000cf0: 6701 6e0b 7400 6a01 6403 6b02 7210 6404  g.n.t.j.d.k.r.d.
-00000d00: 6701 6e03 6700 6405 a201 7d01 7402 7c01  g.n.g.d...}.t.|.
-00000d10: 7c00 6a03 6406 1700 6406 a004 6407 6408  |.j.d...d...d.d.
-00000d20: 8400 7c00 6a05 6a06 6409 640a 8d01 4400  ..|.j.j.d.d...D.
-00000d30: 8301 a101 1700 6409 640b 640c 8d04 0100  ......d.d.d.....
-00000d40: 6400 5300 290d 4eda 0577 696e 3332 da04  d.S.).N..win32..
-00000d50: 636f 7079 da06 6461 7277 696e 5a06 7062  copy..darwinZ.pb
-00000d60: 636f 7079 2903 5a05 7863 6c69 707a 0a2d  copy).Z.xclipz.-
-00000d70: 7365 6c65 6374 696f 6e5a 0963 6c69 7062  selectionZ.clipb
-00000d80: 6f61 7264 da01 2063 0100 0000 0000 0000  oard.. c........
-00000d90: 0000 0000 0200 0000 0500 0000 7300 0001  ............s...
-00000da0: 731e 0000 0081 007c 005d 0a7d 0174 00a0  s......|.].}.t..
-00000db0: 0174 027c 0183 01a1 0156 0001 0071 0264  .t.|.....V...q.d
-00000dc0: 0053 0072 3f00 0000 2903 da05 7368 6c65  .S.r?...)...shle
-00000dd0: 78da 0571 756f 7465 7237 0000 00a9 02da  x..quoter7......
-00000de0: 022e 30da 0178 7248 0000 0072 4800 0000  ..0..xrH...rH...
-00000df0: 7249 0000 00da 093c 6765 6e65 7870 723e  rI.....<genexpr>
-00000e00: 9200 0000 730a 0000 0002 8004 0002 020c  ....s...........
-00000e10: ff0a ff7a 3c43 6f6d 6d61 6e64 4275 696c  ...z<CommandBuil
-00000e20: 6465 722e 6163 7469 6f6e 5f63 6f70 795f  der.action_copy_
-00000e30: 636f 6d6d 616e 645f 7374 7269 6e67 2e3c  command_string.<
-00000e40: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-00000e50: 3e54 2901 5a0d 7265 6461 6374 5f73 6563  >T).Z.redact_sec
-00000e60: 7265 7446 2903 da05 696e 7075 74da 0474  retF)...input..t
-00000e70: 6578 74da 0563 6865 636b 2907 da03 7379  ext..check)...sy
-00000e80: 73da 0870 6c61 7466 6f72 6d72 0700 0000  s..platformr....
-00000e90: 7236 0000 00da 046a 6f69 6e72 4200 0000  r6.....joinrB...
-00000ea0: 725d 0000 0029 0272 4500 0000 da03 636d  r]...).rE.....cm
-00000eb0: 6472 4800 0000 7248 0000 0072 4900 0000  drH...rH...rI...
-00000ec0: da1a 6163 7469 6f6e 5f63 6f70 795f 636f  ..action_copy_co
-00000ed0: 6d6d 616e 645f 7374 7269 6e67 8400 0000  mmand_string....
-00000ee0: 7324 0000 000a 0306 ff0a 0306 ff06 0202  s$..............
-00000ef0: fb02 0902 0104 0102 0102 ff0a 020c 0206  ................
-00000f00: fe02 fe02 0602 010a f77a 2943 6f6d 6d61  .........z)Comma
-00000f10: 6e64 4275 696c 6465 722e 6163 7469 6f6e  ndBuilder.action
-00000f20: 5f63 6f70 795f 636f 6d6d 616e 645f 7374  _copy_command_st
-00000f30: 7269 6e67 6301 0000 0000 0000 0000 0000  ringc...........
-00000f40: 0001 0000 0002 0000 0043 0000 0173 0e00  .........C...s..
-00000f50: 0000 7c00 6a00 a001 a100 0100 6400 5300  ..|.j.......d.S.
-00000f60: 723f 0000 0029 0272 5b00 0000 7232 0000  r?...).r[...r2..
-00000f70: 0072 6000 0000 7248 0000 0072 4800 0000  .r`...rH...rH...
-00000f80: 7249 0000 00da 0b61 6374 696f 6e5f 6578  rI.....action_ex
-00000f90: 6974 9a00 0000 7302 0000 000e 017a 1a43  it....s......z.C
-00000fa0: 6f6d 6d61 6e64 4275 696c 6465 722e 6163  ommandBuilder.ac
-00000fb0: 7469 6f6e 5f65 7869 7463 0100 0000 0000  tion_exitc......
-00000fc0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000fd0: 0001 731e 0000 0064 0164 026c 006d 017d  ..s....d.d.l.m.}
-00000fe0: 0101 007c 006a 02a0 037c 0183 00a1 0101  ...|.j...|......
-00000ff0: 0064 0053 0029 034e 721d 0000 0029 01da  .d.S.).Nr....)..
-00001000: 0b41 626f 7574 4469 616c 6f67 2904 5a0d  .AboutDialog).Z.
-00001010: 7769 6467 6574 732e 6162 6f75 7472 7500  widgets.aboutru.
-00001020: 0000 725b 0000 00da 0b70 7573 685f 7363  ..r[.....push_sc
-00001030: 7265 656e 2902 7245 0000 0072 7500 0000  reen).rE...ru...
-00001040: 7248 0000 0072 4800 0000 7249 0000 00da  rH...rH...rI....
-00001050: 0c61 6374 696f 6e5f 6162 6f75 749d 0000  .action_about...
-00001060: 0073 0400 0000 0c01 1202 7a1b 436f 6d6d  .s........z.Comm
-00001070: 616e 6442 7569 6c64 6572 2e61 6374 696f  andBuilder.actio
-00001080: 6e5f 6162 6f75 74da 0565 7665 6e74 fa0c  n_about..event..
-00001090: 6576 656e 7473 2e4d 6f75 6e74 6302 0000  events.Mountc...
-000010a0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-000010b0: 00c3 0000 0173 1400 0000 8101 7c00 a000  .....s......|...
-000010c0: a100 4900 6400 4800 0100 6400 5300 723f  ..I.d.H...d.S.r?
-000010d0: 0000 0029 01da 155f 7265 6672 6573 685f  ...)..._refresh_
-000010e0: 636f 6d6d 616e 645f 666f 726d a902 7245  command_form..rE
-000010f0: 0000 0072 7800 0000 7248 0000 0072 4800  ...rx...rH...rH.
-00001100: 0000 7249 0000 00da 086f 6e5f 6d6f 756e  ..rI.....on_moun
-00001110: 74a2 0000 0073 0400 0000 0280 1201 7a17  t....s........z.
-00001120: 436f 6d6d 616e 6442 7569 6c64 6572 2e6f  CommandBuilder.o
-00001130: 6e5f 6d6f 756e 74da 046e 6f64 65fa 1e54  n_mount..node..T
-00001140: 7265 654e 6f64 655b 436f 6d6d 616e 6453  reeNode[CommandS
-00001150: 6368 656d 615d 207c 204e 6f6e 6563 0200  chema] | Nonec..
-00001160: 0000 0000 0000 0000 0000 0300 0000 0800  ................
-00001170: 0000 c300 0001 736a 0000 0081 017c 0164  ......sj.....|.d
-00001180: 0075 0072 1a7a 0a7c 00a0 0074 01a1 017d  .u.r.z.|...t...}
-00001190: 027c 026a 027d 0157 006e 0a04 0074 0379  .|.j.}.W.n...t.y
-000011a0: 1901 0001 0001 0059 0064 0053 0077 007c  .......Y.d.S.w.|
-000011b0: 016a 047c 005f 057c 00a0 067c 01a1 0101  .j.|._.|...|....
-000011c0: 007c 00a0 077c 006a 057c 006a 08a1 0201  .|...|.j.|.j....
-000011d0: 007c 00a0 097c 01a1 0149 0064 0048 0001  .|...|...I.d.H..
-000011e0: 0064 0053 0072 3f00 0000 290a da09 7175  .d.S.r?...)...qu
-000011f0: 6572 795f 6f6e 6572 2300 0000 5a0b 6375  ery_oner#...Z.cu
-00001200: 7273 6f72 5f6e 6f64 6572 1500 0000 da04  rsor_noder......
-00001210: 6461 7461 da17 7365 6c65 6374 6564 5f63  data..selected_c
-00001220: 6f6d 6d61 6e64 5f73 6368 656d 61da 1b5f  ommand_schema.._
-00001230: 7570 6461 7465 5f63 6f6d 6d61 6e64 5f64  update_command_d
-00001240: 6573 6372 6970 7469 6f6e da20 5f75 7064  escription. _upd
-00001250: 6174 655f 6578 6563 7574 696f 6e5f 7374  ate_execution_st
-00001260: 7269 6e67 5f70 7265 7669 6577 7242 0000  ring_previewrB..
-00001270: 00da 115f 7570 6461 7465 5f66 6f72 6d5f  ..._update_form_
-00001280: 626f 6479 2903 7245 0000 0072 7d00 0000  body).rE...r}...
-00001290: da0c 636f 6d6d 616e 645f 7472 6565 7248  ..command_treerH
-000012a0: 0000 0072 4800 0000 7249 0000 0072 7a00  ...rH...rI...rz.
-000012b0: 0000 a500 0000 731e 0000 0002 8008 0102  ......s.........
-000012c0: 010a 010a 010c 0106 0102 ff08 030a 0104  ................
-000012d0: 0104 0104 0104 fe14 047a 2443 6f6d 6d61  .........z$Comma
-000012e0: 6e64 4275 696c 6465 722e 5f72 6566 7265  ndBuilder._refre
-000012f0: 7368 5f63 6f6d 6d61 6e64 5f66 6f72 6dfa  sh_command_form.
-00001300: 2354 7265 652e 4e6f 6465 4869 6768 6c69  #Tree.NodeHighli
-00001310: 6768 7465 645b 436f 6d6d 616e 6453 6368  ghted[CommandSch
-00001320: 656d 615d 6302 0000 0000 0000 0000 0000  ema]c...........
-00001330: 0002 0000 0003 0000 00c3 0000 0173 1800  .............s..
-00001340: 0000 8101 7c00 a000 7c01 6a01 a101 4900  ....|...|.j...I.
-00001350: 6401 4800 0100 6401 5300 2902 7a92 5768  d.H...d.S.).z.Wh
-00001360: 656e 2077 6520 6869 6768 6c69 6768 7420  en we highlight 
-00001370: 6120 6e6f 6465 2069 6e20 7468 6520 436f  a node in the Co
-00001380: 6d6d 616e 6454 7265 652c 2074 6865 206d  mmandTree, the m
-00001390: 6169 6e20 626f 6479 206f 6620 7468 6520  ain body of the 
-000013a0: 686f 6d65 2070 6167 6520 7570 6461 7465  home page update
-000013b0: 730a 2020 2020 2020 2020 746f 2064 6973  s.        to dis
-000013c0: 706c 6179 2061 2066 6f72 6d20 7370 6563  play a form spec
-000013d0: 6966 6963 2074 6f20 7468 6520 6869 6768  ific to the high
-000013e0: 6c69 6768 7465 6420 636f 6d6d 616e 642e  lighted command.
-000013f0: 4e29 0272 7a00 0000 727d 0000 0072 7b00  N).rz...r}...r{.
-00001400: 0000 7248 0000 0072 4800 0000 7249 0000  ..rH...rH...rI..
-00001410: 00da 1873 656c 6563 7465 645f 636f 6d6d  ...selected_comm
-00001420: 616e 645f 6368 616e 6765 64b5 0000 0073  and_changed....s
-00001430: 0400 0000 0280 1607 7a27 436f 6d6d 616e  ........z'Comman
-00001440: 6442 7569 6c64 6572 2e73 656c 6563 7465  dBuilder.selecte
-00001450: 645f 636f 6d6d 616e 645f 6368 616e 6765  d_command_change
-00001460: 64fa 1343 6f6d 6d61 6e64 466f 726d 2e43  d..CommandForm.C
-00001470: 6861 6e67 6564 6302 0000 0000 0000 0000  hangedc.........
-00001480: 0000 0002 0000 0004 0000 0043 0000 0173  ...........C...s
-00001490: 1c00 0000 7c01 6a00 7c00 5f00 7c00 a001  ....|.j.|._.|...
-000014a0: 7c00 6a02 7c00 6a00 a102 0100 6400 5300  |.j.|.j.....d.S.
-000014b0: 723f 0000 0029 0372 4200 0000 7283 0000  r?...).rB...r...
-000014c0: 0072 8100 0000 727b 0000 0072 4800 0000  .r....r{...rH...
-000014d0: 7248 0000 0072 4900 0000 da13 7570 6461  rH...rI.....upda
-000014e0: 7465 5f63 6f6d 6d61 6e64 5f64 6174 61be  te_command_data.
-000014f0: 0000 0073 0a00 0000 0802 0401 0401 0401  ...s............
-00001500: 08fe 7a22 436f 6d6d 616e 6442 7569 6c64  ..z"CommandBuild
-00001510: 6572 2e75 7064 6174 655f 636f 6d6d 616e  er.update_comman
-00001520: 645f 6461 7461 fa17 5472 6565 4e6f 6465  d_data..TreeNode
-00001530: 5b43 6f6d 6d61 6e64 5363 6865 6d61 5d63  [CommandSchema]c
-00001540: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00001550: 0400 0000 4300 0001 734c 0000 007c 00a0  ....C...sL...|..
-00001560: 0064 0174 01a1 027d 027c 016a 026a 0370  .d.t...}.|.j.j.p
-00001570: 0b64 027d 037c 03a0 04a1 007d 0364 037c  .d.}.|.....}.d.|
-00001580: 006a 0572 177c 016a 066e 027c 006a 079b  .j.r.|.j.n.|.j..
-00001590: 0064 047c 039b 009d 047d 037c 02a0 087c  .d.|.....}.|...|
-000015a0: 03a1 0101 0064 0553 0029 067a 8455 7064  .....d.S.).z.Upd
-000015b0: 6174 6520 7468 6520 6465 7363 7269 7074  ate the descript
-000015c0: 696f 6e20 6f66 2074 6865 2063 6f6d 6d61  ion of the comma
-000015d0: 6e64 2061 7420 7468 6520 626f 7474 6f6d  nd at the bottom
-000015e0: 206f 6620 7468 6520 7369 6465 6261 720a   of the sidebar.
-000015f0: 2020 2020 2020 2020 6261 7365 6420 6f6e          based on
-00001600: 2074 6865 2063 7572 7265 6e74 6c79 2073   the currently s
-00001610: 656c 6563 7465 6420 6e6f 6465 2069 6e20  elected node in 
-00001620: 7468 6520 636f 6d6d 616e 6420 7472 6565  the command tree
-00001630: 2e7a 1923 686f 6d65 2d63 6f6d 6d61 6e64  .z.#home-command
-00001640: 2d64 6573 6372 6970 7469 6f6e 724f 0000  -descriptionrO..
-00001650: 007a 035b 625d 7a04 5b2f 5d0a 4e29 0972  .z.[b]z.[/].N).r
-00001660: 7f00 0000 721a 0000 0072 8000 0000 da09  ....r....r......
-00001670: 646f 6373 7472 696e 67da 066c 7374 7269  docstring..lstri
-00001680: 7072 3a00 0000 da05 6c61 6265 6c72 3600  pr:.....labelr6.
-00001690: 0000 da06 7570 6461 7465 2904 7245 0000  ....update).rE..
-000016a0: 0072 7d00 0000 5a0f 6465 7363 7269 7074  .r}...Z.descript
-000016b0: 696f 6e5f 626f 785a 1064 6573 6372 6970  ion_boxZ.descrip
-000016c0: 7469 6f6e 5f74 6578 7472 4800 0000 7248  tion_textrH...rH
-000016d0: 0000 0072 4900 0000 7282 0000 00c6 0000  ...rI...r.......
-000016e0: 0073 0a00 0000 0c03 0c01 0801 1e01 0e01  .s..............
-000016f0: 7a2a 436f 6d6d 616e 6442 7569 6c64 6572  z*CommandBuilder
-00001700: 2e5f 7570 6461 7465 5f63 6f6d 6d61 6e64  ._update_command
-00001710: 5f64 6573 6372 6970 7469 6f6e da0e 636f  _description..co
-00001720: 6d6d 616e 645f 7363 6865 6d61 7221 0000  mmand_schemar!..
-00001730: 0072 4200 0000 721f 0000 0063 0300 0000  .rB...r....c....
-00001740: 0000 0000 0000 0000 0900 0000 0600 0000  ................
-00001750: 4300 0001 7374 0000 007c 006a 0064 0175  C...st...|.j.d.u
-00001760: 0172 387c 00a0 0164 02a1 017d 0374 027c  .r8|...d...}.t.|
-00001770: 006a 039b 0064 039d 027c 0383 027d 047c  .j...d...|...}.|
-00001780: 02a0 04a1 007d 0574 02a0 057c 047c 00a0  .....}.t...|.|..
-00001790: 067c 05a1 01a1 027d 067c 00a0 0164 04a1  .|.....}.|...d..
-000017a0: 017d 0774 02a0 0564 057c 0766 027c 06a1  .}.t...d.|.f.|..
-000017b0: 027d 087c 00a0 0764 0674 08a1 02a0 097c  .}.|...d.t.....|
-000017c0: 08a1 0101 0064 0153 0064 0153 0029 077a  .....d.S.d.S.).z
-000017d0: 4055 7064 6174 6520 7468 6520 7072 6576  @Update the prev
-000017e0: 6965 7720 626f 7820 7368 6f77 696e 6720  iew box showing 
-000017f0: 7468 6520 636f 6d6d 616e 6420 7374 7269  the command stri
-00001800: 6e67 2074 6f20 6265 2065 7865 6375 7465  ng to be execute
-00001810: 644e 722a 0000 0072 6500 0000 722c 0000  dNr*...re...r,..
-00001820: 007a 0224 207a 1923 686f 6d65 2d65 7865  .z.$ z.#home-exe
-00001830: 632d 7072 6576 6965 772d 7374 6174 6963  c-preview-static
-00001840: 290a 7242 0000 0072 5000 0000 720b 0000  ).rB...rP...r...
-00001850: 0072 3600 0000 725a 0000 0072 5200 0000  .r6...rZ...rR...
-00001860: 7244 0000 0072 7f00 0000 721a 0000 0072  rD...r....r....r
-00001870: 8e00 0000 2909 7245 0000 0072 8f00 0000  ....).rE...r....
-00001880: 7242 0000 005a 1963 6f6d 6d61 6e64 5f6e  rB...Z.command_n
-00001890: 616d 655f 7379 6e74 6178 5f73 7479 6c65  ame_syntax_style
-000018a0: da06 7072 6566 6978 5a09 6e65 775f 7661  ..prefixZ.new_va
-000018b0: 6c75 655a 1568 6967 686c 6967 6874 6564  lueZ.highlighted
-000018c0: 5f6e 6577 5f76 616c 7565 5a0c 7072 6f6d  _new_valueZ.prom
-000018d0: 7074 5f73 7479 6c65 5a0e 7072 6576 6965  pt_styleZ.previe
-000018e0: 775f 7374 7269 6e67 7248 0000 0072 4800  w_stringrH...rH.
-000018f0: 0000 7249 0000 0072 8300 0000 cf00 0000  ..rI...r........
-00001900: 7316 0000 000a 0604 0102 0104 ff12 0308  s...............
-00001910: 0112 010a 0110 0116 0104 f77a 2f43 6f6d  ...........z/Com
-00001920: 6d61 6e64 4275 696c 6465 722e 5f75 7064  mandBuilder._upd
-00001930: 6174 655f 6578 6563 7574 696f 6e5f 7374  ate_execution_st
-00001940: 7269 6e67 5f70 7265 7669 6577 6302 0000  ring_previewc...
-00001950: 0000 0000 0000 0000 0006 0000 0004 0000  ................
-00001960: 00c3 0000 0173 6200 0000 8101 7c00 a000  .....sb.....|...
-00001970: 6401 7401 a102 7d02 7c02 6a02 4400 5d09  d.t...}.|.j.D.].
-00001980: 7d03 7c03 a003 a100 4900 6400 4800 0100  }.|.....I.d.H...
-00001990: 710a 7c01 6a04 7d04 7405 7c04 7c00 6a06  q.|.j.}.t.|.|.j.
-000019a0: 6402 8d02 7d05 7c02 a007 7c05 a101 4900  d...}.|...|...I.
-000019b0: 6400 4800 0100 7c00 6a08 732f 7c05 a009  d.H...|.j.s/|...
-000019c0: a100 0100 6400 5300 6400 5300 2903 4e7a  ....d.S.d.S.).Nz
-000019d0: 1123 686f 6d65 2d62 6f64 792d 7363 726f  .#home-body-scro
-000019e0: 6c6c 2902 728f 0000 0072 3400 0000 290a  ll).r....r4...).
-000019f0: 727f 0000 0072 1400 0000 da08 6368 696c  r....r......chil
-00001a00: 6472 656e da06 7265 6d6f 7665 7280 0000  dren..remover...
-00001a10: 0072 2400 0000 7234 0000 005a 056d 6f75  .r$...r4...Z.mou
-00001a20: 6e74 723a 0000 0072 5300 0000 2906 7245  ntr:...rS...).rE
-00001a30: 0000 0072 7d00 0000 da06 7061 7265 6e74  ...r}.....parent
-00001a40: da05 6368 696c 6472 8f00 0000 5a0c 636f  ..childr....Z.co
-00001a50: 6d6d 616e 645f 666f 726d 7248 0000 0072  mmand_formrH...r
-00001a60: 4800 0000 7249 0000 0072 8400 0000 e000  H...rI...r......
-00001a70: 0000 731a 0000 0002 800c 020a 0110 0106  ..s.............
-00001a80: 0302 0102 0104 0106 fe10 0406 010c 0104  ................
-00001a90: ff7a 2043 6f6d 6d61 6e64 4275 696c 6465  .z CommandBuilde
-00001aa0: 722e 5f75 7064 6174 655f 666f 726d 5f62  r._update_form_b
-00001ab0: 6f64 7929 034e 4e4e 290e 7234 0000 0072  ody).NNN).r4...r
-00001ac0: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
-00001ad0: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
-00001ae0: 0000 723c 0000 0072 3900 0000 723d 0000  ..r<...r9...r=..
-00001af0: 0072 3900 0000 723e 0000 0072 3900 0000  .r9...r>...r9...
-00001b00: 2902 724a 0000 0072 1000 0000 a902 724a  ).rJ...r......rJ
-00001b10: 0000 0072 5800 0000 2904 7278 0000 0072  ...rX...).rx...r
-00001b20: 7900 0000 724a 0000 0072 5800 0000 723f  y...rJ...rX...r?
-00001b30: 0000 0029 0272 7d00 0000 727e 0000 0029  ...).r}...r~...)
-00001b40: 0472 7800 0000 7286 0000 0072 4a00 0000  .rx...r....rJ...
-00001b50: 7258 0000 0029 0472 7800 0000 7288 0000  rX...).rx...r...
-00001b60: 0072 4a00 0000 7258 0000 0029 0472 7d00  .rJ...rX...).r}.
-00001b70: 0000 728a 0000 0072 4a00 0000 7258 0000  ..r....rJ...rX..
-00001b80: 0029 0672 8f00 0000 7221 0000 0072 4200  .).r....r!...rB.
-00001b90: 0000 721f 0000 0072 4a00 0000 7258 0000  ..r....rJ...rX..
-00001ba0: 0029 19da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
-00001bb0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001bc0: 6c6e 616d 655f 5f5a 1143 4f4d 504f 4e45  lname__Z.COMPONE
-00001bd0: 4e54 5f43 4c41 5353 4553 7211 0000 005a  NT_CLASSESr....Z
-00001be0: 0842 494e 4449 4e47 5372 4100 0000 7257  .BINDINGSrA...rW
-00001bf0: 0000 0072 6100 0000 7273 0000 0072 7400  ...ra...rs...rt.
-00001c00: 0000 7277 0000 0072 7c00 0000 727a 0000  ..rw...r|...rz..
-00001c10: 0072 0d00 0000 721b 0000 005a 0f4e 6f64  .r....r....Z.Nod
-00001c20: 6548 6967 686c 6967 6874 6564 7287 0000  eHighlightedr...
-00001c30: 0072 2400 0000 5a07 4368 616e 6765 6472  .r$...Z.Changedr
-00001c40: 8900 0000 7282 0000 0072 8300 0000 7284  ....r....r....r.
-00001c50: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00001c60: 5f5f 7248 0000 0072 4800 0000 7246 0000  __rH...rH...rF..
-00001c70: 0072 4900 0000 7229 0000 0026 0000 0073  .rI...r)...&...s
-00001c80: 4000 0000 0800 0801 0c03 0c01 0201 0201  @...............
-00001c90: 0201 0201 04fd 0c05 0c01 0c01 0c01 04f5  ................
-00001ca0: 0214 0201 0201 10f8 0a14 0a33 0a06 0a16  ...........3....
-00001cb0: 0a03 0a05 0c03 0810 0c01 0808 0c01 0a07  ................
-00001cc0: 0a09 1211 7229 0000 0063 0000 0000 0000  ....r)...c......
-00001cd0: 0000 0000 0000 0000 0000 0500 0000 0000  ................
-00001ce0: 0001 7392 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
-00001cf0: 0365 0483 016a 0564 011b 005a 0609 0209  .e...j.d...Z....
-00001d00: 0264 2964 2a87 0066 0164 0b64 0c84 0d5a  .d)d*..f.d.d...Z
-00001d10: 0765 0864 2b64 1064 1184 0483 015a 0964  .e.d+d.d.....Z.d
-00001d20: 1264 1384 005a 0a65 0b65 0c6a 0d64 1483  .d...Z.e.e.j.d..
-00001d30: 0264 1564 1684 0083 015a 0e64 1764 0264  .d.d.....Z.d.d.d
-00001d40: 0264 189c 0364 2c87 0066 0164 1f64 2084  .d...d,..f.d.d .
-00001d50: 0e5a 0f64 2d64 2164 2284 045a 1064 2d64  .Z.d-d!d"..Z.d-d
-00001d60: 2364 2484 045a 1164 2e64 2764 2884 045a  #d$..Z.d.d'd(..Z
-00001d70: 1287 0004 005a 1353 0029 2fda 0354 7569  .....Z.S.)/..Tui
-00001d80: 7a08 7475 692e 7363 7373 4e72 3400 0000  z.tui.scssNr4...
-00001d90: 7235 0000 0072 3600 0000 7239 0000 0072  r5...r6...r9...r
-00001da0: 3800 0000 da0e 636f 6d6d 616e 645f 6669  8.....command_fi
-00001db0: 6c74 6572 724a 0000 0072 5800 0000 6305  lterrJ...rX...c.
-00001dc0: 0000 0000 0000 0000 0000 0007 0000 0008  ................
-00001dd0: 0000 0003 0000 0173 1201 0000 7400 8300  .......s....t...
-00001de0: a001 a100 0100 6700 7c00 5f02 6401 7c00  ......g.|._.d.|.
-00001df0: 5f03 7404 7c01 a005 a100 8301 6402 1900  _.t.|.......d...
-00001e00: 7d05 8800 7249 7c01 7c05 1900 6a06 7249  }...rI|.|...j.rI
-00001e10: 8700 6601 6403 6404 8408 7c01 7c05 1900  ..f.d.d...|.|...
-00001e20: 6a06 a007 a100 4400 8301 7d06 7408 7c06  j.....D...}.t.|.
-00001e30: 8301 6405 6b02 7244 7409 8700 6601 6406  ..d.k.rDt...f.d.
-00001e40: 6407 8408 6408 4400 8301 8301 7344 7c06  d...d.D.....sD|.
-00001e50: 7d01 7404 7c01 a005 a100 8301 6402 1900  }.t.|.......d...
-00001e60: 7d05 6e05 7c06 7c01 7c05 1900 5f06 7c01  }.n.|.|.|..._.|.
-00001e70: 7c00 5f0a 7409 6409 6407 8400 7c01 a00b  |._.t.d.d...|...
-00001e80: a100 4400 8301 8301 7c00 5f0c 640a 7c00  ..D.....|._.d.|.
-00001e90: 5f0d 7c02 725f 7c02 6e02 740e 8300 7c00  _.|.r_|.n.t...|.
-00001ea0: 5f0f 7c03 7c00 5f10 7c00 6a10 7387 7411  _.|.|._.|.j.s.t.
-00001eb0: 7412 8301 8f10 0100 7413 a014 7c00 6a0f  t.......t...|.j.
-00001ec0: a101 7c00 5f10 5700 6400 0400 0400 8303  ..|._.W.d.......
-00001ed0: 0100 6400 5300 3100 7380 7701 0100 0100  ..d.S.1.s.w.....
-00001ee0: 0100 5900 0100 6400 5300 6400 5300 290b  ..Y...d.S.d.S.).
-00001ef0: 4e72 4f00 0000 7201 0000 0063 0100 0000  NrO...r....c....
-00001f00: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00001f10: 1300 0001 7320 0000 0069 007c 005d 0c5c  ....s ...i.|.].\
-00001f20: 027d 017d 0274 007c 0188 0083 0272 027c  .}.}.t.|.....r.|
-00001f30: 017c 0293 0271 0253 0072 4800 0000 7204  .|...q.S.rH...r.
-00001f40: 0000 0029 0372 6900 0000 da01 6b72 4e00  ...).ri.....krN.
-00001f50: 0000 a901 729b 0000 0072 4800 0000 7249  ....r....rH...rI
-00001f60: 0000 00da 0a3c 6469 6374 636f 6d70 3e02  .....<dictcomp>.
-00001f70: 0100 0073 0c00 0000 0600 0602 0801 02fd  ...s............
-00001f80: 0401 06ff 7a20 5475 692e 5f5f 696e 6974  ....z Tui.__init
-00001f90: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  __.<locals>.<dic
-00001fa0: 7463 6f6d 703e 721d 0000 0063 0100 0000  tcomp>r....c....
-00001fb0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001fc0: 3300 0001 7318 0000 0081 007c 005d 077d  3...s......|.].}
-00001fd0: 017c 0188 0076 0056 0001 0071 0264 0053  .|...v.V...q.d.S
-00001fe0: 0072 3f00 0000 7248 0000 0072 6800 0000  .r?...rH...rh...
-00001ff0: 729d 0000 0072 4800 0000 7249 0000 0072  r....rH...rI...r
-00002000: 6b00 0000 0701 0000 7308 0000 0002 8004  k.......s.......
-00002010: 0008 010a ff7a 1f54 7569 2e5f 5f69 6e69  .....z.Tui.__ini
-00002020: 745f 5f2e 3c6c 6f63 616c 733e 2e3c 6765  t__.<locals>.<ge
-00002030: 6e65 7870 723e 2902 da01 2afa 013f 6301  nexpr>)...*..?c.
-00002040: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00002050: 0000 0073 0000 0173 1600 0000 8100 7c00  ...s...s......|.
-00002060: 5d06 7d01 7c01 6a00 5600 0100 7102 6400  ].}.|.j.V...q.d.
-00002070: 5300 723f 0000 0029 01da 0b73 7562 636f  S.r?...)...subco
-00002080: 6d6d 616e 6473 2902 7269 0000 0072 4e00  mmands).ri...rN.
-00002090: 0000 7248 0000 0072 4800 0000 7249 0000  ..rH...rH...rI..
-000020a0: 0072 6b00 0000 1101 0000 7304 0000 0002  .rk.......s.....
-000020b0: 8014 0046 2915 7240 0000 0072 4100 0000  ...F).r@...rA...
-000020c0: 725e 0000 0072 5c00 0000 da04 6c69 7374  r^...r\.....list
-000020d0: da04 6b65 7973 72a1 0000 00da 0569 7465  ..keysr......ite
-000020e0: 6d73 da03 6c65 6eda 0361 6e79 7234 0000  ms..len..anyr4..
-000020f0: 00da 0676 616c 7565 7372 3a00 0000 725f  ...valuesr:...r_
-00002100: 0000 0072 1e00 0000 7236 0000 0072 3800  ...r....r6...r8.
-00002110: 0000 7203 0000 00da 0945 7863 6570 7469  ..r......Excepti
-00002120: 6f6e 7228 0000 0072 4300 0000 2907 7245  onr(...rC...).rE
-00002130: 0000 0072 3400 0000 7236 0000 0072 3800  ...r4...r6...r8.
-00002140: 0000 729b 0000 00da 0d72 6f6f 745f 636d  ..r......root_cm
-00002150: 645f 6e61 6d65 5a10 6d61 7463 6869 6e67  d_nameZ.matching
-00002160: 5f73 6368 656d 6173 7246 0000 0072 9d00  _schemasrF...r..
-00002170: 0000 7249 0000 0072 4100 0000 f400 0000  ..rI...rA.......
-00002180: 7330 0000 000a 0706 0206 0110 020e 010a  s0..............
-00002190: 010c 0206 fe18 0502 0108 ff04 0312 010a  ................
-000021a0: 0306 0218 0106 0110 0206 0106 020a 0110  ................
-000021b0: 0122 ff04 ff7a 0c54 7569 2e5f 5f69 6e69  ."...z.Tui.__ini
-000021c0: 745f 5fda 0461 7267 7372 2100 0000 fa05  t__..argsr!.....
-000021d0: 2754 7569 2763 0100 0000 0000 0000 0000  'Tui'c..........
-000021e0: 0000 0600 0000 0400 0000 4f00 0001 7352  ..........O...sR
-000021f0: 0000 007c 0173 0674 0064 0183 0182 017c  ...|.s.t.d.....|
-00002200: 0164 0219 007d 037c 036a 017c 0369 017d  .d...}.|.j.|.i.}
-00002210: 047c 0164 0364 0085 0219 0044 005d 0b7d  .|.d.d.....D.].}
-00002220: 057c 037c 055f 027c 057c 036a 037c 056a  .|.|._.|.|.j.|.j
-00002230: 013c 0071 157c 007c 0466 0169 007c 02a4  .<.q.|.|.f.i.|..
-00002240: 018e 0153 0029 044e 7a14 4e6f 2073 6368  ...S.).Nz.No sch
-00002250: 656d 6173 2070 726f 7669 6465 642e 7201  emas provided.r.
-00002260: 0000 0072 1d00 0000 2904 da0a 5661 6c75  ...r....)...Valu
-00002270: 6545 7272 6f72 723c 0000 0072 9300 0000  eErrorr<...r....
-00002280: 72a1 0000 0029 06da 0363 6c73 72aa 0000  r....)...clsr...
-00002290: 00da 066b 7761 7267 735a 0b72 6f6f 745f  ...kwargsZ.root_
-000022a0: 7363 6865 6d61 da07 7363 6865 6d61 735a  schema..schemasZ
-000022b0: 0673 6368 656d 6172 4800 0000 7248 0000  .schemarH...rH..
-000022c0: 0072 4900 0000 da0c 6672 6f6d 5f73 6368  .rI.....from_sch
-000022d0: 656d 6173 1b01 0000 7310 0000 0004 0208  emas....s.......
-000022e0: 0108 020a 0210 0206 010e 0110 027a 1054  .............z.T
-000022f0: 7569 2e66 726f 6d5f 7363 6865 6d61 7363  ui.from_schemasc
-00002300: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002310: 0800 0000 4300 0001 7322 0000 007c 00a0  ....C...s"...|..
-00002320: 0074 017c 006a 027c 006a 037c 006a 047c  .t.|.j.|.j.|.j.|
-00002330: 006a 0564 018d 04a1 0101 0064 0053 0029  .j.d.......d.S.)
-00002340: 024e 2903 7236 0000 0072 3800 0000 723a  .N).r6...r8...r:
-00002350: 0000 0029 0672 7600 0000 7229 0000 0072  ...).rv...r)...r
-00002360: 3400 0000 7236 0000 0072 3800 0000 723a  4...r6...r8...r:
-00002370: 0000 0072 6000 0000 7248 0000 0072 4800  ...r`...rH...rH.
-00002380: 0000 7249 0000 0072 7c00 0000 2a01 0000  ..rI...r|...*...
-00002390: 7310 0000 0004 0102 0104 0104 0104 0104  s...............
-000023a0: 0104 fc08 ff7a 0c54 7569 2e6f 6e5f 6d6f  .....z.Tui.on_mo
-000023b0: 756e 747a 1123 686f 6d65 2d65 7865 632d  untz.#home-exec-
-000023c0: 6275 7474 6f6e 6301 0000 0000 0000 0000  buttonc.........
-000023d0: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-000023e0: 1200 0000 6401 7c00 5f00 7c00 a001 a100  ....d.|._.|.....
-000023f0: 0100 6400 5300 7259 0000 0029 0272 5f00  ..d.S.rY...).r_.
-00002400: 0000 7232 0000 0072 6000 0000 7248 0000  ..r2...r`...rH..
-00002410: 0072 4800 0000 7249 0000 00da 116f 6e5f  .rH...rI.....on_
-00002420: 6275 7474 6f6e 5f70 7265 7373 6564 3401  button_pressed4.
-00002430: 0000 7304 0000 0006 020c 017a 1554 7569  ..s........z.Tui
-00002440: 2e6f 6e5f 6275 7474 6f6e 5f70 7265 7373  .on_button_press
-00002450: 6564 46a9 03da 0868 6561 646c 6573 73da  edF....headless.
-00002460: 0473 697a 65da 0a61 7574 6f5f 7069 6c6f  .size..auto_pilo
-00002470: 7472 b300 0000 723b 0000 0072 b400 0000  tr....r;...r....
-00002480: fa16 7475 706c 655b 696e 742c 2069 6e74  ..tuple[int, int
-00002490: 5d20 7c20 4e6f 6e65 72b5 0000 00fa 1c41  ] | Noner......A
-000024a0: 7574 6f70 696c 6f74 4361 6c6c 6261 636b  utopilotCallback
-000024b0: 5479 7065 207c 204e 6f6e 6563 0100 0000  Type | Nonec....
-000024c0: 0000 0000 0300 0000 0900 0000 0d00 0000  ................
-000024d0: 0300 0001 7342 0100 007a 5774 0083 006a  ....sB...zWt...j
-000024e0: 017c 017c 027c 0364 018d 0301 0057 007c  .|.|.|.d.....W.|
-000024f0: 006a 0272 5274 0383 007d 047c 006a 0272  .j.rRt...}.|.j.r
-00002500: 547c 006a 0472 567c 04a0 0564 027c 006a  T|.j.rV|...d.|.j
-00002510: 069b 0064 037c 006a 079b 0064 049d 05a1  ...d.|.j...d....
-00002520: 0101 0074 08a0 097c 006a 06a1 017d 057c  ...t...|.j...}.|
-00002530: 0564 0519 007d 0667 007c 05a2 017c 006a  .d...}.g.|...|.j
-00002540: 02a2 017d 0774 0a6a 0ba0 0ca1 007d 0874  ...}.t.j.....}.t
-00002550: 0a6a 0da0 0e74 0aa0 0fa1 007c 0864 0619  .j...t.....|.d..
-00002560: 0067 02a1 017c 0864 063c 0074 0aa0 107c  .g...|.d.<.t...|
-00002570: 067c 077c 08a1 0301 0064 0053 0064 0053  .|.|.....d.S.d.S
-00002580: 0064 0053 0064 0053 007c 006a 0272 9e74  .d.S.d.S.|.j.r.t
-00002590: 0383 007d 047c 006a 0272 9f7c 006a 0472  ...}.|.j.r.|.j.r
-000025a0: a07c 04a0 0564 027c 006a 069b 0064 037c  .|...d.|.j...d.|
-000025b0: 006a 079b 0064 049d 05a1 0101 0074 08a0  .j...d.......t..
-000025c0: 097c 006a 06a1 017d 057c 0564 0519 007d  .|.j...}.|.d...}
-000025d0: 0667 007c 05a2 017c 006a 02a2 017d 0774  .g.|...|.j...}.t
-000025e0: 0a6a 0ba0 0ca1 007d 0874 0a6a 0da0 0e74  .j.....}.t.j...t
-000025f0: 0aa0 0fa1 007c 0864 0619 0067 02a1 017c  .....|.d...g...|
-00002600: 0864 063c 0074 0aa0 107c 067c 077c 08a1  .d.<.t...|.|.|..
-00002610: 0301 0077 0077 0077 0077 0029 074e 72b2  ...w.w.w.w.).Nr.
-00002620: 0000 007a 1052 756e 6e69 6e67 205b 6220  ...z.Running [b 
-00002630: 6379 616e 5d72 6500 0000 7a03 5b2f 5d72  cyan]re...z.[/]r
-00002640: 0100 0000 da04 5041 5448 2911 7240 0000  ......PATH).r@..
-00002650: 0072 0700 0000 725e 0000 0072 0900 0000  .r....r^...r....
-00002660: 725f 0000 00da 0570 7269 6e74 7236 0000  r_.....printr6..
-00002670: 0072 5c00 0000 7266 0000 00da 0573 706c  .r\...rf.....spl
-00002680: 6974 da02 6f73 da07 656e 7669 726f 6e72  it..os..environr
-00002690: 6300 0000 da07 7061 7468 7365 7072 7100  c.....pathseprq.
-000026a0: 0000 da06 6765 7463 7764 da07 6578 6563  ....getcwd..exec
-000026b0: 7670 6529 0972 4500 0000 72b3 0000 0072  vpe).rE...r....r
-000026c0: b400 0000 72b5 0000 00da 0763 6f6e 736f  ....r......conso
-000026d0: 6c65 5a0e 7370 6c69 745f 6170 705f 6e61  leZ.split_app_na
-000026e0: 6d65 5a0c 7072 6f67 7261 6d5f 6e61 6d65  meZ.program_name
-000026f0: da09 6172 6775 6d65 6e74 73da 0365 6e76  ..arguments..env
-00002700: 7246 0000 0072 4800 0000 7249 0000 0072  rF...rH...rI...r
-00002710: 0700 0000 3901 0000 733c 0000 0002 0714  ....9...s<......
-00002720: 0106 0206 010c 0104 0114 0104 ff0c 0408  ................
-00002730: 010e 010a 021c 0112 0104 f308 0206 fe06  ................
-00002740: 010c 0104 0114 0104 ff0c 0408 010e 010a  ................
-00002750: 021c 0110 0102 f304 027a 0754 7569 2e72  .........z.Tui.r
-00002760: 756e 6301 0000 0000 0000 0000 0000 0002  unc.............
-00002770: 0000 0008 0000 0043 0000 0173 3000 0000  .......C...s0...
-00002780: 7a07 7c00 a000 7401 a101 7d01 5700 6e0a  z.|...t...}.W.n.
-00002790: 0400 7402 7911 0100 0100 0100 5900 6400  ..t.y.......Y.d.
-000027a0: 5300 7700 7c01 a003 a100 0100 6400 5300  S.w.|.......d.S.
-000027b0: 723f 0000 0029 0472 7f00 0000 7223 0000  r?...).r....r#..
-000027c0: 0072 1500 0000 7253 0000 0029 0272 4500  .r....rS...).rE.
-000027d0: 0000 7285 0000 0072 4800 0000 7248 0000  ..r....rH...rH..
-000027e0: 0072 4900 0000 da19 6163 7469 6f6e 5f66  .rI.....action_f
-000027f0: 6f63 7573 5f63 6f6d 6d61 6e64 5f74 7265  ocus_command_tre
-00002800: 6552 0100 0073 0c00 0000 0201 0e01 0c01  eR...s..........
-00002810: 0601 02ff 0c03 7a1d 5475 692e 6163 7469  ......z.Tui.acti
-00002820: 6f6e 5f66 6f63 7573 5f63 6f6d 6d61 6e64  on_focus_command
-00002830: 5f74 7265 6563 0100 0000 0000 0000 0000  _treec..........
-00002840: 0000 0200 0000 0400 0000 4300 0001 731e  ..........C...s.
-00002850: 0000 007c 00a0 0074 01a1 017d 017c 00a0  ...|...t...}.|..
-00002860: 0274 037c 016a 0483 01a1 0101 0064 0053  .t.|.j.......d.S
-00002870: 0072 3f00 0000 2905 727f 0000 0072 2900  .r?...).r....r).
-00002880: 0000 7276 0000 0072 2200 0000 7281 0000  ..rv...r"...r...
-00002890: 0029 0272 4500 0000 5a0f 636f 6d6d 616e  .).rE...Z.comman
-000028a0: 645f 6275 696c 6465 7272 4800 0000 7248  d_builderrH...rH
-000028b0: 0000 0072 4900 0000 da18 6163 7469 6f6e  ...rI.....action
-000028c0: 5f73 686f 775f 636f 6d6d 616e 645f 696e  _show_command_in
-000028d0: 666f 5a01 0000 7304 0000 000a 0114 017a  foZ...s........z
-000028e0: 1c54 7569 2e61 6374 696f 6e5f 7368 6f77  .Tui.action_show
-000028f0: 5f63 6f6d 6d61 6e64 5f69 6e66 6fda 0375  _command_info..u
-00002900: 726c 7237 0000 0063 0200 0000 0000 0000  rlr7...c........
-00002910: 0000 0000 0200 0000 0200 0000 4300 0001  ............C...
-00002920: 730c 0000 0074 007c 0183 0101 0064 0153  s....t.|.....d.S
-00002930: 0029 027a 6956 6973 6974 2074 6865 2067  .).ziVisit the g
-00002940: 6976 656e 2055 524c 2c20 7669 6120 7468  iven URL, via th
-00002950: 6520 6f70 6572 6174 696e 6720 7379 7374  e operating syst
-00002960: 656d 2e0a 0a20 2020 2020 2020 2041 7267  em...        Arg
-00002970: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
-00002980: 726c 3a20 5468 6520 5552 4c20 746f 2076  rl: The URL to v
-00002990: 6973 6974 2e0a 2020 2020 2020 2020 4e29  isit..        N)
-000029a0: 01da 086f 7065 6e5f 7572 6c29 0272 4500  ...open_url).rE.
-000029b0: 0000 72c5 0000 0072 4800 0000 7248 0000  ..r....rH...rH..
-000029c0: 0072 4900 0000 da0c 6163 7469 6f6e 5f76  .rI.....action_v
-000029d0: 6973 6974 5e01 0000 7302 0000 000c 067a  isit^...s......z
-000029e0: 1054 7569 2e61 6374 696f 6e5f 7669 7369  .Tui.action_visi
-000029f0: 7429 024e 4e29 0a72 3400 0000 7235 0000  t).NN).r4...r5..
-00002a00: 0072 3600 0000 7239 0000 0072 3800 0000  .r6...r9...r8...
-00002a10: 7239 0000 0072 9b00 0000 7239 0000 0072  r9...r....r9...r
-00002a20: 4a00 0000 7258 0000 0029 0472 aa00 0000  J...rX...).r....
-00002a30: 7221 0000 0072 4a00 0000 72ab 0000 0029  r!...rJ...r....)
-00002a40: 0872 b300 0000 723b 0000 0072 b400 0000  .r....r;...r....
-00002a50: 72b6 0000 0072 b500 0000 72b7 0000 0072  r....r....r....r
-00002a60: 4a00 0000 7258 0000 0072 9500 0000 2904  J...rX...r....).
-00002a70: 72c5 0000 0072 3700 0000 724a 0000 0072  r....r7...rJ...r
-00002a80: 5800 0000 2914 7296 0000 0072 9700 0000  X...).r....r....
-00002a90: 7298 0000 0072 0600 0000 da08 5f5f 6669  r....r......__fi
-00002aa0: 6c65 5f5f 7293 0000 005a 0843 5353 5f50  le__r....Z.CSS_P
-00002ab0: 4154 4872 4100 0000 da0b 636c 6173 736d  ATHrA.....classm
-00002ac0: 6574 686f 6472 b000 0000 727c 0000 0072  ethodr....r|...r
-00002ad0: 0d00 0000 7217 0000 005a 0750 7265 7373  ....r....Z.Press
-00002ae0: 6564 72b1 0000 0072 0700 0000 72c3 0000  edr....r....r...
-00002af0: 0072 c400 0000 72c7 0000 0072 9900 0000  .r....r....r....
-00002b00: 7248 0000 0072 4800 0000 7246 0000 0072  rH...rH...rF...r
-00002b10: 4900 0000 729a 0000 00f1 0000 0073 2200  I...r........s".
-00002b20: 0000 0800 0e01 0206 0201 10fb 0227 0c01  .............'..
-00002b30: 080e 0a0a 0a01 0207 0201 0201 12fb 0a19  ................
-00002b40: 0a08 1204 729a 0000 0029 42da 0a5f 5f66  ....r....)B..__f
-00002b50: 7574 7572 655f 5f72 0200 0000 72bb 0000  uture__r....r...
-00002b60: 0072 6600 0000 726f 0000 00da 0a63 6f6e  .rf...ro.....con
-00002b70: 7465 7874 6c69 6272 0300 0000 7205 0000  textlibr....r...
-00002b80: 00da 0770 6174 686c 6962 7206 0000 00da  ...pathlibr.....
-00002b90: 0a73 7562 7072 6f63 6573 7372 0700 0000  .subprocessr....
-00002ba0: 5a0a 7765 6262 726f 7773 6572 7208 0000  Z.webbrowserr...
-00002bb0: 0072 c600 0000 5a0c 7269 6368 2e63 6f6e  .r....Z.rich.con
-00002bc0: 736f 6c65 7209 0000 005a 1072 6963 682e  soler....Z.rich.
-00002bd0: 6869 6768 6c69 6768 7465 7272 0a00 0000  highlighterr....
-00002be0: 5a09 7269 6368 2e74 6578 7472 0b00 0000  Z.rich.textr....
-00002bf0: 5a07 7465 7874 7561 6c72 0c00 0000 720d  Z.textualr....r.
-00002c00: 0000 005a 0b74 6578 7475 616c 2e61 7070  ...Z.textual.app
-00002c10: 720e 0000 0072 0f00 0000 7210 0000 005a  r....r....r....Z
-00002c20: 0f74 6578 7475 616c 2e62 696e 6469 6e67  .textual.binding
-00002c30: 7211 0000 005a 1274 6578 7475 616c 2e63  r....Z.textual.c
-00002c40: 6f6e 7461 696e 6572 7372 1200 0000 7213  ontainersr....r.
-00002c50: 0000 0072 1400 0000 5a11 7465 7874 7561  ...r....Z.textua
-00002c60: 6c2e 6373 732e 7175 6572 7972 1500 0000  l.css.queryr....
-00002c70: 5a0e 7465 7874 7561 6c2e 7363 7265 656e  Z.textual.screen
-00002c80: 7216 0000 005a 0f74 6578 7475 616c 2e77  r....Z.textual.w
-00002c90: 6964 6765 7473 7217 0000 0072 1800 0000  idgetsr....r....
-00002ca0: 7219 0000 0072 1a00 0000 721b 0000 005a  r....r....r....Z
-00002cb0: 1474 6578 7475 616c 2e77 6964 6765 7473  .textual.widgets
-00002cc0: 2e74 7265 6572 1c00 0000 721e 0000 005a  .treer....r....Z
-00002cd0: 0b72 756e 5f63 6f6d 6d61 6e64 721f 0000  .run_commandr...
-00002ce0: 0072 af00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00002cf0: 5a14 7769 6467 6574 732e 636f 6d6d 616e  Z.widgets.comman
-00002d00: 645f 696e 666f 7222 0000 005a 1477 6964  d_infor"...Z.wid
-00002d10: 6765 7473 2e63 6f6d 6d61 6e64 5f74 7265  gets.command_tre
-00002d20: 6572 2300 0000 5a0c 7769 6467 6574 732e  er#...Z.widgets.
-00002d30: 666f 726d 7224 0000 005a 1777 6964 6765  formr$...Z.widge
-00002d40: 7473 2e6d 756c 7469 706c 655f 6368 6f69  ts.multiple_choi
-00002d50: 6365 7225 0000 00da 0c76 6572 7369 6f6e  cer%.....version
-00002d60: 5f69 6e66 6fda 0969 6d70 6f72 746c 6962  _info..importlib
-00002d70: 7228 0000 00da 1269 6d70 6f72 746c 6962  r(.....importlib
-00002d80: 5f6d 6574 6164 6174 6172 2900 0000 729a  _metadatar)...r.
-00002d90: 0000 0072 4800 0000 7248 0000 0072 4800  ...rH...rH...rH.
-00002da0: 0000 7249 0000 00da 083c 6d6f 6475 6c65  ..rI.....<module
-00002db0: 3e01 0000 0073 4200 0000 0c00 0802 0801  >....sB.........
-00002dc0: 0801 0c01 0c01 0c01 0c01 0c01 0c02 0c01  ................
-00002dd0: 0c01 1001 1401 0c01 1401 0c01 0c01 1c01  ................
-00002de0: 0c01 0c02 0c01 1001 0c01 0c01 0c01 0c01  ................
-00002df0: 0a02 0e01 0802 1003 007f 144c            ...........L
+00000bb0: 0000 0100 0000 0200 0000 4300 0001 733a  ..........C...s:
+00000bc0: 0000 007c 00a0 00a1 0001 007c 006a 01a0  ...|.......|.j..
+00000bd0: 02a1 007c 006a 035f 047c 006a 01a0 05a1  ...|.j._.|.j....
+00000be0: 007c 006a 035f 0664 017c 006a 035f 077c  .|.j._.d.|.j._.|
+00000bf0: 006a 03a0 08a1 0001 0064 0053 00a9 024e  .j.......d.S...N
+00000c00: 5429 09da 1a61 6374 696f 6e5f 636f 7079  T)...action_copy
+00000c10: 5f63 6f6d 6d61 6e64 5f73 7472 696e 6772  _command_stringr
+00000c20: 4200 0000 da0d 746f 5f63 6c69 5f73 7472  B.....to_cli_str
+00000c30: 696e 67da 0361 7070 da19 706f 7374 5f72  ing..app..post_r
+00000c40: 756e 5f63 6f6d 6d61 6e64 5f72 6564 6163  un_command_redac
+00000c50: 7465 64da 0b74 6f5f 636c 695f 6172 6773  ted..to_cli_args
+00000c60: da10 706f 7374 5f72 756e 5f63 6f6d 6d61  ..post_run_comma
+00000c70: 6e64 da0f 6578 6563 7574 655f 6f6e 5f65  nd..execute_on_e
+00000c80: 7869 7472 3200 0000 a901 7245 0000 0072  xitr2.....rE...r
+00000c90: 4800 0000 7248 0000 0072 4900 0000 da14  H...rH...rI.....
+00000ca0: 6163 7469 6f6e 5f63 6c6f 7365 5f61 6e64  action_close_and
+00000cb0: 5f72 756e 7e00 0000 730a 0000 0008 010e  _run~...s.......
+00000cc0: 010e 0108 010e 017a 2343 6f6d 6d61 6e64  .......z#Command
+00000cd0: 4275 696c 6465 722e 6163 7469 6f6e 5f63  Builder.action_c
+00000ce0: 6c6f 7365 5f61 6e64 5f72 756e 6301 0000  lose_and_runc...
+00000cf0: 0000 0000 0000 0000 0002 0000 000a 0000  ................
+00000d00: 0043 0000 0173 8a00 0000 7400 6a01 6401  .C...s....t.j.d.
+00000d10: 6b02 7208 6402 6701 6e0b 7400 6a01 6403  k.r.d.g.n.t.j.d.
+00000d20: 6b02 7210 6404 6701 6e03 6700 6405 a201  k.r.d.g.n.g.d...
+00000d30: 7d01 7402 7403 8301 8f23 0100 7404 7c01  }.t.t....#..t.|.
+00000d40: 7c00 6a05 6406 1700 6406 a006 6407 6408  |.j.d...d...d.d.
+00000d50: 8400 7c00 6a07 6a08 6409 640a 8d01 4400  ..|.j.j.d.d...D.
+00000d60: 8301 a101 1700 6409 640b 640c 8d04 0100  ......d.d.d.....
+00000d70: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+00000d80: 3100 733e 7701 0100 0100 0100 5900 0100  1.s>w.......Y...
+00000d90: 6400 5300 290d 4eda 0577 696e 3332 da04  d.S.).N..win32..
+00000da0: 636f 7079 da06 6461 7277 696e 5a06 7062  copy..darwinZ.pb
+00000db0: 636f 7079 2903 5a05 7863 6c69 707a 0a2d  copy).Z.xclipz.-
+00000dc0: 7365 6c65 6374 696f 6e5a 0963 6c69 7062  selectionZ.clipb
+00000dd0: 6f61 7264 da01 2063 0100 0000 0000 0000  oard.. c........
+00000de0: 0000 0000 0200 0000 0500 0000 7300 0001  ............s...
+00000df0: 731e 0000 0081 007c 005d 0a7d 0174 00a0  s......|.].}.t..
+00000e00: 0174 027c 0183 01a1 0156 0001 0071 0264  .t.|.....V...q.d
+00000e10: 0053 0072 3f00 0000 2903 da05 7368 6c65  .S.r?...)...shle
+00000e20: 78da 0571 756f 7465 7237 0000 00a9 02da  x..quoter7......
+00000e30: 022e 30da 0178 7248 0000 0072 4800 0000  ..0..xrH...rH...
+00000e40: 7249 0000 00da 093c 6765 6e65 7870 723e  rI.....<genexpr>
+00000e50: 9400 0000 730a 0000 0002 8004 0002 020c  ....s...........
+00000e60: ff0a ff7a 3c43 6f6d 6d61 6e64 4275 696c  ...z<CommandBuil
+00000e70: 6465 722e 6163 7469 6f6e 5f63 6f70 795f  der.action_copy_
+00000e80: 636f 6d6d 616e 645f 7374 7269 6e67 2e3c  command_string.<
+00000e90: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+00000ea0: 3e54 2901 5a0d 7265 6461 6374 5f73 6563  >T).Z.redact_sec
+00000eb0: 7265 7446 2903 da05 696e 7075 74da 0474  retF)...input..t
+00000ec0: 6578 74da 0563 6865 636b 2909 da03 7379  ext..check)...sy
+00000ed0: 73da 0870 6c61 7466 6f72 6d72 0300 0000  s..platformr....
+00000ee0: da11 4669 6c65 4e6f 7446 6f75 6e64 4572  ..FileNotFoundEr
+00000ef0: 726f 7272 0700 0000 7236 0000 00da 046a  rorr....r6.....j
+00000f00: 6f69 6e72 4200 0000 725e 0000 0029 0272  oinrB...r^...).r
+00000f10: 4500 0000 da03 636d 6472 4800 0000 7248  E.....cmdrH...rH
+00000f20: 0000 0072 4900 0000 725a 0000 0085 0000  ...rI...rZ......
+00000f30: 0073 2800 0000 0a03 06ff 0a03 06ff 0602  .s(.............
+00000f40: 02fb 0a09 0201 0201 0401 0201 02ff 0a02  ................
+00000f50: 0c02 06fe 02fe 0206 0201 08f7 22ff 7a29  ............".z)
+00000f60: 436f 6d6d 616e 6442 7569 6c64 6572 2e61  CommandBuilder.a
+00000f70: 6374 696f 6e5f 636f 7079 5f63 6f6d 6d61  ction_copy_comma
+00000f80: 6e64 5f73 7472 696e 6763 0100 0000 0000  nd_stringc......
+00000f90: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000fa0: 0001 730e 0000 007c 006a 00a0 01a1 0001  ..s....|.j......
+00000fb0: 0064 0053 0072 3f00 0000 2902 725c 0000  .d.S.r?...).r\..
+00000fc0: 0072 3200 0000 7261 0000 0072 4800 0000  .r2...ra...rH...
+00000fd0: 7248 0000 0072 4900 0000 da0b 6163 7469  rH...rI.....acti
+00000fe0: 6f6e 5f65 7869 749c 0000 0073 0200 0000  on_exit....s....
+00000ff0: 0e01 7a1a 436f 6d6d 616e 6442 7569 6c64  ..z.CommandBuild
+00001000: 6572 2e61 6374 696f 6e5f 6578 6974 6301  er.action_exitc.
+00001010: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001020: 0000 0043 0000 0173 1e00 0000 6401 6402  ...C...s....d.d.
+00001030: 6c00 6d01 7d01 0100 7c00 6a02 a003 7c01  l.m.}...|.j...|.
+00001040: 8300 a101 0100 6400 5300 2903 4e72 1d00  ......d.S.).Nr..
+00001050: 0000 2901 da0b 4162 6f75 7444 6961 6c6f  ..)...AboutDialo
+00001060: 6729 045a 0d77 6964 6765 7473 2e61 626f  g).Z.widgets.abo
+00001070: 7574 7276 0000 0072 5c00 0000 da0b 7075  utrv...r\.....pu
+00001080: 7368 5f73 6372 6565 6e29 0272 4500 0000  sh_screen).rE...
+00001090: 7276 0000 0072 4800 0000 7248 0000 0072  rv...rH...rH...r
+000010a0: 4900 0000 da0c 6163 7469 6f6e 5f61 626f  I.....action_abo
+000010b0: 7574 9f00 0000 7304 0000 000c 0112 027a  ut....s........z
+000010c0: 1b43 6f6d 6d61 6e64 4275 696c 6465 722e  .CommandBuilder.
+000010d0: 6163 7469 6f6e 5f61 626f 7574 da05 6576  action_about..ev
+000010e0: 656e 74fa 0c65 7665 6e74 732e 4d6f 756e  ent..events.Moun
+000010f0: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00001100: 0000 0200 0000 c300 0001 7314 0000 0081  ..........s.....
+00001110: 017c 00a0 00a1 0049 0064 0048 0001 0064  .|.....I.d.H...d
+00001120: 0053 0072 3f00 0000 2901 da15 5f72 6566  .S.r?...)..._ref
+00001130: 7265 7368 5f63 6f6d 6d61 6e64 5f66 6f72  resh_command_for
+00001140: 6da9 0272 4500 0000 7279 0000 0072 4800  m..rE...ry...rH.
+00001150: 0000 7248 0000 0072 4900 0000 da08 6f6e  ..rH...rI.....on
+00001160: 5f6d 6f75 6e74 a400 0000 7304 0000 0002  _mount....s.....
+00001170: 8012 017a 1743 6f6d 6d61 6e64 4275 696c  ...z.CommandBuil
+00001180: 6465 722e 6f6e 5f6d 6f75 6e74 da04 6e6f  der.on_mount..no
+00001190: 6465 fa1e 5472 6565 4e6f 6465 5b43 6f6d  de..TreeNode[Com
+000011a0: 6d61 6e64 5363 6865 6d61 5d20 7c20 4e6f  mandSchema] | No
+000011b0: 6e65 6302 0000 0000 0000 0000 0000 0003  nec.............
+000011c0: 0000 0008 0000 00c3 0000 0173 6a00 0000  ...........sj...
+000011d0: 8101 7c01 6400 7500 721a 7a0a 7c00 a000  ..|.d.u.r.z.|...
+000011e0: 7401 a101 7d02 7c02 6a02 7d01 5700 6e0a  t...}.|.j.}.W.n.
+000011f0: 0400 7403 7919 0100 0100 0100 5900 6400  ..t.y.......Y.d.
+00001200: 5300 7700 7c01 6a04 7c00 5f05 7c00 a006  S.w.|.j.|._.|...
+00001210: 7c01 a101 0100 7c00 a007 7c00 6a05 7c00  |.....|...|.j.|.
+00001220: 6a08 a102 0100 7c00 a009 7c01 a101 4900  j.....|...|...I.
+00001230: 6400 4800 0100 6400 5300 723f 0000 0029  d.H...d.S.r?...)
+00001240: 0ada 0971 7565 7279 5f6f 6e65 7223 0000  ...query_oner#..
+00001250: 005a 0b63 7572 736f 725f 6e6f 6465 7215  .Z.cursor_noder.
+00001260: 0000 00da 0464 6174 61da 1773 656c 6563  .....data..selec
+00001270: 7465 645f 636f 6d6d 616e 645f 7363 6865  ted_command_sche
+00001280: 6d61 da1b 5f75 7064 6174 655f 636f 6d6d  ma.._update_comm
+00001290: 616e 645f 6465 7363 7269 7074 696f 6eda  and_description.
+000012a0: 205f 7570 6461 7465 5f65 7865 6375 7469   _update_executi
+000012b0: 6f6e 5f73 7472 696e 675f 7072 6576 6965  on_string_previe
+000012c0: 7772 4200 0000 da11 5f75 7064 6174 655f  wrB....._update_
+000012d0: 666f 726d 5f62 6f64 7929 0372 4500 0000  form_body).rE...
+000012e0: 727e 0000 00da 0c63 6f6d 6d61 6e64 5f74  r~.....command_t
+000012f0: 7265 6572 4800 0000 7248 0000 0072 4900  reerH...rH...rI.
+00001300: 0000 727b 0000 00a7 0000 0073 1e00 0000  ..r{.......s....
+00001310: 0280 0801 0201 0a01 0a01 0c01 0601 02ff  ................
+00001320: 0803 0a01 0401 0401 0401 04fe 1404 7a24  ..............z$
+00001330: 436f 6d6d 616e 6442 7569 6c64 6572 2e5f  CommandBuilder._
+00001340: 7265 6672 6573 685f 636f 6d6d 616e 645f  refresh_command_
+00001350: 666f 726d fa23 5472 6565 2e4e 6f64 6548  form.#Tree.NodeH
+00001360: 6967 686c 6967 6874 6564 5b43 6f6d 6d61  ighlighted[Comma
+00001370: 6e64 5363 6865 6d61 5d63 0200 0000 0000  ndSchema]c......
+00001380: 0000 0000 0000 0200 0000 0300 0000 c300  ................
+00001390: 0001 7318 0000 0081 017c 00a0 007c 016a  ..s......|...|.j
+000013a0: 01a1 0149 0064 0148 0001 0064 0153 0029  ...I.d.H...d.S.)
+000013b0: 027a 9257 6865 6e20 7765 2068 6967 686c  .z.When we highl
+000013c0: 6967 6874 2061 206e 6f64 6520 696e 2074  ight a node in t
+000013d0: 6865 2043 6f6d 6d61 6e64 5472 6565 2c20  he CommandTree, 
+000013e0: 7468 6520 6d61 696e 2062 6f64 7920 6f66  the main body of
+000013f0: 2074 6865 2068 6f6d 6520 7061 6765 2075   the home page u
+00001400: 7064 6174 6573 0a20 2020 2020 2020 2074  pdates.        t
+00001410: 6f20 6469 7370 6c61 7920 6120 666f 726d  o display a form
+00001420: 2073 7065 6369 6669 6320 746f 2074 6865   specific to the
+00001430: 2068 6967 686c 6967 6874 6564 2063 6f6d   highlighted com
+00001440: 6d61 6e64 2e4e 2902 727b 0000 0072 7e00  mand.N).r{...r~.
+00001450: 0000 727c 0000 0072 4800 0000 7248 0000  ..r|...rH...rH..
+00001460: 0072 4900 0000 da18 7365 6c65 6374 6564  .rI.....selected
+00001470: 5f63 6f6d 6d61 6e64 5f63 6861 6e67 6564  _command_changed
+00001480: b700 0000 7304 0000 0002 8016 077a 2743  ....s........z'C
+00001490: 6f6d 6d61 6e64 4275 696c 6465 722e 7365  ommandBuilder.se
+000014a0: 6c65 6374 6564 5f63 6f6d 6d61 6e64 5f63  lected_command_c
+000014b0: 6861 6e67 6564 fa13 436f 6d6d 616e 6446  hanged..CommandF
+000014c0: 6f72 6d2e 4368 616e 6765 6463 0200 0000  orm.Changedc....
+000014d0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000014e0: 4300 0001 731c 0000 007c 016a 007c 005f  C...s....|.j.|._
+000014f0: 007c 00a0 017c 006a 027c 006a 00a1 0201  .|...|.j.|.j....
+00001500: 0064 0053 0072 3f00 0000 2903 7242 0000  .d.S.r?...).rB..
+00001510: 0072 8400 0000 7282 0000 0072 7c00 0000  .r....r....r|...
+00001520: 7248 0000 0072 4800 0000 7249 0000 00da  rH...rH...rI....
+00001530: 1375 7064 6174 655f 636f 6d6d 616e 645f  .update_command_
+00001540: 6461 7461 c000 0000 730a 0000 0008 0204  data....s.......
+00001550: 0104 0104 0108 fe7a 2243 6f6d 6d61 6e64  .......z"Command
+00001560: 4275 696c 6465 722e 7570 6461 7465 5f63  Builder.update_c
+00001570: 6f6d 6d61 6e64 5f64 6174 61fa 1754 7265  ommand_data..Tre
+00001580: 654e 6f64 655b 436f 6d6d 616e 6453 6368  eNode[CommandSch
+00001590: 656d 615d 6302 0000 0000 0000 0000 0000  ema]c...........
+000015a0: 0004 0000 0004 0000 0043 0000 0173 4c00  .........C...sL.
+000015b0: 0000 7c00 a000 6401 7401 a102 7d02 7c01  ..|...d.t...}.|.
+000015c0: 6a02 6a03 700b 6402 7d03 7c03 a004 a100  j.j.p.d.}.|.....
+000015d0: 7d03 6403 7c00 6a05 7217 7c01 6a06 6e02  }.d.|.j.r.|.j.n.
+000015e0: 7c00 6a07 9b00 6404 7c03 9b00 9d04 7d03  |.j...d.|.....}.
+000015f0: 7c02 a008 7c03 a101 0100 6405 5300 2906  |...|.....d.S.).
+00001600: 7a84 5570 6461 7465 2074 6865 2064 6573  z.Update the des
+00001610: 6372 6970 7469 6f6e 206f 6620 7468 6520  cription of the 
+00001620: 636f 6d6d 616e 6420 6174 2074 6865 2062  command at the b
+00001630: 6f74 746f 6d20 6f66 2074 6865 2073 6964  ottom of the sid
+00001640: 6562 6172 0a20 2020 2020 2020 2062 6173  ebar.        bas
+00001650: 6564 206f 6e20 7468 6520 6375 7272 656e  ed on the curren
+00001660: 746c 7920 7365 6c65 6374 6564 206e 6f64  tly selected nod
+00001670: 6520 696e 2074 6865 2063 6f6d 6d61 6e64  e in the command
+00001680: 2074 7265 652e 7a19 2368 6f6d 652d 636f   tree.z.#home-co
+00001690: 6d6d 616e 642d 6465 7363 7269 7074 696f  mmand-descriptio
+000016a0: 6e72 4f00 0000 7a03 5b62 5d7a 045b 2f5d  nrO...z.[b]z.[/]
+000016b0: 0a4e 2909 7280 0000 0072 1a00 0000 7281  .N).r....r....r.
+000016c0: 0000 00da 0964 6f63 7374 7269 6e67 da06  .....docstring..
+000016d0: 6c73 7472 6970 723a 0000 00da 056c 6162  lstripr:.....lab
+000016e0: 656c 7236 0000 00da 0675 7064 6174 6529  elr6.....update)
+000016f0: 0472 4500 0000 727e 0000 005a 0f64 6573  .rE...r~...Z.des
+00001700: 6372 6970 7469 6f6e 5f62 6f78 5a10 6465  cription_boxZ.de
+00001710: 7363 7269 7074 696f 6e5f 7465 7874 7248  scription_textrH
+00001720: 0000 0072 4800 0000 7249 0000 0072 8300  ...rH...rI...r..
+00001730: 0000 c800 0000 730a 0000 000c 030c 0108  ......s.........
+00001740: 011e 010e 017a 2a43 6f6d 6d61 6e64 4275  .....z*CommandBu
+00001750: 696c 6465 722e 5f75 7064 6174 655f 636f  ilder._update_co
+00001760: 6d6d 616e 645f 6465 7363 7269 7074 696f  mmand_descriptio
+00001770: 6eda 0e63 6f6d 6d61 6e64 5f73 6368 656d  n..command_schem
+00001780: 6172 2100 0000 7242 0000 0072 1f00 0000  ar!...rB...r....
+00001790: 6303 0000 0000 0000 0000 0000 0009 0000  c...............
+000017a0: 0006 0000 0043 0000 0173 7400 0000 7c00  .....C...st...|.
+000017b0: 6a00 6401 7501 7238 7c00 a001 6402 a101  j.d.u.r8|...d...
+000017c0: 7d03 7402 7c00 6a03 9b00 6403 9d02 7c03  }.t.|.j...d...|.
+000017d0: 8302 7d04 7c02 a004 a100 7d05 7402 a005  ..}.|.....}.t...
+000017e0: 7c04 7c00 a006 7c05 a101 a102 7d06 7c00  |.|...|.....}.|.
+000017f0: a001 6404 a101 7d07 7402 a005 6405 7c07  ..d...}.t...d.|.
+00001800: 6602 7c06 a102 7d08 7c00 a007 6406 7408  f.|...}.|...d.t.
+00001810: a102 a009 7c08 a101 0100 6401 5300 6401  ....|.....d.S.d.
+00001820: 5300 2907 7a40 5570 6461 7465 2074 6865  S.).z@Update the
+00001830: 2070 7265 7669 6577 2062 6f78 2073 686f   preview box sho
+00001840: 7769 6e67 2074 6865 2063 6f6d 6d61 6e64  wing the command
+00001850: 2073 7472 696e 6720 746f 2062 6520 6578   string to be ex
+00001860: 6563 7574 6564 4e72 2a00 0000 7266 0000  ecutedNr*...rf..
+00001870: 0072 2c00 0000 7a02 2420 7a19 2368 6f6d  .r,...z.$ z.#hom
+00001880: 652d 6578 6563 2d70 7265 7669 6577 2d73  e-exec-preview-s
+00001890: 7461 7469 6329 0a72 4200 0000 7250 0000  tatic).rB...rP..
+000018a0: 0072 0b00 0000 7236 0000 0072 5b00 0000  .r....r6...r[...
+000018b0: 7252 0000 0072 4400 0000 7280 0000 0072  rR...rD...r....r
+000018c0: 1a00 0000 728f 0000 0029 0972 4500 0000  ....r....).rE...
+000018d0: 7290 0000 0072 4200 0000 5a19 636f 6d6d  r....rB...Z.comm
+000018e0: 616e 645f 6e61 6d65 5f73 796e 7461 785f  and_name_syntax_
+000018f0: 7374 796c 65da 0670 7265 6669 785a 096e  style..prefixZ.n
+00001900: 6577 5f76 616c 7565 5a15 6869 6768 6c69  ew_valueZ.highli
+00001910: 6768 7465 645f 6e65 775f 7661 6c75 655a  ghted_new_valueZ
+00001920: 0c70 726f 6d70 745f 7374 796c 655a 0e70  .prompt_styleZ.p
+00001930: 7265 7669 6577 5f73 7472 696e 6772 4800  review_stringrH.
+00001940: 0000 7248 0000 0072 4900 0000 7284 0000  ..rH...rI...r...
+00001950: 00d1 0000 0073 1600 0000 0a06 0401 0201  .....s..........
+00001960: 04ff 1203 0801 1201 0a01 1001 1601 04f7  ................
+00001970: 7a2f 436f 6d6d 616e 6442 7569 6c64 6572  z/CommandBuilder
+00001980: 2e5f 7570 6461 7465 5f65 7865 6375 7469  ._update_executi
+00001990: 6f6e 5f73 7472 696e 675f 7072 6576 6965  on_string_previe
+000019a0: 7763 0200 0000 0000 0000 0000 0000 0600  wc..............
+000019b0: 0000 0400 0000 c300 0001 7362 0000 0081  ..........sb....
+000019c0: 017c 00a0 0064 0174 01a1 027d 027c 026a  .|...d.t...}.|.j
+000019d0: 0244 005d 097d 037c 03a0 03a1 0049 0064  .D.].}.|.....I.d
+000019e0: 0048 0001 0071 0a7c 016a 047d 0474 057c  .H...q.|.j.}.t.|
+000019f0: 047c 006a 0664 028d 027d 057c 02a0 077c  .|.j.d...}.|...|
+00001a00: 05a1 0149 0064 0048 0001 007c 006a 0873  ...I.d.H...|.j.s
+00001a10: 2f7c 05a0 09a1 0001 0064 0053 0064 0053  /|.......d.S.d.S
+00001a20: 0029 034e 7a11 2368 6f6d 652d 626f 6479  .).Nz.#home-body
+00001a30: 2d73 6372 6f6c 6c29 0272 9000 0000 7234  -scroll).r....r4
+00001a40: 0000 0029 0a72 8000 0000 7214 0000 00da  ...).r....r.....
+00001a50: 0863 6869 6c64 7265 6eda 0672 656d 6f76  .children..remov
+00001a60: 6572 8100 0000 7224 0000 0072 3400 0000  er....r$...r4...
+00001a70: 5a05 6d6f 756e 7472 3a00 0000 7253 0000  Z.mountr:...rS..
+00001a80: 0029 0672 4500 0000 727e 0000 00da 0670  .).rE...r~.....p
+00001a90: 6172 656e 74da 0563 6869 6c64 7290 0000  arent..childr...
+00001aa0: 005a 0c63 6f6d 6d61 6e64 5f66 6f72 6d72  .Z.command_formr
+00001ab0: 4800 0000 7248 0000 0072 4900 0000 7285  H...rH...rI...r.
+00001ac0: 0000 00e2 0000 0073 1a00 0000 0280 0c02  .......s........
+00001ad0: 0a01 1001 0603 0201 0201 0401 06fe 1004  ................
+00001ae0: 0601 0c01 04ff 7a20 436f 6d6d 616e 6442  ......z CommandB
+00001af0: 7569 6c64 6572 2e5f 7570 6461 7465 5f66  uilder._update_f
+00001b00: 6f72 6d5f 626f 6479 2903 4e4e 4e29 0e72  orm_body).NNN).r
+00001b10: 3400 0000 7235 0000 0072 3600 0000 7237  4...r5...r6...r7
+00001b20: 0000 0072 3800 0000 7239 0000 0072 3a00  ...r8...r9...r:.
+00001b30: 0000 723b 0000 0072 3c00 0000 7239 0000  ..r;...r<...r9..
+00001b40: 0072 3d00 0000 7239 0000 0072 3e00 0000  .r=...r9...r>...
+00001b50: 7239 0000 0029 0272 4a00 0000 7210 0000  r9...).rJ...r...
+00001b60: 00a9 0272 4a00 0000 7258 0000 0029 0472  ...rJ...rX...).r
+00001b70: 7900 0000 727a 0000 0072 4a00 0000 7258  y...rz...rJ...rX
+00001b80: 0000 0072 3f00 0000 2902 727e 0000 0072  ...r?...).r~...r
+00001b90: 7f00 0000 2904 7279 0000 0072 8700 0000  ....).ry...r....
+00001ba0: 724a 0000 0072 5800 0000 2904 7279 0000  rJ...rX...).ry..
+00001bb0: 0072 8900 0000 724a 0000 0072 5800 0000  .r....rJ...rX...
+00001bc0: 2904 727e 0000 0072 8b00 0000 724a 0000  ).r~...r....rJ..
+00001bd0: 0072 5800 0000 2906 7290 0000 0072 2100  .rX...).r....r!.
+00001be0: 0000 7242 0000 0072 1f00 0000 724a 0000  ..rB...r....rJ..
+00001bf0: 0072 5800 0000 2919 da08 5f5f 6e61 6d65  .rX...)...__name
+00001c00: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00001c10: 5f5f 7175 616c 6e61 6d65 5f5f 5a11 434f  __qualname__Z.CO
+00001c20: 4d50 4f4e 454e 545f 434c 4153 5345 5372  MPONENT_CLASSESr
+00001c30: 1100 0000 5a08 4249 4e44 494e 4753 7241  ....Z.BINDINGSrA
+00001c40: 0000 0072 5700 0000 7262 0000 0072 5a00  ...rW...rb...rZ.
+00001c50: 0000 7275 0000 0072 7800 0000 727d 0000  ..ru...rx...r}..
+00001c60: 0072 7b00 0000 720d 0000 0072 1b00 0000  .r{...r....r....
+00001c70: 5a0f 4e6f 6465 4869 6768 6c69 6768 7465  Z.NodeHighlighte
+00001c80: 6472 8800 0000 7224 0000 005a 0743 6861  dr....r$...Z.Cha
+00001c90: 6e67 6564 728a 0000 0072 8300 0000 7284  ngedr....r....r.
+00001ca0: 0000 0072 8500 0000 da0d 5f5f 636c 6173  ...r......__clas
+00001cb0: 7363 656c 6c5f 5f72 4800 0000 7248 0000  scell__rH...rH..
+00001cc0: 0072 4600 0000 7249 0000 0072 2900 0000  .rF...rI...r)...
+00001cd0: 2600 0000 7340 0000 0008 0008 010c 030c  &...s@..........
+00001ce0: 0102 0102 0102 0102 0104 fd0c 050c 010c  ................
+00001cf0: 010c 0104 f502 1402 0102 0110 f80a 140a  ................
+00001d00: 330a 070a 170a 030a 050c 0308 100c 0108  3...............
+00001d10: 080c 010a 070a 0912 1172 2900 0000 6300  .........r)...c.
+00001d20: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00001d30: 0000 0000 0000 0173 9200 0000 6500 5a01  .......s....e.Z.
+00001d40: 6400 5a02 6503 6504 8301 6a05 6401 1b00  d.Z.e.e...j.d...
+00001d50: 5a06 0902 0902 6429 642a 8700 6601 640b  Z.....d)d*..f.d.
+00001d60: 640c 840d 5a07 6508 642b 6410 6411 8404  d...Z.e.d+d.d...
+00001d70: 8301 5a09 6412 6413 8400 5a0a 650b 650c  ..Z.d.d...Z.e.e.
+00001d80: 6a0d 6414 8302 6415 6416 8400 8301 5a0e  j.d...d.d.....Z.
+00001d90: 6417 6402 6402 6418 9c03 642c 8700 6601  d.d.d.d...d,..f.
+00001da0: 641f 6420 840e 5a0f 642d 6421 6422 8404  d.d ..Z.d-d!d"..
+00001db0: 5a10 642d 6423 6424 8404 5a11 642e 6427  Z.d-d#d$..Z.d.d'
+00001dc0: 6428 8404 5a12 8700 0400 5a13 5300 292f  d(..Z.....Z.S.)/
+00001dd0: da03 5475 697a 0874 7569 2e73 6373 734e  ..Tuiz.tui.scssN
+00001de0: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
+00001df0: 3900 0000 7238 0000 00da 0e63 6f6d 6d61  9...r8.....comma
+00001e00: 6e64 5f66 696c 7465 7272 4a00 0000 7258  nd_filterrJ...rX
+00001e10: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
+00001e20: 0700 0000 0800 0000 0300 0001 7312 0100  ............s...
+00001e30: 0074 0083 00a0 01a1 0001 0067 007c 005f  .t.........g.|._
+00001e40: 0264 017c 005f 0374 047c 01a0 05a1 0083  .d.|._.t.|......
+00001e50: 0164 0219 007d 0588 0072 497c 017c 0519  .d...}...rI|.|..
+00001e60: 006a 0672 4987 0066 0164 0364 0484 087c  .j.rI..f.d.d...|
+00001e70: 017c 0519 006a 06a0 07a1 0044 0083 017d  .|...j.....D...}
+00001e80: 0674 087c 0683 0164 056b 0272 4474 0987  .t.|...d.k.rDt..
+00001e90: 0066 0164 0664 0784 0864 0844 0083 0183  .f.d.d...d.D....
+00001ea0: 0173 447c 067d 0174 047c 01a0 05a1 0083  .sD|.}.t.|......
+00001eb0: 0164 0219 007d 056e 057c 067c 017c 0519  .d...}.n.|.|.|..
+00001ec0: 005f 067c 017c 005f 0a74 0964 0964 0784  ._.|.|._.t.d.d..
+00001ed0: 007c 01a0 0ba1 0044 0083 0183 017c 005f  .|.....D.....|._
+00001ee0: 0c64 0a7c 005f 0d7c 0272 5f7c 026e 0274  .d.|._.|.r_|.n.t
+00001ef0: 0e83 007c 005f 0f7c 037c 005f 107c 006a  ...|._.|.|._.|.j
+00001f00: 1073 8774 1174 1283 018f 1001 0074 13a0  .s.t.t.......t..
+00001f10: 147c 006a 0fa1 017c 005f 1057 0064 0004  .|.j...|._.W.d..
+00001f20: 0004 0083 0301 0064 0053 0031 0073 8077  .......d.S.1.s.w
+00001f30: 0101 0001 0001 0059 0001 0064 0053 0064  .......Y...d.S.d
+00001f40: 0053 0029 0b4e 724f 0000 0072 0100 0000  .S.).NrO...r....
+00001f50: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00001f60: 0005 0000 0013 0000 0173 2000 0000 6900  .........s ...i.
+00001f70: 7c00 5d0c 5c02 7d01 7d02 7400 7c01 8800  |.].\.}.}.t.|...
+00001f80: 8302 7202 7c01 7c02 9302 7102 5300 7248  ..r.|.|...q.S.rH
+00001f90: 0000 0072 0400 0000 2903 726a 0000 00da  ...r....).rj....
+00001fa0: 016b 724e 0000 00a9 0172 9c00 0000 7248  .krN.....r....rH
+00001fb0: 0000 0072 4900 0000 da0a 3c64 6963 7463  ...rI.....<dictc
+00001fc0: 6f6d 703e 0401 0000 730c 0000 0006 0006  omp>....s.......
+00001fd0: 0208 0102 fd04 0106 ff7a 2054 7569 2e5f  .........z Tui._
+00001fe0: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
+00001ff0: 2e3c 6469 6374 636f 6d70 3e72 1d00 0000  .<dictcomp>r....
+00002000: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002010: 0003 0000 0033 0000 0173 1800 0000 8100  .....3...s......
+00002020: 7c00 5d07 7d01 7c01 8800 7600 5600 0100  |.].}.|...v.V...
+00002030: 7102 6400 5300 723f 0000 0072 4800 0000  q.d.S.r?...rH...
+00002040: 7269 0000 0072 9e00 0000 7248 0000 0072  ri...r....rH...r
+00002050: 4900 0000 726c 0000 0009 0100 0073 0800  I...rl.......s..
+00002060: 0000 0280 0400 0801 0aff 7a1f 5475 692e  ..........z.Tui.
+00002070: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+00002080: 3e2e 3c67 656e 6578 7072 3e29 02da 012a  >.<genexpr>)...*
+00002090: fa01 3f63 0100 0000 0000 0000 0000 0000  ..?c............
+000020a0: 0200 0000 0200 0000 7300 0001 7316 0000  ........s...s...
+000020b0: 0081 007c 005d 067d 017c 016a 0056 0001  ...|.].}.|.j.V..
+000020c0: 0071 0264 0053 0072 3f00 0000 2901 da0b  .q.d.S.r?...)...
+000020d0: 7375 6263 6f6d 6d61 6e64 7329 0272 6a00  subcommands).rj.
+000020e0: 0000 724e 0000 0072 4800 0000 7248 0000  ..rN...rH...rH..
+000020f0: 0072 4900 0000 726c 0000 0013 0100 0073  .rI...rl.......s
+00002100: 0400 0000 0280 1400 4629 1572 4000 0000  ........F).r@...
+00002110: 7241 0000 0072 5f00 0000 725d 0000 00da  rA...r_...r]....
+00002120: 046c 6973 74da 046b 6579 7372 a200 0000  .list..keysr....
+00002130: da05 6974 656d 73da 036c 656e da03 616e  ..items..len..an
+00002140: 7972 3400 0000 da06 7661 6c75 6573 723a  yr4.....valuesr:
+00002150: 0000 0072 6000 0000 721e 0000 0072 3600  ...r`...r....r6.
+00002160: 0000 7238 0000 0072 0300 0000 da09 4578  ..r8...r......Ex
+00002170: 6365 7074 696f 6e72 2800 0000 7243 0000  ceptionr(...rC..
+00002180: 0029 0772 4500 0000 7234 0000 0072 3600  .).rE...r4...r6.
+00002190: 0000 7238 0000 0072 9c00 0000 da0d 726f  ..r8...r......ro
+000021a0: 6f74 5f63 6d64 5f6e 616d 655a 106d 6174  ot_cmd_nameZ.mat
+000021b0: 6368 696e 675f 7363 6865 6d61 7372 4600  ching_schemasrF.
+000021c0: 0000 729e 0000 0072 4900 0000 7241 0000  ..r....rI...rA..
+000021d0: 00f6 0000 0073 3000 0000 0a07 0602 0601  .....s0.........
+000021e0: 1002 0e01 0a01 0c02 06fe 1805 0201 08ff  ................
+000021f0: 0403 1201 0a03 0602 1801 0601 1002 0601  ................
+00002200: 0602 0a01 1001 22ff 04ff 7a0c 5475 692e  ......"...z.Tui.
+00002210: 5f5f 696e 6974 5f5f da04 6172 6773 7221  __init__..argsr!
+00002220: 0000 00fa 0527 5475 6927 6301 0000 0000  .....'Tui'c.....
+00002230: 0000 0000 0000 0006 0000 0004 0000 004f  ...............O
+00002240: 0000 0173 5200 0000 7c01 7306 7400 6401  ...sR...|.s.t.d.
+00002250: 8301 8201 7c01 6402 1900 7d03 7c03 6a01  ....|.d...}.|.j.
+00002260: 7c03 6901 7d04 7c01 6403 6400 8502 1900  |.i.}.|.d.d.....
+00002270: 4400 5d0b 7d05 7c03 7c05 5f02 7c05 7c03  D.].}.|.|._.|.|.
+00002280: 6a03 7c05 6a01 3c00 7115 7c00 7c04 6601  j.|.j.<.q.|.|.f.
+00002290: 6900 7c02 a401 8e01 5300 2904 4e7a 144e  i.|.....S.).Nz.N
+000022a0: 6f20 7363 6865 6d61 7320 7072 6f76 6964  o schemas provid
+000022b0: 6564 2e72 0100 0000 721d 0000 0029 04da  ed.r....r....)..
+000022c0: 0a56 616c 7565 4572 726f 7272 3c00 0000  .ValueErrorr<...
+000022d0: 7294 0000 0072 a200 0000 2906 da03 636c  r....r....)...cl
+000022e0: 7372 ab00 0000 da06 6b77 6172 6773 5a0b  sr......kwargsZ.
+000022f0: 726f 6f74 5f73 6368 656d 61da 0773 6368  root_schema..sch
+00002300: 656d 6173 5a06 7363 6865 6d61 7248 0000  emasZ.schemarH..
+00002310: 0072 4800 0000 7249 0000 00da 0c66 726f  .rH...rI.....fro
+00002320: 6d5f 7363 6865 6d61 731d 0100 0073 1000  m_schemas....s..
+00002330: 0000 0402 0801 0802 0a02 1002 0601 0e01  ................
+00002340: 1002 7a10 5475 692e 6672 6f6d 5f73 6368  ..z.Tui.from_sch
+00002350: 656d 6173 6301 0000 0000 0000 0000 0000  emasc...........
+00002360: 0001 0000 0008 0000 0043 0000 0173 2200  .........C...s".
+00002370: 0000 7c00 a000 7401 7c00 6a02 7c00 6a03  ..|...t.|.j.|.j.
+00002380: 7c00 6a04 7c00 6a05 6401 8d04 a101 0100  |.j.|.j.d.......
+00002390: 6400 5300 2902 4e29 0372 3600 0000 7238  d.S.).N).r6...r8
+000023a0: 0000 0072 3a00 0000 2906 7277 0000 0072  ...r:...).rw...r
+000023b0: 2900 0000 7234 0000 0072 3600 0000 7238  )...r4...r6...r8
+000023c0: 0000 0072 3a00 0000 7261 0000 0072 4800  ...r:...ra...rH.
+000023d0: 0000 7248 0000 0072 4900 0000 727d 0000  ..rH...rI...r}..
+000023e0: 002c 0100 0073 1000 0000 0401 0201 0401  .,...s..........
+000023f0: 0401 0401 0401 04fc 08ff 7a0c 5475 692e  ..........z.Tui.
+00002400: 6f6e 5f6d 6f75 6e74 7a11 2368 6f6d 652d  on_mountz.#home-
+00002410: 6578 6563 2d62 7574 746f 6e63 0100 0000  exec-buttonc....
+00002420: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00002430: 4300 0001 7312 0000 0064 017c 005f 007c  C...s....d.|._.|
+00002440: 00a0 01a1 0001 0064 0053 0072 5900 0000  .......d.S.rY...
+00002450: 2902 7260 0000 0072 3200 0000 7261 0000  ).r`...r2...ra..
+00002460: 0072 4800 0000 7248 0000 0072 4900 0000  .rH...rH...rI...
+00002470: da11 6f6e 5f62 7574 746f 6e5f 7072 6573  ..on_button_pres
+00002480: 7365 6436 0100 0073 0400 0000 0602 0c01  sed6...s........
+00002490: 7a15 5475 692e 6f6e 5f62 7574 746f 6e5f  z.Tui.on_button_
+000024a0: 7072 6573 7365 6446 a903 da08 6865 6164  pressedF....head
+000024b0: 6c65 7373 da04 7369 7a65 da0a 6175 746f  less..size..auto
+000024c0: 5f70 696c 6f74 72b4 0000 0072 3b00 0000  _pilotr....r;...
+000024d0: 72b5 0000 00fa 1674 7570 6c65 5b69 6e74  r......tuple[int
+000024e0: 2c20 696e 745d 207c 204e 6f6e 6572 b600  , int] | Noner..
+000024f0: 0000 fa1c 4175 746f 7069 6c6f 7443 616c  ....AutopilotCal
+00002500: 6c62 6163 6b54 7970 6520 7c20 4e6f 6e65  lbackType | None
+00002510: 6301 0000 0000 0000 0003 0000 0009 0000  c...............
+00002520: 000d 0000 0003 0000 0173 4201 0000 7a57  .........sB...zW
+00002530: 7400 8300 6a01 7c01 7c02 7c03 6401 8d03  t...j.|.|.|.d...
+00002540: 0100 5700 7c00 6a02 7252 7403 8300 7d04  ..W.|.j.rRt...}.
+00002550: 7c00 6a02 7254 7c00 6a04 7256 7c04 a005  |.j.rT|.j.rV|...
+00002560: 6402 7c00 6a06 9b00 6403 7c00 6a07 9b00  d.|.j...d.|.j...
+00002570: 6404 9d05 a101 0100 7408 a009 7c00 6a06  d.......t...|.j.
+00002580: a101 7d05 7c05 6405 1900 7d06 6700 7c05  ..}.|.d...}.g.|.
+00002590: a201 7c00 6a02 a201 7d07 740a 6a0b a00c  ..|.j...}.t.j...
+000025a0: a100 7d08 740a 6a0d a00e 740a a00f a100  ..}.t.j...t.....
+000025b0: 7c08 6406 1900 6702 a101 7c08 6406 3c00  |.d...g...|.d.<.
+000025c0: 740a a010 7c06 7c07 7c08 a103 0100 6400  t...|.|.|.....d.
+000025d0: 5300 6400 5300 6400 5300 6400 5300 7c00  S.d.S.d.S.d.S.|.
+000025e0: 6a02 729e 7403 8300 7d04 7c00 6a02 729f  j.r.t...}.|.j.r.
+000025f0: 7c00 6a04 72a0 7c04 a005 6402 7c00 6a06  |.j.r.|...d.|.j.
+00002600: 9b00 6403 7c00 6a07 9b00 6404 9d05 a101  ..d.|.j...d.....
+00002610: 0100 7408 a009 7c00 6a06 a101 7d05 7c05  ..t...|.j...}.|.
+00002620: 6405 1900 7d06 6700 7c05 a201 7c00 6a02  d...}.g.|...|.j.
+00002630: a201 7d07 740a 6a0b a00c a100 7d08 740a  ..}.t.j.....}.t.
+00002640: 6a0d a00e 740a a00f a100 7c08 6406 1900  j...t.....|.d...
+00002650: 6702 a101 7c08 6406 3c00 740a a010 7c06  g...|.d.<.t...|.
+00002660: 7c07 7c08 a103 0100 7700 7700 7700 7700  |.|.....w.w.w.w.
+00002670: 2907 4e72 b300 0000 7a10 5275 6e6e 696e  ).Nr....z.Runnin
+00002680: 6720 5b62 2063 7961 6e5d 7266 0000 007a  g [b cyan]rf...z
+00002690: 035b 2f5d 7201 0000 00da 0450 4154 4829  .[/]r......PATH)
+000026a0: 1172 4000 0000 7207 0000 0072 5f00 0000  .r@...r....r_...
+000026b0: 7209 0000 0072 6000 0000 da05 7072 696e  r....r`.....prin
+000026c0: 7472 3600 0000 725d 0000 0072 6700 0000  tr6...r]...rg...
+000026d0: da05 7370 6c69 74da 026f 73da 0765 6e76  ..split..os..env
+000026e0: 6972 6f6e 7264 0000 00da 0770 6174 6873  ironrd.....paths
+000026f0: 6570 7273 0000 00da 0667 6574 6377 64da  eprs.....getcwd.
+00002700: 0765 7865 6376 7065 2909 7245 0000 0072  .execvpe).rE...r
+00002710: b400 0000 72b5 0000 0072 b600 0000 da07  ....r....r......
+00002720: 636f 6e73 6f6c 655a 0e73 706c 6974 5f61  consoleZ.split_a
+00002730: 7070 5f6e 616d 655a 0c70 726f 6772 616d  pp_nameZ.program
+00002740: 5f6e 616d 65da 0961 7267 756d 656e 7473  _name..arguments
+00002750: da03 656e 7672 4600 0000 7248 0000 0072  ..envrF...rH...r
+00002760: 4900 0000 7207 0000 003b 0100 0073 3c00  I...r....;...s<.
+00002770: 0000 0207 1401 0602 0601 0c01 0401 1401  ................
+00002780: 04ff 0c04 0801 0e01 0a02 1c01 1201 04f3  ................
+00002790: 0802 06fe 0601 0c01 0401 1401 04ff 0c04  ................
+000027a0: 0801 0e01 0a02 1c01 1001 02f3 0402 7a07  ..............z.
+000027b0: 5475 692e 7275 6e63 0100 0000 0000 0000  Tui.runc........
+000027c0: 0000 0000 0200 0000 0800 0000 4300 0001  ............C...
+000027d0: 7330 0000 007a 077c 00a0 0074 01a1 017d  s0...z.|...t...}
+000027e0: 0157 006e 0a04 0074 0279 1101 0001 0001  .W.n...t.y......
+000027f0: 0059 0064 0053 0077 007c 01a0 03a1 0001  .Y.d.S.w.|......
+00002800: 0064 0053 0072 3f00 0000 2904 7280 0000  .d.S.r?...).r...
+00002810: 0072 2300 0000 7215 0000 0072 5300 0000  .r#...r....rS...
+00002820: 2902 7245 0000 0072 8600 0000 7248 0000  ).rE...r....rH..
+00002830: 0072 4800 0000 7249 0000 00da 1961 6374  .rH...rI.....act
+00002840: 696f 6e5f 666f 6375 735f 636f 6d6d 616e  ion_focus_comman
+00002850: 645f 7472 6565 5401 0000 730c 0000 0002  d_treeT...s.....
+00002860: 010e 010c 0106 0102 ff0c 037a 1d54 7569  ...........z.Tui
+00002870: 2e61 6374 696f 6e5f 666f 6375 735f 636f  .action_focus_co
+00002880: 6d6d 616e 645f 7472 6565 6301 0000 0000  mmand_treec.....
+00002890: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000028a0: 0000 0173 1e00 0000 7c00 a000 7401 a101  ...s....|...t...
+000028b0: 7d01 7c00 a002 7403 7c01 6a04 8301 a101  }.|...t.|.j.....
+000028c0: 0100 6400 5300 723f 0000 0029 0572 8000  ..d.S.r?...).r..
+000028d0: 0000 7229 0000 0072 7700 0000 7222 0000  ..r)...rw...r"..
+000028e0: 0072 8200 0000 2902 7245 0000 005a 0f63  .r....).rE...Z.c
+000028f0: 6f6d 6d61 6e64 5f62 7569 6c64 6572 7248  ommand_builderrH
+00002900: 0000 0072 4800 0000 7249 0000 00da 1861  ...rH...rI.....a
+00002910: 6374 696f 6e5f 7368 6f77 5f63 6f6d 6d61  ction_show_comma
+00002920: 6e64 5f69 6e66 6f5c 0100 0073 0400 0000  nd_info\...s....
+00002930: 0a01 1401 7a1c 5475 692e 6163 7469 6f6e  ....z.Tui.action
+00002940: 5f73 686f 775f 636f 6d6d 616e 645f 696e  _show_command_in
+00002950: 666f da03 7572 6c72 3700 0000 6302 0000  fo..urlr7...c...
+00002960: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00002970: 0043 0000 0173 0c00 0000 7400 7c01 8301  .C...s....t.|...
+00002980: 0100 6401 5300 2902 7a69 5669 7369 7420  ..d.S.).ziVisit 
+00002990: 7468 6520 6769 7665 6e20 5552 4c2c 2076  the given URL, v
+000029a0: 6961 2074 6865 206f 7065 7261 7469 6e67  ia the operating
+000029b0: 2073 7973 7465 6d2e 0a0a 2020 2020 2020   system...      
+000029c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000029d0: 2020 2020 7572 6c3a 2054 6865 2055 524c      url: The URL
+000029e0: 2074 6f20 7669 7369 742e 0a20 2020 2020   to visit..     
+000029f0: 2020 204e 2901 da08 6f70 656e 5f75 726c     N)...open_url
+00002a00: 2902 7245 0000 0072 c600 0000 7248 0000  ).rE...r....rH..
+00002a10: 0072 4800 0000 7249 0000 00da 0c61 6374  .rH...rI.....act
+00002a20: 696f 6e5f 7669 7369 7460 0100 0073 0200  ion_visit`...s..
+00002a30: 0000 0c06 7a10 5475 692e 6163 7469 6f6e  ....z.Tui.action
+00002a40: 5f76 6973 6974 2902 4e4e 290a 7234 0000  _visit).NN).r4..
+00002a50: 0072 3500 0000 7236 0000 0072 3900 0000  .r5...r6...r9...
+00002a60: 7238 0000 0072 3900 0000 729c 0000 0072  r8...r9...r....r
+00002a70: 3900 0000 724a 0000 0072 5800 0000 2904  9...rJ...rX...).
+00002a80: 72ab 0000 0072 2100 0000 724a 0000 0072  r....r!...rJ...r
+00002a90: ac00 0000 2908 72b4 0000 0072 3b00 0000  ....).r....r;...
+00002aa0: 72b5 0000 0072 b700 0000 72b6 0000 0072  r....r....r....r
+00002ab0: b800 0000 724a 0000 0072 5800 0000 7296  ....rJ...rX...r.
+00002ac0: 0000 0029 0472 c600 0000 7237 0000 0072  ...).r....r7...r
+00002ad0: 4a00 0000 7258 0000 0029 1472 9700 0000  J...rX...).r....
+00002ae0: 7298 0000 0072 9900 0000 7206 0000 00da  r....r....r.....
+00002af0: 085f 5f66 696c 655f 5f72 9400 0000 5a08  .__file__r....Z.
+00002b00: 4353 535f 5041 5448 7241 0000 00da 0b63  CSS_PATHrA.....c
+00002b10: 6c61 7373 6d65 7468 6f64 72b1 0000 0072  lassmethodr....r
+00002b20: 7d00 0000 720d 0000 0072 1700 0000 5a07  }...r....r....Z.
+00002b30: 5072 6573 7365 6472 b200 0000 7207 0000  Pressedr....r...
+00002b40: 0072 c400 0000 72c5 0000 0072 c800 0000  .r....r....r....
+00002b50: 729a 0000 0072 4800 0000 7248 0000 0072  r....rH...rH...r
+00002b60: 4600 0000 7249 0000 0072 9b00 0000 f300  F...rI...r......
+00002b70: 0000 7322 0000 0008 000e 0102 0602 0110  ..s"............
+00002b80: fb02 270c 0108 0e0a 0a0a 0102 0702 0102  ..'.............
+00002b90: 0112 fb0a 190a 0812 0472 9b00 0000 2942  .........r....)B
+00002ba0: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
+00002bb0: 0072 bc00 0000 7267 0000 0072 7000 0000  .r....rg...rp...
+00002bc0: da0a 636f 6e74 6578 746c 6962 7203 0000  ..contextlibr...
+00002bd0: 0072 0500 0000 da07 7061 7468 6c69 6272  .r......pathlibr
+00002be0: 0600 0000 da0a 7375 6270 726f 6365 7373  ......subprocess
+00002bf0: 7207 0000 005a 0a77 6562 6272 6f77 7365  r....Z.webbrowse
+00002c00: 7272 0800 0000 72c7 0000 005a 0c72 6963  rr....r....Z.ric
+00002c10: 682e 636f 6e73 6f6c 6572 0900 0000 5a10  h.consoler....Z.
+00002c20: 7269 6368 2e68 6967 686c 6967 6874 6572  rich.highlighter
+00002c30: 720a 0000 005a 0972 6963 682e 7465 7874  r....Z.rich.text
+00002c40: 720b 0000 005a 0774 6578 7475 616c 720c  r....Z.textualr.
+00002c50: 0000 0072 0d00 0000 5a0b 7465 7874 7561  ...r....Z.textua
+00002c60: 6c2e 6170 7072 0e00 0000 720f 0000 0072  l.appr....r....r
+00002c70: 1000 0000 5a0f 7465 7874 7561 6c2e 6269  ....Z.textual.bi
+00002c80: 6e64 696e 6772 1100 0000 5a12 7465 7874  ndingr....Z.text
+00002c90: 7561 6c2e 636f 6e74 6169 6e65 7273 7212  ual.containersr.
+00002ca0: 0000 0072 1300 0000 7214 0000 005a 1174  ...r....r....Z.t
+00002cb0: 6578 7475 616c 2e63 7373 2e71 7565 7279  extual.css.query
+00002cc0: 7215 0000 005a 0e74 6578 7475 616c 2e73  r....Z.textual.s
+00002cd0: 6372 6565 6e72 1600 0000 5a0f 7465 7874  creenr....Z.text
+00002ce0: 7561 6c2e 7769 6467 6574 7372 1700 0000  ual.widgetsr....
+00002cf0: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00002d00: 1b00 0000 5a14 7465 7874 7561 6c2e 7769  ....Z.textual.wi
+00002d10: 6467 6574 732e 7472 6565 721c 0000 0072  dgets.treer....r
+00002d20: 1e00 0000 5a0b 7275 6e5f 636f 6d6d 616e  ....Z.run_comman
+00002d30: 6472 1f00 0000 72b0 0000 0072 2000 0000  dr....r....r ...
+00002d40: 7221 0000 005a 1477 6964 6765 7473 2e63  r!...Z.widgets.c
+00002d50: 6f6d 6d61 6e64 5f69 6e66 6f72 2200 0000  ommand_infor"...
+00002d60: 5a14 7769 6467 6574 732e 636f 6d6d 616e  Z.widgets.comman
+00002d70: 645f 7472 6565 7223 0000 005a 0c77 6964  d_treer#...Z.wid
+00002d80: 6765 7473 2e66 6f72 6d72 2400 0000 5a17  gets.formr$...Z.
+00002d90: 7769 6467 6574 732e 6d75 6c74 6970 6c65  widgets.multiple
+00002da0: 5f63 686f 6963 6572 2500 0000 da0c 7665  _choicer%.....ve
+00002db0: 7273 696f 6e5f 696e 666f da09 696d 706f  rsion_info..impo
+00002dc0: 7274 6c69 6272 2800 0000 da12 696d 706f  rtlibr(.....impo
+00002dd0: 7274 6c69 625f 6d65 7461 6461 7461 7229  rtlib_metadatar)
+00002de0: 0000 0072 9b00 0000 7248 0000 0072 4800  ...r....rH...rH.
+00002df0: 0000 7248 0000 0072 4900 0000 da08 3c6d  ..rH...rI.....<m
+00002e00: 6f64 756c 653e 0100 0000 7342 0000 000c  odule>....sB....
+00002e10: 0008 0208 0108 010c 010c 010c 010c 010c  ................
+00002e20: 010c 020c 010c 0110 0114 010c 0114 010c  ................
+00002e30: 010c 011c 010c 010c 020c 0110 010c 010c  ................
+00002e40: 010c 010c 010a 020e 0108 0210 0300 7f14  ................
+00002e50: 4e                                       N
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/argparse.py` & `argparse-tui-0.1.3/src/argparse_tui/argparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -284,49 +284,54 @@
     )
 
 
 def add_tui_command(
     parser: argparse.ArgumentParser,
     command: str = DEFAULT_COMMAND_NAME,
     help: str = "Open Textual UI.",
-) -> None:
+    **kwargs: Any,
+) -> argparse._SubParsersAction:
     """
 
     Args:
         parser: the argparse parser
         command: name of the CLI command that will invoke the TUI (default=`tui`)
         help: help message for the argument
+        **kwargs: if subparsers do not already exist, create with these kwargs.
 
     Examples:
         >>> import argparse
         >>> from argparse_tui import add_tui_argument
         ...
         >>> parser = argparse.ArgumentParser()
         >>> subparsers = parser.add_subparsers()
         ...
-        >>> add_tui_command(parser)
+        >>> _ = add_tui_command(parser)
         ...
         >>> parser.print_usage()
         usage: __main__.py [-h] {tui} ...
     """
 
     subparsers: argparse._SubParsersAction
-    for action in parser._actions:
-        if isinstance(action, argparse._SubParsersAction):
-            subparsers = action
-            break
+    if parser._subparsers is None:
+        subparsers = parser.add_subparsers(**kwargs)
     else:
-        subparsers = parser.add_subparsers()
+        for action in parser._actions:
+            if isinstance(action, argparse._SubParsersAction):
+                subparsers = action
+                break
 
     tui_parser = subparsers.add_parser(
         command,
         description=argparse.SUPPRESS,
         help=help,
     )
     tui_parser.set_defaults(_parent_parser=parser)
 
     add_tui_argument(
         tui_parser,
         option_strings=["cmd_filter"],
         default=None,
         help="Command filter",
     )
+
+    return subparsers
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/detect_run_string.py` & `argparse-tui-0.1.3/src/argparse_tui/detect_run_string.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/run_command.py` & `argparse-tui-0.1.3/src/argparse_tui/run_command.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/schemas.py` & `argparse-tui-0.1.3/src/argparse_tui/schemas.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/tui.py` & `argparse-tui-0.1.3/src/argparse_tui/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
                 # ),
                 id="home-exec-preview",
             )
 
         yield Footer()
 
     def action_close_and_run(self) -> None:
+        self.action_copy_command_string()
         self.app.post_run_command_redacted = self.command_data.to_cli_string()
         self.app.post_run_command = self.command_data.to_cli_args()
         self.app.execute_on_exit = True
         self.app.exit()
 
     def action_copy_command_string(self) -> None:
         cmd: list[str] = (
@@ -135,25 +136,26 @@
             if sys.platform == "win32"
             else ["pbcopy"]
             if sys.platform == "darwin"
             else ["xclip", "-selection", "clipboard"]
             # if linux
         )
 
-        run(
-            cmd,
-            input=self.app_name
-            + " "
-            + " ".join(
-                shlex.quote(str(x))
-                for x in self.command_data.to_cli_args(redact_secret=True)
-            ),
-            text=True,
-            check=False,
-        )
+        with suppress(FileNotFoundError):
+            run(
+                cmd,
+                input=self.app_name
+                + " "
+                + " ".join(
+                    shlex.quote(str(x))
+                    for x in self.command_data.to_cli_args(redact_secret=True)
+                ),
+                text=True,
+                check=False,
+            )
 
     def action_exit(self) -> None:
         self.app.exit()
 
     def action_about(self) -> None:
         from .widgets.about import AboutDialog
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/tui.scss` & `argparse-tui-0.1.3/src/argparse_tui/tui.scss`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 2647 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 570a 0000  o..........dW...
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 570a 0000  o........E.dW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 4010 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 aa0f 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 aa0f 0000  o........E.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 ac00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 2246 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 c608 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 c608 0000  o........E.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6407  d.l.m.Z.m.Z...d.
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 8067 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 831f 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 831f 0000  o........E.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6406 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 2857 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 290b 0000  o..........d)...
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 290b 0000  o........E.d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc` & `argparse-tui-0.1.3/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 22:05:59 2023 UTC, .py size: 16529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c7f5 be64 9140 0000  o..........d.@..
+00000000: 6f0d 0d0a 0000 0000 fd45 c364 9140 0000  o........E.d.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 3601 0000 5500  .....@...s6...U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 5a02 6400 6403 6c02 6d03 5a03 0100  l.Z.d.d.l.m.Z...
 00000050: 6400 6404 6c04 6d05 5a05 6d06 5a06 6d07  d.d.l.m.Z.m.Z.m.
 00000060: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 0100  Z...d.d.l.m.Z...
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/about.py` & `argparse-tui-0.1.3/src/argparse_tui/widgets/about.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/command_info.py` & `argparse-tui-0.1.3/src/argparse_tui/widgets/command_info.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/command_tree.py` & `argparse-tui-0.1.3/src/argparse_tui/widgets/command_tree.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/form.py` & `argparse-tui-0.1.3/src/argparse_tui/widgets/form.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/multiple_choice.py` & `argparse-tui-0.1.3/src/argparse_tui/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui/widgets/parameter_controls.py` & `argparse-tui-0.1.3/src/argparse_tui/widgets/parameter_controls.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui.egg-info/PKG-INFO` & `argparse-tui-0.1.3/src/argparse_tui.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: argparse-tui
-Version: 0.1.2
-Summary: Display your Python argparse CLI as a TUI.
+Version: 0.1.3
+Summary: Display your Python argparse parser as a TUI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-Project-URL: Homepage, https://www.f2dv.com/code/r/argparse-tui/i
+Project-URL: Homepage, https://www.f2dv.com/r/argparse-tui
 Project-URL: Repository, https://www.github.com/fresh2dev/argparse-tui
 Project-URL: Funding, https://www.f2dv.com/fund
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 # argparse-tui
 
-> Display your Python argparse CLI as a TUI.
+> Display your Python argparse parser as a TUI.
 
-| Links         |                                                      |
-|---------------|------------------------------------------------------|
-| Code Repo     | https://www.github.com/fresh2dev/argparse-tui        |
-| Mirror Repo   | https://www.f2dv.com/code/r/argparse-tui             |
-| Documentation | https://www.f2dv.com/code/r/argparse-tui/i           |
-| Changelog     | https://www.f2dv.com/code/r/argparse-tui/i/changelog |
-| License       | https://www.f2dv.com/code/r/argparse-tui/i/license   |
-| Funding       | https://www.f2dv.com/fund                            |
-
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/releases)
-[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/releases)
-[![License](https://img.shields.io/github/license/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/argparse-tui/i/license)
+| Links         |                                               |
+|---------------|-----------------------------------------------|
+| Code Repo     | https://www.github.com/fresh2dev/argparse-tui |
+| Mirror Repo   | https://www.f2dv.com/r/argparse-tui           |
+| Documentation | https://www.f2dv.com/r/argparse-tui           |
+| Changelog     | https://www.f2dv.com/r/argparse-tui/changelog |
+| License       | https://www.f2dv.com/r/argparse-tui/license   |
+| Funding       | https://www.f2dv.com/fund                     |
+
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/r/argparse-tui/changelog)
+[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/r/argparse-tui/changelog)
+[![License](https://img.shields.io/github/license/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.f2dv.com/r/argparse-tui/license)
+[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/argparse-tui&Date)
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/argparse-tui/pulls)
-[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/argparse-tui&Date)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/argparse-tui?color=blue&style=for-the-badge)](https://pypi.org/project/argparse-tui)
-[![Docs Website](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/argparse-tui/i)](https://www.f2dv.com/code/r/argparse-tui/i)
-[![Coverage Website](https://img.shields.io/website?down_message=unavailable&label=coverage&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/argparse-tui/i/tests/coverage)](https://www.f2dv.com/code/r/argparse-tui/i/tests/coverage)
+[![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/argparse-tui?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/argparse-tui)
+[![Changelog](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/argparse-tui/changelog)](https://www.f2dv.com/r/argparse-tui/changelog)
 [![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.f2dv.com/fund)
 
 ---
 
 ## Overview
 
 This is a fork of the Textualize [Trogon TUI library](https://github.com/Textualize/trogon.git) that introduces these features:
 
 - add support for Python's argparse parsers
+    - add `--tui` flag as an argument
+    - or, add `tui` command to your subparser
+    - or, invoke the TUI with `invoke_tui(parser)`
 - remove support for Click
 - add ability for TUI parameter to filter subcommands
 - support for manually constructing schemas
 - support for argparse
 - add examples for yapx, myke, and sys.argv
 - support ommission of hidden parameters and subcommands from the TUI
 - support the redaction of sensitive "secret" values
@@ -85,17 +88,47 @@
 
 # Or, add tui command (my-cli tui)
 add_tui_command(parser, command="tui", help="Open Textual UI")
 
 parser.print_help()
 ```
 
+### `invoke_tui`
+
+argparse-tui offers this function to display a TUI based on the arguments of the given parser:
+
+```python
+import argparse
+
+from argparse_tui import invoke_tui
+
+parser = argparse.ArgumentParser(prog="echo")
+
+parser.add_argument("STRING", nargs="*")
+
+parser.add_argument(
+    "-n",
+    action="store_true",
+    help="do not output the trailing newline",
+)
+
+invoke_tui(parser)
+```
+
+In this way, `argparse` is not actually serving as an argument parser, but instead as the specification language for the TUI. Whoa.
+
+### ChatGPT and TUIview
+
+Given the structured help text output of some CLI program, it turns out ChatGPT is decent at implementing an equivalent CLI using a Python argparse parser. Whoaaa.
+
+Coupled with `invoke_tui`, this means that argparse-tui is capable of producing a TUI for any CLI. This is the idea behind a tool built using argparse-tui: [TUIview](https://github.com/fresh2dev/tuiview). It does not use ChatGPT itself, but I used ChatGPT to generate equivalent-enough argparse parsers for `git`, `rsync`, `grep`.
+
 ## Docs
 
-See more examples in the [reference docs](https://www.f2dv.com/code/r/argparse-tui/i/reference/).
+See more examples in the [reference docs](https://www.f2dv.com/r/argparse-tui/reference).
 
 
 ## Support
 
 *Brought to you by...*
 
 <a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

### Comparing `argparse-tui-0.1.2/src/argparse_tui.egg-info/SOURCES.txt` & `argparse-tui-0.1.3/src/argparse_tui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/src/argparse_tui.egg-info/requires.txt` & `argparse-tui-0.1.3/src/argparse_tui.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/tests/test_help_argparse.py` & `argparse-tui-0.1.3/tests/test_help_argparse.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.2/tests/test_run_command.py` & `argparse-tui-0.1.3/tests/test_run_command.py`

 * *Files identical despite different names*

