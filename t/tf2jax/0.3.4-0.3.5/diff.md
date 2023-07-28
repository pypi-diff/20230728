# Comparing `tmp/tf2jax-0.3.4.tar.gz` & `tmp/tf2jax-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2jax-0.3.4.tar", last modified: Fri Apr 21 09:07:46 2023, max compression
+gzip compressed data, was "tf2jax-0.3.5.tar", last modified: Fri Jul 28 13:23:23 2023, max compression
```

## Comparing `tf2jax-0.3.4.tar` & `tf2jax-0.3.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 09:07:33.000000 tf2jax-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 09:07:33.000000 tf2jax-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-21 09:07:46.049760 tf2jax-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-21 09:07:33.000000 tf2jax-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 09:07:33.000000 tf2jax-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 09:07:33.000000 tf2jax-0.3.4/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:07:46.049760 tf2jax-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-21 09:07:33.000000 tf2jax-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/linalg_ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/numpy_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/numpy_compat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    86540 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    76011 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    36772 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/roundtrip_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    46673 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/tf2jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/tf2jax_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/xla_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/mhlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/mhlo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/tf2jax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:23.728511 tf2jax-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 13:23:14.000000 tf2jax-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-28 13:23:14.000000 tf2jax-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-07-28 13:23:23.728511 tf2jax-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-07-28 13:23:14.000000 tf2jax-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 13:23:14.000000 tf2jax-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 13:23:14.000000 tf2jax-0.3.5/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:23:23.728511 tf2jax-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-28 13:23:14.000000 tf2jax-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:23.724511 tf2jax-0.3.5/tf2jax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:23.724511 tf2jax-0.3.5/tf2jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/linalg_ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/numpy_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/numpy_compat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88083 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77144 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/roundtrip_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/sharding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50700 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/tf2jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20233 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/tf2jax_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/_src/xla_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:23.728511 tf2jax-0.3.5/tf2jax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/experimental/mhlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/experimental/mhlo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/experimental/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-28 13:23:14.000000 tf2jax-0.3.5/tf2jax/tf2jax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:23:23.724511 tf2jax-0.3.5/tf2jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-07-28 13:23:23.000000 tf2jax-0.3.5/tf2jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-28 13:23:23.000000 tf2jax-0.3.5/tf2jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:23:23.000000 tf2jax-0.3.5/tf2jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:23:23.000000 tf2jax-0.3.5/tf2jax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-28 13:23:23.000000 tf2jax-0.3.5/tf2jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 13:23:23.000000 tf2jax-0.3.5/tf2jax.egg-info/top_level.txt
```

### Comparing `tf2jax-0.3.4/LICENSE` & `tf2jax-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/PKG-INFO` & `tf2jax-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: tf2jax
-Version: 0.3.4
+Version: 0.3.5
 Summary: TF2JAX: Convert TensorFlow to JAX
 Home-page: https://github.com/deepmind/tf2jax
 Author: DeepMind
 Author-email: tf2jax-dev@google.com
 License: Apache 2.0
 Keywords: jax tensorflow conversion translate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
```

### Comparing `tf2jax-0.3.4/README.md` & `tf2jax-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/setup.py` & `tf2jax-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Libraries',
     ],
```

### Comparing `tf2jax-0.3.4/tf2jax/__init__.py` & `tf2jax-0.3.5/tf2jax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from tf2jax._src.tf2jax import AnnotatedFunction
 
 from tf2jax._src.tf2jax import convert
 from tf2jax._src.tf2jax import convert_from_restored
 from tf2jax._src.tf2jax import convert_functional
 from tf2jax._src.tf2jax import convert_functional_from_restored
 
-__version__ = "0.3.4"
+from tf2jax._src.tf2jax import MissingInputError
+
+__version__ = "0.3.5"
 
 #  _________________________________________
 # / Please don't use symbols in `_src` they \
 # \ are not part of the tf2jax public API.    /
 #  -----------------------------------------
 #         \   ^__^
 #          \  (oo)\_______
```

### Comparing `tf2jax-0.3.4/tf2jax/_src/__init__.py` & `tf2jax-0.3.5/tf2jax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/_src/config.py` & `tf2jax-0.3.5/tf2jax/_src/config.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/_src/linalg_ops_test.py` & `tf2jax-0.3.5/tf2jax/_src/linalg_ops_test.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/_src/numpy_compat.py` & `tf2jax-0.3.5/tf2jax/_src/numpy_compat.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/_src/numpy_compat_test.py` & `tf2jax-0.3.5/tf2jax/_src/numpy_compat_test.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/_src/ops.py` & `tf2jax-0.3.5/tf2jax/_src/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import Any, Callable, List, Optional, Mapping, Protocol, Sequence, Set, Tuple, Union
 
 from absl import logging
 
 import jax
 from jax._src.lax import control_flow as lax_control_flow
 from jax.experimental import checkify
