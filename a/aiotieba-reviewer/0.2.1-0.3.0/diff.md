# Comparing `tmp/aiotieba-reviewer-0.2.1.tar.gz` & `tmp/aiotieba-reviewer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotieba-reviewer-0.2.1.tar", last modified: Wed Jun 14 02:11:46 2023, max compression
+gzip compressed data, was "aiotieba-reviewer-0.3.0.tar", last modified: Fri Jul 28 13:33:56 2023, max compression
```

## Comparing `aiotieba-reviewer-0.2.1.tar` & `aiotieba-reviewer-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.592177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/perf_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/punish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.592177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.596177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/user_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.592177 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 02:11:46.000000 aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/examples/cmd_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/examples/reviewer_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-14 02:11:29.000000 aiotieba-reviewer-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 02:11:46.600177 aiotieba-reviewer-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30242 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/perf_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/punish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/user_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    24429 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/examples/cmd_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/examples/reviewer_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/setup.cfg
```

### Comparing `aiotieba-reviewer-0.2.1/LICENSE` & `aiotieba-reviewer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/PKG-INFO` & `aiotieba-reviewer-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: aiotieba-reviewer
-Version: 0.2.1
+Version: 0.3.0
 Summary: Reviewer Framework based on aiotieba
 Author-email: Starry-OvO <starry.qvq@gmail.com>
 Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
 Project-URL: Documentation, https://review.aiotieba.cc/
 Keywords: baidu,tieba
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,61 +28,61 @@
 + 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
 + 支持针对多条相互关联的内容的审查
 + 支持二维码识别、相似图像查找
 + 支持用户黑白名单、图片黑白名单
 + 使用本地缓存避免重复检测，极大提升性能
 + 优先使用websocket接口，节省带宽
 
-## 安装与更新
+## git安装 (更新较快)
 
-### 安装 (git)
+### 安装
 
 ```shell
 git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
 cd ./aiotieba-reviewer
-pip install .
+pip install -e .
 ```
 
-### 更新 (git)
+### 更新
 
 ```shell
 git pull
 ```
 
-### 安装 (pip)
+## pip安装 (更新较慢)
+
+### 安装
 
 ```shell
 pip install aiotieba-reviewer
 ```
 
