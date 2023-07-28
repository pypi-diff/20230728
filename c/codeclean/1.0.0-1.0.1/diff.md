# Comparing `tmp/codeclean-1.0.0.tar.gz` & `tmp/codeclean-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeclean-1.0.0.tar", last modified: Sun Jul 16 10:46:01 2023, max compression
+gzip compressed data, was "codeclean-1.0.1.tar", last modified: Fri Jul 28 08:57:11 2023, max compression
```

## Comparing `codeclean-1.0.0.tar` & `codeclean-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:46:01.730756 codeclean-1.0.0/
--rw-rw-rw-   0        0        0    18429 2023-07-16 10:34:54.000000 codeclean-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1745 2023-07-16 10:46:01.728761 codeclean-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-07-16 10:32:45.000000 codeclean-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 10:46:01.715805 codeclean-1.0.0/codeclean/
--rw-rw-rw-   0        0        0       45 2023-07-16 10:39:37.000000 codeclean-1.0.0/codeclean/__init__.py
--rw-rw-rw-   0        0        0     1971 2023-07-16 10:45:20.000000 codeclean-1.0.0/codeclean/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:46:01.722786 codeclean-1.0.0/codeclean.egg-info/
--rw-rw-rw-   0        0        0     1745 2023-07-16 10:46:01.000000 codeclean-1.0.0/codeclean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-16 10:46:01.000000 codeclean-1.0.0/codeclean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:46:01.000000 codeclean-1.0.0/codeclean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-16 10:46:01.000000 codeclean-1.0.0/codeclean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:46:01.730756 codeclean-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1215 2023-07-16 10:45:43.000000 codeclean-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:57:11.155095 codeclean-1.0.1/
+-rw-rw-rw-   0        0        0    18429 2023-07-28 08:56:22.000000 codeclean-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1730 2023-07-28 08:57:11.154099 codeclean-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2023-07-28 08:56:22.000000 codeclean-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 08:57:11.142096 codeclean-1.0.1/codeclean/
+-rw-rw-rw-   0        0        0       45 2023-07-28 08:56:22.000000 codeclean-1.0.1/codeclean/__init__.py
+-rw-rw-rw-   0        0        0     2227 2023-07-28 08:56:22.000000 codeclean-1.0.1/codeclean/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:57:11.153095 codeclean-1.0.1/codeclean.egg-info/
+-rw-rw-rw-   0        0        0     1730 2023-07-28 08:57:11.000000 codeclean-1.0.1/codeclean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-28 08:57:11.000000 codeclean-1.0.1/codeclean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 08:57:11.000000 codeclean-1.0.1/codeclean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 08:57:11.000000 codeclean-1.0.1/codeclean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 08:57:11.155095 codeclean-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1215 2023-07-28 08:56:22.000000 codeclean-1.0.1/setup.py
```

### Comparing `codeclean-1.0.0/LICENSE` & `codeclean-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codeclean-1.0.0/PKG-INFO` & `codeclean-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeclean
-Version: 1.0.0
+Version: 1.0.1
 Summary: Remove comments and docstrings from Python code.
 Home-page: https://github.com/Ruu3f/cleancode
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/cleancode
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: clean,code,cleaner,comments,docstrings
@@ -15,35 +15,35 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI](https://img.shields.io/pypi/v/codecleaner)](https://pypi.org/project/codecleaner)
-[![Downloads](https://static.pepy.tech/badge/codecleaner)](https://pypi.org/project/codecleaner)
-[![Status](https://img.shields.io/pypi/status/codecleaner)](https://pypi.org/project/codecleaner)
+[![PyPI](https://img.shields.io/pypi/v/codeclean)](https://pypi.org/project/codeclean)
+[![Downloads](https://static.pepy.tech/badge/codeclean)](https://pypi.org/project/codeclean)
+[![Status](https://img.shields.io/pypi/status/codeclean)](https://pypi.org/project/codeclean)
 
-# codecleaner
+# cleancode
 
 Remove comments and docstrings from Python code.
 
 ## Get started:
 
 ```
-python -m pip install --upgrade codecleaner
+python -m pip install -U cleancode
 ```
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Support this repository:
 
 - Star this repository :D
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## Example:
 
 ```
-codecleaner filename.py --comments --docstrings
+python -m cleancode filename.py --comments --docstrings
 ```
```

### Comparing `codeclean-1.0.0/README.md` & `codeclean-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[![PyPI](https://img.shields.io/pypi/v/codecleaner)](https://pypi.org/project/codecleaner)
-[![Downloads](https://static.pepy.tech/badge/codecleaner)](https://pypi.org/project/codecleaner)
-[![Status](https://img.shields.io/pypi/status/codecleaner)](https://pypi.org/project/codecleaner)
+[![PyPI](https://img.shields.io/pypi/v/codeclean)](https://pypi.org/project/codeclean)
+[![Downloads](https://static.pepy.tech/badge/codeclean)](https://pypi.org/project/codeclean)
+[![Status](https://img.shields.io/pypi/status/codeclean)](https://pypi.org/project/codeclean)
 
-# codecleaner
+# cleancode
 
 Remove comments and docstrings from Python code.
 
 ## Get started:
 
 ```
-python -m pip install --upgrade codecleaner
+python -m pip install -U cleancode
 ```
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Support this repository:
 
 - Star this repository :D
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## Example:
 
 ```
-codecleaner filename.py --comments --docstrings
-```
+python -m cleancode filename.py --comments --docstrings
+```
```

### Comparing `codeclean-1.0.0/codeclean/__main__.py` & `codeclean-1.0.1/codeclean/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,80 @@
 """
 codeclean
 
 Remove comments and docstrings from Python code.
 """
-
-import os
-import re
-import argparse
+from re import sub, DOTALL
+from os.path import isfile
+from argparse import ArgumentParser
 
 
 def remove_comments(code):
     """
     Removes comments from the code.
     """
     lines_list = []
     lines = code.split("\n")
     for line in lines:
-        line = re.sub(r"\s*#.*$", "", line)
+        line = sub(r"\s*#.*$", "", line)
         lines_list.append(line)
     return "\n".join(lines_list)
 
 
 def remove_docstrings(code):
     """
     Removes docstrings from the code.
     """
-    code = re.sub(r'(?<!\\)"""[^"]*"""', "", code, flags=re.DOTALL)
-    code = re.sub(r"(?<!\\)'''[^']*'''", "", code, flags=re.DOTALL)
+    code = sub(r'(?<!\\)"""[^"]*"""', "", code, flags=DOTALL)
+    code = sub(r"(?<!\\)'''[^']*'''", "", code, flags=DOTALL)
     return code
 
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(
+def main():
+    parser = ArgumentParser(
         description="Remove comments and docstrings from Python files."
     )
     parser.add_argument(
-        "files", metavar="file", type=str, nargs="+", help="File(s) to process"
+        "files", metavar="file", type=str, nargs="+", help="File(s) to process."
     )
-    parser.add_argument("--comments", action="store_true", help="Remove comments")
-    parser.add_argument("--docstrings", action="store_true", help="Remove docstrings")
+    parser.add_argument("--comments", action="store_true", help="Remove comments.")
+    parser.add_argument("--docstrings", action="store_true", help="Remove docstrings.")
 
     args = parser.parse_args()
 
+    if not args.comments and not args.docstrings:
+        print("Error: You must provide either the --comments or --docstrings flag.")
+        return
+
     modified_code = {}
 
     for file in args.files:
-        if os.path.isfile(file):
-            try:
-                with open(file, "r", encoding="utf-8") as f:
-                    code = f.read()
-            except IOError as e:
-                print(f"Error while processing file {file}: {str(e)}")
-                continue
-
-            if args.comments:
-                code = remove_comments(code)
-
-            if args.docstrings:
-                code = remove_docstrings(code)
-
-            modified_code[file] = code
-        else:
-            print(f"Error: {file} is not a valid file.")
+        if not isfile(file):
+            print(f"Error: '{file}' is not a valid file.")
+            continue
+
+        try:
+            with open(file, "r", encoding="utf-8") as f:
+                code = f.read()
+        except IOError as e:
+            print(f"Error while processing file '{file}': {str(e)}")
+            continue
+
+        if args.comments:
+            code = remove_comments(code)
+
+        if args.docstrings:
+            code = remove_docstrings(code)
+
+        modified_code[file] = code
 
     for file, code in modified_code.items():
         try:
             with open(file, "w", encoding="utf-8") as f:
                 f.write(code)
+                print(f"File '{file}' has been processed and modified.")
         except IOError as e:
-            print(f"Error while writing to file {file}: {str(e)}")
+            print(f"Error while writing to file '{file}': {str(e)}")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `codeclean-1.0.0/codeclean.egg-info/PKG-INFO` & `codeclean-1.0.1/codeclean.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeclean
-Version: 1.0.0
+Version: 1.0.1
 Summary: Remove comments and docstrings from Python code.
 Home-page: https://github.com/Ruu3f/cleancode
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/cleancode
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: clean,code,cleaner,comments,docstrings
@@ -15,35 +15,35 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI](https://img.shields.io/pypi/v/codecleaner)](https://pypi.org/project/codecleaner)
-[![Downloads](https://static.pepy.tech/badge/codecleaner)](https://pypi.org/project/codecleaner)
-[![Status](https://img.shields.io/pypi/status/codecleaner)](https://pypi.org/project/codecleaner)
+[![PyPI](https://img.shields.io/pypi/v/codeclean)](https://pypi.org/project/codeclean)
+[![Downloads](https://static.pepy.tech/badge/codeclean)](https://pypi.org/project/codeclean)
+[![Status](https://img.shields.io/pypi/status/codeclean)](https://pypi.org/project/codeclean)
 
-# codecleaner
+# cleancode
 
 Remove comments and docstrings from Python code.
 
 ## Get started:
 
 ```
-python -m pip install --upgrade codecleaner
+python -m pip install -U cleancode
 ```
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Support this repository:
 
 - Star this repository :D
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
 [![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## Example:
 
 ```
-codecleaner filename.py --comments --docstrings
+python -m cleancode filename.py --comments --docstrings
 ```
```

### Comparing `codeclean-1.0.0/setup.py` & `codeclean-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="codeclean",
-    version="1.0.0",
+    version="1.0.1",
     description="Remove comments and docstrings from Python code.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/cleancode",
     author="Ruu3f",
     license="GPLv2",
     keywords=[
```