+from jax.lib import xla_client
 import jax.numpy as jnp
 import numpy as np
 import tensorflow as tf
 from tf2jax._src import config
 from tf2jax._src import numpy_compat as anp
 from tf2jax._src import xla_utils
 
@@ -269,19 +270,25 @@
   _check_attrs(proto, {"Tidx", "keep_dims"})
   keep_dims = proto.attr["keep_dims"].b
   return lambda x, axis: anp.any_(x, axis=axis.tolist(), keepdims=keep_dims)
 
 
 @register_operation("Assert")
 def _assert(proto):
+  """Parse an Assert Op."""
   _check_attrs(proto, {"T", "summarize"})
 
   logging.warning("Assert has no effect.")
 
-  return lambda cond, *data: _EMPTY_RETURN_VALUE
+  def _func(cond, *data):
+    del cond, data
+    # TODO(shaobohou) Use checkify?
+    return _EMPTY_RETURN_VALUE
+
+  return _func
 
 
 @register_operation("AvgPool")
 def _avg_pool(proto):
   """Parse a AvgPool Op."""
   _check_attrs(
       proto,
@@ -2415,21 +2422,34 @@
 
 
 @register_operation("XlaSharding")
 def _xla_sharding(proto):
   """Parse a XlaSharding op."""
   _check_attrs(proto, {"T", "sharding", "unspecified_dims"})
 
-  sharding = proto.attr["sharding"].s
-  if sharding:
-    raise ValueError(
-        f"Sharding is not yet supported (except identity), found {proto}."
-    )
+  unspecified_dims = tuple(proto.attr["unspecified_dims"].list.i)
+  if unspecified_dims:
+    raise ValueError(f"{unspecified_dims=} is not yet supported.")
+
+  sharding_str = proto.attr["sharding"].s
+
+  # Return identity if sharding annotation is empty.
+  if not sharding_str:
+    return lambda x: x
+
+  sharding = xla_client.OpSharding()
+  sharding.ParseFromString(sharding_str)
+  jax_sharding = jax.sharding.GSPMDSharding(jax.devices(), sharding)
 
-  return lambda x: x
+  # TODO(b/235450851) Remove jax.jit once wsc is usable outside of jit.
+  @jax.jit
+  def _func(x: jnp.ndarray) -> jnp.ndarray:
+    return jax.lax.with_sharding_constraint(x, jax_sharding)
+
+  return _func
 
 
 def _maybe_get_jaxpreqn(
     jaxpr: jax.core.ClosedJaxpr) -> Optional[jax.core.JaxprEqn]:
   def is_all_vars(vs):
     return all([isinstance(v, jax.core.Var) for v in vs])
 
@@ -2790,7 +2810,38 @@
   """Parse a XlaSelectAndScatter op."""
   _check_attrs(proto, {"T", "Tindices", "scatter", "select"})
 
   scatter = proto.attr["scatter"].func.name
   select = proto.attr["select"].func.name
 
   return _XlaSelectAndScatter(dict(scatter=scatter, select=select))
+
+
+def _searchsorted(a: jnp.ndarray, v: jnp.ndarray, side: str):
+  """Vmapped version of searchsorted to implement LowerBound and UpperBound."""
+  return jax.vmap(
+      functools.partial(jnp.searchsorted, side=side),
+      in_axes=0,
+      out_axes=0,
+  )(a, v)
+
+
+def _lower_upper_bound(proto, side: str):
+  """Parse a LowerBound or UpperBound op using searchsorted."""
+  _check_attrs(proto, {"T", "Tvalues", "out_type"})
+  dtype = tf.as_dtype(proto.attr["out_type"].type)
+  if dtype != tf.int32:
+    raise ValueError(
+        f"Return type {dtype} not supported for LowerBound and UpperBound.")
+  return lambda a, v: _searchsorted(a, v, side=side)
+
+
+@register_operation("LowerBound")
+def _lower_bound(proto):
+  """Parse a LowerBound op."""
+  return _lower_upper_bound(proto, side="left")
+
+
+@register_operation("UpperBound")
+def _upper_bound(proto):
+  """Parse an UpperBound op."""
+  return _lower_upper_bound(proto, side="right")
```

### Comparing `tf2jax-0.3.4/tf2jax/_src/ops_test.py` & `tf2jax-0.3.5/tf2jax/_src/ops_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1022,14 +1022,21 @@
     )
 
     self._test_convert(lambda a, x: tf.raw_ops.Igamma(a=a, x=x), inputs)
     self._test_convert(lambda a, x: tf.raw_ops.Igammac(a=a, x=x), inputs)
 
   @chex.variants(with_jit=True, without_jit=True)
   def test_inplace_add(self):
