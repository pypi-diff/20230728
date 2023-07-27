# Comparing `tmp/versioned-hdf5-1.3.8.tar.gz` & `tmp/versioned-hdf5-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rever/dist/versioned-hdf5-1.3.8.tar", last modified: Tue Mar 29 21:53:15 2022, max compression
+gzip compressed data, was "rever/dist/versioned-hdf5-1.3.9.tar", last modified: Thu Apr 28 22:14:08 2022, max compression
```

## Comparing `versioned-hdf5-1.3.8.tar` & `versioned-hdf5-1.3.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-03-29 21:53:15.710920 versioned-hdf5-1.3.8/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3149 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/LICENSE
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       93 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/MANIFEST.in
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1152 2022-03-29 21:53:15.711065 versioned-hdf5-1.3.8/PKG-INFO
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      735 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/README.md
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    68629 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/_versioneer.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      181 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/pytest.ini
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      206 2022-03-29 21:53:15.711589 versioned-hdf5-1.3.8/setup.cfg
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      797 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/setup.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-03-29 21:53:15.711893 versioned-hdf5-1.3.8/versioned_hdf5/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      286 2022-03-17 20:32:16.000000 versioned-hdf5-1.3.8/versioned_hdf5/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      498 2022-03-29 21:53:15.711998 versioned-hdf5-1.3.8/versioned_hdf5/_version.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     8762 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.8/versioned_hdf5/api.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    10980 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/backend.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     7267 2022-03-17 20:32:16.000000 versioned-hdf5-1.3.8/versioned_hdf5/hashtable.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    19363 2022-03-17 20:32:16.000000 versioned-hdf5-1.3.8/versioned_hdf5/replay.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1130 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/slicetools.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-03-29 21:53:15.710427 versioned-hdf5-1.3.8/versioned_hdf5/tests/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)        0 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/__init__.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1681 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/conftest.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      372 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/helpers.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    72964 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/test_api.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    24846 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/test_backend.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     2275 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/test_hashtable.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    13841 2022-03-17 20:32:16.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/test_replay.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1626 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/test_slicetools.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    10833 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/test_versions.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     3347 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/tests/test_wrappers.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     9969 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/versions.py
--rw-r--r--   0 aaronmeurer   (501) staff       (20)    45123 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.8/versioned_hdf5/wrappers.py
-drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-03-29 21:53:15.703089 versioned-hdf5-1.3.8/versioned_hdf5.egg-info/
--rw-r--r--   0 aaronmeurer   (501) staff       (20)     1152 2022-03-29 21:53:15.000000 versioned-hdf5-1.3.8/versioned_hdf5.egg-info/PKG-INFO
--rw-r--r--   0 aaronmeurer   (501) staff       (20)      860 2022-03-29 21:53:15.000000 versioned-hdf5-1.3.8/versioned_hdf5.egg-info/SOURCES.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)        1 2022-03-29 21:53:15.000000 versioned-hdf5-1.3.8/versioned_hdf5.egg-info/dependency_links.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       26 2022-03-29 21:53:15.000000 versioned-hdf5-1.3.8/versioned_hdf5.egg-info/requires.txt
--rw-r--r--   0 aaronmeurer   (501) staff       (20)       15 2022-03-29 21:53:15.000000 versioned-hdf5-1.3.8/versioned_hdf5.egg-info/top_level.txt
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-04-28 22:14:08.517642 versioned-hdf5-1.3.9/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3149 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/LICENSE
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       93 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/MANIFEST.in
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1152 2022-04-28 22:14:08.517876 versioned-hdf5-1.3.9/PKG-INFO
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      735 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/README.md
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    68629 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/_versioneer.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      181 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/pytest.ini
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      206 2022-04-28 22:14:08.518637 versioned-hdf5-1.3.9/setup.cfg
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      797 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/setup.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-04-28 22:14:08.518986 versioned-hdf5-1.3.9/versioned_hdf5/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      286 2022-03-17 20:32:16.000000 versioned-hdf5-1.3.9/versioned_hdf5/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      498 2022-04-28 22:14:08.519099 versioned-hdf5-1.3.9/versioned_hdf5/_version.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     8762 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.9/versioned_hdf5/api.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    10980 2022-04-27 23:07:05.000000 versioned-hdf5-1.3.9/versioned_hdf5/backend.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     7267 2022-03-17 20:32:16.000000 versioned-hdf5-1.3.9/versioned_hdf5/hashtable.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    20905 2022-04-28 22:05:22.000000 versioned-hdf5-1.3.9/versioned_hdf5/replay.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1130 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/versioned_hdf5/slicetools.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-04-28 22:14:08.516895 versioned-hdf5-1.3.9/versioned_hdf5/tests/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)        0 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/__init__.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1681 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/conftest.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      372 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/helpers.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    72964 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/test_api.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    24846 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/test_backend.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     2275 2022-03-29 21:45:21.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/test_hashtable.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    30799 2022-04-28 22:05:22.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/test_replay.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1626 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/test_slicetools.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    10833 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/test_versions.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     3347 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/versioned_hdf5/tests/test_wrappers.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     9969 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/versioned_hdf5/versions.py
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)    45123 2022-01-17 16:59:07.000000 versioned-hdf5-1.3.9/versioned_hdf5/wrappers.py
+drwxr-xr-x   0 aaronmeurer   (501) staff       (20)        0 2022-04-28 22:14:08.508917 versioned-hdf5-1.3.9/versioned_hdf5.egg-info/
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)     1152 2022-04-28 22:14:08.000000 versioned-hdf5-1.3.9/versioned_hdf5.egg-info/PKG-INFO
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)      860 2022-04-28 22:14:08.000000 versioned-hdf5-1.3.9/versioned_hdf5.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)        1 2022-04-28 22:14:08.000000 versioned-hdf5-1.3.9/versioned_hdf5.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       26 2022-04-28 22:14:08.000000 versioned-hdf5-1.3.9/versioned_hdf5.egg-info/requires.txt
+-rw-r--r--   0 aaronmeurer   (501) staff       (20)       15 2022-04-28 22:14:08.000000 versioned-hdf5-1.3.9/versioned_hdf5.egg-info/top_level.txt
```

### Comparing `versioned-hdf5-1.3.8/LICENSE` & `versioned-hdf5-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/PKG-INFO` & `versioned-hdf5-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versioned-hdf5
-Version: 1.3.8
+Version: 1.3.9
 Summary: Versioned HDF5
 Home-page: https://github.com/deshaw/versioned-hdf5
 Author: Quansight
 License: BSD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: versioned-hdf5 Version: 1.3.8 Summary: Versioned