-### 更新 (pip)
+### 更新
 
 ```shell
 pip install -U aiotieba-reviewer
 ```
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.06.14更新*
+*2023.07.28更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 5,067,645  |     1,201,056      |    2,613     |   76,863   |
-|     孙笑川     | 4,192,991  |      663,014       |    5,261     |  217,712   |
-|    原神内鬼    |  602,236   |      379,701       |     735      |   28,531   |
-|      憨批      |   23,131   |      155,320       |    4,012     |   71,069   |
-|    lol半价     | 2,087,686  |       64,620       |     201      |   19,142   |
-|    天堂鸡汤    |  364,725   |       13,804       |     100      |   3,870    |
-|     vtuber     |  225,520   |       11,981       |      77      |    916     |
-|      嘉然      |   61,259   |       8,672        |      60      |    832     |
-|    元气骑士    |  274,123   |       4,216        |      44      |    452     |
-| vtuber自由讨论 |   17,232   |        905         |      1       |     7      |
+|    抗压背锅    | 5,158,566  |     1,494,989      |    3,015     |   89,066   |
+|     孙笑川     | 4,370,625  |      601,586       |    4,686     |  189,109   |
+|    原神内鬼    |  613,663   |      408,731       |     765      |   30,952   |
+|      憨批      |   34,574   |      157,889       |    3,902     |   60,238   |
+|    lol半价     | 2,089,892  |       82,061       |     335      |   19,828   |
+|     vtuber     |  226,724   |       12,474       |      79      |   1,063    |
+|    天堂鸡汤    |  372,240   |       10,919       |      77      |   2,326    |
+| vtuber自由讨论 |   17,265   |        994         |      0       |     4      |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.2.1/README.md` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,88 @@
-## 简介
-
-基于[**aiotieba**](https://github.com/Starry-OvO/aiotieba)实现的百度贴吧高弹性吧务审查框架
-
-+ 类型注解全覆盖，方法注释全覆盖，类属性注释全覆盖，内部命名统一
-+ 支持获取用户主页信息（包括个性签名、发帖量、吧龄、成长等级、ip归属地、虚拟形象信息...）、历史发帖、关注吧、关注用户、粉丝列表...
-+ 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
-+ 支持针对多条相互关联的内容的审查
-+ 支持二维码识别、相似图像查找
-+ 支持用户黑白名单、图片黑白名单
-+ 使用本地缓存避免重复检测，极大提升性能
-+ 优先使用websocket接口，节省带宽
-
-## 安装与更新
-
-### 安装 (git)
-
-```shell
-git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
-cd ./aiotieba-reviewer
-pip install .
-```
-
-### 更新 (git)
-
-```shell
-git pull
-```
-
-### 安装 (pip)
-
-```shell
-pip install aiotieba-reviewer
-```
-
-### 更新 (pip)
-
-```shell
-pip install -U aiotieba-reviewer
-```
-
-## 教程
-
-[**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
-
-## 客户名单
-
-*2023.06.14更新*
-
-|      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
-| :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 5,067,645  |     1,201,056      |    2,613     |   76,863   |
-|     孙笑川     | 4,192,991  |      663,014       |    5,261     |  217,712   |
-|    原神内鬼    |  602,236   |      379,701       |     735      |   28,531   |
-|      憨批      |   23,131   |      155,320       |    4,012     |   71,069   |
-|    lol半价     | 2,087,686  |       64,620       |     201      |   19,142   |
-|    天堂鸡汤    |  364,725   |       13,804       |     100      |   3,870    |
-|     vtuber     |  225,520   |       11,981       |      77      |    916     |
-|      嘉然      |   61,259   |       8,672        |      60      |    832     |
-|    元气骑士    |  274,123   |       4,216        |      44      |    452     |
-| vtuber自由讨论 |   17,232   |        905         |      1       |     7      |
-
-## 友情链接
-
-+ [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
-+ [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
-+ [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
+Metadata-Version: 2.1
+Name: aiotieba-reviewer
+Version: 0.3.0
+Summary: Reviewer Framework based on aiotieba
+Author-email: Starry-OvO <starry.qvq@gmail.com>
+Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
+Project-URL: Documentation, https://review.aiotieba.cc/
+Keywords: baidu,tieba
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Session
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## 简介
+
+基于[**aiotieba**](https://github.com/Starry-OvO/aiotieba)实现的百度贴吧高弹性吧务审查框架
+
++ 类型注解全覆盖，方法注释全覆盖，类属性注释全覆盖，内部命名统一
++ 支持获取用户主页信息（包括个性签名、发帖量、吧龄、成长等级、ip归属地、虚拟形象信息...）、历史发帖、关注吧、关注用户、粉丝列表...
++ 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
++ 支持针对多条相互关联的内容的审查
++ 支持二维码识别、相似图像查找
++ 支持用户黑白名单、图片黑白名单
++ 使用本地缓存避免重复检测，极大提升性能
++ 优先使用websocket接口，节省带宽
+
+## git安装 (更新较快)
+
+### 安装
+
+```shell
+git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
+cd ./aiotieba-reviewer
+pip install -e .
+```
+
+### 更新
+
+```shell
+git pull
+```
+
+## pip安装 (更新较慢)
+
+### 安装
+
+```shell
+pip install aiotieba-reviewer
+```
+
+### 更新
+
+```shell
+pip install -U aiotieba-reviewer
+```
+
+## 教程
+
+[**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
+
+## 客户名单
+
+*2023.07.28更新*
+
+|      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
+| :------------: | :--------: | :----------------: | :----------: | :--------: |
+|    抗压背锅    | 5,158,566  |     1,494,989      |    3,015     |   89,066   |
+|     孙笑川     | 4,370,625  |      601,586       |    4,686     |  189,109   |
+|    原神内鬼    |  613,663   |      408,731       |     765      |   30,952   |
+|      憨批      |   34,574   |      157,889       |    3,902     |   60,238   |
+|    lol半价     | 2,089,892  |       82,061       |     335      |   19,828   |
+|     vtuber     |  226,724   |       12,474       |      79      |   1,063    |
+|    天堂鸡汤    |  372,240   |       10,919       |      77      |   2,326    |
+| vtuber自由讨论 |   17,265   |        994         |      0       |     4      |
+
+## 友情链接
+
++ [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
++ [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
++ [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/client.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/database.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import datetime
 import sqlite3
 from pathlib import Path
 from typing import Any, Callable, Final, List, Optional, Tuple, Union
 
 import aiomysql
-from aiotieba import LOG
 from aiotieba.config import CONFIG
+from aiotieba.logging import get_logger as LOG
 from aiotieba.typing import UserInfo
 
 
 def exec_handler_MySQL(create_table_func: Callable, default_ret: Any):
     """
     处理MySQL异常
```

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/imgproc.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/imgproc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple
 
 import cv2 as cv
 import numpy as np
