# Comparing `tmp/quiltcore-0.2.1.tar.gz` & `tmp/quiltcore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltcore-0.2.1.tar", max compression
+gzip compressed data, was "quiltcore-0.3.0.tar", max compression
```

## Comparing `quiltcore-0.2.1.tar` & `quiltcore-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.2.1/LICENSE
--rw-r--r--   0        0        0     1579 2023-07-06 04:28:48.600645 quiltcore-0.2.1/README.md
--rw-r--r--   0        0        0      852 2023-07-12 20:05:58.181559 quiltcore-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-07-05 18:42:27.110229 quiltcore-0.2.1/quiltcore/__init__.py
--rw-r--r--   0        0        0     2939 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/changes.py
--rw-r--r--   0        0        0      972 2023-07-05 20:12:59.420575 quiltcore-0.2.1/quiltcore/delta.py
--rw-r--r--   0        0        0     3172 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/entry.py
--rw-r--r--   0        0        0     2138 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/manifest.py
--rw-r--r--   0        0        0      632 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/namespace.py
--rw-r--r--   0        0        0     1615 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/registry.py
--rw-r--r--   0        0        0     4050 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/resource.py
--rw-r--r--   0        0        0     1968 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/resource_key.py
--rw-r--r--   0        0        0     1525 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/resource_path.py
--rw-r--r--   0        0        0     4748 2023-07-12 12:22:04.000000 quiltcore-0.2.1/quiltcore/volume.py
--rw-r--r--   0        0        0      774 2023-07-12 03:19:19.355733 quiltcore-0.2.1/quiltcore/yaml/config.py
--rw-r--r--   0        0        0      761 2023-07-12 03:16:11.259596 quiltcore-0.2.1/quiltcore/yaml/quiltcore.yaml
--rw-r--r--   0        0        0      160 2023-06-30 01:13:50.059736 quiltcore-0.2.1/quiltcore/yaml/schema.yaml
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 quiltcore-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1573 2023-07-20 22:18:01.855543 quiltcore-0.3.0/README.md
+-rw-r--r--   0        0        0     1115 2023-07-25 20:44:00.240364 quiltcore-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1291 2023-07-26 23:35:28.000000 quiltcore-0.3.0/quiltcore/__init__.py
+-rw-r--r--   0        0        0     1765 2023-07-28 05:16:48.000000 quiltcore-0.3.0/quiltcore/builder.py
+-rw-r--r--   0        0        0     1924 2023-07-28 05:16:48.000000 quiltcore-0.3.0/quiltcore/changes.py
+-rw-r--r--   0        0        0     2063 2023-07-27 22:25:00.498998 quiltcore-0.3.0/quiltcore/delta.py
+-rw-r--r--   0        0        0     2081 2023-07-27 20:11:29.346954 quiltcore-0.3.0/quiltcore/entry.py
+-rw-r--r--   0        0        0     1451 2023-07-27 21:55:58.252178 quiltcore-0.3.0/quiltcore/header.py
+-rw-r--r--   0        0        0     2532 2023-07-28 05:16:48.000000 quiltcore-0.3.0/quiltcore/manifest.py
+-rw-r--r--   0        0        0      628 2023-07-26 15:49:28.518544 quiltcore-0.3.0/quiltcore/namespace.py
+-rw-r--r--   0        0        0     1729 2023-07-27 01:48:38.308147 quiltcore-0.3.0/quiltcore/registry.py
+-rw-r--r--   0        0        0     4832 2023-07-26 19:06:47.603824 quiltcore-0.3.0/quiltcore/resource.py
+-rw-r--r--   0        0        0     3176 2023-07-25 20:35:00.181308 quiltcore-0.3.0/quiltcore/resource_key.py
+-rw-r--r--   0        0        0     1516 2023-07-25 20:35:00.182089 quiltcore-0.3.0/quiltcore/resource_path.py
+-rw-r--r--   0        0        0     1859 2023-07-27 20:11:40.022675 quiltcore-0.3.0/quiltcore/table.py
+-rw-r--r--   0        0        0     6082 2023-07-27 20:22:02.254112 quiltcore-0.3.0/quiltcore/volume.py
+-rw-r--r--   0        0        0     8926 2023-07-27 22:05:43.358147 quiltcore-0.3.0/quiltcore/yaml/codec.py
+-rw-r--r--   0        0        0      848 2023-07-25 20:35:00.185720 quiltcore-0.3.0/quiltcore/yaml/config.py
+-rw-r--r--   0        0        0     1217 2023-07-27 22:10:38.941860 quiltcore-0.3.0/quiltcore/yaml/quiltcore.yaml
+-rw-r--r--   0        0        0      833 2023-07-27 22:07:49.354966 quiltcore-0.3.0/quiltcore/yaml/quiltspec.yaml
+-rw-r--r--   0        0        0      160 2023-07-20 04:22:58.224611 quiltcore-0.3.0/quiltcore/yaml/schema.yaml
+-rw-r--r--   0        0        0     1053 2023-07-20 22:23:12.863928 quiltcore-0.3.0/quiltcore/yaml/spec.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 quiltcore-0.3.0/PKG-INFO
```

### Comparing `quiltcore-0.2.1/LICENSE` & `quiltcore-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quiltcore-0.2.1/README.md` & `quiltcore-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 entry = manifest.get(TEST_KEY)
 ```
 
 ### Get Object
 
 <!--pytest-codeblocks:cont-->
 ```python
-with TemporaryDirectory() as tmpdirname:
-  dest = UPath(tmpdirname)
+with TemporaryDirectory() as tmpdir:
+  dest = UPath(tmpdir)
   outfile = dest / TEST_KEY
