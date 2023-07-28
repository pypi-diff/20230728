# Comparing `tmp/neoteroi_mkdocs-1.0.3.tar.gz` & `tmp/neoteroi_mkdocs-1.0.4.tar.gz`

## Comparing `neoteroi_mkdocs-1.0.3.tar` & `neoteroi_mkdocs-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/py.typed
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/domain.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/py.typed
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/domain.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/git.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/py.typed
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/txt.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/align.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/images.py
--rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/processors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/py.typed
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/files.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/source.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/text.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/web.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/__init__.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/spantable.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/oad/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/oad/py.typed
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/__init__.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/domain.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/py.typed
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/timeutil.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/__init__.py
--rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/html.py
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/spantable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/spantable/py.typed
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/domain.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/py.typed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/LICENSE
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/README.md
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/py.typed
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/cards/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/cards/domain.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/cards/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/cards/py.typed
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/domain.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/git.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/py.typed
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/txt.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/align.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/images.py
+-rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/py.typed
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/files.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/source.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/text.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/web.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/tables/__init__.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/tables/spantable.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/oad/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/oad/py.typed
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/__init__.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/domain.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/py.typed
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/timeutil.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/gantt/__init__.py
+-rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/gantt/html.py
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/spantable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/spantable/py.typed
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/timeline/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/timeline/domain.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/timeline/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/timeline/py.typed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/README.md
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.4/PKG-INFO
```

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/html.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/cards/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/domain.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/domain.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/git.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/git.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/html.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/txt.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/contribs/txt.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/align.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/align.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/images.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/images.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/processors.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/processors.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/utils.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/utils.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/files.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/files.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/text.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/text.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/web.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/data/web.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/spantable.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/markdown/tables/spantable.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/oad/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/oad/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/domain.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/domain.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/timeutil.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/timeutil.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/gantt/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/html.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/projects/gantt/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/spantable/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/spantable/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/__init__.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/timeline/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/html.py` & `neoteroi_mkdocs-1.0.4/neoteroi/mkdocs/timeline/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/LICENSE` & `neoteroi_mkdocs-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/README.md` & `neoteroi_mkdocs-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.3/pyproject.toml` & `neoteroi_mkdocs-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 keywords = ["MkDocs", "OpenAPI", "Swagger", "Markdown", "plugins", "extensions", "documentation"]
 dependencies = [
     "essentials-openapi",
-    "mkdocs~=1.4.0",
-    "httpx<1",
+    "mkdocs",
+    "httpx",
     "click",
     "Jinja2",
     "rich",
 ]
 
 [tool.hatch.version]
 path = "neoteroi/mkdocs/__init__.py"
```

### Comparing `neoteroi_mkdocs-1.0.3/PKG-INFO` & `neoteroi_mkdocs-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoteroi-mkdocs
-Version: 1.0.3
+Version: 1.0.4
 Summary: Plugins for MkDocs and Python Markdown
 Project-URL: Homepage, https://github.com/Neoteroi/mkdocs-plugins
 Project-URL: Bug Tracker, https://github.com/Neoteroi/mkdocs-plugins/issues
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 License-File: LICENSE
 Keywords: Markdown,MkDocs,OpenAPI,Swagger,documentation,extensions,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: click
 Requires-Dist: essentials-openapi
-Requires-Dist: httpx<1
+Requires-Dist: httpx
 Requires-Dist: jinja2
