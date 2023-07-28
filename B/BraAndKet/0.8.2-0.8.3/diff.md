# Comparing `tmp/BraAndKet-0.8.2.tar.gz` & `tmp/BraAndKet-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BraAndKet-0.8.2.tar", last modified: Wed Apr 19 10:48:23 2023, max compression
+gzip compressed data, was "BraAndKet-0.8.3.tar", last modified: Fri Jul 28 03:27:24 2023, max compression
```

## Comparing `BraAndKet-0.8.2.tar` & `BraAndKet-0.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.736989 BraAndKet-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/BraAndKet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 10:48:23.000000 BraAndKet-0.8.2/src/BraAndKet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/backend/tensorflow_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/model/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/space/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/hilbert_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/num_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/space/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/special.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/tensor/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:48:23.740989 BraAndKet-0.8.2/src/braandket/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-19 10:48:09.000000 BraAndKet-0.8.2/src/braandket/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.431944 BraAndKet-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 03:27:24.431944 BraAndKet-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.423944 BraAndKet-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/BraAndKet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/tensorflow_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/hilbert_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/num_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/utils/utils.py
```

### Comparing `BraAndKet-0.8.2/LICENSE` & `BraAndKet-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.2/PKG-INFO` & `BraAndKet-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BraAndKet
-Version: 0.8.2
+Version: 0.8.3
 Summary: BraAndKet is a library for numeral calculations of discrete quantum systems.
 Author-email: Zheng Keli <zhengkeli2009@126.com>
 Project-URL: repository, https://github.com/ZhengKeli/BraAndKet
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `BraAndKet-0.8.2/README.md` & `BraAndKet-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.2/pyproject.toml` & `BraAndKet-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "BraAndKet"
-version = "0.8.2"
+version = "0.8.3"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 description = "BraAndKet is a library for numeral calculations of discrete quantum systems."
```

### Comparing `BraAndKet-0.8.2/src/BraAndKet.egg-info/PKG-INFO` & `BraAndKet-0.8.3/src/BraAndKet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BraAndKet
-Version: 0.8.2
+Version: 0.8.3
 Summary: BraAndKet is a library for numeral calculations of discrete quantum systems.
 Author-email: Zheng Keli <zhengkeli2009@126.com>
 Project-URL: repository, https://github.com/ZhengKeli/BraAndKet
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `BraAndKet-0.8.2/src/BraAndKet.egg-info/SOURCES.txt` & `BraAndKet-0.8.3/src/BraAndKet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.2/src/braandket/backend/backend.py` & `BraAndKet-0.8.3/src/braandket/backend/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import abc
-from typing import Any, Generic, Iterable, Optional, Union
-from typing import TypeVar
+from typing import Any, Generic, Iterable, Optional, TypeVar, Union
 
 ValuesType = TypeVar('ValuesType')
 
 
 class Backend(Generic[ValuesType], abc.ABC):
 
     def __enter__(self):
@@ -123,18 +122,18 @@
 
     @abc.abstractmethod
     def diag(self, values: ValuesType, axes: tuple[Iterable[int], Iterable[int]]) -> ValuesType:
         pass
 
     @abc.abstractmethod
     def dot(self,
-            values0: ValuesType, values1: ValuesType, *,
-            ndim0: int, ndim1: int,
-            dot_axes: tuple[Iterable[int], Iterable[int]],
-            bat_axes: tuple[Iterable[int], Iterable[int]],
+        values0: ValuesType, values1: ValuesType, *,
+        ndim0: int, ndim1: int,
+        dot_axes: tuple[Iterable[int], Iterable[int]],
+        bat_axes: tuple[Iterable[int], Iterable[int]],
     ) -> tuple[ValuesType, tuple[tuple[int, ...], tuple[int, ...]]]:
         pass
 
     # special
 
     @abc.abstractmethod
     def take(self, values: Iterable[ValuesType], indices: ValuesType) -> ValuesType:
```

