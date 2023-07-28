# Comparing `tmp/histcite-python-0.3.3.tar.gz` & `tmp/histcite-python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.3.3.tar", last modified: Sun Jun 25 01:55:19 2023, max compression
+gzip compressed data, was "histcite-python-0.4.0.tar", last modified: Fri Jul 28 06:44:43 2023, max compression
```

## Comparing `histcite-python-0.3.3.tar` & `histcite-python-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 01:55:10.000000 histcite-python-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-06-25 01:55:19.889989 histcite-python-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-06-25 01:55:10.000000 histcite-python-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/parse_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/recognize_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 01:55:10.000000 histcite-python-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 01:55:19.889989 histcite-python-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-25 01:55:10.000000 histcite-python-0.3.3/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-25 01:55:10.000000 histcite-python-0.3.3/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-25 01:55:10.000000 histcite-python-0.3.3/tests/test_parse_reference.py
+drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.159818 histcite-python-0.4.0/
+-rw-r--r--   0 wang       (501) staff       (20)     1064 2023-07-26 16:29:59.000000 histcite-python-0.4.0/LICENSE
+-rw-r--r--   0 wang       (501) staff       (20)     7868 2023-07-28 06:44:43.159665 histcite-python-0.4.0/PKG-INFO
+-rw-r--r--   0 wang       (501) staff       (20)     7031 2023-07-26 16:29:59.000000 histcite-python-0.4.0/README.md
+drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.157793 histcite-python-0.4.0/histcite/
+-rw-r--r--   0 wang       (501) staff       (20)       21 2023-07-26 16:29:59.000000 histcite-python-0.4.0/histcite/__init__.py
+-rw-r--r--   0 wang       (501) staff       (20)     1828 2023-07-26 16:29:59.000000 histcite-python-0.4.0/histcite/cli.py
+-rw-r--r--   0 wang       (501) staff       (20)     6040 2023-07-28 01:49:03.000000 histcite-python-0.4.0/histcite/compute_metrics.py
+-rw-r--r--   0 wang       (501) staff       (20)     5099 2023-07-28 01:50:03.000000 histcite-python-0.4.0/histcite/network_graph.py
+-rw-r--r--   0 wang       (501) staff       (20)    12536 2023-07-28 00:54:50.000000 histcite-python-0.4.0/histcite/parse_reference.py
+-rw-r--r--   0 wang       (501) staff       (20)    10605 2023-07-28 01:51:59.000000 histcite-python-0.4.0/histcite/process_file.py
+-rw-r--r--   0 wang       (501) staff       (20)     4294 2023-07-28 00:58:03.000000 histcite-python-0.4.0/histcite/recognize_reference.py
+drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.158718 histcite-python-0.4.0/histcite_python.egg-info/
+-rw-r--r--   0 wang       (501) staff       (20)     7868 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 wang       (501) staff       (20)      550 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 wang       (501) staff       (20)        1 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 wang       (501) staff       (20)       47 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 wang       (501) staff       (20)       29 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 wang       (501) staff       (20)        9 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 wang       (501) staff       (20)     1089 2023-07-26 16:29:59.000000 histcite-python-0.4.0/pyproject.toml
+-rw-r--r--   0 wang       (501) staff       (20)       38 2023-07-28 06:44:43.159874 histcite-python-0.4.0/setup.cfg
+drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.159324 histcite-python-0.4.0/tests/
+-rw-r--r--   0 wang       (501) staff       (20)        0 2023-07-28 03:40:33.000000 histcite-python-0.4.0/tests/test_cli.py
+-rw-r--r--   0 wang       (501) staff       (20)     1638 2023-07-26 16:29:59.000000 histcite-python-0.4.0/tests/test_compute_metrics.py
+-rw-r--r--   0 wang       (501) staff       (20)      988 2023-07-26 16:29:59.000000 histcite-python-0.4.0/tests/test_network_graph.py
+-rw-r--r--   0 wang       (501) staff       (20)     1969 2023-07-26 16:29:59.000000 histcite-python-0.4.0/tests/test_parse_reference.py
```

### Comparing `histcite-python-0.3.3/LICENSE` & `histcite-python-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.3/PKG-INFO` & `histcite-python-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,26 @@
-Metadata-Version: 2.1
-Name: histcite-python
-Version: 0.3.3
-Summary: A Python interface for histcite
-Author-email: WangK2 <kw221225@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/doublessay/histcite-python
-Keywords: histcite,citation network,web of science,scopus,cssci
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
+- `v0.4.0` 实现对参考文献信息元的完整解析；
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；  
+- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
 - 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`，Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
+- `GCS`，Global Citation Score， 表示一篇文献在文献数据库中的总被引次数；
 - `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
-- `LCR`， Local Cited References，表示一篇文献所有本地参考文献的数量；
+- `LCR`，Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 工具对比：
 | 对比项 | histcite-python | histcite pro |
