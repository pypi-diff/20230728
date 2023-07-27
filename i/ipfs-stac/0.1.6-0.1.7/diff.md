# Comparing `tmp/ipfs_stac-0.1.6.tar.gz` & `tmp/ipfs_stac-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfs_stac-0.1.6.tar", last modified: Thu Jul 20 23:15:16 2023, max compression
+gzip compressed data, was "ipfs_stac-0.1.7.tar", last modified: Thu Jul 27 23:00:27 2023, max compression
```

## Comparing `ipfs_stac-0.1.6.tar` & `ipfs_stac-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:16.187617 ipfs_stac-0.1.6/ipfs_stac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/ipfs_stac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/ipfs_stac/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/ipfs_stac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 23:15:16.000000 ipfs_stac-0.1.6/ipfs_stac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 23:15:16.191617 ipfs_stac-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 23:15:06.000000 ipfs_stac-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:27.470120 ipfs_stac-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 23:00:16.000000 ipfs_stac-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 23:00:16.000000 ipfs_stac-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-27 23:00:27.470120 ipfs_stac-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-27 23:00:16.000000 ipfs_stac-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:27.470120 ipfs_stac-0.1.7/ipfs_stac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:16.000000 ipfs_stac-0.1.7/ipfs_stac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-27 23:00:16.000000 ipfs_stac-0.1.7/ipfs_stac/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:00:27.470120 ipfs_stac-0.1.7/ipfs_stac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-27 23:00:27.000000 ipfs_stac-0.1.7/ipfs_stac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-27 23:00:27.000000 ipfs_stac-0.1.7/ipfs_stac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:00:27.000000 ipfs_stac-0.1.7/ipfs_stac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 23:00:27.000000 ipfs_stac-0.1.7/ipfs_stac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 23:00:27.000000 ipfs_stac-0.1.7/ipfs_stac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:00:27.470120 ipfs_stac-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 23:00:16.000000 ipfs_stac-0.1.7/setup.py
```

### Comparing `ipfs_stac-0.1.6/LICENSE` & `ipfs_stac-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfs_stac-0.1.6/PKG-INFO` & `ipfs_stac-0.1.7/ipfs_stac.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ipfs_stac
-Version: 0.1.6
+Name: ipfs-stac
+Version: 0.1.7
 Summary: The EASIER Data Initiative Python IPFS-STAC Client
 Author: The EASIER Data Initiative
 License: MIT
 Project-URL: Twitter, https://twitter.com/easierdataorg
 Project-URL: GitHub, https://github.com/easierdata/ipfs-stac
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,15 +35,18 @@
 
 ### Create a client object
 
 ```python
 from ipfs_stac import client
 
 # Create a new client object
-easier = client.web3(local_gateway="", stac="")
+easier = client.web3(local_gateway="", stac_endpoint="")
+
+# If you want to force using a local node, specify the endpoint in the local_gateway argument
+easier = client.web3(local_gateway="http://127.0.0.1:8000", stac_endpoint="")
 ```
 
 ### Fetch a CID from IPFS
 
 ```python
 # Simple hello world example
 data = easier.getFromCID("QmZ4tDuvesekSs4qM5ZBKpXiZGun7S2CYtEZRB3DYXkjGx")
@@ -65,38 +68,47 @@
 """
 ```
 
 ### Query STAC API By Bounding Box
 
 ```python
 easier = client.web3(local_gateway="", stac="<YOUR STAC ENDPOINT GOES HERE>")
+"""
+Retrieve all items from STAC catalog that are in bounding box with searchSTACByBox method (2 arguments)
+1. Coordinates of bounding box
+2. Name(s) of STAC collections)
+"""
+items = easier.searchSTACByBox([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"])
 
 """
-The searchSTACByBox by method takes 3 arguments
+The searchSTACByBoxIndex by method takes 3 arguments
 1. Coordinates for the bounding box
 2. Name of the STAC collection to query
 3. Index of the item you want to retrieve
 """
-item = easier.searchSTACByBox([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"], 0)
-band = easier.getBandFromItem(item, 'BAND NAME GOES HERE') # Returns band object
+item = easier.searchSTACByBoxIndex([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"], 0)
+band = easier.getAssetFromItem(item, 'ASSET NAME GOES HERE') # Returns asset object
 
-# Optionally, you can fetch multiple bands by the getBandsFromItem Method
-bands = easier.getBandsFromItem(item, ["blue", "red"]) # Returns array of bands
+# Optionally, you can fetch multiple assets by the getBandsFromItem Method
+bands = easier.getAssetsFromItem(item, ["blue", "red"]) # Returns array of assets
 ```
 
