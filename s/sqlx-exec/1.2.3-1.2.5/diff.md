# Comparing `tmp/sqlx-exec-1.2.3.tar.gz` & `tmp/sqlx-exec-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.2.3.tar", last modified: Thu Jul 27 11:29:36 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.2.5.tar", last modified: Fri Jul 28 02:48:36 2023, max compression
```

## Comparing `sqlx-exec-1.2.3.tar` & `sqlx-exec-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     2740 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2232 2023-07-27 11:29:33.000000 sqlx-exec-1.2.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-27 11:29:33.000000 sqlx-exec-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlexec/
--rw-rw-rw-   0        0        0      350 2023-07-27 11:09:15.000000 sqlx-exec-1.2.3/sqlexec/constant.py
--rw-rw-rw-   0        0        0     1446 2023-07-27 04:42:17.000000 sqlx-exec-1.2.3/sqlexec/engin.py
--rw-rw-rw-   0        0        0    10206 2023-07-27 11:18:24.000000 sqlx-exec-1.2.3/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1246 2023-07-27 11:21:29.000000 sqlx-exec-1.2.3/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.3/sqlexec/log_support.py
--rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.3/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1134 2023-07-26 14:36:38.000000 sqlx-exec-1.2.3/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.3/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.3/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2740 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2737 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2229 2023-07-28 01:49:35.000000 sqlx-exec-1.2.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-28 02:47:53.000000 sqlx-exec-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/sqlexec/
+-rw-rw-rw-   0        0        0      350 2023-07-27 11:09:15.000000 sqlx-exec-1.2.5/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     1461 2023-07-28 01:52:46.000000 sqlx-exec-1.2.5/sqlexec/Engine.py
+-rw-rw-rw-   0        0        0    10215 2023-07-28 01:52:28.000000 sqlx-exec-1.2.5/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1260 2023-07-28 01:52:28.000000 sqlx-exec-1.2.5/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.5/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.5/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.2.5/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.5/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.5/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.2.5/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2737 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 02:48:35.000000 sqlx-exec-1.2.5/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.2.3/LICENSE` & `sqlx-exec-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.3/PKG-INFO` & `sqlx-exec-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.3
+Version: 1.2.5
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
+       sqlexec.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.2.3/README.rst` & `sqlx-exec-1.2.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
+       sqlexec.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.2.3/setup.py` & `sqlx-exec-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.3',
+    version='1.2.5',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.2.3/sqlexec/engin.py` & `sqlx-exec-1.2.5/sqlexec/Engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Sequence
 from functools import lru_cache
 from .constant import CACHE_SIZE, UNKNOW
 
-_ENGIN = None
+_ENGINE = None
 
 
-class Engin:
+class Engine:
     def __init__(self, name=UNKNOW):
         self.name = name
 
     @classmethod
     def init(cls, name=UNKNOW):
-        global _ENGIN
-        if _ENGIN:
-            if _ENGIN.name == UNKNOW and name != UNKNOW:
-                _ENGIN.name = name
+        global _ENGINE
+        if _ENGINE:
+            if _ENGINE.name == UNKNOW and name != UNKNOW:
+                _ENGINE.name = name
         else:
-            _ENGIN = cls(name)
+            _ENGINE = cls(name)
 
     @staticmethod
-    def current_engin():
-        global _ENGIN
-        if _ENGIN:
-            return _ENGIN.name
+    def current_engine():
+        global _ENGINE
+        if _ENGINE:
+            return _ENGINE.name
         return None
 
     @classmethod
     @lru_cache(maxsize=CACHE_SIZE)
     def create_insert_sql_intf(cls, table: str, cols: Sequence[str]):
-        return _ENGIN.create_insert_sql(table, cols)
+        return _ENGINE.create_insert_sql(table, cols)
 
     @staticmethod
     def get_page_sql_args_intf(sql: str, page_num: int, page_size: int, *args):
-        return _ENGIN.get_page_sql_args(sql, page_num, page_size, *args)
+        return _ENGINE.get_page_sql_args(sql, page_num, page_size, *args)
 
     @staticmethod
     def get_select_key_intf(*args, **kwargs):
-        return _ENGIN.get_select_key(*args, **kwargs)
+        return _ENGINE.get_select_key(*args, **kwargs)
 
     @staticmethod
     def get_table_columns_intf(table: str):
-        return _ENGIN.get_table_columns(table)
+        return _ENGINE.get_table_columns(table)
 
     @staticmethod
     def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
         return 'INSERT INTO {}({}) VALUES({})'.format(table, ', '.join(columns), ','.join(placeholders))
