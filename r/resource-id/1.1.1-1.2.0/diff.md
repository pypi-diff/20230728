# Comparing `tmp/resource-id-1.1.1.tar.gz` & `tmp/resource-id-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resource-id-1.1.1.tar", last modified: Wed Jul 12 15:57:00 2023, max compression
+gzip compressed data, was "resource-id-1.2.0.tar", last modified: Fri Jul 28 16:18:13 2023, max compression
```

## Comparing `resource-id-1.1.1.tar` & `resource-id-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.396359 resource-id-1.1.1/
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.392509 resource-id-1.1.1/.github/
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.394767 resource-id-1.1.1/.github/workflows/
--rw-r--r--   0 charles    (501) staff       (20)      798 2022-08-03 19:18:47.000000 resource-id-1.1.1/.github/workflows/tox.yml
--rw-r--r--   0 charles    (501) staff       (20)       68 2022-08-03 21:40:24.000000 resource-id-1.1.1/.gitignore
--rw-r--r--   0 charles    (501) staff       (20)      246 2023-07-12 15:41:47.000000 resource-id-1.1.1/CHANGELOG.md
--rw-r--r--   0 charles    (501) staff       (20)     1055 2022-08-03 21:44:13.000000 resource-id-1.1.1/LICENSE.txt
--rw-r--r--   0 charles    (501) staff       (20)       20 2022-08-03 21:44:57.000000 resource-id-1.1.1/MANIFEST.in
--rw-r--r--   0 charles    (501) staff       (20)      929 2023-07-12 15:57:00.396460 resource-id-1.1.1/PKG-INFO
--rw-r--r--   0 charles    (501) staff       (20)     2166 2023-07-12 15:52:32.000000 resource-id-1.1.1/README.md
--rw-r--r--   0 charles    (501) staff       (20)      184 2022-08-03 16:07:41.000000 resource-id-1.1.1/pyproject.toml
--rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:42:00.000000 resource-id-1.1.1/pytest.ini
--rw-r--r--   0 charles    (501) staff       (20)      114 2022-08-03 21:39:13.000000 resource-id-1.1.1/requirements.txt
--rw-r--r--   0 charles    (501) staff       (20)     1051 2023-07-12 15:57:00.396823 resource-id-1.1.1/setup.cfg
--rw-r--r--   0 charles    (501) staff       (20)       38 2022-08-03 16:05:04.000000 resource-id-1.1.1/setup.py
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.392991 resource-id-1.1.1/src/
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.395197 resource-id-1.1.1/src/resource_id/
--rw-r--r--   0 charles    (501) staff       (20)      435 2022-08-03 18:32:10.000000 resource-id-1.1.1/src/resource_id/__init__.py
--rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 19:57:16.000000 resource-id-1.1.1/src/resource_id/py.typed
--rw-r--r--   0 charles    (501) staff       (20)     4498 2023-07-12 15:26:10.000000 resource-id-1.1.1/src/resource_id/resource_id.py
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.395947 resource-id-1.1.1/src/resource_id.egg-info/
--rw-r--r--   0 charles    (501) staff       (20)      929 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/PKG-INFO
--rw-r--r--   0 charles    (501) staff       (20)      475 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/SOURCES.txt
--rw-r--r--   0 charles    (501) staff       (20)        1 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/dependency_links.txt
--rw-r--r--   0 charles    (501) staff       (20)       57 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/requires.txt
--rw-r--r--   0 charles    (501) staff       (20)       12 2023-07-12 15:57:00.000000 resource-id-1.1.1/src/resource_id.egg-info/top_level.txt
-drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-12 15:57:00.396221 resource-id-1.1.1/tests/
--rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:44:50.000000 resource-id-1.1.1/tests/__init__.py
--rw-r--r--   0 charles    (501) staff       (20)     2434 2023-07-12 14:30:12.000000 resource-id-1.1.1/tests/test_resource_id.py
--rw-r--r--   0 charles    (501) staff       (20)      315 2023-07-12 15:31:01.000000 resource-id-1.1.1/tox.ini
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-28 16:18:13.477390 resource-id-1.2.0/
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-28 16:18:13.472364 resource-id-1.2.0/.github/
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-28 16:18:13.475034 resource-id-1.2.0/.github/workflows/
+-rw-r--r--   0 charles    (501) staff       (20)      798 2022-08-03 19:18:47.000000 resource-id-1.2.0/.github/workflows/tox.yml
+-rw-r--r--   0 charles    (501) staff       (20)       68 2022-08-03 21:40:24.000000 resource-id-1.2.0/.gitignore
+-rw-r--r--   0 charles    (501) staff       (20)      491 2023-07-28 16:01:30.000000 resource-id-1.2.0/CHANGELOG.md
+-rw-r--r--   0 charles    (501) staff       (20)     1055 2022-08-03 21:44:13.000000 resource-id-1.2.0/LICENSE.txt
+-rw-r--r--   0 charles    (501) staff       (20)       20 2022-08-03 21:44:57.000000 resource-id-1.2.0/MANIFEST.in
+-rw-r--r--   0 charles    (501) staff       (20)      929 2023-07-28 16:18:13.477483 resource-id-1.2.0/PKG-INFO
+-rw-r--r--   0 charles    (501) staff       (20)     2166 2023-07-12 15:52:32.000000 resource-id-1.2.0/README.md
+-rw-r--r--   0 charles    (501) staff       (20)      184 2022-08-03 16:07:41.000000 resource-id-1.2.0/pyproject.toml
+-rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:42:00.000000 resource-id-1.2.0/pytest.ini
+-rw-r--r--   0 charles    (501) staff       (20)      114 2022-08-03 21:39:13.000000 resource-id-1.2.0/requirements.txt
+-rw-r--r--   0 charles    (501) staff       (20)     1051 2023-07-28 16:18:13.477830 resource-id-1.2.0/setup.cfg
+-rw-r--r--   0 charles    (501) staff       (20)       38 2022-08-03 16:05:04.000000 resource-id-1.2.0/setup.py
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-28 16:18:13.472614 resource-id-1.2.0/src/
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-28 16:18:13.475952 resource-id-1.2.0/src/resource_id/
+-rw-r--r--   0 charles    (501) staff       (20)      433 2023-07-28 15:54:47.000000 resource-id-1.2.0/src/resource_id/__init__.py
+-rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 19:57:16.000000 resource-id-1.2.0/src/resource_id/py.typed
+-rw-r--r--   0 charles    (501) staff       (20)     3848 2023-07-28 15:54:26.000000 resource-id-1.2.0/src/resource_id/resource_id.py
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-28 16:18:13.476865 resource-id-1.2.0/src/resource_id.egg-info/
+-rw-r--r--   0 charles    (501) staff       (20)      929 2023-07-28 16:18:13.000000 resource-id-1.2.0/src/resource_id.egg-info/PKG-INFO
+-rw-r--r--   0 charles    (501) staff       (20)      475 2023-07-28 16:18:13.000000 resource-id-1.2.0/src/resource_id.egg-info/SOURCES.txt
+-rw-r--r--   0 charles    (501) staff       (20)        1 2023-07-28 16:18:13.000000 resource-id-1.2.0/src/resource_id.egg-info/dependency_links.txt
+-rw-r--r--   0 charles    (501) staff       (20)       57 2023-07-28 16:18:13.000000 resource-id-1.2.0/src/resource_id.egg-info/requires.txt
+-rw-r--r--   0 charles    (501) staff       (20)       12 2023-07-28 16:18:13.000000 resource-id-1.2.0/src/resource_id.egg-info/top_level.txt
+drwxr-xr-x   0 charles    (501) staff       (20)        0 2023-07-28 16:18:13.477118 resource-id-1.2.0/tests/
+-rw-r--r--   0 charles    (501) staff       (20)        0 2022-08-03 15:44:50.000000 resource-id-1.2.0/tests/__init__.py
+-rw-r--r--   0 charles    (501) staff       (20)     2707 2023-07-28 15:54:35.000000 resource-id-1.2.0/tests/test_resource_id.py
+-rw-r--r--   0 charles    (501) staff       (20)      373 2023-07-28 15:54:03.000000 resource-id-1.2.0/tox.ini
```

### Comparing `resource-id-1.1.1/.github/workflows/tox.yml` & `resource-id-1.2.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `resource-id-1.1.1/LICENSE.txt` & `resource-id-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resource-id-1.1.1/PKG-INFO` & `resource-id-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-id
-Version: 1.1.1
+Version: 1.2.0
 Summary: Base62-encoded identifier.
 Home-page: https://github.com/declaresub/resource-id
 Author: Charles Yeomans
 Author-email: charles@declaresub.com
 License: MIT
 Keywords: identifier,url,base62
 Platform: any
```

