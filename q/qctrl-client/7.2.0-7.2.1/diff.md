# Comparing `tmp/qctrl_client-7.2.0.tar.gz` & `tmp/qctrl_client-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_client-7.2.0.tar", max compression
+gzip compressed data, was "qctrl_client-7.2.1.tar", max compression
```

## Comparing `qctrl_client-7.2.0.tar` & `qctrl_client-7.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    36653 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/LICENSE
--rw-r--r--   0        0        0      214 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/README.md
--rw-r--r--   0        0        0     2614 2023-07-18 04:03:28.678655 qctrl_client-7.2.0/pyproject.toml
--rw-r--r--   0        0        0      747 2023-07-18 04:03:28.690655 qctrl_client-7.2.0/qctrlclient/__init__.py
--rw-r--r--   0        0        0      686 2023-07-18 04:03:28.690655 qctrl_client-7.2.0/qctrlclient/auth/__init__.py
--rw-r--r--   0        0        0     1831 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/qctrlclient/auth/base.py
--rw-r--r--   0        0        0     4969 2023-07-18 04:03:08.586697 qctrl_client-7.2.0/qctrlclient/auth/cli.py
--rw-r--r--   0        0        0      972 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/helpers.py
--rw-r--r--   0        0        0     1042 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/keycloak.py
--rw-r--r--   0        0        0     4308 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/oidc.py
--rw-r--r--   0        0        0     1801 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/password.py
--rw-r--r--   0        0        0     3096 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/redirect_listener.py
--rw-r--r--   0        0        0     1516 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/auth/service_account.py
--rw-r--r--   0        0        0     7742 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/client.py
--rw-r--r--   0        0        0      809 2023-07-18 04:03:28.686655 qctrl_client-7.2.0/qctrlclient/core/__init__.py
--rw-r--r--   0        0        0     2999 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/functions.py
--rw-r--r--   0        0        0      995 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/products.py
--rw-r--r--   0        0        0      638 2023-07-18 04:03:28.686655 qctrl_client-7.2.0/qctrlclient/core/router/__init__.py
--rw-r--r--   0        0        0    12547 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/router/api.py
--rw-r--r--   0        0        0     1189 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/router/base.py
--rw-r--r--   0        0        0     1197 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/router/local.py
--rw-r--r--   0        0        0     2677 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/settings.py
--rw-r--r--   0        0        0     1179 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/core/utils.py
--rw-r--r--   0        0        0     1329 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/defaults.py
--rw-r--r--   0        0        0     2172 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/exceptions.py
--rw-r--r--   0        0        0     1357 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/globals.py
--rw-r--r--   0        0        0     1424 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/pytest_plugin.py
--rw-r--r--   0        0        0      601 2023-07-18 04:03:28.690655 qctrl_client-7.2.0/qctrlclient/transports/__init__.py
--rw-r--r--   0        0        0     4625 2023-07-18 04:03:08.590697 qctrl_client-7.2.0/qctrlclient/transports/requests_transport.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-27 23:39:55.540186 qctrl_client-7.2.1/LICENSE
+-rw-r--r--   0        0        0      214 2023-07-27 23:39:55.540186 qctrl_client-7.2.1/README.md
+-rw-r--r--   0        0        0     2614 2023-07-27 23:40:15.148261 qctrl_client-7.2.1/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-07-27 23:40:15.160261 qctrl_client-7.2.1/qctrlclient/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-27 23:40:15.160261 qctrl_client-7.2.1/qctrlclient/auth/__init__.py
+-rw-r--r--   0        0        0     1831 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/base.py
+-rw-r--r--   0        0        0     4969 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/cli.py
+-rw-r--r--   0        0        0      972 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/helpers.py
+-rw-r--r--   0        0        0     1042 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/keycloak.py
+-rw-r--r--   0        0        0     4308 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/oidc.py
+-rw-r--r--   0        0        0     1801 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/password.py
+-rw-r--r--   0        0        0     3096 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/redirect_listener.py
+-rw-r--r--   0        0        0     1516 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/auth/service_account.py
+-rw-r--r--   0        0        0     7742 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/client.py
+-rw-r--r--   0        0        0      809 2023-07-27 23:40:15.156261 qctrl_client-7.2.1/qctrlclient/core/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/core/functions.py
+-rw-r--r--   0        0        0      995 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/core/products.py
+-rw-r--r--   0        0        0      638 2023-07-27 23:40:15.156261 qctrl_client-7.2.1/qctrlclient/core/router/__init__.py
+-rw-r--r--   0        0        0    12547 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/core/router/api.py
+-rw-r--r--   0        0        0     1189 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/core/router/base.py
+-rw-r--r--   0        0        0     1197 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/core/router/local.py
+-rw-r--r--   0        0        0     2677 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/core/settings.py
+-rw-r--r--   0        0        0     1179 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/core/utils.py
+-rw-r--r--   0        0        0     1329 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/defaults.py
+-rw-r--r--   0        0        0     2172 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/exceptions.py
+-rw-r--r--   0        0        0     1357 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/globals.py
+-rw-r--r--   0        0        0     1424 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/pytest_plugin.py
+-rw-r--r--   0        0        0      601 2023-07-27 23:40:15.164261 qctrl_client-7.2.1/qctrlclient/transports/__init__.py
+-rw-r--r--   0        0        0     4625 2023-07-27 23:39:55.544186 qctrl_client-7.2.1/qctrlclient/transports/requests_transport.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 qctrl_client-7.2.1/PKG-INFO
```

### Comparing `qctrl_client-7.2.0/LICENSE` & `qctrl_client-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/pyproject.toml` & `qctrl_client-7.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-client"
-version = "7.2.0"
+version = "7.2.1"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -69,15 +69,15 @@
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 gql = "^3.4.0"
-qctrl-commons = "^19.0.0"
+qctrl-commons = "^19.2.0"
 requests-oauthlib = "^1.3.1"
 PyJWT = "^2.4.0"
 tenacity = "^8.1.0"
 click = "^8.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