-  entry.get(dest)
+  entry.get(tmpdir)
   print(outfile.resolve())
   assert outfile.exists()
   local_bytes = outfile.read_bytes()
   assert entry.verify(local_bytes)
 ```
```

### Comparing `quiltcore-0.2.1/pyproject.toml` & `quiltcore-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 [tool.poetry]
 name = "quiltcore"
-version = "0.2.1"
+version = "0.3.0"
 description = "low-level plubming to read/write Quilt packages"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
+
 [tool.poetry.dependencies]
 python = "^3.10"
+jsonlines = "1.2.0"
+multiformats = "^0.2.1"
+pandas = "^2.0.2"
+pyarrow = "^12.0.0"
+pandas-stubs = "^2.0.2.230605"
+quilt3 = "^5.3.1"
+s3fs = "^2023.6.0"
 typing-extensions = "^4.6.3"
 tzlocal = "^5.0.1"
 un-yaml = ">=0.3.1"
 # un-yaml = {git = "https://github.com/data-yaml/un-yaml.git", rev = "main"}
-pyarrow = "^12.0.0"
-pandas = "^2.0.2"
-pytest-codeblocks = "^0.16.1"
-universal-pathlib = "^0.0.23"
-s3fs = "^2023.6.0"
-pandas-stubs = "^2.0.2.230605"
-multiformats = "^0.2.1"
-jsonlines = "^3.1.0"
+universal-pathlib = "^0.0.24"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.4.1"
 pytest-watcher = "^0.3.4"
+pytest-codeblocks = "^0.16.1"
 pytest-cov = "^4.0.0"
 types-pyyaml = "^6.0.12.10"
 types-tzlocal = "^5.0.1.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.pytest-watcher]
+now = true
+delay = 0.5
+runner = "pytest"
+runner_args = []
+patterns = ["*.py", "*.yaml", "Makefile", "pyproject.toml", "poetry.lock", "3210f808ac0467726439191eea3bd0a66ab261122ee55758367620fedc77fe08"]
+ignore_patterns = []
```

### Comparing `quiltcore-0.2.1/quiltcore/__init__.py` & `quiltcore-0.3.0/quiltcore/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,16 +20,21 @@
 - Entry
 
 These make use of the 'Config' class which loads and
 manages the 'quiltcore.yaml' configuration file.
 
 """
 
+from .builder import Builder  # noqa: F401
 from .changes import Changes  # noqa: F401
 from .delta import Delta  # noqa: F401
 from .entry import Entry  # noqa: F401
+from .header import Header  # noqa: F401
 from .manifest import Manifest  # noqa: F401
 from .namespace import Namespace  # noqa: F401
 from .registry import Registry  # noqa: F401
 from .resource import Resource  # noqa: F401
+from .table import Table  # noqa: F401
 from .volume import Volume  # noqa: F401
+from .yaml.codec import Codec, Dict3, Dict4, Hash3  # noqa: F401
 from .yaml.config import Config  # noqa: F401
+from .yaml.spec import Spec  # noqa: F401
```

### Comparing `quiltcore-0.2.1/quiltcore/changes.py` & `quiltcore-0.3.0/quiltcore/resource_key.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,109 @@
-from pathlib import Path
+from __future__ import annotations
 
-from upath import UPath
-from yaml import dump
+import logging
+from json import JSONEncoder
+from pathlib import Path
 
-from .delta import Delta
-from .manifest import Manifest
 from .resource import Resource
-from .resource_key import ResourceKey
+from .yaml.codec import Codec
 
 
-class Changes(ResourceKey):
+class ResourceKey(Resource):
     """
