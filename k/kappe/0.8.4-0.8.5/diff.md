# Comparing `tmp/kappe-0.8.4.tar.gz` & `tmp/kappe-0.8.5.tar.gz`

## Comparing `kappe-0.8.4.tar` & `kappe-0.8.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 kappe-0.8.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 kappe-0.8.4/.python-version
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 kappe-0.8.4/CHANGELOG.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kappe-0.8.4/MANIFEST.in
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kappe-0.8.4/committed.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kappe-0.8.4/.github/workflows/pypi-publish.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/__main__.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/cli.py
--rw-r--r--   0        0        0    15660 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/convert.py
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/cut.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/plugin.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/__init__.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/pointcloud.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/qos.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/tf.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/timing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/plugins/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/plugins/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/__init__.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/msg_def.py
--rw-r--r--   0        0        0     8318 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/pointcloud2.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/settings.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/types.py
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 kappe-0.8.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 kappe-0.8.4/LICENSE
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 kappe-0.8.4/README.md
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 kappe-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 kappe-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 kappe-0.8.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 kappe-0.8.5/.python-version
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 kappe-0.8.5/CHANGELOG.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kappe-0.8.5/MANIFEST.in
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kappe-0.8.5/committed.toml
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 kappe-0.8.5/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/__main__.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/cli.py
+-rw-r--r--   0        0        0    15660 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/convert.py
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/cut.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/plugin.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/module/__init__.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/module/pointcloud.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/module/qos.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/module/tf.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/module/timing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/plugins/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/plugins/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/utils/__init__.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/utils/msg_def.py
+-rw-r--r--   0        0        0     8318 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/utils/pointcloud2.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/utils/settings.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 kappe-0.8.5/src/kappe/utils/types.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 kappe-0.8.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 kappe-0.8.5/LICENSE
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 kappe-0.8.5/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 kappe-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 kappe-0.8.5/PKG-INFO
```

### Comparing `kappe-0.8.4/.pre-commit-config.yaml` & `kappe-0.8.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/.github/workflows/pypi-publish.yaml` & `kappe-0.8.5/.github/workflows/workflow.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -20,25 +20,29 @@
 
   build:
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
     needs: lint
 
     runs-on: ubuntu-latest
 
+    environment: release
+    permissions:
+      # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write
+      contents: read
+
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: Install build
         run: python3 -m pip install --upgrade build
 
       - name: Building
         run: python3 -m build
 
-      - name: Publish package
+      - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `kappe-0.8.4/src/kappe/cli.py` & `kappe-0.8.5/src/kappe/cli.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/convert.py` & `kappe-0.8.5/src/kappe/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
 
         # store useful information
         self.writer._writer.add_metadata(  # noqa: SLF001
             name='convert_metadata',
             data={
                 'input_path': str(self.input_path),
                 'output_path': str(self.output_path),
-                'data': datetime.now(tz=timezone.utc).isoformat(),
+                'date': datetime.now(tz=timezone.utc).isoformat(),
                 'version': __version__,
             },
         )
 
         self.writer.finish()
 
         self.f_reader.close()
```

### Comparing `kappe-0.8.4/src/kappe/cut.py` & `kappe-0.8.5/src/kappe/cut.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,27 +142,25 @@
     for split in settings.splits:
         if not split.name.endswith('.mcap'):
             split.name += '.mcap'
 
     output.mkdir(parents=True, exist_ok=True)
 
     outputs: list[SplitWriter] = []
-    first_msg: list[bool] = []
 
     min_start_time = int(min([split.start for split in settings.splits]) * 1e9)
     max_end_time = int(max([split.end for split in settings.splits]) * 1e9)
 
     with input_file.open('rb') as f:
         reader = make_reader(f)
 
         profile = reader.get_header().profile
         for split in settings.splits:
             out = output / split.name
             outputs.append(SplitWriter(str(out), profile))
