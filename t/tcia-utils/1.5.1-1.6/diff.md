# Comparing `tmp/tcia_utils-1.5.1.tar.gz` & `tmp/tcia_utils-1.6.tar.gz`

## Comparing `tcia_utils-1.5.1.tar` & `tcia_utils-1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    67874 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/LICENSE
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    71818 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6/LICENSE
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.6/README.md
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tcia_utils-1.6/pyproject.toml
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 tcia_utils-1.6/PKG-INFO
```

### Comparing `tcia_utils-1.5.1/src/tcia_utils/datacite.py` & `tcia_utils-1.6/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5.1/src/tcia_utils/nbia.py` & `tcia_utils-1.6/src/tcia_utils/nbia.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,36 @@
 import json
 import zipfile
 import io
 import os
 from datetime import datetime
 from datetime import timedelta
 from enum import Enum
+import matplotlib
 import matplotlib.pyplot as plt
+import matplotlib.colors as mcolors
 import pydicom
 import numpy as np
 from ipywidgets import interact
+import tkinter, pydicom_seg, rt_utils 
+from tkinter import filedialog
 
 class StopExecution(Exception):
     def _render_traceback_(self):
         pass
 
 _log = logging.getLogger(__name__)
 logging.basicConfig(
     format='%(asctime)s:%(levelname)s:%(message)s'
     , level=logging.INFO
 )
 
+# set token creation URL for getToken, refreshToken and logoutToken
+token_url = "https://keycloak.dbmi.cloud/auth/realms/TCIA/protocol/openid-connect/token"
+
 # Used by functions that accept parameters used in GUI Simple Search
 # e.g. getSimpleSearchWithModalityAndBodyPartPaged()
 class Criteria(Enum):
     Collection = "CollectionCriteria"
     Species = "SpeciesCriteria"
     ImageModality = "ImageModalityCriteria"
     BodyPart = "AnatomicalSiteCriteria"
@@ -100,18 +107,18 @@
         elif api_url == "nlst":
             if endpoint in searchEndpoints:
                 # Using "Search" API with NLST server (no login required): https://wiki.cancerimagingarchive.net/x/fILTB
                 base_url = "https://nlst.cancerimagingarchive.net/nbia-api/services/v1/"
             if endpoint in advancedEndpoints:
                 # Using "Advanced" API docs (login required): https://wiki.cancerimagingarchive.net/x/YoATBg
                 # Checking to see if a valid NLST authentication token exists
-                if 'nlst_token_exp_time' not in globals():
-                    getToken(user = "nbia_guest", api_url = "nlst")
-                if 'nlst_token_exp_time' in globals() and datetime.now() > nlst_token_exp_time:
-                    refreshToken(api_url = "nlst")
+                if 'token_exp_time' not in globals():
+                    getToken(user = "nbia_guest")
+                if 'token_exp_time' in globals() and datetime.now() > token_exp_time:
+                    refreshToken()
                 base_url = "https://nlst.cancerimagingarchive.net/nbia-api/services/"                
         elif api_url == "restricted":
             if endpoint in searchEndpoints:
                 # Using "Search with Authentication" API (login required): https://wiki.cancerimagingarchive.net/x/X4ATBg
                 # Checking to see if a valid authentication token exists
                 if 'token_exp_time' not in globals():
                     _log.error("Error using token for accessing the Restricted API. Create one using getToken().")
@@ -142,181 +149,115 @@
                     "Remove the api_url parameter unless you are querying the National Lung Screening Trial collection.\n"
                     'Use api_url = "nlst" to query the National Lung Screening Trial collection.'
                 )
                 raise StopExecution
 
         return base_url
 
-def getToken(user = "", pw = "", api_url = ""): 
+def getToken(user = "", pw = ""): 
     """
     getToken() accepts user and pw parameters to create a token to access APIs that require authorization.
-    Access tokens expire 2 hours after creation, and can be refreshed with refreshToken().
+    Access tokens can be refreshed with refreshToken().
+    Set user = "nbia_guest" for anonymous access to Advanced API functions
     Interactive prompts are provided for user/pw if they're not specified as parameters.
-    "Advanced APIs" can be accessed anonymously using the nbia_guest account with a blank password.
-    The api_url = "nlst" parameter is only necessary for "Advanced API" queries since it's a public collection.
+    "Advanced APIs" can be accessed anonymously using the nbia_guest account with the default guest password.
     """
