# Comparing `tmp/vessim-0.1.0.tar.gz` & `tmp/vessim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessim-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vessim-0.2.0.tar", max compression
```

## Comparing `vessim-0.1.0.tar` & `vessim-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,25 @@
--rw-r--r--   0        0        0     1296 2023-07-03 15:22:36.274826 vessim-0.1.0/.github/workflows/vessim-ci.yml
--rw-r--r--   0        0        0     1154 2023-06-29 06:30:43.698698 vessim-0.1.0/.gitignore
--rw-r--r--   0        0        0     1089 2023-06-09 14:00:54.375226 vessim-0.1.0/LICENSE
--rw-r--r--   0        0        0     2738 2023-07-08 10:42:54.147664 vessim-0.1.0/README.md
--rw-r--r--   0        0        0      626 2023-07-03 15:22:36.275084 vessim-0.1.0/examples/_data.py
--rw-r--r--   0        0        0     2767 2023-07-03 15:22:36.275318 vessim-0.1.0/examples/cosim_example.py
--rw-r--r--   0        0        0     3167 2023-07-03 15:22:36.275468 vessim-0.1.0/examples/cosim_sil_example.py
--rw-r--r--   0        0        0  1428270 2023-07-03 15:22:36.280887 vessim-0.1.0/examples/data/carbon_intensity.csv
--rw-r--r--   0        0        0  1128276 2023-07-03 15:22:36.284210 vessim-0.1.0/examples/data/weather_berlin_2021-06.csv
--rw-r--r--   0        0        0     5183 2023-07-03 15:22:32.793112 vessim-0.1.0/examples/sil/carbon-aware_control_unit/carbon_aware_control_unit.py
--rw-r--r--   0        0        0     1450 2023-07-03 15:22:32.793478 vessim-0.1.0/examples/sil/carbon-aware_control_unit/main.py
--rw-r--r--   0        0        0     2097 2023-06-16 14:34:31.939747 vessim-0.1.0/examples/sil/example_node/README.md
--rw-r--r--   0        0        0     2262 2023-06-16 14:53:48.528050 vessim-0.1.0/examples/sil/example_node/node_api_server.py
--rw-r--r--   0        0        0      173 2023-06-16 14:34:31.940065 vessim-0.1.0/examples/sil/example_node/rpi/config/config.txt
--rw-r--r--   0        0        0      159 2023-06-16 14:34:31.940212 vessim-0.1.0/examples/sil/example_node/rpi/config/rc.local
--rw-r--r--   0        0        0     1405 2023-06-16 14:34:31.940332 vessim-0.1.0/examples/sil/example_node/rpi/init.sh
--rw-r--r--   0        0        0     2149 2023-06-29 06:30:43.700176 vessim-0.1.0/examples/sil/example_node/rpi/lib/pi_controller.py
--rw-r--r--   0        0        0       47 2023-06-16 14:34:31.940579 vessim-0.1.0/examples/sil/example_node/rpi/requirements.txt
--rw-r--r--   0        0        0     1290 2023-06-29 06:30:43.700595 vessim-0.1.0/examples/sil/example_node/rpi/rpi_api_server.py
--rw-r--r--   0        0        0      638 2023-06-16 14:34:31.940829 vessim-0.1.0/examples/sil/example_node/virtual_node/linear_power_model.py
--rw-r--r--   0        0        0       23 2023-06-16 14:34:31.940934 vessim-0.1.0/examples/sil/example_node/virtual_node/requirements.txt
--rw-r--r--   0        0        0     3597 2023-06-29 06:30:43.700765 vessim-0.1.0/examples/sil/example_node/virtual_node/v_node_api_server.py
--rw-r--r--   0        0        0      902 2023-06-29 06:30:43.701019 vessim-0.1.0/examples/sil/tf_gcp_node/.gitignore
--rw-r--r--   0        0        0     2253 2023-06-16 14:34:31.941318 vessim-0.1.0/examples/sil/tf_gcp_node/README.md
--rw-r--r--   0        0        0     2920 2023-06-29 06:30:43.701374 vessim-0.1.0/examples/sil/tf_gcp_node/main.tf
--rw-r--r--   0        0        0      249 2023-06-16 14:34:31.941592 vessim-0.1.0/examples/sil/tf_gcp_node/outputs.tf
--rwxr-xr-x   0        0        0      262 2023-06-16 14:34:31.941737 vessim-0.1.0/examples/sil/tf_gcp_node/ssh_scripts/tfreceive
--rwxr-xr-x   0        0        0      248 2023-06-16 14:34:31.941842 vessim-0.1.0/examples/sil/tf_gcp_node/ssh_scripts/tfsend
--rwxr-xr-x   0        0        0      225 2023-06-16 14:34:31.941938 vessim-0.1.0/examples/sil/tf_gcp_node/ssh_scripts/tfssh
--rw-r--r--   0        0        0      667 2023-06-16 14:34:31.942037 vessim-0.1.0/examples/sil/tf_gcp_node/variables.tf
--rw-r--r--   0        0        0   175373 2023-06-29 06:30:43.703104 vessim-0.1.0/experimental/baseline_experiment.ipynb
--rw-r--r--   0        0        0    58362 2023-06-16 14:34:31.942294 vessim-0.1.0/experimental/custom.json
--rw-r--r--   0        0        0     1394 2023-06-29 06:30:43.707622 vessim-0.1.0/experimental/pp_scenario.py
--rw-r--r--   0        0        0     3259 2023-07-08 10:16:04.568903 vessim-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1442 2023-06-16 14:34:31.943217 vessim-0.1.0/tests/test_carbon_api.py
--rw-r--r--   0        0        0     1915 2023-06-16 14:34:31.943608 vessim-0.1.0/tests/test_storage.py
--rw-r--r--   0        0        0       83 2023-07-08 10:06:28.572911 vessim-0.1.0/vessim/__init__.py
--rw-r--r--   0        0        0      188 2023-06-16 14:34:31.943833 vessim-0.1.0/vessim/core/__init__.py
--rw-r--r--   0        0        0     1381 2023-07-03 10:58:34.957722 vessim-0.1.0/vessim/core/microgrid.py
--rw-r--r--   0        0        0     2691 2023-07-08 10:04:28.186893 vessim-0.1.0/vessim/core/simulator.py
--rw-r--r--   0        0        0     4159 2023-07-03 15:22:36.284479 vessim-0.1.0/vessim/core/storage.py
--rw-r--r--   0        0        0      487 2023-07-03 10:58:34.958296 vessim-0.1.0/vessim/cosim/__init__.py
--rw-r--r--   0        0        0     4609 2023-07-03 10:58:34.958809 vessim-0.1.0/vessim/cosim/_util.py
--rw-r--r--   0        0        0     1650 2023-07-03 10:58:34.959274 vessim-0.1.0/vessim/cosim/carbon_api.py
--rw-r--r--   0        0        0     1978 2023-07-03 10:35:01.124497 vessim-0.1.0/vessim/cosim/computing_system.py
--rw-r--r--   0        0        0     1432 2023-07-03 10:58:34.959447 vessim-0.1.0/vessim/cosim/generator.py
--rw-r--r--   0        0        0      975 2023-07-03 10:58:34.959738 vessim-0.1.0/vessim/cosim/microgrid.py
--rw-r--r--   0        0        0     2356 2023-07-03 10:58:34.960060 vessim-0.1.0/vessim/cosim/monitor.py
--rw-r--r--   0        0        0     6102 2023-07-03 15:22:36.284784 vessim-0.1.0/vessim/cosim/sil_interface.py
--rw-r--r--   0        0        0      131 2023-06-16 14:34:31.946456 vessim-0.1.0/vessim/sil/__init__.py
--rw-r--r--   0        0        0     6134 2023-07-03 09:39:51.812632 vessim-0.1.0/vessim/sil/api_server.py
--rw-r--r--   0        0        0     2193 2023-07-03 09:39:51.812770 vessim-0.1.0/vessim/sil/http_client.py
--rw-r--r--   0        0        0      930 2023-06-16 14:34:31.946911 vessim-0.1.0/vessim/sil/node.py
--rw-r--r--   0        0        0     2333 2023-07-03 10:35:01.125242 vessim-0.1.0/vessim/sil/power_meter.py
--rw-r--r--   0        0        0     1009 2023-07-03 09:32:31.700809 vessim-0.1.0/vessim/sil/stoppable_thread.py
--rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 vessim-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-09 10:27:33.382798 vessim-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2738 2023-07-24 10:14:35.301388 vessim-0.2.0/README.md
+-rw-r--r--   0        0        0     3421 2023-07-28 08:41:48.159115 vessim-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 08:41:41.557996 vessim-0.2.0/vessim/__init__.py
+-rw-r--r--   0        0        0      188 2023-07-09 10:27:33.406229 vessim-0.2.0/vessim/core/__init__.py
+-rw-r--r--   0        0        0     1719 2023-07-28 08:25:16.508419 vessim-0.2.0/vessim/core/consumer.py
+-rw-r--r--   0        0        0     1381 2023-07-09 10:27:33.406473 vessim-0.2.0/vessim/core/microgrid.py
+-rw-r--r--   0        0        0     2691 2023-07-10 17:09:40.175365 vessim-0.2.0/vessim/core/simulator.py
+-rw-r--r--   0        0        0     4159 2023-07-09 10:27:33.406942 vessim-0.2.0/vessim/core/storage.py
+-rw-r--r--   0        0        0      387 2023-07-28 08:25:16.508619 vessim-0.2.0/vessim/cosim/__init__.py
+-rw-r--r--   0        0        0     5918 2023-07-28 08:25:16.508844 vessim-0.2.0/vessim/cosim/_util.py
+-rw-r--r--   0        0        0     1650 2023-07-09 10:27:33.407859 vessim-0.2.0/vessim/cosim/carbon_api.py
+-rw-r--r--   0        0        0     1451 2023-07-28 08:25:16.508986 vessim-0.2.0/vessim/cosim/consumer.py
+-rw-r--r--   0        0        0     1432 2023-07-09 10:27:33.408412 vessim-0.2.0/vessim/cosim/generator.py
+-rw-r--r--   0        0        0      975 2023-07-09 10:27:33.408620 vessim-0.2.0/vessim/cosim/microgrid.py
+-rw-r--r--   0        0        0     2356 2023-07-10 17:09:40.175768 vessim-0.2.0/vessim/cosim/monitor.py
+-rw-r--r--   0        0        0      131 2023-07-09 10:27:33.409269 vessim-0.2.0/vessim/sil/__init__.py
+-rw-r--r--   0        0        0     7510 2023-07-28 08:25:13.946416 vessim-0.2.0/vessim/sil/api_server.py
+-rw-r--r--   0        0        0     2057 2023-07-24 10:14:35.354416 vessim-0.2.0/vessim/sil/http_client.py
+-rw-r--r--   0        0        0      929 2023-07-24 10:14:35.354513 vessim-0.2.0/vessim/sil/node.py
+-rw-r--r--   0        0        0     1559 2023-07-28 08:25:16.509179 vessim-0.2.0/vessim/sil/power_meter.py
+-rw-r--r--   0        0        0     2172 2023-07-28 08:25:13.946828 vessim-0.2.0/vessim/sil/redis_docker.py
+-rw-r--r--   0        0        0     6936 2023-07-28 08:25:16.509356 vessim-0.2.0/vessim/sil/sil_interface.py
+-rw-r--r--   0        0        0     1009 2023-07-09 10:27:33.410922 vessim-0.2.0/vessim/sil/stoppable_thread.py
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 vessim-0.2.0/PKG-INFO
```

### Comparing `vessim-0.1.0/LICENSE` & `vessim-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/README.md` & `vessim-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/pyproject.toml` & `vessim-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-[project]
+[tool.poetry]
 name = "vessim"
