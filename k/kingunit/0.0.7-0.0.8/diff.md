# Comparing `tmp/kingunit-0.0.7.tar.gz` & `tmp/kingunit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-nqv24pi6/kingunit-0.0.7.tar", last modified: Thu Jul 27 06:46:47 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-65ou4uus/kingunit-0.0.8.tar", last modified: Fri Jul 28 01:46:03 2023, max compression
```

## Comparing `kingunit-0.0.7.tar` & `kingunit-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:46:47.314899 kingunit-0.0.7/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:46:47.314673 kingunit-0.0.7/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.7/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:46:47.309892 kingunit-0.0.7/kingunit/
--rw-r--r--   0 jiayu      (501) staff       (20)       46 2023-07-27 06:35:32.000000 kingunit-0.0.7/kingunit/__init__.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:46:47.312439 kingunit-0.0.7/kingunit/cmd/
--rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-27 06:35:22.000000 kingunit-0.0.7/kingunit/cmd/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.7/kingunit/cmd/cmd.py
--rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.7/kingunit/cmd/main.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:46:47.313231 kingunit-0.0.7/kingunit/config/
--rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.7/kingunit/config/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.7/kingunit/config/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     4286 2023-07-27 06:46:17.000000 kingunit-0.0.7/kingunit/generator.py
--rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.7/kingunit/init.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:46:47.314410 kingunit-0.0.7/kingunit/utils/
--rw-r--r--   0 jiayu      (501) staff       (20)       66 2023-07-27 06:19:49.000000 kingunit-0.0.7/kingunit/utils/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.7/kingunit/utils/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.7/kingunit/utils/mail.py
--rw-r--r--   0 jiayu      (501) staff       (20)      171 2023-07-27 06:19:42.000000 kingunit-0.0.7/kingunit/utils/validator.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:46:47.311453 kingunit-0.0.7/kingunit.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:46:47.000000 kingunit-0.0.7/kingunit.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      466 2023-07-27 06:46:47.000000 kingunit-0.0.7/kingunit.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-27 06:46:47.000000 kingunit-0.0.7/kingunit.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-27 06:46:47.000000 kingunit-0.0.7/kingunit.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-27 06:46:47.000000 kingunit-0.0.7/kingunit.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-27 06:46:37.000000 kingunit-0.0.7/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-27 06:46:47.314976 kingunit-0.0.7/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.215989 kingunit-0.0.8/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-28 01:46:03.215696 kingunit-0.0.8/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.8/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.208459 kingunit-0.0.8/kingunit/
+-rw-r--r--   0 jiayu      (501) staff       (20)       46 2023-07-27 06:35:32.000000 kingunit-0.0.8/kingunit/__init__.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.212952 kingunit-0.0.8/kingunit/cmd/
+-rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-27 06:35:22.000000 kingunit-0.0.8/kingunit/cmd/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.8/kingunit/cmd/cmd.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.8/kingunit/cmd/main.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.213537 kingunit-0.0.8/kingunit/config/
+-rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.8/kingunit/config/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.8/kingunit/config/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     4302 2023-07-28 01:44:55.000000 kingunit-0.0.8/kingunit/generator.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.8/kingunit/init.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.215110 kingunit-0.0.8/kingunit/utils/
+-rw-r--r--   0 jiayu      (501) staff       (20)       66 2023-07-27 06:19:49.000000 kingunit-0.0.8/kingunit/utils/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.8/kingunit/utils/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.8/kingunit/utils/mail.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      171 2023-07-27 06:19:42.000000 kingunit-0.0.8/kingunit/utils/validator.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 01:46:03.211868 kingunit-0.0.8/kingunit.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      466 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-28 01:46:03.000000 kingunit-0.0.8/kingunit.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-28 01:45:30.000000 kingunit-0.0.8/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-28 01:46:03.216062 kingunit-0.0.8/setup.cfg
```

### Comparing `kingunit-0.0.7/PKG-INFO` & `kingunit-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.7
+Version: 0.0.8
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

### Comparing `kingunit-0.0.7/README.md` & `kingunit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.7/kingunit/cmd/cmd.py` & `kingunit-0.0.8/kingunit/cmd/cmd.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.7/kingunit/generator.py` & `kingunit-0.0.8/kingunit/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
     生成测试报告
     """
 
     # 检查pytest是否安装
     if os.system("pytest --version") == 0:
         allure_path = f"--alluredir={config['output_path']}/{case_name}/allure-jsons"
         os.system(
-            f"pytest {config['output_path']}/{case_name}/{config['test_cases_file']} --html={config['output_path']}/{case_name}/report.html {allure_path if use_allure else ''}"
-        )
+            f"nohup pytest {config['output_path']}/{case_name}/{config['test_cases_file']} --html={config['output_path']}/{case_name}/report.html {allure_path if use_allure else ''} &"
+        )        
     else:
         raise Exception("Pytest not found.")
 
 
 def Test_Case(case_name: str, endpoint: str):
     """
     对测试用例的具体某个测试点进行测试
```

### Comparing `kingunit-0.0.7/kingunit/init.py` & `kingunit-0.0.8/kingunit/init.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.7/kingunit/utils/mail.py` & `kingunit-0.0.8/kingunit/utils/mail.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.7/kingunit.egg-info/PKG-INFO` & `kingunit-0.0.8/kingunit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.7
+Version: 0.0.8
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

