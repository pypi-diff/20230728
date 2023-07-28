# Comparing `tmp/apache-iotdb-1.1.0.tar.gz` & `tmp/apache-iotdb-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-iotdb-1.1.0.tar", last modified: Tue Apr  4 01:53:59 2023, max compression
+gzip compressed data, was "apache-iotdb-1.1.2.tar", last modified: Fri Jul 28 10:30:59 2023, max compression
```

## Comparing `apache-iotdb-1.1.0.tar` & `apache-iotdb-1.1.2.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.528191 apache-iotdb-1.1.0/
--rw-r--r--   0 ht         (501) staff       (20)    16125 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/LICENSE
--rw-r--r--   0 ht         (501) staff       (20)    21336 2023-04-04 01:53:59.527989 apache-iotdb-1.1.0/PKG-INFO
--rw-r--r--   0 ht         (501) staff       (20)    20724 2023-03-09 08:17:43.000000 apache-iotdb-1.1.0/README.md
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.513339 apache-iotdb-1.1.0/apache_iotdb.egg-info/
--rw-r--r--   0 ht         (501) staff       (20)    21336 2023-04-04 01:53:59.000000 apache-iotdb-1.1.0/apache_iotdb.egg-info/PKG-INFO
--rw-r--r--   0 ht         (501) staff       (20)     2146 2023-04-04 01:53:59.000000 apache-iotdb-1.1.0/apache_iotdb.egg-info/SOURCES.txt
--rw-r--r--   0 ht         (501) staff       (20)        1 2023-04-04 01:53:59.000000 apache-iotdb-1.1.0/apache_iotdb.egg-info/dependency_links.txt
--rw-r--r--   0 ht         (501) staff       (20)       73 2023-04-04 01:53:59.000000 apache-iotdb-1.1.0/apache_iotdb.egg-info/entry_points.txt
--rw-r--r--   0 ht         (501) staff       (20)      137 2023-04-04 01:53:59.000000 apache-iotdb-1.1.0/apache_iotdb.egg-info/requires.txt
--rw-r--r--   0 ht         (501) staff       (20)       12 2023-04-04 01:53:59.000000 apache-iotdb-1.1.0/apache_iotdb.egg-info/top_level.txt
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.514377 apache-iotdb-1.1.0/iotdb/
--rw-r--r--   0 ht         (501) staff       (20)     1719 2022-04-13 08:47:20.000000 apache-iotdb-1.1.0/iotdb/IoTDBContainer.py
--rw-r--r--   0 ht         (501) staff       (20)    56618 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/iotdb/Session.py
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-04-13 08:47:20.000000 apache-iotdb-1.1.0/iotdb/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.515215 apache-iotdb-1.1.0/iotdb/dbapi/
--rw-r--r--   0 ht         (501) staff       (20)     2569 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/dbapi/Connection.py
--rw-r--r--   0 ht         (501) staff       (20)     9110 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/dbapi/Cursor.py
--rw-r--r--   0 ht         (501) staff       (20)     1278 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/dbapi/Exceptions.py
--rw-r--r--   0 ht         (501) staff       (20)      953 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/dbapi/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.516096 apache-iotdb-1.1.0/iotdb/dbapi/tests/
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/dbapi/tests/__init__.py
--rw-r--r--   0 ht         (501) staff       (20)     1689 2023-03-09 03:30:14.000000 apache-iotdb-1.1.0/iotdb/dbapi/tests/test_connection.py
--rw-r--r--   0 ht         (501) staff       (20)     3943 2023-03-09 03:30:14.000000 apache-iotdb-1.1.0/iotdb/dbapi/tests/test_cursor.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.517333 apache-iotdb-1.1.0/iotdb/sqlalchemy/
--rw-r--r--   0 ht         (501) staff       (20)     4557 2023-01-10 02:03:17.000000 apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBDialect.py
--rw-r--r--   0 ht         (501) staff       (20)     1089 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBIdentifierPreparer.py
--rw-r--r--   0 ht         (501) staff       (20)     8700 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBSQLCompiler.py
--rw-r--r--   0 ht         (501) staff       (20)     1416 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBTypeCompiler.py
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/sqlalchemy/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.517609 apache-iotdb-1.1.0/iotdb/sqlalchemy/tests/
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/sqlalchemy/tests/__init__.py
--rw-r--r--   0 ht         (501) staff       (20)     3083 2023-03-09 08:17:43.000000 apache-iotdb-1.1.0/iotdb/sqlalchemy/tests/test_dialect.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.518566 apache-iotdb-1.1.0/iotdb/template/
--rw-r--r--   0 ht         (501) staff       (20)     1417 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/template/InternalNode.py
--rw-r--r--   0 ht         (501) staff       (20)     2012 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/template/MeasurementNode.py
--rw-r--r--   0 ht         (501) staff       (20)     3378 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/template/Template.py
--rw-r--r--   0 ht         (501) staff       (20)     1309 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/template/TemplateNode.py
--rw-r--r--   0 ht         (501) staff       (20)     1272 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/template/TemplateQueryType.py
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/template/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.518694 apache-iotdb-1.1.0/iotdb/thrift/
--rw-r--r--   0 ht         (501) staff       (20)        0 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.519199 apache-iotdb-1.1.0/iotdb/thrift/common/
--rw-r--r--   0 ht         (501) staff       (20)       34 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/common/__init__.py
--rw-r--r--   0 ht         (501) staff       (20)      366 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/common/constants.py
--rw-r--r--   0 ht         (501) staff       (20)    52118 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/common/ttypes.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.520832 apache-iotdb-1.1.0/iotdb/thrift/datanode/
--rw-r--r--   0 ht         (501) staff       (20)   380654 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/datanode/IDataNodeRPCService.py
--rw-r--r--   0 ht         (501) staff       (20)    29452 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/datanode/MPPDataExchangeService.py
--rw-r--r--   0 ht         (501) staff       (20)       83 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/datanode/__init__.py
--rw-r--r--   0 ht         (501) staff       (20)      366 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/datanode/constants.py
--rw-r--r--   0 ht         (501) staff       (20)   243098 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/datanode/ttypes.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.522172 apache-iotdb-1.1.0/iotdb/thrift/rpc/
--rw-r--r--   0 ht         (501) staff       (20)   366271 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/rpc/IClientRPCService.py
--rw-r--r--   0 ht         (501) staff       (20)       55 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/rpc/__init__.py
--rw-r--r--   0 ht         (501) staff       (20)      366 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/rpc/constants.py
--rw-r--r--   0 ht         (501) staff       (20)   263370 2023-04-04 01:21:14.000000 apache-iotdb-1.1.0/iotdb/thrift/rpc/ttypes.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.522522 apache-iotdb-1.1.0/iotdb/tsfile/
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/tsfile/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.522741 apache-iotdb-1.1.0/iotdb/tsfile/common/
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/tsfile/common/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.523126 apache-iotdb-1.1.0/iotdb/tsfile/common/constant/
--rw-r--r--   0 ht         (501) staff       (20)     1173 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/tsfile/common/constant/TsFileConstant.py
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/tsfile/common/constant/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.523532 apache-iotdb-1.1.0/iotdb/tsfile/utils/
--rw-r--r--   0 ht         (501) staff       (20)      952 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/tsfile/utils/Pair.py
--rw-r--r--   0 ht         (501) staff       (20)     2953 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/tsfile/utils/ReadWriteIOUtils.py
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-12-20 01:03:48.000000 apache-iotdb-1.1.0/iotdb/tsfile/utils/__init__.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.525812 apache-iotdb-1.1.0/iotdb/utils/
--rw-r--r--   0 ht         (501) staff       (20)     1436 2023-03-09 08:17:43.000000 apache-iotdb-1.1.0/iotdb/utils/BitMap.py
--rw-r--r--   0 ht         (501) staff       (20)     6228 2022-04-13 08:47:20.000000 apache-iotdb-1.1.0/iotdb/utils/Field.py
--rw-r--r--   0 ht         (501) staff       (20)     2370 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/iotdb/utils/IoTDBConstants.py
--rw-r--r--   0 ht         (501) staff       (20)    16617 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/iotdb/utils/IoTDBRpcDataSet.py
--rw-r--r--   0 ht         (501) staff       (20)     6024 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/iotdb/utils/NumpyTablet.py
--rw-r--r--   0 ht         (501) staff       (20)     1750 2022-04-13 08:47:20.000000 apache-iotdb-1.1.0/iotdb/utils/RowRecord.py
--rw-r--r--   0 ht         (501) staff       (20)     6008 2022-12-14 01:44:00.000000 apache-iotdb-1.1.0/iotdb/utils/SessionDataSet.py
--rw-r--r--   0 ht         (501) staff       (20)     8129 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/iotdb/utils/Tablet.py
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-04-13 08:47:20.000000 apache-iotdb-1.1.0/iotdb/utils/__init__.py
--rw-r--r--   0 ht         (501) staff       (20)     1285 2022-04-13 08:47:20.000000 apache-iotdb-1.1.0/pyproject.toml
--rw-r--r--   0 ht         (501) staff       (20)       38 2023-04-04 01:53:59.528226 apache-iotdb-1.1.0/setup.cfg
--rw-r--r--   0 ht         (501) staff       (20)     2198 2023-04-04 01:51:46.000000 apache-iotdb-1.1.0/setup.py
-drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-04-04 01:53:59.527730 apache-iotdb-1.1.0/tests/
--rw-r--r--   0 ht         (501) staff       (20)      789 2022-04-13 08:47:20.000000 apache-iotdb-1.1.0/tests/__init__.py
--rw-r--r--   0 ht         (501) staff       (20)    10732 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/tests/tablet_performance_comparison.py
--rw-r--r--   0 ht         (501) staff       (20)     9910 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/tests/test_aligned_timeseries.py
--rw-r--r--   0 ht         (501) staff       (20)     2743 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/tests/test_dataframe.py
--rw-r--r--   0 ht         (501) staff       (20)     5077 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/tests/test_delete_data.py
--rw-r--r--   0 ht         (501) staff       (20)     7194 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/tests/test_numpy_tablet.py
--rw-r--r--   0 ht         (501) staff       (20)     4734 2023-03-09 03:30:14.000000 apache-iotdb-1.1.0/tests/test_one_device.py
--rw-r--r--   0 ht         (501) staff       (20)    13643 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/tests/test_session.py
--rw-r--r--   0 ht         (501) staff       (20)     4194 2023-01-10 02:03:17.000000 apache-iotdb-1.1.0/tests/test_tablet.py
--rw-r--r--   0 ht         (501) staff       (20)     3955 2023-04-03 08:38:06.000000 apache-iotdb-1.1.0/tests/test_template.py
--rw-r--r--   0 ht         (501) staff       (20)     8071 2023-03-09 08:17:43.000000 apache-iotdb-1.1.0/tests/test_todf.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.932989 apache-iotdb-1.1.2/
+-rw-r--r--   0 ht         (501) staff       (20)    16125 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/LICENSE
+-rw-r--r--   0 ht         (501) staff       (20)    21336 2023-07-28 10:30:59.932749 apache-iotdb-1.1.2/PKG-INFO
+-rw-r--r--   0 ht         (501) staff       (20)    20724 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/README.md
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.923536 apache-iotdb-1.1.2/apache_iotdb.egg-info/
+-rw-r--r--   0 ht         (501) staff       (20)    21336 2023-07-28 10:30:59.000000 apache-iotdb-1.1.2/apache_iotdb.egg-info/PKG-INFO
+-rw-r--r--   0 ht         (501) staff       (20)     2194 2023-07-28 10:30:59.000000 apache-iotdb-1.1.2/apache_iotdb.egg-info/SOURCES.txt
+-rw-r--r--   0 ht         (501) staff       (20)        1 2023-07-28 10:30:59.000000 apache-iotdb-1.1.2/apache_iotdb.egg-info/dependency_links.txt
+-rw-r--r--   0 ht         (501) staff       (20)       73 2023-07-28 10:30:59.000000 apache-iotdb-1.1.2/apache_iotdb.egg-info/entry_points.txt
+-rw-r--r--   0 ht         (501) staff       (20)      137 2023-07-28 10:30:59.000000 apache-iotdb-1.1.2/apache_iotdb.egg-info/requires.txt
+-rw-r--r--   0 ht         (501) staff       (20)       12 2023-07-28 10:30:59.000000 apache-iotdb-1.1.2/apache_iotdb.egg-info/top_level.txt
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.924013 apache-iotdb-1.1.2/iotdb/
+-rw-r--r--   0 ht         (501) staff       (20)     1719 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/IoTDBContainer.py
+-rw-r--r--   0 ht         (501) staff       (20)    56618 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/Session.py
+-rw-r--r--   0 ht         (501) staff       (20)     4542 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/SessionPool.py
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.924460 apache-iotdb-1.1.2/iotdb/dbapi/
+-rw-r--r--   0 ht         (501) staff       (20)     2569 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/dbapi/Connection.py
+-rw-r--r--   0 ht         (501) staff       (20)     9110 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/dbapi/Cursor.py
+-rw-r--r--   0 ht         (501) staff       (20)     1278 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/dbapi/Exceptions.py
+-rw-r--r--   0 ht         (501) staff       (20)      953 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/dbapi/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.924805 apache-iotdb-1.1.2/iotdb/dbapi/tests/
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/dbapi/tests/__init__.py
+-rw-r--r--   0 ht         (501) staff       (20)     1689 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/dbapi/tests/test_connection.py
+-rw-r--r--   0 ht         (501) staff       (20)     3943 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/dbapi/tests/test_cursor.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.925393 apache-iotdb-1.1.2/iotdb/sqlalchemy/
+-rw-r--r--   0 ht         (501) staff       (20)     4557 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBDialect.py
+-rw-r--r--   0 ht         (501) staff       (20)     1089 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBIdentifierPreparer.py
+-rw-r--r--   0 ht         (501) staff       (20)     8700 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBSQLCompiler.py
+-rw-r--r--   0 ht         (501) staff       (20)     1416 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBTypeCompiler.py
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/sqlalchemy/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.925621 apache-iotdb-1.1.2/iotdb/sqlalchemy/tests/
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/sqlalchemy/tests/__init__.py
+-rw-r--r--   0 ht         (501) staff       (20)     3083 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/sqlalchemy/tests/test_dialect.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.926290 apache-iotdb-1.1.2/iotdb/template/
+-rw-r--r--   0 ht         (501) staff       (20)     1417 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/template/InternalNode.py
+-rw-r--r--   0 ht         (501) staff       (20)     2012 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/template/MeasurementNode.py
+-rw-r--r--   0 ht         (501) staff       (20)     3378 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/template/Template.py
+-rw-r--r--   0 ht         (501) staff       (20)     1309 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/template/TemplateNode.py
+-rw-r--r--   0 ht         (501) staff       (20)     1272 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/template/TemplateQueryType.py
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/template/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.926402 apache-iotdb-1.1.2/iotdb/thrift/
+-rw-r--r--   0 ht         (501) staff       (20)        0 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.927018 apache-iotdb-1.1.2/iotdb/thrift/common/
+-rw-r--r--   0 ht         (501) staff       (20)       34 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/common/__init__.py
+-rw-r--r--   0 ht         (501) staff       (20)      366 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/common/constants.py
+-rw-r--r--   0 ht         (501) staff       (20)    52118 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/common/ttypes.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.928020 apache-iotdb-1.1.2/iotdb/thrift/datanode/
+-rw-r--r--   0 ht         (501) staff       (20)   380818 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/datanode/IDataNodeRPCService.py
+-rw-r--r--   0 ht         (501) staff       (20)    29452 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/datanode/MPPDataExchangeService.py
+-rw-r--r--   0 ht         (501) staff       (20)       83 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/datanode/__init__.py
+-rw-r--r--   0 ht         (501) staff       (20)      366 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/datanode/constants.py
+-rw-r--r--   0 ht         (501) staff       (20)   250773 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/datanode/ttypes.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.929017 apache-iotdb-1.1.2/iotdb/thrift/rpc/
+-rw-r--r--   0 ht         (501) staff       (20)   373011 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/rpc/IClientRPCService.py
+-rw-r--r--   0 ht         (501) staff       (20)       55 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/rpc/__init__.py
+-rw-r--r--   0 ht         (501) staff       (20)      366 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/rpc/constants.py
+-rw-r--r--   0 ht         (501) staff       (20)   268322 2023-07-28 10:29:49.000000 apache-iotdb-1.1.2/iotdb/thrift/rpc/ttypes.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.929328 apache-iotdb-1.1.2/iotdb/tsfile/
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/tsfile/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.929454 apache-iotdb-1.1.2/iotdb/tsfile/common/
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/tsfile/common/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.929683 apache-iotdb-1.1.2/iotdb/tsfile/common/constant/
+-rw-r--r--   0 ht         (501) staff       (20)     1173 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/tsfile/common/constant/TsFileConstant.py
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/tsfile/common/constant/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.930028 apache-iotdb-1.1.2/iotdb/tsfile/utils/
+-rw-r--r--   0 ht         (501) staff       (20)      952 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/tsfile/utils/Pair.py
+-rw-r--r--   0 ht         (501) staff       (20)     2953 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/tsfile/utils/ReadWriteIOUtils.py
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/tsfile/utils/__init__.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.931115 apache-iotdb-1.1.2/iotdb/utils/
+-rw-r--r--   0 ht         (501) staff       (20)     1436 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/BitMap.py
+-rw-r--r--   0 ht         (501) staff       (20)     6228 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/Field.py
+-rw-r--r--   0 ht         (501) staff       (20)     2383 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/IoTDBConstants.py
+-rw-r--r--   0 ht         (501) staff       (20)    16617 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/IoTDBRpcDataSet.py
+-rw-r--r--   0 ht         (501) staff       (20)     6024 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/NumpyTablet.py
+-rw-r--r--   0 ht         (501) staff       (20)     1750 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/RowRecord.py
+-rw-r--r--   0 ht         (501) staff       (20)     6008 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/SessionDataSet.py
+-rw-r--r--   0 ht         (501) staff       (20)     8129 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/Tablet.py
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/iotdb/utils/__init__.py
+-rw-r--r--   0 ht         (501) staff       (20)     1285 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/pyproject.toml
+-rw-r--r--   0 ht         (501) staff       (20)       38 2023-07-28 10:30:59.933024 apache-iotdb-1.1.2/setup.cfg
+-rw-r--r--   0 ht         (501) staff       (20)     2198 2023-07-28 10:30:50.000000 apache-iotdb-1.1.2/setup.py
+drwxr-xr-x   0 ht         (501) staff       (20)        0 2023-07-28 10:30:59.932539 apache-iotdb-1.1.2/tests/
+-rw-r--r--   0 ht         (501) staff       (20)      789 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/__init__.py
+-rw-r--r--   0 ht         (501) staff       (20)    10732 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/tablet_performance_comparison.py
+-rw-r--r--   0 ht         (501) staff       (20)     9910 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_aligned_timeseries.py
+-rw-r--r--   0 ht         (501) staff       (20)     2743 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_dataframe.py
+-rw-r--r--   0 ht         (501) staff       (20)     5077 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_delete_data.py
+-rw-r--r--   0 ht         (501) staff       (20)     7194 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_numpy_tablet.py
+-rw-r--r--   0 ht         (501) staff       (20)     4734 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_one_device.py
+-rw-r--r--   0 ht         (501) staff       (20)    14251 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_session.py
+-rw-r--r--   0 ht         (501) staff       (20)     2484 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_session_pool.py
+-rw-r--r--   0 ht         (501) staff       (20)     4194 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_tablet.py
+-rw-r--r--   0 ht         (501) staff       (20)     3955 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_template.py
+-rw-r--r--   0 ht         (501) staff       (20)     8071 2023-07-28 10:26:52.000000 apache-iotdb-1.1.2/tests/test_todf.py
```

### Comparing `apache-iotdb-1.1.0/LICENSE` & `apache-iotdb-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/PKG-INFO` & `apache-iotdb-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-iotdb
-Version: 1.1.0
+Version: 1.1.2
 Summary: Apache IoTDB client API
 Home-page: https://github.com/apache/iotdb
 Author:  Apache Software Foundation
 Author-email: dev@iotdb.apache.org
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `apache-iotdb-1.1.0/README.md` & `apache-iotdb-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/apache_iotdb.egg-info/PKG-INFO` & `apache-iotdb-1.1.2/apache_iotdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-iotdb
-Version: 1.1.0
+Version: 1.1.2
 Summary: Apache IoTDB client API
 Home-page: https://github.com/apache/iotdb
 Author:  Apache Software Foundation
 Author-email: dev@iotdb.apache.org
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `apache-iotdb-1.1.0/apache_iotdb.egg-info/SOURCES.txt` & `apache-iotdb-1.1.2/apache_iotdb.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 apache_iotdb.egg-info/SOURCES.txt
 apache_iotdb.egg-info/dependency_links.txt
 apache_iotdb.egg-info/entry_points.txt
 apache_iotdb.egg-info/requires.txt
 apache_iotdb.egg-info/top_level.txt
 iotdb/IoTDBContainer.py
 iotdb/Session.py