```

### Comparing `sqlx-exec-1.2.3/sqlexec/exec.py` & `sqlx-exec-1.2.5/sqlexec/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
-from .engin import Engin
 from . import sql_support
+from .engine import Engine
 from .constant import MYSQL_CONNECTOR
 from .init_import import import_driver
 from .log_support import logger, insert_log, save_log, get_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
 _SHOW_SQL = False
@@ -13,15 +13,15 @@
 def init_db(driver='', pool_size=0, show_sql=False, debug=False, **kwargs):
     global _DB_CTX, _SHOW_SQL
     if debug:
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
     prepared = MYSQL_CONNECTOR == driver
-    engin, driver, creator = import_driver(driver)
+    engine, driver, creator = import_driver(driver)
     if pool_size <= 0:
         connect = lambda: creator.connect(**kwargs)
     elif prepared:
         # mysql.connector 用自带连接池
         kwargs['pool_size'] = pool_size
         connect = lambda: creator.connect(**kwargs)
     else:
@@ -30,19 +30,19 @@
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _SHOW_SQL = show_sql
         _DB_CTX = DBCtx(connect=connect, prepared=prepared)
 
-    Engin.init(engin)
+    Engine.init(engine)
     if pool_size > 0:
-        logger.info("Inited db engin <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engin, driver, pool_size))
+        logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine, driver, pool_size))
     else:
-        logger.info("Inited db engin <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engin, driver))
+        logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine, driver))
 
 
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
     with connection():
         pass
```

### Comparing `sqlx-exec-1.2.3/sqlexec/init_import.py` & `sqlx-exec-1.2.5/sqlexec/init_import.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import importlib
-from .engin import Engin
+from .engine import Engine
 from .support import DBError
 from .log_support import logger
 from .constant import DRIVERS, UNKNOW
 
 
 def import_driver(driver):
     creator = None
     if driver:
         if driver not in DRIVERS:
             logger.warning(f"Driver '{driver}' not support now, may be you should adapte it youself.")
-        engin = DRIVERS.get(driver)
-        creator = do_import(driver, engin)
+        engine = DRIVERS.get(driver)
+        creator = do_import(driver, engine)
     else:
-        curr_engin = Engin.current_engin()
-        drivers = dict(filter(lambda x: x[1] == curr_engin, DRIVERS.items())) if curr_engin and curr_engin != UNKNOW else DRIVERS
-        for driver, engin in drivers.items():
+        curr_engine = Engine.current_engine()
+        drivers = dict(filter(lambda x: x[1] == curr_engine, DRIVERS.items())) if curr_engine and curr_engine != UNKNOW else DRIVERS
+        for driver, engine in drivers.items():
             try:
                 creator = importlib.import_module(driver)
                 break
             except ModuleNotFoundError:
                 pass
         if not creator:
             raise DBError(f"You may forgot install driver, may be one of {list(DRIVERS.keys())} suit you.")
-    return engin, driver, creator
+    return engine, driver, creator
 
 
-def do_import(driver, engin):
+def do_import(driver, Engine):
     try:
         return importlib.import_module(driver)
     except ModuleNotFoundError:
-        raise DBError(f"Import {engin} driver '{driver}' failed, please sure it was installed or change other driver.")
+        raise DBError(f"Import {Engine} driver '{driver}' failed, please sure it was installed or change other driver.")
```

### Comparing `sqlx-exec-1.2.3/sqlexec/log_support.py` & `sqlx-exec-1.2.5/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.3/sqlexec/pooling.py` & `sqlx-exec-1.2.5/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.3/sqlexec/sql_support.py` & `sqlx-exec-1.2.5/sqlexec/sql_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import re
-from .engin import Engin
+from .engine import Engine
 from typing import Sequence
 from functools import lru_cache
 from .constant import CACHE_SIZE, NAMED_REGEX
 
 def insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
-    sql = Engin.create_insert_sql_intf(table, cols)
+    sql = Engine.create_insert_sql_intf(table, cols)
     return sql, args
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
 def batch_insert_sql_args(table: str, *args):
     args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
     cols, args = zip(*args)  # (cols), (args)
-    sql = Engin.create_insert_sql_intf(table, cols[0])
+    sql = Engine.create_insert_sql_intf(table, cols[0])
     return sql, args
 
 
 def batch_named_sql_args(sql: str, *args):
     args = get_batch_args(*args)
     args = [get_named_args(sql, **arg) for arg in args]
     sql = get_named_sql(sql)
```

### Comparing `sqlx-exec-1.2.3/sqlexec/support.py` & `sqlx-exec-1.2.5/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.3/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.2.5/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.3
+Version: 1.2.5
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
+       sqlexec.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

