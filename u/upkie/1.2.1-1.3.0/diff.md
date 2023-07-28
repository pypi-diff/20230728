# Comparing `tmp/upkie-1.2.1.tar.gz` & `tmp/upkie-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkie-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "upkie-1.3.0.tar", last modified: Fri Jul 28 12:47:19 2023, max compression
```

## Comparing `upkie-1.2.1.tar` & `upkie-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     8466 2023-07-18 17:28:41.190380 upkie-1.2.1/README.md
--rw-r--r--   0        0        0     1890 2023-07-18 17:28:41.190380 upkie-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      695 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/__init__.py
--rw-r--r--   0        0        0     1090 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/BUILD
--rw-r--r--   0        0        0     1275 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/__init__.py
--rw-r--r--   0        0        0     2809 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/standing_reward.py
--rw-r--r--   0        0        0      549 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/tests/BUILD
--rw-r--r--   0        0        0     2530 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/tests/upkie_base_env_test.py
--rw-r--r--   0        0        0     2446 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/tests/upkie_servos_env_test.py
--rw-r--r--   0        0        0     2330 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/tests/upkie_wheels_env_test.py
--rw-r--r--   0        0        0     8982 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/upkie_base_env.py
--rw-r--r--   0        0        0     7387 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/upkie_servos_env.py
--rw-r--r--   0        0        0     7207 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/envs/upkie_wheels_env.py
--rw-r--r--   0        0        0      356 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/observers/base_pitch/BUILD
--rw-r--r--   0        0        0      902 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/observers/base_pitch/__init__.py
--rw-r--r--   0        0        0     5612 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/observers/base_pitch/base_pitch.py
--rw-r--r--   0        0        0      305 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/observers/base_pitch/tests/BUILD
--rw-r--r--   0        0        0     3105 2023-07-18 17:28:41.186380 upkie-1.2.1/upkie/observers/base_pitch/tests/base_pitch_test.py
--rw-r--r--   0        0        0     1171 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/BUILD
--rw-r--r--   0        0        0     1896 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/clamp.py
--rw-r--r--   0        0        0     1137 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/datetime_now_string.h
--rw-r--r--   0        0        0      803 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/exceptions.py
--rw-r--r--   0        0        0     2820 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/filters.py
--rw-r--r--   0        0        0     2433 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/pinocchio.py
--rw-r--r--   0        0        0     1207 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/realtime.py
--rw-r--r--   0        0        0     1900 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/rotations.py
--rw-r--r--   0        0        0     1983 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/spdlog.py
--rw-r--r--   0        0        0      634 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/tests/BUILD
--rw-r--r--   0        0        0     1303 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/tests/clamp_test.py
--rw-r--r--   0        0        0      986 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/tests/datetime_now_string_test.cpp
--rw-r--r--   0        0        0     2232 2023-07-18 17:28:41.190380 upkie-1.2.1/upkie/utils/tests/pinocchio_test.py
--rw-r--r--   0        0        0     9900 1970-01-01 00:00:00.000000 upkie-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8460 2023-07-28 12:47:19.327366 upkie-1.3.0/README.md
+-rw-r--r--   0        0        0     1890 2023-07-28 12:47:19.323366 upkie-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-07-28 12:47:19.327366 upkie-1.3.0/upkie/__init__.py
+-rw-r--r--   0        0        0     1079 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/BUILD
+-rw-r--r--   0        0        0     1275 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/__init__.py
+-rw-r--r--   0        0        0     2809 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/standing_reward.py
+-rw-r--r--   0        0        0      549 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/BUILD
+-rw-r--r--   0        0        0     2555 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/upkie_base_env_test.py
+-rw-r--r--   0        0        0     2465 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/upkie_servos_env_test.py
+-rw-r--r--   0        0        0     2349 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/upkie_wheels_env_test.py
+-rw-r--r--   0        0        0     9299 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/upkie_base_env.py
+-rw-r--r--   0        0        0     7657 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/upkie_servos_env.py
+-rw-r--r--   0        0        0     7387 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/upkie_wheels_env.py
+-rw-r--r--   0        0        0      356 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/BUILD
+-rw-r--r--   0        0        0      902 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/__init__.py
+-rw-r--r--   0        0        0     5612 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/base_pitch.py
+-rw-r--r--   0        0        0      305 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/tests/BUILD
+-rw-r--r--   0        0        0     3105 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/tests/base_pitch_test.py
+-rw-r--r--   0        0        0     1201 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/BUILD
+-rw-r--r--   0        0        0     1896 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/clamp.py
+-rw-r--r--   0        0        0     1137 2023-07-28 12:47:19.323366 upkie-1.3.0/upkie/utils/datetime_now_string.h
+-rw-r--r--   0        0        0      803 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/exceptions.py
+-rw-r--r--   0        0        0     2820 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/filters.py
+-rw-r--r--   0        0        0     2433 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/pinocchio.py
+-rw-r--r--   0        0        0     1430 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/raspi.py
+-rw-r--r--   0        0        0     1900 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/rotations.py
+-rw-r--r--   0        0        0     1983 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/spdlog.py
+-rw-r--r--   0        0        0      634 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/BUILD
+-rw-r--r--   0        0        0     1303 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/clamp_test.py
+-rw-r--r--   0        0        0      986 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/datetime_now_string_test.cpp
+-rw-r--r--   0        0        0     2232 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/pinocchio_test.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 upkie-1.3.0/setup.py
+-rw-r--r--   0        0        0     9894 1970-01-01 00:00:00.000000 upkie-1.3.0/PKG-INFO
```

### Comparing `upkie-1.2.1/README.md` & `upkie-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Upkie wheeled biped
+# Upkie wheeled biped robot
 
