# Comparing `tmp/pytest-elasticsearch-3.0.0.tar.gz` & `tmp/pytest-elasticsearch-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-elasticsearch-3.0.0.tar", last modified: Tue Mar  1 10:22:04 2022, max compression
+gzip compressed data, was "pytest-elasticsearch-4.0.0.tar", last modified: Fri Jul 28 19:11:33 2023, max compression
```

## Comparing `pytest-elasticsearch-3.0.0.tar` & `pytest-elasticsearch-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:22:04.750848 pytest-elasticsearch-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35146 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7650 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9496 2022-03-01 10:22:04.750848 pytest-elasticsearch-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5272 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-03-01 10:22:04.754848 pytest-elasticsearch-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:22:04.750848 pytest-elasticsearch-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:22:04.750848 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6278 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-03-01 10:21:58.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:22:04.750848 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9496 2022-03-01 10:22:04.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-03-01 10:22:04.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 10:22:04.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-03-01 10:22:04.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 10:22:03.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-03-01 10:22:04.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-01 10:22:04.000000 pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/pytest_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:23.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:11:33.000000 pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:11:33.835611 pytest-elasticsearch-4.0.0/setup.cfg
```

### Comparing `pytest-elasticsearch-3.0.0/CONTRIBUTING.rst` & `pytest-elasticsearch-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

```diff
@@ -1,9 +1,9 @@
 Contribute to pytest-elasticsearch
-==============
+==================================
 
 Thank you for taking time to contribute to pytest-elasticsearch!
 
 The following is a set of guidelines for contributing to pytest-elasticsearch. These are just guidelines, not rules, use your best judgment and feel free to propose changes to this document in a pull request.
 
 Bug Reports
 -----------
```

### Comparing `pytest-elasticsearch-3.0.0/COPYING` & `pytest-elasticsearch-4.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-3.0.0/COPYING.lesser` & `pytest-elasticsearch-4.0.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-elasticsearch-3.0.0/README.rst` & `pytest-elasticsearch-4.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 It allows you to specify fixtures for Elasticsearch process and client.
 
 How to use
 ==========
 
 .. warning::
 
-    This plugin requires at least version 5.0 of elasticsearch to work.
+    This plugin requires at least version 6.0 of elasticsearch to work.
 
 The plugin contains two fixtures:
 
 * **elasticsearch** - a client fixture that has functional scope, and which
   cleans Elasticsearch at the end of each test.
 * **elasticsearch_proc** - a session scoped fixture, that starts Elasticsearch
   instance at its first use and stops at the end of the tests.
@@ -104,15 +104,15 @@
      - host
      - --elasticsearch-host
      - elasticsearch_host
      - host
      - 127.0.0.1
    * - port
      - port
-     - -elasticsearch-port
+     - --elasticsearch-port
      - elasticsearch_port
      - 6300
      - random
    * - Elasticsearch cluster name
      - cluster_name
      - --elasticsearch-cluster-name
      - elasticsearch_cluster_name
```

### Comparing `pytest-elasticsearch-3.0.0/setup.py` & `pytest-elasticsearch-4.0.0/pytest_elasticsearch/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,11 +12,9 @@
 # pytest-elasticsearch is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-elasticsearch.  If not, see <http://www.gnu.org/licenses/>.
-"""Installation file for pytest-elasticsearch."""
-from setuptools import setup
-
-setup()
+"""Main packge for pytest-elasticsearch."""
+__version__ = "4.0.0"
```

### Comparing `pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/executor.py` & `pytest-elasticsearch-4.0.0/pytest_elasticsearch/executor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,126 +1,130 @@
 """Elasticsearch executor."""
 
 import re
+from pathlib import Path
 from subprocess import check_output
+from typing import Literal, Optional
 
 from mirakuru import HTTPExecutor
-from pkg_resources import parse_version
+from packaging.version import Version
 
 
 class NoopElasticsearch:  # pylint:disable=too-few-public-methods
     """No operation Elasticsearch executor mock."""
 
