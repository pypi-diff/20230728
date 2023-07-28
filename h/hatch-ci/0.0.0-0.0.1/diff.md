# Comparing `tmp/hatch_ci-0.0.0.tar.gz` & `tmp/hatch_ci-0.0.1.tar.gz`

## Comparing `hatch_ci-0.0.0.tar` & `hatch_ci-0.0.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/.gitattributes
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/Makefile
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/.github/workflows/beta.yml
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/.github/workflows/master.yml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/.github/workflows/tags.yml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/.gitattributes
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/.gitignore
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/HISTORY.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/LICENSE.txt
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/pyproject.toml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/.github/dependabot.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/.github/workflows/build.yml
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/.github/workflows/test.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch_vcs/__about__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch_vcs/__init__.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch_vcs/build_hook.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch_vcs/hooks.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch_vcs/metadata_hook.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch_vcs/vcs_utils.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/hatch_vcs/version_source.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/tests/__init__.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/tests/conftest.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/tests/test_build.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/tests/test_build_config.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/tests/test_metadata_config.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/tests/test_version_config.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/hatch-vcs/tests/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/__about__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/__main__.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/build_hook.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/metadata_hook.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/tests/conftest.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/tests/requirements.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/README.md
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 hatch_ci-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.gitattributes
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/Makefile
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.github/workflows/master.yml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.github/workflows/tags.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.gitattributes
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.gitignore
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/HISTORY.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/LICENSE.txt
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/pyproject.toml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.github/dependabot.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/.github/workflows/test.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/__about__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/build_hook.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/hooks.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/metadata_hook.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/vcs_utils.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/hatch_vcs/version_source.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/__init__.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/conftest.py
+-rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_build.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_build_config.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_metadata_config.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/test_version_config.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/hatch-vcs/tests/utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/__main__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     8240 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/test_scm.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/README.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 hatch_ci-0.0.1/PKG-INFO
```

### Comparing `hatch_ci-0.0.0/.github/workflows/beta.yml` & `hatch_ci-0.0.1/.github/workflows/beta.yml`

 * *Files 23% similar despite different names*

```diff
@@ -32,41 +32,38 @@
       - name: Install dependencies
         shell: bash
         run: |
             python -m pip install --upgrade pip
             pip install setuptools build wheel twine
             pip install -r tests/requirements.txt
 
-      - name: Lint tests (flake8)
+      - name: Lint tests (ruff)
         shell: bash
         env:
           PYTHONPATH: src
         run: |
-            # stop the build if there are Python syntax errors or undefined names
-            flake8 src/setuptools_github --count --select=E9,F63,F7,F82 --show-source --statistics
-            # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-            flake8 src/setuptools_github --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+          ruff check src
 
       - name: Static tests (mypy)
         shell: bash
         env:
           PYTHONPATH: src
           OUTDIR: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
         run: |
-          mypy src/setuptools_github \
+          mypy src \
             --no-incremental --xslt-html-report $OUTDIR/mypy
 
       - name: Runtime tests (unitest, coverage etc.)
         shell: bash
         env:
           PYTHONPATH: src
           OUTDIR: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
         run: |
           py.test \
-              --cov=setuptools_github \
+              --cov=hatch_ci \
               --cov-report=html:$OUTDIR/coverage --cov-report=xml:$OUTDIR/coverage.xml \
               --junitxml=$OUTDIR/junit/junit.xml --html=$OUTDIR/junit/junit.html --self-contained-html \
             tests
 
       - name: Upload pytest test results
         uses: actions/upload-artifact@v2
         with:
@@ -81,18 +78,20 @@
           token: ${{ secrets.CODECOV_TOKEN }}
           fail_ci_if_error: true
           files: build/qa-${{ matrix.python-version }}-${{ matrix.os}}/coverage.xml
           verbose: true
 
       - name: Build wheel package
         env:
