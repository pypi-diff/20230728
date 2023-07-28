# Comparing `tmp/deepsearch_glm-0.2.1.tar.gz` & `tmp/deepsearch_glm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsearch_glm-0.2.1.tar", max compression
+gzip compressed data, was "deepsearch_glm-0.2.2.tar", max compression
```

## Comparing `deepsearch_glm-0.2.1.tar` & `deepsearch_glm-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1088 2023-07-08 03:50:49.893964 deepsearch_glm-0.2.1/LICENSE
--rw-r--r--   0        0        0     2984 2023-07-14 09:21:46.015603 deepsearch_glm-0.2.1/README.md
--rw-r--r--   0        0        0     1840 2023-07-21 12:54:50.598456 deepsearch_glm-0.2.1/build.py
--rw-r--r--   0        0        0        0 2023-07-08 03:50:49.913495 deepsearch_glm-0.2.1/deepsearch_glm/__init__.py
--rw-r--r--   0        0        0     3029 2023-07-19 07:59:42.945265 deepsearch_glm-0.2.1/deepsearch_glm/glm_create_from_docs.py
--rw-r--r--   0        0        0     4988 2023-07-14 09:21:46.051654 deepsearch_glm-0.2.1/deepsearch_glm/glm_docqa.py
--rw-r--r--   0        0        0     3137 2023-07-14 09:21:46.052650 deepsearch_glm-0.2.1/deepsearch_glm/glm_explore.py
--rw-r--r--   0        0        0     2937 2023-07-14 09:21:46.053534 deepsearch_glm-0.2.1/deepsearch_glm/glm_utils.py
--rw-r--r--   0        0        0     4226 2023-07-21 07:26:03.085046 deepsearch_glm-0.2.1/deepsearch_glm/nlp_analyse_docs.py
--rw-r--r--   0        0        0     3856 2023-07-20 05:17:22.733695 deepsearch_glm-0.2.1/deepsearch_glm/nlp_apply_on_docs.py
--rw-r--r--   0        0        0     2161 2023-07-21 07:26:03.085678 deepsearch_glm-0.2.1/deepsearch_glm/nlp_apply_on_text.py
--rw-r--r--   0        0        0    21643 2023-07-21 07:26:03.086794 deepsearch_glm-0.2.1/deepsearch_glm/nlp_train_reference.py
--rw-r--r--   0        0        0     1819 2023-07-21 07:26:03.088127 deepsearch_glm-0.2.1/deepsearch_glm/nlp_utils.py
--rw-r--r--   0        0        0     8534 2023-07-14 09:21:46.056334 deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesRestricted.txt
--rw-r--r--   0        0        0   599388 2023-07-14 09:21:46.058795 deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesSummary.txt
--rw-r--r--   0        0        0       82 2023-07-14 09:21:46.059061 deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/note.txt
--rw-r--r--   0        0        0      679 2023-07-14 09:21:46.059828 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/crf/part-of-speech/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.059928 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/crf/reference/note.md
--rw-r--r--   0        0        0      188 2023-07-14 09:21:46.060169 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/language/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060269 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/person-name/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060409 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/semantic/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060599 deepsearch_glm-0.2.1/deepsearch_glm/resources/models/fasttext/topic/note.md
--rw-r--r--   0        0        0      801 2023-07-14 09:21:46.059514 deepsearch_glm-0.2.1/deepsearch_glm/resources/models.json
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060732 deepsearch_glm-0.2.1/deepsearch_glm/utils/__init__.py
--rw-r--r--   0        0        0     1803 2023-07-15 05:40:03.618146 deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_query.py
--rw-r--r--   0        0        0     7364 2023-07-21 07:26:03.089281 deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_utils.py
--rw-r--r--   0        0        0     1295 2023-07-21 07:26:03.090106 deepsearch_glm-0.2.1/deepsearch_glm/utils/load_pretrained_models.py
--rw-r--r--   0        0        0      729 2023-07-21 12:54:50.600869 deepsearch_glm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 deepsearch_glm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-08 03:50:49.893964 deepsearch_glm-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2984 2023-07-14 09:21:46.015603 deepsearch_glm-0.2.2/README.md
+-rw-r--r--   0        0        0     1981 2023-07-28 09:11:03.283385 deepsearch_glm-0.2.2/build.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:50:49.913495 deepsearch_glm-0.2.2/deepsearch_glm/__init__.py
+-rw-r--r--   0        0        0     3022 2023-07-23 04:35:49.855789 deepsearch_glm-0.2.2/deepsearch_glm/glm_create_from_docs.py
+-rw-r--r--   0        0        0     4988 2023-07-14 09:21:46.051654 deepsearch_glm-0.2.2/deepsearch_glm/glm_docqa.py
+-rw-r--r--   0        0        0     3152 2023-07-23 04:36:41.893381 deepsearch_glm-0.2.2/deepsearch_glm/glm_explore.py
+-rw-r--r--   0        0        0     2974 2023-07-23 04:36:37.575434 deepsearch_glm-0.2.2/deepsearch_glm/glm_utils.py
+-rw-r--r--   0        0        0     6508 2023-07-27 12:59:58.320686 deepsearch_glm-0.2.2/deepsearch_glm/nlp_analyse_docs.py
+-rw-r--r--   0        0        0     4004 2023-07-28 03:55:33.481106 deepsearch_glm-0.2.2/deepsearch_glm/nlp_apply_on_docs.py
+-rw-r--r--   0        0        0     2827 2023-07-23 05:26:44.746779 deepsearch_glm-0.2.2/deepsearch_glm/nlp_apply_on_text.py
+-rw-r--r--   0        0        0    19285 2023-07-22 05:49:57.517610 deepsearch_glm-0.2.2/deepsearch_glm/nlp_train_reference.py
+-rw-r--r--   0        0        0    12115 2023-07-25 05:52:14.456260 deepsearch_glm-0.2.2/deepsearch_glm/nlp_train_semantic.py
+-rw-r--r--   0        0        0     2367 2023-07-23 04:14:53.204506 deepsearch_glm-0.2.2/deepsearch_glm/nlp_utils.py
+-rw-r--r--   0        0        0     8534 2023-07-14 09:21:46.056334 deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesRestricted.txt
+-rw-r--r--   0        0        0   599388 2023-07-14 09:21:46.058795 deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesSummary.txt
+-rw-r--r--   0        0        0       82 2023-07-14 09:21:46.059061 deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/note.txt
+-rw-r--r--   0        0        0      679 2023-07-14 09:21:46.059828 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/crf/part-of-speech/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.059928 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/crf/reference/note.md
+-rw-r--r--   0        0        0      188 2023-07-14 09:21:46.060169 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/language/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060269 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/person-name/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060409 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/semantic/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060599 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/topic/note.md
+-rw-r--r--   0        0        0      801 2023-07-14 09:21:46.059514 deepsearch_glm-0.2.2/deepsearch_glm/resources/models.json
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060732 deepsearch_glm-0.2.2/deepsearch_glm/utils/__init__.py
+-rw-r--r--   0        0        0     1822 2023-07-24 14:23:30.124083 deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_query.py
+-rw-r--r--   0        0        0     7973 2023-07-28 04:05:17.418171 deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_utils.py
+-rw-r--r--   0        0        0     1293 2023-07-21 13:46:59.409978 deepsearch_glm-0.2.2/deepsearch_glm/utils/load_pretrained_models.py
+-rw-r--r--   0        0        0      729 2023-07-28 09:13:41.626532 deepsearch_glm-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 deepsearch_glm-0.2.2/PKG-INFO
```

### Comparing `deepsearch_glm-0.2.1/LICENSE` & `deepsearch_glm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.1/README.md` & `deepsearch_glm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.1/build.py` & `deepsearch_glm-0.2.2/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,33 +9,38 @@
 import subprocess
 
 from deepsearch_glm.utils.load_pretrained_models import load_pretrained_nlp_models
 
 ROOT_DIR=os.path.abspath("./")
 BUILD_DIR=os.path.join(ROOT_DIR, "build")
 
