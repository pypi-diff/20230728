# Comparing `tmp/hirmeos-crossref-citedby-driver-0.1.0.tar.gz` & `tmp/hirmeos-crossref-citedby-driver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hirmeos-crossref-citedby-driver-0.1.0.tar", last modified: Fri Jul 28 09:52:37 2023, max compression
+gzip compressed data, was "hirmeos-crossref-citedby-driver-0.1.1.tar", last modified: Fri Jul 28 11:54:11 2023, max compression
```

## Comparing `hirmeos-crossref-citedby-driver-0.1.0.tar` & `hirmeos-crossref-citedby-driver-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1077 2023-07-26 16:14:03.000000 hirmeos-crossref-citedby-driver-0.1.0/LICENSE
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1444 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/PKG-INFO
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1014 2023-07-28 09:51:33.000000 hirmeos-crossref-citedby-driver-0.1.0/README.rst
--rw-r--r--   0 rowan     (1000) rowan     (1000)      616 2023-07-28 08:04:23.000000 hirmeos-crossref-citedby-driver-0.1.0/pyproject.toml
--rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/setup.cfg
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.930683 hirmeos-crossref-citedby-driver-0.1.0/src/
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.930683 hirmeos-crossref-citedby-driver-0.1.0/src/crossref_citedby_driver/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     6286 2023-07-28 09:41:19.000000 hirmeos-crossref-citedby-driver-0.1.0/src/crossref_citedby_driver/__init__.py
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1444 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/PKG-INFO
--rw-r--r--   0 rowan     (1000) rowan     (1000)      382 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/SOURCES.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/dependency_links.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       63 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/requires.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       24 2023-07-28 09:52:37.000000 hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/top_level.txt
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 09:52:37.934016 hirmeos-crossref-citedby-driver-0.1.0/tests/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     4926 2023-06-09 15:33:17.000000 hirmeos-crossref-citedby-driver-0.1.0/tests/tests.py
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 11:54:11.081573 hirmeos-crossref-citedby-driver-0.1.1/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1077 2023-07-26 16:14:03.000000 hirmeos-crossref-citedby-driver-0.1.1/LICENSE
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1793 2023-07-28 11:54:11.081573 hirmeos-crossref-citedby-driver-0.1.1/PKG-INFO
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1310 2023-07-28 11:51:03.000000 hirmeos-crossref-citedby-driver-0.1.1/README.rst
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      689 2023-07-28 11:53:50.000000 hirmeos-crossref-citedby-driver-0.1.1/pyproject.toml
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2023-07-28 11:54:11.081573 hirmeos-crossref-citedby-driver-0.1.1/setup.cfg
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 11:54:11.078240 hirmeos-crossref-citedby-driver-0.1.1/src/
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 11:54:11.078240 hirmeos-crossref-citedby-driver-0.1.1/src/crossref_citedby_driver/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     6672 2023-07-28 11:46:34.000000 hirmeos-crossref-citedby-driver-0.1.1/src/crossref_citedby_driver/__init__.py
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 11:54:11.081573 hirmeos-crossref-citedby-driver-0.1.1/src/hirmeos_crossref_citedby_driver.egg-info/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1793 2023-07-28 11:54:11.000000 hirmeos-crossref-citedby-driver-0.1.1/src/hirmeos_crossref_citedby_driver.egg-info/PKG-INFO
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      382 2023-07-28 11:54:11.000000 hirmeos-crossref-citedby-driver-0.1.1/src/hirmeos_crossref_citedby_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2023-07-28 11:54:11.000000 hirmeos-crossref-citedby-driver-0.1.1/src/hirmeos_crossref_citedby_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       63 2023-07-28 11:54:11.000000 hirmeos-crossref-citedby-driver-0.1.1/src/hirmeos_crossref_citedby_driver.egg-info/requires.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       24 2023-07-28 11:54:11.000000 hirmeos-crossref-citedby-driver-0.1.1/src/hirmeos_crossref_citedby_driver.egg-info/top_level.txt
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-28 11:54:11.081573 hirmeos-crossref-citedby-driver-0.1.1/tests/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     4926 2023-06-09 15:33:17.000000 hirmeos-crossref-citedby-driver-0.1.1/tests/tests.py
```

### Comparing `hirmeos-crossref-citedby-driver-0.1.0/LICENSE` & `hirmeos-crossref-citedby-driver-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hirmeos-crossref-citedby-driver-0.1.0/PKG-INFO` & `hirmeos-crossref-citedby-driver-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hirmeos-crossref-citedby-driver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions required by the crossref-citedby-driver
-Author-email: Rowan Hatherley <rowan.hatherley@ubiquitypress.com>
+Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>, Rowan Hatherley <rowan.hatherley@ubiquitypress.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -18,14 +18,26 @@
 
 Allows users to fecth citations from the crossref cited-by API.
 
 
 Release Notes:
 ==============
 
