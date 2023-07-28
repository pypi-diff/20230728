# Comparing `tmp/mysqlx-1.6.6.tar.gz` & `tmp/mysqlx-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.6.6.tar", last modified: Thu Jul 27 11:35:26 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.6.8.tar", last modified: Fri Jul 28 02:54:54 2023, max compression
```

## Comparing `mysqlx-1.6.6.tar` & `mysqlx-1.6.8.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:35:26.000000 mysqlx-1.6.6/
-drwxrwxrwx   0        0        0        0 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx/
--rw-rw-rw-   0        0        0      663 2023-07-27 04:34:07.000000 mysqlx-1.6.6/mysqlx/db.py
--rw-rw-rw-   0        0        0      570 2023-07-27 04:34:07.000000 mysqlx-1.6.6/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      761 2023-07-26 15:03:13.000000 mysqlx-1.6.6/mysqlx/engin.py
--rw-rw-rw-   0        0        0      414 2023-07-27 04:35:53.000000 mysqlx-1.6.6/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.6.6/mysqlx/orm.py
--rw-rw-rw-   0        0        0      339 2023-07-26 07:19:23.000000 mysqlx-1.6.6/mysqlx/sql_support.py
--rw-rw-rw-   0        0        0      488 2023-07-27 11:33:28.000000 mysqlx-1.6.6/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4511 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4511 2023-07-27 11:35:26.000000 mysqlx-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-27 11:35:26.000000 mysqlx-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-07-27 11:33:59.000000 mysqlx-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:54:54.000000 mysqlx-1.6.8/
+drwxrwxrwx   0        0        0        0 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx/
+-rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.6.8/mysqlx/db.py
+-rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.6.8/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.6.8/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.6.8/mysqlx/orm.py
+-rw-rw-rw-   0        0        0      491 2023-07-28 02:04:25.000000 mysqlx-1.6.8/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4511 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      279 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4511 2023-07-28 02:54:54.000000 mysqlx-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:54:54.000000 mysqlx-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-07-28 02:54:38.000000 mysqlx-1.6.8/setup.py
```

### Comparing `mysqlx-1.6.6/mysqlx/db.py` & `mysqlx-1.6.8/mysqlx/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import MySqlEngin
+from . import MySqlEngine
 from .log_support import save_log
 
 # Don't remove. Import for not repetitive implementation
 from sqlbatis.db import insert, save_select_key, execute, batch_insert, batch_execute, get, query, query_one, select, select_one, do_execute,\
     do_get, do_query, do_query_one, do_select, do_select_one, do_query_page, do_select_page, query_page, select_page
 
 
@@ -10,8 +10,8 @@
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
     :return: Primary key
     """
     save_log(table, **kwargs)
-    return save_select_key(MySqlEngin.get_select_key(), table, **kwargs)
+    return save_select_key(MySqlEngine.get_select_key(), table, **kwargs)
```

### Comparing `mysqlx-1.6.6/mysqlx/dbx.py` & `mysqlx-1.6.8/mysqlx/dbx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from .engin import MySqlEngin
+from . import MySqlEngine
 from .log_support import sql_id_log
 from sqlbatis import sql_holder as holder
-from sqlbatis.dbx import insert, save_sql, batch_insert, batch_execute, execute, get, query, query_one, select, select_one
+from sqlbatis.dbx import insert, save_select_key, batch_insert, batch_execute, execute, get, query, query_one, select, select_one
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
-    sql_id_log('dbx.save', sql_id, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    select_key = MySqlEngin.get_select_key()
-    return save_sql(select_key, sql, *args)
+    sql_id_log('save', sql_id, *args, **kwargs)
+
+    select_key = MySqlEngine.get_select_key()
+    return save_select_key(select_key, sql_id, *args, **kwargs)
```

### Comparing `mysqlx-1.6.6/mysqlx/orm.py` & `mysqlx-1.6.8/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.6/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.6.8/mysqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.6
+Version: 1.6.8
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.6/PKG-INFO` & `mysqlx-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.6
+Version: 1.6.8
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.6/README.rst` & `mysqlx-1.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.6/setup.py` & `mysqlx-1.6.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
-        'sqlx-batis>=0.1.0',
+        'sqlx-batis>=0.1.1',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.6.6',
+    version='1.6.8',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