### Comparing `BraAndKet-0.8.2/src/braandket/backend/default.py` & `BraAndKet-0.8.3/src/braandket/backend/default.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.2/src/braandket/backend/numpy_backend.py` & `BraAndKet-0.8.3/src/braandket/backend/numpy_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,18 +113,18 @@
             values = np.diagonal(values, axis0, axis1)
             axis_pairs = axis_pairs[1:]
             axis_pairs = np.where(axis_pairs > axis0, axis_pairs - 1, axis_pairs)
             axis_pairs = np.where(axis_pairs > axis1, axis_pairs - 1, axis_pairs)
         return values
 
     def dot(self,
-            values0: np.ndarray, values1: np.ndarray, *,
-            ndim0: int, ndim1: int,
-            dot_axes: tuple[Iterable[int], Iterable[int]],
-            bat_axes: tuple[Iterable[int], Iterable[int]],
+        values0: np.ndarray, values1: np.ndarray, *,
+        ndim0: int, ndim1: int,
+        dot_axes: tuple[Iterable[int], Iterable[int]],
+        bat_axes: tuple[Iterable[int], Iterable[int]],
     ) -> tuple[np.ndarray, tuple[tuple[int, ...], tuple[int, ...]]]:
         bat_axes0, bat_axes1 = tuple(bat_axes[0]), tuple(bat_axes[1])
         if not len(bat_axes0) == len(bat_axes1):
             raise ValueError("len(bat_axes[0]) != len(bat_axes[1])")
         del bat_axes
 
         dot_axes0, dot_axes1 = tuple(dot_axes[0]), tuple(dot_axes[1])
```

### Comparing `BraAndKet-0.8.2/src/braandket/backend/tensorflow_backend.py` & `BraAndKet-0.8.3/src/braandket/backend/tensorflow_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,18 +135,18 @@
             values = tf.linalg.diag(values, axis0, axis1)
             axis_pairs = axis_pairs[1:]
             axis_pairs = tf.where(axis_pairs > axis0, axis_pairs - 1, axis_pairs)
             axis_pairs = tf.where(axis_pairs > axis1, axis_pairs - 1, axis_pairs)
         return values
 
     def dot(self,
-            values0: tf.Tensor, values1: tf.Tensor, *,
-            ndim0: int, ndim1: int,
-            dot_axes: tuple[Iterable[int], Iterable[int]],
-            bat_axes: tuple[Iterable[int], Iterable[int]],
+        values0: tf.Tensor, values1: tf.Tensor, *,
+        ndim0: int, ndim1: int,
+        dot_axes: tuple[Iterable[int], Iterable[int]],
+        bat_axes: tuple[Iterable[int], Iterable[int]],
     ) -> tuple[tf.Tensor, tuple[tuple[int, ...], tuple[int, ...]]]:
         bat_axes0, bat_axes1 = tuple(bat_axes[0]), tuple(bat_axes[1])
         if not len(bat_axes0) == len(bat_axes1):
             raise ValueError("len(bat_axes[0]) != len(bat_axes[1])")
         del bat_axes
 
         dot_axes0, dot_axes1 = tuple(dot_axes[0]), tuple(dot_axes[1])
```

### Comparing `BraAndKet-0.8.2/src/braandket/model/model.py` & `BraAndKet-0.8.3/src/braandket/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import weakref
 from typing import Iterable, Optional
 
 from braandket.backend import Backend
+from braandket.space import KetSpace
 from braandket.tensor import PureStateTensor, StateTensor
-from braandket.space.hilbert_space import KetSpace
 
 
 # state
 
 class QState:
     def __init__(self, tensor: StateTensor, related_systems: Iterable['QModel'] = ()):
         self._tensor = tensor
```

### Comparing `BraAndKet-0.8.2/src/braandket/space/hilbert_space.py` & `BraAndKet-0.8.3/src/braandket/space/hilbert_space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.2/src/braandket/space/num_space.py` & `BraAndKet-0.8.3/src/braandket/space/num_space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.2/src/braandket/space/space.py` & `BraAndKet-0.8.3/src/braandket/space/space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.2/src/braandket/tensor/operations.py` & `BraAndKet-0.8.3/src/braandket/tensor/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from typing import Any, Callable, Iterable, Optional, Union
 
 from braandket.backend import Backend, ValuesType, get_default_backend
 from braandket.space import HSpace, KetSpace, NumSpace, Space
 from .special import NumericTensor, OperatorTensor, PureStateTensor
 from .tensor import QTensor
 