+iotdb/SessionPool.py
 iotdb/__init__.py
 iotdb/dbapi/Connection.py
 iotdb/dbapi/Cursor.py
 iotdb/dbapi/Exceptions.py
 iotdb/dbapi/__init__.py
 iotdb/dbapi/tests/__init__.py
 iotdb/dbapi/tests/test_connection.py
@@ -64,10 +65,11 @@
 tests/tablet_performance_comparison.py
 tests/test_aligned_timeseries.py
 tests/test_dataframe.py
 tests/test_delete_data.py
 tests/test_numpy_tablet.py
 tests/test_one_device.py
 tests/test_session.py
+tests/test_session_pool.py
 tests/test_tablet.py
 tests/test_template.py
 tests/test_todf.py
```

### Comparing `apache-iotdb-1.1.0/iotdb/IoTDBContainer.py` & `apache-iotdb-1.1.2/iotdb/IoTDBContainer.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/Session.py` & `apache-iotdb-1.1.2/iotdb/Session.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/__init__.py` & `apache-iotdb-1.1.2/iotdb/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/dbapi/Connection.py` & `apache-iotdb-1.1.2/iotdb/dbapi/Connection.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/dbapi/Cursor.py` & `apache-iotdb-1.1.2/iotdb/dbapi/Cursor.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/dbapi/Exceptions.py` & `apache-iotdb-1.1.2/iotdb/dbapi/Exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/dbapi/__init__.py` & `apache-iotdb-1.1.2/iotdb/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/dbapi/tests/__init__.py` & `apache-iotdb-1.1.2/iotdb/dbapi/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/dbapi/tests/test_connection.py` & `apache-iotdb-1.1.2/iotdb/dbapi/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/dbapi/tests/test_cursor.py` & `apache-iotdb-1.1.2/iotdb/dbapi/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBDialect.py` & `apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBDialect.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBIdentifierPreparer.py` & `apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBIdentifierPreparer.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBSQLCompiler.py` & `apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBSQLCompiler.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/sqlalchemy/IoTDBTypeCompiler.py` & `apache-iotdb-1.1.2/iotdb/sqlalchemy/IoTDBTypeCompiler.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/sqlalchemy/__init__.py` & `apache-iotdb-1.1.2/iotdb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/sqlalchemy/tests/__init__.py` & `apache-iotdb-1.1.2/iotdb/sqlalchemy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/sqlalchemy/tests/test_dialect.py` & `apache-iotdb-1.1.2/iotdb/sqlalchemy/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/template/InternalNode.py` & `apache-iotdb-1.1.2/iotdb/template/InternalNode.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/template/MeasurementNode.py` & `apache-iotdb-1.1.2/iotdb/template/MeasurementNode.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/template/Template.py` & `apache-iotdb-1.1.2/iotdb/template/Template.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/template/TemplateNode.py` & `apache-iotdb-1.1.2/iotdb/template/TemplateNode.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/template/TemplateQueryType.py` & `apache-iotdb-1.1.2/iotdb/template/TemplateQueryType.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/template/__init__.py` & `apache-iotdb-1.1.2/iotdb/template/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/thrift/common/ttypes.py` & `apache-iotdb-1.1.2/iotdb/thrift/common/ttypes.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/thrift/datanode/IDataNodeRPCService.py` & `apache-iotdb-1.1.2/iotdb/thrift/datanode/IDataNodeRPCService.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
         Parameters:
          - req
 
         """
         pass
 
-    def sendPlanNode(self, req):
+    def sendBatchPlanNode(self, req):
         """
-        dispatch PlanNode to remote node for write request in order to save resource
+        dispatch PlanNodes in batches to remote node for write request in order to save resource
 
         Parameters:
          - req
 
         """
         pass
 
@@ -669,47 +669,47 @@
         result = sendFragmentInstance_result()
         result.read(iprot)
         iprot.readMessageEnd()
         if result.success is not None:
             return result.success
         raise TApplicationException(TApplicationException.MISSING_RESULT, "sendFragmentInstance failed: unknown result")
 
-    def sendPlanNode(self, req):
+    def sendBatchPlanNode(self, req):
         """
