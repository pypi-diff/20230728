# Comparing `tmp/pyaogmaneo-2.0.9.tar.gz` & `tmp/pyaogmaneo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.0.9.tar", last modified: Sat Jul  1 20:12:05 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.1.0.tar", last modified: Fri Jul 28 16:36:41 2023, max compression
```

## Comparing `pyaogmaneo-2.0.9.tar` & `pyaogmaneo-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.9/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-01 20:10:42.000000 pyaogmaneo-2.0.9/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.9/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.9/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.9/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-01 20:12:05.000000 pyaogmaneo-2.0.9/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.9/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-01 20:06:13.000000 pyaogmaneo-2.0.9/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-01 20:12:05.174318 pyaogmaneo-2.0.9/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8213 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-30 23:05:50.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     9041 2023-06-30 23:06:07.000000 pyaogmaneo-2.0.9/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.1.0/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-28 16:35:00.000000 pyaogmaneo-2.1.0/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.0/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.0/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.0/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-28 16:36:41.000000 pyaogmaneo-2.1.0/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.1.0/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-28 16:34:37.000000 pyaogmaneo-2.1.0/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-28 16:36:41.515473 pyaogmaneo-2.1.0/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15775 2023-07-28 16:35:40.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     7014 2023-07-28 16:35:13.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8140 2023-07-28 00:25:43.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-07-26 01:03:23.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     9067 2023-07-28 00:25:43.000000 pyaogmaneo-2.1.0/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.0.9/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.1.0/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.9/CMakeLists.txt` & `pyaogmaneo-2.1.0/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 762fe2dc916bb9f5a491529af3ba31640fdcd65d
+        GIT_TAG a9aacebf334da53f9234858b4fa9557262727b10
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.0.9/LICENSE.md` & `pyaogmaneo-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.9/README.md` & `pyaogmaneo-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.9/setup.py` & `pyaogmaneo-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.0.9",
+    version="2.1.0",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.9/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.1.0/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -245,62 +245,78 @@
 
     for (int j = 0; j < predictions.size(); j++)
         predictions[j] = h.get_prediction_cis(i)[j];
 
     return predictions;
 }
 