-
 # constants
 
-def zero(*, backend: Optional[Backend] = None):
-    return QTensor.of(0, (), backend=backend)
+e = math.e
+pi = math.pi
 
 
-def one(*, backend: Optional[Backend] = None):
-    return QTensor.of(1, (), backend=backend)
+# constructors
 
+def zero(*, backend: Optional[Backend] = None) -> NumericTensor:
+    return NumericTensor.of(0, (), backend=backend)
 
-pi = math.pi
 
+def one(*, backend: Optional[Backend] = None) -> NumericTensor:
+    return NumericTensor.of(1, (), backend=backend)
 
-# constructors
 
 def zeros(space: NumSpace, *, backend: Optional[Backend] = None) -> NumericTensor:
     backend = backend or get_default_backend()
     values = backend.zeros((space.n,))
     return NumericTensor(values, (space,), backend)
```

### Comparing `BraAndKet-0.8.2/src/braandket/tensor/special.py` & `BraAndKet-0.8.3/src/braandket/tensor/special.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 # special tensors
 
 class NumericTensor(QTensor[ValuesType]):
 
     @classmethod
     def of(cls,
-            values: Union[QTensor, Any],
-            spaces: Optional[Iterable[Space]] = None, *,
-            backend: Optional[Backend] = None
+        values: Union[QTensor, Any],
+        spaces: Optional[Iterable[Space]] = None, *,
+        backend: Optional[Backend] = None
     ) -> 'NumericTensor':
         if isinstance(values, NumericTensor):
             return values
         if isinstance(values, QTensor):
             # noinspection PyTypeChecker
             return cls(values._values, values._spaces, values._backend)
         if spaces is None:
@@ -77,26 +77,26 @@
         all_ket_spaces = frozenset(self.ket_spaces)
         remain_ket_spaces_set = frozenset(spaces)
         traced_ket_spaces = all_ket_spaces - remain_ket_spaces_set
         return self.trace(*traced_ket_spaces)
 
     @abc.abstractmethod
     def probabilities(self,
-            *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
+        *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
     ) -> ValuesType:
         pass
 
 
 class PureStateTensor(StateTensor[ValuesType]):
 
     @classmethod
     def of(cls,
-            values: Union[QTensor, Any],
-            spaces: Optional[Iterable[Union[NumSpace, KetSpace]]] = None, *,
-            backend: Optional[Backend] = None
+        values: Union[QTensor, Any],
+        spaces: Optional[Iterable[Union[NumSpace, KetSpace]]] = None, *,
+        backend: Optional[Backend] = None
     ) -> 'PureStateTensor':
         if isinstance(values, PureStateTensor):
             return values
         if isinstance(values, QTensor):
             # noinspection PyTypeChecker
             return cls(values._values, values._spaces, values._backend)
         return cls(values, spaces, backend or get_default_backend())
@@ -142,31 +142,31 @@
             indices = tuple(indices)
         return PureStateTensor.of(self[indices])
 
     def trace(self, *spaces: KetSpace) -> 'MixedStateTensor':
         return MixedStateTensor.of(self @ self.ct).trace(*spaces)
 
     def amplitudes(self,
-            *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
+        *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
     ) -> ValuesType:
         return self.values(*spaces)
 
     def probabilities(self,
-            *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
+        *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
     ) -> ValuesType:
         amplitudes = self.amplitudes(*spaces)
         return self.backend.mul(self.backend.conj(amplitudes), amplitudes)
 
 
 class MixedStateTensor(StateTensor[ValuesType]):
     @classmethod
     def of(cls,
-            values: Union[QTensor, Any],
-            spaces: Optional[Iterable[Union[NumSpace, KetSpace]]] = None, *,
-            backend: Optional[Backend] = None
+        values: Union[QTensor, Any],
+        spaces: Optional[Iterable[Union[NumSpace, KetSpace]]] = None, *,
+        backend: Optional[Backend] = None
     ) -> 'MixedStateTensor':
         if isinstance(values, MixedStateTensor):
             return values
         if isinstance(values, QTensor):
             # noinspection PyTypeChecker
             return cls(values._values, values._spaces, values._backend)
         return cls(values, spaces, backend or get_default_backend())
