# Comparing `tmp/snap_saas_base-0.5.0.tar.gz` & `tmp/snap_saas_base-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snap_saas_base-0.5.0.tar", max compression
+gzip compressed data, was "snap_saas_base-0.6.0.tar", max compression
```

## Comparing `snap_saas_base-0.5.0.tar` & `snap_saas_base-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4822 2023-07-21 15:42:20.738427 snap_saas_base-0.5.0/README.md
--rw-r--r--   0        0        0     4202 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/__init__.py
--rw-r--r--   0        0        0       30 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/__init__.py
--rw-r--r--   0        0        0     2153 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/base_model.py
--rw-r--r--   0        0        0     5740 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/organization.py
--rw-r--r--   0        0        0     3361 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/user.py
--rw-r--r--   0        0        0     6632 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/models/workspace.py
--rw-r--r--   0        0        0        0 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/py.typed
--rw-r--r--   0        0        0       38 2023-07-21 15:42:20.746428 snap_saas_base-0.5.0/src/snap_saas_base/schemas/__init__.py
--rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 snap_saas_base-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4822 2023-07-28 15:19:11.051797 snap_saas_base-0.6.0/README.md
+-rw-r--r--   0        0        0     4208 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/models/__init__.py
+-rw-r--r--   0        0        0     2156 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/models/base_model.py
+-rw-r--r--   0        0        0     5745 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/models/organization.py
+-rw-r--r--   0        0        0     3364 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/models/user.py
+-rw-r--r--   0        0        0     6639 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/models/workspace.py
+-rw-r--r--   0        0        0        0 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/py.typed
+-rw-r--r--   0        0        0       38 2023-07-28 15:19:11.055797 snap_saas_base-0.6.0/src/snap_saas_base/schemas/__init__.py
+-rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 snap_saas_base-0.6.0/PKG-INFO
```

### Comparing `snap_saas_base-0.5.0/README.md` & `snap_saas_base-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.5.0/pyproject.toml` & `snap_saas_base-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "snap-saas-base"
-version = "0.5.0"
+version = "0.6.0"
 description = "Snap Env (https://snapenv.com) Python base module."
 authors = ["Abner G Jacobsen <abner@apoana.com.br>"]
 readme = "README.md"
 repository = "https://github.com/orgs/snapenv/snap-saas-base"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "0.5.0"
+version = "0.6.0"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.11,<4.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.18"}
-cuid = "^0.4"
 pydantic = ">=1.0.0,<2.0.0"
