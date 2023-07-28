# Comparing `tmp/tortoise-api-0.2.1.tar.gz` & `tmp/tortoise-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.2.1.tar", last modified: Thu Jul 27 10:59:42 2023, max compression
+gzip compressed data, was "tortoise-api-0.2.2.tar", last modified: Fri Jul 28 08:04:14 2023, max compression
```

## Comparing `tortoise-api-0.2.1.tar` & `tortoise-api-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 10:59:42.174822 tortoise-api-0.2.1/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.1/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-27 10:59:42.174587 tortoise-api-0.2.1/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.1/README.md
--rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-27 10:59:05.000000 tortoise-api-0.2.1/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-27 10:59:42.174881 tortoise-api-0.2.1/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 10:59:42.173206 tortoise-api-0.2.1/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.1/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     3186 2023-07-27 10:21:50.000000 tortoise-api-0.2.1/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)     1979 2023-07-27 10:21:50.000000 tortoise-api-0.2.1/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 10:59:42.174286 tortoise-api-0.2.1/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:04:14.639323 tortoise-api-0.2.2/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.2/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 08:04:14.639127 tortoise-api-0.2.2/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.2/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-28 08:03:34.000000 tortoise-api-0.2.2/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 08:04:14.639371 tortoise-api-0.2.2/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:04:14.637482 tortoise-api-0.2.2/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.2/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     3186 2023-07-27 10:21:50.000000 tortoise-api-0.2.2/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)     2591 2023-07-28 07:59:54.000000 tortoise-api-0.2.2/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:04:14.638788 tortoise-api-0.2.2/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.2.1/LICENSE` & `tortoise-api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.1/PKG-INFO` & `tortoise-api-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `tortoise-api-0.2.1/README.md` & `tortoise-api-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.1/pyproject.toml` & `tortoise-api-0.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 description = "Simplest fastest minimal REST API CRUD generator for Tortoise ORM models"
 readme = "README.md"
 license = {text = "MIT"}
 dependencies = [
     "asyncpg",
     "python-dotenv",
     "starlette",
-    "tortoise-api-model>=0.0.4",
+    "tortoise-api-model>=0.0.5",
     "uvicorn"
 ]
-version = "0.2.1"
+version = "0.2.2"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.2.1/tortoise_api/api.py` & `tortoise-api-0.2.2/tortoise_api/api.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.1/tortoise_api/util.py` & `tortoise-api-0.2.2/tortoise_api/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from datetime import date
 from urllib.parse import parse_qsl, unquote
 
+from asyncpg import Polygon
 from tortoise.fields import Field
 from tortoise.fields.relational import RelationalField, ReverseRelation
 from tortoise_api_model import Model
 
 
 def jsonify(obj: Model) -> dict:
     def check(field: Field, key: str):
         def rel_pack(mod: Model) -> dict:
             return {'id': mod.id, 'type': mod.__class__.__name__, 'repr': mod.repr()}
 
         prop = getattr(obj, key)
         if isinstance(prop, date):
-            return prop.__str__().split('.')[0].split('+')[0]
+            return prop.__str__().split('+')[0].split('.')[0] # '+' separates tz part, '.' separates millisecond part
+        if isinstance(prop, Polygon):
+            return prop.points
         elif isinstance(field, RelationalField):
             if isinstance(prop, Model):
                 return rel_pack(prop)
             elif isinstance(prop, ReverseRelation) and isinstance(prop.related_objects, list):
                 return [rel_pack(d) for d in prop.related_objects]
             elif prop is None:
                 return ''
@@ -26,19 +29,29 @@
             return getattr(obj, key)
 
     return {key: check(field, key) for key, field in obj._meta.fields_map.items() if not key.endswith('_id')}
 
 def parse_qs(s: str) -> dict:
     data = {}
     for k, v in parse_qsl(unquote(s)):
+        # for collection-like fields (1d tuples): multiple the same name params merges to tuple
         if k in data:
             if isinstance(data[k], tuple):
                 data[k] += (v,)
             else:
                 data[k] = data[k], v
+        # for list-like fields(2d lists: (1d list of 1d tuples)): '.'-separated param names splits to {key}.{index}
+        elif '.' in k:
+            bk, i = k.split('.')
+            i = int(i)
+            data[bk] = data.get(bk, [()])
+            if len(data[bk]) > i:
+                data[bk][i] += (v,)
+            else:
+                data[bk].append((v,))
         else:
             data[k] = v
     return data
 
 # async def upsert(model: type[Model], dct: dict):
 #     meta: MetaInfo = model._meta
 #     if pk := meta.pk_attr in dct.keys():
```

### Comparing `tortoise-api-0.2.1/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.2.2/tortoise_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

