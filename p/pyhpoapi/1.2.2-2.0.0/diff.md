# Comparing `tmp/pyhpoapi-1.2.2.tar.gz` & `tmp/pyhpoapi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhpoapi-1.2.2.tar", last modified: Sun May 30 12:30:51 2021, max compression
+gzip compressed data, was "pyhpoapi-2.0.0.tar", last modified: Fri Jul 28 19:56:40 2023, max compression
```

## Comparing `pyhpoapi-1.2.2.tar` & `pyhpoapi-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 12:30:51.214683 pyhpoapi-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4684 2021-05-30 12:30:51.214683 pyhpoapi-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 12:30:51.214683 pyhpoapi-1.2.2/pyhpoapi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     6769 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 12:30:51.214683 pyhpoapi-1.2.2/pyhpoapi/resources/
--rw-r--r--   0 runner    (1001) docker     (121)    30724 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/resources/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 12:30:51.214683 pyhpoapi-1.2.2/pyhpoapi/routers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7570 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/routers/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5515 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/routers/term.py
--rw-r--r--   0 runner    (1001) docker     (121)    16885 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/routers/terms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/pyhpoapi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-30 12:30:51.214683 pyhpoapi-1.2.2/pyhpoapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4684 2021-05-30 12:30:51.000000 pyhpoapi-1.2.2/pyhpoapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      467 2021-05-30 12:30:51.000000 pyhpoapi-1.2.2/pyhpoapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-30 12:30:51.000000 pyhpoapi-1.2.2/pyhpoapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-05-30 12:30:51.000000 pyhpoapi-1.2.2/pyhpoapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-05-30 12:30:51.000000 pyhpoapi-1.2.2/pyhpoapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-30 12:30:51.214683 pyhpoapi-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2021-05-30 12:30:38.000000 pyhpoapi-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:40.620373 pyhpoapi-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-28 19:56:40.620373 pyhpoapi-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:40.616372 pyhpoapi-2.0.0/pyhpoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:40.620373 pyhpoapi-2.0.0/pyhpoapi/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    30724 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/resources/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:40.620373 pyhpoapi-2.0.0/pyhpoapi/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/routers/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/routers/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/routers/terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyhpoapi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:56:40.620373 pyhpoapi-2.0.0/pyhpoapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-28 19:56:40.000000 pyhpoapi-2.0.0/pyhpoapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-28 19:56:40.000000 pyhpoapi-2.0.0/pyhpoapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:56:40.000000 pyhpoapi-2.0.0/pyhpoapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:56:40.000000 pyhpoapi-2.0.0/pyhpoapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 19:56:40.000000 pyhpoapi-2.0.0/pyhpoapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:56:40.620373 pyhpoapi-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 19:56:07.000000 pyhpoapi-2.0.0/setup.py
```

### Comparing `pyhpoapi-1.2.2/LICENSE` & `pyhpoapi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhpoapi-1.2.2/pyhpoapi/config.py` & `pyhpoapi-2.0.0/pyhpoapi/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 """
 Module to read in a local ``config.ini`` file and store
 as a global configuration.
 """
 
 import os
-import configparser
 from typing import Any, List
 
 
 def config_item_list(value: str, convert=str) -> List[Any]:
     """
     Convert a comma separated string into a list
     """
     return [convert(x) for x in value.split(',')]
 
 
-local_config = os.path.join(
-    os.getcwd(),
-    'config.ini'
-    )
+VERSION = "2.0.0"
 
-
-config = configparser.ConfigParser()
-if os.path.exists(local_config):
-    config.read(local_config)
-
-
-VERSION = config.get('default', 'version', fallback='1.2.2')
+MASTER_DATA = os.environ.get("PYHPOAPI_DATA_DIR", "")
 
 CORS_ORIGINS = config_item_list(
-    config.get('default', 'cors-origins', fallback='')
+    os.environ.get("PYHPOAPI_CORS_ORIGINS", "")
 )
+
 CORS_METHODS = config_item_list(
-    config.get('default', 'cors-methods', fallback='')
+    os.environ.get("PYHPOAPI_CORS_METHODS", "")
 )
