# Comparing `tmp/sphinx_json_schema_spec-2023.7.2.tar.gz` & `tmp/sphinx_json_schema_spec-2023.7.3.tar.gz`

## Comparing `sphinx_json_schema_spec-2023.7.2.tar` & `sphinx_json_schema_spec-2023.7.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.flake8
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.readthedocs.yml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/release.yml
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/Makefile
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/conf.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/index.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/requirements.in
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/tests/test_sphinx.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/COPYING
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/README.rst
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/pyproject.toml
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.2/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.flake8
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.readthedocs.yml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/release.yml
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/Makefile
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/conf.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/index.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/requirements.in
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/tests/test_sphinx.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/COPYING
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/README.rst
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 sphinx_json_schema_spec-2023.7.3/PKG-INFO
```

### Comparing `sphinx_json_schema_spec-2023.7.2/.pre-commit-config.yaml` & `sphinx_json_schema_spec-2023.7.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/noxfile.py` & `sphinx_json_schema_spec-2023.7.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/.github/SECURITY.md` & `sphinx_json_schema_spec-2023.7.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/.github/workflows/ci.yml` & `sphinx_json_schema_spec-2023.7.3/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

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

### Comparing `sphinx_json_schema_spec-2023.7.2/docs/Makefile` & `sphinx_json_schema_spec-2023.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/docs/conf.py` & `sphinx_json_schema_spec-2023.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/docs/index.rst` & `sphinx_json_schema_spec-2023.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/docs/requirements.txt` & `sphinx_json_schema_spec-2023.7.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/sphinx_json_schema_spec/__init__.py` & `sphinx_json_schema_spec-2023.7.3/sphinx_json_schema_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/.gitignore` & `sphinx_json_schema_spec-2023.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/COPYING` & `sphinx_json_schema_spec-2023.7.3/COPYING`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/README.rst` & `sphinx_json_schema_spec-2023.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/pyproject.toml` & `sphinx_json_schema_spec-2023.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_json_schema_spec-2023.7.2/PKG-INFO` & `sphinx_json_schema_spec-2023.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_json_schema_spec
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Sphinx support for the JSON Schema specifications
 Project-URL: Documentation, https://sphinx-json-schema-spec.readthedocs.io/
 Project-URL: Homepage, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Project-URL: Issues, https://github.com/python-jsonschema/sphinx-json-schema-spec/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/sphinx-json-schema-spec
 Author: Julian Berman
```

