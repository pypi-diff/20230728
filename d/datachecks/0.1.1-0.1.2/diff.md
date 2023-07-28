# Comparing `tmp/datachecks-0.1.1.tar.gz` & `tmp/datachecks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachecks-0.1.1.tar", max compression
+gzip compressed data, was "datachecks-0.1.2.tar", max compression
```

## Comparing `datachecks-0.1.1.tar` & `datachecks-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-02-01 07:00:49.705688 datachecks-0.1.1/LICENSE
--rw-r--r--   0        0        0     1879 2023-07-20 07:28:51.188886 datachecks-0.1.1/README.md
--rw-r--r--   0        0        0      745 2023-07-20 05:27:54.101170 datachecks-0.1.1/datachecks/__init__.py
--rw-r--r--   0        0        0      686 2023-07-19 07:09:54.139125 datachecks-0.1.1/datachecks/__main__.py
--rw-r--r--   0        0        0      638 2023-07-19 07:09:54.134314 datachecks-0.1.1/datachecks/__version__.py
--rw-r--r--   0        0        0        0 2023-07-16 02:22:59.418174 datachecks-0.1.1/datachecks/cli/__init__.py
--rw-r--r--   0        0        0     2155 2023-07-20 05:28:58.116256 datachecks-0.1.1/datachecks/cli/cli.py
--rw-r--r--   0        0        0      609 2023-07-19 07:39:16.267604 datachecks-0.1.1/datachecks/core/__init__.py
--rw-r--r--   0        0        0      610 2023-07-19 07:39:16.259157 datachecks-0.1.1/datachecks/core/configuration/__init__.py
--rw-r--r--   0        0        0     3647 2023-07-20 05:37:22.865117 datachecks-0.1.1/datachecks/core/configuration/configuration.py
--rw-r--r--   0        0        0      609 2023-07-19 07:39:16.270686 datachecks-0.1.1/datachecks/core/datasource/__init__.py
--rw-r--r--   0        0        0     7185 2023-07-20 06:18:52.504652 datachecks-0.1.1/datachecks/core/datasource/data_source.py
--rw-r--r--   0        0        0     1448 2023-07-20 05:27:34.269872 datachecks-0.1.1/datachecks/core/inspect.py
--rw-r--r--   0        0        0      609 2023-07-19 07:39:16.269311 datachecks-0.1.1/datachecks/core/metric/__init__.py
--rw-r--r--   0        0        0     7857 2023-07-20 05:27:47.684168 datachecks-0.1.1/datachecks/core/metric/metric.py
--rw-r--r--   0        0        0     1270 2023-07-20 08:38:51.144156 datachecks-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3358 1970-01-01 00:00:00.000000 datachecks-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-01 07:00:49.705688 datachecks-0.1.2/LICENSE
+-rw-r--r--   0        0        0    10378 2023-07-28 16:17:59.134602 datachecks-0.1.2/README.md
+-rw-r--r--   0        0        0      804 2023-07-22 12:00:19.433096 datachecks-0.1.2/datachecks/__init__.py
+-rw-r--r--   0        0        0      685 2023-07-22 12:00:19.433406 datachecks-0.1.2/datachecks/__main__.py
+-rw-r--r--   0        0        0      633 2023-07-28 16:23:34.072452 datachecks-0.1.2/datachecks/__version__.py
+-rw-r--r--   0        0        0      610 2023-07-22 12:00:19.433765 datachecks-0.1.2/datachecks/cli/__init__.py
+-rw-r--r--   0        0        0     2103 2023-07-28 16:17:59.135065 datachecks-0.1.2/datachecks/cli/cli.py
+-rw-r--r--   0        0        0      610 2023-07-22 12:00:19.434223 datachecks-0.1.2/datachecks/core/__init__.py
+-rw-r--r--   0        0        0      610 2023-07-19 07:39:16.259157 datachecks-0.1.2/datachecks/core/configuration/__init__.py
+-rw-r--r--   0        0        0     5162 2023-07-24 15:06:59.173560 datachecks-0.1.2/datachecks/core/configuration/config_loader.py
+-rw-r--r--   0        0        0     4429 2023-07-28 16:17:59.136601 datachecks-0.1.2/datachecks/core/configuration/configuration.py
+-rw-r--r--   0        0        0      610 2023-07-22 12:00:19.434677 datachecks-0.1.2/datachecks/core/datasource/__init__.py
+-rw-r--r--   0        0        0     4854 2023-07-24 15:06:59.174230 datachecks-0.1.2/datachecks/core/datasource/base.py
+-rw-r--r--   0        0        0     3020 2023-07-23 20:49:33.475381 datachecks-0.1.2/datachecks/core/datasource/manager.py
+-rw-r--r--   0        0        0     3389 2023-07-23 20:49:33.475728 datachecks-0.1.2/datachecks/core/datasource/opensearch.py
+-rw-r--r--   0        0        0     1484 2023-07-22 12:00:19.436116 datachecks-0.1.2/datachecks/core/datasource/postgres.py
+-rw-r--r--   0        0        0     2055 2023-07-28 16:17:59.137828 datachecks-0.1.2/datachecks/core/inspect.py
+-rw-r--r--   0        0        0        0 2023-07-28 16:17:59.137928 datachecks-0.1.2/datachecks/core/logger/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-28 16:17:59.138398 datachecks-0.1.2/datachecks/core/logger/base.py
+-rw-r--r--   0        0        0     3526 2023-07-28 16:17:59.138679 datachecks-0.1.2/datachecks/core/logger/default_logger.py
+-rw-r--r--   0        0        0      610 2023-07-22 12:00:19.436682 datachecks-0.1.2/datachecks/core/metric/__init__.py
+-rw-r--r--   0        0        0     5528 2023-07-28 16:17:59.139073 datachecks-0.1.2/datachecks/core/metric/base.py
+-rw-r--r--   0        0        0     1856 2023-07-24 15:06:59.174945 datachecks-0.1.2/datachecks/core/metric/freshness_metric.py
+-rw-r--r--   0        0        0     5133 2023-07-28 16:17:59.139385 datachecks-0.1.2/datachecks/core/metric/manager.py
+-rw-r--r--   0        0        0     3849 2023-07-23 20:49:33.476790 datachecks-0.1.2/datachecks/core/metric/numeric_metric.py
+-rw-r--r--   0        0        0     1504 2023-07-28 16:23:34.073020 datachecks-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11980 1970-01-01 00:00:00.000000 datachecks-0.1.2/PKG-INFO
```

### Comparing `datachecks-0.1.1/LICENSE` & `datachecks-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datachecks-0.1.1/datachecks/__init__.py` & `datachecks-0.1.2/datachecks/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from datachecks.core.configuration.configuration import (Configuration,
+                                                         load_configuration)
 from datachecks.core.inspect import Inspect
