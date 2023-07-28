# Comparing `tmp/profet-0.0.0.tar.gz` & `tmp/profet-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profet-0.0.0.tar", last modified: Fri Jul 28 11:24:41 2023, max compression
+gzip compressed data, was "/Users/bcostagomes/Documents/profet/dist/tmpeoue5zf6/profet-0.0.1.tar", last modified: Thu Apr 14 11:45:34 2022, max compression
```

## Comparing `profet-0.0.0.tar` & `profet-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:24:41.900764 profet-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 11:24:25.000000 profet-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-28 11:24:41.900764 profet-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-28 11:24:25.000000 profet-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:24:41.900764 profet-0.0.0/profet/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 11:24:25.000000 profet-0.0.0/profet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-28 11:24:25.000000 profet-0.0.0/profet/alphafold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-28 11:24:25.000000 profet-0.0.0/profet/pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-28 11:24:25.000000 profet-0.0.0/profet/profet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:24:41.900764 profet-0.0.0/profet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-28 11:24:41.000000 profet-0.0.0/profet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-28 11:24:41.000000 profet-0.0.0/profet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:24:41.000000 profet-0.0.0/profet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 11:24:41.000000 profet-0.0.0/profet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 11:24:41.000000 profet-0.0.0/profet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-28 11:24:25.000000 profet-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-28 11:24:41.904764 profet-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-28 11:24:25.000000 profet-0.0.0/setup.py
+drwxr-xr-x   0 bcostagomes   (503) staff       (20)        0 2022-04-14 11:45:34.588683 profet-0.0.1/
+-rw-r--r--   0 bcostagomes   (503) staff       (20)     1082 2022-04-06 13:38:25.000000 profet-0.0.1/LICENSE
+-rw-r--r--   0 bcostagomes   (503) staff       (20)     2197 2022-04-14 11:45:34.588834 profet-0.0.1/PKG-INFO
+-rw-r--r--   0 bcostagomes   (503) staff       (20)     1605 2022-04-14 11:36:00.000000 profet-0.0.1/README.md
+drwxr-xr-x   0 bcostagomes   (503) staff       (20)        0 2022-04-14 11:45:34.586666 profet-0.0.1/profet/
+-rw-r--r--   0 bcostagomes   (503) staff       (20)       28 2022-04-14 10:28:27.000000 profet-0.0.1/profet/__init__.py
+-rw-r--r--   0 bcostagomes   (503) staff       (20)     2423 2022-04-12 15:08:04.000000 profet-0.0.1/profet/alphafold.py
+-rw-r--r--   0 bcostagomes   (503) staff       (20)     1099 2022-04-12 15:58:55.000000 profet-0.0.1/profet/pdb.py
+-rw-r--r--   0 bcostagomes   (503) staff       (20)     3225 2022-04-14 11:23:21.000000 profet-0.0.1/profet/profet.py
+drwxr-xr-x   0 bcostagomes   (503) staff       (20)        0 2022-04-14 11:45:34.588423 profet-0.0.1/profet.egg-info/
+-rw-r--r--   0 bcostagomes   (503) staff       (20)     2197 2022-04-14 11:45:34.000000 profet-0.0.1/profet.egg-info/PKG-INFO
+-rw-r--r--   0 bcostagomes   (503) staff       (20)      261 2022-04-14 11:45:34.000000 profet-0.0.1/profet.egg-info/SOURCES.txt
+-rw-r--r--   0 bcostagomes   (503) staff       (20)        1 2022-04-14 11:45:34.000000 profet-0.0.1/profet.egg-info/dependency_links.txt
+-rw-r--r--   0 bcostagomes   (503) staff       (20)       60 2022-04-14 11:45:34.000000 profet-0.0.1/profet.egg-info/requires.txt
+-rw-r--r--   0 bcostagomes   (503) staff       (20)        7 2022-04-14 11:45:34.000000 profet-0.0.1/profet.egg-info/top_level.txt
+-rw-r--r--   0 bcostagomes   (503) staff       (20)      283 2022-04-14 11:32:39.000000 profet-0.0.1/pyproject.toml
+-rw-r--r--   0 bcostagomes   (503) staff       (20)      742 2022-04-14 11:45:34.589446 profet-0.0.1/setup.cfg
```

### Comparing `profet-0.0.0/LICENSE` & `profet-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `profet-0.0.0/README.md` & `profet-0.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,56 @@
+Metadata-Version: 2.1
+Name: profet
+Version: 0.0.1
+Summary: Protein structure Fetcher from online databases
+Home-page: https://github.com/alan-turing-institute/profet
+Author: mooniean
+Author-email: bcostagomes@turing.ac.uk
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/alan-turing-institute/profet/issues
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # profet
 A Python 3  **pro**tein structure **fet**cher. Retrieves the cif or pdb files from either the RCSB Protein Data Bank ([PDB](https://www.rcsb.org), using [pypdb](https://github.com/williamgilpin/pypdb)) or [Alphafold](http://alphafold.ebi.ac.uk/) using the [Uniprot](http://uniprot.org/) ID. 
 
-![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![PyPI version shields.io](https://img.shields.io/pypi/v/profet.svg)](https://pypi.python.org/pypi/profet/)
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/python-profet.svg)](https://pypi.python.org/pypi/profet/)
-
-[![Building](https://github.com/alan-turing-institute/profet/actions/workflows/python-package.yml/badge.svg)](https://github.com/alan-turing-institute/profet/actions/workflows/python-package.yml)
-[![Publishing](https://github.com/alan-turing-institute/profet/actions/workflows/python-publish.yml/badge.svg)](https://github.com/alan-turing-institute/profet/actions/workflows/python-publish.yml)
-[![Documentation](https://github.com/alan-turing-institute/profet/actions/workflows/sphinx.yml/badge.svg)](https://github.com/alan-turing-institute/profet/actions/workflows/sphinx.yml)
-
-### Dependencies
-
-Please install the latest version of PyPDB using:
-
-```sh
-pip install pypdb
-```
-
-or
-
-```sh
-pip install git+git://github.com/williamgilpin/pypdb
-```
 
 ### Installation
 
-Install `profet` using pip:
+Install using pip:
 
-```sh
-pip install profet
-```
+`$ pip install profet`
 
 To install the development version, which contains the latest features and fixes, install directly from GitHub using
 
-```sh
-pip install git+git://github.com/alan-turing-institute/profet
-```
+`$ pip install git+git://github.com/alan-turing-institute/profet`
 
 Test the installation, navigate to the root directory and run
 