-    Track Changes to a new or existing Manifest
-    Add a file: put(path, action="add", key="filename.txt", prefix="./")
-    Use 'get' and 'list' to return the Deltas
-
-    Optional: track changes to a directory?
+    Get/List child resources by key in Manifest
     """
 
-    MANIFEST_FILE = "manifest.json"
-    MANIFEST_KEY = "manifest"
+    ENCODE = JSONEncoder(sort_keys=True, separators=(",", ":"), default=str).encode
 
-    @staticmethod
-    def ScratchFile() -> Path:
-        return Changes.TempDir(Changes.MANIFEST_FILE)
-
-    @staticmethod
-    def GetCache(path: Path) -> Path:
-        if not path:
-            return Changes.ScratchFile()
-        if path.exists() and path.is_dir():
-            return path / Changes.MANIFEST_FILE
-        return path
-
-    @staticmethod
-    def GetManifest(args: dict) -> Manifest:
-        if Changes.MANIFEST_KEY in args:
-            return args[Changes.MANIFEST_KEY]
-        path = Changes.ScratchFile()
-        return Manifest(path)
-
-    def __init__(self, path=None, **kwargs):
-        cache = Changes.GetCache(path)
-        super().__init__(cache, **kwargs)
-        self.keystore = {}
-
-    def __str__(self):
-        return dump(self.to_dict())
-
-    def to_dict(self):
-        return {k: v.to_dict() for k, v in self.keystore.items()}
-
-    #
-    # Mutating Changes
-    #
-
-    def post(self, key: str, **kwargs) -> Resource:
-        """
-                Create and track a Delta for this source Path.
-                Options:
-                * action: add [default], rm
-                * key: defaults to filename
-                * prefix: pre-pended to key if non-empty
-        .
-        """
-        path = UPath(key)
-        delta = Delta(path, **kwargs)
-        self.keystore[delta.name] = delta
-        return delta
-
-    def delete(self, key: str, **kwargs) -> None:
-        """Delete the key from this change set"""
-        if key in self.keystore:
-            del self.keystore[key]
-            return
-        raise KeyError(f"Key {key} not found in {self.keystore}")
+    def __init__(self, path: Path, **kwargs):
+        super().__init__(path, **kwargs)
+        self.codec = Codec()
+        self.headers = self.cf.get_dict("quilt3/headers")
 
     #
-    # ResourceKey helper methods
+    # Abstract Methods for child resources
     #
 
+    def _child_names(self, **kwargs) -> list[str]:
+        """Return names of each child resource."""
+        raise NotImplementedError
+
     def _child_dict(self, key: str) -> dict:
         """Return the dict for a child resource."""
-        delta = self.get_delta(key)
-        return {self.kName: [delta.name], self.kPlaces: str(delta.path)}
+        raise NotImplementedError
 
-    def get_delta(self, key: str, **kwargs) -> Delta:
-        """Return a Delta by key. Raise KeyError if not found."""
-        if key in self.keystore:
-            return self.keystore[key]
-        raise KeyError(f"Key {key} not found in {self.keystore}")
+    #
+    # Concrete Methods for child resources
+    #
 
     def key_path(self, key: str, args: dict = {}) -> Path:
         """Return the Path for a child resource."""
-        delta = self.get_delta(key)
-        return delta.path
+        return self.AsPath(args[self.cf.K_PLC])
 
-    def _child_names(self, **kwargs) -> list[str]:
-        """Return keys for each change."""
-        return list(self.keystore.keys())
+    def child(self, key: str, **kwargs):
+        """Return a child resource."""
+        args = self._child_dict(key)
+        path = self.key_path(key, args)
+        merged = {**self.args, **args}
+        self.CheckPath(path)
+        return self.klass(path, **merged)
+
+    #
+    # Hash creation
+    #
+
+    def digest(self, bstring: bytes) -> str:
+        """Return the multihash digest of `bstring`"""
+        return self.codec.digest(bstring)
+
+    def hash_quilt3(self) -> str:
+        """Return the hash of the source file."""
+        mh = self._hash_multihash()
+        hash_struct = self.codec.encode_hash(mh)
+        return hash_struct["value"]
+
+    def _hash_multihash(self) -> str:
+        raise NotImplementedError("subclass must override")
+
+    def _hash_path(self) -> str:
+        """Return the multihash of the source file."""
+        return self.digest(self.to_bytes())
+
+    def _hash_manifest(self) -> str:
+        hashable = b""
+        if hasattr(self, "head"):
+            self.head.hashable()  # type: ignore
+        for entry in self.list():
+            hashable += entry.hashable()  # type: ignore
+        return self.digest(hashable)
+
+    #
+    # Hash retreival
+    #
+
+    def to_hashable(self) -> dict:
+        raise NotImplementedError
+
+    def hashable(self) -> bytes:
+        source = self.to_hashable()
+        return self.ENCODE(source).encode("utf-8")  # type: ignore
+
+    def verify(self, bstring: bytes) -> bool:
+        """Verify that multihash digest of bytes match the multihash"""
+        digest = self.digest(bstring)
+        logging.debug(f"verify.digest: {digest}")
+        if not hasattr(self, self.KEY_MH):
+            raise ValueError("no hash found for {self}")
+        return digest == getattr(self, self.KEY_MH)
+
+    #
+    # Concrete HTTP Methods
+    #
+
+    def get(self, key: str, **kwargs) -> "Resource":
+        """Get a child resource by name."""
+        return self.child(key, **kwargs)
+
+    def list(self, **kwargs) -> list[Resource]:
+        """List all child resources by name."""
+        return [self.child(key, **kwargs) for key in self._child_names(**kwargs)]
```

### Comparing `quiltcore-0.2.1/quiltcore/manifest.py` & `quiltcore-0.3.0/quiltcore/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 import logging
 from pathlib import Path
 
 import pyarrow as pa  # type: ignore
-import pyarrow.compute as pc  # type: ignore
 import pyarrow.json as pj  # type: ignore
 
+from .header import Header
 from .resource_key import ResourceKey
+from .yaml.codec import Codec, Dict3, Dict4
 
 
-class Manifest(ResourceKey):
-    """
-    In-memory representation of a serialized package manifest.
-    list/get returns Entry with Path to the Place data actually lives
-    """
+class Table(ResourceKey):
+    """Abstract away calls to, and encoding of, pyarrow."""
 
     def __init__(self, path: Path, **kwargs):
+        """Read the manifest into a pyarrow Table."""
         super().__init__(path, **kwargs)
-        try:
-            self.body = self.setup_table()
-        except FileNotFoundError:
-            logging.warning(f"Manifest not found: {path}")
-
-    def hash(self) -> str:
-        return self.name
+        self.codec = Codec()
+        with self.path.open(mode="rb") as fi:
+            self.table = pj.read_json(fi)
+        self.head = self._get_head()
+        self.body = self._get_body()
 
     #
     # Parse Table
     #
 
-    def header_keys(self) -> list[str]:
-        headers = self.cf.get_dict("quilt3/headers")
-        return list(headers.keys())
+    def _get_head(self) -> pa.Table:
+        """Extract header values into attributes."""
+        first = self.table.take([0]).to_pylist()[0]
+        return Header(self.path, first=first)
 
-    def header_dict(self) -> dict:
-        return {k: getattr(self, k) for k in self.header_keys()}
-
-    def setup_table(self) -> pa.Table:
+    def _get_body(self) -> pa.Table:
         """
