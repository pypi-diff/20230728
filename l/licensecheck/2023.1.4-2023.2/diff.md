# Comparing `tmp/licensecheck-2023.1.4.tar.gz` & `tmp/licensecheck-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensecheck-2023.1.4.tar", max compression
+gzip compressed data, was "licensecheck-2023.2.tar", max compression
```

## Comparing `licensecheck-2023.1.4.tar` & `licensecheck-2023.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1080 2023-01-01 17:53:39.457996 licensecheck-2023.1.4/LICENSE.md
-drwxr-xr-x   0        0        0        0 2023-06-26 14:29:06.714033 licensecheck-2023.1.4/licensecheck/
--rw-r--r--   0        0        0     3140 2023-06-26 14:29:46.377779 licensecheck-2023.1.4/licensecheck/__init__.py
--rw-r--r--   0        0        0      113 2023-06-26 14:29:06.339833 licensecheck-2023.1.4/licensecheck/__main__.py
--rw-r--r--   0        0        0     4677 2023-06-26 14:29:06.705231 licensecheck-2023.1.4/licensecheck/formatter.py
--rw-r--r--   0        0        0     4606 2023-06-26 14:29:06.711077 licensecheck-2023.1.4/licensecheck/get_deps.py
--rw-r--r--   0        0        0     5744 2023-06-26 14:29:06.336558 licensecheck-2023.1.4/licensecheck/license_matrix.py
--rw-r--r--   0        0        0     5323 2023-06-26 14:29:06.337555 licensecheck-2023.1.4/licensecheck/packageinfo.py
--rw-r--r--   0        0        0     2459 2023-01-01 17:53:39.466968 licensecheck-2023.1.4/licensecheck/pypi_licenses/osi_approved.txt
--rw-r--r--   0        0        0      652 2023-01-01 17:53:39.466968 licensecheck-2023.1.4/licensecheck/pypi_licenses/other.txt
--rw-r--r--   0        0        0     2258 2023-06-26 14:29:06.338832 licensecheck-2023.1.4/licensecheck/types.py
--rw-r--r--   0        0        0     2256 2023-06-26 14:31:57.050210 licensecheck-2023.1.4/pyproject.toml
--rw-r--r--   0        0        0    22924 2023-03-07 00:27:16.455942 licensecheck-2023.1.4/README.md
--rw-r--r--   0        0        0    24672 1970-01-01 00:00:00.000000 licensecheck-2023.1.4/setup.py
--rw-r--r--   0        0        0    24472 1970-01-01 00:00:00.000000 licensecheck-2023.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-01-01 17:53:39.457996 licensecheck-2023.2/LICENSE.md
+drwxr-xr-x   0        0        0        0 2023-07-28 01:28:25.993549 licensecheck-2023.2/licensecheck/
+-rw-r--r--   0        0        0     3151 2023-07-28 01:28:25.666660 licensecheck-2023.2/licensecheck/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-28 01:28:25.666660 licensecheck-2023.2/licensecheck/__main__.py
+-rw-r--r--   0        0        0     4677 2023-07-28 01:28:25.662660 licensecheck-2023.2/licensecheck/formatter.py
+-rw-r--r--   0        0        0     4895 2023-07-28 01:28:25.663661 licensecheck-2023.2/licensecheck/get_deps.py
+-rw-r--r--   0        0        0     4447 2023-07-28 01:28:25.664660 licensecheck-2023.2/licensecheck/license_matrix.py
+-rw-r--r--   0        0        0     1789 2023-07-27 22:51:47.916428 licensecheck-2023.2/licensecheck/matrix.csv
+-rw-r--r--   0        0        0     5323 2023-07-28 01:28:25.665659 licensecheck-2023.2/licensecheck/packageinfo.py
+-rw-r--r--   0        0        0     2459 2023-01-01 17:53:39.466968 licensecheck-2023.2/licensecheck/pypi_licenses/osi_approved.txt
+-rw-r--r--   0        0        0      652 2023-01-01 17:53:39.466968 licensecheck-2023.2/licensecheck/pypi_licenses/other.txt
+-rw-r--r--   0        0        0     2258 2023-07-28 01:28:25.665659 licensecheck-2023.2/licensecheck/types.py
+-rw-r--r--   0        0        0     2218 2023-07-28 01:33:33.406856 licensecheck-2023.2/pyproject.toml
+-rw-r--r--   0        0        0    22924 2023-03-07 00:27:16.455942 licensecheck-2023.2/README.md
+-rw-r--r--   0        0        0    24636 1970-01-01 00:00:00.000000 licensecheck-2023.2/setup.py
+-rw-r--r--   0        0        0    24422 1970-01-01 00:00:00.000000 licensecheck-2023.2/PKG-INFO
```

### Comparing `licensecheck-2023.1.4/LICENSE.md` & `licensecheck-2023.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.1.4/licensecheck/__init__.py` & `licensecheck-2023.2/licensecheck/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,15 +97,17 @@
 
 	# Are any licenses incompatible?
 	incompatible = any(not lice.licenseCompat for lice in depsWithLicenses)
 
 	# Format the results
 	if simpleConf.get("format", "simple") in formatter.formatMap:
 		print(
-			formatter.formatMap[simpleConf.get("format", "simple")](myLice, sorted(depsWithLicenses)),
+			formatter.formatMap[simpleConf.get("format", "simple")](
+				myLice, sorted(depsWithLicenses)
+			),
 			file=filename,
 		)
 	else:
 		exitCode = 2
 
 	# Exit code of 1 if args.zero
 	if simpleConf.get("zero", False) and incompatible:
```

### Comparing `licensecheck-2023.1.4/licensecheck/formatter.py` & `licensecheck-2023.2/licensecheck/formatter.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.1.4/licensecheck/get_deps.py` & `licensecheck-2023.2/licensecheck/get_deps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,24 @@
 """Get a list of packages with package compatibility.
 """
 from __future__ import annotations
 
-import subprocess
-import warnings
+from importlib import metadata
 from pathlib import Path
 
-import requirements
+import pkg_resources
+import requests
 import tomli
-from requirements.requirement import Requirement
 
 from licensecheck import license_matrix, packageinfo
 from licensecheck.types import JOINS, License, PackageInfo
 
 USINGS = ["requirements", "poetry", "PEP631"]
 
 
-def _doSysExec(command: str) -> tuple[int, str]:
-	"""Execute a command and check for errors.
-
-	Args:
-		command (str): commands as a string
-
-	Raises:
-		RuntimeWarning: throw a warning should there be a non exit code
-
-	Returns:
-		tuple[int, str]: exit code and message
-	"""
-	with subprocess.Popen(
-		command,
-		shell=True,
-		stdout=subprocess.PIPE,
-		stderr=subprocess.STDOUT,
-		encoding="utf-8",
-		errors="ignore",
-	) as process:
-		out = process.communicate()[0]
-		exitCode = process.returncode
-	return exitCode, out
-
-
 def getReqs(using: str) -> set[str]:
 	"""Get requirements for the end user project/ lib.
 
 	>>> getReqs("poetry")
 	>>> getReqs("poetry:dev")
 	>>> getReqs("requirements")
 	>>> getReqs("requirements:requirements.txt;requirements-dev.txt")
@@ -53,57 +27,94 @@
 
 	Args:
 		using (str): use requirements, poetry or PEP631.
 
 	Returns:
 		set[str]: set of requirement packages
 	"""
+
+	resolveReq = lambda req: pkg_resources.Requirement.parse(req).project_name.lower()
+
 	_ = using.split(":", 1)
 	using, extras = _[0], _[1] if len(_) > 1 else None
 	if using not in USINGS:
 		using = "poetry"
 	reqs = set()
 
