# Comparing `tmp/iscwatch-0.3.0.tar.gz` & `tmp/iscwatch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iscwatch-0.3.0.tar", max compression
+gzip compressed data, was "iscwatch-0.3.2.tar", max compression
```

## Comparing `iscwatch-0.3.0.tar` & `iscwatch-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     2571 2023-07-25 19:10:32.240679 iscwatch-0.3.0/README.md
--rwxr-xr-x   0        0        0      573 2023-07-25 19:10:32.241345 iscwatch-0.3.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-15 22:53:30.000000 iscwatch-0.3.0/src/iscwatch/__init__.py
--rw-r--r--   0        0        0      265 2023-07-25 18:36:36.175858 iscwatch-0.3.0/src/iscwatch/advisory.py
--rw-r--r--   0        0        0      519 2023-07-25 19:10:32.241567 iscwatch-0.3.0/src/iscwatch/logconfig.py
--rwxr-xr-x   0        0        0     2074 2023-07-25 19:10:32.241861 iscwatch-0.3.0/src/iscwatch/main.py
--rw-r--r--   0        0        0     3590 2023-07-25 19:10:32.242036 iscwatch-0.3.0/src/iscwatch/scrape.py
--rw-r--r--   0        0        0     3038 1970-01-01 00:00:00.000000 iscwatch-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2590 2023-07-28 19:36:55.065038 iscwatch-0.3.2/README.md
+-rwxr-xr-x   0        0        0      573 2023-07-28 19:36:55.065407 iscwatch-0.3.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-15 22:53:30.000000 iscwatch-0.3.2/src/iscwatch/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-25 18:36:36.175858 iscwatch-0.3.2/src/iscwatch/advisory.py
+-rw-r--r--   0        0        0      519 2023-07-25 19:10:32.241567 iscwatch-0.3.2/src/iscwatch/logconfig.py
+-rwxr-xr-x   0        0        0     2427 2023-07-28 19:36:55.065724 iscwatch-0.3.2/src/iscwatch/main.py
+-rw-r--r--   0        0        0     3590 2023-07-25 19:10:32.242036 iscwatch-0.3.2/src/iscwatch/scrape.py
+-rw-r--r--   0        0        0     3057 1970-01-01 00:00:00.000000 iscwatch-0.3.2/PKG-INFO
```

### Comparing `iscwatch-0.3.0/README.md` & `iscwatch-0.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # iscwatch - A Command Line Application For Monitoring Intel Security Center Product Advisories
 
