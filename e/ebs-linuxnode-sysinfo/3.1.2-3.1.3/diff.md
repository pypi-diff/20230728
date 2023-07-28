# Comparing `tmp/ebs-linuxnode-sysinfo-3.1.2.tar.gz` & `tmp/ebs-linuxnode-sysinfo-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebs-linuxnode-sysinfo-3.1.2.tar", last modified: Tue Apr  4 11:38:28 2023, max compression
+gzip compressed data, was "ebs-linuxnode-sysinfo-3.1.3.tar", last modified: Fri Jul 28 15:51:33 2023, max compression
```

## Comparing `ebs-linuxnode-sysinfo-3.1.2.tar` & `ebs-linuxnode-sysinfo-3.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-04 11:38:28.902215 ebs-linuxnode-sysinfo-3.1.2/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      644 2023-04-04 11:38:28.902215 ebs-linuxnode-sysinfo-3.1.2/PKG-INFO
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-04 11:38:28.898215 ebs-linuxnode-sysinfo-3.1.2/ebs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-04 11:38:28.898215 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-04 11:38:28.902215 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       34 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      958 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/app.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1664 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      331 2023-04-04 11:11:40.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      788 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/cpu.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      759 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/disks.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2133 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/display.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4567 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/host.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      784 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/memory.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1856 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/mixin.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2454 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/network.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1192 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/status.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2585 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/temperature.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1250 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/versions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-04 11:38:28.902215 ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      644 2023-04-04 11:38:28.000000 ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      743 2023-04-04 11:38:28.000000 ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-04 11:38:28.000000 ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2023-04-04 11:38:28.000000 ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2023-04-04 11:38:28.000000 ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1027 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/example.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2023-04-04 11:38:28.902215 ebs-linuxnode-sysinfo-3.1.2/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1046 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.2/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-28 15:51:33.959940 ebs-linuxnode-sysinfo-3.1.3/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      644 2023-07-28 15:51:33.959940 ebs-linuxnode-sysinfo-3.1.3/PKG-INFO
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-28 15:51:33.959940 ebs-linuxnode-sysinfo-3.1.3/ebs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-28 15:51:33.959940 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       64 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-28 15:51:33.959940 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       34 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      958 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/app.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1753 2023-07-28 15:11:07.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      331 2023-04-04 11:11:40.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      788 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/cpu.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      759 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/disks.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2133 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/display.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4567 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/host.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      784 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/memory.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1856 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/mixin.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2454 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/network.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1721 2023-07-28 15:10:33.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/status.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2585 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/temperature.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1250 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/versions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-28 15:51:33.959940 ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      644 2023-07-28 15:51:33.000000 ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      743 2023-07-28 15:51:33.000000 ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-28 15:51:33.000000 ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2023-07-28 15:51:33.000000 ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2023-07-28 15:51:33.000000 ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1027 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/example.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2023-07-28 15:51:33.959940 ebs-linuxnode-sysinfo-3.1.3/setup.cfg
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1046 2023-03-15 17:11:01.000000 ebs-linuxnode-sysinfo-3.1.3/setup.py
```

### Comparing `ebs-linuxnode-sysinfo-3.1.2/.gitignore` & `ebs-linuxnode-sysinfo-3.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/PKG-INFO` & `ebs-linuxnode-sysinfo-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebs-linuxnode-sysinfo
-Version: 3.1.2
+Version: 3.1.3
 Summary: System Information Providers for EBS IOT Applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-sysinfo
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/app.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/app.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/base.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from twisted.internet.defer import inlineCallbacks
 
 
 class SysInfoBase(object):
     def __init__(self, actual):
         self._log = None
         self._actual = actual
+        self._post_read = None
         self._items = {}
 
     @property
     def log(self):
         return self._log or self._actual.log
 
     @property
@@ -43,14 +44,16 @@
             elif hasattr(self, v):
                 if callable(getattr(self, v)):
                     rval[k] = yield getattr(self, v)()
                 else:
                     rval[k] = yield getattr(self, v)
             else:
                 rval[k] = v
+        if self._post_read:
+            self._post_read()
         return rval
 
     def __getattr__(self, item):
         if item in self.items.keys():
             v = self.items[item]
             if callable(v):
                 return v()
```

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/cpu.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/cpu.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/disks.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/disks.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/display.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/display.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/host.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/host.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/memory.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/memory.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/mixin.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/mixin.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/network.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/network.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/status.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/status.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,29 @@
 from .temperature import TemperatureInfo
 from .base import SysInfoBase
 
 from twisted.internet import threads
 from twisted.internet.defer import inlineCallbacks
 
 
+class CustomStatusBlock(SysInfoBase):
+    keys = []
+
+    def __init__(self, actual, post_read=None):
+        super(CustomStatusBlock, self).__init__(actual)
+        self._post_read = post_read
+
+    def install(self):
+        super(CustomStatusBlock, self).install()
+        for x in self.keys:
+            if not hasattr(self, x):
+                setattr(self, x, None)
+        self._items = {x: x for x in self.keys}
+
+
 class StatusInfo(SysInfoBase):
     def __init__(self, *args):
         super(StatusInfo, self).__init__(*args)
 
     def install(self):
         super(StatusInfo, self).install()
         temperature = TemperatureInfo(self.actual)
@@ -34,11 +49,15 @@
             'cpu': cpu,
             'disks': disks,
             'memory': memory,
             'display': display,
             'temperature': temperature,
         }
 
+    def register_status_block(self, name, block):
+        block.install()
+        self._items[name] = block
+
     @inlineCallbacks
     def _uptime(self):
         boot_time = yield threads.deferToThread(psutil.boot_time)
         return time.time() - boot_time
```

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/temperature.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/temperature.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs/linuxnode/sysinfo/versions.py` & `ebs-linuxnode-sysinfo-3.1.3/ebs/linuxnode/sysinfo/versions.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/PKG-INFO` & `ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebs-linuxnode-sysinfo
-Version: 3.1.2
+Version: 3.1.3
 Summary: System Information Providers for EBS IOT Applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-sysinfo
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ebs-linuxnode-sysinfo-3.1.2/ebs_linuxnode_sysinfo.egg-info/SOURCES.txt` & `ebs-linuxnode-sysinfo-3.1.3/ebs_linuxnode_sysinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/example.py` & `ebs-linuxnode-sysinfo-3.1.3/example.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-sysinfo-3.1.2/setup.py` & `ebs-linuxnode-sysinfo-3.1.3/setup.py`

 * *Files identical despite different names*

