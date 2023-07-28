# Comparing `tmp/sqlx-batis-0.1.0.tar.gz` & `tmp/sqlx-batis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.0.tar", last modified: Thu Jul 27 11:31:34 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.1.tar", last modified: Fri Jul 28 02:50:40 2023, max compression
```

## Comparing `sqlx-batis-0.1.0.tar` & `sqlx-batis-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/
--rw-rw-rw-   0        0        0     3373 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-27 11:30:05.000000 sqlx-batis-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlbatis/
--rw-rw-rw-   0        0        0      834 2023-07-26 14:53:18.000000 sqlx-batis-0.1.0/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8669 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6449 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     4377 2023-07-27 04:39:23.000000 sqlx-batis-0.1.0/sqlbatis/engin.py
--rw-rw-rw-   0        0        0     3836 2023-07-27 03:54:22.000000 sqlx-batis-0.1.0/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38924 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.0/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.0/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5238 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.0/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.0/sqlbatis/support.py
--rw-rw-rw-   0        0        0      603 2023-07-27 11:30:50.000000 sqlx-batis-0.1.0/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3373 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      464 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/
+-rw-rw-rw-   0        0        0     3373 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-28 02:50:31.000000 sqlx-batis-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlbatis/
+-rw-rw-rw-   0        0        0      834 2023-07-26 14:53:18.000000 sqlx-batis-0.1.1/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.1/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.1/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     4411 2023-07-28 02:00:07.000000 sqlx-batis-0.1.1/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.1/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.1/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.1/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.1/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.1/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.1/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.1/sqlbatis/support.py
+-rw-rw-rw-   0        0        0      606 2023-07-28 01:56:21.000000 sqlx-batis-0.1.1/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3373 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.0/PKG-INFO` & `sqlx-batis-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.0
+Version: 0.1.1
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.1.0/README.rst` & `sqlx-batis-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.0/setup.py` & `sqlx-batis-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.2.2',
+        'sqlx-exec>=1.2.5',
     ],
-    version='0.1.0',
+    version='0.1.1',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.0/sqlbatis/constant.py` & `sqlx-batis-0.1.1/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.0/sqlbatis/db.py` & `sqlx-batis-0.1.1/sqlbatis/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import sql_support, Engin, DBError
+from . import sql_support, Engine, DBError
 from .log_support import sql_log, do_sql_log, save_log, do_page_log, page_log
 
 # Don't remove. Import for not repetitive implementation
 from sqlexec import insert, save as save_select_key, save_sql, batch_insert, batch_execute, execute as supper_execute, get as supper_get, query_one as supper_query_one,\
     query as supper_query, select as supper_select, select_one as supper_select_one
 
 
@@ -11,15 +11,15 @@
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
     :return: Primary key
     """
     save_log(table, **kwargs)
     try:
-        select_key = Engin.get_select_key_intf(table=table)
+        select_key = Engine.get_select_key_intf(table=table)
     except NotImplementedError:
         raise DBError(f"Expect 'select_key' but not. you may should use 'save_select_key' func with 'select_key'.")
     return save_select_key(select_key, table, **kwargs)
 
 
 def execute(sql: str, *args, **kwargs):
     """
@@ -175,19 +175,19 @@
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('select_page', sql.strip(), page_num, page_size, args)
-    sql, args = Engin.get_page_sql_args_intf(sql, page_num, page_size, *args)
+    sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
     return supper_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('do_select_page', sql.strip(), page_num, page_size, args)
-    sql, args = Engin.get_page_sql_args_intf(sql, page_num, page_size, *args)
+    sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
     return supper_select(sql, *args)
```

### Comparing `sqlx-batis-0.1.0/sqlbatis/dbx.py` & `sqlx-batis-0.1.1/sqlbatis/dbx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 from .sql_support import get_batch_args
-from . import Engin, DBError, sql_holder as holder
-from .log_support import logger, sql_id_log, page_sql_id_log
+from . import Engine, DBError, sql_holder as holder
+from .log_support import logger, sql_id_log, page_sql_id_log, sql_id_select_key_log
 
 # Don't remove. Import for not repetitive implementation
 from .db import(do_execute, insert, save_sql, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_select, \
                 do_select_one, do_select_page, do_query_page)
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
-    sql_id_log('dbx.save', sql_id, *args, **kwargs)
+    sql_id_log('save', sql_id, *args, **kwargs)
     sql_model = holder.get_sql_model(sql_id)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
     select_key = sql_model.select_key
