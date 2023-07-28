# Comparing `tmp/PlistParser-2023.7.21.0.tar.gz` & `tmp/PlistParser-2023.7.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlistParser-2023.7.21.0.tar", last modified: Fri Jul 21 02:10:12 2023, max compression
+gzip compressed data, was "PlistParser-2023.7.28.0.tar", last modified: Fri Jul 28 14:34:35 2023, max compression
```

## Comparing `PlistParser-2023.7.21.0.tar` & `PlistParser-2023.7.28.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 02:10:12.849343 PlistParser-2023.7.21.0/
--rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.21.0/LICENSE.txt
--rw-rw-rw-   0        0        0     7034 2023-07-21 02:10:12.849343 PlistParser-2023.7.21.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 02:10:12.844342 PlistParser-2023.7.21.0/PlistParser/
--rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.21.0/PlistParser/Base64.py
--rw-rw-rw-   0        0        0       47 2023-07-19 15:38:09.000000 PlistParser-2023.7.21.0/PlistParser/Extend.py
--rw-rw-rw-   0        0        0     4431 2023-07-21 02:09:57.000000 PlistParser-2023.7.21.0/PlistParser/Info.py
--rw-rw-rw-   0        0        0    12713 2023-07-19 14:20:41.000000 PlistParser-2023.7.21.0/PlistParser/Plist.py
--rw-rw-rw-   0        0        0    13025 2023-07-19 09:07:22.000000 PlistParser-2023.7.21.0/PlistParser/PlistParser.py
--rw-rw-rw-   0        0        0      181 2023-07-19 14:38:45.000000 PlistParser-2023.7.21.0/PlistParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 02:10:12.848342 PlistParser-2023.7.21.0/PlistParser.egg-info/
--rw-rw-rw-   0        0        0     7034 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-21 02:10:12.000000 PlistParser-2023.7.21.0/PlistParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6330 2023-07-21 02:09:09.000000 PlistParser-2023.7.21.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 02:10:12.850343 PlistParser-2023.7.21.0/setup.cfg
--rw-rw-rw-   0        0        0     2192 2023-07-20 04:41:37.000000 PlistParser-2023.7.21.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:35.502077 PlistParser-2023.7.28.0/
+-rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.28.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     7043 2023-07-28 14:34:35.502077 PlistParser-2023.7.28.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:35.467068 PlistParser-2023.7.28.0/PlistParser/
+-rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.28.0/PlistParser/Base64.py
+-rw-rw-rw-   0        0        0       47 2023-07-19 15:38:09.000000 PlistParser-2023.7.28.0/PlistParser/Extend.py
+-rw-rw-rw-   0        0        0     4431 2023-07-28 14:34:17.000000 PlistParser-2023.7.28.0/PlistParser/Info.py
+-rw-rw-rw-   0        0        0    12713 2023-07-19 14:20:41.000000 PlistParser-2023.7.28.0/PlistParser/Plist.py
+-rw-rw-rw-   0        0        0    13025 2023-07-19 09:07:22.000000 PlistParser-2023.7.28.0/PlistParser/PlistParser.py
+-rw-rw-rw-   0        0        0      181 2023-07-19 14:38:45.000000 PlistParser-2023.7.28.0/PlistParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:34:35.501075 PlistParser-2023.7.28.0/PlistParser.egg-info/
+-rw-rw-rw-   0        0        0     7043 2023-07-28 14:34:35.000000 PlistParser-2023.7.28.0/PlistParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-28 14:34:35.000000 PlistParser-2023.7.28.0/PlistParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 14:34:35.000000 PlistParser-2023.7.28.0/PlistParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-28 14:34:35.000000 PlistParser-2023.7.28.0/PlistParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6339 2023-07-28 13:37:31.000000 PlistParser-2023.7.28.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 14:34:35.502077 PlistParser-2023.7.28.0/setup.cfg
+-rw-rw-rw-   0        0        0     2192 2023-07-20 04:41:37.000000 PlistParser-2023.7.28.0/setup.py
```

### Comparing `PlistParser-2023.7.21.0/LICENSE.txt` & `PlistParser-2023.7.28.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.21.0/PKG-INFO` & `PlistParser-2023.7.28.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.21.0
+Version: 2023.7.28.0
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
@@ -69,38 +69,38 @@
       ```
   * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 为标准
 
 * 🪛🔧 使用方法
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info) 
-    * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
+    * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-info`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
   * 🧑‍💻 关于`API`
     * 相关库导入
       ```python
       from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
       from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
       from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
       from PlistParser import Extend  # .plist 解析器 扩展函数库
       from PlistParser import Info  # .plist 解析器 相关信息
       ```
     * 相关库的`API`(接口)
       * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info)
