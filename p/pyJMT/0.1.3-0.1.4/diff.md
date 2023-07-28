# Comparing `tmp/pyJMT-0.1.3.tar.gz` & `tmp/pyJMT-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyJMT-0.1.3.tar", last modified: Fri Jul 28 12:21:50 2023, max compression
+gzip compressed data, was "pyJMT-0.1.4.tar", last modified: Fri Jul 28 16:09:22 2023, max compression
```

## Comparing `pyJMT-0.1.3.tar` & `pyJMT-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 12:21:50.791403 pyJMT-0.1.3/
--rw-rw-r--   0 james     (1000) james     (1000)     1500 2023-07-28 09:57:16.000000 pyJMT-0.1.3/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)     1267 2023-07-28 12:21:50.791403 pyJMT-0.1.3/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      963 2023-07-28 12:21:18.000000 pyJMT-0.1.3/README.md
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 12:21:50.791403 pyJMT-0.1.3/pyJMT/
--rw-rw-r--   0 james     (1000) james     (1000)      631 2023-07-28 11:59:07.000000 pyJMT-0.1.3/pyJMT/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)     1547 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/classes.py
--rw-rw-r--   0 james     (1000) james     (1000)      302 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/drop_strategies.py
--rw-rw-r--   0 james     (1000) james     (1000)      109 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/link.py
--rw-rw-r--   0 james     (1000) james     (1000)     1794 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/metrics.py
--rw-rw-r--   0 james     (1000) james     (1000)    54632 2023-07-28 12:06:06.000000 pyJMT-0.1.3/pyJMT/network.py
--rw-rw-r--   0 james     (1000) james     (1000)    17008 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/nodes.py
--rw-rw-r--   0 james     (1000) james     (1000)     1463 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/routing_strategies.py
--rw-rw-r--   0 james     (1000) james     (1000)     2339 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/scheduling_strategies.py
--rw-rw-r--   0 james     (1000) james     (1000)     7388 2023-07-28 09:43:04.000000 pyJMT-0.1.3/pyJMT/service_distributions.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 12:21:50.791403 pyJMT-0.1.3/pyJMT.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)     1267 2023-07-28 12:21:50.000000 pyJMT-0.1.3/pyJMT.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      400 2023-07-28 12:21:50.000000 pyJMT-0.1.3/pyJMT.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2023-07-28 12:21:50.000000 pyJMT-0.1.3/pyJMT.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)       31 2023-07-28 12:21:50.000000 pyJMT-0.1.3/pyJMT.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)        6 2023-07-28 12:21:50.000000 pyJMT-0.1.3/pyJMT.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)       38 2023-07-28 12:21:50.791403 pyJMT-0.1.3/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)      648 2023-07-28 12:11:37.000000 pyJMT-0.1.3/setup.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 12:21:50.791403 pyJMT-0.1.3/test/
--rw-rw-r--   0 james     (1000) james     (1000)    35185 2023-07-28 11:59:07.000000 pyJMT-0.1.3/test/test_xml.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 16:09:22.977812 pyJMT-0.1.4/
+-rw-rw-r--   0 james     (1000) james     (1000)     1500 2023-07-28 09:57:16.000000 pyJMT-0.1.4/LICENSE
+-rw-rw-r--   0 james     (1000) james     (1000)     1267 2023-07-28 16:09:22.977812 pyJMT-0.1.4/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      963 2023-07-28 12:21:18.000000 pyJMT-0.1.4/README.md
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 16:09:22.977812 pyJMT-0.1.4/pyJMT/
+-rw-rw-r--   0 james     (1000) james     (1000)      631 2023-07-28 11:59:07.000000 pyJMT-0.1.4/pyJMT/__init__.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1547 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/classes.py
+-rw-rw-r--   0 james     (1000) james     (1000)      302 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/drop_strategies.py
+-rw-rw-r--   0 james     (1000) james     (1000)      109 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/link.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1794 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/metrics.py
+-rw-rw-r--   0 james     (1000) james     (1000)    54613 2023-07-28 15:49:58.000000 pyJMT-0.1.4/pyJMT/network.py
+-rw-rw-r--   0 james     (1000) james     (1000)    17008 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/nodes.py
+-rw-rw-r--   0 james     (1000) james     (1000)     1463 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/routing_strategies.py
+-rw-rw-r--   0 james     (1000) james     (1000)     2339 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/scheduling_strategies.py
+-rw-rw-r--   0 james     (1000) james     (1000)     7388 2023-07-28 09:43:04.000000 pyJMT-0.1.4/pyJMT/service_distributions.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 16:09:22.977812 pyJMT-0.1.4/pyJMT.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)     1267 2023-07-28 16:09:22.000000 pyJMT-0.1.4/pyJMT.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      400 2023-07-28 16:09:22.000000 pyJMT-0.1.4/pyJMT.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2023-07-28 16:09:22.000000 pyJMT-0.1.4/pyJMT.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       31 2023-07-28 16:09:22.000000 pyJMT-0.1.4/pyJMT.egg-info/requires.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        6 2023-07-28 16:09:22.000000 pyJMT-0.1.4/pyJMT.egg-info/top_level.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2023-07-28 16:09:22.977812 pyJMT-0.1.4/setup.cfg
+-rw-rw-r--   0 james     (1000) james     (1000)      648 2023-07-28 16:07:25.000000 pyJMT-0.1.4/setup.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-07-28 16:09:22.977812 pyJMT-0.1.4/test/
+-rw-rw-r--   0 james     (1000) james     (1000)    35185 2023-07-28 11:59:07.000000 pyJMT-0.1.4/test/test_xml.py
```

### Comparing `pyJMT-0.1.3/LICENSE` & `pyJMT-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/PKG-INFO` & `pyJMT-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyJMT
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python wrapper for Java Modelling Tools (JMT)
 Home-page: UNKNOWN
 Author: James Stadler
 Author-email: jws22@ic.ac.uk
 License: BSD 3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `pyJMT-0.1.3/README.md` & `pyJMT-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT/__init__.py` & `pyJMT-0.1.4/pyJMT/__init__.py`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT/classes.py` & `pyJMT-0.1.4/pyJMT/classes.py`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT/metrics.py` & `pyJMT-0.1.4/pyJMT/metrics.py`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT/network.py` & `pyJMT-0.1.4/pyJMT/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,29 +552,31 @@
                     probabilityParm = ET.SubElement(empiricalEntryParm, "subParameter", classPath="java.lang.Double",
                                                     name="probability")
                     ET.SubElement(probabilityParm, "value").text = "1.0"
 
         for join in self.nodes['joins']:
             node = ET.SubElement(sim, "node", name=join.name)
 
