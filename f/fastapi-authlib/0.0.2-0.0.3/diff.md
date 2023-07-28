# Comparing `tmp/fastapi_authlib-0.0.2.tar.gz` & `tmp/fastapi_authlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_authlib-0.0.2.tar", max compression
+gzip compressed data, was "fastapi_authlib-0.0.3.tar", max compression
```

## Comparing `fastapi_authlib-0.0.2.tar` & `fastapi_authlib-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     1097 2023-05-25 09:49:48.758784 fastapi_authlib-0.0.2/LICENSE
--rw-r--r--   0        0        0     1809 2023-05-26 08:06:01.388930 fastapi_authlib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3702 2023-05-26 02:36:13.115572 fastapi_authlib-0.0.2/README.md
--rw-r--r--   0        0        0       36 2023-05-26 08:06:01.426754 fastapi_authlib-0.0.2/src/fastapi_authlib/__init__.py
--rw-r--r--   0        0        0     3313 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/alembic.ini
--rw-r--r--   0        0        0     2794 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/env.py
--rw-r--r--   0        0        0       38 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/README
--rw-r--r--   0        0        0      534 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/script.py.mako
--rw-r--r--   0        0        0     3390 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py
--rw-r--r--   0        0        0      356 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.2/src/fastapi_authlib/config/__init__.py
--rw-r--r--   0        0        0       11 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.2/src/fastapi_authlib/config/settings.yml
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.2/src/fastapi_authlib/messages/__init__.py
--rw-r--r--   0        0        0      219 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.2/src/fastapi_authlib/messages/base.py
--rw-r--r--   0        0        0      236 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.2/src/fastapi_authlib/messages/user.py
--rw-r--r--   0        0        0     2906 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.2/src/fastapi_authlib/models.py
--rw-r--r--   0        0        0     3268 2023-05-26 08:06:03.392694 fastapi_authlib-0.0.2/src/fastapi_authlib/oidc.py
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/__init__.py
--rw-r--r--   0        0        0     5767 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/base.py
--rw-r--r--   0        0        0      825 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/group.py
--rw-r--r--   0        0        0     1177 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/group_user_map.py
--rw-r--r--   0        0        0     1121 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/session.py
--rw-r--r--   0        0        0      365 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/user.py
--rw-r--r--   0        0        0       23 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/__init__.py
--rw-r--r--   0        0        0      799 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/exception_handlers.py
--rw-r--r--   0        0        0       13 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/__init__.py
--rw-r--r--   0        0        0      906 2023-05-26 02:01:54.573018 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/login.py
--rw-r--r--   0        0        0      559 2023-05-25 09:49:48.770784 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/logout.py
--rw-r--r--   0        0        0      499 2023-05-25 09:49:48.770784 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/user.py
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/__init__.py
--rw-r--r--   0        0        0      385 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/base.py
--rw-r--r--   0        0        0      504 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/group.py
--rw-r--r--   0        0        0      597 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/group_user_map.py
--rw-r--r--   0        0        0     1011 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/session.py
--rw-r--r--   0        0        0      684 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/user.py
--rw-r--r--   0        0        0      102 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.2/src/fastapi_authlib/services/__init__.py
--rw-r--r--   0        0        0     9167 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.2/src/fastapi_authlib/services/auth.py
--rw-r--r--   0        0        0     3882 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.2/src/fastapi_authlib/services/base.py
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.774785 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/__init__.py
--rw-r--r--   0        0        0     1095 2023-05-26 02:32:44.712026 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/check_user_depend.py
--rw-r--r--   0        0        0      870 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/exceptions.py
--rw-r--r--   0        0        0      439 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/types.py
--rw-r--r--   0        0        0     5066 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.2/setup.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-25 09:49:48.758784 fastapi_authlib-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1903 2023-07-28 05:33:24.612437 fastapi_authlib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3676 2023-07-28 06:34:50.084730 fastapi_authlib-0.0.3/README.md
+-rw-r--r--   0        0        0       36 2023-07-27 03:17:45.034283 fastapi_authlib-0.0.3/src/fastapi_authlib/__init__.py
+-rw-r--r--   0        0        0     3313 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/alembic.ini
+-rw-r--r--   0        0        0     2794 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/env.py
+-rw-r--r--   0        0        0       38 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/README
+-rw-r--r--   0        0        0      534 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/script.py.mako
+-rw-r--r--   0        0        0     3390 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py
+-rw-r--r--   0        0        0      298 2023-07-28 05:55:20.666180 fastapi_authlib-0.0.3/src/fastapi_authlib/config/__init__.py
+-rw-r--r--   0        0        0      245 2023-07-28 06:01:24.727932 fastapi_authlib-0.0.3/src/fastapi_authlib/config/settings.yml
+-rw-r--r--   0        0        0       15 2023-07-28 06:53:47.009372 fastapi_authlib-0.0.3/src/fastapi_authlib/messages/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.3/src/fastapi_authlib/messages/base.py
+-rw-r--r--   0        0        0      236 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.3/src/fastapi_authlib/messages/user.py
+-rw-r--r--   0        0        0     2906 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.3/src/fastapi_authlib/models.py
+-rw-r--r--   0        0        0     3542 2023-07-28 06:06:00.028011 fastapi_authlib-0.0.3/src/fastapi_authlib/oidc.py
+-rw-r--r--   0        0        0       17 2023-07-28 06:53:46.941374 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/__init__.py
+-rw-r--r--   0        0        0     5347 2023-07-28 06:53:46.989373 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/base.py
+-rw-r--r--   0        0        0      767 2023-07-28 06:53:47.054373 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/group.py
+-rw-r--r--   0        0        0      953 2023-07-28 03:20:37.301648 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/group_user_map.py
+-rw-r--r--   0        0        0     1121 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/session.py
+-rw-r--r--   0        0        0      751 2023-07-28 06:53:47.075778 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/user.py
+-rw-r--r--   0        0        0       23 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/__init__.py
+-rw-r--r--   0        0        0      799 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/exception_handlers.py
+-rw-r--r--   0        0        0       13 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/__init__.py
+-rw-r--r--   0        0        0     1126 2023-07-28 06:54:58.918918 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/login.py
+-rw-r--r--   0        0        0      621 2023-07-26 03:57:56.924608 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/logout.py
+-rw-r--r--   0        0        0      489 2023-07-28 03:20:21.991250 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/user.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/base.py
+-rw-r--r--   0        0        0      504 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/group.py
+-rw-r--r--   0        0        0      597 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/group_user_map.py
+-rw-r--r--   0        0        0     1011 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/session.py
+-rw-r--r--   0        0        0      684 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/user.py
+-rw-r--r--   0        0        0      102 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3/src/fastapi_authlib/services/__init__.py
+-rw-r--r--   0        0        0     9737 2023-07-28 06:53:46.967373 fastapi_authlib-0.0.3/src/fastapi_authlib/services/auth.py
+-rw-r--r--   0        0        0     3882 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.3/src/fastapi_authlib/services/base.py
+-rw-r--r--   0        0        0     1291 2023-07-27 06:02:26.732846 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/__init__.py
+-rw-r--r--   0        0        0     2535 2023-07-28 03:19:26.550076 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/auth_dependency.py
+-rw-r--r--   0        0        0      870 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/exceptions.py
+-rw-r--r--   0        0        0      425 2023-07-28 06:41:28.199278 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/types.py
+-rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.3/PKG-INFO
```

### Comparing `fastapi_authlib-0.0.2/LICENSE` & `fastapi_authlib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/pyproject.toml` & `fastapi_authlib-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-authlib"
-version = "0.0.2"
+version = "0.0.3"
 description = "A fastapi authlib authentication library"
 readme = "README.md"
 authors = ["qiang.xie <qiang.xie@zncdata.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
@@ -19,14 +19,15 @@
 itsdangerous = "^2.1.2"
 httpx = "^0.24.0"
 sqlalchemy = "1.4.46"
 inflection = "^0.5.1"
 fastapi-sa = "^0.1.0"
 alembic = "^1.10.3"
 aiomysql = "^0.1.1"
+pyjwt = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.14.5"
 isort = "^5.10.1"
 pytest = "^7.1.2"
 mkdocs = "^1.3.1"
 mkdocs-material = "^8.4.1"
@@ -40,14 +41,19 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = "tests"
 python_files = ["tests.py", "test_*.py", "*_tests.py"]
 log_cli = true
+filterwarnings = [
+    "error",
+    "ignore::sqlalchemy.exc.MovedIn20Warning",
+    "ignore::DeprecationWarning",
+]
 
 [tool.pylint.main]
 disable = [
     "too-many-instance-attributes",
     "broad-except",
     "too-few-public-methods",
     "unused-argument",
@@ -78,16 +84,14 @@
 ]
 
 [tool.pylint.MASTER]
 load-plugins = ["pylint_pytest"]
 ignore-paths = [
     "src/fastapi_authlib/alembic",
     "src/fastapi_authlib/.local",
-    ".*/demo.py",
-    "tests/data.py"
 ]
 
 [tool.pylint.design]
 max-line-length = 120
 max-args = 11
 max-attributes = 10
 min-public-methods = 1
```

### Comparing `fastapi_authlib-0.0.2/README.md` & `fastapi_authlib-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,126 +1,138 @@
-# fastapi-authlib
-
-fastapi-authlib provides easy integration between FastAPI and openid connection in your application.
-Provides the initialization and dependencies of oidc, aiming to unify authentication management and
-reduce the difficulty of use.
-
-## Installing
-
-install and update using pip:
-
-```shell
-pip install fastapi-authlib
-```
-
-## Examples
-
-### Create settings for examples, `settings.py`
-
-```python
-config = {
-    'database': 'sqlite+aiosqlite:////tmp/oidc_demo.db',
-    'oauth_client_id': 'client_id',
-    'oauth_client_secret': 'client_secret',
-    'oauth_conf_url': 'conf_url',
-    'session_secret': 'secret_key',
-    'router_prefix': '',
-}
-```
-
-settings.py is a simple configuration file of the use case, which mainly provides the database link,
-the necessary parameters used by oidc, the session authentication key and the routing prefix.
-
-Please use your authentication server configuration to populate the parameter value prefixed with oauth.
-Other parameters can be modified according to the actual situation.
-
-### Create api route, `api_router.py`
-
-```python
-from fastapi import APIRouter
-from starlette.requests import Request
-
-router = APIRouter()
-
-
-@router.get('/index')
-async def index(
-        *,
-        request: Request,
-):
-    """
-    User
-    """
-    user_info = request.state.user
-    return {'name': user_info.get('user_name')}
-```
-
-For authenticated api, you can use `request.state.user` to get the current user.
-
-### Create oidc demo entry, `main.py`
-
-```python
-"""main"""
-import uvicorn
-from fastapi import Depends, FastAPI
-from fastapi_sa.database import db
-from fastapi_sa.middleware import DBSessionMiddleware
-
-from fastapi_authlib.oidc import OIDCClient
-from fastapi_authlib.utils.check_user_depend import check_auth_session
-from api_router import index
-from .settings import config
-
-
-class OIDCDemo:
-    """OIDCDemo"""
-
-    def __init__(self, settings: dict):
-        self.settings = settings
-        self.router_prefix = self.settings.get('router_prefix')
-
-    def run(self):
-        """Run"""
-        # Early environment initialization
-        app = FastAPI(title='FastAPIOIDCSupportDemo', version='0.1.0')
-        db.init(self.settings.get('database'))
-
-        # Oidc environment initialization
-        client = OIDCClient(
-            app=app,
-            **config
-        )
-        # If you only init app, you should use init_app() instead
-        client.init_oidc()
-
-        # Customize the environment initialization
-        # add dependencies to the interface that needs to be authenticated
-        app.include_router(index.router, tags=['index'], prefix=config.get('router_prefix'),
-                           dependencies=[Depends(check_auth_session)])
-        app.add_middleware(DBSessionMiddleware)
-        return app
-
-
-if __name__ == '__main__':
-    client_app = OIDCDemo(config).run()
-    uvicorn.run(client_app, host="0.0.0.0", port=8001)
-
-```
-
-### Use Step
-
-- Create app and init db
-- Init the environment of oidc, If you don't want to do data migration, you should use init_app method.
-  Usually database migration and oidc initialization are performed together
-- Register routing and other middleware, the DBSessionMiddleware is required
-- Start a fastapi server with uvicorn or other
-
-## Based on
-
-- [FastAPI](https://github.com/tiangolo/fastapi)
-- [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy)
-- [Fastapi-sa](https://github.com/whg517/fastapi-sa)
-- [Authlib](https://github.com/lepture/authlib)
-
-## Develop
-
-You may need to read the [develop document](./docs/development.md) to use SRC Layout in your IDE.
+# fastapi-authlib
+
+fastapi-authlib provides easy integration between FastAPI and openid connection in your application.
+Provides the initialization and dependencies of oidc, aiming to unify authentication management and
+reduce the difficulty of use.
+
+## Installing
+
+install and update using pip:
+
+```shell
+pip install fastapi-authlib
+```
+
+## Examples
+
+### Create settings for examples, `settings.py`
+
+```python
+config = {
+    'database': 'sqlite+aiosqlite:////tmp/oidc_demo.db',
+    'oauth_client_id': 'client_id',
+    'oauth_client_secret': 'client_secret',
+    'oauth_conf_url': 'conf_url',
+    'secret_key': 'secret_key',
+    'router_prefix': '',
+}
+```
+
+settings.py is a simple configuration file of the use case, which mainly provides the database link,
+the necessary parameters used by oidc, the session authentication key and the routing prefix.
+
+Please use your authentication server configuration to populate the parameter value prefixed with oauth.
+Other parameters can be modified according to the actual situation.
+
+### Create api route, `api_router.py`
+
+```python
+from fastapi import APIRouter
+from starlette.requests import Request
+
+router = APIRouter()
+
+
+@router.get('/index')
+async def index(
+        *,
+        request: Request,
+):
+    """
+    User
+    """
+    user_info = request.state.user
+    return {'name': user_info.get('user_name')}
+```
+
+For authenticated api, you can use `request.state.user` to get the current user.
+
+### Create oidc demo entry, `main.py`
+
+```python
+"""main"""
+import uvicorn
+from fastapi import Depends, FastAPI
+from fastapi_sa.database import db
+from fastapi_sa.middleware import DBSessionMiddleware
+
+from fastapi_authlib.oidc import OIDCClient
+from fastapi_authlib.utils.auth_dependency import check_auth_depends
+from api_router import index
+from .settings import config
+
+
+class OIDCDemo:
+    """OIDCDemo"""
+
+    def __init__(self, settings: dict):
+        self.settings = settings
+        self.router_prefix = self.settings.get('router_prefix')
+
+    def run(self):
+        """Run"""
+        # Early environment initialization
+        app = FastAPI(title='FastAPIOIDCSupportDemo', version='0.1.0')
+        db.init(self.settings.get('database'))
+
+        # Oidc environment initialization
+        client = OIDCClient(
+            app=app,
+            **config
+        )
+        # If you only init app, you should use init_app() instead
+        client.init_oidc()
+
+        # Customize the environment initialization
+        # add dependencies to the interface that needs to be authenticated
+        app.include_router(
+            index.router,
+            tags=['index'],
+            prefix=config.get('router_prefix'),
+            dependencies=[Depends(check_auth_depends)]
+        )
+        app.add_middleware(DBSessionMiddleware)
+        return app
+
+
+if __name__ == '__main__':
+    client_app = OIDCDemo(config).run()
+    uvicorn.run(client_app, host="0.0.0.0", port=8001)
+
+```
+
+### Use Step
+
+- Create app and init db
+- Init the environment of oidc, If you don't want to do data migration, you should use init_app method.
+  Usually database migration and oidc initialization are performed together
+- Register routing and other middleware, the DBSessionMiddleware is required
+- Start a fastapi server with uvicorn or other
+
+### Other
+
+Provide the following apis
+- /login
+- /auth
+- /logout
+- /users
+
+## Based on
+
+- [FastAPI](https://github.com/tiangolo/fastapi)
+- [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy)
+- [Fastapi-sa](https://github.com/whg517/fastapi-sa)
+- [Authlib](https://github.com/lepture/authlib)
+
+## Develop
+
+You may need to read the [develop document](./docs/development.md) to use SRC Layout in your IDE.
```

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/alembic.ini` & `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/env.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/script.py.mako` & `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/models.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/oidc.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/oidc.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,55 +6,71 @@
 from alembic.config import Config
 from fastapi import Depends, FastAPI
 from starlette.middleware.sessions import SessionMiddleware
 
 from fastapi_authlib.config import settings
 from fastapi_authlib.rest_api.handler import init_exception_handler
 from fastapi_authlib.rest_api.routers import login, logout, user
-from fastapi_authlib.utils.check_user_depend import check_auth_session
+from fastapi_authlib.utils.auth_dependency import check_auth_depends
 
 
 class OIDCClient:
     """OIDC"""
 
-    def __init__(self, app: FastAPI, oauth_client_id: str, oauth_client_secret: str, oauth_conf_url: str,
-                 database: str, session_secret: str, router_prefix: str = '', **kwargs):
+    def __init__(
+        self,
+        app: FastAPI,
+        oauth_client_id: str,
+        oauth_client_secret: str,
+        oauth_conf_url: str,
+        database: str,
+        secret_key: str,
+        algorithm: str = 'HS256',
+        platform: str = 'default',
+        router_prefix: str = '',
+        exp_period: int = 30,
+        nts_period: int = 10,
+    ) -> None:
         """
         Init OIDC basic configuration
-        :param app:
-        :param oauth_client_id:
+        :param app: fastapi object
+        :param oauth_client_id: oidc client id
         :param oauth_client_secret:
         :param oauth_conf_url:
         :param database:
-        :param session_secret:
+        :param secret_key: jwt secret key
+        :param algorithm: jwt algorithm, default: HS256
+        :param platform:
         :param router_prefix:
-        :param kwargs:
+        :param exp_period: jwt token expiration duration, unit: day
+        :param nts_period: jwt token refresh duration: unit: minute
         """
-        if database:
-            settings.set('DATABASE', database)
-        else:
-            raise TypeError('Database parameter is required parameter')
-
-        if all([oauth_client_id, oauth_client_secret, oauth_conf_url]):
-            settings.set('OAUTH_CLIENT_ID', oauth_client_id)
-            settings.set('OAUTH_CLIENT_SECRET', oauth_client_secret)
-            settings.set('OAUTH_CONF_URL', oauth_conf_url)
-        else:
-            raise TypeError('Missed Oauth parameters, it is required parameters')
-
-        if app:
-            self.app = app
-        else:
-            raise TypeError('App parameter is required parameter')
-
-        if session_secret:
-            self.session_secret = session_secret
-        else:
-            raise TypeError('Session secret is required parameter')
 
+        if not database:
+            raise TypeError('Missing Database parameters, it is required')
+
+        if not all([oauth_client_id, oauth_client_secret, oauth_conf_url]):
+            raise TypeError('Missing Oauth parameters, it is required')
+
+        if not app:
+            raise TypeError('Missing App parameters, it is required')
+
+        if not secret_key:
+            raise TypeError('Missing SECRET_KEY parameters, it is required')
+
+        settings.DATABASE = database
+        settings.OAUTH_CLIENT_ID = oauth_client_id
+        settings.OAUTH_CLIENT_SECRET = oauth_client_secret
+        settings.OAUTH_CONF_URL = oauth_conf_url
+        settings.SECRET_KEY = secret_key
+        settings.PLATFORM = platform
+        settings.ALGORITHM = algorithm
+        settings.EXP_PERIOD = exp_period
+        settings.NTS_PERIOD = nts_period
+        self.app = app
         self.route_prefix = router_prefix
 
     @staticmethod
     def migrate_db():
         """
         Migrates the database
         :return:
@@ -64,32 +80,37 @@
         command.upgrade(alembic_cfg, 'head')
 
     def init_app(self):
         """
         Init app
         :return:
         """
-        # init middleware
-        self.app.add_middleware(SessionMiddleware,
-                                secret_key=self.session_secret,
-                                session_cookie='session_id',
-                                max_age=60 * 60 * 4,
-                                )
-
         # init handle
         init_exception_handler(self.app)
 
         # init route
-        self.app.include_router(login.router, tags=['login'], prefix=self.route_prefix)
-        self.app.include_router(logout.router,
-                                tags=['logout'],
-                                prefix=self.route_prefix,
-                                dependencies=[Depends(check_auth_session)]
-                                )
-        self.app.include_router(user.router, tags=['user'], prefix=self.route_prefix,
-                                dependencies=[Depends(check_auth_session)])
+        self.app.include_router(
+            login.router,
+            tags=['login'],
+            prefix=self.route_prefix
+        )
+
+        self.app.include_router(
+            logout.router,
+            tags=['logout'],
+            prefix=self.route_prefix,
+            dependencies=[Depends(check_auth_depends)]
+        )
+        self.app.include_router(
+            user.router,
+            tags=['user'],
+            prefix=self.route_prefix,
+            dependencies=[Depends(check_auth_depends)]
+        )
+
+        self.app.add_middleware(SessionMiddleware, secret_key=settings.SECRET_KEY)
 
     def init_oidc(self):
         """Init oidc"""
         thread = threading.Thread(target=self.migrate_db)
         thread.start()
         self.init_app()
```

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/repository/group.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/repository/group.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-"""Group"""
-from sqlalchemy import select
-
-from fastapi_authlib.models import Group
-from fastapi_authlib.repository.base import BaseRepository
-from fastapi_authlib.schemas.group import GroupCreate, GroupSchema, GroupUpdate
-from fastapi_authlib.utils.exceptions import ObjectDoesNotExist
-
-
-class GroupRepository(BaseRepository[Group, GroupCreate, GroupUpdate, GroupSchema]):
-    """
-    Group repository
-    """
-    model = Group
-    model_schema = GroupSchema
-
-    async def get_by_name(self, name: str) -> GroupSchema:
-        """Get by name"""
-        stmt = select(Group).filter(Group.name == name)
-        group: Group = await self.session.scalar(stmt)
-        if not group:
-            # Task does not exist
-            raise ObjectDoesNotExist()
-        return self.model_schema.from_orm(group)
+"""Group"""
+from sqlalchemy import select
+
+from fastapi_authlib.models import Group
+from fastapi_authlib.repository.base import BaseRepository
+from fastapi_authlib.schemas.group import GroupCreate, GroupSchema, GroupUpdate
+from fastapi_authlib.utils.exceptions import ObjectDoesNotExist
+
+
+class GroupRepository(BaseRepository[Group, GroupCreate, GroupUpdate, GroupSchema]):
+    """
+    Group repository
+    """
+    model = Group
+    model_schema = GroupSchema
+
+    async def get_by_name(self, name: str) -> GroupSchema:
+        """Get by name"""
+        stmt = select(Group).filter(Group.name == name)
+        group: Group = await self.session.scalar(stmt)
+        if not group:
+            raise ObjectDoesNotExist()
+        return self.model_schema.from_orm(group)
```

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/repository/session.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/repository/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/__init__.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/exception_handlers.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/group_user_map.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/group_user_map.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/session.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/user.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/services/auth.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/services/auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,218 +1,276 @@
-"""auth"""
-import logging
-from datetime import datetime, timedelta
-
-from authlib.integrations.base_client.errors import (OAuthError,
-                                                     TokenExpiredError)
-from authlib.integrations.starlette_client import OAuth
-from starlette.requests import Request
-
-from fastapi_authlib.config import settings
-from fastapi_authlib.models import User
-from fastapi_authlib.repository.group import GroupRepository
-from fastapi_authlib.repository.group_user_map import GroupUserMapRepository
-from fastapi_authlib.repository.session import SessionRepository
-from fastapi_authlib.repository.user import UserRepository
-from fastapi_authlib.schemas.group import GroupCreate
-from fastapi_authlib.schemas.group_user_map import GroupUserMapCreate
-from fastapi_authlib.schemas.session import SessionCreate, SessionUpdate
-from fastapi_authlib.schemas.user import UserCreate, UserSchema, UserUpdate
-from fastapi_authlib.services.base import EntityService
-from fastapi_authlib.utils.exceptions import (AuthenticationError,
-                                              ObjectDoesNotExist, OIDCError)
-
-logger = logging.getLogger(__name__)
-
-
-class AuthService(EntityService[User, UserCreate, UserUpdate, UserSchema]):
-    """
-    Auth service.
-    """
-    REPOSITORY_CLASS = UserRepository
-
-    @property
-    def session_repository(self):
-        """Session repository"""
-        return SessionRepository()
-
-    @property
-    def group_repository(self):
-        """Group repository"""
-        return GroupRepository()
-
-    @property
-    def group_user_map_repository(self):
-        """Group user map repository"""
-        return GroupUserMapRepository()
-
-    def __init__(self):
-        self.oauth_client = OAuth(settings)
-        self.register_oauth()
-
-    def register_oauth(self):
-        """Register OAuth"""
-        self.oauth_client.register(
-            name='oauth',
-            server_metadata_url=settings.OAUTH_CONF_URL,
-            client_kwargs={
-                'scope': 'openid email profile',
-                'verify': False
-            })
-
-    async def login(self, request: Request, redirect_uri: str, **_):
-        """
-        Login
-        :param request:
-        :param redirect_uri:
-        :param _:
-        :return:
-        """
-        return await self.oauth_client.oauth.authorize_redirect(request, redirect_uri)
-
-    async def logout(self, user_id: int, **_):
-        """
-        Logout
-        :param user_id:
-        :param _:
-        :return:
-        """
-        # 清除数据库中的对应数据
-        try:
-            await self.clear_token_info(pk=user_id)
-        except ObjectDoesNotExist:
-            logger.warning('User does not exist')
-
-    async def auth(self, request: Request, **_) -> dict:
-        """
-        Auth
-        :param request:
-        :param _:
-        :return:
-        """
-        # 进行认证处理, 认证的同时已经获取到了userinfo
-        try:
-            token = await self.oauth_client.oauth.authorize_access_token(request)
-        except OAuthError as ex:
-            logger.error('OAuth Error, exception info: %s', ex)
-            raise OIDCError('OAuth Error') from ex
-        userinfo = token.get('userinfo')
-
-        # 使用email作为后端唯一性判断指标
-        try:
-            users = await self.repository.get(search_fields={'email': userinfo.email})
-            user_id = users[0].id
-            active = users[0].active
-            user_obj_in = UserUpdate(name=userinfo.name,
-                                     nickname=userinfo.nickname,
-                                     picture=userinfo.picture,
-                                     active=True)
-            user = await self.repository.update_by_id(pk=user_id, obj_in=user_obj_in)
-            # session表中无user_id对应数据，如有，直接删除
-            if active:
-                # 删除
-                session = await self.session_repository.get_session_from_user_id(user_id)
-                await self.session_repository.delete_by_id(session.id)
-
-        except ObjectDoesNotExist:
-            # 使用email作为后端唯一性判断指标
-            user_obj_in = UserCreate(name=userinfo.name,
-                                     nickname=userinfo.nickname,
-                                     email=userinfo.email,
-                                     email_verified=userinfo.email_verified,
-                                     picture=userinfo.picture,
-                                     active=True,
-                                     )
-            user = await self.repository.create(obj_in=user_obj_in)
-        session_obj_in = SessionCreate(user_id=user.id, platform_name='gitlab', **token)
-        await self.session_repository.create(obj_in=session_obj_in)
-        groups = userinfo.get('groups_direct')
-        await self.save_group_and_group_user_map(groups, user)
-        exp = (datetime.now() + timedelta(hours=3)).timestamp()
-        return {'user_id': user.id, 'user_name': user.name, 'email': user.email, 'exp': int(exp)}
-
-    async def update_token(self, user_id: int) -> bool:
-        """Check token"""
-
-        # 进行user的获取
-        # 通过user_id获取对应的id, 进而获取 oauth_token的信息进行刷新操作
-        try:
-            session = await self.session_repository.get_session_from_user_id(user_id=user_id)
-        except ObjectDoesNotExist:
-            return False
-        try:
-            token = await self.oauth_client.oauth.fetch_access_token(refresh_token=session.refresh_token,
-                                                                     grant_type='refresh_token')
-            # 刷新成功后保存token信息
-            await self.session_repository.update_by_id(pk=session.id,
-                                                       obj_in=SessionUpdate(**token))
-        except TokenExpiredError as ex:
-            logger.warning('Failed to refresh token, exception info: %s', ex)
-            # 清除token相关信息
-            await self.clear_token_info(pk=user_id)
-            return False
-        return True
-
-    async def user(self, user_id: int, **_) -> UserSchema:
-        """User"""
-        # 单独获取userinfo数据
-        # access_token的默认过期时间为3小时
-        # 根据user交换获取 access_token
-        user = await self.repository.get_by_id(user_id)
-        if not user.active:
-            raise AuthenticationError()
-        try:
-            session = await self.session_repository.get_session_from_user_id(user_id)
-            userinfo = await self.oauth_client.oauth.userinfo(token={'access_token': session.access_token})
-            user_obj_in = UserUpdate(name=userinfo.name,
-                                     nickname=userinfo.nickname,
-                                     picture=userinfo.picture)
-            await self.repository.update_by_id(pk=user_id, obj_in=user_obj_in)
-            await self.save_group_and_group_user_map(groups=userinfo.get('groups'), user=user)
-            return user
-        except Exception as ex:
-            logger.warning('Get userinfo error, exception info: %s', ex)
-            await self.clear_token_info(pk=user_id)
-            raise AuthenticationError() from ex
-
-    async def clear_token_info(self, pk: int, **_):
-        """
-        Clear token info
-        :param pk:
-        :param _:
-        :return:
-        """
-
-        # 1. 清除 Session表中关于pk对应的user_id数据
-        await self.clear_session_with_user_id(user_id=pk)
-        # 2. 清除 User表中active字段进行False
-        await self.repository.update_by_id(pk=pk, obj_in=UserUpdate(active=False))
-
-    async def clear_session_with_user_id(self, user_id: int):
-        """
-        Clear session with user id
-        :param user_id:
-        :return:
-        """
-        try:
-            session = await self.session_repository.get_session_from_user_id(user_id=user_id)
-            return await self.session_repository.delete_by_id(session.id)
-        except ObjectDoesNotExist:
-            logger.warning('Session does not exist')
-
-    async def save_group_and_group_user_map(self, groups: list, user: UserSchema):
-        """Save group and group user map"""
-        # 判断group是否已经保存
-        for name in groups:
-            try:
-                group = await self.group_repository.get_by_name(name=name)
-            except ObjectDoesNotExist:
-                # 插入
-                group = await self.group_repository.create(obj_in=GroupCreate(name=name))
-
-            # group user map表逻辑处理
-            try:
-                await self.group_user_map_repository.get_by_group_and_user_id(group_id=group.id,
-                                                                              user_id=user.id)
-            except ObjectDoesNotExist:
-                await self.group_user_map_repository.create(
-                    obj_in=GroupUserMapCreate(group_id=group.id, user_id=user.id))
+"""auth"""
+import logging
+
+from authlib.integrations.base_client.errors import OAuthError
+from authlib.integrations.starlette_client import OAuth
+from starlette.requests import Request
+
+from fastapi_authlib.config import settings
+from fastapi_authlib.models import User
+from fastapi_authlib.repository.group import GroupRepository
+from fastapi_authlib.repository.group_user_map import GroupUserMapRepository
+from fastapi_authlib.repository.session import SessionRepository
+from fastapi_authlib.repository.user import UserRepository
+from fastapi_authlib.schemas.group import GroupCreate
+from fastapi_authlib.schemas.group_user_map import GroupUserMapCreate
+from fastapi_authlib.schemas.session import SessionCreate, SessionUpdate
+from fastapi_authlib.schemas.user import UserCreate, UserSchema, UserUpdate
+from fastapi_authlib.services.base import EntityService
+from fastapi_authlib.utils import get_utc_timestamp
+from fastapi_authlib.utils.exceptions import (AuthenticationError,
+                                              ObjectDoesNotExist, OIDCError)
+
+logger = logging.getLogger(__name__)
+oauth_client = OAuth(settings)
+
+
+class AuthService(EntityService[User, UserCreate, UserUpdate, UserSchema]):
+    """
+    Auth service.
+    """
+    REPOSITORY_CLASS = UserRepository
+    exp_period = settings.EXP_PERIOD
+    nts_period = settings.NTS_PERIOD
+
+    def __init__(self):
+        self.oauth_client = oauth_client
+        self.register_oauth()
+
+    @property
+    def session_repository(self):
+        """Session repository"""
+        return SessionRepository()
+
+    @property
+    def group_repository(self):
+        """Group repository"""
+        return GroupRepository()
+
+    @property
+    def group_user_map_repository(self):
+        """Group user map repository"""
+        return GroupUserMapRepository()
+
+    def register_oauth(self):
+        """Register OAuth"""
+        self.oauth_client.register(
+            name='oauth',
+            server_metadata_url=settings.OAUTH_CONF_URL,
+            client_kwargs={
+                'scope': 'openid email profile',
+                'verify': False
+            }
+        )
+
+    async def login(self, request: Request, redirect_uri: str):
+        """
+        Login
+        :param request:
+        :param redirect_uri:
+        :return:
+        """
+        return await self.oauth_client.oauth.authorize_redirect(request, redirect_uri)
+
+    async def logout(self, user_id: int):
+        """
+        Logout
+        :param user_id:
+        :return:
+        """
+        # 清除数据库中的对应数据
+        try:
+            await self.clear_token_info(pk=user_id)
+        except ObjectDoesNotExist:
+            logger.warning('User does not exist')
+
+    async def auth(self, request: Request, **_) -> dict:
+        """
+        Auth
+        :param request:
+        :param _:
+        :return:
+        """
+        try:
+            token = await self.oauth_client.oauth.authorize_access_token(request)
+        except OAuthError as ex:
+            logger.error('OAuth Error, exception info: %s', ex)
+            raise OIDCError('OAuth Error') from ex
+        userinfo = token.get('userinfo')
+
+        # the email is unique
+        try:
+            user = await self.repository.get_by_email(userinfo.email)
+            active = user.active
+            user_obj_in = UserUpdate(
+                name=userinfo.name,
+                nickname=userinfo.nickname,
+                picture=userinfo.picture,
+                active=True
+            )
+            user = await self.repository.update_by_id(pk=user.id, obj_in=user_obj_in)
+            if active:
+                session = await self.session_repository.get_session_from_user_id(user.id)
+                await self.session_repository.delete_by_id(session.id)
+
+        except ObjectDoesNotExist:
+            user_obj_in = UserCreate(
+                name=userinfo.name,
+                nickname=userinfo.nickname,
+                email=userinfo.email,
+                email_verified=userinfo.email_verified,
+                picture=userinfo.picture,
+                active=True,
+            )
+            user = await self.repository.create(obj_in=user_obj_in)
+
+        session_obj_in = SessionCreate(user_id=user.id, platform_name=settings.PLATFORM, **token)
+        await self.session_repository.create(obj_in=session_obj_in)
+        groups = userinfo.get('groups_direct')
+        await self.save_group_and_group_user_map(groups, user)
+
+        payload = self.format_payload(user)
+        return payload
+
+    async def get_user_by_id(self, pk: int) -> UserSchema:
+        """
+        Get user by id
+        :param pk:
+        :return:
+        """
+        user = await self.repository.get_by_id(pk)
+        if not user.active:
+            raise AuthenticationError()
+        return user
+
+    async def clear_token_info(self, pk: int):
+        """
+        Clear token info
+        :param pk:
+        :return:
+        """
+
+        await self.clear_session_with_user_id(pk=pk)
+        await self.repository.update_by_id(
+            pk=pk,
+            obj_in=UserUpdate(active=False)
+        )
+
+    async def clear_session_with_user_id(self, pk: int):
+        """
+        Clear session with user id
+        :param pk:
+        :return:
+        """
+        try:
+            session = await self.session_repository.get_session_from_user_id(user_id=pk)
+            return await self.session_repository.delete_by_id(session.id)
+        except ObjectDoesNotExist:
+            logger.warning('Session does not exist')
+
+    async def save_group_and_group_user_map(self, groups: list, user: UserSchema) -> None:
+        """
+        Save group and group user map
+        :param groups: group names
+        :param user:
+        :return:
+        """
+        group_ids = []
+        for name in groups:
+            try:
+                group = await self.group_repository.get_by_name(name=name)
+            except ObjectDoesNotExist:
+                group = await self.group_repository.create(obj_in=GroupCreate(name=name))
+            group_ids.append(group.id)
+
+        try:
+            exist_groups = await self.group_user_map_repository.get_by_user_id(user_id=user.id)
+            # compare id
+            exist_group_ids = [group.group_id for group in exist_groups]
+            exist_group_map = {str(group.group_id): group.id for group in exist_groups}
+            # delete id
+            delete_ids = set(exist_group_ids) - set(group_ids)
+            for group_id in delete_ids:
+                await self.group_user_map_repository.delete_by_id(exist_group_map.get(str(group_id)))
+
+            # insert id
+            insert_ids = set(group_ids) - set(exist_group_ids)
+            for group_id in insert_ids:
+                await self.group_user_map_repository.create(
+                    obj_in=GroupUserMapCreate(
+                        group_id=group_id,
+                        user_id=user.id
+                    )
+                )
+
+        except ObjectDoesNotExist:
+            for group_id in group_ids:
+                await self.group_user_map_repository.create(
+                    obj_in=GroupUserMapCreate(
+                        group_id=group_id,
+                        user_id=user.id
+                    )
+                )
+
+    async def verify_user(self, pk: int) -> dict:
+        """
+        Verify user
+        :param pk: user id
+        :return:
+        """
+        # check user active
+        user = await self.repository.get_by_id(pk)
+        if not user.active:
+            raise AuthenticationError()
+
+        session = await self.session_repository.get_session_from_user_id(pk)
+        # check token
+        try:
+            userinfo = await self.oauth_client.oauth.userinfo(token={'access_token': session.access_token})
+        except Exception as ex:
+            logger.warning(
+                'Get userinfo with access_token of user %s error, try use refresh token, exception info: %s',
+                pk,
+                ex
+            )
+            try:
+                # check refresh_token
+                access_token = await self.oauth_client.oauth.fetch_access_token(
+                    refresh_token=session.refresh_token,
+                    grant_type='refresh_token'
+                )
+            except Exception as ex:
+                logger.warning('Get access_token with refresh_token of user %s error', pk)
+                await self.clear_token_info(pk=pk)
+                raise AuthenticationError('Token expired error') from ex
+
+            userinfo = await self.oauth_client.oauth.userinfo(token={'access_token': access_token})
+            # save token
+            await self.session_repository.update_by_id(
+                pk=session.id,
+                obj_in=SessionUpdate(**access_token)
+            )
+        # compare user and userinfo
+        update_fields = {key: userinfo.get(key)
+                         for key in ['name', 'nickname', 'picture']
+                         if getattr(user, key) != userinfo.get(key)}
+        if update_fields:
+            user_obj_in = UserUpdate(**update_fields)
+            user = await self.repository.update_by_id(pk=pk, obj_in=user_obj_in)
+
+        # compare group map
+        await self.save_group_and_group_user_map(groups=userinfo.get('groups'), user=user)
+
+        payload = self.format_payload(user)
+        return payload
+
+    def format_payload(self, user: UserSchema) -> dict:
+        """
+        Format payload with user
+        :param user:
+        :return:
+        """
+
+        iat = get_utc_timestamp()
+        exp = get_utc_timestamp(days=self.exp_period)
+        nst = get_utc_timestamp(minutes=self.nts_period)
+        return {'user_id': user.id, 'user_name': user.name, 'email': user.email, 'iat': iat, 'exp': exp, 'nst': nst}
```

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/services/base.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/services/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/src/fastapi_authlib/utils/exceptions.py` & `fastapi_authlib-0.0.3/src/fastapi_authlib/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.2/setup.py` & `fastapi_authlib-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,166 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-authlib
+Version: 0.0.3
+Summary: A fastapi authlib authentication library
+License: MIT
+Author: qiang.xie
+Author-email: qiang.xie@zncdata.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
+Requires-Dist: alembic (>=1.10.3,<2.0.0)
+Requires-Dist: authlib (>=1.2.0,<2.0.0)
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: fastapi-sa (>=0.1.0,<0.2.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: inflection (>=0.5.1,<0.6.0)
+Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
+Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
+Requires-Dist: sqlalchemy (==1.4.46)
+Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
+Description-Content-Type: text/markdown
+
+# fastapi-authlib
+
+fastapi-authlib provides easy integration between FastAPI and openid connection in your application.
+Provides the initialization and dependencies of oidc, aiming to unify authentication management and
+reduce the difficulty of use.
+
+## Installing
+
+install and update using pip:
+
+```shell
+pip install fastapi-authlib
+```
+
+## Examples
+
+### Create settings for examples, `settings.py`
+
+```python
+config = {
+    'database': 'sqlite+aiosqlite:////tmp/oidc_demo.db',
+    'oauth_client_id': 'client_id',
+    'oauth_client_secret': 'client_secret',
+    'oauth_conf_url': 'conf_url',
+    'secret_key': 'secret_key',
+    'router_prefix': '',
+}
+```
 
-package_dir = \
-{'': 'src'}
+settings.py is a simple configuration file of the use case, which mainly provides the database link,
+the necessary parameters used by oidc, the session authentication key and the routing prefix.
 
-packages = \
-['fastapi_authlib',
- 'fastapi_authlib.alembic',
- 'fastapi_authlib.alembic.versions',
- 'fastapi_authlib.config',
- 'fastapi_authlib.messages',
- 'fastapi_authlib.repository',
- 'fastapi_authlib.rest_api',
- 'fastapi_authlib.rest_api.handler',
- 'fastapi_authlib.rest_api.routers',
- 'fastapi_authlib.schemas',
- 'fastapi_authlib.services',
- 'fastapi_authlib.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiomysql>=0.1.1,<0.2.0',
- 'alembic>=1.10.3,<2.0.0',
- 'authlib>=1.2.0,<2.0.0',
- 'dynaconf>=3.1.12,<4.0.0',
- 'fastapi-sa>=0.1.0,<0.2.0',
- 'fastapi>=0.95.0,<0.96.0',
- 'httpx>=0.24.0,<0.25.0',
- 'inflection>=0.5.1,<0.6.0',
- 'itsdangerous>=2.1.2,<3.0.0',
- 'sqlalchemy==1.4.46',
- 'uvicorn>=0.21.1,<0.22.0']
-
-setup_kwargs = {
-    'name': 'fastapi-authlib',
-    'version': '0.0.2',
-    'description': 'A fastapi authlib authentication library',
-    'long_description': '# fastapi-authlib\n\nfastapi-authlib provides easy integration between FastAPI and openid connection in your application.\nProvides the initialization and dependencies of oidc, aiming to unify authentication management and\nreduce the difficulty of use.\n\n## Installing\n\ninstall and update using pip:\n\n```shell\npip install fastapi-authlib\n```\n\n## Examples\n\n### Create settings for examples, `settings.py`\n\n```python\nconfig = {\n    \'database\': \'sqlite+aiosqlite:////tmp/oidc_demo.db\',\n    \'oauth_client_id\': \'client_id\',\n    \'oauth_client_secret\': \'client_secret\',\n    \'oauth_conf_url\': \'conf_url\',\n    \'session_secret\': \'secret_key\',\n    \'router_prefix\': \'\',\n}\n```\n\nsettings.py is a simple configuration file of the use case, which mainly provides the database link,\nthe necessary parameters used by oidc, the session authentication key and the routing prefix.\n\nPlease use your authentication server configuration to populate the parameter value prefixed with oauth.\nOther parameters can be modified according to the actual situation.\n\n### Create api route, `api_router.py`\n\n```python\nfrom fastapi import APIRouter\nfrom starlette.requests import Request\n\nrouter = APIRouter()\n\n\n@router.get(\'/index\')\nasync def index(\n        *,\n        request: Request,\n):\n    """\n    User\n    """\n    user_info = request.state.user\n    return {\'name\': user_info.get(\'user_name\')}\n```\n\nFor authenticated api, you can use `request.state.user` to get the current user.\n\n### Create oidc demo entry, `main.py`\n\n```python\n"""main"""\nimport uvicorn\nfrom fastapi import Depends, FastAPI\nfrom fastapi_sa.database import db\nfrom fastapi_sa.middleware import DBSessionMiddleware\n\nfrom fastapi_authlib.oidc import OIDCClient\nfrom fastapi_authlib.utils.check_user_depend import check_auth_session\nfrom api_router import index\nfrom .settings import config\n\n\nclass OIDCDemo:\n    """OIDCDemo"""\n\n    def __init__(self, settings: dict):\n        self.settings = settings\n        self.router_prefix = self.settings.get(\'router_prefix\')\n\n    def run(self):\n        """Run"""\n        # Early environment initialization\n        app = FastAPI(title=\'FastAPIOIDCSupportDemo\', version=\'0.1.0\')\n        db.init(self.settings.get(\'database\'))\n\n        # Oidc environment initialization\n        client = OIDCClient(\n            app=app,\n            **config\n        )\n        # If you only init app, you should use init_app() instead\n        client.init_oidc()\n\n        # Customize the environment initialization\n        # add dependencies to the interface that needs to be authenticated\n        app.include_router(index.router, tags=[\'index\'], prefix=config.get(\'router_prefix\'),\n                           dependencies=[Depends(check_auth_session)])\n        app.add_middleware(DBSessionMiddleware)\n        return app\n\n\nif __name__ == \'__main__\':\n    client_app = OIDCDemo(config).run()\n    uvicorn.run(client_app, host="0.0.0.0", port=8001)\n\n```\n\n### Use Step\n\n- Create app and init db\n- Init the environment of oidc, If you don\'t want to do data migration, you should use init_app method.\n  Usually database migration and oidc initialization are performed together\n- Register routing and other middleware, the DBSessionMiddleware is required\n- Start a fastapi server with uvicorn or other\n\n## Based on\n\n- [FastAPI](https://github.com/tiangolo/fastapi)\n- [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy)\n- [Fastapi-sa](https://github.com/whg517/fastapi-sa)\n- [Authlib](https://github.com/lepture/authlib)\n\n## Develop\n\nYou may need to read the [develop document](./docs/development.md) to use SRC Layout in your IDE.\n',
-    'author': 'qiang.xie',
-    'author_email': 'qiang.xie@zncdata.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+Please use your authentication server configuration to populate the parameter value prefixed with oauth.
+Other parameters can be modified according to the actual situation.
+
+### Create api route, `api_router.py`
+
+```python
+from fastapi import APIRouter
+from starlette.requests import Request
+
+router = APIRouter()
+
+
+@router.get('/index')
+async def index(
+        *,
+        request: Request,
+):
+    """
+    User
+    """
+    user_info = request.state.user
+    return {'name': user_info.get('user_name')}
+```
+
+For authenticated api, you can use `request.state.user` to get the current user.
+
+### Create oidc demo entry, `main.py`
+
+```python
+"""main"""
+import uvicorn
+from fastapi import Depends, FastAPI
+from fastapi_sa.database import db
+from fastapi_sa.middleware import DBSessionMiddleware
+
+from fastapi_authlib.oidc import OIDCClient
+from fastapi_authlib.utils.auth_dependency import check_auth_depends
+from api_router import index
+from .settings import config
+
+
+class OIDCDemo:
+    """OIDCDemo"""
+
+    def __init__(self, settings: dict):
+        self.settings = settings
+        self.router_prefix = self.settings.get('router_prefix')
+
+    def run(self):
+        """Run"""
+        # Early environment initialization
+        app = FastAPI(title='FastAPIOIDCSupportDemo', version='0.1.0')
+        db.init(self.settings.get('database'))
+
+        # Oidc environment initialization
+        client = OIDCClient(
+            app=app,
+            **config
+        )
+        # If you only init app, you should use init_app() instead
+        client.init_oidc()
+
+        # Customize the environment initialization
+        # add dependencies to the interface that needs to be authenticated
+        app.include_router(
+            index.router,
+            tags=['index'],
+            prefix=config.get('router_prefix'),
+            dependencies=[Depends(check_auth_depends)]
+        )
+        app.add_middleware(DBSessionMiddleware)
+        return app
+
+
+if __name__ == '__main__':
+    client_app = OIDCDemo(config).run()
+    uvicorn.run(client_app, host="0.0.0.0", port=8001)
+
+```
+
+### Use Step
+
+- Create app and init db
+- Init the environment of oidc, If you don't want to do data migration, you should use init_app method.
+  Usually database migration and oidc initialization are performed together
+- Register routing and other middleware, the DBSessionMiddleware is required
+- Start a fastapi server with uvicorn or other
+
+### Other
+
+Provide the following apis
+- /login
+- /auth
+- /logout
+- /users
+
+## Based on
+
+- [FastAPI](https://github.com/tiangolo/fastapi)
+- [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy)
+- [Fastapi-sa](https://github.com/whg517/fastapi-sa)
+- [Authlib](https://github.com/lepture/authlib)
+
+## Develop
 
+You may need to read the [develop document](./docs/development.md) to use SRC Layout in your IDE.
 
-setup(**setup_kwargs)
```