@@ -60,83 +40,51 @@
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 
->⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
+⚠️ 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
+⚠️ 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
-| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
-| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
+| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[参看QA1](#qa) |
 
 ```console
-$ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
-$ histcite -f /Users/.../downloads/dataset -t wos -n 100
+$ 假设文件夹路径为/Users/.../Downloads/dataset，来源为web of science, 节点数量设置为100
+$ histcite -f /Users/.../Downloads/dataset -t wos -n 100
 $ 或者是
-$ histcite --folder_path /Users/.../downloads/dataset --source_type wos --node_num 100
+$ histcite --folder_path /Users/.../Downloads/dataset --source_type wos --node_num 100
 ```
->注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
-生成的引文网络图：
+注：生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含 ①描述统计表descriptive_statistics.xlsx, ②引文网络图节点信息表graph_node_info.xlsx, ③引文网络图的数据文件graph.dot 三个文件，③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+
+引文网络图示例：
 
 <img src="examples/graph.svg">
 
-对应的文献节点信息：
+对应的节点信息如下：
+|    | AU                                       | TI                                                   |   PY | SO             |   LCS |
+|------------:|:-----------------------------------------|:-----------------------------------------------------|-----:|:---------------|------:|
+|          55 | 张坤; 查先进                             | 我国智慧图书馆的发展沿革及构建策略研究               | 2021 | 国家图书馆学刊 |     6 |
+|          60 | 石婷婷; 徐建华; 张雨浓                   | 数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计 | 2021 | 情报理论与实践 |     7 |
+|          63 | 卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷 | 智慧图书馆建设标准探析                               | 2021 | 中国图书馆学报 |     9 |
+|          81 | 程焕文; 钟远薪                           | 智慧图书馆的三维解析                                 | 2021 | 图书馆论坛     |    10 |
+|          86 | 段美珍; 初景利; 张冬荣; 解贺嘉           | 智慧图书馆的内涵特点及其认知模型研究                 | 2021 | 图书情报工作   |     7 |
+|         ... |                                      |                                                |      |              |       |
 
-|    | AU            |   PY | SO                                               |   VL |   BP |   LCS |   GCS |
-|------------:|:--------------|-----:|:-------------------------------------------------|-----:|-----:|------:|------:|
-|          31 | Iyer R        | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |    4 |  221 |     5 |    24 |
-|          58 | Iyer RM       | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |    7 |   30 |    10 |    55 |
-|          68 | Iver R        | 1999 | COMPUTER SPEECH AND LANGUAGE                     |   13 |  267 |     7 |    14 |
-|          77 | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |    8 |   76 |     7 |    43 |
-|          82 | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |   88 | 1279 |    15 |   210 |
-
-2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
-
-```python
-import os
-import pandas as pd
-from histcite.process_file import ProcessFile
-from histcite.compute_metrics import ComputeMetrics
-from histcite.network_graph import GraphViz
-
-# 读取数据，解析引文
-folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-source_type = 'wos'
-process = ProcessFile(folder_path, source_type)
-process.concat_table() # 合并多个文件
-process.process_citation() # 识别引文关系
-docs_table = process.docs_table
-reference_table = process.reference_table
-
-# 基本描述统计
-cm = ComputeMetrics(docs_table, reference_table, source_type)
-cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
-
-# 生成引文网络图文件
-graph = GraphViz(docs_table, source_type)
-doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
-graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
-
-# 保存引文网络图文件
-with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
-    f.write(graph_dot_file)
-
-# 保存引文网络图节点文件
-graph_node_file = graph.generate_graph_node_file()
-graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
-```
->注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
+2、函数调用，相比命令行工具会更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+
+3、其他API接口（待更新）
 
 ## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
 | 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
@@ -148,8 +96,8 @@
 答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
 
 3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
 答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
-- [x] 支持 `Scopus` 题录数据
+- [x] 支持 `Scopus` 题录数据
```

### Comparing `histcite-python-0.3.3/README.md` & `histcite-python-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,47 @@
+Metadata-Version: 2.1
+Name: histcite-python
+Version: 0.4.0
+Summary: A Python interface for histcite
+Author-email: WangK2 <kw221225@gmail.com>
+License: MIT
+Project-URL: Home-page, https://github.com/doublessay/histcite-python
+Keywords: histcite,citation network,web of science,scopus,cssci
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
+- `v0.4.0` 实现对参考文献信息元的完整解析；
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；  
+- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
 - 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`，Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
+- `GCS`，Global Citation Score， 表示一篇文献在文献数据库中的总被引次数；
 - `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
-- `LCR`， Local Cited References，表示一篇文献所有本地参考文献的数量；
+- `LCR`，Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 工具对比：
 | 对比项 | histcite-python | histcite pro |
@@ -39,83 +61,51 @@
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 
->⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
+⚠️ 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
+⚠️ 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
-| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
-| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
+| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[参看QA1](#qa) |
 
 ```console
-$ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
-$ histcite -f /Users/.../downloads/dataset -t wos -n 100
+$ 假设文件夹路径为/Users/.../Downloads/dataset，来源为web of science, 节点数量设置为100
+$ histcite -f /Users/.../Downloads/dataset -t wos -n 100
 $ 或者是
-$ histcite --folder_path /Users/.../downloads/dataset --source_type wos --node_num 100
+$ histcite --folder_path /Users/.../Downloads/dataset --source_type wos --node_num 100
 ```
->注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
-生成的引文网络图：
+注：生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含 ①描述统计表descriptive_statistics.xlsx, ②引文网络图节点信息表graph_node_info.xlsx, ③引文网络图的数据文件graph.dot 三个文件，③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+
+引文网络图示例：
 
 <img src="examples/graph.svg">
 
-对应的文献节点信息：
+对应的节点信息如下：
+|    | AU                                       | TI                                                   |   PY | SO             |   LCS |
+|------------:|:-----------------------------------------|:-----------------------------------------------------|-----:|:---------------|------:|
+|          55 | 张坤; 查先进                             | 我国智慧图书馆的发展沿革及构建策略研究               | 2021 | 国家图书馆学刊 |     6 |
+|          60 | 石婷婷; 徐建华; 张雨浓                   | 数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计 | 2021 | 情报理论与实践 |     7 |
+|          63 | 卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷 | 智慧图书馆建设标准探析                               | 2021 | 中国图书馆学报 |     9 |
+|          81 | 程焕文; 钟远薪                           | 智慧图书馆的三维解析                                 | 2021 | 图书馆论坛     |    10 |
+|          86 | 段美珍; 初景利; 张冬荣; 解贺嘉           | 智慧图书馆的内涵特点及其认知模型研究                 | 2021 | 图书情报工作   |     7 |
+|         ... |                                      |                                                |      |              |       |
 
-|    | AU            |   PY | SO                                               |   VL |   BP |   LCS |   GCS |
-|------------:|:--------------|-----:|:-------------------------------------------------|-----:|-----:|------:|------:|
-|          31 | Iyer R        | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |    4 |  221 |     5 |    24 |
-|          58 | Iyer RM       | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |    7 |   30 |    10 |    55 |
-|          68 | Iver R        | 1999 | COMPUTER SPEECH AND LANGUAGE                     |   13 |  267 |     7 |    14 |
-|          77 | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |    8 |   76 |     7 |    43 |
-|          82 | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |   88 | 1279 |    15 |   210 |
-
-2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
-
-```python
-import os
-import pandas as pd
-from histcite.process_file import ProcessFile
-from histcite.compute_metrics import ComputeMetrics
-from histcite.network_graph import GraphViz
-
-# 读取数据，解析引文
-folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-source_type = 'wos'
-process = ProcessFile(folder_path, source_type)
-process.concat_table() # 合并多个文件
-process.process_citation() # 识别引文关系
-docs_table = process.docs_table
-reference_table = process.reference_table
-
-# 基本描述统计
-cm = ComputeMetrics(docs_table, reference_table, source_type)
-cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
-
-# 生成引文网络图文件
-graph = GraphViz(docs_table, source_type)
-doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
-graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
-
-# 保存引文网络图文件
-with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
-    f.write(graph_dot_file)
-
-# 保存引文网络图节点文件
-graph_node_file = graph.generate_graph_node_file()
-graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
-```
->注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
+2、函数调用，相比命令行工具会更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+
+3、其他API接口（待更新）
 
 ## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
 | 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
@@ -127,8 +117,8 @@
 答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
 
 3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
 答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
-- [x] 支持 `Scopus` 题录数据
+- [x] 支持 `Scopus` 题录数据
```

### Comparing `histcite-python-0.3.3/histcite/cli.py` & `histcite-python-0.4.0/histcite/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import os
 import argparse
 from histcite.compute_metrics import ComputeMetrics
 from histcite.process_file import ProcessFile
 from histcite.network_graph import GraphViz
-    
+
+
 def main():
     parser = argparse.ArgumentParser(description='A Python interface for histcite.')
-    parser.add_argument('-f','--folder_path', type=str, required=True, help='folder path of the downloaded files')
-    parser.add_argument('-t','--source_type', type=str, required=True, choices=['wos','cssci','scopus'], help='source type of the downloaded files')
-    parser.add_argument('-n','--node_num', type=int, default=50, help='node number in the citation network graph')
-    parser.add_argument('-g','--graph', action="store_true", help='generate graph file only')
+    parser.add_argument('-f','--folder_path', type=str, required=True, help='Folder path of literature metadata.')
+    parser.add_argument('-t','--source_type', type=str, required=True, choices=['wos','cssci','scopus'], help='Source type of literature metadata.')
+    parser.add_argument('-n','--node_num', type=int, default=50, help='N nodes with the highest LCS.')
+    # parser.add_argument('-g','--graph', action="store_true", help='generate graph file only')
     args = parser.parse_args()
 
     # 将结果存放在用户指定的folder_path下的result文件夹中
-    output_path = os.path.join(args.folder_path,'result')
+    output_path = os.path.join(args.folder_path, 'result')
     if not os.path.exists(output_path):
         os.mkdir(output_path)
     process = ProcessFile(args.folder_path, args.source_type)
-    process.concat_table()
+    process.concat_df()
+    process.process_reference()
     process.process_citation()
-    docs_table = process.docs_table
-    reference_table = process.reference_table
+    reference_df = process.reference_df
+    docs_df = process.docs_df
 
-    if not args.graph:
-        cm = ComputeMetrics(docs_table, reference_table, args.source_type)
-        cm_output_path = os.path.join(output_path,'statistics.xlsx')
-        cm.write2excel(cm_output_path)
-
-    doc_indices = docs_table.sort_values('LCS', ascending=False).index[:args.node_num]
-    graph = GraphViz(docs_table,args.source_type)
+    cm = ComputeMetrics(docs_df, reference_df, args.source_type)
+    cm_output_path = os.path.join(output_path, 'descriptive_statistics.xlsx')
+    cm.write2excel(cm_output_path)
     
+    doc_indices = docs_df.sort_values('LCS', ascending=False).index[:args.node_num]
+    graph = GraphViz(docs_df, args.source_type)
+
     # 生成图文件
     graph_dot_file = graph.generate_dot_file(doc_indices)
-    graph_dot_path = os.path.join(output_path,'graph.dot')
-    with open(graph_dot_path,'w') as f:
+    graph_dot_path = os.path.join(output_path, 'graph.dot')
+    with open(graph_dot_path, 'w') as f:
         f.write(graph_dot_file)
 
     # 生成图节点文件
-    graph._export_graph_node_file(os.path.join(output_path,'graph.node.xlsx'))
+    graph._export_graph_node_file(os.path.join(output_path, 'graph_node_info.xlsx'))
```

### Comparing `histcite-python-0.3.3/histcite/compute_metrics.py` & `histcite-python-0.4.0/histcite/compute_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,135 +1,137 @@
 import os
 import pandas as pd
 
-class ComputeMetrics:
-    """生成统计结果"""
 
-    def __init__(self,docs_table,reference_table,source_type:str):
-        self.docs_table = docs_table
-        self.reference_table = reference_table
+class ComputeMetrics:
+    def __init__(self, docs_df: pd.DataFrame, 
+                 reference_df: pd.DataFrame, 
+                 source_type: str):
+        self.docs_df = docs_df
+        self.reference_df = reference_df
         self.source_type = source_type
 
-    def __generate_table(self,use_cols:list,col:str,split_char=None,str_lower=False)->pd.DataFrame:
-        df = self.docs_table[use_cols]
-        
+    def __generate_df(self, use_cols: list, 
+                      col: str, 
+                      split_char = None, 
+                      str_lower = False, 
+                      sort_field = None) -> pd.DataFrame:
+        df = self.docs_df[use_cols]
         # 如果字段包含多个值，则进行拆分
         if split_char:
             df = df.dropna(subset=[col])
-            df = df.astype({col:'str'})
+            df = df.astype({col: 'str'})
             if str_lower:
-                col_str_lower = df[col].str.lower()
-                df[col] = col_str_lower.str.split(split_char)
-            else:
-                df[col] = df[col].str.split(split_char)
-                
+                df[col] = df[col].str.lower()
+            df[col] = df[col].str.split(split_char)
             df = df.explode(col)
             df = df.reset_index(drop=True)
-        
+
         if 'LCS' in use_cols and 'TC' in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count', 'LCS': 'sum', 'TC': 'sum'})
-            grouped_df = grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS', 'TC': 'TGCS'})
+            grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS', 'TC': 'TGCS'}, inplace=True)
         elif 'LCS' in use_cols and 'TC' not in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count', 'LCS': 'sum'})
             grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS'}, inplace=True)
         elif 'LCS' not in use_cols and 'TC' not in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count'}).rename(columns={col: 'Recs'})
         else:
             raise ValueError('Invalid columns list')
 
         if col == 'Author full names':
-            grouped_df.index = grouped_df.index.str.replace(r'\(\d+\)','',regex=True)
-        return grouped_df.sort_values('Recs', ascending=False)
+            grouped_df.index = grouped_df.index.str.replace(r'\(\d+\)', '', regex=True)
+        
+        if not sort_field:
+            sort_field = 'Recs'
+        return grouped_df.sort_values(sort_field, ascending=False)
 
-    def _generate_author_table(self):
+    def _generate_author_df(self):
         if self.source_type == 'wos':
-            use_cols = ['AU','LCS','TC']
+            use_cols = ['AU', 'LCS', 'TC']
         elif self.source_type == 'cssci':
-            use_cols = ['AU','LCS']
+            use_cols = ['AU', 'LCS']
         elif self.source_type == 'scopus':
-            use_cols = ['Author full names','LCS','TC']
+            use_cols = ['Author full names', 'LCS', 'TC']
         else:
             raise ValueError('Invalid source type')
-        return self.__generate_table(use_cols,use_cols[0],'; ')
-    
-    def _generate_keywords_table(self):
-        if self.source_type in ['wos','scopus']:
-            use_cols = ['DE','LCS','TC']
+        return self.__generate_df(use_cols, use_cols[0], '; ')
+
+    def _generate_keywords_df(self):
+        if self.source_type in ['wos', 'scopus']:
+            use_cols = ['DE', 'LCS', 'TC']
         elif self.source_type == 'cssci':
-            use_cols = ['DE','LCS']
+            use_cols = ['DE', 'LCS']
         else:
             raise ValueError('Invalid source type')
-        return self.__generate_table(use_cols,'DE','; ',True)
-    
-    def _generate_institution_table(self):
-        if self.source_type in ['wos','scopus']:
-            use_cols = ['C3','LCS','TC']
+        return self.__generate_df(use_cols, 'DE', '; ', True)
+
+    def _generate_institution_df(self):
+        if self.source_type in ['wos', 'scopus']:
+            use_cols = ['C3', 'LCS', 'TC']
         elif self.source_type == 'cssci':
-            use_cols = ['C3','LCS']
+            use_cols = ['C3', 'LCS']
         else:
             raise ValueError('Invalid source type')
-        return self.__generate_table(use_cols,'C3','; ')
-    
-    def _generate_records_table(self):
-        """生成文献简表"""
-        if self.source_type in ['wos','scopus']:
-            use_cols = ['AU','TI','SO','PY','LCS','TC','LCR','NR','source file']
+        return self.__generate_df(use_cols, 'C3', '; ')
+
+    def _generate_records_df(self):
+        if self.source_type in ['wos', 'scopus']:
+            use_cols = ['AU', 'TI', 'SO', 'PY', 'TI', 'LCS', 'TC', 'LCR', 'NR', 'source file']
         elif self.source_type == 'cssci':
-            use_cols = ['AU','TI','SO','PY','LCS','LCR','NR','source file']
+            use_cols = ['AU', 'TI', 'SO', 'PY', 'LCS', 'LCR', 'NR', 'source file']
         else:
             raise ValueError('Invalid source type')
-        records_table = self.docs_table[use_cols]
-        if self.source_type in ['wos','scopus']:
-            records_table = records_table.rename(columns={'TC':'GCS','NR':'GCR'})
-        return records_table
-    
-    def _generate_journal_table(self):
-        if self.source_type in ['wos','scopus']:
-            use_cols = ['SO','LCS','TC']
+        records_df = self.docs_df[use_cols]
+        if 'TC' in use_cols:
+            records_df.rename(columns={'TC': 'GCS'}, inplace=True)
+        if 'NR' in use_cols:
+            records_df.rename(columns={'NR':'GCR'}, inplace=True)
+        return records_df
+
+    def _generate_journal_df(self):
+        if self.source_type in ['wos', 'scopus']:
+            use_cols = ['SO', 'LCS', 'TC']
         elif self.source_type == 'cssci':
-            use_cols = ['SO','LCS']
+            use_cols = ['SO', 'LCS']
         else:
             raise ValueError('Invalid source type')
-        return self.__generate_table(use_cols,'SO')
+        return self.__generate_df(use_cols, 'SO')
 
-    def _generate_year_table(self):
+    def _generate_year_df(self):
         use_cols = ['PY']
-        return self.__generate_table(use_cols,'PY')
-    
-    def _generate_document_type_table(self):
+        return self.__generate_df(use_cols, 'PY').sort_values(by='PY')
+
+    def _generate_document_type_df(self):
         use_cols = ['DT']
-        return self.__generate_table(use_cols,'DT')
-   
-    def _generate_reference_table(self):
+        return self.__generate_df(use_cols, 'DT')
+
+    def _generate_reference_df(self):
         """生成参考文献表，按照引用次数降序排列，同时标记是否为本地文献"""
         if self.source_type == 'wos':
-            check_cols = ['PY','J9','VL','BP']
-        elif self.source_type in ['cssci','scopus']:
-            check_cols = ['first_AU','TI']
+            keys = ['First_AU', 'PY', 'J9', 'VL', 'BP', 'DI', 'local']
+        elif self.source_type == 'cssci':
+            keys = ['First_AU', 'TI', 'SO', 'PY', 'VL', 'local']
+        elif self.source_type == 'scopus':
+            keys = ['First_AU', 'TI', 'SO', 'VL', 'BP', 'EP', 'PY', 'local']
         else:
             raise ValueError('Invalid source type')
-        use_cols = self.reference_table.columns.tolist()[:-1]  
-        reference_table = self.reference_table.groupby(use_cols,as_index=False).size()
-        reference_table = reference_table.sort_values(by='size',ascending=False)
-        reference_table = reference_table.rename(columns={'size':'Recs'})
-        common_table = reference_table.reset_index().merge(self.docs_table[check_cols],on=check_cols)
-        reference_table['local'] = 0
-        reference_table.loc[common_table['index'],'local'] = 1
-        return reference_table
-    
-    def write2excel(self,save_path:str):
+        reference_df = self.reference_df.groupby(keys).size().reset_index(name='Recs')
+        reference_df.insert(len(reference_df.columns)-1, 'local', reference_df.pop('local'))
+        return reference_df.sort_values(by='Recs', ascending=False)
+
+    def write2excel(self, save_path: str):
         """将统计结果写入excel"""
         save_folder_path = os.path.dirname(save_path)
         if not os.path.exists(save_folder_path):
             os.makedirs(save_folder_path)
         with pd.ExcelWriter(save_path) as writer:
-            self._generate_records_table().to_excel(writer,sheet_name='Records',index=False)
-            self._generate_author_table().to_excel(writer,sheet_name='Authors')
-            self._generate_journal_table().to_excel(writer,sheet_name='Journals')
-            self._generate_reference_table().to_excel(writer,sheet_name='Cited References',index=False)
-            self._generate_keywords_table().to_excel(writer,sheet_name='Keywords')
-            self._generate_year_table().to_excel(writer,sheet_name='Years')
+            self._generate_records_df().to_excel(writer, sheet_name='Records', index=False)
+            self._generate_author_df().to_excel(writer, sheet_name='Authors')
+            self._generate_journal_df().to_excel(writer, sheet_name='Journals')
+            self._generate_reference_df().to_excel(writer, sheet_name='Cited References', index=False)
+            self._generate_keywords_df().to_excel(writer, sheet_name='Keywords')
+            self._generate_year_df().to_excel(writer, sheet_name='Years')
             
-            if self.source_type in ['wos','cssci']:
-                self._generate_institution_table().to_excel(writer,sheet_name='Institutions')
-            if self.source_type in ['wos','scopus']:
-                self._generate_document_type_table().to_excel(writer,sheet_name='Document Type')
+            if self.source_type in ['wos', 'cssci']:
+                self._generate_institution_df().to_excel(writer, sheet_name='Institutions')
+            if self.source_type in ['wos', 'scopus']:
+                self._generate_document_type_df().to_excel(writer, sheet_name='Document Type')
```

### Comparing `histcite-python-0.3.3/histcite/network_graph.py` & `histcite-python-0.4.0/histcite/network_graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,110 +1,111 @@
+from typing import Literal
 import pandas as pd
 
 class GraphViz:
-
-    def __init__(self,docs_table:pd.DataFrame,source_type:str):
-        self.docs_table = docs_table
+    def __init__(self, docs_df: pd.DataFrame, source_type: str):
+        self.docs_df = docs_df
         self.source_type = source_type
-        self.year_empty_index = set(docs_table[docs_table['PY'].isna()].index)
+        self.empty_year_index = docs_df[docs_df['PY'].isna()].index
 
     def __obtain_groups(self):
         """obtain groups of docs by year"""
-        year_series = self.docs_table.loc[self.node_list,'PY']
+        year_series = self.docs_df.loc[self.node_list, 'PY']
         groups = year_series.groupby(year_series)
         year_list = [i[0] for i in groups]
         grouped_doc_index = [i[1].index.tolist() for i in groups]
         self.year_list = year_list
-        for idx,year in enumerate(year_list):
-            grouped_doc_index[idx].insert(0,year)
+        for idx, year in enumerate(year_list):
+            grouped_doc_index[idx].insert(0, year)
         self.grouped_doc_index = grouped_doc_index
-    
-    def __generate_edge(self,doc_index:int,doc_relation:str,relation_type:str):
-        # filter docs with empty year
-        related_doc_list = [int(i) for i in doc_relation.split(';') if int(i) not in self.year_empty_index]
-        if relation_type=='reference':
-            return {(doc_index,ref) for ref in related_doc_list}
-        elif relation_type=='citation':
-            return {(citation,doc_index) for citation in related_doc_list}
-        
+
+    def __generate_edge(self, doc_index: int, 
+                        doc_relation: str, 
+                        relation_type: Literal['reference', 'citation']) -> set[tuple[int, int]]:
+        related_doc_list = [int(i) for i in doc_relation.split(';') if int(i) not in self.empty_year_index]
+        if relation_type == 'reference':
+            return {(doc_index, ref) for ref in related_doc_list}
+        else:
+            return {(citation, doc_index) for citation in related_doc_list}
+
     def __generate_edge_list(self):
-        min_df = self.docs_table.loc[self.doc_indices,['reference','citation']]
-        edge_set = set()
+        min_df = self.docs_df.loc[self.doc_indices, ['reference', 'citation']]
+        edge_set: set[tuple[int, int]] = set()
         for idx in self.doc_indices:
-            doc_index = idx
-            doc_reference = min_df.loc[idx,'reference']
-            doc_citation = min_df.loc[idx,'citation']
-            if pd.notna(doc_citation):
-                edge_set.update(self.__generate_edge(doc_index, doc_citation, 'citation')) # type:ignore
-            if pd.notna(doc_reference):
-                edge_set.update(self.__generate_edge(doc_index, doc_reference,'reference')) # type: ignore
-        
+            doc_reference = min_df.loc[idx, 'reference']
+            doc_citation = min_df.loc[idx, 'citation']
+            if pd.notna(doc_citation) and isinstance(doc_citation, str):
+                cell_edge_set = self.__generate_edge(idx, doc_citation, 'citation')
+                if cell_edge_set:
+                    edge_set.update(cell_edge_set)
+            if pd.notna(doc_reference) and isinstance(doc_reference, str):
+                cell_edge_set  = self.__generate_edge(idx, doc_reference, 'reference')
+                if cell_edge_set:
+                    edge_set.update(cell_edge_set)
+
         # 过滤索引列表之外的文献
         if not self.allow_external_node:
-            edge_set = [(edge[0],edge[1]) for edge in edge_set if edge[0] in self.doc_indices and edge[1] in self.doc_indices]
-        
+            edge_set = {(edge[0], edge[1]) for edge in edge_set if edge[0] in self.doc_indices and edge[1] in self.doc_indices}
+
         # 根据边生成节点
-        source_node = set([i for i,_ in edge_set])
-        target_node = set([j for _,j in edge_set])
-        node_list = sorted(source_node|target_node)
-        self.node_list = node_list
+        source_node = set([i for i, _ in edge_set])
+        target_node = set([j for _, j in edge_set])
+        node_list = sorted(source_node | target_node)
+        self.node_list: list[int] = node_list
 
-        edge_list = {i:[] for i in sorted(source_node)}
+        edge_list: dict[int, list[int]] = {i: [] for i in sorted(source_node)}
         for edge in edge_set:
             edge_list[edge[0]].append(edge[1])
-
         return edge_list
-        
-    def generate_dot_file(self,doc_indices,allow_external_node=False):
-        """生成dot文件
+
+    def generate_dot_file(self, doc_indices:pd.Index, allow_external_node=False):
+        """
         doc_indices: 文献索引列表\n
         allow_external_node: 是否允许出现doc_indices之外的节点，默认False
         """
-        self.doc_indices = [i for i in doc_indices if i not in self.year_empty_index]
+        self.doc_indices = [i for i in doc_indices if i not in self.empty_year_index]
         self.allow_external_node = allow_external_node
 
         raw_edge_list = self.__generate_edge_list()
         self.__obtain_groups()
-        
+
         dot_edge_list = [f'\t{source} -> '+'{ '+' '.join([str(i) for i in raw_edge_list[source]])+' };\n' for source in raw_edge_list]
         dot_groups = [f'\t{{rank=same; {" ".join([str(i) for i in group_index])}}};\n' for group_index in self.grouped_doc_index]
-        
+
         reverse_year_list = self.year_list[::-1]
-        year_edge_list = [(year,reverse_year_list[idx+1]) for idx,year in enumerate(reverse_year_list) if idx < len(reverse_year_list)-1]
+        year_edge_list = [(year, reverse_year_list[idx+1]) for idx,
+                          year in enumerate(reverse_year_list) if idx < len(reverse_year_list)-1]
         dot_year_node_list = [f'\t{year} [ shape="plaintext" ];\n' for year in self.year_list]
         dot_year_edge_list = [f'\t{edge[0]} -> {edge[1]} [ style = invis ];\n' for edge in year_edge_list]
         dot_text = 'digraph metadata{\n\trankdir = BT;\n'
 
         for dot_group in dot_groups:
             dot_text += dot_group
 
         for dot_year_node in dot_year_node_list:
             dot_text += dot_year_node
-        
+
         for dot_year_edge in dot_year_edge_list:
             dot_text += dot_year_edge
-            
+
         for dot_edge in dot_edge_list:
             dot_text += dot_edge
         dot_text += '}'
         return dot_text
-    
-    def generate_graph_node_file(self)->pd.DataFrame:
+
+    def generate_graph_node_file(self) -> pd.DataFrame:
         # source_type会对节点信息产生影响
         if self.source_type == 'wos':
-            use_cols = ['doc_index','AU','PY','SO','VL','BP','LCS','TC']
+            use_cols = ['doc_index', 'AU', 'TI', 'PY', 'SO', 'LCS', 'TC']
         elif self.source_type == 'cssci':
-            use_cols = ['doc_index','AU','TI','PY','SO','LCS']
+            use_cols = ['doc_index', 'AU', 'TI', 'PY', 'SO', 'LCS']
         elif self.source_type == 'scopus':
-            use_cols = ['doc_index','AU','TI','PY','SO','LCS','TC']
+            use_cols = ['doc_index', 'AU', 'TI', 'PY', 'SO', 'LCS', 'TC']
         else:
             raise ValueError('invalid source type')
-        graph_node_table = self.docs_table.loc[self.node_list,use_cols]
-        
-        try:
-            graph_node_table = graph_node_table.rename(columns={'TC':'GCS'})
-        except KeyError:
-            pass
-        return graph_node_table
-    
-    def _export_graph_node_file(self,file_path:str):
-        self.generate_graph_node_file().to_excel(file_path,index=False)
+        graph_node_df = self.docs_df.loc[self.node_list, use_cols]
+        if 'TC' in graph_node_df.columns:
+            graph_node_df.rename(columns={'TC': 'GCS'}, inplace=True)
+        return graph_node_df
+
+    def _export_graph_node_file(self, file_path: str):
+        self.generate_graph_node_file().to_excel(file_path, index=False)
```

### Comparing `histcite-python-0.3.3/histcite/process_file.py` & `histcite-python-0.4.0/histcite/process_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,221 +1,242 @@
 import os
 import re
 import pandas as pd
+from typing import Literal, Callable
 from histcite.parse_reference import ParseReference
 from histcite.recognize_reference import RecognizeReference
 
+
 class ProcessWosFile:
     @staticmethod
-    def extract_first_author(au_cell:str):
-        return au_cell.split(';',1)[0].replace(',','')
+    def extract_first_author(au_field: pd.Series) -> pd.Series:
+        return au_field.str.split(pat=';',n=1,expand=True)[0].str.replace(',',' ')
+
 
 class ProcessCssciFile:
     @staticmethod
-    def process_org(cell):
-        org_set = set(re.findall(r'](.*?)(?:/|$)',cell))
-        org_list = [i.replace('.','') for i in org_set]
+    def process_org(cell: str) -> str:
+        org_set = set(re.findall(r'](.*?)(?:/|$)', cell))
+        org_list = [i.replace('.', '') for i in org_set]
         return '; '.join(org_list)
 
+
 class ProcessScopusFile:
+    pass
+
+
+class ProcessGeneralFile:
     @staticmethod
-    def extract_first_author(au_field:pd.Series):
-        return au_field.str.split(pat=';',n=1,expand=True)[0]
+    def read_all_file(read_file_func: Callable[[str], pd.DataFrame], file_name_list: list[str]) -> pd.DataFrame:
+        if len(file_name_list) > 1:
+            return pd.concat([read_file_func(file_name) for file_name in file_name_list], ignore_index=True, copy=False)
+        elif len(file_name_list) == 1:
+            return read_file_func(file_name_list[0])
+        else:
+            raise FileNotFoundError('No valid file in the folder')
     
+    @staticmethod
+    def generate_ref_df(cr_series: pd.Series, source_type: Literal['wos', 'cssci', 'scopus']) -> pd.DataFrame:
+        parsed_cr_cells = [ParseReference(doc_index, cell, source_type).parse_cr_cell() for doc_index, cell in cr_series.items()]
+        reference_df = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell], ignore_index=True)
+        return reference_df
+
 class ReadFile:
     @staticmethod
-    def _read_csv(file_path:str,use_cols:list,sep:str=',')->pd.DataFrame:
+    def _read_csv(file_path: str, use_cols: list, sep: str = ',') -> pd.DataFrame:
         try:
             df = pd.read_csv(
                 file_path,
                 sep=sep,
                 header=0,
                 on_bad_lines='skip',
                 usecols=use_cols,
                 dtype_backend="pyarrow")
             return df
         except ValueError:
             file_name = os.path.basename(file_path)
             raise ValueError(f'File {file_name} is not a valid csv file')
-        
-class ProcessFile:
 
-    def __init__(self,folder_path:str,source_type:str):
-        """
-        folder_path: 文件夹路径\n
-        source_type: 数据来源 wos|cssci|scopus
-        """
+
+class ProcessFile:
+    def __init__(self, folder_path: str, source_type: Literal['wos', 'cssci', 'scopus']):
         self.folder_path = folder_path
         self.source_type = source_type
-        if source_type=='wos':
-            self.file_name_list = [i.split('.')[0] for i in os.listdir(folder_path) if i[:9]=='savedrecs']
-        elif source_type=='cssci':
-            self.file_name_list = [i for i in os.listdir(folder_path) if i[:3]=='LY_']
-        elif source_type=='scopus':
-            self.file_name_list = [i.split('.')[0] for i in os.listdir(folder_path) if i[:6]=='scopus']
+        if source_type == 'wos':
+            self.file_name_list = [i.split('.')[0] for i in os.listdir(folder_path) if i[:9] == 'savedrecs']
+        elif source_type == 'cssci':
+            self.file_name_list = [i for i in os.listdir(folder_path) if i[:3] == 'LY_']
+        elif source_type == 'scopus':
+            self.file_name_list = [i.split('.')[0] for i in os.listdir(folder_path) if i[:6] == 'scopus']
         else:
             raise ValueError('Invalid source type')
-        
+
         self.file_name_list.sort()
         if source_type == 'wos':
             self.file_name_list = [i+'.txt' for i in self.file_name_list]
         elif source_type == 'scopus':
             self.file_name_list = [i+'.csv' for i in self.file_name_list]
 
-    def _read_wos_file(self,file_name:str)->pd.DataFrame:
-        """读取wos表单"""
-        use_cols = ['AU','TI','SO','DT','CR','DE','C3','NR','TC','Z9','J9','PY','VL','BP','DI','UT']
-        file_path = os.path.join(self.folder_path,file_name)
-        df = ReadFile._read_csv(file_path,use_cols,'\t')
-        
-        # 转换数据类型
-        df['BP'] = df['BP'].apply(pd.to_numeric,errors='coerce')
-        df['VL'] = df['VL'].apply(pd.to_numeric,errors='coerce')
-        df = df.astype({'BP':'int64[pyarrow]', 'VL':'int64[pyarrow]'})
-        
-        # 提取一作
-        first_au = df['AU'].apply(ProcessWosFile.extract_first_author)
-        df.insert(1,'first_AU',first_au)
+    def _read_wos_file(self, file_name: str) -> pd.DataFrame:
+        use_cols = ['AU', 'TI', 'SO', 'DT', 'CR', 'DE', 'C3',
+                    'NR', 'TC', 'Z9', 'J9', 'PY', 'VL', 'BP', 'DI', 'UT']
+        file_path = os.path.join(self.folder_path, file_name)
+        df = ReadFile._read_csv(file_path, use_cols, '\t')
+        df.insert(1, 'First_AU', ProcessWosFile.extract_first_author(df['AU']))
         df['source file'] = file_name
         return df
-    
-    def _read_cssci_file(self,file_name:str)->pd.DataFrame:
-        """读取cssci文本文件"""
-        file_path = os.path.join(self.folder_path,file_name)
-        with open(file_path,'r') as f:
+
+    def _read_cssci_file(self, file_name: str) -> pd.DataFrame:
+        file_path = os.path.join(self.folder_path, file_name)
+        with open(file_path, 'r') as f:
             text = f.read()
-        
+
         if text[:16] != '南京大学中国社会科学研究评价中心':
             raise ValueError(f'File {file_name} is not a valid cssci file')
-        body_text = text.split('\n\n\n',1)[1]
+        body_text = text.split('\n\n\n', 1)[1]
         contents = {}
-        original_fields = ['来源篇名','来源作者','基    金','期    刊','第一机构','机构名称','第一作者','年代卷期','关 键 词','参考文献']
+        original_fields = ['来源篇名', '来源作者', '基    金', '期    刊', '机构名称', '第一作者', '年代卷期', '关 键 词', '参考文献']
         for field in original_fields:
             if field != '参考文献':
                 field_pattern = f'【{field}】(.*?)\n'
-                contents[field] = re.findall(field_pattern,body_text)
+                contents[field] = re.findall(field_pattern, body_text)
             else:
                 field_pattern = '【参考文献】\n(.*?)\n?'+'-'*5
-                contents[field] = re.findall(field_pattern,body_text,flags=re.S)
-        
+                contents[field] = re.findall(field_pattern, body_text, flags=re.S)
+
         df = pd.DataFrame.from_dict(contents)
-        df.columns = ['TI','AU','FU','SO','first_org','C3','first_AU','PY&VL&BP&EP','DE','CR']
-        df['AU'] = df['AU'].str.replace('/','; ')
-        df['DE'] = df['DE'].str.replace('/','; ')
-        df['PY'] = df['PY&VL&BP&EP'].str.extract(r'^(\d{4}),',expand=False)
+
+        # 重命名列标签
+        column_mapping = {
+            '来源篇名': 'TI',
+            '来源作者': 'AU',
+            '基    金': 'FU',
+            '期    刊': 'SO',
+            '机构名称': 'C3',
+            '第一作者': 'First_AU',
+            '年代卷期': 'PY&VL&BP&EP', 
+            '关 键 词': 'DE',
+            '参考文献': 'CR'}
+        df.rename(columns=column_mapping, inplace=True)
+
+        df['AU'] = df['AU'].str.replace('/', '; ')
+        df['DE'] = df['DE'].str.replace('/', '; ')
+        df['PY'] = df['PY&VL&BP&EP'].str.extract(r'^(\d{4}),', expand=False)
         df['C3'] = df['C3'].apply(ProcessCssciFile.process_org)
-        df['CR'] = df['CR'].str.replace('\n','; ')
+        df['CR'] = df['CR'].str.replace('\n', '; ')
         df['NR'] = df['CR'].str.count('; ')
+        df.insert(2, 'First_AU', df.pop('First_AU'))
         df['source file'] = file_name
         return df
-    
-    def _read_scopus_file(self,file_name:str)->pd.DataFrame:
-        """读取scopus表单"""
-        use_cols = ['Authors','Author full names','Title','Year','Source title','Volume','Issue','Cited by','DOI','Affiliations','Author Keywords','References','Document Type','EID']
-        file_path = os.path.join(self.folder_path,file_name)
-        df = ReadFile._read_csv(file_path,use_cols)
-        df.columns = ['AU','Author full names','TI','PY','SO','VL','IS','TC','DI','C3','DE','CR','DT','EID']
+
+    def _read_scopus_file(self, file_name: str) -> pd.DataFrame:
+        use_cols = ['Authors', 'Author full names', 'Title', 'Year', 'Source title', 'Volume', 'Issue',
+                    'Page start', 'Page end', 'Cited by', 'DOI', 'Author Keywords', 'References', 'Document Type', 'EID']
+        file_path = os.path.join(self.folder_path, file_name)
+        df = ReadFile._read_csv(file_path, use_cols)
+        
+        # 重命名列标签
+        column_mapping = {
+            'Authors': 'AU',
+            'Author full names': 'AF',
+            'Title': 'TI',
+            'Year': 'PY',
+            'Source title': 'SO',
+            'Volume': 'VL',
+            'Issue': 'IS',
+            'Page start': 'BP',
+            'Page end': 'EP',
+            'Cited by': 'TC',
+            'DOI': 'DI',
+            'Author Keywords': 'DE',
+            'References': 'CR',
+            'Document Type': 'DT',
+            }
+        df.rename(columns=column_mapping, inplace=True)
+        
         df['NR'] = df['CR'].str.count('; ')
-        df['first_AU'] = ProcessScopusFile.extract_first_author(df['AU'])
+        df.insert(1, 'First_AU', df['AU'].str.split(pat=';', n=1, expand=True)[0])
         df['source file'] = file_name
         return df
-    
-    def concat_table(self):
-        """合并多个dataframe"""
-        if len(self.file_name_list)>1:
-            if self.source_type=='wos':
-                docs_table = pd.concat([self._read_wos_file(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
-            elif self.source_type=='cssci':
-                docs_table = pd.concat([self._read_cssci_file(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
-            elif self.source_type=='scopus':
-                docs_table = pd.concat([self._read_scopus_file(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
-            else:
-                raise ValueError('Invalid source type')
-        
-        elif len(self.file_name_list)==1:
-            if self.source_type=='wos':
-                docs_table = self._read_wos_file(self.file_name_list[0])
-            elif self.source_type=='cssci':
-                docs_table = self._read_cssci_file(self.file_name_list[0])
-            elif self.source_type=='scopus':
-                docs_table = self._read_scopus_file(self.file_name_list[0])
-            else:
-                raise ValueError('Invalid source type')
-        
+
+    def concat_df(self):
+        """concat multi dataframe and drop duplicate rows"""
+        if self.source_type == 'wos':
+            docs_df = ProcessGeneralFile.read_all_file(self._read_wos_file, self.file_name_list)
+            docs_df['DI'] = docs_df['DI'].str.lower()
+        elif self.source_type == 'cssci':
+            docs_df = ProcessGeneralFile.read_all_file(self._read_cssci_file, self.file_name_list)
+            docs_df['TI'] = docs_df['TI'].str.lower()
+        elif self.source_type == 'scopus':
+            docs_df = ProcessGeneralFile.read_all_file(self._read_scopus_file, self.file_name_list)
+            docs_df['TI'] = docs_df['TI'].str.lower()
         else:
-            raise FileNotFoundError('No valid file in the folder')
-        
-        original_num = docs_table.shape[0]
-        # 删除重复数据
-        if self.source_type=='wos':
-            docs_table.drop_duplicates(subset=['UT'],ignore_index=True,inplace=True) # 根据入藏号删除重复数据
-        elif self.source_type=='cssci':
-            docs_table.drop_duplicates(subset=['TI','first_AU'],ignore_index=True,inplace=True) # 根据题名和一作删除重复数据
-        elif self.source_type=='scopus':
-            docs_table.drop_duplicates(subset=['EID'],ignore_index=True,inplace=True) # 根据eid删除重复数据
-        current_num = docs_table.shape[0]
+            raise ValueError('Invalid source type')
+
+        # drop duplicate rows
+        original_num = docs_df.shape[0]
+        if self.source_type == 'wos':
+            check_cols = ['UT']
+        elif self.source_type == 'cssci':
+            check_cols = ['TI', 'First_AU']
+        elif self.source_type == 'scopus':
+            check_cols = ['EID']
+        else:
+            raise ValueError('Invalid source type')
+        docs_df.drop_duplicates(subset=check_cols, ignore_index=True, inplace=True) 
+        current_num = docs_df.shape[0]
         print(f'共读取 {original_num} 条数据，去重后剩余 {current_num} 条')
-        
-        # 按照年份进行排序
-        # docs_table = docs_table.sort_values(by='PY',ignore_index=True)
-        docs_table.insert(0,'doc_index',docs_table.index)
-
-        # scopus题名转小写
-        if self.source_type == 'scopus':
-            self.TI_COPY = docs_table['TI'].copy()
-            docs_table['TI'] = docs_table['TI'].str.lower()
-        
-        self.docs_table = docs_table
-        return docs_table
-    
-    def __generate_reference_table(self,cr_series:pd.Series):
-        """生成参考文献表格"""
-        if self.source_type=='wos':
-            parsed_cr_cells = [ParseReference(doc_index,cell,'wos').parse_cr_cell() for doc_index,cell in cr_series.items()]
-            reference_table = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell],ignore_index=True)
-            reference_table = reference_table.astype({'PY':'int64[pyarrow]', 'VL':'int64[pyarrow]', 'BP':'int64[pyarrow]'})
-        
-        elif self.source_type=='cssci':
-            parsed_cr_cells = [ParseReference(doc_index,cell,'cssci').parse_cr_cell() for doc_index,cell in cr_series.items()]
-            reference_table = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell],ignore_index=True)
-         
-        elif self.source_type=='scopus':
-            parsed_cr_cells = [ParseReference(doc_index,cell,'scopus').parse_cr_cell() for doc_index,cell in cr_series.items()]
-            reference_table = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell],ignore_index=True)
+        docs_df.insert(0, 'doc_index', docs_df.index)
+        self.docs_df = docs_df
 
+    def process_reference(self):
+        """extract total references and generate dataframe"""
+        cr_series = self.docs_df['CR']
+        if self.source_type == 'wos':
+            reference_df = ProcessGeneralFile.generate_ref_df(cr_series, 'wos')
+            reference_df = reference_df.astype({'PY':'int64[pyarrow]'})
+        elif self.source_type == 'cssci':
+            reference_df = ProcessGeneralFile.generate_ref_df(cr_series, 'cssci')
+            reference_df['TI'] = reference_df['TI'].str.lower()
+        elif self.source_type == 'scopus':
+            reference_df = ProcessGeneralFile.generate_ref_df(cr_series, 'scopus')
+            reference_df['TI'] = reference_df['TI'].str.lower()
         else:
             raise ValueError('Invalid source type')
-        self.reference_table = reference_table
-    
+        # appear duplicate reference in some docs' references
+        reference_df.drop_duplicates(ignore_index=True, inplace=True)
+        reference_df.insert(0, 'ref_index', reference_df.index)
+        reference_df['local'] = 0
+        self.reference_df = reference_df
+
     @staticmethod
-    def __reference2citation(reference_field:pd.Series)->pd.Series:
-        """参考文献转换到引文"""
+    def __reference2citation(reference_field: pd.Series) -> pd.Series:
         citation_field = pd.Series([[] for i in range(len(reference_field))])
         for doc_index, ref_list in reference_field.items():
             if ref_list:
                 for ref_index in ref_list:
                     citation_field[ref_index].append(doc_index)
         return citation_field
-    
+
     def process_citation(self):
-        """处理引文"""
-        self.__generate_reference_table(self.docs_table['CR'])
-        
-        if self.source_type=='wos':
-            reference_field = self.docs_table.apply(lambda row:RecognizeReference.recognize_wos_reference(self.docs_table,self.reference_table,row.name),axis=1)
-        elif self.source_type=='cssci':
-            reference_field = self.docs_table.apply(lambda row:RecognizeReference.recognize_cssci_reference(self.docs_table,self.reference_table,row.name),axis=1)
-        elif self.source_type=='scopus':
-            reference_field = self.docs_table.apply(lambda row:RecognizeReference.recognize_scopus_reference(self.docs_table,self.reference_table,row.name),axis=1)
+        """recognize citation relationship"""
+        if self.source_type == 'wos':
+            reference_field = self.docs_df.apply(lambda row: RecognizeReference.recognize_wos_reference(
+                self.docs_df, self.reference_df, row.name), axis=1)
+        elif self.source_type == 'cssci':
+            reference_field = self.docs_df.apply(lambda row: RecognizeReference.recognize_cssci_reference(
+                self.docs_df, self.reference_df, row.name), axis=1)
+        elif self.source_type == 'scopus':
+            reference_field = self.docs_df.apply(lambda row: RecognizeReference.recognize_scopus_reference(
+                self.docs_df, self.reference_df, row.name), axis=1)
         else:
             raise ValueError('Invalid source type')
-        
+
         citation_field = self.__reference2citation(reference_field)
         lcr_field = reference_field.apply(len)
         lcs_field = citation_field.apply(len)
-        self.docs_table['reference'] = [';'.join([str(j) for j in i]) if i else None for i in reference_field]
-        self.docs_table['citation'] = [';'.join([str(j) for j in i]) if i else None for i in citation_field]
-        self.docs_table['LCR'] = lcr_field
-        self.docs_table['LCS'] = lcs_field
-
-        if self.source_type == 'scopus':
-            self.docs_table['TI'] = self.TI_COPY
+        self.docs_df['reference'] = [
+            ';'.join([str(j) for j in i]) if i else None for i in reference_field]
+        self.docs_df['citation'] = [
+            ';'.join([str(j) for j in i]) if i else None for i in citation_field]
+        self.docs_df['LCR'] = lcr_field
+        self.docs_df['LCS'] = lcs_field
```

### Comparing `histcite-python-0.3.3/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.4.0/histcite_python.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.3.3
+Version: 0.4.0
 Summary: A Python interface for histcite
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/doublessay/histcite-python
+Project-URL: Home-page, https://github.com/doublessay/histcite-python
 Keywords: histcite,citation network,web of science,scopus,cssci
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,30 +17,31 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
+- `v0.4.0` 实现对参考文献信息元的完整解析；
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；  
+- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
 - 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`，Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
+- `GCS`，Global Citation Score， 表示一篇文献在文献数据库中的总被引次数；
 - `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
-- `LCR`， Local Cited References，表示一篇文献所有本地参考文献的数量；
+- `LCR`，Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 工具对比：
 | 对比项 | histcite-python | histcite pro |
@@ -60,83 +61,51 @@
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 
->⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
+⚠️ 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
+⚠️ 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
-| -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
-| -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
+| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[参看QA1](#qa) |
 
 ```console
-$ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
-$ histcite -f /Users/.../downloads/dataset -t wos -n 100
+$ 假设文件夹路径为/Users/.../Downloads/dataset，来源为web of science, 节点数量设置为100
+$ histcite -f /Users/.../Downloads/dataset -t wos -n 100
 $ 或者是
-$ histcite --folder_path /Users/.../downloads/dataset --source_type wos --node_num 100
+$ histcite --folder_path /Users/.../Downloads/dataset --source_type wos --node_num 100
 ```
->注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
-生成的引文网络图：
+注：生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含 ①描述统计表descriptive_statistics.xlsx, ②引文网络图节点信息表graph_node_info.xlsx, ③引文网络图的数据文件graph.dot 三个文件，③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+
+引文网络图示例：
 
 <img src="examples/graph.svg">
 
-对应的文献节点信息：
+对应的节点信息如下：
+|    | AU                                       | TI                                                   |   PY | SO             |   LCS |
+|------------:|:-----------------------------------------|:-----------------------------------------------------|-----:|:---------------|------:|
+|          55 | 张坤; 查先进                             | 我国智慧图书馆的发展沿革及构建策略研究               | 2021 | 国家图书馆学刊 |     6 |
+|          60 | 石婷婷; 徐建华; 张雨浓                   | 数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计 | 2021 | 情报理论与实践 |     7 |
+|          63 | 卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷 | 智慧图书馆建设标准探析                               | 2021 | 中国图书馆学报 |     9 |
+|          81 | 程焕文; 钟远薪                           | 智慧图书馆的三维解析                                 | 2021 | 图书馆论坛     |    10 |
+|          86 | 段美珍; 初景利; 张冬荣; 解贺嘉           | 智慧图书馆的内涵特点及其认知模型研究                 | 2021 | 图书情报工作   |     7 |
+|         ... |                                      |                                                |      |              |       |
 
-|    | AU            |   PY | SO                                               |   VL |   BP |   LCS |   GCS |
-|------------:|:--------------|-----:|:-------------------------------------------------|-----:|-----:|------:|------:|
-|          31 | Iyer R        | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |    4 |  221 |     5 |    24 |
-|          58 | Iyer RM       | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |    7 |   30 |    10 |    55 |
-|          68 | Iver R        | 1999 | COMPUTER SPEECH AND LANGUAGE                     |   13 |  267 |     7 |    14 |
-|          77 | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |    8 |   76 |     7 |    43 |
-|          82 | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |   88 | 1279 |    15 |   210 |
-
-2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
-
-```python
-import os
-import pandas as pd
-from histcite.process_file import ProcessFile
-from histcite.compute_metrics import ComputeMetrics
-from histcite.network_graph import GraphViz
-
-# 读取数据，解析引文
-folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
-source_type = 'wos'
-process = ProcessFile(folder_path, source_type)
-process.concat_table() # 合并多个文件
-process.process_citation() # 识别引文关系
-docs_table = process.docs_table
-reference_table = process.reference_table
-
-# 基本描述统计
-cm = ComputeMetrics(docs_table, reference_table, source_type)
-cm.write2excel(os.path.join(folder_path,'result','statistics.xlsx'))
-
-# 生成引文网络图文件
-graph = GraphViz(docs_table, source_type)
-doc_indices = docs_table.sort_values('LCS', ascending=False).index[:100] # 选取LSC最高的100篇文献
-graph_dot_file = graph.generate_dot_file(doc_indices, allow_external_node=False)
-
-# 保存引文网络图文件
-with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
-    f.write(graph_dot_file)
-
-# 保存引文网络图节点文件
-graph_node_file = graph.generate_graph_node_file()
-graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
-```
->注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
+2、函数调用，相比命令行工具会更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+
+3、其他API接口（待更新）
 
 ## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
 | 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
```

### Comparing `histcite-python-0.3.3/histcite_python.egg-info/SOURCES.txt` & `histcite-python-0.4.0/histcite_python.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 histcite/recognize_reference.py
 histcite_python.egg-info/PKG-INFO
 histcite_python.egg-info/SOURCES.txt
 histcite_python.egg-info/dependency_links.txt
 histcite_python.egg-info/entry_points.txt
 histcite_python.egg-info/requires.txt
 histcite_python.egg-info/top_level.txt
+tests/test_cli.py
 tests/test_compute_metrics.py
 tests/test_network_graph.py
 tests/test_parse_reference.py
```

### Comparing `histcite-python-0.3.3/pyproject.toml` & `histcite-python-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "histcite-python"
 authors = [
     {name = "WangK2", email = "kw221225@gmail.com"}
     ]
 description = "A Python interface for histcite"
-version = "0.3.3"
+version = "0.4.0"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["histcite","citation network","web of science","scopus","cssci"]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -27,14 +27,14 @@
 dependencies = [
     "pandas>=2.0",
     "pyarrow",
     "openpyxl",
     ]
 
 [project.urls]
-Homepage = "https://github.com/doublessay/histcite-python"
+Home-page = "https://github.com/doublessay/histcite-python"
 
 [project.scripts]
 histcite = "histcite.cli:main"
 
 [tool.setuptools]
 packages = ["histcite"]
```

### Comparing `histcite-python-0.3.3/tests/test_compute_metrics.py` & `histcite-python-0.4.0/tests/test_compute_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 @pytest.mark.skip(reason='This is a function factory')
 def test_statistics(docs_table_path,reference_table_path,source_type):
     def new_func():
         docs_table = pd.read_csv(docs_table_path,dtype_backend='pyarrow')
         reference_table = pd.read_csv(reference_table_path,dtype_backend='pyarrow')
 
         cm = ComputeMetrics(docs_table,reference_table,source_type)
-        author_table = cm._generate_author_table()
-        keywords_table = cm._generate_keywords_table()
+        author_table = cm._generate_author_df()
+        keywords_table = cm._generate_keywords_df()
         return author_table,keywords_table
     return new_func
 
 def test_wos_statistics():
     docs_table_path = 'tests/wos_docs_table.csv'
     reference_table_path = 'tests/wos_reference_table.csv'
     author_table,keywords_table = test_statistics(docs_table_path,reference_table_path,'wos')()
@@ -23,14 +23,14 @@
 
 def test_cssci_statistics():
     docs_table_path = 'tests/cssci_docs_table.csv'
     reference_table_path = 'tests/cssci_reference_table.csv'
     author_table,keywords_table = test_statistics(docs_table_path,reference_table_path,'cssci')()
     assert isinstance(author_table.index[0],str)
     assert isinstance(keywords_table.index[0],str)
- 
+
 def test_scopus_statistics():
     docs_table_path = 'tests/scopus_docs_table.csv'
     reference_table_path = 'tests/scopus_reference_table.csv'
     author_table,keywords_table = test_statistics(docs_table_path,reference_table_path,'scopus')()
     assert isinstance(author_table.index[0],str)
     assert isinstance(keywords_table.index[0],str)
```

### Comparing `histcite-python-0.3.3/tests/test_network_graph.py` & `histcite-python-0.4.0/tests/test_network_graph.py`

 * *Files identical despite different names*