+    if test_util.parse_version(tf.version.VERSION) >= test_util.parse_version(
+        "2.14.0"
+    ):
+      self.skipTest(
+          f"Requires earlier than tf 2.14.0, found {tf.version.VERSION}."
+      )
+
     np.random.seed(42)
 
     @tf.function
     def inplace_add(x, idx, val):
       return tf.raw_ops.InplaceAdd(x=x, i=idx, v=val)
 
     inputs = [
@@ -1050,14 +1057,21 @@
         ]
         self._test_convert(inplace_add, tpu_inputs)
       else:
         raise e
 
   @chex.variants(with_jit=True, without_jit=True)
   def test_inplace_update(self):
+    if test_util.parse_version(tf.version.VERSION) >= test_util.parse_version(
+        "2.14.0"
+    ):
+      self.skipTest(
+          f"Requires earlier than tf 2.14.0, found {tf.version.VERSION}."
+      )
+
     np.random.seed(42)
 
     @tf.function
     def inplace_update(x, idx, val):
       return tf.raw_ops.InplaceUpdate(x=x, i=idx, v=val)
 
     inputs = [
@@ -2265,10 +2279,31 @@
       return tf.raw_ops.VarHandleOp(dtype=tf.float32, shape=(3, 5), name="blah")
 
     with self.assertRaisesRegex(
         ValueError, "VarHandleOp `blah` cannot be evaluated"
     ):
       self._test_convert(var_handle, [])
 
+  @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.parameters(
+      "LowerBound",
+      "UpperBound",
+      "SearchSorted",
+  )
+  def test_lower_upper_bound(self, op_name):
+    np.random.seed(42)
+    inputs = (
+        np.array([[0, 1, 2, 3, 4], [-4, -3, -2, -1, 0]], dtype=np.float32),
+        np.array(
+            [[3.5, 0, 1.5, 10, -1], [-3.5, 0, -1.5, -10, 1]], dtype=np.float32)
+    )
+    if op_name == "SearchSorted":
+      tf_func = lambda x, y: tf.searchsorted(x, y, out_type=tf.int32)
+    else:
+      # LowerBound and UpperBound expect keyword arguments.
+      def tf_func(x, y):
+        return getattr(tf.raw_ops, op_name)(sorted_inputs=x, values=y)
+    self._test_convert(tf_func, inputs)
+
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tf2jax-0.3.4/tf2jax/_src/roundtrip_test.py` & `tf2jax-0.3.5/tf2jax/_src/roundtrip_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,14 @@
 _NATIVE_SERIALIZATION = flags.DEFINE_bool(
     "use_jax2tf_native_serialization_in_roundtrip_test",
     _bool_env("USE_JAX2TF_NATIVE_SERIALIZATION_IN_ROUNDTRIP_TEST", False),
     "Whether to call jax2tf.convert with native serialization enabled.",
 )
 
 
-def _parse_version(version: str):
-  return tuple(int(x.split("-")[0]) for x in version.split("."))
-
-
 def _compute_gradients(func, *inputs):
   def fn(*args):
     return jax.tree_util.tree_leaves(func(*args))[0]
   return jax.grad(lambda *args: jnp.sum(fn(*args)))(*inputs)
 
 
 def _jax2tf_convert(func, **kwargs):
@@ -695,14 +691,118 @@
                      [None, 8])
     new_tf_outputs = concrete_new_tf_forward(inputs)
     self.assertAllClose(new_tf_outputs, jax_outputs)
 
   @chex.variants(with_jit=True)
   @parameterized.named_parameters(
       chex.params_product(
+          (("without_gradient", False), ("with_gradient", True)),
+          (("disable_xla", False), ("enable_xla", True)),
+          named=True,
+      )
+  )
+  def test_polymorphic_shape_refinement_dot(self, with_grad, enable_xla):
+    if uses_native_serialization():
+      if not enable_xla:
+        self.skipTest("native_serialization does not support enable_xla=False.")
+
+    @jax.jit
+    def forward(x, w):
+      return jnp.dot(x, w)
+
+    x = np.array(range(12), dtype=np.float32).reshape((3, 4))
+    w = np.array(range(20), dtype=np.float32).reshape((4, 5))
+    expected_outputs = forward(x, w)
+
+    # JAX -> TF
+    tf_fn = _jax2tf_convert(
+        forward,
+        polymorphic_shapes=["(b, _)", None],
+        with_gradient=with_grad,
+        enable_xla=enable_xla)
+    tf_fn = tf.function(tf_fn, autograph=False)
+    concrete_tf_fn = tf_fn.get_concrete_function(
+        tf.TensorSpec(shape=(None, 4)), tf.TensorSpec(shape=(4, 5)))
+    tf_outputs = concrete_tf_fn(x, w)
+    self.assertAllClose(expected_outputs, tf_outputs)
+
+    # JAX -> TF -> JAX
+    jax_fn = tf2jax.convert_functional(
+        tf_fn, np.zeros_like(x), np.zeros_like(w)
+    )
+    jax_outputs = self.variant(jax_fn)(x, w)
+    self.assertAllClose(expected_outputs, jax_outputs)
+
+    # JAX -> TF -> JAX -> TF
+    tf_fn2 = _jax2tf_convert(
+        jax_fn,
+        polymorphic_shapes=["(b, _)", None],
+        with_gradient=with_grad,
+        enable_xla=enable_xla)
+    tf_fn2 = tf.function(tf_fn2, autograph=False)
+    concrete_tf_fn2 = tf_fn2.get_concrete_function(
+        tf.TensorSpec(shape=(None, 4)), tf.TensorSpec(shape=(4, 5)))
+    tf_outputs2 = concrete_tf_fn2(x, w)
+    self.assertAllClose(expected_outputs, tf_outputs2)
+
+  @chex.variants(with_jit=True)
+  @parameterized.named_parameters(
+      chex.params_product(
+          (("without_gradient", False), ("with_gradient", True)),
+          (("disable_xla", False), ("enable_xla", True)),
+          named=True,
+      )
+  )
+  def test_polymorphic_shape_refinement_broadcast(self, with_grad, enable_xla):
+    if uses_native_serialization():
+      if not enable_xla:
+        self.skipTest("native_serialization does not support enable_xla=False.")
+
+    @jax.jit
+    def forward(x, y):
+      return (jnp.broadcast_to(x, y.shape), x + y)
+
+    x = np.array(range(12), dtype=np.float32).reshape((3, 4))
+    y = np.array(range(24), dtype=np.float32).reshape((2, 3, 4))
+    expected_outputs = forward(x, y)
+
+    # JAX -> TF
+    tf_fn = _jax2tf_convert(
+        forward,
+        polymorphic_shapes=["(b, _)", "(_, b, _)"],
+        with_gradient=with_grad,
+        enable_xla=enable_xla)
+    tf_fn = tf.function(tf_fn, autograph=False)
+    concrete_tf_fn = tf_fn.get_concrete_function(
+        tf.TensorSpec(shape=(None, 4)), tf.TensorSpec(shape=(2, None, 4)))
+    tf_outputs = concrete_tf_fn(x, y)
+    self.assertAllClose(expected_outputs, tf_outputs)
+
+    # JAX -> TF -> JAX
+    jax_fn = tf2jax.convert_functional(
+        tf_fn, np.zeros_like(x), np.zeros_like(y)
+    )
+    jax_outputs = self.variant(jax_fn)(x, y)
+    self.assertAllClose(expected_outputs, jax_outputs)
+
+    # JAX -> TF -> JAX -> TF
+    tf_fn2 = _jax2tf_convert(
+        jax_fn,
+        polymorphic_shapes=["(b, _)", "(_, b, _)"],
+        with_gradient=with_grad,
+        enable_xla=enable_xla)
+    tf_fn2 = tf.function(tf_fn2, autograph=False)
+    concrete_tf_fn2 = tf_fn2.get_concrete_function(
+        tf.TensorSpec(shape=(None, 4)), tf.TensorSpec(shape=(2, None, 4)))
+    tf_outputs2 = concrete_tf_fn2(x, y)
+    self.assertAllClose(expected_outputs, tf_outputs2)
+
+  @chex.variants(with_jit=True)
+  @parameterized.named_parameters(
+      chex.params_product(
           (("with_gradient", True),),
           (("disable_xla", False), ("enable_xla", True)),
           named=True,
       ))
   def test_custom_gradient(self, with_grad, enable_xla):
     if uses_native_serialization():
       if not enable_xla:
@@ -1010,15 +1110,17 @@
         forward, inputs,
         with_grad=with_grad,
         enable_xla=enable_xla,
         with_custom_grad=with_custom_grad,
         grad_tols=tols)
 
   def test_explicit_native_serialization(self):
-    if _parse_version(tf.version.VERSION) < _parse_version("2.12.0"):
+    if test_util.parse_version(tf.version.VERSION) < test_util.parse_version(
+        "2.12.0"
+    ):
       self.skipTest(f"Requires tf 2.12.0 or later, found {tf.version.VERSION}.")
 
     def forward(x):
       return x + 3.14
 
     tf_fn = jax2tf.convert(forward, native_serialization=True)
     tf_fn = tf.function(tf_fn, autograph=False)
```

### Comparing `tf2jax-0.3.4/tf2jax/_src/test_util.py` & `tf2jax-0.3.5/tf2jax/_src/test_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 from absl import logging
 from absl.testing import parameterized
 
 import jax
 import tensorflow as tf
 
 
+def parse_version(version: str):
+  return tuple(int(x.split("-")[0]) for x in version.split("."))
+
+
 class TestCase(parameterized.TestCase, tf.test.TestCase):
   """Base class for all tests."""
 
   def setUp(self):
     super().setUp()
     # Ensure that all TF ops are created on the proper device (TPU, GPU or CPU)
     jax_default_device = jax.default_backend().upper()
