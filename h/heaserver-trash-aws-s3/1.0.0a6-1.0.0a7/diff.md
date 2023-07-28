# Comparing `tmp/heaserver-trash-aws-s3-1.0.0a6.tar.gz` & `tmp/heaserver-trash-aws-s3-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a6.tar", last modified: Thu Jul 27 02:23:54 2023, max compression
+gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a7.tar", last modified: Fri Jul 28 20:52:28 2023, max compression
```

## Comparing `heaserver-trash-aws-s3-1.0.0a6.tar` & `heaserver-trash-aws-s3-1.0.0a7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.556165 heaserver-trash-aws-s3-1.0.0a6/
--rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/LICENSE
--rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/MANIFEST.in
--rw-rw-rw-   0        0        0     4352 2023-07-27 02:23:54.555167 heaserver-trash-aws-s3-1.0.0a6/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 02:23:54.556165 heaserver-trash-aws-s3-1.0.0a6/setup.cfg
--rw-rw-rw-   0        0        0     1869 2023-07-27 02:23:18.000000 heaserver-trash-aws-s3-1.0.0a6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.514853 heaserver-trash-aws-s3-1.0.0a6/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.513858 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.522856 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    48660 2023-05-20 05:24:56.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.524853 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.550165 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4352 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.515853 heaserver-trash-aws-s3-1.0.0a6/tests/
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.515853 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.554169 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    68605 2023-07-27 02:15:49.000000 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6281 2023-07-27 02:05:15.000000 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.411784 heaserver-trash-aws-s3-1.0.0a7/
+-rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a7/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4352 2023-07-28 20:52:28.411784 heaserver-trash-aws-s3-1.0.0a7/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 20:52:28.411784 heaserver-trash-aws-s3-1.0.0a7/setup.cfg
+-rw-rw-rw-   0        0        0     1869 2023-07-28 20:51:55.000000 heaserver-trash-aws-s3-1.0.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.363799 heaserver-trash-aws-s3-1.0.0a7/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.363799 heaserver-trash-aws-s3-1.0.0a7/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.383683 heaserver-trash-aws-s3-1.0.0a7/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    49200 2023-07-28 20:51:32.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.384683 heaserver-trash-aws-s3-1.0.0a7/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.409681 heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4352 2023-07-28 20:52:28.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-07-28 20:52:28.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 20:52:28.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-28 20:52:28.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-07-28 20:52:28.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 20:52:28.000000 heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.363799 heaserver-trash-aws-s3-1.0.0a7/tests/
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.363799 heaserver-trash-aws-s3-1.0.0a7/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-07-28 20:52:28.411784 heaserver-trash-aws-s3-1.0.0a7/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a7/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    68605 2023-07-27 02:15:49.000000 heaserver-trash-aws-s3-1.0.0a7/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6281 2023-07-27 02:05:15.000000 heaserver-trash-aws-s3-1.0.0a7/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver-trash-aws-s3-1.0.0a6/LICENSE` & `heaserver-trash-aws-s3-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a6/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a6/README.md` & `heaserver-trash-aws-s3-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a6/setup.py` & `heaserver-trash-aws-s3-1.0.0a7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.0.0a6',
+    version='1.0.0a7',
     description="deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
```

### Comparing `heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/service.py` & `heaserver-trash-aws-s3-1.0.0a7/src/heaserver/trashawss3/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -753,15 +753,15 @@
         s3 = await request.app[HEA_DB].get_client(request, 's3', volume_id)
     except ValueError as e:
         raise response.status_not_found()
     loop_ = asyncio.get_running_loop()
     delete_marker = None
     async for response_ in _get_version_objects(s3, bucket_id, key_, loop_):
         keyfunc = lambda x: x['Key']
-        for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain((resp for resp in response_.get('DeleteMarkers', []) if resp['Key'].startswith(key_)), (resp for resp in response_.get('Versions', []) if resp['Key'].startswith(key_)))), key=keyfunc), key=keyfunc):
+        for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain((resp for resp in response_.get('DeleteMarkers', []) if resp['Key'].startswith(key_)), (resp for resp in response_.get('Versions', []) if resp['VersionId'] != 'null' and resp['Key'].startswith(key_)))), key=keyfunc), key=keyfunc):
             for resp_ in sorted(versions, key=lambda x: x['LastModified'], reverse=True):
                 if 'Size' not in resp_ and resp_['VersionId'] == version_:
                     delete_marker = resp_
                     break
     if delete_marker:
         encoded_key = encode_key(key)
         last_modified = delete_marker['LastModified']
@@ -842,15 +842,15 @@
 
 async def _get_deleted_items_private(s3, volume_id, bucket_id, prefix=None, sub_user=None) -> AsyncIterator[DesktopObjectDict]:
     loop_ = asyncio.get_running_loop()
 
     async for response_ in _get_version_objects(s3, bucket_id, prefix, loop_):
         keyfunc = lambda x: x['Key']
         keys = set()  # Potentially delete?
