# Comparing `tmp/lbTool-1.1.1.tar.gz` & `tmp/lbTool-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbTool-1.1.1.tar", last modified: Fri Jul 28 02:18:06 2023, max compression
+gzip compressed data, was "lbTool-1.1.2.tar", last modified: Fri Jul 28 02:38:32 2023, max compression
```

## Comparing `lbTool-1.1.1.tar` & `lbTool-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:18:06.314859 lbTool-1.1.1/
--rw-rw-rw-   0        0        0      129 2023-07-28 02:18:06.313862 lbTool-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 02:18:06.303890 lbTool-1.1.1/lbTool/
--rw-rw-rw-   0        0        0     1234 2023-07-27 08:26:52.000000 lbTool-1.1.1/lbTool/Common.py
--rw-rw-rw-   0        0        0     2981 2023-07-27 01:05:47.000000 lbTool-1.1.1/lbTool/Db.py
--rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbTool-1.1.1/lbTool/EnCipher.py
--rw-rw-rw-   0        0        0     2143 2023-07-26 10:00:46.000000 lbTool-1.1.1/lbTool/FileUtil.py
--rw-rw-rw-   0        0        0      804 2023-07-27 08:09:45.000000 lbTool-1.1.1/lbTool/Logging.py
--rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbTool-1.1.1/lbTool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:18:06.311897 lbTool-1.1.1/lbTool.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-28 02:18:06.000000 lbTool-1.1.1/lbTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-28 02:18:06.000000 lbTool-1.1.1/lbTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 02:18:06.000000 lbTool-1.1.1/lbTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-28 02:18:06.000000 lbTool-1.1.1/lbTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 02:18:06.000000 lbTool-1.1.1/lbTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 02:18:06.314859 lbTool-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      609 2023-07-28 02:17:53.000000 lbTool-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:38:32.112351 lbTool-1.1.2/
+-rw-rw-rw-   0        0        0      214 2023-07-28 02:38:32.111321 lbTool-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-07-28 02:36:43.000000 lbTool-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 02:38:32.101346 lbTool-1.1.2/lbTool/
+-rw-rw-rw-   0        0        0     1234 2023-07-27 08:26:52.000000 lbTool-1.1.2/lbTool/Common.py
+-rw-rw-rw-   0        0        0     2981 2023-07-27 01:05:47.000000 lbTool-1.1.2/lbTool/Db.py
+-rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbTool-1.1.2/lbTool/EnCipher.py
+-rw-rw-rw-   0        0        0     2143 2023-07-26 10:00:46.000000 lbTool-1.1.2/lbTool/FileUtil.py
+-rw-rw-rw-   0        0        0      804 2023-07-27 08:09:45.000000 lbTool-1.1.2/lbTool/Logging.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbTool-1.1.2/lbTool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:38:32.109353 lbTool-1.1.2/lbTool.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-07-28 02:38:32.000000 lbTool-1.1.2/lbTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-28 02:38:32.000000 lbTool-1.1.2/lbTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:38:32.000000 lbTool-1.1.2/lbTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-28 02:38:32.000000 lbTool-1.1.2/lbTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 02:38:32.000000 lbTool-1.1.2/lbTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 02:38:32.112351 lbTool-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-07-28 02:38:19.000000 lbTool-1.1.2/setup.py
```

### Comparing `lbTool-1.1.1/lbTool/Common.py` & `lbTool-1.1.2/lbTool/Common.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.1.1/lbTool/Db.py` & `lbTool-1.1.2/lbTool/Db.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.1.1/lbTool/EnCipher.py` & `lbTool-1.1.2/lbTool/EnCipher.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.1.1/lbTool/FileUtil.py` & `lbTool-1.1.2/lbTool/FileUtil.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.1.1/lbTool/Logging.py` & `lbTool-1.1.2/lbTool/Logging.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.1.1/setup.py` & `lbTool-1.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='lbTool',  # 包的名称
-    version='1.1.1',  # 版本号
+    version='1.1.2',  # 版本号
     author='lb',  # 作者名
     author_email='lcoolb@163.com',
     description='Multifunctional Toolset',  # 包的描述信息
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     packages=find_packages(),  # 包含的所有包
     install_requires=[  # 依赖的其他包
         'gmssl==3.2.2',  # SM4加解密
         'pycryptodome==3.18.0',  # AES加解密
         'pypdf2==3.0.1',  # pdf合并
         'pony==0.7.16',  # orm框架
         'cx-Oracle==8.3.0',
         'comtypes==1.2.0'  # 将word转pdf
     ],
+    python_requires=">=3.6, <3.11"
 )
```