-### The band object
+### The asset object
 
 ```python
 # This snippet extends the previous under "Query STAC API By Bounding Box"
 
-# The band object, when printed, will return the CID
+# The asset object, when printed, will return the CID
 print(band) # QmNddx9BvBsQMXgwp6a83D2wiLrmovgCpRKVYKSJoWNNbx
 
-# You can fetch the band bytes through the fetch method
+# You can fetch the asset bytes through the fetch method
 data = band.fetch()
+
+# Alternatively, you can fetch the asset as an np array
+asset_array = band.fetchNPArray()
 ```
 
 # Attributions
 
 This project was made possible by the following
 
 * [ipfsspec](https://github.com/fsspec/ipfsspec)
```

### Comparing `ipfs_stac-0.1.6/README.md` & `ipfs_stac-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 
 ### Create a client object
 
 ```python
 from ipfs_stac import client
 
 # Create a new client object
-easier = client.web3(local_gateway="", stac="")
+easier = client.web3(local_gateway="", stac_endpoint="")
+
+# If you want to force using a local node, specify the endpoint in the local_gateway argument
+easier = client.web3(local_gateway="http://127.0.0.1:8000", stac_endpoint="")
 ```
 
 ### Fetch a CID from IPFS
 
 ```python
 # Simple hello world example
 data = easier.getFromCID("QmZ4tDuvesekSs4qM5ZBKpXiZGun7S2CYtEZRB3DYXkjGx")
@@ -54,38 +57,47 @@
 """
 ```
 
 ### Query STAC API By Bounding Box
 
 ```python
 easier = client.web3(local_gateway="", stac="<YOUR STAC ENDPOINT GOES HERE>")
+"""
+Retrieve all items from STAC catalog that are in bounding box with searchSTACByBox method (2 arguments)
+1. Coordinates of bounding box
+2. Name(s) of STAC collections)
+"""
+items = easier.searchSTACByBox([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"])
 
 """
-The searchSTACByBox by method takes 3 arguments
+The searchSTACByBoxIndex by method takes 3 arguments
 1. Coordinates for the bounding box
 2. Name of the STAC collection to query
 3. Index of the item you want to retrieve
 """
-item = easier.searchSTACByBox([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"], 0)
-band = easier.getBandFromItem(item, 'BAND NAME GOES HERE') # Returns band object
+item = easier.searchSTACByBoxIndex([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"], 0)
+band = easier.getAssetFromItem(item, 'ASSET NAME GOES HERE') # Returns asset object
 
-# Optionally, you can fetch multiple bands by the getBandsFromItem Method
-bands = easier.getBandsFromItem(item, ["blue", "red"]) # Returns array of bands
+# Optionally, you can fetch multiple assets by the getBandsFromItem Method
+bands = easier.getAssetsFromItem(item, ["blue", "red"]) # Returns array of assets
 ```
 
-### The band object
+### The asset object
 
 ```python
 # This snippet extends the previous under "Query STAC API By Bounding Box"
 
-# The band object, when printed, will return the CID
+# The asset object, when printed, will return the CID
 print(band) # QmNddx9BvBsQMXgwp6a83D2wiLrmovgCpRKVYKSJoWNNbx
 
-# You can fetch the band bytes through the fetch method
+# You can fetch the asset bytes through the fetch method
 data = band.fetch()
+
+# Alternatively, you can fetch the asset as an np array
+asset_array = band.fetchNPArray()
 ```
 
 # Attributions
 
 This project was made possible by the following
 
 * [ipfsspec](https://github.com/fsspec/ipfsspec)
```

### Comparing `ipfs_stac-0.1.6/ipfs_stac.egg-info/PKG-INFO` & `ipfs_stac-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ipfs-stac
-Version: 0.1.6
+Name: ipfs_stac
+Version: 0.1.7
 Summary: The EASIER Data Initiative Python IPFS-STAC Client
 Author: The EASIER Data Initiative
 License: MIT
 Project-URL: Twitter, https://twitter.com/easierdataorg
 Project-URL: GitHub, https://github.com/easierdata/ipfs-stac
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,15 +35,18 @@
 
 ### Create a client object
 
 ```python
 from ipfs_stac import client
 
 # Create a new client object
-easier = client.web3(local_gateway="", stac="")
+easier = client.web3(local_gateway="", stac_endpoint="")
+
+# If you want to force using a local node, specify the endpoint in the local_gateway argument
+easier = client.web3(local_gateway="http://127.0.0.1:8000", stac_endpoint="")
 ```
 
 ### Fetch a CID from IPFS
 
 ```python
 # Simple hello world example
 data = easier.getFromCID("QmZ4tDuvesekSs4qM5ZBKpXiZGun7S2CYtEZRB3DYXkjGx")
@@ -65,38 +68,47 @@
 """
 ```
 
 ### Query STAC API By Bounding Box
 
 ```python
 easier = client.web3(local_gateway="", stac="<YOUR STAC ENDPOINT GOES HERE>")
+"""
+Retrieve all items from STAC catalog that are in bounding box with searchSTACByBox method (2 arguments)
+1. Coordinates of bounding box
+2. Name(s) of STAC collections)
+"""
+items = easier.searchSTACByBox([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"])
 
 """
-The searchSTACByBox by method takes 3 arguments
+The searchSTACByBoxIndex by method takes 3 arguments
 1. Coordinates for the bounding box
 2. Name of the STAC collection to query
 3. Index of the item you want to retrieve
 """
-item = easier.searchSTACByBox([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"], 0)
-band = easier.getBandFromItem(item, 'BAND NAME GOES HERE') # Returns band object
+item = easier.searchSTACByBoxIndex([-76.964657, 38.978967, -76.928008, 39.002783], ["<STAC COLLECTION GOES HERE>"], 0)
+band = easier.getAssetFromItem(item, 'ASSET NAME GOES HERE') # Returns asset object
 
-# Optionally, you can fetch multiple bands by the getBandsFromItem Method
-bands = easier.getBandsFromItem(item, ["blue", "red"]) # Returns array of bands
+# Optionally, you can fetch multiple assets by the getBandsFromItem Method
+bands = easier.getAssetsFromItem(item, ["blue", "red"]) # Returns array of assets
 ```
 
-### The band object
+### The asset object
 
 ```python
 # This snippet extends the previous under "Query STAC API By Bounding Box"
 
-# The band object, when printed, will return the CID
+# The asset object, when printed, will return the CID
 print(band) # QmNddx9BvBsQMXgwp6a83D2wiLrmovgCpRKVYKSJoWNNbx
 
-# You can fetch the band bytes through the fetch method
+# You can fetch the asset bytes through the fetch method
 data = band.fetch()
+
+# Alternatively, you can fetch the asset as an np array
+asset_array = band.fetchNPArray()
 ```
 
 # Attributions
 
 This project was made possible by the following
 
 * [ipfsspec](https://github.com/fsspec/ipfsspec)
```

### Comparing `ipfs_stac-0.1.6/setup.py` & `ipfs_stac-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name='ipfs_stac',
     packages=find_packages(include=['ipfs_stac']),
-    version='0.1.6',
+    version='0.1.7',
     description='The EASIER Data Initiative Python IPFS-STAC Client',
     author='The EASIER Data Initiative',
     license='MIT',
-    install_requires=['ipfsspec', 'fsspec', 'requests', 'pandas', 'beautifulsoup4', 'pystac-client'],
+    install_requires=['ipfsspec', 'fsspec', 'requests', 'pandas', 'beautifulsoup4', 'pystac-client', 'Pillow', 'numpy'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     test_suite='tests',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     project_urls={
         "Twitter": "https://twitter.com/easierdataorg",
```

