# Comparing `tmp/extendable_pydantic-1.0.1.tar.gz` & `tmp/extendable_pydantic-1.1.0.tar.gz`

## Comparing `extendable_pydantic-1.0.1.tar` & `extendable_pydantic-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/extendable_pydantic_patcher.pth
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/__init__.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/_patch.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/py.typed
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/src/extendable_pydantic/version.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/LICENSE
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/README.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/extendable_pydantic_patcher.pth
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/src/extendable_pydantic/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/src/extendable_pydantic/_patch.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/src/extendable_pydantic/main.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/src/extendable_pydantic/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/src/extendable_pydantic/py.typed
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/src/extendable_pydantic/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/src/extendable_pydantic/version.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 extendable_pydantic-1.1.0/PKG-INFO
```

### Comparing `extendable_pydantic-1.0.1/src/extendable_pydantic/_patch.py` & `extendable_pydantic-1.1.0/src/extendable_pydantic/_patch.py`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.1/src/extendable_pydantic/main.py` & `extendable_pydantic-1.1.0/src/extendable_pydantic/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import inspect
 import typing
 import warnings
-from typing import Any, Dict, Optional, cast, no_type_check
+from typing import Any, Dict, List, Optional, cast, no_type_check
 
 from extendable import context, main
 from extendable.main import ExtendableMeta
 from extendable.registry import ExtendableClassesRegistry, ExtendableRegistryListener
 
 try:
     from typing import _TypingBase  # type: ignore[attr-defined,unused-ignore]
@@ -108,14 +108,25 @@
 
 
 class RegistryListener(ExtendableRegistryListener):
     def on_registry_initialized(self, registry: ExtendableClassesRegistry) -> None:
         self.resolve_submodel_fields(registry)
         self.rebuild_models(registry)
 
+    def before_init_registry(
+        self,
+        registry: "ExtendableClassesRegistry",
+        module_matchings: Optional[List[str]] = None,
+    ) -> None:
+        if module_matchings is not None:
+            # ensure that the current module is loaded...
+            # prepend the current module to the module_matchings
+            if "extendable_pydantic" not in module_matchings:
+                module_matchings.insert(0, "extendable_pydantic.models")
+
     def rebuild_models(self, registry: ExtendableClassesRegistry) -> None:
         for cls in registry._extendable_classes.values():
             cast(BaseModel, cls).model_rebuild(force=True)
 
     def resolve_submodel_fields(self, registry: ExtendableClassesRegistry) -> None:
         for cls in registry._extendable_classes.values():
             if issubclass(type(cls), ExtendableModelMeta):
```

### Comparing `extendable_pydantic-1.0.1/src/extendable_pydantic/utils.py` & `extendable_pydantic-1.1.0/src/extendable_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.1/.gitignore` & `extendable_pydantic-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.1/LICENSE` & `extendable_pydantic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.1/README.md` & `extendable_pydantic-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-1.0.1/pyproject.toml` & `extendable_pydantic-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
 dynamic = ["version", "description"]
 dependencies = [
-    "extendable>=1.0.0",
+    "extendable>=1.2.0",
     "pydantic>=2.0.2",
     "wrapt",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 test = [
```

### Comparing `extendable_pydantic-1.0.1/PKG-INFO` & `extendable_pydantic-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable_pydantic
-Version: 1.0.1
+Version: 1.1.0
 Project-URL: Source, https://github.com/lmignon/extendable-pydantic
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 License: MIT License
         
         Copyright (c) 2021 Laurent Mignon (ACSONE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Requires-Dist: extendable>=1.0.0
+Requires-Dist: extendable>=1.2.0
 Requires-Dist: pydantic>=2.0.2
 Requires-Dist: wrapt
 Provides-Extra: mypy
 Requires-Dist: mypy>=1.4.1; extra == 'mypy'
 Provides-Extra: release
 Requires-Dist: bumpversion; extra == 'release'
 Requires-Dist: towncrier; extra == 'release'
```

