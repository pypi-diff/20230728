# Comparing `tmp/equilibrator-cache-0.4.4b1.tar.gz` & `tmp/equilibrator-cache-0.4.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-cache-0.4.4b1.tar", last modified: Wed Oct  6 15:12:24 2021, max compression
+gzip compressed data, was "equilibrator-cache-0.4.4b2.tar", last modified: Sun Oct 17 13:51:50 2021, max compression
```

## Comparing `equilibrator-cache-0.4.4b1.tar` & `equilibrator-cache-0.4.4b2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:12:24.098897 equilibrator-cache-0.4.4b1/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1282 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/LICENSE
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       99 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/MANIFEST.in
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2540 2021-10-06 15:12:24.098897 equilibrator-cache-0.4.4b1/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1146 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/README.md
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      177 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/pyproject.toml
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1980 2021-10-06 15:12:24.102897 equilibrator-cache-0.4.4b1/setup.cfg
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1461 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/setup.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:12:24.094897 equilibrator-cache-0.4.4b1/src/
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:12:24.102897 equilibrator-cache-0.4.4b1/src/equilibrator_cache/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2051 2021-08-03 15:06:06.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/__init__.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      499 2021-10-06 15:12:24.102897 equilibrator-cache-0.4.4b1/src/equilibrator_cache/_version.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2398 2021-07-07 18:52:41.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/api.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     7328 2021-07-07 18:55:37.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/compatibility.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    12488 2021-10-06 15:00:01.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/compound_cache.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1524 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/exceptions.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:12:24.098897 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1965 2021-07-09 19:58:58.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/__init__.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     8365 2021-08-05 14:53:37.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3706 2021-08-02 18:23:29.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound_identifier.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     4205 2021-06-15 08:46:39.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound_microspecies.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3149 2021-08-02 18:23:29.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound_name.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2339 2021-06-15 08:45:23.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/magnesium_dissociation_constant.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2182 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/mixins.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3447 2021-08-03 14:11:27.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/registry.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    23933 2021-02-04 15:07:46.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/reaction.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     4009 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/thermodynamic_constants.py
--rwxrwxr-x   0 moritz    (1000) moritz    (1000)     6665 2021-10-02 21:25:56.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache/zenodo.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-06 15:12:24.098897 equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2540 2021-10-06 15:12:24.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1069 2021-10-06 15:12:24.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/SOURCES.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-10-06 15:12:24.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/dependency_links.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      371 2021-10-06 15:12:24.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/requires.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       19 2021-10-06 15:12:24.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/top_level.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-02-04 15:10:09.000000 equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/zip-safe
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    68611 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b1/versioneer.py
+drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1282 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/LICENSE
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)       99 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/MANIFEST.in
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     2540 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/PKG-INFO
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1146 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/README.md
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)      187 2021-10-17 13:49:42.000000 equilibrator-cache-0.4.4b2/pyproject.toml
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1973 2021-10-17 13:51:50.301437 equilibrator-cache-0.4.4b2/setup.cfg
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1460 2021-10-17 13:47:12.000000 equilibrator-cache-0.4.4b2/setup.py
+drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/src/
+drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.301437 equilibrator-cache-0.4.4b2/src/equilibrator_cache/
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1957 2021-10-17 13:44:45.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/__init__.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)      499 2021-10-17 13:51:50.301437 equilibrator-cache-0.4.4b2/src/equilibrator_cache/_version.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     2398 2021-07-07 18:52:41.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/api.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     7328 2021-07-07 18:55:37.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/compatibility.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)    12488 2021-10-06 15:00:01.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/compound_cache.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1524 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/exceptions.py
+drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1965 2021-07-09 19:58:58.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/__init__.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     8365 2021-08-05 14:53:37.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     3706 2021-08-02 18:23:29.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_identifier.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     4205 2021-06-15 08:46:39.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_microspecies.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     3149 2021-08-02 18:23:29.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_name.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     2339 2021-06-15 08:45:23.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/magnesium_dissociation_constant.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     2182 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/mixins.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     3447 2021-08-03 14:11:27.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/registry.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)    23933 2021-02-04 15:07:46.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/reaction.py
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     4009 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/thermodynamic_constants.py
+-rwxrwxr-x   0 moritz    (1000) moritz    (1000)     6665 2021-10-02 21:25:56.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/zenodo.py
+drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     2540 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/PKG-INFO
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)     1055 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)      365 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/requires.txt
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)       19 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/top_level.txt
+-rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-02-04 15:10:09.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/zip-safe
```

### Comparing `equilibrator-cache-0.4.4b1/LICENSE` & `equilibrator-cache-0.4.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/PKG-INFO` & `equilibrator-cache-0.4.4b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.4b1
+Version: 0.4.4b2
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
```

### Comparing `equilibrator-cache-0.4.4b1/README.md` & `equilibrator-cache-0.4.4b2/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/setup.cfg` & `equilibrator-cache-0.4.4b2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 	pytest-raises
 	pytest-mock
 	hypothesis
 development = 
 	black
 	isort
 	tox
-	twine
 deployment = 
 	click
 	click-log
 	openbabel
 	python-dateutil
 	tqdm
```

### Comparing `equilibrator-cache-0.4.4b1/setup.py` & `equilibrator-cache-0.4.4b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,13 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
-from setuptools import setup
-
 import versioneer
+from setuptools import setup
 
 
 # Most arguments are set in the `setup.cfg`.
 setup(version=versioneer.get_version(), cmdclass=versioneer.get_cmdclass())
```

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/__init__.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,14 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
-from ._version import get_versions
-
-__version__ = get_versions()["version"]
-del get_versions
-
 PROTON_INCHI = "InChI=1S/p+1"
 WATER_INCHI = "InChI=1S/H2O/h1H2"
 PROTON_INCHI_KEY = "GPRLSGONYQIRFK-UHFFFAOYSA-N"
 WATER_INCHI_KEY = "XLYOFNOQVPJJNP-UHFFFAOYSA-N"
 
 
 from .exceptions import ParseException
```

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/api.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/api.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/compatibility.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/compound_cache.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/compound_cache.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/exceptions.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/exceptions.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/__init__.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound_identifier.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_identifier.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound_microspecies.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_microspecies.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/compound_name.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_name.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/magnesium_dissociation_constant.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/magnesium_dissociation_constant.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/mixins.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/mixins.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/models/registry.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/registry.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/reaction.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/reaction.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/thermodynamic_constants.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/thermodynamic_constants.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache/zenodo.py` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache/zenodo.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/PKG-INFO` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.4b1
+Version: 0.4.4b2
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Download-URL: https://pypi.org/project/equilibrator-cache/
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
```

### Comparing `equilibrator-cache-0.4.4b1/src/equilibrator_cache.egg-info/SOURCES.txt` & `equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-versioneer.py
 src/equilibrator_cache/__init__.py
 src/equilibrator_cache/_version.py
 src/equilibrator_cache/api.py
 src/equilibrator_cache/compatibility.py
 src/equilibrator_cache/compound_cache.py
 src/equilibrator_cache/exceptions.py
 src/equilibrator_cache/reaction.py
```