-        Read the manifest into a pyarrow Table.
         Extract header values into attributes.
         Return the Table without header row and columns
         """
-        with self.path.open(mode="rb") as fi:
-            self.table = pj.read_json(fi)
-        first = self.table.take([0]).to_pydict()
-        keys = self.header_keys()
-        for header in keys:
-            setattr(self, header, first[header][0])
-        return self.table.drop_columns(keys).slice(1)
+        body = self.head.drop(self.table)
+        return self.codec.decode_names(body)
 
     #
-    # Private Methods for child resources
+    # Query Table
     #
 
-    def _child_names(self, **kwargs) -> list[str]:
-        """List all child resources."""
-        names = self.body.column(self.kName).to_pylist()
-        return names
+    def names(self) -> list[str]:
+        if self.codec.name_col:
+            return self.codec.name_col.to_pylist()
+        return []
 
-    def _child_dict(self, key: str) -> dict:
+    def get_dict4(self, key: str) -> Dict4:
         """Return the dict for a child resource."""
         # TODO: cache to avoid continually re-calcluating
-        rows = self.body.filter(pc.field(self.kName) == key)
-        if rows.num_rows == 0:
-            raise KeyError(f"Key [{key}] not found in {self.kName} of {self.path}")
-        row = rows.to_pydict()
-        place = row[self.kPlaces][0][0]
-        row[self.KEY_PATH] = place
-        return row
+        index = self.codec.index_name(key).as_py()  # type: ignore
+        if index < 0:
+            raise ValueError(f"Key[{key}] not found in: {self.names()} ")
+        pa_list = self.body.take([index]).to_pylist()
+        pa_dict = pa_list[0]
+        del pa_dict[self.codec.K_NAM]
+
+        logging.debug(f"pa_dict: {pa_dict}")
+        pa_dict3 = Dict3(**pa_dict)
+        return self.codec.decode_dict(pa_dict3)
```

### Comparing `quiltcore-0.2.1/quiltcore/namespace.py` & `quiltcore-0.3.0/quiltcore/namespace.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 
 from .resource_path import ResourcePath
 
 
 class Namespace(ResourcePath):
     """
