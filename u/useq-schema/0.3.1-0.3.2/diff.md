# Comparing `tmp/useq_schema-0.3.1.tar.gz` & `tmp/useq_schema-0.3.2.tar.gz`

## Comparing `useq_schema-0.3.1.tar` & `useq_schema-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 useq_schema-0.3.1/mkdocs.yml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.1/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/images/favicon.ico
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/axes.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/event.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/hardware_autofocus.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_actions.py
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_base_model.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_channel.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_grid.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_hardware_autofocus.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_mda_event.py
--rw-r--r--   0        0        0    21704 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_position.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_time.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_utils.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/py.typed
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_autofocus.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_grid.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_misc.py
--rw-r--r--   0        0        0    18536 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_position_sequence.py
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_sequence.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_serialization.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/fixtures/mda.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.3.1/LICENSE
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 useq_schema-0.3.1/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 useq_schema-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 useq_schema-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 useq_schema-0.3.2/mkdocs.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.2/setup.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/axes.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/event.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/hardware_autofocus.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_actions.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_base_model.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_channel.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_grid.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_hardware_autofocus.py
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    21704 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_position.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_time.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_utils.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/py.typed
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_autofocus.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_grid.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_misc.py
+-rw-r--r--   0        0        0    18536 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_position_sequence.py
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_sequence.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_serialization.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7977 2020-02-02 00:00:00.000000 useq_schema-0.3.2/README.md
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 useq_schema-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 useq_schema-0.3.2/PKG-INFO
```

### Comparing `useq_schema-0.3.1/.pre-commit-config.yaml` & `useq_schema-0.3.2/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,29 @@
   autoupdate_schedule: monthly
   autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
   autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