+    sql, args = holder.do_get_sql(sql_model, False, None, *args, **kwargs)
     if not select_key:
         try:
-            select_key = Engin.get_select_key_intf(sql=sql)
+            select_key = Engine.get_select_key_intf(sql=sql)
         except NotImplementedError:
             raise DBError(f"Expect 'select_key' but not. you can set it in mapper file with 'selectKey'.")
     return save_sql(select_key, sql, *args)
 
 
+def save_select_key(select_key, sql_id: str, *args, **kwargs):
+    """
+    Execute insert SQL, return primary key.
+    :return: Primary key
+    """
+    sql_id_select_key_log('save_select_key', select_key, sql_id, *args, **kwargs)
+    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    return save_sql(select_key, sql, *args)
+
+
 def execute(sql_id: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('dbx.execute', sql_id, *args, **kwargs)
```

### Comparing `sqlx-batis-0.1.0/sqlbatis/engin.py` & `sqlx-batis-0.1.1/sqlbatis/engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 import re
 from sqlexec import get
 from typing import Sequence
 from .support import DBError
 from functools import lru_cache
 from .log_support import logger
-from sqlexec.engin import Engin as BaseEngin
+from sqlexec.engine import Engine as BaseEngine
 from .sql_support import require_limit, get_page_start
 from .constant import MYSQL_COLUMN_SQL, POSTGRES_COLUMN_SQL, MYSQL_SELECT_KEY, LIMIT_1, MYSQL, POSTGRESQL, DEFAULT_KEY_FIELD, CACHE_SIZE
 
 
 # Engin = Enum('Engin', ['MYSQL', 'POSTGRESQL', 'OTHER'])
 # class Engin(Enum):
 #     MYSQL = 'MySQL'
 #     POSTGRESQL = 'PostgreSQL'
 #     OTHER = 'Other'
 
 
-class Engin(BaseEngin):
+class Engine(BaseEngine):
     def __init__(self, name=None):
         super().__init__(name)
 
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
-        if Engin.current_engin() == MYSQL:
-            return MySqlEngin.get_page_sql_args(sql, page_num, page_size, *args)
-        elif Engin.current_engin() == POSTGRESQL:
-            return PostgresEngin.get_page_sql_args(sql, page_num, page_size, *args)
-        raise NotImplementedError(f"Not implement method 'get_page_sql_args' for {Engin.current_engin()}.")
+        if Engine.current_engine() == MYSQL:
+            return MySqlEngine.get_page_sql_args(sql, page_num, page_size, *args)
+        elif Engine.current_engine() == POSTGRESQL:
+            return PostgresEngine.get_page_sql_args(sql, page_num, page_size, *args)
+        raise NotImplementedError(f"Not implement method 'get_page_sql_args' for {Engine.current_engine()}.")
 
     @staticmethod
     def get_select_key(*args, **kwargs):
-        if Engin.current_engin() == MYSQL:
-            return MySqlEngin.get_select_key()
-        elif Engin.current_engin() == POSTGRESQL:
-            return PostgresEngin.get_select_key(*args, **kwargs)
-        raise NotImplementedError(f"Not implement method 'get_select_key' for {Engin.current_engin()}.")
+        if Engine.current_engine() == MYSQL:
+            return MySqlEngine.get_select_key()
+        elif Engine.current_engine() == POSTGRESQL:
+            return PostgresEngine.get_select_key(*args, **kwargs)
+        raise NotImplementedError(f"Not implement method 'get_select_key' for {Engine.current_engine()}.")
 
     @staticmethod
     def get_table_columns(table: str):
-        if Engin.current_engin() == MYSQL:
-            return MySqlEngin.get_table_columns(table)
-        elif Engin.current_engin() == POSTGRESQL:
-            return PostgresEngin.get_table_columns(table)
+        if Engine.current_engine() == MYSQL:
+            return MySqlEngine.get_table_columns(table)
+        elif Engine.current_engine() == POSTGRESQL:
+            return PostgresEngine.get_table_columns(table)
         raise "*"
 
 
 
-class MySqlEngin(Engin):
+class MySqlEngine(Engine):
     def __init__(self, engin):
         super().__init__(engin)
 
     @classmethod
     def init(cls, name=MYSQL):
         super().init(name)
 
@@ -71,15 +71,15 @@
     def get_table_columns(table: str):
         return get(MYSQL_COLUMN_SQL, table, LIMIT_1)
 
     @staticmethod
     def get_select_key():
         return MYSQL_SELECT_KEY
 
-class PostgresEngin(Engin):
+class PostgresEngine(Engine):
     def __init__(self, engin):
         super().__init__(engin)
 
     @classmethod
     def init(cls, name=POSTGRESQL):
         super().init(name)
 
@@ -95,28 +95,28 @@
     def get_table_columns(table: str):
         return get(POSTGRES_COLUMN_SQL, table, LIMIT_1)
 
     @staticmethod
     def get_select_key(key_seq: str = None, table: str = None, key: str =None, sql: str = None):
         if not key_seq:
             if table:
-                key_seq = PostgresEngin.build_key_seq(table, key)
+                key_seq = PostgresEngine.build_key_seq(table, key)
             else:
                 if sql:
-                    key_seq = PostgresEngin._get_key_seq_from_sql(sql)
+                    key_seq = PostgresEngine._get_key_seq_from_sql(sql)
                 else:
                     raise DBError("Get PostgreSQL select key fail, all of 'key_seq', 'table', 'sql' are None")
         return f"SELECT currval('{key_seq}')"
 
     @staticmethod
     def build_key_seq(table: str, key: str = None):
         if not key:
             key = DEFAULT_KEY_FIELD
         return f'{table}_{key}_seq'
 
     @staticmethod
     @lru_cache(maxsize=CACHE_SIZE)
     def _get_key_seq_from_sql(sql: str):
         table = re.search('(?<=into )\w+', sql, re.I)
-        key_seq = PostgresEngin.build_key_seq(table.group())
+        key_seq = PostgresEngine.build_key_seq(table.group())
         logger.warning("'key_seq' is None, will use default '{}' from sql.".format(key_seq))
         return key_seq
```

### Comparing `sqlx-batis-0.1.0/sqlbatis/log_support.py` & `sqlx-batis-0.1.1/sqlbatis/log_support.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     logger.debug("Exec func 'sqlbatis.dbx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (function, page_num, page_size, sql_id, args, kwargs))
 
 
 def sql_id_log(function: str, sql_id: str, *args, **kwargs):
     logger.debug("Exec func 'sqlbatis.dbx.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
 
 
+def sql_id_select_key_log(function: str, select_key: str, sql_id: str, *args, **kwargs):
+    logger.debug("Exec func 'sqlbatis.dbx.%s', select_key: %s, sql_id: %s, args: %s, kwargs: %s" % (function, select_key, sql_id.strip(), args, kwargs))
+
+
 def orm_insert_log(function, class_name, **kwargs):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def orm_delete_by_id_log(function, class_name, _id, update_by):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
```

### Comparing `sqlx-batis-0.1.0/sqlbatis/orm.py` & `sqlx-batis-0.1.1/sqlbatis/orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from .engin import Engin
+from .engine import Engine
 from datetime import datetime
 from enum import Enum, IntEnum
 from .sql_support import simple_sql
 from .snowflake import get_snowflake_id
 from . import db, log_support, transaction
 from .support import DBError, NotFoundError
 from typing import Sequence, Union, List, Tuple
@@ -206,15 +206,15 @@
             kwargs[key] = get_snowflake_id()
             db.insert(table, **kwargs)
             return kwargs[key]
         else:
             select_key = cls._get_select_key()
             if not select_key:
                 try:
-                    select_key = Engin.get_select_key_intf(table=table, key=key)
+                    select_key = Engine.get_select_key_intf(table=table, key=key)
                 except NotImplementedError:
                     raise DBError(f"Expect 'select_key' but not. you can set it in model class with '__select_key__'.")
             return db.save_select_key(select_key, table, **kwargs)
 
     @classmethod
     def create(cls, **kwargs):
         """
@@ -817,15 +817,15 @@
 
 
 # ----------------------------------------------------------Private function------------------------------------------------------------------
 def select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
     if fields:
         fields = ','.join([col if '(' in col else '{}'.format(col) for col in fields])
     else:
-        fields = Engin.get_table_columns_intf(table)
+        fields = Engine.get_table_columns_intf(table)
 
     if limit:
         if isinstance(limit, int):
             return 'SELECT {} FROM {} {} LIMIT ?'.format(fields, table, where)
         elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
             return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(fields, table, where)
         else:
```

### Comparing `sqlx-batis-0.1.0/sqlbatis/snowflake.py` & `sqlx-batis-0.1.1/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.0/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.1/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.0/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.1/sqlbatis/sql_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sqlexec
 import functools
-from .engin import Engin
+from .engine import Engine
 from .log_support import logger
 from .support import SqlAction, DBError
 from .sql_support import simple_sql, get_named_sql_args
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
@@ -21,15 +21,15 @@
             if return_key:
                 use_select_key = select_key
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
                 if use_select_key is None:
                     use_select_key = sql_model.select_key
                     if use_select_key is None:
                         try:
-                            use_select_key = Engin.get_select_key_intf(sql=use_sql)
+                            use_select_key = Engine.get_select_key_intf(sql=use_sql)
                         except NotImplementedError:
                             return DBError(
                                 f"Expect 'select_key' but not. you can set it in mapper file with 'selectKey', or @mapper with 'select_key'")
                 return sqlexec.save_sql(use_select_key, use_sql, *args)
             if batch:
                 if kwargs:
                     logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
@@ -55,15 +55,15 @@
                     if kwargs:
                         args = list(kwargs.values())[0]
                     return sqlexec.batch_execute(use_sql, *args)
                 if return_key:
                     use_select_key = select_key
                     if use_select_key is None:
                         try:
-                            use_select_key = Engin.get_select_key_intf(sql=use_sql)
+                            use_select_key = Engine.get_select_key_intf(sql=use_sql)
                         except NotImplementedError:
                             return DBError(f"Expect 'select_key' but not in func '{func.__name__}' at file: '{func.__code__.co_filename}', line {func.__code__.co_firstlineno}. you can set it @sql with 'select_key'")
                     assert SqlAction.INSERT.value in low_sql, 'Only insert sql can return primary key.'
                     if kwargs:
                         use_sql, args = get_named_sql_args(use_sql, **kwargs)
                     return sqlexec.save_sql(use_select_key, use_sql, *args)
```

### Comparing `sqlx-batis-0.1.0/sqlbatis/sql_support.py` & `sqlx-batis-0.1.1/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.0/sqlbatis/__init__.py` & `sqlx-batis-0.1.1/sqlbatis/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,19 @@
     connection,
     transaction,
     with_connection,
     with_transaction,
     get_connection,
     DBError
 )
-from .engin import Engin
+from .engine import Engine
 from .sql_mapper import sql, mapper
 from .snowflake import init_snowflake, get_snowflake_id
 
 def init_db(driver='', mapper_path='mapper', pool_size=0, show_sql=False, debug=False,  **kwargs):
     from .sql_holder import load_mapper
     from sqlexec import init_db as supper_init_db
-    Engin.init()
+    Engine.init()
     supper_init_db(driver=driver, pool_size=pool_size, show_sql=show_sql,debug=debug, **kwargs)
     load_mapper(mapper_path)
```

### Comparing `sqlx-batis-0.1.0/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.1.1/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.0
+Version: 0.1.1
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

