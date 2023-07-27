# Comparing `tmp/pkgmt-0.7.1.tar.gz` & `tmp/pkgmt-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.7.1.tar", last modified: Fri Jul 14 14:44:54 2023, max compression
+gzip compressed data, was "pkgmt-0.7.2.tar", last modified: Thu Jul 27 22:00:49 2023, max compression
```

## Comparing `pkgmt-0.7.1.tar` & `pkgmt-0.7.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-14 14:44:38.000000 pkgmt-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-14 14:44:38.000000 pkgmt-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-14 14:44:38.000000 pkgmt-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-14 14:44:54.720089 pkgmt-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 14:44:38.000000 pkgmt-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 14:44:38.000000 pkgmt-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 14:44:54.720089 pkgmt-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-14 14:44:38.000000 pkgmt-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.712089 pkgmt-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.716089 pkgmt-0.7.1/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.716089 pkgmt-0.7.1/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.712089 pkgmt-0.7.1/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/src/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/src/package_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/fail_if_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/fail_if_not_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioner/versioner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.716089 pkgmt-0.7.1/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.093568 pkgmt-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-27 22:00:32.000000 pkgmt-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 22:00:32.000000 pkgmt-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 22:00:32.000000 pkgmt-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-27 22:00:49.093568 pkgmt-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-27 22:00:32.000000 pkgmt-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 22:00:32.000000 pkgmt-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 22:00:49.093568 pkgmt-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-27 22:00:32.000000 pkgmt-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.085569 pkgmt-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.089568 pkgmt-0.7.2/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.089568 pkgmt-0.7.2/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.089568 pkgmt-0.7.2/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.093568 pkgmt-0.7.2/src/pkgmt/assets/template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.093568 pkgmt-0.7.2/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.085569 pkgmt-0.7.2/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.093568 pkgmt-0.7.2/src/pkgmt/assets/template/src/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/src/package_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.093568 pkgmt-0.7.2/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/fail_if_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/fail_if_not_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.093568 pkgmt-0.7.2/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-27 22:00:32.000000 pkgmt-0.7.2/src/pkgmt/versioner/versioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:00:49.089568 pkgmt-0.7.2/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-27 22:00:48.000000 pkgmt-0.7.2/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-27 22:00:48.000000 pkgmt-0.7.2/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:00:48.000000 pkgmt-0.7.2/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 22:00:48.000000 pkgmt-0.7.2/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 22:00:48.000000 pkgmt-0.7.2/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 22:00:48.000000 pkgmt-0.7.2/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.7.1/CHANGELOG.md` & `pkgmt-0.7.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # CHANGELOG
 