-          PYTHONPATH: .
+          PYTHONPATH: src
           GITHUB_DUMP: ${{ toJson(github) }}
         run: |
-          python -m build
+          # this is special for hatch-ci plugin
+          python -m pip install --edit .
+          python -m build -n
 
       - name: Publish packages to pypi (beta)
         shell: bash
         env:
           TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
           TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
         run: |
```

### Comparing `hatch_ci-0.0.0/.github/workflows/master.yml` & `hatch_ci-0.0.1/.github/workflows/master.yml`

 * *Files 13% similar despite different names*

```diff
@@ -32,41 +32,38 @@
       - name: Install dependencies
         shell: bash
         run: |
             python -m pip install --upgrade pip
             pip install setuptools build wheel twine
             pip install -r tests/requirements.txt
 
-      - name: Lint tests (flake8)
+      - name: Lint tests (ruff)
         shell: bash
         env:
           PYTHONPATH: src
         run: |
-            # stop the build if there are Python syntax errors or undefined names
-            flake8 src/setuptools_github --count --select=E9,F63,F7,F82 --show-source --statistics
-            # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-            flake8 src/setuptools_github --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+          ruff check src
 
       - name: Static tests (mypy)
         shell: bash
         env:
           PYTHONPATH: src
           OUTDIR: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
         run: |
-          mypy src/setuptools_github \
+          mypy src \
             --no-incremental --xslt-html-report $OUTDIR/mypy
 
       - name: Runtime tests (unitest, coverage etc.)
         shell: bash
         env:
           PYTHONPATH: src
           OUTDIR: build/qa-${{ matrix.python-version }}-${{ matrix.os}}
         run: |
           py.test \
-              --cov=setuptools_github \
+              --cov=hatch_ci \
               --cov-report=html:$OUTDIR/coverage --cov-report=xml:$OUTDIR/coverage.xml \
               --junitxml=$OUTDIR/junit/junit.xml --html=$OUTDIR/junit/junit.html --self-contained-html \
             tests
 
       - name: Upload pytest test results
         uses: actions/upload-artifact@v2
         with:
```

### Comparing `hatch_ci-0.0.0/.github/workflows/tags.yml` & `hatch_ci-0.0.1/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/HISTORY.md` & `hatch_ci-0.0.1/hatch-vcs/HISTORY.md`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/LICENSE.txt` & `hatch_ci-0.0.1/hatch-vcs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/README.md` & `hatch_ci-0.0.1/hatch-vcs/README.md`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/hatch.toml` & `hatch_ci-0.0.1/hatch-vcs/hatch.toml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/pyproject.toml` & `hatch_ci-0.0.1/hatch-vcs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/.github/workflows/build.yml` & `hatch_ci-0.0.1/hatch-vcs/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/.github/workflows/test.yml` & `hatch_ci-0.0.1/hatch-vcs/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/hatch_vcs/build_hook.py` & `hatch_ci-0.0.1/hatch-vcs/hatch_vcs/build_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/hatch_vcs/metadata_hook.py` & `hatch_ci-0.0.1/hatch-vcs/hatch_vcs/metadata_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/hatch_vcs/version_source.py` & `hatch_ci-0.0.1/hatch-vcs/hatch_vcs/version_source.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/tests/conftest.py` & `hatch_ci-0.0.1/hatch-vcs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/tests/test_build.py` & `hatch_ci-0.0.1/hatch-vcs/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/tests/test_build_config.py` & `hatch_ci-0.0.1/hatch-vcs/tests/test_build_config.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/tests/test_metadata_config.py` & `hatch_ci-0.0.1/hatch-vcs/tests/test_metadata_config.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/tests/test_version_config.py` & `hatch_ci-0.0.1/hatch-vcs/tests/test_version_config.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/hatch-vcs/tests/utils.py` & `hatch_ci-0.0.1/hatch-vcs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/src/hatch_ci/__main__.py` & `hatch_ci-0.0.1/src/hatch_ci/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
+
 import argparse
 import functools
 import logging