-	# Is poetry installed?
-	if using == "poetry" and _doSysExec("poetry -h")[0] != 0:
-		using = "requirements"  # Poetry not installed - fall back to requirements
-		warnings.warn(RuntimeWarning("poetry is not on the system path"))
-
-	# Poetry
-	if using == "poetry":  # Use poetry show to get dependents of dependencies
-		lines = _doSysExec("poetry show " + ("" if extras else "--only main"))[1].splitlines(False)
-		for line in lines:
-			try:
-				parts = line.split()
-				reqs.add(parts[0].lower())
-			except IndexError:
-				print(
-					"An error occurred with poetry, try running 'poetry show' to "
-					"see what went wrong! - (fall back to requirements)"
-				)
-				using = "requirements"  # Poetry died - fall back to requirements
-				break
+	pyprojectPath = Path("pyproject.toml")
+	pyproject = {}
+	if pyprojectPath.exists():
+		pyproject = tomli.loads(pyprojectPath.read_text(encoding="utf-8"))
+
+	if using == "poetry":
+		try:
+			project = pyproject["tool"]["poetry"]
+			reqLists = [project["dependencies"]]
+		except KeyError as error:
+			raise RuntimeError(
+				"Could not find specification of requirements (pyproject.toml)."
+			) from error
+		if extras:
+			reqLists.extend(
+				project.get("group", {x: {"dependencies": {}}})[x]["dependencies"]
+				for x in extras.split(";")
+			)
+			reqLists.append(project.get("dev-dependencies", {}))
+		for reqList in reqLists:
+			for req in reqList:
+				reqs.add(resolveReq(req))
 
 	# PEP631 (hatch)
 	if using == "PEP631":
-		project = tomli.loads(Path("pyproject.toml").read_text(encoding="utf-8"))["project"]
-		reqLists = [project["dependencies"]]
+		try:
+			project = pyproject["project"]
+			reqLists = [project["dependencies"]]
+		except KeyError as error:
+			raise RuntimeError(
+				"Could not find specification of requirements (pyproject.toml)."
+			) from error
 		if extras:
 			reqLists.extend(project["optional-dependencies"][x] for x in extras.split(";"))
 		for reqList in reqLists:
 			for req in reqList:
-				reqs.add(str(Requirement.parse(req).name).lower())
+				reqs.add(resolveReq(req))
 
 	# Requirements
 	if using == "requirements":
 		for reqTxt in (extras or "requirements.txt").split(";"):
