# Comparing `tmp/shtab-1.6.3.tar.gz` & `tmp/shtab-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shtab-1.6.3.tar", last modified: Mon Jul 24 15:17:58 2023, max compression
+gzip compressed data, was "shtab-1.6.4.tar", last modified: Fri Jul 28 20:44:50 2023, max compression
```

## Comparing `shtab-1.6.3.tar` & `shtab-1.6.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.011869 shtab-1.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.003869 shtab-1.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.003869 shtab-1.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-24 15:17:37.000000 shtab-1.6.3/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-24 15:17:37.000000 shtab-1.6.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-24 15:17:37.000000 shtab-1.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-24 15:17:37.000000 shtab-1.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-24 15:17:37.000000 shtab-1.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-24 15:17:37.000000 shtab-1.6.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-24 15:17:58.011869 shtab-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-24 15:17:37.000000 shtab-1.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/pydoc-markdown.yml
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/pydoc_markdown_shtab.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-24 15:17:37.000000 shtab-1.6.3/docs/use.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-07-24 15:17:37.000000 shtab-1.6.3/examples/customcomplete.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-24 15:17:37.000000 shtab-1.6.3/examples/docopt-greeter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-07-24 15:17:37.000000 shtab-1.6.3/examples/pathcomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-07-24 15:17:37.000000 shtab-1.6.3/meta/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-24 15:17:37.000000 shtab-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:17:58.011869 shtab-1.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.007869 shtab-1.6.3/shtab/
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-24 15:17:37.000000 shtab-1.6.3/shtab/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.011869 shtab-1.6.3/shtab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 15:17:57.000000 shtab-1.6.3/shtab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:58.011869 shtab-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:17:37.000000 shtab-1.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-24 15:17:37.000000 shtab-1.6.3/tests/test_shtab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.351006 shtab-1.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-28 20:44:33.000000 shtab-1.6.4/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-28 20:44:33.000000 shtab-1.6.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 20:44:33.000000 shtab-1.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-28 20:44:33.000000 shtab-1.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-28 20:44:33.000000 shtab-1.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-28 20:44:33.000000 shtab-1.6.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-28 20:44:50.355006 shtab-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-28 20:44:33.000000 shtab-1.6.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-28 20:44:33.000000 shtab-1.6.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-28 20:44:33.000000 shtab-1.6.4/docs/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-28 20:44:33.000000 shtab-1.6.4/docs/pydoc_markdown_shtab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-28 20:44:33.000000 shtab-1.6.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-28 20:44:33.000000 shtab-1.6.4/docs/use.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-07-28 20:44:33.000000 shtab-1.6.4/examples/customcomplete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-28 20:44:33.000000 shtab-1.6.4/examples/docopt-greeter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-07-28 20:44:33.000000 shtab-1.6.4/examples/pathcomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)    16145 2023-07-28 20:44:33.000000 shtab-1.6.4/meta/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-28 20:44:33.000000 shtab-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:44:50.355006 shtab-1.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/shtab/
+-rw-r--r--   0 runner    (1001) docker     (123)    30608 2023-07-28 20:44:33.000000 shtab-1.6.4/shtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 20:44:33.000000 shtab-1.6.4/shtab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:44:50.000000 shtab-1.6.4/shtab/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-28 20:44:33.000000 shtab-1.6.4/shtab/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 20:44:33.000000 shtab-1.6.4/shtab/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/shtab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-28 20:44:50.000000 shtab-1.6.4/shtab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 20:44:50.000000 shtab-1.6.4/shtab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:44:50.000000 shtab-1.6.4/shtab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 20:44:50.000000 shtab-1.6.4/shtab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 20:44:50.000000 shtab-1.6.4/shtab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:44:50.000000 shtab-1.6.4/shtab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:50.355006 shtab-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:44:33.000000 shtab-1.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-28 20:44:33.000000 shtab-1.6.4/tests/test_shtab.py
```

### Comparing `shtab-1.6.3/.github/workflows/comment-bot.yml` & `shtab-1.6.4/.github/workflows/comment-bot.yml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/.github/workflows/test.yml` & `shtab-1.6.4/.github/workflows/test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,14 @@
 name: Test
 on:
   push:
   pull_request:
   schedule: [{cron: '0 9 * * 1'}]  # M H d m w (Mondays at 9:00)
   workflow_dispatch:
 jobs:
-  check:
-    if: github.event_name != 'pull_request' || !contains('OWNER,MEMBER,COLLABORATOR', github.event.pull_request.author_association)
-    name: Check
-    runs-on: ubuntu-latest
-    steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.x'
-    - name: set PYSHA
-      run: echo "PYSHA=$(python -VV | sha256sum | cut -d' ' -f1)" >> $GITHUB_ENV
-    - uses: actions/cache@v3
-      with:
-        path: ~/.cache/pre-commit
-        key: pre-commit|${{ env.PYSHA }}|${{ hashFiles('.pre-commit-config.yaml') }}
-    - run: pip install -U pre-commit
-    - uses: reviewdog/action-setup@v1
-    - if: github.event_name == 'push' || github.event_name == 'pull_request'
-      name: comment
-      run: |
-        if [[ $EVENT == pull_request ]]; then
-          REPORTER=github-pr-review
-        else
-          REPORTER=github-check
-        fi
-        pre-commit run -a todo | reviewdog -efm="%f:%l: %m" -name=TODO -tee -reporter=$REPORTER -filter-mode nofilter
-        pre-commit run -a flake8 | reviewdog -f=pep8 -name=flake8 -tee -reporter=$REPORTER -filter-mode nofilter
-        pre-commit run -a mypy | reviewdog -efm="%f:%l: %m" -name=mypy -tee -reporter=$REPORTER -filter-mode nofilter
-      env:
-        REVIEWDOG_GITHUB_API_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        EVENT: ${{ github.event_name }}
-    - run: pre-commit run -a --show-diff-on-failure
   test:
     if: github.event_name != 'pull_request' || !contains('OWNER,MEMBER,COLLABORATOR', github.event.pull_request.author_association)
     name: Test py${{ matrix.python }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python: [3.7, 3.11]
@@ -52,15 +20,15 @@
       with:
         python-version: ${{ matrix.python }}
     - name: Install
       run: pip install -U -e .[dev]
     - run: pytest
     - uses: codecov/codecov-action@v3
   deploy:
-    needs: [check, test]
+    needs: test
     name: PyPI Deploy
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
         token: ${{ secrets.GH_TOKEN || github.token }}
@@ -76,15 +44,15 @@
     - if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       name: Release
       run: |
         changelog=$(git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD)
         tag="${GITHUB_REF#refs/tags/}"
         gh release create --title "shtab $tag beta" --draft --notes "$changelog" "$tag" dist/${{ steps.dist.outputs.whl }} dist/${{ steps.dist.outputs.targz }}
       env:
-        GH_TOKEN: ${{ github.token }}
+        GH_TOKEN: ${{ secrets.GH_TOKEN || github.token }}
     - name: Docs
       run: |
         pushd docs
         pip install -U -r requirements.txt
         PYTHONPATH=. pydoc-markdown --build --site-dir=../../../dist/site
         popd
     - if: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') || github.event_name == 'workflow_dispatch' }}
```

### Comparing `shtab-1.6.3/.pre-commit-config.yaml` & `shtab-1.6.4/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 default_language_version:
   python: python3
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: check-added-large-files
+  - id: check-builtin-literals
   - id: check-case-conflict
   - id: check-docstring-first
   - id: check-executables-have-shebangs
-  - id: check-toml
   - id: check-merge-conflict
+  - id: check-toml
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: sort-simple-yaml
   - id: trailing-whitespace
 - repo: local
@@ -35,21 +36,24 @@
     - flake8-bugbear
     - flake8-comprehensions
     - flake8-debugger
     - flake8-isort
     - flake8-pyproject
     - flake8-string-format
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.3.0
+  rev: v1.4.1
   hooks:
   - id: mypy
     additional_dependencies: [types-setuptools]
 - repo: https://github.com/google/yapf
-  rev: v0.33.0
+  rev: v0.40.0
   hooks:
   - id: yapf
     args: [-i]
     additional_dependencies: [toml]
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
+ci:
+  autoupdate_schedule: monthly
+  skip: [flake8]
```

### Comparing `shtab-1.6.3/CONTRIBUTING.md` & `shtab-1.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/LICENCE` & `shtab-1.6.4/LICENCE`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/PKG-INFO` & `shtab-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shtab
-Version: 1.6.3
+Version: 1.6.4
 Summary: Automagic shell tab completion for Python CLI applications
 Author-email: Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: Iterative <support@iterative.ai>
 License: Apache-2.0
 Project-URL: documentation, https://docs.iterative.ai/shtab
 Project-URL: repository, https://github.com/iterative/shtab
 Project-URL: changelog, https://github.com/iterative/shtab/releases
```

### Comparing `shtab-1.6.3/README.rst` & `shtab-1.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/docs/index.md` & `shtab-1.6.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/docs/pydoc-markdown.yml` & `shtab-1.6.4/docs/pydoc-markdown.yml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/docs/pydoc_markdown_shtab.py` & `shtab-1.6.4/docs/pydoc_markdown_shtab.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/docs/use.md` & `shtab-1.6.4/docs/use.md`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/examples/customcomplete.py` & `shtab-1.6.4/examples/customcomplete.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/examples/docopt-greeter.py` & `shtab-1.6.4/examples/docopt-greeter.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/examples/pathcomplete.py` & `shtab-1.6.4/examples/pathcomplete.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/meta/logo.png` & `shtab-1.6.4/meta/logo.png`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/pyproject.toml` & `shtab-1.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/shtab/__init__.py` & `shtab-1.6.4/shtab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 _shtab_replace_nonword() {
   echo "${1//[^[:word:]]/_}"
 }
 
 # set default values (called for the initial parser & any subparsers)
 _set_parser_defaults() {
   local subparsers_var="${prefix}_subparsers[@]"
-  sub_parsers=${!subparsers_var}
+  sub_parsers=${!subparsers_var-}
 
   local current_option_strings_var="${prefix}_option_strings[@]"
   current_option_strings=${!current_option_strings_var}
 
   completed_positional_actions=0
 
   _set_new_action "pos_${completed_positional_actions}" true
@@ -352,21 +352,21 @@
 # $1=action identifier
 # $2=positional action (bool)
 # set all identifiers for an action's parameters
 _set_new_action() {
   current_action="${prefix}_$(_shtab_replace_nonword $1)"
 
   local current_action_compgen_var=${current_action}_COMPGEN
-  current_action_compgen="${!current_action_compgen_var}"
+  current_action_compgen="${!current_action_compgen_var-}"
 
   local current_action_choices_var="${current_action}_choices[@]"
-  current_action_choices="${!current_action_choices_var}"
+  current_action_choices="${!current_action_choices_var-}"
 
   local current_action_nargs_var="${current_action}_nargs"
-  if [ -n "${!current_action_nargs_var}" ]; then
+  if [ -n "${!current_action_nargs_var-}" ]; then
     current_action_nargs="${!current_action_nargs_var}"
   else
     current_action_nargs=1
   fi
 
   current_action_args_start_index=$(( $word_index + 1 ))
 
@@ -380,31 +380,31 @@
 #     hello="world"
 #     x="hello"
 #     ${!x} -> ${hello} -> "world"
 ${root_prefix}() {
   local completing_word="${COMP_WORDS[COMP_CWORD]}"
   COMPREPLY=()
 
-  prefix=${root_prefix}
-  word_index=0
+  local prefix=${root_prefix}
+  local word_index=0
   _set_parser_defaults
   word_index=1
 
   # determine what arguments are appropriate for the current state
   # of the arg parser
   while [ $word_index -ne $COMP_CWORD ]; do
     local this_word="${COMP_WORDS[$word_index]}"
 
-    if [[ -n $sub_parsers && " ${sub_parsers[@]} " =~ " ${this_word} " ]]; then
+    if [[ -n $sub_parsers && " ${sub_parsers[@]} " == *" ${this_word} "* ]]; then
       # valid subcommand: add it to the prefix & reset the current action
       prefix="${prefix}_$(_shtab_replace_nonword $this_word)"
       _set_parser_defaults
     fi
 
-    if [[ " ${current_option_strings[@]} " =~ " ${this_word} " ]]; then
+    if [[ " ${current_option_strings[@]} " == *" ${this_word} "* ]]; then
       # a new action should be acquired (due to recognised option string or
       # no more input expected from current action);
       # the next positional action can fill in here
       _set_new_action $this_word false
     fi
 
     if [[ "$current_action_nargs" != "*" ]] && \\
```

### Comparing `shtab-1.6.3/shtab/main.py` & `shtab-1.6.4/shtab/main.py`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/shtab.egg-info/PKG-INFO` & `shtab-1.6.4/shtab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shtab
-Version: 1.6.3
+Version: 1.6.4
 Summary: Automagic shell tab completion for Python CLI applications
 Author-email: Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: Iterative <support@iterative.ai>
 License: Apache-2.0
 Project-URL: documentation, https://docs.iterative.ai/shtab
 Project-URL: repository, https://github.com/iterative/shtab
 Project-URL: changelog, https://github.com/iterative/shtab/releases
```

### Comparing `shtab-1.6.3/shtab.egg-info/SOURCES.txt` & `shtab-1.6.4/shtab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shtab-1.6.3/tests/test_shtab.py` & `shtab-1.6.4/tests/test_shtab.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class Bash:
     def __init__(self, init_script=""):
         self.init = init_script
 
     def test(self, cmd="1", failure_message=""):
         """Equivalent to `bash -c '{init}; [[ {cmd} ]]'`."""
         init = self.init + "\n" if self.init else ""
-        proc = subprocess.Popen(["bash", "-o", "pipefail", "-ec", f"{init}[[ {cmd} ]]"])
+        proc = subprocess.Popen(["bash", "-o", "pipefail", "-euc", f"{init}[[ {cmd} ]]"])
         stdout, stderr = proc.communicate()
         assert (0 == proc.wait() and not stdout and not stderr), f"""\
 {failure_message}
 {cmd}
 === stdout ===
 {stdout or ""}=== stderr ===
 {stderr or ""}"""
@@ -32,15 +32,15 @@
     def compgen(self, compgen_cmd, word, expected_completions, failure_message=""):
         self.test(
             f'"$(echo $(compgen {compgen_cmd} -- "{word}"))" = "{expected_completions}"',
             failure_message,
         )
 
 
-@pytest.mark.parametrize("init,test", [("export FOO=1", '"$FOO" -eq 1'), ("", '-z "$FOO"')])
+@pytest.mark.parametrize("init,test", [("export FOO=1", '"$FOO" -eq 1'), ("", '-z "${FOO-}"')])
 def test_bash(init, test):
     shell = Bash(init)
     shell.test(test)
 
 
 def test_bash_compgen():
     shell = Bash()
@@ -188,15 +188,15 @@
     print(completion)
 
     if shell == "bash":
         shell = Bash(completion)
         shell.compgen('-W "${_shtab_test_subparsers[*]}"', "s", "sub")
         shell.compgen('-W "$_shtab_test_pos_0_choices"', "s", "sub")
         shell.test('"$($_shtab_test_sub_pos_0_COMPGEN o)" = "one"')
-        shell.test('-z "$_shtab_test_COMPGEN"')
+        shell.test('-z "${_shtab_test_COMPGEN-}"')
 
     assert not caplog.record_tuples
 
 
 @fix_shell
 def test_subparser_aliases(shell, caplog):
     parser = ArgumentParser(prog="test")
@@ -213,15 +213,15 @@
         shell.compgen('-W "${_shtab_test_subparsers[*]}"', "s", "sub")
         shell.compgen('-W "${_shtab_test_pos_0_choices[*]}"', "s", "sub")
         shell.compgen('-W "${_shtab_test_subparsers[*]}"', "x", "xsub")
         shell.compgen('-W "${_shtab_test_pos_0_choices[*]}"', "x", "xsub")
         shell.compgen('-W "${_shtab_test_subparsers[*]}"', "y", "ysub")
         shell.compgen('-W "${_shtab_test_pos_0_choices[*]}"', "y", "ysub")
         shell.test('"$($_shtab_test_sub_pos_0_COMPGEN o)" = "one"')
-        shell.test('-z "$_shtab_test_COMPGEN"')
+        shell.test('-z "${_shtab_test_COMPGEN-}"')
 
     assert not caplog.record_tuples
 
 
 @fix_shell
 def test_subparser_colons(shell, caplog):
     parser = ArgumentParser(prog="test")
@@ -231,15 +231,15 @@
         completion = shtab.complete(parser, shell=shell)
     print(completion)
 
     if shell == "bash":
         shell = Bash(completion)
         shell.compgen('-W "${_shtab_test_subparsers[*]}"', "s", "sub:cmd")
         shell.compgen('-W "${_shtab_test_pos_0_choices[*]}"', "s", "sub:cmd")
-        shell.test('-z "$_shtab_test_COMPGEN"')
+        shell.test('-z "${_shtab_test_COMPGEN-}"')
 
     assert not caplog.record_tuples
 
 
 @fix_shell
 def test_add_argument_to_optional(shell, caplog):
     parser = ArgumentParser(prog="test")
```

