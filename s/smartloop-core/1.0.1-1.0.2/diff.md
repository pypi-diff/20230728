# Comparing `tmp/smartloop-core-1.0.1.tar.gz` & `tmp/smartloop-core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartloop-core-1.0.1.tar", last modified: Fri Jul 28 21:30:19 2023, max compression
+gzip compressed data, was "smartloop-core-1.0.2.tar", last modified: Fri Jul 28 21:34:48 2023, max compression
```

## Comparing `smartloop-core-1.0.1.tar` & `smartloop-core-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.954938 smartloop-core-1.0.1/
--rw-r--r--   0 mehfuz     (501) staff       (20)     1065 2023-06-20 05:48:15.000000 smartloop-core-1.0.1/LICENSE.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)       24 2022-06-27 05:07:42.000000 smartloop-core-1.0.1/MANIFEST.in
--rw-r--r--   0 mehfuz     (501) staff       (20)      643 2023-07-28 21:30:19.954986 smartloop-core-1.0.1/PKG-INFO
--rw-r--r--   0 mehfuz     (501) staff       (20)     4704 2023-07-28 18:42:15.000000 smartloop-core-1.0.1/README.md
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.950973 smartloop-core-1.0.1/data/
--rw-r--r--   0 mehfuz     (501) staff       (20)    19738 2023-07-20 21:20:54.000000 smartloop-core-1.0.1/data/sample.json
--rw-r--r--   0 mehfuz     (501) staff       (20)       79 2023-07-28 21:30:19.955146 smartloop-core-1.0.1/setup.cfg
--rw-r--r--   0 mehfuz     (501) staff       (20)     1115 2023-07-28 21:27:02.000000 smartloop-core-1.0.1/setup.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.953402 smartloop-core-1.0.1/sl_core/
--rw-r--r--   0 mehfuz     (501) staff       (20)      344 2023-01-06 20:04:52.000000 smartloop-core-1.0.1/sl_core/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      171 2022-06-27 05:07:42.000000 smartloop-core-1.0.1/sl_core/classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      387 2023-01-06 20:04:52.000000 smartloop-core-1.0.1/sl_core/config.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      109 2022-06-01 06:34:59.000000 smartloop-core-1.0.1/sl_core/default_config.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.953618 smartloop-core-1.0.1/sl_core/errors/
--rw-r--r--   0 mehfuz     (501) staff       (20)       41 2022-08-05 16:36:45.000000 smartloop-core-1.0.1/sl_core/errors/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)       69 2022-08-05 16:36:45.000000 smartloop-core-1.0.1/sl_core/errors/mode_not_found.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      229 2022-06-01 06:34:59.000000 smartloop-core-1.0.1/sl_core/file_config.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      904 2022-08-25 21:26:36.000000 smartloop-core-1.0.1/sl_core/label_parser.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1428 2023-05-03 01:19:44.000000 smartloop-core-1.0.1/sl_core/model_loader.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.953734 smartloop-core-1.0.1/sl_core/nlu/
--rw-r--r--   0 mehfuz     (501) staff       (20)       47 2022-06-01 06:34:59.000000 smartloop-core-1.0.1/sl_core/nlu/__init__.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.953988 smartloop-core-1.0.1/sl_core/nlu/callbacks/
--rw-r--r--   0 mehfuz     (501) staff       (20)       51 2022-06-27 05:07:42.000000 smartloop-core-1.0.1/sl_core/nlu/callbacks/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1217 2022-06-27 05:07:42.000000 smartloop-core-1.0.1/sl_core/nlu/callbacks/train_status_report.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.954224 smartloop-core-1.0.1/sl_core/nlu/classifiers/
--rw-r--r--   0 mehfuz     (501) staff       (20)       67 2022-06-27 05:07:42.000000 smartloop-core-1.0.1/sl_core/nlu/classifiers/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     6787 2023-06-01 05:48:29.000000 smartloop-core-1.0.1/sl_core/nlu/classifiers/embedding_intent_classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1819 2023-05-02 05:20:47.000000 smartloop-core-1.0.1/sl_core/project.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      723 2023-01-06 20:04:52.000000 smartloop-core-1.0.1/sl_core/sanitizer.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1593 2023-05-03 01:09:11.000000 smartloop-core-1.0.1/sl_core/text_classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      627 2023-01-06 20:04:52.000000 smartloop-core-1.0.1/sl_core/tokenizer.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:30:19.954855 smartloop-core-1.0.1/smartloop_core.egg-info/
--rw-r--r--   0 mehfuz     (501) staff       (20)      643 2023-07-28 21:30:19.000000 smartloop-core-1.0.1/smartloop_core.egg-info/PKG-INFO
--rw-r--r--   0 mehfuz     (501) staff       (20)      757 2023-07-28 21:30:19.000000 smartloop-core-1.0.1/smartloop_core.egg-info/SOURCES.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)        1 2023-07-28 21:30:19.000000 smartloop-core-1.0.1/smartloop_core.egg-info/dependency_links.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)       56 2023-07-28 21:30:19.000000 smartloop-core-1.0.1/smartloop_core.egg-info/requires.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)        8 2023-07-28 21:30:19.000000 smartloop-core-1.0.1/smartloop_core.egg-info/top_level.txt
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.286527 smartloop-core-1.0.2/
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1065 2023-06-20 05:48:15.000000 smartloop-core-1.0.2/LICENSE.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       24 2022-06-27 05:07:42.000000 smartloop-core-1.0.2/MANIFEST.in
+-rw-r--r--   0 mehfuz     (501) staff       (20)     5398 2023-07-28 21:34:48.286579 smartloop-core-1.0.2/PKG-INFO
+-rw-r--r--   0 mehfuz     (501) staff       (20)     4704 2023-07-28 18:42:15.000000 smartloop-core-1.0.2/README.md
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.284052 smartloop-core-1.0.2/data/
+-rw-r--r--   0 mehfuz     (501) staff       (20)    19738 2023-07-20 21:20:54.000000 smartloop-core-1.0.2/data/sample.json
+-rw-r--r--   0 mehfuz     (501) staff       (20)       79 2023-07-28 21:34:48.286752 smartloop-core-1.0.2/setup.cfg
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1344 2023-07-28 21:34:38.000000 smartloop-core-1.0.2/setup.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.285218 smartloop-core-1.0.2/sl_core/
+-rw-r--r--   0 mehfuz     (501) staff       (20)      344 2023-01-06 20:04:52.000000 smartloop-core-1.0.2/sl_core/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      171 2022-06-27 05:07:42.000000 smartloop-core-1.0.2/sl_core/classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      387 2023-01-06 20:04:52.000000 smartloop-core-1.0.2/sl_core/config.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      109 2022-06-01 06:34:59.000000 smartloop-core-1.0.2/sl_core/default_config.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.285440 smartloop-core-1.0.2/sl_core/errors/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       41 2022-08-05 16:36:45.000000 smartloop-core-1.0.2/sl_core/errors/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)       69 2022-08-05 16:36:45.000000 smartloop-core-1.0.2/sl_core/errors/mode_not_found.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      229 2022-06-01 06:34:59.000000 smartloop-core-1.0.2/sl_core/file_config.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      904 2022-08-25 21:26:36.000000 smartloop-core-1.0.2/sl_core/label_parser.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1428 2023-05-03 01:19:44.000000 smartloop-core-1.0.2/sl_core/model_loader.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.285557 smartloop-core-1.0.2/sl_core/nlu/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       47 2022-06-01 06:34:59.000000 smartloop-core-1.0.2/sl_core/nlu/__init__.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.285785 smartloop-core-1.0.2/sl_core/nlu/callbacks/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       51 2022-06-27 05:07:42.000000 smartloop-core-1.0.2/sl_core/nlu/callbacks/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1217 2022-06-27 05:07:42.000000 smartloop-core-1.0.2/sl_core/nlu/callbacks/train_status_report.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.285961 smartloop-core-1.0.2/sl_core/nlu/classifiers/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       67 2022-06-27 05:07:42.000000 smartloop-core-1.0.2/sl_core/nlu/classifiers/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     6787 2023-06-01 05:48:29.000000 smartloop-core-1.0.2/sl_core/nlu/classifiers/embedding_intent_classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1819 2023-05-02 05:20:47.000000 smartloop-core-1.0.2/sl_core/project.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      723 2023-01-06 20:04:52.000000 smartloop-core-1.0.2/sl_core/sanitizer.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1593 2023-05-03 01:09:11.000000 smartloop-core-1.0.2/sl_core/text_classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      627 2023-01-06 20:04:52.000000 smartloop-core-1.0.2/sl_core/tokenizer.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 21:34:48.286436 smartloop-core-1.0.2/smartloop_core.egg-info/
+-rw-r--r--   0 mehfuz     (501) staff       (20)     5398 2023-07-28 21:34:48.000000 smartloop-core-1.0.2/smartloop_core.egg-info/PKG-INFO
+-rw-r--r--   0 mehfuz     (501) staff       (20)      757 2023-07-28 21:34:48.000000 smartloop-core-1.0.2/smartloop_core.egg-info/SOURCES.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)        1 2023-07-28 21:34:48.000000 smartloop-core-1.0.2/smartloop_core.egg-info/dependency_links.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       56 2023-07-28 21:34:48.000000 smartloop-core-1.0.2/smartloop_core.egg-info/requires.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)        8 2023-07-28 21:34:48.000000 smartloop-core-1.0.2/smartloop_core.egg-info/top_level.txt
```

### Comparing `smartloop-core-1.0.1/LICENSE.txt` & `smartloop-core-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/README.md` & `smartloop-core-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/data/sample.json` & `smartloop-core-1.0.2/data/sample.json`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/setup.py` & `smartloop-core-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import sys
 from setuptools import setup, find_packages
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 install_requires = [
     'nltk==3.7',
     'joblib==1.1.1',
     'PyYAML==6.0',
     'scikit-learn~=1.2.2',
 ]
 
 setup(
     name='smartloop-core',
     description='Natural language processing framework for text processing',
-    version='1.0.1',
+    version='1.0.2',
     author_email='mehfuz@smartloop.ai',
     author='Smartloop Inc.',
     url='https://github.com/SmartloopAI/sl-core',
     download_url='https://github.com/SmartloopAI/sl-core/archive/refs/tags/1.0.1.tar.gz',
-    keywords=['NLP', 'framework', 'tensorflow'],
+    keywords=['NLP', 'framework', 'tensorflow', 'smartloop'],
     packages=find_packages(exclude=['tests*']),
     license='LICENSE.txt',
     install_requires=install_requires,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 4 - Beta',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  # Again, pick a license
         'Programming Language :: Python :: 3.9',
```

### Comparing `smartloop-core-1.0.1/sl_core/label_parser.py` & `smartloop-core-1.0.2/sl_core/label_parser.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/sl_core/model_loader.py` & `smartloop-core-1.0.2/sl_core/model_loader.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/sl_core/nlu/callbacks/train_status_report.py` & `smartloop-core-1.0.2/sl_core/nlu/callbacks/train_status_report.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/sl_core/nlu/classifiers/embedding_intent_classifier.py` & `smartloop-core-1.0.2/sl_core/nlu/classifiers/embedding_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/sl_core/project.py` & `smartloop-core-1.0.2/sl_core/project.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/sl_core/sanitizer.py` & `smartloop-core-1.0.2/sl_core/sanitizer.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/sl_core/text_classifier.py` & `smartloop-core-1.0.2/sl_core/text_classifier.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/sl_core/tokenizer.py` & `smartloop-core-1.0.2/sl_core/tokenizer.py`

 * *Files identical despite different names*

### Comparing `smartloop-core-1.0.1/smartloop_core.egg-info/SOURCES.txt` & `smartloop-core-1.0.2/smartloop_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

