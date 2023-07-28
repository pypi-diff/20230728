# Comparing `tmp/airflowconversion-1.0.1.tar.gz` & `tmp/airflowconversion-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflowconversion-1.0.1.tar", last modified: Tue Jul 18 08:53:46 2023, max compression
+gzip compressed data, was "airflowconversion-1.0.2.tar", last modified: Fri Jul 28 06:20:40 2023, max compression
```

## Comparing `airflowconversion-1.0.1.tar` & `airflowconversion-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 08:53:46.097988 airflowconversion-1.0.1/
--rw-rw-rw-   0        0        0      764 2023-07-18 08:53:46.097988 airflowconversion-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-18 08:48:52.000000 airflowconversion-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 08:53:46.069191 airflowconversion-1.0.1/airflowconversion/
--rw-rw-rw-   0        0        0     2939 2023-07-18 06:27:29.000000 airflowconversion-1.0.1/airflowconversion/ParseXML.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:53:46.097988 airflowconversion-1.0.1/airflowconversion/airflowconversion.egg-info/
--rw-rw-rw-   0        0        0      764 2023-07-18 08:53:45.000000 airflowconversion-1.0.1/airflowconversion/airflowconversion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-18 08:53:45.000000 airflowconversion-1.0.1/airflowconversion/airflowconversion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 08:53:45.000000 airflowconversion-1.0.1/airflowconversion/airflowconversion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 08:53:45.000000 airflowconversion-1.0.1/airflowconversion/airflowconversion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 08:53:46.097988 airflowconversion-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-07-18 08:52:29.000000 airflowconversion-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:20:40.380359 airflowconversion-1.0.2/
+-rw-rw-rw-   0        0        0      764 2023-07-28 06:20:40.378367 airflowconversion-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-18 08:48:52.000000 airflowconversion-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 06:20:40.363363 airflowconversion-1.0.2/airflowconversion/
+-rw-rw-rw-   0        0        0     3044 2023-07-26 12:06:32.000000 airflowconversion-1.0.2/airflowconversion/ParseXML.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:20:40.375358 airflowconversion-1.0.2/airflowconversion/airflowconversion.egg-info/
+-rw-rw-rw-   0        0        0      764 2023-07-28 06:20:40.000000 airflowconversion-1.0.2/airflowconversion/airflowconversion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-28 06:20:40.000000 airflowconversion-1.0.2/airflowconversion/airflowconversion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 06:20:40.000000 airflowconversion-1.0.2/airflowconversion/airflowconversion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 06:20:40.000000 airflowconversion-1.0.2/airflowconversion/airflowconversion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 06:20:40.380359 airflowconversion-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-07-28 06:18:54.000000 airflowconversion-1.0.2/setup.py
```

### Comparing `airflowconversion-1.0.1/PKG-INFO` & `airflowconversion-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflowconversion
-Version: 1.0.1
+Version: 1.0.2
 Summary: Converting Oozie workflows in XML to Python (Airflow Syntax)
 Home-page: https://repo1.uhc.com/artifactory/api/pypi/pypi-virtual/simple
 Author: Rashi Agarwal
 Author-email: rashi_agarwal@optum.com
 Description-Content-Type: text/markdown
 
 ## Python Utility tool for migration of workflows from Oozie to Airflow
```

### Comparing `airflowconversion-1.0.1/airflowconversion/ParseXML.py` & `airflowconversion-1.0.2/airflowconversion/ParseXML.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from StartingNode import StartingNode
 from UndefinedNodes import Undefined
 
 arr = []
 
 global cnt
 
+input_dir=r"C:\Users\ragarw59\Documents\AirflowMigration\Git\PythonPackage\input"
 
 ##checking dependency
 
 # MAIN
 
 def process_file(xmlfile, queue,output_dir):
     ## xml file is parsed
@@ -44,15 +45,14 @@
         print(child[i].tag)
     
     ## the dag and the child array is passed to the startingnode and then the returned value is stored in string1
     start_node=StartingNode(child,dag,queue)
     string1=start_node.starting_node()
 
     ## recursion starts, by passing the value of the node that start element points to.
-    #dependency_flow(child,dag,string1,mylist,dagarr,queue)
     depend=DependencyFlow(child,dag,string1,mylist,dagarr,queue)
     depend.dependency_flow()
     #print("dag sequence is: ",dag.sequence,"\n\n")
 
     ## create object of the Traverse class
     node1=Traverse(dag,queue,root,dagname)
     ## call the node_traversal method which will append all the mapped ozzie nodes to the python file
@@ -75,10 +75,10 @@
 #         self.output_dir=output_dir
 #         self.queue=queue
 def conversion(input_dir,output_dir,queue):
         os.chdir(input_dir)
         for file in glob.glob("*.xml"):
             process_file(file, queue,output_dir)
 
-# conv=conversion(input_dir)
+# conv=conversion(input_dir,r"C:\Users\ragarw59\Documents\AirflowMigration\Git\PythonPackage\output",'opsitst')
 # conv.conversion_main()
```

### Comparing `airflowconversion-1.0.1/airflowconversion/airflowconversion.egg-info/PKG-INFO` & `airflowconversion-1.0.2/airflowconversion/airflowconversion.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflowconversion
-Version: 1.0.1
+Version: 1.0.2
 Summary: Converting Oozie workflows in XML to Python (Airflow Syntax)
 Home-page: https://repo1.uhc.com/artifactory/api/pypi/pypi-virtual/simple
 Author: Rashi Agarwal
 Author-email: rashi_agarwal@optum.com
 Description-Content-Type: text/markdown
 
 ## Python Utility tool for migration of workflows from Oozie to Airflow
```

### Comparing `airflowconversion-1.0.1/setup.py` & `airflowconversion-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md","r") as fh:
     long_description=fh.read()
 setup(
     name='airflowconversion',
-    version='1.0.1',
+    version='1.0.2',
     description='Converting Oozie workflows in XML to Python (Airflow Syntax)',
     py_modules=["ParseXML"],
     package_dir={'': 'airflowconversion'},
     url="https://repo1.uhc.com/artifactory/api/pypi/pypi-virtual/simple",
     author="Rashi Agarwal",
     author_email="rashi_agarwal@optum.com",
     long_description=long_description,
```

