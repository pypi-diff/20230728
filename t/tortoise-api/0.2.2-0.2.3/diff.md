# Comparing `tmp/tortoise-api-0.2.2.tar.gz` & `tmp/tortoise-api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.2.2.tar", last modified: Fri Jul 28 08:04:14 2023, max compression
+gzip compressed data, was "tortoise-api-0.2.3.tar", last modified: Fri Jul 28 19:32:32 2023, max compression
```

## Comparing `tortoise-api-0.2.2.tar` & `tortoise-api-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:04:14.639323 tortoise-api-0.2.2/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.2/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 08:04:14.639127 tortoise-api-0.2.2/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.2/README.md
--rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-28 08:03:34.000000 tortoise-api-0.2.2/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 08:04:14.639371 tortoise-api-0.2.2/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:04:14.637482 tortoise-api-0.2.2/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.2/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     3186 2023-07-27 10:21:50.000000 tortoise-api-0.2.2/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)     2591 2023-07-28 07:59:54.000000 tortoise-api-0.2.2/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:04:14.638788 tortoise-api-0.2.2/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-28 08:04:14.000000 tortoise-api-0.2.2/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:32:32.330144 tortoise-api-0.2.3/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.3/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 19:32:32.329777 tortoise-api-0.2.3/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.3/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-28 19:32:07.000000 tortoise-api-0.2.3/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 19:32:32.330228 tortoise-api-0.2.3/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:32:32.327515 tortoise-api-0.2.3/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.3/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     3186 2023-07-27 10:21:50.000000 tortoise-api-0.2.3/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)     2768 2023-07-28 19:32:07.000000 tortoise-api-0.2.3/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:32:32.329301 tortoise-api-0.2.3/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.2.2/LICENSE` & `tortoise-api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.2/PKG-INFO` & `tortoise-api-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `tortoise-api-0.2.2/README.md` & `tortoise-api-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.2/pyproject.toml` & `tortoise-api-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 dependencies = [
     "asyncpg",
     "python-dotenv",
     "starlette",
     "tortoise-api-model>=0.0.5",
     "uvicorn"
 ]
-version = "0.2.2"
+version = "0.2.3"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.2.2/tortoise_api/api.py` & `tortoise-api-0.2.3/tortoise_api/api.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.2/tortoise_api/util.py` & `tortoise-api-0.2.3/tortoise_api/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date
 from urllib.parse import parse_qsl, unquote
 
-from asyncpg import Polygon
+from asyncpg import Polygon, Range
 from tortoise.fields import Field
 from tortoise.fields.relational import RelationalField, ReverseRelation
 from tortoise_api_model import Model
 
 
 def jsonify(obj: Model) -> dict:
     def check(field: Field, key: str):
@@ -13,14 +13,16 @@
             return {'id': mod.id, 'type': mod.__class__.__name__, 'repr': mod.repr()}
 
         prop = getattr(obj, key)
         if isinstance(prop, date):
             return prop.__str__().split('+')[0].split('.')[0] # '+' separates tz part, '.' separates millisecond part
         if isinstance(prop, Polygon):
             return prop.points
+        if isinstance(prop, Range):
+            return prop.lower, prop.upper
         elif isinstance(field, RelationalField):
             if isinstance(prop, Model):
                 return rel_pack(prop)
             elif isinstance(prop, ReverseRelation) and isinstance(prop.related_objects, list):
                 return [rel_pack(d) for d in prop.related_objects]
             elif prop is None:
                 return ''
@@ -34,26 +36,26 @@
     data = {}
     for k, v in parse_qsl(unquote(s)):
         # for collection-like fields (1d tuples): multiple the same name params merges to tuple
         if k in data:
             if isinstance(data[k], tuple):
                 data[k] += (v,)
             else:
-                data[k] = data[k], v
+                data[k] = data[k], float(v)
         # for list-like fields(2d lists: (1d list of 1d tuples)): '.'-separated param names splits to {key}.{index}
         elif '.' in k:
             bk, i = k.split('.')
             i = int(i)
             data[bk] = data.get(bk, [()])
             if len(data[bk]) > i:
                 data[bk][i] += (v,)
             else:
                 data[bk].append((v,))
-        else:
-            data[k] = v
+        else: # if v is IntEnum - it requires explicit convert to int
+            data[k] = int(v) if v.isnumeric() else v
     return data
 
 # async def upsert(model: type[Model], dct: dict):
 #     meta: MetaInfo = model._meta
 #     if pk := meta.pk_attr in dct.keys():
 #         unq = {pk: dct.pop(pk)}
 #     else:
```

### Comparing `tortoise-api-0.2.2/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.2.3/tortoise_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