-    Namespacespace of Manifests by Hash
+    Namespace of Manifests by Hash
     list/get returns a specific Manifest
     """
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
-        self.manifests = kwargs["manifests"]
+        self.manifests = kwargs[self.KEY_MAN]
 
     def hash(self, tag: str = ResourcePath.TAG_DEFAULT) -> str:
         hash_file = self.path / tag
         return hash_file.read_text()
 
     def _child_path(self, key: str) -> Path:
         """Return the path for a child resource."""
```

### Comparing `quiltcore-0.2.1/quiltcore/registry.py` & `quiltcore-0.3.0/quiltcore/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,42 +8,47 @@
 class Registry(ResourcePath):
     """
     Top-level Resource reperesenting a Quilt Registry.
     Defines core paths containing Namespaces and Manifests.
     `list` and `get` return Namespace objects
     """
 
+    DIR_PREFIX = "quilt3/dirs/"
+
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         self.root = path
-        self.base = self.setup_dir(path, "quilt3/dirs/config")
-        self.path = self.setup_dir(self.base, "quilt3/dirs/names")
-        self.manifests = self.setup_dir(self.base, "quilt3/dirs/manifests")
+        self.base = self._setup_dir(path, "config")
+        self.path = self._setup_dir(self.base, "names")
+        self.manifests = self._setup_dir(self.base, "manifests")
+        self.stage = self._setup_dir(self.base, "stage")
 
-    def setup_dir(self, path: Path, key: str) -> Path:
+    def _setup_dir(self, path: Path, key: str) -> Path:
         """Form dir and create if it does not exist."""
-        dir = path / self.cf.get_path(key)
+
+        dir = path / self.cf.get_path(self.DIR_PREFIX + key)
         if not dir.exists():
             dir.mkdir(parents=True, exist_ok=True)
         return dir
 
     def _child_args(self, key: str) -> dict:
-        return {"manifests": self.manifests}
+        return {self.KEY_MAN: self.manifests}
 
     def put(self, res: Resource, **kwargs) -> "Resource":
         """Link manifest into namespace"""
         if not isinstance(res, Manifest):
             raise TypeError(f"Expected Manifest, got {type(res)}")
-        hash = res.hash()
-        name = kwargs[self.KEY_NAME]
+        hash = res.hash_quilt3()
+        name = kwargs[self.KEY_NS]
         name_dir = self.path / name
         name_dir.mkdir(parents=True, exist_ok=True)
 
-        tag = self.Timestamp()
+        tag = self.Now()
         tag_file = name_dir / tag
         tag_file.write_text(hash)
 
         latest_file = name_dir / self.TAG_DEFAULT
         latest_file.unlink(missing_ok=True)
         latest_file.write_text(hash)
 
+        res.args[self.KEY_TAG] = tag
         return res
```

### Comparing `quiltcore-0.2.1/quiltcore/resource.py` & `quiltcore-0.3.0/quiltcore/resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,152 @@
 from __future__ import annotations
 
+import logging
 from pathlib import Path
-from tempfile import TemporaryDirectory
+from re import compile
 from time import time
-from typing import Generator
-from urllib.parse import quote, unquote
+from urllib.parse import parse_qs, urlparse
 
 import quiltcore
 from upath import UPath
 
 from .yaml.config import Config
 
 
 class Resource:
     """
     Base class for all Quilt resources.
     Manages configuration and provides common methods.
     Subclasses override child* to customize get/list behavior
     """
 
-    DEFAULT_HASH_TYPE = "SHA256"
+    ARG_REG = "registry"
+    ARG_MAN = "manifest"
+    ARG_NS = "namespace"
+
+    KEY_FRC = "force"
     KEY_GLOB = "glob"
     KEY_KEY = "_key"
-    KEY_NAME = f"namespace.{KEY_KEY}"
+    KEY_HSH = "hash"
+    KEY_MAN = "_manifest"
+    KEY_META = "meta"
+    KEY_MH = "multihash"
+    KEY_MSG = "message"
+    KEY_NCP = "nocopy"
+    KEY_NS = f"{ARG_NS}.{KEY_KEY}"
     KEY_PATH = "_path"
-    MANIFEST = "_manifest"
-    TAG_DEFAULT = "latest"
-    UNQUOTED = "/:"
+    KEY_S3VER = "version_id"
+    KEY_SELF = "."
+    KEY_SZ = "size"
+    KEY_TAG = "tag"
+    KEY_USER = "user_meta"
+    KEY_UVER = "VersionId"
+    KEY_VER = "versionId"
 
-    @staticmethod
-    def TempGen(filename: str = "") -> Generator[Path, None, None]:
-        """Return generator to a temporary directory."""
-        with TemporaryDirectory() as tmpdirname:
-            temp_path = (
-                Path(tmpdirname) / filename if len(filename) > 0 else Path(tmpdirname)
-            )
-            yield temp_path
-
-    @staticmethod
-    def TempDir(filename: str = "") -> Path:
-        for path in Resource.TempGen(filename):
-            return path
-        return Path(".")  # should never happen
+    TAG_DEFAULT = "latest"
+    IS_LOCAL = compile(r"file:\/*")
+    IS_REL = "./"
+    IS_URI = ":/"
 
     @staticmethod
     def ClassFromName(name: str) -> type:
         """Return a class from a string."""
         return getattr(quiltcore, name)
 
     @staticmethod
-    def Timestamp() -> str:
+    def Now() -> str:
         "Return integer timestamp."
         return str(int(time()))
 
+    @classmethod
+    def AsPath(cls, key: str) -> Path:
+        """Return a Path from a string."""
+        if not isinstance(key, str):
+            raise TypeError(f"[{key}]Expected str, got {type(key)}")
+        return UPath(key, version_aware=True)
+
+    @classmethod
+    def CheckPath(cls, path) -> Path:
+        if not isinstance(path, Path):
+            raise TypeError(f"[{path}]Expected Path, got {type(path)}")
+        return path
+
+    @classmethod
+    def GetVersion(cls, uri: str) -> str:
+        """Extract `versionId` from URI query string."""
+        query = urlparse(uri).query
+        if not query:
+            return ""
+        qs = parse_qs(query)
+        vlist = qs.get(Resource.KEY_VER)
+        return vlist[0] if vlist else ""
+
+    @classmethod
+    def FromURI(cls, uri: str) -> "Resource":
+        path = cls.AsPath(uri)
+        ver = cls.GetVersion(uri)
+        opts = {cls.KEY_VER: ver} if len(ver) > 0 else {}
+        return cls(path, **opts)
+
     def __init__(self, path: Path, **kwargs):
-        self.path = path
+        self.path = self.CheckPath(path)
         self.args = kwargs
         self.name = path.name
         self.class_name = self.__class__.__name__
         self.class_key = self.class_name.lower()
         self.args[self.class_key] = self
         key = kwargs.get(self.KEY_KEY, None)
         if key is not None:
             self.args[f"{self.class_key}.{self.KEY_KEY}"] = key
         self.cf = Config()
-        self.setup_params()
+        self._setup_params()
 
     def __repr__(self):
         return f"<{self.class_name}({self.path}, {self.args})>"
 
     def __str__(self):
         return f"<{self.class_name}({self.path})>"
 
     def __eq__(self, other):
         return str(self) == str(other)
 
     def param(self, key: str, default: str) -> str:
         """Return a param."""
         return self.params[key] if key in self.params else default  # type: ignore
 
-    def setup_params(self):
+    def _setup_params(self):
         """Load Resource-specific params from config file."""
         self.params = self.cf.get_dict(f"resources/{self.class_name}")
         self.glob = self.param("glob", "*")
         _child = self.param("child", "Resource")
         self.klass = Resource.ClassFromName(_child)
 
     #
-    # URL Encoding of Physical Keys
+    # Read Bytes/Text
     #
 
-    def encoded(self) -> bool:
-        """Return True if Resource keys should be encoded."""
-        return self.cf.get_bool("quilt3/urlencode")
-
-    def encode(self, path: Path) -> str:
-        """Encode path as a string."""
-        key = str(path)
-        return quote(key, safe=self.UNQUOTED) if self.encoded() else key
-
-    def decode(self, key: str) -> Path:
-        """Decode string into a Path."""
-        if not self.encoded():
-            return UPath(key)
-        decoded = unquote(key)
-        return UPath(decoded)
+    def read_opts(self) -> dict:
+        if self.KEY_VER in self.args:
+            opts = {self.KEY_S3VER: self.args[self.KEY_VER]}
+            logging.debug(f"read_opts: {opts}")
+            return opts
+        return {}
+
+    def to_bytes(self) -> bytes:
+        """Return bytes from path."""
+        opts = self.read_opts()
+        if len(opts) > 0:
+            with self.path.open(mode="rb", **opts) as fi:
+                return fi.read()
+        return self.path.read_bytes()
+
+    def to_text(self, strip=True) -> str:
+        """Return text from path."""
+        text = self.to_bytes().decode("utf-8")
+        return text.strip() if strip else text
 
     #
     # Abstract HTTP Methods
     #
 
     def list(self, **kwargs) -> list["Resource"]:
         """List all child resources."""
@@ -118,18 +156,14 @@
         """Get a child resource by key."""
         return self
 
     def patch(self, res: Resource, **kwargs) -> "Resource":
         """Update and return a child resource."""
         raise NotImplementedError
 
-    def post(self, key: str, **kwargs) -> "Resource":
-        """Create and return a child resource using key."""
-        raise NotImplementedError
-
     def put(self, res: Resource, **kwargs) -> "Resource":
         """Insert/Replace and return a child resource."""
         raise NotImplementedError
 
     def delete(self, key: str, **kwargs) -> None:
         """Delete a child resource by name."""
         raise NotImplementedError
```

### Comparing `quiltcore-0.2.1/quiltcore/resource_key.py` & `quiltcore-0.3.0/quiltcore/resource_path.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,54 @@
 from __future__ import annotations
 
 from pathlib import Path
 
-from upath import UPath
-
 from .resource import Resource
 
 
-class ResourceKey(Resource):
+class ResourcePath(Resource):
     """