+def download_nlp_models():
+    load_pretrained_nlp_models(False)
+
 def run(cmd, cwd="./"):
 
     print(f"\nlaunch: {cmd}")
     
     parts = cmd.split(" ")
     message = subprocess.run(parts, cwd=cwd)    
 
     if "returncode=0" in str(message):
         print(f" -> SUCCESS")
         return True
 
     print(f" -> ERROR with message: '{message}'\n")        
     return False
     
-def build(setup_kwargs=None):
+def build_local(setup_kwargs=None):
 
     if not os.path.exists(BUILD_DIR):
         cmd = f"cmake -B {BUILD_DIR}"
         run(cmd, cwd=ROOT_DIR)
+    else:
+        print(f"build directory detected: {BUILD_DIR}")
         
     cmd = f"cmake --build {BUILD_DIR} --target install -j"
     run(cmd, cwd=ROOT_DIR)    
 
 def build_all_python_versions():
 
     candidates = glob.glob("/usr/local/bin/python3.*")
@@ -66,12 +71,9 @@
         cmd = f"cmake --build {PYBUILD_DIR} --target install -j"
         run(cmd, cwd=ROOT_DIR)    
     
 if "__main__"==__name__:
 
     #load_pretrained_nlp_models(False)
 
-    #build()
+    #build_local()
     build_all_python_versions()