-std::vector<float> Hierarchy::get_prediction_acts(
+std::vector<int> Hierarchy::get_layer_prediction_cis(
+    int l
+) const {
+    if (l < 1 || l >= h.get_num_layers())
+        throw std::runtime_error("layer index " + std::to_string(l) + " out of range [1, " + std::to_string(h.get_num_layers() - 1) + "]!");
+
+    const aon::Int_Buffer &cis = h.get_decoder(l, h.get_ticks_per_update(l) - 1 - h.get_ticks(l)).get_hidden_cis();
+
+    std::vector<int> predictions(cis.size());
+
+    for (int j = 0; j < predictions.size(); j++)
+        predictions[j] = cis[j];
+
+    return predictions;
+}
+
+std::vector<float> Hierarchy::get_prediction_probs(
     int i
 ) const {
     if (i < 0 || i >= h.get_num_io())
         throw std::runtime_error("prediction index " + std::to_string(i) + " out of range [0, " + std::to_string(h.get_num_io() - 1) + "]!");
 
-    if (!h.io_layer_exists(i) || h.get_io_type(i) == aon::none)
+    if (!h.io_layer_exists(i) || h.get_io_type(i) != aon::prediction)
         throw std::runtime_error("no decoder exists at index " + std::to_string(i) + " - did you set it to the correct type?");
 
-    std::vector<float> predictions(h.get_prediction_acts(i).size());
+    std::vector<float> predictions(h.get_prediction_probs(i).size());
 
     for (int j = 0; j < predictions.size(); j++)
-        predictions[j] = h.get_prediction_acts(i)[j];
+        predictions[j] = h.get_prediction_probs(i)[j];
 
     return predictions;
 }
 
 std::vector<int> Hierarchy::sample_prediction(
     int i,
     float temperature
 ) const {
     if (temperature == 0.0f)
         return get_prediction_cis(i);
 
     if (i < 0 || i >= h.get_num_io())
         throw std::runtime_error("prediction index " + std::to_string(i) + " out of range [0, " + std::to_string(h.get_num_io() - 1) + "]!");
 
-    if (!h.io_layer_exists(i) || h.get_io_type(i) == aon::none)
+    if (!h.io_layer_exists(i) || h.get_io_type(i) != aon::prediction)
         throw std::runtime_error("no decoder exists at index " + std::to_string(i) + " - did you set it to the correct type?");
 
     std::vector<int> sample(h.get_prediction_cis(i).size());
 
     int size_z = h.get_io_size(i).z;
 
     float temperature_inv = 1.0f / temperature;
 
     for (int j = 0; j < sample.size(); j++) {
         float total = 0.0f;
 
         for (int k = 0; k < size_z; k++)
-            total += aon::powf(h.get_prediction_acts(i)[k + j * size_z], temperature_inv);
+            total += aon::powf(h.get_prediction_probs(i)[k + j * size_z], temperature_inv);
 
         float cusp = aon::randf(0.0f, total);
 
         float sum_so_far = 0.0f;
 
         for (int k = 0; k < size_z; k++) {
-            sum_so_far += aon::powf(h.get_prediction_acts(i)[k + j * size_z], temperature_inv);
+            sum_so_far += aon::powf(h.get_prediction_probs(i)[k + j * size_z], temperature_inv);
 
             if (sum_so_far >= cusp) {
                 sample[j] = k;
 
                 break;
             }
         }
@@ -365,15 +381,15 @@
             aon::Int2 offset(ix - field_lower_bound.x, iy - field_lower_bound.y);
 
             int wi_start = vld.size.z * (offset.y + diam * (offset.x + diam * hidden_cell_index));
 
             int field_start = vld.size.z * (offset.y + diam * offset.x);
 
             for (int vc = 0; vc < vld.size.z; vc++) {
-                float w = vl.weights[vc + wi_start];
+                float w = vl.weights[vc + wi_start] / 255.0f;
 
                 field[vc + field_start] = w;
             }
         }
 
     return std::make_tuple(field, std::make_tuple(size.x, size.y, size.z));
 }
@@ -419,15 +435,15 @@
             aon::Int2 offset(ix - field_lower_bound.x, iy - field_lower_bound.y);
 
             int wi_start = vld.size.z * (offset.y + diam * (offset.x + diam * hidden_cell_index));
 
             int field_start = vld.size.z * (offset.y + diam * offset.x);
 
             for (int vc = 0; vc < vld.size.z; vc++) {
-                float w = vl.weights[vc + wi_start];
+                float w = vl.weights[vc + wi_start] / 255.0f;
 
                 field[vc + field_start] = w;
             }
         }
 
     return std::make_tuple(field, std::make_tuple(size.x, size.y, size.z));
 }
```

### Comparing `pyaogmaneo-2.0.9/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.1.0/source/pyaogmaneo/py_hierarchy.h`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #pragma once
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace pyaon {
-const int hierarchy_magic = 1138225;
+const int hierarchy_magic = 3133285;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
 
@@ -135,15 +135,19 @@
         return h.get_num_layers();
     }
 
     std::vector<int> get_prediction_cis(
         int i
     ) const;
 
-    std::vector<float> get_prediction_acts(
+    std::vector<int> get_layer_prediction_cis(
+        int l
+    ) const;
+
+    std::vector<float> get_prediction_probs(
         int i
     ) const;
 
     std::vector<int> sample_prediction(
         int i,
         float temperature
     ) const;
```

### Comparing `pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -210,16 +210,15 @@
             aon::Int2 offset(ix - field_lower_bound.x, iy - field_lower_bound.y);
 
             int wi_start = vld.size.z * (offset.y + diam * (offset.x + diam * hidden_cell_index));
 
             int field_start = vld.size.z * (offset.y + diam * offset.x);
 
             for (int vc = 0; vc < vld.size.z; vc++) {
-                float w0 = vl.weights0[vc + wi_start];
-                float w1 = vl.weights1[vc + wi_start];
+                float w = vl.protos[vc + wi_start];
 
-                field[vc + vld.size.z * (offset.y + diam * offset.x)] = (w0 + w1) * 0.5f;
+                field[vc + vld.size.z * (offset.y + diam * offset.x)] = w;
             }
         }
 
     return std::make_tuple(field, std::make_tuple(size.x, size.y, size.z));
 }