-    Get/List child resources by key in Manifest
+    Path-based list and get.
     """
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
-        self.defaultHash = self.cf.get_str("quilt3/hash_type", self.DEFAULT_HASH_TYPE)
-        self.kHash = self.cf.get_str("quilt3/hash", "hash")
-        self.kMeta = self.cf.get_str("quilt3/meta", "meta")
-        self.kName = self.cf.get_str("quilt3/name", "logical_key")
-        self.kPlaces = self.cf.get_str("quilt3/places", "physical_keys")
-        self.kSize = self.cf.get_str("quilt3/size", "size")
+        self.glob = self.param(self.KEY_GLOB, "*")
 
     #
-    # Abstract Methods for child resources
+    # Private Methods for Path-based child resources
     #
 
-    def _child_names(self, **kwargs) -> list[str]:
-        """Return names of each child resource."""
-        return []
-
-    def _child_dict(self, key: str) -> dict:
-        """Return the dict for a child resource."""
+    def _child_args(self, key: str) -> dict:
+        """Return the kwargs for a child resource."""
         return {}
 
-    #
-    # Concrete Methods for child resources
-    #
-
-    def key_path(self, key: str, args: dict = {}) -> Path:
-        """Return the Path for a child resource."""
-        if self.KEY_PATH not in args:
-            raise KeyError(f"Missing {self.KEY_PATH} in {args.keys()}")
-        place = args[self.KEY_PATH]
-        self.decode(place)
-        return UPath(place)
-
-    def child(self, key: str, **kwargs):
+    def child(self, path: Path, key: str = ""):
         """Return a child resource."""
-        args = self._child_dict(key)
-        path = self.key_path(key, args)
+        args = self._child_args(key)
+        args[self.KEY_KEY] = key
         merged = {**self.args, **args}
+        self.CheckPath(path)
         return self.klass(path, **merged)
 
+    def _child_path(self, key: str) -> Path:
+        """Return the path for a child resource."""
+        return self.path / key
+
+    def _child_list(self) -> list[Path]:
+        """List/generator of valid child paths; defaults to self.glob"""
+        return sorted(self.path.glob(self.glob))
+
     #
-    # Concrete HTTP Methods
+    # Public HTTP-like Methods
     #
 
+    def list(self, **kwargs) -> list["Resource"]:
+        """List all child resources."""
+        return [self.child(x) for x in self._child_list()]
+
     def get(self, key: str, **kwargs) -> "Resource":
         """Get a child resource by name."""
-        return self.child(key, **kwargs)
-
-    def list(self, **kwargs) -> list[Resource]:
-        """List all child resources by name."""
-        return [self.child(key, **kwargs) for key in self._child_names(**kwargs)]
+        path = self._child_path(key)
+        if not path.exists():
+            raise KeyError(f"Key {key} not found in {self.path}")
+        return self.child(path, key)
```

### Comparing `quiltcore-0.2.1/quiltcore/volume.py` & `quiltcore-0.3.0/quiltcore/volume.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,177 @@
+import logging
 from pathlib import Path
 
-import pyarrow as pa  # type: ignore
-from jsonlines import Writer
-from upath import UPath
-
-from .entry import Entry
 from .manifest import Manifest
+from .namespace import Namespace
 from .registry import Registry
 from .resource import Resource
 from .resource_key import ResourceKey
 
 
 class Volume(ResourceKey):
     """
     Top-level Resource reperesenting a logical unit of storage
     with a single type of filesystem or blob storage
     and its own Registry
     """
 
     ERR_REQUIRE_REGISTRY = "Volume.get requires registry keyword argument"
-    KEY_MH = "multihash"
-    KEY_HSH = "hash"
-    KEY_TAG = "tag"
-    KEY_SELF = "."
-    MH_PREFIX = Entry.MH_PREFIX["SHA256"]
 
     @staticmethod
     def FromURI(uri: str, **kwargs) -> "Volume":
         """Create a Volume from a URI"""
-        path = UPath(uri)
+        path = Volume.AsPath(uri)
         return Volume(path, **kwargs)
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         self.registry = Registry(path, **self.args)
-        self.uri = self.path.as_uri()
-        self.keystore: dict[str, dict] = {
+        self.uri = str(self.path)
+        self.pkgcache: dict[str, dict] = {
             self.KEY_SELF: self.args,
         }
 
+    #
+    # Helper Methods
+    #
+
     def is_local(self) -> bool:
-        return self.uri.startswith("file://")
+        return self.uri.startswith("file://") or "://" not in self.uri
 
     def _child_names(self, **kwargs) -> list[str]:
         """Return names of each child resource."""
-        names = list(self.keystore.keys())
+        names = list(self.pkgcache.keys())
         names.remove(self.KEY_SELF)
-        return names
+        return [n.split(":")[0].split("@")[0] for n in names]
+
+    def _man_path(self, hash: str) -> Path:
+        """Return path to a manifest"""
+        return self.registry.manifests / hash
+
+    def _stage_path(self, hash: str) -> Path:
+        """Return path to a manifest"""
+        return self.registry.stage / hash
 
     #
-    # List/Delete vs keystore
+    # List/Delete vs keycache
     #
 
     def delete(self, key: str, **kwargs) -> None:
-        """Delete the key from this keystore"""
-        if key in self.keystore:
-            del self.keystore[key]
-            return
-        raise KeyError(f"Key {key} not found in {self.keystore.keys()}")
+        """Delete the key from this keycache"""
+        for pkg in self.pkgcache:
+            if key in pkg:
+                del self.pkgcache[pkg]
+                logging.debug(f"Deleted {pkg} from {self.pkgcache.keys()}")
+                return
+        raise KeyError(f"Key {key} not found in {self.pkgcache.keys()}")
 
     def list(self, **kwargs) -> list["Resource"]:
         """List all child resources."""
         return [self.get(x) for x in self._child_names()]
 
     #
     # GET and helpers - return a Manfiest
     #
 
     def get(self, key: str, **kwargs) -> "Resource":
         """