```

### Comparing `qctrl_client-7.2.0/qctrlclient/__init__.py` & `qctrl_client-7.2.1/qctrlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/__init__.py` & `qctrl_client-7.2.1/qctrlclient/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/base.py` & `qctrl_client-7.2.1/qctrlclient/auth/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/cli.py` & `qctrl_client-7.2.1/qctrlclient/auth/cli.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/helpers.py` & `qctrl_client-7.2.1/qctrlclient/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/keycloak.py` & `qctrl_client-7.2.1/qctrlclient/auth/keycloak.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/oidc.py` & `qctrl_client-7.2.1/qctrlclient/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/password.py` & `qctrl_client-7.2.1/qctrlclient/auth/password.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/redirect_listener.py` & `qctrl_client-7.2.1/qctrlclient/auth/redirect_listener.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/auth/service_account.py` & `qctrl_client-7.2.1/qctrlclient/auth/service_account.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/client.py` & `qctrl_client-7.2.1/qctrlclient/client.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/__init__.py` & `qctrl_client-7.2.1/qctrlclient/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/functions.py` & `qctrl_client-7.2.1/qctrlclient/core/functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/products.py` & `qctrl_client-7.2.1/qctrlclient/core/products.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/router/__init__.py` & `qctrl_client-7.2.1/qctrlclient/core/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/router/api.py` & `qctrl_client-7.2.1/qctrlclient/core/router/api.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/router/base.py` & `qctrl_client-7.2.1/qctrlclient/core/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/router/local.py` & `qctrl_client-7.2.1/qctrlclient/core/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/settings.py` & `qctrl_client-7.2.1/qctrlclient/core/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/core/utils.py` & `qctrl_client-7.2.1/qctrlclient/core/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/defaults.py` & `qctrl_client-7.2.1/qctrlclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/exceptions.py` & `qctrl_client-7.2.1/qctrlclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/globals.py` & `qctrl_client-7.2.1/qctrlclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/pytest_plugin.py` & `qctrl_client-7.2.1/qctrlclient/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/transports/__init__.py` & `qctrl_client-7.2.1/qctrlclient/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/qctrlclient/transports/requests_transport.py` & `qctrl_client-7.2.1/qctrlclient/transports/requests_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl_client-7.2.0/PKG-INFO` & `qctrl_client-7.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-client
-Version: 7.2.0
+Version: 7.2.1
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -31,15 +31,15 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
-Requires-Dist: qctrl-commons (>=19.0.0,<20.0.0)
+Requires-Dist: qctrl-commons (>=19.2.0,<20.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
```