-
-
-
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/glm_create_from_docs.py` & `deepsearch_glm-0.2.2/deepsearch_glm/glm_create_from_docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 import argparse
 import textwrap
 import datetime
 
 from tabulate import tabulate
 
-from glm_utils import create_glm_dir, create_glm_from_docs
+from deepsearch_glm.glm_utils import create_glm_dir, create_glm_from_docs
 
-#import andromeda_nlp
 import andromeda_glm
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = 'create_glm_from_docs',
         description = 'Create GLM from Deep Search documents',
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/glm_docqa.py` & `deepsearch_glm-0.2.2/deepsearch_glm/glm_docqa.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/glm_explore.py` & `deepsearch_glm-0.2.2/deepsearch_glm/glm_explore.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import argparse
 import textwrap
 import datetime
 
 from tabulate import tabulate
 
-from glm_utils import load_glm
+from deepsearch_glm.glm_utils import load_glm
 
 import andromeda_nlp
 import andromeda_glm
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/glm_utils.py` & `deepsearch_glm-0.2.2/deepsearch_glm/glm_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+#!/usr/bin/env python
 
 import os
 
 import json
 import glob
 
 import argparse
 import textwrap
 import datetime
 
 from tabulate import tabulate
 
-from utils.ds_utils import get_scratch_dir
+from deepsearch_glm.utils.ds_utils import get_scratch_dir
 
 #import andromeda_nlp
 import andromeda_glm
 
 def create_glm_dir():
 
     tdir = get_scratch_dir()
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/nlp_apply_on_docs.py` & `deepsearch_glm-0.2.2/deepsearch_glm/nlp_apply_on_docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,32 +100,36 @@
 
     json_files = sorted(list(set(json_files)))        
 
     model = init_nlp_model(model_names)
 
     for json_file in json_files:
 
+        print(f"reading {json_file} ... ", end="")
         with open(json_file, "r") as fr:
             doc_i = json.load(fr)
-    
+
+        print(f"applying models ... ", end="")
         doc_j = model.apply_on_doc(doc_i)
 
