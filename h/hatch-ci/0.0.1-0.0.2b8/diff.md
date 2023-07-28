# Comparing `tmp/hatch_ci-0.0.1.tar.gz` & `tmp/hatch_ci-0.0.2b8.tar.gz`

## Comparing `hatch_ci-0.0.1.tar` & `hatch_ci-0.0.2b8.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.gitattributes
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/Makefile
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.github/workflows/beta.yml
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.github/workflows/master.yml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.github/workflows/tags.yml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.gitattributes
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.gitignore
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/HISTORY.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/LICENSE.txt
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/pyproject.toml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.github/dependabot.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.github/workflows/build.yml
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.github/workflows/test.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/__about__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/__init__.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/build_hook.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/hooks.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/metadata_hook.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/vcs_utils.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/version_source.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/__init__.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/conftest.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_build.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_build_config.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_metadata_config.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_version_config.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/utils.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/__main__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/test_scm.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/README.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.gitattributes
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/Makefile
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.github/workflows/master.yml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    18965 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    26555 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943___main___py.html
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    82207 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    84461 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    22034 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    19337 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/__main__.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    44011 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    49030 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    14045 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/build/qa-3.9-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/__main__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/test_scm.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/LICENSE.txt
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/README.md
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/pyproject.toml
+-rw-r--r--   0        0        0     7977 2020-02-02 00:00:00.000000 hatch_ci-0.0.2b8/PKG-INFO
```

### Comparing `hatch_ci-0.0.1/.pre-commit-config.yaml` & `hatch_ci-0.0.2b8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/.github/workflows/beta.yml` & `hatch_ci-0.0.2b8/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/.github/workflows/master.yml` & `hatch_ci-0.0.2b8/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/.github/workflows/tags.yml` & `hatch_ci-0.0.2b8/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/hatch-vcs/LICENSE.txt` & `hatch_ci-0.0.2b8/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
 
-Copyright (c) 2022-present Ofek Lev <oss@ofek.dev>
+Copyright (c) 2022-present Antonio Cavallo <a.cavallo@cavallinux.eu>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hatch_ci-0.0.1/hatch-vcs/README.md` & `hatch_ci-0.0.2b8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-# hatch-vcs
+# hatch-ci
 
