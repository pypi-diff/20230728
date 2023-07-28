# Comparing `tmp/Xssec-0.1.0.tar.gz` & `tmp/Xssec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xssec-0.1.0.tar", last modified: Fri Jul 28 08:09:34 2023, max compression
+gzip compressed data, was "Xssec-0.1.5.tar", last modified: Fri Jul 28 08:27:43 2023, max compression
```

## Comparing `Xssec-0.1.0.tar` & `Xssec-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwx------   0 u0_a697  (10697) u0_a697  (10697)        0 2023-07-28 08:09:34.474018 Xssec-0.1.0/
--rw-------   0 u0_a697  (10697) u0_a697  (10697)      743 2023-07-28 08:01:45.000000 Xssec-0.1.0/LICENSE
--rw-------   0 u0_a697  (10697) u0_a697  (10697)      904 2023-07-28 08:09:34.470018 Xssec-0.1.0/PKG-INFO
--rw-------   0 u0_a697  (10697) u0_a697  (10697)      483 2023-07-28 07:39:46.000000 Xssec-0.1.0/README.md
-drwx------   0 u0_a697  (10697) u0_a697  (10697)        0 2023-07-28 08:09:34.470018 Xssec-0.1.0/Xssec.egg-info/
--rw-------   0 u0_a697  (10697) u0_a697  (10697)      904 2023-07-28 08:09:34.000000 Xssec-0.1.0/Xssec.egg-info/PKG-INFO
--rw-------   0 u0_a697  (10697) u0_a697  (10697)      142 2023-07-28 08:09:34.000000 Xssec-0.1.0/Xssec.egg-info/SOURCES.txt
--rw-------   0 u0_a697  (10697) u0_a697  (10697)        1 2023-07-28 08:09:34.000000 Xssec-0.1.0/Xssec.egg-info/dependency_links.txt
--rw-------   0 u0_a697  (10697) u0_a697  (10697)        1 2023-07-28 08:09:34.000000 Xssec-0.1.0/Xssec.egg-info/top_level.txt
--rw-------   0 u0_a697  (10697) u0_a697  (10697)       38 2023-07-28 08:09:34.474018 Xssec-0.1.0/setup.cfg
--rw-------   0 u0_a697  (10697) u0_a697  (10697)      659 2023-07-28 07:39:45.000000 Xssec-0.1.0/setup.py
+drwx------   0 u0_a697  (10697) u0_a697  (10697)        0 2023-07-28 08:27:43.422018 Xssec-0.1.5/
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)      743 2023-07-28 08:01:45.000000 Xssec-0.1.5/LICENSE
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)      843 2023-07-28 08:27:43.422018 Xssec-0.1.5/PKG-INFO
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)      422 2023-07-28 08:16:41.000000 Xssec-0.1.5/README.md
+drwx------   0 u0_a697  (10697) u0_a697  (10697)        0 2023-07-28 08:27:43.422018 Xssec-0.1.5/Xssec.egg-info/
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)      843 2023-07-28 08:27:43.000000 Xssec-0.1.5/Xssec.egg-info/PKG-INFO
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)      142 2023-07-28 08:27:43.000000 Xssec-0.1.5/Xssec.egg-info/SOURCES.txt
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)        1 2023-07-28 08:27:43.000000 Xssec-0.1.5/Xssec.egg-info/dependency_links.txt
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)        1 2023-07-28 08:27:43.000000 Xssec-0.1.5/Xssec.egg-info/top_level.txt
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)       38 2023-07-28 08:27:43.422018 Xssec-0.1.5/setup.cfg
+-rw-------   0 u0_a697  (10697) u0_a697  (10697)      659 2023-07-28 08:22:07.000000 Xssec-0.1.5/setup.py
```

### Comparing `Xssec-0.1.0/LICENSE` & `Xssec-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Xssec-0.1.0/PKG-INFO` & `Xssec-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xssec
-Version: 0.1.0
+Version: 0.1.5
 Summary: 一个可以加密文本的库
 Home-page: https://github.com/your_username/Xssec
 Author: Xssoft
 Author-email: xssoft2022@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,17 +39,9 @@
 # 将加密文本解密
 unlock_txt = unlock(lock_txt, psw)
 print("解密后的文本:", unlock_txt)
 ```
 
 
 
-_txt, psw)
-print("解密后的文本:", umlock_txt)
-```
-
-
-
-
-
```

### Comparing `Xssec-0.1.0/Xssec.egg-info/PKG-INFO` & `Xssec-0.1.5/Xssec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xssec
-Version: 0.1.0
+Version: 0.1.5
 Summary: 一个可以加密文本的库
 Home-page: https://github.com/your_username/Xssec
 Author: Xssoft
 Author-email: xssoft2022@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,17 +39,9 @@
 # 将加密文本解密
 unlock_txt = unlock(lock_txt, psw)
 print("解密后的文本:", unlock_txt)
 ```
 
 
 
-_txt, psw)
-print("解密后的文本:", umlock_txt)
-```
-
-
-
-
-
```

### Comparing `Xssec-0.1.0/setup.py` & `Xssec-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Xssec",
-    version="0.1.0",
+    version="0.1.5",
     author="Xssoft",
     author_email="xssoft2022@gmail.com",
     description="一个可以加密文本的库",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/your_username/Xssec",
     packages=find_packages(),
```