-[![Build instructions](https://img.shields.io/badge/build-instructions-brightgreen?logo=read-the-docs&style=flat)](https://github.com/tasts-robots/upkie/wiki)
 [![CI](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml/badge.svg)](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml)
+[![Build instructions](https://img.shields.io/badge/build-instructions-brightgreen?logo=read-the-docs&style=flat)](https://github.com/tasts-robots/upkie/wiki)
+[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/upkie/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/upkie/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/upkie?branch=main)
-[![Vulp](https://img.shields.io/badge/%F0%9F%A6%8A%20vulp-1.2.0-orange)](https://github.com/tasts-robots/vulp)
-[![Chat](https://img.shields.io/matrix/tasts-robots:matrix.org?color=4EB899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
-
-Build and control **Upkie** wheeled bipeds. Made for Linux 🐧
+[![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
+[![Chat](https://img.shields.io/badge/matrix-chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
-Questions about building and using an Upkie, or balancing robots in general, are all welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://app.element.io/#/room/#tasts-robots:matrix.org).
+Build instructions and software for **Upkie** wheeled bipeds. Develop on Linux 🐧 or macOS 🍏, deploy to the robot's Raspberry Pi 🍓. Questions about building and using an Upkie, or balancing robots in general, are welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://app.element.io/#/room/#tasts-robots:matrix.org).
 
 ## Quick sim
 
 If you have Python and a C++ compiler (Ubuntu: ``sudo apt install curl g++ python3-dev``), you can run an Upkie simulation right from the command line. It won't install anything on your machine, everything will run locally from the repository:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
@@ -61,31 +60,29 @@
 
 ## Running an agent
 
 There are two ways we can develop and run agents: using the [PyPI](#pypi) distribution, or [Bazel](#bazel). PyPI is better to get started and prototype everything in Python, while Bazel is better to recompile things from source.
 
 ### PyPI
 
-[![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
-[![PyPI downloads](https://pepy.tech/badge/upkie/month)](https://pepy.tech/project/upkie)
 
 The PyPI distribution is the recommended way to control Upkie in Python. It is already [fast enough](https://github.com/tasts-robots/vulp#performance) for real-time control.
 
 #### Installation
 
 ```console
 pip install upkie
 ```
 
 #### Example
 
 While [running a spine](#running-a-spine), you can execute the following code in a Python interpreter or as a standalone Python script:
 
 ```python
-import gym
+import gymnasium as gym
 import upkie.envs
 
 upkie.envs.register()
 
 with gym.make("UpkieWheelsEnv-v4", frequency=200.0) as env:
     observation = env.reset()
     action = 0.0 * env.action_space.sample()
```

### Comparing `upkie-1.2.1/pyproject.toml` & `upkie-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "gymnasium >=0.28.1",
-    "loop-rate-limiters >=0.4.0",
+    "loop-rate-limiters >=0.5.0",
     "mpacklog >=3.0.0",
     "numpy >=1.22.0",
-    "upkie_description >=1.2.0",
-    "vulp >=1.2.1",
+    "upkie_description >=1.4.0",
+    "vulp >=1.3.0",
 ]
 keywords = ["wheeled", "biped", "robot", "balance", "motion", "control", "robotics"]
 
 [project.urls]
 Documentation = "https://tasts-robots.org/doc/upkie/"
 Source = "https://github.com/tasts-robots/upkie"
 Tracker = "https://github.com/tasts-robots/upkie/issues"
```

### Comparing `upkie-1.2.1/upkie/__init__.py` & `upkie-1.3.0/upkie/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python module to control Upkie wheeled bipeds."""
 
-__version__ = "1.2.1"
+__version__ = "1.3.0"
```

### Comparing `upkie-1.2.1/upkie/envs/BUILD` & `upkie-1.3.0/upkie/envs/BUILD`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 py_library(
     name = "upkie_base_env",
     srcs = [
         "standing_reward.py",
         "upkie_base_env.py",
     ],
     deps = [
+        "//config",
         "@upkie//observers/base_pitch",
         "@vulp//spine:python",
         requirement("gymnasium"),
         requirement("loop_rate_limiters"),
-        requirement("pyyaml"),
         requirement("upkie_description"),
     ],
 )
 
 py_library(
-    name = "upkie_wheels_env",
+    name = "upkie_servos_env",
     srcs = [
-        "upkie_wheels_env.py",
+        "upkie_servos_env.py",
     ],
     deps = [
         ":upkie_base_env",
+        "//utils:pinocchio",
     ],
 )
 
 py_library(
-    name = "upkie_servos_env",
+    name = "upkie_wheels_env",
     srcs = [
-        "upkie_servos_env.py",
+        "upkie_wheels_env.py",
     ],
     deps = [
         ":upkie_base_env",
-        "//utils:pinocchio",
     ],
 )
 
 py_library(
     name = "envs",
     srcs = [
         "__init__.py",
```

### Comparing `upkie-1.2.1/upkie/envs/__init__.py` & `upkie-1.3.0/upkie/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/envs/standing_reward.py` & `upkie-1.3.0/upkie/envs/standing_reward.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/envs/tests/BUILD` & `upkie-1.3.0/upkie/envs/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/envs/tests/upkie_base_env_test.py` & `upkie-1.3.0/upkie/envs/tests/upkie_base_env_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,22 +72,23 @@
 class TestUpkieBaseEnv(unittest.TestCase):
     def setUp(self):
         shm_name = "/vroum"
         shared_memory = posix_ipc.SharedMemory(
             shm_name, posix_ipc.O_RDWR | posix_ipc.O_CREAT, size=42
         )
         self.env = UpkieBaseChild(
-            config=None,
             fall_pitch=1.0,
             frequency=100.0,
             shm_name=shm_name,
+            spine_config=None,
         )
         shared_memory.close_fd()
         self.env._spine = MockSpine()
 
     def test_reset(self):
-        _, observation_dict = self.env.reset(return_info=True)
+        _, info = self.env.reset()
+        observation_dict = info["observation"]
         self.assertGreaterEqual(observation_dict["number"], 1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `upkie-1.2.1/upkie/envs/tests/upkie_servos_env_test.py` & `upkie-1.3.0/upkie/envs/tests/upkie_servos_env_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,16 @@
             frequency=100.0,
             shm_name=shm_name,
         )
         shared_memory.close_fd()
         self.env._spine = MockSpine()
 
     def test_reset(self):
-        observation, observation_dict = self.env.reset(return_info=True)
+        observation, info = self.env.reset()
+        observation_dict = info["observation"]
         self.assertAlmostEqual(
             observation[1], observation_dict["wheel_odometry"]["position"]
         )
         self.assertGreaterEqual(observation_dict["number"], 1)
 
 
 if __name__ == "__main__":
```

### Comparing `upkie-1.2.1/upkie/envs/tests/upkie_wheels_env_test.py` & `upkie-1.3.0/upkie/envs/tests/upkie_wheels_env_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             frequency=100.0,
             shm_name=shm_name,
         )
         shared_memory.close_fd()
         self.env._spine = MockSpine()
 
     def test_reset(self):
-        observation, observation_dict = self.env.reset(return_info=True)
+        observation, info = self.env.reset()
+        observation_dict = info["observation"]
         self.assertAlmostEqual(
             observation[1], observation_dict["wheel_odometry"]["position"]
         )
         self.assertGreaterEqual(observation_dict["number"], 1)
 
 
 if __name__ == "__main__":
```

### Comparing `upkie-1.2.1/upkie/envs/upkie_base_env.py` & `upkie-1.3.0/upkie/envs/upkie_base_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,48 +13,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 import asyncio
-from typing import Dict, Optional, Tuple, Union
+from typing import Dict, Optional, Tuple
 
-import gymnasium as gym
+import gymnasium
 import numpy as np
 from loop_rate_limiters import AsyncRateLimiter, RateLimiter
 from vulp.spine import SpineInterface
 
+import upkie.config
 from upkie.observers.base_pitch import compute_base_pitch_from_imu
 
-DEFAULT_CONFIG = {
-    "bullet": {
-        "control_mode": "torque",
-        "follower_camera": False,
-        "gui": True,
-        "position_init_base_in_world": [0.0, 0.0, 0.6],
-        "torque_control": {
-            "kp": 20.0,
-            "kd": 1.0,
-        },
-    },
-    "floor_contact": {
-        "upper_leg_torque_threshold": 10.0,
-    },
-    "wheel_contact": {
-        "cutoff_period": 0.2,
-        "liftoff_inertia": 0.001,
-        "min_touchdown_acceleration": 2.0,
-        "min_touchdown_torque": 0.015,
-        "touchdown_inertia": 0.004,
-    },
-}
 
-
-class UpkieBaseEnv(abc.ABC, gym.Env):
+class UpkieBaseEnv(abc.ABC, gymnasium.Env):
 
     """!
     Base class for Upkie environments.
 
     This class has the following attributes:
 
     - ``config``: Configuration dictionary sent to the spine.
@@ -62,85 +40,92 @@
 
     @note This environment is made to run on a single CPU thread rather than on
     GPU/TPU. The downside for reinforcement learning is that computations are
     not massively parallel. The upside is that it simplifies deployment to the
     real robot, as it relies on the same spine interface that runs on Upkie.
     """
 
-    __frequency: Optional[float]
     __async_rate: Optional[AsyncRateLimiter]
+    __frequency: Optional[float]
     __rate: Optional[RateLimiter]
     _spine: SpineInterface
-    config: dict
     fall_pitch: float
+    spine_config: dict
 
     def __init__(
         self,
-        config: Optional[dict],
         fall_pitch: float,
         frequency: Optional[float],
         shm_name: str,
+        spine_config: Optional[dict],
     ) -> None:
         """!
         Initialize environment.
 
-        @param config Configuration dictionary sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
         @param frequency Regulated frequency of the control loop, in Hz. Set to
             ``None`` to disable loop frequency regulation.
         @param shm_name Name of shared-memory file.
+        @param spine_config Additional spine configuration overriding the
+            defaults from ``//config:spine.yaml``. The combined configuration
+            dictionary is sent to the spine at every :func:`reset`.
         """
-        if config is None:
-            config = DEFAULT_CONFIG
+        merged_spine_config = upkie.config.SPINE_CONFIG.copy()
+        if spine_config is not None:
+            merged_spine_config.update(spine_config)
         self.__frequency = frequency
         self._spine = SpineInterface(shm_name)
-        self.config = config
         self.fall_pitch = fall_pitch
+        self.spine_config = merged_spine_config
 
     @property
     def frequency(self) -> Optional[float]:
+        """!
+        Regulated frequency of the control loop in Hz, or ``None`` if there is
+        no loop frequency regulation.
+        """
         return self.__frequency
 
     def close(self) -> None:
         """!
         Stop the spine properly.
         """
         self._spine.stop()
 
     def reset(
         self,
         *,
         seed: Optional[int] = None,
-        return_info: bool = True,
         options: Optional[dict] = None,
-    ) -> Union[np.ndarray, Tuple[np.ndarray, Dict]]:
+    ) -> Tuple[np.ndarray, Dict]:
         """!
         Resets the spine and get an initial observation.
 
         @param seed It is not used yet but should be. TODO(perrin-isir)
-        @param return_info If true, return the dictionary observation as an
-            extra info dictionary.
         @param options Currently unused.
         @returns
-            - ``observation``: the initial vectorized observation.
-            - ``info``: an optional dictionary containing extra information.
-                It is only returned if ``return_info`` is set to true.
+            - ``observation``: Initial vectorized observation, i.e. an element
+              of the environment's ``observation_space``.
+            - ``info``: Dictionary with auxiliary diagnostic information. For
+              us this will be the full observation dictionary coming sent by
+              the spine.
         """
-        # super().reset(seed=seed)
+        super().reset(seed=seed)
         self.__reset_rates()
         self._spine.stop()
-        self._spine.start(self.config)
+        self._spine.start(self.spine_config)
         self._spine.get_observation()  # might be a pre-reset observation
         observation_dict = self._spine.get_observation()
         self.parse_first_observation(observation_dict)
         observation = self.vectorize_observation(observation_dict)
-        if not return_info:
-            return observation
-        else:  # return_info
-            return observation, observation_dict
+        info = {
+            "action": None,
+            "observation": observation_dict,
+        }
+        return observation, info
 
     def __reset_rates(self):
         self.__async_rate = None
         self.__rate = None
         if self.__frequency is None:  # no rate
             return
         try:
@@ -156,23 +141,27 @@
         """!
         Run one timestep of the environment's dynamics. When the end of the
         episode is reached, you are responsible for calling `reset()` to reset
         the environment's state.
 
         @param action Action from the agent.
         @returns
-            - ``observation``: Agent's observation of the environment.
-            - ``reward``: Amount of reward returned after previous action.
-            - ``terminated``: Whether the agent reaches the terminal state,
-              which can be a good or a bad thing. If true, the user needs to
+            - ``observation``: Observation of the environment, i.e. an element
+              of its ``observation_space``.
+            - ``reward``: Reward returned after taking the action.
+            - ``terminated``: Whether the agent reached a terminal state,
+              which can be a good or a bad thing. When true, the user needs to
               call :func:`reset()`.
             - ``truncated'': Whether the episode is reaching max number of
-              steps.
-            - ``info``: Contains auxiliary diagnostic information (helpful for
-              debugging, logging, and sometimes learning).
+              steps. This boolean can signal a premature end of the episode,
+              i.e. before a terminal state is reached. When true, the user
+              needs to call :func:`reset()`.
+            - ``info``: Dictionary with auxiliary diagnostic information. For
+              us this will be the full observation dictionary coming sent by
+              the spine.
         """
         action_dict = self.dictionarize_action(action)
         if self.__rate is not None:
             self.__rate.sleep()  # wait until clock tick to send the action
         return self.__step(action_dict)
 
     async def async_step(
@@ -181,23 +170,27 @@
         """!
         Run one timestep of the environment's dynamics using asynchronous I/O.
         When the end of the episode is reached, you are responsible for calling
         `reset()` to reset the environment's state.
 
         @param action Action from the agent.
         @returns
-            - ``observation``: Agent's observation of the environment.
-            - ``reward``: Amount of reward returned after previous action.
-            - ``terminated``: Whether the agent reaches the terminal state,
-              which can be a good or a bad thing. If true, the user needs to
+            - ``observation``: Observation of the environment, i.e. an element
+              of its ``observation_space``.
+            - ``reward``: Reward returned after taking the action.
+            - ``terminated``: Whether the agent reached a terminal state,
+              which can be a good or a bad thing. When true, the user needs to
               call :func:`reset()`.
-            - ``truncated'': Whether the episode is truncated (reaching max
-              number of steps).
-            - ``info``: Contains auxiliary diagnostic information (helpful for
-              debugging, logging, and sometimes learning).
+            - ``truncated'': Whether the episode is reaching max number of
+              steps. This boolean can signal a premature end of the episode,
+              i.e. before a terminal state is reached. When true, the user
+              needs to call :func:`reset()`.
+            - ``info``: Dictionary with auxiliary diagnostic information. For
+              us this will be the full observation dictionary coming sent by
+              the spine.
         """
         action_dict = self.dictionarize_action(action)
         if self.__async_rate is not None:
             await self.__async_rate.sleep()  # send action at next clock tick
         return self.__step(action_dict)
 
     def __step(
```

### Comparing `upkie-1.2.1/upkie/envs/upkie_servos_env.py` & `upkie-1.3.0/upkie/envs/upkie_servos_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,126 +34,136 @@
 
 
 class UpkieServosEnv(UpkieBaseEnv):
 
     """!
     Upkie with full observation and joint position-velocity-torque actions.
 
-    The environment has the following attributes:
-
-    - ``reward``: Reward function.
-    - ``robot``: Pinocchio robot wrapper.
-    - ``state_max``: Maximum values for the action and observation vectors.
-    - ``state_min``: Minimum values for the action and observation vectors.
-    - ``version``: Environment version number.
+    ### Action space
 
-    Vectorized observations have the following structure:
+    Vectorized actions have the following structure:
 
     <table>
         <tr>
             <td><strong>Index</strong></td>
             <td><strong>Description</strong></td>
             </tr>
         <tr>
             <td>``[0:nq]``</td>
-            <td>Joint positions in [rad].</td>
+            <td>Joint position commands in [rad].</td>
         </tr>
         <tr>
             <td>``[nq:nq + nv]``</td>
-            <td>Joint velocities in [rad] / [s].</td>
+            <td>Joint velocity commands in [rad] / [s].</td>
         </tr>
         <tr>
             <td>``[nq + nv:nq + 2 * nv]``</td>
             <td>Joint torques in [N] * [m].</td>
         </tr>
     </table>
 
-    Vectorized actions have the following structure:
+    ### Observation space
+
+    Vectorized observations have the following structure:
 
     <table>
         <tr>
             <td><strong>Index</strong></td>
             <td><strong>Description</strong></td>
             </tr>
         <tr>
             <td>``[0:nq]``</td>
-            <td>Joint position commands in [rad].</td>
+            <td>Joint positions in [rad].</td>
         </tr>
         <tr>
             <td>``[nq:nq + nv]``</td>
-            <td>Joint velocity commands in [rad] / [s].</td>
+            <td>Joint velocities in [rad] / [s].</td>
         </tr>
         <tr>
             <td>``[nq + nv:nq + 2 * nv]``</td>
             <td>Joint torques in [N] * [m].</td>
         </tr>
     </table>
 
-    The reward function is defined in @ref
-    envs.standing_reward.StandingReward "StandingReward".
+    ### Rewards
+
+    The reward function is defined in @ref envs.standing_reward.StandingReward
+    "StandingReward".
+
+    ### Attributes
+
+    The environment has the following attributes:
+
+    - ``reward``: Reward function.
+    - ``robot``: Pinocchio robot wrapper.
+    - ``state_max``: Maximum values for the action and observation vectors.
+    - ``state_min``: Minimum values for the action and observation vectors.
+    - ``version``: Environment version number.
 
     See also @ref envs.upkie_base_env.UpkieBaseEnv "UpkieBaseEnv" for notes on
     using this environment.
     """
 
     reward: StandingReward
     robot: pin.RobotWrapper
     version: int = 2
 
     def __init__(
         self,
-        config: Optional[dict] = None,
         fall_pitch: float = 1.0,
         frequency: float = 200.0,
         shm_name: str = "/vulp",
+        spine_config: Optional[dict] = None,
     ):
         """!
         Initialize environment.
 
-        @param config Configuration dictionary, also sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
         @param frequency Regulated frequency of the control loop, in Hz.
         @param shm_name Name of shared-memory file.
+        @param spine_config Additional spine configuration overriding the
+            defaults from ``//config:spine.yaml``. The combined configuration
+            dictionary is sent to the spine at every :func:`reset`.
         """
         super().__init__(
-            config=config,
             fall_pitch=fall_pitch,
             frequency=frequency,
             shm_name=shm_name,
+            spine_config=spine_config,
         )
 
         robot = upkie_description.load_in_pinocchio(root_joint=None)
         model = robot.model
 
         q_min, q_max = box_position_limits(model)
         v_max = box_velocity_limits(model)
         tau_max = box_torque_limits(model)
         state_dim = model.nq + 2 * model.nv
         state_max = np.hstack([q_max, v_max, tau_max])
         state_min = np.hstack([q_min, -v_max, -tau_max])
         state_max = np.float32(state_max)
         state_min = np.float32(state_min)
 
-        # gym.Env: action_space
+        # gymnasium.Env: action_space
         self.action_space = spaces.Box(
             state_min,
             state_max,
             shape=(state_dim,),
             dtype=np.float32,
         )
 
-        # gym.Env: observation_space
+        # gymnasium.Env: observation_space
         self.observation_space = spaces.Box(
             state_min,
             state_max,
             shape=(state_dim,),
             dtype=np.float32,
         )
 
-        # gym.Env: reward_range
+        # gymnasium.Env: reward_range
         self.reward_range = StandingReward.get_range()
 
         # Class members
         self.__joints = list(robot.model.names)[1:]
         self.__last_positions = {}
         self.q_max = q_max
         self.q_min = q_min
```

### Comparing `upkie-1.2.1/upkie/envs/upkie_wheels_env.py` & `upkie-1.3.0/upkie/envs/upkie_wheels_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,23 +34,35 @@
 MAX_GROUND_POSITION: float = float("inf")
 MAX_BASE_ANGULAR_VELOCITY: float = 1000.0  # rad/s
 
 
 class UpkieWheelsEnv(UpkieBaseEnv):
 
     """!
-    Upkie with ground velocity as the action.
+    Upkie with ground velocity actions.
+
+    The environment id is ``UpkieWheelsEnv-v4``.
+
+    ### Action space
+
+    Vectorized actions have the following structure:
 
     <table>
         <tr>
-            <td><strong>Environment id</strong></td>
-            <td>UpkieWheelsEnv-v4</td>
+            <td><strong>Index</strong></td>
+            <td><strong>Description</strong></td>
+            </tr>
+        <tr>
+            <td>``0``</td>
+            <td>Ground velocity in [m] / [s].</td>
         </tr>
     </table>
 
+    ### Observation space
+
     Vectorized observations have the following structure:
 
     <table>
         <tr>
             <td><strong>Index</strong></td>
             <td><strong>Description</strong></td>
         </tr>
@@ -71,37 +83,29 @@
         <tr>
             <td>3</td>
             <td>Velocity of the average wheel contact point, in meters per
             seconds.</td>
         </tr>
     </table>
 
-    Vectorized actions have the following structure:
+    ### Rewards
 
-    <table>
-        <tr>
-            <td><strong>Index</strong></td>
-            <td><strong>Description</strong></td>
-            </tr>
-        <tr>
-            <td>``0``</td>
-            <td>Ground velocity in [m] / [s].</td>
-        </tr>
-    </table>
+    The reward function is defined in @ref envs.standing_reward.StandingReward
+    "StandingReward". See also @ref envs.upkie_base_env.UpkieBaseEnv
+    "UpkieBaseEnv" for notes on using this environment.
+
+    ### Attributes
 
-    The environment has the following attributes:
+    The environment class defines the following attributes:
 
     - ``fall_pitch``: Fall pitch angle, in radians.
     - ``max_ground_velocity``: Maximum commanded ground velocity in m/s.
     - ``version``: Environment version number.
     - ``wheel_radius``: Wheel radius in [m].
 
-    The reward function is defined in @ref envs.standing_reward.StandingReward
-    "StandingReward". See also @ref envs.upkie_base_env.UpkieBaseEnv
-    "UpkieBaseEnv" for notes on using this environment.
     """
 
     fall_pitch: float
     max_ground_velocity: float
     version: int = 4
     wheel_radius: float
 
@@ -109,65 +113,67 @@
         f"{side}_{joint}"
         for side in ("left", "right")
         for joint in ("hip", "knee")
     ]
 
     def __init__(
         self,
-        config: Optional[dict] = None,
         fall_pitch: float = 1.0,
         frequency: float = 200.0,
         max_ground_velocity: float = 1.0,
         shm_name: str = "/vulp",
+        spine_config: Optional[dict] = None,
         wheel_radius: float = 0.06,
     ):
         """!
         Initialize environment.
 
-        @param config Configuration dictionary, also sent to the spine.
         @param fall_pitch Fall pitch angle, in radians.
         @param frequency Regulated frequency of the control loop, in Hz.
         @param max_ground_velocity Maximum commanded ground velocity in m/s.
         @param shm_name Name of shared-memory file.
+        @param spine_config Additional spine configuration overriding the
+            defaults from ``//config:spine.yaml``. The combined configuration
+            dictionary is sent to the spine at every :func:`reset`.
         @param wheel_radius Wheel radius in [m].
         """
         super().__init__(
-            config=config,
             fall_pitch=fall_pitch,
             frequency=frequency,
             shm_name=shm_name,
+            spine_config=spine_config,
         )
 
         observation_limit = np.array(
             [
                 MAX_BASE_PITCH,
                 MAX_GROUND_POSITION,
                 MAX_BASE_ANGULAR_VELOCITY,
                 max_ground_velocity,
             ],
             dtype=np.float32,
         )
 
-        # gym.Env: action_space
+        # gymnasium.Env: action_space
         self.action_space = spaces.Box(
             -np.float32(max_ground_velocity),
             +np.float32(max_ground_velocity),
             shape=(1,),
             dtype=np.float32,
         )
 
-        # gym.Env: observation_space
+        # gymnasium.Env: observation_space
         self.observation_space = spaces.Box(
             -observation_limit,
             +observation_limit,
             shape=(4,),
             dtype=np.float32,
         )
 
-        # gym.Env: reward_range
+        # gymnasium.Env: reward_range
         self.reward_range = StandingReward.get_range()
 
         # Class members
         self.fall_pitch = fall_pitch
         self.init_position = {}
         self.max_ground_velocity = max_ground_velocity
         self.reward = StandingReward()
```

### Comparing `upkie-1.2.1/upkie/observers/base_pitch/__init__.py` & `upkie-1.3.0/upkie/observers/base_pitch/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/observers/base_pitch/base_pitch.py` & `upkie-1.3.0/upkie/observers/base_pitch/base_pitch.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/observers/base_pitch/tests/base_pitch_test.py` & `upkie-1.3.0/upkie/observers/base_pitch/tests/base_pitch_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/BUILD` & `upkie-1.3.0/upkie/utils/BUILD`

 * *Files 7% similar despite different names*

```diff
@@ -43,16 +43,19 @@
 
 py_library(
     name = "pinocchio",
     srcs = ["pinocchio.py"],
 )
 
 py_library(
-    name = "realtime",
-    srcs = ["realtime.py"],
+    name = "raspi",
+    srcs = ["raspi.py"],
+    deps = [
+        ":spdlog",
+    ],
 )
 
 py_library(
     name = "rotations",
     srcs = ["rotations.py"],
 )
 
@@ -64,14 +67,14 @@
 py_library(
     name = "python",
     deps = [
         ":clamp",
         ":exceptions",
         ":filters",
         ":pinocchio",
-        ":realtime",
+        ":raspi",
         ":rotations",
         ":spdlog",
     ],
 )
 
 add_lint_tests()
```

### Comparing `upkie-1.2.1/upkie/utils/clamp.py` & `upkie-1.3.0/upkie/utils/clamp.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/datetime_now_string.h` & `upkie-1.3.0/upkie/utils/datetime_now_string.h`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/exceptions.py` & `upkie-1.3.0/upkie/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/filters.py` & `upkie-1.3.0/upkie/utils/filters.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/pinocchio.py` & `upkie-1.3.0/upkie/utils/pinocchio.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/rotations.py` & `upkie-1.3.0/upkie/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/spdlog.py` & `upkie-1.3.0/upkie/utils/spdlog.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/tests/BUILD` & `upkie-1.3.0/upkie/utils/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/tests/clamp_test.py` & `upkie-1.3.0/upkie/utils/tests/clamp_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/tests/datetime_now_string_test.cpp` & `upkie-1.3.0/upkie/utils/tests/datetime_now_string_test.cpp`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/upkie/utils/tests/pinocchio_test.py` & `upkie-1.3.0/upkie/utils/tests/pinocchio_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.2.1/PKG-INFO` & `upkie-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upkie
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python module to control Upkie wheeled bipeds.
 Keywords: wheeled,biped,robot,balance,motion,control,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -16,35 +16,34 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: gymnasium >=0.28.1
-Requires-Dist: loop-rate-limiters >=0.4.0
+Requires-Dist: loop-rate-limiters >=0.5.0
 Requires-Dist: mpacklog >=3.0.0
 Requires-Dist: numpy >=1.22.0
-Requires-Dist: upkie_description >=1.2.0
-Requires-Dist: vulp >=1.2.1
+Requires-Dist: upkie_description >=1.4.0
+Requires-Dist: vulp >=1.3.0
 Project-URL: Changelog, https://github.com/tasts-robots/upkie/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://tasts-robots.org/doc/upkie/
 Project-URL: Source, https://github.com/tasts-robots/upkie
 Project-URL: Tracker, https://github.com/tasts-robots/upkie/issues
 
-# Upkie wheeled biped
+# Upkie wheeled biped robot
 
-[![Build instructions](https://img.shields.io/badge/build-instructions-brightgreen?logo=read-the-docs&style=flat)](https://github.com/tasts-robots/upkie/wiki)
 [![CI](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml/badge.svg)](https://github.com/tasts-robots/upkie/actions/workflows/bazel.yml)
+[![Build instructions](https://img.shields.io/badge/build-instructions-brightgreen?logo=read-the-docs&style=flat)](https://github.com/tasts-robots/upkie/wiki)
+[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/upkie/)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/upkie/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/upkie?branch=main)
-[![Vulp](https://img.shields.io/badge/%F0%9F%A6%8A%20vulp-1.2.0-orange)](https://github.com/tasts-robots/vulp)
-[![Chat](https://img.shields.io/matrix/tasts-robots:matrix.org?color=4EB899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
-
-Build and control **Upkie** wheeled bipeds. Made for Linux 🐧
+[![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
+[![Chat](https://img.shields.io/badge/matrix-chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
-Questions about building and using an Upkie, or balancing robots in general, are all welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://app.element.io/#/room/#tasts-robots:matrix.org).
+Build instructions and software for **Upkie** wheeled bipeds. Develop on Linux 🐧 or macOS 🍏, deploy to the robot's Raspberry Pi 🍓. Questions about building and using an Upkie, or balancing robots in general, are welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://app.element.io/#/room/#tasts-robots:matrix.org).
 
 ## Quick sim
 
 If you have Python and a C++ compiler (Ubuntu: ``sudo apt install curl g++ python3-dev``), you can run an Upkie simulation right from the command line. It won't install anything on your machine, everything will run locally from the repository:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
@@ -93,31 +92,29 @@
 
 ## Running an agent
 
 There are two ways we can develop and run agents: using the [PyPI](#pypi) distribution, or [Bazel](#bazel). PyPI is better to get started and prototype everything in Python, while Bazel is better to recompile things from source.
 
 ### PyPI
 
-[![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
-[![PyPI downloads](https://pepy.tech/badge/upkie/month)](https://pepy.tech/project/upkie)
 
 The PyPI distribution is the recommended way to control Upkie in Python. It is already [fast enough](https://github.com/tasts-robots/vulp#performance) for real-time control.
 
 #### Installation
 
 ```console
 pip install upkie
 ```
 
 #### Example
 
 While [running a spine](#running-a-spine), you can execute the following code in a Python interpreter or as a standalone Python script:
 
 ```python
-import gym
+import gymnasium as gym
 import upkie.envs
 
 upkie.envs.register()
 
 with gym.make("UpkieWheelsEnv-v4", frequency=200.0) as env:
     observation = env.reset()
     action = 0.0 * env.action_space.sample()
```

