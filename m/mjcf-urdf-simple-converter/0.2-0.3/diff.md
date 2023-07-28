# Comparing `tmp/mjcf_urdf_simple_converter-0.2.tar.gz` & `tmp/mjcf_urdf_simple_converter-0.3.tar.gz`

## Comparing `mjcf_urdf_simple_converter-0.2.tar` & `mjcf_urdf_simple_converter-0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/.vscode/settings.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/mjcf_urdf_simple_converter/__init__.py
--rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/mjcf_urdf_simple_converter/mjcf_urdf_simple_converter.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/LICENSE
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/README.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/pyproject.toml
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.2/PKG-INFO
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/requirements.txt
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/mjcf_urdf_simple_converter/__init__.py
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/mjcf_urdf_simple_converter/mjcf_urdf_simple_converter.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/LICENSE
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/README.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mjcf_urdf_simple_converter-0.3/PKG-INFO
```

### Comparing `mjcf_urdf_simple_converter-0.2/.github/workflows/python-package.yml` & `mjcf_urdf_simple_converter-0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mjcf_urdf_simple_converter-0.2/mjcf_urdf_simple_converter/mjcf_urdf_simple_converter.py` & `mjcf_urdf_simple_converter-0.3/mjcf_urdf_simple_converter/mjcf_urdf_simple_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,15 @@
             # load joint info
             jntid = model.body_jntadr[id]
             assert model.jnt_type[jntid] == mujoco.mjtJoint.mjJNT_HINGE, "only hinge joints supported"
             jnt_name = mujoco.mj_id2name(model, mujoco.mjtObj.mjOBJ_JOINT, jntid)
             jnt_range = model.jnt_range[jntid]  # [min, max]
             jnt_axis_childbody = model.jnt_axis[jntid]  # [x, y, z]
             childbody2jnt_pos = model.jnt_pos[jntid]  # [x, y, z]
-            # joint axis expressed in parent body frame
-            parentbody2jnt_axis = parentbody2childbody_Rot @ jnt_axis_childbody
+            parentbody2jnt_axis = jnt_axis_childbody
         else:
             # create a fixed joint instead
             jnt_name = f"{parent_name}2{child_name}_fixed"
             jnt_range = None
             childbody2jnt_pos = np.zeros(3)
             parentbody2jnt_axis = None
```

### Comparing `mjcf_urdf_simple_converter-0.2/.gitignore` & `mjcf_urdf_simple_converter-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mjcf_urdf_simple_converter-0.2/LICENSE` & `mjcf_urdf_simple_converter-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mjcf_urdf_simple_converter-0.2/README.md` & `mjcf_urdf_simple_converter-0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # mjcf_urdf_simple_converter
 A minimal and simple script to convert **limited elements** of MJCF (MuJoCo modeling format) robot model files to URDF. Developed from a need to visualize MJCF robots in ROS environments like Rviz, it only converts a limited subset of the robot model elements to URDF.
 The model file is loaded in the Python `mujoco` package, and its model elements are parsed using the library and then output according to the URDF XML format.
 
 I do **not** intend to expand this into a full-fledged transclation script from MJCF to URDF.
 
+# installation
+```
+pip install mjcf-urdf-simple-converter
+```
+
 ## usage
 ```python
 from mjcf_urdf_simple_converter import convert
 convert("model.xml", "model.urdf")
 # or, if you are using it in your ROS package and would like for the mesh directories to be resolved correctly, set meshfile_prefix, for example:
 convert("model.xml", "model.urdf", asset_file_prefix="package://your_package_name/model/")
 ```
```

### Comparing `mjcf_urdf_simple_converter-0.2/pyproject.toml` & `mjcf_urdf_simple_converter-0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="mjcf_urdf_simple_converter"
-version="0.2"
+version="0.3"
 authors = [{name="Yasunori Toshimitsu", email="yasu313nori@gmail.com"}]
 description = "Minimal script to convert MuJoCo MJCF robot model files to URDF files usable in ROS"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `mjcf_urdf_simple_converter-0.2/PKG-INFO` & `mjcf_urdf_simple_converter-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mjcf_urdf_simple_converter
-Version: 0.2
+Version: 0.3
 Summary: Minimal script to convert MuJoCo MJCF robot model files to URDF files usable in ROS
 Project-URL: Hompage, https://github.com/Yasu31/mjcf_urdf_simple_converter
 Author-email: Yasunori Toshimitsu <yasu313nori@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,19 @@
 
 # mjcf_urdf_simple_converter
 A minimal and simple script to convert **limited elements** of MJCF (MuJoCo modeling format) robot model files to URDF. Developed from a need to visualize MJCF robots in ROS environments like Rviz, it only converts a limited subset of the robot model elements to URDF.
 The model file is loaded in the Python `mujoco` package, and its model elements are parsed using the library and then output according to the URDF XML format.
 
 I do **not** intend to expand this into a full-fledged transclation script from MJCF to URDF.
 
+# installation
+```
+pip install mjcf-urdf-simple-converter
+```
+
 ## usage
 ```python
 from mjcf_urdf_simple_converter import convert
 convert("model.xml", "model.urdf")
 # or, if you are using it in your ROS package and would like for the mesh directories to be resolved correctly, set meshfile_prefix, for example:
 convert("model.xml", "model.urdf", asset_file_prefix="package://your_package_name/model/")
 ```
```

