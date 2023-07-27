# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051.tar", last modified: Thu Jul 27 18:21:43 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917.tar", last modified: Thu Jul 27 22:30:09 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:21:43.267366 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 18:21:43.267366 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 18:21:43.267366 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-27 18:21:40.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:21:43.263366 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:21:43.267366 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    22845 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
--rw-r--r--   0 root         (0) root         (0)     1288 2023-07-27 18:20:46.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/test_dynamo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:21:43.267366 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 18:21:43.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-27 18:21:43.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 18:21:43.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-27 18:21:43.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-27 18:21:43.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:09.841889 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 22:30:09.841889 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 22:30:09.841889 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-27 22:30:07.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:09.837889 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:09.841889 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    24047 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2023-07-27 22:29:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/test_dynamo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 22:30:09.841889 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 22:30:09.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-27 22:30:09.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 22:30:09.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-27 22:30:09.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-27 22:30:09.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230727182051
+Version: 1.0.0.dev20230727222917
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230727182051",
+  version="1.0.0.dev20230727222917",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,18 +307,18 @@
         # path should be like: f's3://{input_zarr_bucket}/{input_zarr_path}'
         store = self.__s3fs.s3_map(
             s3_zarr_store_path=f"s3://{self.__output_bucket}/{zarr_path}",
             access_key_id=self.__output_bucket_access_key,
             secret_access_key=self.__output_bucket_secret_access_key,
         )
         # You are already using dask, this is assumed by open_zarr, not the same as open_dataset(engine=“zarr”)
-        import fsspec
         return xr.open_zarr(store=store, consolidated=None)  # synchronizer=SYNCHRONIZER
 
     ############################################################################
+    ############################################################################
     def __interpolate_data(
             self,
             minimum_resolution: float,  # get from df
             maximum_cruise_depth_meters: float,  # get from df
             file_xr: xr.Dataset,  # need to figure out which time values are removed
             cruise_zarr: zarr.Group,
             start_ping_time_index: int,
@@ -421,26 +421,52 @@
         longitude = geo_json.dropna().longitude.tolist()
         latitude = geo_json.dropna().latitude.tolist()
         #
         return latitude, longitude, epoch_seconds
 
 
     ############################################################################
+    def __read_s3_geo_json(
+            self,
+            input_zarr_path: str,
+            access_key_id: str = None,
+            secret_access_key: str = None,
+    ) -> str:
+        # reads geojson file from s3 bucket w boto3
+        # session = boto3.Session()
+        # s3 = boto3.resource(
+        #     service_name='s3',
+        #     aws_access_key_id=access_key_id,
+        #     aws_secret_access_key=secret_access_key,
+        # )
+        s3 = self.__s3.get_object(
+            self.__output_bucket,
+            input_zarr_path,
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        )
+        content_object = s3.Object(self.__output_bucket, f'{input_zarr_path}/geo.json')
+        file_content = content_object.get()['Body'].read().decode('utf-8')
+        json_content = json.loads(file_content)
+        return json_content
+
+
+    ############################################################################
     def __publish_done_message(self, message):
         print("Sending done message")
         self.__sns_operations.publish(self.__done_topic_arn, json.dumps(message))
 
 
     ############################################################################
     def execute(self, message):
         # {"shipName":"Henry_B._Bigelow","cruiseName":"HB0707","sensorName":"EK60","fileName":"D20070711-T210709.raw"}
         ship_name = message['shipName']  # 'Henry_B._Bigelow'
         cruise_name = message['cruiseName']  # 'HB0707'
         sensor_name = message['sensorName']  # 'EK60'
-        input_file_name = message['fileName']
+        input_file_name = message['fileName']  # 'D20070711-T210709.raw'
         #
         file_stem = os.path.splitext(input_file_name)[0]
         input_zarr_path = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{file_stem}.zarr"
         #
         os.chdir(TEMPDIR)
         #
         ### COPY N PASTED IN BELOW #######################################################
@@ -458,17 +484,17 @@
         input_zarr_path = file_info['ZARR_PATH']
         output_zarr_bucket = file_info['ZARR_BUCKET']
         #
         #################################################################
         # [1] read file-level Zarr store using xarray
         file_xr = self.__get_s3_zarr_as_xr(zarr_path=input_zarr_path)
         geo_json = self.__read_s3_geo_json(
-            s3_geo_json_path=f's3://{input_zarr_bucket}/{input_zarr_path}/geo.json',
+            input_zarr_path=input_zarr_path,
             access_key_id=os.getenv('ACCESS_KEY_ID'),
-            secret_access_key=os.getenv('SECRET_ACCESS_KEY'),
+            secret_access_key=os.getenv('SECRET_ACCESS_KEY')
         )
         #geo_json['features'][0]
         # {'id': '2007-07-12T15:24:16.032000000', 'type': 'Feature', 'properties': {'latitude': None, 'longitude': None}, 'geometry': None}
         # reads GeoJSON with the id as the index
         geospatial = geopandas.GeoDataFrame.from_features(geo_json['features']).set_index(pd.json_normalize(geo_json["features"])["id"].values)
         geospatial_index = geospatial.dropna().index.values.astype('datetime64[ns]')
         # find the indices where 'v' can be inserted into 'a'
@@ -476,15 +502,16 @@
         #
         # TODO: only need to read the geojson file once instead of twice here...
         #
         #########################################################################
         #########################################################################
         # [2] open cruise level zarr store for writing
         # output_zarr_path: str = f'',
-        cruise_zarr = self.__get_s3_zarr(
+        print('opening cruise zarr')
+        cruise_zarr = self.__s3_zarr(
             output_zarr_bucket,
             ship_name,
             cruise_name,
             sensor_name,
             # zarr_synchronizer  # TODO:
         )
         #########################################################################
@@ -511,17 +538,21 @@
         #########################################################################
         # [5] write subset of latitude/longitude
         cruise_zarr.latitude[start_ping_time_index:end_ping_time_index] = latitude
         cruise_zarr.longitude[start_ping_time_index:end_ping_time_index] = longitude
         #########################################################################
         # [6] get interpolated Sv data
         filename = os.path.basename(input_zarr_path)
+        print('interpolate_data')
+        print(type(df['MIN_ECHO_RANGE']))
+        print(df['MIN_ECHO_RANGE'])
+        print(np.float32(df['MIN_ECHO_RANGE']))
         all_Sv_prototype = self.__interpolate_data(
             minimum_resolution = np.nanmin(np.float32(df['MIN_ECHO_RANGE'])),
-            maximum_cruise_depth_meters = np.max(np.float32(df['MAX_ECHO_RANGE'])),
+            maximum_cruise_depth_meters = np.nanmax(np.float32(df['MAX_ECHO_RANGE'])),
             # num_ping_time_dropna = int(df.iloc[index]['NUM_PING_TIME_DROPNA']),
             file_xr=file_xr,
             cruise_zarr=cruise_zarr,
             start_ping_time_index=start_ping_time_index,
             end_ping_time_index=end_ping_time_index,
             indices=indices,
         )  # TODO:
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         else:
             s3_fs = s3fs.S3FileSystem()
         return s3_fs
 
     #####################################################################
     def s3_map(
             self,
-            s3_zarr_store_path,
+            s3_zarr_store_path,  # f's3://{bucket}/{input_zarr_path}'
             access_key_id=None,
             secret_access_key=None,
     ):
         s3_fs = self.__get_s3_fs(
             access_key_id=access_key_id,
             secret_access_key=secret_access_key
         )
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda/test_dynamo.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda/test_dynamo.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230727182051
+Version: 1.0.0.dev20230727222917
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727182051/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727222917/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