-dynamic = ["version", "description"]
+version = "0.2.0"
+description = "A simulator for carbon-aware applications and systems."
+keywords = ["simulation", "energy system", "testbed", "carbon-aware computing", "software-in-the-loop"]
+authors = ["Philipp Wiesner <wiesner@tu-berlin.de>"]
 readme = "README.md"
-requires-python = ">=3.8"
-license = {file = "LICENSE"}
-keywords = ["simulation", "energy system", "testbed", "carbon-aware"]
-authors = [{name = "Philipp Wiesner", email = "wiesner@tu-berlin.de"}]
+license = "MIT"
+homepage = "https://github.com/dos-group/vessim"
+repository = "https://github.com/dos-group/vessim"
+documentation = "https://github.com/dos-group/vessim"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Scientific/Engineering",
   "Topic :: Software Development :: Testing",
@@ -18,68 +21,50 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
-dependencies = [
-  "pandas",
-  "mosaik",
-  "mosaik-api",
-  "loguru",  # TODO shall we remove this?
-]
-
-[project.optional-dependencies]
-sil = [
-  "requests",
-  "fastapi",
-  "docker",
-  "uvicorn",
-]
-dev = [
-  # testing
-  "pytest",
-  # typechecking
-  "mypy",
-  "types-psutil",
-  "pandas-stubs",
-  "types-requests",
-  # linting
-  "black",
-  "ruff",
-  # build
-  "flit",
-]
-analysis = [
-  "jupyterlab",
-  "matplotlib",
-  "seaborn==0.12.2",
-]
-
-
-[project.urls]  # Optional
-"Homepage" = "https://github.com/dos-group/vessim"
-"Source" = "https://github.com/dos-group/vessim"
+[tool.poetry.urls]
 "Bug Reports" = "https://github.com/dos-group/vessim/issues"
 
