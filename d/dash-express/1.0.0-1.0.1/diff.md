# Comparing `tmp/dash_express-1.0.0.tar.gz` & `tmp/dash_express-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express-1.0.0.tar", last modified: Fri Jul 28 10:17:11 2023, max compression
+gzip compressed data, was "dash_express-1.0.1.tar", last modified: Fri Jul 28 16:21:52 2023, max compression
```

## Comparing `dash_express-1.0.0.tar` & `dash_express-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 10:17:11.361693 dash_express-1.0.0/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1071 2023-07-26 08:37:30.000000 dash_express-1.0.0/LICENSE
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     5980 2023-07-28 10:17:11.361693 dash_express-1.0.0/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     5497 2023-07-28 09:55:52.000000 dash_express-1.0.0/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 10:17:11.353693 dash_express-1.0.0/dash_express/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)    33830 2023-07-28 08:52:09.000000 dash_express-1.0.0/dash_express/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)    16493 2023-07-28 08:52:30.000000 dash_express-1.0.0/dash_express/_app_shell.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 10:17:11.357693 dash_express-1.0.0/dash_express/filters/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       88 2023-07-26 08:21:26.000000 dash_express-1.0.0/dash_express/filters/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     3374 2023-07-26 08:21:26.000000 dash_express-1.0.0/dash_express/filters/autofilter.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      612 2023-07-26 08:21:26.000000 dash_express-1.0.0/dash_express/filters/filterfunc.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 10:17:11.361693 dash_express-1.0.0/dash_express/kpi/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1761 2023-07-26 17:26:07.000000 dash_express-1.0.0/dash_express/kpi/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     2360 2023-07-26 08:27:32.000000 dash_express-1.0.0/dash_express/preview_chart.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        7 2023-07-28 02:54:43.000000 dash_express-1.0.0/dash_express/version.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 10:17:11.357693 dash_express-1.0.0/dash_express.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     5980 2023-07-28 10:17:11.000000 dash_express-1.0.0/dash_express.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      443 2023-07-28 10:17:11.000000 dash_express-1.0.0/dash_express.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-07-28 10:17:11.000000 dash_express-1.0.0/dash_express.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      135 2023-07-28 10:17:11.000000 dash_express-1.0.0/dash_express.egg-info/requires.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       13 2023-07-28 10:17:11.000000 dash_express-1.0.0/dash_express.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-07-28 10:17:11.361693 dash_express-1.0.0/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1366 2023-07-28 10:17:01.000000 dash_express-1.0.0/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.943342 dash_express-1.0.1/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1071 2023-07-26 08:37:30.000000 dash_express-1.0.1/LICENSE
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-28 16:21:52.943342 dash_express-1.0.1/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     5606 2023-07-28 14:45:31.000000 dash_express-1.0.1/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.939342 dash_express-1.0.1/dash_express/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)    33840 2023-07-28 14:08:58.000000 dash_express-1.0.1/dash_express/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)    16493 2023-07-28 08:52:30.000000 dash_express-1.0.1/dash_express/_app_shell.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.943342 dash_express-1.0.1/dash_express/filters/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       88 2023-07-26 08:21:26.000000 dash_express-1.0.1/dash_express/filters/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     3374 2023-07-26 08:21:26.000000 dash_express-1.0.1/dash_express/filters/autofilter.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      612 2023-07-26 08:21:26.000000 dash_express-1.0.1/dash_express/filters/filterfunc.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.943342 dash_express-1.0.1/dash_express/kpi/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1761 2023-07-26 17:26:07.000000 dash_express-1.0.1/dash_express/kpi/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     2360 2023-07-26 08:27:32.000000 dash_express-1.0.1/dash_express/preview_chart.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        7 2023-07-28 02:54:43.000000 dash_express-1.0.1/dash_express/version.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.939342 dash_express-1.0.1/dash_express.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      443 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      135 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/requires.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       13 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-07-28 16:21:52.943342 dash_express-1.0.1/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1366 2023-07-28 16:21:13.000000 dash_express-1.0.1/setup.py
```

### Comparing `dash_express-1.0.0/LICENSE` & `dash_express-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.0/PKG-INFO` & `dash_express-1.0.1/dash_express.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
-Name: dash_express
-Version: 1.0.0
+Name: dash-express
+Version: 1.0.1
 Summary: A tool for faster application development Plotly Dash
 Home-page: https://github.com/stpnvkirill/dash-express
 Author: Kirill Stepanov
 Author-email: stpnv.kirill.o@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast analytical web application with DashExpress
 
