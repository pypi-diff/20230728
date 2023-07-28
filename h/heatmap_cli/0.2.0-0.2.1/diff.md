# Comparing `tmp/heatmap_cli-0.2.0.tar.gz` & `tmp/heatmap_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatmap_cli-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "heatmap_cli-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `heatmap_cli-0.2.0.tar` & `heatmap_cli-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      146 2023-07-19 03:38:50.545154 heatmap_cli-0.2.0/.coveragerc
--rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/.gitignore
--rw-r--r--   0        0        0     2589 2023-07-19 03:34:58.303707 heatmap_cli-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/.prettierignore
--rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/.python-version
--rw-r--r--   0        0        0     1338 2023-07-23 13:16:55.486422 heatmap_cli-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1967 2023-07-22 05:51:16.547471 heatmap_cli-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/LICENSE.md
--rw-r--r--   0        0        0      509 2023-07-21 00:25:50.551442 heatmap_cli-0.2.0/Pipfile
--rw-r--r--   0        0        0   126616 2023-07-22 05:38:41.247816 heatmap_cli-0.2.0/Pipfile.lock
--rw-r--r--   0        0        0     2154 2023-07-19 10:02:05.708726 heatmap_cli-0.2.0/README.md
--rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0      779 2023-07-23 13:17:18.614611 heatmap_cli-0.2.0/heatmap_cli/__init__.py
--rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.2.0/heatmap_cli/__main__.py
--rw-r--r--   0        0        0     6792 2023-07-19 10:08:43.813639 heatmap_cli-0.2.0/heatmap_cli/cli.py
--rw-r--r--   0        0        0     1077 2023-07-17 23:52:03.000872 heatmap_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.2.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      358 2023-07-19 03:58:00.025209 heatmap_cli-0.2.0/tests/test_debug_flag.py
--rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.2.0/tests/test_help_flag.py
--rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.2.0/tests/test_verbose_flag.py
--rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.2.0/tests/test_version_flag.py
--rw-r--r--   0        0        0      306 2023-07-19 23:00:14.071564 heatmap_cli-0.2.0/tests/test_week_flag.py
--rw-r--r--   0        0        0      516 2023-07-19 03:33:39.924975 heatmap_cli-0.2.0/tests/test_year_flag.py
--rw-r--r--   0        0        0      682 2023-07-22 05:50:59.467336 heatmap_cli-0.2.0/tox.ini
--rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 heatmap_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      194 2023-07-26 03:15:34.005426 heatmap_cli-0.2.1/.coveragerc
+-rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/.gitignore
+-rw-r--r--   0        0        0     2589 2023-07-19 03:34:58.303707 heatmap_cli-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/.prettierignore
+-rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/.python-version
+-rw-r--r--   0        0        0     1570 2023-07-28 02:24:37.938195 heatmap_cli-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1967 2023-07-22 05:51:16.547471 heatmap_cli-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0      509 2023-07-21 00:25:50.551442 heatmap_cli-0.2.1/Pipfile
+-rw-r--r--   0        0        0   126618 2023-07-24 03:36:11.870630 heatmap_cli-0.2.1/Pipfile.lock
+-rw-r--r--   0        0        0     2154 2023-07-19 10:02:05.708726 heatmap_cli-0.2.1/README.md
+-rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0      779 2023-07-28 02:24:49.394119 heatmap_cli-0.2.1/heatmap_cli/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/heatmap_cli/__main__.py
+-rw-r--r--   0        0        0     6921 2023-07-27 03:36:02.562136 heatmap_cli-0.2.1/heatmap_cli/cli.py
+-rw-r--r--   0        0        0     1077 2023-07-17 23:52:03.000872 heatmap_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      358 2023-07-19 03:58:00.025209 heatmap_cli-0.2.1/tests/test_debug_flag.py
+-rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/test_help_flag.py
+-rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/test_verbose_flag.py
+-rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.2.1/tests/test_version_flag.py
+-rw-r--r--   0        0        0      306 2023-07-19 23:00:14.071564 heatmap_cli-0.2.1/tests/test_week_flag.py
+-rw-r--r--   0        0        0      516 2023-07-19 03:33:39.924975 heatmap_cli-0.2.1/tests/test_year_flag.py
+-rw-r--r--   0        0        0      661 2023-07-26 03:15:49.357516 heatmap_cli-0.2.1/tox.ini
+-rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 heatmap_cli-0.2.1/PKG-INFO
```

### Comparing `heatmap_cli-0.2.0/.gitignore` & `heatmap_cli-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/.pre-commit-config.yaml` & `heatmap_cli-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/CHANGELOG.md` & `heatmap_cli-0.2.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.2.1 (2023-07-28)
+
+### Changed
+
+- Move `coverage` config from `tox` to its own file
+- Reset Dataframe index after filtering
+
+## Fixed
+
+- Show verbose log of last date of current week
+- Fix incorrect header level in changelog
+
 ## v0.2.0 (2023-07-23)
 
-## Added
+### Added
 
 - Add `yr` or `--year` argument to filter CSV data by year
 - Add `wk` or `--week` argument to filter CSV data until week of the year
 - Add additional pre-commit default checks
 - Show generated PNG filename upon completion
 
 ### Changed
