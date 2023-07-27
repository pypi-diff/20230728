# Comparing `tmp/software_mentions_client-0.1.8.tar.gz` & `tmp/software_mentions_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "software_mentions_client-0.1.8.tar", last modified: Thu Jul 13 18:41:17 2023, max compression
+gzip compressed data, was "software_mentions_client-0.1.9.tar", last modified: Thu Jul 27 22:54:03 2023, max compression
```

## Comparing `software_mentions_client-0.1.8.tar` & `software_mentions_client-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/
--rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-07 10:52:06.000000 software_mentions_client-0.1.8/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      112 2023-03-07 19:00:06.000000 software_mentions_client-0.1.8/MANIFEST.in
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     6694 2023-05-22 13:05:07.000000 software_mentions_client-0.1.8/Readme.md
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      504 2023-03-07 18:31:51.000000 software_mentions_client-0.1.8/config.json
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       34 2023-07-13 18:40:17.000000 software_mentions_client-0.1.8/requirements.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      921 2023-07-13 18:40:28.000000 software_mentions_client-0.1.8/setup.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/software_mentions_client/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     2908 2022-02-17 14:19:32.000000 software_mentions_client-0.1.8/software_mentions_client/S3.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2022-02-17 14:19:32.000000 software_mentions_client-0.1.8/software_mentions_client/__init__.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    52167 2023-05-30 13:10:19.000000 software_mentions_client-0.1.8/software_mentions_client/client.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3620 2022-02-17 14:19:32.000000 software_mentions_client-0.1.8/software_mentions_client/consistency_check.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/software_mentions_client/resources/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3605 2021-08-30 13:06:10.000000 software_mentions_client-0.1.8/software_mentions_client/resources/covid_blacklist.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3191 2021-08-08 01:18:57.000000 software_mentions_client-0.1.8/software_mentions_client/resources/stopwords_en.txt
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/software_mentions_client.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      562 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       35 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/requires.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       25 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/top_level.txt
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-27 22:54:03.672834 software_mentions_client-0.1.9/
+-rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-07 10:52:06.000000 software_mentions_client-0.1.9/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      112 2023-03-07 19:00:06.000000 software_mentions_client-0.1.9/MANIFEST.in
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     7326 2023-07-27 22:54:03.672834 software_mentions_client-0.1.9/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     6805 2023-07-22 10:06:39.000000 software_mentions_client-0.1.9/Readme.md
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      504 2023-03-07 18:31:51.000000 software_mentions_client-0.1.9/config.json
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       34 2023-07-13 18:40:17.000000 software_mentions_client-0.1.9/requirements.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-27 22:54:03.672834 software_mentions_client-0.1.9/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      921 2023-07-27 22:53:20.000000 software_mentions_client-0.1.9/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-27 22:54:03.672834 software_mentions_client-0.1.9/software_mentions_client/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     2908 2022-02-17 14:19:32.000000 software_mentions_client-0.1.9/software_mentions_client/S3.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2022-02-17 14:19:32.000000 software_mentions_client-0.1.9/software_mentions_client/__init__.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    52972 2023-07-27 21:48:47.000000 software_mentions_client-0.1.9/software_mentions_client/client.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3620 2022-02-17 14:19:32.000000 software_mentions_client-0.1.9/software_mentions_client/consistency_check.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-27 22:54:03.672834 software_mentions_client-0.1.9/software_mentions_client/resources/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3605 2021-08-30 13:06:10.000000 software_mentions_client-0.1.9/software_mentions_client/resources/covid_blacklist.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3191 2021-08-08 01:18:57.000000 software_mentions_client-0.1.9/software_mentions_client/resources/stopwords_en.txt
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-27 22:54:03.672834 software_mentions_client-0.1.9/software_mentions_client.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     7326 2023-07-27 22:54:03.000000 software_mentions_client-0.1.9/software_mentions_client.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      562 2023-07-27 22:54:03.000000 software_mentions_client-0.1.9/software_mentions_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-27 22:54:03.000000 software_mentions_client-0.1.9/software_mentions_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       35 2023-07-27 22:54:03.000000 software_mentions_client-0.1.9/software_mentions_client.egg-info/requires.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       25 2023-07-27 22:54:03.000000 software_mentions_client-0.1.9/software_mentions_client.egg-info/top_level.txt
```

### Comparing `software_mentions_client-0.1.8/LICENSE` & `software_mentions_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.8/PKG-INFO` & `software_mentions_client-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software_mentions_client
-Version: 0.1.8
+Version: 0.1.9
 Summary: A client for extracting software mentions in scholar publications
 Home-page: https://github.com/kermitt2/software_mentions_client
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -15,17 +15,17 @@
 # Softcite software mention recognizer client
 
 [![PyPI version](https://badge.fury.io/py/software_mentions_client.svg)](https://badge.fury.io/py/software_mentions_client)
 [![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
 
 Python client for using the Softcite software mention recognition service. It can be applied to 
 
-* individual PDF files
+* individual PDF or XML fulltext file
 
-* recursively to a local directory, processing all the encountered PDF 
+* recursively to a local directory, processing all the encountered PDF and XML fulltext files
 
 * to a collection of documents harvested by [biblio-glutton-harvester](https://github.com/kermitt2/biblio-glutton-harvester) and [article-dataset-builder](https://github.com/kermitt2/article-dataset-builder), with the benefit of re-using the collection manifest for injectng metadata and keeping track of progress. The collection can be stored locally or on a S3 storage. 
 
 ## Requirements
 
 The client has been tested with Python 3.5-3.8. 
 
@@ -57,45 +57,44 @@
 > python3 -m pip install -e .
 ```
 
 
 ## Usage and options
 
 ```
-usage: client.py [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
+usage: python3 -m software_mentions_client.client [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
                  [--data-path DATA_PATH] [--config CONFIG] [--reprocess] [--reset] [--load]
                  [--diagnostic-mongo] [--diagnostic-files] [--scorched-earth]
 
 Softcite software mention recognizer client
 
 optional arguments:
   -h, --help            show this help message and exit
-  --repo-in REPO_IN     path to a directory of PDF files to be processed by the Softcite
-                        software mention recognizer
-  --file-in FILE_IN     a single PDF input file to be processed by the Softcite software
+  --repo-in REPO_IN     path to a directory of PDF or XML fulltext files to be processed by the
+                        Softcite software mention recognizer
+  --file-in FILE_IN     a single PDF or XML input file to be processed by the Softcite software
                         mention recognizer
   --file-out FILE_OUT   path to a single output the software mentions in JSON format, extracted
                         from the PDF file-in
   --data-path DATA_PATH
-                        path to the resource files created/harvested by biblio-glutton-
-                        harvester
+                        path to the resource files created/harvested by biblio-glutton-harvester
   --config CONFIG       path to the config file, default is ./config.json
-  --reprocess           reprocessed failed PDF
+  --reprocess           reprocessed failed PDF or XML fulltexts
   --reset               ignore previous processing states and re-init the annotation process
                         from the beginning
   --load                load json files into the MongoDB instance, the --repo-in or --data-path
                         parameter must indicate the path to the directory of resulting json
                         files to be loaded, --dump must indicate the path to the json dump file
                         of document metadata
   --diagnostic-mongo    perform a full count of annotations and diagnostic using MongoDB
                         regarding the harvesting and annotation process
   --diagnostic-files    perform a full count of annotations and diagnostic using repository
                         files regarding the harvesting and annotation process
-  --scorched-earth      remove a PDF file after its sucessful processing in order to save
-                        storage space, careful with this!
+  --scorched-earth      remove the PDF or XML fulltext files file after their sucessful
+                        processing in order to save storage space, careful with this!
 ```
 
 The logs are written by default in a file `./client.log`, but the location of the logs can be changed in the configuration file (default `./config.json`).
 
 ### Processing local PDF files
 
 For processing a single file., the resulting json being written as file at the indicated output path:
```

### Comparing `software_mentions_client-0.1.8/Readme.md` & `software_mentions_client-0.1.9/Readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Softcite software mention recognizer client
 
 [![PyPI version](https://badge.fury.io/py/software_mentions_client.svg)](https://badge.fury.io/py/software_mentions_client)
 [![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
 
 Python client for using the Softcite software mention recognition service. It can be applied to 
 
-* individual PDF files
+* individual PDF or XML fulltext file
 
-* recursively to a local directory, processing all the encountered PDF 
+* recursively to a local directory, processing all the encountered PDF and XML fulltext files
 
 * to a collection of documents harvested by [biblio-glutton-harvester](https://github.com/kermitt2/biblio-glutton-harvester) and [article-dataset-builder](https://github.com/kermitt2/article-dataset-builder), with the benefit of re-using the collection manifest for injectng metadata and keeping track of progress. The collection can be stored locally or on a S3 storage. 
 
 ## Requirements
 
 The client has been tested with Python 3.5-3.8. 
 
@@ -43,45 +43,44 @@
 > python3 -m pip install -e .
 ```
 
 
 ## Usage and options
 
 ```
-usage: client.py [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
+usage: python3 -m software_mentions_client.client [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
                  [--data-path DATA_PATH] [--config CONFIG] [--reprocess] [--reset] [--load]
                  [--diagnostic-mongo] [--diagnostic-files] [--scorched-earth]
 
 Softcite software mention recognizer client
 
 optional arguments:
   -h, --help            show this help message and exit
-  --repo-in REPO_IN     path to a directory of PDF files to be processed by the Softcite
-                        software mention recognizer
-  --file-in FILE_IN     a single PDF input file to be processed by the Softcite software
+  --repo-in REPO_IN     path to a directory of PDF or XML fulltext files to be processed by the
+                        Softcite software mention recognizer
+  --file-in FILE_IN     a single PDF or XML input file to be processed by the Softcite software
                         mention recognizer
   --file-out FILE_OUT   path to a single output the software mentions in JSON format, extracted
                         from the PDF file-in
   --data-path DATA_PATH
-                        path to the resource files created/harvested by biblio-glutton-
-                        harvester
+                        path to the resource files created/harvested by biblio-glutton-harvester
   --config CONFIG       path to the config file, default is ./config.json
-  --reprocess           reprocessed failed PDF
+  --reprocess           reprocessed failed PDF or XML fulltexts
   --reset               ignore previous processing states and re-init the annotation process
                         from the beginning
   --load                load json files into the MongoDB instance, the --repo-in or --data-path
                         parameter must indicate the path to the directory of resulting json
                         files to be loaded, --dump must indicate the path to the json dump file
                         of document metadata
   --diagnostic-mongo    perform a full count of annotations and diagnostic using MongoDB
                         regarding the harvesting and annotation process
   --diagnostic-files    perform a full count of annotations and diagnostic using repository
                         files regarding the harvesting and annotation process
-  --scorched-earth      remove a PDF file after its sucessful processing in order to save
-                        storage space, careful with this!
+  --scorched-earth      remove the PDF or XML fulltext files file after their sucessful
+                        processing in order to save storage space, careful with this!
 ```
 
 The logs are written by default in a file `./client.log`, but the location of the logs can be changed in the configuration file (default `./config.json`).
 
 ### Processing local PDF files
 
 For processing a single file., the resulting json being written as file at the indicated output path:
```

### Comparing `software_mentions_client-0.1.8/setup.py` & `software_mentions_client-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     reqs = f.readlines()
 
 setup(
     name="software_mentions_client",
-    version="0.1.8",
+    version="0.1.9",
     author="Patrice Lopez",
     author_email="patrice.lopez@science-miner.com",
     description="A client for extracting software mentions in scholar publications",
     long_description=open("Readme.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/kermitt2/software_mentions_client',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "my_config*", "*.log"]),
```

### Comparing `software_mentions_client-0.1.8/software_mentions_client/S3.py` & `software_mentions_client-0.1.9/software_mentions_client/S3.py`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.8/software_mentions_client/client.py` & `software_mentions_client-0.1.9/software_mentions_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-    Run the software mention recognizer service on PDF collections
+Run the software mention recognizer service on PDF or XML fulltext file collections
 '''
 
 import gzip
 import sys
 import os
 import shutil
 import json
@@ -147,28 +147,36 @@
                     elif filename.endswith(".pdf.gz"):
                         filename_json = filename.replace(".pdf.gz", ".software.json")
                     elif filename.endswith(".PDF"):
                         filename_json = filename.replace(".PDF", ".software.json")
                     elif filename.endswith(".xml"):
                         filename_json = filename.replace(".xml", ".software.json")
 
+                    # prioretize TEI XML because better quality and faster
+                    filename_tei1 = os.path.join(root, filename_json.replace(".software.json", ".pub2tei.tei.xml"))
+                    filename_tei2 = os.path.join(root, filename_json.replace(".software.json", ".pub2tei.tei.xml"))
+                    if os.path.isfile(filename_tei1) or os.path.isfile(filename_tei2):
+                        # we have a TEI file, so if the current filename is not this TEI, we skip
+                        if not filename.endswith(".tei.xml"):
+                            continue
+
                     sha1 = getSHA1(os.path.join(root,filename))
 
                     # if the json file already exists and not force, we skip 
                     if os.path.isfile(os.path.join(root, filename_json)) and not force:
                         # check that this id is considered in the lmdb keeping track of the process
                         with self.env_software.begin() as txn:
                             status = txn.get(sha1.encode(encoding='UTF-8'))
                         if status is None:
                             with self.env_software.begin(write=True) as txn2:
                                 txn2.put(sha1.encode(encoding='UTF-8'), "True".encode(encoding='UTF-8')) 
                         continue
 
                     # if identifier already processed successfully in the local lmdb, we skip
-                    # the hash of the PDF file is used as unique identifier for the PDF (SHA1)
+                    # the hash of the fulltext file is used as unique identifier for the document (SHA1)
                     with self.env_software.begin() as txn:
                         status = txn.get(sha1.encode(encoding='UTF-8'))
                         if status is not None and not force:
                             continue
 
                     pdf_files.append(os.path.join(root,filename))
                     out_files.append(os.path.join(root, filename_json))
@@ -192,15 +200,16 @@
             nb_total += len(pdf_files)
             runtime = round(time.time() - start_time, 3)
             sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
             sys.stdout.flush()
 
     def annotate_collection(self, data_path, force=False):
         '''
-        Annotate a collection harvested by biblio_glutton_harvester or article_dataset_builder, only PDF for the moment
+        Annotate a collection of fulltexts harvested by biblio_glutton_harvester or article_dataset_builder. 
+        The documents can be PDF or XML (TEI or other publisher XML format supported by Pub2TEI, e.g. JATS) 
         '''
         # init lmdb transactions
         # open in read mode
         envFilePath = os.path.join(data_path, 'entries')
         self.env = lmdb.open(envFilePath, map_size=map_size)
 
         with self.env.begin(write=True) as txn:
@@ -559,15 +568,15 @@
                 if jsonObject is not None:
                     txn.put(full_record['id'].encode(encoding='UTF-8'), "True".encode(encoding='UTF-8')) 
                 else:
                     # the process failed
                     txn.put(full_record['id'].encode(encoding='UTF-8'), "False".encode(encoding='UTF-8'))
 
         if self.scorched_earth and jsonObject is not None:
-            # processed is done, remove local PDF file
+            # processed is done, remove local document file
             try:
                 os.remove(file_in) 
             except:
                 logging.exception("Error while deleting file " + file_in)
 
     def diagnostic(self, full_diagnostic_mongo=False, full_diagnostic_files=False, directory=None):
         """
@@ -997,28 +1006,28 @@
                 break
             sha1.update(data)
 
     return sha1.hexdigest()
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description = "Softcite software mention recognizer client")
-    parser.add_argument("--repo-in", default=None, help="path to a directory of PDF files to be processed by the Softcite software mention recognizer")  
-    parser.add_argument("--file-in", default=None, help="a single PDF input file to be processed by the Softcite software mention recognizer") 
+    parser.add_argument("--repo-in", default=None, help="path to a directory of PDF or XML fulltext files to be processed by the Softcite software mention recognizer")  
+    parser.add_argument("--file-in", default=None, help="a single PDF or XML input file to be processed by the Softcite software mention recognizer") 
     parser.add_argument("--file-out", default=None, help="path to a single output the software mentions in JSON format, extracted from the PDF file-in") 
     parser.add_argument("--data-path", default=None, help="path to the resource files created/harvested by biblio-glutton-harvester") 
     parser.add_argument("--config", default="./config.json", help="path to the config file, default is ./config.json") 
-    parser.add_argument("--reprocess", action="store_true", help="reprocessed failed PDF") 
+    parser.add_argument("--reprocess", action="store_true", help="reprocessed failed PDF or XML fulltexts") 
     parser.add_argument("--reset", action="store_true", help="ignore previous processing states and re-init the annotation process from the beginning") 
     parser.add_argument("--load", action="store_true", help="load json files into the MongoDB instance, the --repo-in or --data-path parameter must indicate the path "
         +"to the directory of resulting json files to be loaded, --dump must indicate the path to the json dump file of document metadata") 
     parser.add_argument("--diagnostic-mongo", action="store_true", help="perform a full count of annotations and diagnostic using MongoDB "  
         +"regarding the harvesting and annotation process") 
     parser.add_argument("--diagnostic-files", action="store_true", help="perform a full count of annotations and diagnostic using repository files "  
         +"regarding the harvesting and annotation process") 
-    parser.add_argument("--scorched-earth", action="store_true", help="remove a PDF file after its sucessful processing in order to save storage space" 
+    parser.add_argument("--scorched-earth", action="store_true", help="remove the PDF or XML fulltext files file after their sucessful processing in order to save storage space" 
         +", careful with this!") 
 
     args = parser.parse_args()
 
     data_path = args.data_path
     config_path = args.config
     reprocess = args.reprocess
@@ -1050,15 +1059,15 @@
             sys.exit("the mongodb server where to load the json files is not indicated in the config file, leaving...")
 
         if repo_in is not None:
             client.load_mongo(repo_in)
         elif data_path is None and len(client.config["data_path"])>0:
             data_path = client.config["data_path"] 
             if repo_in is None and (data_path is None or len(client.config["data_path"])==0): 
-                sys.exit("the repo_in where to find the PDF files to be processed is not indicated, leaving...")
+                sys.exit("the repo_in where to find the PDF or XML fulltext files to be processed is not indicated, leaving...")
             if data_path is not None:
                 client.load_mongo(data_path)
         
     elif reprocess:
         client.reprocess_failed(repo_in)
     elif repo_in is not None and not full_diagnostic_files: 
         client.annotate_directory(repo_in, force)
```

### Comparing `software_mentions_client-0.1.8/software_mentions_client/consistency_check.py` & `software_mentions_client-0.1.9/software_mentions_client/consistency_check.py`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.8/software_mentions_client/resources/covid_blacklist.txt` & `software_mentions_client-0.1.9/software_mentions_client/resources/covid_blacklist.txt`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.8/software_mentions_client/resources/stopwords_en.txt` & `software_mentions_client-0.1.9/software_mentions_client/resources/stopwords_en.txt`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.8/software_mentions_client.egg-info/PKG-INFO` & `software_mentions_client-0.1.9/software_mentions_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software-mentions-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: A client for extracting software mentions in scholar publications
 Home-page: https://github.com/kermitt2/software_mentions_client
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -15,17 +15,17 @@
 # Softcite software mention recognizer client
 
 [![PyPI version](https://badge.fury.io/py/software_mentions_client.svg)](https://badge.fury.io/py/software_mentions_client)
 [![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
 
 Python client for using the Softcite software mention recognition service. It can be applied to 
 
-* individual PDF files
+* individual PDF or XML fulltext file
 
-* recursively to a local directory, processing all the encountered PDF 
+* recursively to a local directory, processing all the encountered PDF and XML fulltext files
 
 * to a collection of documents harvested by [biblio-glutton-harvester](https://github.com/kermitt2/biblio-glutton-harvester) and [article-dataset-builder](https://github.com/kermitt2/article-dataset-builder), with the benefit of re-using the collection manifest for injectng metadata and keeping track of progress. The collection can be stored locally or on a S3 storage. 
 
 ## Requirements
 
 The client has been tested with Python 3.5-3.8. 
 
@@ -57,45 +57,44 @@
 > python3 -m pip install -e .
 ```
 
 
 ## Usage and options
 
 ```
-usage: client.py [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
+usage: python3 -m software_mentions_client.client [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
                  [--data-path DATA_PATH] [--config CONFIG] [--reprocess] [--reset] [--load]
                  [--diagnostic-mongo] [--diagnostic-files] [--scorched-earth]
 
 Softcite software mention recognizer client
 
 optional arguments:
   -h, --help            show this help message and exit
-  --repo-in REPO_IN     path to a directory of PDF files to be processed by the Softcite
-                        software mention recognizer
-  --file-in FILE_IN     a single PDF input file to be processed by the Softcite software
+  --repo-in REPO_IN     path to a directory of PDF or XML fulltext files to be processed by the
+                        Softcite software mention recognizer
+  --file-in FILE_IN     a single PDF or XML input file to be processed by the Softcite software
                         mention recognizer
   --file-out FILE_OUT   path to a single output the software mentions in JSON format, extracted
                         from the PDF file-in
   --data-path DATA_PATH
-                        path to the resource files created/harvested by biblio-glutton-
-                        harvester
+                        path to the resource files created/harvested by biblio-glutton-harvester
   --config CONFIG       path to the config file, default is ./config.json
-  --reprocess           reprocessed failed PDF
+  --reprocess           reprocessed failed PDF or XML fulltexts
   --reset               ignore previous processing states and re-init the annotation process
                         from the beginning
   --load                load json files into the MongoDB instance, the --repo-in or --data-path
                         parameter must indicate the path to the directory of resulting json
                         files to be loaded, --dump must indicate the path to the json dump file
                         of document metadata
   --diagnostic-mongo    perform a full count of annotations and diagnostic using MongoDB
                         regarding the harvesting and annotation process
   --diagnostic-files    perform a full count of annotations and diagnostic using repository
                         files regarding the harvesting and annotation process
-  --scorched-earth      remove a PDF file after its sucessful processing in order to save
-                        storage space, careful with this!
+  --scorched-earth      remove the PDF or XML fulltext files file after their sucessful
+                        processing in order to save storage space, careful with this!
 ```
 
 The logs are written by default in a file `./client.log`, but the location of the logs can be changed in the configuration file (default `./config.json`).
 
 ### Processing local PDF files
 
 For processing a single file., the resulting json being written as file at the indicated output path:
```

### Comparing `software_mentions_client-0.1.8/software_mentions_client.egg-info/SOURCES.txt` & `software_mentions_client-0.1.9/software_mentions_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

