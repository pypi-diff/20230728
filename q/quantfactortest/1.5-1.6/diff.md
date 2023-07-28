# Comparing `tmp/quantfactortest-1.5.tar.gz` & `tmp/quantfactortest-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfactortest-1.5.tar", last modified: Fri Jul 28 03:08:59 2023, max compression
+gzip compressed data, was "quantfactortest-1.6.tar", last modified: Fri Jul 28 03:14:40 2023, max compression
```

## Comparing `quantfactortest-1.5.tar` & `quantfactortest-1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 03:08:59.093264 quantfactortest-1.5/
--rw-rw-rw-   0        0        0     6701 2023-07-28 03:08:59.092267 quantfactortest-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6109 2023-07-27 03:23:34.000000 quantfactortest-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 03:08:59.091288 quantfactortest-1.5/quantfactortest.egg-info/
--rw-rw-rw-   0        0        0     6701 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    39751 2023-07-28 03:07:37.000000 quantfactortest-1.5/quantfactortest.py
--rw-rw-rw-   0        0        0       42 2023-07-28 03:08:59.093264 quantfactortest-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1371 2023-07-28 03:07:55.000000 quantfactortest-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 03:14:40.003889 quantfactortest-1.6/
+-rw-rw-rw-   0        0        0     6701 2023-07-28 03:14:40.003889 quantfactortest-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6109 2023-07-27 03:23:34.000000 quantfactortest-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 03:14:40.002893 quantfactortest-1.6/quantfactortest.egg-info/
+-rw-rw-rw-   0        0        0     6701 2023-07-28 03:14:39.000000 quantfactortest-1.6/quantfactortest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-28 03:14:39.000000 quantfactortest-1.6/quantfactortest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 03:14:39.000000 quantfactortest-1.6/quantfactortest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-28 03:14:39.000000 quantfactortest-1.6/quantfactortest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 03:14:39.000000 quantfactortest-1.6/quantfactortest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    39743 2023-07-28 03:13:49.000000 quantfactortest-1.6/quantfactortest.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 03:14:40.003889 quantfactortest-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-07-28 03:14:05.000000 quantfactortest-1.6/setup.py
```

### Comparing `quantfactortest-1.5/PKG-INFO` & `quantfactortest-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfactortest
-Version: 1.5
+Version: 1.6
 Summary: 单因子的测试（日级别and分钟级别）,非交互式
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
```

### Comparing `quantfactortest-1.5/README.md` & `quantfactortest-1.6/README.md`

 * *Files identical despite different names*

### Comparing `quantfactortest-1.5/quantfactortest.egg-info/PKG-INFO` & `quantfactortest-1.6/quantfactortest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfactortest
-Version: 1.5
+Version: 1.6
 Summary: 单因子的测试（日级别and分钟级别）,非交互式
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
```

### Comparing `quantfactortest-1.5/quantfactortest.py` & `quantfactortest-1.6/quantfactortest.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         df['策略收益率详情'][1]=Abs_return
         df['策略收益率详情'][2]=sr
         df['策略收益率详情'][3]=maxDrawdown
         df['策略收益率详情'][4]=victory_rate
         print()
         print(df.T)
         fig, ax = plt.subplots(figsize=(30,20))         
-        ax.plot(factor.index.strftime('%Y-%m-%d'), self.group_compound_return, label="复利累计收益率")
+        ax.plot(factor.index.strftime('%Y-%m-%d'), self.group_compound_return, label="Compounded Return")
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/8))
         plt.xlabel("Time",fontsize=20)
         plt.ylabel("Return Rate",fontsize=20)
         self.set_picture()           
         text=str(time_gap)+'days: The Compouned Return of buying '
         for i in buy:
@@ -624,15 +624,15 @@
         df['策略收益率详情'][1]=Abs_return
         df['策略收益率详情'][2]=sr
         df['策略收益率详情'][3]=maxDrawdown
         df['策略收益率详情'][4]=victory_rate
         print()
         print(df.T)
         fig, ax = plt.subplots(figsize=(30,20))         
-        ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return, label="复利累计收益率")
+        ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return, label="Compounded Return")
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/6))
         plt.xlabel("Time",fontsize=20)
         plt.ylabel("Return Rate",fontsize=20)
         self.set_picture()   
         if self.type=='K':        
             text='The Compounded Return of ' +str(time_gap)+'K Line: buy '
```

### Comparing `quantfactortest-1.5/setup.py` & `quantfactortest-1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
  
 setup(
     name='quantfactortest',#包名
-    version='1.5',#版本
+    version='1.6',#版本
     description="单因子的测试（日级别and分钟级别）,非交互式",#包简介
     long_description=open('README.md', encoding='utf-8').read(),#读取文件中介绍包的详细内容
     include_package_data=True,#是否允许上传资源文件
     author='IDEA_Wenzhi',#作者
     author_email='1259429314@qq.com',#作者邮件
     maintainer='IDEA_Wenzhi',#维护者
     maintainer_email='1259429314@qq.com',#维护者邮件
```

