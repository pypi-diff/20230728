# Comparing `tmp/dspawpy-1.0.4.tar.gz` & `tmp/dspawpy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspawpy-1.0.4.tar", last modified: Fri Jul 21 06:14:01 2023, max compression
+gzip compressed data, was "dspawpy-1.0.5.tar", last modified: Fri Jul 28 07:57:40 2023, max compression
```

## Comparing `dspawpy-1.0.4.tar` & `dspawpy-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 06:14:01.609486 dspawpy-1.0.4/
--rw-rw-rw-   0        0        0     7343 2023-07-21 06:14:01.608487 dspawpy-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7090 2023-07-21 06:11:12.000000 dspawpy-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 06:14:01.556490 dspawpy-1.0.4/dspawpy/
--rw-rw-rw-   0        0        0       48 2023-07-21 06:13:56.000000 dspawpy-1.0.4/dspawpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:14:01.577487 dspawpy-1.0.4/dspawpy/analysis/
--rw-rw-rw-   0        0        0        0 2023-07-17 06:41:29.000000 dspawpy-1.0.4/dspawpy/analysis/__init__.py
--rw-rw-rw-   0        0        0    26301 2023-07-18 06:01:24.000000 dspawpy-1.0.4/dspawpy/analysis/aimdtools.py
--rw-rw-rw-   0        0        0    20177 2023-07-17 06:41:28.000000 dspawpy-1.0.4/dspawpy/analysis/vacf.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:14:01.588486 dspawpy-1.0.4/dspawpy/diffusion/
--rw-rw-rw-   0        0        0        0 2023-07-17 06:41:03.000000 dspawpy-1.0.4/dspawpy/diffusion/__init__.py
--rw-rw-rw-   0        0        0     3887 2023-07-17 06:41:30.000000 dspawpy-1.0.4/dspawpy/diffusion/neb.py
--rw-rw-rw-   0        0        0    60226 2023-07-17 06:41:02.000000 dspawpy-1.0.4/dspawpy/diffusion/nebtools.py
--rw-rw-rw-   0        0        0    11045 2023-07-17 06:41:02.000000 dspawpy-1.0.4/dspawpy/diffusion/pathfinder.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:14:01.601487 dspawpy-1.0.4/dspawpy/io/
--rw-rw-rw-   0        0        0        0 2023-07-17 06:41:15.000000 dspawpy-1.0.4/dspawpy/io/__init__.py
--rw-rw-rw-   0        0        0    62596 2023-07-21 06:09:24.000000 dspawpy-1.0.4/dspawpy/io/read.py
--rw-rw-rw-   0        0        0    15397 2023-07-17 06:41:10.000000 dspawpy-1.0.4/dspawpy/io/structure.py
--rw-rw-rw-   0        0        0    34344 2023-07-17 06:41:13.000000 dspawpy-1.0.4/dspawpy/io/utils.py
--rw-rw-rw-   0        0        0    27999 2023-07-17 06:41:13.000000 dspawpy-1.0.4/dspawpy/io/write.py
--rw-rw-rw-   0        0        0    28606 2023-07-19 05:11:35.000000 dspawpy-1.0.4/dspawpy/plot.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:14:01.569489 dspawpy-1.0.4/dspawpy.egg-info/
--rw-rw-rw-   0        0        0     7343 2023-07-21 06:14:01.000000 dspawpy-1.0.4/dspawpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2023-07-21 06:14:01.000000 dspawpy-1.0.4/dspawpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 06:14:01.000000 dspawpy-1.0.4/dspawpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-21 06:14:01.000000 dspawpy-1.0.4/dspawpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 06:14:01.000000 dspawpy-1.0.4/dspawpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 06:14:01.609486 dspawpy-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-07-21 06:13:56.000000 dspawpy-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:14:01.606490 dspawpy-1.0.4/tests/
--rw-rw-rw-   0        0        0      243 2023-07-17 06:41:31.000000 dspawpy-1.0.4/tests/test_from_pdb.py
--rw-rw-rw-   0        0        0      528 2023-07-17 06:41:31.000000 dspawpy-1.0.4/tests/test_write_VESTA.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:57:40.203811 dspawpy-1.0.5/
+-rw-rw-rw-   0        0        0     7592 2023-07-28 07:57:40.201810 dspawpy-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7339 2023-07-27 02:01:47.000000 dspawpy-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 07:57:40.168809 dspawpy-1.0.5/dspawpy/
+-rw-rw-rw-   0        0        0       48 2023-07-28 07:56:21.000000 dspawpy-1.0.5/dspawpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:57:40.181811 dspawpy-1.0.5/dspawpy/analysis/
+-rw-rw-rw-   0        0        0        0 2023-07-17 06:41:29.000000 dspawpy-1.0.5/dspawpy/analysis/__init__.py
+-rw-rw-rw-   0        0        0    26301 2023-07-18 06:01:24.000000 dspawpy-1.0.5/dspawpy/analysis/aimdtools.py
+-rw-rw-rw-   0        0        0    20177 2023-07-17 06:41:28.000000 dspawpy-1.0.5/dspawpy/analysis/vacf.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:57:40.187808 dspawpy-1.0.5/dspawpy/diffusion/
+-rw-rw-rw-   0        0        0        0 2023-07-17 06:41:03.000000 dspawpy-1.0.5/dspawpy/diffusion/__init__.py
+-rw-rw-rw-   0        0        0     3887 2023-07-17 06:41:30.000000 dspawpy-1.0.5/dspawpy/diffusion/neb.py
+-rw-rw-rw-   0        0        0    60226 2023-07-17 06:41:02.000000 dspawpy-1.0.5/dspawpy/diffusion/nebtools.py
+-rw-rw-rw-   0        0        0    11045 2023-07-17 06:41:02.000000 dspawpy-1.0.5/dspawpy/diffusion/pathfinder.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:57:40.196842 dspawpy-1.0.5/dspawpy/io/
+-rw-rw-rw-   0        0        0        0 2023-07-17 06:41:15.000000 dspawpy-1.0.5/dspawpy/io/__init__.py
+-rw-rw-rw-   0        0        0    62596 2023-07-21 06:09:24.000000 dspawpy-1.0.5/dspawpy/io/read.py
+-rw-rw-rw-   0        0        0    15397 2023-07-17 06:41:10.000000 dspawpy-1.0.5/dspawpy/io/structure.py
+-rw-rw-rw-   0        0        0    34344 2023-07-17 06:41:13.000000 dspawpy-1.0.5/dspawpy/io/utils.py
+-rw-rw-rw-   0        0        0    28103 2023-07-24 05:21:22.000000 dspawpy-1.0.5/dspawpy/io/write.py
+-rw-rw-rw-   0        0        0    28606 2023-07-19 05:11:35.000000 dspawpy-1.0.5/dspawpy/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:57:40.175815 dspawpy-1.0.5/dspawpy.egg-info/
+-rw-rw-rw-   0        0        0     7592 2023-07-28 07:57:39.000000 dspawpy-1.0.5/dspawpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2023-07-28 07:57:40.000000 dspawpy-1.0.5/dspawpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 07:57:39.000000 dspawpy-1.0.5/dspawpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-28 07:57:39.000000 dspawpy-1.0.5/dspawpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 07:57:39.000000 dspawpy-1.0.5/dspawpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 07:57:40.203811 dspawpy-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-07-28 07:56:21.000000 dspawpy-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:57:40.199810 dspawpy-1.0.5/tests/
+-rw-rw-rw-   0        0        0      243 2023-07-17 06:41:31.000000 dspawpy-1.0.5/tests/test_from_pdb.py
+-rw-rw-rw-   0        0        0      528 2023-07-17 06:41:31.000000 dspawpy-1.0.5/tests/test_write_VESTA.py
```

### Comparing `dspawpy-1.0.4/PKG-INFO` & `dspawpy-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package) ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
+![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
+![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
+![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # 简介
 
 dspawpy 是 DS-PAW 的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能
 
 ## 安装提示
 
@@ -31,14 +33,18 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 1.0.5
+
+- 功能强化： to_file() 写pdb文件时，结构可以不含晶胞信息
+
 ### 1.0.4
 
 - BUG修复： build_Structures_from_datafile()选择原子序号时上限设置，h5文件里最后一个离子步信息改成尝试读取
 - 功能强化： build_Structures_from_datafile()支持读取pdb格式
 - 细节修改： AIMD读不到PressureKinetic信息时增加相应警告
 
 ### 1.0.3
```

### Comparing `dspawpy-1.0.4/README.md` & `dspawpy-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package) ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
+![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
+![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
+![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # 简介
 
 dspawpy 是 DS-PAW 的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能
 
 ## 安装提示
 
@@ -20,14 +22,18 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 1.0.5
+
+- 功能强化： to_file() 写pdb文件时，结构可以不含晶胞信息
+
 ### 1.0.4
 
 - BUG修复： build_Structures_from_datafile()选择原子序号时上限设置，h5文件里最后一个离子步信息改成尝试读取
 - 功能强化： build_Structures_from_datafile()支持读取pdb格式
 - 细节修改： AIMD读不到PressureKinetic信息时增加相应警告
 
 ### 1.0.3
```

### Comparing `dspawpy-1.0.4/dspawpy/analysis/aimdtools.py` & `dspawpy-1.0.5/dspawpy/analysis/aimdtools.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/analysis/vacf.py` & `dspawpy-1.0.5/dspawpy/analysis/vacf.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/diffusion/neb.py` & `dspawpy-1.0.5/dspawpy/diffusion/neb.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/diffusion/nebtools.py` & `dspawpy-1.0.5/dspawpy/diffusion/nebtools.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/diffusion/pathfinder.py` & `dspawpy-1.0.5/dspawpy/diffusion/pathfinder.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/io/read.py` & `dspawpy-1.0.5/dspawpy/io/read.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/io/structure.py` & `dspawpy-1.0.5/dspawpy/io/structure.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/io/utils.py` & `dspawpy-1.0.5/dspawpy/io/utils.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy/io/write.py` & `dspawpy-1.0.5/dspawpy/io/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,21 +677,23 @@
         warnings.warn("%s already exists and will be overwritten!" % absfile)
     os.makedirs(os.path.dirname(absfile), exist_ok=True)
     with open(absfile, "w", encoding="utf-8") as file:
         for i, s in enumerate(structures):
             file.write("MODEL         %d\n" % (i + 1))
             file.write("REMARK   Converted from Structures\n")
             file.write("REMARK   Converted using dspawpy\n")
-            lengths = s.lattice.lengths
-            angles = s.lattice.angles
-            file.write(
-                "CRYST1{0:9.3f}{1:9.3f}{2:9.3f}{3:7.2f}{4:7.2f}{5:7.2f}\n".format(
-                    lengths[0], lengths[1], lengths[2], angles[0], angles[1], angles[2]
+            # may lack lattice info
+            if hasattr(s, "lattice"):
+                lengths = s.lattice.lengths
+                angles = s.lattice.angles
+                file.write(
+                    "CRYST1{0:9.3f}{1:9.3f}{2:9.3f}{3:7.2f}{4:7.2f}{5:7.2f}\n".format(
+                        lengths[0], lengths[1], lengths[2], angles[0], angles[1], angles[2]
+                    )
                 )
-            )
             for j, site in enumerate(s):
                 file.write(
                     "%4s%7d%4s%5s%6d%4s%8.3f%8.3f%8.3f%6.2f%6.2f%12s\n"
                     % (
                         "ATOM",
                         j + 1,
                         site.species_string,
```

### Comparing `dspawpy-1.0.4/dspawpy/plot.py` & `dspawpy-1.0.5/dspawpy/plot.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/dspawpy.egg-info/PKG-INFO` & `dspawpy-1.0.5/dspawpy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package) ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
+![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
+![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
+![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # 简介
 
 dspawpy 是 DS-PAW 的后处理辅助工具，提供一些数据抓取、换算、结构转化、绘图功能
 
 ## 安装提示
 
@@ -31,14 +33,18 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 1.0.5
+
+- 功能强化： to_file() 写pdb文件时，结构可以不含晶胞信息
+
 ### 1.0.4
 
 - BUG修复： build_Structures_from_datafile()选择原子序号时上限设置，h5文件里最后一个离子步信息改成尝试读取
 - 功能强化： build_Structures_from_datafile()支持读取pdb格式
 - 细节修改： AIMD读不到PressureKinetic信息时增加相应警告
 
 ### 1.0.3
```

### Comparing `dspawpy-1.0.4/dspawpy.egg-info/SOURCES.txt` & `dspawpy-1.0.5/dspawpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.0.4/setup.py` & `dspawpy-1.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         encoding="utf-8",
     ) as fin:
         return fin.read()
 
 
 setup(
     name="dspawpy",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     url="http://www.hzwtech.com/",
     license="MIT",
     author="Hzwtech",
     author_email="ZhengZhilin@hzwtech.com",
     description="Tools for dspaw",
     install_requires=[
```

### Comparing `dspawpy-1.0.4/tests/test_write_VESTA.py` & `dspawpy-1.0.5/tests/test_write_VESTA.py`

 * *Files identical despite different names*

