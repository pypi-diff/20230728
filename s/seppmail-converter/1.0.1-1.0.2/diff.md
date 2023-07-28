# Comparing `tmp/seppmail_converter-1.0.1.tar.gz` & `tmp/seppmail_converter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail_converter-1.0.1.tar", max compression
+gzip compressed data, was "seppmail_converter-1.0.2.tar", max compression
```

## Comparing `seppmail_converter-1.0.1.tar` & `seppmail_converter-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1061 2023-07-27 12:44:20.677395 seppmail_converter-1.0.1/README.md
--rw-r--r--   0        0        0      839 2023-07-27 12:44:51.317212 seppmail_converter-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-27 12:44:51.393212 seppmail_converter-1.0.1/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      133 2023-07-27 12:44:20.677395 seppmail_converter-1.0.1/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     5336 2023-07-27 12:44:20.677395 seppmail_converter-1.0.1/seppmail_converter/main.py
--rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 seppmail_converter-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-28 11:22:56.105512 seppmail_converter-1.0.2/README.md
+-rw-r--r--   0        0        0      839 2023-07-28 11:23:27.177927 seppmail_converter-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-28 11:23:27.261928 seppmail_converter-1.0.2/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-28 11:22:56.105512 seppmail_converter-1.0.2/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     5394 2023-07-28 11:22:56.105512 seppmail_converter-1.0.2/seppmail_converter/main.py
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 seppmail_converter-1.0.2/PKG-INFO
```

### Comparing `seppmail_converter-1.0.1/README.md` & `seppmail_converter-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `seppmail_converter-1.0.1/pyproject.toml` & `seppmail_converter-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seppmail-converter"
-version = "1.0.1"
+version = "1.0.2"
 description = "Decode SEPPMail emails into EML files"
 license = "MIT"
 authors = ["Daniel Malik <daniel.malik@mhsp.solutions>"]
 readme = "README.md"
 classifiers = ["Environment :: Console"]
 
 [tool.poetry.dependencies]
```

### Comparing `seppmail_converter-1.0.1/seppmail_converter/main.py` & `seppmail_converter-1.0.2/seppmail_converter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,15 @@
                 )
             )
         )
         if output.exists() and overwrite:
             output.unlink()
 
     output.write_bytes(req.content)
+    output.touch()
 
     if delete:
         input_file.unlink()
     if quiet:
         click.echo(output.absolute())
     else:
         click.echo(
@@ -180,14 +181,16 @@
                 continue
             if not attachment_filename:
                 continue
             attachment_output = pathlib.Path(
                 pathlib.Path.joinpath(output.parent, attachment_filename)
             )
             attachment_output.write_bytes(attachment.get_payload(decode=True))
+            attachment_output.touch()
+
             if not quiet:
                 click.echo(
                     f"Extracted {click.format_filename(attachment_output.absolute())}"
                 )
 
 
 def entry():
```

### Comparing `seppmail_converter-1.0.1/PKG-INFO` & `seppmail_converter-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Decode SEPPMail emails into EML files
 License: MIT
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

