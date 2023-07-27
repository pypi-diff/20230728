# Comparing `tmp/py_build_cmake-0.1.9a2.tar.gz` & `tmp/py_build_cmake-0.1.9a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_build_cmake-0.1.9a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_build_cmake-0.1.9a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_build_cmake-0.1.9a2.tar` & `py_build_cmake-0.1.9a3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1086 2023-07-26 14:01:41.811766 py_build_cmake-0.1.9a2/LICENSE
--rw-r--r--   0        0        0     5273 2023-07-26 14:01:41.811766 py_build_cmake-0.1.9a2/README.md
--rw-r--r--   0        0        0     1446 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/pyproject.toml
--rw-r--r--   0        0        0      139 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/__init__.py
--rw-r--r--   0        0        0    31524 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/build.py
--rw-r--r--   0        0        0     9433 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/build_component.py
--rw-r--r--   0        0        0    10695 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/cli.py
--rw-r--r--   0        0        0     9339 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/cmake.py
--rw-r--r--   0        0        0     2490 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/cmd_runner.py
--rw-r--r--   0        0        0    10414 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/config.py
--rw-r--r--   0        0        0    33227 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/config_options.py
--rw-r--r--   0        0        0      306 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/datastructures.py
--rw-r--r--   0        0        0     4217 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/help/__init__.py
--rw-r--r--   0        0        0      180 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/help/__main__.py
--rw-r--r--   0        0        0        0 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/py.typed
--rw-r--r--   0        0        0    22009 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/pyproject_options.py
--rw-r--r--   0        0        0       89 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/quirks/__init__.py
--rw-r--r--   0        0        0     6530 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/quirks/config.py
--rw-r--r--   0        0        0     2612 2023-07-26 14:01:41.843027 py_build_cmake-0.1.9a2/src/py_build_cmake/tags.py
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 py_build_cmake-0.1.9a2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-27 22:52:56.298855 py_build_cmake-0.1.9a3/LICENSE
+-rw-r--r--   0        0        0     5273 2023-07-27 22:52:56.298855 py_build_cmake-0.1.9a3/README.md
+-rw-r--r--   0        0        0     1446 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/__init__.py
+-rw-r--r--   0        0        0    33198 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/build.py
+-rw-r--r--   0        0        0     9433 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/build_component.py
+-rw-r--r--   0        0        0    10695 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/cli.py
+-rw-r--r--   0        0        0     9339 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/cmake.py
+-rw-r--r--   0        0        0     2490 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/cmd_runner.py
+-rw-r--r--   0        0        0    10414 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/config.py
+-rw-r--r--   0        0        0    34154 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/config_options.py
+-rw-r--r--   0        0        0      306 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/datastructures.py
+-rw-r--r--   0        0        0     4217 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/help/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/help/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/py.typed
+-rw-r--r--   0        0        0    23844 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/pyproject_options.py
+-rw-r--r--   0        0        0       89 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/quirks/__init__.py
+-rw-r--r--   0        0        0     6530 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/quirks/config.py
+-rw-r--r--   0        0        0     2612 2023-07-27 22:52:56.330058 py_build_cmake-0.1.9a3/src/py_build_cmake/tags.py
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 py_build_cmake-0.1.9a3/PKG-INFO
```

### Comparing `py_build_cmake-0.1.9a2/LICENSE` & `py_build_cmake-0.1.9a3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/README.md` & `py_build_cmake-0.1.9a3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.9a2"]
+requires = ["py-build-cmake~=0.1.9a3"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

### Comparing `py_build_cmake-0.1.9a2/pyproject.toml` & `py_build_cmake-0.1.9a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/build.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from copy import copy
 import shutil
 import textwrap
 from typing import Any, Dict, List, Optional
 import tempfile
 from glob import glob
+import re
 
 from . import config
 from . import cmake
 from .datastructures import BuildPaths, PackageInfo
 from .cmd_runner import CommandRunner
 
 from flit_core.common import Module as flit_Module  # type: ignore
@@ -285,25 +286,27 @@
     @staticmethod
     def create_wheel(paths, cfg, package_info):
         """Create a wheel package from the build directory."""
         from distlib.wheel import Wheel  # type: ignore
         whl = Wheel()
         whl.name = package_info.package_name
         whl.version = package_info.version
-        pure = not cfg.cmake
+        pure = _BuildBackend.is_pure(cfg)
         libdir = 'purelib' if pure else 'platlib'
         staging_dir = paths.pkg_staging_dir
         whl_paths = {'prefix': str(staging_dir), libdir: str(staging_dir)}
         whl.dirname = paths.wheel_dir
         if pure:
             tags = {'pyver': ['py3']}
         elif cfg.cross:
             tags = _BuildBackend.get_cross_tags(cfg.cross)
+            tags = _BuildBackend.convert_wheel_tags(tags, cfg)
         else:
             tags = _BuildBackend.get_native_tags()
+            tags = _BuildBackend.convert_wheel_tags(tags, cfg)
         wheel_path = whl.build(whl_paths, tags=tags, wheel_version=(1, 0))
         whl_name = os.path.relpath(wheel_path, paths.wheel_dir)
         return whl_name
 
     @staticmethod
     def get_cmake_configs(cfg):
         native_cmake_cfg = cfg.cmake[_BuildBackend.get_os_name()]
@@ -628,14 +631,54 @@
     @staticmethod
     def normalize_version(version):
         from distlib.version import NormalizedVersion
         norm_version = str(NormalizedVersion(version))
         return norm_version
 
     @staticmethod
+    def convert_abi_tag(abi_tag: str, cmake_cfg: Optional[dict]):
+        """Set the ABI tag to 'none' or 'abi3', depending on the config options
+        specified by the user."""
+        if not cmake_cfg:
+            return 'none'
+        elif cmake_cfg['abi'] == 'auto':
+            return abi_tag
+        elif cmake_cfg['abi'] == 'none':
+            return 'none'
+        elif cmake_cfg['abi'] == 'abi3':
+            # Only use abi3 if we're actually building for CPython
+            m = re.match(r"^cp(\d+).*$", abi_tag)
+            if m and int(m[1]) >= cmake_cfg['abi3_minimum_cpython_version']:
+                return 'abi3'
+            return abi_tag
+        else:
+            assert False, "Unsupported abi"
+
+    @staticmethod
+    def convert_wheel_tags(tags, cfg):
+        """Apply convert_abi_tag to each of the abi tags."""
+        assert cfg.cmake
+        tags = copy(tags)
+        cmake_cfg, _ = _BuildBackend.get_cmake_configs(cfg)
+        cvt_abi = lambda tag: _BuildBackend.convert_abi_tag(tag, cmake_cfg)
+        tags['abi'] = list(map(cvt_abi, tags['abi']))
+        if 'none' in tags['abi']:
+            tags['pyver'] = ['py3']
+        return tags
+
+    @staticmethod
+    def is_pure(cfg):
+        """Check if the package is a pure-Python package without platform-
+        specific binaries."""
+        if not cfg.cmake:
+            return True
+        cmake_cfg, _ = _BuildBackend.get_cmake_configs(cfg)
+        return cmake_cfg['pure_python']
+
+    @staticmethod
     def get_native_tags():
         """Get the PEP 425 tags for the current platform."""
         from .tags import get_python_tag, get_abi_tag, get_platform_tag
         return {
             'pyver': [get_python_tag()],
             'abi': [get_abi_tag()],
             'arch': [get_platform_tag()],
```

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/build_component.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/build_component.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/cli.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/cli.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/cmake.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/cmd_runner.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/cmd_runner.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/config.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/config.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/config_options.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/config_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import os.path as osp
 from pathlib import Path
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 
 from flit_core.config import ConfigError  # type: ignore
 
 ConfPath = Tuple[str, ...]
-ConfValue = Optional[Union[bool, str, List[str], Dict[str, Any]]]
+ConfValue = Optional[Union[bool, int, str, List[str], Dict[str, Any]]]
 Conf = Dict[str, Any]
 
 
 def pth(s: str) -> ConfPath:
     if not s:
         return ()
     return tuple(s.split('/'))
@@ -528,14 +528,37 @@
             raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
                               f'{str}, not {dict}')
         elif not isinstance(cfg[cfgpath].value, str):
             raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
                               f'{str}, not {type(cfg[cfgpath].value)}')
 
 
+class IntConfigOption(ConfigOption):
+
+    def get_typename(self, md: bool = False):
+        return 'int'
+
+    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        assert not self.sub
+        assert not selfcfg.sub
+        assert not overridecfg.sub
+        selfcfg.value = deepcopy(overridecfg.value)
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if cfg[cfgpath].sub:
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{int}, not {dict}')
+        elif not isinstance(cfg[cfgpath].value, int):
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{int}, not {type(cfg[cfgpath].value)}')
+
+
 class EnumConfigOption(ConfigOption):
 
     def __init__(self,
                  name: str,
                  description: str = '',
                  example: str = '',
                  default: DefaultValue = NoDefaultValue(),
```

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/help/__init__.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/help/__init__.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/pyproject_options.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/pyproject_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -197,14 +197,42 @@
         DictOfStrConfigOption("env",
                               "Environment variables to set when running "
                               "CMake. Supports variable expansion using "
                               "`${VAR}` (but not `$VAR`).",
                               "env = { \"CMAKE_PREFIX_PATH\" "
                               "= \"${HOME}/.local\" }",
                               default=DefaultValueValue({})),
+        BoolConfigOption("pure_python",
+                         "Indicate that this package contains no platform-"
+                         "specific binaries, only Python scripts and other "
+                         "platform-agnostic files. It causes the Wheel tags "
+                         "to be set to `py3-none-any`.",
+                         "pure_python = true",
+                         default=DefaultValueValue(False)),
+        EnumConfigOption("abi",
+                         "Override the default ABI tag for the Wheel package.\n"
+                         "If your package does not contain Python extension "
+                         "modules (e.g. because it only includes executables "
+                         "to run as a subprocess, or only shared library files "
+                         "to be loaded using ctypes), you can set this to "
+                         "'none'.\n"
+                         "If your package only includes Python extension "
+                         "modules that use the CPython stable ABI, set this "
+                         "'abi3' (see also 'abi3_minimum_cpython_version' "
+                         "below).",
+                         "abi = 'none'",
+                         default=DefaultValueValue("auto"),
+                         options=["auto", "none", "abi3"]),
+        IntConfigOption("abi3_minimum_cpython_version",
+                        "If 'abi' is set to 'abi3', only use the stable "
+                        "CPython API for CPython version that are newer than "
+                        "'abi3_minimum_version'. Useful for nanobind, which "
+                        "supports the stable ABI for CPython 12 and later.",
+                        "abi3_minimum_cpython_version = 312",
+                        default=DefaultValueValue(32)),
     ])# yapf: disable
 
     # [tool.py-build-cmake.stubgen]
     stubgen = pbc.insert(
         ConfigOption(
             "stubgen",
             "If specified, mypy's stubgen utility will be used to generate "
```

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/quirks/config.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/quirks/config.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/src/py_build_cmake/tags.py` & `py_build_cmake-0.1.9a3/src/py_build_cmake/tags.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.1.9a2/PKG-INFO` & `py_build_cmake-0.1.9a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-build-cmake
-Version: 0.1.9a2
+Version: 0.1.9a3
 Summary: Modern, PEP 517 compliant build backend for creating Python packages with
 Keywords: pep517,cmake
 Author-email: Pieter P <pieter.p.dev@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -86,15 +86,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.9a2"]
+requires = ["py-build-cmake~=0.1.9a3"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

