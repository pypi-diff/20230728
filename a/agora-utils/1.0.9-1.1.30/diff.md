# Comparing `tmp/agora_utils-1.0.9-py2.py3-none-any.whl.zip` & `tmp/agora_utils-1.1.30-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2445 bytes, number of entries: 8
--rw-r--r--  2.0 fat       74 b- defN 23-Feb-13 15:17 agora_utils/__init__.py
--rw-r--r--  2.0 fat       22 b- defN 23-Jan-23 16:40 agora_utils/_version.py
--rw-r--r--  2.0 fat      486 b- defN 23-Feb-13 14:30 agora_utils/agora_time.py
--rw-r--r--  2.0 fat       24 b- defN 23-Mar-16 20:19 agora_utils/version.py
--rw-r--r--  2.0 fat      139 b- defN 23-Mar-07 09:10 agora_utils-1.0.9.dist-info/LICENSE
-?rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.0.9.dist-info/WHEEL
-?rw-r--r--  2.0 fat      719 b- defN 16-Jan-01 00:00 agora_utils-1.0.9.dist-info/METADATA
-?rw-r--r--  2.0 fat      622 b- defN 16-Jan-01 00:00 agora_utils-1.0.9.dist-info/RECORD
-8 files, 2185 bytes uncompressed, 1353 bytes compressed:  38.1%
+Zip file size: 2560 bytes, number of entries: 8
+-rw-r--r--  2.0 fat       75 b- defN 23-May-12 13:38 agora_utils/__init__.py
+-rw-r--r--  2.0 fat       23 b- defN 23-May-12 13:38 agora_utils/_version.py
+-rw-r--r--  2.0 fat      521 b- defN 23-Jul-27 17:24 agora_utils/agora_time.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 11:19 agora_utils/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_utils-1.1.30.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.1.30.dist-info/WHEEL
+-rw-r--r--  2.0 fat      880 b- defN 16-Jan-01 00:00 agora_utils-1.1.30.dist-info/METADATA
+-rw-r--r--  2.0 fat      626 b- defN 16-Jan-01 00:00 agora_utils-1.1.30.dist-info/RECORD
+8 files, 2383 bytes uncompressed, 1460 bytes compressed:  38.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: agora_utils/agora_time.py
 Comment: 
 
 Filename: agora_utils/version.py
 Comment: 
 
-Filename: agora_utils-1.0.9.dist-info/LICENSE
+Filename: agora_utils-1.1.30.dist-info/LICENSE
 Comment: 
 
-Filename: agora_utils-1.0.9.dist-info/WHEEL
+Filename: agora_utils-1.1.30.dist-info/WHEEL
 Comment: 
 
-Filename: agora_utils-1.0.9.dist-info/METADATA
+Filename: agora_utils-1.1.30.dist-info/METADATA
 Comment: 
 
-Filename: agora_utils-1.0.9.dist-info/RECORD
+Filename: agora_utils-1.1.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_utils/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-from .agora_time import AgoraTimeStamp
+from .agora_time import AgoraTimeStamp
 from .agora_time import UTCDateTime
```

## agora_utils/_version.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-__version__ = "1.0.4"
+__version__ = "1.0.4"
```

## agora_utils/agora_time.py

```diff
@@ -1,12 +1,15 @@
 from datetime import datetime, timezone
 
-def AgoraTimeStamp(tm = datetime.utcnow()) -> float:
-    dt_utc = datetime(tm.year, tm.month, tm.day, 
-                      tm.hour, tm.minute, tm.second, tm. microsecond, 
+def AgoraTimeStamp(tm=-1) -> float:
+    if tm == -1:
+        tm = datetime.utcnow()
+    dt_utc = datetime(tm.year, tm.month, tm.day,
+                      tm.hour, tm.minute, tm.second, tm.microsecond,
                       tzinfo=timezone.utc)
     delta = dt_utc.timestamp() - tm.timestamp()
     return (tm.timestamp() + delta) * 1000
 
-def UTCDateTime(tm:float) -> datetime:
+
+def UTCDateTime(tm: float) -> datetime:
     dt = datetime.utcfromtimestamp(tm/1000).replace(tzinfo=timezone.utc)
-    return dt
+    return dt
```

## agora_utils/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.9'
+__version__ = '1.1.30'
```