-| | |
-| --- | --- |
-| CI/CD | [![CI - Test](https://github.com/ofek/hatch-vcs/actions/workflows/test.yml/badge.svg)](https://github.com/ofek/hatch-vcs/actions/workflows/test.yml) [![CD - Build](https://github.com/ofek/hatch-vcs/actions/workflows/build.yml/badge.svg)](https://github.com/ofek/hatch-vcs/actions/workflows/build.yml) |
-| Package | [![PyPI - Version](https://img.shields.io/pypi/v/hatch-vcs.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/hatch-vcs/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-vcs.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/hatch-vcs/) |
-| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/ofek?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/ofek) |
+[![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
+[![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions)
+[![Coverage](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg)](Coverage)
+
+[![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
 -----
 
-This provides a plugin for [Hatch](https://github.com/pypa/hatch) that uses your preferred version control system (like Git) to determine project versions.
+This provides a plugin to [Hatch](https://github.com/pypa/hatch) leveraging a CI/CD system (github at the moment)
+to deliver packages to [PyPi](https://pypi.org).
+
+> **NOTE**: this is heavily inspired from  [hatch-vcs](https://github.com/ofek/hatch-vcs)
+
 
 **Table of Contents**
 
 - [Global dependency](#global-dependency)
 - [Version source](#version-source)
   - [Version source options](#version-source-options)
   - [Version source environment variables](#version-source-environment-variables)
@@ -23,38 +29,38 @@
   - [Metadata hook options](#metadata-hook-options)
     - [URLs](#urls)
   - [Example](#example)
 - [License](#license)
 
 ## Global dependency
 
-Ensure `hatch-vcs` is defined within the `build-system.requires` field in your `pyproject.toml` file.
+Ensure `hatch-ci` is defined within the `build-system.requires` field in your `pyproject.toml` file.
 
 ```toml
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
+requires = ["hatchling", "hatch-ci"]
 build-backend = "hatchling.build"
 ```
 
 ## Version source
 
 The [version source plugin](https://hatch.pypa.io/latest/plugins/version-source/reference/) name is `vcs`.
 
 - ***pyproject.toml***
 
     ```toml
     [tool.hatch.version]
-    source = "vcs"
+    source = "ci"
     ```
 
 - ***hatch.toml***
 
     ```toml
     [version]
-    source = "vcs"
+    source = "ci"
     ```
 
 ### Version source options
 
 | Option | Type | Default | Description |
 | --- | --- | --- | --- |
 | `tag-pattern` | `str` | see [code](https://github.com/pypa/setuptools_scm/blob/v6.4.0/src/setuptools_scm/config.py#L13) | A regular expression used to extract the version part from VCS tags. The pattern needs to contain either a single match group, or a group named `version`, that captures the actual version information. |
@@ -68,22 +74,23 @@
 ## Build hook
 
 The [build hook plugin](https://hatch.pypa.io/latest/plugins/build-hook/reference/) name is `vcs`.
 
 - ***pyproject.toml***
 
     ```toml
-    [tool.hatch.build.hooks.vcs]
+    [tool.hatch.version]
     version-file = "_version.py"
+    version-file = "src/hatch_ci/__init__.py"
     ```
 
 - ***hatch.toml***
 
     ```toml
-    [build.hooks.vcs]
+    [build.version]
     version-file = "_version.py"
     ```
 
 Building or installing when the latest tag is ``v1.2.3`` will generate the file
 
 - ***_version.py***
```

### Comparing `hatch_ci-0.0.1/hatch-vcs/pyproject.toml` & `hatch_ci-0.0.2b8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,61 @@
 [build-system]
-requires = ["hatchling>=1.1.0"]
+requires = ["hatchling>=1.1.0", "hatch-ci", "typing-extensions"]
 build-backend = "hatchling.build"
 
 [project]
-name = "hatch-vcs"
+name = "hatch-ci"
 dynamic = ["version"]
-description = 'Hatch plugin for versioning with your preferred VCS'
+description = "Hatch plugin for ci system versioning"
 readme = "README.md"
 license = { text = "MIT" }
-requires-python = ">= 3.7"
+requires-python = ">= 3.8"
+packages = ["src/hatch_ci"]
 keywords = [
   "git",
   "hatch",
-  "mercurial",
   "plugin",
   "scm",
-  "vcs",
   "version",
 ]
 authors = [
-  { name = "Ofek Lev", email = "oss@ofek.dev" },
+  { name = "Antonio Cavallo", email = "a.cavallo@cavallinux.eu" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "hatchling>=1.1.0",
-  "setuptools-scm>=6.4.0",
+  "typing-extensions",
 ]
 
+[project.scripts]
+hatch-ci = "hatch_ci:__main__.main"
+
 [project.urls]
-Funding = "https://github.com/sponsors/ofek"
-History = "https://github.com/ofek/hatch-vcs/blob/master/HISTORY.md"
-Issues = "https://github.com/ofek/hatch-vcs/issues"
-Source = "https://github.com/ofek/hatch-vcs"
+Issues = "https://github.com/cav71/hatch-ci/issues"
+Source = "https://github.com/cav71/hatch-ci"
 
 [project.entry-points.hatch]
-vcs = "hatch_vcs.hooks"
+ci = "hatch_ci.hooks"
 
 [tool.hatch.version]
-path = "hatch_vcs/__about__.py"
-
-[tool.black]
-target-version = ["py37"]
-line-length = 120
-skip-string-normalization = true
+source = "ci"
+version-file = "src/hatch_ci/__init__.py"
 
 [tool.ruff]
-target-version = "py37"
-line-length = 120
+target-version = "py38"
+line-length = 88
 select = [
   "A",
   "B",
   "C",
   "E",
   "F",
   "FBT",
@@ -76,28 +71,29 @@
 ]
 ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Ignore McCabe complexity
   "C901",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
+  "FBT001", "FBT002", "FBT003",
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["hatch_vcs"]
+known-first-party = ["hatch_ci"]
 
 [tool.ruff.flake8-quotes]
-inline-quotes = "single"
+inline-quotes = "double"
+
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use relative imports and assertions
 "tests/**/*" = ["TID252", "S101"]
@@ -109,24 +105,24 @@
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 warn_no_return = false
 warn_unused_ignores = true
 
 [tool.coverage.run]
-source_pkgs = ["hatch_vcs", "tests"]
+source_pkgs = ["hatch_ci", "tests"]
 branch = true
 parallel = true
 omit = [
-  "hatch_vcs/__about__.py",
+  "hatch_ci/__about__.py",
 ]
 
 [tool.coverage.paths]
-hatch_vcs = ["hatch_vcs", "*/hatch-vcs/hatch_vcs"]
-tests = ["tests", "*/hatch-vcs/tests"]
+hatch_ci = ["hatch_ci", "*/hatch-ci/hatch_ci"]
+tests = ["tests", "*/hatch-ci/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```

### Comparing `hatch_ci-0.0.1/src/hatch_ci/__main__.py` & `hatch_ci-0.0.2b8/src/hatch_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/src/hatch_ci/scm.py` & `hatch_ci-0.0.2b8/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/src/hatch_ci/tools.py` & `hatch_ci-0.0.2b8/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.2b8/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/tests/conftest.py` & `hatch_ci-0.0.2b8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/tests/test_scm.py` & `hatch_ci-0.0.2b8/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/tests/test_tools.py` & `hatch_ci-0.0.2b8/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.1/README.md` & `hatch_ci-0.0.2b8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: hatch-ci
+Version: 0.0.2b8
+Summary: Hatch plugin for ci system versioning
+Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
+Project-URL: Source, https://github.com/cav71/hatch-ci
+Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
+License: MIT
+License-File: LICENSE.txt
+Keywords: git,hatch,plugin,scm,version
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Requires-Dist: hatchling>=1.1.0
+Requires-Dist: typing-extensions
+Description-Content-Type: text/markdown
+
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![Build](https://github.com/cav71/hatch-ci/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions)
 [![Coverage](https://codecov.io/gh/cav71/hatch-ci/branch/master/graph/badge.svg)](Coverage)
 
@@ -74,22 +97,23 @@
 ## Build hook
 
 The [build hook plugin](https://hatch.pypa.io/latest/plugins/build-hook/reference/) name is `vcs`.
 
 - ***pyproject.toml***
 
     ```toml
-    [tool.hatch.build.hooks.vcs]
+    [tool.hatch.version]
     version-file = "_version.py"
+    version-file = "src/hatch_ci/__init__.py"
     ```
 
 - ***hatch.toml***
 
     ```toml
-    [build.hooks.vcs]
+    [build.version]
     version-file = "_version.py"
     ```
 
 Building or installing when the latest tag is ``v1.2.3`` will generate the file
 
 - ***_version.py***
```