+        """
         props = pd.DataFrame(doc_j["properties"]["data"],
                              columns=doc_j["properties"]["headers"])
         print("properties: \n\n", props)
 
         ints = pd.DataFrame(doc_j["instances"]["data"], 
                             columns=doc_j["instances"]["headers"])
         print("instances: \n\n", ints)
 
-        """
         ents = pd.DataFrame(doc_j["entities"]["data"], 
                             columns=doc_j["entities"]["headers"])
         print(ents)
         """
         
         nlp_file = json_file.replace(".json", ".nlp.json")
+        print(f"writing  models {nlp_file}")
+        
         with open(nlp_file, "w") as fw:
             fw.write(json.dumps(doc_j, indent=2))
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/nlp_train_reference.py` & `deepsearch_glm-0.2.2/deepsearch_glm/nlp_train_reference.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 
 #import fasttext
 import textColor as tc
 
 #import deepsearch as ds
-
-from utils.ds_utils import convert_pdffiles
-from nlp_utils import create_nlp_dir
+#from tabulate import tabulate
 
 import andromeda_nlp
 
-from tabulate import tabulate
+from deepsearch_glm.utils.ds_utils import convert_pdffiles
+from deepsearch_glm.nlp_utils import create_nlp_dir
+
+
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = "nlp_train_reference",
         description = 'Prepare CRF data for CRF-reference parser',
         epilog =
@@ -86,85 +87,14 @@
         json_files=[]
     
     if not os.path.exists(args.output_dir):
         os.mkdir(args.output_dir)
     
     return args.mode, pdf_files, json_files, args.output_dir
 
-"""
-def convert(sdirectory, username, password):
-
-    pdfs_files=glob.glob(os.path.join(sdirectory, "*.pdf"))
-    json_files=glob.glob(os.path.join(sdirectory, "*.json"))
-
-    new_pdfs=[]
-    
-    found_new_pdfs=False
-    for pdf_file in pdfs_files:
-
-        json_file = pdf_file.replace(".pdf", ".json")
-        if json_file not in json_files:
-            new_pdfs.append(pdf_file)
-            found_new_pdfs = True
-
-    print("found new pdf's: ", found_new_pdfs)
-            
-    if not found_new_pdfs:
-        return found_new_pdfs
-    
-    config_ = {
-        "host": deepsearch_host,
-        "auth": {
-            "username": username,
-            "api_key": password,
-        },
-        "verify_ssl": True
-    }
-
-    config_file = "ds_config.json"
-    with open(config_file, "w") as fw:
-        fw.write(json.dumps(config_))
-    
-    config = ds.DeepSearchConfig.parse_file(config_file)
-    
-    client = ds.CpsApiClient(config)
-    api = ds.CpsApi(client)
-
-    documents = ds.convert_documents(api=api, proj_key=deepsearch_proj,
-                                     source_path=sdirectory, progress_bar=True)           
-    documents.download_all(result_dir=sdirectory)
-
-    info = documents.generate_report(result_dir=sdirectory)
-    return found_new_pdfs
-
-def process_zip_files(sdir):
-
-    jsonfiles = sorted(glob.glob(os.path.join(sdir, "*.json")))
-    for i,jsonfile in enumerate(jsonfiles):
-        subprocess.call(["rm", jsonfile])
-
-    cellsfiles = sorted(glob.glob(os.path.join(sdir, "*.cells")))
-    for i,cellsfile in enumerate(cellsfiles):
-        subprocess.call(["rm", cellsfile])            
-    
-    zipfiles = sorted(glob.glob(os.path.join(sdir, "*.zip")))
-    print("#-zips: ", len(zipfiles))
-
-    for zipfile in zipfiles:
-        subprocess.call(["unzip", zipfile, "-d", sdir])    
-
-    for i,zipfile in enumerate(zipfiles):
-        print(i, "\t removing ", zipfile)
-        subprocess.call(["rm", zipfile])        
-
-    cellsfiles = sorted(glob.glob(os.path.join(sdir, "*.cells")))
-    for i,cellsfile in enumerate(cellsfiles):
-        subprocess.call(["rm", cellsfile])            
-"""
-        
 def shorten_text(text):
     
     ntext = text.replace("\n", "")
     
     return ntext.strip()
         
 def extract_references(filenames, sfile, rfile):
@@ -632,21 +562,14 @@
             config["files"]["train-file"] = train_file 
             config["files"]["metrics-file"] = metrics_file
             
             model.train(config)
             
 if __name__ == '__main__':
 
-    """
-    mode, sdir, tdir, username, password = parse_arguments()
-
-
-
-    """
-
     mode, pdf_files, json_files, tdir = parse_arguments()
     
     if len(pdf_files)>0:
         new_json_files = convert_pdffiles(pdf_files, force=False)
 
         for _ in new_json_files:
             json_files.append(_)
@@ -656,22 +579,14 @@
     sfile = os.path.join(tdir, "nlp-train-semantic-classification.annot.jsonl")
     rfile = os.path.join(tdir, "nlp-train-references-crf.jsonl")
     afile = os.path.join(tdir, "nlp-train-references-crf.annot.jsonl")
     
     crf_model_file = os.path.join(tdir, "crf_reference")
     fst_model_file = os.path.join(tdir, "fst_sematic")
 
-    """
-    if mode=="convert" or mode=="all":
-        found_new_pdfs = convert(sdir, username, password)    
-
-        if found_new_pdfs:
-            process_zip_files(sdir)
-    """
-    
     if mode=="extract" or mode=="all":
         extract_references(json_files, sfile, rfile)
 
     if mode=="annotate" or mode=="all":
         annotate(rfile, afile)
 
     if "classify" in mode or mode=="all":
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesRestricted.txt` & `deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesRestricted.txt`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/resources/confusables/confusablesSummary.txt` & `deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesSummary.txt`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/resources/models/crf/part-of-speech/note.md` & `deepsearch_glm-0.2.2/deepsearch_glm/resources/models/crf/part-of-speech/note.md`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/resources/models.json` & `deepsearch_glm-0.2.2/deepsearch_glm/resources/models.json`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_query.py` & `deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 import os
 
 import json
 import glob
 
+import datetime
 import argparse
 
 import pandas as pd
 
 from ds_utils import create_docs_dir, ds_list_indices, ds_index_query
 
 def parse_arguments():
@@ -21,28 +22,30 @@
 examples of execution: 
 
 1. search for documents:
 
     poetry run python ./deepsearch_glm/ds_query.py --index esg-reports --query "\\\"net zero\\\""
     poetry run python ./deepsearch_glm/ds_query.py --index patent-uspto --query "\\\"global warming potential\\\" AND \\\"etching\\\""
     poetry run python ./deepsearch_glm/ds_query.py --index arxiv --query "\\\"quantum computing\\\""
+
+
 """,
         formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('--index', required=True,
                         type=str,
                         help="Deep Search document index")
 
     parser.add_argument('--query', required=True,
                         type=str, 
                         help="Query for document")
 
     parser.add_argument('--output-dir', required=False,
                         type=bool, default=create_docs_dir(),
-                        help="output root directory for GLM")        
+                        help="output directory for documents")        
 
     args = parser.parse_args()
 
     return args.index, args.query, args.output_dir
 
 if __name__ == '__main__':
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/utils/ds_utils.py` & `deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 
 import os
 
 import json
 import copy
 import glob
 import hashlib