-    def __init__(self, host, port):
-        """
-        Initialize Elasticsearch executor mock
+    def __init__(self, host: str, port: int) -> None:
+        """Initialize Elasticsearch executor mock.
+
         :param str host: hostname under which elasticsearch is available
-        :param int port: port under which elasticsearch is available
+        :param int port: port under which elasticsearch is available.
         """
         self.host = host
         self.port = port
 
     @staticmethod
-    def running():
+    def running() -> Literal[True]:
         """Mock method pretending the executor is running."""
         return True
 
 
 # pylint:disable=too-many-instance-attributes
 class ElasticSearchExecutor(HTTPExecutor):
     """Elasticsearch executor."""
 
     def __init__(
         self,
-        executable,
-        host,
-        port,
-        tcp_port,
-        pidfile,
-        logs_path,
-        works_path,
-        cluster_name,
-        network_publish_host,
-        index_store_type,
-        timeout,
-    ):  # pylint:disable=too-many-arguments
-        """
-        Initialize ElasticSearchExecutor.
-
-        :param pathlib.Path executable: Executable path
-        :param str host: hostname under which elasticsearch will be running
-        :param int port: port elasticsearch listens on
-        :param int tcp_port: port used for unternal communication
-        :param pathlib.Path pidfile: pidfile location
-        :param pathlib.Path logs_path: log files location
-        :param pathlib.Path works_path: workdir location
-        :param str cluster_name: cluster name
-        :param str network_publish_host: network host to which elasticsearch
+        executable: Path,
+        host: str,
+        port: int,
+        tcp_port: int,
+        pidfile: Path,
+        logs_path: Path,
+        works_path: Path,
+        cluster_name: str,
+        network_publish_host: str,
+        index_store_type: str,
+        timeout: int,
+    ) -> None:  # pylint:disable=too-many-arguments
+        """Initialize ElasticSearchExecutor.
+
+        :param executable: Executable path
+        :param host: hostname under which elasticsearch will be running
+        :param port: port elasticsearch listens on
+        :param tcp_port: port used for internal communication
+        :param pidfile: pidfile location
+        :param logs_path: log files location
+        :param works_path: workdir location
+        :param cluster_name: cluster name
+        :param network_publish_host: network host to which elasticsearch
             publish to connect to cluseter'
-        :param str index_store_type: type of the index to use in the
+        :param index_store_type: type of the index to use in the
             elasticsearch process fixture
-        :param int timeout: Time after which to give up to start elasticsearch
+        :param timeout: Time after which to give up to start elasticsearch
         """
-        self._version = None
+        self._version: Optional[Version] = None
         self.executable = executable
         self.host = host
         self.port = port
+        # TODO: rename to transport_port
         self.tcp_port = tcp_port
         self.pidfile = pidfile
         self.logs_path = logs_path
         self.works_path = works_path
         self.cluster_name = cluster_name
         self.network_publish_host = network_publish_host
         self.index_store_type = index_store_type
         super().__init__(
             self._exec_command(),
             f"http://{self.host}:{self.port}",
             timeout=timeout,
         )
 
     @property
-    def version(self):
-        """
-        Get the given elasticsearch executable version parts.
+    def version(self) -> Version:
+        """Get the given elasticsearch executable version parts.
 
         :return: Elasticsearch version
-        :rtype: pkg_resources.Version
         """
         if not self._version:
             try:
                 output = check_output([self.executable, "-Vv"]).decode("utf-8")
                 match = re.search(r"Version: (?P<major>\d)\.(?P<minor>\d+)\.(?P<patch>\d+)", output)
                 if not match:
                     raise RuntimeError(
                         "Elasticsearch version is not recognized. "
                         "It is probably not supported. \n"
                         "Output is: " + output
                     )
                 version = match.groupdict()
-                self._version = parse_version(
+                self._version = Version(
                     ".".join([version["major"], version["minor"], version["patch"]])
                 )
             except OSError as exc:
                 raise RuntimeError(
                     "'%s' does not point to elasticsearch." % self.executable
                 ) from exc
         return self._version
 
-    def _exec_command(self):
-        """
-        Get command to run elasticsearch binary based on the version.
+    def _exec_command(self) -> str:
+        """Get command to run elasticsearch binary based on the version.
 
         :return: command to run elasticsearch
-        :rtype: str
         """