-from aiotieba import LOG
+from aiotieba.logging import get_logger as LOG
 
 from .client import get_db
 
 _qrdetector = None
 _img_hasher = None
```

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/perf_stat.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/perf_stat.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/punish.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/punish.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,29 +12,32 @@
         op (Ops, optional): 删除类型. Defaults to Ops.NORMAL.
         days (int, optional): 封禁天数. Defaults to 0.
         note (str, optional): 处罚理由. Defaults to ''.
     """
 
     __slots__ = [
         'obj',
+        'line',
         'op',
         'day',
-        'trace',
-        'note',
+        '_note',
+        '_raw_note',
     ]
 
     def __init__(self, obj: TypeObj, op: Ops = Ops.NORMAL, day: int = 0, note: str = ''):
         self.obj = obj
         self.op = op
         self.day = day
+        self._note = None
         if op > Ops.NORMAL:
-            line = sys._getframe(1).f_lineno
-            self.note = f"L{line} {note}"
+            self.line = sys._getframe(1).f_lineno
+            self._raw_note = note
         else:
-            self.note = note
+            self.line = 0
+            self._raw_note = ''
 
     def __bool__(self) -> bool:
         if self.op > Ops.NORMAL:
             return True
         if self.day:
             return True
         return False
@@ -50,7 +53,13 @@
 
     def __or__(self, rhs: "Punish") -> "Punish":
         if rhs.day > self.day:
             return rhs
         if rhs.op > self.op:
             return rhs
         return self
+
+    @property
+    def note(self) -> str:
+        if self._note is None:
+            self._note = f"L{self.line} {self._raw_note}"
+        return self._note
```

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/checker.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comment/runner.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/producer.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/comments/runner.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/entry.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import contextlib
 from typing import Generator, List, NoReturn, Optional
 
-from aiotieba import LOG
 from aiotieba.enums import PostSortType
+from aiotieba.logging import get_logger as LOG
 
 from .. import client, executor
 from ..client import get_client
 from ..punish import Punish
 from ..typing import Post, Thread
 from . import comment, post, posts, thread, threads
 
@@ -126,33 +126,25 @@
                 if _comment.pid == pid:
                     comment.checker.set_checker(True, False)(comment.checker.ori_checker)
                     return await comment.checker.checker(_comment)
             LOG().warning("Comment not exist")
 
 
 @contextlib.asynccontextmanager
-async def no_test(use_del_list=False) -> None:
+async def no_test() -> None:
     """
     取消测试模式以实际执行删封
-
-    Args:
-        use_del_list (bool): 是否使用更节省带宽但延迟更高的批量删除模式. Defaults to False.
     """
 
     thread.runner.set_thread_runner(False)(thread.runner.ori_runner)
     threads.runner.set_threads_runner(False)(threads.runner.ori_runner)
 
     try:
-        if use_del_list:
-            async with executor.DeleteList() as del_list:
-                executor.punish_executor = del_list.group_punish_executor
-                yield
-        else:
-            executor.punish_executor = executor.default_punish_executor
-            yield
+        executor.punish_executor = executor.default_punish_executor
+        yield
 
     except Exception:
         import traceback
 
         LOG().critical(traceback.format_exc())
 
     executor.punish_executor = executor.default_punish_executor_test
```

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/checker.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/post/runner.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/producer.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/posts/runner.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/checker.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/thread/runner.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Awaitable, Callable
 
-from aiotieba import LOG
+from aiotieba.logging import get_logger as LOG
 
 from ... import executor
 from ...perf_stat import aperf_stat
 from ...typing import Thread
 from .. import posts
 from . import checker
```

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/producer.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/threads/runner.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from typing import Awaitable, Callable
 
-from aiotieba import LOG
+from aiotieba.logging import get_logger as LOG
 
 from ... import executor
 from ...perf_stat import aperf_stat
 from ..thread import runner as t_runner
 from . import filter, producer
 
 TypeThreadsRunner = Callable[[str, int], Awaitable[None]]
