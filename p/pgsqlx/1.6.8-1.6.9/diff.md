# Comparing `tmp/pgsqlx-1.6.8.tar.gz` & `tmp/pgsqlx-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.6.8.tar", last modified: Thu Jul 27 11:39:37 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.6.9.tar", last modified: Fri Jul 28 02:53:01 2023, max compression
```

## Comparing `pgsqlx-1.6.8.tar` & `pgsqlx-1.6.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx/
--rw-rw-rw-   0        0        0      156 2023-07-26 07:07:24.000000 pgsqlx-1.6.8/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     1080 2023-07-27 04:20:30.000000 pgsqlx-1.6.8/pgsqlx/db.py
--rw-rw-rw-   0        0        0      695 2023-07-27 04:21:57.000000 pgsqlx-1.6.8/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      544 2023-07-27 04:10:16.000000 pgsqlx-1.6.8/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     2283 2023-07-27 04:21:57.000000 pgsqlx-1.6.8/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     3318 2023-07-27 04:21:26.000000 pgsqlx-1.6.8/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0      508 2023-07-27 11:38:44.000000 pgsqlx-1.6.8/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4612 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      319 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4612 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-07-27 11:39:31.000000 pgsqlx-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/
+drwxrwxrwx   0        0        0        0 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx/
+-rw-rw-rw-   0        0        0      156 2023-07-26 07:07:24.000000 pgsqlx-1.6.9/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.6.9/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     1250 2023-07-28 02:45:27.000000 pgsqlx-1.6.9/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.6.9/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.6.9/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.6.9/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      511 2023-07-28 02:01:22.000000 pgsqlx-1.6.9/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4612 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      319 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4612 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-28 02:51:58.000000 pgsqlx-1.6.9/setup.py
```

### Comparing `pgsqlx-1.6.8/pgsqlx/db.py` & `pgsqlx-1.6.9/pgsqlx/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import PostgresEngin
+from . import PostgresEngine
 from .log_support import save_log, save_key_seq_log
 
 # Don't remove. Import for not repetitive implementation
 from sqlbatis.db import insert, save_select_key, execute, batch_insert, batch_execute, get, query, query_one, select, select_one,\
     do_execute, do_get, do_query, do_query_one, do_select, do_select_one, do_select_page, do_query_page, select_page, query_page
 
 
@@ -10,20 +10,20 @@
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
     :return: Primary key
     """
     save_log(table, **kwargs)
-    return save_key_seq(PostgresEngin.build_key_seq(table), table, **kwargs)
+    return save_key_seq(PostgresEngine.build_key_seq(table), table, **kwargs)
 
 
 def save_key_seq(key_seq: str, table: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param key_seq: primary key sequnece
     :param table: table
     :param kwargs:
     :return: Primary key
     """
     save_key_seq_log(key_seq, table, **kwargs)
-    return save_select_key(PostgresEngin.get_select_key(key_seq=key_seq, table=table), table, **kwargs)
+    return save_select_key(PostgresEngine.get_select_key(key_seq=key_seq, table=table), table, **kwargs)
```

### Comparing `pgsqlx-1.6.8/pgsqlx/orm.py` & `pgsqlx-1.6.9/pgsqlx/orm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .constant import KEY_SEQ
 from .db import insert, save_key_seq
-from . import get_snowflake_id, PostgresEngin
+from . import get_snowflake_id, PostgresEngine
 from .log_support import orm_insert_log, logger
 
 # Don't remove. Import for not repetitive implementation
 from sqlbatis.orm import DelFlag, KeyStrategy, Model as BaseModel, get_where_arg_limit, select_sql
 
 
 class Model(BaseModel):
@@ -58,8 +58,8 @@
 
     @classmethod
     def _get_key_seq(cls):
         if hasattr(cls, KEY_SEQ):
             return cls.__key_seq__
         logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY_SEQ))
         key, table = cls._get_key_and_table()
-        return PostgresEngin.build_key_seq(table=table, key=key)
+        return PostgresEngine.build_key_seq(table=table, key=key)
```

### Comparing `pgsqlx-1.6.8/pgsqlx/sql_mapper.py` & `pgsqlx-1.6.9/pgsqlx/sql_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sqlexec
 import functools
 from .log_support import logger
 from sqlbatis.support import SqlAction
-from sqlbatis.engin import PostgresEngin
+from sqlbatis.engine import PostgresEngine
 from sqlbatis.sql_support import simple_sql, get_named_sql_args
 from sqlbatis.sql_holder import get_sql_model, do_get_sql
 from sqlbatis.sql_mapper import get_exec_func, before, get_select_func
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
@@ -19,15 +19,15 @@
             sql_model = get_sql_model(full_sql_id)
             exec_func = get_exec_func(func, sql_model.action, batch)
             if return_key:
                 use_key_seq = key_seq
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
                 if use_key_seq is None:
                     use_key_seq = sql_model.key_seq
-                select_key = PostgresEngin.get_select_key(key_seq=use_key_seq, sql=use_sql)
+                select_key = PostgresEngine.get_select_key(key_seq=use_key_seq, sql=use_sql)
                 return sqlexec.save_sql(select_key, use_sql, *args)
             if batch:
                 if kwargs:
                     logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             else:
@@ -49,15 +49,15 @@
                     if kwargs:
                         args = list(kwargs.values())[0]
                     return sqlexec.batch_execute(use_sql, *args)
                 if return_key:
                     assert SqlAction.INSERT.value in low_sql, 'Only insert sql can return primary key.'
                     if kwargs:
                         use_sql, args = get_named_sql_args(use_sql, **kwargs)
-                    select_key = PostgresEngin.get_select_key(key_seq=key_seq, sql=use_sql)
+                    select_key = PostgresEngine.get_select_key(key_seq=key_seq, sql=use_sql)
                     return sqlexec.save_sql(select_key, use_sql, *args)
 
                 if kwargs:
                     use_sql, args = get_named_sql_args(use_sql, **kwargs)
                 return sqlexec.execute(use_sql, *args)
             elif SqlAction.SELECT.value in low_sql:
                 select_func = get_select_func(func)
```

### Comparing `pgsqlx-1.6.8/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.6.9/pgsqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.8
+Version: 1.6.9
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.8/PKG-INFO` & `pgsqlx-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.8
+Version: 1.6.9
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.8/README.rst` & `pgsqlx-1.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.8/setup.py` & `pgsqlx-1.6.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     packages=['pgsqlx'],
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
         # 'psycopg2>=2.7.4',
-        'sqlx-batis>=0.0.9',
+        'sqlx-batis>=0.1.1',
     ],
-    version='1.6.8',
+    version='1.6.9',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

