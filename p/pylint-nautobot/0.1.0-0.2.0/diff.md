# Comparing `tmp/pylint_nautobot-0.1.0.tar.gz` & `tmp/pylint_nautobot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_nautobot-0.1.0.tar", max compression
+gzip compressed data, was "pylint_nautobot-0.2.0.tar", max compression
```

## Comparing `pylint_nautobot-0.1.0.tar` & `pylint_nautobot-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0      585 2023-06-05 13:05:40.679256 pylint_nautobot-0.1.0/LICENSE
--rw-r--r--   0        0        0     2575 2023-06-05 13:05:40.679256 pylint_nautobot-0.1.0/README.md
--rw-r--r--   0        0        0     1920 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/__init__.py
--rw-r--r--   0        0        0     2022 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/code_location_changes.py
--rw-r--r--   0        0        0     2140 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-api-behavior-changes.yaml
--rw-r--r--   0        0        0     2994 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-api-removed-fields.yaml
--rw-r--r--   0        0        0     2889 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-api-renamed-fields.yaml
--rw-r--r--   0        0        0     9157 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-code-location-changes.yaml
--rw-r--r--   0        0        0     1286 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-database-behavior-changes.yaml
--rw-r--r--   0        0        0     3587 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-database-removed-fields.yaml
--rw-r--r--   0        0        0     9500 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-database-renamed-fields.yaml
--rw-r--r--   0        0        0     1033 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-corrected-fields.yaml
--rw-r--r--   0        0        0     7062 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-enhanced-fields.yaml
--rw-r--r--   0        0        0    11790 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-removed-fields.yaml
--rw-r--r--   0        0        0     5058 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-renamed-fields.yaml
--rw-r--r--   0        0        0      918 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-logging-renamed-loggers.yaml
--rw-r--r--   0        0        0     2981 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/replaced_models.py
--rw-r--r--   0        0        0      680 2023-06-05 13:05:40.683256 pylint_nautobot-0.1.0/pylint_nautobot/utils.py
--rw-r--r--   0        0        0     3041 2023-06-05 13:05:52.083478 pylint_nautobot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 pylint_nautobot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-07-28 14:23:55.729374 pylint_nautobot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2575 2023-07-28 14:23:55.729374 pylint_nautobot-0.2.0/README.md
+-rw-r--r--   0        0        0     2497 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/__init__.py
+-rw-r--r--   0        0        0     2683 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/code_location_changes.py
+-rw-r--r--   0        0        0     2140 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-api-behavior-changes.yaml
+-rw-r--r--   0        0        0     2994 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-api-removed-fields.yaml
+-rw-r--r--   0        0        0     2889 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-api-renamed-fields.yaml
+-rw-r--r--   0        0        0     9157 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-code-location-changes.yaml
+-rw-r--r--   0        0        0     1286 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-database-behavior-changes.yaml
+-rw-r--r--   0        0        0     3587 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-database-removed-fields.yaml
+-rw-r--r--   0        0        0     9500 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-database-renamed-fields.yaml
+-rw-r--r--   0        0        0     1033 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-corrected-fields.yaml
+-rw-r--r--   0        0        0     7062 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-enhanced-fields.yaml
+-rw-r--r--   0        0        0    11790 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-removed-fields.yaml
+-rw-r--r--   0        0        0     5058 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-renamed-fields.yaml
+-rw-r--r--   0        0        0      918 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-logging-renamed-loggers.yaml
+-rw-r--r--   0        0        0     1112 2023-07-28 14:23:55.733374 pylint_nautobot-0.2.0/pylint_nautobot/deprecated_status_model.py
+-rw-r--r--   0        0        0     2741 2023-07-28 14:23:55.737374 pylint_nautobot-0.2.0/pylint_nautobot/incorrect_base_class.py
+-rw-r--r--   0        0        0     3107 2023-07-28 14:23:55.737374 pylint_nautobot-0.2.0/pylint_nautobot/model_label.py
+-rw-r--r--   0        0        0     2981 2023-07-28 14:23:55.737374 pylint_nautobot-0.2.0/pylint_nautobot/replaced_models.py
+-rw-r--r--   0        0        0     1739 2023-07-28 14:23:55.737374 pylint_nautobot-0.2.0/pylint_nautobot/string_field_blank_null.py
+-rw-r--r--   0        0        0      680 2023-07-28 14:23:55.737374 pylint_nautobot-0.2.0/pylint_nautobot/utils.py
+-rw-r--r--   0        0        0     3239 2023-07-28 14:24:07.505386 pylint_nautobot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 pylint_nautobot-0.2.0/PKG-INFO
```

### Comparing `pylint_nautobot-0.1.0/LICENSE` & `pylint_nautobot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/README.md` & `pylint_nautobot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/__init__.py` & `pylint_nautobot-0.2.0/pylint_nautobot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 """Initialization file for library."""
 from pathlib import Path
 