-![Version](https://img.shields.io/badge/version-0.3.0-blue.svg)
+![Version](https://img.shields.io/badge/version-0.3.1-blue.svg)
 ![License](https://img.shields.io/badge/license-MIT-green.svg)
 
 ## Description
 
 `iscwatch` is a command line application that searches for summaries of [Intel's Security Center Product Advisories](https://www.intel.com/content/www/us/en/security-center/default.html) and outputs those summaries in CSV format. Included in the output per advisory is its title, full text url, advisory ID, updated date, and released date.
 
 ## Features
 
-- Fetches summaries of Intel's Security Center Product Advisories.
-- Outputs advisory data in CSV format to stdout.
-- Optionally filters advisories based on date using the --since option.
-- Enables or disables CSV column headers with --headers and --no-headers options, respectively.
+- Fetches some or all summaries of Intel's Security Center Product advisories.
+- Outputs advisory summary data in CSV format with our without headers.
+- Date filtering enables iscwatch to be used to only show latest changes.
 
 ## Installation
 
 You can install `iscwatch` using pip:
 
 ```
 pip install iscwatch
@@ -26,18 +25,20 @@
 
 ```
 Usage: iscwatch [OPTIONS]
 
 Retrieve Security Advisory summaries from Intel website and output as CSV.
 
 Options
---since                     Output only those summaries released or updated since specified date. [default: None]
---version    --no-version   Output product version and exit. [default: no-version]
---headers    --no-headers   Include column headers in CSV output. [default: headers]
---help                      Show this message and exit.
+--since         -s      [%Y-%m-%d]  Exclude summaries before date.
+                                    [default: 0001-01-01 00:00:00]
+--version       -v                  Output product version and exit.
+--no-headers    -n                  Omit column headers from CSV output.
+--last-updated  -l                  Output date when last updated and exit.
+--help                              Show this message and exit.
 ```
 
 The application will fetch the latest advisories from Intel's Security Center and display the summaries in CSV format to the standard output (stdout). You can redirect the output to a file if needed:
 
 ```bash
 iscwatch > advisories.csv
 ```
```

### Comparing `iscwatch-0.3.0/pyproject.toml` & `iscwatch-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iscwatch"
-version = "0.3.0"
+version = "0.3.2"
 description = ""
 authors = ["Roger Hurwitz <rogerhurwitz@inspirsmith.com>"]
 readme = "README.md"
 packages = [{include = "iscwatch", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `iscwatch-0.3.0/src/iscwatch/logconfig.py` & `iscwatch-0.3.2/src/iscwatch/logconfig.py`

 * *Files identical despite different names*

### Comparing `iscwatch-0.3.0/src/iscwatch/main.py` & `iscwatch-0.3.2/src/iscwatch/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,38 +23,48 @@
     typer.run(main)
 
 
 def main(
     since: Annotated[
         datetime.datetime,
         typer.Option(
-            help="Output only those summaries released or updated since specified date."
+            "--since", "-s", help="Exclude summaries before date.", formats=["%Y-%m-%d"]
         ),
     ] = datetime.datetime.min,
-    version: Annotated[bool, typer.Option(help="Output product version and exit.")] = False,
-    headers: Annotated[
-        bool, typer.Option(help="Include column headers in CSV output.")
-    ] = True,
+    version: Annotated[
+        bool,
+        typer.Option("--version", "-v", help="Output product version and exit."),
+    ] = False,
+    no_headers: Annotated[
+        bool,
+        typer.Option("--no-headers", "-n", help="Omit column headers from CSV output."),
+    ] = False,
+    last_updated: Annotated[
+        bool,
+        typer.Option("--last-updated", "-l", help="Output date when last updated and exit."),
+    ] = False,
 ):
     """Disposition command line and vector work to appropriate sub-function."""
     if version:
         print_version()
-    else:
-        if since:
-            selected_advisories = [a for a in iter_advisories() if a.updated >= since.date()]
-        else:
-            selected_advisories = list(iter_advisories())
-        print_csv_advisories(selected_advisories, headers)
+    elif last_updated:
+        last_updated_advisory = max(iter_advisories(), key=lambda a: a.updated)
+        print(last_updated_advisory.updated)
+    else:  # output advisories
+        selected_advisories = [
+            a for a in iter_advisories() if not since or a.updated >= since.date()
+        ]
+        print_csv_advisories(selected_advisories, no_headers)
 
 
-def print_csv_advisories(advisories: list[Advisory], use_headers: bool):
+def print_csv_advisories(advisories: list[Advisory], no_headers: bool):
     """Convert advisories into dictionaries and output in CSV format."""
     fieldnames = [field.name for field in fields(Advisory)]
     writer = csv.DictWriter(sys.stdout, fieldnames=fieldnames)
-    if use_headers:
+    if not no_headers:
         writer.writeheader()
     writer.writerows(asdict(advisory) for advisory in advisories)
 
 
 def print_version():
     """Output current version of the application."""
     try:
```

### Comparing `iscwatch-0.3.0/src/iscwatch/scrape.py` & `iscwatch-0.3.2/src/iscwatch/scrape.py`

 * *Files identical despite different names*

### Comparing `iscwatch-0.3.0/PKG-INFO` & `iscwatch-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: iscwatch
-Version: 0.3.0
+Version: 0.3.2
 Summary: 
 Author: Roger Hurwitz
 Author-email: rogerhurwitz@inspirsmith.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # iscwatch - A Command Line Application For Monitoring Intel Security Center Product Advisories
 
-![Version](https://img.shields.io/badge/version-0.3.0-blue.svg)
+![Version](https://img.shields.io/badge/version-0.3.1-blue.svg)
 ![License](https://img.shields.io/badge/license-MIT-green.svg)
 
 ## Description
 
 `iscwatch` is a command line application that searches for summaries of [Intel's Security Center Product Advisories](https://www.intel.com/content/www/us/en/security-center/default.html) and outputs those summaries in CSV format. Included in the output per advisory is its title, full text url, advisory ID, updated date, and released date.
 
 ## Features
 
-- Fetches summaries of Intel's Security Center Product Advisories.
-- Outputs advisory data in CSV format to stdout.
-- Optionally filters advisories based on date using the --since option.
-- Enables or disables CSV column headers with --headers and --no-headers options, respectively.
+- Fetches some or all summaries of Intel's Security Center Product advisories.
+- Outputs advisory summary data in CSV format with our without headers.
+- Date filtering enables iscwatch to be used to only show latest changes.
 
 ## Installation
 
 You can install `iscwatch` using pip:
 
 ```
 pip install iscwatch
@@ -41,18 +40,20 @@
 
 ```
 Usage: iscwatch [OPTIONS]
 
 Retrieve Security Advisory summaries from Intel website and output as CSV.
 
 Options
---since                     Output only those summaries released or updated since specified date. [default: None]
---version    --no-version   Output product version and exit. [default: no-version]
---headers    --no-headers   Include column headers in CSV output. [default: headers]
---help                      Show this message and exit.
+--since         -s      [%Y-%m-%d]  Exclude summaries before date.
+                                    [default: 0001-01-01 00:00:00]
+--version       -v                  Output product version and exit.
+--no-headers    -n                  Omit column headers from CSV output.
+--last-updated  -l                  Output date when last updated and exit.
+--help                              Show this message and exit.
 ```
 
 The application will fetch the latest advisories from Intel's Security Center and display the summaries in CSV format to the standard output (stdout). You can redirect the output to a file if needed:
 
 ```bash
 iscwatch > advisories.csv
 ```
```