+import sys
 from typing import Any
 
+from . import tools
 
 log = logging.getLogger(__name__)
 
 
-def parse_args(args: str|None = None, testmode: bool = False) -> dict[str, Any]:
+def parse_args(args: str | None = None, testmode: bool = False) -> dict[str, Any]:
     """parses args from the command line
 
     Args:
         args: command line arguments or None to pull from sys.argv
         testmode: internal flag, if set will not SystemExit but will
                   raises tools.AbortExecution
     """
+
     class F(
         argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter
     ):
         pass
 
-    parser = argparse.ArgumentParser(
-        formatter_class=F, description=__doc__)
+    parser = argparse.ArgumentParser(formatter_class=F, description=__doc__)
 
     parser.add_argument("-n", "--dry-run", dest="dryrun", action="store_true")
     parser.add_argument("-v", "--verbose", action="store_true")
 
     options = parser.parse_args(args)
 
     def error(message, explain="", hint="", parser=None, testmode=False):
@@ -41,16 +44,16 @@
         if hint:
             out.append("hint:")
             out.extend(tools.indent(hint).split("\n"))
 
         if testmode:
             raise tools.AbortExecution(message, explain, hint)
         else:
-            print()
-            print("\n".join(out), file=sys.stderr)
+            print()  # noqa: T201
+            print("\n".join(out), file=sys.stderr)  # noqa: T201
             raise SystemExit(2)
 
     options.error = functools.partial(error, parser=parser, testmode=testmode)
 
     logging.basicConfig(
         format="%(levelname)s:%(name)s:(dry-run) %(message)s"
         if options.dryrun
```

### Comparing `hatch_ci-0.0.0/LICENSE.txt` & `hatch_ci-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.0/README.md` & `hatch_ci-0.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,34 +33,34 @@
 
 ## Global dependency
 
 Ensure `hatch-ci` is defined within the `build-system.requires` field in your `pyproject.toml` file.
 
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
```

### Comparing `hatch_ci-0.0.0/pyproject.toml` & `hatch_ci-0.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [project]
 name = "hatch-ci"
 dynamic = ["version"]
 description = 'Hatch plugin for ci system versioning'
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
+packages = ["src/hatch_ci"]
 keywords = [
   "git",
   "hatch",
   "mercurial",
   "plugin",
   "scm",
   "version",
@@ -34,33 +35,27 @@
   "hatchling>=1.1.0",
 ]
 
 [project.scripts]
 hatch-ci = "hatch_ci:__main__.main"
 
 [project.urls]
-#Funding = "https://github.com/sponsors/ofek"
-#History = "https://github.com/ofek/hatch-vcs/blob/master/HISTORY.md"
 Issues = "https://github.com/cav71/hatch-ci/issues"
 Source = "https://github.com/cav71/hatch-ci"
 
 [project.entry-points.hatch]
 ci = "hatch_ci.hooks"
 
 [tool.hatch.version]
-path = "src/hatch_ci/__init__.py"
-
-[tool.black]
-target-version = ["py38"]
-line-length = 120
-skip-string-normalization = true
+source = "ci"
+version-file = "src/hatch_ci/__init__.py"
 
 [tool.ruff]
 target-version = "py38"
-line-length = 120
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
 known-first-party = ["hatch_ci"]
 
 [tool.ruff.flake8-quotes]
-inline-quotes = "single"
+inline-quotes = "double"
+
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use relative imports and assertions
 "tests/**/*" = ["TID252", "S101"]
```

### Comparing `hatch_ci-0.0.0/PKG-INFO` & `hatch_ci-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.0
+Version: 0.0.1
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,mercurial,plugin,scm,version
@@ -55,34 +55,34 @@
 
 ## Global dependency
 
 Ensure `hatch-ci` is defined within the `build-system.requires` field in your `pyproject.toml` file.
 
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
```

