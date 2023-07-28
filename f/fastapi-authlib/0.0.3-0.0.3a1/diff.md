# Comparing `tmp/fastapi_authlib-0.0.3.tar.gz` & `tmp/fastapi_authlib-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_authlib-0.0.3.tar", max compression
+gzip compressed data, was "fastapi_authlib-0.0.3a1.tar", max compression
```

## Comparing `fastapi_authlib-0.0.3.tar` & `fastapi_authlib-0.0.3a1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1097 2023-05-25 09:49:48.758784 fastapi_authlib-0.0.3/LICENSE
--rw-r--r--   0        0        0     1903 2023-07-28 05:33:24.612437 fastapi_authlib-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3676 2023-07-28 06:34:50.084730 fastapi_authlib-0.0.3/README.md
--rw-r--r--   0        0        0       36 2023-07-27 03:17:45.034283 fastapi_authlib-0.0.3/src/fastapi_authlib/__init__.py
--rw-r--r--   0        0        0     3313 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/alembic.ini
--rw-r--r--   0        0        0     2794 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/env.py
--rw-r--r--   0        0        0       38 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/README
--rw-r--r--   0        0        0      534 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/script.py.mako
--rw-r--r--   0        0        0     3390 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py
--rw-r--r--   0        0        0      298 2023-07-28 05:55:20.666180 fastapi_authlib-0.0.3/src/fastapi_authlib/config/__init__.py
--rw-r--r--   0        0        0      245 2023-07-28 06:01:24.727932 fastapi_authlib-0.0.3/src/fastapi_authlib/config/settings.yml
--rw-r--r--   0        0        0       15 2023-07-28 06:53:47.009372 fastapi_authlib-0.0.3/src/fastapi_authlib/messages/__init__.py
--rw-r--r--   0        0        0      219 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.3/src/fastapi_authlib/messages/base.py
--rw-r--r--   0        0        0      236 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.3/src/fastapi_authlib/messages/user.py
--rw-r--r--   0        0        0     2906 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.3/src/fastapi_authlib/models.py
--rw-r--r--   0        0        0     3542 2023-07-28 06:06:00.028011 fastapi_authlib-0.0.3/src/fastapi_authlib/oidc.py
--rw-r--r--   0        0        0       17 2023-07-28 06:53:46.941374 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/__init__.py
--rw-r--r--   0        0        0     5347 2023-07-28 06:53:46.989373 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/base.py
--rw-r--r--   0        0        0      767 2023-07-28 06:53:47.054373 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/group.py
--rw-r--r--   0        0        0      953 2023-07-28 03:20:37.301648 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/group_user_map.py
--rw-r--r--   0        0        0     1121 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/session.py
--rw-r--r--   0        0        0      751 2023-07-28 06:53:47.075778 fastapi_authlib-0.0.3/src/fastapi_authlib/repository/user.py
--rw-r--r--   0        0        0       23 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/__init__.py
--rw-r--r--   0        0        0      799 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/exception_handlers.py
--rw-r--r--   0        0        0       13 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/__init__.py
--rw-r--r--   0        0        0     1126 2023-07-28 06:54:58.918918 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/login.py
--rw-r--r--   0        0        0      621 2023-07-26 03:57:56.924608 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/logout.py
--rw-r--r--   0        0        0      489 2023-07-28 03:20:21.991250 fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/user.py
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/__init__.py
--rw-r--r--   0        0        0      385 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/base.py
--rw-r--r--   0        0        0      504 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/group.py
--rw-r--r--   0        0        0      597 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/group_user_map.py
--rw-r--r--   0        0        0     1011 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/session.py
--rw-r--r--   0        0        0      684 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/user.py
--rw-r--r--   0        0        0      102 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3/src/fastapi_authlib/services/__init__.py
--rw-r--r--   0        0        0     9737 2023-07-28 06:53:46.967373 fastapi_authlib-0.0.3/src/fastapi_authlib/services/auth.py
--rw-r--r--   0        0        0     3882 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.3/src/fastapi_authlib/services/base.py
--rw-r--r--   0        0        0     1291 2023-07-27 06:02:26.732846 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/__init__.py
--rw-r--r--   0        0        0     2535 2023-07-28 03:19:26.550076 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/auth_dependency.py
--rw-r--r--   0        0        0      870 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/exceptions.py
--rw-r--r--   0        0        0      425 2023-07-28 06:41:28.199278 fastapi_authlib-0.0.3/src/fastapi_authlib/utils/types.py
--rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-25 09:49:48.758784 fastapi_authlib-0.0.3a1/LICENSE
+-rw-r--r--   0        0        0     1911 2023-07-28 07:56:46.053613 fastapi_authlib-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0     3676 2023-07-28 06:34:50.084730 fastapi_authlib-0.0.3a1/README.md
+-rw-r--r--   0        0        0       44 2023-07-28 07:56:46.071848 fastapi_authlib-0.0.3a1/src/fastapi_authlib/__init__.py
+-rw-r--r--   0        0        0     3313 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/alembic.ini
+-rw-r--r--   0        0        0     2794 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/env.py
+-rw-r--r--   0        0        0       38 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/README
+-rw-r--r--   0        0        0      534 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/script.py.mako
+-rw-r--r--   0        0        0     3390 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py
+-rw-r--r--   0        0        0      298 2023-07-28 05:55:20.666180 fastapi_authlib-0.0.3a1/src/fastapi_authlib/config/__init__.py
+-rw-r--r--   0        0        0      251 2023-07-28 07:38:31.953514 fastapi_authlib-0.0.3a1/src/fastapi_authlib/config/settings.yml
+-rw-r--r--   0        0        0       15 2023-07-28 06:53:47.009372 fastapi_authlib-0.0.3a1/src/fastapi_authlib/messages/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.3a1/src/fastapi_authlib/messages/base.py
+-rw-r--r--   0        0        0      236 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.3a1/src/fastapi_authlib/messages/user.py
+-rw-r--r--   0        0        0     2906 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/models.py
+-rw-r--r--   0        0        0     3542 2023-07-28 06:06:00.028011 fastapi_authlib-0.0.3a1/src/fastapi_authlib/oidc.py
+-rw-r--r--   0        0        0       17 2023-07-28 06:53:46.941374 fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/__init__.py
+-rw-r--r--   0        0        0     5347 2023-07-28 06:53:46.989373 fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/base.py
+-rw-r--r--   0        0        0      767 2023-07-28 06:53:47.054373 fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/group.py
+-rw-r--r--   0        0        0      953 2023-07-28 03:20:37.301648 fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/group_user_map.py
+-rw-r--r--   0        0        0     1121 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/session.py
+-rw-r--r--   0        0        0      751 2023-07-28 06:53:47.075778 fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/user.py
+-rw-r--r--   0        0        0       23 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/__init__.py
+-rw-r--r--   0        0        0      799 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/handler/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/handler/exception_handlers.py
+-rw-r--r--   0        0        0       13 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/routers/__init__.py
+-rw-r--r--   0        0        0     1126 2023-07-28 06:54:58.918918 fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/routers/login.py
+-rw-r--r--   0        0        0      621 2023-07-26 03:57:56.924608 fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/routers/logout.py
+-rw-r--r--   0        0        0      489 2023-07-28 03:20:21.991250 fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/routers/user.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/base.py
+-rw-r--r--   0        0        0      504 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/group.py
+-rw-r--r--   0        0        0      597 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/group_user_map.py
+-rw-r--r--   0        0        0     1011 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/session.py
+-rw-r--r--   0        0        0      684 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/user.py
+-rw-r--r--   0        0        0      102 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/services/__init__.py
+-rw-r--r--   0        0        0     9723 2023-07-28 07:53:34.740815 fastapi_authlib-0.0.3a1/src/fastapi_authlib/services/auth.py
+-rw-r--r--   0        0        0     3882 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.3a1/src/fastapi_authlib/services/base.py
+-rw-r--r--   0        0        0     1291 2023-07-27 06:02:26.732846 fastapi_authlib-0.0.3a1/src/fastapi_authlib/utils/__init__.py
+-rw-r--r--   0        0        0     2535 2023-07-28 07:52:19.579122 fastapi_authlib-0.0.3a1/src/fastapi_authlib/utils/auth_dependency.py
+-rw-r--r--   0        0        0      870 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.3a1/src/fastapi_authlib/utils/exceptions.py
+-rw-r--r--   0        0        0      425 2023-07-28 06:41:28.199278 fastapi_authlib-0.0.3a1/src/fastapi_authlib/utils/types.py
+-rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.3a1/PKG-INFO
```

### Comparing `fastapi_authlib-0.0.3/LICENSE` & `fastapi_authlib-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/pyproject.toml` & `fastapi_authlib-0.0.3a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-authlib"
-version = "0.0.3"
+version = "0.0.3-alpha.1"
 description = "A fastapi authlib authentication library"
 readme = "README.md"
 authors = ["qiang.xie <qiang.xie@zncdata.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
@@ -88,10 +88,10 @@
 ignore-paths = [
     "src/fastapi_authlib/alembic",
     "src/fastapi_authlib/.local",
 ]
 
 [tool.pylint.design]
 max-line-length = 120
-max-args = 11
+max-args = 12
 max-attributes = 10
 min-public-methods = 1
```

### Comparing `fastapi_authlib-0.0.3/README.md` & `fastapi_authlib-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/alembic.ini` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/env.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/script.py.mako` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/models.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/oidc.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/oidc.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/repository/base.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/repository/group.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/group.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/repository/group_user_map.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/group_user_map.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/repository/session.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/repository/user.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/repository/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/__init__.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/handler/exception_handlers.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/handler/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/login.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/routers/login.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/rest_api/routers/logout.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/rest_api/routers/logout.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/group_user_map.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/group_user_map.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/session.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/schemas/user.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/services/auth.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/services/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,27 @@
 from fastapi_authlib.schemas.user import UserCreate, UserSchema, UserUpdate
 from fastapi_authlib.services.base import EntityService
 from fastapi_authlib.utils import get_utc_timestamp
 from fastapi_authlib.utils.exceptions import (AuthenticationError,
                                               ObjectDoesNotExist, OIDCError)
 
 logger = logging.getLogger(__name__)
-oauth_client = OAuth(settings)
 
 
 class AuthService(EntityService[User, UserCreate, UserUpdate, UserSchema]):
     """
     Auth service.
     """
     REPOSITORY_CLASS = UserRepository
-    exp_period = settings.EXP_PERIOD
-    nts_period = settings.NTS_PERIOD
 
     def __init__(self):
-        self.oauth_client = oauth_client
+        self.oauth_client = OAuth(settings)
         self.register_oauth()
+        self.exp_period = settings.EXP_PERIOD
+        self.nts_period = settings.NTS_PERIOD
 
     @property
     def session_repository(self):
         """Session repository"""
         return SessionRepository()
 
     @property
@@ -223,27 +222,27 @@
             raise AuthenticationError()
 
         session = await self.session_repository.get_session_from_user_id(pk)
         # check token
         try:
             userinfo = await self.oauth_client.oauth.userinfo(token={'access_token': session.access_token})
         except Exception as ex:
-            logger.warning(
+            logger.debug(
                 'Get userinfo with access_token of user %s error, try use refresh token, exception info: %s',
                 pk,
                 ex
             )
             try:
                 # check refresh_token
                 access_token = await self.oauth_client.oauth.fetch_access_token(
                     refresh_token=session.refresh_token,
                     grant_type='refresh_token'
                 )
             except Exception as ex:
-                logger.warning('Get access_token with refresh_token of user %s error', pk)
+                logger.debug('Get access_token with refresh_token of user %s error', pk)
                 await self.clear_token_info(pk=pk)
                 raise AuthenticationError('Token expired error') from ex
 
             userinfo = await self.oauth_client.oauth.userinfo(token={'access_token': access_token})
             # save token
             await self.session_repository.update_by_id(
                 pk=session.id,
```

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/services/base.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/services/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/utils/__init__.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/utils/auth_dependency.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/utils/auth_dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     except DecodeError as ex:
         raise HTTPException(
             status_code=HTTP_401_UNAUTHORIZED,
             detail='Invalid token',
             headers={"WWW-Authenticate": "Bearer"}
         ) from ex
     except (AuthenticationError, Exception) as ex:
-        logger.error('Verify token error, exception info: %s', ex)
+        logger.debug('Verify token error, exception info: %s', ex)
         raise HTTPException(
             status_code=HTTP_401_UNAUTHORIZED,
             detail='Authentication failed',
             headers={"WWW-Authenticate": "Bearer"}
         ) from ex
```

### Comparing `fastapi_authlib-0.0.3/src/fastapi_authlib/utils/exceptions.py` & `fastapi_authlib-0.0.3a1/src/fastapi_authlib/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.3/PKG-INFO` & `fastapi_authlib-0.0.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-authlib
-Version: 0.0.3
+Version: 0.0.3a1
 Summary: A fastapi authlib authentication library
 License: MIT
 Author: qiang.xie
 Author-email: qiang.xie@zncdata.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