+[0.1.1] - 2023-07-28
+--------------------
+
+Added:
+    - Attempt to fix breaking changes: Temporarily added fetch_citation_xml,
+      get_crossref_citations and get_citation_data functions
+
+Changed:
+    - **Bugfix** | Timestamp format now uses "YYYY-MM-DD", not "YYYYMMDD"
+
+
+def get_citation_data
 
 [0.1.0] - 2023-07-28
 --------------------
 
 Changed:
     - Functions are now run as methods, via the CrossrefCitedByClient class
```

### Comparing `hirmeos-crossref-citedby-driver-0.1.0/README.rst` & `hirmeos-crossref-citedby-driver-0.1.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,26 @@
 
 Allows users to fecth citations from the crossref cited-by API.
 
 
 Release Notes:
 ==============
 
+[0.1.1] - 2023-07-28
+--------------------
+
+Added:
+    - Attempt to fix breaking changes: Temporarily added fetch_citation_xml,
+      get_crossref_citations and get_citation_data functions
+
+Changed:
+    - **Bugfix** | Timestamp format now uses "YYYY-MM-DD", not "YYYYMMDD"
+
+
+def get_citation_data
 
 [0.1.0] - 2023-07-28
 --------------------
 
 Changed:
     - Functions are now run as methods, via the CrossrefCitedByClient class
```

### Comparing `hirmeos-crossref-citedby-driver-0.1.0/pyproject.toml` & `hirmeos-crossref-citedby-driver-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hirmeos-crossref-citedby-driver"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
+  { name="Cristian Garcia", email="cristian.garcia@ubiquitypress.com" },
   { name="Rowan Hatherley", email="rowan.hatherley@ubiquitypress.com" },
 ]
 description = "Functions required by the crossref-citedby-driver"
 readme = "README.rst"
 requires-python = ">=3.10"
 dependencies = [
   'beautifulsoup4>=4.8.0,<5.0',
```

### Comparing `hirmeos-crossref-citedby-driver-0.1.0/src/crossref_citedby_driver/__init__.py` & `hirmeos-crossref-citedby-driver-0.1.1/src/crossref_citedby_driver/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             str: Publication timestamp in "YYYY-MM-DD HH:MM:SS" format.
         """
         keys = ['published', 'published-print', 'published-online', 'created']
         for key in keys:
             if key in message and len(message[key]['date-parts'][0]) == 3:
                 year, month, day = message[key]['date-parts'][0]
                 month, day = str(month).zfill(2), str(day).zfill(2)
-                return f'{year}{month}{day} 00:00:00'
+                return f'{year}-{month}-{day} 00:00:00'
 
         raise ValueError('No valid publish date found')
 
     def get_citation_data(
             self,
             citation_entry: bs4.element.Tag,
     ) -> Citation(str, str):
@@ -191,7 +191,22 @@
         Returns:
             Citation: containing cited-by DOI and timestamp.
         """
         cited_by_doi = citation_entry.find('doi').text
         timestamp = self.get_doi_date_value(cited_by_doi)
 
         return Citation(cited_by=cited_by_doi, timestamp=timestamp)
+
+
+_TEMP_CLIENT = CrossrefCitedByClient(tech_email='support@crossref.org')
+
+
+def fetch_citation_xml(*args, **kwargs):
+    return _TEMP_CLIENT.fetch_citation_xml(*args, **kwargs)
+
+
+def get_crossref_citations(*args, **kwargs):
+    return _TEMP_CLIENT.get_citation_data(*args, **kwargs)
+
+
+def get_citation_data(*args, **kwargs):
+    return _TEMP_CLIENT.get_citation_data(*args, **kwargs)
```

### Comparing `hirmeos-crossref-citedby-driver-0.1.0/src/hirmeos_crossref_citedby_driver.egg-info/PKG-INFO` & `hirmeos-crossref-citedby-driver-0.1.1/src/hirmeos_crossref_citedby_driver.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hirmeos-crossref-citedby-driver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions required by the crossref-citedby-driver
-Author-email: Rowan Hatherley <rowan.hatherley@ubiquitypress.com>
+Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>, Rowan Hatherley <rowan.hatherley@ubiquitypress.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -18,14 +18,26 @@
 
 Allows users to fecth citations from the crossref cited-by API.
 
 
 Release Notes:
 ==============
 
+[0.1.1] - 2023-07-28
+--------------------
+
+Added:
+    - Attempt to fix breaking changes: Temporarily added fetch_citation_xml,
+      get_crossref_citations and get_citation_data functions
+
+Changed:
+    - **Bugfix** | Timestamp format now uses "YYYY-MM-DD", not "YYYYMMDD"
+
+
+def get_citation_data
 
 [0.1.0] - 2023-07-28
 --------------------
 
 Changed:
     - Functions are now run as methods, via the CrossrefCitedByClient class
```

### Comparing `hirmeos-crossref-citedby-driver-0.1.0/tests/tests.py` & `hirmeos-crossref-citedby-driver-0.1.1/tests/tests.py`

 * *Files identical despite different names*