+import datetime
 import subprocess
 
 from tqdm import tqdm
 from numerize.numerize import numerize
 from dotenv import load_dotenv
 
 import deepsearch as ds
 
 from deepsearch.cps.client.components.elastic import ElasticDataCollectionSource
 from deepsearch.cps.queries import DataQuery
 from deepsearch.cps.client.components.queries import RunQueryError
 
-#from deepsearch.artifacts.artifact_manager import ArtifactManager
-
 def get_scratch_dir():
     
     load_dotenv()
 
     tmpdir = os.path.abspath(os.getenv("DEEPSEARCH_GLM_SCRATCH_DIR"))
 
     if not os.path.exists(tmpdir):
@@ -197,16 +196,22 @@
 
     now = datetime.datetime.now()
     odir = now.strftime("document-collection-%Y-%m-%d_%H-%M-%S")
 
     odir = os.path.join(tdir, odir)
     return odir    
 
-def ds_index_query(index, query, odir=None, force=False):
-
+def ds_index_query(index, query, odir=None, force=False, limit=-1,
+                   sources=["file-info", "description",
+                            "main-text",
+                            "texts", "tables", "figures",                
+                            "page-headers", "page-footers",
+                            "footnotes"] # Which fields of documents we want to fetch
+                   ):
+    
     api, proj_key = get_ds_api()
     
     tdir = get_scratch_dir()
 
     if odir==None:
         dumpdir = hashlib.md5(f"{index}:{query}".encode()).hexdigest()
         dumpdir = os.path.join(tdir, dirname)
@@ -221,41 +226,58 @@
     # Input query
     search_query = f"{query}" #"\"global warming potential\" AND \"etching\""
     print(f"query: {query}")
     
     data_collection = ElasticDataCollectionSource(elastic_id="default", index_key=index)
     page_size = 50
 