-        if self.version < parse_version("6.0.0"):
+        port_param = "transport.port"
+        if self.version < Version("7.0.0"):
             raise RuntimeError("This elasticsearch version is not supported.")
+        elif self.version < Version("8.0.0"):
+            port_param = "transport.tcp.port"
+        else:
+            port_param = "transport.port"
         return f"""
             {self.executable} -p {self.pidfile}
             -E http.port={self.port}
-            -E transport.tcp.port={self.tcp_port}
+            -E {port_param}={self.tcp_port}
             -E path.logs={self.logs_path}
             -E path.data={self.works_path}
             -E cluster.name={self.cluster_name}
             -E network.host='{self.network_publish_host}'
             -E index.store.type={self.index_store_type}
+            -E xpack.security.enabled=false
         """
```

### Comparing `pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/factories.py` & `pytest-elasticsearch-4.0.0/pytest_elasticsearch/factories.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,93 +13,76 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-elasticsearch.  If not, see <http://www.gnu.org/licenses/>.
 """Fixture factories."""
 import shutil
+from pathlib import Path
+from typing import Callable, Iterator, Optional
 
 import pytest
-from pytest import FixtureRequest, TempPathFactory
 from elasticsearch import Elasticsearch
 from mirakuru import ProcessExitedWithError
 from port_for import get_port
+from port_for.api import PortType
+from pytest import FixtureRequest, TempPathFactory
 
+from pytest_elasticsearch.config import get_config
 from pytest_elasticsearch.executor import ElasticSearchExecutor, NoopElasticsearch
 
 
-def return_config(request):
-    """Return a dictionary with config options."""
-    config = {}
-    options = [
-        "port",
-        "transport_tcp_port",
-        "host",
-        "cluster_name",
-        "network_publish_host",
-        "index_store_type",
-        "executable",
-    ]
-    for option in options:
-        option_name = "elasticsearch_" + option
-        conf = request.config.getoption(option_name) or request.config.getini(option_name)
-        config[option] = conf
-    return config
-
-
 def elasticsearch_proc(
-    executable=None,
-    host=None,
-    port=-1,
-    transport_tcp_port=None,
-    cluster_name=None,
-    network_publish_host=None,
-    index_store_type=None,
-):
-
-    """
-    Create elasticsearch process fixture.
-
-    .. warning::
-
-        This fixture requires at least version 1.0 of elasticsearch to work.
-
-    :param str executable: elasticsearch's executable
-    :param str host: host that the instance listens on
-    :param str|int|tuple|set|list port:
+    executable: Optional[Path] = None,
+    host: Optional[str] = None,
+    port: Optional[PortType] = -1,
+    transport_tcp_port: Optional[PortType] = None,
+    cluster_name: Optional[str] = None,
+    network_publish_host: Optional[str] = None,
+    index_store_type: Optional[str] = None,
+) -> Callable[[FixtureRequest, TempPathFactory], Iterator[ElasticSearchExecutor]]:
+    """Create elasticsearch process fixture.
+
+    :param executable: elasticsearch's executable
+    :param host: host that the instance listens on
+    :param port:
         exact port (e.g. '8000', 8000)
         randomly selected port (None) - any random available port
         [(2000,3000)] or (2000,3000) - random available port from a given range
         [{4002,4003}] or {4002,4003} - random of 4002 or 4003 ports
         [(2000,3000), {4002,4003}] -random of given range and set
-    :param str cluster_name: name of a cluser this node should work on.
+    :param transport_tcp_port: Port used for communication between nodes
+    :param cluster_name: name of a cluser this node should work on.
         Used for autodiscovery. By default each node is in it's own cluser.
-    :param str network_publish_host: host to publish itself within cluser
+    :param network_publish_host: host to publish itself within cluser
         http://www.elasticsearch.org/guide/en/elasticsearch/reference/current/modules-network.html
