# Comparing `tmp/seagoat-0.5.6.tar.gz` & `tmp/seagoat-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.5.6.tar", max compression
+gzip compressed data, was "seagoat-0.6.0.tar", max compression
```

## Comparing `seagoat-0.5.6.tar` & `seagoat-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-28 11:20:56.366351 seagoat-0.5.6/LICENSE
--rw-r--r--   0        0        0      957 2023-07-28 11:20:56.366351 seagoat-0.5.6/README.md
--rw-r--r--   0        0        0     3056 2023-07-28 11:20:57.306421 seagoat-0.5.6/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/cache.py
--rw-r--r--   0        0        0     2859 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/common.py
--rw-r--r--   0        0        0     4512 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/result.py
--rw-r--r--   0        0        0     5624 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/server.py
--rw-r--r--   0        0        0     1878 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1210 2023-07-28 11:20:56.374351 seagoat-0.5.6/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 seagoat-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-28 14:24:18.425915 seagoat-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1847 2023-07-28 14:24:18.425915 seagoat-0.6.0/README.md
+-rw-r--r--   0        0        0     3084 2023-07-28 14:24:19.461926 seagoat-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/cache.py
+-rw-r--r--   0        0        0     2955 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/common.py
+-rw-r--r--   0        0        0     4512 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/result.py
+-rw-r--r--   0        0        0     5624 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/server.py
+-rw-r--r--   0        0        0     1878 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1210 2023-07-28 14:24:18.433915 seagoat-0.6.0/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2862 1970-01-01 00:00:00.000000 seagoat-0.6.0/PKG-INFO
```

### Comparing `seagoat-0.5.6/LICENSE` & `seagoat-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/README.md` & `seagoat-0.6.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,68 @@
 <!-- markdownlint-disable MD033 -->
 
 <h1>
   <p align="center">
-    <img src="branding/logo-small.png" alt="Logo" width="200"/>
+    <img src="assets/logo-small.png" alt="Logo" width="200"/>
     <font size="8"><b>SeaGOAT</b></font>
   </p>
 </h1>
 
-A code search engine for the AI age. SeaGOAT leverages vector embeddings to
-enable to search your codebase semantically.
+A code search engine for the AI age. SeaGOAT leverages vector
+embeddings to enable to search your codebase semantically.
+
+## Getting started
+
+### Install SeaGOAT
+
+In order to install SeaGOAT, you need to have the following
+dependencies already installed on your computer:
+
+- Python 3.11 or newer
+- ripgrep
+
+To install SeaGOAT using `pip`, use the following command:
+
+```bash
+pip install seagoat
+```
+
+### Start SeaGOAT server
+
+In order to use SeaGOAT in your project, you have to start the SeaGOAT server
+using the following command:
+
+```bash
+seagoat-server start /path/to/your/repo
+```
+
+### Search your repository
+
+If you have the server running, you can simply use the
+`gt` or `seagoat` command to query your repository. For example:
+
+```bash
+gt "Where are the numbers rounded"
+```
+
+### Stopping the server
+
+You can stop the running server using the following command:
+
+```bash
+seagoat-server stop /path/to/your/repo
+```
 
 ## Development
 
 **Requirements**:
 
-* [Poetry](https://python-poetry.org/)
-* Python 3.11 or newer
-* [ripgrep](https://github.com/BurntSushi/ripgrep)
+- [Poetry](https://python-poetry.org/)
+- Python 3.11 or newer
+- [ripgrep](https://github.com/BurntSushi/ripgrep)
 
 ### Install dependencies
 
 After cloning the repository, install dependencies using the following command:
 
 ```bash
 poetry install
@@ -42,15 +84,16 @@
 
 #### Test all files
 
 ```bash
 poetry run pytest .
 ```
 
-### Manually testing
+### Manual testing
 
-To manually test this app against a code repository,
-you can use the following command:
+You can test any SeaGOAT command manually in your local development
+environment. For example to test the development version of the
+`seagoat-server` command, you can run:
 
 ```bash
-poetry run seagoat ~/path/to/your/repository
+poetry run seagoat-server ~/path/an/example/repository
 ```
```

### Comparing `seagoat-0.5.6/pyproject.toml` & `seagoat-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.5.6"
+version = "0.6.0"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
@@ -47,14 +47,15 @@
 exceptiongroup = "^1.1.2"
 pytest-mock = "^3.11.1"
 pytest-fast-first = "^1.0.5"
 pytest-sugar = "^0.9.7"
 pytest-testmon = "^2.0.12"
 pytest-leaks = "^0.3.1"
 mkdocs-material = "^9.1.19"
+markdown-include = "^0.8.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 venvPath = "."
```

### Comparing `seagoat-0.5.6/seagoat/cache.py` & `seagoat-0.6.0/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/seagoat/cli.py` & `seagoat-0.6.0/seagoat/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import requests
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import get_lexer_for_filename
 from pygments.lexers.javascript import JavascriptLexer
 from pygments.lexers.javascript import TypeScriptLexer
 
+from seagoat import __version__
 from seagoat.server import get_server_info_file
 from seagoat.server import load_server_info
 
 
 def query_server(query, server_address):
     response = requests.get(f"{server_address}/query/{query}")
     try:
@@ -63,14 +64,15 @@
 @click.argument("query")
 @click.argument("repo_path", required=False, default=os.getcwd())
 @click.option(
     "--no-color",
     is_flag=True,
     help="Disable formatting. Automatically enabled when part of a bash pipeline.",
 )
+@click.version_option(version=__version__, prog_name="seagoat")
 def seagoat(query, repo_path, no_color):
     """
     Query your codebase for your QUERY in the Git repository REPO_PATH.
 
     Your query can either be text that you expect to find in a file,
     or a description of what you are looking for.
```

### Comparing `seagoat-0.5.6/seagoat/engine.py` & `seagoat-0.6.0/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/seagoat/file.py` & `seagoat-0.6.0/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/seagoat/repository.py` & `seagoat-0.6.0/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/seagoat/result.py` & `seagoat-0.6.0/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/seagoat/server.py` & `seagoat-0.6.0/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/seagoat/sources/chroma.py` & `seagoat-0.6.0/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.5.6/seagoat/sources/ripgrep.py` & `seagoat-0.6.0/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

