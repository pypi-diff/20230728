# Comparing `tmp/pytest-mqtt-0.2.0.tar.gz` & `tmp/pytest-mqtt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mqtt-0.2.0.tar", last modified: Wed Mar 15 18:15:49 2023, max compression
+gzip compressed data, was "pytest-mqtt-0.3.0.tar", last modified: Thu Jul 27 23:09:04 2023, max compression
```

## Comparing `pytest-mqtt-0.2.0.tar` & `pytest-mqtt-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-03-15 18:15:49.084692 pytest-mqtt-0.2.0/
--rw-r--r--   0 amo        (501) staff       (20)     1161 2022-09-20 10:04:35.000000 pytest-mqtt-0.2.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)     6969 2023-03-15 18:15:49.084169 pytest-mqtt-0.2.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     4680 2023-03-15 18:10:27.000000 pytest-mqtt-0.2.0/README.rst
--rw-r--r--   0 amo        (501) staff       (20)     4146 2023-03-15 18:15:05.000000 pytest-mqtt-0.2.0/pyproject.toml
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-03-15 18:15:49.080908 pytest-mqtt-0.2.0/pytest_mqtt/
--rw-r--r--   0 amo        (501) staff       (20)      358 2022-09-20 10:04:35.000000 pytest-mqtt-0.2.0/pytest_mqtt/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     4819 2022-09-20 10:04:35.000000 pytest-mqtt-0.2.0/pytest_mqtt/capmqtt.py
--rw-r--r--   0 amo        (501) staff       (20)      251 2022-09-20 10:04:35.000000 pytest-mqtt-0.2.0/pytest_mqtt/model.py
--rw-r--r--   0 amo        (501) staff       (20)     2272 2023-03-15 18:10:27.000000 pytest-mqtt-0.2.0/pytest_mqtt/mosquitto.py
--rw-r--r--   0 amo        (501) staff       (20)      554 2022-09-20 10:04:35.000000 pytest-mqtt-0.2.0/pytest_mqtt/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-03-15 18:15:49.083475 pytest-mqtt-0.2.0/pytest_mqtt.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     6969 2023-03-15 18:15:49.000000 pytest-mqtt-0.2.0/pytest_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      367 2023-03-15 18:15:49.000000 pytest-mqtt-0.2.0/pytest_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-03-15 18:15:49.000000 pytest-mqtt-0.2.0/pytest_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       75 2023-03-15 18:15:49.000000 pytest-mqtt-0.2.0/pytest_mqtt.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      311 2023-03-15 18:15:49.000000 pytest-mqtt-0.2.0/pytest_mqtt.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       12 2023-03-15 18:15:49.000000 pytest-mqtt-0.2.0/pytest_mqtt.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-03-15 18:15:49.084774 pytest-mqtt-0.2.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)      210 2022-09-20 10:04:35.000000 pytest-mqtt-0.2.0/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-27 23:09:04.112872 pytest-mqtt-0.3.0/
+-rw-r--r--   0 amo        (501) staff       (20)     1161 2022-09-20 10:04:35.000000 pytest-mqtt-0.3.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)     6969 2023-07-27 23:09:04.112637 pytest-mqtt-0.3.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     4680 2023-03-15 18:10:27.000000 pytest-mqtt-0.3.0/README.rst
+-rw-r--r--   0 amo        (501) staff       (20)     4180 2023-07-27 23:08:57.000000 pytest-mqtt-0.3.0/pyproject.toml
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-27 23:09:04.110699 pytest-mqtt-0.3.0/pytest_mqtt/
+-rw-r--r--   0 amo        (501) staff       (20)      358 2022-09-20 10:04:35.000000 pytest-mqtt-0.3.0/pytest_mqtt/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     4830 2023-07-27 23:08:25.000000 pytest-mqtt-0.3.0/pytest_mqtt/capmqtt.py
+-rw-r--r--   0 amo        (501) staff       (20)      251 2022-09-20 10:04:35.000000 pytest-mqtt-0.3.0/pytest_mqtt/model.py
+-rw-r--r--   0 amo        (501) staff       (20)     2584 2023-07-27 23:08:25.000000 pytest-mqtt-0.3.0/pytest_mqtt/mosquitto.py
+-rw-r--r--   0 amo        (501) staff       (20)      554 2022-09-20 10:04:35.000000 pytest-mqtt-0.3.0/pytest_mqtt/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-27 23:09:04.112315 pytest-mqtt-0.3.0/pytest_mqtt.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     6969 2023-07-27 23:09:04.000000 pytest-mqtt-0.3.0/pytest_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      367 2023-07-27 23:09:04.000000 pytest-mqtt-0.3.0/pytest_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-07-27 23:09:04.000000 pytest-mqtt-0.3.0/pytest_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       75 2023-07-27 23:09:04.000000 pytest-mqtt-0.3.0/pytest_mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      311 2023-07-27 23:09:04.000000 pytest-mqtt-0.3.0/pytest_mqtt.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       12 2023-07-27 23:09:04.000000 pytest-mqtt-0.3.0/pytest_mqtt.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-07-27 23:09:04.113033 pytest-mqtt-0.3.0/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)      210 2022-09-20 10:04:35.000000 pytest-mqtt-0.3.0/setup.py
```

### Comparing `pytest-mqtt-0.2.0/LICENSE` & `pytest-mqtt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-mqtt-0.2.0/PKG-INFO` & `pytest-mqtt-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mqtt
-Version: 0.2.0
+Version: 0.3.0
 Summary: pytest-mqtt supports testing systems based on MQTT
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: homepage, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: documentation, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: repository, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: changelog, https://github.com/mqtt-tools/pytest-mqtt/blob/main/CHANGES.rst
```

### Comparing `pytest-mqtt-0.2.0/README.rst` & `pytest-mqtt-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-mqtt-0.2.0/pyproject.toml` & `pytest-mqtt-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Project definition
 # ==================
 
 # Derived from https://peps.python.org/pep-0621/
 
 [project]
 name = "pytest-mqtt"