-        Return and keystore manifest for Namespace `key`
+        Return and keycache manifest for Namespace `key`
 
         * hash
         * multihash
         * tag [default: latest]
         """
-        if key in self.keystore:
-            opts = self.keystore[key]
-            print(f"Volume.get({key}) opts: {opts.keys()}")
+        pkg = self.get_pkg_name(key, **kwargs)
+        if pkg in self.pkgcache:
+            opts = self.pkgcache[pkg]
             return opts["manifest"]
 
         manifest = self.get_manifest(key, **kwargs)
         args = manifest.args.copy()
         args[self.KEY_PATH] = manifest.path
-        self.keystore[key] = args
+        self.pkgcache[pkg] = args
         return manifest
 
+    def read_manifest(self, hash: str) -> Manifest:
+        """Read a manifest from the registry"""
+        paths = [self._stage_path(hash), self._man_path(hash)]
+        for path in paths:
+            if path.exists():
+                return Manifest(path, **self.args)
+        raise FileNotFoundError(f"Manifest not found: {hash}\n\tin: {paths}")
+
+    def get_pkg_name(self, key: str, **kwargs) -> str:
+        opts: dict[str, str] = kwargs
+        hash = opts.get(self.KEY_HSH, "")
+        tag = opts.get(self.KEY_TAG, self.TAG_DEFAULT)
+        if hash:
+            return f"{key}@{hash}"
+        if tag:
+            return f"{key}:{tag}"
+        return key
+
     def get_manifest(self, key: str, **kwargs) -> "Resource":
         """
