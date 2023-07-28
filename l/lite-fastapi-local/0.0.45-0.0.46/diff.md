# Comparing `tmp/lite_fastapi_local-0.0.45.tar.gz` & `tmp/lite_fastapi_local-0.0.46.tar.gz`

## Comparing `lite_fastapi_local-0.0.45.tar` & `lite_fastapi_local-0.0.46.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/QR_READ_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/__init__.py
--rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/requirements.txt
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/common/__init__.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/common/function.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/common/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/boxDoorModel.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/drimmLedModel.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/innerLedModel.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/motorModel.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/registrationModel.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/setupModel.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/solModel.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/sprayModel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/router/__init__.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/router/motorRouter.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/router/sensorRouter.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/src/lite_fastapi_local/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.45/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/__init__.py
+-rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/__init__.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/drimmLedModel.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/innerLedModel.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/registrationModel.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/__init__.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/QR_CHK_dep.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/QR_READ_dep.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/main.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/main.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/requirements.txt` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/settings.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/common/function.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,16 @@
                 i +=1
                 if i > 1:
                     is_ready = False
 
             if i>1:
                 up_ret, up_frame = up_cap.read()
                 up_filename = f'./Save_file/{date_time_string}/product/up_img_{datetime.now().strftime("%Y-%m-%d-%H-%M-%S-%f")}.jpg'
-                data_name_list.append(up_filename)
+                if i < 5:
+                    data_name_list.append(up_filename)
                 cv2.imwrite(up_filename,up_frame)
                 print(i)
                 if i < 8:
                     i += 1
                 else:
                     if len(data_name_list) < 10:
                         common.set_image_directory(data_name_list[0])
```

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/common/variable.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/motorModel.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/setupModel.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/setupModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/model/solModel.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/router/motorRouter.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/motorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/router/sensorRouter.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/src/lite_fastapi_local/router/setupRouter.py` & `lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/LICENSE` & `lite_fastapi_local-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.45/pyproject.toml` & `lite_fastapi_local-0.0.46/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.45"
+version = "0.0.46"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.45/PKG-INFO` & `lite_fastapi_local-0.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.45
+Version: 0.0.46
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