-        dispatch PlanNode to remote node for write request in order to save resource
+        dispatch PlanNodes in batches to remote node for write request in order to save resource
 
         Parameters:
          - req
 
         """
-        self.send_sendPlanNode(req)
-        return self.recv_sendPlanNode()
+        self.send_sendBatchPlanNode(req)
+        return self.recv_sendBatchPlanNode()
 
-    def send_sendPlanNode(self, req):
-        self._oprot.writeMessageBegin('sendPlanNode', TMessageType.CALL, self._seqid)
-        args = sendPlanNode_args()
+    def send_sendBatchPlanNode(self, req):
+        self._oprot.writeMessageBegin('sendBatchPlanNode', TMessageType.CALL, self._seqid)
+        args = sendBatchPlanNode_args()
         args.req = req
         args.write(self._oprot)
         self._oprot.writeMessageEnd()
         self._oprot.trans.flush()
 
-    def recv_sendPlanNode(self):
+    def recv_sendBatchPlanNode(self):
         iprot = self._iprot
         (fname, mtype, rseqid) = iprot.readMessageBegin()
         if mtype == TMessageType.EXCEPTION:
             x = TApplicationException()
             x.read(iprot)
             iprot.readMessageEnd()
             raise x
-        result = sendPlanNode_result()
+        result = sendBatchPlanNode_result()
         result.read(iprot)
         iprot.readMessageEnd()
         if result.success is not None:
             return result.success
-        raise TApplicationException(TApplicationException.MISSING_RESULT, "sendPlanNode failed: unknown result")
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "sendBatchPlanNode failed: unknown result")
 
     def fetchFragmentInstanceInfo(self, req):
         """
         Parameters:
          - req
 
         """
@@ -2689,15 +2689,15 @@
 
 
 class Processor(Iface, TProcessor):
     def __init__(self, handler):
         self._handler = handler
         self._processMap = {}
         self._processMap["sendFragmentInstance"] = Processor.process_sendFragmentInstance
-        self._processMap["sendPlanNode"] = Processor.process_sendPlanNode
+        self._processMap["sendBatchPlanNode"] = Processor.process_sendBatchPlanNode
         self._processMap["fetchFragmentInstanceInfo"] = Processor.process_fetchFragmentInstanceInfo
         self._processMap["cancelQuery"] = Processor.process_cancelQuery
         self._processMap["cancelPlanFragment"] = Processor.process_cancelPlanFragment
         self._processMap["cancelFragmentInstance"] = Processor.process_cancelFragmentInstance
         self._processMap["fetchSchema"] = Processor.process_fetchSchema
         self._processMap["sendTsFilePieceNode"] = Processor.process_sendTsFilePieceNode
         self._processMap["sendLoadCommand"] = Processor.process_sendLoadCommand
@@ -2793,33 +2793,33 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("sendFragmentInstance", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
-    def process_sendPlanNode(self, seqid, iprot, oprot):
-        args = sendPlanNode_args()
+    def process_sendBatchPlanNode(self, seqid, iprot, oprot):
+        args = sendBatchPlanNode_args()
         args.read(iprot)
         iprot.readMessageEnd()
-        result = sendPlanNode_result()
+        result = sendBatchPlanNode_result()
         try:
-            result.success = self._handler.sendPlanNode(args.req)
+            result.success = self._handler.sendBatchPlanNode(args.req)
             msg_type = TMessageType.REPLY
         except TTransport.TTransportException:
             raise
         except TApplicationException as ex:
             logging.exception('TApplication exception in handler')
             msg_type = TMessageType.EXCEPTION
             result = ex
         except Exception:
             logging.exception('Unexpected exception in handler')
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
-        oprot.writeMessageBegin("sendPlanNode", msg_type, seqid)
+        oprot.writeMessageBegin("sendBatchPlanNode", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
     def process_fetchFragmentInstanceInfo(self, seqid, iprot, oprot):
         args = fetchFragmentInstanceInfo_args()
         args.read(iprot)
@@ -4275,15 +4275,15 @@
         return not (self == other)
 all_structs.append(sendFragmentInstance_result)
 sendFragmentInstance_result.thrift_spec = (
     (0, TType.STRUCT, 'success', [TSendFragmentInstanceResp, None], None, ),  # 0
 )
 
 
-class sendPlanNode_args(object):
+class sendBatchPlanNode_args(object):
     """
     Attributes:
      - req
 
     """
 
 
@@ -4297,28 +4297,28 @@
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == -1:
                 if ftype == TType.STRUCT:
-                    self.req = TSendPlanNodeReq()
+                    self.req = TSendBatchPlanNodeReq()
                     self.req.read(iprot)
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('sendPlanNode_args')
+        oprot.writeStructBegin('sendBatchPlanNode_args')
         if self.req is not None:
             oprot.writeFieldBegin('req', TType.STRUCT, -1)
             self.req.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
@@ -4331,19 +4331,19 @@
         return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
-all_structs.append(sendPlanNode_args)
-sendPlanNode_args.thrift_spec = ()
+all_structs.append(sendBatchPlanNode_args)
+sendBatchPlanNode_args.thrift_spec = ()
 
 
-class sendPlanNode_result(object):
+class sendBatchPlanNode_result(object):
     """
     Attributes:
      - success
 
     """
 
 
@@ -4357,28 +4357,28 @@
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.STRUCT:
-                    self.success = TSendPlanNodeResp()
+                    self.success = TSendBatchPlanNodeResp()
                     self.success.read(iprot)
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('sendPlanNode_result')
+        oprot.writeStructBegin('sendBatchPlanNode_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.STRUCT, 0)
             self.success.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
@@ -4391,17 +4391,17 @@
         return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
-all_structs.append(sendPlanNode_result)
-sendPlanNode_result.thrift_spec = (
-    (0, TType.STRUCT, 'success', [TSendPlanNodeResp, None], None, ),  # 0
+all_structs.append(sendBatchPlanNode_result)
+sendBatchPlanNode_result.thrift_spec = (
+    (0, TType.STRUCT, 'success', [TSendBatchPlanNodeResp, None], None, ),  # 0
 )
 
 
 class fetchFragmentInstanceInfo_args(object):
     """
     Attributes:
      - req
```

### Comparing `apache-iotdb-1.1.0/iotdb/thrift/datanode/MPPDataExchangeService.py` & `apache-iotdb-1.1.2/iotdb/thrift/datanode/MPPDataExchangeService.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/thrift/datanode/ttypes.py` & `apache-iotdb-1.1.2/iotdb/thrift/datanode/ttypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1400,15 +1400,15 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class TSendPlanNodeReq(object):
+class TSendSinglePlanNodeReq(object):
     """
     Attributes:
      - planNode
      - consensusGroupId
 
     """
 
@@ -1443,15 +1443,15 @@
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('TSendPlanNodeReq')
+        oprot.writeStructBegin('TSendSinglePlanNodeReq')
         if self.planNode is not None:
             oprot.writeFieldBegin('planNode', TType.STRUCT, 1)
             self.planNode.write(oprot)
             oprot.writeFieldEnd()
         if self.consensusGroupId is not None:
             oprot.writeFieldBegin('consensusGroupId', TType.STRUCT, 2)
             self.consensusGroupId.write(oprot)
@@ -1474,15 +1474,15 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class TSendPlanNodeResp(object):
+class TSendSinglePlanNodeResp(object):
     """
     Attributes:
      - accepted
      - message
      - status
 
     """
@@ -1523,15 +1523,15 @@
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('TSendPlanNodeResp')
+        oprot.writeStructBegin('TSendSinglePlanNodeResp')
         if self.accepted is not None:
             oprot.writeFieldBegin('accepted', TType.BOOL, 1)
             oprot.writeBool(self.accepted)
             oprot.writeFieldEnd()
         if self.message is not None:
             oprot.writeFieldBegin('message', TType.STRING, 2)
             oprot.writeString(self.message.encode('utf-8') if sys.version_info[0] == 2 else self.message)
@@ -1556,14 +1556,150 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class TSendBatchPlanNodeReq(object):
+    """
+    Attributes:
+     - requests
+
+    """
+
+
+    def __init__(self, requests=None,):
+        self.requests = requests
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.LIST:
+                    self.requests = []
+                    (_etype24, _size21) = iprot.readListBegin()
+                    for _i25 in range(_size21):
+                        _elem26 = TSendSinglePlanNodeReq()
+                        _elem26.read(iprot)
+                        self.requests.append(_elem26)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('TSendBatchPlanNodeReq')
+        if self.requests is not None:
+            oprot.writeFieldBegin('requests', TType.LIST, 1)
+            oprot.writeListBegin(TType.STRUCT, len(self.requests))
+            for iter27 in self.requests:
+                iter27.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        if self.requests is None:
+            raise TProtocolException(message='Required field requests is unset!')
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class TSendBatchPlanNodeResp(object):
+    """
+    Attributes:
+     - responses
+
+    """
+
+
+    def __init__(self, responses=None,):
+        self.responses = responses
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.LIST:
+                    self.responses = []
+                    (_etype31, _size28) = iprot.readListBegin()
+                    for _i32 in range(_size28):
+                        _elem33 = TSendSinglePlanNodeResp()
+                        _elem33.read(iprot)
+                        self.responses.append(_elem33)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('TSendBatchPlanNodeResp')
+        if self.responses is not None:
+            oprot.writeFieldBegin('responses', TType.LIST, 1)
+            oprot.writeListBegin(TType.STRUCT, len(self.responses))
+            for iter34 in self.responses:
+                iter34.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        if self.responses is None:
+            raise TProtocolException(message='Required field responses is unset!')
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class TFetchFragmentInstanceInfoReq(object):
     """
     Attributes:
      - fragmentInstanceId
 
     """
 
@@ -1655,28 +1791,28 @@
                 if ftype == TType.I64:
                     self.endTime = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.failedMessages = []
-                    (_etype24, _size21) = iprot.readListBegin()
-                    for _i25 in range(_size21):
-                        _elem26 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.failedMessages.append(_elem26)
+                    (_etype38, _size35) = iprot.readListBegin()
+                    for _i39 in range(_size35):
+                        _elem40 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.failedMessages.append(_elem40)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.failureInfoList = []
-                    (_etype30, _size27) = iprot.readListBegin()
-                    for _i31 in range(_size27):
-                        _elem32 = iprot.readBinary()
-                        self.failureInfoList.append(_elem32)
+                    (_etype44, _size41) = iprot.readListBegin()
+                    for _i45 in range(_size41):
+                        _elem46 = iprot.readBinary()
+                        self.failureInfoList.append(_elem46)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -1693,23 +1829,23 @@
         if self.endTime is not None:
             oprot.writeFieldBegin('endTime', TType.I64, 2)
             oprot.writeI64(self.endTime)
             oprot.writeFieldEnd()
         if self.failedMessages is not None:
             oprot.writeFieldBegin('failedMessages', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.failedMessages))
-            for iter33 in self.failedMessages:
-                oprot.writeString(iter33.encode('utf-8') if sys.version_info[0] == 2 else iter33)
+            for iter47 in self.failedMessages:
+                oprot.writeString(iter47.encode('utf-8') if sys.version_info[0] == 2 else iter47)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.failureInfoList is not None:
             oprot.writeFieldBegin('failureInfoList', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.failureInfoList))
-            for iter34 in self.failureInfoList:
-                oprot.writeBinary(iter34)
+            for iter48 in self.failureInfoList:
+                oprot.writeBinary(iter48)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.state is None:
@@ -1729,21 +1865,23 @@
 
 
 class TCancelQueryReq(object):
     """
     Attributes:
      - queryId
      - fragmentInstanceIds
+     - hasThrowable
 
     """
 
 
-    def __init__(self, queryId=None, fragmentInstanceIds=None,):
+    def __init__(self, queryId=None, fragmentInstanceIds=None, hasThrowable=None,):
         self.queryId = queryId
         self.fragmentInstanceIds = fragmentInstanceIds
+        self.hasThrowable = hasThrowable
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1754,22 +1892,27 @@
                 if ftype == TType.STRING:
                     self.queryId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.fragmentInstanceIds = []
-                    (_etype38, _size35) = iprot.readListBegin()
-                    for _i39 in range(_size35):
-                        _elem40 = TFragmentInstanceId()
-                        _elem40.read(iprot)
-                        self.fragmentInstanceIds.append(_elem40)
+                    (_etype52, _size49) = iprot.readListBegin()
+                    for _i53 in range(_size49):
+                        _elem54 = TFragmentInstanceId()
+                        _elem54.read(iprot)
+                        self.fragmentInstanceIds.append(_elem54)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.BOOL:
+                    self.hasThrowable = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1779,26 +1922,32 @@
         if self.queryId is not None:
             oprot.writeFieldBegin('queryId', TType.STRING, 1)
             oprot.writeString(self.queryId.encode('utf-8') if sys.version_info[0] == 2 else self.queryId)
             oprot.writeFieldEnd()
         if self.fragmentInstanceIds is not None:
             oprot.writeFieldBegin('fragmentInstanceIds', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.fragmentInstanceIds))
-            for iter41 in self.fragmentInstanceIds:
-                iter41.write(oprot)
+            for iter55 in self.fragmentInstanceIds:
+                iter55.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
+        if self.hasThrowable is not None:
+            oprot.writeFieldBegin('hasThrowable', TType.BOOL, 3)
+            oprot.writeBool(self.hasThrowable)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.queryId is None:
             raise TProtocolException(message='Required field queryId is unset!')
         if self.fragmentInstanceIds is None:
             raise TProtocolException(message='Required field fragmentInstanceIds is unset!')
+        if self.hasThrowable is None:
+            raise TProtocolException(message='Required field hasThrowable is unset!')
         return
 
     def __repr__(self):
         L = ['%s=%r' % (key, value)
              for key, value in self.__dict__.items()]
         return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
 
@@ -2895,22 +3044,24 @@
 
 class THeartbeatReq(object):
     """
     Attributes:
      - heartbeatTimestamp
      - needJudgeLeader
      - needSamplingLoad
+     - schemaQuotaCount
 
     """
 
 
-    def __init__(self, heartbeatTimestamp=None, needJudgeLeader=None, needSamplingLoad=None,):
+    def __init__(self, heartbeatTimestamp=None, needJudgeLeader=None, needSamplingLoad=None, schemaQuotaCount=None,):
         self.heartbeatTimestamp = heartbeatTimestamp
         self.needJudgeLeader = needJudgeLeader
         self.needSamplingLoad = needSamplingLoad
+        self.schemaQuotaCount = schemaQuotaCount
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -2928,14 +3079,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.BOOL:
                     self.needSamplingLoad = iprot.readBool()
                 else:
                     iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I64:
+                    self.schemaQuotaCount = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -2950,24 +3106,30 @@
             oprot.writeFieldBegin('needJudgeLeader', TType.BOOL, 2)
             oprot.writeBool(self.needJudgeLeader)
             oprot.writeFieldEnd()
         if self.needSamplingLoad is not None:
             oprot.writeFieldBegin('needSamplingLoad', TType.BOOL, 3)
             oprot.writeBool(self.needSamplingLoad)
             oprot.writeFieldEnd()
+        if self.schemaQuotaCount is not None:
+            oprot.writeFieldBegin('schemaQuotaCount', TType.I64, 4)
+            oprot.writeI64(self.schemaQuotaCount)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.heartbeatTimestamp is None:
             raise TProtocolException(message='Required field heartbeatTimestamp is unset!')
         if self.needJudgeLeader is None:
             raise TProtocolException(message='Required field needJudgeLeader is unset!')
         if self.needSamplingLoad is None:
             raise TProtocolException(message='Required field needSamplingLoad is unset!')
+        if self.schemaQuotaCount is None:
+            raise TProtocolException(message='Required field schemaQuotaCount is unset!')
         return
 
     def __repr__(self):
         L = ['%s=%r' % (key, value)
              for key, value in self.__dict__.items()]
         return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
 
@@ -2982,24 +3144,26 @@
     """
     Attributes:
      - heartbeatTimestamp
      - status
      - statusReason
      - judgedLeaders
      - loadSample
+     - schemaCountMap
 
     """
 
 
-    def __init__(self, heartbeatTimestamp=None, status=None, statusReason=None, judgedLeaders=None, loadSample=None,):
+    def __init__(self, heartbeatTimestamp=None, status=None, statusReason=None, judgedLeaders=None, loadSample=None, schemaCountMap=None,):
         self.heartbeatTimestamp = heartbeatTimestamp
         self.status = status
         self.statusReason = statusReason
         self.judgedLeaders = judgedLeaders
         self.loadSample = loadSample
+        self.schemaCountMap = schemaCountMap
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -3020,29 +3184,41 @@
                 if ftype == TType.STRING:
                     self.statusReason = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.MAP:
                     self.judgedLeaders = {}
-                    (_ktype43, _vtype44, _size42) = iprot.readMapBegin()
-                    for _i46 in range(_size42):
-                        _key47 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _key47.read(iprot)
-                        _val48 = iprot.readBool()
-                        self.judgedLeaders[_key47] = _val48
+                    (_ktype57, _vtype58, _size56) = iprot.readMapBegin()
+                    for _i60 in range(_size56):
+                        _key61 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _key61.read(iprot)
+                        _val62 = iprot.readBool()
+                        self.judgedLeaders[_key61] = _val62
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.loadSample = TLoadSample()
                     self.loadSample.read(iprot)
                 else:
                     iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.MAP:
+                    self.schemaCountMap = {}
+                    (_ktype64, _vtype65, _size63) = iprot.readMapBegin()
+                    for _i67 in range(_size63):
+                        _key68 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _key68.read(iprot)
+                        _val69 = iprot.readI64()
+                        self.schemaCountMap[_key68] = _val69
+                    iprot.readMapEnd()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -3060,23 +3236,31 @@
         if self.statusReason is not None:
             oprot.writeFieldBegin('statusReason', TType.STRING, 3)
             oprot.writeString(self.statusReason.encode('utf-8') if sys.version_info[0] == 2 else self.statusReason)
             oprot.writeFieldEnd()
         if self.judgedLeaders is not None:
             oprot.writeFieldBegin('judgedLeaders', TType.MAP, 4)
             oprot.writeMapBegin(TType.STRUCT, TType.BOOL, len(self.judgedLeaders))
-            for kiter49, viter50 in self.judgedLeaders.items():
-                kiter49.write(oprot)
-                oprot.writeBool(viter50)
+            for kiter70, viter71 in self.judgedLeaders.items():
+                kiter70.write(oprot)
+                oprot.writeBool(viter71)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.loadSample is not None:
             oprot.writeFieldBegin('loadSample', TType.STRUCT, 5)
             self.loadSample.write(oprot)
             oprot.writeFieldEnd()
+        if self.schemaCountMap is not None:
+            oprot.writeFieldBegin('schemaCountMap', TType.MAP, 6)
+            oprot.writeMapBegin(TType.STRUCT, TType.I64, len(self.schemaCountMap))
+            for kiter72, viter73 in self.schemaCountMap.items():
+                kiter72.write(oprot)
+                oprot.writeI64(viter73)
+            oprot.writeMapEnd()
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.heartbeatTimestamp is None:
             raise TProtocolException(message='Required field heartbeatTimestamp is unset!')
         if self.status is None:
@@ -3219,21 +3403,21 @@
                 if ftype == TType.I64:
                     self.timestamp = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.regionRouteMap = {}
-                    (_ktype52, _vtype53, _size51) = iprot.readMapBegin()
-                    for _i55 in range(_size51):
-                        _key56 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _key56.read(iprot)
-                        _val57 = iotdb.thrift.common.ttypes.TRegionReplicaSet()
-                        _val57.read(iprot)
-                        self.regionRouteMap[_key56] = _val57
+                    (_ktype75, _vtype76, _size74) = iprot.readMapBegin()
+                    for _i78 in range(_size74):
+                        _key79 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _key79.read(iprot)
+                        _val80 = iotdb.thrift.common.ttypes.TRegionReplicaSet()
+                        _val80.read(iprot)
+                        self.regionRouteMap[_key79] = _val80
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3246,17 +3430,17 @@
         if self.timestamp is not None:
             oprot.writeFieldBegin('timestamp', TType.I64, 1)
             oprot.writeI64(self.timestamp)
             oprot.writeFieldEnd()
         if self.regionRouteMap is not None:
             oprot.writeFieldBegin('regionRouteMap', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRUCT, TType.STRUCT, len(self.regionRouteMap))
-            for kiter58, viter59 in self.regionRouteMap.items():
-                kiter58.write(oprot)
-                viter59.write(oprot)
+            for kiter81, viter82 in self.regionRouteMap.items():
+                kiter81.write(oprot)
+                viter82.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.timestamp is None:
@@ -3296,19 +3480,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.configNodeLocations = []
-                    (_etype63, _size60) = iprot.readListBegin()
-                    for _i64 in range(_size60):
-                        _elem65 = iotdb.thrift.common.ttypes.TConfigNodeLocation()
-                        _elem65.read(iprot)
-                        self.configNodeLocations.append(_elem65)
+                    (_etype86, _size83) = iprot.readListBegin()
+                    for _i87 in range(_size83):
+                        _elem88 = iotdb.thrift.common.ttypes.TConfigNodeLocation()
+                        _elem88.read(iprot)
+                        self.configNodeLocations.append(_elem88)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3317,16 +3501,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TUpdateConfigNodeGroupReq')
         if self.configNodeLocations is not None:
             oprot.writeFieldBegin('configNodeLocations', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.configNodeLocations))
-            for iter66 in self.configNodeLocations:
-                iter66.write(oprot)
+            for iter89 in self.configNodeLocations:
+                iter89.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.configNodeLocations is None:
@@ -3678,19 +3862,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype70, _size67) = iprot.readListBegin()
-                    for _i71 in range(_size67):
-                        _elem72 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem72.read(iprot)
-                        self.schemaRegionIdList.append(_elem72)
+                    (_etype93, _size90) = iprot.readListBegin()
+                    for _i94 in range(_size90):
+                        _elem95 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem95.read(iprot)
+                        self.schemaRegionIdList.append(_elem95)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.pathPatternTree = iprot.readBinary()
                 else:
@@ -3704,16 +3888,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TConstructSchemaBlackListReq')
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter73 in self.schemaRegionIdList:
-                iter73.write(oprot)
+            for iter96 in self.schemaRegionIdList:
+                iter96.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.pathPatternTree is not None:
             oprot.writeFieldBegin('pathPatternTree', TType.STRING, 2)
             oprot.writeBinary(self.pathPatternTree)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3759,19 +3943,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype77, _size74) = iprot.readListBegin()
-                    for _i78 in range(_size74):
-                        _elem79 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem79.read(iprot)
-                        self.schemaRegionIdList.append(_elem79)
+                    (_etype100, _size97) = iprot.readListBegin()
+                    for _i101 in range(_size97):
+                        _elem102 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem102.read(iprot)
+                        self.schemaRegionIdList.append(_elem102)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.pathPatternTree = iprot.readBinary()
                 else:
@@ -3785,16 +3969,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TRollbackSchemaBlackListReq')
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter80 in self.schemaRegionIdList:
-                iter80.write(oprot)
+            for iter103 in self.schemaRegionIdList:
+                iter103.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.pathPatternTree is not None:
             oprot.writeFieldBegin('pathPatternTree', TType.STRING, 2)
             oprot.writeBinary(self.pathPatternTree)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3899,19 +4083,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype84, _size81) = iprot.readListBegin()
-                    for _i85 in range(_size81):
-                        _elem86 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem86.read(iprot)
-                        self.schemaRegionIdList.append(_elem86)
+                    (_etype107, _size104) = iprot.readListBegin()
+                    for _i108 in range(_size104):
+                        _elem109 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem109.read(iprot)
+                        self.schemaRegionIdList.append(_elem109)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.pathPatternTree = iprot.readBinary()
                 else:
@@ -3925,16 +4109,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TFetchSchemaBlackListReq')
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter87 in self.schemaRegionIdList:
-                iter87.write(oprot)
+            for iter110 in self.schemaRegionIdList:
+                iter110.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.pathPatternTree is not None:
             oprot.writeFieldBegin('pathPatternTree', TType.STRING, 2)
             oprot.writeBinary(self.pathPatternTree)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4053,19 +4237,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.dataRegionIdList = []
-                    (_etype91, _size88) = iprot.readListBegin()
-                    for _i92 in range(_size88):
-                        _elem93 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem93.read(iprot)
-                        self.dataRegionIdList.append(_elem93)
+                    (_etype114, _size111) = iprot.readListBegin()
+                    for _i115 in range(_size111):
+                        _elem116 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem116.read(iprot)
+                        self.dataRegionIdList.append(_elem116)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.pathPatternTree = iprot.readBinary()
                 else:
@@ -4079,16 +4263,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TDeleteDataForDeleteSchemaReq')
         if self.dataRegionIdList is not None:
             oprot.writeFieldBegin('dataRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.dataRegionIdList))
-            for iter94 in self.dataRegionIdList:
-                iter94.write(oprot)
+            for iter117 in self.dataRegionIdList:
+                iter117.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.pathPatternTree is not None:
             oprot.writeFieldBegin('pathPatternTree', TType.STRING, 2)
             oprot.writeBinary(self.pathPatternTree)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4134,19 +4318,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype98, _size95) = iprot.readListBegin()
-                    for _i99 in range(_size95):
-                        _elem100 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem100.read(iprot)
-                        self.schemaRegionIdList.append(_elem100)
+                    (_etype121, _size118) = iprot.readListBegin()
+                    for _i122 in range(_size118):
+                        _elem123 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem123.read(iprot)
+                        self.schemaRegionIdList.append(_elem123)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.pathPatternTree = iprot.readBinary()
                 else:
@@ -4160,16 +4344,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TDeleteTimeSeriesReq')
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter101 in self.schemaRegionIdList:
-                iter101.write(oprot)
+            for iter124 in self.schemaRegionIdList:
+                iter124.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.pathPatternTree is not None:
             oprot.writeFieldBegin('pathPatternTree', TType.STRING, 2)
             oprot.writeBinary(self.pathPatternTree)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4215,35 +4399,35 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype105, _size102) = iprot.readListBegin()
-                    for _i106 in range(_size102):
-                        _elem107 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem107.read(iprot)
-                        self.schemaRegionIdList.append(_elem107)
+                    (_etype128, _size125) = iprot.readListBegin()
+                    for _i129 in range(_size125):
+                        _elem130 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem130.read(iprot)
+                        self.schemaRegionIdList.append(_elem130)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.templateSetInfo = {}
-                    (_ktype109, _vtype110, _size108) = iprot.readMapBegin()
-                    for _i112 in range(_size108):
-                        _key113 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        _val114 = []
-                        (_etype118, _size115) = iprot.readListBegin()
-                        for _i119 in range(_size115):
-                            _elem120 = iprot.readI32()
-                            _val114.append(_elem120)
+                    (_ktype132, _vtype133, _size131) = iprot.readMapBegin()
+                    for _i135 in range(_size131):
+                        _key136 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        _val137 = []
+                        (_etype141, _size138) = iprot.readListBegin()
+                        for _i142 in range(_size138):
+                            _elem143 = iprot.readI32()
+                            _val137.append(_elem143)
                         iprot.readListEnd()
-                        self.templateSetInfo[_key113] = _val114
+                        self.templateSetInfo[_key136] = _val137
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4252,26 +4436,26 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TConstructSchemaBlackListWithTemplateReq')
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter121 in self.schemaRegionIdList:
-                iter121.write(oprot)
+            for iter144 in self.schemaRegionIdList:
+                iter144.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.templateSetInfo is not None:
             oprot.writeFieldBegin('templateSetInfo', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.LIST, len(self.templateSetInfo))