+## 0.7.2 (2023-07-27)
+
+* [Feature] Added `push` and `tag` versioner configuration keys to `pyproject.toml` ([#63](https://github.com/ploomber/pkgmt/issues/63))
+
 ## 0.7.1 (2023-07-14)
 
 * [Fix] Fixed `black` `--extend-exclude` override in `pyproject.toml`([#66](https://github.com/ploomber/pkgmt/issues/66))
+* [Fix] Validation of keys in `pyproject.toml` ([#65](https://github.com/ploomber/pkgmt/issues/65))
 
 ## 0.7.0 (2023-07-11)
 
 * [API Change] Support for projects containing `version` key in `pyproject.toml`. ([#58](https://github.com/ploomber/pkgmt/issues/58))
 * [Fix] Fix bug when running git hook
 * [Fix] Proper error message when version file is empty, or version string not found. Display version file location when inconsistent version in changelog ([#64](https://github.com/ploomber/pkgmt/issues/64))
```

### Comparing `pkgmt-0.7.1/LICENSE` & `pkgmt-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/README.md` & `pkgmt-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/setup.py` & `pkgmt-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/assets/template/.github/pull_request_template.md` & `pkgmt-0.7.2/src/pkgmt/assets/template/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/assets/template/.github/workflows/ci.yml` & `pkgmt-0.7.2/src/pkgmt/assets/template/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.7.2/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/assets/template/pyproject.toml` & `pkgmt-0.7.2/src/pkgmt/assets/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/assets/template/setup.py` & `pkgmt-0.7.2/src/pkgmt/assets/template/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.7.2/src/pkgmt/assets/template/tasks.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/assets/template/tests/conftest.py` & `pkgmt-0.7.2/src/pkgmt/assets/template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/changelog.py` & `pkgmt-0.7.2/src/pkgmt/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     pattern = r"(?<!\[)@([\w\-_]+)(?!\]\(https:\/\/github\.com\/\w+\))"
     repl = r"[\g<0>](https://github.com/\g<1>)"
     return re.sub(pattern, repl, text)
 
 
 def _expand_github_from_text(text):
     """Convert strings with the #{number} format into their"""
-    cfg = config.load()
+    cfg = config.Config.from_file("pyproject.toml")
     url = f'https://github.com/{cfg["github"]}/issues/'
     return _replace_handles_with_links(_replace_issue_number_with_links(url, text))
 
 
 def expand_github_from_changelog(path="CHANGELOG.md"):
     path = Path(path)
     changelog = path.read_text()
```

### Comparing `pkgmt-0.7.1/src/pkgmt/cli.py` & `pkgmt-0.7.2/src/pkgmt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     default=False,
     help="Only consider 404 code as broken",
 )
 def check_links(only_404):
     """Check for broken links"""
     broken_http_codes = None if not only_404 else [404]
 
-    cfg = config.load()["check_links"]
+    cfg = config.Config.from_file("pyproject.toml")["check_links"]
     out = links.find_broken_in_files(
         cfg["extensions"],
         cfg.get("ignore_substrings"),
         verbose=True,
         broken_http_codes=broken_http_codes,
     )
 
@@ -91,20 +91,29 @@
 @cli.command()
 @click.option(
     "--yes",
     is_flag=True,
     default=False,
     help="Do not ask for confirmation",
 )
-@click.option("--push/--no-push", default=True)
-@click.option("--tag/--no-tag", default=True)
+@click.option("--push/--no-push", default=None)
+@click.option("--tag/--no-tag", default=None)
 @click.option("--target", default=None)
 def version(yes, push, tag, target):
     """Create a new package version"""
-    versioneer.version(project_root=".", tag=tag, yes=yes, push=push, target=target)
+
+    cfg = config.Config.from_file("pyproject.toml", cli_args=dict(push=push, tag=tag))
+
+    versioneer.version(
+        project_root=".",
+        tag=cfg["version"]["tag"],
+        yes=yes,
+        push=cfg["version"]["push"],
+        target=target,
+    )
 
 
 @cli.command()
 @click.argument("tag")
 @click.option(
     "--production",
     is_flag=True,
```

### Comparing `pkgmt-0.7.1/src/pkgmt/dependencies.py` & `pkgmt-0.7.2/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/deprecation.py` & `pkgmt-0.7.2/src/pkgmt/deprecation.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/dev.py` & `pkgmt-0.7.2/src/pkgmt/dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import platform
 import os
 import shutil
 from pathlib import Path
 
 from invoke import task
-from pkgmt.config import load
+from pkgmt.config import Config
 
 community = "https://ploomber.io/community"
 
 
 class CommandError(SystemExit):
     def __init__(self, msg) -> None:
         super().__init__(
@@ -39,15 +39,15 @@
     Setup dev environment, requires conda
     """
     _check()
 
     if not shutil.which("conda"):
         raise CommandError("conda not installed. Install it an try again.")
 
-    cfg = load()
+    cfg = Config.from_file("pyproject.toml")
 
     env_prefix = cfg.get("env_name", cfg["package_name"])
     pkg_name = cfg["package_name"]
 
     version = version or "3.10"
     suffix = "" if version == "3.10" else version.replace(".", "")
     env_name = f"{env_prefix}{suffix}"
```

### Comparing `pkgmt-0.7.1/src/pkgmt/fail_if_modified.py` & `pkgmt-0.7.2/src/pkgmt/fail_if_modified.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/fail_if_not_modified.py` & `pkgmt-0.7.2/src/pkgmt/fail_if_not_modified.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/formatting.py` & `pkgmt-0.7.2/src/pkgmt/formatting.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/github.py` & `pkgmt-0.7.2/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/hook.py` & `pkgmt-0.7.2/src/pkgmt/hook.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/links.py` & `pkgmt-0.7.2/src/pkgmt/links.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/new.py` & `pkgmt-0.7.2/src/pkgmt/new.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/test.py` & `pkgmt-0.7.2/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/versioneer.py` & `pkgmt-0.7.2/src/pkgmt/versioneer.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt/versioner/util.py` & `pkgmt-0.7.2/src/pkgmt/versioner/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import os
 import click
 import warnings
 from pathlib import Path
-from pkgmt.config import load
+from pkgmt.config import Config
 
 
 def is_pre_release(version):
     return "a" in version or "b" in version or "rc" in version
 
 
 def is_major_version(version):
@@ -134,15 +134,15 @@
     """
     Function to find the path of the package containing the
     version file. If version_file key is found in pyproject.toml
     file, this path is considered as the path to the version file.
     Else version file in __init__.py found in the first package
     inside src directory.
     """
-    cfg = load()
+    cfg = Config.from_file("pyproject.toml")
     version_file = cfg.get("version", {}).get("version_file", None)
     validate_version_file(version_file)
     if version_file:
         package_name, PACKAGE, version_file_name = find_package_of_version_file(
             version_file, project_root
         )
     else:
```

### Comparing `pkgmt-0.7.1/src/pkgmt/versioner/versioner.py` & `pkgmt-0.7.2/src/pkgmt/versioner/versioner.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.1/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.7.2/src/pkgmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