-    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token, nlst_refresh_token
+    global token_exp_time, api_call_headers, refresh_token, id_token
 
-    # assumes nbia_guest account for Advanced API on NLST server (all public data)
-    if api_url == "nlst":
-        token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token"
-        userName = "nbia_guest"
-        passWord = ""        
     # specify user/pw unless nbia_guest is being used for accessing Advanced API anonymously
-    else:
-        token_url = "https://nbia.cancerimagingarchive.net/nbia-api/oauth/token"
 
-        if user == "":
-            print("Enter User: ")
-            userName = input()
-        else:
-            userName = user
-        # if user is nbia_guest, we leave password blank for anonymous access
-        if pw == "" and user != "nbia_guest":
-            passWord = getpass.getpass(prompt = 'Enter Password: ')
-        else:
-            passWord = pw
+    if user != "":
+        userName = user
+    else:
+        print("Enter User: ")
+        userName = input()
+    # set password for non-guest logins
+    if userName == "nbia_guest":
+        passWord = "ItsBetweenUAndMe" # this guest account password is documented in the public API guide
+    elif pw == "":
+        passWord = getpass.getpass(prompt = 'Enter Password: ')
+    else:
+        passWord = pw
 
     # request API token
     try:
         params = {
-        'client_id': 'nbiaRestAPIClient',
-        'client_secret' : 'ItsBetweenUAndMe',
+        'client_id': 'nbia',
+        'scope': 'openid',
         'grant_type': 'password',
         'username' : userName,
         'password': passWord
         }
         
         data = requests.post(token_url, data = params)
         data.raise_for_status()
         access_token = data.json()["access_token"]
         expires_in = data.json()["expires_in"]
+        id_token = data.json()["id_token"]
         # track expiration status/time
         current_time = datetime.now()
-        if api_url == "nlst":
-            nlst_token_exp_time = current_time + timedelta(seconds=expires_in)
-            nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
-            nlst_refresh_token = data.json()["refresh_token"]
-            _log.info(f'Success - Token saved to nlst_api_call_headers variable and expires at {nlst_token_exp_time}')
-        else:
-            token_exp_time = current_time + timedelta(seconds=expires_in)            
-            api_call_headers = {'Authorization': 'Bearer ' + access_token}
-            refresh_token = data.json()["refresh_token"]
-            _log.info(f'Success - Token saved to api_call_headers variable and expires at {token_exp_time}')
+        token_exp_time = current_time + timedelta(seconds=expires_in)            
+        api_call_headers = {'Authorization': 'Bearer ' + access_token}
+        refresh_token = data.json()["refresh_token"]
+        _log.info(f'Success - Token saved to api_call_headers variable and expires at {token_exp_time}')
+
     # handle errors
     except requests.exceptions.HTTPError as errh:
         _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
     except requests.exceptions.ConnectionError as errc:
         _log.error(f"Connection Error: {data.status_code}")
     except requests.exceptions.Timeout as errt:
         _log.error(f"Timeout Error: {data.status_code}")
     except requests.exceptions.RequestException as err:
         _log.error(f"Request Error: {data.status_code}")
 
-def refreshToken(api_url = ""):
+def refreshToken():
     """
     refreshToken() refreshes security tokens to extend access time for APIs that require authorization.
     It attempts to verify that a refresh token exists and recommends using getToken() to create a new token if needed.
     This function is called as needed by setApiUrl() and is generally not something that needs to be called directly in your code.    
     """
-    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers
+    global token_exp_time, api_call_headers
    
-    # token URLs
-    if api_url == "nlst":
-        try:
-            token = nlst_refresh_token
-        except NameError:
-            _log.warning(f"No NLST refresh token found. Creating a new token...")
-            getToken(api_url = "nlst")
-            raise StopExecution
-        else:
-            token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token"
-    
-    else:
-        try:
-            token = refresh_token
-        except NameError:
-            _log.error("Error refreshing token for accessing the Restricted API. Create one using getToken().")
-            raise StopExecution
-        else:
-            token_url = "https://nbia.cancerimagingarchive.net/nbia-api/oauth/token"
+    try:
+        token = refresh_token
+    except NameError:
+        _log.error("No token found. Create one using getToken().")
+        raise StopExecution
 
     # refresh token request
     try:
         params = {
-        'client_id': 'nbiaRestAPIClient',
-        'client_secret' : 'ItsBetweenUAndMe',
+        'client_id': 'nbia',
         'grant_type': 'refresh_token',
-        'refresh_token' : token,
+        'refresh_token' : token
         }
         
         # obtain new access token
         data = requests.post(token_url, data = params)
         data.raise_for_status()
         access_token = data.json()["access_token"]
         expires_in = data.json()["expires_in"]