+uuid6 = "^2023.5.2"
 
 [tool.poetry.group.test.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 black = ">=23.3.0"
 commitizen = ">=3.2.1"
 coverage = { extras = ["toml"], version = ">=7.2.5" }
 mypy = ">=1.2.0"
 poethepoet = ">=0.20.0"
```

### Comparing `snap_saas_base-0.5.0/src/snap_saas_base/models/base_model.py` & `snap_saas_base-0.6.0/src/snap_saas_base/models/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
-import cuid
 import sqlalchemy as sa
 import sqlalchemy.orm as so
+import uuid6
 
 db_naming_convention = {
     "ix": "ix_%(column_0_label)s",
     "uq": "uq_%(table_name)s_%(column_0_N_name)s",
     "ck": "ck_%(table_name)s_%(constraint_name)s",
     "fk": "fk_%(table_name)s_%(column_0_N_name)s_%(referred_table_name)s",
     "pk": "pk_%(table_name)s",
@@ -37,15 +37,15 @@
         The `created_at` and `updated_at` attributes use the `datetime.utcnow` function to generate timestamps.
         The `updated_at` attribute is also updated every time the instance is updated.
     """
 
     __abstract__ = True
     metadata: sa.MetaData = sa.MetaData(naming_convention=db_naming_convention)  # type: ignore
 
-    id: so.Mapped[str] = so.mapped_column(nullable=False, default=cuid.cuid, primary_key=True)
+    id: so.Mapped[str] = so.mapped_column(nullable=False, default=uuid6.uuid7, primary_key=True)
     created_at: so.Mapped[datetime] = so.mapped_column(
         sa.DateTime(timezone=False),
         nullable=False,
         default=datetime.utcnow,
         # server_default=func.now(),
     )
     updated_at: so.Mapped[datetime] = so.mapped_column(
```

### Comparing `snap_saas_base-0.5.0/src/snap_saas_base/models/organization.py` & `snap_saas_base-0.6.0/src/snap_saas_base/models/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import cuid
 import sqlalchemy as sa
 import sqlalchemy.orm as so
+import uuid6
 
 from snap_saas_base.models.base_model import AbstractModel
 
 # https://github.com/sqlalchemy/sqlalchemy/discussions/6165
 
 
 class Organization(AbstractModel):
@@ -68,15 +68,15 @@
         dict
             A dictionary where the keys are the column names and the values are the corresponding attribute values of the Organization instance.
         """
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
 
     def __init__(self, *args, **kwargs):
         if "id" not in kwargs:
-            kwargs["id"] = cuid.cuid()
+            kwargs["id"] = uuid6.uuid7()
         super().__init__(*args, **kwargs)
 
 
 class OrgMember(AbstractModel):
     """A class used to represent an Organization Member in a database.
 
     This class is a mapping to the "organizations_members" table in the database. It contains
@@ -138,9 +138,9 @@
         dict
             a dictionary representing the object
         """
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
 
     def __init__(self, *args, **kwargs):
         if "id" not in kwargs:
-            kwargs["id"] = cuid.cuid()
+            kwargs["id"] = uuid6.uuid7()
         super().__init__(*args, **kwargs)
```

### Comparing `snap_saas_base-0.5.0/src/snap_saas_base/models/user.py` & `snap_saas_base-0.6.0/src/snap_saas_base/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import cuid
 import sqlalchemy as sa
 import sqlalchemy.orm as so
+import uuid6
 
 from snap_saas_base.models.base_model import AbstractModel
 
 # https://github.com/sqlalchemy/sqlalchemy/discussions/6165
 
 
 class User(AbstractModel):
@@ -79,9 +79,9 @@
         dict
             a dictionary containing the user's attributes
         """
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
 
     def __init__(self, *args, **kwargs):
         if "id" not in kwargs:
-            kwargs["id"] = cuid.cuid()
+            kwargs["id"] = uuid6.uuid7()
         super().__init__(*args, **kwargs)
```

### Comparing `snap_saas_base-0.5.0/src/snap_saas_base/models/workspace.py` & `snap_saas_base-0.6.0/src/snap_saas_base/models/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import cuid
 import sqlalchemy as sa
 import sqlalchemy.orm as so
+import uuid6
 from sqlalchemy.dialects.postgresql import JSONB
 
 from snap_saas_base.models.base_model import AbstractModel
 
 # https://github.com/sqlalchemy/sqlalchemy/discussions/6165
 
 
@@ -58,15 +58,15 @@
         dict
             A dictionary representation of the workspace.
         """
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
 
     def __init__(self, *args, **kwargs):
         if "id" not in kwargs:
-            kwargs["id"] = cuid.cuid()
+            kwargs["id"] = uuid6.uuid7()
         super().__init__(*args, **kwargs)
 
 
 class WorkspaceMember(AbstractModel):
     """A class used to represent a member in a workspace.
 
     This class is a model for the table "workspaces_members" in the database. It contains the workspace_id, member_id and role
@@ -120,15 +120,15 @@
         dict
             A dictionary where the keys are the column names and the values are the corresponding attributes of the object.
         """
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
 
     def __init__(self, *args, **kwargs):
         if "id" not in kwargs:
-            kwargs["id"] = cuid.cuid()
+            kwargs["id"] = uuid6.uuid7()
         super().__init__(*args, **kwargs)
 
 
 class WorkspaceKv(AbstractModel):
     """A class used to represent the Workspace Key-Value pair model.
 
     This class is a subclass of the AbstractModel and is used to map the
@@ -176,9 +176,9 @@
             A dictionary where the keys are the column names and the values
             are the corresponding attribute values from the WorkspaceKv object.
         """
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
 
     def __init__(self, *args, **kwargs):
         if "id" not in kwargs:
-            kwargs["id"] = cuid.cuid()
+            kwargs["id"] = uuid6.uuid7()
         super().__init__(*args, **kwargs)
```

### Comparing `snap_saas_base-0.5.0/PKG-INFO` & `snap_saas_base-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: snap-saas-base
-Version: 0.5.0
+Version: 0.6.0
 Summary: Snap Env (https://snapenv.com) Python base module.
 Home-page: https://github.com/orgs/snapenv/snap-saas-base
 Author: Abner G Jacobsen
 Author-email: abner@apoana.com.br
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cuid (>=0.4,<0.5)
 Requires-Dist: pydantic (>=1.0.0,<2.0.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.18,<3.0.0)
+Requires-Dist: uuid6 (>=2023.5.2,<2024.0.0)
 Project-URL: Repository, https://github.com/orgs/snapenv/snap-saas-base
 Description-Content-Type: text/markdown
 
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/orgs/snapenv/snap-saas-base)
 
 # Snap SAAS Base
```

