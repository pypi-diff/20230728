# Comparing `tmp/cog2-0.1.6.tar.gz` & `tmp/cog2-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog2-0.1.6.tar", max compression
+gzip compressed data, was "cog2-0.1.7.tar", max compression
```

## Comparing `cog2-0.1.6.tar` & `cog2-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.6/cog2/__init__.py
--rw-r--r--   0        0        0     3699 2023-07-28 06:30:37.059296 cog2-0.1.6/cog2/main.py
--rw-r--r--   0        0        0      427 2023-07-28 06:30:37.066072 cog2-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 cog2-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.7/cog2/__init__.py
+-rw-r--r--   0        0        0     3699 2023-07-28 15:27:27.329031 cog2-0.1.7/cog2/main.py
+-rw-r--r--   0        0        0      426 2023-07-28 15:26:16.468015 cog2-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 cog2-0.1.7/PKG-INFO
```

### Comparing `cog2-0.1.6/cog2/main.py` & `cog2-0.1.7/cog2/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,13 +103,13 @@
         prefix_cmd = prefix_cmd + " -p {}".format(publish)
     os.system(prefix_cmd)
     typer.echo("Run cmd finished: " + prefix_cmd)
 
 
 @app.command()
 def version():
-    typer.echo('0.1.6')
+    typer.echo('0.1.7')
 
 
 @app.command()
 def debug():
     os.system("cog debug")
```

### Comparing `cog2-0.1.6/PKG-INFO` & `cog2-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cog2
-Version: 0.1.6
-Summary: wizmodel.com cog2 sdk
+Version: 0.1.7
+Summary: wizmodel.com wiz sdk
 Author: incoming
 Author-email: 18320122+incomingflyingbrick@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