-version = "0.2.0"
+version = "0.3.0"
 description = "pytest-mqtt supports testing systems based on MQTT"
 readme = "README.rst"
 requires-python = ">=3.6"
 license = {text = "MIT"}
 keywords = ["mqtt", "pytest", "testing", "mosquitto", "paho"]
 authors = [
   {name = "Andreas Motl", email = "andreas.motl@panodata.org"},
@@ -159,9 +159,9 @@
   {cmd="coverage report"},
   {cmd="coverage xml"},
 ]
 
 release = [
   {cmd="minibump bump --relax minor"},
   {cmd="python -m build"},
-  {cmd="twine upload dist/*"},
+  {cmd="twine upload --skip-existing dist/*.tar.gz dist/*.whl"},
 ]
```

### Comparing `pytest-mqtt-0.2.0/pytest_mqtt/capmqtt.py` & `pytest-mqtt-0.3.0/pytest_mqtt/capmqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         message = MqttMessage(
             topic=msg.topic,
             payload=payload,
             userdata=userdata,
         )
         self._buffer.append(message)
-        logger.debug("[PYTEST] MQTT message received: %s", message)
+        logger.debug("[PYTEST] MQTT message received: %s", str(message)[:200])
 
     def finalize(self) -> None:
         """Finalizes the fixture."""
         self.mqtt_client.stop()
         self.mqtt_client.join(timeout=4.2)
         self._buffer = []
```

### Comparing `pytest-mqtt-0.2.0/pytest_mqtt/mosquitto.py` & `pytest-mqtt-0.3.0/pytest_mqtt/mosquitto.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,25 +40,31 @@
 
     def check(self):
         # TODO: Add real implementation.
         return True
 
     def pull_image(self):
         """
-        Image needs to be pull explicitly.
+        Image needs to be pulled explicitly.
         Workaround against `404 Client Error: Not Found for url: http+docker://localhost/v1.23/containers/create`.
 
         - https://github.com/jpmens/mqttwarn/pull/589#issuecomment-1249680740
         - https://github.com/docker/docker-py/issues/2101
         """
         docker_client = docker.from_env(version=self.docker_version)
         image_name = self.image
         docker_client.images.pull(image_name)
 
     def run(self):
+        docker_client = docker.from_env(version=self.docker_version)
+        docker_url = docker_client.api.base_url
+        try:
+            docker_client.ping()
+        except Exception:
+            raise ConnectionError(f"Cannot connect to the Docker daemon at {docker_url}. Is the docker daemon running?")
         self.pull_image()
         return super(Mosquitto, self).run()
 
 
 mosquitto_image = Mosquitto()
```

### Comparing `pytest-mqtt-0.2.0/pytest_mqtt/util.py` & `pytest-mqtt-0.3.0/pytest_mqtt/util.py`

 * *Files identical despite different names*

### Comparing `pytest-mqtt-0.2.0/pytest_mqtt.egg-info/PKG-INFO` & `pytest-mqtt-0.3.0/pytest_mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mqtt
-Version: 0.2.0
+Version: 0.3.0
 Summary: pytest-mqtt supports testing systems based on MQTT
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: homepage, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: documentation, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: repository, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: changelog, https://github.com/mqtt-tools/pytest-mqtt/blob/main/CHANGES.rst
```