-# The following would provide a command line executable called `sample`
-# which executes the function `main` from this package when invoked.
-# [project.scripts]  # Optional
-# sample = "sample:main"
+[tool.poetry.dependencies]
+python = "^3.8"
+# Mandatory dependencies
+pandas = "*"
+mosaik = "*"
+mosaik-api = "*"
+loguru = "*"
+# Optional dependencies (software-in-the-loop)
+requests = {version = "*", optional = true}
+fastapi = {version = "*", optional = true}
+docker = {version = "*", optional = true}
+uvicorn = {version = "*", optional = true}
+# Optional dependencies (analysis)
+jupyterlab = {version = "*", optional = true}
+matplotlib = {version = "*", optional = true}
+seaborn = {version = "0.12.2", optional = true}
+
+[tool.poetry.extras]
+sil = ["requests", "fastapi", "docker", "uvicorn"]
+analysis = ["jupyterlab", "matplotlib", "seaborn"]
+
+[tool.poetry.group.dev.dependencies]
+pytest = "*"
+mypy = "*"
+types-psutil = "*"
+pandas-stubs = "*"
+types-requests = "*"
+black = "*"
+ruff = "*"
 
 [build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[tool.flit.sdist]
-exclude = ["data"]
-
-[tool.flit.module]
-name = "vessim"
+requires = ["poetry-core>=1.1.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 90  # Set the maximum characters per line
 target-version = ['py38']   # Set python versions that black should format the code for
 include = '\.py$'  # Format only python files
 
 [tool.ruff]
```

### Comparing `vessim-0.1.0/vessim/core/microgrid.py` & `vessim-0.2.0/vessim/core/microgrid.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/vessim/core/simulator.py` & `vessim-0.2.0/vessim/core/simulator.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/vessim/core/storage.py` & `vessim-0.2.0/vessim/core/storage.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/vessim/cosim/carbon_api.py` & `vessim-0.2.0/vessim/cosim/carbon_api.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/vessim/cosim/computing_system.py` & `vessim-0.2.0/vessim/cosim/consumer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import List
-
+from vessim.core.consumer import Consumer
 from vessim.cosim._util import VessimSimulator, VessimModel
-from vessim.sil.power_meter import PowerMeter
 
 
-class ComputingSystemSim(VessimSimulator):
+class ConsumerSim(VessimSimulator):
     """Computing System simulator that executes its model."""
 
     META = {
         "type": "time-based",
         "models": {
-            "ComputingSystem": {
+            "Consumer": {
                 "public": True,
-                "params": ["power_meters", "pue"],
+                "params": ["consumer"],
                 "attrs": ["p"],
             },
         },
     }
 
     def __init__(self):
         self.step_size = None
@@ -26,38 +24,26 @@
         self.step_size = step_size
         return super().init(sid, time_resolution, eid_prefix=eid_prefix)
 
     def finalize(self) -> None:
         """Stops power meters' threads."""
         super().finalize()
         for model_instance in self.entities.values():
-            for power_meter in model_instance.power_meters: # type: ignore
-                power_meter.finalize()
+            model_instance.consumer.finalize()  # type: ignore
 
     def next_step(self, time):
         return time + self.step_size
 
 
 class _ComputingSystemModel(VessimModel):
-    """Model of the computing system.
-
-    This model considers the power usage effectiveness (PUE) and power
-    consumption of a list of power meters.
 
-    Args:
-        power_meters: A list of PowerMeter objects
-            representing power meters in the system.
-        pue: The power usage effectiveness of the system.
-    """
-
-    def __init__(self, power_meters: List[PowerMeter], pue: float = 1):
-        self.power_meters = power_meters
-        self.pue = pue
+    def __init__(self, consumer: Consumer):
+        self.consumer = consumer
         self.p = 0.0
 
     def step(self, time: int, inputs: dict) -> None:
         """Updates the power consumption of the system.
 
         The power consumption is calculated as the product of the PUE and the
         sum of the node power of all power meters.
         """
-        self.p = -self.pue * sum(pm.measure() for pm in self.power_meters)
+        self.p = -self.consumer.consumption()
```

### Comparing `vessim-0.1.0/vessim/cosim/generator.py` & `vessim-0.2.0/vessim/cosim/generator.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/vessim/cosim/microgrid.py` & `vessim-0.2.0/vessim/cosim/microgrid.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/vessim/cosim/monitor.py` & `vessim-0.2.0/vessim/cosim/monitor.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/vessim/cosim/sil_interface.py` & `vessim-0.2.0/vessim/sil/sil_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -102,35 +102,47 @@
 
         self.collector_thread = StoppableThread(self._api_collector, collection_interval)
         self.collector_thread.start()
 
     def _api_collector(self):
         """Collects data from the API server.
 
+        The endpoint "/sim/collect-set" yields the 3 fields `battery_min_soc`,
+        `battery_grid_charge` and `nodes_power_mode`. Since multiple set
+        request of these values from different actors are possible, each of
+        these fields is a list of dictionaries with the timestamp (formated as
+        `datetime.now().isoformat()`) and the set value at that time.
+
         TODO implement user defined collection method. Current static
         collection method: most recent entry.
         """
         collection = self.http_client.get("/sim/collect-set")
 
+        # The value of the keys is None by default if no set request was made
+        # by an actor => Check if not None first.
         if collection["battery_min_soc"]:
+            # The newest entry is the one with the highest iso timestamp.
             newest_key = max(collection["battery_min_soc"].keys())
             self.storage.min_soc = float(collection["battery_min_soc"][newest_key])
 
         if collection["battery_grid_charge"]:
             newest_key = max(collection["battery_grid_charge"].keys())
             self.policy.grid_power = float(collection["battery_grid_charge"][newest_key])
 
         if collection["nodes_power_mode"]:
             newest_key = max(collection["nodes_power_mode"].keys())
-            nodes_power_mode = {
-                int(k): v for k, v in collection['nodes_power_mode'][newest_key].items()
-            }
+            nodes_power_mode = dict(collection['nodes_power_mode'][newest_key].items())
+            # nodes_power_mode looks e.g. like {"gcp": "normal",...}
+            # Loop through all nodes,
             for node in self.nodes:
-                if node.id in nodes_power_mode[node.id]:
+                if node.id in nodes_power_mode:
+                    # update the power_mode if it changed
                     node.power_mode = nodes_power_mode[node.id]
+                    # and save whatever node had its powermode updated to
+                    # remotely update only that nodes' power mode in step().
                     self.updated_nodes.append(node)
 
     def step(self, time: int, inputs: dict) -> None:
         inputs = simplify_inputs(inputs)
         self.p_cons = inputs["p_cons"]
         self.p_gen = inputs["p_gen"]
         self.ci = inputs["ci"]
@@ -158,10 +170,9 @@
                 try:
                     http_client.put("/power_mode", {"power_mode": node.power_mode})
                 except HTTPClientError as e:
                     print(e)
             # use thread to not slow down simulation
             node_update_thread = Thread(target=update_node_power_model)
             node_update_thread.start()
-            self.updated_nodes.clear()
-
+        self.updated_nodes.clear()
```

### Comparing `vessim-0.1.0/vessim/sil/http_client.py` & `vessim-0.2.0/vessim/sil/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
         Returns:
             A dictionary containing the response.
         """
         response = requests.get(self.server_address + route)
         if response.status_code == 200:
             data = response.json() # assuming the response data is in JSON format
-            print(f'Data received at {route}: {data}')
             return data
 
         raise HTTPClientError(
             response.status_code,
             f'Failed to retrieve data from {route}'
         )
 
@@ -56,15 +55,13 @@
         """
         headers = {'Content-type': 'application/json'}
         response = requests.put(
             self.server_address + route,
             data=json.dumps(data),
             headers=headers
         )
-        if response.status_code == 200:
-            print(f'Data successfully updated at {route}: {data}')
-        else:
+        if response.status_code != 200:
             raise HTTPClientError(
                 response.status_code,
                 f'Failed to update data at {route}'
             )
```

### Comparing `vessim-0.1.0/vessim/sil/node.py` & `vessim-0.2.0/vessim/sil/node.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+from typing import Set
+
 class Node:
     """Represents a physical or virtual computing node.
 
-    This class keeps track of nodes and assigns unique IDs to each new instance. It also
-    allows the setting of a power meter and power mode.
+    This class keeps track of nodes and assigns unique IDs to each new
+    instance. It also allows the setting of a power meter and power mode.
 
     Args:
+        id: A unique ID assigned to each node.
         address: The network address of the node.
-        power_mode: The power mode of the node. Default is "high performance".
-
-    Attributes:
-        id: A unique ID assigned to each node. The ID is auto-incremented for
-            each new node.
-        address: The network address of the node.
+        port: The application port of the node api.
         power_mode: The power mode of the node. Default is "high performance".
     """
 
-    # keep track of ids
-    id = 0
+    existing_ids: Set[str] = set()
 
     def __init__(
         self,
+        id: str,
         address: str,
         port: int = 8000,
         power_mode: str = "high performance"
     ) -> None:
-        Node.id += 1
-        self.id = Node.id
+        if id in self.existing_ids:
+            raise ValueError(f"Node ID \"{id}\" already exists.")
+        self.existing_ids.add(id)
+        self.id = id
         self.address = address
         self.port = port
         self.power_mode = power_mode
```

### Comparing `vessim-0.1.0/vessim/sil/power_meter.py` & `vessim-0.2.0/vessim/sil/power_meter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,14 @@
-from abc import ABC, abstractmethod
 from typing import Optional
 
+from vessim.core.consumer import PowerMeter
 from vessim.sil.http_client import HTTPClient
 from vessim.sil.stoppable_thread import StoppableThread
 
 
-class PowerMeter(ABC):
-    """Abstract base class for power meters.
-
-    Args:
-        name: The name of the power meter.
-    """
-
-    def __init__(self, name: Optional[str] = None):
-        self.name = name
-
-    @abstractmethod
-    def measure(self) -> float:
-        """Abstract method to measure and return the current node power demand.
-
-        Returns:
-            float: The current power demand of the node.
-        """
-        pass
-
-    @abstractmethod
-    def finalize(self) -> None:
-        pass
-
-
 class HttpPowerMeter(PowerMeter):
     """Power meter for an external node that implements the vessim node API.
 
     This class represents a power meter for an external node. It creates a thread
     that updates the power demand from the node API at a given interval.
 
     Args:
@@ -63,22 +39,7 @@
         """Returns the current power demand of the node."""
         return self.power
 
     def finalize(self) -> None:
         """Terminates the power update thread when the instance is finalized."""
         self.update_thread.stop()
         self.update_thread.join()
-
-
-class MockPowerMeter(PowerMeter):
-
-    def __init__(self, p: float, name: Optional[str] = None):
-        super().__init__(name)
-        assert p >= 0
-        self.p = p
-
-    def measure(self) -> float:
-        return self.p
-
-    def finalize(self) -> None:
-        pass
-
```

### Comparing `vessim-0.1.0/vessim/sil/stoppable_thread.py` & `vessim-0.2.0/vessim/sil/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `vessim-0.1.0/PKG-INFO` & `vessim-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,47 @@
 Metadata-Version: 2.1
 Name: vessim
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simulator for carbon-aware applications and systems.
-Keywords: simulation,energy system,testbed,carbon-aware
-Author-email: Philipp Wiesner <wiesner@tu-berlin.de>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Home-page: https://github.com/dos-group/vessim
+License: MIT
+Keywords: simulation,energy system,testbed,carbon-aware computing,software-in-the-loop
+Author: Philipp Wiesner
+Author-email: wiesner@tu-berlin.de
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: pandas
-Requires-Dist: mosaik
-Requires-Dist: mosaik-api
-Requires-Dist: loguru
+Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Testing
+Provides-Extra: analysis
+Provides-Extra: sil
+Requires-Dist: docker ; extra == "sil"
+Requires-Dist: fastapi ; extra == "sil"
 Requires-Dist: jupyterlab ; extra == "analysis"
+Requires-Dist: loguru
 Requires-Dist: matplotlib ; extra == "analysis"
-Requires-Dist: seaborn==0.12.2 ; extra == "analysis"
-Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: mypy ; extra == "dev"
-Requires-Dist: types-psutil ; extra == "dev"
-Requires-Dist: pandas-stubs ; extra == "dev"
-Requires-Dist: types-requests ; extra == "dev"
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: ruff ; extra == "dev"
-Requires-Dist: flit ; extra == "dev"
+Requires-Dist: mosaik
+Requires-Dist: mosaik-api
+Requires-Dist: pandas
 Requires-Dist: requests ; extra == "sil"
-Requires-Dist: fastapi ; extra == "sil"
-Requires-Dist: docker ; extra == "sil"
+Requires-Dist: seaborn (==0.12.2) ; extra == "analysis"
 Requires-Dist: uvicorn ; extra == "sil"
 Project-URL: Bug Reports, https://github.com/dos-group/vessim/issues
-Project-URL: Homepage, https://github.com/dos-group/vessim
-Project-URL: Source, https://github.com/dos-group/vessim
-Provides-Extra: analysis
-Provides-Extra: dev
-Provides-Extra: sil
+Project-URL: Documentation, https://github.com/dos-group/vessim
+Project-URL: Repository, https://github.com/dos-group/vessim
+Description-Content-Type: text/markdown
 
 # Vessim
 
 [![PyPI version](https://img.shields.io/pypi/v/vessim.svg?color=52c72b)](https://pypi.org/project/vessim/)
 ![Build](https://github.com/dos-group/vessim/actions/workflows/vessim-ci.yml/badge.svg)
 [![License](https://img.shields.io/pypi/l/vessim.svg)](https://pypi.org/project/vessim/)
 [![Supported versions](https://img.shields.io/pypi/pyversions/vessim.svg)](https://pypi.org/project/vessim/)
```