+Metadata-Version: 2.1 Name: versioned-hdf5 Version: 1.3.9 Summary: Versioned
 HDF5 Home-page: https://github.com/deshaw/versioned-hdf5 Author: Quansight
 License: BSD Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # versioned-hdf5 [![Build Status](https://
 travis-ci.org/deshaw/versioned-hdf5.svg?branch=master)](https://travis-ci.org/
 deshaw/versioned-hdf5) Versioned HDF5 provides a versioned abstraction on top
```

### Comparing `versioned-hdf5-1.3.8/README.md` & `versioned-hdf5-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/_versioneer.py` & `versioned-hdf5-1.3.9/_versioneer.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/setup.py` & `versioned-hdf5-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/api.py` & `versioned-hdf5-1.3.9/versioned_hdf5/api.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/backend.py` & `versioned-hdf5-1.3.9/versioned_hdf5/backend.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/hashtable.py` & `versioned-hdf5-1.3.9/versioned_hdf5/hashtable.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/replay.py` & `versioned-hdf5-1.3.9/versioned_hdf5/replay.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from h5py import VirtualLayout, VirtualSource, Dataset
+from h5py import VirtualLayout, VirtualSource, Dataset, Group, __version__ as h5py_version
 from h5py._hl.vds import VDSmap
 from h5py._hl.selections import select
 from h5py.h5i import get_name
 
 from ndindex import Slice, ChunkSize, Tuple
 
 import numpy as np
@@ -135,43 +135,61 @@
     for version_name in all_versions(f):
         if (version_name in versions_to_delete
             or name not in f['_version_data/versions'][version_name]):
             continue
 
         dataset = f['_version_data/versions'][version_name][name]
 
-        virtual_sources = dataset.virtual_sources()
-        slice_map = {spaceid_to_slice(i.vspace):
-                     spaceid_to_slice(i.src_space) for i in
-                     virtual_sources}
+        if dataset.is_virtual:
+            virtual_sources = dataset.virtual_sources()
+            slice_map = {spaceid_to_slice(i.vspace):
+                         spaceid_to_slice(i.src_space) for i in
+                         virtual_sources}
+        else:
+            slice_map = {}
         chunks_map[version_name].update(slice_map)
 
     chunks_to_keep = set().union(*[map.values() for map in
                                  chunks_map.values()])
 
     chunks_to_keep = sorted(chunks_to_keep, key=lambda i: i.args[0].args[0])
 
     if not chunks_to_keep:
         return {}
 
     raw_data = f['_version_data'][name]['raw_data']
     chunks = ChunkSize(raw_data.chunks)
     new_shape = (len(chunks_to_keep)*chunks[0], *chunks[1:])
 