-```sh
-pytest
-```
+`$ pytest `
 
 This code has been designed and tested for Python 3.
 
 ### Usage
 
 This package can be used to retrieve the available protein structure from any Uniprot ID. 
 
 The `Fetcher` class can search the IDs in both PDB and Alphafold, and saves the search results in a dictionary.
 
 `get_file` returns the structure corresponding to `uniprot_id` in the defined `filetype:` (default as `'pdb'`, option as `'cif'`), searching first in the defaulted database `db` (default as `'pdb'`, option as `'alphafold'`).
 The files can be saved to a local file with `filesave`.
 
 `set_default_db` changes the default database into the given one between `'pdb'` and `'alphafold'`.
 
-`set_directory` changes the directory where the files are saved. Files save as `<directory>/<id>.<filetype>`.
-
 Run `search_history()` to see the search history of the fetcher.
 
-#### Example usage:
-
-```python
-import profet as pf
-fetcher = pf.Fetcher()
-fetcher.set_directory("/path/to/directory/folder")
-fetcher.get_file(uniprot_id = "P61316", filetype = "pdb", filesave = True, db = "alphafold")
-
-fetcher.search_history()
-```
-
-returns:
-```
-{'P61316': ['pdb', 'alphafold']}
-```
-
-Loads Profet and the file-fetcher, then specifies a directory to save the files at.
-Lastly, downloads the protein with uniprod ID "P61316", in pdb format from the Alphafold databank and saves it in the specified directory.
-
-For more detailed examples consult the following [Python notebook](./run_profet.ipynb).
-
-### Documentation
-
-You can find more documentation including a description of the python api [here](https://alan-turing-institute.github.io/profet/).
-
 ### Issues and Feature Requests
+If you run into an issue, or if you find a workaround for an existing issue, we would very much appreciate it if you could post your question or code as a [GitHub issue](https://github.com/alan-turing-institute/profet/issues).
 
-If you run into an issue, or if you find a workaround for an existing issue, we would very much appreciate it if you could post your question or code as a [GitHub issue](https://github.com/alan-turing-institute/profet/issues). 
-
-### Contributions
 
-If you would like to help contribute to profet, please read our [contribution](CONTRIBUTING.md) guide and [code of conduct](CODE_OF_CONDUCT.md).
```

### Comparing `profet-0.0.0/setup.cfg` & `profet-0.0.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 [metadata]
 name = profet
+version = 0.0.1
 author = mooniean
 author_email = bcostagomes@turing.ac.uk
 description = Protein structure Fetcher from online databases
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alan-turing-institute/profet
 project_urls = 
 	Bug Tracker = https://github.com/alan-turing-institute/profet/issues
 classifiers = 
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 include_package_data = True
 install_requires = 
 	numpy
 	pypdb
 	requests
 	pandas
 	requests_html
 	bs4
-	pypdb@git+https://github.com/williamgilpin/pypdb@master#egg=pypdb
 
 [options.extras_require]
 dev = 
 	pytest
-	pytest-cov
-build_sphinx = 
-	sphinx
-	sphinx_rtd_theme
-	sphinx-argparse
-
-[tool:pytest]
-addopts = --cov=profet --cov-report term --cov-report html
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