-        # track expiration status/time (2 hours from creation)
-        current_time = datetime.now()
-        if api_url == "nlst":
-            nlst_token_exp_time = current_time + timedelta(seconds=expires_in)
-            nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
-            _log.info(f'Success - Token refreshed to nlst_api_call_headers variable and expires at {nlst_token_exp_time}')
-        else:
-            token_exp_time = current_time + timedelta(seconds=expires_in)
-            api_call_headers = {'Authorization': 'Bearer ' + access_token}
-            _log.info(f'Success - Token refreshed to api_call_headers variable and expires at {token_exp_time}')
-    # handle errors
-    except requests.exceptions.HTTPError as errh:
-        _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
-    except requests.exceptions.ConnectionError as errc:
-        _log.error(f"Connection Error: {data.status_code}")
-    except requests.exceptions.Timeout as errt:
-        _log.error(f"Timeout Error: {data.status_code}")
-    except requests.exceptions.RequestException as err:
-        _log.error(f"Request Error: {data.status_code}")
-            
-def logoutToken(api_url = ""): 
-    """
-    logoutToken() logs out security tokens used for APIs that require authorization.
-    Variables holding access token information are also deleted by this operation.
-    The api_url parameter can be used to specify whether your token was for the main server (leave empty) or NLST.
-    Use getToken() to create a new token if needed.
-    """
-    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token, nlst_refresh_token
-
-    # determine which server the token was created on
-    if api_url == "nlst" and 'nlst_api_call_headers' in globals():
-        url = "https://nlst.cancerimagingarchive.net/nbia-api/logout"
-        api_call_headers = nlst_api_call_headers
-    elif api_url != "nlst" and 'api_call_headers' in globals():
-        url = "https://services.cancerimagingarchive.net/nbia-api/logout"
-    else: 
-        _log.error("Error: You haven't created a token yet, or have already logged out.")
-        raise StopExecution
 
-    try:
-        _log.info(f'Logging out of... {url}')
-        data = requests.get(url, headers = api_call_headers)
-        _log.info(f'{data.text}')
-        # remove variables holding token details
-        if api_url == "nlst":
-            del nlst_token_exp_time, nlst_api_call_headers, nlst_refresh_token
-        else:
-            del token_exp_time, api_call_headers, refresh_token
+        # track expiration status/time 
+        current_time = datetime.now()
+        token_exp_time = current_time + timedelta(seconds=expires_in)
+        api_call_headers = {'Authorization': 'Bearer ' + access_token}
+        _log.info(f'Success - Token refreshed to api_call_headers variable and expires at {token_exp_time}')
 
     # handle errors
     except requests.exceptions.HTTPError as errh:
         _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
     except requests.exceptions.ConnectionError as errc:
         _log.error(f"Connection Error: {data.status_code}")
     except requests.exceptions.Timeout as errt:
         _log.error(f"Timeout Error: {data.status_code}")
     except requests.exceptions.RequestException as err:
         _log.error(f"Request Error: {data.status_code}")
