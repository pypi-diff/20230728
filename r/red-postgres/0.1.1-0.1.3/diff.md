# Comparing `tmp/red-postgres-0.1.1.tar.gz` & `tmp/red-postgres-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red-postgres-0.1.1.tar", last modified: Fri Jun  2 15:00:58 2023, max compression
+gzip compressed data, was "red-postgres-0.1.3.tar", last modified: Fri Jul 28 20:00:54 2023, max compression
```

## Comparing `red-postgres-0.1.1.tar` & `red-postgres-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 15:00:58.138639 red-postgres-0.1.1/
--rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6287 2023-06-02 15:00:58.137639 red-postgres-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5750 2023-06-02 15:00:17.000000 red-postgres-0.1.1/README.md
--rw-rw-rw-   0        0        0     1630 2023-06-02 14:57:44.000000 red-postgres-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-02 15:00:58.125639 red-postgres-0.1.1/red_postgres/
--rw-rw-rw-   0        0        0      180 2023-05-29 17:18:29.000000 red-postgres-0.1.1/red_postgres/__init__.py
--rw-rw-rw-   0        0        0     5377 2023-06-02 14:57:37.000000 red-postgres-0.1.1/red_postgres/engine.py
-drwxrwxrwx   0        0        0        0 2023-06-02 15:00:58.136639 red-postgres-0.1.1/red_postgres.egg-info/
--rw-rw-rw-   0        0        0     6287 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 15:00:58.000000 red-postgres-0.1.1/red_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 15:00:58.138639 red-postgres-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 20:00:54.707491 red-postgres-0.1.3/
+-rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6287 2023-07-28 20:00:54.707491 red-postgres-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5750 2023-06-02 15:00:17.000000 red-postgres-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1583 2023-07-28 20:00:29.000000 red-postgres-0.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-28 20:00:54.686491 red-postgres-0.1.3/red_postgres/
+-rw-rw-rw-   0        0        0      235 2023-07-28 19:59:22.000000 red-postgres-0.1.3/red_postgres/__init__.py
+-rw-rw-rw-   0        0        0     5303 2023-07-17 00:55:17.000000 red-postgres-0.1.3/red_postgres/engine.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:00:54.705490 red-postgres-0.1.3/red_postgres.egg-info/
+-rw-rw-rw-   0        0        0     6287 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-28 20:00:54.000000 red-postgres-0.1.3/red_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 20:00:54.708490 red-postgres-0.1.3/setup.cfg
```

### Comparing `red-postgres-0.1.1/LICENSE` & `red-postgres-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `red-postgres-0.1.1/PKG-INFO` & `red-postgres-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.1.1
+Version: 0.1.3
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `red-postgres-0.1.1/README.md` & `red-postgres-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `red-postgres-0.1.1/pyproject.toml` & `red-postgres-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [build-system]
-requires = ["setuptools>=61.0", "discord.py>=2.2.3", "piccolo[postgres]>=0.113.0"]
+requires = [
+  "setuptools>=61.0",
+  "discord.py>=2.2.3",
+  "piccolo[postgres]>=0.113.0",
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "red-postgres"
-version = "0.1.1"
-authors = [
-  { name="Vertyco" },
-]
+version = "0.1.3"
+authors = [{ name = "Vertyco" }]
 description = "Piccolo Postgres integration for Red"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
+  "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/vertyco/red-postgres"
 "Bug Tracker" = "https://github.com/vertyco/red-postgres/issues"
 
 [tool.ruff]
@@ -28,40 +30,40 @@
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
-    ".md",
-    "locales/",
-    "tests/",
-    "defaults.py",
-    ".idea",
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
+  ".md",
+  "locales/",
+  "tests/",
+  "defaults.py",
+  ".idea",
+  ".bzr",
+  ".direnv",
+  ".eggs",
+  ".git",
+  ".hg",
+  ".mypy_cache",
+  ".nox",
+  ".pants.d",
+  ".ruff_cache",
+  ".svn",
+  ".tox",
+  ".venv",
+  "__pypackages__",
+  "_build",
+  "buck-out",
+  "build",
+  "dist",
+  "node_modules",
+  "venv",
 ]
-per-file-ignores = { }
+per-file-ignores = {}
 
 line-length = 88
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 target-version = "py311"
```

### Comparing `red-postgres-0.1.1/red_postgres/engine.py` & `red-postgres-0.1.3/red_postgres/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,14 @@
     """Registers a cog by creating a database for it and initializing any tables it has
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
         max_size (int): maximum number of database connections, 20 by default
-        make (bool): automatically make new migrations, False by default
 
     Returns:
         PostgresEngine
     """
     # Create databse under root folder name
     await create_database(cog, config)
     # Run any migrations
```

### Comparing `red-postgres-0.1.1/red_postgres.egg-info/PKG-INFO` & `red-postgres-0.1.3/red_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.1.1
+Version: 0.1.3
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
```