-    :param str index_store_type: index.store.type setting. *memory* by default
+    :param index_store_type: index.store.type setting. *memory* by default
         to speed up tests
     """
 
     @pytest.fixture(scope="session")
     def elasticsearch_proc_fixture(
         request: FixtureRequest, tmp_path_factory: TempPathFactory
-    ) -> ElasticSearchExecutor:
+    ) -> Iterator[ElasticSearchExecutor]:
         """Elasticsearch process starting fixture."""
-        config = return_config(request)
+        config = get_config(request)
         elasticsearch_host = host or config["host"]
         elasticsearch_executable = executable or config["executable"]
 
         elasticsearch_port = get_port(port) or get_port(config["port"])
-        elasticsearch_transport_port = get_port(transport_tcp_port) or get_port(
-            config["transport_tcp_port"]
-        )
+        assert elasticsearch_port
+        elasticsearch_transport_port = get_port(
+            transport_tcp_port, exclude_ports=[elasticsearch_port]
+        ) or get_port(config["transport_tcp_port"], exclude_ports=[elasticsearch_port])
+        assert elasticsearch_transport_port
 
         elasticsearch_cluster_name = (
             cluster_name or config["cluster_name"] or f"elasticsearch_cluster_{elasticsearch_port}"
         )
+        assert elasticsearch_cluster_name
         elasticsearch_index_store_type = index_store_type or config["index_store_type"]
         elasticsearch_network_publish_host = network_publish_host or config["network_publish_host"]
         tmpdir = tmp_path_factory.mktemp(f"pytest-elasticsearch-{request.fixturename}")
 
         logs_path = tmpdir / "logs"
 
         pidfile = tmpdir / f"elasticsearch.{elasticsearch_port}.pid"
@@ -114,74 +97,74 @@
             logs_path,
             work_path,
             elasticsearch_cluster_name,
             elasticsearch_network_publish_host,
             elasticsearch_index_store_type,
             timeout=60,
         )
+        print(elasticsearch_executor.command)
 
         elasticsearch_executor.start()
         yield elasticsearch_executor
         try:
             elasticsearch_executor.stop()
         except ProcessExitedWithError:
             pass
         shutil.rmtree(work_path)
         shutil.rmtree(logs_path)
 
     return elasticsearch_proc_fixture
 
 
-def elasticsearch_noproc(host=None, port=None):
-    """
-    Elasticsearch noprocess factory.
+def elasticsearch_noproc(
+    host: Optional[str] = None, port: Optional[int] = None
+) -> Callable[[FixtureRequest], Iterator[NoopElasticsearch]]:
+    """Elasticsearch noprocess factory.
 
-    :param str host: hostname
-    :param str|int port: exact port (e.g. '8000', 8000)
-    :rtype: func
+    :param host: hostname
+    :param port: exact port (e.g. '8000', 8000)
     :returns: function which makes a elasticsearch process
     """
 
     @pytest.fixture(scope="session")
-    def elasticsearch_noproc_fixture(request):
-        """
-        Noop Process fixture for PostgreSQL.
+    def elasticsearch_noproc_fixture(request: FixtureRequest) -> Iterator[NoopElasticsearch]:
+        """Noop Process fixture for PostgreSQL.
 
         :param FixtureRequest request: fixture request object
         :rtype: pytest_dbfixtures.executors.TCPExecutor
         :returns: tcp executor-like object
         """
-        config = return_config(request)
-        pg_host = host or config["host"]
-        pg_port = port or config["port"] or 9300
+        config = get_config(request)
+        es_host = host or config["host"]
+        assert es_host
+        es_port = port or config["port"] or 9300
+        assert es_port
 
-        noop_exec = NoopElasticsearch(host=pg_host, port=pg_port)
-
-        yield noop_exec
+        yield NoopElasticsearch(host=es_host, port=es_port)
 
     return elasticsearch_noproc_fixture
 
 
-def elasticsearch(process_fixture_name):
-    """
-    Create Elasticsearch client fixture.
+def elasticsearch(process_fixture_name: str) -> Callable[[FixtureRequest], Iterator[Elasticsearch]]:
+    """Create Elasticsearch client fixture.
 
-    :param str process_fixture_name: elasticsearch process fixture name
+    :param process_fixture_name: elasticsearch process fixture name
     """
 
     @pytest.fixture