-
+            
 def makeCredentialFile(user = "", pw = ""):
     """
     Creates a credential file to use with NBIA Data Retriever. 
     Interactive prompts are provided for user/pw if they're not specified as parameters.
     The credential file is a text file that passes the user's credentials in the following format:
         userName = YourUserName
         passWord = YourPassword
@@ -357,19 +298,20 @@
     base_url = setApiUrl(endpoint, api_url)
     # display full URL with endpoint & parameters
     url = base_url + endpoint
     _log.info(f'Calling... {url} with parameters {options}')
     # get the data
     try:
         # include api_call_headers for restricted queries
-        if api_url == "restricted" or (endpoint in advancedEndpoints and api_url == ""):
+        #if api_url == "restricted" or (endpoint in advancedEndpoints and api_url == ""):
+        if api_url == "restricted" or endpoint in advancedEndpoints:
             data = requests.get(url, params = options, headers = api_call_headers)
         # include nlst_api_call_headers for nlst-advanced
-        elif api_url == "nlst" and endpoint in advancedEndpoints:
-            data = requests.get(url, params = options, headers = nlst_api_call_headers)
+        #elif api_url == "nlst" and endpoint in advancedEndpoints:
+        #    data = requests.get(url, params = options, headers = nlst_api_call_headers)
         else:
             data = requests.get(url, params = options)
         data.raise_for_status()
 
         # check for empty results and format output
         if data.text != "":
             data = data.json()
@@ -629,68 +571,54 @@
         options['Manufacturer'] = manufacturer
     if manufacturerModel:
         options['ManufacturerModelName'] = manufacturerModel
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
-####### getUpdatedSeries function
-# Gets "new" series metadata from a specified api_url
-# Requires specifying date
-# Date format is YYYY/MM/DD
-# NOTE: NBIA API expects MM/DD/YYYY (unlike any other API endpoint!)
-#        so we'll convert from YYYY/MM/DD so tcia-utils is consistent
-
 def getUpdatedSeries(date,
                      api_url = "",
                      format = ""):
     """
     Optional: api_url, format
-    Gets "new" series metadata from a specified api_url
-    The date format is YYYY/MM/DD
-    NOTE: Unlike other API endpoints, this function expects MM/DD/YYYY, we'll convert from YYYY/MM/DD so tcia-utils is consistent
+    Gets "new" series metadata from a specified api_url.
+    The date format is YYYY/MM/DD.
+    NOTE: Unlike other API endpoints, this one expects MM/DD/YYYY, 
+      but we convert from YYYY/MM/DD so tcia-utils date inputs are consistent.
     """
     endpoint = "getUpdatedSeries"
 
     # convert to NBIA's expected date format
     nbiaDate = datetime.strptime(date, "%Y/%m/%d").strftime("%m/%d/%Y")
 
     # create options dict to construct URL
     options = {}
     options['fromDate'] = nbiaDate
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
-####### getSeriesMetadata function
-# Gets Series (scan) metadata from a specified api_url
-# Requires a specific Series Instance UID as input
-# Output includes DOI and license details that are not in getSeries()
-
 def getSeriesMetadata(seriesUid,
                       api_url = "",
                       format = ""):
     """
     Optional: api_url, format
-    Gets Series (scan) metadata from a specified api_url
-    Output includes DOI and license details that are not in the getSeries() function
+    Gets Series (scan) metadata from a specified api_url.
+    Output includes DOI and license details that were historically
+      not in the getSeries() function.
     """
     endpoint = "getSeriesMetaData"
 
     # create options dict to construct URL
     options = {}
     options['SeriesInstanceUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
-####### getSeriesSize function
-# Gets the file count and disk size of a series/scan
-# Requires Series Instance UID as input
-
 def getSeriesSize(seriesUid,
                   api_url = "",
                   format = ""):
     """
     Optional: api_url, format
     Gets the file count and disk size of a series/scan
     """
@@ -699,18 +627,14 @@
     # create options dict to construct URL
     options = {}
     options['SeriesInstanceUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
-####### getSopInstanceUids function
-# Gets SOP Instance UIDs from a specific series/scan
-# Requires a specific Series Instance UID as input
-
 def getSopInstanceUids(seriesUid,
                        api_url = "",
                        format = ""):
     """
     Optional: api_url, format
     Gets SOP Instance UIDs from a specific series/scan
     """
@@ -719,27 +643,24 @@
     # create options dict to construct URL
     options = {}
     options['SeriesInstanceUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
-####### getManufacturer function
-# Gets manufacturer metadata from a specified api_url
-# Allows filtering by collection, body part & modality
 
 def getManufacturer(collection = "",
                     modality = "",
                     bodyPart = "",
                     api_url = "",
                     format = ""):
     """
     All parameters are optional.
-    Gets manufacturer metadata from a specified api_url
-    Allows filtering by collection, body part & modality
+    Gets manufacturer metadata from a specified api_url.
+    Allows filtering by collection, body part & modality.
     """
     endpoint = "getManufacturerValues"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
@@ -748,71 +669,55 @@
         options['Modality'] = modality
     if bodyPart:
         options['BodyPartExamined'] = bodyPart
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
-####### getSharedCart function
-# Gets "Shared Cart" (scan) metadata from a specified api_url
-# Use https://nbia.cancerimagingarchive.net/nbia-search/ to create a cart
-# Add data to your basket, then click "Share" > "Share my cart"
-# The "name" parameter is part of the URL that generates.
-# E.g https://nbia.cancerimagingarchive.net/nbia-search/?saved-cart=nbia-49121659384603347
-#  has a cart "name" of "nbia-49121659384603347".
 
 def getSharedCart(name,
                   api_url = "",
                   format = ""):
     """
     Optional: api_url, format