-Requires-Dist: mkdocs~=1.4.0
+Requires-Dist: mkdocs
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 ![Build](https://github.com/Neoteroi/mkdocs-plugins/workflows/Build/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/neoteroi-mkdocs.svg)](https://pypi.python.org/pypi/neoteroi-mkdocs)
 [![versions](https://img.shields.io/pypi/pyversions/neoteroi-mkdocs.svg)](https://github.com/neoteroi/mkdocs-plugins)
 [![license](https://img.shields.io/github/license/neoteroi/mkdocs-plugins.svg)](https://github.com/neoteroi/mkdocs-plugins/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: neoteroi-mkdocs Version: 1.0.3 Summary: Plugins for
+Metadata-Version: 2.1 Name: neoteroi-mkdocs Version: 1.0.4 Summary: Plugins for
 MkDocs and Python Markdown Project-URL: Homepage, https://github.com/Neoteroi/
 mkdocs-plugins Project-URL: Bug Tracker, https://github.com/Neoteroi/mkdocs-
 plugins/issues Author-email: Roberto Prevato
 prevato@gmail.com> License-File: LICENSE Keywords:
 Markdown,MkDocs,OpenAPI,Swagger,documentation,extensions,plugins Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: >=3.7 Requires-Dist: click Requires-Dist: essentials-openapi Requires-
-Dist: httpx<1 Requires-Dist: jinja2 Requires-Dist: mkdocs~=1.4.0 Requires-Dist:
-rich Description-Content-Type: text/markdown ![Build](https://github.com/
-Neoteroi/mkdocs-plugins/workflows/Build/badge.svg) [![pypi](https://
-img.shields.io/pypi/v/neoteroi-mkdocs.svg)](https://pypi.python.org/pypi/
-neoteroi-mkdocs) [![versions](https://img.shields.io/pypi/pyversions/neoteroi-
-mkdocs.svg)](https://github.com/neoteroi/mkdocs-plugins) [![license](https://
-img.shields.io/github/license/neoteroi/mkdocs-plugins.svg)](https://github.com/
-neoteroi/mkdocs-plugins/blob/main/LICENSE) [![codecov](https://codecov.io/gh/
-Neoteroi/mkdocs-plugins/branch/main/graph/badge.svg)](https://codecov.io/gh/
-Neoteroi/mkdocs-plugins) [![documentation](https://img.shields.io/badge/ð-
-docs-purple)](https://www.neoteroi.dev/mkdocs-plugins/) # Plugins for MkDocs
-and Python Markdown ```bash pip install neoteroi-mkdocs ``` This package
-includes the following plugins and extensions: | Name | Description | | :------
----------------------------------------------------------- | :-----------------
-------------------------------------------------------- | | [`mkdocsoad`]
-(https://www.neoteroi.dev/mkdocs-plugins/web/oad/) | Generates documentation
-from OpenAPI specification files. | | [`cards`](https://www.neoteroi.dev/
-mkdocs-plugins/cards/) | Component to display cards. | | [`timeline`](https://
+Dist: httpx Requires-Dist: jinja2 Requires-Dist: mkdocs Requires-Dist: rich
+Description-Content-Type: text/markdown ![Build](https://github.com/Neoteroi/
+mkdocs-plugins/workflows/Build/badge.svg) [![pypi](https://img.shields.io/pypi/
+v/neoteroi-mkdocs.svg)](https://pypi.python.org/pypi/neoteroi-mkdocs) [!
+[versions](https://img.shields.io/pypi/pyversions/neoteroi-mkdocs.svg)](https:/
+/github.com/neoteroi/mkdocs-plugins) [![license](https://img.shields.io/github/
+license/neoteroi/mkdocs-plugins.svg)](https://github.com/neoteroi/mkdocs-
+plugins/blob/main/LICENSE) [![codecov](https://codecov.io/gh/Neoteroi/mkdocs-
+plugins/branch/main/graph/badge.svg)](https://codecov.io/gh/Neoteroi/mkdocs-
+plugins) [![documentation](https://img.shields.io/badge/ð-docs-purple)]
+(https://www.neoteroi.dev/mkdocs-plugins/) # Plugins for MkDocs and Python
+Markdown ```bash pip install neoteroi-mkdocs ``` This package includes the
+following plugins and extensions: | Name | Description | | :-------------------
+--------------------------------------------- | :------------------------------
+------------------------------------------ | | [`mkdocsoad`](https://
+www.neoteroi.dev/mkdocs-plugins/web/oad/) | Generates documentation from
+OpenAPI specification files. | | [`cards`](https://www.neoteroi.dev/mkdocs-
+plugins/cards/) | Component to display cards. | | [`timeline`](https://
 www.neoteroi.dev/mkdocs-plugins/timeline/) | Component to display chronological
 information with style. | | [`gantt`](https://www.neoteroi.dev/mkdocs-plugins/
 gantt/) | Component to display Gantt diagrams. | | [`spantable`](https://
 www.neoteroi.dev/mkdocs-plugins/spantable/) | Tables supporting colspan and
 rowspan. | | [`contribs`](https://www.neoteroi.dev/mkdocs-plugins/contribs/) |
 MkDocs plugin to display last commit time and contributors for each file. | ##
 Documentation Refer to the [documentation site](https://www.neoteroi.dev/
```