```

### Comparing `tf2jax-0.3.4/tf2jax/_src/tf2jax.py` & `tf2jax-0.3.5/tf2jax/_src/tf2jax.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Experimental functions for converting TF graphs to Jax functions."""
 
 import collections
+import functools
 import inspect
 import itertools
+import json
 from typing import Any, Callable, Iterable, Iterator, Optional, Mapping, NamedTuple, Sequence, Tuple, Union
 
 from absl import logging
 
 import jax
 import jax.numpy as jnp
 import numpy as np
@@ -689,34 +691,74 @@
     subgraph_map = {v.name: v for v in subgraph}
     for node in nodes:
       if node.name in subgraph_map:
         processed.append(node)
         if node == self.output_node:
           new_nodes.append(self)
       else:
+        # Rewire control inputs to point to the subgraph.
+        new_control_inputs = tuple(
+            v._replace(op_name=self.name) if v.op_name in subgraph_map else v
+            for v in node.control_inputs
+        )
+        node.control_inputs = new_control_inputs
         new_nodes.append(node)
 
-    assert len(processed) == len(subgraph)
+    assert len(processed) == len(subgraph), (len(processed), len(subgraph))
     return tuple(new_nodes)
 
 
 def _contains_custom_gradient(node: tf.compat.v1.NodeDef) -> bool:
   # IdentityN are used to override gradients.
   return node.op == "IdentityN"
 
 
+def _get_consumers_and_producers_fns(nodes):
+  """Returns functions to get consumers and producers for a node."""
+  op_map = {n.name: (idx, n) for idx, n in enumerate(nodes)}
+
+  # Maps node name to immediate consumers.
+  consumers_map = {n.name: [] for n in nodes}
+  for node in nodes:
+    for inp in node.inputs:
+      consumers_map[inp.op_name].append(node.name)
+
+  # Get all consumers for a node.
+  @functools.lru_cache(None)
+  def get_consumers(node_name: str) -> list[str]:
+    if not consumers_map[node_name]:
+      return [node_name]
+    else:
+      return sum([get_consumers(n) for n in consumers_map[node_name]], [])
+
+  # Get all producers for a node.
+  @functools.lru_cache(None)
+  def get_producers(node_name: str):
+    _, node = op_map[node_name]
+    if node.inputs:
+      return set.union(
+          set([node_name]), *[get_producers(x.op_name) for x in node.inputs]
+      )
+    else:
+      return set([node_name])
+
+  return get_consumers, get_producers
+
+
 # Extract subgraphs for custom_gradient.
 def _extract_subgraphs(graphdef, nodes, library):
   """Extract all subgraphs with their own custom_gradients."""
 
   op_map = {n.name: (idx, n) for idx, n in enumerate(nodes)}
   if _EMPTY_RETURN_OP_NAME in op_map:
     logging.info("Skip subgraph extraction for function with no return values.")
     return {}
 
+  get_consumers, get_producers = _get_consumers_and_producers_fns(nodes)
+
   subgraphs = {}
   for node in graphdef.node:
     if _contains_custom_gradient(node):
       grad_fn_name = str(node.attr["_gradient_op_type"].s, "utf-8")
       grad_fn = library[grad_fn_name]
 
       output_node = op_map[node.name][1]
@@ -752,14 +794,36 @@
         if inp not in used_inputs:
           unused_captures.append(inp)
         elif is_internal:
           internal_captures.append(inp)
         else:
           external_captures.append(inp)
 
+      # Find side-effects, i.e. nodes that depends on the subgraph but do not
+      # feed into the subgraph outputs, e.g. shape check asserts from jax2tf.
+      side_effects = []
+      subgraph_and_output = subgraph | set([output_node.name])
+      for node in nodes:
+        if node.name not in subgraph_and_output:
+          if any(inp.op_name in subgraph for inp in node.inputs):
+            side_effects.append(set(get_consumers(node.name)))
+      # Gather all dependencies of side-effects, assume they are not depended on
+      # by other nodes outside of the subgraph + side-effects. This may only
+      # work for shape check assert added by jax2tf.
+      side_effects = set.union(set(), *side_effects)
+      side_effect_deps = set()
+      for x in set.union(set(), *[get_producers(x) for x in side_effects]):
+        if op_map[x][1].op != "Placeholder":
+          side_effect_deps.add(x)
+      # Merge side-effects and dependencies into the subgraph.
+      subgraph = subgraph | side_effects | side_effect_deps
+      output_node.control_inputs = output_node.control_inputs + tuple(
+          _TensorEdge(op_name=x, is_control=True) for x in side_effects
+      )
+
       excluded = inputs + unused_captures + external_captures
       subgraph = subgraph.difference(set([x.op_name for x in excluded]))
       sub_nodes = [op_map[x] for x in subgraph]
       sub_nodes = [x for _, x in sorted(sub_nodes)]
       subgraphs[grad_fn_name] = _Subgraph(
           subgraph=tuple(sub_nodes),
           captures=tuple(external_captures),
@@ -837,14 +901,49 @@
   attr: Optional[Mapping[str, tf.compat.v1.AttrValue]] = None
 
 
 class _GraphDef(NamedTuple):
   node: Tuple[Union[tf.compat.v1.NodeDef, _NodeDef], ...]
 
 
+def _validate_inputs(
+    signature: inspect.Signature,
+    structured_specs: Any,
+    input_map: Mapping[str, Any],
+) -> str:
+  """Validate inputs against input specs."""
+
+  class _ExpectedArg:
+    def __init__(self, path: Tuple[Any, ...], spec: Any):
+      self.path = path
+      self.spec = spec
+
+  expected_args = [
+      _ExpectedArg(p, v) for p, v in tree.flatten_with_path(structured_specs)
+  ]
+  expected_tree = tree.unflatten_as(structured_specs, expected_args)
+
+  def format_spec(spec: tf.TensorSpec) -> str:
+    return "{}[{}]".format(spec.dtype.name, ",".join(map(str, spec.shape)))
+
+  def check_arg(arg: _ExpectedArg):
+    arg_desc = "UNUSED" if arg.spec is _UNUSED_INPUT else format_spec(arg.spec)
+    return "." if arg.path in input_map else arg_desc
+
+  checked_args, checked_kwargs = tree.map_structure(check_arg, expected_tree)
+  bound_checked_args = signature.bind(*checked_args, **checked_kwargs)
+  # TODO(b/282901848) Use a better pretty printer than json which does not
+  # render namedtuple correctly.
+  return json.dumps(bound_checked_args.arguments, indent=4)
+
+
+class MissingInputError(Exception):
+  ...
+
+
 def _convert(
     graphdef: Union[tf.compat.v1.GraphDef, _GraphDef],
     signature: inspect.Signature,
     structured_inputs,
     structured_outputs,
     captured_input_names: Optional[Tuple[str, ...]] = None,
     variable_map: Optional[Mapping[str, tf.Variable]] = None,
@@ -1011,15 +1110,23 @@
     if num_rng_required and rng is None:
       raise ValueError(f"PRNG key required for random ops, found rng={rng}.")
 
     bound_args = signature.bind(*func_args, **func_kwargs)
     bound_args.apply_defaults()
     inputs = dict(
         tree.flatten_with_path((bound_args.args, bound_args.kwargs)))
-    inputs = tuple([inputs[p] for p, _ in input_path_to_specs])
+    try:
+      inputs = tuple([inputs[p] for p, _ in input_path_to_specs])
+    except KeyError as e:
+      input_err_message = _validate_inputs(signature, structured_inputs, inputs)
+      err_message = (
+          "\nSome input(s) are missing (entries that map to dtype[shape]"
+          f" annotations in the following structure): \n{input_err_message}"
+      )
+      raise MissingInputError(err_message) from e
 
     if len(inputs) != len(input_names):
       raise ValueError(
           f"Expected {len(input_names)} args, found {len(inputs)}.")
 
     inputs = tree.map_structure(
         lambda x: x if isinstance(x, jnp.ndarray) else np.array(x), inputs)
```

### Comparing `tf2jax-0.3.4/tf2jax/_src/tf2jax_test.py` & `tf2jax-0.3.5/tf2jax/_src/tf2jax_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 
 import sonnet as snt
 import tensorflow as tf
 from tf2jax._src import config
 from tf2jax._src import tf2jax
 import tree
 
+# Parse absl flags test_srcdir and test_tmpdir.
+jax.config.parse_flags_with_absl()
+
 
 class TestDense(tf.Module):
 
   def __init__(self, input_dim, output_size, name=None):
     super().__init__(name=name)
     self.w = tf.Variable(tf.random.normal([input_dim, output_size]), name="w")
     self.b = tf.Variable(tf.zeros([output_size]), name="b")
@@ -529,14 +532,32 @@
     outputs = self.variant(jax_func)(inputs)
 
     self.assertAllClose(inputs + 1, outputs[0])
     self.assertIsNone(outputs[1])
     self.assertAllClose(inputs + 3.14, outputs[2])
 
   @chex.variants(with_jit=True, without_jit=True)
+  def test_missing_inputs(self):
+    params = dict(
+        a=np.array(3.14, np.float32), b=np.array([42, 47], np.float32)
+    )
+
+    @tf.function
+    def tf_func(x, params):
+      return x + params["a"] + params["b"]
+
+    np_inputs = np.array(range(6), dtype=np.float32).reshape(3, 2)
+    jax_func = tf2jax.convert_functional(
+        tf_func, *tree.map_structure(np.zeros_like, (np_inputs, params))
+    )
+
+    with self.assertRaises(tf2jax.MissingInputError):
+      self.variant(jax_func)(np_inputs, {"a": params["a"]})
+
+  @chex.variants(with_jit=True, without_jit=True)
   def test_missing_params(self):
     variables = dict(
         a=tf.Variable(3.14, trainable=True, name="aaa"),
         b=tf.Variable(42.0, trainable=False, name="bbb"),
     )
 
     @tf.function
```

### Comparing `tf2jax-0.3.4/tf2jax/_src/utils.py` & `tf2jax-0.3.5/tf2jax/_src/utils.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/_src/xla_utils.py` & `tf2jax-0.3.5/tf2jax/_src/xla_utils.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/experimental/__init__.py` & `tf2jax-0.3.5/tf2jax/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.4/tf2jax/experimental/mhlo_test.py` & `tf2jax-0.3.5/tf2jax/experimental/mhlo_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,25 +59,27 @@
     @jax.jit
     def fn(x):
       return x * 2 + 3.14
 
     inputs = (np.ones((3, 2), dtype=np.float32) * 10,)
     mhlo_text = _convert_to_mhlo(
         fn, jax.tree_map(np.zeros_like, inputs), dialect=dialect)
+    mhlo_module = mhlo.MhloModule(module=mhlo_text, fun_name="test_module")
+
     chex.assert_trees_all_close(
-        mhlo.mhlo_apply(*inputs, mhlo_text=mhlo_text), fn(*inputs))
+        mhlo.mhlo_apply(*inputs, module=mhlo_module), fn(*inputs))
 
     def make_top_fn(sub_fn):
       def top_fn(x):
         return sub_fn(x + 8) * 10
       return top_fn
 
     expect_top_fn = make_top_fn(fn)
     actual_top_fn = make_top_fn(
-        functools.partial(mhlo.mhlo_apply, mhlo_text=mhlo_text))
+        functools.partial(mhlo.mhlo_apply, module=mhlo_module))
     self._assert_all_close(expect_top_fn, actual_top_fn, inputs)
     _check_transforms(actual_top_fn, inputs, dialect=dialect)
 
   @chex.variants(with_jit=True, without_jit=True)
   @parameterized.named_parameters(
       ("mhlo", "mhlo"),
       ("stablehlo", "stablehlo"),
@@ -89,25 +91,26 @@
 
     inputs = (
         np.ones((3, 2), dtype=np.float32) * 10,
         np.ones((3, 2), dtype=np.float32) * 20,
     )
     mhlo_text = _convert_to_mhlo(
         fn, jax.tree_map(np.zeros_like, inputs), dialect=dialect)
+    mhlo_module = mhlo.MhloModule(module=mhlo_text, fun_name="test_module")
     chex.assert_trees_all_close(
-        mhlo.mhlo_apply(*inputs, mhlo_text=mhlo_text), fn(*inputs))
+        mhlo.mhlo_apply(*inputs, module=mhlo_module), fn(*inputs))
 
     def make_top_fn(sub_fn):
       def top_fn(x, y):
         return sub_fn(x + 8, y + 9) * 10
       return top_fn
 
     expect_top_fn = make_top_fn(fn)
     actual_top_fn = make_top_fn(
-        functools.partial(mhlo.mhlo_apply, mhlo_text=mhlo_text))
+        functools.partial(mhlo.mhlo_apply, module=mhlo_module))
     self._assert_all_close(expect_top_fn, actual_top_fn, inputs)
     _check_transforms(actual_top_fn, inputs, dialect=dialect)
 
   @chex.variants(with_jit=True, without_jit=True)
   @parameterized.named_parameters(
       ("mhlo", "mhlo"),
       ("stablehlo", "stablehlo"),
@@ -119,25 +122,55 @@
 
     inputs = (
         np.ones((3, 2), dtype=np.float32) * 10,
         np.ones((3, 2), dtype=np.float32) * 20,
     )
     mhlo_text = _convert_to_mhlo(
         fn, jax.tree_map(np.zeros_like, inputs), dialect=dialect)
+    mhlo_module = mhlo.MhloModule(module=mhlo_text, fun_name="test_module")
     chex.assert_trees_all_close(
-        mhlo.mhlo_apply(*inputs, mhlo_text=mhlo_text), fn(*inputs))
+        mhlo.mhlo_apply(*inputs, module=mhlo_module), fn(*inputs))
 
     def make_top_fn(sub_fn):
       def top_fn(x, y):
         res0, res1 = sub_fn(x + 8, y + 9)
         return res0 * 10, res1 * 3.14
       return top_fn
 
     expect_top_fn = make_top_fn(fn)
     actual_top_fn = make_top_fn(
-        functools.partial(mhlo.mhlo_apply, mhlo_text=mhlo_text))
+        functools.partial(mhlo.mhlo_apply, module=mhlo_module))
     self._assert_all_close(expect_top_fn, actual_top_fn, inputs)
     _check_transforms(actual_top_fn, inputs, dialect=dialect)
 
+  @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.named_parameters(
+      ("mhlo", "mhlo"),
+      ("stablehlo", "stablehlo"),
+  )
+  def test_boolean(self, dialect):
+    @jax.jit
+    def fn(x):
+      return x > 0
+
+    inputs = (
+        np.ones((4,), dtype=np.int32) * 10,
+    )
+    mhlo_text = _convert_to_mhlo(
+        fn, jax.tree_map(np.zeros_like, inputs), dialect=dialect)
+    mhlo_module = mhlo.MhloModule(module=mhlo_text, fun_name="test_module")
+    chex.assert_trees_all_close(
+        mhlo.mhlo_apply(*inputs, module=mhlo_module), fn(*inputs))
+
+    def make_top_fn(sub_fn):
+      def top_fn(x):
+        return sub_fn(x) * x
+      return top_fn
+
+    expect_top_fn = make_top_fn(fn)
+    actual_top_fn = make_top_fn(
+        functools.partial(mhlo.mhlo_apply, module=mhlo_module))
+    self._assert_all_close(expect_top_fn, actual_top_fn, inputs)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `tf2jax-0.3.4/tf2jax/experimental/util.py` & `tf2jax-0.3.5/tf2jax/tf2jax_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-# Copyright 2023 DeepMind Technologies Limited. All Rights Reserved.
+# Copyright 2021 DeepMind Technologies Limited. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Utils.
+"""Tests for tf2jax."""
 
-A subset of functions provided in
-https://github.com/google/jax/blob/main/jax/_src/util.py
-"""
+from absl.testing import absltest
+import tf2jax
 
