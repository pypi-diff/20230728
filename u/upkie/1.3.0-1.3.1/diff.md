# Comparing `tmp/upkie-1.3.0.tar.gz` & `tmp/upkie-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkie-1.3.0.tar", last modified: Fri Jul 28 12:47:19 2023, max compression
+gzip compressed data, was "upkie-1.3.1.tar", last modified: Fri Jul 28 17:56:55 2023, max compression
```

## Comparing `upkie-1.3.0.tar` & `upkie-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     8460 2023-07-28 12:47:19.327366 upkie-1.3.0/README.md
--rw-r--r--   0        0        0     1890 2023-07-28 12:47:19.323366 upkie-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      695 2023-07-28 12:47:19.327366 upkie-1.3.0/upkie/__init__.py
--rw-r--r--   0        0        0     1079 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/BUILD
--rw-r--r--   0        0        0     1275 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/__init__.py
--rw-r--r--   0        0        0     2809 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/standing_reward.py
--rw-r--r--   0        0        0      549 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/BUILD
--rw-r--r--   0        0        0     2555 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/upkie_base_env_test.py
--rw-r--r--   0        0        0     2465 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/upkie_servos_env_test.py
--rw-r--r--   0        0        0     2349 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/tests/upkie_wheels_env_test.py
--rw-r--r--   0        0        0     9299 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/upkie_base_env.py
--rw-r--r--   0        0        0     7657 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/upkie_servos_env.py
--rw-r--r--   0        0        0     7387 2023-07-28 12:47:19.299365 upkie-1.3.0/upkie/envs/upkie_wheels_env.py
--rw-r--r--   0        0        0      356 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/BUILD
--rw-r--r--   0        0        0      902 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/__init__.py
--rw-r--r--   0        0        0     5612 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/base_pitch.py
--rw-r--r--   0        0        0      305 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/tests/BUILD
--rw-r--r--   0        0        0     3105 2023-07-28 12:47:19.311365 upkie-1.3.0/upkie/observers/base_pitch/tests/base_pitch_test.py
--rw-r--r--   0        0        0     1201 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/BUILD
--rw-r--r--   0        0        0     1896 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/clamp.py
--rw-r--r--   0        0        0     1137 2023-07-28 12:47:19.323366 upkie-1.3.0/upkie/utils/datetime_now_string.h
--rw-r--r--   0        0        0      803 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/exceptions.py
--rw-r--r--   0        0        0     2820 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/filters.py
--rw-r--r--   0        0        0     2433 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/pinocchio.py
--rw-r--r--   0        0        0     1430 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/raspi.py
--rw-r--r--   0        0        0     1900 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/rotations.py
--rw-r--r--   0        0        0     1983 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/spdlog.py
--rw-r--r--   0        0        0      634 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/BUILD
--rw-r--r--   0        0        0     1303 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/clamp_test.py
--rw-r--r--   0        0        0      986 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/datetime_now_string_test.cpp
--rw-r--r--   0        0        0     2232 2023-07-28 12:47:19.319366 upkie-1.3.0/upkie/utils/tests/pinocchio_test.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 upkie-1.3.0/setup.py
--rw-r--r--   0        0        0     9894 1970-01-01 00:00:00.000000 upkie-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     8557 2023-07-28 17:56:55.319436 upkie-1.3.1/README.md
+-rw-r--r--   0        0        0     1942 2023-07-28 17:56:55.315436 upkie-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-07-28 17:56:55.315436 upkie-1.3.1/upkie/__init__.py
+-rw-r--r--   0        0        0     1079 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/BUILD
+-rw-r--r--   0        0        0     1275 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/__init__.py
+-rw-r--r--   0        0        0     2809 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/standing_reward.py
+-rw-r--r--   0        0        0      549 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/tests/BUILD
+-rw-r--r--   0        0        0     2555 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/tests/upkie_base_env_test.py
+-rw-r--r--   0        0        0     2465 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/tests/upkie_servos_env_test.py
+-rw-r--r--   0        0        0     2349 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/tests/upkie_wheels_env_test.py
+-rw-r--r--   0        0        0     9575 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/upkie_base_env.py
+-rw-r--r--   0        0        0     7657 2023-07-28 17:56:55.291436 upkie-1.3.1/upkie/envs/upkie_servos_env.py
+-rw-r--r--   0        0        0     7387 2023-07-28 17:56:55.287436 upkie-1.3.1/upkie/envs/upkie_wheels_env.py
+-rw-r--r--   0        0        0      356 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/BUILD
+-rw-r--r--   0        0        0      902 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/__init__.py
+-rw-r--r--   0        0        0     5612 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/base_pitch.py
+-rw-r--r--   0        0        0      305 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/tests/BUILD
+-rw-r--r--   0        0        0     3105 2023-07-28 17:56:55.299436 upkie-1.3.1/upkie/observers/base_pitch/tests/base_pitch_test.py
+-rw-r--r--   0        0        0     1201 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/BUILD
+-rw-r--r--   0        0        0     1896 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/clamp.py
+-rw-r--r--   0        0        0     1137 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/datetime_now_string.h
+-rw-r--r--   0        0        0      803 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/exceptions.py
+-rw-r--r--   0        0        0     2815 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/filters.py
+-rw-r--r--   0        0        0     2433 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/pinocchio.py
+-rw-r--r--   0        0        0     1430 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/raspi.py
+-rw-r--r--   0        0        0     1900 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/rotations.py
+-rw-r--r--   0        0        0     1983 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/spdlog.py
+-rw-r--r--   0        0        0      634 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/BUILD
+-rw-r--r--   0        0        0     1303 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/clamp_test.py
+-rw-r--r--   0        0        0      986 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/datetime_now_string_test.cpp
+-rw-r--r--   0        0        0     2232 2023-07-28 17:56:55.311436 upkie-1.3.1/upkie/utils/tests/pinocchio_test.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 upkie-1.3.1/setup.py
+-rw-r--r--   0        0        0     9991 1970-01-01 00:00:00.000000 upkie-1.3.1/PKG-INFO
```

### Comparing `upkie-1.3.0/README.md` & `upkie-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
 [![Chat](https://img.shields.io/badge/matrix-chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
 Build instructions and software for **Upkie** wheeled bipeds. Develop on Linux 🐧 or macOS 🍏, deploy to the robot's Raspberry Pi 🍓. Questions about building and using an Upkie, or balancing robots in general, are welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://app.element.io/#/room/#tasts-robots:matrix.org).
 
 ## Quick sim
 
-If you have Python and a C++ compiler (Ubuntu: ``sudo apt install curl g++ python3-dev``), you can run an Upkie simulation right from the command line. It won't install anything on your machine, everything will run locally from the repository:
+If you have Python and a C++ compiler (setup one-liners: [Fedora](https://github.com/tasts-robots/upkie/discussions/100), [Ubuntu](https://github.com/tasts-robots/upkie/discussions/101)), you can run an Upkie simulation right from the command line. It won't install anything on your machine, everything will run locally from the repository:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
 ```console
 git clone https://github.com/tasts-robots/upkie.git
 cd upkie
 ./start_wheel_balancer.sh
```

### Comparing `upkie-1.3.0/pyproject.toml` & `upkie-1.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 Documentation = "https://tasts-robots.org/doc/upkie/"
 Source = "https://github.com/tasts-robots/upkie"
 Tracker = "https://github.com/tasts-robots/upkie/issues"
 Changelog = "https://github.com/tasts-robots/upkie/blob/main/CHANGELOG.md"
 
 [tool.flit.sdist]
 include = [
+    "upkie/config/*.py",
+    "upkie/config/*.yaml",
     "upkie/envs/*.py",
     "upkie/observers/base_pitch/*.py",
     "upkie/utils/*.py",
 ]
 
 [tool.ruff]
 line-length = 79
```

### Comparing `upkie-1.3.0/upkie/__init__.py` & `upkie-1.3.1/upkie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python module to control Upkie wheeled bipeds."""
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
```

### Comparing `upkie-1.3.0/upkie/envs/BUILD` & `upkie-1.3.1/upkie/envs/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/__init__.py` & `upkie-1.3.1/upkie/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/standing_reward.py` & `upkie-1.3.1/upkie/envs/standing_reward.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/tests/BUILD` & `upkie-1.3.1/upkie/envs/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/tests/upkie_base_env_test.py` & `upkie-1.3.1/upkie/envs/tests/upkie_base_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/tests/upkie_servos_env_test.py` & `upkie-1.3.1/upkie/envs/tests/upkie_servos_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/tests/upkie_wheels_env_test.py` & `upkie-1.3.1/upkie/envs/tests/upkie_wheels_env_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/upkie_base_env.py` & `upkie-1.3.1/upkie/envs/upkie_base_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,22 @@
             merged_spine_config.update(spine_config)
         self.__frequency = frequency
         self._spine = SpineInterface(shm_name)
         self.fall_pitch = fall_pitch
         self.spine_config = merged_spine_config
 
     @property
+    def dt(self) -> Optional[float]:
+        """!
+        Regulated period of the control loop in seconds, or ``None`` if there
+        is no loop frequency regulation.
+        """
+        return 1.0 / self.__frequency if self.__frequency is not None else None
+
+    @property
     def frequency(self) -> Optional[float]:
         """!
         Regulated frequency of the control loop in Hz, or ``None`` if there is
         no loop frequency regulation.
         """
         return self.__frequency
```

### Comparing `upkie-1.3.0/upkie/envs/upkie_servos_env.py` & `upkie-1.3.1/upkie/envs/upkie_servos_env.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/envs/upkie_wheels_env.py` & `upkie-1.3.1/upkie/envs/upkie_wheels_env.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/observers/base_pitch/__init__.py` & `upkie-1.3.1/upkie/observers/base_pitch/__init__.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/observers/base_pitch/base_pitch.py` & `upkie-1.3.1/upkie/observers/base_pitch/base_pitch.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/observers/base_pitch/tests/base_pitch_test.py` & `upkie-1.3.1/upkie/observers/base_pitch/tests/base_pitch_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/BUILD` & `upkie-1.3.1/upkie/utils/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/clamp.py` & `upkie-1.3.1/upkie/utils/clamp.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/datetime_now_string.h` & `upkie-1.3.1/upkie/utils/datetime_now_string.h`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/exceptions.py` & `upkie-1.3.1/upkie/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/filters.py` & `upkie-1.3.1/upkie/utils/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Tuple
 
-from utils.clamp import clamp
+from .clamp import clamp
 
 
 def abs_bounded_derivative_filter(
     prev_output: float,
     new_input: float,
     dt: float,
     max_output: float,
```

### Comparing `upkie-1.3.0/upkie/utils/pinocchio.py` & `upkie-1.3.1/upkie/utils/pinocchio.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/raspi.py` & `upkie-1.3.1/upkie/utils/raspi.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/rotations.py` & `upkie-1.3.1/upkie/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/spdlog.py` & `upkie-1.3.1/upkie/utils/spdlog.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/tests/BUILD` & `upkie-1.3.1/upkie/utils/tests/BUILD`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/tests/clamp_test.py` & `upkie-1.3.1/upkie/utils/tests/clamp_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/tests/datetime_now_string_test.cpp` & `upkie-1.3.1/upkie/utils/tests/datetime_now_string_test.cpp`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/upkie/utils/tests/pinocchio_test.py` & `upkie-1.3.1/upkie/utils/tests/pinocchio_test.py`

 * *Files identical despite different names*

### Comparing `upkie-1.3.0/setup.py` & `upkie-1.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'loop-rate-limiters >=0.5.0',
  'mpacklog >=3.0.0',
  'numpy >=1.22.0',
  'upkie_description >=1.4.0',
  'vulp >=1.3.0']
 
 setup(name='upkie',
-      version='1.3.0',
+      version='1.3.1',
       description='Python module to control Upkie wheeled bipeds.',
       author=None,
       author_email='Stéphane Caron <stephane.caron@normalesup.org>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `upkie-1.3.0/PKG-INFO` & `upkie-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upkie
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python module to control Upkie wheeled bipeds.
 Keywords: wheeled,biped,robot,balance,motion,control,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -39,15 +39,15 @@
 [![PyPI version](https://img.shields.io/pypi/v/upkie)](https://pypi.org/project/upkie/)
 [![Chat](https://img.shields.io/badge/matrix-chat-%234eb899)](https://app.element.io/#/room/#tasts-robots:matrix.org)
 
 Build instructions and software for **Upkie** wheeled bipeds. Develop on Linux 🐧 or macOS 🍏, deploy to the robot's Raspberry Pi 🍓. Questions about building and using an Upkie, or balancing robots in general, are welcome in the [Discussions](https://github.com/tasts-robots/upkie/discussions) forum or on the [Chat](https://app.element.io/#/room/#tasts-robots:matrix.org).
 
 ## Quick sim
 
-If you have Python and a C++ compiler (Ubuntu: ``sudo apt install curl g++ python3-dev``), you can run an Upkie simulation right from the command line. It won't install anything on your machine, everything will run locally from the repository:
+If you have Python and a C++ compiler (setup one-liners: [Fedora](https://github.com/tasts-robots/upkie/discussions/100), [Ubuntu](https://github.com/tasts-robots/upkie/discussions/101)), you can run an Upkie simulation right from the command line. It won't install anything on your machine, everything will run locally from the repository:
 
 <img src="https://user-images.githubusercontent.com/1189580/170496331-e1293dd3-b50c-40ee-9c2e-f75f3096ebd8.png" height="100" align="right" />
 
 ```console
 git clone https://github.com/tasts-robots/upkie.git
 cd upkie
 ./start_wheel_balancer.sh
```