```

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer/reviewer/user_checker.py` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/user_checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/aiotieba_reviewer.egg-info/SOURCES.txt` & `aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.2.1/examples/cmd_handler.py` & `aiotieba-reviewer-0.3.0/examples/cmd_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 import aiotieba as tb
 import async_timeout
 from aiotieba.api.get_ats import At
 from aiotieba.api.get_comments._classdef import Contents_cp
 from aiotieba.api.get_posts._classdef import Contents_p, Contents_pt
 from aiotieba.config import tomllib
+from aiotieba.logging import get_logger as LOG
 
 import aiotieba_reviewer as tbr
 
+tb.logging.enable_filelog()
+
 with open("cmd_handler.toml", 'rb') as file:
     LISTEN_CONFIG = tomllib.load(file)
     FORUMS = {f['fname']: f for f in LISTEN_CONFIG['Forum']}
     del LISTEN_CONFIG['Forum']
 
 
 class TimerRecorder(object):
@@ -212,25 +215,25 @@
     def wrapper(func):
         @functools.wraps(func)
         async def _(self: "Listener", ctx: Context) -> None:
             try:
                 ctx.admin, ctx.admin_db, ctx.speaker = await self.get_admin(ctx.fname)
 
                 await ctx._init()
-                tb.LOG().info(f"user={ctx.user} type={ctx.cmd_type} args={ctx.args} tid={ctx.tid}")
+                LOG().info(f"user={ctx.user} type={ctx.cmd_type} args={ctx.args} tid={ctx.tid}")
 
                 if len(ctx.args) < need_arg_num:
                     raise ValueError("参数量不足")
                 if ctx.permission < need_permission:
                     raise ValueError("权限不足")
 
                 await func(self, ctx)
 
             except Exception as err:
-                tb.LOG().error(err)
+                LOG().error(err)
 
         return _
 
     return wrapper
 
 
 class Listener(object):
@@ -254,21 +257,21 @@
             *[c.__aexit__() for c in itertools.chain.from_iterable(self.admins.values())], self.listener.__aexit__()
         )
 
     async def run(self) -> None:
         while 1:
             try:
                 asyncio.create_task(self.__fetch_and_execute_cmds())
-                tb.LOG().debug('heartbeat')
+                LOG().debug('heartbeat')
                 await asyncio.sleep(4.0)
 
             except asyncio.CancelledError:
                 return
             except Exception:
-                tb.LOG().critical("Unhandled error", exc_info=True)
+                LOG().critical("Unhandled error", exc_info=True)
                 return
 
     async def get_admin(self, fname: str) -> Tuple[tb.Client, tbr.MySQLDB, tb.Client]:
         tup = self.admins.get(fname)
 
         if tup is None:
             cfg = FORUMS.get(fname)
@@ -337,15 +340,15 @@
 
         old_permission, old_note, _ = await ctx.admin_db.get_user_id_full(user_id)
         if old_permission >= ctx.permission:
             raise ValueError("原权限大于等于操作者权限")
         if new_permission >= ctx.permission:
             raise ValueError("新权限大于等于操作者权限")
 
-        tb.LOG().info(f"forum={ctx.fname} user_id={user_id} old_note={old_note}")
+        LOG().info(f"forum={ctx.fname} user_id={user_id} old_note={old_note}")
 
         if new_permission != 0:
             success = await ctx.admin_db.add_user_id(user_id, new_permission, note=note)
         else:
             success = await ctx.admin_db.del_user_id(user_id)
 
         return success
@@ -374,35 +377,35 @@
 
         if _id < 1e11:
             success = await ctx.admin.recover_thread(ctx.fname, _id)
         else:
             success = await ctx.admin.recover_post(ctx.fname, _id)
 
         if success:
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=0)
     async def cmd_hide(self, ctx: Context) -> None:
         """
         hide指令
         屏蔽指令所在主题帖
         """
 
         if await ctx.admin.hide_thread(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=0)
     async def cmd_unhide(self, ctx: Context) -> None:
         """
         unhide指令
         解除指令所在主题帖的屏蔽
         """
 
         if await ctx.admin.unhide_thread(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=1)
     async def cmd_block(self, ctx: Context) -> None:
         """
         block指令
         通过id封禁对应用户10天
         """