```

### Comparing `pyaogmaneo-2.0.9/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.1.0/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.9/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.1.0/source/pyaogmaneo/py_module.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,20 @@
         .def_readwrite("down_radius", &pyaon::Layer_Desc::down_radius)
         .def_readwrite("ticks_per_update", &pyaon::Layer_Desc::ticks_per_update)
         .def_readwrite("temporal_horizon", &pyaon::Layer_Desc::temporal_horizon);
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
-        .def_readwrite("code_iters", &aon::Encoder::Params::code_iters)
-        .def_readwrite("lr", &aon::Encoder::Params::lr)
-        .def_readwrite("gcurve", &aon::Encoder::Params::gcurve);
+        .def_readwrite("lr", &aon::Encoder::Params::lr);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
-        .def_readwrite("lr", &aon::Decoder::Params::lr)
-        .def_readwrite("gcurve", &aon::Decoder::Params::gcurve);
+        .def_readwrite("temperature", &aon::Decoder::Params::temperature)
+        .def_readwrite("lr", &aon::Decoder::Params::lr);
 
     py::class_<aon::Actor::Params>(m, "ActorParams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
         .def_readwrite("alr", &aon::Actor::Params::alr)
         .def_readwrite("bias", &aon::Actor::Params::bias)
         .def_readwrite("discount", &aon::Actor::Params::discount)
@@ -127,15 +125,16 @@
             py::arg("learn_enabled") = true,
             py::arg("reward") = 0.0f,
             py::arg("mimic") = 0.0f
         )
         .def("clear_state", &pyaon::Hierarchy::clear_state)
         .def("get_num_layers", &pyaon::Hierarchy::get_num_layers)
         .def("get_prediction_cis", &pyaon::Hierarchy::get_prediction_cis)
-        .def("get_prediction_acts", &pyaon::Hierarchy::get_prediction_acts)
+        .def("get_layer_prediction_cis", &pyaon::Hierarchy::get_layer_prediction_cis)
+        .def("get_prediction_probs", &pyaon::Hierarchy::get_prediction_probs)
         .def("sample_prediction", &pyaon::Hierarchy::sample_prediction)
         .def("get_hidden_cis", &pyaon::Hierarchy::get_hidden_cis)
         .def("get_hidden_size", &pyaon::Hierarchy::get_hidden_size)
         .def("get_num_encoder_visible_layers", &pyaon::Hierarchy::get_num_encoder_visible_layers)
         .def("get_ticks", &pyaon::Hierarchy::get_ticks)
         .def("get_ticks_per_update", &pyaon::Hierarchy::get_ticks_per_update)
         .def("get_num_io", &pyaon::Hierarchy::get_num_io)
@@ -157,17 +156,18 @@
         )
         .def_readwrite("size", &pyaon::Image_Visible_Layer_Desc::size)
         .def_readwrite("radius", &pyaon::Image_Visible_Layer_Desc::radius);
 
     // bind params
     py::class_<aon::Image_Encoder::Params>(m, "ImageEncoderParams")
         .def(py::init<>())
-        .def_readwrite("choice", &aon::Image_Encoder::Params::choice)
-        .def_readwrite("vigilance", &aon::Image_Encoder::Params::vigilance)
-        .def_readwrite("lr", &aon::Image_Encoder::Params::lr);
+        .def_readwrite("threshold", &aon::Image_Encoder::Params::threshold)
+        .def_readwrite("falloff", &aon::Image_Encoder::Params::falloff)
+        .def_readwrite("lr", &aon::Image_Encoder::Params::lr)
+        .def_readwrite("rr", &aon::Image_Encoder::Params::rr);
 
     py::class_<pyaon::Image_Encoder>(m, "ImageEncoder")
         .def(py::init<
                 const std::tuple<int, int, int>&,
                 const std::vector<pyaon::Image_Visible_Layer_Desc>&,
                 const std::string&,
                 const std::vector<unsigned char>&
```