@@ -206,15 +206,15 @@
 
     def trace(self, *spaces: KetSpace) -> 'MixedStateTensor':
         values, spaces = self.values_and_slices(*spaces)
         ket_axes, bra_axes = _index_spaces_pairs(spaces)
         return self.backend.trace(values, (ket_axes, bra_axes))
 
     def probabilities(self,
-            *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
+        *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
     ) -> ValuesType:
         bra_spaces = []
         for space_or_pair in spaces:
             if isinstance(space_or_pair, Space):
                 space, index = space_or_pair, None
             else:
                 space, index = space_or_pair
@@ -225,34 +225,34 @@
                     bra_spaces.append((space.ct, index))
         return self.values(*spaces, *bra_spaces)
 
 
 class OperatorTensor(QTensor[ValuesType]):
     @classmethod
     def of(cls,
-            values: Union[QTensor, Any],
-            spaces: Optional[Iterable[Space]] = None, *,
-            backend: Optional[Backend] = None
+        values: Union[QTensor, Any],
+        spaces: Optional[Iterable[Space]] = None, *,
+        backend: Optional[Backend] = None
     ) -> 'OperatorTensor':
         if isinstance(values, OperatorTensor):
             return values
         if isinstance(values, QTensor):
             # noinspection PyTypeChecker
             return cls(values._values, values._spaces, values._backend)
         return cls(values, spaces, backend or get_default_backend())
 
     @classmethod
     def from_matrix(cls,
-            matrix: ValuesType,
-            ket_spaces: Iterable[KetSpace],
-            num_spaces: Iterable[KetSpace] = (), *,
-            backend: Optional[Backend] = None
+        matrix: ValuesType,
+        ket_spaces: Iterable[KetSpace] | KetSpace,
+        num_spaces: Iterable[NumSpace] | NumSpace = (), *,
+        backend: Optional[Backend] = None
     ) -> 'OperatorTensor':
-        num_spaces = tuple(num_spaces)
-        ket_spaces = tuple(ket_spaces)
+        num_spaces = (num_spaces,) if isinstance(num_spaces, NumSpace) else tuple(num_spaces)
+        ket_spaces = (ket_spaces,) if isinstance(ket_spaces, KetSpace) else tuple(ket_spaces)
         bra_spaces = tuple(space.ct for space in ket_spaces)
         spaces = num_spaces + ket_spaces + bra_spaces
         backend = backend or get_default_backend()
         shape = tuple(space.n for space in spaces)
         values = backend.reshape(matrix, shape)
         return cls(values, spaces, backend)
```

### Comparing `BraAndKet-0.8.2/src/braandket/tensor/tensor.py` & `BraAndKet-0.8.3/src/braandket/tensor/tensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 from typing import Any, Generic, Iterable, Optional, Union
 
 from braandket.backend import Backend, ValuesType, get_default_backend
 from braandket.space import BraSpace, HSpace, KetSpace, NumSpace, Space
+from braandket.utils import iter_structure
 
 
 class QTensor(Generic[ValuesType], abc.ABC):
 
     @classmethod
     def of(cls, values: Any, spaces: Iterable[Space], *, backend: Optional[Backend] = None) -> 'QTensor':
         if backend is None:
@@ -61,15 +62,15 @@
         return self._spaces
 
     def values(self, *slices: Union[Space, tuple[Space, Union[int, None]]]) -> ValuesType:
         """ get values from this tensor """
         return self.values_and_slices(*slices)[0]
 
     def values_and_slices(self,
-            *slices: Union[Space, tuple[Space, Union[int, None]]]
+        *slices: Union[Space, tuple[Space, Union[int, None]]]
     ) -> tuple[ValuesType, tuple[Union[Space, tuple[Space, int]], ...]]:
         if len(slices) == 0:
             return self._values, self._spaces
 
         # parse arguments
         sp_slices = slices
         spaces = []