-        Create manifest for Namespace `key` and `kwargs`
+        Get or Create manifest for Namespace `key` and `kwargs`
         """
         opts: dict[str, str] = kwargs
-        hash = self.get_hash(opts)
-        if len(hash) > 0:
-            return Manifest(self.registry.manifests / hash, **self.args)
-
+        hash = opts.get(self.KEY_HSH, "")
         tag = opts.get(self.KEY_TAG, self.TAG_DEFAULT)
-        name = self.registry.get(key)
-        return name.get(tag)
-
-    def get_hash(self, opts: dict[str, str]) -> str:
-        if self.KEY_HSH in opts:
-            return opts[self.KEY_HSH]
-        if self.KEY_MH in opts:
-            mh = opts[self.KEY_MH]
-            return mh.strip(self.MH_PREFIX)
-        return ""
+        if len(hash) == 0:
+            name = self.registry.get(key)
+            if not isinstance(name, Namespace):
+                raise TypeError(f"Volume.get requires a Namespace, not {type(name)}")
+            hash = name.hash(tag)
+            name.get(tag)
+        return self.read_manifest(hash)
 
     #
     # PUT and helpers - upload a Manfiest or other resource
     #
-    # - PUT Entry: copies individual file onto Volume
+    # - PUT Entry: copies individual file onto Volume (TBD)
     # - PUT Manifest:
     #   - copies necessary Entries onto Volume (unless --nocopy and non-local)
     #   - calculates hash and creates Namespaced folders
     #   - copies Manifest onto Volume
+    #
+    #  OPTS:
+    #  - namespace_key="PKG/NAME": namespace to register manifest
+    #  - force=True: overwrite any existing manifest
+    #  - nocopy=True: do not copy any files onto new Volume (just copy manifest)
 
     def put(self, res: Resource, **kwargs) -> "Resource":
         """Insert/Replace and return a child resource."""
+        logging.debug(f"Volume.put: {res} [{kwargs}]]")
         if not isinstance(res, Manifest):
             raise TypeError(f"Volume.put requires a Manifest, not {type(res)}")
         man: Manifest = res
-        hash_path = self.registry.manifests / man.hash()
-        if hash_path.exists():
-            raise FileExistsError(f"Manifest {hash_path} already exists")
+        hash = man.hash_quilt3()
+        stage_path = self._stage_path(hash)
+        Manifest.WriteToPath(man.head, man.list(), stage_path)  # type: ignore
+
+        new_path = self._man_path(hash)
+        if new_path.exists() and not kwargs.get(self.KEY_FRC, False):
+            raise FileExistsError(f"Manifest {new_path} already exists")
 
         ns_name = (
-            kwargs.get(self.KEY_NAME)
-            or man.args.get(self.KEY_NAME)
-            or f"unknown/{self.Timestamp()}"
+            kwargs.get(self.KEY_NS)
+            or man.args.get(self.KEY_NS)
+            or f"unknown/{self.Now()}"
         )
-        kwargs[self.KEY_NAME] = ns_name
-
-        ns_name = self.write_entries(man, hash_path, ns_name)
-        man2 = Manifest(hash_path, **self.args)
-        self.registry.put(man2, **kwargs)
-        return man2
+        kwargs[self.KEY_NS] = ns_name
+        if self.KEY_META in kwargs:
+            man.head.user_meta = kwargs[self.KEY_META]
+        if self.KEY_MSG in kwargs:
+            man.head.message = kwargs[self.KEY_MSG]
+
+        if not kwargs.get(self.KEY_NCP, False):
+            man = self.translate_manifest(man, new_path, ns_name)
+        self.registry.put(man, **kwargs)
+        return man
 
-    def write_entries(self, man: Manifest, path: Path, name: str) -> str:
+    def translate_manifest(self, man: ResourceKey, path: Path, name: str) -> Manifest:
+        """Translate entries from manifest into this Volume"""
         dest = str(self.path / name)
         entries = [entry.get(dest) for entry in man.list()]
-        rows = [entry.to_row() for entry in entries]  # type: ignore
-        table = pa.Table.from_pylist(rows)
-        with path.open(mode="wb") as fo:
-            with Writer(fo) as writer:
-                writer.write(man.header_dict())
-                writer.write(table.to_pydict())
-        return name
+        Manifest.WriteToPath(man.head, entries, path)  # type: ignore
+        return Manifest(path, **self.args)
```

### Comparing `quiltcore-0.2.1/quiltcore/yaml/config.py` & `quiltcore-0.3.0/quiltcore/yaml/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from pathlib import Path
-
 from un_yaml import UnYaml  # type: ignore
+from upath import UPath
 
 
 class Config(UnYaml):
     CONFIG_FILE = "quiltcore.yaml"
+    K_MAP = "map"
+    K_NAM = "name"
+    K_PLC = "place"
+    K_HSH = "hash"
 
     @classmethod
     def DefaultConfig(cls) -> dict:
         return UnYaml.LoadYaml(cls.CONFIG_FILE, __package__)
 
     def __init__(self, yaml_data: dict = {}) -> None:
-        data = yaml_data if len(yaml_data) > 0 else Config.DefaultConfig()
+        data = yaml_data if len(yaml_data) > 0 else self.DefaultConfig()
         super().__init__(data)
 
     def get_str(self, key: str, default="") -> str:
         return super().get(key) or default
 
-    def get_path(self, key: str) -> Path:
+    def get_path(self, key: str) -> UPath:
         str_path = self.get_str(key, ".")
-        return Path(str_path)
+        return UPath(str_path)
 
     def get_bool(self, key: str) -> bool:
         return self.get(key) or False
 
     def get_dict(self, key: str) -> dict:
         return self.get(key) or {}
```

### Comparing `quiltcore-0.2.1/quiltcore/yaml/quiltcore.yaml` & `quiltcore-0.3.0/quiltcore/yaml/quiltcore.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -2,45 +2,72 @@
 _yaml:
   _version: 0.3.1
   app: quiltcore
   app_version: 0.2.0
   doc: quilt3
   doc_version: 0.2.0
 multihash:
-  SHA256: sha2-256
+  prefix:
+    SHA256: "1220"
+  digest:
+    SHA256: sha2-256
 resources:
   Volume:
     child: Manifest
   Registry:
     child: Namespace
     glob: "*/*"
   Namespace:
     child: Manifest
     glob: "*"
   Manifest:
     child: Entry
-  Changes:
-    child: Entry
   Delta:
     child: Entry
+  Changes:
+    child: Delta
+  Builder:
+    child: Entry
 quilt3:
-  columns:
-    logical_key: string
-    physical_keys: [string]
-    size: int64
-    hash:
-      type: string
-      value: string
-    meta: struct
   dirs:
     config: .quilt
     names: named_packages
     manifests: packages
+    stage: remotes
+  format:
+    datetime: "%Y-%m-%d"
   hash_type: SHA256
-  hash: hash
   headers:
-    version: string
-    message: string
+    version: v0
+    message: commit message
+    user_meta: {}
+  map:
+    name: logical_key
   mime_type: application/ld+json
-  name: logical_key
-  places: physical_keys
-  urlencode: True
+  schema:
+    logical_key:
+      format: path
+      is_quoted: false
+      name: name
+      type: str
+    physical_keys:
+      format: uri
+      is_list: true
+      is_quoted: true
+      name: place
+      type: str
+    size:
+      name: size
+      type: int64
+    hash:
+      format:
+        type: string
+        value: string
+      is_hash: true
+      name: multihash
+      type: struct
+    meta:
+      name: metadata
+      type: struct
+      format:
+        user_meta: struct
+      is_optional: true
```

### Comparing `quiltcore-0.2.1/PKG-INFO` & `quiltcore-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: quiltcore
-Version: 0.2.1
+Version: 0.3.0
 Summary: low-level plubming to read/write Quilt packages
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
+Requires-Dist: jsonlines (==1.2.0)
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
-Requires-Dist: pytest-codeblocks (>=0.16.1,<0.17.0)
+Requires-Dist: quilt3 (>=5.3.1,<6.0.0)
 Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
 Requires-Dist: un-yaml (>=0.3.1)
-Requires-Dist: universal-pathlib (>=0.0.23,<0.0.24)
+Requires-Dist: universal-pathlib (>=0.0.24,<0.0.25)
 Description-Content-Type: text/markdown
 
 # QuiltCore
 
 QuiltCore is a library for building and running [Quilt](https://quiltdata.com) data packages.
 It is designed to leverage standard open source technology and YAML configuration files
 so that it can easily be ported to other languages and platforms.
@@ -66,17 +66,17 @@
 entry = manifest.get(TEST_KEY)
 ```
 
 ### Get Object
 
 <!--pytest-codeblocks:cont-->
 ```python
-with TemporaryDirectory() as tmpdirname:
-  dest = UPath(tmpdirname)
+with TemporaryDirectory() as tmpdir:
+  dest = UPath(tmpdir)
   outfile = dest / TEST_KEY
-  entry.get(dest)
+  entry.get(tmpdir)
   print(outfile.resolve())
   assert outfile.exists()
   local_bytes = outfile.read_bytes()
   assert entry.verify(local_bytes)
 ```
```

