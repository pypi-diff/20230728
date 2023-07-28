# Comparing `tmp/hojichar-0.6.1.tar.gz` & `tmp/hojichar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.6.1.tar", max compression
+gzip compressed data, was "hojichar-0.7.0.tar", max compression
```

## Comparing `hojichar-0.6.1.tar` & `hojichar-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-07-27 04:42:29.862017 hojichar-0.6.1/LICENSE
--rw-r--r--   0        0        0    13408 2023-07-27 04:42:29.862017 hojichar-0.6.1/README.md
--rw-r--r--   0        0        0      547 2023-07-27 04:43:03.425428 hojichar-0.6.1/hojichar/__init__.py
--rw-r--r--   0        0        0     3261 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/__main__.py
--rw-r--r--   0        0        0       42 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/core/__init__.py
--rw-r--r--   0        0        0     4331 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/core/composition.py
--rw-r--r--   0        0        0     5269 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     4914 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/core/inspection.py
--rw-r--r--   0        0        0     1087 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    12104 2023-07-27 04:42:29.862017 hojichar-0.6.1/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    23692 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1606 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2530 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0        0 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/py.typed
--rw-r--r--   0        0        0      595 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3380 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1920 2023-07-27 04:42:29.866017 hojichar-0.6.1/hojichar/utils/process.py
--rw-r--r--   0        0        0     1714 2023-07-27 04:43:03.425428 hojichar-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    14141 1970-01-01 00:00:00.000000 hojichar-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-28 04:01:09.966417 hojichar-0.7.0/LICENSE
+-rw-r--r--   0        0        0    13612 2023-07-28 04:01:09.966417 hojichar-0.7.0/README.md
+-rw-r--r--   0        0        0      547 2023-07-28 04:01:32.878969 hojichar-0.7.0/hojichar/__init__.py
+-rw-r--r--   0        0        0     4269 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/cli.py
+-rw-r--r--   0        0        0       42 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     4448 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/composition.py
+-rw-r--r--   0        0        0     5641 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     6221 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/inspection.py
+-rw-r--r--   0        0        0     1087 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    12104 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    23939 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1606 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2530 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0        0 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/py.typed
+-rw-r--r--   0        0        0      595 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3380 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1920 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1746 2023-07-28 04:01:32.874969 hojichar-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    14345 1970-01-01 00:00:00.000000 hojichar-0.7.0/PKG-INFO
```

### Comparing `hojichar-0.6.1/LICENSE` & `hojichar-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/README.md` & `hojichar-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,29 +128,29 @@
   ```bash
   cat <your_text.jsonl> | hojichar -p your_preprocessing_profile.py -o your_text_preprocessed.jsonl
   ```
 
 - `hojichar --help`
 
   ```man
+    usage: hojichar [-h] --profile <profile.py> [--args ARGS [ARGS ...]] [--output OUTPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--all] [--jobs JOBS]
 
     options:
     -h, --help            show this help message and exit
     --profile <profile.py>, -p <profile.py>
                             Path to a Python file that implements your custom filter.
-    --args ARGS [ARGS ...]
+    --args ARGS [ARGS ...]E
                             Pass additional arguments to the profile. Use it like `--args arg1 arg2` etc. The arguments should be space-separated.
     --output OUTPUT, -o OUTPUT
                             Specifies the path for the output file. Defaults to standard output.
     --dump-stats <path to stats.json>
                             Dump statistics to file. If the file exists, it will be appended.
     --exit-on-error       Exit if an exception occurs during filtering. Useful for debugging custom filters.
-    --redirect-stdout REDIRECT_STDOUT
-                            This option is used to redirect standard output to a specified file during the profile. By default, it redirects to /dev/null.
-
+    --all                 A flag that specifies whether to include discarded samples. This is useful when inspecting discarded samples.
+    --jobs JOBS, -j JOBS  The number ob parallel jobs. By default, the nuber of the CPU core.
   ```
 
 ## Definition of Profile
 
 - HojiChar CLI receives a series of preprocessing as a profile.
 - The preprocessing profile is provided as a Python file. Two patterns of the file are allowed.
 - hojichar.utils.load_compose.load_compose() loads these profile.
```

### Comparing `hojichar-0.6.1/hojichar/__init__.py` & `hojichar-0.7.0/hojichar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.6.1"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.7.0"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "utils",
     "Compose",
     "Filter",
```

### Comparing `hojichar-0.6.1/hojichar/core/composition.py` & `hojichar-0.7.0/hojichar/core/composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import pprint
 from typing import Any, List, Optional, Union
 
 import numpy as np
 
 from hojichar.core.filter_interface import Filter, TokenFilter
-from hojichar.core.inspection import Inspector, StatisticsCounter
+from hojichar.core.inspection import Inspector, StatisticsCounter, StatsContainer
 from hojichar.core.models import Document
 
 
 class BeforeProcessFilter(Filter):
     def apply(self, doc: Document) -> Document:
         return doc
 
@@ -93,14 +93,18 @@
         self._statistics.update_changes(document, self.before_process_inspector, self.inspectors)
         return document
 
     @property
     def statistics(self) -> dict:
         return self._statistics.get_statistics()
 
