# Comparing `tmp/work-1.0.1.tar.gz` & `tmp/work-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.0.1.tar", max compression
+gzip compressed data, was "work-1.0.2.tar", max compression
```

## Comparing `work-1.0.1.tar` & `work-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.0.1/README.md
--rw-r--r--   0        0        0      592 2023-07-25 18:13:04.321615 work-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    88787 2023-07-25 18:11:55.336963 work-1.0.1/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.0.1/src/work_components/__init__.py
--rw-r--r--   0        0        0    24173 2023-07-20 13:19:00.050197 work-1.0.1/src/work_components/arguments.py
--rw-r--r--   0        0        0     2045 2023-07-25 18:13:09.261661 work-1.0.1/src/work_components/consts.py
--rw-r--r--   0        0        0    22034 2023-07-18 16:04:16.421220 work-1.0.1/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.0.1/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    15926 2023-07-05 14:46:26.049963 work-1.0.1/src/work_components/dao/core.py
--rw-r--r--   0        0        0     1523 2023-07-05 14:05:08.910489 work-1.0.1/src/work_components/dao/flags.py
--rw-r--r--   0        0        0    11530 2023-07-05 13:33:23.043915 work-1.0.1/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    11011 2023-07-19 09:32:06.070610 work-1.0.1/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     6209 2023-07-05 17:58:05.483335 work-1.0.1/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     4470 2023-07-25 18:11:55.340963 work-1.0.1/src/work_components/migrate.py
--rw-r--r--   0        0        0      344 2023-07-05 13:32:05.419111 work-1.0.1/src/work_components/protocols.py
--rw-r--r--   0        0        0      471 2023-06-20 12:46:12.229256 work-1.0.1/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8067 2023-07-11 18:36:01.409614 work-1.0.1/src/work_components/util.py
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 work-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.0.2/README.md
+-rw-r--r--   0        0        0      592 2023-07-28 11:30:43.175038 work-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    88783 2023-07-28 11:30:02.066801 work-1.0.2/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.0.2/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24173 2023-07-20 13:19:00.050197 work-1.0.2/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2045 2023-07-28 11:30:42.663035 work-1.0.2/src/work_components/consts.py
+-rw-r--r--   0        0        0    22034 2023-07-18 16:04:16.421220 work-1.0.2/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.0.2/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    15926 2023-07-05 14:46:26.049963 work-1.0.2/src/work_components/dao/core.py
+-rw-r--r--   0        0        0     1523 2023-07-28 11:29:52.010744 work-1.0.2/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0    11530 2023-07-05 13:33:23.043915 work-1.0.2/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    11011 2023-07-19 09:32:06.070610 work-1.0.2/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     6209 2023-07-05 17:58:05.483335 work-1.0.2/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     4470 2023-07-25 18:11:55.340963 work-1.0.2/src/work_components/migrate.py
+-rw-r--r--   0        0        0      344 2023-07-05 13:32:05.419111 work-1.0.2/src/work_components/protocols.py
+-rw-r--r--   0        0        0      471 2023-06-20 12:46:12.229256 work-1.0.2/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8067 2023-07-11 18:36:01.409614 work-1.0.2/src/work_components/util.py
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 work-1.0.2/PKG-INFO
```

### Comparing `work-1.0.1/README.md` & `work-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `work-1.0.1/pyproject.toml` & `work-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.0.1"
+version = "1.0.2"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.0.1/src/work.py` & `work-1.0.2/src/work.py`

 * *Files 0% similar despite different names*

```diff
@@ -1576,15 +1576,15 @@
         def to_selector(self, given_date: dt.date) -> str:
             """Transform given date to bucket selector."""
 
             # Handle special case of a week that spans multiple years...
             if (
                 self.name == "week"
                 and given_date.month == 1
-                and given_date.isocalendar().week >= 52
+                and given_date.isocalendar()[1] >= 52
             ):
                 # ...by always using Monday of that week for the selector.
                 given_date -= dt.timedelta(days=given_date.weekday())
 
             formatter: str = {
                 "day": "%Y-%m-%d",
                 "week": "%V-%G",
@@ -2289,15 +2289,15 @@
     def _minute_balance_up_to(self, day: dt.date) -> float:
         """
         Return the minute balance for all days in the given day's week, excluding itself.
         Correctly handles Monday and Sunday.
          see: `_minute_balance()`
         """
 
-        week_no: int = day.isocalendar().week
+        week_no: int = day.isocalendar()[1]
         week: List[dt.date] = self._containing_week(week_no=week_no)
         week_up_to: List[dt.date] = week[: week.index(day)]
 
         return self._minute_balance(week=week_up_to)
 
     ### Convenience functions ###
```

### Comparing `work-1.0.1/src/work_components/arguments.py` & `work-1.0.2/src/work_components/arguments.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/consts.py` & `work-1.0.2/src/work_components/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """ Shared constants """
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.0.1"
+VERSION: str = "1.0.2"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
```

### Comparing `work-1.0.1/src/work_components/container.py` & `work-1.0.2/src/work_components/container.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/dao/core.py` & `work-1.0.2/src/work_components/dao/core.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/dao/flags.py` & `work-1.0.2/src/work_components/dao/flags.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/dao/rc.py` & `work-1.0.2/src/work_components/dao/rc.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/dao/recess.py` & `work-1.0.2/src/work_components/dao/recess.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/dt_parse.py` & `work-1.0.2/src/work_components/dt_parse.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/migrate.py` & `work-1.0.2/src/work_components/migrate.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/src/work_components/util.py` & `work-1.0.2/src/work_components/util.py`

 * *Files identical despite different names*

### Comparing `work-1.0.1/PKG-INFO` & `work-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.0.1
+Version: 1.0.2
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

