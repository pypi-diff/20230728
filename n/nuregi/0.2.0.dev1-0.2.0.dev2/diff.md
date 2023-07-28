# Comparing `tmp/nuregi-0.2.0.dev1.tar.gz` & `tmp/nuregi-0.2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuregi-0.2.0.dev1.tar", last modified: Sat Jul 30 19:56:50 2022, max compression
+gzip compressed data, was "nuregi-0.2.0.dev2.tar", last modified: Fri Jul 28 12:05:34 2023, max compression
```

## Comparing `nuregi-0.2.0.dev1.tar` & `nuregi-0.2.0.dev2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.982163 nuregi-0.2.0.dev1/
--rw-rw-rw-   0        0        0    35821 2022-04-26 10:28:24.000000 nuregi-0.2.0.dev1/LICENSE.txt
--rw-rw-rw-   0        0        0     3421 2022-07-30 19:56:50.982163 nuregi-0.2.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     2398 2022-07-30 19:48:10.000000 nuregi-0.2.0.dev1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.962162 nuregi-0.2.0.dev1/nuregi/
--rw-rw-rw-   0        0        0       68 2022-07-30 19:17:10.000000 nuregi-0.2.0.dev1/nuregi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.977162 nuregi-0.2.0.dev1/nuregi/api/
--rw-rw-rw-   0        0        0      184 2022-07-30 18:37:42.000000 nuregi-0.2.0.dev1/nuregi/api/__init__.py
--rw-rw-rw-   0        0        0     6195 2022-07-30 19:14:16.000000 nuregi-0.2.0.dev1/nuregi/api/api.py
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.979163 nuregi-0.2.0.dev1/nuregi/exceptions/
--rw-rw-rw-   0        0        0       27 2022-07-30 19:04:08.000000 nuregi-0.2.0.dev1/nuregi/exceptions/__init__.py
--rw-rw-rw-   0        0        0      359 2022-07-30 17:20:18.000000 nuregi-0.2.0.dev1/nuregi/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.979163 nuregi-0.2.0.dev1/nuregi/scraper/
--rw-rw-rw-   0        0        0        0 2022-07-30 11:33:15.000000 nuregi-0.2.0.dev1/nuregi/scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.981163 nuregi-0.2.0.dev1/nuregi/scraper/pdf/
--rw-rw-rw-   0        0        0       69 2022-07-30 13:47:47.000000 nuregi-0.2.0.dev1/nuregi/scraper/pdf/__init__.py
--rw-rw-rw-   0        0        0     4227 2022-07-30 19:42:38.000000 nuregi-0.2.0.dev1/nuregi/scraper/pdf/pdf.py
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.981163 nuregi-0.2.0.dev1/nuregi/scraper/web/
--rw-rw-rw-   0        0        0        0 2022-07-30 11:33:22.000000 nuregi-0.2.0.dev1/nuregi/scraper/web/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-30 19:56:50.976161 nuregi-0.2.0.dev1/nuregi.egg-info/
--rw-rw-rw-   0        0        0     3421 2022-07-30 19:56:50.000000 nuregi-0.2.0.dev1/nuregi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2022-07-30 19:56:50.000000 nuregi-0.2.0.dev1/nuregi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-30 19:56:50.000000 nuregi-0.2.0.dev1/nuregi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-07-30 19:56:50.000000 nuregi-0.2.0.dev1/nuregi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-30 19:56:50.000000 nuregi-0.2.0.dev1/nuregi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2022-07-30 17:08:05.000000 nuregi-0.2.0.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       85 2022-07-30 19:56:50.986163 nuregi-0.2.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0     1497 2022-07-30 11:15:58.000000 nuregi-0.2.0.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.393742 nuregi-0.2.0.dev2/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3421 2023-07-28 12:05:34.393742 nuregi-0.2.0.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     2398 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.372210 nuregi-0.2.0.dev2/nuregi/
+-rw-rw-rw-   0        0        0       68 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.388235 nuregi-0.2.0.dev2/nuregi/api/
+-rw-rw-rw-   0        0        0      184 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/api/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-07-28 11:55:55.000000 nuregi-0.2.0.dev2/nuregi/api/api.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.390235 nuregi-0.2.0.dev2/nuregi/exceptions/
+-rw-rw-rw-   0        0        0       27 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      359 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.391236 nuregi-0.2.0.dev2/nuregi/scraper/
+-rw-rw-rw-   0        0        0        0 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.392737 nuregi-0.2.0.dev2/nuregi/scraper/pdf/
+-rw-rw-rw-   0        0        0       69 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/scraper/pdf/__init__.py
+-rw-rw-rw-   0        0        0     4483 2023-07-28 11:59:45.000000 nuregi-0.2.0.dev2/nuregi/scraper/pdf/pdf.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.392737 nuregi-0.2.0.dev2/nuregi/scraper/web/
+-rw-rw-rw-   0        0        0        0 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/scraper/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.387230 nuregi-0.2.0.dev2/nuregi.egg-info/
+-rw-rw-rw-   0        0        0     3421 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-28 12:05:34.396742 nuregi-0.2.0.dev2/setup.cfg
+-rw-rw-rw-   0        0        0     1497 2023-07-28 12:02:20.000000 nuregi-0.2.0.dev2/setup.py
```

### Comparing `nuregi-0.2.0.dev1/LICENSE.txt` & `nuregi-0.2.0.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuregi-0.2.0.dev1/PKG-INFO` & `nuregi-0.2.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuregi
-Version: 0.2.0.dev1
+Version: 0.2.0.dev2
 Summary: A basic Python-based API client library for registrar.nu.edu.kz
 Home-page: https://github.com/aldan/nuregi
 Author: aldan
 Author-email: gitaldan@gmail.com
 Project-URL: Source, https://github.com/aldan/nuregi
 Project-URL: Tracker, https://github.com/aldan/nuregi/issues
 Keywords: api library registrar.nu.edu.kz scraper
