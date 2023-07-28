# Comparing `tmp/mysql-mimic-2.3.0.tar.gz` & `tmp/mysql-mimic-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.3.0.tar", last modified: Mon Jul 17 22:38:55 2023, max compression
+gzip compressed data, was "mysql-mimic-2.3.1.tar", last modified: Fri Jul 28 20:45:53 2023, max compression
```

## Comparing `mysql-mimic-2.3.0.tar` & `mysql-mimic-2.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.816597 mysql-mimic-2.3.0/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    19029 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.816597 mysql-mimic-2.3.0/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19029 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 20:45:53.000000 mysql-mimic-2.3.1/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:45:53.841586 mysql-mimic-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29117 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 20:44:55.000000 mysql-mimic-2.3.1/tests/test_version.py
```

### Comparing `mysql-mimic-2.3.0/LICENSE` & `mysql-mimic-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/PKG-INFO` & `mysql-mimic-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.3.0
+Version: 2.3.1
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.3.0/README.md` & `mysql-mimic-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/auth.py` & `mysql-mimic-2.3.1/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/charset.py` & `mysql-mimic-2.3.1/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/connection.py` & `mysql-mimic-2.3.1/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/constants.py` & `mysql-mimic-2.3.1/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/errors.py` & `mysql-mimic-2.3.1/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/intercept.py` & `mysql-mimic-2.3.1/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/packets.py` & `mysql-mimic-2.3.1/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/results.py` & `mysql-mimic-2.3.1/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/schema.py` & `mysql-mimic-2.3.1/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/server.py` & `mysql-mimic-2.3.1/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/session.py` & `mysql-mimic-2.3.1/mysql_mimic/session.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/stream.py` & `mysql-mimic-2.3.1/mysql_mimic/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     f"Expected seq({expected}) got seq({sequence_id})",
                     ErrorCode.MALFORMED_PACKET,
                 )
 
             if payload_length == 0:
                 return data
 
-            data += await self.reader.read(payload_length)
+            data += await self.reader.readexactly(payload_length)
 
             if payload_length < 0xFFFFFF:
                 return data
 
     async def write(self, data: bytes) -> None:
         while True:
             # Grab first 0xFFFFFF bytes to send
```

### Comparing `mysql-mimic-2.3.0/mysql_mimic/types.py` & `mysql-mimic-2.3.1/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/utils.py` & `mysql-mimic-2.3.1/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic/variables.py` & `mysql-mimic-2.3.1/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.3.1/mysql_mimic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.3.0
+Version: 2.3.1
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.3.0/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.3.1/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/setup.py` & `mysql-mimic-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/tests/test_auth.py` & `mysql-mimic-2.3.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/tests/test_query.py` & `mysql-mimic-2.3.1/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import io
 from contextlib import closing
 from datetime import date, datetime, timedelta
-from functools import partial
-from typing import Any, Callable, Awaitable, Sequence, Dict, List, Tuple
+from typing import Any, Callable, Awaitable, Sequence, Dict, List, Tuple, Type
 
 import pytest
 import pytest_asyncio
 from mysql.connector.abstracts import MySQLConnectionAbstract
+from mysql.connector.cursor import MySQLCursorDict, MySQLCursor
 from sqlalchemy import text
 from sqlalchemy.ext.asyncio import AsyncEngine
 import aiomysql
 from freezegun import freeze_time
 
 from mysql_mimic import ResultColumn, ResultSet, MysqlServer, context
 from mysql_mimic.charset import CharacterSet
@@ -263,37 +263,37 @@
         assert result[0]["DATABASE()"] == "db"
 
         result = await query(conn, "SELECT schema()")
         assert result[0]["SCHEMA()"] == "db"
 
 
 @pytest.mark.asyncio
+@pytest.mark.parametrize("cursor_class", [MySQLCursorDict, PreparedDictCursor])
 async def test_query_attributes(
     session: MockSession,
     server: MysqlServer,
     mysql_connector_conn: MySQLConnectionAbstract,
+    cursor_class: Type[MySQLCursor],
 ) -> None:
     session.echo = True
 
-    for i, q in enumerate(
-        [
-            partial(query, conn=mysql_connector_conn),
-            partial(query, conn=mysql_connector_conn, cursor_class=PreparedDictCursor),
-        ]
-    ):
-        session.last_query_attrs = None
-        sql = "SELECT 1 FROM x"
-        query_attrs = {
-            "idx": i,
-            "str": "foo",
-            "int": 1,
-            "float": 1.1,
-        }
-        await q(sql=sql, query_attributes=query_attrs)
-        assert session.last_query_attrs == query_attrs
+    sql = "SELECT 1 FROM x"
+    query_attrs = {
+        "id": cursor_class.__name__,
+        "str": "foo",
+        "int": 1,
+        "float": 1.1,
+    }
+    await query(
+        sql=sql,
+        conn=mysql_connector_conn,
+        query_attributes=query_attrs,  # type: ignore
+        cursor_class=cursor_class,
+    )
+    assert session.last_query_attrs == query_attrs
 
 
 # pylint: disable=trailing-whitespace
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "sql, expected",
     [
```

### Comparing `mysql-mimic-2.3.0/tests/test_ssl.py` & `mysql-mimic-2.3.1/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/tests/test_stream.py` & `mysql-mimic-2.3.1/tests/test_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     async def read(self, n: int) -> bytes:
         start = self.pos
         end = self.pos + n
         self.pos = end
 
         return self.data[start:end]
 
+    readexactly = read
+
 
 class MockWriter:
     def __init__(self) -> None:
         self.data = b""
 
     def write(self, data: bytes) -> None:
         self.data += data
```

### Comparing `mysql-mimic-2.3.0/tests/test_types.py` & `mysql-mimic-2.3.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.3.0/tests/test_variables.py` & `mysql-mimic-2.3.1/tests/test_variables.py`

 * *Files identical despite different names*

