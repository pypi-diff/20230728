# Comparing `tmp/fourdigits-cli-1.5.0.tar.gz` & `tmp/fourdigits-cli-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fourdigits-cli-1.5.0.tar", last modified: Thu Jul 27 07:37:28 2023, max compression
+gzip compressed data, was "fourdigits-cli-1.6.0.tar", last modified: Fri Jul 28 11:38:42 2023, max compression
```

## Comparing `fourdigits-cli-1.5.0.tar` & `fourdigits-cli-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:37:28.231394 fourdigits-cli-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-27 07:37:28.231394 fourdigits-cli-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:37:28.228394 fourdigits-cli-1.5.0/fourdigits_cli/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:37:28.230394 fourdigits-cli-1.5.0/fourdigits_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5604 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/commands/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/commands/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:37:28.230394 fourdigits-cli-1.5.0/fourdigits_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3459 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/utils/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/fourdigits_cli/utils/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:37:28.229394 fourdigits-cli-1.5.0/fourdigits_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-27 07:37:28.000000 fourdigits-cli-1.5.0/fourdigits_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      625 2023-07-27 07:37:28.000000 fourdigits-cli-1.5.0/fourdigits_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 07:37:28.000000 fourdigits-cli-1.5.0/fourdigits_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-27 07:37:28.000000 fourdigits-cli-1.5.0/fourdigits_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-27 07:37:28.000000 fourdigits-cli-1.5.0/fourdigits_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 07:37:28.000000 fourdigits-cli-1.5.0/fourdigits_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-27 07:37:28.231394 fourdigits-cli-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 07:37:28.231394 fourdigits-cli-1.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-27 07:36:27.000000 fourdigits-cli-1.5.0/tests/test_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 11:38:42.803023 fourdigits-cli-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-28 11:38:42.803023 fourdigits-cli-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 11:38:42.799023 fourdigits-cli-1.6.0/fourdigits_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-28 11:36:17.000000 fourdigits-cli-1.6.0/fourdigits_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/fourdigits_cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/fourdigits_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 11:38:42.803023 fourdigits-cli-1.6.0/fourdigits_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 11:37:45.000000 fourdigits-cli-1.6.0/fourdigits_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5610 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/fourdigits_cli/commands/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/fourdigits_cli/commands/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/fourdigits_cli/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 11:38:42.803023 fourdigits-cli-1.6.0/fourdigits_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 11:37:45.000000 fourdigits-cli-1.6.0/fourdigits_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3483 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/fourdigits_cli/utils/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/fourdigits_cli/utils/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 11:38:42.803023 fourdigits-cli-1.6.0/fourdigits_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-28 11:38:42.000000 fourdigits-cli-1.6.0/fourdigits_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-28 11:38:42.000000 fourdigits-cli-1.6.0/fourdigits_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 11:38:42.000000 fourdigits-cli-1.6.0/fourdigits_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-28 11:38:42.000000 fourdigits-cli-1.6.0/fourdigits_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-28 11:38:42.000000 fourdigits-cli-1.6.0/fourdigits_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-28 11:38:42.000000 fourdigits-cli-1.6.0/fourdigits_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-28 11:38:42.807023 fourdigits-cli-1.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 11:38:42.803023 fourdigits-cli-1.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-28 08:36:00.000000 fourdigits-cli-1.6.0/tests/test_settings.py
```

### Comparing `fourdigits-cli-1.5.0/PKG-INFO` & `fourdigits-cli-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.5.0
+Version: 1.6.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
```

### Comparing `fourdigits-cli-1.5.0/README.md` & `fourdigits-cli-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli/cli.py` & `fourdigits-cli-1.6.0/fourdigits_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli/commands/docker.py` & `fourdigits-cli-1.6.0/fourdigits_cli/commands/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     build_image_name = uuid4().hex
     try:
         docker.build(
             build_image_name,
             file=options.get("file"),
             context=options.get("context"),
             target=options.get("target"),
-            build_tag=str(version),
+            release_version=str(version),
             cache_from=latest_image,
             build_args=options.get("build_arg"),
         )
         for tag in [environment, str(version)]:
             docker.image_tag(
                 build_image_name,
                 docker.get_image_name(
```

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli/commands/gitlab.py` & `fourdigits-cli-1.6.0/fourdigits_cli/commands/gitlab.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli/settings.py` & `fourdigits-cli-1.6.0/fourdigits_cli/settings.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli/utils/docker.py` & `fourdigits-cli-1.6.0/fourdigits_cli/utils/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     def build(
         self,
         tag,
         file="Dockerfile",
         context=".",
         target=None,
-        build_tag="",
+        release_version="",
         cache_from=None,
         build_args=None,
     ):
         logger.info(f"Docker build image {tag}")
         logger.info(f" - file={file}")
         logger.info(f" - context={context}")
         logger.info(f" - target={target}")
@@ -88,15 +88,15 @@
                     [
                         "build",
                         "--pull",
                         f"--target={target}" if target else None,
                         f"--tag={tag}",
                         f"--file={file}",
                         f"--cache-from={cache_from}" if cache_from else None,
-                        f"--build-arg=TAG={build_tag}",
+                        f"--build-arg=RELEASE_VERSION={release_version}",
                         "--secret=id=pip_extra_index_url,env=PIP_EXTRA_INDEX_URL"
                         if "PIP_EXTRA_INDEX_URL" in os.environ
                         else None,
                         *[f"--build-arg={arg}" for arg in build_args or []],
                         context,
                     ],
                 )
```

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli/utils/git.py` & `fourdigits-cli-1.6.0/fourdigits_cli/utils/git.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli.egg-info/PKG-INFO` & `fourdigits-cli-1.6.0/fourdigits_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.5.0
+Version: 1.6.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
```

### Comparing `fourdigits-cli-1.5.0/fourdigits_cli.egg-info/SOURCES.txt` & `fourdigits-cli-1.6.0/fourdigits_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.5.0/setup.py` & `fourdigits-cli-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.5.0/tests/test_settings.py` & `fourdigits-cli-1.6.0/tests/test_settings.py`

 * *Files identical despite different names*

