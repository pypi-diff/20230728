# Comparing `tmp/virtue-2023.7.4.tar.gz` & `tmp/virtue-2023.7.5.tar.gz`

## Comparing `virtue-2023.7.4.tar` & `virtue-2023.7.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.7.4/.coveragerc
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.7.4/.flake8
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 virtue-2023.7.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.7.4/.readthedocs.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.7.4/.testr.conf
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 virtue-2023.7.4/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/release.yml
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 virtue-2023.7.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/Makefile
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/api.rst
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/conf.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/index.rst
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/requirements.in
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/requirements.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 virtue-2023.7.4/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/__main__.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/_cli.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/loaders.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/locators.py
--rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/reporters.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_cli.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_loaders.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_locators.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_reporters.py
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/test_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/dynamic_test.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/failures_and_errors.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/failures_and_unexpected_passes.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/mixin.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/module_for_TestLoaders.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/module_for_TestObjectLocator.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/module_with_exception.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/no_tests.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_expected_failure.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_expected_failure_mispassing.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_successful_test.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/one_unsuccessful_test.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/repeated_similar_output.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/subtests.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/success_and_warning.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.7.4/virtue/tests/samples/two_unsuccessful_tests.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.7.4/COPYING
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.7.4/README.rst
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 virtue-2023.7.4/pyproject.toml
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 virtue-2023.7.4/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.7.5/.coveragerc
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.7.5/.flake8
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 virtue-2023.7.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.7.5/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.7.5/.testr.conf
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 virtue-2023.7.5/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 virtue-2023.7.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.5/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.7.5/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.7.5/.github/release.yml
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 virtue-2023.7.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.7.5/docs/Makefile
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.7.5/docs/api.rst
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 virtue-2023.7.5/docs/conf.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.7.5/docs/index.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 virtue-2023.7.5/docs/requirements.in
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 virtue-2023.7.5/docs/requirements.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 virtue-2023.7.5/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/__main__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/_cli.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/loaders.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/locators.py
+-rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/reporters.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/test_cli.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/test_loaders.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/test_locators.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/test_reporters.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/test_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/dynamic_test.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/failures_and_errors.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/failures_and_unexpected_passes.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/mixin.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/module_for_TestLoaders.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/module_for_TestObjectLocator.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/module_with_exception.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/no_tests.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/one_expected_failure.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/one_expected_failure_mispassing.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/one_successful_test.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/one_unsuccessful_test.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/repeated_similar_output.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/subtests.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/success_and_warning.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.7.5/virtue/tests/samples/two_unsuccessful_tests.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.7.5/COPYING
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.7.5/README.rst
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 virtue-2023.7.5/pyproject.toml
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 virtue-2023.7.5/PKG-INFO
```

### Comparing `virtue-2023.7.4/.flake8` & `virtue-2023.7.5/.flake8`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/.pre-commit-config.yaml` & `virtue-2023.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/noxfile.py` & `virtue-2023.7.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/.github/SECURITY.md` & `virtue-2023.7.5/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/.github/workflows/ci.yml` & `virtue-2023.7.5/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -30,18 +30,15 @@
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
-            nox --list-sessions |
-            grep '^* ' |
-            cut -d ' ' -f 2- |
-            jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
+            nox --list-sessions --json | jq '[.[].session]'
           )
 
   ci:
     needs: list
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
```

### Comparing `virtue-2023.7.4/docs/Makefile` & `virtue-2023.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/docs/conf.py` & `virtue-2023.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/docs/requirements.txt` & `virtue-2023.7.5/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/_cli.py` & `virtue-2023.7.5/virtue/_cli.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/loaders.py` & `virtue-2023.7.5/virtue/loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/locators.py` & `virtue-2023.7.5/virtue/locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/reporters.py` & `virtue-2023.7.5/virtue/reporters.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/runner.py` & `virtue-2023.7.5/virtue/runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/tests/test_cli.py` & `virtue-2023.7.5/virtue/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/tests/test_loaders.py` & `virtue-2023.7.5/virtue/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/tests/test_locators.py` & `virtue-2023.7.5/virtue/tests/test_locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/tests/test_reporters.py` & `virtue-2023.7.5/virtue/tests/test_reporters.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/tests/test_runner.py` & `virtue-2023.7.5/virtue/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/virtue/tests/samples/subtests.py` & `virtue-2023.7.5/virtue/tests/samples/subtests.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/COPYING` & `virtue-2023.7.5/COPYING`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/README.rst` & `virtue-2023.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/pyproject.toml` & `virtue-2023.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `virtue-2023.7.4/PKG-INFO` & `virtue-2023.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtue
-Version: 2023.7.4
+Version: 2023.7.5
 Summary: After trial comes virtue. A test runner for good.
 Project-URL: Documentation, https://virtue.readthedocs.io/
 Project-URL: Homepage, https://github.com/Julian/Virtue
 Project-URL: Issues, https://github.com/Julian/Virtue/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/Virtue
 Author: Julian Berman
```