-            for kiter122, viter123 in self.templateSetInfo.items():
-                oprot.writeString(kiter122.encode('utf-8') if sys.version_info[0] == 2 else kiter122)
-                oprot.writeListBegin(TType.I32, len(viter123))
-                for iter124 in viter123:
-                    oprot.writeI32(iter124)
+            for kiter145, viter146 in self.templateSetInfo.items():
+                oprot.writeString(kiter145.encode('utf-8') if sys.version_info[0] == 2 else kiter145)
+                oprot.writeListBegin(TType.I32, len(viter146))
+                for iter147 in viter146:
+                    oprot.writeI32(iter147)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
@@ -4314,35 +4498,35 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype128, _size125) = iprot.readListBegin()
-                    for _i129 in range(_size125):
-                        _elem130 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem130.read(iprot)
-                        self.schemaRegionIdList.append(_elem130)
+                    (_etype151, _size148) = iprot.readListBegin()
+                    for _i152 in range(_size148):
+                        _elem153 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem153.read(iprot)
+                        self.schemaRegionIdList.append(_elem153)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.templateSetInfo = {}
-                    (_ktype132, _vtype133, _size131) = iprot.readMapBegin()
-                    for _i135 in range(_size131):
-                        _key136 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        _val137 = []
-                        (_etype141, _size138) = iprot.readListBegin()
-                        for _i142 in range(_size138):
-                            _elem143 = iprot.readI32()
-                            _val137.append(_elem143)
+                    (_ktype155, _vtype156, _size154) = iprot.readMapBegin()
+                    for _i158 in range(_size154):
+                        _key159 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        _val160 = []
+                        (_etype164, _size161) = iprot.readListBegin()
+                        for _i165 in range(_size161):
+                            _elem166 = iprot.readI32()
+                            _val160.append(_elem166)
                         iprot.readListEnd()
-                        self.templateSetInfo[_key136] = _val137
+                        self.templateSetInfo[_key159] = _val160
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4351,26 +4535,26 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TRollbackSchemaBlackListWithTemplateReq')
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter144 in self.schemaRegionIdList:
-                iter144.write(oprot)
+            for iter167 in self.schemaRegionIdList:
+                iter167.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.templateSetInfo is not None:
             oprot.writeFieldBegin('templateSetInfo', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.LIST, len(self.templateSetInfo))
-            for kiter145, viter146 in self.templateSetInfo.items():
-                oprot.writeString(kiter145.encode('utf-8') if sys.version_info[0] == 2 else kiter145)
-                oprot.writeListBegin(TType.I32, len(viter146))
-                for iter147 in viter146:
-                    oprot.writeI32(iter147)
+            for kiter168, viter169 in self.templateSetInfo.items():
+                oprot.writeString(kiter168.encode('utf-8') if sys.version_info[0] == 2 else kiter168)
+                oprot.writeListBegin(TType.I32, len(viter169))
+                for iter170 in viter169:
+                    oprot.writeI32(iter170)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
@@ -4413,35 +4597,35 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype151, _size148) = iprot.readListBegin()
-                    for _i152 in range(_size148):
-                        _elem153 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem153.read(iprot)
-                        self.schemaRegionIdList.append(_elem153)
+                    (_etype174, _size171) = iprot.readListBegin()
+                    for _i175 in range(_size171):
+                        _elem176 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem176.read(iprot)
+                        self.schemaRegionIdList.append(_elem176)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.templateSetInfo = {}
-                    (_ktype155, _vtype156, _size154) = iprot.readMapBegin()
-                    for _i158 in range(_size154):
-                        _key159 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        _val160 = []
-                        (_etype164, _size161) = iprot.readListBegin()
-                        for _i165 in range(_size161):
-                            _elem166 = iprot.readI32()
-                            _val160.append(_elem166)
+                    (_ktype178, _vtype179, _size177) = iprot.readMapBegin()
+                    for _i181 in range(_size177):
+                        _key182 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        _val183 = []
+                        (_etype187, _size184) = iprot.readListBegin()
+                        for _i188 in range(_size184):
+                            _elem189 = iprot.readI32()
+                            _val183.append(_elem189)
                         iprot.readListEnd()
-                        self.templateSetInfo[_key159] = _val160
+                        self.templateSetInfo[_key182] = _val183
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4450,26 +4634,26 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TDeactivateTemplateReq')
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter167 in self.schemaRegionIdList:
-                iter167.write(oprot)
+            for iter190 in self.schemaRegionIdList:
+                iter190.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.templateSetInfo is not None:
             oprot.writeFieldBegin('templateSetInfo', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.LIST, len(self.templateSetInfo))
-            for kiter168, viter169 in self.templateSetInfo.items():
-                oprot.writeString(kiter168.encode('utf-8') if sys.version_info[0] == 2 else kiter168)
-                oprot.writeListBegin(TType.I32, len(viter169))
-                for iter170 in viter169:
-                    oprot.writeI32(iter170)
+            for kiter191, viter192 in self.templateSetInfo.items():
+                oprot.writeString(kiter191.encode('utf-8') if sys.version_info[0] == 2 else kiter191)
+                oprot.writeListBegin(TType.I32, len(viter192))
+                for iter193 in viter192:
+                    oprot.writeI32(iter193)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
@@ -4524,19 +4708,19 @@
                 if ftype == TType.STRING:
                     self.patternTree = iprot.readBinary()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.schemaRegionIdList = []
-                    (_etype174, _size171) = iprot.readListBegin()
-                    for _i175 in range(_size171):
-                        _elem176 = iotdb.thrift.common.ttypes.TConsensusGroupId()
-                        _elem176.read(iprot)
-                        self.schemaRegionIdList.append(_elem176)
+                    (_etype197, _size194) = iprot.readListBegin()
+                    for _i198 in range(_size194):
+                        _elem199 = iotdb.thrift.common.ttypes.TConsensusGroupId()
+                        _elem199.read(iprot)
+                        self.schemaRegionIdList.append(_elem199)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4553,16 +4737,16 @@
         if self.patternTree is not None:
             oprot.writeFieldBegin('patternTree', TType.STRING, 2)
             oprot.writeBinary(self.patternTree)
             oprot.writeFieldEnd()
         if self.schemaRegionIdList is not None:
             oprot.writeFieldBegin('schemaRegionIdList', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaRegionIdList))
-            for iter177 in self.schemaRegionIdList:
-                iter177.write(oprot)
+            for iter200 in self.schemaRegionIdList:
+                iter200.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.templateId is None:
@@ -5033,18 +5217,18 @@
                 if ftype == TType.I64:
                     self.statementId = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.queryExpressions = []
-                    (_etype181, _size178) = iprot.readListBegin()
-                    for _i182 in range(_size178):
-                        _elem183 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.queryExpressions.append(_elem183)
+                    (_etype204, _size201) = iprot.readListBegin()
+                    for _i205 in range(_size201):
+                        _elem206 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.queryExpressions.append(_elem206)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRING:
                     self.queryFilter = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
@@ -5076,16 +5260,16 @@
         if self.statementId is not None:
             oprot.writeFieldBegin('statementId', TType.I64, 2)
             oprot.writeI64(self.statementId)
             oprot.writeFieldEnd()
         if self.queryExpressions is not None:
             oprot.writeFieldBegin('queryExpressions', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.queryExpressions))
-            for iter184 in self.queryExpressions:
-                oprot.writeString(iter184.encode('utf-8') if sys.version_info[0] == 2 else iter184)
+            for iter207 in self.queryExpressions:
+                oprot.writeString(iter207.encode('utf-8') if sys.version_info[0] == 2 else iter207)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.queryFilter is not None:
             oprot.writeFieldBegin('queryFilter', TType.STRING, 4)
             oprot.writeString(self.queryFilter.encode('utf-8') if sys.version_info[0] == 2 else self.queryFilter)
             oprot.writeFieldEnd()
         if self.fetchSize is not None:
@@ -5162,49 +5346,49 @@
                 if ftype == TType.I64:
                     self.queryId = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.columnNameList = []
-                    (_etype188, _size185) = iprot.readListBegin()
-                    for _i189 in range(_size185):
-                        _elem190 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.columnNameList.append(_elem190)
+                    (_etype211, _size208) = iprot.readListBegin()
+                    for _i212 in range(_size208):
+                        _elem213 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.columnNameList.append(_elem213)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.columnTypeList = []
-                    (_etype194, _size191) = iprot.readListBegin()
-                    for _i195 in range(_size191):
-                        _elem196 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.columnTypeList.append(_elem196)
+                    (_etype217, _size214) = iprot.readListBegin()
+                    for _i218 in range(_size214):
+                        _elem219 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.columnTypeList.append(_elem219)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.MAP:
                     self.columnNameIndexMap = {}
-                    (_ktype198, _vtype199, _size197) = iprot.readMapBegin()
-                    for _i201 in range(_size197):
-                        _key202 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        _val203 = iprot.readI32()
-                        self.columnNameIndexMap[_key202] = _val203
+                    (_ktype221, _vtype222, _size220) = iprot.readMapBegin()
+                    for _i224 in range(_size220):
+                        _key225 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        _val226 = iprot.readI32()
+                        self.columnNameIndexMap[_key225] = _val226
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.tsDataset = []
-                    (_etype207, _size204) = iprot.readListBegin()
-                    for _i208 in range(_size204):
-                        _elem209 = iprot.readBinary()
-                        self.tsDataset.append(_elem209)
+                    (_etype230, _size227) = iprot.readListBegin()
+                    for _i231 in range(_size227):
+                        _elem232 = iprot.readBinary()
+                        self.tsDataset.append(_elem232)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.BOOL:
                     self.hasMoreData = iprot.readBool()
                 else:
@@ -5226,38 +5410,38 @@
         if self.queryId is not None:
             oprot.writeFieldBegin('queryId', TType.I64, 2)
             oprot.writeI64(self.queryId)
             oprot.writeFieldEnd()
         if self.columnNameList is not None:
             oprot.writeFieldBegin('columnNameList', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.columnNameList))
-            for iter210 in self.columnNameList:
-                oprot.writeString(iter210.encode('utf-8') if sys.version_info[0] == 2 else iter210)
+            for iter233 in self.columnNameList:
+                oprot.writeString(iter233.encode('utf-8') if sys.version_info[0] == 2 else iter233)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columnTypeList is not None:
             oprot.writeFieldBegin('columnTypeList', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.columnTypeList))
-            for iter211 in self.columnTypeList:
-                oprot.writeString(iter211.encode('utf-8') if sys.version_info[0] == 2 else iter211)
+            for iter234 in self.columnTypeList:
+                oprot.writeString(iter234.encode('utf-8') if sys.version_info[0] == 2 else iter234)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columnNameIndexMap is not None:
             oprot.writeFieldBegin('columnNameIndexMap', TType.MAP, 5)
             oprot.writeMapBegin(TType.STRING, TType.I32, len(self.columnNameIndexMap))
-            for kiter212, viter213 in self.columnNameIndexMap.items():
-                oprot.writeString(kiter212.encode('utf-8') if sys.version_info[0] == 2 else kiter212)
-                oprot.writeI32(viter213)
+            for kiter235, viter236 in self.columnNameIndexMap.items():
+                oprot.writeString(kiter235.encode('utf-8') if sys.version_info[0] == 2 else kiter235)
+                oprot.writeI32(viter236)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.tsDataset is not None:
             oprot.writeFieldBegin('tsDataset', TType.LIST, 6)
             oprot.writeListBegin(TType.STRING, len(self.tsDataset))
-            for iter214 in self.tsDataset:
-                oprot.writeBinary(iter214)
+            for iter237 in self.tsDataset:
+                oprot.writeBinary(iter237)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.hasMoreData is not None:
             oprot.writeFieldBegin('hasMoreData', TType.BOOL, 7)
             oprot.writeBool(self.hasMoreData)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5333,18 +5517,18 @@
                 if ftype == TType.I64:
                     self.statementId = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.queryExpressions = []
-                    (_etype218, _size215) = iprot.readListBegin()
-                    for _i219 in range(_size215):
-                        _elem220 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.queryExpressions.append(_elem220)
+                    (_etype241, _size238) = iprot.readListBegin()
+                    for _i242 in range(_size238):
+                        _elem243 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.queryExpressions.append(_elem243)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.groupByTimeParameter = TGroupByTimeParameter()
                     self.groupByTimeParameter.read(iprot)
@@ -5382,16 +5566,16 @@
         if self.statementId is not None:
             oprot.writeFieldBegin('statementId', TType.I64, 2)
             oprot.writeI64(self.statementId)
             oprot.writeFieldEnd()
         if self.queryExpressions is not None:
             oprot.writeFieldBegin('queryExpressions', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.queryExpressions))
-            for iter221 in self.queryExpressions:
-                oprot.writeString(iter221.encode('utf-8') if sys.version_info[0] == 2 else iter221)
+            for iter244 in self.queryExpressions:
+                oprot.writeString(iter244.encode('utf-8') if sys.version_info[0] == 2 else iter244)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.groupByTimeParameter is not None:
             oprot.writeFieldBegin('groupByTimeParameter', TType.STRUCT, 4)
             self.groupByTimeParameter.write(oprot)
             oprot.writeFieldEnd()
         if self.queryFilter is not None:
@@ -5479,18 +5663,18 @@
                 if ftype == TType.I64:
                     self.slidingStep = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.indexes = []
