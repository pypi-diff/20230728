# Comparing `tmp/jupyter_resource_usage-0.7.2.tar.gz` & `tmp/jupyter_resource_usage-1.0.0.tar.gz`

## Comparing `jupyter_resource_usage-0.7.2.tar` & `jupyter_resource_usage-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.eslintignore
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.eslintrc.js
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.flake8
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.prettierrc
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.travis.yml
--rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/RELEASE.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/install.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/lerna.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/package.json
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/screenshot.png
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/setup.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/warn-screenshot.png
--rw-r--r--   0        0        0   332382 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/yarn.lock
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter-config/jupyter_notebook_config.d/jupyter_resource_usage.json
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter-config/jupyter_server_config.d/jupyter_resource_usage.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter-config/nbconfig/notebook.d/jupyter_resource_usage.json
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/_version.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/api.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/config.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/metrics.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/prometheus.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/server_extension.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/utils.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/package.json
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/114.8d6e04d9186cda5f713e.js
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/361.fa4d5aead5d48c87a0d3.js
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/428.7776162567d49ede3047.js
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/643.5797b52f61f8b1b44c6c.js
--rw-r--r--   0        0        0     8001 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/remoteEntry.fd0401d26424daec88e3.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/style.js
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/static/main.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/tests/__init__.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/jupyter_resource_usage/tests/test_basic.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/.gitignore
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/LICENSE
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/README.md
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 jupyter_resource_usage-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/.flake8
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/.prettierignore
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/.travis.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0    25697 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/RELEASE.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/install.json
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/lerna.json
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/setup.py
+-rw-r--r--   0        0        0   344461 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/yarn.lock
+-rw-r--r--   0        0        0    39236 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/doc/kernel-usage.png
+-rw-r--r--   0        0        0    39075 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/doc/settings.png
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/doc/statusbar-cpu.png
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/doc/statusbar-warn.png
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/doc/statusbar.png
+-rw-r--r--   0        0        0   179449 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/doc/topbar.gif
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter-config/jupyter_notebook_config.d/jupyter_resource_usage.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter-config/jupyter_server_config.d/jupyter_resource_usage.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter-config/nbconfig/notebook.d/jupyter_resource_usage.json
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/_version.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/api.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/config.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/metrics.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/prometheus.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/server_extension.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/utils.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/package.json
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/schemas/@jupyter-server/resource-usage/package.json.orig
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/schemas/@jupyter-server/resource-usage/topbar-item.json
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/114.8d6e04d9186cda5f713e.js
+-rw-r--r--   0        0        0    16761 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/291.449767e171a6d2cb3a4f.js
+-rw-r--r--   0        0        0    28307 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/311.dc54ab57a76db15e51e8.js
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/643.5f6e52f2446514289fab.js
+-rw-r--r--   0        0        0     7992 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/remoteEntry.240d382d3a835c7f1a2e.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/style.js
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/static/main.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/tests/__init__.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/jupyter_resource_usage/tests/test_basic.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/README.md
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 jupyter_resource_usage-1.0.0/PKG-INFO
```

### Comparing `jupyter_resource_usage-0.7.2/.pre-commit-config.yaml` & `jupyter_resource_usage-1.0.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 repos:
-- repo: https://github.com/asottile/reorder_python_imports
-  rev: v3.9.0
+- repo: https://github.com/asottile/reorder-python-imports
+  rev: v3.10.0
   hooks:
   - id: reorder-python-imports
     language_version: python3
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.7.0
   hooks:
   - id: black
 - repo: https://github.com/PyCQA/flake8
   rev: "6.0.0"
   hooks:
     - id: flake8
 - repo: https://github.com/pre-commit/pre-commit-hooks
