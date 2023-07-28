# Comparing `tmp/screener-0.4.1.tar.gz` & `tmp/screener-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screener-0.4.1.tar", max compression
+gzip compressed data, was "screener-0.5.0.tar", max compression
```

## Comparing `screener-0.4.1.tar` & `screener-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1808 2023-06-09 12:49:06.826100 screener-0.4.1/README.md
--rw-r--r--   0        0        0     2549 2023-06-11 13:17:10.597748 screener-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.4.1/screener/__init__.py
--rw-r--r--   0        0        0     2022 2023-06-11 13:17:10.597748 screener-0.4.1/screener/__main__.py
--rw-r--r--   0        0        0      313 2023-06-09 12:49:06.826100 screener-0.4.1/screener/checker.py
--rw-r--r--   0        0        0      859 2023-06-09 12:49:06.827100 screener-0.4.1/screener/diagnostic.py
--rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.4.1/screener/parser/__init__.py
--rw-r--r--   0        0        0      960 2023-06-09 12:49:06.827100 screener-0.4.1/screener/parser/epub.py
--rw-r--r--   0        0        0      902 2023-06-09 12:49:06.827100 screener-0.4.1/screener/parser/kindle.py
--rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.4.1/screener/reader/__init__.py
--rw-r--r--   0        0        0      806 2023-06-11 13:17:10.597748 screener-0.4.1/screener/reader/abstract.py
--rw-r--r--   0        0        0      831 2023-06-11 13:17:10.598748 screener-0.4.1/screener/reader/epub.py
--rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.4.1/screener/reader/kindle.py
--rw-r--r--   0        0        0     1040 2023-06-09 12:49:06.827100 screener-0.4.1/screener/utils.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 screener-0.4.1/setup.py
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 screener-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-07-23 20:31:38.538067 screener-0.5.0/README.md
+-rw-r--r--   0        0        0     2654 2023-07-28 15:00:22.602674 screener-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-06-12 09:05:19.412082 screener-0.5.0/screener/__init__.py
+-rw-r--r--   0        0        0     2013 2023-07-28 15:00:22.602674 screener-0.5.0/screener/__main__.py
+-rw-r--r--   0        0        0      313 2023-06-12 09:05:19.412082 screener-0.5.0/screener/checker.py
+-rw-r--r--   0        0        0     1150 2023-07-28 15:00:22.602674 screener-0.5.0/screener/diagnostic.py
+-rw-r--r--   0        0        0      157 2023-06-12 09:05:19.412082 screener-0.5.0/screener/parser/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-12 09:05:19.412082 screener-0.5.0/screener/parser/epub.py
+-rw-r--r--   0        0        0      902 2023-06-12 09:05:19.412082 screener-0.5.0/screener/parser/kindle.py
+-rw-r--r--   0        0        0      150 2023-06-12 09:05:19.412082 screener-0.5.0/screener/reader/__init__.py
+-rw-r--r--   0        0        0      806 2023-06-12 09:05:19.412082 screener-0.5.0/screener/reader/abstract.py
+-rw-r--r--   0        0        0      831 2023-06-12 09:05:19.412082 screener-0.5.0/screener/reader/epub.py
+-rw-r--r--   0        0        0     1379 2023-07-23 20:25:21.921706 screener-0.5.0/screener/reader/kindle.py
+-rw-r--r--   0        0        0     1069 2023-07-28 15:00:22.602674 screener-0.5.0/screener/utils.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 screener-0.5.0/PKG-INFO
```

### Comparing `screener-0.4.1/pyproject.toml` & `screener-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Screener"
-version = "0.4.1"
+version = "0.5.0"
 description = "Check e-book files for security and privacy issues."
 authors = ["Tom Kuson <mail@tjkuson.me>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "screener", from = "." },
 ]
@@ -23,15 +23,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 mypy = "^1.2.0"
 types-beautifulsoup4 = "^4.12.0.5"
-ruff = "^0.0.272"
+ruff = ">=0.0.274,<0.0.281"
 ssort = "^0.11.6"
 
 [tool.black]
 line-length = 88
 target-version = ["py310"]
 
 [tool.ruff]
@@ -50,26 +50,29 @@
     "A",       # flake8-builtins
     "C4",      # flake8-comprehensions
     "DTZ",     # flake8-datetimez
     "EM",      # flake8-errmsg
     "EXE",     # flake8-executable
     "FA",      # flake8-future-annotations
     "ISC",     # flake8-implicit-str-concat
+    "ICN",     # flake8-import-conventions
     "G",       # flake8-logging-format
     "PIE",     # flake8-pie
     "PT",      # flak8-pytest-style
     "RET",     # flake8-return
     "SIM",     # flake8-simplify
     "TID",     # flake8-tidy-imports
     "TCH",     # flake8-type-checking
     "ARG",     # flake8-unused-arguments
     "PTH",     # flake8-use-pathlib
     "PGH",     # pygrep-hooks
     "PL",      # Pylint
     "TRY",     # tryceratops
