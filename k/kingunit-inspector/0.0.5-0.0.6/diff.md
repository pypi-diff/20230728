# Comparing `tmp/kingunit_inspector-0.0.5.tar.gz` & `tmp/kingunit_inspector-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit-Inspector/dist/.tmp-tk8xfn3u/kingunit_inspector-0.0.5.tar", last modified: Wed Jul 19 08:17:48 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit-Inspector/dist/.tmp-a7vs63k9/kingunit_inspector-0.0.6.tar", last modified: Fri Jul 28 06:31:44 2023, max compression
```

## Comparing `kingunit_inspector-0.0.5.tar` & `kingunit_inspector-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 08:17:48.766437 kingunit_inspector-0.0.5/
--rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-07-19 06:48:32.000000 kingunit_inspector-0.0.5/LICENSE
--rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-19 08:17:48.766120 kingunit_inspector-0.0.5/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      111 2023-07-19 06:51:51.000000 kingunit_inspector-0.0.5/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 08:17:48.764369 kingunit_inspector-0.0.5/kingunit_inspector/
--rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-07-19 07:08:08.000000 kingunit_inspector-0.0.5/kingunit_inspector/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     3093 2023-07-19 08:17:33.000000 kingunit_inspector-0.0.5/kingunit_inspector/inspector.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 08:17:48.765795 kingunit_inspector-0.0.5/kingunit_inspector.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-19 08:17:48.000000 kingunit_inspector-0.0.5/kingunit_inspector.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      304 2023-07-19 08:17:48.000000 kingunit_inspector-0.0.5/kingunit_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-19 08:17:48.000000 kingunit_inspector-0.0.5/kingunit_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-19 08:17:48.000000 kingunit_inspector-0.0.5/kingunit_inspector.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-19 08:17:48.000000 kingunit_inspector-0.0.5/kingunit_inspector.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      443 2023-07-19 08:17:43.000000 kingunit_inspector-0.0.5/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-19 08:17:48.766550 kingunit_inspector-0.0.5/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 06:31:44.303296 kingunit_inspector-0.0.6/
+-rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-07-19 06:48:32.000000 kingunit_inspector-0.0.6/LICENSE
+-rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-28 06:31:44.303084 kingunit_inspector-0.0.6/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      111 2023-07-19 06:51:51.000000 kingunit_inspector-0.0.6/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 06:31:44.301563 kingunit_inspector-0.0.6/kingunit_inspector/
+-rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-07-19 07:08:08.000000 kingunit_inspector-0.0.6/kingunit_inspector/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     3478 2023-07-28 06:31:29.000000 kingunit_inspector-0.0.6/kingunit_inspector/inspector.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 06:31:44.302777 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      304 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      443 2023-07-28 06:31:34.000000 kingunit_inspector-0.0.6/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-28 06:31:44.303368 kingunit_inspector-0.0.6/setup.cfg
```

### Comparing `kingunit_inspector-0.0.5/LICENSE` & `kingunit_inspector-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kingunit_inspector-0.0.5/PKG-INFO` & `kingunit_inspector-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit_inspector
-Version: 0.0.5
+Version: 0.0.6
 Summary: KingUnit Inspector
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kingunit_inspector-0.0.5/kingunit_inspector/inspector.py` & `kingunit_inspector-0.0.6/kingunit_inspector/inspector.py`

 * *Files 15% similar despite different names*

```diff
@@ -87,18 +87,27 @@
     检查响应数据是否符合预期，对每一个参数进行检查，如不匹配则输出错误信息
     :param response: 响应
     :param expected_data: 预期数据
     :return: None
     """
 
     if "expected" not in test_case.keys() or test_case["expected"] == {} :
-        print("Expected data not configured, please check by yourself.")
+        print("未设定预期结果，请自行检查结果正确性。")
 
     # 输出响应结果
-    print(f"input:\n {test_case['input']}")
-    print(f"output:\n {response.json()}")
+    print(f"输入:\n {test_case['input']}")
+    print(f"输出:\n {response.json()}")
 
 
     if "expected" in test_case.keys() and test_case["expected"] != {}:
-        assert (
-            response.json() == test_case["expected"]
-        ), f"response expected: {str(test_case['expected'])}, actual: {str(response.json())}"
+        for key in test_case["expected"].keys():
+            assert (
+                key in response.json().keys()
+            ), f"key: {key}, not found in response"
+            assert (
+                str(response.json()[key]) == str(test_case["expected"][key])
+            ), f"response expected: {str(test_case['expected'][key])}, actual: {str(response.json()[key])}"
+
+
+        # assert (
+        #     response.json() == test_case["expected"]
+        # ), f"response expected: {str(test_case['expected'])}, actual: {str(response.json())}"
```

### Comparing `kingunit_inspector-0.0.5/kingunit_inspector.egg-info/PKG-INFO` & `kingunit_inspector-0.0.6/kingunit_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit-inspector
-Version: 0.0.5
+Version: 0.0.6
 Summary: KingUnit Inspector
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