-  - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v2.3.0
-    hooks:
-      - id: conventional-pre-commit
-        stages: [commit-msg]
-
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-docstring-first
-      - id: end-of-file-fixer
-      - id: trailing-whitespace
       - id: pretty-format-json
         args: ["--autofix"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.275
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.13
     hooks:
       - id: validate-pyproject
```

### Comparing `useq_schema-0.3.1/mkdocs.yml` & `useq_schema-0.3.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/setup.py` & `useq_schema-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/.github/workflows/test_and_deploy.yml` & `useq_schema-0.3.2/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
   test:
     name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9 ,"3.10", "3.11"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
         platform: [ubuntu-latest, macos-latest, windows-latest]
     steps:
       - name: Cancel Previous Runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
 
@@ -58,15 +58,15 @@
         with:
           repository: pymmcore-plus/pymmcore-plus
           path: pymmcore-plus-from-github
 
       - name: Set up Python 3.10
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: "3.10"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e pymmcore-plus-from-github[testing]
           pip install -e .[test]
 
@@ -86,30 +86,29 @@
         with:
           repository: pymmcore-plus/pymmcore-widgets
           path: pymmcore-widgets-from-github
 
       - name: Set up Python 3.10
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: "3.10"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e pymmcore-widgets-from-github[test,image,pyqt6]
           pip install -e .[test]
 
       - name: Install Micro-Manager
         run: mmcore install
 
       - name: Test
         run: pytest -v --color=yes -W ignore
         working-directory: pymmcore-widgets-from-github
 
-
   deploy:
     needs: test
     runs-on: ubuntu-latest
     if: ${{ github.repository == 'pymmcore-plus/useq-schema' && contains(github.ref, 'tags') }}
     steps:
       - uses: actions/checkout@v3
```

### Comparing `useq_schema-0.3.1/docs/api.md` & `useq_schema-0.3.2/docs/api.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/docs/index.md` & `useq_schema-0.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/docs/images/favicon.ico` & `useq_schema-0.3.2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/docs/schema/axes.md` & `useq_schema-0.3.2/docs/schema/axes.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/docs/stylesheets/extra.css` & `useq_schema-0.3.2/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/__init__.py` & `useq_schema-0.3.2/src/useq/__init__.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_actions.py` & `useq_schema-0.3.2/src/useq/_actions.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_base_model.py` & `useq_schema-0.3.2/src/useq/_base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 
 import warnings
 from pathlib import Path
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
+    ClassVar,
     Dict,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
+import numpy as np
 from pydantic import BaseModel, root_validator
 from pydantic.error_wrappers import ErrorWrapper, ValidationError
 from pydantic.utils import ROOT_KEY
 
+from useq._utils import ReadOnlyDict
+
 if TYPE_CHECKING:
     from pydantic.types import StrBytes
 
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
 
 
 __all__ = ["UseqModel", "FrozenModel"]
@@ -32,14 +36,15 @@
 
 
 class FrozenModel(BaseModel):
     class Config:
         allow_population_by_field_name = True
         extra = "allow"
         frozen = True
+        json_encoders: ClassVar[dict] = {"ReadOnlyDict": dict}
 
     @root_validator(pre=False, skip_on_failure=True)
     def _validate_kwargs(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Validate kwargs for MDASequence."""
         extra_kwargs = set(values) - set(cls.__fields__)
         if extra_kwargs:
             name = getattr(cls, "__name__", "")
@@ -193,14 +198,20 @@
 
         yaml.SafeDumper.add_multi_representer(
             timedelta, lambda dumper, data: dumper.represent_str(str(data))
         )
         yaml.SafeDumper.add_multi_representer(
             Enum, lambda dumper, data: dumper.represent_str(str(data.value))
         )
+        yaml.SafeDumper.add_multi_representer(
+            ReadOnlyDict, lambda dumper, data: dumper.represent_dict(data)
+        )
+        yaml.SafeDumper.add_multi_representer(
+            np.floating, lambda dumper, data: dumper.represent_float(float(data))
+        )
 
         data = self.dict(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
```

### Comparing `useq_schema-0.3.1/src/useq/_channel.py` & `useq_schema-0.3.2/src/useq/_channel.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_grid.py` & `useq_schema-0.3.2/src/useq/_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_hardware_autofocus.py` & `useq_schema-0.3.2/src/useq/_hardware_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_mda_event.py` & `useq_schema-0.3.2/src/useq/_mda_event.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_mda_sequence.py` & `useq_schema-0.3.2/src/useq/_mda_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_position.py` & `useq_schema-0.3.2/src/useq/_position.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_time.py` & `useq_schema-0.3.2/src/useq/_time.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_utils.py` & `useq_schema-0.3.2/src/useq/_utils.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/src/useq/_z.py` & `useq_schema-0.3.2/src/useq/_z.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/tests/conftest.py` & `useq_schema-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/tests/test_autofocus.py` & `useq_schema-0.3.2/tests/test_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/tests/test_grid.py` & `useq_schema-0.3.2/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/tests/test_position_sequence.py` & `useq_schema-0.3.2/tests/test_position_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/tests/test_sequence.py` & `useq_schema-0.3.2/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/tests/fixtures/mda.json` & `useq_schema-0.3.2/tests/fixtures/mda.json`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/tests/fixtures/mda.yaml` & `useq_schema-0.3.2/tests/fixtures/mda.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/.gitignore` & `useq_schema-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/LICENSE` & `useq_schema-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.1/README.md` & `useq_schema-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # useq-schema
 
 [![License](https://img.shields.io/pypi/l/useq-schema.svg?color=green)](https://github.com/pymmcore-plus/useq-schema/raw/main/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/useq-schema)](https://pypi.org/project/useq-schema)
 [![PyPI](https://img.shields.io/pypi/v/useq-schema.svg?color=green)](https://pypi.org/project/useq-schema)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/useq-schema)](https://anaconda.org/conda-forge/useq-schema)
 [![tests](https://github.com/pymmcore-plus/useq-schema/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/pymmcore-plus/useq-schema/actions/workflows/test_and_deploy.yml)
 [![docs](https://github.com/pymmcore-plus/useq-schema/actions/workflows/docs.yml/badge.svg)](https://pymmcore-plus.github.io/useq-schema/)
 [![codecov](https://codecov.io/gh/pymmcore-plus/useq-schema/branch/main/graph/badge.svg)](https://codecov.io/gh/pymmcore-plus/useq-schema)
 
 *An implementation agnostic schema for describing a sequence of events during a
 multi-dimensional imaging acquisition.*
```

### Comparing `useq_schema-0.3.1/pyproject.toml` & `useq_schema-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 
 # https://peps.python.org/pep-0621/
 [project]
 name = "useq-schema"
 description = "Schema for multi-dimensional microscopy experiments"
 readme = "README.md"
 keywords = ["microscopy", "schema"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { text = "BSD 3-Clause License" }
 authors = [{ email = "talley.lambert@gmail.com", name = "Talley Lambert" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Software Development",
+    "Topic :: System :: Hardware",
+    "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = ["pydantic<2.0", "numpy"]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
@@ -58,30 +64,32 @@
 # https://hatch.pypa.io/latest/config/build/#file-selection
 [tool.hatch.build.targets.wheel]
 packages = ["src/useq"]
 
 # https://beta.ruff.rs/docs/rules/
 [tool.ruff]
 line-length = 88
-target-version = "py37"
+target-version = "py38"
 src = ["src", "tests"]
 select = [
+    "W",    # style warnings
     "E",    # style errors
     "F",    # flakes
     "D",    # pydocstyle
     "I",    # isort
     "UP",   # pyupgrade
     "S",    # bandit
     "C4",   # comprehensions
     "B",    # bugbear
     "A001", # Variable shadowing a python builtin
     "TCH",  # flake8-type-checking
     "TID",  # flake8-tidy-imports
     "RUF",  # ruff-specific rules
     "PERF", # performance
+    "SLF",  # private access
 ]
 ignore = [
     "D100",  # Missing docstring in public module
     "D104",  # Missing docstring in public package
     "D107",  # Missing docstring in __init__
     "D203",  # 1 blank line required before class docstring
     "D212",  # Multi-line docstring summary should start at the first line
```

### Comparing `useq_schema-0.3.1/PKG-INFO` & `useq_schema-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.3.1
+Version: 0.3.2
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development
-Requires-Python: >=3.7
+Classifier: Topic :: System :: Hardware
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Requires-Dist: numpy
 Requires-Dist: pydantic<2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
@@ -44,15 +50,17 @@
 Provides-Extra: yaml
 Requires-Dist: pyyaml; extra == 'yaml'
 Description-Content-Type: text/markdown
 
 # useq-schema
 
 [![License](https://img.shields.io/pypi/l/useq-schema.svg?color=green)](https://github.com/pymmcore-plus/useq-schema/raw/main/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/useq-schema)](https://pypi.org/project/useq-schema)
 [![PyPI](https://img.shields.io/pypi/v/useq-schema.svg?color=green)](https://pypi.org/project/useq-schema)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/useq-schema)](https://anaconda.org/conda-forge/useq-schema)
 [![tests](https://github.com/pymmcore-plus/useq-schema/actions/workflows/test_and_deploy.yml/badge.svg)](https://github.com/pymmcore-plus/useq-schema/actions/workflows/test_and_deploy.yml)
 [![docs](https://github.com/pymmcore-plus/useq-schema/actions/workflows/docs.yml/badge.svg)](https://pymmcore-plus.github.io/useq-schema/)
 [![codecov](https://codecov.io/gh/pymmcore-plus/useq-schema/branch/main/graph/badge.svg)](https://codecov.io/gh/pymmcore-plus/useq-schema)
 
 *An implementation agnostic schema for describing a sequence of events during a
 multi-dimensional imaging acquisition.*
```