-    Gets "Shared Cart" (scan) metadata from a specified api_url
-    First use https://nbia.cancerimagingarchive.net/nbia-search/ to create a cart, then add data to your basket, then click "Share" > "Share my cart".
-    The "name" parameter is part of the URL that generates. E.g https://nbia.cancerimagingarchive.net/nbia-search/?saved-cart=nbia-49121659384603347 has a cart "name" of "nbia-49121659384603347".
+    Gets "Shared Cart" metadata from a specified api_url.
+    First use https://nbia.cancerimagingarchive.net/nbia-search/ in a browser, 
+    then add data to your cart and click "Share" > "Share my cart".
+    This creates a shared cart with a URL like,
+    https://nbia.cancerimagingarchive.net/nbia-search/?saved-cart=nbia-49121659384603347 
+    You can then use this with a getSharedCart "name" of "nbia-49121659384603347".
     """
     endpoint = "getContentsByName"
 
     # create options dict to construct URL
     options = {}
     options['name'] = name
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
-####### downloadSeries function
-# Ingests a set of seriesUids and downloads them
-# By default, series_data expects JSON containing "SeriesInstanceUID" elements
-# Set number = n to download the first n series if you don't want the full dataset
-# Set hash = "y" if you'd like to retrieve MD5 hash values for each image
-# Saves to tciaDownload folder in current directory if no path is specified
-# Set input_type = "list" to pass a list of Series UIDs instead of JSON
-# Set input_type = "manifest" to pass the path of a *.TCIA manifest file as series_data
-# Format can be set to "df" or "csv" to return series metadata
-# Setting a csv_filename will create the csv even if format isn't specified
-# The metadata includes info about series that have previously been downloaded
-
 def downloadSeries(series_data,
                    number = 0,
                    path = "",
                    hash = "",
                    api_url = "",
                    input_type = "",
                    format = "",
                    csv_filename = ""):
     """
-    Ingests a set of seriesUids and downloads them
+    Ingests a set of seriesUids and downloads them.
     By default, series_data expects JSON containing "SeriesInstanceUID" elements.
     Set number = n to download the first n series if you don't want the full dataset.
     Set hash = "y" if you'd like to retrieve MD5 hash values for each image.
-    Saves to tciaDownload folder in current directory if no path is specified
+    Saves to tciaDownload folder in current directory if no path is specified.
     Set input_type = "list" to pass a list of Series UIDs instead of JSON.
     Set input_type = "manifest" to pass the path of a *.TCIA manifest file as series_data.
     Format can be set to "df" or "csv" to return series metadata.
     Setting a csv_filename will create the csv even if format isn't specified.