-      * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
+      * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-info`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 最后
        * Extend.py库 Info.py库
        * `Extend` `Info` 这两个库/包 可以不用管 因为是预留的 哪怕里面有 `内容` `功能` 实现 哪大概率您也用不到
   * 🛠️ 实例
     * 功能实例
       * 解析一个plist文件
         * `pass`
     * 测试实例
-      * 参考项目源码压缩包中的 `PlistParser.test-s` 或 `PlistParser.doc-info` 目录
+      * 参考项目源码压缩包中的 `PlistParser.test-info` 或 `PlistParser.doc-info` 目录
   * 扩展
     * 基础设计扩展
       * `pass`
     * 高级设计扩展
       * `pass`
     * 🔖 本扩展程序皆可 `继承` `重写` 或者 `修改/补充源代码` 等方式实现 功能的扩展等 使该扩展库更符合 `需求`
     * 🔖🔖 好了 最后有问题欢迎 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)  [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)
```

### Comparing `PlistParser-2023.7.21.0/PlistParser/Info.py` & `PlistParser-2023.7.28.0/PlistParser/Info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
-__version__ = '2023.7.21.0'
+__version__ = '2023.7.28.0'
 
 __build_peoples__ = {
     r'white-EelsYikes': '2172989337@qq.com',
 }
 
 __license_body__ = \
     """
```

### Comparing `PlistParser-2023.7.21.0/PlistParser/Plist.py` & `PlistParser-2023.7.28.0/PlistParser/Plist.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.21.0/PlistParser/PlistParser.py` & `PlistParser-2023.7.28.0/PlistParser/PlistParser.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.21.0/PlistParser.egg-info/PKG-INFO` & `PlistParser-2023.7.28.0/PlistParser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.21.0
+Version: 2023.7.28.0
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
@@ -69,38 +69,38 @@
       ```
   * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 为标准
 
 * 🪛🔧 使用方法
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info) 
-    * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
+    * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-info`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
   * 🧑‍💻 关于`API`
     * 相关库导入
       ```python
       from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
       from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
       from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
       from PlistParser import Extend  # .plist 解析器 扩展函数库
       from PlistParser import Info  # .plist 解析器 相关信息
       ```
     * 相关库的`API`(接口)
       * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info)
-      * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
+      * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-info`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 最后
        * Extend.py库 Info.py库
        * `Extend` `Info` 这两个库/包 可以不用管 因为是预留的 哪怕里面有 `内容` `功能` 实现 哪大概率您也用不到
   * 🛠️ 实例
     * 功能实例
       * 解析一个plist文件
         * `pass`
     * 测试实例
-      * 参考项目源码压缩包中的 `PlistParser.test-s` 或 `PlistParser.doc-info` 目录
+      * 参考项目源码压缩包中的 `PlistParser.test-info` 或 `PlistParser.doc-info` 目录
   * 扩展
     * 基础设计扩展
       * `pass`
     * 高级设计扩展
       * `pass`
     * 🔖 本扩展程序皆可 `继承` `重写` 或者 `修改/补充源代码` 等方式实现 功能的扩展等 使该扩展库更符合 `需求`
     * 🔖🔖 好了 最后有问题欢迎 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)  [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)
```

### Comparing `PlistParser-2023.7.21.0/README.md` & `PlistParser-2023.7.28.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,38 +48,38 @@
       ```
   * 🔖 [`PyPi`](https://pypi.org/project/PlistParser/) 与 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 可能存在不同步或者一定差异等情况 主要以 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser) 为标准
 
 * 🪛🔧 使用方法
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info) 
-    * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
+    * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-info`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
   * 🧑‍💻 关于`API`
     * 相关库导入
       ```python
       from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
       from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
       from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
       from PlistParser import Extend  # .plist 解析器 扩展函数库
       from PlistParser import Info  # .plist 解析器 相关信息
       ```
     * 相关库的`API`(接口)
       * [`GitHub 文档集`](https://github.com/whiteEelsYikes/PlistParser/tree/main/PlistParser.doc-info)
-      * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
+      * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-info`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 最后
        * Extend.py库 Info.py库
        * `Extend` `Info` 这两个库/包 可以不用管 因为是预留的 哪怕里面有 `内容` `功能` 实现 哪大概率您也用不到
   * 🛠️ 实例
     * 功能实例
       * 解析一个plist文件
         * `pass`
     * 测试实例
-      * 参考项目源码压缩包中的 `PlistParser.test-s` 或 `PlistParser.doc-info` 目录
+      * 参考项目源码压缩包中的 `PlistParser.test-info` 或 `PlistParser.doc-info` 目录
   * 扩展
     * 基础设计扩展
       * `pass`
     * 高级设计扩展
       * `pass`
     * 🔖 本扩展程序皆可 `继承` `重写` 或者 `修改/补充源代码` 等方式实现 功能的扩展等 使该扩展库更符合 `需求`
     * 🔖🔖 好了 最后有问题欢迎 [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)  [`QQ群`](https://qm.qq.com/cgi-bin/qm/qr?k=8kVUWBck0_zVoOit738kkHSRxW9UU6Ya&jump_from=webapi&authKey=IeeWqgHhgAnLkaeJgKBQxnBG+A7gb0C3ZjKLM2/6tsDzMz2rbuieSNmMaQzI3mo+) 讨论 供电功能和用法  等待您来发掘 (`文档写不动了 太肝了`)
```

### Comparing `PlistParser-2023.7.21.0/setup.py` & `PlistParser-2023.7.28.0/setup.py`

 * *Files identical despite different names*