-			with open(reqTxt, encoding="utf-8") as requirementsTxt:
-				for req in requirements.parse(requirementsTxt):
-					reqs.add(str(req.name).lower())
-	return reqs
+
+			reqPath = Path(reqTxt)
+			if not reqPath.exists():
+				raise RuntimeError(f"Could not find specification of requirements ({reqPath}).")
+
+			for req in reqPath.read_text("utf-8").strip().split("\n"):
+				reqs.add(resolveReq(req))
+
+	try:
+		reqs.remove("python")
+	except KeyError:
+		pass
+
+	# Get Dependencies (1 deep)
+	requirementsWithDeps = reqs.copy()
+	for requirement in reqs:
+		try:
+			pkgMetadata = metadata.metadata(resolveReq(requirement))
+			for req in [resolveReq(req) for req in pkgMetadata.get_all("Requires-Dist") or []]:
+				requirementsWithDeps.add(req)
+		except metadata.PackageNotFoundError:
+			request = requests.get(f"https://pypi.org/pypi/{requirement}/json", timeout=60)
+			response = request.json()
+			try:
+				for req in [resolveReq(req) for req in response["info"]["requires_dist"]]:
+					requirementsWithDeps.add(req)
+			except KeyError:
+				pass
+
+	return requirementsWithDeps
 
 
 def getDepsWithLicenses(
 	using: str,
 	ignorePackages: list[str],
 	failPackages: list[str],
 	ignoreLicenses: list[str],
```

### Comparing `licensecheck-2023.1.4/licensecheck/packageinfo.py` & `licensecheck-2023.2/licensecheck/packageinfo.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.1.4/licensecheck/pypi_licenses/osi_approved.txt` & `licensecheck-2023.2/licensecheck/pypi_licenses/osi_approved.txt`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.1.4/licensecheck/pypi_licenses/other.txt` & `licensecheck-2023.2/licensecheck/pypi_licenses/other.txt`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.1.4/licensecheck/types.py` & `licensecheck-2023.2/licensecheck/types.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.1.4/pyproject.toml` & `licensecheck-2023.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "licensecheck"
-version = "2023.1.4"
+version = "2023.2"
 license = "mit"
 description = "Output the licenses used by dependencies and check if these are compatible with the project license"
 authors = ["FredHappyface"]
 classifiers = [
 	"Environment :: Console",
 	"Environment :: MacOS X",
 	"Environment :: Win32 (MS Windows)",
@@ -24,15 +24,14 @@
 readme = "README.md"
 
 [tool.poetry.scripts]
 licensecheck = 'licensecheck:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requirements-parser = "<2,>=0.5.0"
 requests = "<3,>=2.31.0"
 fhconfparser = "<2024,>=2022"
 tomli = "<3,>=2.0.1"
 rich = "<14,>=13.4.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
```

### Comparing `licensecheck-2023.1.4/README.md` & `licensecheck-2023.2/README.md`

 * *Files identical despite different names*

### Comparing `licensecheck-2023.1.4/setup.py` & `licensecheck-2023.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
 package_data = \
 {'': ['*'], 'licensecheck': ['pypi_licenses/*']}
 
 install_requires = \
 ['fhconfparser>=2022,<2024',
  'requests>=2.31.0,<3',
- 'requirements-parser>=0.5.0,<2',
  'rich>=13.4.2,<14',
  'tomli>=2.0.1,<3']
 
 entry_points = \
 {'console_scripts': ['licensecheck = licensecheck:cli']}
 
 setup_kwargs = {
     'name': 'licensecheck',
-    'version': '2023.1.4',
+    'version': '2023.2',
     'description': 'Output the licenses used by dependencies and check if these are compatible with the project license',
     'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/licensecheck.svg?style=for-the-badge)](https://pypistats.org/packages/licensecheck)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Flicensecheck)](https://pepy.tech/project/licensecheck)\n[![PyPI Version](https://img.shields.io/pypi/v/licensecheck.svg?style=for-the-badge)](https://pypi.org/project/licensecheck)\n\n<!-- omit in toc -->\n# LicenseCheck\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nOutput the licences used by dependencies and check if these are compatible with\nthe project license\n\n<!-- omit in toc -->\n## Table of Contents\n\n- [Examples from the command-line](#examples-from-the-command-line)\n\t- [Using requirements](#using-requirements)\n\t- [Failing on packages under MIT license](#failing-on-packages-under-mit-license)\n\t- [Custom requirements.txt in json format](#custom-requirementstxt-in-json-format)\n\t- [Poetry with dev requirements](#poetry-with-dev-requirements)\n\t- [PEP 631 (with or without optional dependencies)](#pep-631-with-or-without-optional-dependencies)\n- [Help](#help)\n- [Configuration Example](#configuration-example)\n\t- [Example 1: pyproject.toml](#example-1-pyprojecttoml)\n\t- [Example 2: licensecheck.json](#example-2-licensecheckjson)\n\t- [Example 3: licensecheck.ini](#example-3-licensecheckini)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Examples from the command-line\n\nSee below for the output if you run `licensecheck` in this directory\n\n```txt\n>> licensecheck\n\n                             list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                           ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ urllib3             │ MIT License                          │\n│ ✔          │ types-setuptools    │ Apache Software License              │\n│ ✔          │ tomli               │ MIT License                          │\n│ ✔          │ idna                │ BSD License                          │\n│ ✔          │ Pygments            │ BSD License                          │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0) │\n│ ✔          │ fhconfparser        │ MIT License                          │\n│ ✔          │ rich                │ MIT License                          │\n│ ✔          │ charset-normalizer  │ MIT License                          │\n│ ✔          │ requirements-parser │ Apache Software License              │\n│ ✔          │ commonmark          │ BSD License                          │\n│ ✔          │ requests            │ Apache Software License              │\n│ ✔          │ attrs               │ MIT License                          │\n└────────────┴─────────────────────┴──────────────────────────────────────┘\n```\n\n### Using requirements\n\n```txt\n>> licensecheck -u requirements\n\n                       list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)              ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ requirements-parser │ Apache Software License │\n│ ✔          │ requests            │ Apache Software License │\n│ ✔          │ rich                │ MIT License             │\n│ ✔          │ fhconfparser        │ MIT License             │\n│ ✔          │ tomli               │ MIT License             │\n└────────────┴─────────────────────┴─────────────────────────┘\n```\n\n### Failing on packages under MIT license\n\n```txt\n>> licensecheck --fail-licenses mit\n\n                             list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                           ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ idna                │ BSD License                          │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0) │\n│ ✔          │ Pygments            │ BSD License                          │\n│ ✔          │ commonmark          │ BSD License                          │\n│ ✔          │ requirements-parser │ Apache Software License              │\n│ ✖          │ fhconfparser        │ MIT License                          │\n│ ✖          │ tomli               │ MIT License                          │\n│ ✔          │ types-setuptools    │ Apache Software License              │\n│ ✖          │ attrs               │ MIT License                          │\n│ ✖          │ charset-normalizer  │ MIT License                          │\n│ ✖          │ rich                │ MIT License                          │\n│ ✖          │ urllib3             │ MIT License                          │\n│ ✔          │ requests            │ Apache Software License              │\n└────────────┴─────────────────────┴──────────────────────────────────────┘\n```\n\n### Custom requirements.txt in json format\n\nAdd optional path to requirements.txt as outlined in https://github.com/FHPythonUtils/LicenseCheck/issues/9#issuecomment-898878228. Eg. `licensecheck --using requirements:c:/path/to/reqs.txt;path/to/other/reqs.txt`\n\n```txt\n>> licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json\n{\n\t"info": {\n\t\t"program": "licensecheck",\n\t\t"version": "2022.2.0"\n\t},\n\t"packages": [\n\t\t{\n\t\t\t"name": "requests",\n\t\t\t"version": "2.28.1",\n\t\t\t"namever": "requests-2.28.1",\n\t\t\t"size": 180253,\n\t\t\t"homePage": "https://requests.readthedocs.io",\n\t\t\t"author": "Kenneth Reitz",\n\t\t\t"license": "Apache Software License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "rich",\n\t\t\t"version": "12.6.0",\n\t\t\t"namever": "rich-12.6.0",\n\t\t\t"size": 905975,\n\t\t\t"homePage": "https://github.com/willmcgugan/rich",\n\t\t\t"author": "Will McGugan",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "tomli",\n\t\t\t"version": "2.0.1",\n\t\t\t"namever": "tomli-2.0.1",\n\t\t\t"size": 26252,\n\t\t\t"homePage": "UNKNOWN",\n\t\t\t"author": "UNKNOWN",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "requirements-parser",\n\t\t\t"version": "0.5.0",\n\t\t\t"namever": "requirements-parser-0.5.0",\n\t\t\t"size": 11523,\n\t\t\t"homePage": "https://github.com/madpah/requirements-parser",\n\t\t\t"author": "Paul Horton",\n\t\t\t"license": "Apache Software License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t},\n\t\t{\n\t\t\t"name": "fhconfparser",\n\t\t\t"version": "2022",\n\t\t\t"namever": "fhconfparser-2022",\n\t\t\t"size": 14586,\n\t\t\t"homePage": "https://github.com/FHPythonUtils/FHConfParser",\n\t\t\t"author": "FredHappyface",\n\t\t\t"license": "MIT License",\n\t\t\t"licenseCompat": true,\n\t\t\t"errorCode": 0\n\t\t}\n\t]\n}\n```\n\n### Poetry with dev requirements\n\nAdd `-u poetry:dev` to command-line to include dev packages (excluded by default)\n\n```txt\n>> licensecheck -u poetry:dev\n\n                                  list of packages\n┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Compatible ┃ Package             ┃ License(s)                                    ┃\n┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ ✔          │ astroid             │ GNU Lesser General Public License v2 (LGPLv2) │\n│ ✔          │ rich                │ MIT License                                   │\n│ ✔          │ types-setuptools    │ Apache Software License                       │\n│ ✔          │ fhconfparser        │ MIT License                                   │\n│ ✔          │ typed-ast           │ Apache License 2.0                            │\n│ ✔          │ py                  │ MIT License                                   │\n│ ✔          │ mccabe              │ MIT License                                   │\n│ ✔          │ tomlkit             │ MIT License                                   │\n│ ✔          │ coverage            │ Apache Software License                       │\n│ ✔          │ Pygments            │ BSD License                                   │\n│ ✔          │ requests            │ Apache Software License                       │\n│ ✔          │ requirements-parser │ Apache Software License                       │\n│ ✔          │ tomli               │ MIT License                                   │\n│ ✔          │ pluggy              │ MIT License                                   │\n│ ✔          │ isort               │ MIT License                                   │\n│ ✔          │ urllib3             │ MIT License                                   │\n│ ✖          │ pylint              │ GNU General Public License v2 (GPLv2)         │\n│ ✔          │ iniconfig           │ MIT License                                   │\n│ ✔          │ wrapt               │ BSD License                                   │\n│ ✔          │ pytest              │ MIT License                                   │\n│ ✔          │ pip                 │ MIT License                                   │\n│ ✔          │ charset-normalizer  │ MIT License                                   │\n│ ✔          │ packaging           │ Apache Software License, BSD License          │\n│ ✔          │ commonmark          │ BSD License                                   │\n│ ✔          │ lazy-object-proxy   │ BSD License                                   │\n│ ✔          │ platformdirs        │ MIT License                                   │\n│ ✔          │ certifi             │ Mozilla Public License 2.0 (MPL 2.0)          │\n│ ✔          │ colorama            │ BSD License                                   │\n│ ✔          │ attrs               │ MIT License                                   │\n│ ✔          │ dill                │ BSD License                                   │\n│ ✔          │ idna                │ BSD License                                   │\n│ ✔          │ importlib-resources │ Apache Software License                       │\n│ ✔          │ handsdown           │ MIT License                                   │\n│ ✔          │ pyparsing           │ MIT License                                   │\n└────────────┴─────────────────────┴───────────────────────────────────────────────┘\n```\n\n### PEP 631 (with or without optional dependencies)\n\nPEP 631 mode enables support for reading dependency information from `pyproject.toml` in the format specified by PEP 631.\nThis format is used by build systems such as hatch.\n\nYou can enable this mode by using `-u PEP631`, and include the optional dependencies of extras by using `-u PEP631:tests;dev;docs`,\nbut it\'s recommended to use this instead:\n\n```toml\n[tool.licensecheck]\nusing = "PEP631"\n\n# OR\n\n[tool.licensecheck]\nusing = "PEP631:tests;dev;docs"\n```\n\nBy default no optional dependencies are included.\n\n## Help\n\n```txt\nusage: __main__.py [-h] [--format FORMAT] [--file FILE] [--using USING]\n                   [--ignore-packages IGNORE_PACKAGES [IGNORE_PACKAGES ...]]\n                   [--fail-packages FAIL_PACKAGES [FAIL_PACKAGES ...]]\n                   [--ignore-licenses IGNORE_LICENSES [IGNORE_LICENSES ...]]\n                   [--fail-licenses FAIL_LICENSES [FAIL_LICENSES ...]] [--zero]\n\nOutput the licenses used by dependencies and check if these are compatible with the project license.\n\noptions:\n  -h, --help            show this help message and exit\n  --format FORMAT, -f FORMAT\n                        Output format. one of: json, markdown, csv, ansi, simple. default=simple\n  --file FILE, -o FILE  Filename to write to (omit for stdout)\n  --using USING, -u USING\n                        Environment to use e.g. requirements.txt. one of: requirements, poetry, PEP631. default=poetry\n  --ignore-packages IGNORE_PACKAGES [IGNORE_PACKAGES ...]\n                        a list of packages to ignore (compat=True)\n  --fail-packages FAIL_PACKAGES [FAIL_PACKAGES ...]\n                        a list of packages to fail (compat=False)\n  --ignore-licenses IGNORE_LICENSES [IGNORE_LICENSES ...]\n                        a list of licenses to ignore (skipped, compat may still be False)\n  --fail-licenses FAIL_LICENSES [FAIL_LICENSES ...]\n                        a list of licenses to fail (compat=False)\n  --zero, -0            Return non zero exit code if an incompatible license is found\n```\n\nYou can also import this into your own project and use any of the functions\nin the DOCS\n\n## Configuration Example\n\nConfiguration files are parsed in the following order: `pyproject.toml`,\n`setup.cfg`, `licensecheck.toml`, `licensecheck.json`, `licensecheck.ini`,\n`~/licensecheck.toml`, `~/licensecheck.json`, `~/licensecheck.ini`\n\n- ⚠ All config files are parsed, however configuration defined in previous files takes precedent\n\nAdd optional path to requirements.txt as outlined in\nhttps://github.com/FHPythonUtils/LicenseCheck/issues/9#issuecomment-898878228\nfor example: `licensecheck --using requirements:c:/path/to/reqs.txt;path/to/other/reqs.txt`\n\n### Example 1: pyproject.toml\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```toml\n[tool.licensecheck]\nusing = "requirements:requirements.txt;requirements_optional.txt"\nformat = "json"\n```\n\n### Example 2: licensecheck.json\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```json\n{\n\t"tool": {\n\t\t"licensecheck": {\n\t\t\t"using": "requirements:requirements.txt;requirements_optional.txt",\n\t\t\t"format": "json"\n\t\t}\n\t}\n}\n```\n\n### Example 3: licensecheck.ini\n\nThe following config is equivalent to `licensecheck -u \'requirements:requirements.txt;requirements_optional.txt\' -f json`\n\n```ini\n[licensecheck]\nusing = "requirements:requirements.txt;requirements_optional.txt"\nformat = "json"\n```\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install licensecheck\n```\n\nHead to https://pypi.org/project/licensecheck/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/LicenseCheck\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
     'author': 'FredHappyface',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FHPythonUtils/LicenseCheck',
```

### Comparing `licensecheck-2023.1.4/PKG-INFO` & `licensecheck-2023.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensecheck
-Version: 2023.1.4
+Version: 2023.2
 Summary: Output the licenses used by dependencies and check if these are compatible with the project license
 Home-page: https://github.com/FHPythonUtils/LicenseCheck
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: fhconfparser (>=2022,<2024)
 Requires-Dist: requests (>=2.31.0,<3)
-Requires-Dist: requirements-parser (>=0.5.0,<2)
 Requires-Dist: rich (>=13.4.2,<14)
 Requires-Dist: tomli (>=2.0.1,<3)
 Project-URL: Documentation, https://github.com/FHPythonUtils/LicenseCheck/blob/master/README.md
 Project-URL: Repository, https://github.com/FHPythonUtils/LicenseCheck
 Description-Content-Type: text/markdown
 
 [![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/LicenseCheck.svg?style=for-the-badge)](../../)
```