-                    (_etype225, _size222) = iprot.readListBegin()
-                    for _i226 in range(_size222):
-                        _elem227 = iprot.readI32()
-                        self.indexes.append(_elem227)
+                    (_etype248, _size245) = iprot.readListBegin()
+                    for _i249 in range(_size245):
+                        _elem250 = iprot.readI32()
+                        self.indexes.append(_elem250)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5515,16 +5699,16 @@
         if self.slidingStep is not None:
             oprot.writeFieldBegin('slidingStep', TType.I64, 4)
             oprot.writeI64(self.slidingStep)
             oprot.writeFieldEnd()
         if self.indexes is not None:
             oprot.writeFieldBegin('indexes', TType.LIST, 5)
             oprot.writeListBegin(TType.I32, len(self.indexes))
-            for iter228 in self.indexes:
-                oprot.writeI32(iter228)
+            for iter251 in self.indexes:
+                oprot.writeI32(iter251)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.startTime is None:
@@ -5591,54 +5775,54 @@
                 if ftype == TType.I64:
                     self.queryId = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.columnNameList = []
-                    (_etype232, _size229) = iprot.readListBegin()
-                    for _i233 in range(_size229):
-                        _elem234 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.columnNameList.append(_elem234)
+                    (_etype255, _size252) = iprot.readListBegin()
+                    for _i256 in range(_size252):
+                        _elem257 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.columnNameList.append(_elem257)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.columnTypeList = []
-                    (_etype238, _size235) = iprot.readListBegin()
-                    for _i239 in range(_size235):
-                        _elem240 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.columnTypeList.append(_elem240)
+                    (_etype261, _size258) = iprot.readListBegin()
+                    for _i262 in range(_size258):
+                        _elem263 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.columnTypeList.append(_elem263)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.MAP:
                     self.columnNameIndexMap = {}
-                    (_ktype242, _vtype243, _size241) = iprot.readMapBegin()
-                    for _i245 in range(_size241):
-                        _key246 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        _val247 = iprot.readI32()
-                        self.columnNameIndexMap[_key246] = _val247
+                    (_ktype265, _vtype266, _size264) = iprot.readMapBegin()
+                    for _i268 in range(_size264):
+                        _key269 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        _val270 = iprot.readI32()
+                        self.columnNameIndexMap[_key269] = _val270
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.windowDataset = []
-                    (_etype251, _size248) = iprot.readListBegin()
-                    for _i252 in range(_size248):
-                        _elem253 = []
-                        (_etype257, _size254) = iprot.readListBegin()
-                        for _i258 in range(_size254):
-                            _elem259 = iprot.readBinary()
-                            _elem253.append(_elem259)
+                    (_etype274, _size271) = iprot.readListBegin()
+                    for _i275 in range(_size271):
+                        _elem276 = []
+                        (_etype280, _size277) = iprot.readListBegin()
+                        for _i281 in range(_size277):
+                            _elem282 = iprot.readBinary()
+                            _elem276.append(_elem282)
                         iprot.readListEnd()
-                        self.windowDataset.append(_elem253)
+                        self.windowDataset.append(_elem276)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.BOOL:
                     self.hasMoreData = iprot.readBool()
                 else:
@@ -5660,40 +5844,40 @@
         if self.queryId is not None:
             oprot.writeFieldBegin('queryId', TType.I64, 2)
             oprot.writeI64(self.queryId)
             oprot.writeFieldEnd()
         if self.columnNameList is not None:
             oprot.writeFieldBegin('columnNameList', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.columnNameList))
-            for iter260 in self.columnNameList:
-                oprot.writeString(iter260.encode('utf-8') if sys.version_info[0] == 2 else iter260)
+            for iter283 in self.columnNameList:
+                oprot.writeString(iter283.encode('utf-8') if sys.version_info[0] == 2 else iter283)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columnTypeList is not None:
             oprot.writeFieldBegin('columnTypeList', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.columnTypeList))
-            for iter261 in self.columnTypeList:
-                oprot.writeString(iter261.encode('utf-8') if sys.version_info[0] == 2 else iter261)
+            for iter284 in self.columnTypeList:
+                oprot.writeString(iter284.encode('utf-8') if sys.version_info[0] == 2 else iter284)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columnNameIndexMap is not None:
             oprot.writeFieldBegin('columnNameIndexMap', TType.MAP, 5)
             oprot.writeMapBegin(TType.STRING, TType.I32, len(self.columnNameIndexMap))
-            for kiter262, viter263 in self.columnNameIndexMap.items():
-                oprot.writeString(kiter262.encode('utf-8') if sys.version_info[0] == 2 else kiter262)
-                oprot.writeI32(viter263)
+            for kiter285, viter286 in self.columnNameIndexMap.items():
+                oprot.writeString(kiter285.encode('utf-8') if sys.version_info[0] == 2 else kiter285)
+                oprot.writeI32(viter286)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.windowDataset is not None:
             oprot.writeFieldBegin('windowDataset', TType.LIST, 6)
             oprot.writeListBegin(TType.LIST, len(self.windowDataset))
-            for iter264 in self.windowDataset:
-                oprot.writeListBegin(TType.STRING, len(iter264))
-                for iter265 in iter264:
-                    oprot.writeBinary(iter265)
+            for iter287 in self.windowDataset:
+                oprot.writeListBegin(TType.STRING, len(iter287))
+                for iter288 in iter287:
+                    oprot.writeBinary(iter288)
                 oprot.writeListEnd()
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.hasMoreData is not None:
             oprot.writeFieldBegin('hasMoreData', TType.BOOL, 7)
             oprot.writeBool(self.hasMoreData)
             oprot.writeFieldEnd()
@@ -5766,33 +5950,33 @@
                 if ftype == TType.STRING:
                     self.trialId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.metrics = []
-                    (_etype269, _size266) = iprot.readListBegin()
-                    for _i270 in range(_size266):
-                        _elem271 = iprot.readI32()
-                        self.metrics.append(_elem271)
+                    (_etype292, _size289) = iprot.readListBegin()
+                    for _i293 in range(_size289):
+                        _elem294 = iprot.readI32()
+                        self.metrics.append(_elem294)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.timestamp = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype275, _size272) = iprot.readListBegin()
-                    for _i276 in range(_size272):
-                        _elem277 = iprot.readDouble()
-                        self.values.append(_elem277)
+                    (_etype298, _size295) = iprot.readListBegin()
+                    for _i299 in range(_size295):
+                        _elem300 = iprot.readDouble()
+                        self.values.append(_elem300)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5809,27 +5993,27 @@
         if self.trialId is not None:
             oprot.writeFieldBegin('trialId', TType.STRING, 2)
             oprot.writeString(self.trialId.encode('utf-8') if sys.version_info[0] == 2 else self.trialId)
             oprot.writeFieldEnd()
         if self.metrics is not None:
             oprot.writeFieldBegin('metrics', TType.LIST, 3)
             oprot.writeListBegin(TType.I32, len(self.metrics))
-            for iter278 in self.metrics:
-                oprot.writeI32(iter278)
+            for iter301 in self.metrics:
+                oprot.writeI32(iter301)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.timestamp is not None:
             oprot.writeFieldBegin('timestamp', TType.I64, 4)
             oprot.writeI64(self.timestamp)
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 5)
             oprot.writeListBegin(TType.DOUBLE, len(self.values))
-            for iter279 in self.values:
-                oprot.writeDouble(iter279)
+            for iter302 in self.values:
+                oprot.writeDouble(iter302)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.modelId is None:
@@ -5962,27 +6146,37 @@
 )
 all_structs.append(TSendFragmentInstanceResp)
 TSendFragmentInstanceResp.thrift_spec = (
     None,  # 0
     (1, TType.BOOL, 'accepted', None, None, ),  # 1
     (2, TType.STRING, 'message', 'UTF8', None, ),  # 2
 )
-all_structs.append(TSendPlanNodeReq)
-TSendPlanNodeReq.thrift_spec = (
+all_structs.append(TSendSinglePlanNodeReq)
+TSendSinglePlanNodeReq.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'planNode', [TPlanNode, None], None, ),  # 1
     (2, TType.STRUCT, 'consensusGroupId', [iotdb.thrift.common.ttypes.TConsensusGroupId, None], None, ),  # 2
 )
-all_structs.append(TSendPlanNodeResp)
-TSendPlanNodeResp.thrift_spec = (
+all_structs.append(TSendSinglePlanNodeResp)
+TSendSinglePlanNodeResp.thrift_spec = (
     None,  # 0
     (1, TType.BOOL, 'accepted', None, None, ),  # 1
     (2, TType.STRING, 'message', 'UTF8', None, ),  # 2
     (3, TType.STRUCT, 'status', [iotdb.thrift.common.ttypes.TSStatus, None], None, ),  # 3
 )
+all_structs.append(TSendBatchPlanNodeReq)
+TSendBatchPlanNodeReq.thrift_spec = (
+    None,  # 0
+    (1, TType.LIST, 'requests', (TType.STRUCT, [TSendSinglePlanNodeReq, None], False), None, ),  # 1
+)
+all_structs.append(TSendBatchPlanNodeResp)
+TSendBatchPlanNodeResp.thrift_spec = (
+    None,  # 0
+    (1, TType.LIST, 'responses', (TType.STRUCT, [TSendSinglePlanNodeResp, None], False), None, ),  # 1
+)
 all_structs.append(TFetchFragmentInstanceInfoReq)
 TFetchFragmentInstanceInfoReq.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'fragmentInstanceId', [TFragmentInstanceId, None], None, ),  # 1
 )
 all_structs.append(TFragmentInstanceInfoResp)
 TFragmentInstanceInfoResp.thrift_spec = (
@@ -5993,14 +6187,15 @@
     (4, TType.LIST, 'failureInfoList', (TType.STRING, 'BINARY', False), None, ),  # 4
 )
 all_structs.append(TCancelQueryReq)
 TCancelQueryReq.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'queryId', 'UTF8', None, ),  # 1
     (2, TType.LIST, 'fragmentInstanceIds', (TType.STRUCT, [TFragmentInstanceId, None], False), None, ),  # 2
+    (3, TType.BOOL, 'hasThrowable', None, None, ),  # 3
 )
 all_structs.append(TCancelPlanFragmentReq)
 TCancelPlanFragmentReq.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'planFragmentId', 'UTF8', None, ),  # 1
 )
 all_structs.append(TCancelFragmentInstanceReq)
@@ -6091,23 +6286,25 @@
 )
 all_structs.append(THeartbeatReq)
 THeartbeatReq.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'heartbeatTimestamp', None, None, ),  # 1
     (2, TType.BOOL, 'needJudgeLeader', None, None, ),  # 2
     (3, TType.BOOL, 'needSamplingLoad', None, None, ),  # 3
+    (4, TType.I64, 'schemaQuotaCount', None, None, ),  # 4
 )
 all_structs.append(THeartbeatResp)
 THeartbeatResp.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'heartbeatTimestamp', None, None, ),  # 1
     (2, TType.STRING, 'status', 'UTF8', None, ),  # 2
     (3, TType.STRING, 'statusReason', 'UTF8', None, ),  # 3
     (4, TType.MAP, 'judgedLeaders', (TType.STRUCT, [iotdb.thrift.common.ttypes.TConsensusGroupId, None], TType.BOOL, None, False), None, ),  # 4
     (5, TType.STRUCT, 'loadSample', [TLoadSample, None], None, ),  # 5