-from datachecks.core.configuration.configuration import Configuration, load_configuration
```

### Comparing `datachecks-0.1.1/datachecks/__main__.py` & `datachecks-0.1.2/datachecks/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,10 +9,9 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from datachecks.cli.cli import main
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `datachecks-0.1.1/datachecks/__version__.py` & `datachecks-0.1.2/datachecks/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.1.0-beta"
+__version__ = "0.1.2"
```

### Comparing `datachecks-0.1.1/datachecks/core/__init__.py` & `datachecks-0.1.2/datachecks/cli/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
-#  limitations under the License.
+#  limitations under the License.
```

### Comparing `datachecks-0.1.1/datachecks/core/configuration/__init__.py` & `datachecks-0.1.2/datachecks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `datachecks-0.1.1/datachecks/core/datasource/__init__.py` & `datachecks-0.1.2/datachecks/core/configuration/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
-#  limitations under the License.
+#  limitations under the License.
```

### Comparing `datachecks-0.1.1/datachecks/core/inspect.py` & `datachecks-0.1.2/datachecks/core/inspect.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,47 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import List, Dict
+from typing import Dict, List
+
+import requests
 
 from datachecks.core.configuration.configuration import Configuration
-from datachecks.core.datasource.data_source import DataSourceManager
-from datachecks.core.metric.metric import MetricManager
+from datachecks.core.datasource.manager import DataSourceManager
+from datachecks.core.logger.default_logger import DefaultLogger
+from datachecks.core.metric.manager import MetricManager
 
+requests.packages.urllib3.disable_warnings(
+    requests.packages.urllib3.exceptions.InsecureRequestWarning
+)
 
-class Inspect:
 
+class Inspect:
     def __init__(self, configuration: Configuration):
         self.configuration = configuration
         self.data_source_manager = DataSourceManager(configuration.data_sources)
+
+        self.metric_logger = None
+
+        if self.configuration.metric_logger:
+            if self.configuration.metric_logger.type == "default":
+                self.metric_logger = DefaultLogger(
+                    **self.configuration.metric_logger.config
+                    if self.configuration.metric_logger.config
+                    else {}
+                )
+
         self.metric_manager = MetricManager(
             metric_config=configuration.metrics,
-            data_source_manager=self.data_source_manager
+            data_source_manager=self.data_source_manager,
+            metric_logger=self.metric_logger,
         )
 
     def start(self):
         metric_values: List[Dict] = []
         for metric_name, metric in self.metric_manager.metrics.items():
             metric_value = metric.get_value()
             metric_values.append(metric_value)
```

### Comparing `datachecks-0.1.1/datachecks/core/metric/__init__.py` & `datachecks-0.1.2/datachecks/core/datasource/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
-#  limitations under the License.
+#  limitations under the License.
```

### Comparing `datachecks-0.1.1/pyproject.toml` & `datachecks-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datachecks"
-version = "0.1.1"
+version = "0.1.2"
 description = "Open Source Data Quality Monitoring"
 license = "Apache-2.0"
 authors = [
     "Waterdip Labs <hello@waterdip.ai>"
 ]
 repository = "https://github.com/waterdipai/datachecks"
 readme = "README.md"
@@ -22,22 +22,32 @@
 ]
 packages = [{ include = "datachecks" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 click = "^8.1.5"
 pyyaml = "^6.0"
+requests = "^2.31.0"
 opensearch-py = { version="^2.2.0", optional=true }
 sqlalchemy = { version="^2.0.19", optional=true }
 psycopg2 = { version="^2.9.6", optional=true }
+python-dateutil = "^2.8.2"
+loguru = "^0.7.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.1.3"
+pytest-docker = "^2.0.0"
+pytest-mock = "^3.10.0"
+mongomock = "^4.1.2"
+pre-commit = "^2.20.0"
+pytest-cov = "^4.0.0"
 
 [tool.poetry.extras]
 # When adding, update also: README + dev deps just above
-postgresql = ["psycopg2", "sqlalchemy"]
+postgres = ["psycopg2", "sqlalchemy"]
 opensearch = ["opensearch-py"]
 
 [tool.poetry.scripts]
 datachecks = "datachecks.cli.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
```