+    "FLY",     # flynt
+    "PERF",    # perflint
     "RUF",     # Ruff-specific rules
 ]
 ignore = [
     "ANN101",  # missing-type-self
     "ANN102",  # missing-type-cls
     "D203",    # one-blank-line-before-class
     "D213",    # multi-line-summary-second-line
```

### Comparing `screener-0.4.1/screener/__main__.py` & `screener-0.5.0/screener/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,21 @@
         usage="%(prog)s [OPTION] [FILE]...",
         description="Check e-book files for security and privacy issues.",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
-        version=f"{parser.prog} version 0.4.1",
+        version=f"{parser.prog} version 0.5.0",
     )
     parser.add_argument("files", nargs="*")
     return parser
 
 
-def check_file(
-    file: Path,
-) -> Checker:
+def check_file(file: Path) -> Checker:
     """Check file."""
     checker = Checker(file)
     match extension := file.suffix:
         case ".epub":
             with EpubFileReader(file) as epub:
                 parse_epub(checker, epub.file_path)
         case ".azw3" | ".mobi":
```

### Comparing `screener-0.4.1/screener/parser/epub.py` & `screener-0.5.0/screener/parser/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.1/screener/parser/kindle.py` & `screener-0.5.0/screener/parser/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.1/screener/reader/abstract.py` & `screener-0.5.0/screener/reader/abstract.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.1/screener/reader/epub.py` & `screener-0.5.0/screener/reader/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.1/screener/reader/kindle.py` & `screener-0.5.0/screener/reader/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.4.1/screener/utils.py` & `screener-0.5.0/screener/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 def html_contains_javascript(
     checker: Checker, content: bytes
 ) -> list[JavaScriptDiagnostic] | None:
     """Check if HTML contains JavaScript."""
     soup = BeautifulSoup(content, "html.parser")
     if scripts := soup.find_all("script"):
-        return [JavaScriptDiagnostic(checker.file_path.name) for _ in scripts]
+        return [JavaScriptDiagnostic(checker.file_path.name, str(s)) for s in scripts]
     return None
 
 
 def html_contains_images_with_external_sources(
     checker: Checker, content: bytes
 ) -> list[ExternalImageDiagnostic] | None:
     """Check if HTML contains images with external sources."""
     soup = BeautifulSoup(content, "html.parser")
     images = soup.find_all("img")
     if external_images := tuple(i for i in images if i["src"].startswith("http")):
         return [
-            ExternalImageDiagnostic(checker.file_path.name) for _ in external_images
+            ExternalImageDiagnostic(checker.file_path.name, str(i))
+            for i in external_images
         ]
     return None
```

### Comparing `screener-0.4.1/setup.py` & `screener-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,95 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: screener
+Version: 0.5.0
+Summary: Check e-book files for security and privacy issues.
+Home-page: https://github.com/tjkuson/screener/
+License: LGPL-3.0-only
+Keywords: ebook,security,privacy,epub,mobi,kindle
+Author: Tom Kuson
+Author-email: mail@tjkuson.me
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Security
+Classifier: Topic :: Utilities
+Requires-Dist: EbookLib (>=0.18,<0.19)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: mobi (>=0.3.3,<0.4.0)
+Project-URL: Repository, https://github.com/tjkuson/screener/
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': '.'}
+# Screener
 
-packages = \
-['screener', 'screener.parser', 'screener.reader']
+[![image](https://img.shields.io/pypi/v/screener.svg)](https://pypi.python.org/pypi/screener)
+[![image](https://img.shields.io/pypi/pyversions/screener.svg)](https://pypi.python.org/pypi/screener)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['EbookLib>=0.18,<0.19', 'beautifulsoup4>=4.12.2,<5.0.0', 'mobi>=0.3.3,<0.4.0']
-
-entry_points = \
-{'console_scripts': ['screener = screener.__main__:main']}
-
-setup_kwargs = {
-    'name': 'screener',
-    'version': '0.4.1',
-    'description': 'Check e-book files for security and privacy issues.',
-    'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreener is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
-    'author': 'Tom Kuson',
-    'author_email': 'mail@tjkuson.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/tjkuson/screener/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+Check e-book files for security and privacy issues.
 
+## Motivation
+
+E-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.
+
+Screener aims to check e-book files for these issues so that you can read with peace of mind!
+
+## Features
+
+- Check e-book files for JavaScript tags.
+- Check e-book files for images with external sources to prevent tracking.
+- Supports `.epub`, `.mobi`, and `.azw3` files.
+
+## Get started
+
+### Prerequisites
+
+Screener requires [Python](https://www.python.org/about/gettingstarted/).
+
+### Installing
+
+Screener is available on [PyPI](https://pypi.org/project/screener/). To install, run:
+
+```bash
+pip install screener
+```
+
+#### Development installation
+
+To install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:
+
+```bash
+poetry install
+```
+
+### Usage
+
+To check a file, try:
+
+```shell
+screener path/to/file.epub
+```
+
+For help:
+
+```shell
+screener --help
+```
+
+## Contributing
+
+Pull requests are welcome and appreciated. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.
+
+If you have found a bug or have a feature request, please open an issue.
+
+## Versioning
+
+This project uses [SemVer](http://semver.org/) for versioning.
+
+## Authors
+
+Screener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).
+
+## Licence
+
+Screener is released under the [LGPL version 3](LICENCE).
 
-setup(**setup_kwargs)
```