-    # Prepare the data query
-    query = DataQuery(
-        search_query, # The search query to be executed
+    """
         source=["file-info", "description",
                 "main-text",
                 "texts", "tables", "figures",                
                 "page-headers", "page-footers",
-                "footnotes"], # Which fields of documents we want to fetch
+                "footnotes"], 
+    """
+    
+    # Prepare the data query
+    query = DataQuery(
+        search_query, # The search query to be executed
+        source=sources, # Which fields of documents we want to fetch
         limit=page_size, # The size of each request page
         coordinates=data_collection # The data collection to be queries
     )
 
     # [Optional] Compute the number of total results matched. This can be used to monitor the pagination progress.
     count_query = copy.deepcopy(query)
     count_query.paginated_task.parameters["limit"] = 0
     count_results = api.queries.run(count_query)
+       
     expected_total = count_results.outputs["data_count"]
     print(f"#-found documents: {expected_total}")
-    
+
+    if limit!=-1 and expected_total>limit:
+        expected_total=limit    
+
     expected_pages = (expected_total + page_size - 1) // page_size # this is simply a ceiling formula
     
     # Iterate through all results by fetching `page_size` results at the same time
     bar_format = '{desc:<5.5}{percentage:3.0f}%|{bar:70}{r_bar}'
+
+    count=0
     
     all_results = []
     cursor = api.queries.run_paginated_query(query)
     for result_page in tqdm(cursor, total=expected_pages, bar_format=bar_format):
         for row in result_page.outputs["data_outputs"]:
             _id = row["_id"]
             with open(f"{dumpdir}/{_id}.json", "w") as fw:
                 fw.write(json.dumps(row["_source"], indent=2))
-    
+
+            count+=1
+            if limit!=-1 and count>=limit:
+                break
+
+        if limit!=-1 and count>=limit:
+            break            
+                
     return dumpdir
```

### Comparing `deepsearch_glm-0.2.1/deepsearch_glm/utils/load_pretrained_models.py` & `deepsearch_glm-0.2.2/deepsearch_glm/utils/load_pretrained_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     COS_PATH = os.path.join(COS_URL, COS_PRFX)
     
     cmds=[]
     for name,files in models["nlp"]["trained-models"].items():
         source = os.path.join(COS_PATH, files[0])
         target = os.path.join(RESOURCES_DIR, files[1])
 
-        cmd = ["curl", source, "-o", target]#, "-s"]
+        cmd = ["curl", source, "-o", target, "-s"]
         #print(" ".join(cmd))        
         cmds.append(cmd)
         
     for cmd in cmds:
         if force or (not os.path.exists(cmd[3])):
             #print(f"downloading {cmd[3]} ... ", end="")
             print(f"downloading {os.path.basename(cmd[3])} ... ", end="")
```

### Comparing `deepsearch_glm-0.2.1/pyproject.toml` & `deepsearch_glm-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsearch-glm"
-version = "0.2.1"
+version = "0.2.2"
 description = "Graph Language Models"
 authors = ["Peter Staar <taa@zurich.ibm.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "deepsearch_glm"}]
 include = [
     {path = "deepsearch_glm/*.so", format = "wheel"}
```

### Comparing `deepsearch_glm-0.2.1/PKG-INFO` & `deepsearch_glm-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsearch-glm
-Version: 0.2.1
+Version: 0.2.2
 Summary: Graph Language Models
 License: MIT
 Author: Peter Staar
 Author-email: taa@zurich.ibm.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_dmiav_nv_/tmph7ygc7qe_TarContainer/0/28", line 140, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_dmiav_nv_/tmph7ygc7qe_TarContainer/0/28", line 140, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deepsearch-glm Version: 0.2.1 Summary: Graph
+Metadata-Version: 2.1 Name: deepsearch-glm Version: 0.2.2 Summary: Graph
 Language Models License: MIT Author: Peter Staar Author-email:
 taa@zurich.ibm.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: deepsearch-toolkit (>=0.19.1,<0.20.0)
 Requires-Dist: fastapi (>=0.99.0,<0.100.0) Requires-Dist: matplotlib
 (>=3.7.1,<4.0.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist: netwulf
```