@@ -432,27 +435,27 @@
         封禁用户
         """
 
         user = await self.__arg2user_info(ctx.args[0])
         note = ctx.args[1] if len(ctx.args) > 1 else ctx.note
 
         if await ctx.admin.block(ctx.fname, user.portrait, day=day, reason=note):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=1)
     async def cmd_unblock(self, ctx: Context) -> None:
         """
         unblock指令
         通过id解封用户
         """
 
         user = await self.__arg2user_info(ctx.args[0])
 
         if await ctx.admin.unblock(ctx.fname, user.user_id):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=0)
     async def cmd_drop(self, ctx: Context) -> None:
         """
         drop指令
         删帖并封10天
         """
@@ -482,36 +485,36 @@
         封禁用户并删除父级
         """
 
         await ctx.init_full()
 
         note = ctx.args[0] if len(ctx.args) > 0 else ctx.note
 
-        tb.LOG().info(f"Try to del {ctx.parent.__class__.__name__}. parent={ctx.parent} user_id={ctx.parent.author_id}")
+        LOG().info(f"Try to del {ctx.parent.__class__.__name__}. parent={ctx.parent} user_id={ctx.parent.author_id}")
 
         if ctx.at.is_thread:
             if ctx.fname != ctx.parent.fname:
                 raise ValueError("被转发帖不来自同一个吧")
             if ctx.parent.author_id == 0:
                 raise ValueError("无法获取被转发帖的作者信息")
 
-        await ctx.admin.del_post(ctx.parent.fid, ctx.parent.pid)
-        await ctx.admin.del_post(ctx.fname, ctx.pid)
+        await ctx.admin.del_post(ctx.parent.fid, ctx.parent.tid, ctx.parent.pid)
+        await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
         if day:
             await ctx.admin.block(ctx.parent.fid, ctx.parent.author_id, day=day, reason=note)
 
     @check_and_log(need_permission=1, need_arg_num=0)
     async def cmd_recommend(self, ctx: Context) -> None:
         """
         recommend指令
         对指令所在主题帖执行“大吧主首页推荐”操作
         """
 
         if await ctx.admin.recommend(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=1)
     async def cmd_move(self, ctx: Context) -> None:
         """
         move指令
         将指令所在主题帖移动至名为tab_name的分区
         """
@@ -522,93 +525,93 @@
         from_tab_id = 0
         for thread in threads:
             if thread.tid == ctx.tid:
                 from_tab_id = thread.tab_id
         to_tab_id = threads.tab_map.get(ctx.args[0], 0)
 
         if await ctx.admin.move(ctx.fname, ctx.tid, to_tab_id=to_tab_id, from_tab_id=from_tab_id):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=0)
     async def cmd_good(self, ctx: Context) -> None:
         """
         good指令
         将指令所在主题帖加到以cname为名的精华分区。cname默认为''即不分区
         """
 
         cname = ctx.args[0] if len(ctx.args) else ''
 
         if await ctx.admin.good(ctx.fname, ctx.tid, cname=cname):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=2, need_arg_num=0)
     async def cmd_ungood(self, ctx: Context) -> None:
         """
         ungood指令
         撤销指令所在主题帖的精华
         """
 
         if await ctx.admin.ungood(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=4, need_arg_num=0)
     async def cmd_top(self, ctx: Context) -> None:
         """
         top指令
         置顶指令所在主题帖
         """
 
         if await ctx.admin.top(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=4, need_arg_num=0)
     async def cmd_untop(self, ctx: Context) -> None:
         """
         untop指令
         撤销指令所在主题帖的置顶
         """
 
         if await ctx.admin.untop(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=4, need_arg_num=1)
     async def cmd_black(self, ctx: Context) -> None:
         """
         black指令
         将id加入脚本黑名单
         """
 
         note = ctx.args[1] if len(ctx.args) > 1 else ctx.note
 
         if await self.__cmd_set(ctx, -5, note):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=3, need_arg_num=1)
     async def cmd_white(self, ctx: Context) -> None:
         """
         white指令
         将id加入脚本白名单
         """
 
         note = ctx.args[1] if len(ctx.args) > 1 else ctx.note
 
         if await self.__cmd_set(ctx, 1, note):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=3, need_arg_num=1)
     async def cmd_reset(self, ctx: Context) -> None:
         """
         reset指令
         将id移出脚本名单
         """
 
         note = ctx.args[1] if len(ctx.args) > 1 else ctx.note
 
         if await self.__cmd_set(ctx, 0, note):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=4, need_arg_num=0)
     async def cmd_exdrop(self, ctx: Context) -> None:
         """
         exdrop指令
         删帖并将发帖人加入脚本黑名单+封禁十天
         """