@@ -304,34 +305,30 @@
         from .special import OperatorTensor
         return OperatorTensor.of(self)
 
     # inflate & flatten
 
     @classmethod
     def inflate(cls,
-            values: ValuesType,
-            spaces: Iterable[Union[NumSpace, Iterable[KetSpace], Iterable[BraSpace]]], *,
-            backend: Optional[Backend] = None
+        values: ValuesType,
+        spaces: Iterable[Union[NumSpace, KetSpace, BraSpace, Iterable[Union[NumSpace, KetSpace, BraSpace]]]], *,
+        backend: Optional[Backend] = None
     ) -> 'QTensor':
         if backend is None:
             backend = get_default_backend()
-
-        *num_spaces, ket_spaces, bra_spaces = spaces
-
-        shape = (*(space.n for space in num_spaces),
-                 *(space.n for space in ket_spaces),
-                 *(space.n for space in bra_spaces))
+        spaces = tuple(iter_structure(spaces))
+        shape = tuple(space.n for space in spaces)
         values = backend.reshape(values, shape)
-        return cls.of(values, (*num_spaces, *ket_spaces, *bra_spaces), backend=backend)
+        return cls.of(values, spaces, backend=backend)
 
     def flatten(self,
-            spaces: Optional[Iterable[Union[NumSpace, KetSpace, BraSpace]]] = None, *,
-            num_spaces: Optional[Iterable[NumSpace]] = None,
-            ket_spaces: Optional[Iterable[KetSpace]] = None,
-            bra_spaces: Optional[Iterable[BraSpace]] = None,
+        spaces: Optional[Iterable[Union[NumSpace, KetSpace, BraSpace]]] = None, *,
+        num_spaces: Optional[Iterable[NumSpace]] = None,
+        ket_spaces: Optional[Iterable[KetSpace]] = None,
+        bra_spaces: Optional[Iterable[BraSpace]] = None,
     ) -> tuple[ValuesType, tuple[Union[NumSpace, tuple[KetSpace, ...], tuple[BraSpace, ...]], ...]]:
         num_spaces_sl = tuple(space for space in self.spaces if isinstance(space, NumSpace))
         ket_spaces_sl = tuple(space for space in self.spaces if isinstance(space, KetSpace))
         bra_spaces_sl = tuple(space for space in self.spaces if isinstance(space, BraSpace))
 
         spaces = tuple(spaces) if spaces is not None else ()
         num_spaces_sp = tuple(space for space in spaces if isinstance(space, NumSpace))
@@ -357,18 +354,18 @@
         shape = (*(space.n for space in num_spaces),
                  prod(*(space.n for space in ket_spaces)),
                  prod(*(space.n for space in bra_spaces)))
         values = self.backend.reshape(self.values(*num_spaces, *ket_spaces, *bra_spaces), shape)
         return values, (*num_spaces, tuple(ket_spaces), tuple(bra_spaces))
 
     def flattened_values(self,
-            spaces: Optional[Iterable[Union[NumSpace, KetSpace, BraSpace]]] = None, *,
-            num_spaces: Optional[Iterable[NumSpace]] = None,
-            ket_spaces: Optional[Iterable[KetSpace]] = None,
-            bra_spaces: Optional[Iterable[BraSpace]] = None,
+        spaces: Optional[Iterable[Union[NumSpace, KetSpace, BraSpace]]] = None, *,
+        num_spaces: Optional[Iterable[NumSpace]] = None,
+        ket_spaces: Optional[Iterable[KetSpace]] = None,
+        bra_spaces: Optional[Iterable[BraSpace]] = None,
     ) -> ValuesType:
         return self.flatten(
             spaces,
             num_spaces=num_spaces,
             ket_spaces=ket_spaces,
             bra_spaces=bra_spaces
         )[0]
```

### Comparing `BraAndKet-0.8.2/src/braandket/utils/utils.py` & `BraAndKet-0.8.3/src/braandket/utils/utils.py`

 * *Files identical despite different names*