```

### Comparing `heatmap_cli-0.2.0/CONTRIBUTING.md` & `heatmap_cli-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/LICENSE.md` & `heatmap_cli-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/Pipfile.lock` & `heatmap_cli-0.2.1/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982862903225806%*

 * *Differences: {"'develop'": "{'certifi': {'hashes': "*

 * *              "['sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082', "*

 * *              "'sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9'], "*

 * *              "'version': '==2023.7.22'}, 'dill': {'hashes': "*

 * *              "['sha256:76b122c08ef4ce2eedcd4d1abd8e641114bfc6c2867f49f3c41facf65bf19f5e', "*

 * *              "'sha256:cc1c8b182eb3013e24bd475ff2e9295af86c1a38eb1aff128dac8962a9ce3c03'], "*

 * *              "'version': '==0.3.7'}, […]*

```diff
@@ -440,19 +440,19 @@
                 "sha256:903f024859b7c7687d7a7f3a3f73b17301f8e42dfd9cc9df9d4418172d3e2dbd"
             ],
             "markers": "python_full_version >= '3.7.2'",
             "version": "==2.15.6"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -659,19 +659,19 @@
                 "sha256:9c87405839a19696e837b3b818fed3f5f69f16f1eec1a1ad77e043dcea9c772f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.11.0"
         },
         "dill": {
             "hashes": [
-                "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
-                "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
+                "sha256:76b122c08ef4ce2eedcd4d1abd8e641114bfc6c2867f49f3c41facf65bf19f5e",
+                "sha256:cc1c8b182eb3013e24bd475ff2e9295af86c1a38eb1aff128dac8962a9ce3c03"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "distlib": {
             "hashes": [
                 "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057",
                 "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"
             ],
             "version": "==0.3.7"
@@ -766,19 +766,19 @@
         },
         "heatmap-cli": {
             "editable": true,
             "path": "."
         },
         "identify": {
             "hashes": [
-                "sha256:9df2489842707d431b38ce3410ef8df40da5b10a3e28a3fcac1a42523e956409",
-                "sha256:db4de0e758c0db8f81996816cd2f3f2f8c5c8d49a7fd02f3b4109aac6fd80e29"
+                "sha256:7243800bce2f58404ed41b7c002e53d4d22bcf3ae1b7900c2d7aefd95394bf7f",
+                "sha256:c22a8ead0d4ca11f1edd6c9418c3220669b3b7533ada0a0ffa6cc0ef85cf9b54"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==2.5.25"
+            "version": "==2.5.26"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -1480,19 +1480,19 @@
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.12.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
                 "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
                 "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
                 "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
```

### Comparing `heatmap_cli-0.2.0/README.md` & `heatmap_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/docs/Makefile` & `heatmap_cli-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/docs/make.bat` & `heatmap_cli-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/docs/source/_static/logo.jpg` & `heatmap_cli-0.2.1/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/docs/source/conf.py` & `heatmap_cli-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/heatmap_cli/__init__.py` & `heatmap_cli-0.2.1/heatmap_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap."""
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `heatmap_cli-0.2.0/heatmap_cli/__main__.py` & `heatmap_cli-0.2.1/heatmap_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/heatmap_cli/cli.py` & `heatmap_cli-0.2.1/heatmap_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,18 +140,24 @@
     dataframe["week"] = dataframe["date"].dt.strftime("%W")
     dataframe["count"] = round(dataframe["count"], -2) / 100
 
     steps = dataframe[
         (dataframe["date"].dt.year == config.year)
         & (dataframe["week"] <= str(config.week).zfill(2))
     ]
+    steps.reset_index(drop=True, inplace=True)
+
     if steps.empty:
         raise ValueError("no data extracted from csv file")
 
-    _logger.debug(max(steps["date"]).date())
+    _logger.debug(
+        "last date: %s of current week: %s",
+        max(steps["date"]).date(),
+        config.week,
+    )
     missing_df = pd.DataFrame(
         {
             "date": pd.date_range(
                 start=max(steps["date"]).date() + datetime.timedelta(days=1),
                 end=f"{config.year}-12-31",
             )
         }
```

### Comparing `heatmap_cli-0.2.0/pyproject.toml` & `heatmap_cli-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/tests/conftest.py` & `heatmap_cli-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/tests/fixtures/sample.csv` & `heatmap_cli-0.2.1/tests/fixtures/sample.csv`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/tests/test_verbose_flag.py` & `heatmap_cli-0.2.1/tests/test_verbose_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/tests/test_year_flag.py` & `heatmap_cli-0.2.1/tests/test_year_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.0/tox.ini` & `heatmap_cli-0.2.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     pipenv run pytest tests
 
 [testenv:cov]
 description = generate code coverage report in html
 deps = pipenv
 commands=
     pipenv install --dev
-    pipenv run pytest tests --cov-fail-under=100 --numprocesses auto --cov=heatmap_cli --cov-report term-missing --cov-report html {toxinidir}/tests
+    pipenv run pytest tests --numprocesses auto --cov=heatmap_cli --cov-report term-missing --cov-report html {toxinidir}/tests
 
 [testenv:doc]
 description = generate sphinx documentation in html
 basepython = python3.11
 deps = pipenv
 commands =
     pipenv install --categories doc
```

### Comparing `heatmap_cli-0.2.0/PKG-INFO` & `heatmap_cli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatmap_cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A console program that generates yearly calendar heatmap.
 Keywords: heatmap,cli
 Author-email: Kian-Meng Ang <kianmeng@cpan.org>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