### Comparing `resource-id-1.1.1/README.md` & `resource-id-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `resource-id-1.1.1/setup.cfg` & `resource-id-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `resource-id-1.1.1/src/resource_id.egg-info/PKG-INFO` & `resource-id-1.2.0/src/resource_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-id
-Version: 1.1.1
+Version: 1.2.0
 Summary: Base62-encoded identifier.
 Home-page: https://github.com/declaresub/resource-id
 Author: Charles Yeomans
 Author-email: charles@declaresub.com
 License: MIT
 Keywords: identifier,url,base62
 Platform: any
```

### Comparing `resource-id-1.1.1/tests/test_resource_id.py` & `resource-id-1.2.0/tests/test_resource_id.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,103 @@
 from typing import Union
 from uuid import UUID
 
 import pydantic
 import pytest
 
-from resource_id import ResourceId
-from resource_id.resource_id import Base62Encodable
+from resource_id.resource_id import Base62Encodable, ResourceId, b62decode, b62encode
 
 pydantic_major_version = int(pydantic.VERSION.split(".")[0])
 
 
-@pytest.mark.parametrize("arg", [1, "test", UUID(int=1728)])
-def test_init(arg: Union[str, Base62Encodable]):
-    assert ResourceId(arg)
+@pytest.mark.parametrize("src, expected", [(1, "1"), (62, "10")])
+def test_b62encode(src: Base62Encodable, expected: str):
+    assert b62encode(src) == expected
 
 
-def test_init_bad_value():
+def test_b62encode_fail():
     with pytest.raises(ValueError):