-    def elasticsearch_fixture(request):
+    def elasticsearch_fixture(request: FixtureRequest) -> Iterator[Elasticsearch]:
         """Elasticsearch client fixture."""
         process = request.getfixturevalue(process_fixture_name)
         if not process.running():
             process.start()
+        client = Elasticsearch(
+            hosts=[{"host": process.host, "port": process.port, "scheme": "http"}],
+            request_timeout=30,
+            verify_certs=False,
+        )
+        client.options(ignore_status=400)
 
-        client = Elasticsearch([{"host": process.host, "port": process.port}])
-
-        def drop_indexes():
-            client.indices.delete(index="*")
-
-        request.addfinalizer(drop_indexes)
-
-        return client
+        yield client
+        for index in client.indices.get_alias():
+            client.indices.delete(index=index)
 
     return elasticsearch_fixture
```

### Comparing `pytest-elasticsearch-3.0.0/src/pytest_elasticsearch/plugin.py` & `pytest-elasticsearch-4.0.0/pytest_elasticsearch/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-elasticsearch.  If not, see <http://www.gnu.org/licenses/>.
 """Pytest-elasticsearch py.test's plugin configuration."""
+from pytest import Parser
 
 from pytest_elasticsearch import factories
 
 # pylint:disable=invalid-name
 _help_host = "Elasticsearch host"
 _help_executable = "Elasticsearch executable"
 _help_port = "Elasticsearch port"
 _help_cluster_name = "Cluster name of the elasticsearch process fixture"
 _help_index_store_type = "type of the index to use in the elasticsearch process fixture"
 _help_network_publish_host = "network host to which elasticsearch publish to connect to cluseter"
 _help_elasticsearch_transport_tcp_port = "The tcp ansport port used \
     for internal communication between nodes within the cluster"
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: Parser) -> None:
     """Add plugin's configuration options."""
-
     parser.addini(name="elasticsearch_host", help=_help_host, default="127.0.0.1")
 
     parser.addini(
         name="elasticsearch_executable",
         help=_help_executable,
         default="/usr/share/elasticsearch/bin/elasticsearch",
     )
```

### Comparing `pytest-elasticsearch-3.0.0/src/pytest_elasticsearch.egg-info/SOURCES.txt` & `pytest-elasticsearch-4.0.0/pytest_elasticsearch.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 CHANGES.rst
 CONTRIBUTING.rst
 COPYING
 COPYING.lesser
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
-src/pytest_elasticsearch/__init__.py
-src/pytest_elasticsearch/executor.py
-src/pytest_elasticsearch/factories.py
-src/pytest_elasticsearch/plugin.py
-src/pytest_elasticsearch.egg-info/PKG-INFO
-src/pytest_elasticsearch.egg-info/SOURCES.txt
-src/pytest_elasticsearch.egg-info/dependency_links.txt
-src/pytest_elasticsearch.egg-info/entry_points.txt
-src/pytest_elasticsearch.egg-info/not-zip-safe
-src/pytest_elasticsearch.egg-info/requires.txt
-src/pytest_elasticsearch.egg-info/top_level.txt
+pytest_elasticsearch/__init__.py
+pytest_elasticsearch/config.py
+pytest_elasticsearch/executor.py
+pytest_elasticsearch/factories.py
+pytest_elasticsearch/plugin.py
+pytest_elasticsearch/py.typed
+pytest_elasticsearch.egg-info/PKG-INFO
+pytest_elasticsearch.egg-info/SOURCES.txt
+pytest_elasticsearch.egg-info/dependency_links.txt
+pytest_elasticsearch.egg-info/entry_points.txt
+pytest_elasticsearch.egg-info/requires.txt
+pytest_elasticsearch.egg-info/top_level.txt
+pytest_elasticsearch.egg-info/zip-safe
```

