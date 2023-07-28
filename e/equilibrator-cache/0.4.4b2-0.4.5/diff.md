# Comparing `tmp/equilibrator-cache-0.4.4b2.tar.gz` & `tmp/equilibrator-cache-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-cache-0.4.4b2.tar", last modified: Sun Oct 17 13:51:50 2021, max compression
+gzip compressed data, was "equilibrator-cache-0.4.5.tar", last modified: Fri Jul 28 03:13:20 2023, max compression
```

## Comparing `equilibrator-cache-0.4.4b2.tar` & `equilibrator-cache-0.4.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1282 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/LICENSE
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       99 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/MANIFEST.in
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2540 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1146 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/README.md
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      187 2021-10-17 13:49:42.000000 equilibrator-cache-0.4.4b2/pyproject.toml
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1973 2021-10-17 13:51:50.301437 equilibrator-cache-0.4.4b2/setup.cfg
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1460 2021-10-17 13:47:12.000000 equilibrator-cache-0.4.4b2/setup.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/src/
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.301437 equilibrator-cache-0.4.4b2/src/equilibrator_cache/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1957 2021-10-17 13:44:45.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/__init__.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      499 2021-10-17 13:51:50.301437 equilibrator-cache-0.4.4b2/src/equilibrator_cache/_version.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2398 2021-07-07 18:52:41.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/api.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     7328 2021-07-07 18:55:37.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/compatibility.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    12488 2021-10-06 15:00:01.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/compound_cache.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1524 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/exceptions.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1965 2021-07-09 19:58:58.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/__init__.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     8365 2021-08-05 14:53:37.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3706 2021-08-02 18:23:29.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_identifier.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     4205 2021-06-15 08:46:39.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_microspecies.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3149 2021-08-02 18:23:29.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_name.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2339 2021-06-15 08:45:23.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/magnesium_dissociation_constant.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2182 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/mixins.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     3447 2021-08-03 14:11:27.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/registry.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)    23933 2021-02-04 15:07:46.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/reaction.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     4009 2020-11-11 21:58:35.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/thermodynamic_constants.py
--rwxrwxr-x   0 moritz    (1000) moritz    (1000)     6665 2021-10-02 21:25:56.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache/zenodo.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2021-10-17 13:51:50.297437 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     2540 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1055 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/SOURCES.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/dependency_links.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      365 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/requires.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       19 2021-10-17 13:51:50.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/top_level.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2021-02-04 15:10:09.000000 equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.559857 equilibrator-cache-0.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-07-28 03:13:20.559857 equilibrator-cache-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-07-28 03:13:20.560857 equilibrator-cache-0.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.551857 equilibrator-cache-0.4.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.560857 equilibrator-cache-0.4.5/src/equilibrator_cache/
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-28 03:13:20.560857 equilibrator-cache-0.4.5/src/equilibrator_cache/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)    12786 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/compound_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.559857 equilibrator-cache-0.4.5/src/equilibrator_cache/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11380 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4205 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_microspecies.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/magnesium_dissociation_constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4442 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/models/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    25544 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/reaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/thermodynamic_constants.py
+-rwxrwxrwx   0 root         (0) root         (0)     6665 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/src/equilibrator_cache/zenodo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:13:20.557857 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:13:20.000000 equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-28 03:13:08.000000 equilibrator-cache-0.4.5/versioneer.py
```

### Comparing `equilibrator-cache-0.4.4b2/LICENSE` & `equilibrator-cache-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/PKG-INFO` & `equilibrator-cache-0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.4b2
+Version: 0.4.5
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
+Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
-Download-URL: https://pypi.org/project/equilibrator-cache/
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
 Project-URL: Bug Tracker, https://gitlab.com/equilibrator/equilibrator-cache/-/issues
 Keywords: component contribution,Gibbs energy,biochemical reaction,eQuilibrator,cache
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 equilibrator-cache
@@ -47,9 +45,7 @@
 
 ## Supported Chemical Databases:
 
 * [MetaNetX](https://www.metanetx.org/)
 * [KEGG](https://www.kegg.jp/)
 * [ChEBI](https://www.ebi.ac.uk/chebi/)
 
-
-
```

### Comparing `equilibrator-cache-0.4.4b2/README.md` & `equilibrator-cache-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/setup.cfg` & `equilibrator-cache-0.4.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Chemistry
 license = MIT
 description = Cache application for compounds, reactions, and enzymes
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = 
@@ -31,26 +30,26 @@
 	eQuilibrator
 	cache
 
 [options]
 zip_safe = True
 install_requires = 
 	importlib_resources; python_version <'3.9'
-	tqdm~=4.50
+	tqdm~=4.65
 	appdirs~=1.4
-	numpy~=1.19
-	pandas~=1.0
+	numpy~=1.25
+	pandas~=2.0
 	python-Levenshtein-wheels~=0.13
-	scipy~=1.5
-	sqlalchemy~=1.4
-	pint~=0.14
-	periodictable~=1.5
-	httpx~=0.16
-	tenacity~=6.2
-python_requires = >=3.6
+	scipy~=1.11
+	sqlalchemy>=1.3,<1.4
+	pint~=0.22
+	periodictable~=1.6
+	httpx~=0.24
+	tenacity~=6.3
+python_requires = >=3.8
 tests_require = 
 	tox
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
@@ -60,23 +59,24 @@
 test = 
 	pytest
 	pytest-cov
 	pytest-raises
 	pytest-mock
 	hypothesis
 development = 
-	black
-	isort
-	tox
+	black~=23.3
+	isort~=5.12
+	safety~=2.3
+	tox~=4.6
+	twine~=4.0
 deployment = 
 	click
 	click-log
 	openbabel
 	python-dateutil
-	tqdm
 
 [versioneer]
 VCS = git
 style = pep440
 versionfile_source = src/equilibrator_cache/_version.py
 versionfile_build = equilibrator_cache/_version.py
 tag_prefix =
```

### Comparing `equilibrator-cache-0.4.4b2/setup.py` & `equilibrator-cache-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,13 +21,14 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
-import versioneer
 from setuptools import setup
 
+import versioneer
+
 
 # Most arguments are set in the `setup.cfg`.
 setup(version=versioneer.get_version(), cmdclass=versioneer.get_cmdclass())
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/__init__.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,30 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
+from ._version import get_versions
+
+__version__ = get_versions()["version"]
+del get_versions
+
 PROTON_INCHI = "InChI=1S/p+1"
 WATER_INCHI = "InChI=1S/H2O/h1H2"
 PROTON_INCHI_KEY = "GPRLSGONYQIRFK-UHFFFAOYSA-N"
 WATER_INCHI_KEY = "XLYOFNOQVPJJNP-UHFFFAOYSA-N"
 
 
 from .exceptions import ParseException
 from .models import (
     Compound,
     CompoundIdentifier,
     CompoundMicrospecies,
-    CompoundName,
     Base,
     Registry,
     MagnesiumDissociationConstant,
 )
 from .thermodynamic_constants import (
     ureg,
     Q_,
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/api.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/api.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/compatibility.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/compatibility.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/compound_cache.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/compound_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
 import logging
 from functools import partial
-from typing import Iterable, List, Optional, Tuple
+from typing import Iterable, List, Optional, Set, Tuple
 
 import pandas as pd
 import sqlalchemy
 from Levenshtein import ratio
 from sqlalchemy import exists
 from sqlalchemy.orm import joinedload, sessionmaker
 from sqlalchemy.orm.session import make_transient
 
-from . import PROTON_INCHI_KEY, WATER_INCHI_KEY, CompoundName
+from . import PROTON_INCHI_KEY, WATER_INCHI_KEY
 from .models import Compound, CompoundIdentifier, CompoundMicrospecies, Registry
 
 
 __all__ = ("CompoundCache",)
 
 
 logger = logging.getLogger(__name__)
@@ -68,23 +68,23 @@
         self.engine = engine
         self.session = Session(bind=self.engine)
         self._protons = None
         self._waters = None
         logger.debug("Loading synonyms into data frame.")
         query = (
             self.session.query(
-                CompoundName.compound_id, Registry.namespace, CompoundName.name
+                CompoundIdentifier.compound_id, CompoundIdentifier.accession
             )
-            .select_from(CompoundName)
             .join(Registry)
+            .filter(Registry.namespace == "synonyms")
         )
         self._synonyms = pd.read_sql(
             query.statement, query.session.bind, index_col="compound_id"
         )
-        self._synonyms["name"] = self._synonyms["name"].str.lower()
+        self._synonyms["accession"] = self._synonyms["accession"].str.lower()
 
     @property
     def proton(self) -> Compound:
         """Return the H+ compound object."""
 
         if self._protons is None:
             self._protons = self.search_compound_by_inchi_key(PROTON_INCHI_KEY)
@@ -107,15 +107,15 @@
     def is_water(self, cpd: Compound) -> bool:
         """Return True if this compound is H2O."""
 
         self.water  # this is used to initialize the _water member
         return cpd in self._waters
 
     def all_compound_accessions(self, ascending: bool = True) -> List[str]:
-        """Return a sorted list of all compound accessions."""
+        """Return a list of all compound accessions."""
 
         return sorted(
             (
                 row.accession
                 for row in self.session.query(
                     CompoundIdentifier.accession
                 ).distinct()
@@ -133,20 +133,14 @@
     def get_compound_by_internal_id(self, compound_id: int) -> Compound:
         """Find a compound in the cache based on the internal ID."""
 
         return (
             self.session.query(Compound).filter_by(id=compound_id).one_or_none()
         )
 
-    def get_compound_by_inchi_key(self, key: str) -> Optional[Compound]:
-        """Return a compound by exact match of the InChIKey."""
-        return (
-            self.session.query(Compound).filter_by(inchi_key=key).one_or_none()
-        )
-
     def get_compound_by_inchi(self, inchi: str) -> Optional[Compound]:
         """Return a compound by exact match of the InChI."""
 
         hits = (
             self.session.query(Compound)
             .filter_by(inchi=inchi)
             .options(joinedload("microspecies"))
@@ -174,15 +168,15 @@
         """
         query = self.session.query(Compound)
         if len(inchi_key) < 27:
             return query.filter(Compound.inchi_key.like(f"{inchi_key}%")).all()
         else:
             return query.filter_by(inchi_key=inchi_key).all()
 
-    def get_compound(self, compound_id: str) -> Optional[Compound]:
+    def get_compound(self, compound_id: str) -> Compound:
         """Find a compound object based on the compound ID."""
 
         try:
             namespace, accession = compound_id.split(":", 1)
         except ValueError:
             namespace, accession = None, compound_id
         else:
@@ -193,15 +187,15 @@
             else:
                 namespace = namespace.lower()
 
         return self.get_compound_from_registry(namespace, accession)
 
     def get_compound_from_registry(
         self, namespace: str, accession: str
-    ) -> Optional[Compound]:
+    ) -> Compound:
         """Find a compound object by its accession (and namespace)."""
 
         if (namespace, accession) in self.compound_dict:
             logging.debug(f"Cache hit for {accession} in {namespace} in RAM")
             return self.compound_dict[(namespace, accession)]
 
         query = self.session.query(Compound)
@@ -219,18 +213,18 @@
             query = query.outerjoin(Registry).filter(
                 Registry.namespace == namespace
             )
 
         compound = query.one_or_none()
 
         if compound is None:
-            logging.debug("Not found")
-            return
+            logging.debug("Cache miss")
+            return None
         else:
-            logging.debug("Found")
+            logging.debug("Cache hit")
             self.compound_dict[(namespace, accession)] = compound
             return compound
 
     @staticmethod
     def get_element_data_frame(compounds: Iterable[Compound]) -> pd.DataFrame:
         """Tabulate the elemental composition of the given compounds.
 
@@ -253,14 +247,29 @@
 
         # create the elemental matrix, where each row is a compound and each
         # column is an element (or e-)
         return pd.DataFrame.from_dict(
             atom_bags, orient="columns", dtype=int
         ).fillna(0)
 
+    def get_compound_names(self, compound: Compound) -> Set[str]:
+        """Return all names for this compound."""
+        query = (
+            self.session.query(CompoundIdentifier)
+            .join(Registry)
+            .filter(CompoundIdentifier.compound_id == compound.id)
+            .filter(CompoundIdentifier.registry_id == Registry.id)
+            .filter(Registry.name == "Synonyms")
+        )
+
+        names = set()
+        for identifier in query:
+            names.update(identifier.accession.split("|"))
+        return names
+
     def search(
         self, query: str, page: int = 1, page_size: int = 10
     ) -> List[Tuple[Compound, float]]:
         """Search for compounds with names similar to the query.
 
         Parameters
         ----------
@@ -277,15 +286,15 @@
         -------
         List[Tuple[Compound, float]]
             A list of pairs of compounds and their scores from the
             specified search result page.
         """
         levenshtein_ratio = partial(ratio, query.lower())
         logger.debug("Scoring all synonyms with the query.")
-        scores = self._synonyms["name"].map(levenshtein_ratio)
+        scores = self._synonyms["accession"].map(levenshtein_ratio)
         # Only consider the highest score for each compound.
         result = scores.groupby(scores.index, sort=False).max()
         # Filter out low scores and sort in descending order.
         hits: pd.Series = result[result > 0.5].sort_values(ascending=False)
         if len(hits) == 0:
             raise ValueError(
                 f"There are no significant results for your query '{query}'."
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/exceptions.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/exceptions.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/__init__.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,19 @@
 SYMBOL_TO_CHARGE["e-"] = -1
 
 
 from .mixins import TimeStampMixin
 from .registry import Registry
 from .compound import Compound
 from .compound_identifier import CompoundIdentifier
-from .compound_name import CompoundName
 from .compound_microspecies import CompoundMicrospecies
 from .magnesium_dissociation_constant import MagnesiumDissociationConstant
 
 
 __all__ = (
     "Base",
     "Registry",
     "Compound",
     "CompoundIdentifier",
-    "CompoundName",
     "CompoundMicrospecies",
     "MagnesiumDissociationConstant",
 )
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
+import re
 from functools import reduce
-from typing import Optional
+from typing import Iterable, Optional, Union
 
 import numpy as np
-from sqlalchemy import Column, Integer, PickleType, String
+from sqlalchemy import Column, Float, Integer, PickleType, String
 from sqlalchemy.orm import relationship
 
 from ..exceptions import MissingDissociationConstantsException
 from ..thermodynamic_constants import Q_, R, default_pMg, ureg
 from . import SYMBOL_TO_CHARGE, Base
 from .mixins import TimeStampMixin
 
@@ -79,31 +80,29 @@
     )
     inchi: Optional[str] = Column(
         String(), default=None, nullable=True, index=True
     )
     smiles: Optional[str] = Column(
         String(), default=None, nullable=True, index=True
     )
+    mass: Optional[float] = Column(Float, default=None, nullable=True)
     atom_bag: Optional[dict] = Column(PickleType, nullable=True)
     dissociation_constants: Optional[list] = Column(PickleType, nullable=True)
     group_vector: Optional[list] = Column(PickleType, nullable=True)
     magnesium_dissociation_constants: list = relationship(
         "MagnesiumDissociationConstant",
         cascade="all, delete-orphan",
         lazy="select",
     )
     microspecies: list = relationship(
         "CompoundMicrospecies", cascade="all, delete-orphan", lazy="select"
     )
     identifiers: list = relationship(
         "CompoundIdentifier", cascade="all, delete-orphan", lazy="select"
     )
-    names: list = relationship(
-        "CompoundName", cascade="all, delete-orphan", lazy="select"
-    )
 
     def __repr__(self) -> str:
         """Return a string representation of this object."""
         return (
             f"{type(self).__name__}(id={self.id}, inchi_key={self.inchi_key})"
         )
 
@@ -155,14 +154,37 @@
 
         Returns
         -------
         True if the compound can be transformed
         """
         return len(self.microspecies) != 0 and None not in self.microspecies
 
+    def _get_ms_ddg_over_rt(
+        self,
+        p_h: Q_,
+        ionic_strength: Q_,
+        temperature: Q_,
+        p_mg: Q_ = default_pMg,
+    ) -> Iterable:
+        if not self.can_be_transformed():
+            raise MissingDissociationConstantsException(
+                f"{self} has not yet been analyzed by ChemAxon."
+            )
+
+        pH = p_h.m_as("")
+        pMg = p_mg.m_as("")
+        ionic_strength_M = ionic_strength.m_as("M")
+        T_in_K = temperature.m_as("K")
+        return map(
+            lambda ms: -ms.transform(
+                pH=pH, pMg=pMg, ionic_strength_M=ionic_strength_M, T_in_K=T_in_K
+            ),
+            self.microspecies,
+        )
+
     @ureg.check(None, "", "[concentration]", "[temperature]", "")
     def transform(
         self,
         p_h: Q_,
         ionic_strength: Q_,
         temperature: Q_,
         p_mg: Q_ = default_pMg,
@@ -184,52 +206,125 @@
 
         Returns
         -------
         Quantity
             The transformed relative :math:`\Delta G` of this compound.
 
         """
-        if not self.can_be_transformed():
-            raise MissingDissociationConstantsException(
-                f"{self} has not yet been analyzed by ChemAxon."
-            )
-
-        pH = p_h.m_as("")
-        pMg = p_mg.m_as("")
-        ionic_strength_M = ionic_strength.m_as("M")
-        T_in_K = temperature.m_as("K")
-        ms_ddg_over_rt_list = map(
-            lambda ms: -ms.transform(
-                pH=pH, pMg=pMg, ionic_strength_M=ionic_strength_M, T_in_K=T_in_K
-            ),
-            self.microspecies,
-        )
 
         # Since the ddg_over_rt values of different microspecies can span
         # a large range, summing their exponents directly will cause floating
         # point overflow issue. Therefore, we use logsumexp instead.
-        return -R * temperature * reduce(np.logaddexp, ms_ddg_over_rt_list)
+        return (
+            -R
+            * temperature
+            * reduce(
+                np.logaddexp,
+                self._get_ms_ddg_over_rt(
+                    p_h=p_h,
+                    p_mg=p_mg,
+                    ionic_strength=ionic_strength,
+                    temperature=temperature,
+                ),
+            )
+        )
 
-    def get_common_name(self) -> Optional[str]:
+    @ureg.check(None, "", "[concentration]", "[temperature]", "")
+    def sensitivity_to_p_h(
+        self,
+        p_h: Q_,
+        ionic_strength: Q_,
+        temperature: Q_,
+        p_mg: Q_ = default_pMg,
+    ) -> Q_:
+        r"""Calculate the derivative of the formation ΔG' w.r.t. pH.
+
+        By derivating the Legendre transform as a function of pH, we get
+        the slope which is a linear approximation of the pH response.
+
+        Parameters
+        ----------
+        p_h : Quantity
+            The pH value, i.e., the logarithmic scale for the molar
+            concentration of hydrogen ions :math:`-log10([H+])`
+        ionic_strength : Quantity
+            Set the ionic strength
+        temperature : Quantity
+            Set the temperature
+        p_mg : Quantity, optional
+            The logarithmic molar concentration of magnesium ions
+            :math:`-log10([Mg2+])`, (Default value = default_pMg)
+
+        Returns
+        -------
+        Quantity
+            The derivative of  :math:`\Delta G_f` with respect to pH.
+
+        """
+        ms_ddg_over_rt_list = list(
+            self._get_ms_ddg_over_rt(
+                p_h=p_h,
+                p_mg=p_mg,
+                ionic_strength=ionic_strength,
+                temperature=temperature,
+            )
+        )
+        numerator = sum(
+            [
+                ms.number_protons * np.exp(ddg)
+                for ms, ddg in zip(self.microspecies, ms_ddg_over_rt_list)
+            ]
+        )
+        denominator = sum([np.exp(ddg) for ddg in ms_ddg_over_rt_list])
+        return R * temperature * np.log(10) * numerator / denominator
+
+    def get_common_name(self) -> Union[str, None]:
         """Return the most common name for this compound.
 
         Right now, we simply choose the first identifier with the smallest
         ID in the list, which is not ideal.
         """
-        for name in self.names:
-            if name.is_preferred:
-                return name.name
+        best_priority = np.inf
+        synonym = None
+        for identifier in self.identifiers:
+            if identifier.registry.name == "Synonyms":
+                priority = identifier.id  # TODO: find a better way to choose
+                if priority < best_priority:
+                    synonym = identifier.accession.split("|")[0]
+                    best_priority = priority
+        return synonym
 
     ORDER_OF_REGISTRIES = (
         "MIR:00000567",  # MetaNetX chemical
         "MIR:00000578",  # KEGG
         "MIR:00000556",  # BiGG
         "MIR:00000002",  # ChEBI
         "MIR:00000552",  # SEED
     )
 
-    def get_accession(self) -> Optional[str]:
+    @staticmethod
+    def _identifier_sorting_key(identifier) -> tuple:
+        try:
+            priority = Compound.ORDER_OF_REGISTRIES.index(
+                identifier.registry.identifier
+            )
+        except ValueError:
+            return np.inf, np.inf
+
+        # try to find a the numeric value in the accession
+        numbers = re.findall(r"(\d+)", identifier.accession)
+        try:
+            return priority, int(numbers[0])
+        except IndexError:
+            # since we lack any other options, just use the length of the
+            # accession string
+            return priority, len(identifier.accession)
+
+    def get_accession(self) -> Union[str, None]:
         """Get an accession code for this compound."""
-        for namespace in ("metanetx.chemical", "kegg.compound"):
-            for cmpnd_id in self.identifiers:
-                if cmpnd_id.registry.namespace == namespace:
-                    return f"{namespace}:{cmpnd_id.accession}"
+        try:
+            best_id = min(
+                self.identifiers, key=Compound._identifier_sorting_key
+            )
+            return best_id.registry.namespace + ":" + best_id.accession
+        except ValueError:
+            return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_identifier.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_identifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,22 +22,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
 import logging
 
-from sqlalchemy import (
-    Boolean,
-    Column,
-    ForeignKey,
-    Integer,
-    String,
-    UniqueConstraint,
-)
+from sqlalchemy import Column, ForeignKey, Integer, String
 from sqlalchemy.orm import relationship
 
 from . import Base
 from .compound import Compound
 from .mixins import TimeStampMixin
 from .registry import Registry
 
@@ -67,30 +60,20 @@
 
     # SQLAlchemy column descriptors.
     id: int = Column(Integer, primary_key=True, autoincrement=True)
     compound_id: int = Column(Integer, ForeignKey(Compound.id), nullable=False)
     registry_id: int = Column(Integer, ForeignKey(Registry.id), nullable=False)
     registry: Registry = relationship(Registry, lazy="selectin")
     accession: str = Column(String, nullable=False, index=True)
-    is_deprecated: bool = Column(Boolean, default=False, nullable=False)
-
-    __table_args__ = (
-        UniqueConstraint("compound_id", "registry_id", "accession"),
-    )
-
-    def __init__(self, *, is_deprecated: bool = False, **kwargs) -> None:
-        """Create an instance with a default value."""
-        super().__init__(**kwargs)
-        self.is_deprecated = is_deprecated
 
     def __repr__(self) -> str:
         """Return a string representation of this object."""
         return (
             f"{type(self).__name__}(registry={repr(self.registry)},"
-            f" accession={self.accession}, is_deprecated={self.is_deprecated})"
+            f" accession={self.accession})"
         )
 
     def is_valid(self) -> bool:
         """Use the registry to validate the accession."""
         if self.registry is None:
             logger.error("No associated registry.")
             return False
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/compound_microspecies.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/models/compound_microspecies.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/magnesium_dissociation_constant.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/models/magnesium_dissociation_constant.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/models/mixins.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/models/mixins.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/reaction.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/reaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,17 +338,19 @@
         """
         atom_bags = {
             compound: compound.atom_bag or {} for compound in self.keys()
         }
 
         # create the elemental matrix, where each row is a compound and each
         # column is an element (or e-)
-        return pd.DataFrame.from_dict(
-            atom_bags, orient="columns", dtype=int
-        ).fillna(0)
+        return (
+            pd.DataFrame.from_dict(atom_bags, orient="columns")
+            .fillna(0)
+            .astype(int)
+        )
 
     def _get_reaction_atom_bag(
         self, minimal_stoichiometry: Optional[float] = None
     ) -> Dict[str, int]:
         """Use for checking if all elements are conserved.
 
         Parameters
@@ -615,14 +617,61 @@
             except MissingDissociationConstantsException as e:
                 warnings.warn(
                     f"Cannot calculate Legendre transform for {compound}: "
                     + str(e)
                 )
         return ddg
 
+    @ureg.check(None, "", "[concentration]", "[temperature]", "")
+    def sensitivity_to_p_h(
+        self,
+        p_h: Q_,
+        ionic_strength: Q_,
+        temperature: Q_,
+        p_mg: Q_ = default_pMg,
+    ) -> Q_:
+        r"""Calculate the derivative of the reaction ΔG' w.r.t. pH.
+
+        By derivating the Legendre transform as a function of pH, we get
+        the slope which is a linear approximation of the pH response.
+
+        Parameters
+        ----------
+        p_h : Quantity
+            Set the -log10 of the proton concentration [H+].
+        ionic_strength : Quantity
+            Set the ionic strength.
+        temperature : Quantity
+            Set the temperature.
+        p_mg : Quantity
+            Set the -log10 of the magnesium ion concentration [Mg++].
+            (Default value = default_pMg)
+
+        Returns
+        -------
+        Quantity
+            The derivative of  :math:`\Delta G_r` with respect to pH.
+
+        """
+        sensitivity = Q_(0.0, "kJ/mol")
+        for compound, coeff in self.items(protons=False):  # ignore protons
+            try:
+                sensitivity += coeff * compound.sensitivity_to_p_h(
+                    p_h=p_h,
+                    ionic_strength=ionic_strength,
+                    temperature=temperature,
+                    p_mg=p_mg,
+                )
+            except MissingDissociationConstantsException as e:
+                warnings.warn(
+                    f"Cannot calculate Legendre transform for {compound}: "
+                    + str(e)
+                )
+        return sensitivity
+
     def _sum_coefficients(self) -> float:
         r"""Calculate the sum of all coefficients (excluding water).
 
         This is useful for shifting the :math:`\Delta G0`to another set
         of standard concentrations (e.g. 1 mM).
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/thermodynamic_constants.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/thermodynamic_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         temperature in kJ/mol
 
     """
     _a1 = 9.20483e-3  # kJ / mol / M^0.5 / K
     _a2 = 1.284668e-5  # kJ / mol / M^0.5 / K^2
     _a3 = 4.95199e-8  # kJ / mol / M^0.5 / K^3
     B = 1.6  # 1 / M^0.5
-    alpha = _a1 * T_in_K - _a2 * T_in_K ** 2 + _a3 * T_in_K ** 3  # kJ / mol
+    alpha = _a1 * T_in_K - _a2 * T_in_K**2 + _a3 * T_in_K**3  # kJ / mol
     return alpha / (1.0 / sqrt_ionic_strength + B)  # kJ / mol
 
 
 def _legendre_transform(
     pH: float,
     pMg: float,
     ionic_strength_M: float,
@@ -104,13 +104,13 @@
     proton_term = num_protons * RT * LOG10 * pH
     _dg_mg = (T_in_K / default_T_in_K) * standard_dg_formation_mg + (
         1.0 - T_in_K / default_T_in_K
     ) * standard_dh_formation_mg
     magnesium_term = num_magnesiums * (RT * LOG10 * pMg - _dg_mg)
 
     if ionic_strength_M > 0:
-        dh_factor = debye_hueckel(ionic_strength_M ** 0.5, T_in_K)
-        is_term = dh_factor * (charge ** 2 - num_protons - 4 * num_magnesiums)
+        dh_factor = debye_hueckel(ionic_strength_M**0.5, T_in_K)
+        is_term = dh_factor * (charge**2 - num_protons - 4 * num_magnesiums)
     else:
         is_term = 0.0
 
     return (proton_term + magnesium_term - is_term) / RT
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache/zenodo.py` & `equilibrator-cache-0.4.5/src/equilibrator_cache/zenodo.py`

 * *Files identical despite different names*

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/PKG-INFO` & `equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: equilibrator-cache
-Version: 0.4.4b2
+Version: 0.4.5
 Summary: Cache application for compounds, reactions, and enzymes
 Home-page: https://gitlab.com/equilibrator/equilibrator-cache
+Download-URL: https://pypi.org/project/equilibrator-cache/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
-Download-URL: https://pypi.org/project/equilibrator-cache/
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-cache
 Project-URL: Bug Tracker, https://gitlab.com/equilibrator/equilibrator-cache/-/issues
 Keywords: component contribution,Gibbs energy,biochemical reaction,eQuilibrator,cache
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: development
 Provides-Extra: deployment
 License-File: LICENSE
 
 equilibrator-cache
@@ -47,9 +45,7 @@
 
 ## Supported Chemical Databases:
 
 * [MetaNetX](https://www.metanetx.org/)
 * [KEGG](https://www.kegg.jp/)
 * [ChEBI](https://www.ebi.ac.uk/chebi/)
 
-
-
```

### Comparing `equilibrator-cache-0.4.4b2/src/equilibrator_cache.egg-info/SOURCES.txt` & `equilibrator-cache-0.4.5/src/equilibrator_cache.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+versioneer.py
 src/equilibrator_cache/__init__.py
 src/equilibrator_cache/_version.py
 src/equilibrator_cache/api.py
 src/equilibrator_cache/compatibility.py
 src/equilibrator_cache/compound_cache.py
 src/equilibrator_cache/exceptions.py
 src/equilibrator_cache/reaction.py
@@ -19,11 +20,10 @@
 src/equilibrator_cache.egg-info/requires.txt
 src/equilibrator_cache.egg-info/top_level.txt
 src/equilibrator_cache.egg-info/zip-safe
 src/equilibrator_cache/models/__init__.py
 src/equilibrator_cache/models/compound.py
 src/equilibrator_cache/models/compound_identifier.py
 src/equilibrator_cache/models/compound_microspecies.py
-src/equilibrator_cache/models/compound_name.py
 src/equilibrator_cache/models/magnesium_dissociation_constant.py
 src/equilibrator_cache/models/mixins.py
 src/equilibrator_cache/models/registry.py
```