-        ResourceId(-1)
+        b62encode(-1)
 
 
-def test_init_bad_type():
-    with pytest.raises(TypeError):
-        ResourceId(None)  # type: ignore
+@pytest.mark.parametrize("src, expected", [("1", 1), ("11", 63)])
+def test_b62decode(src: str, expected: int):
+    assert b62decode(src) == expected
 
 
-def test_bad_value_after_init():
-    res_id = ResourceId(1)
-    res_id.value = -1
+def test_b62decode_fail():
     with pytest.raises(ValueError):
-        repr(res_id)
+        b62decode("*")
 
 
-def test_repr():
-    arg = 1
-    assert repr(ResourceId(arg)) == "1"
+@pytest.mark.parametrize("arg, value", [(1, 1), ("11", 63), (UUID(int=1728), 1728)])
+def test_init(arg: Union[str, Base62Encodable], value: int):
+    assert ResourceId(arg).value == value
 
 
-def test_invalid_base62():
+def test_init_bad_arg_value():
     with pytest.raises(ValueError):
-        ResourceId("bad-value")
+        ResourceId(-1)
+
+
+def test_init_bad_arg_type():
+    with pytest.raises(TypeError):
+        ResourceId({})  # type: ignore
 
 
 def test_uuid():
     value = UUID(int=123)
     assert ResourceId(value).uuid == value
 
 
+def test_repr():
+    arg = 1
+    assert repr(ResourceId(arg)) == "1"
+
+
 def test_eq():
     assert ResourceId(1) == ResourceId(1)
 
 
-def test_eq_class_mismatch():
-    with pytest.raises(TypeError):
-        ResourceId(1) != 1  # type: ignore
+def test_not_eq():
+    assert ResourceId(1) != 1
 
 
 def test_hash():
-    assert hash(ResourceId(1))
+    assert hash(ResourceId(1)) == hash(1)
 
 
 def test_int():
     value = 2
     assert int(ResourceId(value)) == value
 
 
 def test___get_validators__():
-    assert next(ResourceId.__get_validators__()) == ResourceId.validate
-
-
-@pytest.mark.parametrize("arg", [1, "test", UUID(int=1728)])
-def test_validate(arg: Union[str, Base62Encodable]):
-    assert ResourceId.validate(arg)
+    # for pydantic 2, ResourceId is wrapped with Annotated, and special methot lookup bypasses __getattr__.  Thus we must
+    # get the actual ResourceId class from the Annootated object.
+    __get_validators__ = ResourceId.__origin__.__get_validators__ if hasattr(ResourceId, "__origin__") else ResourceId.__get_validators__  # type: ignore
+    assert next(__get_validators__()) == ResourceId.validate  # type: ignore
 
 
-def test___modify_schema__():
-    field_schema = {}
-    ResourceId.__modify_schema__(field_schema)
-    assert field_schema["title"] == ResourceId.__name__
+def test_validate():
+    assert ResourceId.validate("test") == ResourceId("test")
 
 
-class Foo(pydantic.BaseModel):
-    id: ResourceId
+def test_modify_schema():
+    __modify_schema__ = ResourceId.__origin__.__modify_schema__ if hasattr(ResourceId, "__origin__") else ResourceId.__modify_schema__  # type: ignore
+    schema = {}
+    __modify_schema__(schema)
+    assert schema == ResourceId._json_schema()  # type: ignore
 
 
-def test_foo_init():
-    foo = Foo(id=ResourceId("test"))
-    assert foo.id == ResourceId("test")
+def test__json_schema():
+    assert isinstance(ResourceId._json_schema(), dict)  # type: ignore
 
 
-def test_pydantic_json_schema():
-    # it is not so easy to test __get_pydantic_json_schema__ directly without digging around in the innards of pydantic 2.
-    # so we just check the schema generated for Foo to see that its id item has the expected JSON schema for ResourceId.
-    foo = Foo(id=ResourceId("test"))
-    schema = foo.schema() if pydantic_major_version < 2 else foo.model_json_schema()  # type: ignore
-    assert "properties" in schema
-    assert schema["properties"]["id"] == {
-        "description": ResourceId.schema_description,
-        "title": ResourceId.__name__,
-        "type": "string",
-    }
+@pytest.mark.skipif(
+    not hasattr(pydantic, "TypeAdapter"),
+    reason="Serialization is only implemented for pydantic 2.",
+)
+def test_serialization_pydantic2():
+    V = pydantic.TypeAdapter(ResourceId)
+    id = ResourceId("test")
+    assert V.dump_json(id) == b'"test"'
```

