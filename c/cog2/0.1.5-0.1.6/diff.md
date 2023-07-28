# Comparing `tmp/cog2-0.1.5.tar.gz` & `tmp/cog2-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog2-0.1.5.tar", max compression
+gzip compressed data, was "cog2-0.1.6.tar", max compression
```

## Comparing `cog2-0.1.5.tar` & `cog2-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.5/cog2/__init__.py
--rw-r--r--   0        0        0     3642 2023-07-27 09:14:01.846636 cog2-0.1.5/cog2/main.py
--rw-r--r--   0        0        0      427 2023-07-27 09:13:08.546621 cog2-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 cog2-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.6/cog2/__init__.py
+-rw-r--r--   0        0        0     3699 2023-07-28 06:30:37.059296 cog2-0.1.6/cog2/main.py
+-rw-r--r--   0        0        0      427 2023-07-28 06:30:37.066072 cog2-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 cog2-0.1.6/PKG-INFO
```

### Comparing `cog2-0.1.5/cog2/main.py` & `cog2-0.1.6/cog2/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,8 +103,13 @@
         prefix_cmd = prefix_cmd + " -p {}".format(publish)
     os.system(prefix_cmd)
     typer.echo("Run cmd finished: " + prefix_cmd)
 
 
 @app.command()
 def version():
-    typer.echo('0.1.5')
+    typer.echo('0.1.6')
+
+
+@app.command()
+def debug():
+    os.system("cog debug")
```

### Comparing `cog2-0.1.5/PKG-INFO` & `cog2-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog2
-Version: 0.1.5
+Version: 0.1.6
 Summary: wizmodel.com cog2 sdk
 Author: incoming
 Author-email: 18320122+incomingflyingbrick@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