@@ -628,37 +631,33 @@
 
         await self.__cmd_drop(ctx, 10)
 
         note = ctx.args[0] if len(ctx.args) > 0 else ctx.note
         user_id = ctx.parent.author_id
         await self.__cmd_set(ctx, -5, note, user_id=user_id)
 
-        pids = []
         for pn in range(1, 0xFFFF):
             threads = await ctx.admin.get_user_threads(user_id, pn)
-            pids += [thread.pid for thread in threads if thread.fname == ctx.fname]
-            if len(threads) < 60:
-                break
-
-        step = 30
-        for i in range(0, len(pids) % 30, 30):
-            await ctx.admin.del_posts(ctx.fname, pids[i : i + step])
+            for thread in threads:
+                if thread.fname != ctx.fname:
+                    continue
+                await ctx.admin.del_post(thread.fid, thread.tid, thread.pid)
 
     @check_and_log(need_permission=4, need_arg_num=2)
     async def cmd_set(self, ctx: Context) -> None:
         """
         set指令
         设置用户的权限级别
         """
 
         new_permission = int(ctx.args[1])
         note = ctx.args[2] if len(ctx.args) > 2 else ctx.note
 
         if await self.__cmd_set(ctx, new_permission, note):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=0, need_arg_num=1)
     async def cmd_get(self, ctx: Context) -> None:
         """
         get指令
         获取用户的个人信息与标记信息
         """
@@ -668,15 +667,15 @@
 
         user = await self.__arg2user_info(ctx.args[0])
 
         permission, note, record_time = await ctx.admin_db.get_user_id_full(user.user_id)
         msg_content = f"""user_name: {user.user_name}\nuser_id: {user.user_id}\nportrait: {user.portrait}\npermission: {permission}\nnote: {note}\nrecord_time: {record_time.strftime("%Y-%m-%d %H:%M:%S")}"""
 
         if await ctx.speaker.send_msg(ctx.user.user_id, msg_content):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=4, need_arg_num=2)
     async def cmd_img_set(self, ctx: Context) -> None:
         """
         img_set指令
         设置图片的封锁级别
         """
@@ -699,15 +698,15 @@
                 continue
             img_hash = tbr.imgproc.compute_imghash(image)
             if img_hash == 4412820541203793671:
                 continue
 
             await ctx.admin_db.add_imghash(img_hash, img.hash, permission=permission, note=note)
 
-        await ctx.admin.del_post(ctx.fname, ctx.pid)
+        await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=3, need_arg_num=0)
     async def cmd_img_reset(self, ctx: Context) -> None:
         """
         img_reset指令
         重置图片的封锁级别
         """
@@ -723,15 +722,15 @@
             image = await self.listener.get_image(img.src)
             if image is None:
                 continue
             img_hash = tbr.imgproc.compute_imghash(image)
 
             await ctx.admin_db.del_imghash(img_hash)
 
-        await ctx.admin.del_post(ctx.fname, ctx.pid)
+        await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=1, need_arg_num=0)
     async def cmd_recom_status(self, ctx: Context) -> None:
         """
         recom_status指令
         获取大吧主推荐功能的月度配额状态
         """
@@ -740,48 +739,48 @@
             raise ValueError("speaker尚未冷却完毕")
 
         status = await ctx.admin.get_recom_status(ctx.fname)
         percent = status.used_recom_num / status.total_recom_num * 100
         content = f"Used: {status.used_recom_num} / {status.total_recom_num} = {percent:.2f}%"
 
         if await ctx.speaker.send_msg(ctx.user.user_id, content):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=4, need_arg_num=1)
     async def cmd_tb_black(self, ctx: Context) -> None:
         """
         tb_black指令
         将id加入贴吧黑名单
         """
 
         user = await self.__arg2user_info(ctx.args[0])
 
