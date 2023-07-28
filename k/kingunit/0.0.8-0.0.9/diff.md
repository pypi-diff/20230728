# Comparing `tmp/kingunit-0.0.8.tar.gz` & `tmp/kingunit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-65ou4uus/kingunit-0.0.8.tar", last modified: Fri Jul 28 01:46:03 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-0igysd4s/kingunit-0.0.9.tar", last modified: Fri Jul 28 01:52:21 2023, max compression
```

## Comparing `kingunit-0.0.8.tar` & `kingunit-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.215989 kingunit-0.0.8/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-28 01:46:03.215696 kingunit-0.0.8/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.8/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.208459 kingunit-0.0.8/kingunit/
--rw-r--r--   0 jiayu      (501) staff       (20)       46 2023-07-27 06:35:32.000000 kingunit-0.0.8/kingunit/__init__.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.212952 kingunit-0.0.8/kingunit/cmd/
--rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-27 06:35:22.000000 kingunit-0.0.8/kingunit/cmd/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.8/kingunit/cmd/cmd.py
--rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.8/kingunit/cmd/main.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.213537 kingunit-0.0.8/kingunit/config/
--rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.8/kingunit/config/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.8/kingunit/config/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     4302 2023-07-28 01:44:55.000000 kingunit-0.0.8/kingunit/generator.py
--rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.8/kingunit/init.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.215110 kingunit-0.0.8/kingunit/utils/
--rw-r--r--   0 jiayu      (501) staff       (20)       66 2023-07-27 06:19:49.000000 kingunit-0.0.8/kingunit/utils/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.8/kingunit/utils/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.8/kingunit/utils/mail.py
--rw-r--r--   0 jiayu      (501) staff       (20)      171 2023-07-27 06:19:42.000000 kingunit-0.0.8/kingunit/utils/validator.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.211868 kingunit-0.0.8/kingunit.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      466 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-28 01:45:30.000000 kingunit-0.0.8/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-28 01:46:03.216062 kingunit-0.0.8/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:52:21.728565 kingunit-0.0.9/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-28 01:52:21.728337 kingunit-0.0.9/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.9/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:52:21.724770 kingunit-0.0.9/kingunit/
+-rw-r--r--   0 jiayu      (501) staff       (20)       46 2023-07-27 06:35:32.000000 kingunit-0.0.9/kingunit/__init__.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:52:21.726806 kingunit-0.0.9/kingunit/cmd/
+-rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-27 06:35:22.000000 kingunit-0.0.9/kingunit/cmd/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.9/kingunit/cmd/cmd.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.9/kingunit/cmd/main.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:52:21.727327 kingunit-0.0.9/kingunit/config/
+-rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.9/kingunit/config/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.9/kingunit/config/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     4363 2023-07-28 01:51:42.000000 kingunit-0.0.9/kingunit/generator.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.9/kingunit/init.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:52:21.728058 kingunit-0.0.9/kingunit/utils/
+-rw-r--r--   0 jiayu      (501) staff       (20)       66 2023-07-27 06:19:49.000000 kingunit-0.0.9/kingunit/utils/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.9/kingunit/utils/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.9/kingunit/utils/mail.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      171 2023-07-27 06:19:42.000000 kingunit-0.0.9/kingunit/utils/validator.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:52:21.725995 kingunit-0.0.9/kingunit.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-28 01:52:21.000000 kingunit-0.0.9/kingunit.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      466 2023-07-28 01:52:21.000000 kingunit-0.0.9/kingunit.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-28 01:52:21.000000 kingunit-0.0.9/kingunit.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-28 01:52:21.000000 kingunit-0.0.9/kingunit.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-28 01:52:21.000000 kingunit-0.0.9/kingunit.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-28 01:51:55.000000 kingunit-0.0.9/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-28 01:52:21.728632 kingunit-0.0.9/setup.cfg
```

### Comparing `kingunit-0.0.8/PKG-INFO` & `kingunit-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.8
+Version: 0.0.9
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

### Comparing `kingunit-0.0.8/README.md` & `kingunit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.8/kingunit/cmd/cmd.py` & `kingunit-0.0.9/kingunit/cmd/cmd.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.8/kingunit/generator.py` & `kingunit-0.0.9/kingunit/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,17 @@
     """    
 
     # 创建测试文件夹，检查是否存在
     if not os.path.exists(f"{config['output_path']}"):
         os.mkdir(f"{config['output_path']}")
 
     print(api_file)
-    if not os.path.exists(f"{config['output_path']}/{api_file['name']}"):
-        os.mkdir(f"{config['output_path']}/{api_file['name']}")
+    if os.path.exists(f"{config['output_path']}/{api_file['name']}"):
+        shutil.rmtree(f"{config['output_path']}/{api_file['name']}")
+    os.mkdir(f"{config['output_path']}/{api_file['name']}")
 
     # 生成测试文件
     with open(
         f"{config['output_path']}/{api_file['name']}/{config['test_cases_file']}", "w"
     ) as file:
         file.write("from kingunit_inspector.inspector import *\n")
         for case in api_file["apis"]:
```

### Comparing `kingunit-0.0.8/kingunit/init.py` & `kingunit-0.0.9/kingunit/init.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.8/kingunit/utils/mail.py` & `kingunit-0.0.9/kingunit/utils/mail.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.8/kingunit.egg-info/PKG-INFO` & `kingunit-0.0.9/kingunit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.8
+Version: 0.0.9
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