+import tomli
 from packaging.specifiers import SpecifierSet
 from packaging.version import Version
 from pylint.lint import PyLinter
-import tomli
+
+from pylint_nautobot.code_location_changes import NautobotCodeLocationChangesChecker
+from pylint_nautobot.deprecated_status_model import NautobotDeprecatedStatusModelChecker
+from pylint_nautobot.incorrect_base_class import NautobotIncorrectBaseClassChecker
+from pylint_nautobot.model_label import NautobotModelLabelChecker
+from pylint_nautobot.replaced_models import NautobotReplacedModelsImportChecker
+from pylint_nautobot.string_field_blank_null import NautobotStringFieldBlankNull
 
 try:
     from importlib import metadata
 except ImportError:
     # Python version < 3.8
     import importlib_metadata as metadata
 
 __version__ = metadata.version(__name__)
 
-from pylint_nautobot.replaced_models import NautobotReplacedModelsImportChecker
-from pylint_nautobot.code_location_changes import NautobotCodeLocationChangesChecker
-
 CHECKERS = [
     NautobotCodeLocationChangesChecker,
+    NautobotDeprecatedStatusModelChecker,
+    NautobotIncorrectBaseClassChecker,
+    NautobotModelLabelChecker,
     NautobotReplacedModelsImportChecker,
+    NautobotStringFieldBlankNull,
 ]
 
 
-def register(linter: PyLinter):
-    """Pylint plugin entrypoint - register all the checks to the linter."""
-    # Try to discover the target projects 'pyproject.toml' to access its pylint-nautobot configuration.
+def _read_target_pyproject_toml() -> dict:
+    """Try to discover the target projects 'pyproject.toml' to access its pylint-nautobot configuration."""
     # TODO: It would be great if we could infer this from the Nautobot dependency constraint for the target project.
-    pyproject_toml_content = None
     for directory in [*Path.cwd().parents, Path.cwd()]:
         pyproject_toml_path = directory / "pyproject.toml"
         if pyproject_toml_path.exists():
             with open(pyproject_toml_path, "rb") as file:
-                pyproject_toml_content = tomli.load(file)
-                break
+                return tomli.load(file)
+
+    raise RuntimeError("Unable to find pyproject.toml for target project.")
+
+
+def register(linter: PyLinter):
+    """Pylint plugin entrypoint - register all the checks to the linter."""
+    pyproject_toml_content = _read_target_pyproject_toml()
+
     try:
         supported_nautobot_versions = [
             Version(version)
             for version in pyproject_toml_content["tool"]["pylint-nautobot"]["supported_nautobot_versions"]
         ]
     except KeyError as error:
         raise Exception("[tool.pylint-nautobot] configuration missing from pyproject.toml.") from error