-            ET.SubElement(node, "section", className="ServiceTunnel")
 
             # generate join section
             joinSection = ET.SubElement(node, "section", className="Join")
             parm = ET.SubElement(joinSection, "parameter", array="true",
                                  classPath="jmt.engine.NetStrategies.JoinStrategy", name="JoinStrategy")
             for jobclass in self.classes:
                 ET.SubElement(parm, "refClass").text = jobclass.name
                 outersubparm = ET.SubElement(parm, "subParameter",
                                              classPath="jmt.engine.NetStrategies.JoinStrategies.NormalJoin",
                                              name="Standard Join")
                 innersubparm = ET.SubElement(outersubparm, "subParameter", classPath="java.lang.Integer",
                                              name="numRequired")
                 ET.SubElement(innersubparm, "value").text = "-1"
 
+            ET.SubElement(node, "section", className="ServiceTunnel")
+
+
             self.generate_router(join, node)
 
         for logger in self.nodes['loggers']:
             node = ET.SubElement(sim, "node", name=logger.name)
 
             self.generate_queuesection(logger, node)
 
@@ -658,15 +660,15 @@
             tree.write(f, encoding='ISO-8859-1', xml_declaration=True)
 
         tree.write(fileName)
 
     def generate_metrics(self, sim):
         if self.defaultMetrics:
             # TODO CHECK WHAT DEFAULTS SHOULD BE EXACTLY
-            measuresQueue = ["Number of Customers", "Utilization", "Response Time", "Throughput", "Arrival Rate"] #TODO RESIDENCE TIME
+            measuresQueue = ["Number of Customers", "Utilization", "Response Time", "Throughput", "Arrival Rate"]
             for measure in measuresQueue:
                 for queue in self.nodes['queues']:
                     for oclass in queue.services.keys():
                         ET.SubElement(sim, "measure", alpha="0.01", name=f"{queue.name}_{oclass}_{measure}",
                                       nodeType="station",
                                       precision="0.03", referenceNode=queue.name, referenceUserClass=f"{oclass}",
                                       type=measure,
```

### Comparing `pyJMT-0.1.3/pyJMT/nodes.py` & `pyJMT-0.1.4/pyJMT/nodes.py`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT/routing_strategies.py` & `pyJMT-0.1.4/pyJMT/routing_strategies.py`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT/scheduling_strategies.py` & `pyJMT-0.1.4/pyJMT/scheduling_strategies.py`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT/service_distributions.py` & `pyJMT-0.1.4/pyJMT/service_distributions.py`

 * *Files identical despite different names*

### Comparing `pyJMT-0.1.3/pyJMT.egg-info/PKG-INFO` & `pyJMT-0.1.4/pyJMT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyJMT
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python wrapper for Java Modelling Tools (JMT)
 Home-page: UNKNOWN
 Author: James Stadler
 Author-email: jws22@ic.ac.uk
 License: BSD 3-Clause
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `pyJMT-0.1.3/setup.py` & `pyJMT-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyJMT',
-    version='0.1.3',
+    version='0.1.4',
     author='James Stadler',
     author_email='jws22@ic.ac.uk',
     packages=find_packages(exclude=["test*", "docs*"]),
     license="BSD 3-Clause",
     description='A python wrapper for Java Modelling Tools (JMT)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `pyJMT-0.1.3/test/test_xml.py` & `pyJMT-0.1.4/test/test_xml.py`

 * *Files identical despite different names*