```

### Comparing `jupyter_resource_usage-0.7.2/.travis.yml` & `jupyter_resource_usage-1.0.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/CHANGELOG.md` & `jupyter_resource_usage-1.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,47 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.0.0
+
+([Full Changelog](https://github.com/jupyter-server/jupyter-resource-usage/compare/@jupyter-server/resource-usage@0.7.2...1cf0e15ed06ce37d8fd4883464beb902fb562d86))
+
+### Enhancements made
+
+- Integrate `jupyterlab-system-monitor` extension [#202](https://github.com/jupyter-server/jupyter-resource-usage/pull/202) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
+
+### Bugs fixed
+
+- Handle `currentWidget` in `KernelWidgetTracker` [#206](https://github.com/jupyter-server/jupyter-resource-usage/pull/206) ([@jtpio](https://github.com/jtpio))
+- Stop all channels to allow ZMQContext to properly cleanup between calls [#183](https://github.com/jupyter-server/jupyter-resource-usage/pull/183) ([@Zsailer](https://github.com/Zsailer))
+
+### Maintenance and upkeep improvements
+
+- Make `IStatusBar` optional for `resourceStatusPlugin` [#207](https://github.com/jupyter-server/jupyter-resource-usage/pull/207) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
+- Require Python 3.8+ [#201](https://github.com/jupyter-server/jupyter-resource-usage/pull/201) ([@jtpio](https://github.com/jtpio))
+- Bump word-wrap from 1.2.3 to 1.2.4 [#200](https://github.com/jupyter-server/jupyter-resource-usage/pull/200) ([@dependabot](https://github.com/dependabot))
+- Bump semver from 5.7.1 to 5.7.2 [#198](https://github.com/jupyter-server/jupyter-resource-usage/pull/198) ([@dependabot](https://github.com/dependabot))
+- Update to Jupyterlab 4 [#195](https://github.com/jupyter-server/jupyter-resource-usage/pull/195) ([@jtpio](https://github.com/jtpio))
+- chore: move `prettier` and `eslint` configuration under `package.json` [#188](https://github.com/jupyter-server/jupyter-resource-usage/pull/188) ([@SauravMaheshkar](https://github.com/SauravMaheshkar))
+- Bump webpack from 5.75.0 to 5.76.1 [#184](https://github.com/jupyter-server/jupyter-resource-usage/pull/184) ([@dependabot](https://github.com/dependabot))
+- Rename references from `master` to `main` [#179](https://github.com/jupyter-server/jupyter-resource-usage/pull/179) ([@jtpio](https://github.com/jtpio))
+
+### Documentation improvements
+
+- Update README and fix settings file [#205](https://github.com/jupyter-server/jupyter-resource-usage/pull/205) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-resource-usage/graphs/contributors?from=2023-02-20&to=2023-07-28&type=c))
+
+[@dependabot](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Adependabot+updated%3A2023-02-20..2023-07-28&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Ajtpio+updated%3A2023-02-20..2023-07-28&type=Issues) | [@mahendrapaipuri](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Amahendrapaipuri+updated%3A2023-02-20..2023-07-28&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Apre-commit-ci+updated%3A2023-02-20..2023-07-28&type=Issues) | [@SauravMaheshkar](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3ASauravMaheshkar+updated%3A2023-02-20..2023-07-28&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Awelcome+updated%3A2023-02-20..2023-07-28&type=Issues) | [@Zsailer](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3AZsailer+updated%3A2023-02-20..2023-07-28&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.7.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-resource-usage/compare/@jupyter-server/resource-usage@0.7.1...143f4568643af18f668d6388fb65fff06695d58d))
 
 ### Bugs fixed
 
 - Clear state when switching away, add blank state indicator [#178](https://github.com/jupyter-server/jupyter-resource-usage/pull/178) ([@krassowski](https://github.com/krassowski))
@@ -15,16 +51,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-resource-usage/graphs/contributors?from=2023-02-06&to=2023-02-20&type=c))
 
 [@Gsbreddy](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3AGsbreddy+updated%3A2023-02-06..2023-02-20&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Ajtpio+updated%3A2023-02-06..2023-02-20&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Akrassowski+updated%3A2023-02-06..2023-02-20&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Aminrk+updated%3A2023-02-06..2023-02-20&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Apre-commit-ci+updated%3A2023-02-06..2023-02-20&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-resource-usage+involves%3Awelcome+updated%3A2023-02-06..2023-02-20&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.7.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-resource-usage/compare/@jupyter-server/resource-usage@0.7.0...dfef59b8aa27eb768eb9e70e849c832d2841e6e9))
 
 ### Enhancements made
 
 - Use `pss` if available [#171](https://github.com/jupyter-server/jupyter-resource-usage/pull/171) ([@jtpio](https://github.com/jtpio))
```

### Comparing `jupyter_resource_usage-0.7.2/CONTRIBUTING.md` & `jupyter_resource_usage-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/__init__.py` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/api.py` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,24 +118,25 @@
         control_channel.send(usage_request)
         poller = zmq.asyncio.Poller()
         control_socket = control_channel.socket
         poller.register(control_socket, zmq.POLLIN)
         timeout_ms = 10_000
         events = dict(await poller.poll(timeout_ms))
         if control_socket not in events:
-            self.write(
-                json.dumps(
-                    {
-                        "content": {"reason": "timeout", "timeout_ms": timeout_ms},
-                        "kernel_id": kernel_id,
-                    }
-                )
+            out = json.dumps(
+                {
+                    "content": {"reason": "timeout", "timeout_ms": timeout_ms},
+                    "kernel_id": kernel_id,
+                }
             )
+
         else:
             res = client.control_channel.get_msg(timeout=0)
             if isawaitable(res):
                 # control_channel.get_msg may return a Future,
                 # depending on configured KernelManager class
                 res = await res
             if res:
                 res["kernel_id"] = kernel_id
-            self.write(json.dumps(res, default=date_default))
+            out = json.dumps(res, default=date_default)
+        client.stop_channels()
+        self.write(out)
```

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/config.py` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/config.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/metrics.py` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/metrics.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/prometheus.py` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/prometheus.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/server_extension.py` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/server_extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/package.json` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9529166666666665%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/console': '^4.0.0', '@jupyterlab/coreutils': '^6.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   "'@jupyterlab/statusbar': '^4.0.0', '@jupyterlab/translation': '^4.0.0', "*

 * *                   "'@lumino/polling': '^2.1.1', 'react-sparklines': '^1.7.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', 'types […]*

```diff
@@ -1,61 +1,64 @@
 {
     "author": "Jupyter Development Team",
     "bugs": {
         "url": "https://github.com/jupyter-server/jupyter-resource-usage/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.5.1",
-        "@jupyterlab/apputils": "^3.5.1",
-        "@jupyterlab/console": "^3.5.1",
-        "@jupyterlab/coreutils": "^5.5.1",
-        "@jupyterlab/notebook": "^3.5.1",
-        "@jupyterlab/services": "^6.5.1",
-        "@jupyterlab/statusbar": "^3.5.1",
-        "@jupyterlab/translation": "^3.5.1",
-        "@lumino/polling": "^1.11.3",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/console": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/statusbar": "^4.0.0",
+        "@jupyterlab/translation": "^4.0.0",
+        "@lumino/polling": "^2.1.1",
+        "react-sparklines": "^1.7.0",
         "typestyle": "^2.4.0"
     },
     "description": "JupyterLab extension to add resource usage UI items",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.5.1",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/react-sparklines": "^1.7.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "typescript": "~5.0.0"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyter-server/jupyter-resource-usage",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fd0401d26424daec88e3.js",
+            "load": "static/remoteEntry.240d382d3a835c7f1a2e.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_kernel_usage"
                 },
                 "managers": [
                     "pip"
                 ]
             }
         },
         "extension": true,
-        "outputDir": "../../jupyter_resource_usage/labextension"
+        "outputDir": "../../jupyter_resource_usage/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -88,9 +91,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "1.0.0"
 }
```

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/114.8d6e04d9186cda5f713e.js` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/114.8d6e04d9186cda5f713e.js`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/428.7776162567d49ede3047.js` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/291.449767e171a6d2cb3a4f.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,421 +1,597 @@
 "use strict";
 (self.webpackChunk_jupyter_server_resource_usage = self.webpackChunk_jupyter_server_resource_usage || []).push([
-    [428], {
-        428: (e, t, r) => {
+    [291], {
+        291: (e, t, r) => {
             r.r(t), r.d(t, {
-                default: () => I
+                default: () => G
             });
-            var s = r(866),
-                n = r(767),
-                a = r(591),
-                o = r(510),
-                i = r(468),
-                l = r(431),
-                c = r(271),
-                m = r.n(c),
-                u = r(886),
-                d = r(258);
-            const _ = {
+            var n = r(4),
+                a = r(172),
+                s = r(663),
+                l = r(861),
+                i = r(580),
+                o = r(787),
+                c = r(760),
+                u = r(354),
+                m = r(778),
+                d = r(29),
+                _ = r.n(d),
+                p = r(987),
+                h = r(790);
+            const v = {
                 B: 1,
                 KB: 1024,
                 MB: 1048576,
                 GB: 1073741824,
                 TB: 1099511627776,
                 PB: 0x4000000000000
             };
 
-            function h(e) {
-                const t = g(e);
+            function g(e) {
+                const t = y(e);
                 return t[0].toFixed(2) + " " + t[1]
             }
 
-            function g(e) {
-                return e ? e < _.KB ? [e, "B"] : _.KB === e || e < _.MB ? [e / _.KB, "KB"] : _.MB === e || e < _.GB ? [e / _.MB, "MB"] : _.GB === e || e < _.TB ? [e / _.GB, "GB"] : _.TB === e || e < _.PB ? [e / _.TB, "TB"] : [e / _.PB, "PB"] : [0, "B"]
+            function y(e) {
+                return e ? e < v.KB ? [e, "B"] : v.KB === e || e < v.MB ? [e / v.KB, "KB"] : v.MB === e || e < v.GB ? [e / v.MB, "MB"] : v.GB === e || e < v.TB ? [e / v.GB, "GB"] : v.TB === e || e < v.PB ? [e / v.TB, "TB"] : [e / v.PB, "PB"] : [0, "B"]
             }
-            let p = null;
-            const v = e => {
+            let C = null;
+            const k = e => {
                     const {
                         reason: t
                     } = e;
-                    return "not_supported" === t.reason ? m().createElement("div", {
+                    return "not_supported" === t.reason ? _().createElement("div", {
                         className: "jp-KernelUsage-section-separator"
-                    }, e.trans.__("Please check with your system administrator that you are running IPyKernel version 6.10.0 or above."), t.kernel_version ? e.trans.__("Detected IPyKernel version: %1", t.kernel_version) : e.trans.__("No IPyKernel installation detected.")) : "no_kernel_widget" === t.reason ? m().createElement("div", {
+                    }, e.trans.__("Please check with your system administrator that you are running IPyKernel version 6.10.0 or above."), t.kernel_version ? e.trans.__("Detected IPyKernel version: %1", t.kernel_version) : e.trans.__("No IPyKernel installation detected.")) : "no_kernel_widget" === t.reason ? _().createElement("div", {
                         className: "jp-KernelUsage-section-separator"
-                    }, e.trans.__("Switch to a notebook or console to see kernel usage details.")) : "no_kernel" === t.reason ? m().createElement("div", {
+                    }, e.trans.__("Switch to a notebook or console to see kernel usage details.")) : "no_kernel" === t.reason ? _().createElement("div", {
                         className: "jp-KernelUsage-section-separator"
-                    }, e.trans.__("No active kernel found.")) : m().createElement("div", {
+                    }, e.trans.__("No active kernel found.")) : _().createElement("div", {
                         className: "jp-KernelUsage-section-separator"
                     }, e.trans.__("Reason: %1.", t.reason))
                 },
-                y = e => {
+                f = e => {
                     var t;
                     const {
                         panel: r
-                    } = e, [s, n] = (0, c.useState)(), [a, o] = (0, c.useState)(), [i, l] = (0, c.useState)(), [_, g] = (0, c.useState)({
+                    } = e, [n, a] = (0, d.useState)(), [s, l] = (0, d.useState)(), [i, o] = (0, d.useState)(), [c, u] = (0, d.useState)({
                         reason: "loading"
                     });
                     ((e, t) => {
-                        const r = (0, c.useRef)();
-                        (0, c.useEffect)((() => {
+                        const r = (0, d.useRef)();
+                        (0, d.useEffect)((() => {
                             r.current = e
-                        }), [e]), (0, c.useEffect)((() => {
+                        }), [e]), (0, d.useEffect)((() => {
                             if (null !== t) {
                                 const e = setInterval((function() {
                                     r.current && r.current()
                                 }), t);
                                 return () => {
                                     clearInterval(e)
                                 }
                             }
                         }), [e, t])
                     })((async () => {
-                        s && r.isVisible && C(s).catch((() => {
-                            console.warn(`Request failed for ${s}. Kernel restarting?`)
+                        n && r.isVisible && v(n).catch((() => {
+                            console.warn(`Request failed for ${n}. Kernel restarting?`)
                         }))
                     }), 5e3);
-                    const y = (0, c.useRef)(s);
-                    y.current = s;
-                    const C = e => async function(e = "", t = {}) {
-                        const r = d.ServerConnection.makeSettings(),
-                            s = u.URLExt.join(r.baseUrl, "api/metrics/v1/kernel_usage", e);
-                        let n;
+                    const m = (0, d.useRef)(n);
+                    m.current = n;
+                    const v = e => async function(e = "", t = {}) {
+                        const r = h.ServerConnection.makeSettings(),
+                            n = p.URLExt.join(r.baseUrl, "api/metrics/v1/kernel_usage", e);
+                        let a;
                         try {
-                            n = await d.ServerConnection.makeRequest(s, t, r)
+                            a = await h.ServerConnection.makeRequest(n, t, r)
                         } catch (e) {
-                            throw new d.ServerConnection.NetworkError(e)
+                            throw new h.ServerConnection.NetworkError(e)
                         }
-                        let a = await n.text();
-                        if (a.length > 0) try {
-                            a = JSON.parse(a)
+                        let s = await a.text();
+                        if (s.length > 0) try {
+                            s = JSON.parse(s)
                         } catch (e) {
-                            console.log("Not a JSON response body.", n)
+                            console.log("Not a JSON response body.", a)
                         }
-                        if (!n.ok) throw new d.ServerConnection.ResponseError(n, a.message || a);
-                        return a
+                        if (!a.ok) throw new h.ServerConnection.ResponseError(a, s.message || s);
+                        return s
                     }(`get_usage/${e}`).then((t => {
                         var r;
-                        if (e !== y.current) return;
+                        if (e !== m.current) return;
                         if (null === (r = t.content) || void 0 === r ? void 0 : r.reason) {
                             const e = t.content;
-                            return void g(e)
+                            return void u(e)
                         }
-                        g(void 0);
-                        const s = {
+                        u(void 0);
+                        const n = {
                             ...t.content,
                             timestamp: new Date,
                             kernel_id: e
                         };
-                        l(s)
+                        o(n)
                     }));
-                    return (0, c.useEffect)((() => {
+                    return (0, d.useEffect)((() => {
                         const t = e => (t, r) => {
-                                var s, a;
-                                const i = null === (s = r.newValue) || void 0 === s ? void 0 : s.id;
+                                var n, s;
+                                const i = null === (n = r.newValue) || void 0 === n ? void 0 : n.id;
                                 if (i) {
-                                    n(i);
-                                    const t = null === (a = null == e ? void 0 : e.sessionContext.session) || void 0 === a ? void 0 : a.model.path;
-                                    o(t), C(i)
-                                } else g({
+                                    a(i);
+                                    const t = null === (s = null == e ? void 0 : e.sessionContext.session) || void 0 === s ? void 0 : s.model.path;
+                                    l(t), v(i)
+                                } else u({
                                     reason: "no_kernel"
-                                }), n(i)
+                                }), a(i)
                             },
                             r = (e, r) => {
-                                var a, i, c, m, u;
-                                if (null === r) return n(void 0), void g({
+                                var s, i, c, m, d;
+                                if (null === r) return a(void 0), void u({
                                     reason: "no_kernel_widget"
                                 });
-                                if (p && p.panel.sessionContext.kernelChanged.disconnect(p.callback), p = {
+                                if (C && C.panel.sessionContext.kernelChanged.disconnect(C.callback), C = {
                                         callback: t(r),
                                         panel: r
-                                    }, r.sessionContext.kernelChanged.connect(p.callback), (null === (i = null === (a = r.sessionContext.session) || void 0 === a ? void 0 : a.kernel) || void 0 === i ? void 0 : i.id) !== s) {
+                                    }, r.sessionContext.kernelChanged.connect(C.callback), (null === (i = null === (s = r.sessionContext.session) || void 0 === s ? void 0 : s.kernel) || void 0 === i ? void 0 : i.id) !== n) {
                                     const e = null === (m = null === (c = r.sessionContext.session) || void 0 === c ? void 0 : c.kernel) || void 0 === m ? void 0 : m.id;
                                     if (e) {
-                                        n(e);
-                                        const t = null === (u = r.sessionContext.session) || void 0 === u ? void 0 : u.model.path;
-                                        o(t), l(void 0), g({
+                                        a(e);
+                                        const t = null === (d = r.sessionContext.session) || void 0 === d ? void 0 : d.model.path;
+                                        l(t), o(void 0), u({
                                             reason: "loading"
-                                        }), C(e)
-                                    } else n(void 0), g({
+                                        }), v(e)
+                                    } else a(void 0), u({
                                         reason: "no_kernel"
                                     })
                                 }
                             };
-                        return e.currentChanged.connect(r), () => {
-                            e.currentChanged.disconnect(r)
+                        return e.tracker.currentChanged.connect(r), e.tracker.currentWidget && r(e.tracker, e.tracker.currentWidget), () => {
+                            e.tracker.currentChanged.disconnect(r)
                         }
-                    }), [s]), _ && "timeout" !== (null == _ ? void 0 : _.reason) && "loading" !== (null == _ ? void 0 : _.reason) ? m().createElement(m().Fragment, null, m().createElement("h3", {
+                    }), [n]), c && "timeout" !== (null == c ? void 0 : c.reason) && "loading" !== (null == c ? void 0 : c.reason) ? _().createElement(_().Fragment, null, _().createElement("h3", {
                         className: "jp-KernelUsage-section-separator"
-                    }, e.trans.__("Kernel usage not available")), m().createElement(v, {
+                    }, e.trans.__("Kernel usage not available")), _().createElement(k, {
                         trans: e.trans,
-                        reason: _
-                    })) : s ? m().createElement(m().Fragment, null, m().createElement("h3", {
+                        reason: c
+                    })) : n ? _().createElement(_().Fragment, null, _().createElement("h3", {
                         className: "jp-KernelUsage-section-separator"
-                    }, e.trans.__("Kernel usage")), "timeout" === (null == _ ? void 0 : _.reason) ? m().createElement("strong", null, e.trans.__("Timed out in: %1 ms", _.timeout_ms)) : null, m().createElement("div", {
+                    }, e.trans.__("Kernel usage")), "timeout" === (null == c ? void 0 : c.reason) ? _().createElement("strong", null, e.trans.__("Timed out in: %1 ms", c.timeout_ms)) : null, _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Notebook:"), " ", a), m().createElement("div", {
+                    }, e.trans.__("Notebook:"), " ", s), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Kernel ID:"), " ", s), m().createElement("div", {
-                        className: "timeout" === (null == _ ? void 0 : _.reason) ? "jp-KernelUsage-timedOut" : ""
-                    }, i ? m().createElement(m().Fragment, null, m().createElement("div", {
+                    }, e.trans.__("Kernel ID:"), " ", n), _().createElement("div", {
+                        className: "timeout" === (null == c ? void 0 : c.reason) ? "jp-KernelUsage-timedOut" : ""
+                    }, i ? _().createElement(_().Fragment, null, _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Kernel Host:"), " ", i.hostname), m().createElement("div", {
+                    }, e.trans.__("Kernel Host:"), " ", i.hostname), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Timestamp:"), " ", null === (t = i.timestamp) || void 0 === t ? void 0 : t.toLocaleString()), m().createElement("div", {
+                    }, e.trans.__("Timestamp:"), " ", null === (t = i.timestamp) || void 0 === t ? void 0 : t.toLocaleString()), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Process ID:"), " ", i.pid), m().createElement("div", {
+                    }, e.trans.__("Process ID:"), " ", i.pid), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("CPU:"), " ", i.kernel_cpu), m().createElement("div", {
+                    }, e.trans.__("CPU:"), " ", i.kernel_cpu), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Memory:"), " ", h(i.kernel_memory)), m().createElement("hr", {
+                    }, e.trans.__("Memory:"), " ", g(i.kernel_memory)), _().createElement("hr", {
                         className: "jp-KernelUsage-section-separator"
-                    }), m().createElement("h4", {
+                    }), _().createElement("h4", {
                         className: "jp-KernelUsage-section-separator"
-                    }, e.trans.__("Host CPU")), i.host_cpu_percent && m().createElement("div", {
+                    }, e.trans.__("Host CPU")), i.host_cpu_percent && _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans._n("%2%% used on %1 CPU", "%2%% used on %1 CPUs", i.cpu_count, i.host_cpu_percent.toFixed(1))), m().createElement("h4", {
+                    }, e.trans._n("%2%% used on %1 CPU", "%2%% used on %1 CPUs", i.cpu_count, i.host_cpu_percent.toFixed(1))), _().createElement("h4", {
                         className: "jp-KernelUsage-section-separator"
-                    }, e.trans.__("Host Virtual Memory")), m().createElement("div", {
+                    }, e.trans.__("Host Virtual Memory")), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Active:"), " ", h(i.host_virtual_memory.active)), m().createElement("div", {
+                    }, e.trans.__("Active:"), " ", g(i.host_virtual_memory.active)), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Available:"), " ", h(i.host_virtual_memory.available)), m().createElement("div", {
+                    }, e.trans.__("Available:"), " ", g(i.host_virtual_memory.available)), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Free:"), " ", h(i.host_virtual_memory.free)), m().createElement("div", {
+                    }, e.trans.__("Free:"), " ", g(i.host_virtual_memory.free)), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Inactive:"), " ", h(i.host_virtual_memory.inactive)), i.host_virtual_memory.percent && m().createElement("div", {
+                    }, e.trans.__("Inactive:"), " ", g(i.host_virtual_memory.inactive)), i.host_virtual_memory.percent && _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Percent used:"), " ", i.host_virtual_memory.percent.toFixed(1), "%"), m().createElement("div", {
+                    }, e.trans.__("Percent used:"), " ", i.host_virtual_memory.percent.toFixed(1), "%"), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Total:"), " ", h(i.host_virtual_memory.total)), m().createElement("div", {
+                    }, e.trans.__("Total:"), " ", g(i.host_virtual_memory.total)), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Used:"), " ", h(i.host_virtual_memory.used)), m().createElement("div", {
+                    }, e.trans.__("Used:"), " ", g(i.host_virtual_memory.used)), _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Wired:"), " ", h(i.host_virtual_memory.wired))) : "loading" === (null == _ ? void 0 : _.reason) ? m().createElement("div", {
+                    }, e.trans.__("Wired:"), " ", g(i.host_virtual_memory.wired))) : "loading" === (null == c ? void 0 : c.reason) ? _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Loading…")) : m().createElement("div", {
+                    }, e.trans.__("Loading…")) : _().createElement("div", {
                         className: "jp-KernelUsage-separator"
-                    }, e.trans.__("Usage data is missing")))) : m().createElement("h3", null, e.trans.__("Kernel usage is missing"))
+                    }, e.trans.__("Usage data is missing")))) : _().createElement("h3", null, e.trans.__("Kernel usage is missing"))
                 };
-            class C extends o.ReactWidget {
+            class b extends a.ReactWidget {
                 constructor(e) {
-                    super(), this._currentChanged = e.currentChanged, this._panel = e.panel, this._trans = e.trans, this.addClass("jp-KernelUsage-content")
+                    super(), this._tracker = e.tracker, this._panel = e.panel, this._trans = e.trans, this.addClass("jp-KernelUsage-content")
                 }
                 render() {
-                    return m().createElement(y, {
-                        currentChanged: this._currentChanged,
+                    return _().createElement(f, {
+                        tracker: this._tracker,
                         panel: this._panel,
                         trans: this._trans
                     })
                 }
             }
-            const f = '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">\r\n  <g class="jp-icon3" fill="#616161">\r\n    <path d="m256 43c-141 0-256 115-256 256 0 62 22 118 59 163l6 8h383l6-8c37-44 59-101 59-163-0.1-141-115-256-256-256zm0 43c118 0 213 95 213 213 0 48-17 92-44 128h-339c-27-36-44-80-44-128 0-118 95-213 213-213zm0 21c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm-85 23c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.6-21-21-21zm171 0c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm-233 63c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm290 0.7-121 69c-6.3-3.7-14-6-21-6-24 0-43 19-43 43s19 43 43 43c23 0 42-19 43-42v-0.7l121-69-21-37zm-313 85c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm341 0c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.6-21-21-21zm-319 85c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm296 0c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21z"/>\r\n  </g>\r\n</svg>\r\n\x3c!-- Downloaded from https://seekicon.com/free-icon/tachometer-alt_1 under MIT License. --\x3e\r\n';
-            class k extends l.StackedPanel {
+            const E = '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">\r\n  <g class="jp-icon3" fill="#616161">\r\n    <path d="m256 43c-141 0-256 115-256 256 0 62 22 118 59 163l6 8h383l6-8c37-44 59-101 59-163-0.1-141-115-256-256-256zm0 43c118 0 213 95 213 213 0 48-17 92-44 128h-339c-27-36-44-80-44-128 0-118 95-213 213-213zm0 21c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm-85 23c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.6-21-21-21zm171 0c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm-233 63c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm290 0.7-121 69c-6.3-3.7-14-6-21-6-24 0-43 19-43 43s19 43 43 43c23 0 42-19 43-42v-0.7l121-69-21-37zm-313 85c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm341 0c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.6-21-21-21zm-319 85c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21zm296 0c-12 0-21 9.6-21 21s9.6 21 21 21 21-9.6 21-21-9.5-21-21-21z"/>\r\n  </g>\r\n</svg>\r\n\x3c!-- Downloaded from https://seekicon.com/free-icon/tachometer-alt_1 under MIT License. --\x3e\r\n';
+            class j extends m.StackedPanel {
                 constructor(e) {
-                    super(), this.addClass("jp-KernelUsage-view"), this.id = "kernelusage-panel-id", this.title.caption = e.trans.__("Kernel Usage"), this.title.icon = new a.LabIcon({
+                    super(), this.addClass("jp-KernelUsage-view"), this.id = "kernelusage-panel-id", this.title.caption = e.trans.__("Kernel Usage"), this.title.icon = new i.LabIcon({
                         name: "jupyterlab-kernel-usage:icon",
-                        svgstr: f
+                        svgstr: E
                     }), this.title.closable = !0;
-                    const t = new C({
-                        currentChanged: e.currentChanged,
+                    const t = new b({
+                        tracker: e.tracker,
                         panel: this,
                         trans: e.trans
                     });
                     this.addWidget(t)
                 }
                 dispose() {
                     super.dispose()
                 }
                 onCloseRequest(e) {
                     super.onCloseRequest(e), this.dispose()
                 }
             }
-            var E = r(169),
-                K = r(442),
-                U = r(722);
-            const j = (0, r(95).style)({
-                fontSize: "var(--jp-ui-font-size1)",
-                fontFamily: "var(--jp-ui-font-family)"
-            }, {
-                backgroundColor: "#FFD2D2",
-                color: "#D8000C"
-            });
-            class w extends o.VDomRenderer {
-                constructor(e) {
-                    super(new w.Model({
-                        refreshRate: 5e3
-                    })), this._trans = e
-                }
-                render() {
-                    if (!this.model) return m().createElement("div", null);
-                    let e;
-                    return e = null === this.model.memoryLimit ? this._trans.__("Mem: %1 %2", this.model.currentMemory.toFixed(b.DECIMAL_PLACES), this.model.units) : this._trans.__("Mem: %1 / %2 %3", this.model.currentMemory.toFixed(b.DECIMAL_PLACES), this.model.memoryLimit.toFixed(b.DECIMAL_PLACES), this.model.units), this.model.usageWarning ? m().createElement(E.TextItem, {
-                        title: this._trans.__("Current memory usage"),
-                        source: e,
-                        className: j
-                    }) : m().createElement(E.TextItem, {
-                        title: this._trans.__("Current memory usage"),
-                        source: e
-                    })
-                }
-            }
-            var b;
+            var K, w, U = r(797);
             ! function(e) {
-                class t extends o.VDomModel {
+                class t extends a.VDomModel {
                     constructor(e) {
-                        super(), this._currentMemory = 0, this._memoryLimit = null, this._metricsAvailable = !1, this._units = "B", this._warn = !1, this._poll = new U.Poll({
-                            factory: () => b.factory(),
+                        super(), this._memoryAvailable = !1, this._cpuAvailable = !1, this._currentMemory = 0, this._currentCpuPercent = 0, this._memoryLimit = null, this._cpuLimit = null, this._units = "B", this._warn = !1, this._values = [];
+                        for (let e = 0; e < 20; e++) this._values.push({
+                            memoryPercent: 0,
+                            cpuPercent: 0
+                        });
+                        this._poll = new U.Poll({
+                            factory: () => w.factory(),
                             frequency: {
                                 interval: e.refreshRate,
                                 backoff: !0
                             },
-                            name: "@jupyterlab/statusbar:MemoryUsage#metrics"
+                            name: "@jupyterlab/statusbar:ResourceUsage#metrics"
                         }), this._poll.ticked.connect((e => {
                             const {
                                 payload: t,
                                 phase: r
                             } = e.state;
                             if ("resolved" !== r) {
                                 if ("rejected" === r) {
-                                    const e = this._metricsAvailable;
-                                    return this._metricsAvailable = !1, this._currentMemory = 0, this._memoryLimit = null, this._units = "B", void(e && this.stateChanged.emit())
+                                    const e = this._memoryAvailable,
+                                        t = this._cpuAvailable;
+                                    return this._memoryAvailable = !1, this._cpuAvailable = !1, this._currentMemory = 0, this._memoryLimit = null, this._cpuLimit = null, this._units = "B", void((e || t) && this.stateChanged.emit())
                                 }
                             } else this._updateMetricsValues(t)
                         }))
                     }
+                    async refresh() {
+                        await this._poll.refresh(), await this._poll.tick
+                    }
                     get metricsAvailable() {
-                        return this._metricsAvailable
+                        return this._memoryAvailable || this._cpuAvailable
+                    }
+                    get memoryAvailable() {
+                        return this._memoryAvailable
+                    }
+                    get cpuAvailable() {
+                        return this._cpuAvailable
                     }
                     get currentMemory() {
                         return this._currentMemory
                     }
                     get memoryLimit() {
                         return this._memoryLimit
                     }
+                    get cpuLimit() {
+                        return this._cpuLimit
+                    }
                     get units() {
                         return this._units
                     }
+                    get currentCpuPercent() {
+                        return this._currentCpuPercent
+                    }
+                    get values() {
+                        return this._values
+                    }
                     get usageWarning() {
                         return this._warn
                     }
                     dispose() {
                         super.dispose(), this._poll.dispose()
                     }
                     _updateMetricsValues(e) {
-                        var t, r, s;
-                        const n = this._metricsAvailable,
-                            a = this._currentMemory,
-                            o = this._memoryLimit,
-                            i = this._units,
-                            l = this._warn;
-                        if (null === e) this._metricsAvailable = !1, this._currentMemory = 0, this._memoryLimit = null, this._units = "B", this._warn = !1;
-                        else {
-                            const n = null !== (t = e.pss) && void 0 !== t ? t : e.rss,
-                                a = e.limits.memory,
-                                o = null !== (s = null !== (r = null == a ? void 0 : a.pss) && void 0 !== r ? r : null == a ? void 0 : a.rss) && void 0 !== s ? s : null,
-                                [i, l] = g(n),
-                                c = !!e.limits.memory && e.limits.memory.warn;
-                            this._metricsAvailable = !0, this._currentMemory = i, this._units = l, this._memoryLimit = o ? o / _[l] : null, this._warn = c
-                        }
-                        this._currentMemory === a && this._units === i && this._memoryLimit === o && this._metricsAvailable === n && this._warn === l || this.stateChanged.emit(void 0)
+                        var t, r, n;
+                        if (null === e) return this._memoryAvailable = !1, this._cpuAvailable = !1, this._currentMemory = 0, this._memoryLimit = null, this._units = "B", void(this._warn = !1);
+                        const a = null !== (t = e.pss) && void 0 !== t ? t : e.rss,
+                            s = e.limits.memory,
+                            l = null !== (n = null !== (r = null == s ? void 0 : s.pss) && void 0 !== r ? r : null == s ? void 0 : s.rss) && void 0 !== n ? n : null,
+                            [i, o] = y(a),
+                            c = !!e.limits.memory && e.limits.memory.warn;
+                        this._memoryAvailable = void 0 !== a, this._currentMemory = i, this._units = o, this._memoryLimit = l ? l / v[o] : null;
+                        const u = this.memoryLimit ? Math.min(this._currentMemory / this.memoryLimit, 1) : 0;
+                        this._warn = c, this._cpuLimit = e.limits.cpu ? e.limits.cpu.cpu : null, this._cpuAvailable = void 0 !== e.cpu_percent, this._currentCpuPercent = void 0 !== e.cpu_percent ? e.cpu_percent / 100 : 0, this._values.push({
+                            memoryPercent: u,
+                            cpuPercent: this._currentCpuPercent
+                        }), this._values.shift(), this.stateChanged.emit(void 0)
                     }
                 }
                 e.Model = t
-            }(w || (w = {})),
+            }(K || (K = {})),
             function(e) {
-                e.DECIMAL_PLACES = 2;
-                const t = d.ServerConnection.makeSettings(),
-                    r = u.URLExt.join(t.baseUrl, "api/metrics/v1");
-                e.factory = async function() {
-                    const e = d.ServerConnection.makeRequest(r, {}, t),
-                        s = await e;
-                    return await s.json()
-                }
-            }(b || (b = {}));
-            var N, B = r(840);
-            class S {
+                const t = h.ServerConnection.makeSettings(),
+                    r = p.URLExt.join(t.baseUrl, "api/metrics/v1");
+                e.factory = async () => {
+                    const e = h.ServerConnection.makeRequest(r, {}, t),
+                        n = await e;
+                    return n.ok ? await n.json() : null
+                }
+            }(w || (w = {}));
+            const N = (0, r(95).style)({
+                fontSize: "var(--jp-ui-font-size1)",
+                fontFamily: "var(--jp-ui-font-family)"
+            }, {
+                backgroundColor: "#FFD2D2",
+                color: "#D8000C"
+            });
+            class S extends a.VDomRenderer {
                 constructor(e) {
+                    super(new K.Model({
+                        refreshRate: 5e3
+                    })), this._trans = e
+                }
+                render() {
+                    if (!this.model) return _().createElement("div", null);
+                    let e;
+                    return e = null === this.model.memoryLimit ? this._trans.__("Mem: %1 %2", this.model.currentMemory.toFixed(B.DECIMAL_PLACES), this.model.units) : this._trans.__("Mem: %1 / %2 %3", this.model.currentMemory.toFixed(B.DECIMAL_PLACES), this.model.memoryLimit.toFixed(B.DECIMAL_PLACES), this.model.units), this.model.cpuAvailable && (e = `CPU: ${(100*this.model.currentCpuPercent).toFixed(B.DECIMAL_PLACES)} % ${e}`), this.model.usageWarning ? _().createElement(c.TextItem, {
+                        title: this._trans.__("Current resource usage"),
+                        source: e,
+                        className: N
+                    }) : _().createElement(c.TextItem, {
+                        title: this._trans.__("Current resource usage"),
+                        source: e
+                    })
+                }
+            }
+            var B;
+            ! function(e) {
+                e.DECIMAL_PLACES = 2
+            }(B || (B = {}));
+            var P = r(901);
+
+            function x(e) {
+                return e instanceof o.ConsolePanel || e instanceof l.NotebookPanel
+            }
+            class M {
+                constructor(e) {
+                    var t, r;
+                    this._currentWidget = null;
                     const {
-                        labShell: t,
-                        notebookTracker: r,
+                        labShell: n,
+                        notebookTracker: a,
                         consoleTracker: s
                     } = e;
-                    this._currentChanged = new B.Signal(this), t ? t.currentChanged.connect(((e, t) => {
+                    this._currentChanged = new P.Signal(this), n ? n.currentChanged.connect(((e, t) => {
                         const r = t.newValue;
-                        r && function(e) {
-                            return e instanceof i.ConsolePanel || e instanceof n.NotebookPanel
-                        }(r) ? this._currentChanged.emit(r) : this._currentChanged.emit(null)
-                    })) : (r.currentChanged.connect(((e, t) => {
-                        this._currentChanged.emit(t)
+                        r && x(r) ? (this._currentChanged.emit(r), this._currentWidget = r) : (this._currentChanged.emit(null), this._currentWidget = null)
+                    })) : (a.currentChanged.connect(((e, t) => {
+                        this._currentChanged.emit(t), this._currentWidget = t
                     })), s && s.currentChanged.connect(((e, t) => {
-                        this._currentChanged.emit(t)
-                    })))
+                        this._currentChanged.emit(t), this._currentWidget = t
+                    }))), (null == n ? void 0 : n.currentWidget) && x(null == n ? void 0 : n.currentWidget) ? this._currentWidget = n.currentWidget : this._currentWidget = null !== (r = null !== (t = a.currentWidget) && void 0 !== t ? t : null == s ? void 0 : s.currentWidget) && void 0 !== r ? r : null
                 }
                 get currentChanged() {
                     return this._currentChanged
                 }
-            }! function(e) {
+                get currentWidget() {
+                    return this._currentWidget
+                }
+            }
+            var A = r(686);
+            const L = ({
+                    percentage: e,
+                    color: t
+                }) => _().createElement("div", {
+                    className: "jp-IndicatorFiller",
+                    style: {
+                        width: 100 * e + "%",
+                        background: `${t}`
+                    }
+                }),
+                I = ({
+                    values: e,
+                    percentage: t,
+                    baseColor: r
+                }) => {
+                    const [n, a] = (0, d.useState)(!1), s = t > .5 ? t > .8 ? "red" : "orange" : r;
+                    return _().createElement("div", {
+                        className: "jp-IndicatorBar",
+                        onClick: () => {
+                            a(!n)
+                        }
+                    }, n && _().createElement(A.Sparklines, {
+                        data: e,
+                        min: 0,
+                        max: 1,
+                        limit: e.length,
+                        margin: 0
+                    }, _().createElement(A.SparklinesLine, {
+                        style: {
+                            stroke: s,
+                            strokeWidth: 4,
+                            fill: s,
+                            fillOpacity: 1
+                        }
+                    }), _().createElement(A.SparklinesSpots, null)), !n && _().createElement(L, {
+                        percentage: t,
+                        color: s
+                    }))
+                },
+                W = ({
+                    enabled: e,
+                    values: t,
+                    label: r,
+                    color: n,
+                    text: a
+                }) => {
+                    const s = t[t.length - 1];
+                    return _().createElement(_().Fragment, null, e && _().createElement("div", {
+                        className: "jp-IndicatorContainer"
+                    }, _().createElement("div", {
+                        className: "jp-IndicatorText"
+                    }, r), null !== s && _().createElement("div", {
+                        className: "jp-IndicatorWrapper"
+                    }, _().createElement(I, {
+                        values: t,
+                        percentage: s,
+                        baseColor: n
+                    })), _().createElement("div", {
+                        className: "jp-IndicatorText"
+                    }, a)))
+                },
+                T = ({
+                    model: e,
+                    label: t
+                }) => {
+                    const [r, n] = (0, d.useState)(""), [a, s] = (0, d.useState)([]), l = () => {
+                        const {
+                            cpuLimit: t,
+                            currentCpuPercent: r
+                        } = e, a = e.values.map((e => Math.min(1, e.cpuPercent / (t || 1)))), l = `${(100*r).toFixed(0)}%`;
+                        n(l), s(a)
+                    };
+                    return (0, d.useEffect)((() => (e.stateChanged.connect(l), () => {
+                        e.stateChanged.disconnect(l)
+                    })), [e]), _().createElement(W, {
+                        enabled: e.cpuAvailable,
+                        values: a,
+                        label: t,
+                        color: "#0072B3",
+                        text: r
+                    })
+                };
+            var R;
+            ! function(e) {
+                e.createCpuView = (e, t) => a.ReactWidget.create(_().createElement(T, {
+                    model: e,
+                    label: t
+                }))
+            }(R || (R = {}));
+            const F = ({
+                model: e,
+                label: t
+            }) => {
+                const [r, n] = (0, d.useState)(""), [a, s] = (0, d.useState)([]), l = () => {
+                    const {
+                        memoryLimit: t,
+                        currentMemory: r,
+                        units: a
+                    } = e, l = ["B", "KB", "MB"].indexOf(a) > 0 ? 0 : 2, i = `${r.toFixed(l)} ${t?"/ "+t.toFixed(l):""} ${a}`, o = e.values.map((e => e.memoryPercent));
+                    n(i), s(o)
+                };
+                return (0, d.useEffect)((() => (e.stateChanged.connect(l), () => {
+                    e.stateChanged.disconnect(l)
+                })), [e]), _().createElement(W, {
+                    enabled: e.memoryAvailable,
+                    values: a,
+                    label: t,
+                    color: "#00B35B",
+                    text: r
+                })
+            };
+            var D, z;
+            ! function(e) {
+                e.createMemoryView = (e, t) => a.ReactWidget.create(_().createElement(F, {
+                    model: e,
+                    label: t
+                }))
+            }(D || (D = {})),
+            function(e) {
                 e.getKernelUsage = "kernel-usage:get"
-            }(N || (N = {}));
-            const M = {
-                    id: "@jupyter-server/resource-usage:memory-status-item",
+            }(z || (z = {}));
+            const V = {
+                    id: "@jupyter-server/resource-usage:status-item",
                     autoStart: !0,
-                    requires: [E.IStatusBar, K.ITranslator],
+                    requires: [u.ITranslator],
+                    optional: [c.IStatusBar],
                     activate: (e, t, r) => {
-                        const s = r.load("jupyter-resource-usage"),
-                            n = new w(s);
-                        t.registerStatusItem(M.id, {
-                            item: n,
+                        const n = t.load("jupyter-resource-usage"),
+                            a = new S(n);
+                        r && r.registerStatusItem(V.id, {
+                            item: a,
                             align: "left",
                             rank: 2,
-                            isActive: () => n.model.metricsAvailable,
-                            activeStateChanged: n.model.stateChanged
+                            isActive: () => a.model.metricsAvailable,
+                            activeStateChanged: a.model.stateChanged
                         })
                     }
                 },
-                x = {
+                q = {
+                    id: "@jupyter-server/resource-usage:topbar-item",
+                    autoStart: !0,
+                    requires: [a.IToolbarWidgetRegistry],
+                    optional: [s.ISettingRegistry],
+                    activate: async (e, t, r) => {
+                        let n = !1,
+                            a = 5e3,
+                            s = "CPU: ",
+                            l = "Mem: ";
+                        if (r) {
+                            const e = await r.load(q.id);
+                            n = e.get("enable").composite, a = e.get("refreshRate").composite;
+                            const t = e.get("cpu").composite;
+                            s = t.label;
+                            const i = e.get("memory").composite;
+                            l = i.label
+                        }
+                        const i = new K.Model({
+                            refreshRate: a
+                        });
+                        await i.refresh(), n && i.cpuAvailable && t.addFactory("TopBar", "cpu", (() => R.createCpuView(i, s))), n && i.memoryAvailable && t.addFactory("TopBar", "memory", (() => D.createMemoryView(i, l)))
+                    }
+                },
+                $ = {
                     id: "@jupyter-server/resource-usage:kernel-panel-item",
                     autoStart: !0,
-                    optional: [o.ICommandPalette, s.ILabShell, i.IConsoleTracker],
-                    requires: [K.ITranslator, n.INotebookTracker],
-                    activate: (e, t, r, s, n, o) => {
-                        const i = t.load("jupyter-resource-usage"),
+                    optional: [a.ICommandPalette, n.ILabShell, o.IConsoleTracker],
+                    requires: [u.ITranslator, l.INotebookTracker],
+                    activate: (e, t, r, n, a, s) => {
+                        const l = t.load("jupyter-resource-usage"),
                             {
-                                commands: l,
+                                commands: o,
                                 shell: c
                             } = e,
-                            m = i.__("Kernel Resource");
-                        let u = null;
+                            u = l.__("Kernel Resource");
+                        let m = null;
 
                         function d() {
-                            if (!u || u.isDisposed) {
-                                const e = new S({
+                            if (!m || m.isDisposed) {
+                                const e = new M({
                                     notebookTracker: r,
-                                    labShell: n,
-                                    consoleTracker: o
+                                    labShell: a,
+                                    consoleTracker: s
                                 });
-                                u = new k({
-                                    currentChanged: e.currentChanged,
-                                    trans: i
-                                }), c.add(u, "right", {
+                                m = new j({
+                                    tracker: e,
+                                    trans: l
+                                }), c.add(m, "right", {
                                     rank: 200
                                 })
                             }
                         }
-                        l.addCommand(N.getKernelUsage, {
-                            label: i.__("Kernel Usage"),
-                            caption: i.__("Kernel Usage"),
-                            icon: new a.LabIcon({
+                        o.addCommand(z.getKernelUsage, {
+                            label: l.__("Kernel Usage"),
+                            caption: l.__("Kernel Usage"),
+                            icon: new i.LabIcon({
                                 name: "jupyterlab-kernel-usage:icon",
-                                svgstr: f
+                                svgstr: E
                             }),
                             execute: d
-                        }), s && s.addItem({
-                            command: N.getKernelUsage,
-                            category: m
+                        }), n && n.addItem({
+                            command: z.getKernelUsage,
+                            category: u
                         }), d()
                     }
                 },
-                I = [M, x]
+                G = [V, q, $]
         }
     }
 ]);
```

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/remoteEntry.fd0401d26424daec88e3.js` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/remoteEntry.240d382d3a835c7f1a2e.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,303 +1,303 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, u, i, l, s, d, f, c, p, h, v, g, b, y = {
+    var e, r, t, a, n, o, u, i, l, s, f, c, d, p, h, v, b, g, y, m = {
             357: (e, r, t) => {
-                var n = {
-                        "./index": () => Promise.all([t.e(840), t.e(428)]).then((() => () => t(428))),
-                        "./extension": () => Promise.all([t.e(840), t.e(428)]).then((() => () => t(428))),
+                var a = {
+                        "./index": () => Promise.all([t.e(29), t.e(291)]).then((() => () => t(291))),
+                        "./extension": () => Promise.all([t.e(29), t.e(291)]).then((() => () => t(291))),
                         "./style": () => t.e(643).then((() => () => t(643)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
-                            var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            var a = "default",
+                                n = t.S[a];
+                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => n,
+                    init: () => o
                 })
             }
         },
-        m = {};
+        j = {};
 
-    function j(e) {
-        var r = m[e];
+    function w(e) {
+        var r = j[e];
         if (void 0 !== r) return r.exports;
-        var t = m[e] = {
+        var t = j[e] = {
             id: e,
             exports: {}
         };
-        return y[e](t, t.exports, j), t.exports
+        return m[e].call(t.exports, t, t.exports, w), t.exports
     }
-    j.m = y, j.c = m, j.n = e => {
+    w.m = m, w.c = j, w.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return j.d(r, {
+        return w.d(r, {
             a: r
         }), r
-    }, j.d = (e, r) => {
-        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
+    }, w.d = (e, r) => {
+        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
+        29: "6c1b944c8a320967478b",
         114: "8d6e04d9186cda5f713e",
-        361: "fa4d5aead5d48c87a0d3",
-        428: "7776162567d49ede3047",
-        526: "3fd4140c4ce0b9213917",
-        643: "5797b52f61f8b1b44c6c",
-        840: "e084cd5a24a6e059138b"
+        291: "449767e171a6d2cb3a4f",
+        311: "dc54ab57a76db15e51e8",
+        643: "5f6e52f2446514289fab"
     } [e] + ".js?v=" + {
+        29: "6c1b944c8a320967478b",
         114: "8d6e04d9186cda5f713e",
-        361: "fa4d5aead5d48c87a0d3",
-        428: "7776162567d49ede3047",
-        526: "3fd4140c4ce0b9213917",
-        643: "5797b52f61f8b1b44c6c",
-        840: "e084cd5a24a6e059138b"
-    } [e], j.g = function() {
+        291: "449767e171a6d2cb3a4f",
+        311: "dc54ab57a76db15e51e8",
+        643: "5f6e52f2446514289fab"
+    } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter-server/resource-usage:", j.l = (t, n, o, a) => {
-        if (e[t]) e[t].push(n);
+    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter-server/resource-usage:", w.l = (t, a, n, o) => {
+        if (e[t]) e[t].push(a);
         else {
             var u, i;
-            if (void 0 !== o)
+            if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        u = d;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        u = f;
                         break
                     }
                 }
-            u || (i = !0, (u = document.createElement("script")).charset = "utf-8", u.timeout = 120, j.nc && u.setAttribute("nonce", j.nc), u.setAttribute("data-webpack", r + o), u.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    u.onerror = u.onload = null, clearTimeout(c);
-                    var o = e[t];
-                    if (delete e[t], u.parentNode && u.parentNode.removeChild(u), o && o.forEach((e => e(n))), r) return r(n)
+            u || (i = !0, (u = document.createElement("script")).charset = "utf-8", u.timeout = 120, w.nc && u.setAttribute("nonce", w.nc), u.setAttribute("data-webpack", r + n), u.src = t), e[t] = [a];
+            var c = (r, a) => {
+                    u.onerror = u.onload = null, clearTimeout(d);
+                    var n = e[t];
+                    if (delete e[t], u.parentNode && u.parentNode.removeChild(u), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                d = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: u
                 }), 12e4);
-            u.onerror = f.bind(null, u.onerror), u.onload = f.bind(null, u.onload), i && document.head.appendChild(u)
+            u.onerror = c.bind(null, u.onerror), u.onload = c.bind(null, u.onload), i && document.head.appendChild(u)
         }
-    }, j.r = e => {
+    }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        j.S = {};
+        w.S = {};
         var e = {},
             r = {};
-        j.I = (t, n) => {
-            n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
-                j.o(j.S, t) || (j.S[t] = {});
-                var a = j.S[t],
+        w.I = (t, a) => {
+            a || (a = []);
+            var n = r[t];
+            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
+                if (a.push(n), e[t]) return e[t];
+                w.o(w.S, t) || (w.S[t] = {});
+                var o = w.S[t],
                     u = "@jupyter-server/resource-usage",
-                    i = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            i = o[r];
-                        (!i || !i.loaded && (!n != !i.eager ? n : u > i.from)) && (o[r] = {
+                    i = (e, r, t, a) => {
+                        var n = o[e] = o[e] || {},
+                            i = n[r];
+                        (!i || !i.loaded && (!a != !i.eager ? a : u > i.from)) && (n[r] = {
                             get: t,
                             from: u,
-                            eager: !!n
+                            eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (i("@jupyter-server/resource-usage", "0.7.2", (() => Promise.all([j.e(840), j.e(428)]).then((() => () => j(428))))), i("@lumino/polling", "1.11.4", (() => Promise.all([j.e(361), j.e(840), j.e(526)]).then((() => () => j(361))))), i("typestyle", "2.4.0", (() => j.e(114).then((() => () => j(114)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@jupyter-server/resource-usage", "1.0.0", (() => Promise.all([w.e(29), w.e(291)]).then((() => () => w(291))))), i("react-sparklines", "1.7.0", (() => Promise.all([w.e(311), w.e(29)]).then((() => () => w(311))))), i("typestyle", "2.4.0", (() => w.e(114).then((() => () => w(114)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        j.g.importScripts && (e = j.g.location + "");
-        var r = j.g.document;
+        w.g.importScripts && (e = w.g.location + "");
+        var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
-            var u = r[n],
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var n = e[a],
+                o = (typeof n)[0];
+            if (a >= r.length) return "u" == o;
+            var u = r[a],
                 i = (typeof u)[0];
-            if (a != i) return "o" == a && "n" == i || "s" == i || "u" == a;
-            if ("o" != a && "u" != a && o != u) return o < u;
-            n++
+            if (o != i) return "o" == o && "n" == i || "s" == i || "u" == o;
+            if ("o" != o && "u" != o && n != u) return n < u;
+            a++
         }
-    }, o = e => {
+    }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(i = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, i);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(i = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, i);
             return t
         }
         var u = [];
-        for (a = 1; a < e.length; a++) {
-            var i = e[a];
-            u.push(0 === i ? "not(" + l() + ")" : 1 === i ? "(" + l() + " || " + l() + ")" : 2 === i ? u.pop() + " " + u.pop() : o(i))
+        for (o = 1; o < e.length; o++) {
+            var i = e[o];
+            u.push(0 === i ? "not(" + l() + ")" : 1 === i ? "(" + l() + " || " + l() + ")" : 2 === i ? u.pop() + " " + u.pop() : n(i))
         }
         return l();
 
         function l() {
             return u.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
+            var a = e[0],
+                n = a < 0;
+            n && (a = -a - 1);
             for (var u = 0, i = 1, l = !0;; i++, u++) {
-                var s, d, f = i < e.length ? (typeof e[i])[0] : "";
-                if (u >= r.length || "o" == (d = (typeof(s = r[u]))[0])) return !l || ("u" == f ? i > n && !o : "" == f != o);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
+                var s, f, c = i < e.length ? (typeof e[i])[0] : "";
+                if (u >= r.length || "o" == (f = (typeof(s = r[u]))[0])) return !l || ("u" == c ? i > a && !n : "" == c != n);
+                if ("u" == f) {
+                    if (!l || "u" != c) return !1
                 } else if (l)
-                    if (f == d)
-                        if (i <= n) {
+                    if (c == f)
+                        if (i <= a) {
                             if (s != e[i]) return !1
                         } else {
-                            if (o ? s > e[i] : s < e[i]) return !1;
+                            if (n ? s > e[i] : s < e[i]) return !1;
                             s != e[i] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (o || i <= n) return !1;
+                else if ("s" != c && "n" != c) {
+                    if (n || i <= a) return !1;
                     l = !1, i--
                 } else {
-                    if (i <= n || d < f != o) return !1;
+                    if (i <= a || f < c != n) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, i--)
+                } else "s" != c && "n" != c && (l = !1, i--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var d = [],
+            p = d.pop.bind(d);
         for (u = 1; u < e.length; u++) {
             var h = e[u];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            d.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
         return !!p()
     }, u = (e, r) => {
-        var t = j.S[e];
-        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = w.S[e];
+        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, i = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
-        var o = i(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
-    }, d = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, o) {
-        var a = j.I(r);
-        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
-    })(((e, r, t, n) => (u(e, t), s(r, 0, t, n)))), h = c(((e, r, t, n, o) => {
-        var a = r && j.o(r, t) && d(r, t, n);
-        return a ? f(a) : o()
-    })), v = {}, g = {
-        840: () => p("default", "@lumino/signaling", [1, 1, 10, 0]),
-        95: () => h("default", "typestyle", [1, 2, 4, 0], (() => j.e(114).then((() => () => j(114))))),
-        169: () => p("default", "@jupyterlab/statusbar", [1, 3, 6, 1]),
-        258: () => p("default", "@jupyterlab/services", [1, 6, 6, 1]),
-        271: () => p("default", "react", [1, 17, 0, 1]),
-        431: () => p("default", "@lumino/widgets", [1, 1, 37, 1]),
-        442: () => p("default", "@jupyterlab/translation", [1, 3, 6, 1]),
-        468: () => p("default", "@jupyterlab/console", [1, 3, 6, 1]),
-        510: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
-        591: () => p("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
-        722: () => h("default", "@lumino/polling", [1, 1, 11, 3], (() => Promise.all([j.e(361), j.e(526)]).then((() => () => j(361))))),
-        767: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 1]),
-        866: () => p("default", "@jupyterlab/application", [1, 3, 6, 1]),
-        886: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 1]),
-        526: () => p("default", "@lumino/coreutils", [1, 1, 11, 0])
-    }, b = {
-        428: [95, 169, 258, 271, 431, 442, 468, 510, 591, 722, 767, 866, 886],
-        526: [526],
-        840: [840]
-    }, j.f.consumes = (e, r) => {
-        j.o(b, e) && b[e].forEach((e => {
-            if (j.o(v, e)) return r.push(v[e]);
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", s = (e, r, t, a) => {
+        var n = i(e, t);
+        return o(a, n) || c(l(e, t, n, a)), d(e[t][n])
+    }, f = (e, r, t) => {
+        var n = e[r];
+        return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
+    }, c = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, d = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
+        var o = w.I(r);
+        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, a, n)) : e(r, w.S[r], t, a, n)
+    })(((e, r, t, a) => (u(e, t), s(r, 0, t, a)))), v = p(((e, r, t, a, n) => {
+        var o = r && w.o(r, t) && f(r, t, a);
+        return o ? d(o) : n()
+    })), b = {}, g = {
+        29: () => h("default", "react", [1, 18, 2, 0]),
+        4: () => h("default", "@jupyterlab/application", [1, 4, 0, 3]),
+        95: () => v("default", "typestyle", [1, 2, 4, 0], (() => w.e(114).then((() => () => w(114))))),
+        172: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 3]),
+        354: () => h("default", "@jupyterlab/translation", [1, 4, 0, 3]),
+        580: () => h("default", "@jupyterlab/ui-components", [1, 4, 0, 3]),
+        663: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 3]),
+        686: () => v("default", "react-sparklines", [1, 1, 7, 0], (() => w.e(311).then((() => () => w(311))))),
+        760: () => h("default", "@jupyterlab/statusbar", [1, 4, 0, 3]),
+        778: () => h("default", "@lumino/widgets", [1, 2, 0, 1]),
+        787: () => h("default", "@jupyterlab/console", [1, 4, 0, 3]),
+        790: () => h("default", "@jupyterlab/services", [1, 7, 0, 3]),
+        797: () => h("default", "@lumino/polling", [1, 2, 0, 0]),
+        861: () => h("default", "@jupyterlab/notebook", [1, 4, 0, 3]),
+        901: () => h("default", "@lumino/signaling", [1, 2, 0, 0]),
+        987: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 3])
+    }, y = {
+        29: [29],
+        291: [4, 95, 172, 354, 580, 663, 686, 760, 778, 787, 790, 797, 861, 901, 987]
+    }, w.f.consumes = (e, r) => {
+        w.o(y, e) && y[e].forEach((e => {
+            if (w.o(b, e)) return r.push(b[e]);
             var t = r => {
-                    v[e] = 0, j.m[e] = t => {
-                        delete j.c[e], t.exports = r()
+                    b[e] = 0, w.m[e] = t => {
+                        delete w.c[e], t.exports = r()
                     }
                 },
-                n = r => {
-                    delete v[e], j.m[e] = t => {
-                        throw delete j.c[e], r
+                a = r => {
+                    delete b[e], w.m[e] = t => {
+                        throw delete w.c[e], r
                     }
                 };
             try {
-                var o = g[e]();
-                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
+                var n = g[e]();
+                n.then ? r.push(b[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
-                n(e)
+                a(e)
             }
         }))
     }, (() => {
         var e = {
             461: 0
         };
-        j.f.j = (r, t) => {
-            var n = j.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
-                else if (/^(526|840)$/.test(r)) e[r] = 0;
-            else {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = j.p + j.u(r),
+        w.f.j = (r, t) => {
+            var a = w.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
+                else if (29 != r) {
+                var n = new Promise(((t, n) => a = e[r] = [t, n]));
+                t.push(a[2] = n);
+                var o = w.p + w.u(r),
                     u = new Error;
-                j.l(a, (t => {
-                    if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        u.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", u.name = "ChunkLoadError", u.type = o, u.request = a, n[1](u)
+                w.l(o, (t => {
+                    if (w.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                        var n = t && ("load" === t.type ? "missing" : t.type),
+                            o = t && t.target && t.target.src;
+                        u.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", u.name = "ChunkLoadError", u.type = n, u.request = o, a[1](u)
                     }
                 }), "chunk-" + r, r)
-            }
+            } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [a, u, i] = t,
+                var a, n, [o, u, i] = t,
                     l = 0;
-                if (a.some((r => 0 !== e[r]))) {
-                    for (n in u) j.o(u, n) && (j.m[n] = u[n]);
-                    i && i(j)
+                if (o.some((r => 0 !== e[r]))) {
+                    for (a in u) w.o(u, a) && (w.m[a] = u[a]);
+                    i && i(w)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < o.length; l++) n = o[l], w.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_jupyter_server_resource_usage = self.webpackChunk_jupyter_server_resource_usage || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), j.nc = void 0;
-    var w = j(357);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-server/resource-usage"] = w
+    })(), w.nc = void 0;
+    var S = w(357);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-server/resource-usage"] = S
 })();
```

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/labextension/static/third-party-licenses.json` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/labextension/static/third-party-licenses.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8125%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.8.1'}, 3: {'versionInfo': '3.3.3'}, insert: [(2, "*

 * *               "OrderedDict([('name', 'react-sparklines'), ('versionInfo', '1.7.0'), ('licenseId', "*

 * *               "'MIT'), ('extractedText', 'The MIT License (MIT)\\n\\nCopyright (c) 2015 Boris "*

 * *               'Yankov\\n\\nPermission is hereby granted, free of charge, to any person obtaining '*

 * *               'a copy\\nof this software and associated documentation files (the "Software"), to '*

 * *               'deal\\ni […]*

```diff
@@ -1,32 +1,32 @@
 {
     "packages": [
         {
-            "extractedText": "",
-            "licenseId": "BSD-3-Clause",
-            "name": "@lumino/polling",
-            "versionInfo": "1.11.4"
-        },
-        {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.8.1"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014 Blake Embrey (hello@blakeembrey.com)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "free-style",
             "versionInfo": "3.1.0"
         },
         {
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015 Boris Yankov\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n",
+            "licenseId": "MIT",
+            "name": "react-sparklines",
+            "versionInfo": "1.7.0"
+        },
+        {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.3"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2016 typestyle\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "typestyle",
             "versionInfo": "2.4.0"
         }
```

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/static/main.js` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/static/main.js`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/jupyter_resource_usage/tests/test_basic.py` & `jupyter_resource_usage-1.0.0/jupyter_resource_usage/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/LICENSE` & `jupyter_resource_usage-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_resource_usage-0.7.2/pyproject.toml` & `jupyter_resource_usage-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [build-system]
 requires = [
-    "hatchling",
-    "jupyterlab~=3.0",
+    "hatchling>=1.5.0",
+    "jupyterlab>=4.0,<5",
+    "pip",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter-resource-usage"
 description = "Jupyter Extension to show resource usage"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
     { name = "Jupyter Development Team" },
 ]
 keywords = [
     "IPython",
     "Jupyter",
     "JupyterLab",
 ]
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
-    "Framework :: Jupyter :: JupyterLab :: 3",
+    "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "jupyter_server>=1.0",
+    "jupyter_server>=2.0",
     "prometheus_client",
     "psutil~=5.6",
     "pyzmq>=19",
 ]
 dynamic = ["version"]
 
 [project.license]
@@ -57,16 +57,15 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/jupyter-server/jupyter-resource-usage"
 
 [tool.hatch.build.targets.wheel.shared-data]
 "jupyter_resource_usage/static" = "share/jupyter/nbextensions/jupyter_resource_usage"
-"jupyter_resource_usage/labextension/package.json" = "share/jupyter/labextensions/@jupyter-server/resource-usage/package.json"
-"jupyter_resource_usage/labextension/static" = "share/jupyter/labextensions/@jupyter-server/resource-usage/static"
+"jupyter_resource_usage/labextension" = "share/jupyter/labextensions/@jupyter-server/resource-usage"
 "install.json" = "share/jupyter/labextensions/@jupyter-server/resource-usage/install.json"
 "jupyter-config/jupyter_server_config.d" = "etc/jupyter/jupyter_server_config.d"
 "jupyter-config/jupyter_notebook_config.d" = "etc/jupyter/jupyter_notebook_config.d"
 "jupyter-config/nbconfig/notebook.d" = "etc/jupyter/nbconfig/notebook.d"
 
 [tool.hatch.version]
 path = "jupyter_resource_usage/_version.py"
@@ -84,31 +83,28 @@
     "jupyter_resource_usage/labextension/static/style.js",
     "jupyter_resource_usage/labextension/package.json",
 ]
 skip-if-exists = [
     "jupyter_resource_usage/labextension/static/style.js",
 ]
 
-[tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
+[tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 build_cmd = "build:prod"
 npm = [
     "jlpm",
 ]
-force = true
 
-[tool.hatch.build.hooks.jupyter-builder.build-kwargs]
-build_cmd = "build:prod"
+[tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
+build_cmd = "build"
 npm = [
     "jlpm",
 ]
-source_dir = "packages/labextension"
-build_dir = "jupyter_resource_usage/labextension"
 
 [tool.tbump.version]
-current = "0.7.2"
+current = "1.0.0"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
@@ -126,15 +122,15 @@
 
 [[tool.tbump.field]]
 name = "release"
 default = ""
 
 [tool.jupyter-releaser.hooks]
 before-build-npm = [
-    "python -m pip install jupyterlab~=3.0",
+    "python -m pip install jupyterlab~=4.0",
     "jlpm",
     "jlpm clean",
     "jlpm build:prod",
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W002", "W004"]
```

### Comparing `jupyter_resource_usage-0.7.2/PKG-INFO` & `jupyter_resource_usage-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-resource-usage
-Version: 0.7.2
+Version: 1.0.0
 Summary: Jupyter Extension to show resource usage
 Project-URL: Homepage, https://github.com/jupyter-server/jupyter-resource-usage
 Author: Jupyter Development Team
 License: Copyright (c) 2016, Yuvi Panda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -27,29 +27,28 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Keywords: IPython,Jupyter,JupyterLab
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: jupyter-server>=1.0
+Requires-Python: >=3.8
+Requires-Dist: jupyter-server>=2.0
 Requires-Dist: prometheus-client
 Requires-Dist: psutil~=5.6
 Requires-Dist: pyzmq>=19
 Provides-Extra: dev
 Requires-Dist: autopep8; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
@@ -62,44 +61,79 @@
 **[Configuration](#configuration)** |
 **[Resources Displayed](#resources-displayed)** |
 **[Contributing](#contributing)**
 
 # jupyter-resource-usage
 
 ![Github Actions Status](https://github.com/jupyter-server/jupyter-resource-usage/workflows/Tests/badge.svg)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyter-resource-usage/master)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyter-resource-usage/main)
 [![PyPI](https://img.shields.io/pypi/v/jupyter-resource-usage)](https://pypi.python.org/pypi/jupyter-resource-usage)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/jupyter-resource-usage.svg)](https://anaconda.org/conda-forge/jupyter-resource-usage)
 [![PyPI](https://img.shields.io/pypi/l/jupyter-resource-usage)](https://pypi.python.org/pypi/jupyter-resource-usage)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/jupyter-server/jupyter-resource-usage/issues)
 
-![Screenshot with memory limit](screenshot.png)
+![Screenshot with memory limit](./doc/statusbar.png)
 
 Jupyter Resource Usage is an extension for Jupyter Notebooks and JupyterLab that
 displays an indication of how much resources your current notebook server and
 its children (kernels, terminals, etc) are using. This is displayed in the
-main toolbar in the notebook itself, refreshing every 5s.
+status bar in the JupyterLab and notebook, refreshing every 5s.
 
 Kernel resource usage can be displayed in a sidebar for IPython kernels with
 [ipykernel](https://github.com/ipython/ipykernel) >= 6.11.0.
 
+![Screenshot for kernel usage](./doc/kernel-usage.png)
+
+The kernel usage is available for Notebook 7.x too which can be enabled at
+`View -> Right Sidebar -> Show Kernel Usage`. In the case of JupyterLab interface, it is
+enough to click `tachometer` icon on the right sidebar.
+
+The package provides an alternative frontend for the `jupyter-resource-usage` metrics:
+
+![screencast](./doc/topbar.gif)
+
+Previously, this extension used to be distributed with
+[jupyterlab-system-monitor](https://github.com/jtpio/jupyterlab-system-monitor) package.
+Starting from `1.0.0`, the alternative frontend has been integrated into the
+current repository. Check [Alternative frontend](#enable-alternative-frontend) section
+on how to enable and configure this alternative frontend.
+
+**Note** that for JupyterLab 3.x and 2.x, users should install the alternative frontend
+from [jupyterlab-system-monitor](https://github.com/jtpio/jupyterlab-system-monitor).
+
 ## Installation
 
-You can currently install this package from PyPI.
+### JupyterLab 4.x and Notebook 7.x
+
+You should install the latest version `>=1.0.0` for JupyterLab 4 compatability.
 
 ```bash
 pip install jupyter-resource-usage
 ```
 
 Or with `conda`:
 
 ```bash
 conda install -c conda-forge jupyter-resource-usage
 ```
 
+### JupyterLab 3.x and Notebook 6.x
+
+You should pin the versions to `<1.0.0`
+
+```bash
+pip install 'jupyter-resource-usage<1.0.0'
+```
+
+Or with `conda`:
+
+```bash
+conda install -c conda-forge 'jupyter-resource-usage<1.0.0'
+```
+
 **If your notebook version is < 5.3**, you need to enable the extension manually.
 
 ```
 jupyter serverextension enable --py jupyter_resource_usage --sys-prefix
 jupyter nbextension install --py jupyter_resource_usage --sys-prefix
 jupyter nbextension enable --py jupyter_resource_usage --sys-prefix
 ```
@@ -116,15 +150,15 @@
 2. In the commandline when starting `jupyter notebook`, as `--ResourceUseDisplay.mem_limit`.
 3. In your Jupyter notebook [traitlets](https://traitlets.readthedocs.io/en/stable/) config file
 
 The limit needs to be set as an integer in Bytes.
 
 ### Memory usage warning threshold
 
-![Screenshot with memory warning](warn-screenshot.png)
+![Screenshot with memory warning](./doc/statusbar-warn.png)
 
 The background of the resource display can be changed to red when the user is near a memory limit.
 The threshold for this warning can be configured as a fraction of the memory limit.
 
 If you want to flash the warning to the user when they are within 10% of the memory limit, you
 can set the parameter `--ResourceUseDisplay.mem_warning_threshold=0.1`.
 
@@ -150,23 +184,42 @@
 
 As a command line argument:
 
 ```bash
 jupyter notebook --ResourceUseDisplay.track_cpu_percent=True
 ```
 
+When `track_cpu_percent` is set to `True`, status will report CPU utilisation along with
+memory:
+
+![Screenshot with CPU and memory](./doc/statusbar-cpu.png)
+
 ### Disable Prometheus Metrics
 
 There is a [known bug](https://github.com/jupyter-server/jupyter-resource-usage/issues/123) with Prometheus metrics which
 causes "lag"/pauses in the UI. To workaround this you can disable Prometheus metric reporting using:
 
 ```
 --ResourceUseDisplay.enable_prometheus_metrics=False
 ```
 
+## Enable alternative frontend
+
+By default, the alternative frontend is disabled. To enable it, users should go to
+`Settings -> Settings Editor -> Resource Usage Indicator` which will render following
+form
+
+![jupyterlab_setting](./doc/settings.png)
+
+By checking "Enable resource usage indicators" and refreshing the browser tab will
+render the alternative frontend in the topbar.
+
+Users can change the label and refresh rate for the alternative frontend using settings
+editor.
+
 ## Resources Displayed
 
 Currently the server extension only reports memory usage and CPU usage. Other metrics will be added in the future as needed.
 
 Memory usage will show the PSS whenever possible (Linux only feature), and default to RSS otherwise.
 
 The notebook extension currently doesn't show CPU usage, only memory usage.
```