```

### Comparing `nuregi-0.2.0.dev1/README.md` & `nuregi-0.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `nuregi-0.2.0.dev1/nuregi/api/api.py` & `nuregi-0.2.0.dev2/nuregi/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Tools to interact with Registrar Public Course Catalog API
 """
 
 import logging
 from enum import Enum
 
 import requests
+from requests.exceptions import SSLError
 
 from nuregi.exceptions import APIError, ValidationError
 
 BASE_URL = "https://registrar.nu.edu.kz/my-registrar/public-course-catalog/json"
 
 
 class RegistrarObject(Enum):
@@ -27,15 +28,20 @@
     Get course data from public course catalog
     :param request_data: request form data
     :param sort_by: key to sort by if specified
     :param timeout: time to wait for Registrar to respond
     :return: course data in JSON format
     """
 
-    response = requests.post(BASE_URL, data=request_data, timeout=timeout)
+    try:
+        response = requests.post(BASE_URL, data=request_data, timeout=timeout)
+    except SSLError:
+        # nu.edu.kz isnt providing full certificate chain so requests raises SSLError
+        response = requests.post(BASE_URL, data=request_data, timeout=timeout, verify=False)
+
     logging.info(response.url, response.status_code)
     response.raise_for_status()
 
     response_data = response.json()
 
     if isinstance(response_data, dict) and response_data.get("status") == "error":
         logging.error(response_data)
```

### Comparing `nuregi-0.2.0.dev1/nuregi/scraper/pdf/pdf.py` & `nuregi-0.2.0.dev2/nuregi/scraper/pdf/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import logging
 from enum import Enum
 from io import BytesIO
 
 import pandas as pd
 import requests
+from requests.exceptions import SSLError
 from tabula import read_pdf
 
 from nuregi.exceptions import ValidationError
 
 BASE_URL = "https://registrar.nu.edu.kz/registrar_downloads/json"
 
 
@@ -41,15 +42,20 @@
 
     if data_format not in ("table", "columns"):
         raise ValidationError("data_format must be equal to either 'table' or 'column'.")
 
     if extra_params is not None and not isinstance(extra_params, dict):
         raise ValidationError("extra_params must be a dict")
 
-    response = requests.get(BASE_URL, params=params, timeout=timeout)
+    try:
+        response = requests.get(BASE_URL, params=params, timeout=timeout)
+    except SSLError:
+        # nu.edu.kz isnt providing full certificate chain so requests raises SSLError
+        response = requests.get(BASE_URL, params=params, timeout=timeout, verify=False)
+
     logging.info(response.url, response.status_code)
     response.raise_for_status()
     content = BytesIO(response.content)
 
     try:
         # try to read binary file with utf-8 encoding
         dataframe = read_pdf(content, pages='all', lattice=True, pandas_options={'header': None})
```

### Comparing `nuregi-0.2.0.dev1/nuregi.egg-info/PKG-INFO` & `nuregi-0.2.0.dev2/nuregi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuregi
-Version: 0.2.0.dev1
+Version: 0.2.0.dev2
 Summary: A basic Python-based API client library for registrar.nu.edu.kz
 Home-page: https://github.com/aldan/nuregi
 Author: aldan
 Author-email: gitaldan@gmail.com
 Project-URL: Source, https://github.com/aldan/nuregi
 Project-URL: Tracker, https://github.com/aldan/nuregi/issues
 Keywords: api library registrar.nu.edu.kz scraper
```

### Comparing `nuregi-0.2.0.dev1/setup.py` & `nuregi-0.2.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 base_dir = pathlib.Path(__file__).parent.resolve()
 long_description = (base_dir / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='nuregi',
-    version='0.2.0.dev1',
+    version='0.2.0.dev2',
     description='A basic Python-based API client library for registrar.nu.edu.kz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aldan/nuregi',
     author='aldan',
     author_email='gitaldan@gmail.com',
 
@@ -33,15 +33,15 @@
         'Source': 'https://github.com/aldan/nuregi',
         'Tracker': 'https://github.com/aldan/nuregi/issues',
     },
 
     packages=find_packages(),
 
     install_requires=[
-        'requests==2.28.1',
-        'numpy==1.23.1',
-        'pandas==1.4.3',
-        'tabula-py==2.4.0',
+        'requests==2.31.0',
+        'numpy==1.25.1',
+        'pandas==2.0.3',
+        'tabula-py==2.7.0',
     ],
 
     python_requires='>=3.8',
 )
```