-import itertools as it
-from typing import Iterable, List, Sequence, TypeVar
 
+class Tf2jaxTest(absltest.TestCase):
+  """Test tf2jax can be imported correctly."""
 
-T = TypeVar("T")
+  def test_import(self):
+    self.assertTrue(hasattr(tf2jax, 'convert'))
 
 
-def concatenate(xs: Iterable[Sequence[T]]) -> List[T]:
-  """Concatenates/flattens a list of lists."""
-  return list(it.chain.from_iterable(xs))
-
-flatten = concatenate
-
-_UNFLATTEN_DONE = object()
-
-
-def unflatten(xs: Iterable[T], ns: Sequence[int]) -> List[List[T]]:
-  """Splits `xs` into subsequences of lengths `ns`."""
-  xs_iter = iter(xs)
-  unflattened = [[next(xs_iter) for _ in range(n)] for n in ns]
-  assert next(xs_iter, _UNFLATTEN_DONE) is _UNFLATTEN_DONE
-  return unflattened
+if __name__ == '__main__':
+  absltest.main()
```

### Comparing `tf2jax-0.3.4/tf2jax.egg-info/PKG-INFO` & `tf2jax-0.3.5/tf2jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: tf2jax
-Version: 0.3.4
+Version: 0.3.5
 Summary: TF2JAX: Convert TensorFlow to JAX
 Home-page: https://github.com/deepmind/tf2jax
 Author: DeepMind
 Author-email: tf2jax-dev@google.com
 License: Apache 2.0
 Keywords: jax tensorflow conversion translate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
```

### Comparing `tf2jax-0.3.4/tf2jax.egg-info/SOURCES.txt` & `tf2jax-0.3.5/tf2jax.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 tf2jax/_src/config.py
 tf2jax/_src/linalg_ops_test.py
 tf2jax/_src/numpy_compat.py
 tf2jax/_src/numpy_compat_test.py
 tf2jax/_src/ops.py
 tf2jax/_src/ops_test.py
 tf2jax/_src/roundtrip_test.py
+tf2jax/_src/sharding_test.py
 tf2jax/_src/test_util.py
 tf2jax/_src/tf2jax.py
 tf2jax/_src/tf2jax_test.py
 tf2jax/_src/utils.py
 tf2jax/_src/xla_utils.py
 tf2jax/experimental/__init__.py
 tf2jax/experimental/mhlo.py
 tf2jax/experimental/mhlo_test.py
-tf2jax/experimental/ops.py
-tf2jax/experimental/util.py
+tf2jax/experimental/ops.py
```