+    (6, TType.MAP, 'schemaCountMap', (TType.STRUCT, [iotdb.thrift.common.ttypes.TConsensusGroupId, None], TType.I64, None, False), None, ),  # 6
 )
 all_structs.append(TLoadSample)
 TLoadSample.thrift_spec = (
     None,  # 0
     (1, TType.DOUBLE, 'cpuUsageRate', None, None, ),  # 1
     (2, TType.DOUBLE, 'memoryUsageRate', None, None, ),  # 2
     (3, TType.DOUBLE, 'diskUsageRate', None, None, ),  # 3
```

### Comparing `apache-iotdb-1.1.0/iotdb/thrift/rpc/IClientRPCService.py` & `apache-iotdb-1.1.2/iotdb/thrift/rpc/IClientRPCService.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,14 +437,22 @@
         """
         Parameters:
          - req
 
         """
         pass
 
+    def createTimeseriesUsingSchemaTemplate(self, req):
+        """
+        Parameters:
+         - req
+
+        """
+        pass
+
     def handshake(self, info):
         """
         Parameters:
          - info
 
         """
         pass
@@ -2172,14 +2180,46 @@
         result = dropSchemaTemplate_result()
         result.read(iprot)
         iprot.readMessageEnd()
         if result.success is not None:
             return result.success
         raise TApplicationException(TApplicationException.MISSING_RESULT, "dropSchemaTemplate failed: unknown result")
 
+    def createTimeseriesUsingSchemaTemplate(self, req):
+        """
+        Parameters:
+         - req
+
+        """
+        self.send_createTimeseriesUsingSchemaTemplate(req)
+        return self.recv_createTimeseriesUsingSchemaTemplate()
+
+    def send_createTimeseriesUsingSchemaTemplate(self, req):
+        self._oprot.writeMessageBegin('createTimeseriesUsingSchemaTemplate', TMessageType.CALL, self._seqid)
+        args = createTimeseriesUsingSchemaTemplate_args()
+        args.req = req
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_createTimeseriesUsingSchemaTemplate(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = createTimeseriesUsingSchemaTemplate_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "createTimeseriesUsingSchemaTemplate failed: unknown result")
+
     def handshake(self, info):
         """
         Parameters:
          - info
 
         """
         self.send_handshake(info)
@@ -2380,14 +2420,15 @@
         self._processMap["createSchemaTemplate"] = Processor.process_createSchemaTemplate
         self._processMap["appendSchemaTemplate"] = Processor.process_appendSchemaTemplate
         self._processMap["pruneSchemaTemplate"] = Processor.process_pruneSchemaTemplate
         self._processMap["querySchemaTemplate"] = Processor.process_querySchemaTemplate
         self._processMap["setSchemaTemplate"] = Processor.process_setSchemaTemplate
         self._processMap["unsetSchemaTemplate"] = Processor.process_unsetSchemaTemplate
         self._processMap["dropSchemaTemplate"] = Processor.process_dropSchemaTemplate
+        self._processMap["createTimeseriesUsingSchemaTemplate"] = Processor.process_createTimeseriesUsingSchemaTemplate
         self._processMap["handshake"] = Processor.process_handshake
         self._processMap["sendPipeData"] = Processor.process_sendPipeData
         self._processMap["sendFile"] = Processor.process_sendFile
         self._processMap["getBackupConfiguration"] = Processor.process_getBackupConfiguration
         self._processMap["fetchAllConnectionsInfo"] = Processor.process_fetchAllConnectionsInfo
         self._on_message_begin = None
 
@@ -3626,14 +3667,37 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("dropSchemaTemplate", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_createTimeseriesUsingSchemaTemplate(self, seqid, iprot, oprot):
+        args = createTimeseriesUsingSchemaTemplate_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = createTimeseriesUsingSchemaTemplate_result()
+        try:
+            result.success = self._handler.createTimeseriesUsingSchemaTemplate(args.req)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("createTimeseriesUsingSchemaTemplate", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_handshake(self, seqid, iprot, oprot):
         args = handshake_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = handshake_result()
         try:
             result.success = self._handler.handshake(args.info)
@@ -6764,18 +6828,18 @@
                 if ftype == TType.I64:
                     self.sessionId = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.path = []
-                    (_etype620, _size617) = iprot.readListBegin()
-                    for _i621 in range(_size617):
-                        _elem622 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.path.append(_elem622)
+                    (_etype627, _size624) = iprot.readListBegin()
+                    for _i628 in range(_size624):
+                        _elem629 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.path.append(_elem629)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -6788,16 +6852,16 @@
         if self.sessionId is not None:
             oprot.writeFieldBegin('sessionId', TType.I64, 1)
             oprot.writeI64(self.sessionId)
             oprot.writeFieldEnd()
         if self.path is not None:
             oprot.writeFieldBegin('path', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.path))
-            for iter623 in self.path:
-                oprot.writeString(iter623.encode('utf-8') if sys.version_info[0] == 2 else iter623)
+            for iter630 in self.path:
+                oprot.writeString(iter630.encode('utf-8') if sys.version_info[0] == 2 else iter630)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -6908,18 +6972,18 @@
                 if ftype == TType.I64:
                     self.sessionId = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.storageGroup = []
-                    (_etype627, _size624) = iprot.readListBegin()
-                    for _i628 in range(_size624):
-                        _elem629 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.storageGroup.append(_elem629)
+                    (_etype634, _size631) = iprot.readListBegin()
+                    for _i635 in range(_size631):
+                        _elem636 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.storageGroup.append(_elem636)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -6932,16 +6996,16 @@
         if self.sessionId is not None:
             oprot.writeFieldBegin('sessionId', TType.I64, 1)
             oprot.writeI64(self.sessionId)
             oprot.writeFieldEnd()
         if self.storageGroup is not None:
             oprot.writeFieldBegin('storageGroup', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.storageGroup))
-            for iter630 in self.storageGroup:
-                oprot.writeString(iter630.encode('utf-8') if sys.version_info[0] == 2 else iter630)
+            for iter637 in self.storageGroup:
+                oprot.writeString(iter637.encode('utf-8') if sys.version_info[0] == 2 else iter637)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -10395,14 +10459,139 @@
         return not (self == other)
 all_structs.append(dropSchemaTemplate_result)
 dropSchemaTemplate_result.thrift_spec = (
     (0, TType.STRUCT, 'success', [iotdb.thrift.common.ttypes.TSStatus, None], None, ),  # 0
 )
 
 
+class createTimeseriesUsingSchemaTemplate_args(object):
+    """
+    Attributes:
+     - req
+
+    """
+
+
+    def __init__(self, req=None,):
+        self.req = req
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRUCT:
+                    self.req = TCreateTimeseriesUsingSchemaTemplateReq()
+                    self.req.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('createTimeseriesUsingSchemaTemplate_args')
+        if self.req is not None:
+            oprot.writeFieldBegin('req', TType.STRUCT, 1)
+            self.req.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(createTimeseriesUsingSchemaTemplate_args)
+createTimeseriesUsingSchemaTemplate_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRUCT, 'req', [TCreateTimeseriesUsingSchemaTemplateReq, None], None, ),  # 1
+)
+
+
+class createTimeseriesUsingSchemaTemplate_result(object):
+    """
+    Attributes:
+     - success
+
+    """
+
+
+    def __init__(self, success=None,):
+        self.success = success
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.STRUCT:
+                    self.success = iotdb.thrift.common.ttypes.TSStatus()
+                    self.success.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('createTimeseriesUsingSchemaTemplate_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.STRUCT, 0)
+            self.success.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(createTimeseriesUsingSchemaTemplate_result)
+createTimeseriesUsingSchemaTemplate_result.thrift_spec = (
+    (0, TType.STRUCT, 'success', [iotdb.thrift.common.ttypes.TSStatus, None], None, ),  # 0
+)
+
+
 class handshake_args(object):
     """
     Attributes:
      - info
 
     """
```

### Comparing `apache-iotdb-1.1.0/iotdb/thrift/rpc/ttypes.py` & `apache-iotdb-1.1.2/iotdb/thrift/rpc/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3826,28 +3826,30 @@
      - fetchSize
      - startTime
      - endTime
      - statementId
      - enableRedirectQuery
      - jdbcQuery
      - timeout
+     - legalPathNodes
 
     """
 
 
-    def __init__(self, sessionId=None, paths=None, fetchSize=None, startTime=None, endTime=None, statementId=None, enableRedirectQuery=None, jdbcQuery=None, timeout=None,):
+    def __init__(self, sessionId=None, paths=None, fetchSize=None, startTime=None, endTime=None, statementId=None, enableRedirectQuery=None, jdbcQuery=None, timeout=None, legalPathNodes=None,):
         self.sessionId = sessionId
         self.paths = paths
         self.fetchSize = fetchSize
         self.startTime = startTime
         self.endTime = endTime
         self.statementId = statementId
         self.enableRedirectQuery = enableRedirectQuery
         self.jdbcQuery = jdbcQuery
         self.timeout = timeout
+        self.legalPathNodes = legalPathNodes
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -3900,14 +3902,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
                 if ftype == TType.I64:
                     self.timeout = iprot.readI64()
                 else:
                     iprot.skip(ftype)
+            elif fid == 10:
+                if ftype == TType.BOOL:
+                    self.legalPathNodes = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -3949,14 +3956,18 @@
             oprot.writeFieldBegin('jdbcQuery', TType.BOOL, 8)
             oprot.writeBool(self.jdbcQuery)
             oprot.writeFieldEnd()
         if self.timeout is not None:
             oprot.writeFieldBegin('timeout', TType.I64, 9)
             oprot.writeI64(self.timeout)
             oprot.writeFieldEnd()
+        if self.legalPathNodes is not None:
+            oprot.writeFieldBegin('legalPathNodes', TType.BOOL, 10)
+            oprot.writeBool(self.legalPathNodes)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.sessionId is None:
             raise TProtocolException(message='Required field sessionId is unset!')
         if self.paths is None:
@@ -3988,27 +3999,29 @@
      - paths
      - fetchSize
      - time
      - statementId
      - enableRedirectQuery
      - jdbcQuery
      - timeout
+     - legalPathNodes
 
     """
 
 
-    def __init__(self, sessionId=None, paths=None, fetchSize=None, time=None, statementId=None, enableRedirectQuery=None, jdbcQuery=None, timeout=None,):
+    def __init__(self, sessionId=None, paths=None, fetchSize=None, time=None, statementId=None, enableRedirectQuery=None, jdbcQuery=None, timeout=None, legalPathNodes=None,):
         self.sessionId = sessionId
         self.paths = paths
         self.fetchSize = fetchSize
         self.time = time
         self.statementId = statementId
         self.enableRedirectQuery = enableRedirectQuery
         self.jdbcQuery = jdbcQuery
         self.timeout = timeout
+        self.legalPathNodes = legalPathNodes
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -4056,14 +4069,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.I64:
                     self.timeout = iprot.readI64()
                 else:
                     iprot.skip(ftype)
+            elif fid == 9:
+                if ftype == TType.BOOL:
+                    self.legalPathNodes = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -4101,14 +4119,18 @@
             oprot.writeFieldBegin('jdbcQuery', TType.BOOL, 7)
             oprot.writeBool(self.jdbcQuery)
             oprot.writeFieldEnd()
         if self.timeout is not None:
             oprot.writeFieldBegin('timeout', TType.I64, 8)
             oprot.writeI64(self.timeout)
             oprot.writeFieldEnd()
+        if self.legalPathNodes is not None:
+            oprot.writeFieldBegin('legalPathNodes', TType.BOOL, 9)
+            oprot.writeBool(self.legalPathNodes)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.sessionId is None:
             raise TProtocolException(message='Required field sessionId is unset!')
         if self.paths is None:
@@ -4140,29 +4162,31 @@
      - aggregations
      - startTime
      - endTime
      - interval
      - slidingStep
      - fetchSize
      - timeout
+     - legalPathNodes
 
     """
 
 
-    def __init__(self, sessionId=None, statementId=None, paths=None, aggregations=None, startTime=None, endTime=None, interval=None, slidingStep=None, fetchSize=None, timeout=None,):
+    def __init__(self, sessionId=None, statementId=None, paths=None, aggregations=None, startTime=None, endTime=None, interval=None, slidingStep=None, fetchSize=None, timeout=None, legalPathNodes=None,):
         self.sessionId = sessionId
         self.statementId = statementId
         self.paths = paths
         self.aggregations = aggregations
         self.startTime = startTime
         self.endTime = endTime
         self.interval = interval
         self.slidingStep = slidingStep
         self.fetchSize = fetchSize
         self.timeout = timeout
+        self.legalPathNodes = legalPathNodes
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -4225,14 +4249,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 10:
                 if ftype == TType.I64:
                     self.timeout = iprot.readI64()
                 else:
                     iprot.skip(ftype)
+            elif fid == 11:
+                if ftype == TType.BOOL:
+                    self.legalPathNodes = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -4281,14 +4310,18 @@
             oprot.writeFieldBegin('fetchSize', TType.I32, 9)
             oprot.writeI32(self.fetchSize)
             oprot.writeFieldEnd()
         if self.timeout is not None:
             oprot.writeFieldBegin('timeout', TType.I64, 10)
             oprot.writeI64(self.timeout)
             oprot.writeFieldEnd()
+        if self.legalPathNodes is not None:
+            oprot.writeFieldBegin('legalPathNodes', TType.BOOL, 11)
+            oprot.writeBool(self.legalPathNodes)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.sessionId is None:
             raise TProtocolException(message='Required field sessionId is unset!')
         if self.statementId is None:
@@ -5528,14 +5561,94 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class TCreateTimeseriesUsingSchemaTemplateReq(object):
+    """
+    Attributes:
+     - sessionId
+     - devicePathList
+
+    """
+
+
+    def __init__(self, sessionId=None, devicePathList=None,):
+        self.sessionId = sessionId
+        self.devicePathList = devicePathList
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I64:
+                    self.sessionId = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.LIST:
+                    self.devicePathList = []
+                    (_etype613, _size610) = iprot.readListBegin()
+                    for _i614 in range(_size610):
+                        _elem615 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.devicePathList.append(_elem615)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('TCreateTimeseriesUsingSchemaTemplateReq')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.I64, 1)
+            oprot.writeI64(self.sessionId)
+            oprot.writeFieldEnd()
+        if self.devicePathList is not None:
+            oprot.writeFieldBegin('devicePathList', TType.LIST, 2)
+            oprot.writeListBegin(TType.STRING, len(self.devicePathList))
+            for iter616 in self.devicePathList:
+                oprot.writeString(iter616.encode('utf-8') if sys.version_info[0] == 2 else iter616)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        if self.sessionId is None:
+            raise TProtocolException(message='Required field sessionId is unset!')
+        if self.devicePathList is None:
+            raise TProtocolException(message='Required field devicePathList is unset!')
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class TSyncIdentityInfo(object):
     """
     Attributes:
      - pipeName
      - createTime
      - version
      - database
@@ -5912,19 +6025,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.connectionInfoList = []
-                    (_etype613, _size610) = iprot.readListBegin()
-                    for _i614 in range(_size610):
-                        _elem615 = TSConnectionInfo()
-                        _elem615.read(iprot)
-                        self.connectionInfoList.append(_elem615)
+                    (_etype620, _size617) = iprot.readListBegin()
+                    for _i621 in range(_size617):
+                        _elem622 = TSConnectionInfo()
+                        _elem622.read(iprot)
+                        self.connectionInfoList.append(_elem622)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5933,16 +6046,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TSConnectionInfoResp')
         if self.connectionInfoList is not None:
             oprot.writeFieldBegin('connectionInfoList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.connectionInfoList))
-            for iter616 in self.connectionInfoList:
-                iter616.write(oprot)
+            for iter623 in self.connectionInfoList:
+                iter623.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.connectionInfoList is None:
@@ -6238,40 +6351,43 @@
     (3, TType.I32, 'fetchSize', None, None, ),  # 3
     (4, TType.I64, 'startTime', None, None, ),  # 4
     (5, TType.I64, 'endTime', None, None, ),  # 5
     (6, TType.I64, 'statementId', None, None, ),  # 6
     (7, TType.BOOL, 'enableRedirectQuery', None, None, ),  # 7
     (8, TType.BOOL, 'jdbcQuery', None, None, ),  # 8
     (9, TType.I64, 'timeout', None, None, ),  # 9
+    (10, TType.BOOL, 'legalPathNodes', None, None, ),  # 10
 )
 all_structs.append(TSLastDataQueryReq)
 TSLastDataQueryReq.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'sessionId', None, None, ),  # 1
     (2, TType.LIST, 'paths', (TType.STRING, 'UTF8', False), None, ),  # 2
     (3, TType.I32, 'fetchSize', None, None, ),  # 3
     (4, TType.I64, 'time', None, None, ),  # 4
     (5, TType.I64, 'statementId', None, None, ),  # 5
     (6, TType.BOOL, 'enableRedirectQuery', None, None, ),  # 6
     (7, TType.BOOL, 'jdbcQuery', None, None, ),  # 7
     (8, TType.I64, 'timeout', None, None, ),  # 8