-        for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_.get('DeleteMarkers', []), response_.get('Versions', []))), key=keyfunc), key=keyfunc):
+        for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain((vers for vers in response_.get('DeleteMarkers', []) if vers['VersionId'] != 'null'), (vers for vers in response_.get('Versions', []) if vers['VersionId'] != 'null'))), key=keyfunc), key=keyfunc):
             if prefix is not None and not key.startswith(prefix):
                 continue
             delete_markers_to_versions = {}
             delete_markers = []
             prev_delete_marker = None
             for is_delete_marker, versions_ in itertools.groupby(versions, key=lambda x: 'Size' not in x):
                 if is_delete_marker:
@@ -940,22 +940,22 @@
         if not await _get_deleted_item(request):
             return response.status_not_found(f'Object {display_name(key_)} is not in the trash')
         s3_client = await request.app[HEA_DB].get_client(request, 's3', volume_id)
         async for response_ in _get_version_objects(s3_client, bucket_name, key_, loop):
             keyfunc = lambda x: x['Key']
 
             # Preflight
-            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_['DeleteMarkers'], response_.get('Versions', []))), key=keyfunc), key=keyfunc):
+            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain((vers for vers in response_['DeleteMarkers'] if vers['VersionId'] != 'null'), (vers for vers in response_.get('Versions', []) if vers['VersionId'] != 'null'))), key=keyfunc), key=keyfunc):
                 resps = sorted(versions, key=lambda x: x['LastModified'], reverse=True)
                 if resps and 'Size' in resps[0]:
                     if not is_folder(resps[0]['Key']):
                         return response.status_bad_request(f'Object {display_name(key)} has been overwritten')
 
             # Actual
-            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_['DeleteMarkers'], response_.get('Versions', []))), key=keyfunc), key=keyfunc):
+            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain((vers for vers in response_['DeleteMarkers'] if vers['VersionId'] != 'null'), (vers for vers in response_.get('Versions', []) if vers['VersionId'] != 'null'))), key=keyfunc), key=keyfunc):
                 resps = sorted(versions, key=lambda x: x['LastModified'], reverse=True)
                 for resp_ in resps:
                     if 'Size' not in resp_:  # Delete the delete markers until we reach actual version objects.
                         s3_client.delete_object(Bucket=bucket_name, Key=resp_['Key'], VersionId=resp_['VersionId'])
                     else:
                         break
 
@@ -1097,15 +1097,15 @@
 
     try:
         s3_client = await request.app[HEA_DB].get_client(request, 's3', volume_id)
         async for response_ in _get_version_objects(s3_client, bucket_name, key, loop):
             delete_markers_to_delete = []
             versions_to_delete = []
             delete_marker = False
-            for resp_ in sorted((resp for resp in itertools.chain(response_.get('DeleteMarkers', []), response_.get('Versions', [])) if resp['Key'] == key), key=lambda x: x['LastModified'], reverse=True):
+            for resp_ in sorted((resp for resp in itertools.chain((vers for vers in response_.get('DeleteMarkers', []) if vers['VersionId'] != 'null'), (vers for vers in response_.get('Versions', []) if vers['VersionId'] != 'null')) if resp['Key'] == key), key=lambda x: x['LastModified'], reverse=True):
                 if not delete_marker and resp_['VersionId'] == version:
                     delete_marker = True
                     delete_markers_to_delete.append(resp_)
                     continue
                 if delete_marker and 'Size' not in resp_ and versions_to_delete:
                     delete_marker = False
                     break
@@ -1145,15 +1145,15 @@
 
     loop = asyncio.get_running_loop()
 
     try:
         s3_client = await request.app[HEA_DB].get_client(request, 's3', volume_id)
         async for response_ in _get_version_objects(s3_client, bucket_name, None, loop):
             keyfunc = lambda x: x['Key']
-            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_.get('DeleteMarkers', []), response_['Versions'])), key=keyfunc), key=keyfunc):
+            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain((vers for vers in response_.get('DeleteMarkers', []) if vers['VersionId'] != 'null'), (vers for vers in response_.get('Versions', []) if vers['VersionId'] != 'null'))), key=keyfunc), key=keyfunc):
                 delete_markers_to_delete = []
                 versions_to_delete = []
                 delete_markers = True
                 for resp_ in sorted((resp for resp in versions), key=lambda x: x['LastModified'], reverse=True):
                     if delete_markers and 'Size' not in resp_:
                         delete_markers_to_delete.append(resp_)
                     elif 'Size' in resp_ and delete_markers_to_delete:
```

### Comparing `heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/wstl/all.json` & `heaserver-trash-aws-s3-1.0.0a7/src/heaserver/trashawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver-trash-aws-s3-1.0.0a7/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/test_all.py` & `heaserver-trash-aws-s3-1.0.0a7/tests/heaserver/trashawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/testcase.py` & `heaserver-trash-aws-s3-1.0.0a7/tests/heaserver/trashawss3test/testcase.py`

 * *Files identical despite different names*