-        if await ctx.admin.blacklist_add(ctx.fname, user.user_id):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+        if await ctx.admin.add_bawu_blacklist(ctx.fname, user.user_id):
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=3, need_arg_num=1)
     async def cmd_tb_reset(self, ctx: Context) -> None:
         """
         tb_reset指令
         将id移出贴吧黑名单
         """
 
         user = await self.__arg2user_info(ctx.args[0])
 
-        if await ctx.admin.blacklist_del(ctx.fname, user.user_id):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
+        if await ctx.admin.del_bawu_blacklist(ctx.fname, user.user_id):
+            await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=1, need_arg_num=0)
     async def cmd_ping(self, ctx: Context) -> None:
         """
         ping指令
         用于测试bot可用性的空指令
         """
 
-        await ctx.admin.del_post(ctx.fname, ctx.pid)
+        await ctx.admin.del_post(ctx.fname, ctx.tid, ctx.pid)
 
     @check_and_log(need_permission=129, need_arg_num=65536)
     async def cmd_default(self, _: Context) -> None:
         """
         default指令
         """
```

### Comparing `aiotieba-reviewer-0.2.1/examples/reviewer_example.py` & `aiotieba-reviewer-0.3.0/examples/reviewer_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import asyncio
 import re
 from typing import List, Optional, Tuple
 
 import aiotieba as tb
-from aiotieba.api.get_homepage import Thread_home, UserInfo_home
+from aiotieba.api.profile import Thread_pf, UserInfo_pf
 from aiotieba.typing import Comment, Post, Thread
 from cacheout import Cache
 
 import aiotieba_reviewer as tbr
 from aiotieba_reviewer import Ops, Punish, TypeObj, imgproc
 
 sign_check_exp = re.compile(r'企鹅|扣扣', re.I)
@@ -22,16 +22,16 @@
     if pimg.size and imgproc.has_QRcode(pimg):
         return True
     return False
 
 
 # 同理 缓存返回的结果
 @Cache(maxsize=64).memoize()
-async def get_homepage(client: tb.Client, portrait: str) -> Tuple[UserInfo_home, List[Thread_home]]:
-    return await client.get_homepage(portrait, with_threads=True)
+async def get_homepage(client: tb.Client, user_id: int) -> Tuple[UserInfo_pf, List[Thread_pf]]:
+    return await client.get_homepage(user_id)
 
 
 # 使用装饰器将以下函数设置为针对主题帖的checker
 @tbr.reviewer.thread.set_checker()
 async def check_thread(thread: Thread) -> Optional[Punish]:
     # 水经验
     if thread.is_help:
@@ -50,15 +50,15 @@
 
     client = await tbr.get_client()
 
     # 老用户提早返回 跳过后续检查
     if user.level >= 4 or user.glevel >= 4 or user.priv_like == 3:
         return
 
-    hpuser, hpthreads = await get_homepage(client, user.portrait)
+    hpuser, hpthreads = await get_homepage(client, user.user_id)
 
     # 用户个性签名是否包含违规内容
     if sign_check_exp.search(hpuser.sign):
         return Punish(thread, Ops.DELETE, 10, note="麦片sig")
 
     # 头像是否包含二维码
     if await portrait_hasQR(client, user.portrait):
```

### Comparing `aiotieba-reviewer-0.2.1/pyproject.toml` & `aiotieba-reviewer-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
-urls = { Repository = "https://github.com/Starry-OvO/aiotieba-reviewer/", Documentation = "https://review.aiotieba.cc/" }
 name = "aiotieba-reviewer"
 description = "Reviewer Framework based on aiotieba"
-readme = "README.md"
-requires-python = ">=3.8"
 authors = [{ name = "Starry-OvO", email = "starry.qvq@gmail.com" }]
+urls = { Repository = "https://github.com/Starry-OvO/aiotieba-reviewer/", Documentation = "https://review.aiotieba.cc/" }
+readme = "README.md"
 keywords = ["baidu", "tieba"]
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: The Unlicense (Unlicense)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
-dependencies = ["aiotieba[img,speedup]<4.0,>=3.4.0", "aiomysql<0.3,>=0.1.0"]
+requires-python = ">=3.8"
+dependencies = ["aiotieba[img,speedup]<4.0,>=3.6.0", "aiomysql<0.3,>=0.1.0"]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.dynamic]
 version = { attr = "aiotieba_reviewer.__version__.__version__" }
```