-            first_msg.append(True)  # noqa: FBT003
 
         if settings.keep_tf_tree:
             tf_static_schema, tf_static_channel, tf_static_msgs = collect_tf(reader)
             for w in outputs:
                 w.set_static_tf(tf_static_schema, tf_static_channel, tf_static_msgs)
 
         for schema, channel, message in tqdm(reader.iter_messages(
@@ -200,15 +198,14 @@
 
         tf_static_schema, tf_static_channel, tf_static_msgs = None, None, None
         if settings.keep_tf_tree:
             tf_static_schema, tf_static_channel, tf_static_msgs = collect_tf(reader)
             writer.set_static_tf(tf_static_schema, tf_static_channel, tf_static_msgs)
 
         # TODO: check if topic exists
-
         for schema, channel, message in tqdm(reader.iter_messages()):
             if schema is None:
                 continue
 
             if channel.topic == settings.split_on_topic.topic and \
                     message.publish_time - last_split_time > debounce_ns:
                 logger.info('Found split point at %.2fs', message.publish_time / 1e9)
```

### Comparing `kappe-0.8.4/src/kappe/plugin.py` & `kappe-0.8.5/src/kappe/plugin.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/settings.py` & `kappe-0.8.5/src/kappe/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/module/pointcloud.py` & `kappe-0.8.5/src/kappe/module/pointcloud.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/module/qos.py` & `kappe-0.8.5/src/kappe/module/qos.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/module/tf.py` & `kappe-0.8.5/src/kappe/module/tf.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/module/timing.py` & `kappe-0.8.5/src/kappe/module/timing.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/plugins/image.py` & `kappe-0.8.5/src/kappe/plugins/image.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/utils/msg_def.py` & `kappe-0.8.5/src/kappe/utils/msg_def.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/utils/pointcloud2.py` & `kappe-0.8.5/src/kappe/utils/pointcloud2.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/src/kappe/utils/settings.py` & `kappe-0.8.5/src/kappe/utils/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/.gitignore` & `kappe-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/LICENSE` & `kappe-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kappe-0.8.4/README.md` & `kappe-0.8.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -24,15 +24,19 @@
     - [Pointcloud](#pointcloud)
       - [Remove zero points from PointCloud2](#remove-zero-points-from-pointcloud2)
       - [Rotate a pointcloud](#rotate-a-pointcloud)
       - [Rename PointCloud2 field name](#rename-pointcloud2-field-name)
     - [TF](#tf)
     - [Remove Transform](#remove-transform)
       - [Insert Static Transform](#insert-static-transform)
+    - [Schema Mapping](#schema-mapping)
+    - [Trim](#trim)
     - [Plugins](#plugins)
+    - [ROS1 to ROS2 conversion](#ros1-to-ros2-conversion)
+    - [Reproducibility](#reproducibility)
   - [Cut](#cut)
     - [Split on time](#split-on-time)
     - [Split on topic](#split-on-topic)
 
 </details>
 
 ------
@@ -57,16 +61,15 @@
 topic:
   mapping:
     /points: /sensor/points
 ```
 
 Run the converter:
 
-`kappe convert --config config.yaml ./input.bag`
-
+`kappe convert --config config.yaml ./input.mcap`
 
 ## Convert
 
 `kappe convert [-h] [--config CONFIG] [--overwrite] input output`
 
 Converts a single file or a directory of files to the MCAP format.
 
@@ -176,27 +179,65 @@
       rotation:
         euler_deg:
           - 0
           - 90
           - 0
 ```
 
+### Schema Mapping
+
+If the new schema is not already in the mcap, kappe will try to load it either from your ROS2 environment or from `./msgs`.
+
+```yaml
+msg_schema:
+  mapping:
+    std_msgs/Int32: std_msgs/Int64
+```
+
+### Trim
+
+Trim the mcap file to a specific time range.
+
+```yaml
+time_start:  1676549454.0
+time_end:    1676549554.0
+```
+
 ### Plugins
 
 Kappe can be extended with plugins, for example to compress images. Source code for plugins can be found in the [plugins](./src/kappe/), additional plugins can be loaded from `./plugins`.
 
 ```yaml
 plugins:
   - name: image.CompressImage
     input_topic: /image
     output_topic: /compressed/image
     settings:
       quality: 50
 ```
 
+### ROS1 to ROS2 conversion
+
+Kappe automatic converts ROS1 messages to ROS2 messages.
+It will not reuse ROS1 definitions, all schemas will be loaded either from your ROS2 environment or from `./msgs`. If the ROS2 schema name has changed use the `msg_schema.mapping` to map the old schema to the new schema.
+
+The msg field will be mapped exactly, ROS1 time and duration will be converted to ROS2 time and duration (`secs -> sec` & `nsecs -> nanosec`).
+
+To download the common ROS2 schemas run:
+
+```sh
+git clone --depth=1 --branch=humble https://github.com/ros2/common_interfaces.git ./msgs/common_interfaces
+git clone --depth=1 --branch=humble https://github.com/ros2/geometry2.git ./msgs/geometry2
+```
+
+### Reproducibility
+
+Kappe saves the input/output path, the time and the version into a MCAP metadata field, called `convert_metadata`.
+The config will be saved as an attachment named `convert_config.yaml`.
+
 ## Cut
 
 `usage: kappe cut [-h] --config CONFIG [--overwrite] input [output_folder]`
 
 Cuts a directory of mcaps into smaller mcaps, based on timestamp or topic.
 
 When `keep_tf_tree` is set to `true` all splits will have the same `/tf_static` messages.
@@ -204,15 +245,15 @@
 ### Split on time
 
 ```yaml
 keep_tf_tree: true
 splits:
   - start:  1676549454.0
     end:    1676549554.0
-    name:   beginning
+    name:   beginning.mcap
   - start:  1676549554.0
     end:    1676549654.0
     name:   end.mcap
 ```
 
 `kappe cut --config config.yaml ./input.mcap ./output_folder`
```

### Comparing `kappe-0.8.4/pyproject.toml` & `kappe-0.8.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     "scipy",
     "tqdm",
     "pyyaml>=6.0.1",
 ]
 
 dynamic = ["version"]
 
+[project.urls]
+repository = "https://github.com/sensmore/kappe"
+
 [project.scripts]
 kappe = "kappe.cli:main"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `kappe-0.8.4/PKG-INFO` & `kappe-0.8.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: kappe
-Version: 0.8.4
+Version: 0.8.5
 Summary: Converts ROS MCAPs
+Project-URL: repository, https://github.com/sensmore/kappe
 Author: Marko Bausch
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -46,15 +47,19 @@
     - [Pointcloud](#pointcloud)
       - [Remove zero points from PointCloud2](#remove-zero-points-from-pointcloud2)
       - [Rotate a pointcloud](#rotate-a-pointcloud)
       - [Rename PointCloud2 field name](#rename-pointcloud2-field-name)
     - [TF](#tf)
     - [Remove Transform](#remove-transform)
       - [Insert Static Transform](#insert-static-transform)
+    - [Schema Mapping](#schema-mapping)
+    - [Trim](#trim)
     - [Plugins](#plugins)
+    - [ROS1 to ROS2 conversion](#ros1-to-ros2-conversion)
+    - [Reproducibility](#reproducibility)
   - [Cut](#cut)
     - [Split on time](#split-on-time)
     - [Split on topic](#split-on-topic)
 
 </details>
 
 ------
@@ -79,16 +84,15 @@
 topic:
   mapping:
     /points: /sensor/points
 ```
 
 Run the converter:
 
-`kappe convert --config config.yaml ./input.bag`
-
+`kappe convert --config config.yaml ./input.mcap`
 
 ## Convert
 
 `kappe convert [-h] [--config CONFIG] [--overwrite] input output`
 
 Converts a single file or a directory of files to the MCAP format.
 
@@ -198,27 +202,65 @@
       rotation:
         euler_deg:
           - 0
           - 90
           - 0
 ```
 
+### Schema Mapping
+
+If the new schema is not already in the mcap, kappe will try to load it either from your ROS2 environment or from `./msgs`.
+
+```yaml
+msg_schema:
+  mapping:
+    std_msgs/Int32: std_msgs/Int64
+```
+
+### Trim
+
+Trim the mcap file to a specific time range.
+
+```yaml
+time_start:  1676549454.0
+time_end:    1676549554.0
+```
+
 ### Plugins
 
 Kappe can be extended with plugins, for example to compress images. Source code for plugins can be found in the [plugins](./src/kappe/), additional plugins can be loaded from `./plugins`.
 
 ```yaml
 plugins:
   - name: image.CompressImage
     input_topic: /image
     output_topic: /compressed/image
     settings:
       quality: 50
 ```
 
+### ROS1 to ROS2 conversion
+
+Kappe automatic converts ROS1 messages to ROS2 messages.
+It will not reuse ROS1 definitions, all schemas will be loaded either from your ROS2 environment or from `./msgs`. If the ROS2 schema name has changed use the `msg_schema.mapping` to map the old schema to the new schema.
+
+The msg field will be mapped exactly, ROS1 time and duration will be converted to ROS2 time and duration (`secs -> sec` & `nsecs -> nanosec`).
+
+To download the common ROS2 schemas run:
+
+```sh
+git clone --depth=1 --branch=humble https://github.com/ros2/common_interfaces.git ./msgs/common_interfaces
+git clone --depth=1 --branch=humble https://github.com/ros2/geometry2.git ./msgs/geometry2
+```
+
+### Reproducibility
+
+Kappe saves the input/output path, the time and the version into a MCAP metadata field, called `convert_metadata`.
+The config will be saved as an attachment named `convert_config.yaml`.
+
 ## Cut
 
 `usage: kappe cut [-h] --config CONFIG [--overwrite] input [output_folder]`
 
 Cuts a directory of mcaps into smaller mcaps, based on timestamp or topic.
 
 When `keep_tf_tree` is set to `true` all splits will have the same `/tf_static` messages.
@@ -226,15 +268,15 @@
 ### Split on time
 
 ```yaml
 keep_tf_tree: true
 splits:
   - start:  1676549454.0
     end:    1676549554.0
-    name:   beginning
+    name:   beginning.mcap
   - start:  1676549554.0
     end:    1676549654.0
     name:   end.mcap
 ```
 
 `kappe cut --config config.yaml ./input.mcap ./output_folder`
```

