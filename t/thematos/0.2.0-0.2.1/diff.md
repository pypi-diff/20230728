# Comparing `tmp/thematos-0.2.0.tar.gz` & `tmp/thematos-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thematos-0.2.0.tar", max compression
+gzip compressed data, was "thematos-0.2.1.tar", max compression
```

## Comparing `thematos-0.2.0.tar` & `thematos-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-07-27 09:00:53.178073 thematos-0.2.0/LICENSE
--rw-r--r--   0        0        0     2112 2023-07-27 09:00:53.178073 thematos-0.2.0/README.md
--rw-r--r--   0        0        0     2879 2023-07-27 09:01:19.226149 thematos-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/__init__.py
--rw-r--r--   0        0        0       21 2023-07-27 09:01:19.186149 thematos-0.2.0/src/thematos/_version.py
--rw-r--r--   0        0        0        0 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/conf/__init__.py
--rw-r--r--   0        0        0      179 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/conf/about/thematos.yaml
--rw-r--r--   0        0        0        0 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/conf/topic/__init__.yaml
--rw-r--r--   0        0        0      197 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/project.toml
--rw-r--r--   0        0        0        0 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/py.typed
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 thematos-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-28 06:55:54.395306 thematos-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2112 2023-07-28 06:55:54.395306 thematos-0.2.1/README.md
+-rw-r--r--   0        0        0     3118 2023-07-28 06:56:20.383753 thematos-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-28 06:56:20.339752 thematos-0.2.1/src/thematos/_version.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/conf/__init__.py
+-rw-r--r--   0        0        0      179 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/conf/about/thematos.yaml
+-rw-r--r--   0        0        0        0 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/conf/topic/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-28 06:55:54.395306 thematos-0.2.1/src/thematos/py.typed
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 thematos-0.2.1/PKG-INFO
```

### Comparing `thematos-0.2.0/LICENSE` & `thematos-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thematos-0.2.0/README.md` & `thematos-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `thematos-0.2.0/pyproject.toml` & `thematos-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "thematos"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python Library for Topic Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://thematos.entelecheia.ai"
 repository = "https://github.com/entelecheia/thematos"
 readme = "README.md"
 packages = [{ include = "thematos", from = "src" }]
 
 [tool.poetry.scripts]
 thematos = 'thematos.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.11.0"
+hyfi = "^1.12.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
@@ -30,28 +30,65 @@
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe]
 include = [".tasks.toml", ".tasks-extra.toml"]
 
 [tool.black]
-exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+exclude = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.isort]
 profile = "black"
-skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
+skip = [
+    '_version.py',
+    'node_modules',
+    '_build',
+    'docs',
+    'tests',
+    'venv',
+    '.copier-template',
+    '.refs',
+]
 
 [tool.flake8]
 ignore = ['F401', 'E501', 'W503']
-exclude = ["node_modules", "_build", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "_build",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+    "workspace",
+]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
-exclude = ["node_modules", "build", "_build", "dist", "docs", "tests", "venv", ".copier-template", ".refs"]
+exclude = [
+    "node_modules",
+    "build",
+    "_build",
+    "dist",
+    "docs",
+    "tests",
+    "venv",
+    ".copier-template",
+    ".refs",
+]
 # 3rd party import
 ignore_missing_imports = true
 # dynamic typing
 disallow_any_unimported = true
 disallow_any_expr = false
 disallow_any_decorated = false
 disallow_any_explicit = true
@@ -84,22 +121,21 @@
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/thematos/_version.py:__version__"
 version_source = "tag"
-commit_version_number = true # required for version_source = "tag"
+commit_version_number = true                                    # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-hvcs = "github" # hosting version control system, gitlab is also supported
+hvcs = "github"                                                 # hosting version control system, gitlab is also supported
 build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `thematos-0.2.0/PKG-INFO` & `thematos-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: thematos
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python Library for Topic Modeling
 Home-page: https://thematos.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=1.11.0,<2.0.0)
+Requires-Dist: hyfi (>=1.12.0,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/thematos
 Description-Content-Type: text/markdown
 
 # ThematOS
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