+
 CORS_HEADERS = config_item_list(
-    config.get('default', 'cors-headers', fallback='')
+    os.environ.get("PYHPOAPI_CORS_HEADERS", "")
 )
 
 OPENAPI_TAGS = [
     {
         'name': 'term',
         'description': 'Operate on a single HPOTerm',
     },
```

### Comparing `pyhpoapi-1.2.2/pyhpoapi/models.py` & `pyhpoapi-2.0.0/pyhpoapi/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from enum import Enum
 from typing import List, Optional
 from pydantic import BaseModel
 
 
-class Information_Content(BaseModel):
+class InformationContent(BaseModel):
     gene: float
     omim: float
     orpha: float
     decipher: float
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'omim': 5.528020005103167,
             'gene': 4.915866634310163,
             'orpha': 6.491229223514548,
             'decipher': 0
         }
 
 
-class HPO(BaseModel):
+class HpoTerm(BaseModel):
     int: int
     id: str
     name: str
-    definition: Optional[str]
-    comment: Optional[str]
-    xref: Optional[List[str]]
-    is_a: Optional[List[str]]
-    ic: Optional[Information_Content]
+    definition: Optional[str] = None
+    comment: Optional[str] = None
+    synonym: Optional[List[str]] = None
+    xref: Optional[List[str]] = None
+    is_a: Optional[List[str]] = None
+    ic: Optional[InformationContent] = None
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
                 'int': 7401,
                 'id': 'HP:0007401',
                 'name': 'Macular atrophy',
                 'definition': (
                     '"Well-demarcated area(s) of partial or complete '
                     'depigmentation in the macula, reflecting atrophy '
@@ -57,135 +57,135 @@
                     'orpha': 6.491229223514548,
                     'decipher': 0
                 }
             }
         }
 
 
-class HPOSimple(BaseModel):
+class HpoTermMinimal(BaseModel):
     int: int
     id: str
     name: str
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
                 'int': 7401,
                 'id': 'HP:0007401',
                 'name': 'Macular atrophy',
                 }
             }
 
 
-class HPONeighbours(BaseModel):
-    parents: List[HPO]
-    children: List[HPO]
-    neighbours: List[HPO]
+class HpoNeighborTerms(BaseModel):
+    parents: List[HpoTerm]
+    children: List[HpoTerm]
+    neighbours: List[HpoTerm]
 
 
 class Omim(BaseModel):
     id: int
     name: str
-    hpo: Optional[List[HPO]]
+    hpo: Optional[List[HpoTerm]] = None
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
                 'id': 230800,
                 'name': 'GAUCHER DISEASE, TYPE I'
             }
         }
 
 
 class Gene(BaseModel):
     id: int
     name: str
     symbol: str
-    hpo: Optional[List[HPO]]
+    hpo: Optional[List[HpoTerm]] = None
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
                 'id': 2629,
                 'name': 'GBA',
                 'symbol': 'GBA'
             }
         }
 
 
-class Similarity_Score(BaseModel):
-    set1: List[HPOSimple]
-    set2: List[HPOSimple]
+class SimilarityScore(BaseModel):
+    set1: List[HpoTermMinimal]
+    set2: List[HpoTermMinimal]
     similarity: float
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
-                'set1': [HPOSimple.Config.schema_extra['example']],
-                'set2': [HPOSimple.Config.schema_extra['example']],
+                'set1': [HpoTermMinimal.Config.json_schema_extra['example']],
+                'set2': [HpoTermMinimal.Config.json_schema_extra['example']],
                 'similarity': 0.3422332
             }
         }
 
 
-class Similarity_Score_OMIM(BaseModel):
-    set1: List[HPOSimple]
-    set2: List[HPOSimple]
+class SimilarityScore_Omim(BaseModel):
+    set1: List[HpoTermMinimal]
+    set2: List[HpoTermMinimal]
     omim: Omim
     similarity: float
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
-                'set1': [HPOSimple.Config.schema_extra['example']],
-                'set2': [HPOSimple.Config.schema_extra['example']],
-                'omim': Omim.Config.schema_extra['example'],
+                'set1': [HpoTermMinimal.Config.json_schema_extra['example']],
+                'set2': [HpoTermMinimal.Config.json_schema_extra['example']],
+                'omim': Omim.Config.json_schema_extra['example'],
                 'similarity': 0.3422332
             }
         }
 
 