+    (9, TType.BOOL, 'legalPathNodes', None, None, ),  # 9
 )
 all_structs.append(TSAggregationQueryReq)
 TSAggregationQueryReq.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'sessionId', None, None, ),  # 1
     (2, TType.I64, 'statementId', None, None, ),  # 2
     (3, TType.LIST, 'paths', (TType.STRING, 'UTF8', False), None, ),  # 3
     (4, TType.LIST, 'aggregations', (TType.I32, None, False), None, ),  # 4
     (5, TType.I64, 'startTime', None, None, ),  # 5
     (6, TType.I64, 'endTime', None, None, ),  # 6
     (7, TType.I64, 'interval', None, None, ),  # 7
     (8, TType.I64, 'slidingStep', None, None, ),  # 8
     (9, TType.I32, 'fetchSize', None, None, ),  # 9
     (10, TType.I64, 'timeout', None, None, ),  # 10
+    (11, TType.BOOL, 'legalPathNodes', None, None, ),  # 11
 )
 all_structs.append(TSCreateMultiTimeseriesReq)
 TSCreateMultiTimeseriesReq.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'sessionId', None, None, ),  # 1
     (2, TType.LIST, 'paths', (TType.STRING, 'UTF8', False), None, ),  # 2
     (3, TType.LIST, 'dataTypes', (TType.I32, None, False), None, ),  # 3
@@ -6355,14 +6471,20 @@
 )
 all_structs.append(TSDropSchemaTemplateReq)
 TSDropSchemaTemplateReq.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'sessionId', None, None, ),  # 1
     (2, TType.STRING, 'templateName', 'UTF8', None, ),  # 2
 )
+all_structs.append(TCreateTimeseriesUsingSchemaTemplateReq)
+TCreateTimeseriesUsingSchemaTemplateReq.thrift_spec = (
+    None,  # 0
+    (1, TType.I64, 'sessionId', None, None, ),  # 1
+    (2, TType.LIST, 'devicePathList', (TType.STRING, 'UTF8', False), None, ),  # 2
+)
 all_structs.append(TSyncIdentityInfo)
 TSyncIdentityInfo.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'pipeName', 'UTF8', None, ),  # 1
     (2, TType.I64, 'createTime', None, None, ),  # 2
     (3, TType.STRING, 'version', 'UTF8', None, ),  # 3
     (4, TType.STRING, 'database', 'UTF8', None, ),  # 4
```

### Comparing `apache-iotdb-1.1.0/iotdb/tsfile/__init__.py` & `apache-iotdb-1.1.2/iotdb/tsfile/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/tsfile/common/__init__.py` & `apache-iotdb-1.1.2/iotdb/tsfile/common/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/tsfile/common/constant/TsFileConstant.py` & `apache-iotdb-1.1.2/iotdb/tsfile/common/constant/TsFileConstant.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/tsfile/common/constant/__init__.py` & `apache-iotdb-1.1.2/iotdb/tsfile/common/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/tsfile/utils/Pair.py` & `apache-iotdb-1.1.2/iotdb/tsfile/utils/Pair.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/tsfile/utils/ReadWriteIOUtils.py` & `apache-iotdb-1.1.2/iotdb/tsfile/utils/ReadWriteIOUtils.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/tsfile/utils/__init__.py` & `apache-iotdb-1.1.2/iotdb/tsfile/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/BitMap.py` & `apache-iotdb-1.1.2/iotdb/utils/BitMap.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/Field.py` & `apache-iotdb-1.1.2/iotdb/utils/Field.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/IoTDBConstants.py` & `apache-iotdb-1.1.2/iotdb/utils/IoTDBConstants.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     SNAPPY = 1
     GZIP = 2
     LZO = 3
     SDT = 4
     PAA = 5
     PLA = 6
     LZ4 = 7
+    ZSTD = 8
 
     # this method is implemented to avoid the issue reported by:
     # https://bugs.python.org/issue30545
     def __eq__(self, other) -> bool:
         return self.value == other.value
 
     def __hash__(self):
```

### Comparing `apache-iotdb-1.1.0/iotdb/utils/IoTDBRpcDataSet.py` & `apache-iotdb-1.1.2/iotdb/utils/IoTDBRpcDataSet.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/NumpyTablet.py` & `apache-iotdb-1.1.2/iotdb/utils/NumpyTablet.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/RowRecord.py` & `apache-iotdb-1.1.2/iotdb/utils/RowRecord.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/SessionDataSet.py` & `apache-iotdb-1.1.2/iotdb/utils/SessionDataSet.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/Tablet.py` & `apache-iotdb-1.1.2/iotdb/utils/Tablet.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/iotdb/utils/__init__.py` & `apache-iotdb-1.1.2/iotdb/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/pyproject.toml` & `apache-iotdb-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/setup.py` & `apache-iotdb-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     long_description = ""
 
 
 print(long_description)
 
 setuptools.setup(
     name="apache-iotdb",  # Replace with your own username
-    version="1.1.0",
+    version="1.1.2",
     author=" Apache Software Foundation",
     author_email="dev@iotdb.apache.org",
     description="Apache IoTDB client API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/apache/iotdb",
     packages=setuptools.find_packages(),
```

### Comparing `apache-iotdb-1.1.0/tests/__init__.py` & `apache-iotdb-1.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/tablet_performance_comparison.py` & `apache-iotdb-1.1.2/tests/tablet_performance_comparison.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_aligned_timeseries.py` & `apache-iotdb-1.1.2/tests/test_aligned_timeseries.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_dataframe.py` & `apache-iotdb-1.1.2/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_delete_data.py` & `apache-iotdb-1.1.2/tests/test_delete_data.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_numpy_tablet.py` & `apache-iotdb-1.1.2/tests/test_numpy_tablet.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_one_device.py` & `apache-iotdb-1.1.2/tests/test_one_device.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_session.py` & `apache-iotdb-1.1.2/tests/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # under the License.
 #
 
 # Uncomment the following line to use apache-iotdb module installed by pip3
 import numpy as np
 
 from iotdb.Session import Session
+from iotdb.SessionPool import PoolConfig, create_session_pool
 from iotdb.utils.BitMap import BitMap
 from iotdb.utils.IoTDBConstants import TSDataType, TSEncoding, Compressor
 from iotdb.utils.NumpyTablet import NumpyTablet
 from iotdb.utils.Tablet import Tablet
 from iotdb.IoTDBContainer import IoTDBContainer
 
 # whether the test has passed
@@ -42,17 +43,32 @@
     print("*********")
     print(message)
     print("*********")
     assert False
 
 
 def test_session():
+    session_test()
+
+
+def test_session_pool():
+    session_test(True)
+
+
+def session_test(use_session_pool=False):
     with IoTDBContainer("iotdb:dev") as db:
         db: IoTDBContainer
-        session = Session(db.get_container_host_ip(), db.get_exposed_port(6667))
+
+        if use_session_pool:
+            pool_config = PoolConfig(db.get_container_host_ip(), db.get_exposed_port(6667), "root", "root", 1024,
+                                     "Asia/Shanghai", 3)
+            session_pool = create_session_pool(pool_config, 1, 3000)
+            session = session_pool.get_session()
+        else:
+            session = Session(db.get_container_host_ip(), db.get_exposed_port(6667))
         session.open(False)
 
         if not session.is_open():
             print("can't open session")
             exit(1)
 
         # set and delete databases
@@ -150,22 +166,22 @@
             tags_lst_,
             attributes_lst_,
             None,
         )
 
         # delete time series
         if (
-            session.delete_time_series(
-                [
-                    "root.sg_test_01.d_01.s_07",
-                    "root.sg_test_01.d_01.s_08",
-                    "root.sg_test_01.d_01.s_09",
-                ]
-            )
-            < 0
+                session.delete_time_series(
+                    [
+                        "root.sg_test_01.d_01.s_07",
+                        "root.sg_test_01.d_01.s_08",
+                        "root.sg_test_01.d_01.s_09",
+                    ]
+                )
+                < 0
         ):
             test_fail()
             print_message("delete time series failed")
 
         # checking time series
         # s_07 expecting False
         if session.check_time_series_exists("root.sg_test_01.d_01.s_07"):
@@ -193,18 +209,18 @@
             TSDataType.INT32,
             TSDataType.INT64,
             TSDataType.FLOAT,
             TSDataType.DOUBLE,
             TSDataType.TEXT,
         ]
         if (
-            session.insert_record(
-                "root.sg_test_01.d_01", 1, measurements_, data_types_, values_
-            )
-            < 0
+                session.insert_record(
+                    "root.sg_test_01.d_01", 1, measurements_, data_types_, values_
+                )
+                < 0
         ):
             test_fail()
             print_message("insert record failed")
 
         # insert multiple records into database
         measurements_list_ = [
             ["s_01", "s_02", "s_03", "s_04", "s_05", "s_06"],
@@ -213,18 +229,18 @@
         values_list_ = [
             [False, 22, 33, 4.4, 55.1, "test_records01"],
             [True, 77, 88, 1.25, 8.125, "test_records02"],
         ]
         data_type_list_ = [data_types_, data_types_]
         device_ids_ = ["root.sg_test_01.d_01", "root.sg_test_01.d_02"]
         if (
-            session.insert_records(
-                device_ids_, [2, 3], measurements_list_, data_type_list_, values_list_
-            )
-            < 0
+                session.insert_records(
+                    device_ids_, [2, 3], measurements_list_, data_type_list_, values_list_
+                )
+                < 0
         ):
             test_fail()
             print_message("insert records failed")
 
         # insert one tablet into the database.
         values_ = [
             [False, 10, 11, 1.1, 10011.1, "test01"],
@@ -299,15 +315,15 @@
             np.array([11, 11111, 0, 0], np.dtype(">i8")),
             np.array([1.1, 1.25, 188.1, 0], np.dtype(">f4")),
             np.array([10011.1, 101.0, 688.25, 0], np.dtype(">f8")),
             np.array(["test01", "test02", "test03", ""]),
         ]
         np_timestamps_ = np.array([30, 31, 32, 33], np.dtype(">i8"))
         np_bitmaps_ = []
-        for i in range(len(measurements_)):
+        for _ in range(len(measurements_)):
             np_bitmaps_.append(BitMap(len(np_timestamps_)))
         np_bitmaps_[0].mark(0)
         np_bitmaps_[1].mark(1)
         np_bitmaps_[2].mark(2)
         np_bitmaps_[4].mark(3)
         np_bitmaps_[5].mark(3)
         np_tablet_ = NumpyTablet(
@@ -328,22 +344,22 @@
             [TSDataType.BOOLEAN, TSDataType.INT32, TSDataType.INT64],
             [TSDataType.BOOLEAN, TSDataType.INT32, TSDataType.INT64],
             [TSDataType.BOOLEAN, TSDataType.INT32, TSDataType.INT64],
         ]
         values_list = [[False, 22, 33], [True, 1, 23], [False, 15, 26]]
 
         if (
-            session.insert_records_of_one_device(
-                "root.sg_test_01.d_01",
-                time_list,
-                measurements_list,
-                data_types_list,
-                values_list,
-            )
-            < 0
+                session.insert_records_of_one_device(
+                    "root.sg_test_01.d_01",
+                    time_list,
+                    measurements_list,
+                    data_types_list,
+                    values_list,
+                )
+                < 0
         ):
             test_fail()
             print_message("insert records of one device failed")
 
         # execute non-query sql statement
         if (
             session.execute_non_query_statement(
```

### Comparing `apache-iotdb-1.1.0/tests/test_tablet.py` & `apache-iotdb-1.1.2/tests/test_tablet.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_template.py` & `apache-iotdb-1.1.2/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `apache-iotdb-1.1.0/tests/test_todf.py` & `apache-iotdb-1.1.2/tests/test_todf.py`

 * *Files identical despite different names*