```

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/code_location_changes.py` & `pylint_nautobot-0.2.0/pylint_nautobot/code_location_changes.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,34 @@
         "E4252": (
             "Import location has changed for %s (%s -> %s).",
             "nb-code-location-changed-object",
             "https://docs.nautobot.com/projects/core/en/next/installation/upgrading-from-nautobot-v1/#python-code-location-changes",
         ),
     }
 
+    def visit_import(self, node):
+        """Verifies whether entire module imports have moved.
+
+        e.g.: `import nautobot.core.fields` is invalid.
+        """
+        for name, _ in node.names:
+            if name in MAP_CODE_LOCATION_CHANGES:
+                import_changed_to = MAP_CODE_LOCATION_CHANGES[name]
+                if "(all)" in import_changed_to:
+                    self.add_message(
+                        "nb-code-location-changed",
+                        node=node,
+                        args=(name, import_changed_to["(all)"]),
+                    )
+
     def visit_importfrom(self, node):
-        """Verifies whether entire module imports or individual objects have moved."""
+        """Verifies whether entire module imports or individual objects have moved.
+
+        e.g. `from nautobot.utilities import templatetags` is invalid.
+        """
         if node.modname in MAP_CODE_LOCATION_CHANGES:
             import_changed_to = MAP_CODE_LOCATION_CHANGES[node.modname]
             if "(all)" in import_changed_to:
                 # from nautobot.utilities.templatetags import ...
                 self.add_message(
                     "nb-code-location-changed",
                     node=node,
```

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-api-behavior-changes.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-api-behavior-changes.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-api-removed-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-api-removed-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-api-renamed-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-api-renamed-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-code-location-changes.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-code-location-changes.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-database-behavior-changes.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-database-behavior-changes.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-database-removed-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-database-removed-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-database-renamed-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-database-renamed-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-corrected-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-corrected-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-enhanced-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-enhanced-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-removed-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-removed-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-filters-renamed-fields.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-filters-renamed-fields.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/data/v2/v2-logging-renamed-loggers.yaml` & `pylint_nautobot-0.2.0/pylint_nautobot/data/v2/v2-logging-renamed-loggers.yaml`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/replaced_models.py` & `pylint_nautobot-0.2.0/pylint_nautobot/replaced_models.py`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pylint_nautobot/utils.py` & `pylint_nautobot-0.2.0/pylint_nautobot/utils.py`

 * *Files identical despite different names*

### Comparing `pylint_nautobot-0.1.0/pyproject.toml` & `pylint_nautobot-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-nautobot"
-version = "v0.1.0"
+version = "v0.2.0"
 description = "Custom Pylint Rules for Nautobot"
 authors = ["Cristian Sirbu <cristian.sirbu@networktocode.com>", "Leo Kirchner <leo.kirchner@networktocode.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pylint = "^2.13"
@@ -26,14 +26,17 @@
 # Material for MkDocs theme
 mkdocs-material = "9.1.14"
 # Render custom markdown for version added/changed/remove notes
 mkdocs-version-annotations = "1.0.0"
 # Automatic documentation from sources, for MkDocs
 mkdocstrings = "0.21.2"
 mkdocstrings-python = "0.10.1"
+# Django and nautobot have to be installed for the inference in the tests of the class hierarchy to work correctly
+django = "3.2.19"
+nautobot = "^1.5.19"
 
 [tool.pylint-nautobot]
 # Normally this configuration goes into the apps that should be linted, but this is required so that the checkers
 # activate correctly during unit testing.
 supported_nautobot_versions = [
     "1",
     "2"
@@ -59,15 +62,18 @@
   )/
   | settings.py     # This is where you define files that should not be stylized by black
                      # the root of the project
 )
 '''
 
 [tool.pylint.master]
-ignore=".venv"
+ignore=[
+    ".venv",
+    "tests/inputs/",
+]
 
 [tool.pylint.basic]
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$|visit_)"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
@@ -98,18 +104,21 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = [
-    "tests"
+    "tests",
 ]
 norecursedirs = [
-    "tests/input"
+    "tests/inputs",
 ]
 addopts = "-vv --doctest-modules"
 
 [tool.bandit]
 skips = []
 # No need to check for security issues in the test scripts!
-exclude_dirs = ["./tests/", "./.venv/"]
+exclude_dirs = [
+    "./tests/",
+    "./.venv/",
+]
```

### Comparing `pylint_nautobot-0.1.0/PKG-INFO` & `pylint_nautobot-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-nautobot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Custom Pylint Rules for Nautobot
 Author: Cristian Sirbu
 Author-email: cristian.sirbu@networktocode.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylint-nautobot Version: 0.1.0 Summary: Custom
+Metadata-Version: 2.1 Name: pylint-nautobot Version: 0.2.0 Summary: Custom
 Pylint Rules for Nautobot Author: Cristian Sirbu Author-email:
 cristian.sirbu@networktocode.com Requires-Python: >=3.7,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: importlib-resources (>=5.12.0,<6.0.0) Requires-Dist: pylint (>=2.13,<3.0)
```

