# Comparing `tmp/chartart-0.0.3.dev20.tar.gz` & `tmp/chartart-0.0.3.dev21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev20.tar", last modified: Wed Jul 26 15:07:07 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev21.tar", last modified: Fri Jul 28 13:06:56 2023, max compression
```

## Comparing `chartart-0.0.3.dev20.tar` & `chartart-0.0.3.dev21.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-26 15:07:07.816886 chartart-0.0.3.dev20/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2733 2023-07-26 15:07:07.817155 chartart-0.0.3.dev20/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     2211 2023-07-26 15:06:28.000000 chartart-0.0.3.dev20/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-07-26 15:07:07.818193 chartart-0.0.3.dev20/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-26 15:07:07.794099 chartart-0.0.3.dev20/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-26 15:07:07.806076 chartart-0.0.3.dev20/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    87285 2023-07-26 15:00:37.000000 chartart-0.0.3.dev20/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-26 15:07:07.814650 chartart-0.0.3.dev20/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-26 15:07:07.812887 chartart-0.0.3.dev20/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2733 2023-07-26 15:07:07.000000 chartart-0.0.3.dev20/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-07-26 15:07:07.000000 chartart-0.0.3.dev20/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-07-26 15:07:07.000000 chartart-0.0.3.dev20/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-07-26 15:07:07.000000 chartart-0.0.3.dev20/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-07-26 15:07:07.000000 chartart-0.0.3.dev20/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-26 15:07:07.815680 chartart-0.0.3.dev20/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev20/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.704010 chartart-0.0.3.dev21/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2788 2023-07-28 13:06:56.704252 chartart-0.0.3.dev21/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2266 2023-07-28 13:05:48.000000 chartart-0.0.3.dev21/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-07-28 13:06:56.705463 chartart-0.0.3.dev21/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.682018 chartart-0.0.3.dev21/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.693149 chartart-0.0.3.dev21/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    87504 2023-07-28 13:01:20.000000 chartart-0.0.3.dev21/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.702185 chartart-0.0.3.dev21/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.699994 chartart-0.0.3.dev21/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2788 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.703091 chartart-0.0.3.dev21/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev20/LICENSE` & `chartart-0.0.3.dev21/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev20/PKG-INFO` & `chartart-0.0.3.dev21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev20
+Version: 0.0.3.dev21
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -80,7 +80,10 @@
 
 0.0.3.dev19
 - added support to specify axis type 
 - Made default bin interval is 0 . 0 means syncfusion will calculate internally.
 
 0.0.3.dev20
 - preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
+
+- 0.0.3.dev21
+Fix for communicate with Jupyter kernel
```

### Comparing `chartart-0.0.3.dev20/README.md` & `chartart-0.0.3.dev21/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,8 +63,11 @@
 - Added number format on axis
 
 0.0.3.dev19
 - added support to specify axis type 
 - Made default bin interval is 0 . 0 means syncfusion will calculate internally.
 
 0.0.3.dev20
-- preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
+- preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
+
+- 0.0.3.dev21
+Fix for communicate with Jupyter kernel
```

### Comparing `chartart-0.0.3.dev20/setup.cfg` & `chartart-0.0.3.dev21/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev20
+version = 0.0.3.dev21
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev20/src/chartart/__init__.py` & `chartart-0.0.3.dev21/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev20/src/chartart/conftest.py` & `chartart-0.0.3.dev21/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev20/src/chartart/helpers.py` & `chartart-0.0.3.dev21/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev20/src/chartart/plot.py` & `chartart-0.0.3.dev21/src/chartart/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1872,42 +1872,46 @@
     
     if features is not None:
         myData['features'] = features
     
     
     my_comm = ''
     try:
+        my_comm = Comm(target_name='my_comm_target', data={'url': ''})
         response = doPost(
             apiGatewayBaseUrl + '/previewPost', data=myData, headers={'authorization': 'Bearer ' + idToken})
    
         respJson = {}
         try:
             respJson = response.json()
             print(respJson)
 
             if 'code' in respJson and respJson['code'] == 401:
                 return 'Error: ' + respJson['message']
         
         except Exception as e:
             print(response)
-            return {'error' : 'Internal Error'}
+            return {'Error' : 'Internal Error'}
 
         url = webAppBaseUrl + '/#/previewPost?uid=' + str(
             respJson['userId']) + '&notebookName=' + id + '&idToken=' + idToken
+        my_comm.send(url)
 
         # self.db.collection(u'preview').document(str(uuid.uuid1())) #.collection('charts')
         # .document(str(uuid.uuid1())).set(data)
         #return IFrame(url, width=900, height=500)
         # Script mode
         return webAppBaseUrl + '/#/previewPost?uid=' + str(
             respJson['userId']) + '&notebookName=' + id + '&idToken=<Token>'
         # return self.data.to_json()
     except Exception as e:
-        print(e)
-        raise
+        my_comm = Comm(target_name='my_comm_target', data={'url': ''})
+        my_comm.send("Error in connection")
+
+        return "Error in connection"
 
 class Post:
     def __init__(self, postId: str, postTitle: str = None):
         self.postId = postId
         self.postTitle = postTitle
         self.chartIds: list = []
         self.addedPostTitleInfo = False
```

### Comparing `chartart-0.0.3.dev20/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev21/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev20/src/chartart/test_plot.py` & `chartart-0.0.3.dev21/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev20/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev21/src/chartart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev20
+Version: 0.0.3.dev21
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -80,7 +80,10 @@
 
 0.0.3.dev19
 - added support to specify axis type 
 - Made default bin interval is 0 . 0 means syncfusion will calculate internally.
 
 0.0.3.dev20
 - preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
+
+- 0.0.3.dev21
+Fix for communicate with Jupyter kernel
```