+[Documentation](https://stpnvkirill.github.io/dash-express/)
+
 Build your next dashboard even faster with premade responsive UI and automatic callback-function. DashExpress is a wrapper over the Plotly Dash web framework, which allows you to simplify and speed up the creation of multi-page analytical applications based on data from pd.DataFrame.
 
+```console
+pip install dash-express
+```
+
 Currently supported: Charts, KPI, Geographical Maps
 
 The key features are:
 
 * **High Performance**: Provided by built-in optimization methods of Dash callback functions.
 * **Fast to code**: Using a pre-configured UI and automatically generated callback functions.
 * **Based on Pandas**: A library familiar to all analysts.
@@ -32,15 +38,15 @@
 
 ![Image title](https://raw.githubusercontent.com/stpnvkirill/dash-express/main/docs/assets/gifs/min_app.gif)
 
 The first step is to import the necessary libraries
 
 ```python
 import pandas as pd
-import plotly.express as px
+import plotly.graph_objects as go
 import dash_mantine_components as dmc
 
 from dash_express import DashExpress, Page
 ```
 
 Next, you need to initialize an instance of the Dash Express application.
```

### Comparing `dash_express-1.0.0/README.md` & `dash_express-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Fast analytical web application with DashExpress
 
+[Documentation](https://stpnvkirill.github.io/dash-express/)
+
 Build your next dashboard even faster with premade responsive UI and automatic callback-function. DashExpress is a wrapper over the Plotly Dash web framework, which allows you to simplify and speed up the creation of multi-page analytical applications based on data from pd.DataFrame.
 
+```console
+pip install dash-express
+```
+
 Currently supported: Charts, KPI, Geographical Maps
 
 The key features are:
 
 * **High Performance**: Provided by built-in optimization methods of Dash callback functions.
 * **Fast to code**: Using a pre-configured UI and automatically generated callback functions.
 * **Based on Pandas**: A library familiar to all analysts.
@@ -17,15 +23,15 @@
 
 ![Image title](https://raw.githubusercontent.com/stpnvkirill/dash-express/main/docs/assets/gifs/min_app.gif)
 
 The first step is to import the necessary libraries
 
 ```python
 import pandas as pd
-import plotly.express as px
+import plotly.graph_objects as go
 import dash_mantine_components as dmc
 
 from dash_express import DashExpress, Page
 ```
 
 Next, you need to initialize an instance of the Dash Express application.
```

### Comparing `dash_express-1.0.0/dash_express/__init__.py` & `dash_express-1.0.1/dash_express/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,15 @@
         geojson_func = geojson_func or self.geojson_wrapper
         self.GEOJSON_FUNC[id] = geojson_func
         self.GEOJSON_FUNC['default'] = self.geojson_wrapper
         return dmc.LoadingOverlay(dmc.Card(
             [
                 html.Div(
                     dl.Map(
-                        [dl.TileLayer(url=self.app.LIGHT_LEAFLET_TILE, id=dict(type='map-layer', id=id)),
+                        [dl.TileLayer(url=self.app.app_shell.LIGHT_LEAFLET_TILE, id=dict(type='map-layer', id=id)),
                          dl.GeoJSON(id={'type': "geojson", 'id': id}, **dl_geojson_kwargs),],
                         markerZoomAnimation=True,
                         style={'height': '100%', 'width': '100%',
                                'z-index': '2'},
                         id='map-container',
                         bounds=[[55.072, 82.907], [54.92, 82.97]],
                         attributionControl=False
```

### Comparing `dash_express-1.0.0/dash_express/_app_shell.py` & `dash_express-1.0.1/dash_express/_app_shell.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.0/dash_express/filters/autofilter.py` & `dash_express-1.0.1/dash_express/filters/autofilter.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.0/dash_express/filters/filterfunc.py` & `dash_express-1.0.1/dash_express/filters/filterfunc.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.0/dash_express/kpi/__init__.py` & `dash_express-1.0.1/dash_express/kpi/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.0/dash_express/preview_chart.py` & `dash_express-1.0.1/dash_express/preview_chart.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.0/dash_express.egg-info/PKG-INFO` & `dash_express-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
-Name: dash-express
-Version: 1.0.0
+Name: dash_express
+Version: 1.0.1
 Summary: A tool for faster application development Plotly Dash
 Home-page: https://github.com/stpnvkirill/dash-express
 Author: Kirill Stepanov
 Author-email: stpnv.kirill.o@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast analytical web application with DashExpress
 
+[Documentation](https://stpnvkirill.github.io/dash-express/)
+
 Build your next dashboard even faster with premade responsive UI and automatic callback-function. DashExpress is a wrapper over the Plotly Dash web framework, which allows you to simplify and speed up the creation of multi-page analytical applications based on data from pd.DataFrame.
 
+```console
+pip install dash-express
+```
+
 Currently supported: Charts, KPI, Geographical Maps
 
 The key features are:
 
 * **High Performance**: Provided by built-in optimization methods of Dash callback functions.
 * **Fast to code**: Using a pre-configured UI and automatically generated callback functions.
 * **Based on Pandas**: A library familiar to all analysts.
@@ -32,15 +38,15 @@
 
 ![Image title](https://raw.githubusercontent.com/stpnvkirill/dash-express/main/docs/assets/gifs/min_app.gif)
 
 The first step is to import the necessary libraries
 
 ```python
 import pandas as pd
-import plotly.express as px
+import plotly.graph_objects as go
 import dash_mantine_components as dmc
 
 from dash_express import DashExpress, Page
 ```
 
 Next, you need to initialize an instance of the Dash Express application.
```

### Comparing `dash_express-1.0.0/setup.py` & `dash_express-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dash_express",
-    version="1.0.0",                        # Обновляйте это для каждой новой версии
+    version="1.0.1",                        # Обновляйте это для каждой новой версии
     author="Kirill Stepanov",
     author_email="stpnv.kirill.o@gmail.com",
     description="A tool for faster application development Plotly Dash",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[                      
         "dash>=2.11.1",
```