-    The metadata includes info about series that have previously been downloaded.
+    The metadata includes info about series that have previously been downloaded if they're part of series_data.
     """
     endpoint = "getImage"
     seriesUID = ''
     success = 0
     failed = 0
     previous = 0
 
@@ -1179,19 +1084,20 @@
     # create options dict to construct URL
     options = {}
     options['SeriesUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
     return data
     
-####### getSegRefSeries function (Advanced)
-# Gets DICOM tag metadata for a given SEG/RTSTRUCT series UID (scan)
-# and then look up the series UID they were derived from
 
 def getSegRefSeries(uid):
+    """
+    Gets DICOM tag metadata for a given SEG/RTSTRUCT series UID (scan)
+    and looks up the corresponding original/reference series UID
+    """
     # get dicom tags for the series as a dataframe
     df = getDicomTags(uid, format="df")
 
     if df is not None:
         # Find the row where element = "(0008,0060) Modality"
         findModality = df['element'] == '(0008,0060)'
         modality = df.loc[findModality, 'data'].item()
@@ -1206,15 +1112,15 @@
                 index = df.index[refElements].item()
 
                 # Retrieve the value of "Series Instance UID" from the next row
                 refSeriesUid = df.loc[index + 1, 'data']
                 return refSeriesUid
             
             else:
-                print("Segmentation doesn't contain a reference series UID.")
+                _log.warning(f"Series {uid} does not contain a Reference Series UID.")
                 refSeriesUid = "N/A"
                 return refSeriesUid
 
         elif modality == "SEG":
             # Locate ">(0008,114A) End Referenced Instance Sequence"
             # and ">(0020,000E) Series Instance UID" in the dataframe
             refElements = (df['element'] == '>(0008,114A)') & (df['element'].shift(-1) == '>(0020,000E)')
@@ -1224,25 +1130,25 @@
                 index = df.index[refElements].item()
 
                 # Retrieve the value of "Series Instance UID" from the next row
                 refSeriesUid = df.loc[index + 1, 'data']
                 return refSeriesUid
             
             else:
-                print("Segmentation doesn't contain a reference series UID.")
+                _log.warning(f"Series {uid} does not contain a Reference Series UID.")
                 refSeriesUid = "N/A"
                 return refSeriesUid
 
         else:
-            print("Segmentation series must be RTSTRUCT or SEG modality.")
+            _log.warning(f"Series {uid} is not a SEG/RTSTRUCT segmentation.")
             refSeriesUid = "N/A"
             return refSeriesUid
 
     else:
-        print("Segmentation series UID not found:", uid)
+        _log.warning(f"Series {uid} couldn't be found.")
         refSeriesUid = "N/A"
         return refSeriesUid
 
 
 
 ####### getDoiMetadata function
 # Gets a list of Collections or Series associated with a DOI
@@ -1717,7 +1623,218 @@
         # slide through dicom images using a slide bar
         def dicom_animation(x):
             plt.imshow(pixel_data[x], cmap = plt.cm.gray)
             plt.show()
         interact(dicom_animation, x=(0, len(pixel_data)-1))
     else:
         seriesInvalid(seriesUid)
+
+
+####### viewSeriesSEG function
+# Visualizes a Series (scan) you've downloaded in the notebook
+# Adds an overlay from the SEG series
+# Requires a path parameter for the reference series
+# Requires the file path for the annotative series
+# Not recommended to be used as a standalone function
+def viewSeriesSEG(seriesPath = "", SEGPath = ""):
+    """
+    Visualizes a Series (scan) you've downloaded in the notebook
+    Adds an overlay from the SEG series
+    Requires a path parameter for the reference series
+    Requires the file path for the annotative series
+    Not recommended to be used as a standalone function
+    """
+    slices = [pydicom.dcmread(seriesPath + '/' + s) for s in os.listdir(seriesPath) if s.endswith(".dcm")]
+    slices.sort(key = lambda x: int(x.InstanceNumber), reverse = True)
+
+    try:
+        modality = slices[0].Modality
+    except IndexError:
+        seriesInvalid(seriesUid)
+        raise StopExecution
+    
+    image = np.stack([s.pixel_array for s in slices])
+    image = image.astype(np.int16)
+
+    if modality == "CT":
+        # Set outside-of-scan pixels to 0
+        # The intercept is usually -1024, so air is approximately 0
+        image[image == -2000] = 0
+
+        # Convert to Hounsfield units (HU)
+        intercept = slices[0].RescaleIntercept
+        slope = slices[0].RescaleSlope
+
+        if slope != 1:
+            image = slope * image.astype(np.float64)
+            image = image.astype(np.int16)
+
+        image += np.int16(intercept)
+
+    pixel_data = np.array(image, dtype=np.int16)     
+    SEG_data = pydicom.dcmread(SEGPath)
+    try:
+        reader = pydicom_seg.MultiClassReader()
+        result = reader.read(SEG_data)
+    except ValueError:
+        reader = pydicom_seg.SegmentReader()
+        result = reader.read(SEG_data)
+
+    if slices[0].SeriesInstanceUID != result.referenced_series_uid:
+        raise Exception("The selected reference series and the annotative series don't match!")
+    
+    colorPaleatte = ["blue", "orange", "green", "red", "cyan", "brown", "lime", "purple", "yellow", "pink", "olive"] 
+    def seg_animation(x, **kwargs):
+        plt.imshow(pixel_data[x], cmap = plt.cm.gray)
+        if reader == pydicom_seg.MultiClassReader():
+            mask_data = result.data
+            cmap = matplotlib.colors.ListedColormap(colorPaleatte[i])
+            plt.imshow(mask_data[x], cmap = cmap, alpha = 0.5*(mask_data[x] > 0), interpolation = None)
+        else:
+            for i in result.available_segments:
+                if kwargs[list(kwargs)[i-1]] == True:
+                    mask_data = result.segment_data(i)
+                    cmap = matplotlib.colors.ListedColormap(colorPaleatte[i])
+                    plt.imshow(mask_data[x], cmap = cmap, alpha = 0.5*(mask_data[x] > 0), interpolation = None)
+        plt.axis('scaled')
+        plt.show()
+
+    if reader == pydicom_seg.MultiClassReader():
+        interact(seg_animation, x=(0, len(pixel_data)-1))
+    else:
+        kwargs = {v.SegmentDescription:True for i, v in enumerate(SEG_data.SegmentSequence)}
+        interact(seg_animation, x=(0, len(pixel_data)-1), **kwargs)
+
+
+####### viewSeriesRT function
+# Visualizes a Series (scan) you've downloaded in the notebook
+# Adds an overlay from the RTSTRUCT series
+# Requires a path parameter for the reference series
+# Requires the file path for the annotative series
+# Not recommended to be used as a standalone function
+def viewSeriesRT(seriesPath = "", RTPath = ""):
+    """
+    Visualizes a Series (scan) you've downloaded in the notebook
+    Adds an overlay from the RTSTRUCT series
+    Requires a path parameter for the reference series
+    Requires the file path for the annotative series
+    Not recommended to be used as a standalone function
+    """
+    rtstruct = rt_utils.RTStructBuilder.create_from(seriesPath, RTPath)
+    roi_names = rtstruct.get_roi_names()
+    
+    slices = rtstruct.series_data
+    try:
+        modality = slices[0].Modality
+    except IndexError:
+        seriesInvalid(seriesUid)
+        raise StopExecution
+    
+    image = np.stack([s.pixel_array for s in slices])
+    image = image.astype(np.int16)
+
+    if modality == "CT":
+        # Set outside-of-scan pixels to 0
+        # The intercept is usually -1024, so air is approximately 0
+        image[image == -2000] = 0
+
+        # Convert to Hounsfield units (HU)
+        intercept = slices[0].RescaleIntercept
+        slope = slices[0].RescaleSlope
+
+        if slope != 1:
+            image = slope * image.astype(np.float64)
+            image = image.astype(np.int16)
+
+        image += np.int16(intercept)
+
+    pixel_data = np.array(image, dtype=np.int16)
+    colorPaleatte = ["blue", "orange", "green", "red", "cyan", "brown", "lime", "purple", "yellow", "pink", "olive"] 
+    def rt_animation(x, **kwargs):
+        plt.imshow(pixel_data[x], cmap = plt.cm.gray, interpolation = None)
+        for i in range(len(roi_names)):
+            if kwargs[roi_names[i]] == True:
+                mask_data = rtstruct.get_roi_mask_by_name(roi_names[i])
+                cmap = matplotlib.colors.ListedColormap(colorPaleatte[i])
+                plt.imshow(mask_data[:, :, x], cmap = cmap, alpha = 0.5*(mask_data[:, :, x] > 0), interpolation = None)
+        plt.axis('scaled')
+        plt.show()
+    
+    kwargs = {v: True for i, v in enumerate(roi_names)}
+    interact(rt_animation, x = (0, len(pixel_data)-1), **kwargs)
+
+
+####### viewSeriesAnnotative function
+# Visualizes a Series (scan) you've downloaded in the notebook
+# Adds an overlay from the annotative series (SEG or RTSTRUCT)
+# Directs to the correct visualization function depending on the modality of the annotative series
+# Requires EITHER a seriesUid or path parameter for the reference series
+# Requires EITHER a annotationUid or path parameter for the segmentation series
+# Opens a file browser for users to choose folder/file if the required parameters are not specified
+# Leave seriesUid and/or annotationUid empty if you want to provide a custom path
+# The function assumes "tciaDownload/<UID>/" as path if seriesUid and/or annotationUid is
+#   provided since this is where downloadSeries() saves data
+# Note that non-axial images might not be correctly displayed.
+def viewSeriesAnnotation(seriesUid = "", seriesPath = "", annotationUid = "", annotationPath = ""):
+    """
+    Visualizes a Series (scan) you've downloaded in the notebook
+    Adds an overlay from the annotative series (SEG or RTSTRUCT)
+    Directs to the correct visualization function depending on the modality of the annotative series
+    Requires EITHER a seriesUid or path parameter for the reference series
+    Requires EITHER a annotationUid or path parameter for the segmentation series
+    Opens a file browser for users to choose folder/file if the required parameters are not specified
+    Leave seriesUid and/or annotationUid empty if you want to provide a custom path
+    The function assumes "tciaDownload/<UID>/" as path if seriesUid and/or annotationUid is provided since this is where downloadSeries() saves data.
+    Note that non-axial images might not be correctly displayed.
+    """
+    def seriesInvalid(uid, path):
+        if uid:
+            link = f"https://nbia.cancerimagingarchive.net/viewer/?series={uid}"
+        else:
+            link = "https://nbia.cancerimagingarchive.net/viewer/?series=YOUR_SERIES_UID"
+        _log.error(
+            f"Cannot find a valid DICOM series at: {path}\n"
+            'Try running downloadSeries(seriesUid, input_type = "uid") to download it first.\n'
+            "If the data isn't restricted, you can alternatively view it in your browser (without downloading) using this link:\n"
+            f"{link}"
+        )
+    
+    if seriesUid == "" and seriesPath == "":
+        try:
+            tkinter.Tk().withdraw()
+            folder_path = filedialog.askdirectory()
+            seriesPath = folder_path
+        except Exception:
+            _log.error(
+                f"\nYou are executing the function with unspecified parameters in an unsupported envrioment,"
+                "\nplease specify the reference series UID or the folder path instead."
+            )
+            return
+    elif seriesUid != "":
+        seriesPath = "tciaDownload/" + seriesUid
+        
+    if annotationUid == "" and annotationPath == "":
+        try:
+            tkinter.Tk().withdraw()
+            file_path = filedialog.askopenfilename()
+            annotationPath = file_path
+        except Exception:
+            _log.error(
+                f"\nYou are executing the function with unspecified parameters in an unsupported envrioment,"
+                "\nplease specify the annotation series UID or the folder path instead."
+            )
+            return
+    elif annotationUid != "":
+        annotationPath = "tciaDownload/" + annotationUid + "/1-1.dcm"
+
+    if os.path.isdir(seriesPath) and os.path.isfile(annotationPath):
+        annotationModality = pydicom.dcmread(annotationPath).Modality
+        if annotationModality == "SEG":
+            viewSeriesSEG(seriesPath, annotationPath)
+        elif annotationModality == "RTSTRUCT":
+            viewSeriesRT(seriesPath, annotationPath)
+        else:
+            print("Wrong modality for the segmentation series, please check your selection.")
+    elif not os.path.isdir(seriesPath):
+        seriesInvalid(seriesUid, seriesPath)
+    else:
+        seriesInvalid(annotationUid, annotationPath)
```

### Comparing `tcia_utils-1.5.1/src/tcia_utils/pathdb.py` & `tcia_utils-1.6/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5.1/.gitignore` & `tcia_utils-1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5.1/LICENSE` & `tcia_utils-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5.1/README.md` & `tcia_utils-1.6/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5.1/pyproject.toml` & `tcia_utils-1.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.5.1"
+version = "1.6"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,13 +19,15 @@
 
 dependencies = [
   "pydicom",
   "requests",
   "pandas",
   "matplotlib",
   "numpy",
-  "ipywidgets"
+  "ipywidgets", 
+  "pydicom-seg", 
+  "rt-utils"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/kirbyju/tcia_utils"
 "Bug Tracker" = "https://github.com/kirbyju/tcia_utils/issues"
```

### Comparing `tcia_utils-1.5.1/PKG-INFO` & `tcia_utils-1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.5.1
+Version: 1.6
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: ipywidgets
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pydicom
+Requires-Dist: pydicom-seg
 Requires-Dist: requests
+Requires-Dist: rt-utils
 Description-Content-Type: text/markdown
 
 # Overview
 The [tcia_utils](https://pypi.org/project/tcia-utils/) package contains functions to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python. Learn more about TCIA and its open-access datasets at https://www.cancerimagingarchive.net/.  Please be sure to comply with the [TCIA Data Usage Policy](https://wiki.cancerimagingarchive.net/x/c4hF).
 
 # Installation
 ```
```