+    # See InMemoryDataset.fillvalue. In h5py3 variable length strings use None
+    # for the h5py fillvalue, but require a string fillvalue for NumPy.
+    def _get_np_fillvalue(data):
+        if data.fillvalue is not None:
+            return data.fillvalue
+        if data.dtype.metadata:
+             if 'vlen' in raw_data.dtype.metadata:
+                 if (h5py_version.startswith('3') and
+                     data.dtype.metadata['vlen'] == str):
+                     return bytes()
+                 return data.dtype.metadata['vlen']()
+             elif 'h5py_encoding' in raw_data.dtype.metadata:
+                 return data.dtype.type()
+        return np.zeros((), dtype=data.dtype)[()]
+
     new_raw_data = f['_version_data'][name].create_dataset(
         '_tmp_raw_data', shape=new_shape, maxshape=(None,)+chunks[1:],
         chunks=raw_data.chunks, dtype=raw_data.dtype,
         compression=raw_data.compression,
         compression_opts=raw_data.compression_opts,
         fillvalue=raw_data.fillvalue)
     for key, val in raw_data.attrs.items():
         new_raw_data.attrs[key] = val
 
     r = raw_data[:]
-    n = np.full(new_raw_data.shape, new_raw_data.fillvalue, dtype=new_raw_data.dtype)
+    n = np.full(new_raw_data.shape, _get_np_fillvalue(raw_data), dtype=new_raw_data.dtype)
     raw_data_chunks_map = {}
     for new_chunk, chunk in zip(chunks.indices(new_shape), chunks_to_keep):
         # Shrink new_chunk to the size of chunk, in case chunk isn't a full
         # chunk in one of the dimensions.
         # TODO: Implement something in ndindex to do this.
         new_chunk = Tuple(
             *[Slice(new_chunk.args[i].start,
@@ -215,16 +233,16 @@
 
     if not tmp:
         del f['_version_data'][name]['hash_table']
         f['_version_data'][name].move('_tmp_hash_table', 'hash_table')
 
 def _recreate_virtual_dataset(f, name, versions, raw_data_chunks_map, tmp=False):
     """
-    Recreate every virtual dataset `name` in the version versions according to
-    the new raw_data chunks.
+    Recreate every virtual dataset `name` in the versions `versions` according
+    to the new raw_data chunks in `raw_data_chunks_map`.
 
     Returns a dict mapping the chunks from the old raw dataset to the chunks
     in the new raw dataset. Chunks not in the mapping were deleted. If the
     dict is empty, then no remaining version contains the given dataset.
 
     If tmp is True, the new virtual datasets are named `'_tmp_' + name` and
     are placed alongside the existing ones. Otherwise the existing virtual
@@ -243,46 +261,50 @@
 
         layout = VirtualLayout(dataset.shape, dtype=dataset.dtype)
         layout_has_sources = hasattr(layout, 'sources')
 
         if not layout_has_sources:
             vs = VirtualSource('.', name=raw_data.name, shape=raw_data.shape, dtype=raw_data.dtype)
 
-        virtual_sources = dataset.virtual_sources()
-        for vmap in virtual_sources:
-            vspace, fname, dset_name, src_space = vmap
-            fname = fname.encode('utf-8')
-            assert fname == b'.', fname
-
-            vslice = spaceid_to_slice(vspace)
-            src_slice = spaceid_to_slice(src_space)
-            if src_slice not in raw_data_chunks_map:
-                raise ValueError(f"Could not find the chunk for {vslice} ({src_slice} in the old raw dataset) for {name!r} in {version_name!r}")
-            new_src_slice = raw_data_chunks_map[src_slice]
-
-            # h5py 3.3 changed the VirtualLayout code. See
-            # https://github.com/h5py/h5py/pull/1905 and the code in
-            # create_virtual_dataset().
-            if layout_has_sources:
-                vs_sel = select(raw_data.shape, new_src_slice.raw, None)
-                layout_sel = select(dataset.shape, vslice.raw, None)
-                new_vmap = VDSmap(layout_sel.id, fname, dset_name, vs_sel.id)
-                layout.sources.append(new_vmap)
-            else:
-                layout[vslice.raw] = vs[new_src_slice.raw]
-
-        tmp_name = '_tmp_' + name
-        tmp_dataset = group.create_virtual_dataset(tmp_name, layout, fillvalue=dataset.fillvalue)
+        # If a dataset has no data except for the fillvalue, it will not be virtual
+        if dataset.is_virtual:
+            virtual_sources = dataset.virtual_sources()
+            for vmap in virtual_sources:
+                vspace, fname, dset_name, src_space = vmap
+                fname = fname.encode('utf-8')
+                assert fname == b'.', fname
+
+                vslice = spaceid_to_slice(vspace)
+                src_slice = spaceid_to_slice(src_space)
+                if src_slice not in raw_data_chunks_map:
+                    raise ValueError(f"Could not find the chunk for {vslice} ({src_slice} in the old raw dataset) for {name!r} in {version_name!r}")
+                new_src_slice = raw_data_chunks_map[src_slice]
+
+                # h5py 3.3 changed the VirtualLayout code. See
+                # https://github.com/h5py/h5py/pull/1905 and the code in
+                # create_virtual_dataset().
+                if layout_has_sources:
+                    vs_sel = select(raw_data.shape, new_src_slice.raw, None)
+                    layout_sel = select(dataset.shape, vslice.raw, None)
+                    new_vmap = VDSmap(layout_sel.id, fname, dset_name, vs_sel.id)
+                    layout.sources.append(new_vmap)
+                else:
+                    layout[vslice.raw] = vs[new_src_slice.raw]
+
+        head, tail = pp.split(name)
+        tmp_name = '_tmp_' + tail
+        tmp_path = pp.join(head, tmp_name)
+        tmp_dataset = group.create_virtual_dataset(tmp_path, layout, fillvalue=dataset.fillvalue)
 
         for key, val in dataset.attrs.items():
             tmp_dataset.attrs[key] = val
 
         if not tmp:
             del group[name]
-            group.move(tmp_name, name)
+            group.move(tmp_path, name)
 
 def delete_versions(f, versions_to_delete):
     """
     Completely delete the versions from `versions_to_delete` from the versioned file `f`.
 
     This function should be used instead of deleting the version group
     directly, as this will not delete the underlying data that is unique to
@@ -302,30 +324,42 @@
             raise ValueError(f"Version {version!r} does not exist")
 
     versions_to_keep = set(versions) - set(versions_to_delete)
 
     def delete_dataset(name):
         if name == 'versions':
             return
+
         # Recreate the raw data.
         raw_data_chunks_map = _recreate_raw_data(f, name, versions_to_delete)
 
         if not raw_data_chunks_map:
             del version_data[name]
             return
 
         # Recreate the hash table.
         _recreate_hashtable(f, name, raw_data_chunks_map)
 
         # Recreate every virtual dataset in every kept version.
         _recreate_virtual_dataset(f, name, versions_to_keep, raw_data_chunks_map)
 
-    for name in version_data:
-        if name == 'versions':
-            continue
+    # We use this instead of version_data.visit(delete_dataset) because
+    # visit() has trouble with the groups being deleted from under it.
+    def _walk(g, prefix=''):
+        for name in g:
+            obj = g[name]
+            if isinstance(obj, Group):
+                if 'raw_data' in obj:
+                    to_delete.append(prefix + name)
+                else:
+                    _walk(obj, prefix + name + '/')
+
+    to_delete = []
+    _walk(version_data)
+    for name in to_delete:
         delete_dataset(name)
 
     for version in versions_to_delete:
         del versions[version]
 
 # Backwards compatibility
 delete_version = delete_versions
```

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/slicetools.py` & `versioned-hdf5-1.3.9/versioned_hdf5/slicetools.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/tests/conftest.py` & `versioned-hdf5-1.3.9/versioned_hdf5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/tests/test_api.py` & `versioned-hdf5-1.3.9/versioned_hdf5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/tests/test_backend.py` & `versioned-hdf5-1.3.9/versioned_hdf5/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/tests/test_hashtable.py` & `versioned-hdf5-1.3.9/versioned_hdf5/tests/test_hashtable.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/tests/test_slicetools.py` & `versioned-hdf5-1.3.9/versioned_hdf5/tests/test_slicetools.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/tests/test_versions.py` & `versioned-hdf5-1.3.9/versioned_hdf5/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/tests/test_wrappers.py` & `versioned-hdf5-1.3.9/versioned_hdf5/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/versions.py` & `versioned-hdf5-1.3.9/versioned_hdf5/versions.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5/wrappers.py` & `versioned-hdf5-1.3.9/versioned_hdf5/wrappers.py`

 * *Files identical despite different names*

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5.egg-info/PKG-INFO` & `versioned-hdf5-1.3.9/versioned_hdf5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versioned-hdf5
-Version: 1.3.8
+Version: 1.3.9
 Summary: Versioned HDF5
 Home-page: https://github.com/deshaw/versioned-hdf5
 Author: Quansight
 License: BSD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: versioned-hdf5 Version: 1.3.8 Summary: Versioned
+Metadata-Version: 2.1 Name: versioned-hdf5 Version: 1.3.9 Summary: Versioned
 HDF5 Home-page: https://github.com/deshaw/versioned-hdf5 Author: Quansight
 License: BSD Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # versioned-hdf5 [![Build Status](https://
 travis-ci.org/deshaw/versioned-hdf5.svg?branch=master)](https://travis-ci.org/
 deshaw/versioned-hdf5) Versioned HDF5 provides a versioned abstraction on top
```

### Comparing `versioned-hdf5-1.3.8/versioned_hdf5.egg-info/SOURCES.txt` & `versioned-hdf5-1.3.9/versioned_hdf5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