+    @property
+    def statistics_obj(self) -> StatsContainer:
+        return self._statistics.stats
+
     def summary(self, format: str = "print") -> None:
         info = [
             {
                 "layer": i,
                 "name": filt.name,
                 "doc": filt.__doc__,
             }
```

### Comparing `hojichar-0.6.1/hojichar/core/filter_interface.py` & `hojichar-0.7.0/hojichar/core/filter_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,21 @@
     If you apply the filter to tokens, you can use `TokenFilter` class.
 
     Parameters
     ----------
     p: float
         The probability apply the filter organized by hojichar.Compose
     skip_reject: bool
-        If set True, hojichar.Compose make this filter ignore the document
-        which has `is_rejected` flag. By default, set True.
+        If set `True`, `hojichar.Compose` make this filter ignore the document
+        which has `is_rejected` flag.
+        This flag is `True` by default since processing discarded documents
+        in subsequent filters is meaningless. However, in some cases, docs that
+        have been rejected need another filter. For example, analyzing false-positive,
+        discarded docs must be passed to JSON Dump filters. In such case,
+        set the `skip_reject` flag as `False` and make it pass all docs.
     """
 
     def __init__(
         self, p: float = 1, skip_rejected: bool = True, *args: Any, **kwargs: Any
     ) -> None:
         """
         Parameters
```

### Comparing `hojichar-0.6.1/hojichar/core/models.py` & `hojichar-0.7.0/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.7.0/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.7.0/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.7.0/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.7.0/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.7.0/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/filters/__init__.py` & `hojichar-0.7.0/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/filters/deduplication.py` & `hojichar-0.7.0/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/filters/document_filters.py` & `hojichar-0.7.0/hojichar/filters/document_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,17 @@
 
         return document
 
 
 class JSONDumper(Filter):
     """
     Document.text の文字列を json に変換します.
-    必要に応じ Document のメタデータを付与します.
+    必要に応じ Document のメタデータを付与します. これはドキュメントの破棄事由が含まれ、偽陽性の分析に有効です。
+    デフォルトで `skip_rejected` が `False` にセットされており、Document の破棄フラグにかかわらず
+    処理されます。
     """
 
     def __init__(
         self,
         dump_reason: bool = False,
         p: float = 1,
         skip_rejected: bool = False,
```

### Comparing `hojichar-0.6.1/hojichar/filters/token_filters.py` & `hojichar-0.7.0/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/filters/tokenization.py` & `hojichar-0.7.0/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/utils/__init__.py` & `hojichar-0.7.0/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/utils/io_iter.py` & `hojichar-0.7.0/hojichar/utils/io_iter.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/utils/load_compose.py` & `hojichar-0.7.0/hojichar/utils/load_compose.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/hojichar/utils/process.py` & `hojichar-0.7.0/hojichar/utils/process.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.6.1/pyproject.toml` & `hojichar-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.6.1" # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.7.0"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
 
 [tool.poetry.scripts]
-hojichar = "hojichar.__main__:main"
+hojichar = "hojichar.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = ">=1.17.0"
 mmh3 = "^4.0"
 
 [tool.poetry.group.dev]
@@ -68,8 +68,8 @@
 test = "pytest . --doctest-modules && mypy ."
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
-[tool.poetry-dynamic-versioning.substitution]
+[tool.poetry-dynamic-versioning.substitution]
```

### Comparing `hojichar-0.6.1/PKG-INFO` & `hojichar-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.6.1
+Version: 0.7.0
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -148,29 +148,29 @@
   ```bash
   cat <your_text.jsonl> | hojichar -p your_preprocessing_profile.py -o your_text_preprocessed.jsonl
   ```
 
 - `hojichar --help`
 
   ```man
+    usage: hojichar [-h] --profile <profile.py> [--args ARGS [ARGS ...]] [--output OUTPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--all] [--jobs JOBS]
 
     options:
     -h, --help            show this help message and exit
     --profile <profile.py>, -p <profile.py>
                             Path to a Python file that implements your custom filter.
-    --args ARGS [ARGS ...]
+    --args ARGS [ARGS ...]E
                             Pass additional arguments to the profile. Use it like `--args arg1 arg2` etc. The arguments should be space-separated.
     --output OUTPUT, -o OUTPUT
                             Specifies the path for the output file. Defaults to standard output.
     --dump-stats <path to stats.json>
                             Dump statistics to file. If the file exists, it will be appended.
     --exit-on-error       Exit if an exception occurs during filtering. Useful for debugging custom filters.
-    --redirect-stdout REDIRECT_STDOUT
-                            This option is used to redirect standard output to a specified file during the profile. By default, it redirects to /dev/null.
-
+    --all                 A flag that specifies whether to include discarded samples. This is useful when inspecting discarded samples.
+    --jobs JOBS, -j JOBS  The number ob parallel jobs. By default, the nuber of the CPU core.
   ```
 
 ## Definition of Profile
 
 - HojiChar CLI receives a series of preprocessing as a profile.
 - The preprocessing profile is provided as a Python file. Two patterns of the file are allowed.
 - hojichar.utils.load_compose.load_compose() loads these profile.
```

