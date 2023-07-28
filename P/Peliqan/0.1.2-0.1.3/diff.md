# Comparing `tmp/Peliqan-0.1.2.tar.gz` & `tmp/Peliqan-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-0.1.2.tar", last modified: Thu Jul 27 13:12:20 2023, max compression
+gzip compressed data, was "Peliqan-0.1.3.tar", last modified: Fri Jul 28 11:35:53 2023, max compression
```

## Comparing `Peliqan-0.1.2.tar` & `Peliqan-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-27 13:12:20.620772 Peliqan-0.1.2/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-27 13:12:20.620634 Peliqan-0.1.2/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-27 13:12:20.620336 Peliqan-0.1.2/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-07-27 13:05:47.000000 Peliqan-0.1.2/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-27 13:12:20.620439 Peliqan-0.1.2/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    38718 2023-07-27 13:10:58.000000 Peliqan-0.1.2/peliqan/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-07-27 13:12:20.620811 Peliqan-0.1.2/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-07-27 13:05:47.000000 Peliqan-0.1.2/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-28 11:35:53.300680 Peliqan-0.1.3/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-28 11:35:53.300561 Peliqan-0.1.3/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-28 11:35:53.300253 Peliqan-0.1.3/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-07-28 11:35:53.000000 Peliqan-0.1.3/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-07-28 06:15:32.000000 Peliqan-0.1.3/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-28 11:35:53.300358 Peliqan-0.1.3/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    40386 2023-07-28 07:29:22.000000 Peliqan-0.1.3/peliqan/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-07-28 11:35:53.300723 Peliqan-0.1.3/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-07-28 06:15:32.000000 Peliqan-0.1.3/setup.py
```

### Comparing `Peliqan-0.1.2/PKG-INFO` & `Peliqan-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.2/Peliqan.egg-info/PKG-INFO` & `Peliqan-0.1.3/Peliqan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.2/README.md` & `Peliqan-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-0.1.2/peliqan/__init__.py` & `Peliqan-0.1.3/peliqan/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 # import necessary modules
 import logging
 
 import pandas
@@ -493,24 +493,58 @@
            :param resource_id: id of the resource.
            :param resource_name: name of the resource.
            :param kwargs: additional kwargs can also be passed.
            :return: resource details as a dict.
         """
         return self.__service_client__.find_resource(resource_type, resource_id, resource_name, **kwargs)
 
+    def _to_dtype(self, column_type, tz):
+        if (
+            column_type[0:3].lower() == "int" or
+            column_type[0:3].lower() == "num" or
+            column_type[0:6].lower() == "bigint"
+        ):  # todo add more field types
+            type_name = int
+
+        elif (
+            column_type[0:6].lower() == "double" or
+            column_type[0:5].lower() == "float" or
+            column_type[0:7].lower() == "decimal"
+        ):
+            type_name = float
+
+        elif column_type == "date":
+            type_name = pd.DatetimeTZDtype(tz=tz)
+
+        elif column_type[0:9].lower() == "timestamp" or column_type[0:8].lower() == "datetime":
+            type_name = pd.DatetimeTZDtype(tz=tz)
+
+        elif column_type[0:4].lower() == "bool":
+            type_name = bool
+        else:
+            type_name = str
+
+        return type_name
+
     # todo allow user to set a PK column for the query (or update the guessed PK)
-    def load_table(self, table_name='', query='', table_id=None, fillna_with=''):
+    def load_table(self, table_name='', query='', table_id=None, fillna_with='', to_dict=False,
+                   enable_python_types=False, tz='UTC'):
         """
         Return the records in a table.
 
         :param table_name: The name of a table.
         :param query: A valid Trino sql query.
         :param table_id: An integer value that uniquely identifies a table.
         :param fillna_with: Replace empty value with a default placeholder.
         Pass None if empty values should not be replaced.
+        :param to_dict: Get the records as a list of python dicts.
+        :param enable_python_types: This flag will cause the record's values to be returned as python types
+        :param tz: This is the timezone that will be used to convert date and datetime strings
+        to timezone aware datetime objects. This value defaults to 'UTC'.
+
         :return:
         """
 
         # table_id will return the raw table data.
         # This causes multiple select and single select to be returned as json objects
 
         # query and table_name will return the data as if the queried table is a prepended statement.
@@ -528,24 +562,39 @@
         json_response = self.__service_client__.get_records(url_suffix)
 
         error = json_response['error']
         if error:
             raise PeliqanClientException(f"Client encountered a error while fetching records,\n{error}")
 
         records = json_response['records']
-        columns = json_response['columns']
+        column_data = json_response['columns']
+
+        columns = []
+        dtypes = []
+        for column in column_data:
+            dtypes.append((column[0], self._to_dtype(column[1], tz)))
+            columns.append(column[0])
 
         # Create dataframe
         df = pd.DataFrame(records, columns=columns)
+        if enable_python_types:
+            for dtype in dtypes:
+                df[dtype[0]] = df[dtype[0]].astype(dtype[1])
+
         if fillna_with is not None:
             # replace Na/NaN
             df.fillna(fillna_with, inplace=True)
             # replace NaT
-            df.replace({pandas.NaT: fillna_with}, inplace=True)
-        return df
+            df.replace({pandas.NaT: None}, inplace=True)
+
+        if to_dict:
+            return df.to_dict('records')
+
+        else:
+            return df
 
     # todo: make it easier to find table & field ids in UI
     def update_cell(self, row_pk, value, table_id=None, table_name=None, field_id=None, field_name=None):
         if not row_pk:
             raise PeliqanClientException("row_pk must be provided.")
 
         # BACKEND_URL and JWT are prepended to the generated script,
```

### Comparing `Peliqan-0.1.2/setup.py` & `Peliqan-0.1.3/setup.py`

 * *Files identical despite different names*

