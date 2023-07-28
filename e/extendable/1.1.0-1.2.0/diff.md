# Comparing `tmp/extendable-1.1.0.tar.gz` & `tmp/extendable-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extendable-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "extendable-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `extendable-1.1.0.tar` & `extendable-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1081 2023-07-15 16:23:03.710562 extendable-1.1.0/LICENSE
--rw-r--r--   0        0        0     7477 2023-07-15 16:23:03.710562 extendable-1.1.0/README.md
--rw-r--r--   0        0        0     1457 2023-07-15 16:23:03.710562 extendable-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      393 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/__init__.py
--rw-r--r--   0        0        0      332 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/context.py
--rw-r--r--   0        0        0       55 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/exceptions.py
--rw-r--r--   0        0        0    10056 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/main.py
--rw-r--r--   0        0        0        0 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/py.typed
--rw-r--r--   0        0        0     8212 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/registry.py
--rw-r--r--   0        0        0     1059 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/utils.py
--rw-r--r--   0        0        0       22 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/version.py
--rw-r--r--   0        0        0     8480 1970-01-01 00:00:00.000000 extendable-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-28 09:57:09.886874 extendable-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7477 2023-07-28 09:57:09.886874 extendable-1.2.0/README.md
+-rw-r--r--   0        0        0     1457 2023-07-28 09:57:09.886874 extendable-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      393 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/__init__.py
+-rw-r--r--   0        0        0      332 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/context.py
+-rw-r--r--   0        0        0       55 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/exceptions.py
+-rw-r--r--   0        0        0    10056 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/main.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/py.typed
+-rw-r--r--   0        0        0     8875 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/registry.py
+-rw-r--r--   0        0        0     1059 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/utils.py
+-rw-r--r--   0        0        0       22 2023-07-28 09:57:09.890874 extendable-1.2.0/src/extendable/version.py
+-rw-r--r--   0        0        0     8480 1970-01-01 00:00:00.000000 extendable-1.2.0/PKG-INFO
```

### Comparing `extendable-1.1.0/LICENSE` & `extendable-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable-1.1.0/README.md` & `extendable-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `extendable-1.1.0/pyproject.toml` & `extendable-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extendable-1.1.0/src/extendable/main.py` & `extendable-1.2.0/src/extendable/main.py`

 * *Files identical despite different names*

### Comparing `extendable-1.1.0/src/extendable/registry.py` & `extendable-1.2.0/src/extendable/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,29 @@
 from .utils import LastOrderedSet
 
 
 class ExtendableRegistryListener:
     def on_registry_initialized(self, registry: "ExtendableClassesRegistry") -> None:
         ...
 
+    def before_init_registry(
+        self,
+        registry: "ExtendableClassesRegistry",
+        module_matchings: Optional[List[str]] = None,
+    ) -> None:
+        """Called before the registry is initialized.
+
+        This hook allows you to add your own specific module matching
+        rules into the provided one. A common use case is when you
+        define a base Extendable class into a specific python module and
+        you want to ensure that this base class is always loaded when
+        the registry is initialized.
+        """
+        ...
+
 
 class ExtendableClassesRegistry:
     """Store all the extendableClasses and allow to retrieve them by name.
 
     The key is the ``cls.__module__ + "." + cls.__qualname__`` of the
     extendable classes.
 
@@ -154,14 +169,16 @@
         aggregated classes will be the inverse one of the given module list. If no
         module list given, build the aggregated classes for all the modules loaded by
         the metaclass in the same order as the loading process.
 
         The module list accept wildcard expression as last character
         """
         module_matchings = module_matchings if module_matchings else ["*"]
+        for listener in self.listeners:
+            listener.before_init_registry(self, module_matchings)
         with self.build_mode(), ModuleIndex() as idx:
             for match in module_matchings:
                 for module in idx.get_modules(match):
                     self.load_extendable_classes(module)
             self.build_extendable_classes()
             for listener in self.listeners:
                 listener.on_registry_initialized(self)
```

### Comparing `extendable-1.1.0/src/extendable/utils.py` & `extendable-1.2.0/src/extendable/utils.py`

 * *Files identical despite different names*

### Comparing `extendable-1.1.0/PKG-INFO` & `extendable-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable
-Version: 1.1.0
+Version: 1.2.0
 Summary: A lib to define class extendable at runtime.
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