-class Similarity_Score_Gene(BaseModel):
-    set1: List[HPOSimple]
-    set2: List[HPOSimple]
+class SimilarityScore_Gene(BaseModel):
+    set1: List[HpoTermMinimal]
+    set2: List[HpoTermMinimal]
     gene: Gene
     similarity: float
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
-                'set1': [HPOSimple.Config.schema_extra['example']],
-                'set2': [HPOSimple.Config.schema_extra['example']],
-                'gene': Gene.Config.schema_extra['example'],
+                'set1': [HpoTermMinimal.Config.json_schema_extra['example']],
+                'set2': [HpoTermMinimal.Config.json_schema_extra['example']],
+                'gene': Gene.Config.json_schema_extra['example'],
                 'similarity': 0.3422332
             }
         }
 
 
-class Batch_Similarity_Set(BaseModel):
+class SimilarityScore_SingleSet(BaseModel):
     name: str
-    similarity: Optional[float]
-    error: Optional[str]
+    similarity: Optional[float] = None
+    error: Optional[str] = None
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
                 'name': 'Comparison-Set 123',
                 'similarity': 0.3763421567579537,
                 'error': None
             }
         }
 
 
-class Batch_Similarity_Score(BaseModel):
-    set1: List[HPOSimple]
-    other_sets: List[Batch_Similarity_Set]
+class SimilarityScore_Batch(BaseModel):
+    set1: List[HpoTermMinimal]
+    other_sets: List[SimilarityScore_SingleSet]
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             'example': {
                 'set1': [{
                     'int': 7401,
                     'id': 'HP:0007401',
                     'name': 'Macular atrophy'
                 }, {
                     'int': 6530,
@@ -193,79 +193,61 @@
                     'name': 'Interstitial pulmonary abnormality'
                 }, {
                     'int': 10885,
                     'id': 'HP:0010885',
                     'name': 'Avascular necrosis'
                 }],
                 'other_sets': [
-                    Batch_Similarity_Set.Config.schema_extra['example'],
-                    Batch_Similarity_Set.Config.schema_extra['example']
+                    SimilarityScore_SingleSet.Config.json_schema_extra['example'],
+                    SimilarityScore_SingleSet.Config.json_schema_extra['example']
                 ]
             }
         }
 
 
-class POST_OMIM_Batch(BaseModel):
+class PostBody_Similarity_Omim(BaseModel):
     set1: str
     omim_diseases: List[int]
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             "example": {
                 "set1": "HP:0007401,HP:0010885,HP:0006530",
                 "omim_diseases": [230800, 230900, 231000, 231005, 608013]
             }
         }
 
 
-class POST_Gene_Batch(BaseModel):
+class PostBody_Similarity_Gene(BaseModel):
     set1: str
     genes: List[str]
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             "example": {
                 "set1": "HP:0007401,HP:0010885,HP:0006530",
                 "genes": ['GBA', 'EZH2']
             }
         }
 
 
-class Similarity_Method(Enum):
-    resnik = 'resnik'
-    lin = 'lin'
-    jc = 'jc'
-    jc2 = 'jc2'
-    rel = 'rel'
-    ic = 'ic'
-    graphic = 'graphic'
-    dist = 'dist'
-    equal = 'equal'
-
-
-class Combination_Method(Enum):
-    funSimAvg = 'funSimAvg'
-    funSimMax = 'funSimMax'
-    BMA = 'BMA'
-
-
-class POST_HPOSet(BaseModel):
+class NamedHpoSet(BaseModel):
     """
     Defines the POST body for an HPO Set
     """
     set2: str
     name: str
 
 
-class POST_Batch(BaseModel):
+class PostBody_HpoSets(BaseModel):
     set1: str
-    other_sets: List[POST_HPOSet]
+    other_sets: List[NamedHpoSet]
 
     class Config:
-        schema_extra = {
+        json_schema_extra = {
             "example": {
                 "set1": "HP:0007401,HP:0010885,HP:0006530",
                 "other_sets": [
                     {
                         "set2": "HP:0200070,HP:0002754,HP:0031630",
                         "name": "Comparison-Set 123"
                     }, {
```

### Comparing `pyhpoapi-1.2.2/pyhpoapi/resources/logo.png` & `pyhpoapi-2.0.0/pyhpoapi/resources/logo.png`

 * *Files identical despite different names*

### Comparing `pyhpoapi-1.2.2/pyhpoapi/routers/annotations.py` & `pyhpoapi-2.0.0/pyhpoapi/routers/annotations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from fastapi import APIRouter, HTTPException, Path, Query
 
-from pyhpo.ontology import Ontology
+from pyhpo import Ontology
 from pyhpo.annotations import Gene, Omim
-from pyhpo.set import HPOSet
+from pyhpo import HPOSet
 
 from pyhpoapi.helpers import get_hpo_set
 from pyhpoapi import models
 from pyhpoapi.routers import terms
 
 router = APIRouter()
 
@@ -94,16 +94,16 @@
         pass
     return res
 
 
 @router.get(
     '/similarity/omim',
     tags=['similarity', 'terms', 'disease'],
-    response_description='Similarity score',
-    response_model=models.Similarity_Score_OMIM
+    response_description='Similarity score for OMIM Diseases',
+    response_model=models.SimilarityScore_Omim
     )
 async def omim_similarity(
     set1: str = Query(..., example='HP:0007401,HP:0010885,HP:0006530'),
     omim: int = Query(..., example=230800),
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
@@ -117,87 +117,104 @@
     except KeyError:
         raise HTTPException(
             status_code=404,
             detail="OMIM disease does not exist"
         )
     set2 = HPOSet.from_queries([int(x) for x in disease.hpo])
 
-    return {
-        'set1': hposet.toJSON(),
-        'set2': set2.toJSON(),
-        'omim': disease.toJSON(),
-        'similarity': hposet.similarity(
-            set2,
-            kind=kind,
-            method=method,
-            combine=combine
-        )
-    }
+    try:
+        return {
+            'set1': hposet.toJSON(),
+            'set2': set2.toJSON(),
+            'omim': disease.toJSON(),
+            'similarity': hposet.similarity(
+                set2,
+                kind=kind,
+                method=method,
+                combine=combine
+            )
+        }
+    except NotImplementedError:
+        raise HTTPException(
+            status_code=400,
+            detail="The similarity method is not properly implemented"
+            )
+    except RuntimeError:
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid `method` or `combine` parameter"
+            )
+    except AttributeError:
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid information content kind specified"
+            )
+
 
 
 @router.post(
     '/similarity/omim',
     tags=['similarity', 'terms', 'disease'],
     response_description='Similarity score',
-    response_model=models.Batch_Similarity_Score
+    response_model=models.SimilarityScore_Batch
     )
 async def batch_omim_similarity(
-    data: models.POST_OMIM_Batch,
+    data: models.PostBody_Similarity_Omim,
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
 ) -> dict:
     """
     Similarity score between one HPOSet and several OMIM Diseases
     """
     other_sets = []
 
     for other in data.omim_diseases:
         try:
             disease = Omim.get(other)
             hpos = ','.join([str(x) for x in disease.hpo])
         except KeyError:
-            hpos = ''
+            hpos = f"unknown Omim disease {other}"
 
         other_sets.append(
-            models.POST_HPOSet(
+            models.NamedHpoSet(
                 set2=hpos,
-                name=other
+                name=str(other)
             )
         )
 
     res = await terms.batch_similarity(
-        data=models.POST_Batch(
+        data=models.PostBody_HpoSets(
             set1=data.set1,
             other_sets=other_sets
             ),
         method=method,
         combine=combine,
         kind=kind
     )
     return res
 
 
 @router.get(
     '/similarity/omim/all',
     tags=['similarity', 'terms', 'disease'],
     response_description='Similarity score',
-    response_model=models.Batch_Similarity_Score
+    response_model=models.SimilarityScore_Batch
     )
 async def all_omim_similarity(
     set1: str = Query(..., example='HP:0007401,HP:0010885,HP:0006530'),
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
 ) -> dict:
     """
     Calculate Similarity scores between query set and all OMIM diseases
     """
 
-    data = models.POST_OMIM_Batch(
+    data = models.PostBody_Similarity_Omim(
         set1=set1,
         omim_diseases=[x.id for x in Ontology.omim_diseases]
     )
     res = await batch_omim_similarity(
         data=data,
         method=method,
         combine=combine,
@@ -205,16 +222,16 @@
     )
     return res
 
 
 @router.get(
     '/similarity/gene',
     tags=['similarity', 'terms', 'disease'],
-    response_description='Similarity score',
-    response_model=models.Similarity_Score_Gene
+    response_description='Similarity score for genes',
+    response_model=models.SimilarityScore_Gene
     )
 async def gene_similarity(
     set1: str = Query(..., example='HP:0007401,HP:0010885,HP:0006530'),
     gene: str = Query(..., example='GBA'),
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
@@ -225,89 +242,105 @@
     hposet = get_hpo_set(set1)
     try:
         actual_gene = Gene.get(gene)
     except KeyError:
         raise HTTPException(status_code=404, detail="Gene does not exist")
     set2 = HPOSet.from_queries([int(x) for x in actual_gene.hpo])
 
-    return {
-        'set1': hposet.toJSON(),
-        'set2': set2.toJSON(),
-        'gene': actual_gene.toJSON(),
-        'similarity': hposet.similarity(
-            set2,
-            kind=kind,
-            method=method,
-            combine=combine
-        )
-    }
+    try:
+        return {
+            'set1': hposet.toJSON(),
+            'set2': set2.toJSON(),
+            'gene': actual_gene.toJSON(),
+            'similarity': hposet.similarity(
+                set2,
+                kind=kind,
+                method=method,
+                combine=combine
+            )
+        }
+    except NotImplementedError:
+        raise HTTPException(
+            status_code=400,
+            detail="The similarity method is not properly implemented"
+            )
+    except RuntimeError:
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid `method` or `combine` parameter"
+            )
+    except AttributeError:
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid information content kind specified"
+            )
 
 
 @router.post(
     '/similarity/gene',
     tags=['similarity', 'terms', 'gene'],
     response_description='Similarity score',
-    response_model=models.Batch_Similarity_Score
+    response_model=models.SimilarityScore_Batch
     )
 async def batch_gene_similarity(
-    data: models.POST_Gene_Batch,
+    data: models.PostBody_Similarity_Gene,
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
 ) -> dict:
     """
     Similarity score between one HPOSet and several OMIM Diseases
     """
     other_sets = []
 
     for other in data.genes:
         try:
             actual_gene = Gene.get(other)
             hpos = ','.join([str(x) for x in actual_gene.hpo])
         except KeyError:
-            hpos = ''
+            hpos = f"unknown gene {other}"
 
         other_sets.append(
-            models.POST_HPOSet(
+            models.NamedHpoSet(
                 set2=hpos,
-                name=actual_gene.name
+                name=other
             )
         )
 
     res = await terms.batch_similarity(
-        data=models.POST_Batch(
+        data=models.PostBody_HpoSets(
             set1=data.set1,
             other_sets=other_sets
             ),
         method=method,
         combine=combine,
         kind=kind
     )
     return res
 
 
 @router.get(
     '/similarity/gene/all',
     tags=['similarity', 'terms', 'gene'],
     response_description='Similarity score',
-    response_model=models.Batch_Similarity_Score
+    response_model=models.SimilarityScore_Batch
     )
 async def all_gene_similarity(
     set1: str = Query(..., example='HP:0007401,HP:0010885,HP:0006530'),
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
 ) -> dict:
     """
     Calculate Similarity scores between query set and all genes
     """
 
-    data = models.POST_Gene_Batch(
+    data = models.PostBody_Similarity_Gene(
         set1=set1,
-        genes=[x.id for x in Ontology.genes]
+        genes=[x.name for x in Ontology.genes]
     )
     res = await batch_gene_similarity(
         data=data,
         method=method,
         combine=combine,
         kind=kind
     )
```

### Comparing `pyhpoapi-1.2.2/pyhpoapi/routers/term.py` & `pyhpoapi-2.0.0/pyhpoapi/routers/term.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from fastapi import APIRouter, Path
 from typing import List, Dict
 
-from pyhpo.set import HPOSet
+from pyhpo import HPOSet
 from pyhpoapi.helpers import get_hpo_term
 from pyhpoapi import models
 
 router = APIRouter()
 
 
 @router.get(
     '/{term_id}',
-    response_description='HPOTerm object',
-    response_model=models.HPO
+    response_description='One HPO term',
+    response_model=models.HpoTerm
 )
 async def HPO_term(
         term_id: str = Path(..., example='HP:0000822'),
         verbose: bool = False
 ) -> dict:
     """
     Show info about a single HPO term.
@@ -35,21 +35,23 @@
 
     Returns
     -------
     dict
         HPOTerm as JSON object
 
     """
-    return get_hpo_term(term_id).toJSON(bool(verbose))
+    term = get_hpo_term(term_id).toJSON(bool(verbose))
+    res = models.HpoTerm(**term)
+    return res.model_dump()
 
 
 @router.get(
     '/{term_id}/parents',
-    response_description='HPOTerm object',
-    response_model=List[models.HPO]
+    response_description='List of HPO terms',
+    response_model=List[models.HpoTerm]
 )
 async def parent_terms(
     term_id: str = Path(..., example='HP:0000822'),
     verbose: bool = False
 ) -> List[dict]:
     """
     Get all parents of an HPOterm
@@ -77,16 +79,16 @@
         t.toJSON(verbose)
         for t in get_hpo_term(term_id).parents
         ]
 
 
 @router.get(
     '/{term_id}/children',
-    response_description='HPOTerm object',
-    response_model=List[models.HPO]
+    response_description='List of HPO terms',
+    response_model=List[models.HpoTerm]
 
 )
 async def child_terms(
     term_id: str = Path(..., example='HP:0000822'),
     verbose: bool = False
 ) -> List[dict]:
     """
@@ -115,16 +117,16 @@
         t.toJSON(verbose)
         for t in get_hpo_term(term_id).children
         ]
 
 
 @router.get(
     '/{term_id}/neighbours',
-    response_description='HPOTerm object',
-    response_model=models.HPONeighbours
+    response_description='The neighouring HPO terms',
+    response_model=models.HpoNeighborTerms
 )
 async def neighbour_terms(
     term_id: str = Path(..., example='HP:0000822'),
     verbose: bool = False
 ) -> Dict[str, List[dict]]:
     """
     Get all surrounding terms of an HPOterm
@@ -149,16 +151,16 @@
 
         * **parents**: Array of parent HPOTerms
         * **children**: Array of child HPOTerms
         * **neighbours**: Array of 'sibling' HPOTerms
 
     """
     term = get_hpo_term(term_id)
-    parents = HPOSet(term.parents)
-    children = HPOSet(term.children)
+    parents = HPOSet(list(term.parents))
+    children = HPOSet(list(term.children))
     neighbours = HPOSet([])
     for parent in parents:
         for t in parent.children:
             if t != term and t not in parents and t not in children:
                 neighbours.add(t)
 
     for child in children:
```

### Comparing `pyhpoapi-1.2.2/pyhpoapi/routers/terms.py` & `pyhpoapi-2.0.0/pyhpoapi/routers/terms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from fastapi import APIRouter, Query, HTTPException
 from typing import List, Optional
 
-from pyhpo.ontology import Ontology
-from pyhpo.stats import EnrichmentModel, HPOEnrichment
+from pyhpo import Ontology
+from pyhpo.stats import EnrichmentModel
+try:
+    from pyhpo.stats import HPOEnrichment
+except ImportError:
+    from pyhpoapi.helpers import MockHPOEnrichment as HPOEnrichment
+
 from pyhpo import HPOTerm
 
 from pyhpoapi.helpers import get_hpo_set
 from pyhpoapi import models
 
 router = APIRouter()
 
@@ -16,15 +21,15 @@
 hpo_model_omim: Optional[HPOEnrichment] = None
 
 
 @router.get(
     '/search/{query}',
     tags=['terms'],
     response_description='List of HPOTerms',
-    response_model=List[models.HPO],
+    response_model=List[models.HpoTerm],
     response_model_exclude_none=True
 )
 async def HPO_search(
     query: str,
     verbose: bool = False,
     limit: int = 10,
     offset: int = 0
@@ -215,15 +220,15 @@
         ]
 
 
 @router.get(
     '/similarity',
     tags=['similarity'],
     response_description='Similarity score',
-    response_model=models.Similarity_Score
+    response_model=models.SimilarityScore
 )
 async def terms_similarity(
     set1: str = Query(..., example='HP:0007401,HP:0010885,HP:0006530'),
     set2: str = Query(..., example='HP:0200070,HP:0002754,HP:0031630'),
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
@@ -281,35 +286,52 @@
     -------
     float
         The similarity score to the other HPOSet
     """
     hposet1 = get_hpo_set(set1)
     hposet2 = get_hpo_set(set2)
 
-    return {
-        'set1': hposet1.toJSON(),
-        'set2': hposet2.toJSON(),
-        'similarity': hposet1.similarity(
-            hposet2,
-            kind=kind,
-            method=method,
-            combine=combine
-        )
-    }
+    try:
+        return {
+            'set1': hposet1.toJSON(),
+            'set2': hposet2.toJSON(),
+            'similarity': hposet1.similarity(
+                hposet2,
+                kind=kind,
+                method=method,
+                combine=combine
+            )
+        }
+    except NotImplementedError:
+        raise HTTPException(
+            status_code=400,
+            detail="The similarity method is not properly implemented"
+            )
+    except RuntimeError:
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid `method` or `combine` parameter"
+            )
+    except AttributeError:
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid information content kind specified"
+            )
+
 
 
 @router.post('/similarity/', include_in_schema=False)
 @router.post(
     '/similarity',
     tags=['similarity'],
     response_description='Similarity scores',
-    response_model=models.Batch_Similarity_Score
+    response_model=models.SimilarityScore_Batch
 )
 async def batch_similarity(
-    data: models.POST_Batch,
+    data: models.PostBody_HpoSets,
     method: str = 'graphic',
     combine: str = 'funSimAvg',
     kind: str = 'omim'
 ) -> dict:
     """
     Calculate similarity scores between one base and
     several other HPOSets
@@ -318,15 +340,15 @@
 
     * **HPO Identifier**: ``'HP:0000003'``
     * **Term name**: ``'Multicystic kidney dysplasia'``
     * **Integer representation of HPO ID**: ``3``
 
     Parameters
     ----------
-    data: POST_Batch
+    data: PostBody_HpoSets
 
     kind: str, default ``None``
         Which kind of information content should be calculated.
         Options are ['omim', 'orpha', 'decipher', 'gene']
         See :func:`pyhpo.HPOTerm.similarity_score` for options
 
     method: string, default ``None``
@@ -373,17 +395,35 @@
                 set2,
                 kind=kind,
                 method=method,
                 combine=combine
             )
         except HTTPException as ex:
             res['similarity'] = None
-            res['error'] = ex.headers.get(
-                'X-TermNotFound', 'Unknown error'
-            )  # type: ignore
+            if ex.headers:
+                res['error'] = ex.headers.get(
+                    'X-TermNotFound', 'Unknown error'
+                )
+            else:
+                res['error'] = 'Unknown error'
+        except NotImplementedError:
+            raise HTTPException(
+                status_code=400,
+                detail="The similarity method is not properly implemented"
+                )
+        except RuntimeError:
+            raise HTTPException(
+                status_code=400,
+                detail="Invalid `method` or `combine` parameter"
+                )
+        except AttributeError:
+            raise HTTPException(
+                status_code=400,
+                detail="Invalid information content kind specified"
+                )
 
         other_sets.append(res)
     return {
         'set1': set1.toJSON(),
         'other_sets': other_sets
     }
 
@@ -423,15 +463,22 @@
     Returns
     -------
     list of dict
         A ordered list with enriched genes
     """
     assert gene_model, 'The Gene Enrichment Model is not defined'
     hposet = get_hpo_set(set1)
-    res = gene_model.enrichment(method, hposet)
+    try:
+        res = gene_model.enrichment(method, hposet)
+    except (NotImplementedError, RuntimeError):
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid parameter"
+            )
+
     return [{
         'gene': x['item'].toJSON(),
         'count': x['count'],
         'enrichment': x['enrichment']
     } for x in res[offset:(limit+offset)]]
 
 
@@ -474,28 +521,35 @@
     -------
     list of dict
         A ordered list with enriched genes
     """
     assert omim_model, 'The OMIM Enrichment Model is not defined'
 
     hposet = get_hpo_set(set1)
-    res = omim_model.enrichment(method, hposet)
+    try:
+        res = omim_model.enrichment(method, hposet)
+    except (NotImplementedError, RuntimeError):
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid parameter"
+            )
+
     return [{
         'omim': x['item'].toJSON(),
         'count': x['count'],
         'enrichment': x['enrichment']
     } for x in res[offset:(limit+offset)]]
 
 
 @router.get('/suggest/', include_in_schema=False)
 @router.get(
     '/suggest',
     tags=['enrichment'],
     response_description='HPOTerm list',
-    response_model=List[models.HPO]
+    response_model=List[models.HpoTerm]
 )
 async def hpo_suggest(
     set1: str = Query(..., example='HP:0007401,HP:0010885,HP:0006530'),
     method: str = 'hypergeom',
     limit: int = 10,
     offset: int = 0,
     n_genes: int = 5,
@@ -541,28 +595,39 @@
     assert gene_model, 'The Gene Enrichment Model is not defined'
     assert omim_model, 'The OMIM Enrichment Model is not defined'
     assert hpo_model_genes, 'The HPO Gene Enrichment Model is not defined'
     assert hpo_model_omim, 'The HPO OMIM Enrichment Model is not defined'
 
     hposet = get_hpo_set(set1)
 
-    if n_omim:
-        omim_res = hpo_model_omim.enrichment(
-            method,
-            [x['item'] for x in omim_model.enrichment(method, hposet)[0:n_omim]]
-        )
-    else:
-        omim_res = []
-    if n_genes:
-        gene_res = hpo_model_genes.enrichment(
-            method,
-            [x['item'] for x in gene_model.enrichment(method, hposet)[0:n_genes]]
-        )
-    else:
-        gene_res = []
+    try:
+        if n_omim:
+            omim_res = hpo_model_omim.enrichment(
+                method,
+                [x['item'] for x in omim_model.enrichment(method, hposet)[0:n_omim]]
+            )
+        else:
+            omim_res = []
+        if n_genes:
+            gene_res = hpo_model_genes.enrichment(
+                method,
+                [x['item'] for x in gene_model.enrichment(method, hposet)[0:n_genes]]
+            )
+        else:
+            gene_res = []
+    except NotImplementedError:
+        raise HTTPException(
+            status_code=404,
+            detail="This method is not implemented"
+            )
+    except RuntimeError:
+        raise HTTPException(
+            status_code=400,
+            detail="Invalid parameter"
+            )
 
     res = sorted(omim_res + gene_res, key=lambda x: x['enrichment'])[offset:]
 
     hpos: List[HPOTerm] = []
     while len(hpos) < limit and len(res):
         hpo = res.pop(0)['hpo']
         if hpo not in hpos and hpo not in hposet:
@@ -581,17 +646,19 @@
 ) -> List[dict]:
     hposet = get_hpo_set(set1)
 
     children = set()
     for term in hposet:
         for child in term.children:
             if child not in hposet and child not in children:
-                children.add(term)
+                children.add(child)
+    for term in hposet:
+        children.add(term)
 
     return [{
         'name': term.name,
         'omim': term.information_content['omim'],
         'gene': term.information_content['gene'],
         'imports': [t.name for t in term.children],
         'diseases': [d.name for d in term.omim_diseases],
         'genes': [g.name for g in term.genes]
-    } for term in (hposet | children)]
+    } for term in (children)]
```

### Comparing `pyhpoapi-1.2.2/pyhpoapi/server.py` & `pyhpoapi-2.0.0/pyhpoapi/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import os
+import logging
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.openapi.utils import get_openapi
 from fastapi.responses import FileResponse
 
-from pyhpo.ontology import Ontology
-from pyhpo.stats import EnrichmentModel, HPOEnrichment
+from pyhpo import Ontology
+from pyhpo.stats import EnrichmentModel
+try:
+    from pyhpo.stats import HPOEnrichment
+except ImportError:
+    from pyhpoapi.helpers import MockHPOEnrichment as HPOEnrichment
+
 import pyhpo
 
 from pyhpoapi.routers import term, terms, annotations
 from pyhpoapi import config
 
+logger = logging.getLogger("uvicorn.error")
 
 def custom_openapi_wrapper(app):
     def custom_openapi():
         if app.openapi_schema:
             return app.openapi_schema
         openapi_schema = get_openapi(
             title='PyHPO API',
@@ -31,15 +38,23 @@
         }
         app.openapi_schema = openapi_schema
         return app.openapi_schema
     return custom_openapi
 
 
 def initialize_ontology() -> None:
-    _ = Ontology()
+    data_dir = config.MASTER_DATA
+
+    if data_dir == "":
+        logger.debug("Using builtin standard ontology")
+        _ = Ontology()
+    else:
+        logger.info(f"Loading Ontology from {data_dir}")
+        _ = Ontology(data_dir)
+
     terms.gene_model = EnrichmentModel('gene')
     terms.omim_model = EnrichmentModel('omim')
     terms.hpo_model_genes = HPOEnrichment('gene')
     terms.hpo_model_omim = HPOEnrichment('omim')
 
 
 def main():
```

