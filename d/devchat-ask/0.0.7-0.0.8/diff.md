# Comparing `tmp/devchat_ask-0.0.7-cp311-cp311-win_amd64.whl.zip` & `tmp/devchat_ask-0.0.8-cp311-cp311-macosx_12_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,61 @@
-Zip file size: 1093269 bytes, number of entries: 12
--rw-r--r--  2.0 fat    25922 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/devlake_qa_examples.json
--rw-r--r--  2.0 fat    12351 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/devlake_test_set_mini.json
--rw-r--r--  2.0 fat    18301 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/langchain_test_set.json
--rw-r--r--  2.0 fat      880 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/mock.json
--rw-r--r--  2.0 fat      571 b- defN 80-Jan-01 00:00 chat/evaluation/qa/README.md
--rw-r--r--  2.0 fat     5117 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/README.md
--rw-r--r--  2.0 fat   407954 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/scores.csv
--rw-r--r--  2.0 fat  1179453 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/snippets.zip
--rw-r--r--  2.0 fat       64 b- defN 80-Jan-01 00:00 chat/README.md
--rw-r--r--  2.0 fat      704 b- defN 80-Jan-01 00:00 devchat_ask-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 fat       98 b- defN 80-Jan-01 00:00 devchat_ask-0.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1173 b- defN 16-Jan-01 00:00 devchat_ask-0.0.7.dist-info/RECORD
-12 files, 1652588 bytes uncompressed, 1091251 bytes compressed:  34.0%
+Zip file size: 2133884 bytes, number of entries: 59
+-rw-r--r--  2.0 unx       62 b- defN 80-Jan-01 00:00 chat/README.md
+-rwxr-xr-x  2.0 unx    54331 b- defN 80-Jan-01 00:00 chat/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55979 b- defN 80-Jan-01 00:00 chat/ask_codebase/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54395 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    96524 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/simple_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    98430 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/stuff_dc_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54395 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   117916 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/embedding.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54411 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77223 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/base.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   144151 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/file.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   137883 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/function.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    97735 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/util.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54379 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    98695 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/file.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   157849 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/qdrant.cpython-311-darwin.so
+-rw-r--r--  2.0 unx      548 b- defN 80-Jan-01 00:00 chat/evaluation/qa/README.md
+-rwxr-xr-x  2.0 unx    54363 b- defN 80-Jan-01 00:00 chat/evaluation/qa/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77814 b- defN 80-Jan-01 00:00 chat/evaluation/qa/cli.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55163 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   117755 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/evaluate.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    95579 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/markdown.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77753 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/resume.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    78727 b- defN 80-Jan-01 00:00 chat/evaluation/qa/commands/show.cpython-311-darwin.so
+-rw-r--r--  2.0 unx    25583 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/devlake_qa_examples.json
+-rw-r--r--  2.0 unx    12247 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/devlake_test_set_mini.json
+-rw-r--r--  2.0 unx    18107 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/langchain_test_set.json
+-rw-r--r--  2.0 unx      848 b- defN 80-Jan-01 00:00 chat/evaluation/qa/data/dataset/mock.json
+-rwxr-xr-x  2.0 unx    74603 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    79239 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/base.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    97664 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/prototype_bot.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    79004 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/simple_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    79182 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/stuff_dc_qa.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77769 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluable/yes_no.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   155597 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluation.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55163 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77687 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/base.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    78350 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/correctness.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54443 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    55831 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/conf.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77117 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/judge_pair.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77343 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/judge_single.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    77018 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/llm_helper/rate_it.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    78121 b- defN 80-Jan-01 00:00 chat/evaluation/qa/evaluator/rating.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    96095 b- defN 80-Jan-01 00:00 chat/evaluation/qa/question_set.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   173961 b- defN 80-Jan-01 00:00 chat/evaluation/qa/report.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    96887 b- defN 80-Jan-01 00:00 chat/evaluation/qa/util.cpython-311-darwin.so
+-rw-r--r--  2.0 unx     4979 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/README.md
+-rwxr-xr-x  2.0 unx   141255 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/load.cpython-311-darwin.so
+-rw-r--r--  2.0 unx   407954 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/scores.csv
+-rw-r--r--  2.0 unx  1179453 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/data/code_search_net_eval/snippets.zip
+-rwxr-xr-x  2.0 unx    57562 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/example.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   195377 b- defN 80-Jan-01 00:00 chat/evaluation/retrieval/retrieval_eval.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    54347 b- defN 80-Jan-01 00:00 chat/util/__init__.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx    96700 b- defN 80-Jan-01 00:00 chat/util/decorator.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx   116071 b- defN 80-Jan-01 00:00 chat/util/misc.cpython-311-darwin.so
+-rw-r--r--  2.0 unx      704 b- defN 80-Jan-01 00:00 devchat_ask-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 devchat_ask-0.0.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     6560 b- defN 16-Jan-01 00:00 devchat_ask-0.0.8.dist-info/RECORD
+59 files, 5870987 bytes uncompressed, 2122994 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,37 +1,178 @@
+Filename: chat/README.md
+Comment: 
+
+Filename: chat/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/chains/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/chains/simple_qa.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/chains/stuff_dc_qa.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/indexing/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/indexing/embedding.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/indexing/loader/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/indexing/loader/base.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/indexing/loader/file.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/indexing/loader/function.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/indexing/util.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/store/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/store/file.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/ask_codebase/store/qdrant.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/README.md
+Comment: 
+
+Filename: chat/evaluation/qa/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/cli.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/commands/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/commands/evaluate.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/commands/markdown.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/commands/resume.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/commands/show.cpython-311-darwin.so
+Comment: 
+
 Filename: chat/evaluation/qa/data/dataset/devlake_qa_examples.json
 Comment: 
 
 Filename: chat/evaluation/qa/data/dataset/devlake_test_set_mini.json
 Comment: 
 
 Filename: chat/evaluation/qa/data/dataset/langchain_test_set.json
 Comment: 
 
 Filename: chat/evaluation/qa/data/dataset/mock.json
 Comment: 
 
-Filename: chat/evaluation/qa/README.md
+Filename: chat/evaluation/qa/evaluable/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/base.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/prototype_bot.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/simple_qa.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/stuff_dc_qa.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluable/yes_no.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluation.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/base.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/correctness.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/conf.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/judge_pair.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/judge_single.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/llm_helper/rate_it.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/evaluator/rating.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/question_set.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/report.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/qa/util.cpython-311-darwin.so
 Comment: 
 
 Filename: chat/evaluation/retrieval/data/code_search_net_eval/README.md
 Comment: 
 
+Filename: chat/evaluation/retrieval/data/code_search_net_eval/load.cpython-311-darwin.so
+Comment: 
+
 Filename: chat/evaluation/retrieval/data/code_search_net_eval/scores.csv
 Comment: 
 
 Filename: chat/evaluation/retrieval/data/code_search_net_eval/snippets.zip
 Comment: 
 
-Filename: chat/README.md
+Filename: chat/evaluation/retrieval/example.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/evaluation/retrieval/retrieval_eval.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/util/__init__.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/util/decorator.cpython-311-darwin.so
+Comment: 
+
+Filename: chat/util/misc.cpython-311-darwin.so
 Comment: 
 
-Filename: devchat_ask-0.0.7.dist-info/METADATA
+Filename: devchat_ask-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: devchat_ask-0.0.7.dist-info/WHEEL
+Filename: devchat_ask-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: devchat_ask-0.0.7.dist-info/RECORD
+Filename: devchat_ask-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chat/evaluation/qa/data/dataset/devlake_qa_examples.json

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

```diff
@@ -1,1621 +1,1599 @@
-00000000: 7b0d 0a20 2020 2022 6e61 6d65 223a 2022  {..    "name": "
-00000010: 4465 764c 616b 6522 2c0d 0a20 2020 2022  DevLake",..    "
-00000020: 6465 7363 7269 7074 696f 6e22 3a20 2245  description": "E
-00000030: 7861 6d70 6c65 2051 7565 7365 7469 6f6e  xample Quesetion
-00000040: 7320 616e 6420 416e 7377 6572 7320 666f  s and Answers fo
-00000050: 7220 4465 764c 616b 6522 2c0d 0a20 2020  r DevLake",..   
-00000060: 2022 6361 7365 7322 3a20 5b0d 0a20 2020   "cases": [..   
-00000070: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00000080: 2020 2020 2269 6422 3a20 2264 6576 6c61      "id": "devla
-00000090: 6b65 2d30 3122 2c0d 0a20 2020 2020 2020  ke-01",..       
-000000a0: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
-000000b0: 2022 486f 7720 6973 2074 6865 206c 6561   "How is the lea
-000000c0: 6420 7469 6d65 2066 6f72 2063 6861 6e67  d time for chang
-000000d0: 6573 2063 616c 6375 6c61 7465 643f 222c  es calculated?",
-000000e0: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-000000f0: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-00000100: 3a20 2254 6865 206c 6561 6420 7469 6d65  : "The lead time
-00000110: 2066 6f72 2063 6861 6e67 6573 2069 7320   for changes is 
-00000120: 6361 6c63 756c 6174 6564 2069 6e20 7468  calculated in th
-00000130: 6520 6043 616c 6375 6c61 7465 4368 616e  e `CalculateChan
-00000140: 6765 4c65 6164 5469 6d65 6020 6675 6e63  geLeadTime` func
-00000150: 7469 6f6e 2062 7920 666f 6c6c 6f77 696e  tion by followin
-00000160: 6720 7468 6573 6520 7374 6570 733a 5c6e  g these steps:\n
-00000170: 5c6e 312e 2047 6574 2070 756c 6c20 7265  \n1. Get pull re
-00000180: 7175 6573 7473 2062 7920 7468 6520 7072  quests by the pr
-00000190: 6f6a 6563 7420 6e61 6d65 2e5c 6e32 2e20  oject name.\n2. 
-000001a0: 466f 7220 6561 6368 2070 756c 6c20 7265  For each pull re
-000001b0: 7175 6573 742c 2067 6574 2074 6865 2066  quest, get the f
-000001c0: 6972 7374 2063 6f6d 6d69 7420 616e 6420  irst commit and 
-000001d0: 6361 6c63 756c 6174 6520 7468 6520 5052  calculate the PR
-000001e0: 2063 6f64 696e 6720 7469 6d65 2061 7320   coding time as 
-000001f0: 7468 6520 7469 6d65 2073 7061 6e20 6265  the time span be
-00000200: 7477 6565 6e20 7468 6520 6669 7273 7420  tween the first 
-00000210: 636f 6d6d 6974 2773 2061 7574 686f 7265  commit's authore
-00000220: 6420 6461 7465 2061 6e64 2074 6865 2070  d date and the p
-00000230: 756c 6c20 7265 7175 6573 7427 7320 6372  ull request's cr
-00000240: 6561 7465 6420 6461 7465 2e5c 6e33 2e20  eated date.\n3. 
-00000250: 4765 7420 7468 6520 6669 7273 7420 7265  Get the first re
-00000260: 7669 6577 2066 6f72 2074 6865 2070 756c  view for the pul
-00000270: 6c20 7265 7175 6573 7420 2865 7863 6c75  l request (exclu
-00000280: 6469 6e67 2063 6f6d 6d65 6e74 7320 6672  ding comments fr
-00000290: 6f6d 2074 6865 2050 5220 6372 6561 746f  om the PR creato
-000002a0: 7229 2061 6e64 2063 616c 6375 6c61 7465  r) and calculate
-000002b0: 2074 6865 2050 5220 7069 636b 7570 2074   the PR pickup t
-000002c0: 696d 6520 6173 2074 6865 2074 696d 6520  ime as the time 
-000002d0: 7370 616e 2062 6574 7765 656e 2074 6865  span between the
-000002e0: 2070 756c 6c20 7265 7175 6573 7427 7320   pull request's 
-000002f0: 6372 6561 7465 6420 6461 7465 2061 6e64  created date and
-00000300: 2074 6865 2066 6972 7374 2072 6576 6965   the first revie
-00000310: 7727 7320 6372 6561 7465 6420 6461 7465  w's created date
-00000320: 2e20 4361 6c63 756c 6174 6520 7468 6520  . Calculate the 
-00000330: 5052 2072 6576 6965 7720 7469 6d65 2061  PR review time a
-00000340: 7320 7468 6520 7469 6d65 2073 7061 6e20  s the time span 
-00000350: 6265 7477 6565 6e20 7468 6520 6669 7273  between the firs
-00000360: 7420 7265 7669 6577 2773 2063 7265 6174  t review's creat
-00000370: 6564 2064 6174 6520 616e 6420 7468 6520  ed date and the 
-00000380: 7075 6c6c 2072 6571 7565 7374 2773 206d  pull request's m
-00000390: 6572 6765 6420 6461 7465 2e5c 6e34 2e20  erged date.\n4. 
-000003a0: 4765 7420 7468 6520 6465 706c 6f79 6d65  Get the deployme
-000003b0: 6e74 2066 6f72 2074 6865 2070 756c 6c20  nt for the pull 
-000003c0: 7265 7175 6573 7420 7573 696e 6720 7468  request using th
-000003d0: 6520 6d65 7267 6520 636f 6d6d 6974 2053  e merge commit S
-000003e0: 4841 2061 6e64 2063 616c 6375 6c61 7465  HA and calculate
-000003f0: 2074 6865 2050 5220 6465 706c 6f79 2074   the PR deploy t
-00000400: 696d 6520 6173 2074 6865 2074 696d 6520  ime as the time 
-00000410: 7370 616e 2062 6574 7765 656e 2074 6865  span between the
-00000420: 2070 756c 6c20 7265 7175 6573 7427 7320   pull request's 
-00000430: 6d65 7267 6564 2064 6174 6520 616e 6420  merged date and 
-00000440: 7468 6520 6465 706c 6f79 6d65 6e74 2773  the deployment's
-00000450: 2066 696e 6973 6865 6420 6461 7465 2e5c   finished date.\
-00000460: 6e35 2e20 4361 6c63 756c 6174 6520 7468  n5. Calculate th
-00000470: 6520 5052 2063 7963 6c65 2074 696d 6520  e PR cycle time 
-00000480: 6279 2061 6464 696e 6720 7468 6520 5052  by adding the PR
-00000490: 2063 6f64 696e 6720 7469 6d65 2c20 5052   coding time, PR
-000004a0: 2064 7572 696e 6720 7469 6d65 2028 7469   during time (ti
-000004b0: 6d65 2073 7061 6e20 6265 7477 6565 6e20  me span between 
-000004c0: 7468 6520 7075 6c6c 2072 6571 7565 7374  the pull request
-000004d0: 2773 2063 7265 6174 6564 2064 6174 6520  's created date 
-000004e0: 616e 6420 6d65 7267 6564 2064 6174 6529  and merged date)
-000004f0: 2c20 616e 6420 5052 2064 6570 6c6f 7920  , and PR deploy 
-00000500: 7469 6d65 2e5c 6e5c 6e54 6865 2066 756e  time.\n\nThe fun
-00000510: 6374 696f 6e20 7265 7475 726e 7320 6120  ction returns a 
-00000520: 6050 726f 6a65 6374 5072 4d65 7472 6963  `ProjectPrMetric
-00000530: 6020 6f62 6a65 6374 2063 6f6e 7461 696e  ` object contain
-00000540: 696e 6720 7468 6520 6361 6c63 756c 6174  ing the calculat
-00000550: 6564 206c 6561 6420 7469 6d65 7320 666f  ed lead times fo
-00000560: 7220 6561 6368 2070 756c 6c20 7265 7175  r each pull requ
-00000570: 6573 7420 696e 2074 6865 2070 726f 6a65  est in the proje
-00000580: 6374 2e22 2c0d 0a20 2020 2020 2020 2020  ct.",..         
-00000590: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
-000005a0: 7274 6965 7322 3a20 5b5d 2c0d 0a20 2020  rties": [],..   
-000005b0: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
-000005c0: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-000005d0: 2020 2020 2022 6c65 7665 6c22 3a20 226d       "level": "m
-000005e0: 6964 220d 0a20 2020 2020 2020 2020 2020  id"..           
-000005f0: 207d 0d0a 2020 2020 2020 2020 7d2c 0d0a   }..        },..
-00000600: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00000610: 2020 2020 2020 2022 6964 223a 2022 6465         "id": "de
-00000620: 766c 616b 652d 3032 222c 0d0a 2020 2020  vlake-02",..    
-00000630: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
-00000640: 6e22 3a20 2257 6879 2063 616e 2074 6865  n": "Why can the
-00000650: 206c 6561 6420 7469 6d65 2066 6f72 2063   lead time for c
-00000660: 6861 6e67 6573 206d 6574 7269 6320 6265  hanges metric be
-00000670: 206e 756c 6c20 736f 6d65 7469 6d65 733f   null sometimes?
-00000680: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000690: 2272 6566 6572 656e 6365 5f61 6e73 7765  "reference_answe
-000006a0: 7222 3a20 2254 6865 206c 6561 6420 7469  r": "The lead ti
-000006b0: 6d65 2066 6f72 2063 6861 6e67 6573 206d  me for changes m
-000006c0: 6574 7269 6320 6361 6e20 6265 206e 756c  etric can be nul
-000006d0: 6c20 736f 6d65 7469 6d65 7320 6265 6361  l sometimes beca
-000006e0: 7573 6520 736f 6d65 206f 6620 7468 6520  use some of the 
-000006f0: 7469 6d65 2073 7061 6e73 2075 7365 6420  time spans used 
-00000700: 746f 2063 616c 6375 6c61 7465 2069 7420  to calculate it 
-00000710: 6d69 6768 7420 6265 206e 756c 6c2e 2049  might be null. I
-00000720: 6e20 7468 6520 6043 616c 6375 6c61 7465  n the `Calculate
-00000730: 4368 616e 6765 4c65 6164 5469 6d65 6020  ChangeLeadTime` 
-00000740: 6675 6e63 7469 6f6e 2c20 7468 6520 5052  function, the PR
-00000750: 2063 6f64 696e 6720 7469 6d65 2c20 5052   coding time, PR
-00000760: 2070 6963 6b75 7020 7469 6d65 2c20 5052   pickup time, PR
-00000770: 2072 6576 6965 7720 7469 6d65 2c20 616e   review time, an
-00000780: 6420 5052 2064 6570 6c6f 7920 7469 6d65  d PR deploy time
-00000790: 2061 7265 2063 616c 6375 6c61 7465 642e   are calculated.
-000007a0: 2049 6620 616e 7920 6f66 2074 6865 7365   If any of these
-000007b0: 2074 696d 6520 7370 616e 7320 6172 6520   time spans are 
-000007c0: 6e75 6c6c 206f 7220 6861 7665 206e 6567  null or have neg
-000007d0: 6174 6976 6520 7661 6c75 6573 2c20 7468  ative values, th
-000007e0: 6520 6669 6e61 6c20 5052 2063 7963 6c65  e final PR cycle
-000007f0: 2074 696d 6520 286c 6561 6420 7469 6d65   time (lead time
-00000800: 2066 6f72 2063 6861 6e67 6573 2920 6d69   for changes) mi
-00000810: 6768 7420 6e6f 7420 6265 2063 616c 6375  ght not be calcu
-00000820: 6c61 7465 642c 2072 6573 756c 7469 6e67  lated, resulting
-00000830: 2069 6e20 6120 6e75 6c6c 2076 616c 7565   in a null value
-00000840: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00000850: 2022 616e 7377 6572 5f70 726f 7065 7274   "answer_propert
-00000860: 6965 7322 3a20 5b5d 2c0d 0a20 2020 2020  ies": [],..     
-00000870: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
-00000880: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00000890: 2020 2022 6c65 7665 6c22 3a20 226c 6f77     "level": "low
-000008a0: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
-000008b0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-000008c0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-000008d0: 2020 2020 2022 6964 223a 2022 6465 766c       "id": "devl
-000008e0: 616b 652d 3033 222c 0d0a 2020 2020 2020  ake-03",..      
-000008f0: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00000900: 3a20 2243 616e 2079 6f75 2070 726f 7669  : "Can you provi
-00000910: 6465 2061 2068 6967 682d 6c65 7665 6c20  de a high-level 
-00000920: 6465 7363 7269 7074 696f 6e20 6f66 2044  description of D
-00000930: 6576 4c61 6b65 2773 2061 7263 6869 7465  evLake's archite
-00000940: 6374 7572 653f 222c 0d0a 2020 2020 2020  cture?",..      
-00000950: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
-00000960: 5f61 6e73 7765 7222 3a20 2244 6576 4c61  _answer": "DevLa
-00000970: 6b65 2063 6f6e 7369 7374 7320 6f66 2074  ke consists of t
-00000980: 6865 7365 206d 6169 6e20 636f 6d70 6f6e  hese main compon
-00000990: 656e 7473 3a20 5c6e 5c6e 312e 2043 6f6e  ents: \n\n1. Con
-000009a0: 6669 6720 5549 2c20 5c6e 5c6e 322e 2041  fig UI, \n\n2. A
-000009b0: 5049 2053 6572 7665 722c 205c 6e5c 6e33  PI Server, \n\n3
-000009c0: 2e20 5275 6e6e 6572 2c20 5c6e 5c6e 342e  . Runner, \n\n4.
-000009d0: 2044 6174 6162 6173 652c 205c 6e5c 6e35   Database, \n\n5
-000009e0: 2e20 506c 7567 696e 732c 205c 6e5c 6e36  . Plugins, \n\n6
-000009f0: 2e20 4461 7368 626f 6172 6473 2e20 4974  . Dashboards. It
-00000a00: 7320 6461 7461 2066 6c6f 7720 6861 7320  s data flow has 
-00000a10: 7468 7265 6520 6c61 7973 6572 733a 205c  three laysers: \
-00000a20: 6e5c 6e31 2e20 5261 7720 6c61 7965 722c  n\n1. Raw layer,
-00000a30: 205c 6e5c 6e32 2c20 546f 6f6c 206c 6179   \n\n2, Tool lay
-00000a40: 6572 2c20 5c6e 5c6e 332e 2044 6f6d 6169  er, \n\n3. Domai
-00000a50: 6e20 6c61 7965 722e 2046 6f72 2064 6574  n layer. For det
-00000a60: 6169 6c65 6420 6578 706c 616e 6174 696f  ailed explanatio
-00000a70: 6e73 2c20 706c 6561 7365 2072 6566 6572  ns, please refer
-00000a80: 2074 6f20 7468 6973 2064 6f63 3a20 6874   to this doc: ht
-00000a90: 7470 733a 2f2f 6465 766c 616b 652e 6170  tps://devlake.ap
-00000aa0: 6163 6865 2e6f 7267 2f64 6f63 732f 4f76  ache.org/docs/Ov
-00000ab0: 6572 7669 6577 2f41 7263 6869 7465 6374  erview/Architect
-00000ac0: 7572 6522 2c0d 0a20 2020 2020 2020 2020  ure",..         
-00000ad0: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
-00000ae0: 7274 6965 7322 3a20 5b5d 2c0d 0a20 2020  rties": [],..   
-00000af0: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
-00000b00: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00000b10: 2020 2020 2022 6c65 7665 6c22 3a20 2268       "level": "h
-00000b20: 6967 6822 0d0a 2020 2020 2020 2020 2020  igh"..          
-00000b30: 2020 7d0d 0a20 2020 2020 2020 207d 2c0d    }..        },.
-00000b40: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-00000b50: 2020 2020 2020 2020 2269 6422 3a20 2264          "id": "d
-00000b60: 6576 6c61 6b65 2d30 3422 2c0d 0a20 2020  evlake-04",..   
-00000b70: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
-00000b80: 6f6e 223a 2022 5768 6174 2064 6174 6120  on": "What data 
-00000b90: 646f 6573 2074 6865 2041 7a75 7265 2044  does the Azure D
-00000ba0: 6576 4f70 7320 706c 7567 696e 2063 6f6c  evOps plugin col
-00000bb0: 6c65 6374 3f22 2c0d 0a20 2020 2020 2020  lect?",..       
-00000bc0: 2020 2020 2022 7265 6665 7265 6e63 655f       "reference_
-00000bd0: 616e 7377 6572 223a 2022 5468 6520 417a  answer": "The Az
-00000be0: 7572 6520 4465 764f 7073 2070 6c75 6769  ure DevOps plugi
-00000bf0: 6e20 636f 6c6c 6563 7473 2064 6174 6120  n collects data 
-00000c00: 7265 6c61 7465 6420 746f 2047 6974 2072  related to Git r
-00000c10: 6570 6f73 6974 6f72 6965 732c 2047 6974  epositories, Git
-00000c20: 2070 756c 6c20 7265 7175 6573 7473 2c20   pull requests, 
-00000c30: 4769 7420 7075 6c6c 2072 6571 7565 7374  Git pull request
-00000c40: 2063 6f6d 6d69 7473 2c20 6275 696c 6473   commits, builds
-00000c50: 2c20 616e 6420 6a6f 6273 2e20 5370 6563  , and jobs. Spec
-00000c60: 6966 6963 616c 6c79 2c20 6974 2063 6f6c  ifically, it col
-00000c70: 6c65 6374 7320 696e 666f 726d 6174 696f  lects informatio
-00000c80: 6e20 7375 6368 2061 733a 5c6e 5c6e 312e  n such as:\n\n1.
-00000c90: 2047 6974 5075 6c6c 5265 7175 6573 7473   GitPullRequests
-00000ca0: 3a20 4261 7365 2072 6570 6f73 6974 6f72  : Base repositor
-00000cb0: 7920 4944 2c20 6865 6164 2072 6570 6f73  y ID, head repos
-00000cc0: 6974 6f72 7920 4944 2c20 7374 6174 7573  itory ID, status
-00000cd0: 2c20 6f72 6967 696e 616c 2073 7461 7475  , original statu
-00000ce0: 732c 2074 6974 6c65 2c20 6465 7363 7269  s, title, descri
-00000cf0: 7074 696f 6e2c 2055 524c 2c20 6175 7468  ption, URL, auth
-00000d00: 6f72 206e 616d 652c 2061 7574 686f 7220  or name, author 
-00000d10: 4944 2c20 7075 6c6c 2072 6571 7565 7374  ID, pull request
-00000d20: 206b 6579 2c20 6372 6561 7465 6420 6461   key, created da
-00000d30: 7465 2c20 6d65 7267 6564 2064 6174 652c  te, merged date,
-00000d40: 2063 6c6f 7365 6420 6461 7465 2c20 7479   closed date, ty
-00000d50: 7065 2c20 636f 6d70 6f6e 656e 742c 206d  pe, component, m
-00000d60: 6572 6765 2063 6f6d 6d69 7420 5348 412c  erge commit SHA,
-00000d70: 2068 6561 6420 7265 6665 7265 6e63 652c   head reference,
-00000d80: 2062 6173 6520 7265 6665 7265 6e63 652c   base reference,
-00000d90: 2068 6561 6420 636f 6d6d 6974 2053 4841   head commit SHA
-00000da0: 2c20 616e 6420 6261 7365 2063 6f6d 6d69  , and base commi
-00000db0: 7420 5348 412e 5c6e 5c6e 322e 2047 6974  t SHA.\n\n2. Git
-00000dc0: 5075 6c6c 5265 7175 6573 7443 6f6d 6d69  PullRequestCommi
-00000dd0: 7473 3a20 436f 6d6d 6974 2053 4841 2028  ts: Commit SHA (
-00000de0: 636f 6d6d 6974 5f69 6429 2c20 7075 6c6c  commit_id), pull
-00000df0: 2072 6571 7565 7374 2049 442c 2063 6f6d   request ID, com
-00000e00: 6d69 7420 6175 7468 6f72 206e 616d 6520  mit author name 
-00000e10: 2861 7574 686f 725f 6e61 6d65 292c 2063  (author_name), c
-00000e20: 6f6d 6d69 7420 6175 7468 6f72 2065 6d61  ommit author ema
-00000e30: 696c 2028 6175 7468 6f72 5f65 6d61 696c  il (author_email
-00000e40: 292c 2061 6e64 2063 6f6d 6d69 7420 6175  ), and commit au
-00000e50: 7468 6f72 6564 2064 6174 6520 2861 7574  thored date (aut
-00000e60: 686f 725f 6461 7465 292e 5c6e 5c6e 332e  hor_date).\n\n3.
-00000e70: 2042 7569 6c64 733a 2042 7569 6c64 2773   Builds: Build's
-00000e80: 206e 616d 652c 2073 7461 7475 732c 2063   name, status, c
-00000e90: 7265 6174 6564 2064 6174 652c 2066 696e  reated date, fin
-00000ea0: 6973 6865 6420 6461 7465 2c20 7265 7375  ished date, resu
-00000eb0: 6c74 2c20 6475 7261 7469 6f6e 2069 6e20  lt, duration in 
-00000ec0: 7365 636f 6e64 732c 2065 6e76 6972 6f6e  seconds, environ
-00000ed0: 6d65 6e74 2c20 7479 7065 2c20 616e 6420  ment, type, and 
-00000ee0: 6f74 6865 7220 7265 6c61 7465 6420 6465  other related de
-00000ef0: 7461 696c 7320 6c69 6b65 2063 6f6d 6d69  tails like commi
-00000f00: 7420 5348 412c 2062 7261 6e63 682c 2072  t SHA, branch, r
-00000f10: 6570 6f73 6974 6f72 7920 4944 2c20 616e  epository ID, an
-00000f20: 6420 7265 706f 7369 746f 7279 2055 524c  d repository URL
-00000f30: 2e5c 6e5c 6e34 2e20 4a6f 6273 3a20 4a6f  .\n\n4. Jobs: Jo
-00000f40: 6220 4944 2c20 6e61 6d65 2c20 6275 696c  b ID, name, buil
-00000f50: 6420 4944 2c20 7374 6174 7573 2c20 7374  d ID, status, st
-00000f60: 6172 7420 7469 6d65 2c20 6669 6e69 7368  art time, finish
-00000f70: 2074 696d 652c 2072 6573 756c 742c 2074   time, result, t
-00000f80: 7970 652c 2064 7572 6174 696f 6e20 696e  ype, duration in
-00000f90: 2073 6563 6f6e 6473 2c20 656e 7669 726f   seconds, enviro
-00000fa0: 6e6d 656e 742c 2061 6e64 2043 4943 4420  nment, and CICD 
-00000fb0: 7363 6f70 6520 4944 2e22 2c0d 0a20 2020  scope ID.",..   
-00000fc0: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
-00000fd0: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
-00000fe0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000ff0: 6e6f 7465 7322 3a20 7b0d 0a20 2020 2020  notes": {..     
-00001000: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
-00001010: 6c22 3a20 226d 6964 220d 0a20 2020 2020  l": "mid"..     
-00001020: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00001030: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
-00001040: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
-00001050: 223a 2022 6465 766c 616b 652d 3035 222c  ": "devlake-05",
-00001060: 0d0a 2020 2020 2020 2020 2020 2020 2271  ..            "q
-00001070: 7565 7374 696f 6e22 3a20 2257 6861 7420  uestion": "What 
-00001080: 6172 6520 7468 6520 6665 6174 7572 6573  are the features
-00001090: 206f 6620 4465 764c 616b 653f 222c 0d0a   of DevLake?",..
-000010a0: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
-000010b0: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
-000010c0: 2241 7061 6368 6520 4465 764c 616b 6520  "Apache DevLake 
-000010d0: 6973 2061 6e20 6f70 656e 2d73 6f75 7263  is an open-sourc
-000010e0: 6520 6465 7620 6461 7461 2070 6c61 7466  e dev data platf
-000010f0: 6f72 6d20 746f 2069 6e67 6573 742c 2061  orm to ingest, a
-00001100: 6e61 6c79 7a65 2c20 616e 6420 7669 7375  nalyze, and visu
-00001110: 616c 697a 6520 6672 6167 6d65 6e74 6564  alize fragmented
-00001120: 2064 6174 6120 6672 6f6d 2044 6576 4f70   data from DevOp
-00001130: 7320 746f 6f6c 732c 2065 7874 7261 6374  s tools, extract
-00001140: 696e 6720 696e 7369 6768 7473 2066 6f72  ing insights for
-00001150: 2065 6e67 696e 6565 7269 6e67 2065 7863   engineering exc
-00001160: 656c 6c65 6e63 652c 2064 6576 656c 6f70  ellence, develop
-00001170: 6572 2065 7870 6572 6965 6e63 652c 2061  er experience, a
-00001180: 6e64 2063 6f6d 6d75 6e69 7479 2067 726f  nd community gro
-00001190: 7774 682e 2046 6f72 2061 2063 6f6d 706c  wth. For a compl
-000011a0: 6574 6520 6c69 7374 206f 6620 6665 6174  ete list of feat
-000011b0: 7572 6573 2c20 706c 6561 7365 2076 6973  ures, please vis
-000011c0: 6974 2074 6865 2041 7061 6368 6520 4465  it the Apache De
-000011d0: 764c 616b 6520 7765 6273 6974 6520 6f72  vLake website or
-000011e0: 2070 726f 7669 6465 206d 6f72 6520 696e   provide more in
-000011f0: 666f 726d 6174 696f 6e2e 222c 0d0a 2020  formation.",..  
-00001200: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
-00001210: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
-00001220: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00001230: 226e 6f74 6573 223a 207b 0d0a 2020 2020  "notes": {..    
-00001240: 2020 2020 2020 2020 2020 2020 226c 6576              "lev
-00001250: 656c 223a 2022 6c6f 7722 0d0a 2020 2020  el": "low"..    
-00001260: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00001270: 2020 207d 2c0d 0a20 2020 2020 2020 207b     },..        {
-00001280: 0d0a 2020 2020 2020 2020 2020 2020 2269  ..            "i
-00001290: 6422 3a20 2264 6576 6c61 6b65 2d30 3622  d": "devlake-06"
-000012a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000012b0: 7175 6573 7469 6f6e 223a 2022 5768 6174  question": "What
-000012c0: 2061 7265 2074 6865 2075 7365 2063 6173   are the use cas
-000012d0: 6573 206f 6620 4465 764c 616b 653f 222c  es of DevLake?",
-000012e0: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-000012f0: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-00001300: 3a20 2244 6576 4c61 6b65 2069 7320 6465  : "DevLake is de
-00001310: 7369 676e 6564 2074 6f20 6865 6c70 2064  signed to help d
-00001320: 6576 656c 6f70 6572 7320 616e 6420 7465  evelopers and te
-00001330: 616d 7320 6d61 6e61 6765 2061 6e64 2061  ams manage and a
-00001340: 6e61 6c79 7a65 2074 6865 6972 2073 6f66  nalyze their sof
-00001350: 7477 6172 6520 6465 7665 6c6f 706d 656e  tware developmen
-00001360: 7420 6461 7461 2e20 5573 6520 6361 7365  t data. Use case
-00001370: 7320 666f 7220 4465 764c 616b 6520 696e  s for DevLake in
-00001380: 636c 7564 653a 5c6e 5c6e 312e 2043 656e  clude:\n\n1. Cen
-00001390: 7472 616c 697a 696e 6720 6461 7461 2066  tralizing data f
-000013a0: 726f 6d20 7661 7269 6f75 7320 6465 7665  rom various deve
-000013b0: 6c6f 706d 656e 7420 746f 6f6c 7320 616e  lopment tools an
-000013c0: 6420 706c 6174 666f 726d 732c 2073 7563  d platforms, suc
-000013d0: 6820 6173 2047 6974 4875 622c 2047 6974  h as GitHub, Git
-000013e0: 4c61 622c 204a 6972 612c 2061 6e64 206d  Lab, Jira, and m
-000013f0: 6f72 652c 2069 6e74 6f20 6120 7369 6e67  ore, into a sing
-00001400: 6c65 2064 6174 6120 6c61 6b65 2e5c 6e32  le data lake.\n2
-00001410: 2e20 456e 6162 6c69 6e67 2061 6476 616e  . Enabling advan
-00001420: 6365 6420 616e 616c 7974 6963 7320 616e  ced analytics an
-00001430: 6420 696e 7369 6768 7473 206f 6e20 6465  d insights on de
-00001440: 7665 6c6f 706d 656e 7420 6461 7461 2c20  velopment data, 
-00001450: 7375 6368 2061 7320 636f 6465 2071 7561  such as code qua
-00001460: 6c69 7479 2c20 7465 616d 2070 6572 666f  lity, team perfo
-00001470: 726d 616e 6365 2c20 616e 6420 7072 6f6a  rmance, and proj
-00001480: 6563 7420 7072 6f67 7265 7373 2e5c 6e33  ect progress.\n3
-00001490: 2e20 4661 6369 6c69 7461 7469 6e67 2074  . Facilitating t
-000014a0: 6865 2063 7265 6174 696f 6e20 6f66 2063  he creation of c
-000014b0: 7573 746f 6d20 706c 7567 696e 7320 746f  ustom plugins to
-000014c0: 2069 6e74 6567 7261 7465 2077 6974 6820   integrate with 
-000014d0: 6164 6469 7469 6f6e 616c 2064 6174 6120  additional data 
-000014e0: 736f 7572 6365 7320 6f72 2074 6f6f 6c73  sources or tools
-000014f0: 2c20 616c 6c6f 7769 6e67 2066 6f72 2067  , allowing for g
-00001500: 7265 6174 6572 2066 6c65 7869 6269 6c69  reater flexibili
-00001510: 7479 2061 6e64 2065 7874 656e 7369 6269  ty and extensibi
-00001520: 6c69 7479 2e5c 6e34 2e20 5375 7070 6f72  lity.\n4. Suppor
-00001530: 7469 6e67 2074 6865 2064 6576 656c 6f70  ting the develop
-00001540: 6d65 6e74 206f 6620 6375 7374 6f6d 2064  ment of custom d
-00001550: 6173 6862 6f61 7264 7320 616e 6420 7265  ashboards and re
-00001560: 706f 7274 7320 746f 2076 6973 7561 6c69  ports to visuali
-00001570: 7a65 2061 6e64 206d 6f6e 6974 6f72 2064  ze and monitor d
-00001580: 6576 656c 6f70 6d65 6e74 206d 6574 7269  evelopment metri
-00001590: 6373 222c 0d0a 2020 2020 2020 2020 2020  cs",..          
-000015a0: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
-000015b0: 7469 6573 223a 205b 5d2c 0d0a 2020 2020  ties": [],..    
-000015c0: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
-000015d0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000015e0: 2020 2020 226c 6576 656c 223a 2022 6c6f      "level": "lo
-000015f0: 7722 0d0a 2020 2020 2020 2020 2020 2020  w"..            
-00001600: 7d0d 0a20 2020 2020 2020 207d 2c0d 0a20  }..        },.. 
-00001610: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00001620: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
-00001630: 6c61 6b65 2d30 3722 2c0d 0a20 2020 2020  lake-07",..     
-00001640: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
-00001650: 223a 2022 486f 7720 6361 6e20 4920 636f  ": "How can I co
-00001660: 6e74 7269 6275 7465 2074 6f20 4465 764c  ntribute to DevL
-00001670: 616b 653f 222c 0d0a 2020 2020 2020 2020  ake?",..        
-00001680: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
-00001690: 6e73 7765 7222 3a20 2259 6f75 2063 616e  nswer": "You can
-000016a0: 2063 6f6e 7472 6962 7574 6520 746f 2044   contribute to D
-000016b0: 6576 4c61 6b65 2069 6e20 7365 7665 7261  evLake in severa
-000016c0: 6c20 7761 7973 3a5c 6e5c 6e31 2e20 4372  l ways:\n\n1. Cr
-000016d0: 6561 7465 2061 6e20 4973 7375 653a 2052  eate an Issue: R
-000016e0: 6570 6f72 7420 6120 6275 6720 6f72 2066  eport a bug or f
-000016f0: 6561 7475 7265 2072 6571 7565 7374 2074  eature request t
-00001700: 6f20 4170 6163 6865 2044 6576 4c61 6b65  o Apache DevLake
-00001710: 2e5c 6e32 2e20 5375 626d 6974 2061 2050  .\n2. Submit a P
-00001720: 5220 2850 756c 6c20 5265 7175 6573 7429  R (Pull Request)
-00001730: 3a20 5374 6172 7420 7769 7468 2067 6f6f  : Start with goo
-00001740: 6420 6669 7273 7420 6973 7375 6573 206f  d first issues o
-00001750: 7220 6973 7375 6573 2077 6974 6820 6e6f  r issues with no
-00001760: 2061 7373 6967 6e65 6573 2e20 5265 6164   assignees. Read
-00001770: 2074 6872 6f75 6768 2074 6865 205b 436f   through the [Co
-00001780: 6e74 7269 6275 7469 6e67 2044 6f63 756d  ntributing Docum
-00001790: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-000017a0: 2f2f 6465 766c 616b 652e 6170 6163 6865  //devlake.apache
-000017b0: 2e6f 7267 2f63 6f6d 6d75 6e69 7479 2f29  .org/community/)
-000017c0: 2c20 6164 6420 7265 6c65 7661 6e74 2074  , add relevant t
-000017d0: 6573 7473 2c20 646f 6375 6d65 6e74 6174  ests, documentat
-000017e0: 696f 6e2c 2061 6e64 206c 6162 656c 7320  ion, and labels 
-000017f0: 746f 2074 6865 2050 522e 5c6e 332e 204a  to the PR.\n3. J
-00001800: 6f69 6e20 4d61 696c 696e 6720 6c69 7374  oin Mailing list
-00001810: 3a20 496e 6974 6961 7465 206f 7220 7061  : Initiate or pa
-00001820: 7274 6963 6970 6174 6520 696e 2070 726f  rticipate in pro
-00001830: 6a65 6374 2064 6973 6375 7373 696f 6e73  ject discussions
-00001840: 206f 6e20 7468 6520 6d61 696c 696e 6720   on the mailing 
-00001850: 6c69 7374 2e5c 6e34 2e20 5772 6974 6520  list.\n4. Write 
-00001860: 6120 426c 6f67 3a20 5772 6974 6520 6120  a Blog: Write a 
-00001870: 626c 6f67 2074 6f20 7368 6172 6520 796f  blog to share yo
-00001880: 7572 2075 7365 2063 6173 6573 2061 626f  ur use cases abo
-00001890: 7574 2041 7061 6368 6520 4465 764c 616b  ut Apache DevLak
-000018a0: 652e 5c6e 352e 2043 6f6e 7472 6962 7574  e.\n5. Contribut
-000018b0: 6520 6120 506c 7567 696e 3a20 4164 6420  e a Plugin: Add 
-000018c0: 6120 706c 7567 696e 2074 6f20 696e 7465  a plugin to inte
-000018d0: 6772 6174 6520 4170 6163 6865 2044 6576  grate Apache Dev
-000018e0: 4c61 6b65 2077 6974 6820 6d6f 7265 2064  Lake with more d
-000018f0: 6174 6120 736f 7572 6365 7320 666f 7220  ata sources for 
-00001900: 7468 6520 636f 6d6d 756e 6974 792e 5c6e  the community.\n
-00001910: 5c6e 506c 6561 7365 2072 6561 6420 7468  \nPlease read th
-00001920: 6520 5b63 6f6e 7472 6962 7574 696f 6e20  e [contribution 
-00001930: 6775 6964 656c 696e 6573 5d28 6874 7470  guidelines](http
-00001940: 733a 2f2f 6465 766c 616b 652e 6170 6163  s://devlake.apac
-00001950: 6865 2e6f 7267 2f63 6f6d 6d75 6e69 7479  he.org/community
-00001960: 2920 6265 666f 7265 2079 6f75 206d 616b  ) before you mak
-00001970: 6520 6120 636f 6e74 7269 6275 7469 6f6e  e a contribution
-00001980: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00001990: 2022 616e 7377 6572 5f70 726f 7065 7274   "answer_propert
-000019a0: 6965 7322 3a20 5b5d 2c0d 0a20 2020 2020  ies": [],..     
-000019b0: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
-000019c0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000019d0: 2020 2022 6c65 7665 6c22 3a20 226c 6f77     "level": "low
-000019e0: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
-000019f0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00001a00: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00001a10: 2020 2020 2022 6964 223a 2022 6465 766c       "id": "devl
-00001a20: 616b 652d 3038 222c 0d0a 2020 2020 2020  ake-08",..      
-00001a30: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00001a40: 3a20 2244 6f65 7320 4465 764c 616b 6527  : "Does DevLake'
-00001a50: 7320 4769 7448 7562 2070 6c75 6769 6e20  s GitHub plugin 
-00001a60: 7375 7070 6f72 7420 696e 6372 656d 656e  support incremen
-00001a70: 7461 6c20 7379 6e63 3f22 2c0d 0a20 2020  tal sync?",..   
-00001a80: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-00001a90: 6e63 655f 616e 7377 6572 223a 2022 5965  nce_answer": "Ye
-00001aa0: 732e 2044 6576 4c61 6b65 2773 2047 6974  s. DevLake's Git
-00001ab0: 4875 6220 706c 7567 696e 2073 7570 706f  Hub plugin suppo
-00001ac0: 7274 7320 696e 6372 656d 656e 7461 6c20  rts incremental 
-00001ad0: 7379 6e63 2e20 496e 2074 6865 2063 6f64  sync. In the cod
-00001ae0: 652c 2079 6f75 2063 616e 2073 6565 2074  e, you can see t
-00001af0: 6865 2066 6f6c 6c6f 7769 6e67 206c 696e  he following lin
-00001b00: 653a 5c6e 5c6e 6069 6e63 7265 6d65 6e74  e:\n\n`increment
-00001b10: 616c 203a 3d20 636f 6c6c 6563 746f 7257  al := collectorW
-00001b20: 6974 6853 7461 7465 2e49 7349 6e63 7265  ithState.IsIncre
-00001b30: 6d65 6e74 616c 2829 605c 6e5c 6e54 6869  mental()`\n\nThi
-00001b40: 7320 6c69 6e65 2063 6865 636b 7320 6966  s line checks if
-00001b50: 2074 6865 2063 6f6c 6c65 6374 6f72 2069   the collector i
-00001b60: 7320 7275 6e6e 696e 6720 696e 2069 6e63  s running in inc
-00001b70: 7265 6d65 6e74 616c 206d 6f64 652e 222c  remental mode.",
-00001b80: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-00001b90: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-00001ba0: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-00001bb0: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 226c 6576 656c 223a 2022 6d69 6422 0d0a  "level": "mid"..
-00001be0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00001bf0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00001c00: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00001c10: 2020 2269 6422 3a20 2264 6576 6c61 6b65    "id": "devlake
-00001c20: 2d30 3922 2c0d 0a20 2020 2020 2020 2020  -09",..         
-00001c30: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
-00001c40: 486f 7720 6361 6e20 4920 6372 6561 7465  How can I create
-00001c50: 2044 6576 4c61 6b65 2070 6c75 6769 6e73   DevLake plugins
-00001c60: 2069 6e20 5079 7468 6f6e 3f22 2c0d 0a20   in Python?",.. 
-00001c70: 2020 2020 2020 2020 2020 2022 7265 6665             "refe
-00001c80: 7265 6e63 655f 616e 7377 6572 223a 2022  rence_answer": "
-00001c90: 546f 2063 7265 6174 6520 6120 4465 764c  To create a DevL
-00001ca0: 616b 6520 706c 7567 696e 2069 6e20 5079  ake plugin in Py
-00001cb0: 7468 6f6e 2c20 666f 6c6c 6f77 2074 6865  thon, follow the
-00001cc0: 7365 2073 7465 7073 3a5c 6e5c 6e31 2e20  se steps:\n\n1. 
-00001cd0: 4d61 6b65 2073 7572 6520 796f 7520 6861  Make sure you ha
-00001ce0: 7665 205b 506f 6574 7279 5d28 6874 7470  ve [Poetry](http
-00001cf0: 733a 2f2f 7079 7468 6f6e 2d70 6f65 7472  s://python-poetr
-00001d00: 792e 6f72 672f 646f 6373 2f23 696e 7374  y.org/docs/#inst
-00001d10: 616c 6c61 7469 6f6e 2920 696e 7374 616c  allation) instal
-00001d20: 6c65 642e 5c6e 322e 204d 6f76 6520 746f  led.\n2. Move to
-00001d30: 2060 7079 7468 6f6e 2f70 6c75 6769 6e73   `python/plugins
-00001d40: 6020 616e 6420 6578 6563 7574 6520 6070  ` and execute `p
-00001d50: 6f65 7472 7920 6e65 7720 6d79 706c 7567  oetry new myplug
-00001d60: 696e 602e 2054 6869 7320 7769 6c6c 2067  in`. This will g
-00001d70: 656e 6572 6174 6520 6120 6e65 7720 6469  enerate a new di
-00001d80: 7265 6374 6f72 7920 666f 7220 796f 7572  rectory for your
-00001d90: 2070 6c75 6769 6e2e 5c6e 332e 2049 6e20   plugin.\n3. In 
-00001da0: 7468 6520 6070 7970 726f 6a65 6374 2e74  the `pyproject.t
-00001db0: 6f6d 6c60 2066 696c 652c 2061 6464 2074  oml` file, add t
-00001dc0: 6865 2066 6f6c 6c6f 7769 6e67 206c 696e  he following lin
-00001dd0: 6520 6174 2074 6865 2065 6e64 206f 6620  e at the end of 
-00001de0: 7468 6520 605b 746f 6f6c 2e70 6f65 7472  the `[tool.poetr
-00001df0: 792e 6465 7065 6e64 656e 6369 6573 5d60  y.dependencies]`
-00001e00: 2073 6563 7469 6f6e 3a5c 6e60 6060 5c6e   section:\n```\n
-00001e10: 7079 6465 766c 616b 6520 3d20 7b20 7061  pydevlake = { pa
-00001e20: 7468 203d 205c 222e 2e2f 2e2e 2f70 7964  th = \"../../pyd
-00001e30: 6576 6c61 6b65 5c22 2c20 6465 7665 6c6f  evlake\", develo
-00001e40: 7020 3d20 7472 7565 207d 5c6e 6060 605c  p = true }\n```\
-00001e50: 6e34 2e20 5275 6e20 6070 6f65 7472 7920  n4. Run `poetry 
-00001e60: 696e 7374 616c 6c60 2e5c 6e35 2e20 4372  install`.\n5. Cr
-00001e70: 6561 7465 2061 2060 6d61 696e 2e70 7960  eate a `main.py`
-00001e80: 2066 696c 6520 7769 7468 2074 6865 206e   file with the n
-00001e90: 6563 6573 7361 7279 2063 6f6e 7465 6e74  ecessary content
-00001ea0: 2c20 696e 636c 7564 696e 6720 636c 6173  , including clas
-00001eb0: 7365 7320 666f 7220 636f 6e6e 6563 7469  ses for connecti
-00001ec0: 6f6e 2c20 7472 616e 7366 6f72 6d61 7469  on, transformati
-00001ed0: 6f6e 2072 756c 652c 2074 6f6f 6c20 7363  on rule, tool sc
-00001ee0: 6f70 652c 2061 6e64 2070 6c75 6769 6e2e  ope, and plugin.
-00001ef0: 5c6e 362e 2043 7265 6174 6520 7368 656c  \n6. Create shel
-00001f00: 6c20 7363 7269 7074 7320 6062 7569 6c64  l scripts `build
-00001f10: 2e73 6860 2061 6e64 2060 7275 6e2e 7368  .sh` and `run.sh
-00001f20: 6020 696e 2074 6865 2070 6c75 6769 6e20  ` in the plugin 
-00001f30: 726f 6f74 2064 6972 6563 746f 7279 2074  root directory t
-00001f40: 6f20 6275 696c 6420 616e 6420 7275 6e20  o build and run 
-00001f50: 7468 6520 706c 7567 696e 2e5c 6e37 2e20  the plugin.\n7. 
-00001f60: 4465 6669 6e65 2063 6f6e 6e65 6374 696f  Define connectio
-00001f70: 6e20 7061 7261 6d65 7465 7273 2c20 7472  n parameters, tr
-00001f80: 616e 7366 6f72 6d61 7469 6f6e 2072 756c  ansformation rul
-00001f90: 6520 7061 7261 6d65 7465 7273 2c20 616e  e parameters, an
-00001fa0: 6420 746f 6f6c 2073 636f 7065 2074 7970  d tool scope typ
-00001fb0: 652e 5c6e 382e 2049 6d70 6c65 6d65 6e74  e.\n8. Implement
-00001fc0: 206d 6574 686f 6473 206c 696b 6520 6064   methods like `d
-00001fd0: 6f6d 6169 6e5f 7363 6f70 6573 602c 2060  omain_scopes`, `
-00001fe0: 7265 6d6f 7465 5f73 636f 7065 602c 2060  remote_scope`, `
-00001ff0: 7265 6d6f 7465 5f73 636f 7065 5f67 726f  remote_scope_gro
-00002000: 7570 7360 2c20 616e 6420 6074 6573 745f  ups`, and `test_
-00002010: 636f 6e6e 6563 7469 6f6e 602e 5c6e 392e  connection`.\n9.
-00002020: 2041 6464 2061 206e 6577 2064 6174 6120   Add a new data 
-00002030: 7374 7265 616d 2062 7920 6372 6561 7469  stream by creati
-00002040: 6e67 2061 2074 6f6f 6c20 6d6f 6465 6c2c  ng a tool model,
-00002050: 2073 7472 6561 6d20 636c 6173 732c 2061   stream class, a
-00002060: 6e64 2041 5049 2077 7261 7070 6572 2e5c  nd API wrapper.\
-00002070: 6e31 302e 2049 6d70 6c65 6d65 6e74 206d  n10. Implement m
-00002080: 6574 686f 6473 206c 696b 6520 6063 6f6c  ethods like `col
-00002090: 6c65 6374 602c 2060 6578 7472 6163 7460  lect`, `extract`
-000020a0: 2c20 616e 6420 6063 6f6e 7665 7274 6020  , and `convert` 
-000020b0: 666f 7220 7468 6520 7374 7265 616d 2063  for the stream c
-000020c0: 6c61 7373 2e5c 6e31 312e 2049 6620 6e65  lass.\n11. If ne
-000020d0: 6564 6564 2c20 6372 6561 7465 2073 7562  eded, create sub
-000020e0: 7374 7265 616d 7320 666f 7220 6869 6572  streams for hier
-000020f0: 6172 6368 6963 616c 2064 6174 6120 736f  archical data so
-00002100: 7572 6365 732e 5c6e 3132 2e20 5465 7374  urces.\n12. Test
-00002110: 2074 6865 2070 6c75 6769 6e20 7374 616e   the plugin stan
-00002120: 6461 6c6f 6e65 2075 7369 6e67 2074 6865  dalone using the
-00002130: 2060 6d61 696e 2e70 7960 2066 696c 6520   `main.py` file 
-00002140: 7769 7468 2064 6966 6665 7265 6e74 2063  with different c
-00002150: 6f6d 6d61 6e64 732e 5c6e 3133 2e20 5772  ommands.\n13. Wr
-00002160: 6974 6520 756e 6974 2d74 6573 7473 2066  ite unit-tests f
-00002170: 6f72 2079 6f75 7220 706c 7567 696e 2063  or your plugin c
-00002180: 6f64 652c 2077 6974 6820 7465 7374 2066  ode, with test f
-00002190: 696c 6573 2065 6e64 696e 6720 696e 2060  iles ending in `
-000021a0: 5f74 6573 742e 7079 602e 5c6e 5c6e 4865  _test.py`.\n\nHe
-000021b0: 7265 2773 2061 2067 656e 6572 616c 206f  re's a general o
-000021c0: 7574 6c69 6e65 206f 6620 6120 4465 764c  utline of a DevL
-000021d0: 616b 6520 706c 7567 696e 2063 6c61 7373  ake plugin class
-000021e0: 3a5c 6e5c 6e60 6060 7079 7468 6f6e 5c6e  :\n\n```python\n
-000021f0: 6672 6f6d 2070 7964 6576 6c61 6b65 2e70  from pydevlake.p
-00002200: 6c75 6769 6e20 696d 706f 7274 2050 6c75  lugin import Plu
-00002210: 6769 6e5c 6e5c 6e63 6c61 7373 204d 7944  gin\n\nclass MyD
-00002220: 6576 4c61 6b65 506c 7567 696e 2850 6c75  evLakePlugin(Plu
-00002230: 6769 6e29 3a5c 6e20 2020 2023 2049 6d70  gin):\n    # Imp
-00002240: 6c65 6d65 6e74 2072 6571 7569 7265 6420  lement required 
-00002250: 7072 6f70 6572 7469 6573 2061 6e64 206d  properties and m
-00002260: 6574 686f 6473 2068 6572 655c 6e20 2020  ethods here\n   
-00002270: 2023 2065 2e67 2e2c 206e 616d 652c 2064   # e.g., name, d
-00002280: 6573 6372 6970 7469 6f6e 2c20 636f 6e6e  escription, conn
-00002290: 6563 7469 6f6e 5f74 7970 652c 2074 6f6f  ection_type, too
-000022a0: 6c5f 7363 6f70 655f 7479 7065 2c20 7472  l_scope_type, tr
-000022b0: 616e 7366 6f72 6d61 7469 6f6e 5f72 756c  ansformation_rul
-000022c0: 655f 7479 7065 2c20 7374 7265 616d 732c  e_type, streams,
-000022d0: 2065 7463 2e5c 6e60 6060 5c6e 5c6e 596f   etc.\n```\n\nYo
-000022e0: 7520 776f 756c 6420 7468 656e 206e 6565  u would then nee
-000022f0: 6420 746f 2069 6d70 6c65 6d65 6e74 2074  d to implement t
-00002300: 6865 2072 6571 7569 7265 6420 7072 6f70  he required prop
-00002310: 6572 7469 6573 2061 6e64 206d 6574 686f  erties and metho
-00002320: 6473 2066 6f72 2079 6f75 7220 7370 6563  ds for your spec
-00002330: 6966 6963 2070 6c75 6769 6e2c 2073 7563  ific plugin, suc
-00002340: 6820 6173 2060 6e61 6d65 602c 2060 6465  h as `name`, `de
-00002350: 7363 7269 7074 696f 6e60 2c20 6063 6f6e  scription`, `con
-00002360: 6e65 6374 696f 6e5f 7479 7065 602c 2060  nection_type`, `
-00002370: 746f 6f6c 5f73 636f 7065 5f74 7970 6560  tool_scope_type`
-00002380: 2c20 6074 7261 6e73 666f 726d 6174 696f  , `transformatio
-00002390: 6e5f 7275 6c65 5f74 7970 6560 2c20 616e  n_rule_type`, an
-000023a0: 6420 6073 7472 6561 6d73 602e 2059 6f75  d `streams`. You
-000023b0: 2063 616e 2072 6566 6572 2074 6f20 7468   can refer to th
-000023c0: 6520 7072 6f76 6964 6564 2063 6f64 6527  e provided code'
-000023d0: 7320 7465 7374 2066 756e 6374 696f 6e73  s test functions
-000023e0: 2028 652e 672e 2c20 6061 7373 6572 745f   (e.g., `assert_
-000023f0: 7661 6c69 645f 6e61 6d65 602c 2060 6173  valid_name`, `as
-00002400: 7365 7274 5f76 616c 6964 5f64 6573 6372  sert_valid_descr
-00002410: 6970 7469 6f6e 602c 2060 6173 7365 7274  iption`, `assert
-00002420: 5f76 616c 6964 5f63 6f6e 6e65 6374 696f  _valid_connectio
-00002430: 6e5f 7479 7065 602c 2065 7463 2e29 2074  n_type`, etc.) t
-00002440: 6f20 756e 6465 7273 7461 6e64 2074 6865  o understand the
-00002450: 2072 6571 7569 7265 6d65 6e74 7320 616e   requirements an
-00002460: 6420 636f 6e73 7472 6169 6e74 7320 666f  d constraints fo
-00002470: 7220 6561 6368 2070 726f 7065 7274 7920  r each property 
-00002480: 616e 6420 6d65 7468 6f64 2e5c 6e5c 6e4f  and method.\n\nO
-00002490: 6e63 6520 796f 7520 6861 7665 2069 6d70  nce you have imp
-000024a0: 6c65 6d65 6e74 6564 2079 6f75 7220 706c  lemented your pl
-000024b0: 7567 696e 2c20 796f 7520 6361 6e20 7573  ugin, you can us
-000024c0: 6520 7468 6520 7072 6f76 6964 6564 2074  e the provided t
-000024d0: 6573 7420 6675 6e63 7469 6f6e 7320 746f  est functions to
-000024e0: 2076 616c 6964 6174 6520 796f 7572 2070   validate your p
-000024f0: 6c75 6769 6e20 616e 6420 656e 7375 7265  lugin and ensure
-00002500: 2069 7420 776f 726b 7320 636f 7272 6563   it works correc
-00002510: 746c 792e 222c 0d0a 2020 2020 2020 2020  tly.",..        
-00002520: 2020 2020 2261 6e73 7765 725f 7072 6f70      "answer_prop
-00002530: 6572 7469 6573 223a 205b 5d2c 0d0a 2020  erties": [],..  
-00002540: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
-00002550: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00002560: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
-00002570: 6c6f 7722 0d0a 2020 2020 2020 2020 2020  low"..          
-00002580: 2020 7d0d 0a20 2020 2020 2020 207d 2c0d    }..        },.
-00002590: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-000025a0: 2020 2020 2020 2020 2269 6422 3a20 2264          "id": "d
-000025b0: 6576 6c61 6b65 2d31 3022 2c0d 0a20 2020  evlake-10",..   
-000025c0: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
-000025d0: 6f6e 223a 2022 486f 7720 646f 2049 2072  on": "How do I r
-000025e0: 6573 6f6c 7665 2074 6865 2060 7061 6e69  esolve the `pani
-000025f0: 633a 2069 6e76 616c 6964 2065 6e63 4b65  c: invalid encKe
-00002600: 7960 2065 7272 6f72 3f22 2c0d 0a20 2020  y` error?",..   
-00002610: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-00002620: 6e63 655f 616e 7377 6572 223a 2022 546f  nce_answer": "To
-00002630: 2072 6573 6f6c 7665 2074 6865 2027 7061   resolve the 'pa
-00002640: 6e69 633a 2069 6e76 616c 6964 2065 6e63  nic: invalid enc
-00002650: 4b65 7927 2065 7272 6f72 2c20 796f 7520  Key' error, you 
-00002660: 6e65 6564 2074 6f20 656e 7375 7265 2074  need to ensure t
-00002670: 6861 7420 796f 7520 6861 7665 2061 2076  hat you have a v
-00002680: 616c 6964 2065 6e63 7279 7074 696f 6e20  alid encryption 
-00002690: 6b65 7920 7365 7420 696e 2079 6f75 7220  key set in your 
-000026a0: 656e 7669 726f 6e6d 656e 7420 6f72 2063  environment or c
-000026b0: 6f6e 6669 6775 7261 7469 6f6e 2e20 4865  onfiguration. He
-000026c0: 7265 2061 7265 2073 6f6d 6520 7374 6570  re are some step
-000026d0: 7320 796f 7520 6361 6e20 666f 6c6c 6f77  s you can follow
-000026e0: 3a5c 6e5c 6e31 2e20 4d61 6b65 2073 7572  :\n\n1. Make sur
-000026f0: 6520 796f 7520 6861 7665 2061 2076 616c  e you have a val
-00002700: 6964 2065 6e63 7279 7074 696f 6e20 6b65  id encryption ke
-00002710: 7920 616e 6420 6974 2773 2062 6569 6e67  y and it's being
-00002720: 2063 6f72 7265 6374 6c79 2066 6574 6368   correctly fetch
-00002730: 6564 2075 7369 6e67 2074 6865 2060 706c  ed using the `pl
-00002740: 7567 696e 2e45 6e63 6f64 654b 6579 456e  ugin.EncodeKeyEn
-00002750: 7653 7472 6020 636f 6e73 7461 6e74 206f  vStr` constant o
-00002760: 7220 6120 7369 6d69 6c61 7220 6d65 7468  r a similar meth
-00002770: 6f64 2069 6e20 796f 7572 2063 6f64 652e  od in your code.
-00002780: 5c6e 322e 2049 6620 796f 7520 6172 6520  \n2. If you are 
-00002790: 7573 696e 6720 6120 7261 6e64 6f6d 6c79  using a randomly
-000027a0: 2067 656e 6572 6174 6564 2065 6e63 7279   generated encry
-000027b0: 7074 696f 6e20 6b65 792c 206d 616b 6520  ption key, make 
-000027c0: 7375 7265 2074 6f20 7374 6f72 6520 6974  sure to store it
-000027d0: 2073 6563 7572 656c 7920 616e 6420 7573   securely and us
-000027e0: 6520 7468 6520 7361 6d65 206b 6579 2066  e the same key f
-000027f0: 6f72 2062 6f74 6820 656e 6372 7970 7469  or both encrypti
-00002800: 6f6e 2061 6e64 2064 6563 7279 7074 696f  on and decryptio
-00002810: 6e20 7072 6f63 6573 7365 732e 5c6e 332e  n processes.\n3.
-00002820: 2043 6865 636b 2074 6861 7420 7468 6520   Check that the 
-00002830: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00002840: 6162 6c65 2073 7065 6369 6669 6564 2062  able specified b
-00002850: 7920 6070 6c75 6769 6e2e 456e 636f 6465  y `plugin.Encode
-00002860: 4b65 7945 6e76 5374 7260 206f 7220 6120  KeyEnvStr` or a 
-00002870: 7369 6d69 6c61 7220 6d65 7468 6f64 2069  similar method i
-00002880: 7320 7365 7420 7769 7468 2061 2076 616c  s set with a val
-00002890: 6964 2065 6e63 7279 7074 696f 6e20 6b65  id encryption ke
-000028a0: 792e 5c6e 342e 2056 6572 6966 7920 7468  y.\n4. Verify th
-000028b0: 6174 2074 6865 2065 6e63 4b65 7920 6973  at the encKey is
-000028c0: 2062 6569 6e67 2073 6574 2061 6e64 2073   being set and s
-000028d0: 6176 6564 2074 6f20 7468 6520 636f 6e66  aved to the conf
-000028e0: 6967 2070 726f 7065 726c 7920 7573 696e  ig properly usin
-000028f0: 6720 6076 2e53 6574 2870 6c75 6769 6e2e  g `v.Set(plugin.
-00002900: 456e 636f 6465 4b65 7945 6e76 5374 722c  EncodeKeyEnvStr,
-00002910: 2065 6e63 4b65 7929 6020 616e 6420 6063   encKey)` and `c
-00002920: 6f6e 6669 672e 5772 6974 6543 6f6e 6669  onfig.WriteConfi
-00002930: 6728 7629 6020 6f72 2073 696d 696c 6172  g(v)` or similar
-00002940: 206d 6574 686f 6473 2069 6e20 796f 7572   methods in your
-00002950: 2063 6f64 652e 5c6e 5c6e 4966 2074 6865   code.\n\nIf the
-00002960: 2069 7373 7565 2070 6572 7369 7374 732c   issue persists,
-00002970: 2079 6f75 206d 6179 206e 6565 6420 746f   you may need to
-00002980: 2070 726f 7669 6465 206d 6f72 6520 636f   provide more co
-00002990: 6e74 6578 7420 6f72 2072 6566 6572 2074  ntext or refer t
-000029a0: 6f20 7468 6520 646f 6375 6d65 6e74 6174  o the documentat
-000029b0: 696f 6e20 6f66 2074 6865 2073 7065 6369  ion of the speci
-000029c0: 6669 6320 736f 6674 7761 7265 2079 6f75  fic software you
-000029d0: 2061 7265 2077 6f72 6b69 6e67 2077 6974   are working wit
-000029e0: 682e 222c 0d0a 2020 2020 2020 2020 2020  h.",..          
-000029f0: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
-00002a00: 7469 6573 223a 205b 5d2c 0d0a 2020 2020  ties": [],..    
-00002a10: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
-00002a20: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00002a30: 2020 2020 226c 6576 656c 223a 2022 6d69      "level": "mi
-00002a40: 6422 0d0a 2020 2020 2020 2020 2020 2020  d"..            
-00002a50: 7d0d 0a20 2020 2020 2020 207d 2c0d 0a20  }..        },.. 
-00002a60: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00002a70: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
-00002a80: 6c61 6b65 2d31 3122 2c0d 0a20 2020 2020  lake-11",..     
-00002a90: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
-00002aa0: 223a 2022 486f 7720 646f 6573 2044 6576  ": "How does Dev
-00002ab0: 4c61 6b65 2067 656e 6572 6174 6520 6120  Lake generate a 
+00000000: 7b0a 2020 2020 226e 616d 6522 3a20 2244  {.    "name": "D
+00000010: 6576 4c61 6b65 222c 0a20 2020 2022 6465  evLake",.    "de
+00000020: 7363 7269 7074 696f 6e22 3a20 2245 7861  scription": "Exa
+00000030: 6d70 6c65 2051 7565 7365 7469 6f6e 7320  mple Quesetions 
+00000040: 616e 6420 416e 7377 6572 7320 666f 7220  and Answers for 
+00000050: 4465 764c 616b 6522 2c0a 2020 2020 2263  DevLake",.    "c
+00000060: 6173 6573 223a 205b 0a20 2020 2020 2020  ases": [.       
+00000070: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000080: 6964 223a 2022 6465 766c 616b 652d 3031  id": "devlake-01
+00000090: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000000a0: 7175 6573 7469 6f6e 223a 2022 486f 7720  question": "How 
+000000b0: 6973 2074 6865 206c 6561 6420 7469 6d65  is the lead time
+000000c0: 2066 6f72 2063 6861 6e67 6573 2063 616c   for changes cal
+000000d0: 6375 6c61 7465 643f 222c 0a20 2020 2020  culated?",.     
+000000e0: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
+000000f0: 655f 616e 7377 6572 223a 2022 5468 6520  e_answer": "The 
+00000100: 6c65 6164 2074 696d 6520 666f 7220 6368  lead time for ch
+00000110: 616e 6765 7320 6973 2063 616c 6375 6c61  anges is calcula
+00000120: 7465 6420 696e 2074 6865 2060 4361 6c63  ted in the `Calc
+00000130: 756c 6174 6543 6861 6e67 654c 6561 6454  ulateChangeLeadT
+00000140: 696d 6560 2066 756e 6374 696f 6e20 6279  ime` function by
+00000150: 2066 6f6c 6c6f 7769 6e67 2074 6865 7365   following these
+00000160: 2073 7465 7073 3a5c 6e5c 6e31 2e20 4765   steps:\n\n1. Ge
+00000170: 7420 7075 6c6c 2072 6571 7565 7374 7320  t pull requests 
+00000180: 6279 2074 6865 2070 726f 6a65 6374 206e  by the project n
+00000190: 616d 652e 5c6e 322e 2046 6f72 2065 6163  ame.\n2. For eac
+000001a0: 6820 7075 6c6c 2072 6571 7565 7374 2c20  h pull request, 
+000001b0: 6765 7420 7468 6520 6669 7273 7420 636f  get the first co
+000001c0: 6d6d 6974 2061 6e64 2063 616c 6375 6c61  mmit and calcula
+000001d0: 7465 2074 6865 2050 5220 636f 6469 6e67  te the PR coding
+000001e0: 2074 696d 6520 6173 2074 6865 2074 696d   time as the tim
+000001f0: 6520 7370 616e 2062 6574 7765 656e 2074  e span between t
+00000200: 6865 2066 6972 7374 2063 6f6d 6d69 7427  he first commit'
+00000210: 7320 6175 7468 6f72 6564 2064 6174 6520  s authored date 
+00000220: 616e 6420 7468 6520 7075 6c6c 2072 6571  and the pull req
+00000230: 7565 7374 2773 2063 7265 6174 6564 2064  uest's created d
+00000240: 6174 652e 5c6e 332e 2047 6574 2074 6865  ate.\n3. Get the
+00000250: 2066 6972 7374 2072 6576 6965 7720 666f   first review fo
+00000260: 7220 7468 6520 7075 6c6c 2072 6571 7565  r the pull reque
+00000270: 7374 2028 6578 636c 7564 696e 6720 636f  st (excluding co
+00000280: 6d6d 656e 7473 2066 726f 6d20 7468 6520  mments from the 
+00000290: 5052 2063 7265 6174 6f72 2920 616e 6420  PR creator) and 
+000002a0: 6361 6c63 756c 6174 6520 7468 6520 5052  calculate the PR
+000002b0: 2070 6963 6b75 7020 7469 6d65 2061 7320   pickup time as 
+000002c0: 7468 6520 7469 6d65 2073 7061 6e20 6265  the time span be
+000002d0: 7477 6565 6e20 7468 6520 7075 6c6c 2072  tween the pull r
+000002e0: 6571 7565 7374 2773 2063 7265 6174 6564  equest's created
+000002f0: 2064 6174 6520 616e 6420 7468 6520 6669   date and the fi
+00000300: 7273 7420 7265 7669 6577 2773 2063 7265  rst review's cre
+00000310: 6174 6564 2064 6174 652e 2043 616c 6375  ated date. Calcu
+00000320: 6c61 7465 2074 6865 2050 5220 7265 7669  late the PR revi
+00000330: 6577 2074 696d 6520 6173 2074 6865 2074  ew time as the t
+00000340: 696d 6520 7370 616e 2062 6574 7765 656e  ime span between
+00000350: 2074 6865 2066 6972 7374 2072 6576 6965   the first revie
+00000360: 7727 7320 6372 6561 7465 6420 6461 7465  w's created date
+00000370: 2061 6e64 2074 6865 2070 756c 6c20 7265   and the pull re
+00000380: 7175 6573 7427 7320 6d65 7267 6564 2064  quest's merged d
+00000390: 6174 652e 5c6e 342e 2047 6574 2074 6865  ate.\n4. Get the
+000003a0: 2064 6570 6c6f 796d 656e 7420 666f 7220   deployment for 
+000003b0: 7468 6520 7075 6c6c 2072 6571 7565 7374  the pull request
+000003c0: 2075 7369 6e67 2074 6865 206d 6572 6765   using the merge
+000003d0: 2063 6f6d 6d69 7420 5348 4120 616e 6420   commit SHA and 
+000003e0: 6361 6c63 756c 6174 6520 7468 6520 5052  calculate the PR
+000003f0: 2064 6570 6c6f 7920 7469 6d65 2061 7320   deploy time as 
+00000400: 7468 6520 7469 6d65 2073 7061 6e20 6265  the time span be
+00000410: 7477 6565 6e20 7468 6520 7075 6c6c 2072  tween the pull r
+00000420: 6571 7565 7374 2773 206d 6572 6765 6420  equest's merged 
+00000430: 6461 7465 2061 6e64 2074 6865 2064 6570  date and the dep
+00000440: 6c6f 796d 656e 7427 7320 6669 6e69 7368  loyment's finish
+00000450: 6564 2064 6174 652e 5c6e 352e 2043 616c  ed date.\n5. Cal
+00000460: 6375 6c61 7465 2074 6865 2050 5220 6379  culate the PR cy
+00000470: 636c 6520 7469 6d65 2062 7920 6164 6469  cle time by addi
+00000480: 6e67 2074 6865 2050 5220 636f 6469 6e67  ng the PR coding
+00000490: 2074 696d 652c 2050 5220 6475 7269 6e67   time, PR during
+000004a0: 2074 696d 6520 2874 696d 6520 7370 616e   time (time span
+000004b0: 2062 6574 7765 656e 2074 6865 2070 756c   between the pul
+000004c0: 6c20 7265 7175 6573 7427 7320 6372 6561  l request's crea
+000004d0: 7465 6420 6461 7465 2061 6e64 206d 6572  ted date and mer
+000004e0: 6765 6420 6461 7465 292c 2061 6e64 2050  ged date), and P
+000004f0: 5220 6465 706c 6f79 2074 696d 652e 5c6e  R deploy time.\n
+00000500: 5c6e 5468 6520 6675 6e63 7469 6f6e 2072  \nThe function r
+00000510: 6574 7572 6e73 2061 2060 5072 6f6a 6563  eturns a `Projec
+00000520: 7450 724d 6574 7269 6360 206f 626a 6563  tPrMetric` objec
+00000530: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
+00000540: 2063 616c 6375 6c61 7465 6420 6c65 6164   calculated lead
+00000550: 2074 696d 6573 2066 6f72 2065 6163 6820   times for each 
+00000560: 7075 6c6c 2072 6571 7565 7374 2069 6e20  pull request in 
+00000570: 7468 6520 7072 6f6a 6563 742e 222c 0a20  the project.",. 
+00000580: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
+00000590: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
+000005a0: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+000005b0: 226e 6f74 6573 223a 207b 0a20 2020 2020  "notes": {.     
+000005c0: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
+000005d0: 6c22 3a20 226d 6964 220a 2020 2020 2020  l": "mid".      
+000005e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000005f0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00000600: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+00000610: 6465 766c 616b 652d 3032 222c 0a20 2020  devlake-02",.   
+00000620: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
+00000630: 6f6e 223a 2022 5768 7920 6361 6e20 7468  on": "Why can th
+00000640: 6520 6c65 6164 2074 696d 6520 666f 7220  e lead time for 
+00000650: 6368 616e 6765 7320 6d65 7472 6963 2062  changes metric b
+00000660: 6520 6e75 6c6c 2073 6f6d 6574 696d 6573  e null sometimes
+00000670: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
+00000680: 2272 6566 6572 656e 6365 5f61 6e73 7765  "reference_answe
+00000690: 7222 3a20 2254 6865 206c 6561 6420 7469  r": "The lead ti
+000006a0: 6d65 2066 6f72 2063 6861 6e67 6573 206d  me for changes m
+000006b0: 6574 7269 6320 6361 6e20 6265 206e 756c  etric can be nul
+000006c0: 6c20 736f 6d65 7469 6d65 7320 6265 6361  l sometimes beca
+000006d0: 7573 6520 736f 6d65 206f 6620 7468 6520  use some of the 
+000006e0: 7469 6d65 2073 7061 6e73 2075 7365 6420  time spans used 
+000006f0: 746f 2063 616c 6375 6c61 7465 2069 7420  to calculate it 
+00000700: 6d69 6768 7420 6265 206e 756c 6c2e 2049  might be null. I
+00000710: 6e20 7468 6520 6043 616c 6375 6c61 7465  n the `Calculate
+00000720: 4368 616e 6765 4c65 6164 5469 6d65 6020  ChangeLeadTime` 
+00000730: 6675 6e63 7469 6f6e 2c20 7468 6520 5052  function, the PR
+00000740: 2063 6f64 696e 6720 7469 6d65 2c20 5052   coding time, PR
+00000750: 2070 6963 6b75 7020 7469 6d65 2c20 5052   pickup time, PR
+00000760: 2072 6576 6965 7720 7469 6d65 2c20 616e   review time, an
+00000770: 6420 5052 2064 6570 6c6f 7920 7469 6d65  d PR deploy time
+00000780: 2061 7265 2063 616c 6375 6c61 7465 642e   are calculated.
+00000790: 2049 6620 616e 7920 6f66 2074 6865 7365   If any of these
+000007a0: 2074 696d 6520 7370 616e 7320 6172 6520   time spans are 
+000007b0: 6e75 6c6c 206f 7220 6861 7665 206e 6567  null or have neg
+000007c0: 6174 6976 6520 7661 6c75 6573 2c20 7468  ative values, th
+000007d0: 6520 6669 6e61 6c20 5052 2063 7963 6c65  e final PR cycle
+000007e0: 2074 696d 6520 286c 6561 6420 7469 6d65   time (lead time
+000007f0: 2066 6f72 2063 6861 6e67 6573 2920 6d69   for changes) mi
+00000800: 6768 7420 6e6f 7420 6265 2063 616c 6375  ght not be calcu
+00000810: 6c61 7465 642c 2072 6573 756c 7469 6e67  lated, resulting
+00000820: 2069 6e20 6120 6e75 6c6c 2076 616c 7565   in a null value
+00000830: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00000840: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
+00000850: 6573 223a 205b 5d2c 0a20 2020 2020 2020  es": [],.       
+00000860: 2020 2020 2022 6e6f 7465 7322 3a20 7b0a       "notes": {.
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 226c 6576 656c 223a 2022 6c6f 7722 0a20  "level": "low". 
+00000890: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000008a0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000008b0: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
+000008c0: 6422 3a20 2264 6576 6c61 6b65 2d30 3322  d": "devlake-03"
+000008d0: 2c0a 2020 2020 2020 2020 2020 2020 2271  ,.            "q
+000008e0: 7565 7374 696f 6e22 3a20 2243 616e 2079  uestion": "Can y
+000008f0: 6f75 2070 726f 7669 6465 2061 2068 6967  ou provide a hig
+00000900: 682d 6c65 7665 6c20 6465 7363 7269 7074  h-level descript
+00000910: 696f 6e20 6f66 2044 6576 4c61 6b65 2773  ion of DevLake's
+00000920: 2061 7263 6869 7465 6374 7572 653f 222c   architecture?",
+00000930: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00000940: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+00000950: 2022 4465 764c 616b 6520 636f 6e73 6973   "DevLake consis
+00000960: 7473 206f 6620 7468 6573 6520 6d61 696e  ts of these main
+00000970: 2063 6f6d 706f 6e65 6e74 733a 205c 6e5c   components: \n\
+00000980: 6e31 2e20 436f 6e66 6967 2055 492c 205c  n1. Config UI, \
+00000990: 6e5c 6e32 2e20 4150 4920 5365 7276 6572  n\n2. API Server
+000009a0: 2c20 5c6e 5c6e 332e 2052 756e 6e65 722c  , \n\n3. Runner,
+000009b0: 205c 6e5c 6e34 2e20 4461 7461 6261 7365   \n\n4. Database
+000009c0: 2c20 5c6e 5c6e 352e 2050 6c75 6769 6e73  , \n\n5. Plugins
+000009d0: 2c20 5c6e 5c6e 362e 2044 6173 6862 6f61  , \n\n6. Dashboa
+000009e0: 7264 732e 2049 7473 2064 6174 6120 666c  rds. Its data fl
+000009f0: 6f77 2068 6173 2074 6872 6565 206c 6179  ow has three lay
+00000a00: 7365 7273 3a20 5c6e 5c6e 312e 2052 6177  sers: \n\n1. Raw
+00000a10: 206c 6179 6572 2c20 5c6e 5c6e 322c 2054   layer, \n\n2, T
+00000a20: 6f6f 6c20 6c61 7965 722c 205c 6e5c 6e33  ool layer, \n\n3
+00000a30: 2e20 446f 6d61 696e 206c 6179 6572 2e20  . Domain layer. 
+00000a40: 466f 7220 6465 7461 696c 6564 2065 7870  For detailed exp
+00000a50: 6c61 6e61 7469 6f6e 732c 2070 6c65 6173  lanations, pleas
+00000a60: 6520 7265 6665 7220 746f 2074 6869 7320  e refer to this 
+00000a70: 646f 633a 2068 7474 7073 3a2f 2f64 6576  doc: https://dev
+00000a80: 6c61 6b65 2e61 7061 6368 652e 6f72 672f  lake.apache.org/
+00000a90: 646f 6373 2f4f 7665 7276 6965 772f 4172  docs/Overview/Ar
+00000aa0: 6368 6974 6563 7475 7265 222c 0a20 2020  chitecture",.   
+00000ab0: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
+00000ac0: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
+00000ad0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00000ae0: 6f74 6573 223a 207b 0a20 2020 2020 2020  otes": {.       
+00000af0: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
+00000b00: 3a20 2268 6967 6822 0a20 2020 2020 2020  : "high".       
+00000b10: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00000b20: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00000b30: 2020 2020 2020 2020 2269 6422 3a20 2264          "id": "d
+00000b40: 6576 6c61 6b65 2d30 3422 2c0a 2020 2020  evlake-04",.    
+00000b50: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00000b60: 6e22 3a20 2257 6861 7420 6461 7461 2064  n": "What data d
+00000b70: 6f65 7320 7468 6520 417a 7572 6520 4465  oes the Azure De
+00000b80: 764f 7073 2070 6c75 6769 6e20 636f 6c6c  vOps plugin coll
+00000b90: 6563 743f 222c 0a20 2020 2020 2020 2020  ect?",.         
+00000ba0: 2020 2022 7265 6665 7265 6e63 655f 616e     "reference_an
+00000bb0: 7377 6572 223a 2022 5468 6520 417a 7572  swer": "The Azur
+00000bc0: 6520 4465 764f 7073 2070 6c75 6769 6e20  e DevOps plugin 
+00000bd0: 636f 6c6c 6563 7473 2064 6174 6120 7265  collects data re
+00000be0: 6c61 7465 6420 746f 2047 6974 2072 6570  lated to Git rep
+00000bf0: 6f73 6974 6f72 6965 732c 2047 6974 2070  ositories, Git p
+00000c00: 756c 6c20 7265 7175 6573 7473 2c20 4769  ull requests, Gi
+00000c10: 7420 7075 6c6c 2072 6571 7565 7374 2063  t pull request c
+00000c20: 6f6d 6d69 7473 2c20 6275 696c 6473 2c20  ommits, builds, 
+00000c30: 616e 6420 6a6f 6273 2e20 5370 6563 6966  and jobs. Specif
+00000c40: 6963 616c 6c79 2c20 6974 2063 6f6c 6c65  ically, it colle
+00000c50: 6374 7320 696e 666f 726d 6174 696f 6e20  cts information 
+00000c60: 7375 6368 2061 733a 5c6e 5c6e 312e 2047  such as:\n\n1. G
+00000c70: 6974 5075 6c6c 5265 7175 6573 7473 3a20  itPullRequests: 
+00000c80: 4261 7365 2072 6570 6f73 6974 6f72 7920  Base repository 
+00000c90: 4944 2c20 6865 6164 2072 6570 6f73 6974  ID, head reposit
+00000ca0: 6f72 7920 4944 2c20 7374 6174 7573 2c20  ory ID, status, 
+00000cb0: 6f72 6967 696e 616c 2073 7461 7475 732c  original status,
+00000cc0: 2074 6974 6c65 2c20 6465 7363 7269 7074   title, descript
+00000cd0: 696f 6e2c 2055 524c 2c20 6175 7468 6f72  ion, URL, author
+00000ce0: 206e 616d 652c 2061 7574 686f 7220 4944   name, author ID
+00000cf0: 2c20 7075 6c6c 2072 6571 7565 7374 206b  , pull request k
+00000d00: 6579 2c20 6372 6561 7465 6420 6461 7465  ey, created date
+00000d10: 2c20 6d65 7267 6564 2064 6174 652c 2063  , merged date, c
+00000d20: 6c6f 7365 6420 6461 7465 2c20 7479 7065  losed date, type
+00000d30: 2c20 636f 6d70 6f6e 656e 742c 206d 6572  , component, mer
+00000d40: 6765 2063 6f6d 6d69 7420 5348 412c 2068  ge commit SHA, h
+00000d50: 6561 6420 7265 6665 7265 6e63 652c 2062  ead reference, b
+00000d60: 6173 6520 7265 6665 7265 6e63 652c 2068  ase reference, h
+00000d70: 6561 6420 636f 6d6d 6974 2053 4841 2c20  ead commit SHA, 
+00000d80: 616e 6420 6261 7365 2063 6f6d 6d69 7420  and base commit 
+00000d90: 5348 412e 5c6e 5c6e 322e 2047 6974 5075  SHA.\n\n2. GitPu
+00000da0: 6c6c 5265 7175 6573 7443 6f6d 6d69 7473  llRequestCommits
+00000db0: 3a20 436f 6d6d 6974 2053 4841 2028 636f  : Commit SHA (co
+00000dc0: 6d6d 6974 5f69 6429 2c20 7075 6c6c 2072  mmit_id), pull r
+00000dd0: 6571 7565 7374 2049 442c 2063 6f6d 6d69  equest ID, commi
+00000de0: 7420 6175 7468 6f72 206e 616d 6520 2861  t author name (a
+00000df0: 7574 686f 725f 6e61 6d65 292c 2063 6f6d  uthor_name), com
+00000e00: 6d69 7420 6175 7468 6f72 2065 6d61 696c  mit author email
+00000e10: 2028 6175 7468 6f72 5f65 6d61 696c 292c   (author_email),
+00000e20: 2061 6e64 2063 6f6d 6d69 7420 6175 7468   and commit auth
+00000e30: 6f72 6564 2064 6174 6520 2861 7574 686f  ored date (autho
+00000e40: 725f 6461 7465 292e 5c6e 5c6e 332e 2042  r_date).\n\n3. B
+00000e50: 7569 6c64 733a 2042 7569 6c64 2773 206e  uilds: Build's n
+00000e60: 616d 652c 2073 7461 7475 732c 2063 7265  ame, status, cre
+00000e70: 6174 6564 2064 6174 652c 2066 696e 6973  ated date, finis
+00000e80: 6865 6420 6461 7465 2c20 7265 7375 6c74  hed date, result
+00000e90: 2c20 6475 7261 7469 6f6e 2069 6e20 7365  , duration in se
+00000ea0: 636f 6e64 732c 2065 6e76 6972 6f6e 6d65  conds, environme
+00000eb0: 6e74 2c20 7479 7065 2c20 616e 6420 6f74  nt, type, and ot
+00000ec0: 6865 7220 7265 6c61 7465 6420 6465 7461  her related deta
+00000ed0: 696c 7320 6c69 6b65 2063 6f6d 6d69 7420  ils like commit 
+00000ee0: 5348 412c 2062 7261 6e63 682c 2072 6570  SHA, branch, rep
+00000ef0: 6f73 6974 6f72 7920 4944 2c20 616e 6420  ository ID, and 
+00000f00: 7265 706f 7369 746f 7279 2055 524c 2e5c  repository URL.\
+00000f10: 6e5c 6e34 2e20 4a6f 6273 3a20 4a6f 6220  n\n4. Jobs: Job 
+00000f20: 4944 2c20 6e61 6d65 2c20 6275 696c 6420  ID, name, build 
+00000f30: 4944 2c20 7374 6174 7573 2c20 7374 6172  ID, status, star
+00000f40: 7420 7469 6d65 2c20 6669 6e69 7368 2074  t time, finish t
+00000f50: 696d 652c 2072 6573 756c 742c 2074 7970  ime, result, typ
+00000f60: 652c 2064 7572 6174 696f 6e20 696e 2073  e, duration in s
+00000f70: 6563 6f6e 6473 2c20 656e 7669 726f 6e6d  econds, environm
+00000f80: 656e 742c 2061 6e64 2043 4943 4420 7363  ent, and CICD sc
+00000f90: 6f70 6520 4944 2e22 2c0a 2020 2020 2020  ope ID.",.      
+00000fa0: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00000fb0: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00000fc0: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00000fd0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00000fe0: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+00000ff0: 6d69 6422 0a20 2020 2020 2020 2020 2020  mid".           
+00001000: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00001010: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001020: 2020 2020 2269 6422 3a20 2264 6576 6c61      "id": "devla
+00001030: 6b65 2d30 3522 2c0a 2020 2020 2020 2020  ke-05",.        
+00001040: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
+00001050: 2257 6861 7420 6172 6520 7468 6520 6665  "What are the fe
+00001060: 6174 7572 6573 206f 6620 4465 764c 616b  atures of DevLak
+00001070: 653f 222c 0a20 2020 2020 2020 2020 2020  e?",.           
+00001080: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
+00001090: 6572 223a 2022 4170 6163 6865 2044 6576  er": "Apache Dev
+000010a0: 4c61 6b65 2069 7320 616e 206f 7065 6e2d  Lake is an open-
+000010b0: 736f 7572 6365 2064 6576 2064 6174 6120  source dev data 
+000010c0: 706c 6174 666f 726d 2074 6f20 696e 6765  platform to inge
+000010d0: 7374 2c20 616e 616c 797a 652c 2061 6e64  st, analyze, and
+000010e0: 2076 6973 7561 6c69 7a65 2066 7261 676d   visualize fragm
+000010f0: 656e 7465 6420 6461 7461 2066 726f 6d20  ented data from 
+00001100: 4465 764f 7073 2074 6f6f 6c73 2c20 6578  DevOps tools, ex
+00001110: 7472 6163 7469 6e67 2069 6e73 6967 6874  tracting insight
+00001120: 7320 666f 7220 656e 6769 6e65 6572 696e  s for engineerin
+00001130: 6720 6578 6365 6c6c 656e 6365 2c20 6465  g excellence, de
+00001140: 7665 6c6f 7065 7220 6578 7065 7269 656e  veloper experien
+00001150: 6365 2c20 616e 6420 636f 6d6d 756e 6974  ce, and communit
+00001160: 7920 6772 6f77 7468 2e20 466f 7220 6120  y growth. For a 
+00001170: 636f 6d70 6c65 7465 206c 6973 7420 6f66  complete list of
+00001180: 2066 6561 7475 7265 732c 2070 6c65 6173   features, pleas
+00001190: 6520 7669 7369 7420 7468 6520 4170 6163  e visit the Apac
+000011a0: 6865 2044 6576 4c61 6b65 2077 6562 7369  he DevLake websi
+000011b0: 7465 206f 7220 7072 6f76 6964 6520 6d6f  te or provide mo
+000011c0: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e22  re information."
+000011d0: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+000011e0: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
+000011f0: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
+00001200: 2020 2022 6e6f 7465 7322 3a20 7b0a 2020     "notes": {.  
+00001210: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00001220: 6576 656c 223a 2022 6c6f 7722 0a20 2020  evel": "low".   
+00001230: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001240: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00001250: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00001260: 3a20 2264 6576 6c61 6b65 2d30 3622 2c0a  : "devlake-06",.
+00001270: 2020 2020 2020 2020 2020 2020 2271 7565              "que
+00001280: 7374 696f 6e22 3a20 2257 6861 7420 6172  stion": "What ar
+00001290: 6520 7468 6520 7573 6520 6361 7365 7320  e the use cases 
+000012a0: 6f66 2044 6576 4c61 6b65 3f22 2c0a 2020  of DevLake?",.  
+000012b0: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
+000012c0: 656e 6365 5f61 6e73 7765 7222 3a20 2244  ence_answer": "D
+000012d0: 6576 4c61 6b65 2069 7320 6465 7369 676e  evLake is design
+000012e0: 6564 2074 6f20 6865 6c70 2064 6576 656c  ed to help devel
+000012f0: 6f70 6572 7320 616e 6420 7465 616d 7320  opers and teams 
+00001300: 6d61 6e61 6765 2061 6e64 2061 6e61 6c79  manage and analy
+00001310: 7a65 2074 6865 6972 2073 6f66 7477 6172  ze their softwar
+00001320: 6520 6465 7665 6c6f 706d 656e 7420 6461  e development da
+00001330: 7461 2e20 5573 6520 6361 7365 7320 666f  ta. Use cases fo
+00001340: 7220 4465 764c 616b 6520 696e 636c 7564  r DevLake includ
+00001350: 653a 5c6e 5c6e 312e 2043 656e 7472 616c  e:\n\n1. Central
+00001360: 697a 696e 6720 6461 7461 2066 726f 6d20  izing data from 
+00001370: 7661 7269 6f75 7320 6465 7665 6c6f 706d  various developm
+00001380: 656e 7420 746f 6f6c 7320 616e 6420 706c  ent tools and pl
+00001390: 6174 666f 726d 732c 2073 7563 6820 6173  atforms, such as
+000013a0: 2047 6974 4875 622c 2047 6974 4c61 622c   GitHub, GitLab,
+000013b0: 204a 6972 612c 2061 6e64 206d 6f72 652c   Jira, and more,
+000013c0: 2069 6e74 6f20 6120 7369 6e67 6c65 2064   into a single d
+000013d0: 6174 6120 6c61 6b65 2e5c 6e32 2e20 456e  ata lake.\n2. En
+000013e0: 6162 6c69 6e67 2061 6476 616e 6365 6420  abling advanced 
+000013f0: 616e 616c 7974 6963 7320 616e 6420 696e  analytics and in
+00001400: 7369 6768 7473 206f 6e20 6465 7665 6c6f  sights on develo
+00001410: 706d 656e 7420 6461 7461 2c20 7375 6368  pment data, such
+00001420: 2061 7320 636f 6465 2071 7561 6c69 7479   as code quality
+00001430: 2c20 7465 616d 2070 6572 666f 726d 616e  , team performan
+00001440: 6365 2c20 616e 6420 7072 6f6a 6563 7420  ce, and project 
+00001450: 7072 6f67 7265 7373 2e5c 6e33 2e20 4661  progress.\n3. Fa
+00001460: 6369 6c69 7461 7469 6e67 2074 6865 2063  cilitating the c
+00001470: 7265 6174 696f 6e20 6f66 2063 7573 746f  reation of custo
+00001480: 6d20 706c 7567 696e 7320 746f 2069 6e74  m plugins to int
+00001490: 6567 7261 7465 2077 6974 6820 6164 6469  egrate with addi
+000014a0: 7469 6f6e 616c 2064 6174 6120 736f 7572  tional data sour
+000014b0: 6365 7320 6f72 2074 6f6f 6c73 2c20 616c  ces or tools, al
+000014c0: 6c6f 7769 6e67 2066 6f72 2067 7265 6174  lowing for great
+000014d0: 6572 2066 6c65 7869 6269 6c69 7479 2061  er flexibility a
+000014e0: 6e64 2065 7874 656e 7369 6269 6c69 7479  nd extensibility
+000014f0: 2e5c 6e34 2e20 5375 7070 6f72 7469 6e67  .\n4. Supporting
+00001500: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
+00001510: 206f 6620 6375 7374 6f6d 2064 6173 6862   of custom dashb
+00001520: 6f61 7264 7320 616e 6420 7265 706f 7274  oards and report
+00001530: 7320 746f 2076 6973 7561 6c69 7a65 2061  s to visualize a
+00001540: 6e64 206d 6f6e 6974 6f72 2064 6576 656c  nd monitor devel
+00001550: 6f70 6d65 6e74 206d 6574 7269 6373 222c  opment metrics",
+00001560: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
+00001570: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
+00001580: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+00001590: 2020 226e 6f74 6573 223a 207b 0a20 2020    "notes": {.   
+000015a0: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
+000015b0: 7665 6c22 3a20 226c 6f77 220a 2020 2020  vel": "low".    
+000015c0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000015d0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+000015e0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+000015f0: 2022 6465 766c 616b 652d 3037 222c 0a20   "devlake-07",. 
+00001600: 2020 2020 2020 2020 2020 2022 7175 6573             "ques
+00001610: 7469 6f6e 223a 2022 486f 7720 6361 6e20  tion": "How can 
+00001620: 4920 636f 6e74 7269 6275 7465 2074 6f20  I contribute to 
+00001630: 4465 764c 616b 653f 222c 0a20 2020 2020  DevLake?",.     
+00001640: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
+00001650: 655f 616e 7377 6572 223a 2022 596f 7520  e_answer": "You 
+00001660: 6361 6e20 636f 6e74 7269 6275 7465 2074  can contribute t
+00001670: 6f20 4465 764c 616b 6520 696e 2073 6576  o DevLake in sev
+00001680: 6572 616c 2077 6179 733a 5c6e 5c6e 312e  eral ways:\n\n1.
+00001690: 2043 7265 6174 6520 616e 2049 7373 7565   Create an Issue
+000016a0: 3a20 5265 706f 7274 2061 2062 7567 206f  : Report a bug o
+000016b0: 7220 6665 6174 7572 6520 7265 7175 6573  r feature reques
+000016c0: 7420 746f 2041 7061 6368 6520 4465 764c  t to Apache DevL
+000016d0: 616b 652e 5c6e 322e 2053 7562 6d69 7420  ake.\n2. Submit 
+000016e0: 6120 5052 2028 5075 6c6c 2052 6571 7565  a PR (Pull Reque
+000016f0: 7374 293a 2053 7461 7274 2077 6974 6820  st): Start with 
+00001700: 676f 6f64 2066 6972 7374 2069 7373 7565  good first issue
+00001710: 7320 6f72 2069 7373 7565 7320 7769 7468  s or issues with
+00001720: 206e 6f20 6173 7369 676e 6565 732e 2052   no assignees. R
+00001730: 6561 6420 7468 726f 7567 6820 7468 6520  ead through the 
+00001740: 5b43 6f6e 7472 6962 7574 696e 6720 446f  [Contributing Do
+00001750: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00001760: 7073 3a2f 2f64 6576 6c61 6b65 2e61 7061  ps://devlake.apa
+00001770: 6368 652e 6f72 672f 636f 6d6d 756e 6974  che.org/communit
+00001780: 792f 292c 2061 6464 2072 656c 6576 616e  y/), add relevan
+00001790: 7420 7465 7374 732c 2064 6f63 756d 656e  t tests, documen
+000017a0: 7461 7469 6f6e 2c20 616e 6420 6c61 6265  tation, and labe
+000017b0: 6c73 2074 6f20 7468 6520 5052 2e5c 6e33  ls to the PR.\n3
+000017c0: 2e20 4a6f 696e 204d 6169 6c69 6e67 206c  . Join Mailing l
+000017d0: 6973 743a 2049 6e69 7469 6174 6520 6f72  ist: Initiate or
+000017e0: 2070 6172 7469 6369 7061 7465 2069 6e20   participate in 
+000017f0: 7072 6f6a 6563 7420 6469 7363 7573 7369  project discussi
+00001800: 6f6e 7320 6f6e 2074 6865 206d 6169 6c69  ons on the maili
+00001810: 6e67 206c 6973 742e 5c6e 342e 2057 7269  ng list.\n4. Wri
+00001820: 7465 2061 2042 6c6f 673a 2057 7269 7465  te a Blog: Write
+00001830: 2061 2062 6c6f 6720 746f 2073 6861 7265   a blog to share
+00001840: 2079 6f75 7220 7573 6520 6361 7365 7320   your use cases 
+00001850: 6162 6f75 7420 4170 6163 6865 2044 6576  about Apache Dev
+00001860: 4c61 6b65 2e5c 6e35 2e20 436f 6e74 7269  Lake.\n5. Contri
+00001870: 6275 7465 2061 2050 6c75 6769 6e3a 2041  bute a Plugin: A
+00001880: 6464 2061 2070 6c75 6769 6e20 746f 2069  dd a plugin to i
+00001890: 6e74 6567 7261 7465 2041 7061 6368 6520  ntegrate Apache 
+000018a0: 4465 764c 616b 6520 7769 7468 206d 6f72  DevLake with mor
+000018b0: 6520 6461 7461 2073 6f75 7263 6573 2066  e data sources f
+000018c0: 6f72 2074 6865 2063 6f6d 6d75 6e69 7479  or the community
+000018d0: 2e5c 6e5c 6e50 6c65 6173 6520 7265 6164  .\n\nPlease read
+000018e0: 2074 6865 205b 636f 6e74 7269 6275 7469   the [contributi
+000018f0: 6f6e 2067 7569 6465 6c69 6e65 735d 2868  on guidelines](h
+00001900: 7474 7073 3a2f 2f64 6576 6c61 6b65 2e61  ttps://devlake.a
+00001910: 7061 6368 652e 6f72 672f 636f 6d6d 756e  pache.org/commun
+00001920: 6974 7929 2062 6566 6f72 6520 796f 7520  ity) before you 
+00001930: 6d61 6b65 2061 2063 6f6e 7472 6962 7574  make a contribut
+00001940: 696f 6e2e 222c 0a20 2020 2020 2020 2020  ion.",.         
+00001950: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
+00001960: 7274 6965 7322 3a20 5b5d 2c0a 2020 2020  rties": [],.    
+00001970: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
+00001980: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001990: 2020 2022 6c65 7665 6c22 3a20 226c 6f77     "level": "low
+000019a0: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+000019b0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000019c0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000019d0: 2022 6964 223a 2022 6465 766c 616b 652d   "id": "devlake-
+000019e0: 3038 222c 0a20 2020 2020 2020 2020 2020  08",.           
+000019f0: 2022 7175 6573 7469 6f6e 223a 2022 446f   "question": "Do
+00001a00: 6573 2044 6576 4c61 6b65 2773 2047 6974  es DevLake's Git
+00001a10: 4875 6220 706c 7567 696e 2073 7570 706f  Hub plugin suppo
+00001a20: 7274 2069 6e63 7265 6d65 6e74 616c 2073  rt incremental s
+00001a30: 796e 633f 222c 0a20 2020 2020 2020 2020  ync?",.         
+00001a40: 2020 2022 7265 6665 7265 6e63 655f 616e     "reference_an
+00001a50: 7377 6572 223a 2022 5965 732e 2044 6576  swer": "Yes. Dev
+00001a60: 4c61 6b65 2773 2047 6974 4875 6220 706c  Lake's GitHub pl
+00001a70: 7567 696e 2073 7570 706f 7274 7320 696e  ugin supports in
+00001a80: 6372 656d 656e 7461 6c20 7379 6e63 2e20  cremental sync. 
+00001a90: 496e 2074 6865 2063 6f64 652c 2079 6f75  In the code, you
+00001aa0: 2063 616e 2073 6565 2074 6865 2066 6f6c   can see the fol
+00001ab0: 6c6f 7769 6e67 206c 696e 653a 5c6e 5c6e  lowing line:\n\n
+00001ac0: 6069 6e63 7265 6d65 6e74 616c 203a 3d20  `incremental := 
+00001ad0: 636f 6c6c 6563 746f 7257 6974 6853 7461  collectorWithSta
+00001ae0: 7465 2e49 7349 6e63 7265 6d65 6e74 616c  te.IsIncremental
+00001af0: 2829 605c 6e5c 6e54 6869 7320 6c69 6e65  ()`\n\nThis line
+00001b00: 2063 6865 636b 7320 6966 2074 6865 2063   checks if the c
+00001b10: 6f6c 6c65 6374 6f72 2069 7320 7275 6e6e  ollector is runn
+00001b20: 696e 6720 696e 2069 6e63 7265 6d65 6e74  ing in increment
+00001b30: 616c 206d 6f64 652e 222c 0a20 2020 2020  al mode.",.     
+00001b40: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
+00001b50: 726f 7065 7274 6965 7322 3a20 5b5d 2c0a  roperties": [],.
+00001b60: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
+00001b70: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
+00001b80: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
+00001b90: 226d 6964 220a 2020 2020 2020 2020 2020  "mid".          
+00001ba0: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+00001bb0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001bc0: 2020 2020 2022 6964 223a 2022 6465 766c       "id": "devl
+00001bd0: 616b 652d 3039 222c 0a20 2020 2020 2020  ake-09",.       
+00001be0: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
+00001bf0: 2022 486f 7720 6361 6e20 4920 6372 6561   "How can I crea
+00001c00: 7465 2044 6576 4c61 6b65 2070 6c75 6769  te DevLake plugi
+00001c10: 6e73 2069 6e20 5079 7468 6f6e 3f22 2c0a  ns in Python?",.
+00001c20: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
+00001c30: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
+00001c40: 2254 6f20 6372 6561 7465 2061 2044 6576  "To create a Dev
+00001c50: 4c61 6b65 2070 6c75 6769 6e20 696e 2050  Lake plugin in P
+00001c60: 7974 686f 6e2c 2066 6f6c 6c6f 7720 7468  ython, follow th
+00001c70: 6573 6520 7374 6570 733a 5c6e 5c6e 312e  ese steps:\n\n1.
+00001c80: 204d 616b 6520 7375 7265 2079 6f75 2068   Make sure you h
+00001c90: 6176 6520 5b50 6f65 7472 795d 2868 7474  ave [Poetry](htt
+00001ca0: 7073 3a2f 2f70 7974 686f 6e2d 706f 6574  ps://python-poet
+00001cb0: 7279 2e6f 7267 2f64 6f63 732f 2369 6e73  ry.org/docs/#ins
+00001cc0: 7461 6c6c 6174 696f 6e29 2069 6e73 7461  tallation) insta
+00001cd0: 6c6c 6564 2e5c 6e32 2e20 4d6f 7665 2074  lled.\n2. Move t
+00001ce0: 6f20 6070 7974 686f 6e2f 706c 7567 696e  o `python/plugin
+00001cf0: 7360 2061 6e64 2065 7865 6375 7465 2060  s` and execute `
+00001d00: 706f 6574 7279 206e 6577 206d 7970 6c75  poetry new myplu
+00001d10: 6769 6e60 2e20 5468 6973 2077 696c 6c20  gin`. This will 
+00001d20: 6765 6e65 7261 7465 2061 206e 6577 2064  generate a new d
+00001d30: 6972 6563 746f 7279 2066 6f72 2079 6f75  irectory for you
+00001d40: 7220 706c 7567 696e 2e5c 6e33 2e20 496e  r plugin.\n3. In
+00001d50: 2074 6865 2060 7079 7072 6f6a 6563 742e   the `pyproject.
+00001d60: 746f 6d6c 6020 6669 6c65 2c20 6164 6420  toml` file, add 
+00001d70: 7468 6520 666f 6c6c 6f77 696e 6720 6c69  the following li
+00001d80: 6e65 2061 7420 7468 6520 656e 6420 6f66  ne at the end of
+00001d90: 2074 6865 2060 5b74 6f6f 6c2e 706f 6574   the `[tool.poet
+00001da0: 7279 2e64 6570 656e 6465 6e63 6965 735d  ry.dependencies]
+00001db0: 6020 7365 6374 696f 6e3a 5c6e 6060 605c  ` section:\n```\
+00001dc0: 6e70 7964 6576 6c61 6b65 203d 207b 2070  npydevlake = { p
+00001dd0: 6174 6820 3d20 5c22 2e2e 2f2e 2e2f 7079  ath = \"../../py
+00001de0: 6465 766c 616b 655c 222c 2064 6576 656c  devlake\", devel
+00001df0: 6f70 203d 2074 7275 6520 7d5c 6e60 6060  op = true }\n```
+00001e00: 5c6e 342e 2052 756e 2060 706f 6574 7279  \n4. Run `poetry
+00001e10: 2069 6e73 7461 6c6c 602e 5c6e 352e 2043   install`.\n5. C
+00001e20: 7265 6174 6520 6120 606d 6169 6e2e 7079  reate a `main.py
+00001e30: 6020 6669 6c65 2077 6974 6820 7468 6520  ` file with the 
+00001e40: 6e65 6365 7373 6172 7920 636f 6e74 656e  necessary conten
+00001e50: 742c 2069 6e63 6c75 6469 6e67 2063 6c61  t, including cla
+00001e60: 7373 6573 2066 6f72 2063 6f6e 6e65 6374  sses for connect
+00001e70: 696f 6e2c 2074 7261 6e73 666f 726d 6174  ion, transformat
+00001e80: 696f 6e20 7275 6c65 2c20 746f 6f6c 2073  ion rule, tool s
+00001e90: 636f 7065 2c20 616e 6420 706c 7567 696e  cope, and plugin
+00001ea0: 2e5c 6e36 2e20 4372 6561 7465 2073 6865  .\n6. Create she
+00001eb0: 6c6c 2073 6372 6970 7473 2060 6275 696c  ll scripts `buil
+00001ec0: 642e 7368 6020 616e 6420 6072 756e 2e73  d.sh` and `run.s
+00001ed0: 6860 2069 6e20 7468 6520 706c 7567 696e  h` in the plugin
+00001ee0: 2072 6f6f 7420 6469 7265 6374 6f72 7920   root directory 
+00001ef0: 746f 2062 7569 6c64 2061 6e64 2072 756e  to build and run
+00001f00: 2074 6865 2070 6c75 6769 6e2e 5c6e 372e   the plugin.\n7.
+00001f10: 2044 6566 696e 6520 636f 6e6e 6563 7469   Define connecti
+00001f20: 6f6e 2070 6172 616d 6574 6572 732c 2074  on parameters, t
+00001f30: 7261 6e73 666f 726d 6174 696f 6e20 7275  ransformation ru
+00001f40: 6c65 2070 6172 616d 6574 6572 732c 2061  le parameters, a
+00001f50: 6e64 2074 6f6f 6c20 7363 6f70 6520 7479  nd tool scope ty
+00001f60: 7065 2e5c 6e38 2e20 496d 706c 656d 656e  pe.\n8. Implemen
+00001f70: 7420 6d65 7468 6f64 7320 6c69 6b65 2060  t methods like `
+00001f80: 646f 6d61 696e 5f73 636f 7065 7360 2c20  domain_scopes`, 
+00001f90: 6072 656d 6f74 655f 7363 6f70 6560 2c20  `remote_scope`, 
+00001fa0: 6072 656d 6f74 655f 7363 6f70 655f 6772  `remote_scope_gr
+00001fb0: 6f75 7073 602c 2061 6e64 2060 7465 7374  oups`, and `test
+00001fc0: 5f63 6f6e 6e65 6374 696f 6e60 2e5c 6e39  _connection`.\n9
+00001fd0: 2e20 4164 6420 6120 6e65 7720 6461 7461  . Add a new data
+00001fe0: 2073 7472 6561 6d20 6279 2063 7265 6174   stream by creat
+00001ff0: 696e 6720 6120 746f 6f6c 206d 6f64 656c  ing a tool model
+00002000: 2c20 7374 7265 616d 2063 6c61 7373 2c20  , stream class, 
+00002010: 616e 6420 4150 4920 7772 6170 7065 722e  and API wrapper.
+00002020: 5c6e 3130 2e20 496d 706c 656d 656e 7420  \n10. Implement 
+00002030: 6d65 7468 6f64 7320 6c69 6b65 2060 636f  methods like `co
+00002040: 6c6c 6563 7460 2c20 6065 7874 7261 6374  llect`, `extract
+00002050: 602c 2061 6e64 2060 636f 6e76 6572 7460  `, and `convert`
+00002060: 2066 6f72 2074 6865 2073 7472 6561 6d20   for the stream 
+00002070: 636c 6173 732e 5c6e 3131 2e20 4966 206e  class.\n11. If n
+00002080: 6565 6465 642c 2063 7265 6174 6520 7375  eeded, create su
+00002090: 6273 7472 6561 6d73 2066 6f72 2068 6965  bstreams for hie
+000020a0: 7261 7263 6869 6361 6c20 6461 7461 2073  rarchical data s
+000020b0: 6f75 7263 6573 2e5c 6e31 322e 2054 6573  ources.\n12. Tes
+000020c0: 7420 7468 6520 706c 7567 696e 2073 7461  t the plugin sta
+000020d0: 6e64 616c 6f6e 6520 7573 696e 6720 7468  ndalone using th
+000020e0: 6520 606d 6169 6e2e 7079 6020 6669 6c65  e `main.py` file
+000020f0: 2077 6974 6820 6469 6666 6572 656e 7420   with different 
+00002100: 636f 6d6d 616e 6473 2e5c 6e31 332e 2057  commands.\n13. W
+00002110: 7269 7465 2075 6e69 742d 7465 7374 7320  rite unit-tests 
+00002120: 666f 7220 796f 7572 2070 6c75 6769 6e20  for your plugin 
+00002130: 636f 6465 2c20 7769 7468 2074 6573 7420  code, with test 
+00002140: 6669 6c65 7320 656e 6469 6e67 2069 6e20  files ending in 
+00002150: 605f 7465 7374 2e70 7960 2e5c 6e5c 6e48  `_test.py`.\n\nH
+00002160: 6572 6527 7320 6120 6765 6e65 7261 6c20  ere's a general 
+00002170: 6f75 746c 696e 6520 6f66 2061 2044 6576  outline of a Dev
+00002180: 4c61 6b65 2070 6c75 6769 6e20 636c 6173  Lake plugin clas
+00002190: 733a 5c6e 5c6e 6060 6070 7974 686f 6e5c  s:\n\n```python\
+000021a0: 6e66 726f 6d20 7079 6465 766c 616b 652e  nfrom pydevlake.
+000021b0: 706c 7567 696e 2069 6d70 6f72 7420 506c  plugin import Pl
+000021c0: 7567 696e 5c6e 5c6e 636c 6173 7320 4d79  ugin\n\nclass My
+000021d0: 4465 764c 616b 6550 6c75 6769 6e28 506c  DevLakePlugin(Pl
+000021e0: 7567 696e 293a 5c6e 2020 2020 2320 496d  ugin):\n    # Im
+000021f0: 706c 656d 656e 7420 7265 7175 6972 6564  plement required
+00002200: 2070 726f 7065 7274 6965 7320 616e 6420   properties and 
+00002210: 6d65 7468 6f64 7320 6865 7265 5c6e 2020  methods here\n  
+00002220: 2020 2320 652e 672e 2c20 6e61 6d65 2c20    # e.g., name, 
+00002230: 6465 7363 7269 7074 696f 6e2c 2063 6f6e  description, con
+00002240: 6e65 6374 696f 6e5f 7479 7065 2c20 746f  nection_type, to
+00002250: 6f6c 5f73 636f 7065 5f74 7970 652c 2074  ol_scope_type, t
+00002260: 7261 6e73 666f 726d 6174 696f 6e5f 7275  ransformation_ru
+00002270: 6c65 5f74 7970 652c 2073 7472 6561 6d73  le_type, streams
+00002280: 2c20 6574 632e 5c6e 6060 605c 6e5c 6e59  , etc.\n```\n\nY
+00002290: 6f75 2077 6f75 6c64 2074 6865 6e20 6e65  ou would then ne
+000022a0: 6564 2074 6f20 696d 706c 656d 656e 7420  ed to implement 
+000022b0: 7468 6520 7265 7175 6972 6564 2070 726f  the required pro
+000022c0: 7065 7274 6965 7320 616e 6420 6d65 7468  perties and meth
+000022d0: 6f64 7320 666f 7220 796f 7572 2073 7065  ods for your spe
+000022e0: 6369 6669 6320 706c 7567 696e 2c20 7375  cific plugin, su
+000022f0: 6368 2061 7320 606e 616d 6560 2c20 6064  ch as `name`, `d
+00002300: 6573 6372 6970 7469 6f6e 602c 2060 636f  escription`, `co
+00002310: 6e6e 6563 7469 6f6e 5f74 7970 6560 2c20  nnection_type`, 
+00002320: 6074 6f6f 6c5f 7363 6f70 655f 7479 7065  `tool_scope_type
+00002330: 602c 2060 7472 616e 7366 6f72 6d61 7469  `, `transformati
+00002340: 6f6e 5f72 756c 655f 7479 7065 602c 2061  on_rule_type`, a
+00002350: 6e64 2060 7374 7265 616d 7360 2e20 596f  nd `streams`. Yo
+00002360: 7520 6361 6e20 7265 6665 7220 746f 2074  u can refer to t
+00002370: 6865 2070 726f 7669 6465 6420 636f 6465  he provided code
+00002380: 2773 2074 6573 7420 6675 6e63 7469 6f6e  's test function
+00002390: 7320 2865 2e67 2e2c 2060 6173 7365 7274  s (e.g., `assert
+000023a0: 5f76 616c 6964 5f6e 616d 6560 2c20 6061  _valid_name`, `a
+000023b0: 7373 6572 745f 7661 6c69 645f 6465 7363  ssert_valid_desc
+000023c0: 7269 7074 696f 6e60 2c20 6061 7373 6572  ription`, `asser
+000023d0: 745f 7661 6c69 645f 636f 6e6e 6563 7469  t_valid_connecti
+000023e0: 6f6e 5f74 7970 6560 2c20 6574 632e 2920  on_type`, etc.) 
+000023f0: 746f 2075 6e64 6572 7374 616e 6420 7468  to understand th
+00002400: 6520 7265 7175 6972 656d 656e 7473 2061  e requirements a
+00002410: 6e64 2063 6f6e 7374 7261 696e 7473 2066  nd constraints f
+00002420: 6f72 2065 6163 6820 7072 6f70 6572 7479  or each property
+00002430: 2061 6e64 206d 6574 686f 642e 5c6e 5c6e   and method.\n\n
+00002440: 4f6e 6365 2079 6f75 2068 6176 6520 696d  Once you have im
+00002450: 706c 656d 656e 7465 6420 796f 7572 2070  plemented your p
+00002460: 6c75 6769 6e2c 2079 6f75 2063 616e 2075  lugin, you can u
+00002470: 7365 2074 6865 2070 726f 7669 6465 6420  se the provided 
+00002480: 7465 7374 2066 756e 6374 696f 6e73 2074  test functions t
+00002490: 6f20 7661 6c69 6461 7465 2079 6f75 7220  o validate your 
+000024a0: 706c 7567 696e 2061 6e64 2065 6e73 7572  plugin and ensur
+000024b0: 6520 6974 2077 6f72 6b73 2063 6f72 7265  e it works corre
+000024c0: 6374 6c79 2e22 2c0a 2020 2020 2020 2020  ctly.",.        
+000024d0: 2020 2020 2261 6e73 7765 725f 7072 6f70      "answer_prop
+000024e0: 6572 7469 6573 223a 205b 5d2c 0a20 2020  erties": [],.   
+000024f0: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
+00002500: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00002510: 2020 2020 226c 6576 656c 223a 2022 6c6f      "level": "lo
+00002520: 7722 0a20 2020 2020 2020 2020 2020 207d  w".            }
+00002530: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00002540: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00002550: 2020 2269 6422 3a20 2264 6576 6c61 6b65    "id": "devlake
+00002560: 2d31 3022 2c0a 2020 2020 2020 2020 2020  -10",.          
+00002570: 2020 2271 7565 7374 696f 6e22 3a20 2248    "question": "H
+00002580: 6f77 2064 6f20 4920 7265 736f 6c76 6520  ow do I resolve 
+00002590: 7468 6520 6070 616e 6963 3a20 696e 7661  the `panic: inva
+000025a0: 6c69 6420 656e 634b 6579 6020 6572 726f  lid encKey` erro
+000025b0: 723f 222c 0a20 2020 2020 2020 2020 2020  r?",.           
+000025c0: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
+000025d0: 6572 223a 2022 546f 2072 6573 6f6c 7665  er": "To resolve
+000025e0: 2074 6865 2027 7061 6e69 633a 2069 6e76   the 'panic: inv
+000025f0: 616c 6964 2065 6e63 4b65 7927 2065 7272  alid encKey' err
+00002600: 6f72 2c20 796f 7520 6e65 6564 2074 6f20  or, you need to 
+00002610: 656e 7375 7265 2074 6861 7420 796f 7520  ensure that you 
+00002620: 6861 7665 2061 2076 616c 6964 2065 6e63  have a valid enc
+00002630: 7279 7074 696f 6e20 6b65 7920 7365 7420  ryption key set 
+00002640: 696e 2079 6f75 7220 656e 7669 726f 6e6d  in your environm
+00002650: 656e 7420 6f72 2063 6f6e 6669 6775 7261  ent or configura
+00002660: 7469 6f6e 2e20 4865 7265 2061 7265 2073  tion. Here are s
+00002670: 6f6d 6520 7374 6570 7320 796f 7520 6361  ome steps you ca
+00002680: 6e20 666f 6c6c 6f77 3a5c 6e5c 6e31 2e20  n follow:\n\n1. 
+00002690: 4d61 6b65 2073 7572 6520 796f 7520 6861  Make sure you ha
+000026a0: 7665 2061 2076 616c 6964 2065 6e63 7279  ve a valid encry
+000026b0: 7074 696f 6e20 6b65 7920 616e 6420 6974  ption key and it
+000026c0: 2773 2062 6569 6e67 2063 6f72 7265 6374  's being correct
+000026d0: 6c79 2066 6574 6368 6564 2075 7369 6e67  ly fetched using
+000026e0: 2074 6865 2060 706c 7567 696e 2e45 6e63   the `plugin.Enc
+000026f0: 6f64 654b 6579 456e 7653 7472 6020 636f  odeKeyEnvStr` co
+00002700: 6e73 7461 6e74 206f 7220 6120 7369 6d69  nstant or a simi
+00002710: 6c61 7220 6d65 7468 6f64 2069 6e20 796f  lar method in yo
+00002720: 7572 2063 6f64 652e 5c6e 322e 2049 6620  ur code.\n2. If 
+00002730: 796f 7520 6172 6520 7573 696e 6720 6120  you are using a 
+00002740: 7261 6e64 6f6d 6c79 2067 656e 6572 6174  randomly generat
+00002750: 6564 2065 6e63 7279 7074 696f 6e20 6b65  ed encryption ke
+00002760: 792c 206d 616b 6520 7375 7265 2074 6f20  y, make sure to 
+00002770: 7374 6f72 6520 6974 2073 6563 7572 656c  store it securel
+00002780: 7920 616e 6420 7573 6520 7468 6520 7361  y and use the sa
+00002790: 6d65 206b 6579 2066 6f72 2062 6f74 6820  me key for both 
+000027a0: 656e 6372 7970 7469 6f6e 2061 6e64 2064  encryption and d
+000027b0: 6563 7279 7074 696f 6e20 7072 6f63 6573  ecryption proces
+000027c0: 7365 732e 5c6e 332e 2043 6865 636b 2074  ses.\n3. Check t
+000027d0: 6861 7420 7468 6520 656e 7669 726f 6e6d  hat the environm
+000027e0: 656e 7420 7661 7269 6162 6c65 2073 7065  ent variable spe
+000027f0: 6369 6669 6564 2062 7920 6070 6c75 6769  cified by `plugi
+00002800: 6e2e 456e 636f 6465 4b65 7945 6e76 5374  n.EncodeKeyEnvSt
+00002810: 7260 206f 7220 6120 7369 6d69 6c61 7220  r` or a similar 
+00002820: 6d65 7468 6f64 2069 7320 7365 7420 7769  method is set wi
+00002830: 7468 2061 2076 616c 6964 2065 6e63 7279  th a valid encry
+00002840: 7074 696f 6e20 6b65 792e 5c6e 342e 2056  ption key.\n4. V
+00002850: 6572 6966 7920 7468 6174 2074 6865 2065  erify that the e
+00002860: 6e63 4b65 7920 6973 2062 6569 6e67 2073  ncKey is being s
+00002870: 6574 2061 6e64 2073 6176 6564 2074 6f20  et and saved to 
+00002880: 7468 6520 636f 6e66 6967 2070 726f 7065  the config prope
+00002890: 726c 7920 7573 696e 6720 6076 2e53 6574  rly using `v.Set
+000028a0: 2870 6c75 6769 6e2e 456e 636f 6465 4b65  (plugin.EncodeKe
+000028b0: 7945 6e76 5374 722c 2065 6e63 4b65 7929  yEnvStr, encKey)
+000028c0: 6020 616e 6420 6063 6f6e 6669 672e 5772  ` and `config.Wr
+000028d0: 6974 6543 6f6e 6669 6728 7629 6020 6f72  iteConfig(v)` or
+000028e0: 2073 696d 696c 6172 206d 6574 686f 6473   similar methods
+000028f0: 2069 6e20 796f 7572 2063 6f64 652e 5c6e   in your code.\n
+00002900: 5c6e 4966 2074 6865 2069 7373 7565 2070  \nIf the issue p
+00002910: 6572 7369 7374 732c 2079 6f75 206d 6179  ersists, you may
+00002920: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
+00002930: 206d 6f72 6520 636f 6e74 6578 7420 6f72   more context or
+00002940: 2072 6566 6572 2074 6f20 7468 6520 646f   refer to the do
+00002950: 6375 6d65 6e74 6174 696f 6e20 6f66 2074  cumentation of t
+00002960: 6865 2073 7065 6369 6669 6320 736f 6674  he specific soft
+00002970: 7761 7265 2079 6f75 2061 7265 2077 6f72  ware you are wor
+00002980: 6b69 6e67 2077 6974 682e 222c 0a20 2020  king with.",.   
+00002990: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
+000029a0: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
+000029b0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+000029c0: 6f74 6573 223a 207b 0a20 2020 2020 2020  otes": {.       
+000029d0: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
+000029e0: 3a20 226d 6964 220a 2020 2020 2020 2020  : "mid".        
+000029f0: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
+00002a00: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00002a10: 2020 2020 2020 2022 6964 223a 2022 6465         "id": "de
+00002a20: 766c 616b 652d 3131 222c 0a20 2020 2020  vlake-11",.     
+00002a30: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
+00002a40: 223a 2022 486f 7720 646f 6573 2044 6576  ": "How does Dev
+00002a50: 4c61 6b65 2067 656e 6572 6174 6520 6120  Lake generate a 
+00002a60: 7069 7065 6c69 6e65 2062 6173 6564 206f  pipeline based o
+00002a70: 6e20 6120 626c 7565 7072 696e 7427 7320  n a blueprint's 
+00002a80: 7365 7474 696e 673f 222c 0a20 2020 2020  setting?",.     
+00002a90: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
+00002aa0: 655f 616e 7377 6572 223a 2022 4465 764c  e_answer": "DevL
+00002ab0: 616b 6520 6765 6e65 7261 7465 7320 6120  ake generates a 
 00002ac0: 7069 7065 6c69 6e65 2062 6173 6564 206f  pipeline based o
 00002ad0: 6e20 6120 626c 7565 7072 696e 7427 7320  n a blueprint's 
-00002ae0: 7365 7474 696e 673f 222c 0d0a 2020 2020  setting?",..    
-00002af0: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
-00002b00: 6365 5f61 6e73 7765 7222 3a20 2244 6576  ce_answer": "Dev
-00002b10: 4c61 6b65 2067 656e 6572 6174 6573 2061  Lake generates a
-00002b20: 2070 6970 656c 696e 6520 6261 7365 6420   pipeline based 
-00002b30: 6f6e 2061 2062 6c75 6570 7269 6e74 2773  on a blueprint's
-00002b40: 2073 6574 7469 6e67 2074 6872 6f75 6768   setting through
-00002b50: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
-00002b60: 7465 7073 3a5c 6e5c 6e31 2e20 5468 6520  teps:\n\n1. The 
-00002b70: 626c 7565 7072 696e 7420 7365 7474 696e  blueprint settin
-00002b80: 6773 2061 7265 2064 6566 696e 6564 2069  gs are defined i
-00002b90: 6e20 6120 4a53 4f4e 2066 6f72 6d61 742c  n a JSON format,
-00002ba0: 2077 6869 6368 2069 6e63 6c75 6465 7320   which includes 
-00002bb0: 7468 6520 7665 7273 696f 6e2c 2063 6f6e  the version, con
-00002bc0: 6e65 6374 696f 6e73 2c20 706c 7567 696e  nections, plugin
-00002bd0: 2c20 636f 6e6e 6563 7469 6f6e 4964 2c20  , connectionId, 
-00002be0: 616e 6420 7363 6f70 6573 2e5c 6e5c 6e32  and scopes.\n\n2
-00002bf0: 2e20 5468 6520 6050 6c75 6769 6e42 6c75  . The `PluginBlu
-00002c00: 6570 7269 6e74 5632 3030 2e4d 616b 6550  eprintV200.MakeP
-00002c10: 6970 656c 696e 6550 6c61 6e60 2066 756e  ipelinePlan` fun
-00002c20: 6374 696f 6e20 6973 2063 616c 6c65 6420  ction is called 
-00002c30: 7769 7468 2061 6e20 6172 7261 7920 6f66  with an array of
-00002c40: 2073 636f 7065 732e 2054 6865 2070 6c75   scopes. The plu
-00002c50: 6769 6e20 7265 7475 726e 7320 6120 6050  gin returns a `P
-00002c60: 6970 656c 696e 6550 6c61 6e60 2069 6e20  ipelinePlan` in 
-00002c70: 4a53 4f4e 2066 6f72 6d61 7420 616e 6420  JSON format and 
-00002c80: 616e 2061 7272 6179 206f 6620 6053 636f  an array of `Sco
-00002c90: 7065 6020 666f 7220 7072 6f6a 6563 745f  pe` for project_
-00002ca0: 6d61 7070 696e 672e 5c6e 5c6e 332e 2054  mapping.\n\n3. T
-00002cb0: 6865 2066 7261 6d65 776f 726b 206d 6169  he framework mai
-00002cc0: 6e74 6169 6e73 2074 6865 2070 726f 6a65  ntains the proje
-00002cd0: 6374 5f6d 6170 7069 6e67 2074 6162 6c65  ct_mapping table
-00002ce0: 2062 6173 6564 206f 6e20 7468 6520 605b   based on the `[
-00002cf0: 5d53 636f 7065 6020 6172 7261 792e 5c6e  ]Scope` array.\n
-00002d00: 5c6e 5468 6573 6520 7374 6570 7320 6865  \nThese steps he
-00002d10: 6c70 2044 6576 4c61 6b65 2067 656e 6572  lp DevLake gener
-00002d20: 6174 6520 6120 7069 7065 6c69 6e65 2070  ate a pipeline p
-00002d30: 6c61 6e20 6261 7365 6420 6f6e 2074 6865  lan based on the
-00002d40: 2062 6c75 6570 7269 6e74 2773 2073 6574   blueprint's set
-00002d50: 7469 6e67 732c 2077 6869 6368 2063 616e  tings, which can
-00002d60: 2062 6520 7573 6564 2074 6f20 6578 6563   be used to exec
-00002d70: 7574 6520 7468 6520 7069 7065 6c69 6e65  ute the pipeline
-00002d80: 2061 6e64 2063 6f6c 6c65 6374 2064 6174   and collect dat
-00002d90: 6120 6672 6f6d 2076 6172 696f 7573 2073  a from various s
-00002da0: 6f75 7263 6573 2e22 2c0d 0a20 2020 2020  ources.",..     
-00002db0: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
-00002dc0: 726f 7065 7274 6965 7322 3a20 5b5d 2c0d  roperties": [],.
-00002dd0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00002de0: 7465 7322 3a20 7b0d 0a20 2020 2020 2020  tes": {..       
-00002df0: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
-00002e00: 3a20 226c 6f77 220d 0a20 2020 2020 2020  : "low"..       
-00002e10: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00002e20: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00002e30: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00002e40: 2022 6465 766c 616b 652d 3132 222c 0d0a   "devlake-12",..
-00002e50: 2020 2020 2020 2020 2020 2020 2271 7565              "que
-00002e60: 7374 696f 6e22 3a20 2248 6f77 2064 6f65  stion": "How doe
-00002e70: 7320 4465 764c 616b 6520 6465 6c65 7465  s DevLake delete
-00002e80: 2061 2070 726f 6a65 6374 3f22 2c0d 0a20   a project?",.. 
-00002e90: 2020 2020 2020 2020 2020 2022 7265 6665             "refe
-00002ea0: 7265 6e63 655f 616e 7377 6572 223a 2022  rence_answer": "
-00002eb0: 4465 764c 616b 6520 6465 6c65 7465 7320  DevLake deletes 
-00002ec0: 6120 7072 6f6a 6563 7420 6279 2066 6f6c  a project by fol
-00002ed0: 6c6f 7769 6e67 2074 6865 7365 2073 7465  lowing these ste
-00002ee0: 7073 3a5c 6e5c 6e31 2e20 5665 7269 6679  ps:\n\n1. Verify
-00002ef0: 2074 6865 2069 6e70 7574 2070 726f 6a65   the input proje
-00002f00: 6374 206e 616d 6520 6973 206e 6f74 2065  ct name is not e
-00002f10: 6d70 7479 2e5c 6e32 2e20 4265 6769 6e20  mpty.\n2. Begin 
-00002f20: 6120 6461 7461 6261 7365 2074 7261 6e73  a database trans
-00002f30: 6163 7469 6f6e 2e5c 6e33 2e20 4765 7420  action.\n3. Get 
-00002f40: 7468 6520 7072 6f6a 6563 7420 6279 2069  the project by i
-00002f50: 7473 206e 616d 6520 7573 696e 6720 7468  ts name using th
-00002f60: 6520 6067 6574 5072 6f6a 6563 7442 794e  e `getProjectByN
-00002f70: 616d 6560 2066 756e 6374 696f 6e2e 5c6e  ame` function.\n
-00002f80: 342e 2044 656c 6574 6520 7468 6520 7072  4. Delete the pr
-00002f90: 6f6a 6563 7420 6672 6f6d 2074 6865 2060  oject from the `
-00002fa0: 6d6f 6465 6c73 2e50 726f 6a65 6374 6020  models.Project` 
-00002fb0: 7461 626c 6520 7573 696e 6720 7468 6520  table using the 
-00002fc0: 7072 6f6a 6563 7420 6e61 6d65 2e5c 6e35  project name.\n5
-00002fd0: 2e20 4465 6c65 7465 2074 6865 2070 726f  . Delete the pro
-00002fe0: 6a65 6374 206d 6170 7069 6e67 2066 726f  ject mapping fro
-00002ff0: 6d20 7468 6520 6063 726f 7373 646f 6d61  m the `crossdoma
-00003000: 696e 2e50 726f 6a65 6374 4d61 7070 696e  in.ProjectMappin
-00003010: 6760 2074 6162 6c65 2075 7369 6e67 2074  g` table using t
-00003020: 6865 2070 726f 6a65 6374 206e 616d 652e  he project name.
-00003030: 5c6e 362e 2044 656c 6574 6520 7468 6520  \n6. Delete the 
-00003040: 7072 6f6a 6563 7420 6d65 7472 6963 2073  project metric s
-00003050: 6574 7469 6e67 2066 726f 6d20 7468 6520  etting from the 
-00003060: 606d 6f64 656c 732e 5072 6f6a 6563 744d  `models.ProjectM
-00003070: 6574 7269 6353 6574 7469 6e67 6020 7461  etricSetting` ta
-00003080: 626c 6520 7573 696e 6720 7468 6520 7072  ble using the pr
-00003090: 6f6a 6563 7420 6e61 6d65 2e5c 6e37 2e20  oject name.\n7. 
-000030a0: 4465 6c65 7465 2074 6865 2070 726f 6a65  Delete the proje
-000030b0: 6374 2050 5220 6d65 7472 6963 2066 726f  ct PR metric fro
-000030c0: 6d20 7468 6520 6063 726f 7373 646f 6d61  m the `crossdoma
-000030d0: 696e 2e50 726f 6a65 6374 5072 4d65 7472  in.ProjectPrMetr
-000030e0: 6963 6020 7461 626c 6520 7573 696e 6720  ic` table using 
-000030f0: 7468 6520 7072 6f6a 6563 7420 6e61 6d65  the project name
-00003100: 2e5c 6e38 2e20 4465 6c65 7465 2074 6865  .\n8. Delete the
-00003110: 2070 726f 6a65 6374 2069 7373 7565 206d   project issue m
-00003120: 6574 7269 6320 6672 6f6d 2074 6865 2060  etric from the `
-00003130: 6372 6f73 7364 6f6d 6169 6e2e 5072 6f6a  crossdomain.Proj
-00003140: 6563 7449 7373 7565 4d65 7472 6963 6020  ectIssueMetric` 
-00003150: 7461 626c 6520 7573 696e 6720 7468 6520  table using the 
-00003160: 7072 6f6a 6563 7420 6e61 6d65 2e5c 6e39  project name.\n9
-00003170: 2e20 436f 6d6d 6974 2074 6865 2074 7261  . Commit the tra
-00003180: 6e73 6163 7469 6f6e 2e5c 6e31 302e 2047  nsaction.\n10. G
-00003190: 6574 2074 6865 2062 6c75 6570 7269 6e74  et the blueprint
-000031a0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000031b0: 2074 6865 2070 726f 6a65 6374 206e 616d   the project nam
-000031c0: 6520 7573 696e 6720 7468 6520 6062 704d  e using the `bpM
-000031d0: 616e 6167 6572 2e47 6574 4462 426c 7565  anager.GetDbBlue
-000031e0: 7072 696e 7442 7950 726f 6a65 6374 4e61  printByProjectNa
-000031f0: 6d65 6020 6675 6e63 7469 6f6e 2e5c 6e31  me` function.\n1
-00003200: 312e 2044 656c 6574 6520 7468 6520 626c  1. Delete the bl
-00003210: 7565 7072 696e 7420 7573 696e 6720 7468  ueprint using th
-00003220: 6520 6062 704d 616e 6167 6572 2e44 656c  e `bpManager.Del
-00003230: 6574 6542 6c75 6570 7269 6e74 6020 6675  eteBlueprint` fu
-00003240: 6e63 7469 6f6e 2077 6974 6820 7468 6520  nction with the 
-00003250: 626c 7565 7072 696e 7420 4944 2e22 2c0d  blueprint ID.",.
-00003260: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
-00003270: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
-00003280: 3a20 5b5d 2c0d 0a20 2020 2020 2020 2020  : [],..         
-00003290: 2020 2022 6e6f 7465 7322 3a20 7b0d 0a20     "notes": {.. 
-000032a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000032b0: 6c65 7665 6c22 3a20 2268 6967 6822 0d0a  level": "high"..
-000032c0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-000032d0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000032e0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000032f0: 2020 2269 6422 3a20 2264 6576 6c61 6b65    "id": "devlake
-00003300: 2d31 3322 2c0d 0a20 2020 2020 2020 2020  -13",..         
-00003310: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
-00003320: 486f 7720 646f 6573 2044 6576 4c61 6b65  How does DevLake
-00003330: 2067 656e 6572 6174 6520 7468 6520 7465   generate the te
-00003340: 6d70 6c61 7465 2060 7573 6572 5f61 6363  mplate `user_acc
-00003350: 6f75 6e74 5f6d 6170 7069 6e67 2e63 7376  ount_mapping.csv
-00003360: 6020 6669 6c65 3f22 2c0d 0a20 2020 2020  ` file?",..     
-00003370: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
-00003380: 655f 616e 7377 6572 223a 2022 4465 764c  e_answer": "DevL
-00003390: 616b 6520 6765 6e65 7261 7465 7320 7468  ake generates th
-000033a0: 6520 7465 6d70 6c61 7465 2075 7365 725f  e template user_
-000033b0: 6163 636f 756e 745f 6d61 7070 696e 672e  account_mapping.
-000033c0: 6373 7620 6669 6c65 2075 7369 6e67 2074  csv file using t
-000033d0: 6865 2047 6574 5573 6572 4163 636f 756e  he GetUserAccoun
-000033e0: 744d 6170 7069 6e67 2066 756e 6374 696f  tMapping functio
-000033f0: 6e2e 2054 6869 7320 6675 6e63 7469 6f6e  n. This function
-00003400: 2072 6574 7269 6576 6573 2061 6c6c 2075   retrieves all u
-00003410: 7365 722f 6163 636f 756e 7420 6d61 7070  ser/account mapp
-00003420: 696e 6773 2066 726f 6d20 7468 6520 7374  ings from the st
-00003430: 6f72 652c 206d 6172 7368 616c 7320 7468  ore, marshals th
-00003440: 656d 2069 6e74 6f20 4353 5620 666f 726d  em into CSV form
-00003450: 6174 2075 7369 6e67 2067 6f63 7376 2e4d  at using gocsv.M
-00003460: 6172 7368 616c 4279 7465 7328 6163 636f  arshalBytes(acco
-00003470: 756e 7473 292c 2061 6e64 2072 6574 7572  unts), and retur
-00003480: 6e73 2074 6865 2043 5356 2064 6174 6120  ns the CSV data 
-00003490: 6173 2061 6e20 4f75 7470 7574 4669 6c65  as an OutputFile
-000034a0: 2077 6974 6820 436f 6e74 656e 7454 7970   with ContentTyp
-000034b0: 6520 5c22 7465 7874 2f63 7376 5c22 2e22  e \"text/csv\"."
-000034c0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000034d0: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
-000034e0: 7322 3a20 5b5d 2c0d 0a20 2020 2020 2020  s": [],..       
-000034f0: 2020 2020 2022 6e6f 7465 7322 3a20 7b0d       "notes": {.
-00003500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003510: 2022 6c65 7665 6c22 3a20 2268 6967 6822   "level": "high"
-00003520: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-00003530: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00003540: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00003550: 2020 2020 2269 6422 3a20 2264 6576 6c61      "id": "devla
-00003560: 6b65 2d31 3422 2c0d 0a20 2020 2020 2020  ke-14",..       
-00003570: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
-00003580: 2022 486f 7720 6973 2074 6865 2060 6669   "How is the `fi
-00003590: 6e64 416c 6c41 6363 6f75 6e74 7360 2066  ndAllAccounts` f
-000035a0: 756e 6374 696f 6e20 696d 706c 656d 656e  unction implemen
-000035b0: 7465 643f 222c 0d0a 2020 2020 2020 2020  ted?",..        
-000035c0: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
-000035d0: 6e73 7765 7222 3a20 2222 2c0d 0a20 2020  nswer": "",..   
-000035e0: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
-000035f0: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
-00003600: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00003610: 6e6f 7465 7322 3a20 7b0d 0a20 2020 2020  notes": {..     
-00003620: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
-00003630: 6c22 3a20 226c 6f77 220d 0a20 2020 2020  l": "low"..     
-00003640: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00003650: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
-00003660: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
-00003670: 223a 2022 6465 766c 616b 652d 3135 222c  ": "devlake-15",
-00003680: 0d0a 2020 2020 2020 2020 2020 2020 2271  ..            "q
-00003690: 7565 7374 696f 6e22 3a20 2248 6f77 2069  uestion": "How i
-000036a0: 7320 7468 6520 6068 2e73 746f 7265 2e66  s the `h.store.f
-000036b0: 696e 6441 6c6c 4163 636f 756e 7473 6020  indAllAccounts` 
-000036c0: 6675 6e63 7469 6f6e 2069 6d70 6c65 6d65  function impleme
-000036d0: 6e74 6564 3f22 2c0d 0a20 2020 2020 2020  nted?",..       
-000036e0: 2020 2020 2022 7265 6665 7265 6e63 655f       "reference_
-000036f0: 616e 7377 6572 223a 2022 5468 6520 682e  answer": "The h.
-00003700: 7374 6f72 652e 6669 6e64 416c 6c41 6363  store.findAllAcc
-00003710: 6f75 6e74 7320 6675 6e63 7469 6f6e 2069  ounts function i
-00003720: 7320 696d 706c 656d 656e 7465 6420 6173  s implemented as
-00003730: 2066 6f6c 6c6f 7773 3a5c 6e5c 6e60 6060   follows:\n\n```
-00003740: 676f 5c6e 6675 6e63 2028 6420 2a64 6253  go\nfunc (d *dbS
-00003750: 746f 7265 2920 6669 6e64 416c 6c41 6363  tore) findAllAcc
-00003760: 6f75 6e74 7328 2920 285b 5d61 6363 6f75  ounts() ([]accou
-00003770: 6e74 2c20 6572 726f 7273 2e45 7272 6f72  nt, errors.Error
-00003780: 2920 7b5c 6e5c 7476 6172 2061 6120 5b5d  ) {\n\tvar aa []
-00003790: 6372 6f73 7364 6f6d 6169 6e2e 4163 636f  crossdomain.Acco
-000037a0: 756e 745c 6e5c 7465 7272 203a 3d20 642e  unt\n\terr := d.
-000037b0: 6462 2e41 6c6c 2826 6161 295c 6e5c 7469  db.All(&aa)\n\ti
-000037c0: 6620 6572 7220 213d 206e 696c 207b 5c6e  f err != nil {\n
-000037d0: 5c74 5c74 7265 7475 726e 206e 696c 2c20  \t\treturn nil, 
-000037e0: 6572 725c 6e5c 747d 5c6e 5c74 7661 7220  err\n\t}\n\tvar 
-000037f0: 7561 205b 5d63 726f 7373 646f 6d61 696e  ua []crossdomain
-00003800: 2e55 7365 7241 6363 6f75 6e74 5c6e 5c74  .UserAccount\n\t
-00003810: 6572 7220 3d20 642e 6462 2e41 6c6c 2826  err = d.db.All(&
-00003820: 7561 295c 6e5c 7469 6620 6572 7220 213d  ua)\n\tif err !=
-00003830: 206e 696c 207b 5c6e 5c74 5c74 7265 7475   nil {\n\t\tretu
-00003840: 726e 206e 696c 2c20 6572 725c 6e5c 747d  rn nil, err\n\t}
-00003850: 5c6e 5c74 7661 7220 6120 2a61 6363 6f75  \n\tvar a *accou
-00003860: 6e74 5c6e 5c74 7265 7475 726e 2061 2e66  nt\n\treturn a.f
-00003870: 726f 6d44 6f6d 6169 6e4c 6179 6572 2861  romDomainLayer(a
-00003880: 612c 2075 6129 2c20 6e69 6c5c 6e7d 5c6e  a, ua), nil\n}\n
-00003890: 6060 605c 6e5c 6e49 7420 7265 7472 6965  ```\n\nIt retrie
-000038a0: 7665 7320 616c 6c20 6163 636f 756e 7473  ves all accounts
-000038b0: 2061 6e64 2075 7365 7220 6163 636f 756e   and user accoun
-000038c0: 7473 2066 726f 6d20 7468 6520 6461 7461  ts from the data
-000038d0: 6261 7365 2c20 616e 6420 7468 656e 2063  base, and then c
-000038e0: 616c 6c73 2074 6865 2066 726f 6d44 6f6d  alls the fromDom
-000038f0: 6169 6e4c 6179 6572 2066 756e 6374 696f  ainLayer functio
-00003900: 6e20 746f 2063 6f6e 7665 7274 2074 6865  n to convert the
-00003910: 6d20 696e 746f 2074 6865 2061 7070 726f  m into the appro
-00003920: 7072 6961 7465 2066 6f72 6d61 742e 222c  priate format.",
-00003930: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-00003940: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-00003950: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-00003960: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 226c 6576 656c 223a 2022 6c6f 7722 0d0a  "level": "low"..
-00003990: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-000039a0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000039b0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000039c0: 2020 2269 6422 3a20 2264 6576 6c61 6b65    "id": "devlake
-000039d0: 2d31 3622 2c0d 0a20 2020 2020 2020 2020  -16",..         
-000039e0: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
-000039f0: 486f 7720 6973 2074 6865 2060 6672 6f6d  How is the `from
-00003a00: 446f 6d61 696e 4c61 7965 7260 206d 6574  DomainLayer` met
-00003a10: 686f 6420 6f66 2074 6865 2061 6363 6f75  hod of the accou
-00003a20: 6e74 2074 7970 6520 696d 706c 656d 656e  nt type implemen
-00003a30: 7465 643f 222c 0d0a 2020 2020 2020 2020  ted?",..        
-00003a40: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
-00003a50: 6e73 7765 7222 3a20 2222 2c0d 0a20 2020  nswer": "",..   
-00003a60: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
-00003a70: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
-00003a80: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00003a90: 6e6f 7465 7322 3a20 7b0d 0a20 2020 2020  notes": {..     
-00003aa0: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
-00003ab0: 6c22 3a20 226c 6f77 220d 0a20 2020 2020  l": "low"..     
-00003ac0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00003ad0: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
-00003ae0: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
-00003af0: 223a 2022 6465 766c 616b 652d 3137 222c  ": "devlake-17",
-00003b00: 0d0a 2020 2020 2020 2020 2020 2020 2271  ..            "q
-00003b10: 7565 7374 696f 6e22 3a20 2249 7320 7468  uestion": "Is th
-00003b20: 6520 696e 666f 726d 6174 696f 6e20 636f  e information co
-00003b30: 6c6c 6563 7465 6420 6672 6f6d 2061 6c6c  llected from all
-00003b40: 2062 7261 6e63 6865 7320 6672 6f6d 2067   branches from g
-00003b50: 6974 3f22 2c0d 0a20 2020 2020 2020 2020  it?",..         
-00003b60: 2020 2022 7265 6665 7265 6e63 655f 616e     "reference_an
-00003b70: 7377 6572 223a 2022 5468 6520 6769 7420  swer": "The git 
-00003b80: 6578 7472 6163 746f 7220 706c 7567 696e  extractor plugin
-00003b90: 2063 6f6c 6c65 6374 7320 636f 6d6d 6974   collects commit
-00003ba0: 7320 6f6e 2061 6c6c 2062 7261 6e63 6865  s on all branche
-00003bb0: 732e 222c 0d0a 2020 2020 2020 2020 2020  s.",..          
-00003bc0: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
-00003bd0: 7469 6573 223a 205b 5d2c 0d0a 2020 2020  ties": [],..    
-00003be0: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
-00003bf0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00003c00: 2020 2020 226c 6576 656c 223a 2022 6c6f      "level": "lo
-00003c10: 7722 0d0a 2020 2020 2020 2020 2020 2020  w"..            
-00003c20: 7d0d 0a20 2020 2020 2020 207d 2c0d 0a20  }..        },.. 
-00003c30: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00003c40: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
-00003c50: 6c61 6b65 2d31 3822 2c0d 0a20 2020 2020  lake-18",..     
-00003c60: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
-00003c70: 223a 2022 446f 6573 2044 6576 4c61 6b65  ": "Does DevLake
-00003c80: 2073 7570 706f 7274 2050 6f73 7467 7265   support Postgre
-00003c90: 5351 4c3f 222c 0d0a 2020 2020 2020 2020  SQL?",..        
-00003ca0: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
-00003cb0: 6e73 7765 7222 3a20 2259 6573 2c20 506f  nswer": "Yes, Po
-00003cc0: 7374 6772 6553 514c 2069 7320 7375 7070  stgreSQL is supp
-00003cd0: 6f72 7465 6420 666f 7220 616c 6c20 7665  orted for all ve
-00003ce0: 7273 696f 6e73 2066 726f 6d20 7630 2e31  rsions from v0.1
-00003cf0: 3120 7570 2c20 6275 7420 7468 6520 7072  1 up, but the pr
-00003d00: 652d 6275 696c 7420 4772 6166 616e 6120  e-built Grafana 
-00003d10: 6461 7368 626f 6172 6473 206f 6e6c 7920  dashboards only 
-00003d20: 7375 7070 6f72 7420 4d79 5351 4c2e 2050  support MySQL. P
-00003d30: 6f73 7467 7265 5351 4c20 7375 7070 6f72  ostgreSQL suppor
-00003d40: 7420 6973 206e 6f74 2062 6569 6e67 2072  t is not being r
-00003d50: 656d 6f76 6564 2065 6e74 6972 656c 792c  emoved entirely,
-00003d60: 2062 7574 2074 6865 2072 656c 6174 6564   but the related
-00003d70: 2069 6e66 6f72 6d61 7469 6f6e 2068 6173   information has
-00003d80: 2062 6565 6e20 7465 6d70 6f72 6172 696c   been temporaril
-00003d90: 7920 7265 6d6f 7665 6420 6475 6520 746f  y removed due to
-00003da0: 2074 6865 2070 6172 7469 616c 2063 6f6d   the partial com
-00003db0: 7061 7469 6269 6c69 7479 2077 6974 6820  patibility with 
-00003dc0: 4772 6166 616e 6120 6461 7368 626f 6172  Grafana dashboar
-00003dd0: 6473 2e20 5573 6572 7320 7768 6f20 7761  ds. Users who wa
-00003de0: 6e74 2074 6f20 7573 6520 506f 7374 6772  nt to use Postgr
-00003df0: 6553 514c 2077 6974 6820 4465 764c 616b  eSQL with DevLak
-00003e00: 6520 6361 6e20 7374 696c 6c20 646f 2073  e can still do s
-00003e10: 6f2c 2062 7574 2074 6865 7920 6d61 7920  o, but they may 
-00003e20: 6e65 6564 2074 6f20 636f 6e76 6572 7420  need to convert 
-00003e30: 7468 6520 4d79 5351 4c20 7175 6572 6965  the MySQL querie
-00003e40: 7320 7072 6f76 6964 6564 2062 7920 4465  s provided by De
-00003e50: 764c 616b 6520 746f 2050 6f73 7467 7265  vLake to Postgre
-00003e60: 5351 4c2e 222c 0d0a 2020 2020 2020 2020  SQL.",..        
-00003e70: 2020 2020 2261 6e73 7765 725f 7072 6f70      "answer_prop
-00003e80: 6572 7469 6573 223a 205b 5d2c 0d0a 2020  erties": [],..  
-00003e90: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
-00003ea0: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00003eb0: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
-00003ec0: 6c6f 7722 0d0a 2020 2020 2020 2020 2020  low"..          
-00003ed0: 2020 7d0d 0a20 2020 2020 2020 207d 2c0d    }..        },.
-00003ee0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-00003ef0: 2020 2020 2020 2020 2269 6422 3a20 2264          "id": "d
-00003f00: 6576 6c61 6b65 2d31 3922 2c0d 0a20 2020  evlake-19",..   
-00003f10: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
-00003f20: 6f6e 223a 2022 5768 7920 6973 2069 7420  on": "Why is it 
-00003f30: 7468 6174 206e 6f74 2061 6c6c 206f 7267  that not all org
-00003f40: 616e 6973 6174 696f 6e73 2069 6e20 6d79  anisations in my
-00003f50: 2047 6974 6875 6220 6172 6520 6265 696e   Github are bein
-00003f60: 6720 7368 6f77 6e3f 222c 0d0a 2020 2020  g shown?",..    
-00003f70: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
-00003f80: 6365 5f61 6e73 7765 7222 3a20 2249 6620  ce_answer": "If 
-00003f90: 796f 7527 7265 206e 6f74 2073 6565 696e  you're not seein
-00003fa0: 6720 616c 6c20 6f66 2079 6f75 7220 4769  g all of your Gi
-00003fb0: 7448 7562 206f 7267 732c 2070 6c65 6173  tHub orgs, pleas
-00003fc0: 6520 6368 6563 6b20 6966 2079 6f75 7220  e check if your 
-00003fd0: 4769 7448 7562 206f 7267 2068 6173 2061  GitHub org has a
-00003fe0: 6c6c 6f77 6564 2050 4154 2061 6363 6573  llowed PAT acces
-00003ff0: 732e 222c 0d0a 2020 2020 2020 2020 2020  s.",..          
-00004000: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
-00004010: 7469 6573 223a 205b 5d2c 0d0a 2020 2020  ties": [],..    
-00004020: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
-00004030: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00004040: 2020 2020 226c 6576 656c 223a 2022 6d69      "level": "mi
-00004050: 6422 0d0a 2020 2020 2020 2020 2020 2020  d"..            
-00004060: 7d0d 0a20 2020 2020 2020 207d 2c0d 0a20  }..        },.. 
-00004070: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00004080: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
-00004090: 6c61 6b65 2d32 3022 2c0d 0a20 2020 2020  lake-20",..     
-000040a0: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
-000040b0: 223a 2022 4973 2069 7420 706f 7373 6962  ": "Is it possib
-000040c0: 6c65 2074 6f20 636f 6e73 756d 6520 6576  le to consume ev
-000040d0: 656e 7473 2f64 6174 6120 6672 6f6d 2061  ents/data from a
-000040e0: 2073 7472 6561 6d20 696e 7374 6561 6420   stream instead 
-000040f0: 6f66 2070 756c 6c69 6e67 2061 6e20 4150  of pulling an AP
-00004100: 493f 222c 0d0a 2020 2020 2020 2020 2020  I?",..          
-00004110: 2020 2272 6566 6572 656e 6365 5f61 6e73    "reference_ans
-00004120: 7765 7222 3a20 2244 6576 4c61 6b65 2064  wer": "DevLake d
-00004130: 6f65 736e e280 9974 2068 6176 6520 6675  oesn...t have fu
-00004140: 6c6c 2d62 6c6f 776e 2073 7570 706f 7274  ll-blown support
-00004150: 2066 6f72 2063 6f6e 7375 6d69 6e67 2065   for consuming e
-00004160: 7665 6e74 732f 6461 7461 2066 726f 6d20  vents/data from 
-00004170: 6120 7374 7265 616d 2061 7320 6f66 2072  a stream as of r
-00004180: 6967 6874 206e 6f77 2e20 4275 7420 7468  ight now. But th
-00004190: 6572 6527 7320 616e 2069 6e63 6f6d 696e  ere's an incomin
-000041a0: 6720 7765 6268 6f6f 6b20 6665 6174 7572  g webhook featur
-000041b0: 6520 666f 7220 7265 6769 7374 6572 696e  e for registerin
-000041c0: 6720 6465 706c 6f79 6d65 6e74 7320 7769  g deployments wi
-000041d0: 7468 2044 6576 4c61 6b65 2e22 2c0d 0a20  th DevLake.",.. 
-000041e0: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
-000041f0: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
-00004200: 5b5d 2c0d 0a20 2020 2020 2020 2020 2020  [],..           
-00004210: 2022 6e6f 7465 7322 3a20 7b0d 0a20 2020   "notes": {..   
-00004220: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
-00004230: 7665 6c22 3a20 226c 6f77 220d 0a20 2020  vel": "low"..   
-00004240: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00004250: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00004260: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00004270: 6964 223a 2022 6465 766c 616b 652d 3231  id": "devlake-21
-00004280: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004290: 2271 7565 7374 696f 6e22 3a20 2249 7320  "question": "Is 
-000042a0: 4465 766c 616b 6520 6d6f 7669 6e67 2074  Devlake moving t
-000042b0: 6f20 5079 7468 6f6e 2062 6173 6564 2070  o Python based p
-000042c0: 6c75 6769 6e20 7261 7468 6572 2074 6861  lugin rather tha
-000042d0: 6e20 476f 4c61 6e67 3f22 2c0d 0a20 2020  n GoLang?",..   
-000042e0: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-000042f0: 6e63 655f 616e 7377 6572 223a 2022 4465  nce_answer": "De
-00004300: 764c 616b 6520 7769 6c6c 2073 7570 706f  vLake will suppo
-00004310: 7274 2062 6f74 6820 476f 6c61 6e67 2061  rt both Golang a
-00004320: 6e64 2050 7974 686f 6e20 706c 7567 696e  nd Python plugin
-00004330: 2066 6f72 2074 6865 2066 6f72 6573 6565   for the foresee
-00004340: 6162 6c65 2066 7574 7572 652c 2062 7574  able future, but
-00004350: 2077 6527 7265 2069 6e64 6565 6420 656e   we're indeed en
-00004360: 636f 7572 6167 696e 6720 7573 6572 7320  couraging users 
-00004370: 746f 2074 7279 206f 7574 2074 6865 206e  to try out the n
-00004380: 6577 2070 7974 686f 6e20 5344 4b2c 2077  ew python SDK, w
-00004390: 6869 6368 2069 7320 6f75 7220 6174 7465  hich is our atte
-000043a0: 6d70 7420 746f 2069 6d70 726f 7665 2064  mpt to improve d
-000043b0: 6576 656c 6f70 6572 2065 7870 6572 6965  eveloper experie
-000043c0: 6e63 6520 666f 7220 706c 7567 696e 2064  nce for plugin d
-000043d0: 6576 656c 6f70 6d65 6e74 2e22 2c0d 0a20  evelopment.",.. 
-000043e0: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
-000043f0: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
-00004400: 5b5d 2c0d 0a20 2020 2020 2020 2020 2020  [],..           
-00004410: 2022 6e6f 7465 7322 3a20 7b0d 0a20 2020   "notes": {..   
-00004420: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
-00004430: 7665 6c22 3a20 226d 6964 220d 0a20 2020  vel": "mid"..   
-00004440: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00004450: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00004460: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00004470: 6964 223a 2022 6465 766c 616b 652d 3232  id": "devlake-22
-00004480: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004490: 2271 7565 7374 696f 6e22 3a20 2249 2064  "question": "I d
-000044a0: 6f20 6e6f 7420 7365 6520 616e 7974 6869  o not see anythi
-000044b0: 6e67 206f 6e20 444f 5241 2064 6173 6862  ng on DORA dashb
-000044c0: 6f61 7264 2c20 6361 6e20 616e 796f 6e65  oard, can anyone
-000044d0: 2068 656c 7020 7769 7468 2074 6869 733f   help with this?
-000044e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000044f0: 2272 6566 6572 656e 6365 5f61 6e73 7765  "reference_answe
-00004500: 7222 3a20 2274 6f20 6865 6c70 2077 6974  r": "to help wit
-00004510: 6820 7468 6520 444f 5241 2063 6f6e 6669  h the DORA confi
-00004520: 6775 7261 7469 6f6e 2070 726f 6365 7373  guration process
-00004530: 2c20 4920 7265 636f 6d6d 656e 6420 676f  , I recommend go
-00004540: 696e 6720 7468 726f 7567 6820 6f75 7220  ing through our 
-00004550: 444f 5241 2067 7569 6465 3a20 6874 7470  DORA guide: http
-00004560: 733a 2f2f 6465 766c 616b 652e 6170 6163  s://devlake.apac
-00004570: 6865 2e6f 7267 2f64 6f63 732f 6e65 7874  he.org/docs/next
-00004580: 2f44 4f52 412f 2e20 596f 7520 6361 6e20  /DORA/. You can 
-00004590: 616c 736f 2066 696e 6420 646f 6373 2066  also find docs f
-000045a0: 6f72 2074 6865 2074 6f6f 6c73 2079 6f75  or the tools you
-000045b0: 2075 7365 2068 6572 653a 2068 7474 7073   use here: https
-000045c0: 3a2f 2f64 6576 6c61 6b65 2e61 7061 6368  ://devlake.apach
-000045d0: 652e 6f72 672f 646f 6373 2f6e 6578 742f  e.org/docs/next/
-000045e0: 436f 6e66 6967 7572 6174 696f 6e22 2c0d  Configuration",.
-000045f0: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
-00004600: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
-00004610: 3a20 5b5d 2c0d 0a20 2020 2020 2020 2020  : [],..         
-00004620: 2020 2022 6e6f 7465 7322 3a20 7b0d 0a20     "notes": {.. 
-00004630: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004640: 6c65 7665 6c22 3a20 226d 6964 220d 0a20  level": "mid".. 
-00004650: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00004660: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00004670: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00004680: 2022 6964 223a 2022 6465 766c 616b 652d   "id": "devlake-
-00004690: 3233 222c 0d0a 2020 2020 2020 2020 2020  23",..          
-000046a0: 2020 2271 7565 7374 696f 6e22 3a20 2244    "question": "D
-000046b0: 6f65 7320 4170 6163 6865 2044 6576 6c61  oes Apache Devla
-000046c0: 6b65 2073 7570 706f 7274 7320 6465 706c  ke supports depl
-000046d0: 6f79 6d65 6e74 206d 6574 7269 6373 2066  oyment metrics f
-000046e0: 726f 6d20 436c 6f75 6442 7569 6c64 2c20  rom CloudBuild, 
-000046f0: 436c 6f75 6420 4465 706c 6f79 2061 6e64  Cloud Deploy and
-00004700: 2041 6e74 686f 7320 436f 6e66 6967 204d   Anthos Config M
-00004710: 616e 6167 656d 656e 743f 222c 0d0a 2020  anagement?",..  
-00004720: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
-00004730: 656e 6365 5f61 6e73 7765 7222 3a20 2244  ence_answer": "D
-00004740: 6576 4c61 6b65 2068 6173 6e27 7420 7375  evLake hasn't su
-00004750: 7070 6f72 7465 6420 436c 6f75 6442 7569  pported CloudBui
-00004760: 6c64 2c20 436c 6f75 6420 6465 706c 6f79  ld, Cloud deploy
-00004770: 2061 6e64 2041 434d 2079 6574 2e20 4665   and ACM yet. Fe
-00004780: 656c 2066 7265 6520 746f 206f 7065 6e20  el free to open 
-00004790: 6665 6174 7572 6520 7265 7175 6573 7420  feature request 
-000047a0: 6973 7375 6520 6f6e 2047 6974 4875 622e  issue on GitHub.
-000047b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000047c0: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
-000047d0: 6573 223a 205b 5d2c 0d0a 2020 2020 2020  es": [],..      
-000047e0: 2020 2020 2020 226e 6f74 6573 223a 207b        "notes": {
-000047f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004800: 2020 226c 6576 656c 223a 2022 6c6f 7722    "level": "low"
-00004810: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-00004820: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00004830: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00004840: 2020 2020 2269 6422 3a20 2264 6576 6c61      "id": "devla
-00004850: 6b65 2d32 3422 2c0d 0a20 2020 2020 2020  ke-24",..       
-00004860: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
-00004870: 2022 4920 6861 7665 2073 6574 2075 7020   "I have set up 
-00004880: 4465 764c 616b 6520 6f6e 6c79 2074 6f20  DevLake only to 
-00004890: 636f 6c6c 6563 7420 7468 6520 444f 5241  collect the DORA
-000048a0: 206d 6574 7269 6373 2075 7369 6e67 2068   metrics using h
-000048b0: 656c 6d20 6275 7420 6974 2069 7320 6f70  elm but it is op
-000048c0: 656e 696e 6720 7468 6520 4465 764c 616b  ening the DevLak
-000048d0: 6520 5549 2077 6974 686f 7574 2061 6e79  e UI without any
-000048e0: 2061 7574 6865 6e74 6963 6174 696f 6e2c   authentication,
-000048f0: 2069 2e65 2e20 6e6f 2075 7365 726e 616d   i.e. no usernam
-00004900: 6520 616e 6420 7061 7373 776f 7264 2e20  e and password. 
-00004910: 4173 2049 2061 6d20 656e 7465 7269 6e67  As I am entering
-00004920: 2074 6865 2049 5020 6974 2069 7320 7461   the IP it is ta
-00004930: 6b69 6e67 206d 6520 746f 2044 6576 6c61  king me to Devla
-00004940: 6b65 2064 6173 6862 6f61 7264 2077 6974  ke dashboard wit
-00004950: 686f 7574 2061 736b 696e 6720 616e 7920  hout asking any 
-00004960: 7573 6572 6e61 6d65 2061 6e64 2070 6173  username and pas
-00004970: 7377 6f72 642e 2049 7320 6974 2074 6865  sword. Is it the
-00004980: 2063 6f72 7265 6374 2062 6568 6176 696f   correct behavio
-00004990: 7572 3f22 2c0d 0a20 2020 2020 2020 2020  ur?",..         
-000049a0: 2020 2022 7265 6665 7265 6e63 655f 616e     "reference_an
-000049b0: 7377 6572 223a 2022 5468 6572 6520 6172  swer": "There ar
-000049c0: 6520 7661 6c75 6573 2074 6f20 7365 7420  e values to set 
-000049d0: 7573 6572 2f70 6173 7377 6f72 6420 696e  user/password in
-000049e0: 2074 6865 2068 656c 6d20 6368 6172 742e   the helm chart.
-000049f0: 2042 7920 6465 6661 756c 742c 2074 6865   By default, the
-00004a00: 7920 6172 6520 6e6f 7420 7365 742e 222c  y are not set.",
-00004a10: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-00004a20: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-00004a30: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-00004a40: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a60: 226c 6576 656c 223a 2022 6d69 6422 0d0a  "level": "mid"..
-00004a70: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00004a80: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00004a90: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00004aa0: 2020 2269 6422 3a20 2264 6576 6c61 6b65    "id": "devlake
-00004ab0: 2d32 3522 2c0d 0a20 2020 2020 2020 2020  -25",..         
-00004ac0: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
-00004ad0: 446f 2079 6f75 2068 6176 6520 706c 616e  Do you have plan
-00004ae0: 7320 746f 2061 6464 2075 7365 7220 6d61  s to add user ma
-00004af0: 6e61 6765 6d65 6e74 2069 6e20 4465 764c  nagement in DevL
-00004b00: 616b 6520 5549 3f20 222c 0d0a 2020 2020  ake UI? ",..    
-00004b10: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
-00004b20: 6365 5f61 6e73 7765 7222 3a20 2254 6865  ce_answer": "The
-00004b30: 2063 7572 7265 6e74 2070 6c61 6e20 6973   current plan is
-00004b40: 2074 6f20 e280 9c6f 7574 736f 7572 6365   to ...outsource
-00004b50: e280 9d20 7573 6572 206d 616e 6167 656d  ... user managem
-00004b60: 656e 7420 746f 2070 726f 6a65 6374 7320  ent to projects 
-00004b70: 6c69 6b65 206f 6175 7468 322d 7072 6f78  like oauth2-prox
-00004b80: 7920 696e 7374 6561 6420 6f66 2072 6569  y instead of rei
-00004b90: 6e76 656e 7469 6e67 2074 6865 2077 6865  nventing the whe
-00004ba0: 656c 2069 6e20 686f 7573 652e 2057 6520  el in house. We 
-00004bb0: 7769 6c6c 2073 6565 2069 6620 7765 2063  will see if we c
-00004bc0: 616e 2072 6f6c 6c20 6f75 7420 6120 626c  an roll out a bl
-00004bd0: 6f67 206f 6e20 686f 7720 746f 2070 726f  og on how to pro
-00004be0: 7465 6374 2043 6f6e 6669 672d 5549 2077  tect Config-UI w
-00004bf0: 6974 6820 6f61 7574 6832 2d70 726f 7879  ith oauth2-proxy
-00004c00: 2061 7320 6120 7374 6172 7469 6e67 2070   as a starting p
-00004c10: 6f69 6e74 2066 6f72 2075 7365 7273 2077  oint for users w
-00004c20: 686f 2061 7265 2069 6e74 6572 6573 7465  ho are intereste
-00004c30: 6420 696e 2067 6f69 6e67 2064 6f77 6e20  d in going down 
-00004c40: 7468 6174 2070 6174 682e 222c 0d0a 2020  that path.",..  
-00004c50: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
-00004c60: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
-00004c70: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00004c80: 226e 6f74 6573 223a 207b 0d0a 2020 2020  "notes": {..    
-00004c90: 2020 2020 2020 2020 2020 2020 226c 6576              "lev
-00004ca0: 656c 223a 2022 6869 6768 220d 0a20 2020  el": "high"..   
-00004cb0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00004cc0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00004cd0: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00004ce0: 6964 223a 2022 6465 766c 616b 652d 3236  id": "devlake-26
-00004cf0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00004d00: 2271 7565 7374 696f 6e22 3a20 2257 6520  "question": "We 
-00004d10: 6861 7665 2064 6f7a 656e 7320 6f66 2047  have dozens of G
-00004d20: 6974 4875 6220 6f72 6761 6e69 7a61 7469  itHub organizati
-00004d30: 6f6e 7320 616e 6420 6875 6e64 7265 6473  ons and hundreds
-00004d40: 206f 6620 7265 706f 7369 746f 7269 6573   of repositories
-00004d50: 2074 6f20 7472 6163 6b2e 2041 7420 7468   to track. At th
-00004d60: 6174 2073 6361 6c65 2069 7420 6973 2064  at scale it is d
-00004d70: 6966 6669 6375 6c74 2074 6f20 6d61 6e61  ifficult to mana
-00004d80: 6765 2075 7369 6e67 2074 6865 2050 726f  ge using the Pro
-00004d90: 6a65 6374 2069 6e74 6572 6661 6365 2061  ject interface a
-00004da0: 6e64 2055 492e 2048 6173 2061 6e79 6f6e  nd UI. Has anyon
-00004db0: 6520 7472 6965 6420 746f 2075 7365 2044  e tried to use D
-00004dc0: 6576 4c61 6b65 2074 6f20 776f 726b 2077  evLake to work w
-00004dd0: 6974 6820 616e 7974 6869 6e67 2063 6c6f  ith anything clo
-00004de0: 7365 2074 6f20 7468 6174 206b 696e 6420  se to that kind 
-00004df0: 6f66 2073 6361 6c65 3f22 2c0d 0a20 2020  of scale?",..   
-00004e00: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-00004e10: 6e63 655f 616e 7377 6572 223a 2022 496e  nce_answer": "In
-00004e20: 2043 6f6e 6669 6720 5549 2c20 796f 7520   Config UI, you 
-00004e30: 6361 6e20 7472 7920 7365 6c65 6374 696e  can try selectin
-00004e40: 6720 7468 6520 6f72 6720 746f 2073 656c  g the org to sel
-00004e50: 6563 7420 616c 6c20 7265 706f 7369 746f  ect all reposito
-00004e60: 7269 6573 2075 6e64 6572 2074 6861 7420  ries under that 
-00004e70: 6f72 672e 2042 7574 2069 6620 796f 7520  org. But if you 
-00004e80: 6e65 6564 2074 6f20 6164 6420 6120 6c61  need to add a la
-00004e90: 7267 6520 6e75 6d62 6572 206f 6620 7265  rge number of re
-00004ea0: 706f 7369 746f 7269 6573 2075 6e64 6572  positories under
-00004eb0: 2064 6966 6665 7265 6e74 206f 7267 7320   different orgs 
-00004ec0: 746f 2061 2070 726f 6a65 6374 2c20 7468  to a project, th
-00004ed0: 6520 6163 7469 6f6e 2077 696c 6c20 6265  e action will be
-00004ee0: 2069 6e65 7669 7461 626c 7920 6375 6d62   inevitably cumb
-00004ef0: 6572 736f 6d65 2069 6e20 7468 6520 6375  ersome in the cu
-00004f00: 7272 656e 7420 4465 764c 616b 652e 222c  rrent DevLake.",
-00004f10: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-00004f20: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-00004f30: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-00004f40: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 226c 6576 656c 223a 2022 6869 6768 220d  "level": "high".
-00004f70: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-00004f80: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00004f90: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00004fa0: 2020 2022 6964 223a 2022 6465 766c 616b     "id": "devlak
-00004fb0: 652d 3237 222c 0d0a 2020 2020 2020 2020  e-27",..        
-00004fc0: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
-00004fd0: 2249 2077 616e 7420 746f 2064 6566 696e  "I want to defin
-00004fe0: 6520 736f 6d65 2063 6f6d 6d69 7473 2061  e some commits a
-00004ff0: 7320 6465 706c 6f79 6d65 6e74 206a 6f62  s deployment job
-00005000: 732c 2073 7563 6820 6173 2063 6f6d 6d69  s, such as commi
-00005010: 7420 6d65 7373 6167 6573 2073 7461 7274  t messages start
-00005020: 696e 6720 7769 7468 20e2 809c 6d65 7267  ing with ...merg
-00005030: 652e 2ee2 809d 206f 7220 736f 6d65 2073  e..... or some s
-00005040: 7065 6369 6669 6320 6163 636f 756e 7420  pecific account 
-00005050: 6c69 6b65 2061 646d 696e 2e20 486f 7720  like admin. How 
-00005060: 6361 6e20 4920 646f 2074 6869 733f 222c  can I do this?",
-00005070: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00005080: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-00005090: 3a20 2249 6620 4920 756e 6465 7273 7461  : "If I understa
-000050a0: 6e64 2063 6f72 7265 6374 6c79 2c20 796f  nd correctly, yo
-000050b0: 7520 776f 756c 6420 6c69 6b65 2074 6f20  u would like to 
-000050c0: 7265 6769 7374 6572 2064 6570 6c6f 796d  register deploym
-000050d0: 656e 7473 2077 6974 6820 636f 6d6d 6974  ents with commit
-000050e0: 7320 6669 6c74 6572 6564 2062 7920 7468  s filtered by th
-000050f0: 6569 7220 636f 6d6d 6974 206d 6573 7361  eir commit messa
-00005100: 6765 732e 2054 6869 7320 6973 206e 6f74  ges. This is not
-00005110: 2073 7570 706f 7274 6564 206e 6174 6976   supported nativ
-00005120: 656c 7920 6279 2044 6576 4c61 6b65 2e20  ely by DevLake. 
-00005130: 4275 7420 6120 706f 7465 6e74 6961 6c20  But a potential 
-00005140: 776f 726b 6172 6f75 6e64 2069 7320 746f  workaround is to
-00005150: 2077 7269 7465 2061 2073 6372 6970 7420   write a script 
-00005160: 7468 6174 2074 616b 6573 2079 6f75 7220  that takes your 
-00005170: 6769 7420 7265 706f 2061 7320 696e 7075  git repo as inpu
-00005180: 742c 2066 696c 7465 7220 7468 6520 636f  t, filter the co
-00005190: 6d6d 6974 7320 7769 7468 2079 6f75 7220  mmits with your 
-000051a0: 7275 6c65 732c 2061 6e64 2073 656e 6420  rules, and send 
-000051b0: 504f 5354 2072 6571 7565 7374 7320 746f  POST requests to
-000051c0: 2044 6576 4c61 6b65 2074 6f20 7265 6769   DevLake to regi
-000051d0: 7374 6572 2074 6865 2064 6570 6c6f 796d  ster the deploym
-000051e0: 656e 7473 2075 7369 6e67 2044 6576 4c61  ents using DevLa
-000051f0: 6b65 2773 2069 6e63 6f6d 696e 6720 7765  ke's incoming we
-00005200: 6268 6f6f 6b20 666f 7220 6465 706c 6f79  bhook for deploy
-00005210: 6d65 6e74 733a 2068 7474 7073 3a2f 2f64  ments: https://d
-00005220: 6576 6c61 6b65 2e61 7061 6368 652e 6f72  evlake.apache.or
-00005230: 672f 646f 6373 2f6e 6578 742f 506c 7567  g/docs/next/Plug
-00005240: 696e 732f 7765 6268 6f6f 6b22 2c0d 0a20  ins/webhook",.. 
-00005250: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
-00005260: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
-00005270: 5b5d 2c0d 0a20 2020 2020 2020 2020 2020  [],..           
-00005280: 2022 6e6f 7465 7322 3a20 7b0d 0a20 2020   "notes": {..   
-00005290: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
-000052a0: 7665 6c22 3a20 2268 6967 6822 0d0a 2020  vel": "high"..  
-000052b0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-000052c0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-000052d0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000052e0: 2269 6422 3a20 2264 6576 6c61 6b65 2d32  "id": "devlake-2
-000052f0: 3822 2c0d 0a20 2020 2020 2020 2020 2020  8",..           
-00005300: 2022 7175 6573 7469 6f6e 223a 2022 446f   "question": "Do
-00005310: 6573 204c 6561 6420 5469 6d65 2066 6f72  es Lead Time for
-00005320: 2043 6861 6e67 6573 2073 7570 706f 7274   Changes support
-00005330: 2074 7275 6e6b 2d62 6173 6564 2064 6576   trunk-based dev
-00005340: 656c 6f70 6d65 6e74 3f22 2c0d 0a20 2020  elopment?",..   
-00005350: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-00005360: 6e63 655f 616e 7377 6572 223a 2022 5468  nce_answer": "Th
-00005370: 6520 6375 7272 656e 7420 6c65 6164 2074  e current lead t
-00005380: 696d 6520 666f 7220 6368 616e 6765 7320  ime for changes 
-00005390: 6973 2050 522d 6261 7365 6420 616e 6420  is PR-based and 
-000053a0: 776f 756c 6420 6e65 6564 2073 6f6d 6520  would need some 
-000053b0: 6164 6a75 7374 6d65 6e74 2066 6f72 2064  adjustment for d
-000053c0: 6972 6563 7420 7075 7368 2069 6e74 6f20  irect push into 
-000053d0: 7472 756e 6b2e 222c 0d0a 2020 2020 2020  trunk.",..      
-000053e0: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
-000053f0: 6f70 6572 7469 6573 223a 205b 5d2c 0d0a  operties": [],..
-00005400: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
-00005410: 6573 223a 207b 0d0a 2020 2020 2020 2020  es": {..        
-00005420: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
-00005430: 2022 6c6f 7722 0d0a 2020 2020 2020 2020   "low"..        
-00005440: 2020 2020 7d0d 0a20 2020 2020 2020 207d      }..        }
-00005450: 2c0d 0a20 2020 2020 2020 207b 0d0a 2020  ,..        {..  
-00005460: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-00005470: 2264 6576 6c61 6b65 2d32 3922 2c0d 0a20  "devlake-29",.. 
-00005480: 2020 2020 2020 2020 2020 2022 7175 6573             "ques
-00005490: 7469 6f6e 223a 2022 486f 7720 6361 6e20  tion": "How can 
-000054a0: 4920 6465 706c 6f79 2044 6576 4c61 6b65  I deploy DevLake
-000054b0: 2077 6974 6820 356b 2b20 7265 706f 7369   with 5k+ reposi
-000054c0: 746f 7269 6573 2077 6974 686f 7574 2063  tories without c
-000054d0: 6f6e 7374 616e 746c 7920 6869 7474 696e  onstantly hittin
-000054e0: 6720 7468 6520 7261 7465 206c 696d 6974  g the rate limit
-000054f0: 2070 726f 626c 656d 3f22 2c0d 0a20 2020   problem?",..   
-00005500: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-00005510: 6e63 655f 616e 7377 6572 223a 2022 312e  nce_answer": "1.
-00005520: 2044 6576 4c61 6b65 2773 2047 6974 4875   DevLake's GitHu
-00005530: 6220 706c 7567 696e 2064 6f65 7320 696e  b plugin does in
-00005540: 6372 656d 656e 7461 6c20 7379 6e63 2066  cremental sync f
-00005550: 6f72 206d 6f73 7420 656e 7469 7469 6573  or most entities
-00005560: 2e20 546f 2073 6565 2074 6865 2062 6568  . To see the beh
-00005570: 6176 696f 7220 6f66 206f 7468 6572 2070  avior of other p
-00005580: 6c75 6769 6e73 2c20 6368 6563 6b20 6f75  lugins, check ou
-00005590: 7420 7468 6520 436f 6c6c 6563 7469 6f6e  t the Collection
-000055a0: 204d 6f64 6520 636f 6c75 6d6e 2068 6572   Mode column her
-000055b0: 653a 2068 7474 7073 3a2f 2f64 6576 6c61  e: https://devla
-000055c0: 6b65 2e61 7061 6368 652e 6f72 672f 646f  ke.apache.org/do
-000055d0: 6373 2f6e 6578 742f 4f76 6572 7669 6577  cs/next/Overview
-000055e0: 2f53 7570 706f 7274 6564 4461 7461 536f  /SupportedDataSo
-000055f0: 7572 6365 7320 322e 2050 726f 7669 6469  urces 2. Providi
-00005600: 6e67 206d 756c 7469 706c 6520 4769 7448  ng multiple GitH
-00005610: 7562 2050 4154 7320 6672 6f6d 2064 6966  ub PATs from dif
-00005620: 6665 7265 6e74 2075 7365 7273 2077 6f75  ferent users wou
-00005630: 6c64 206d 756c 7469 706c 7920 796f 7572  ld multiply your
-00005640: 2072 6174 6520 6c69 6d69 742e 2033 2e20   rate limit. 3. 
-00005650: 5468 6572 6527 7320 616e 206f 7065 6e20  There's an open 
-00005660: 5052 2066 6f72 2073 7570 706f 7274 696e  PR for supportin
-00005670: 6720 4769 7448 7562 2061 7070 2c20 7768  g GitHub app, wh
-00005680: 6963 6820 6d61 7920 656e 6861 6e63 6520  ich may enhance 
-00005690: 7468 6520 7261 7465 206c 696d 6974 2066  the rate limit f
-000056a0: 6f72 206c 6172 6765 7220 6f72 6773 2e22  or larger orgs."
-000056b0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000056c0: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
-000056d0: 7322 3a20 5b5d 2c0d 0a20 2020 2020 2020  s": [],..       
-000056e0: 2020 2020 2022 6e6f 7465 7322 3a20 7b0d       "notes": {.
-000056f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005700: 2022 6c65 7665 6c22 3a20 2268 6967 6822   "level": "high"
-00005710: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-00005720: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00005730: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00005740: 2020 2020 2269 6422 3a20 2264 6576 6c61      "id": "devla
-00005750: 6b65 2d33 3022 2c0d 0a20 2020 2020 2020  ke-30",..       
-00005760: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
-00005770: 2022 5768 656e 2063 7265 6174 696e 6720   "When creating 
-00005780: 7465 616d 732c 2069 6620 4920 6861 7665  teams, if I have
-00005790: 2061 2068 6965 7261 7263 6879 206f 6620   a hierarchy of 
-000057a0: 7061 7265 6e74 7320 616e 6420 7375 622d  parents and sub-
-000057b0: 7465 616d 732c 2064 6f20 4920 6e65 6564  teams, do I need
-000057c0: 2074 6f20 7075 7420 7468 6520 7375 622d   to put the sub-
-000057d0: 7465 616d 206d 656d 6265 7273 2069 6e20  team members in 
-000057e0: 626f 7468 2070 6172 656e 7473 2061 6e64  both parents and
-000057f0: 2073 7562 2d74 6561 6d73 2c20 6f72 206a   sub-teams, or j
-00005800: 7573 7420 7375 622d 7465 616d 733f 222c  ust sub-teams?",
-00005810: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00005820: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-00005830: 3a20 2254 6561 6d73 2077 6974 6869 6e20  : "Teams within 
-00005840: 4465 764c 616b 6520 646f 6e27 7420 6861  DevLake don't ha
-00005850: 7665 2068 6965 7261 7263 6869 6573 2e20  ve hierarchies. 
-00005860: 536f 2079 6f75 2070 726f 6261 626c 7920  So you probably 
-00005870: 7761 6e74 2074 6f20 7075 7420 7468 6520  want to put the 
-00005880: 7375 622d 7465 616d 206d 656d 6265 7273  sub-team members
-00005890: 2069 6e20 626f 7468 2074 6865 2070 6172   in both the par
-000058a0: 656e 7420 616e 6420 7375 622d 7465 616d  ent and sub-team
-000058b0: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-000058c0: 2022 616e 7377 6572 5f70 726f 7065 7274   "answer_propert
-000058d0: 6965 7322 3a20 5b5d 2c0d 0a20 2020 2020  ies": [],..     
-000058e0: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
-000058f0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00005900: 2020 2022 6c65 7665 6c22 3a20 226d 6964     "level": "mid
-00005910: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
-00005920: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00005930: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00005940: 2020 2020 2022 6964 223a 2022 6465 766c       "id": "devl
-00005950: 616b 652d 3331 222c 0d0a 2020 2020 2020  ake-31",..      
-00005960: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00005970: 3a20 2249 7320 5353 4f20 7375 7070 6f72  : "Is SSO suppor
-00005980: 7465 6420 666f 7220 7468 6520 4465 764c  ted for the DevL
-00005990: 616b 6520 5549 2061 6e64 2074 6865 2064  ake UI and the d
-000059a0: 6173 6862 6f61 7264 733f 222c 0d0a 2020  ashboards?",..  
-000059b0: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
-000059c0: 656e 6365 5f61 6e73 7765 7222 3a20 2253  ence_answer": "S
-000059d0: 534f 2069 7320 6e6f 7420 7375 7070 6f72  SO is not suppor
-000059e0: 7465 6420 6375 7272 656e 746c 792e 222c  ted currently.",
-000059f0: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-00005a00: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-00005a10: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-00005a20: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a40: 226c 6576 656c 223a 2022 6c6f 7722 0d0a  "level": "low"..
-00005a50: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00005a60: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00005a70: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00005a80: 2020 2269 6422 3a20 2264 6576 6c61 6b65    "id": "devlake
-00005a90: 2d33 3222 2c0d 0a20 2020 2020 2020 2020  -32",..         
-00005aa0: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
-00005ab0: 4920 656e 7465 7265 6420 6120 4769 7448  I entered a GitH
-00005ac0: 7562 2074 6f6b 656e 2062 7574 2069 7420  ub token but it 
-00005ad0: 7368 6f77 6564 2060 494e 5641 4c49 4420  showed `INVALID 
-00005ae0: 544f 4b45 4e60 2e20 5768 6174 2063 6f75  TOKEN`. What cou
-00005af0: 6c64 2062 6520 7468 6520 6361 7573 6573  ld be the causes
-00005b00: 3f22 2c0d 0a20 2020 2020 2020 2020 2020  ?",..           
-00005b10: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
-00005b20: 6572 223a 2022 506c 6561 7365 2072 6566  er": "Please ref
-00005b30: 6572 2074 6f20 6f75 7220 646f 6373 2066  er to our docs f
-00005b40: 6f72 2077 6861 7420 7065 726d 6973 7369  or what permissi
-00005b50: 6f6e 7320 6f66 2047 6974 4875 6220 746f  ons of GitHub to
-00005b60: 6b65 6e73 2061 7265 2072 6571 7569 7265  kens are require
-00005b70: 643a 2068 7474 7073 3a2f 2f64 6576 6c61  d: https://devla
-00005b80: 6b65 2e61 7061 6368 652e 6f72 672f 646f  ke.apache.org/do
-00005b90: 6373 2f43 6f6e 6669 6775 7261 7469 6f6e  cs/Configuration
-00005ba0: 2f47 6974 4875 6222 2c0d 0a20 2020 2020  /GitHub",..     
-00005bb0: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
-00005bc0: 726f 7065 7274 6965 7322 3a20 5b5d 2c0d  roperties": [],.
-00005bd0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00005be0: 7465 7322 3a20 7b0d 0a20 2020 2020 2020  tes": {..       
-00005bf0: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
-00005c00: 3a20 226c 6f77 220d 0a20 2020 2020 2020  : "low"..       
-00005c10: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00005c20: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00005c30: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00005c40: 2022 6465 766c 616b 652d 3333 222c 0d0a   "devlake-33",..
-00005c50: 2020 2020 2020 2020 2020 2020 2271 7565              "que
-00005c60: 7374 696f 6e22 3a20 2243 616e 2049 2066  stion": "Can I f
-00005c70: 696c 7465 7220 6f75 7420 4769 7448 7562  ilter out GitHub
-00005c80: 2069 7373 7565 7320 6372 6561 7465 6420   issues created 
-00005c90: 6279 2062 6f74 733f 222c 0d0a 2020 2020  by bots?",..    
-00005ca0: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
-00005cb0: 6365 5f61 6e73 7765 7222 3a20 2255 6e66  ce_answer": "Unf
-00005cc0: 6f72 7475 6e61 7465 6c79 2c20 7468 6572  ortunately, ther
-00005cd0: 6520 6973 206e 6f20 6275 696c 742d 696e  e is no built-in
-00005ce0: 2063 6170 6162 696c 6974 7920 7769 7468   capability with
-00005cf0: 696e 2044 6576 4c61 6b65 2074 6f20 6175  in DevLake to au
-00005d00: 746f 2d66 696c 7465 7220 626f 7420 6163  to-filter bot ac
-00005d10: 7469 7669 7469 6573 2e20 4275 7420 6120  tivities. But a 
-00005d20: 776f 726b 2d61 726f 756e 6420 736f 6c75  work-around solu
-00005d30: 7469 6f6e 2069 7320 746f 2073 6c69 6768  tion is to sligh
-00005d40: 746c 7920 6d6f 6469 6679 2074 6865 2053  tly modify the S
-00005d50: 514c 2071 7565 7279 2069 6e20 4772 6166  QL query in Graf
-00005d60: 616e 6120 6461 7368 626f 6172 6473 2074  ana dashboards t
-00005d70: 6f20 6669 6c74 6572 2069 7373 7565 732f  o filter issues/
-00005d80: 5052 7320 6279 2074 6865 6972 2061 7574  PRs by their aut
-00005d90: 686f 7273 2e22 2c0d 0a20 2020 2020 2020  hors.",..       
-00005da0: 2020 2020 2022 616e 7377 6572 5f70 726f       "answer_pro
-00005db0: 7065 7274 6965 7322 3a20 5b5d 2c0d 0a20  perties": [],.. 
-00005dc0: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
-00005dd0: 7322 3a20 7b0d 0a20 2020 2020 2020 2020  s": {..         
-00005de0: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
-00005df0: 226d 6964 220d 0a20 2020 2020 2020 2020  "mid"..         
-00005e00: 2020 207d 0d0a 2020 2020 2020 2020 7d2c     }..        },
-00005e10: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00005e20: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-00005e30: 6465 766c 616b 652d 3334 222c 0d0a 2020  devlake-34",..  
-00005e40: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
-00005e50: 696f 6e22 3a20 2248 6f77 2064 6f20 4920  ion": "How do I 
-00005e60: 6c6f 6769 6e20 746f 2047 7261 6661 6e61  login to Grafana
-00005e70: 2074 6f20 6163 6365 7373 2074 6865 2064   to access the d
-00005e80: 6173 6862 6f61 7264 7322 2c0d 0a20 2020  ashboards",..   
-00005e90: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-00005ea0: 6e63 655f 616e 7377 6572 223a 2022 4279  nce_answer": "By
-00005eb0: 2064 6566 6175 6c74 2074 6865 2075 7365   default the use
-00005ec0: 7220 616e 6420 7061 7373 776f 7264 2061  r and password a
-00005ed0: 7265 2073 6574 2074 6f20 6164 6d69 6e2e  re set to admin.
-00005ee0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005ef0: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
-00005f00: 6573 223a 205b 5d2c 0d0a 2020 2020 2020  es": [],..      
-00005f10: 2020 2020 2020 226e 6f74 6573 223a 207b        "notes": {
-00005f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005f30: 2020 226c 6576 656c 223a 2022 6c6f 7722    "level": "low"
-00005f40: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-00005f50: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00005f60: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00005f70: 2020 2020 2269 6422 3a20 2264 6576 6c61      "id": "devla
-00005f80: 6b65 2d33 3522 2c0d 0a20 2020 2020 2020  ke-35",..       
-00005f90: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
-00005fa0: 2022 4973 2069 7420 706f 7373 6962 6c65   "Is it possible
-00005fb0: 2074 6f20 6d6f 6469 6679 2061 2062 6c75   to modify a blu
-00005fc0: 6570 7269 6e74 2077 6974 6820 616e 2061  eprint with an a
-00005fd0: 6464 6974 696f 6e61 6c20 696e 7465 6772  dditional integr
-00005fe0: 6174 696f 6e20 6166 7465 7220 6974 7320  ation after its 
-00005ff0: 6265 656e 2063 7265 6174 6564 3f22 2c0d  been created?",.
-00006000: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00006010: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
-00006020: 2022 5965 732c 2066 726f 6d20 7630 2e31   "Yes, from v0.1
-00006030: 3720 796f 7520 6361 6e20 6164 6420 6d6f  7 you can add mo
-00006040: 7265 2064 6174 6120 636f 6e6e 6563 7469  re data connecti
-00006050: 6f6e 7320 746f 2061 6e20 6578 6973 7469  ons to an existi
-00006060: 6e67 2062 6c75 6570 7269 6e74 222c 0d0a  ng blueprint",..
-00006070: 2020 2020 2020 2020 2020 2020 2261 6e73              "ans
-00006080: 7765 725f 7072 6f70 6572 7469 6573 223a  wer_properties":
-00006090: 205b 5d2c 0d0a 2020 2020 2020 2020 2020   [],..          
-000060a0: 2020 226e 6f74 6573 223a 207b 0d0a 2020    "notes": {..  
-000060b0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-000060c0: 6576 656c 223a 2022 6c6f 7722 0d0a 2020  evel": "low"..  
-000060d0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-000060e0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-000060f0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00006100: 2269 6422 3a20 2264 6576 6c61 6b65 2d33  "id": "devlake-3
-00006110: 3622 2c0d 0a20 2020 2020 2020 2020 2020  6",..           
-00006120: 2022 7175 6573 7469 6f6e 223a 2022 5768   "question": "Wh
-00006130: 656e 2073 686f 756c 6420 4920 7573 6520  en should I use 
-00006140: 6164 7661 6e63 6564 206d 6f64 6520 666f  advanced mode fo
-00006150: 7220 6120 626c 7565 7072 696e 743f 222c  r a blueprint?",
-00006160: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00006170: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-00006180: 3a20 2241 6476 616e 6365 6420 6d6f 6465  : "Advanced mode
-00006190: 2061 6c6c 6f77 7320 7573 6572 7320 746f   allows users to
-000061a0: 2063 7265 6174 6520 616e 7920 7069 7065   create any pipe
-000061b0: 6c69 6e65 2062 7920 7772 6974 696e 6720  line by writing 
-000061c0: 4a53 4f4e 2e20 5468 6973 2069 7320 7573  JSON. This is us
-000061d0: 6566 756c 2066 6f72 2075 7365 7273 2077  eful for users w
-000061e0: 686f 2077 616e 7420 746f 2063 6f6c 6c65  ho want to colle
-000061f0: 6374 206d 756c 7469 706c 6520 4769 7448  ct multiple GitH
-00006200: 7562 2f47 6974 4c61 6220 7265 706f 7320  ub/GitLab repos 
-00006210: 6f72 204a 6972 6120 7072 6f6a 6563 7473  or Jira projects
-00006220: 2077 6974 6869 6e20 6120 7369 6e67 6c65   within a single
-00006230: 2070 6970 656c 696e 652c 2068 6176 6520   pipeline, have 
-00006240: 6669 6e65 2d67 7261 696e 6564 2063 6f6e  fine-grained con
-00006250: 7472 6f6c 206f 7665 7220 7768 6174 2065  trol over what e
-00006260: 6e74 6974 6965 7320 746f 2063 6f6c 6c65  ntities to colle
-00006270: 6374 206f 7220 7768 6174 2073 7562 7461  ct or what subta
-00006280: 736b 7320 746f 2072 756e 2066 6f72 2065  sks to run for e
-00006290: 6163 6820 706c 7567 696e 2c20 616e 6420  ach plugin, and 
-000062a0: 6f72 6368 6573 7472 6174 6520 6120 636f  orchestrate a co
-000062b0: 6d70 6c65 7820 7069 7065 6c69 6e65 2074  mplex pipeline t
-000062c0: 6861 7420 636f 6e73 6973 7473 206f 6620  hat consists of 
-000062d0: 6d75 6c74 6970 6c65 2073 7461 6765 7320  multiple stages 
-000062e0: 6f66 2070 6c75 6769 6e73 2e20 596f 7520  of plugins. You 
-000062f0: 6361 6e20 7265 6665 7220 746f 206f 7572  can refer to our
-00006300: 2064 6f63 2066 6f72 206d 6f72 6520 6465   doc for more de
-00006310: 7461 696c 733a 2068 7474 7073 3a2f 2f64  tails: https://d
-00006320: 6576 6c61 6b65 2e61 7061 6368 652e 6f72  evlake.apache.or
-00006330: 672f 646f 6373 2f43 6f6e 6669 6775 7261  g/docs/Configura
-00006340: 7469 6f6e 2f41 6476 616e 6365 644d 6f64  tion/AdvancedMod
-00006350: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-00006360: 2022 616e 7377 6572 5f70 726f 7065 7274   "answer_propert
-00006370: 6965 7322 3a20 5b5d 2c0d 0a20 2020 2020  ies": [],..     
-00006380: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
-00006390: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000063a0: 2020 2022 6c65 7665 6c22 3a20 226c 6f77     "level": "low
-000063b0: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
-000063c0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-000063d0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-000063e0: 2020 2020 2022 6964 223a 2022 6465 766c       "id": "devl
-000063f0: 616b 652d 3337 222c 0d0a 2020 2020 2020  ake-37",..      
-00006400: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00006410: 3a20 2248 6f77 2064 6f20 4920 636f 6e66  : "How do I conf
-00006420: 6967 7572 6520 536f 6e61 7251 7562 653f  igure SonarQube?
-00006430: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00006440: 2272 6566 6572 656e 6365 5f61 6e73 7765  "reference_answe
-00006450: 7222 3a20 2250 6c65 6173 6520 666f 6c6c  r": "Please foll
-00006460: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
-00006470: 6f6e 2069 6e20 7468 6973 2064 6f63 3a20  on in this doc: 
-00006480: 6874 7470 733a 2f2f 6465 766c 616b 652e  https://devlake.
-00006490: 6170 6163 6865 2e6f 7267 2f64 6f63 732f  apache.org/docs/
-000064a0: 6e65 7874 2f43 6f6e 6669 6775 7261 7469  next/Configurati
-000064b0: 6f6e 2f53 6f6e 6172 5175 6265 222c 0d0a  on/SonarQube",..
-000064c0: 2020 2020 2020 2020 2020 2020 2261 6e73              "ans
-000064d0: 7765 725f 7072 6f70 6572 7469 6573 223a  wer_properties":
-000064e0: 205b 5d2c 0d0a 2020 2020 2020 2020 2020   [],..          
-000064f0: 2020 226e 6f74 6573 223a 207b 0d0a 2020    "notes": {..  
-00006500: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00006510: 6576 656c 223a 2022 6c6f 7722 0d0a 2020  evel": "low"..  
-00006520: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00006530: 2020 2020 207d 0d0a 2020 2020 5d0d 0a7d       }..    ]..}
-00006540: 0d0a                                     ..
+00002ae0: 7365 7474 696e 6720 7468 726f 7567 6820  setting through 
+00002af0: 7468 6520 666f 6c6c 6f77 696e 6720 7374  the following st
+00002b00: 6570 733a 5c6e 5c6e 312e 2054 6865 2062  eps:\n\n1. The b
+00002b10: 6c75 6570 7269 6e74 2073 6574 7469 6e67  lueprint setting
+00002b20: 7320 6172 6520 6465 6669 6e65 6420 696e  s are defined in
+00002b30: 2061 204a 534f 4e20 666f 726d 6174 2c20   a JSON format, 
+00002b40: 7768 6963 6820 696e 636c 7564 6573 2074  which includes t
+00002b50: 6865 2076 6572 7369 6f6e 2c20 636f 6e6e  he version, conn
+00002b60: 6563 7469 6f6e 732c 2070 6c75 6769 6e2c  ections, plugin,
+00002b70: 2063 6f6e 6e65 6374 696f 6e49 642c 2061   connectionId, a
+00002b80: 6e64 2073 636f 7065 732e 5c6e 5c6e 322e  nd scopes.\n\n2.
+00002b90: 2054 6865 2060 506c 7567 696e 426c 7565   The `PluginBlue
+00002ba0: 7072 696e 7456 3230 302e 4d61 6b65 5069  printV200.MakePi
+00002bb0: 7065 6c69 6e65 506c 616e 6020 6675 6e63  pelinePlan` func
+00002bc0: 7469 6f6e 2069 7320 6361 6c6c 6564 2077  tion is called w
+00002bd0: 6974 6820 616e 2061 7272 6179 206f 6620  ith an array of 
+00002be0: 7363 6f70 6573 2e20 5468 6520 706c 7567  scopes. The plug
+00002bf0: 696e 2072 6574 7572 6e73 2061 2060 5069  in returns a `Pi
+00002c00: 7065 6c69 6e65 506c 616e 6020 696e 204a  pelinePlan` in J
+00002c10: 534f 4e20 666f 726d 6174 2061 6e64 2061  SON format and a
+00002c20: 6e20 6172 7261 7920 6f66 2060 5363 6f70  n array of `Scop
+00002c30: 6560 2066 6f72 2070 726f 6a65 6374 5f6d  e` for project_m
+00002c40: 6170 7069 6e67 2e5c 6e5c 6e33 2e20 5468  apping.\n\n3. Th
+00002c50: 6520 6672 616d 6577 6f72 6b20 6d61 696e  e framework main
+00002c60: 7461 696e 7320 7468 6520 7072 6f6a 6563  tains the projec
+00002c70: 745f 6d61 7070 696e 6720 7461 626c 6520  t_mapping table 
+00002c80: 6261 7365 6420 6f6e 2074 6865 2060 5b5d  based on the `[]
+00002c90: 5363 6f70 6560 2061 7272 6179 2e5c 6e5c  Scope` array.\n\
+00002ca0: 6e54 6865 7365 2073 7465 7073 2068 656c  nThese steps hel
+00002cb0: 7020 4465 764c 616b 6520 6765 6e65 7261  p DevLake genera
+00002cc0: 7465 2061 2070 6970 656c 696e 6520 706c  te a pipeline pl
+00002cd0: 616e 2062 6173 6564 206f 6e20 7468 6520  an based on the 
+00002ce0: 626c 7565 7072 696e 7427 7320 7365 7474  blueprint's sett
+00002cf0: 696e 6773 2c20 7768 6963 6820 6361 6e20  ings, which can 
+00002d00: 6265 2075 7365 6420 746f 2065 7865 6375  be used to execu
+00002d10: 7465 2074 6865 2070 6970 656c 696e 6520  te the pipeline 
+00002d20: 616e 6420 636f 6c6c 6563 7420 6461 7461  and collect data
+00002d30: 2066 726f 6d20 7661 7269 6f75 7320 736f   from various so
+00002d40: 7572 6365 732e 222c 0a20 2020 2020 2020  urces.",.       
+00002d50: 2020 2020 2022 616e 7377 6572 5f70 726f       "answer_pro
+00002d60: 7065 7274 6965 7322 3a20 5b5d 2c0a 2020  perties": [],.  
+00002d70: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
+00002d80: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00002d90: 2020 2020 2022 6c65 7665 6c22 3a20 226c       "level": "l
+00002da0: 6f77 220a 2020 2020 2020 2020 2020 2020  ow".            
+00002db0: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00002dc0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00002dd0: 2020 2022 6964 223a 2022 6465 766c 616b     "id": "devlak
+00002de0: 652d 3132 222c 0a20 2020 2020 2020 2020  e-12",.         
+00002df0: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
+00002e00: 486f 7720 646f 6573 2044 6576 4c61 6b65  How does DevLake
+00002e10: 2064 656c 6574 6520 6120 7072 6f6a 6563   delete a projec
+00002e20: 743f 222c 0a20 2020 2020 2020 2020 2020  t?",.           
+00002e30: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
+00002e40: 6572 223a 2022 4465 764c 616b 6520 6465  er": "DevLake de
+00002e50: 6c65 7465 7320 6120 7072 6f6a 6563 7420  letes a project 
+00002e60: 6279 2066 6f6c 6c6f 7769 6e67 2074 6865  by following the
+00002e70: 7365 2073 7465 7073 3a5c 6e5c 6e31 2e20  se steps:\n\n1. 
+00002e80: 5665 7269 6679 2074 6865 2069 6e70 7574  Verify the input
+00002e90: 2070 726f 6a65 6374 206e 616d 6520 6973   project name is
+00002ea0: 206e 6f74 2065 6d70 7479 2e5c 6e32 2e20   not empty.\n2. 
+00002eb0: 4265 6769 6e20 6120 6461 7461 6261 7365  Begin a database
+00002ec0: 2074 7261 6e73 6163 7469 6f6e 2e5c 6e33   transaction.\n3
+00002ed0: 2e20 4765 7420 7468 6520 7072 6f6a 6563  . Get the projec
+00002ee0: 7420 6279 2069 7473 206e 616d 6520 7573  t by its name us
+00002ef0: 696e 6720 7468 6520 6067 6574 5072 6f6a  ing the `getProj
+00002f00: 6563 7442 794e 616d 6560 2066 756e 6374  ectByName` funct
+00002f10: 696f 6e2e 5c6e 342e 2044 656c 6574 6520  ion.\n4. Delete 
+00002f20: 7468 6520 7072 6f6a 6563 7420 6672 6f6d  the project from
+00002f30: 2074 6865 2060 6d6f 6465 6c73 2e50 726f   the `models.Pro
+00002f40: 6a65 6374 6020 7461 626c 6520 7573 696e  ject` table usin
+00002f50: 6720 7468 6520 7072 6f6a 6563 7420 6e61  g the project na
+00002f60: 6d65 2e5c 6e35 2e20 4465 6c65 7465 2074  me.\n5. Delete t
+00002f70: 6865 2070 726f 6a65 6374 206d 6170 7069  he project mappi
+00002f80: 6e67 2066 726f 6d20 7468 6520 6063 726f  ng from the `cro
+00002f90: 7373 646f 6d61 696e 2e50 726f 6a65 6374  ssdomain.Project
+00002fa0: 4d61 7070 696e 6760 2074 6162 6c65 2075  Mapping` table u
+00002fb0: 7369 6e67 2074 6865 2070 726f 6a65 6374  sing the project
+00002fc0: 206e 616d 652e 5c6e 362e 2044 656c 6574   name.\n6. Delet
+00002fd0: 6520 7468 6520 7072 6f6a 6563 7420 6d65  e the project me
+00002fe0: 7472 6963 2073 6574 7469 6e67 2066 726f  tric setting fro
+00002ff0: 6d20 7468 6520 606d 6f64 656c 732e 5072  m the `models.Pr
+00003000: 6f6a 6563 744d 6574 7269 6353 6574 7469  ojectMetricSetti
+00003010: 6e67 6020 7461 626c 6520 7573 696e 6720  ng` table using 
+00003020: 7468 6520 7072 6f6a 6563 7420 6e61 6d65  the project name
+00003030: 2e5c 6e37 2e20 4465 6c65 7465 2074 6865  .\n7. Delete the
+00003040: 2070 726f 6a65 6374 2050 5220 6d65 7472   project PR metr
+00003050: 6963 2066 726f 6d20 7468 6520 6063 726f  ic from the `cro
+00003060: 7373 646f 6d61 696e 2e50 726f 6a65 6374  ssdomain.Project
+00003070: 5072 4d65 7472 6963 6020 7461 626c 6520  PrMetric` table 
+00003080: 7573 696e 6720 7468 6520 7072 6f6a 6563  using the projec
+00003090: 7420 6e61 6d65 2e5c 6e38 2e20 4465 6c65  t name.\n8. Dele
+000030a0: 7465 2074 6865 2070 726f 6a65 6374 2069  te the project i
+000030b0: 7373 7565 206d 6574 7269 6320 6672 6f6d  ssue metric from
+000030c0: 2074 6865 2060 6372 6f73 7364 6f6d 6169   the `crossdomai
+000030d0: 6e2e 5072 6f6a 6563 7449 7373 7565 4d65  n.ProjectIssueMe
+000030e0: 7472 6963 6020 7461 626c 6520 7573 696e  tric` table usin
+000030f0: 6720 7468 6520 7072 6f6a 6563 7420 6e61  g the project na
+00003100: 6d65 2e5c 6e39 2e20 436f 6d6d 6974 2074  me.\n9. Commit t
+00003110: 6865 2074 7261 6e73 6163 7469 6f6e 2e5c  he transaction.\
+00003120: 6e31 302e 2047 6574 2074 6865 2062 6c75  n10. Get the blu
+00003130: 6570 7269 6e74 2061 7373 6f63 6961 7465  eprint associate
+00003140: 6420 7769 7468 2074 6865 2070 726f 6a65  d with the proje
+00003150: 6374 206e 616d 6520 7573 696e 6720 7468  ct name using th
+00003160: 6520 6062 704d 616e 6167 6572 2e47 6574  e `bpManager.Get
+00003170: 4462 426c 7565 7072 696e 7442 7950 726f  DbBlueprintByPro
+00003180: 6a65 6374 4e61 6d65 6020 6675 6e63 7469  jectName` functi
+00003190: 6f6e 2e5c 6e31 312e 2044 656c 6574 6520  on.\n11. Delete 
+000031a0: 7468 6520 626c 7565 7072 696e 7420 7573  the blueprint us
+000031b0: 696e 6720 7468 6520 6062 704d 616e 6167  ing the `bpManag
+000031c0: 6572 2e44 656c 6574 6542 6c75 6570 7269  er.DeleteBluepri
+000031d0: 6e74 6020 6675 6e63 7469 6f6e 2077 6974  nt` function wit
+000031e0: 6820 7468 6520 626c 7565 7072 696e 7420  h the blueprint 
+000031f0: 4944 2e22 2c0a 2020 2020 2020 2020 2020  ID.",.          
+00003200: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
+00003210: 7469 6573 223a 205b 5d2c 0a20 2020 2020  ties": [],.     
+00003220: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
+00003230: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003240: 2020 226c 6576 656c 223a 2022 6869 6768    "level": "high
+00003250: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+00003260: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00003270: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00003280: 2022 6964 223a 2022 6465 766c 616b 652d   "id": "devlake-
+00003290: 3133 222c 0a20 2020 2020 2020 2020 2020  13",.           
+000032a0: 2022 7175 6573 7469 6f6e 223a 2022 486f   "question": "Ho
+000032b0: 7720 646f 6573 2044 6576 4c61 6b65 2067  w does DevLake g
+000032c0: 656e 6572 6174 6520 7468 6520 7465 6d70  enerate the temp
+000032d0: 6c61 7465 2060 7573 6572 5f61 6363 6f75  late `user_accou
+000032e0: 6e74 5f6d 6170 7069 6e67 2e63 7376 6020  nt_mapping.csv` 
+000032f0: 6669 6c65 3f22 2c0a 2020 2020 2020 2020  file?",.        
+00003300: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
+00003310: 6e73 7765 7222 3a20 2244 6576 4c61 6b65  nswer": "DevLake
+00003320: 2067 656e 6572 6174 6573 2074 6865 2074   generates the t
+00003330: 656d 706c 6174 6520 7573 6572 5f61 6363  emplate user_acc
+00003340: 6f75 6e74 5f6d 6170 7069 6e67 2e63 7376  ount_mapping.csv
+00003350: 2066 696c 6520 7573 696e 6720 7468 6520   file using the 
+00003360: 4765 7455 7365 7241 6363 6f75 6e74 4d61  GetUserAccountMa
+00003370: 7070 696e 6720 6675 6e63 7469 6f6e 2e20  pping function. 
+00003380: 5468 6973 2066 756e 6374 696f 6e20 7265  This function re
+00003390: 7472 6965 7665 7320 616c 6c20 7573 6572  trieves all user
+000033a0: 2f61 6363 6f75 6e74 206d 6170 7069 6e67  /account mapping
+000033b0: 7320 6672 6f6d 2074 6865 2073 746f 7265  s from the store
+000033c0: 2c20 6d61 7273 6861 6c73 2074 6865 6d20  , marshals them 
+000033d0: 696e 746f 2043 5356 2066 6f72 6d61 7420  into CSV format 
+000033e0: 7573 696e 6720 676f 6373 762e 4d61 7273  using gocsv.Mars
+000033f0: 6861 6c42 7974 6573 2861 6363 6f75 6e74  halBytes(account
+00003400: 7329 2c20 616e 6420 7265 7475 726e 7320  s), and returns 
+00003410: 7468 6520 4353 5620 6461 7461 2061 7320  the CSV data as 
+00003420: 616e 204f 7574 7075 7446 696c 6520 7769  an OutputFile wi
+00003430: 7468 2043 6f6e 7465 6e74 5479 7065 205c  th ContentType \
+00003440: 2274 6578 742f 6373 765c 222e 222c 0a20  "text/csv\".",. 
+00003450: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
+00003460: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
+00003470: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+00003480: 226e 6f74 6573 223a 207b 0a20 2020 2020  "notes": {.     
+00003490: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
+000034a0: 6c22 3a20 2268 6967 6822 0a20 2020 2020  l": "high".     
+000034b0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000034c0: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+000034d0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+000034e0: 2264 6576 6c61 6b65 2d31 3422 2c0a 2020  "devlake-14",.  
+000034f0: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
+00003500: 696f 6e22 3a20 2248 6f77 2069 7320 7468  ion": "How is th
+00003510: 6520 6066 696e 6441 6c6c 4163 636f 756e  e `findAllAccoun
+00003520: 7473 6020 6675 6e63 7469 6f6e 2069 6d70  ts` function imp
+00003530: 6c65 6d65 6e74 6564 3f22 2c0a 2020 2020  lemented?",.    
+00003540: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
+00003550: 6365 5f61 6e73 7765 7222 3a20 2222 2c0a  ce_answer": "",.
+00003560: 2020 2020 2020 2020 2020 2020 2261 6e73              "ans
+00003570: 7765 725f 7072 6f70 6572 7469 6573 223a  wer_properties":
+00003580: 205b 5d2c 0a20 2020 2020 2020 2020 2020   [],.           
+00003590: 2022 6e6f 7465 7322 3a20 7b0a 2020 2020   "notes": {.    
+000035a0: 2020 2020 2020 2020 2020 2020 226c 6576              "lev
+000035b0: 656c 223a 2022 6c6f 7722 0a20 2020 2020  el": "low".     
+000035c0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+000035d0: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+000035e0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+000035f0: 2264 6576 6c61 6b65 2d31 3522 2c0a 2020  "devlake-15",.  
+00003600: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
+00003610: 696f 6e22 3a20 2248 6f77 2069 7320 7468  ion": "How is th
+00003620: 6520 6068 2e73 746f 7265 2e66 696e 6441  e `h.store.findA
+00003630: 6c6c 4163 636f 756e 7473 6020 6675 6e63  llAccounts` func
+00003640: 7469 6f6e 2069 6d70 6c65 6d65 6e74 6564  tion implemented
+00003650: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
+00003660: 2272 6566 6572 656e 6365 5f61 6e73 7765  "reference_answe
+00003670: 7222 3a20 2254 6865 2068 2e73 746f 7265  r": "The h.store
+00003680: 2e66 696e 6441 6c6c 4163 636f 756e 7473  .findAllAccounts
+00003690: 2066 756e 6374 696f 6e20 6973 2069 6d70   function is imp
+000036a0: 6c65 6d65 6e74 6564 2061 7320 666f 6c6c  lemented as foll
+000036b0: 6f77 733a 5c6e 5c6e 6060 6067 6f5c 6e66  ows:\n\n```go\nf
+000036c0: 756e 6320 2864 202a 6462 5374 6f72 6529  unc (d *dbStore)
+000036d0: 2066 696e 6441 6c6c 4163 636f 756e 7473   findAllAccounts
+000036e0: 2829 2028 5b5d 6163 636f 756e 742c 2065  () ([]account, e
+000036f0: 7272 6f72 732e 4572 726f 7229 207b 5c6e  rrors.Error) {\n
+00003700: 5c74 7661 7220 6161 205b 5d63 726f 7373  \tvar aa []cross
+00003710: 646f 6d61 696e 2e41 6363 6f75 6e74 5c6e  domain.Account\n
+00003720: 5c74 6572 7220 3a3d 2064 2e64 622e 416c  \terr := d.db.Al
+00003730: 6c28 2661 6129 5c6e 5c74 6966 2065 7272  l(&aa)\n\tif err
+00003740: 2021 3d20 6e69 6c20 7b5c 6e5c 745c 7472   != nil {\n\t\tr
+00003750: 6574 7572 6e20 6e69 6c2c 2065 7272 5c6e  eturn nil, err\n
+00003760: 5c74 7d5c 6e5c 7476 6172 2075 6120 5b5d  \t}\n\tvar ua []
+00003770: 6372 6f73 7364 6f6d 6169 6e2e 5573 6572  crossdomain.User
+00003780: 4163 636f 756e 745c 6e5c 7465 7272 203d  Account\n\terr =
+00003790: 2064 2e64 622e 416c 6c28 2675 6129 5c6e   d.db.All(&ua)\n
+000037a0: 5c74 6966 2065 7272 2021 3d20 6e69 6c20  \tif err != nil 
+000037b0: 7b5c 6e5c 745c 7472 6574 7572 6e20 6e69  {\n\t\treturn ni
+000037c0: 6c2c 2065 7272 5c6e 5c74 7d5c 6e5c 7476  l, err\n\t}\n\tv
+000037d0: 6172 2061 202a 6163 636f 756e 745c 6e5c  ar a *account\n\
+000037e0: 7472 6574 7572 6e20 612e 6672 6f6d 446f  treturn a.fromDo
+000037f0: 6d61 696e 4c61 7965 7228 6161 2c20 7561  mainLayer(aa, ua
+00003800: 292c 206e 696c 5c6e 7d5c 6e60 6060 5c6e  ), nil\n}\n```\n
+00003810: 5c6e 4974 2072 6574 7269 6576 6573 2061  \nIt retrieves a
+00003820: 6c6c 2061 6363 6f75 6e74 7320 616e 6420  ll accounts and 
+00003830: 7573 6572 2061 6363 6f75 6e74 7320 6672  user accounts fr
+00003840: 6f6d 2074 6865 2064 6174 6162 6173 652c  om the database,
+00003850: 2061 6e64 2074 6865 6e20 6361 6c6c 7320   and then calls 
+00003860: 7468 6520 6672 6f6d 446f 6d61 696e 4c61  the fromDomainLa
+00003870: 7965 7220 6675 6e63 7469 6f6e 2074 6f20  yer function to 
+00003880: 636f 6e76 6572 7420 7468 656d 2069 6e74  convert them int
+00003890: 6f20 7468 6520 6170 7072 6f70 7269 6174  o the appropriat
+000038a0: 6520 666f 726d 6174 2e22 2c0a 2020 2020  e format.",.    
+000038b0: 2020 2020 2020 2020 2261 6e73 7765 725f          "answer_
+000038c0: 7072 6f70 6572 7469 6573 223a 205b 5d2c  properties": [],
+000038d0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+000038e0: 7465 7322 3a20 7b0a 2020 2020 2020 2020  tes": {.        
+000038f0: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
+00003900: 2022 6c6f 7722 0a20 2020 2020 2020 2020   "low".         
+00003910: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+00003920: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00003930: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
+00003940: 6c61 6b65 2d31 3622 2c0a 2020 2020 2020  lake-16",.      
+00003950: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+00003960: 3a20 2248 6f77 2069 7320 7468 6520 6066  : "How is the `f
+00003970: 726f 6d44 6f6d 6169 6e4c 6179 6572 6020  romDomainLayer` 
+00003980: 6d65 7468 6f64 206f 6620 7468 6520 6163  method of the ac
+00003990: 636f 756e 7420 7479 7065 2069 6d70 6c65  count type imple
+000039a0: 6d65 6e74 6564 3f22 2c0a 2020 2020 2020  mented?",.      
+000039b0: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
+000039c0: 5f61 6e73 7765 7222 3a20 2222 2c0a 2020  _answer": "",.  
+000039d0: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
+000039e0: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
+000039f0: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00003a00: 6e6f 7465 7322 3a20 7b0a 2020 2020 2020  notes": {.      
+00003a10: 2020 2020 2020 2020 2020 226c 6576 656c            "level
+00003a20: 223a 2022 6c6f 7722 0a20 2020 2020 2020  ": "low".       
+00003a30: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00003a40: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00003a50: 2020 2020 2020 2020 2269 6422 3a20 2264          "id": "d
+00003a60: 6576 6c61 6b65 2d31 3722 2c0a 2020 2020  evlake-17",.    
+00003a70: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00003a80: 6e22 3a20 2249 7320 7468 6520 696e 666f  n": "Is the info
+00003a90: 726d 6174 696f 6e20 636f 6c6c 6563 7465  rmation collecte
+00003aa0: 6420 6672 6f6d 2061 6c6c 2062 7261 6e63  d from all branc
+00003ab0: 6865 7320 6672 6f6d 2067 6974 3f22 2c0a  hes from git?",.
+00003ac0: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
+00003ad0: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
+00003ae0: 2254 6865 2067 6974 2065 7874 7261 6374  "The git extract
+00003af0: 6f72 2070 6c75 6769 6e20 636f 6c6c 6563  or plugin collec
+00003b00: 7473 2063 6f6d 6d69 7473 206f 6e20 616c  ts commits on al
+00003b10: 6c20 6272 616e 6368 6573 2e22 2c0a 2020  l branches.",.  
+00003b20: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
+00003b30: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
+00003b40: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00003b50: 6e6f 7465 7322 3a20 7b0a 2020 2020 2020  notes": {.      
+00003b60: 2020 2020 2020 2020 2020 226c 6576 656c            "level
+00003b70: 223a 2022 6c6f 7722 0a20 2020 2020 2020  ": "low".       
+00003b80: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00003b90: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00003ba0: 2020 2020 2020 2020 2269 6422 3a20 2264          "id": "d
+00003bb0: 6576 6c61 6b65 2d31 3822 2c0a 2020 2020  evlake-18",.    
+00003bc0: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00003bd0: 6e22 3a20 2244 6f65 7320 4465 764c 616b  n": "Does DevLak
+00003be0: 6520 7375 7070 6f72 7420 506f 7374 6772  e support Postgr
+00003bf0: 6553 514c 3f22 2c0a 2020 2020 2020 2020  eSQL?",.        
+00003c00: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
+00003c10: 6e73 7765 7222 3a20 2259 6573 2c20 506f  nswer": "Yes, Po
+00003c20: 7374 6772 6553 514c 2069 7320 7375 7070  stgreSQL is supp
+00003c30: 6f72 7465 6420 666f 7220 616c 6c20 7665  orted for all ve
+00003c40: 7273 696f 6e73 2066 726f 6d20 7630 2e31  rsions from v0.1
+00003c50: 3120 7570 2c20 6275 7420 7468 6520 7072  1 up, but the pr
+00003c60: 652d 6275 696c 7420 4772 6166 616e 6120  e-built Grafana 
+00003c70: 6461 7368 626f 6172 6473 206f 6e6c 7920  dashboards only 
+00003c80: 7375 7070 6f72 7420 4d79 5351 4c2e 2050  support MySQL. P
+00003c90: 6f73 7467 7265 5351 4c20 7375 7070 6f72  ostgreSQL suppor
+00003ca0: 7420 6973 206e 6f74 2062 6569 6e67 2072  t is not being r
+00003cb0: 656d 6f76 6564 2065 6e74 6972 656c 792c  emoved entirely,
+00003cc0: 2062 7574 2074 6865 2072 656c 6174 6564   but the related
+00003cd0: 2069 6e66 6f72 6d61 7469 6f6e 2068 6173   information has
+00003ce0: 2062 6565 6e20 7465 6d70 6f72 6172 696c   been temporaril
+00003cf0: 7920 7265 6d6f 7665 6420 6475 6520 746f  y removed due to
+00003d00: 2074 6865 2070 6172 7469 616c 2063 6f6d   the partial com
+00003d10: 7061 7469 6269 6c69 7479 2077 6974 6820  patibility with 
+00003d20: 4772 6166 616e 6120 6461 7368 626f 6172  Grafana dashboar
+00003d30: 6473 2e20 5573 6572 7320 7768 6f20 7761  ds. Users who wa
+00003d40: 6e74 2074 6f20 7573 6520 506f 7374 6772  nt to use Postgr
+00003d50: 6553 514c 2077 6974 6820 4465 764c 616b  eSQL with DevLak
+00003d60: 6520 6361 6e20 7374 696c 6c20 646f 2073  e can still do s
+00003d70: 6f2c 2062 7574 2074 6865 7920 6d61 7920  o, but they may 
+00003d80: 6e65 6564 2074 6f20 636f 6e76 6572 7420  need to convert 
+00003d90: 7468 6520 4d79 5351 4c20 7175 6572 6965  the MySQL querie
+00003da0: 7320 7072 6f76 6964 6564 2062 7920 4465  s provided by De
+00003db0: 764c 616b 6520 746f 2050 6f73 7467 7265  vLake to Postgre
+00003dc0: 5351 4c2e 222c 0a20 2020 2020 2020 2020  SQL.",.         
+00003dd0: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
+00003de0: 7274 6965 7322 3a20 5b5d 2c0a 2020 2020  rties": [],.    
+00003df0: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
+00003e00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003e10: 2020 2022 6c65 7665 6c22 3a20 226c 6f77     "level": "low
+00003e20: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+00003e30: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00003e40: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00003e50: 2022 6964 223a 2022 6465 766c 616b 652d   "id": "devlake-
+00003e60: 3139 222c 0a20 2020 2020 2020 2020 2020  19",.           
+00003e70: 2022 7175 6573 7469 6f6e 223a 2022 5768   "question": "Wh
+00003e80: 7920 6973 2069 7420 7468 6174 206e 6f74  y is it that not
+00003e90: 2061 6c6c 206f 7267 616e 6973 6174 696f   all organisatio
+00003ea0: 6e73 2069 6e20 6d79 2047 6974 6875 6220  ns in my Github 
+00003eb0: 6172 6520 6265 696e 6720 7368 6f77 6e3f  are being shown?
+00003ec0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00003ed0: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
+00003ee0: 223a 2022 4966 2079 6f75 2772 6520 6e6f  ": "If you're no
+00003ef0: 7420 7365 6569 6e67 2061 6c6c 206f 6620  t seeing all of 
+00003f00: 796f 7572 2047 6974 4875 6220 6f72 6773  your GitHub orgs
+00003f10: 2c20 706c 6561 7365 2063 6865 636b 2069  , please check i
+00003f20: 6620 796f 7572 2047 6974 4875 6220 6f72  f your GitHub or
+00003f30: 6720 6861 7320 616c 6c6f 7765 6420 5041  g has allowed PA
+00003f40: 5420 6163 6365 7373 2e22 2c0a 2020 2020  T access.",.    
+00003f50: 2020 2020 2020 2020 2261 6e73 7765 725f          "answer_
+00003f60: 7072 6f70 6572 7469 6573 223a 205b 5d2c  properties": [],
+00003f70: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+00003f80: 7465 7322 3a20 7b0a 2020 2020 2020 2020  tes": {.        
+00003f90: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
+00003fa0: 2022 6d69 6422 0a20 2020 2020 2020 2020   "mid".         
+00003fb0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+00003fc0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00003fd0: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
+00003fe0: 6c61 6b65 2d32 3022 2c0a 2020 2020 2020  lake-20",.      
+00003ff0: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+00004000: 3a20 2249 7320 6974 2070 6f73 7369 626c  : "Is it possibl
+00004010: 6520 746f 2063 6f6e 7375 6d65 2065 7665  e to consume eve
+00004020: 6e74 732f 6461 7461 2066 726f 6d20 6120  nts/data from a 
+00004030: 7374 7265 616d 2069 6e73 7465 6164 206f  stream instead o
+00004040: 6620 7075 6c6c 696e 6720 616e 2041 5049  f pulling an API
+00004050: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
+00004060: 2272 6566 6572 656e 6365 5f61 6e73 7765  "reference_answe
+00004070: 7222 3a20 2244 6576 4c61 6b65 2064 6f65  r": "DevLake doe
+00004080: 736e e280 9974 2068 6176 6520 6675 6c6c  sn...t have full
+00004090: 2d62 6c6f 776e 2073 7570 706f 7274 2066  -blown support f
+000040a0: 6f72 2063 6f6e 7375 6d69 6e67 2065 7665  or consuming eve
+000040b0: 6e74 732f 6461 7461 2066 726f 6d20 6120  nts/data from a 
+000040c0: 7374 7265 616d 2061 7320 6f66 2072 6967  stream as of rig
+000040d0: 6874 206e 6f77 2e20 4275 7420 7468 6572  ht now. But ther
+000040e0: 6527 7320 616e 2069 6e63 6f6d 696e 6720  e's an incoming 
+000040f0: 7765 6268 6f6f 6b20 6665 6174 7572 6520  webhook feature 
+00004100: 666f 7220 7265 6769 7374 6572 696e 6720  for registering 
+00004110: 6465 706c 6f79 6d65 6e74 7320 7769 7468  deployments with
+00004120: 2044 6576 4c61 6b65 2e22 2c0a 2020 2020   DevLake.",.    
+00004130: 2020 2020 2020 2020 2261 6e73 7765 725f          "answer_
+00004140: 7072 6f70 6572 7469 6573 223a 205b 5d2c  properties": [],
+00004150: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+00004160: 7465 7322 3a20 7b0a 2020 2020 2020 2020  tes": {.        
+00004170: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
+00004180: 2022 6c6f 7722 0a20 2020 2020 2020 2020   "low".         
+00004190: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+000041a0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000041b0: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
+000041c0: 6c61 6b65 2d32 3122 2c0a 2020 2020 2020  lake-21",.      
+000041d0: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+000041e0: 3a20 2249 7320 4465 766c 616b 6520 6d6f  : "Is Devlake mo
+000041f0: 7669 6e67 2074 6f20 5079 7468 6f6e 2062  ving to Python b
+00004200: 6173 6564 2070 6c75 6769 6e20 7261 7468  ased plugin rath
+00004210: 6572 2074 6861 6e20 476f 4c61 6e67 3f22  er than GoLang?"
+00004220: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+00004230: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
+00004240: 3a20 2244 6576 4c61 6b65 2077 696c 6c20  : "DevLake will 
+00004250: 7375 7070 6f72 7420 626f 7468 2047 6f6c  support both Gol
+00004260: 616e 6720 616e 6420 5079 7468 6f6e 2070  ang and Python p
+00004270: 6c75 6769 6e20 666f 7220 7468 6520 666f  lugin for the fo
+00004280: 7265 7365 6561 626c 6520 6675 7475 7265  reseeable future
+00004290: 2c20 6275 7420 7765 2772 6520 696e 6465  , but we're inde
+000042a0: 6564 2065 6e63 6f75 7261 6769 6e67 2075  ed encouraging u
+000042b0: 7365 7273 2074 6f20 7472 7920 6f75 7420  sers to try out 
+000042c0: 7468 6520 6e65 7720 7079 7468 6f6e 2053  the new python S
+000042d0: 444b 2c20 7768 6963 6820 6973 206f 7572  DK, which is our
+000042e0: 2061 7474 656d 7074 2074 6f20 696d 7072   attempt to impr
+000042f0: 6f76 6520 6465 7665 6c6f 7065 7220 6578  ove developer ex
+00004300: 7065 7269 656e 6365 2066 6f72 2070 6c75  perience for plu
+00004310: 6769 6e20 6465 7665 6c6f 706d 656e 742e  gin development.
+00004320: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00004330: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
+00004340: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+00004350: 2020 2020 226e 6f74 6573 223a 207b 0a20      "notes": {. 
+00004360: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004370: 6c65 7665 6c22 3a20 226d 6964 220a 2020  level": "mid".  
+00004380: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00004390: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+000043a0: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
+000043b0: 223a 2022 6465 766c 616b 652d 3232 222c  ": "devlake-22",
+000043c0: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
+000043d0: 6573 7469 6f6e 223a 2022 4920 646f 206e  estion": "I do n
+000043e0: 6f74 2073 6565 2061 6e79 7468 696e 6720  ot see anything 
+000043f0: 6f6e 2044 4f52 4120 6461 7368 626f 6172  on DORA dashboar
+00004400: 642c 2063 616e 2061 6e79 6f6e 6520 6865  d, can anyone he
+00004410: 6c70 2077 6974 6820 7468 6973 3f22 2c0a  lp with this?",.
+00004420: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
+00004430: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
+00004440: 2274 6f20 6865 6c70 2077 6974 6820 7468  "to help with th
+00004450: 6520 444f 5241 2063 6f6e 6669 6775 7261  e DORA configura
+00004460: 7469 6f6e 2070 726f 6365 7373 2c20 4920  tion process, I 
+00004470: 7265 636f 6d6d 656e 6420 676f 696e 6720  recommend going 
+00004480: 7468 726f 7567 6820 6f75 7220 444f 5241  through our DORA
+00004490: 2067 7569 6465 3a20 6874 7470 733a 2f2f   guide: https://
+000044a0: 6465 766c 616b 652e 6170 6163 6865 2e6f  devlake.apache.o
+000044b0: 7267 2f64 6f63 732f 6e65 7874 2f44 4f52  rg/docs/next/DOR
+000044c0: 412f 2e20 596f 7520 6361 6e20 616c 736f  A/. You can also
+000044d0: 2066 696e 6420 646f 6373 2066 6f72 2074   find docs for t
+000044e0: 6865 2074 6f6f 6c73 2079 6f75 2075 7365  he tools you use
+000044f0: 2068 6572 653a 2068 7474 7073 3a2f 2f64   here: https://d
+00004500: 6576 6c61 6b65 2e61 7061 6368 652e 6f72  evlake.apache.or
+00004510: 672f 646f 6373 2f6e 6578 742f 436f 6e66  g/docs/next/Conf
+00004520: 6967 7572 6174 696f 6e22 2c0a 2020 2020  iguration",.    
+00004530: 2020 2020 2020 2020 2261 6e73 7765 725f          "answer_
+00004540: 7072 6f70 6572 7469 6573 223a 205b 5d2c  properties": [],
+00004550: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+00004560: 7465 7322 3a20 7b0a 2020 2020 2020 2020  tes": {.        
+00004570: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
+00004580: 2022 6d69 6422 0a20 2020 2020 2020 2020   "mid".         
+00004590: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+000045a0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000045b0: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
+000045c0: 6c61 6b65 2d32 3322 2c0a 2020 2020 2020  lake-23",.      
+000045d0: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+000045e0: 3a20 2244 6f65 7320 4170 6163 6865 2044  : "Does Apache D
+000045f0: 6576 6c61 6b65 2073 7570 706f 7274 7320  evlake supports 
+00004600: 6465 706c 6f79 6d65 6e74 206d 6574 7269  deployment metri
+00004610: 6373 2066 726f 6d20 436c 6f75 6442 7569  cs from CloudBui
+00004620: 6c64 2c20 436c 6f75 6420 4465 706c 6f79  ld, Cloud Deploy
+00004630: 2061 6e64 2041 6e74 686f 7320 436f 6e66   and Anthos Conf
+00004640: 6967 204d 616e 6167 656d 656e 743f 222c  ig Management?",
+00004650: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00004660: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+00004670: 2022 4465 764c 616b 6520 6861 736e 2774   "DevLake hasn't
+00004680: 2073 7570 706f 7274 6564 2043 6c6f 7564   supported Cloud
+00004690: 4275 696c 642c 2043 6c6f 7564 2064 6570  Build, Cloud dep
+000046a0: 6c6f 7920 616e 6420 4143 4d20 7965 742e  loy and ACM yet.
+000046b0: 2046 6565 6c20 6672 6565 2074 6f20 6f70   Feel free to op
+000046c0: 656e 2066 6561 7475 7265 2072 6571 7565  en feature reque
+000046d0: 7374 2069 7373 7565 206f 6e20 4769 7448  st issue on GitH
+000046e0: 7562 2e22 2c0a 2020 2020 2020 2020 2020  ub.",.          
+000046f0: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
+00004700: 7469 6573 223a 205b 5d2c 0a20 2020 2020  ties": [],.     
+00004710: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
+00004720: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00004730: 2020 226c 6576 656c 223a 2022 6c6f 7722    "level": "low"
+00004740: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00004750: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00004760: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00004770: 2269 6422 3a20 2264 6576 6c61 6b65 2d32  "id": "devlake-2
+00004780: 3422 2c0a 2020 2020 2020 2020 2020 2020  4",.            
+00004790: 2271 7565 7374 696f 6e22 3a20 2249 2068  "question": "I h
+000047a0: 6176 6520 7365 7420 7570 2044 6576 4c61  ave set up DevLa
+000047b0: 6b65 206f 6e6c 7920 746f 2063 6f6c 6c65  ke only to colle
+000047c0: 6374 2074 6865 2044 4f52 4120 6d65 7472  ct the DORA metr
+000047d0: 6963 7320 7573 696e 6720 6865 6c6d 2062  ics using helm b
+000047e0: 7574 2069 7420 6973 206f 7065 6e69 6e67  ut it is opening
+000047f0: 2074 6865 2044 6576 4c61 6b65 2055 4920   the DevLake UI 
+00004800: 7769 7468 6f75 7420 616e 7920 6175 7468  without any auth
+00004810: 656e 7469 6361 7469 6f6e 2c20 692e 652e  entication, i.e.
+00004820: 206e 6f20 7573 6572 6e61 6d65 2061 6e64   no username and
+00004830: 2070 6173 7377 6f72 642e 2041 7320 4920   password. As I 
+00004840: 616d 2065 6e74 6572 696e 6720 7468 6520  am entering the 
+00004850: 4950 2069 7420 6973 2074 616b 696e 6720  IP it is taking 
+00004860: 6d65 2074 6f20 4465 766c 616b 6520 6461  me to Devlake da
+00004870: 7368 626f 6172 6420 7769 7468 6f75 7420  shboard without 
+00004880: 6173 6b69 6e67 2061 6e79 2075 7365 726e  asking any usern
+00004890: 616d 6520 616e 6420 7061 7373 776f 7264  ame and password
+000048a0: 2e20 4973 2069 7420 7468 6520 636f 7272  . Is it the corr
+000048b0: 6563 7420 6265 6861 7669 6f75 723f 222c  ect behaviour?",
+000048c0: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+000048d0: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+000048e0: 2022 5468 6572 6520 6172 6520 7661 6c75   "There are valu
+000048f0: 6573 2074 6f20 7365 7420 7573 6572 2f70  es to set user/p
+00004900: 6173 7377 6f72 6420 696e 2074 6865 2068  assword in the h
+00004910: 656c 6d20 6368 6172 742e 2042 7920 6465  elm chart. By de
+00004920: 6661 756c 742c 2074 6865 7920 6172 6520  fault, they are 
+00004930: 6e6f 7420 7365 742e 222c 0a20 2020 2020  not set.",.     
+00004940: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
+00004950: 726f 7065 7274 6965 7322 3a20 5b5d 2c0a  roperties": [],.
+00004960: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
+00004970: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
+00004980: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
+00004990: 226d 6964 220a 2020 2020 2020 2020 2020  "mid".          
+000049a0: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+000049b0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000049c0: 2020 2020 2022 6964 223a 2022 6465 766c       "id": "devl
+000049d0: 616b 652d 3235 222c 0a20 2020 2020 2020  ake-25",.       
+000049e0: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
+000049f0: 2022 446f 2079 6f75 2068 6176 6520 706c   "Do you have pl
+00004a00: 616e 7320 746f 2061 6464 2075 7365 7220  ans to add user 
+00004a10: 6d61 6e61 6765 6d65 6e74 2069 6e20 4465  management in De
+00004a20: 764c 616b 6520 5549 3f20 222c 0a20 2020  vLake UI? ",.   
+00004a30: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
+00004a40: 6e63 655f 616e 7377 6572 223a 2022 5468  nce_answer": "Th
+00004a50: 6520 6375 7272 656e 7420 706c 616e 2069  e current plan i
+00004a60: 7320 746f 20e2 809c 6f75 7473 6f75 7263  s to ...outsourc
+00004a70: 65e2 809d 2075 7365 7220 6d61 6e61 6765  e... user manage
+00004a80: 6d65 6e74 2074 6f20 7072 6f6a 6563 7473  ment to projects
+00004a90: 206c 696b 6520 6f61 7574 6832 2d70 726f   like oauth2-pro
+00004aa0: 7879 2069 6e73 7465 6164 206f 6620 7265  xy instead of re
+00004ab0: 696e 7665 6e74 696e 6720 7468 6520 7768  inventing the wh
+00004ac0: 6565 6c20 696e 2068 6f75 7365 2e20 5765  eel in house. We
+00004ad0: 2077 696c 6c20 7365 6520 6966 2077 6520   will see if we 
+00004ae0: 6361 6e20 726f 6c6c 206f 7574 2061 2062  can roll out a b
+00004af0: 6c6f 6720 6f6e 2068 6f77 2074 6f20 7072  log on how to pr
+00004b00: 6f74 6563 7420 436f 6e66 6967 2d55 4920  otect Config-UI 
+00004b10: 7769 7468 206f 6175 7468 322d 7072 6f78  with oauth2-prox
+00004b20: 7920 6173 2061 2073 7461 7274 696e 6720  y as a starting 
+00004b30: 706f 696e 7420 666f 7220 7573 6572 7320  point for users 
+00004b40: 7768 6f20 6172 6520 696e 7465 7265 7374  who are interest
+00004b50: 6564 2069 6e20 676f 696e 6720 646f 776e  ed in going down
+00004b60: 2074 6861 7420 7061 7468 2e22 2c0a 2020   that path.",.  
+00004b70: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
+00004b80: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
+00004b90: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00004ba0: 6e6f 7465 7322 3a20 7b0a 2020 2020 2020  notes": {.      
+00004bb0: 2020 2020 2020 2020 2020 226c 6576 656c            "level
+00004bc0: 223a 2022 6869 6768 220a 2020 2020 2020  ": "high".      
+00004bd0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00004be0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00004bf0: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+00004c00: 6465 766c 616b 652d 3236 222c 0a20 2020  devlake-26",.   
+00004c10: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
+00004c20: 6f6e 223a 2022 5765 2068 6176 6520 646f  on": "We have do
+00004c30: 7a65 6e73 206f 6620 4769 7448 7562 206f  zens of GitHub o
+00004c40: 7267 616e 697a 6174 696f 6e73 2061 6e64  rganizations and
+00004c50: 2068 756e 6472 6564 7320 6f66 2072 6570   hundreds of rep
+00004c60: 6f73 6974 6f72 6965 7320 746f 2074 7261  ositories to tra
+00004c70: 636b 2e20 4174 2074 6861 7420 7363 616c  ck. At that scal
+00004c80: 6520 6974 2069 7320 6469 6666 6963 756c  e it is difficul
+00004c90: 7420 746f 206d 616e 6167 6520 7573 696e  t to manage usin
+00004ca0: 6720 7468 6520 5072 6f6a 6563 7420 696e  g the Project in
+00004cb0: 7465 7266 6163 6520 616e 6420 5549 2e20  terface and UI. 
+00004cc0: 4861 7320 616e 796f 6e65 2074 7269 6564  Has anyone tried
+00004cd0: 2074 6f20 7573 6520 4465 764c 616b 6520   to use DevLake 
+00004ce0: 746f 2077 6f72 6b20 7769 7468 2061 6e79  to work with any
+00004cf0: 7468 696e 6720 636c 6f73 6520 746f 2074  thing close to t
+00004d00: 6861 7420 6b69 6e64 206f 6620 7363 616c  hat kind of scal
+00004d10: 653f 222c 0a20 2020 2020 2020 2020 2020  e?",.           
+00004d20: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
+00004d30: 6572 223a 2022 496e 2043 6f6e 6669 6720  er": "In Config 
+00004d40: 5549 2c20 796f 7520 6361 6e20 7472 7920  UI, you can try 
+00004d50: 7365 6c65 6374 696e 6720 7468 6520 6f72  selecting the or
+00004d60: 6720 746f 2073 656c 6563 7420 616c 6c20  g to select all 
+00004d70: 7265 706f 7369 746f 7269 6573 2075 6e64  repositories und
+00004d80: 6572 2074 6861 7420 6f72 672e 2042 7574  er that org. But
+00004d90: 2069 6620 796f 7520 6e65 6564 2074 6f20   if you need to 
+00004da0: 6164 6420 6120 6c61 7267 6520 6e75 6d62  add a large numb
+00004db0: 6572 206f 6620 7265 706f 7369 746f 7269  er of repositori
+00004dc0: 6573 2075 6e64 6572 2064 6966 6665 7265  es under differe
+00004dd0: 6e74 206f 7267 7320 746f 2061 2070 726f  nt orgs to a pro
+00004de0: 6a65 6374 2c20 7468 6520 6163 7469 6f6e  ject, the action
+00004df0: 2077 696c 6c20 6265 2069 6e65 7669 7461   will be inevita
+00004e00: 626c 7920 6375 6d62 6572 736f 6d65 2069  bly cumbersome i
+00004e10: 6e20 7468 6520 6375 7272 656e 7420 4465  n the current De
+00004e20: 764c 616b 652e 222c 0a20 2020 2020 2020  vLake.",.       
+00004e30: 2020 2020 2022 616e 7377 6572 5f70 726f       "answer_pro
+00004e40: 7065 7274 6965 7322 3a20 5b5d 2c0a 2020  perties": [],.  
+00004e50: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
+00004e60: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00004e70: 2020 2020 2022 6c65 7665 6c22 3a20 2268       "level": "h
+00004e80: 6967 6822 0a20 2020 2020 2020 2020 2020  igh".           
+00004e90: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00004ea0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00004eb0: 2020 2020 2269 6422 3a20 2264 6576 6c61      "id": "devla
+00004ec0: 6b65 2d32 3722 2c0a 2020 2020 2020 2020  ke-27",.        
+00004ed0: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
+00004ee0: 2249 2077 616e 7420 746f 2064 6566 696e  "I want to defin
+00004ef0: 6520 736f 6d65 2063 6f6d 6d69 7473 2061  e some commits a
+00004f00: 7320 6465 706c 6f79 6d65 6e74 206a 6f62  s deployment job
+00004f10: 732c 2073 7563 6820 6173 2063 6f6d 6d69  s, such as commi
+00004f20: 7420 6d65 7373 6167 6573 2073 7461 7274  t messages start
+00004f30: 696e 6720 7769 7468 20e2 809c 6d65 7267  ing with ...merg
+00004f40: 652e 2ee2 809d 206f 7220 736f 6d65 2073  e..... or some s
+00004f50: 7065 6369 6669 6320 6163 636f 756e 7420  pecific account 
+00004f60: 6c69 6b65 2061 646d 696e 2e20 486f 7720  like admin. How 
+00004f70: 6361 6e20 4920 646f 2074 6869 733f 222c  can I do this?",
+00004f80: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00004f90: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+00004fa0: 2022 4966 2049 2075 6e64 6572 7374 616e   "If I understan
+00004fb0: 6420 636f 7272 6563 746c 792c 2079 6f75  d correctly, you
+00004fc0: 2077 6f75 6c64 206c 696b 6520 746f 2072   would like to r
+00004fd0: 6567 6973 7465 7220 6465 706c 6f79 6d65  egister deployme
+00004fe0: 6e74 7320 7769 7468 2063 6f6d 6d69 7473  nts with commits
+00004ff0: 2066 696c 7465 7265 6420 6279 2074 6865   filtered by the
+00005000: 6972 2063 6f6d 6d69 7420 6d65 7373 6167  ir commit messag
+00005010: 6573 2e20 5468 6973 2069 7320 6e6f 7420  es. This is not 
+00005020: 7375 7070 6f72 7465 6420 6e61 7469 7665  supported native
+00005030: 6c79 2062 7920 4465 764c 616b 652e 2042  ly by DevLake. B
+00005040: 7574 2061 2070 6f74 656e 7469 616c 2077  ut a potential w
+00005050: 6f72 6b61 726f 756e 6420 6973 2074 6f20  orkaround is to 
+00005060: 7772 6974 6520 6120 7363 7269 7074 2074  write a script t
+00005070: 6861 7420 7461 6b65 7320 796f 7572 2067  hat takes your g
+00005080: 6974 2072 6570 6f20 6173 2069 6e70 7574  it repo as input
+00005090: 2c20 6669 6c74 6572 2074 6865 2063 6f6d  , filter the com
+000050a0: 6d69 7473 2077 6974 6820 796f 7572 2072  mits with your r
+000050b0: 756c 6573 2c20 616e 6420 7365 6e64 2050  ules, and send P
+000050c0: 4f53 5420 7265 7175 6573 7473 2074 6f20  OST requests to 
+000050d0: 4465 764c 616b 6520 746f 2072 6567 6973  DevLake to regis
+000050e0: 7465 7220 7468 6520 6465 706c 6f79 6d65  ter the deployme
+000050f0: 6e74 7320 7573 696e 6720 4465 764c 616b  nts using DevLak
+00005100: 6527 7320 696e 636f 6d69 6e67 2077 6562  e's incoming web
+00005110: 686f 6f6b 2066 6f72 2064 6570 6c6f 796d  hook for deploym
+00005120: 656e 7473 3a20 6874 7470 733a 2f2f 6465  ents: https://de
+00005130: 766c 616b 652e 6170 6163 6865 2e6f 7267  vlake.apache.org
+00005140: 2f64 6f63 732f 6e65 7874 2f50 6c75 6769  /docs/next/Plugi
+00005150: 6e73 2f77 6562 686f 6f6b 222c 0a20 2020  ns/webhook",.   
+00005160: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
+00005170: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
+00005180: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00005190: 6f74 6573 223a 207b 0a20 2020 2020 2020  otes": {.       
+000051a0: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
+000051b0: 3a20 2268 6967 6822 0a20 2020 2020 2020  : "high".       
+000051c0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+000051d0: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+000051e0: 2020 2020 2020 2020 2269 6422 3a20 2264          "id": "d
+000051f0: 6576 6c61 6b65 2d32 3822 2c0a 2020 2020  evlake-28",.    
+00005200: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00005210: 6e22 3a20 2244 6f65 7320 4c65 6164 2054  n": "Does Lead T
+00005220: 696d 6520 666f 7220 4368 616e 6765 7320  ime for Changes 
+00005230: 7375 7070 6f72 7420 7472 756e 6b2d 6261  support trunk-ba
+00005240: 7365 6420 6465 7665 6c6f 706d 656e 743f  sed development?
+00005250: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00005260: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
+00005270: 223a 2022 5468 6520 6375 7272 656e 7420  ": "The current 
+00005280: 6c65 6164 2074 696d 6520 666f 7220 6368  lead time for ch
+00005290: 616e 6765 7320 6973 2050 522d 6261 7365  anges is PR-base
+000052a0: 6420 616e 6420 776f 756c 6420 6e65 6564  d and would need
+000052b0: 2073 6f6d 6520 6164 6a75 7374 6d65 6e74   some adjustment
+000052c0: 2066 6f72 2064 6972 6563 7420 7075 7368   for direct push
+000052d0: 2069 6e74 6f20 7472 756e 6b2e 222c 0a20   into trunk.",. 
+000052e0: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
+000052f0: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
+00005300: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+00005310: 226e 6f74 6573 223a 207b 0a20 2020 2020  "notes": {.     
+00005320: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
+00005330: 6c22 3a20 226c 6f77 220a 2020 2020 2020  l": "low".      
+00005340: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00005350: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00005360: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+00005370: 6465 766c 616b 652d 3239 222c 0a20 2020  devlake-29",.   
+00005380: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
+00005390: 6f6e 223a 2022 486f 7720 6361 6e20 4920  on": "How can I 
+000053a0: 6465 706c 6f79 2044 6576 4c61 6b65 2077  deploy DevLake w
+000053b0: 6974 6820 356b 2b20 7265 706f 7369 746f  ith 5k+ reposito
+000053c0: 7269 6573 2077 6974 686f 7574 2063 6f6e  ries without con
+000053d0: 7374 616e 746c 7920 6869 7474 696e 6720  stantly hitting 
+000053e0: 7468 6520 7261 7465 206c 696d 6974 2070  the rate limit p
+000053f0: 726f 626c 656d 3f22 2c0a 2020 2020 2020  roblem?",.      
+00005400: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
+00005410: 5f61 6e73 7765 7222 3a20 2231 2e20 4465  _answer": "1. De
+00005420: 764c 616b 6527 7320 4769 7448 7562 2070  vLake's GitHub p
+00005430: 6c75 6769 6e20 646f 6573 2069 6e63 7265  lugin does incre
+00005440: 6d65 6e74 616c 2073 796e 6320 666f 7220  mental sync for 
+00005450: 6d6f 7374 2065 6e74 6974 6965 732e 2054  most entities. T
+00005460: 6f20 7365 6520 7468 6520 6265 6861 7669  o see the behavi
+00005470: 6f72 206f 6620 6f74 6865 7220 706c 7567  or of other plug
+00005480: 696e 732c 2063 6865 636b 206f 7574 2074  ins, check out t
+00005490: 6865 2043 6f6c 6c65 6374 696f 6e20 4d6f  he Collection Mo
+000054a0: 6465 2063 6f6c 756d 6e20 6865 7265 3a20  de column here: 
+000054b0: 6874 7470 733a 2f2f 6465 766c 616b 652e  https://devlake.
+000054c0: 6170 6163 6865 2e6f 7267 2f64 6f63 732f  apache.org/docs/
+000054d0: 6e65 7874 2f4f 7665 7276 6965 772f 5375  next/Overview/Su
+000054e0: 7070 6f72 7465 6444 6174 6153 6f75 7263  pportedDataSourc
+000054f0: 6573 2032 2e20 5072 6f76 6964 696e 6720  es 2. Providing 
+00005500: 6d75 6c74 6970 6c65 2047 6974 4875 6220  multiple GitHub 
+00005510: 5041 5473 2066 726f 6d20 6469 6666 6572  PATs from differ
+00005520: 656e 7420 7573 6572 7320 776f 756c 6420  ent users would 
+00005530: 6d75 6c74 6970 6c79 2079 6f75 7220 7261  multiply your ra
+00005540: 7465 206c 696d 6974 2e20 332e 2054 6865  te limit. 3. The
+00005550: 7265 2773 2061 6e20 6f70 656e 2050 5220  re's an open PR 
+00005560: 666f 7220 7375 7070 6f72 7469 6e67 2047  for supporting G
+00005570: 6974 4875 6220 6170 702c 2077 6869 6368  itHub app, which
+00005580: 206d 6179 2065 6e68 616e 6365 2074 6865   may enhance the
+00005590: 2072 6174 6520 6c69 6d69 7420 666f 7220   rate limit for 
+000055a0: 6c61 7267 6572 206f 7267 732e 222c 0a20  larger orgs.",. 
+000055b0: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
+000055c0: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
+000055d0: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+000055e0: 226e 6f74 6573 223a 207b 0a20 2020 2020  "notes": {.     
+000055f0: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
+00005600: 6c22 3a20 2268 6967 6822 0a20 2020 2020  l": "high".     
+00005610: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00005620: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00005630: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+00005640: 2264 6576 6c61 6b65 2d33 3022 2c0a 2020  "devlake-30",.  
+00005650: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
+00005660: 696f 6e22 3a20 2257 6865 6e20 6372 6561  ion": "When crea
+00005670: 7469 6e67 2074 6561 6d73 2c20 6966 2049  ting teams, if I
+00005680: 2068 6176 6520 6120 6869 6572 6172 6368   have a hierarch
+00005690: 7920 6f66 2070 6172 656e 7473 2061 6e64  y of parents and
+000056a0: 2073 7562 2d74 6561 6d73 2c20 646f 2049   sub-teams, do I
+000056b0: 206e 6565 6420 746f 2070 7574 2074 6865   need to put the
+000056c0: 2073 7562 2d74 6561 6d20 6d65 6d62 6572   sub-team member
+000056d0: 7320 696e 2062 6f74 6820 7061 7265 6e74  s in both parent
+000056e0: 7320 616e 6420 7375 622d 7465 616d 732c  s and sub-teams,
+000056f0: 206f 7220 6a75 7374 2073 7562 2d74 6561   or just sub-tea
+00005700: 6d73 3f22 2c0a 2020 2020 2020 2020 2020  ms?",.          
+00005710: 2020 2272 6566 6572 656e 6365 5f61 6e73    "reference_ans
+00005720: 7765 7222 3a20 2254 6561 6d73 2077 6974  wer": "Teams wit
+00005730: 6869 6e20 4465 764c 616b 6520 646f 6e27  hin DevLake don'
+00005740: 7420 6861 7665 2068 6965 7261 7263 6869  t have hierarchi
+00005750: 6573 2e20 536f 2079 6f75 2070 726f 6261  es. So you proba
+00005760: 626c 7920 7761 6e74 2074 6f20 7075 7420  bly want to put 
+00005770: 7468 6520 7375 622d 7465 616d 206d 656d  the sub-team mem
+00005780: 6265 7273 2069 6e20 626f 7468 2074 6865  bers in both the
+00005790: 2070 6172 656e 7420 616e 6420 7375 622d   parent and sub-
+000057a0: 7465 616d 2e22 2c0a 2020 2020 2020 2020  team.",.        
+000057b0: 2020 2020 2261 6e73 7765 725f 7072 6f70      "answer_prop
+000057c0: 6572 7469 6573 223a 205b 5d2c 0a20 2020  erties": [],.   
+000057d0: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
+000057e0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000057f0: 2020 2020 226c 6576 656c 223a 2022 6d69      "level": "mi
+00005800: 6422 0a20 2020 2020 2020 2020 2020 207d  d".            }
+00005810: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00005820: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00005830: 2020 2269 6422 3a20 2264 6576 6c61 6b65    "id": "devlake
+00005840: 2d33 3122 2c0a 2020 2020 2020 2020 2020  -31",.          
+00005850: 2020 2271 7565 7374 696f 6e22 3a20 2249    "question": "I
+00005860: 7320 5353 4f20 7375 7070 6f72 7465 6420  s SSO supported 
+00005870: 666f 7220 7468 6520 4465 764c 616b 6520  for the DevLake 
+00005880: 5549 2061 6e64 2074 6865 2064 6173 6862  UI and the dashb
+00005890: 6f61 7264 733f 222c 0a20 2020 2020 2020  oards?",.       
+000058a0: 2020 2020 2022 7265 6665 7265 6e63 655f       "reference_
+000058b0: 616e 7377 6572 223a 2022 5353 4f20 6973  answer": "SSO is
+000058c0: 206e 6f74 2073 7570 706f 7274 6564 2063   not supported c
+000058d0: 7572 7265 6e74 6c79 2e22 2c0a 2020 2020  urrently.",.    
+000058e0: 2020 2020 2020 2020 2261 6e73 7765 725f          "answer_
+000058f0: 7072 6f70 6572 7469 6573 223a 205b 5d2c  properties": [],
+00005900: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+00005910: 7465 7322 3a20 7b0a 2020 2020 2020 2020  tes": {.        
+00005920: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
+00005930: 2022 6c6f 7722 0a20 2020 2020 2020 2020   "low".         
+00005940: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+00005950: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00005960: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
+00005970: 6c61 6b65 2d33 3222 2c0a 2020 2020 2020  lake-32",.      
+00005980: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+00005990: 3a20 2249 2065 6e74 6572 6564 2061 2047  : "I entered a G
+000059a0: 6974 4875 6220 746f 6b65 6e20 6275 7420  itHub token but 
+000059b0: 6974 2073 686f 7765 6420 6049 4e56 414c  it showed `INVAL
+000059c0: 4944 2054 4f4b 454e 602e 2057 6861 7420  ID TOKEN`. What 
+000059d0: 636f 756c 6420 6265 2074 6865 2063 6175  could be the cau
+000059e0: 7365 733f 222c 0a20 2020 2020 2020 2020  ses?",.         
+000059f0: 2020 2022 7265 6665 7265 6e63 655f 616e     "reference_an
+00005a00: 7377 6572 223a 2022 506c 6561 7365 2072  swer": "Please r
+00005a10: 6566 6572 2074 6f20 6f75 7220 646f 6373  efer to our docs
+00005a20: 2066 6f72 2077 6861 7420 7065 726d 6973   for what permis
+00005a30: 7369 6f6e 7320 6f66 2047 6974 4875 6220  sions of GitHub 
+00005a40: 746f 6b65 6e73 2061 7265 2072 6571 7569  tokens are requi
+00005a50: 7265 643a 2068 7474 7073 3a2f 2f64 6576  red: https://dev
+00005a60: 6c61 6b65 2e61 7061 6368 652e 6f72 672f  lake.apache.org/
+00005a70: 646f 6373 2f43 6f6e 6669 6775 7261 7469  docs/Configurati
+00005a80: 6f6e 2f47 6974 4875 6222 2c0a 2020 2020  on/GitHub",.    
+00005a90: 2020 2020 2020 2020 2261 6e73 7765 725f          "answer_
+00005aa0: 7072 6f70 6572 7469 6573 223a 205b 5d2c  properties": [],
+00005ab0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+00005ac0: 7465 7322 3a20 7b0a 2020 2020 2020 2020  tes": {.        
+00005ad0: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
+00005ae0: 2022 6c6f 7722 0a20 2020 2020 2020 2020   "low".         
+00005af0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+00005b00: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00005b10: 2020 2020 2020 2269 6422 3a20 2264 6576        "id": "dev
+00005b20: 6c61 6b65 2d33 3322 2c0a 2020 2020 2020  lake-33",.      
+00005b30: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+00005b40: 3a20 2243 616e 2049 2066 696c 7465 7220  : "Can I filter 
+00005b50: 6f75 7420 4769 7448 7562 2069 7373 7565  out GitHub issue
+00005b60: 7320 6372 6561 7465 6420 6279 2062 6f74  s created by bot
+00005b70: 733f 222c 0a20 2020 2020 2020 2020 2020  s?",.           
+00005b80: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
+00005b90: 6572 223a 2022 556e 666f 7274 756e 6174  er": "Unfortunat
+00005ba0: 656c 792c 2074 6865 7265 2069 7320 6e6f  ely, there is no
+00005bb0: 2062 7569 6c74 2d69 6e20 6361 7061 6269   built-in capabi
+00005bc0: 6c69 7479 2077 6974 6869 6e20 4465 764c  lity within DevL
+00005bd0: 616b 6520 746f 2061 7574 6f2d 6669 6c74  ake to auto-filt
+00005be0: 6572 2062 6f74 2061 6374 6976 6974 6965  er bot activitie
+00005bf0: 732e 2042 7574 2061 2077 6f72 6b2d 6172  s. But a work-ar
+00005c00: 6f75 6e64 2073 6f6c 7574 696f 6e20 6973  ound solution is
+00005c10: 2074 6f20 736c 6967 6874 6c79 206d 6f64   to slightly mod
+00005c20: 6966 7920 7468 6520 5351 4c20 7175 6572  ify the SQL quer
+00005c30: 7920 696e 2047 7261 6661 6e61 2064 6173  y in Grafana das
+00005c40: 6862 6f61 7264 7320 746f 2066 696c 7465  hboards to filte
+00005c50: 7220 6973 7375 6573 2f50 5273 2062 7920  r issues/PRs by 
+00005c60: 7468 6569 7220 6175 7468 6f72 732e 222c  their authors.",
+00005c70: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
+00005c80: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
+00005c90: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+00005ca0: 2020 226e 6f74 6573 223a 207b 0a20 2020    "notes": {.   
+00005cb0: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
+00005cc0: 7665 6c22 3a20 226d 6964 220a 2020 2020  vel": "mid".    
+00005cd0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00005ce0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00005cf0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+00005d00: 2022 6465 766c 616b 652d 3334 222c 0a20   "devlake-34",. 
+00005d10: 2020 2020 2020 2020 2020 2022 7175 6573             "ques
+00005d20: 7469 6f6e 223a 2022 486f 7720 646f 2049  tion": "How do I
+00005d30: 206c 6f67 696e 2074 6f20 4772 6166 616e   login to Grafan
+00005d40: 6120 746f 2061 6363 6573 7320 7468 6520  a to access the 
+00005d50: 6461 7368 626f 6172 6473 222c 0a20 2020  dashboards",.   
+00005d60: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
+00005d70: 6e63 655f 616e 7377 6572 223a 2022 4279  nce_answer": "By
+00005d80: 2064 6566 6175 6c74 2074 6865 2075 7365   default the use
+00005d90: 7220 616e 6420 7061 7373 776f 7264 2061  r and password a
+00005da0: 7265 2073 6574 2074 6f20 6164 6d69 6e2e  re set to admin.
+00005db0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00005dc0: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
+00005dd0: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+00005de0: 2020 2020 226e 6f74 6573 223a 207b 0a20      "notes": {. 
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005e00: 6c65 7665 6c22 3a20 226c 6f77 220a 2020  level": "low".  
+00005e10: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00005e20: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+00005e30: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
+00005e40: 223a 2022 6465 766c 616b 652d 3335 222c  ": "devlake-35",
+00005e50: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
+00005e60: 6573 7469 6f6e 223a 2022 4973 2069 7420  estion": "Is it 
+00005e70: 706f 7373 6962 6c65 2074 6f20 6d6f 6469  possible to modi
+00005e80: 6679 2061 2062 6c75 6570 7269 6e74 2077  fy a blueprint w
+00005e90: 6974 6820 616e 2061 6464 6974 696f 6e61  ith an additiona
+00005ea0: 6c20 696e 7465 6772 6174 696f 6e20 6166  l integration af
+00005eb0: 7465 7220 6974 7320 6265 656e 2063 7265  ter its been cre
+00005ec0: 6174 6564 3f22 2c0a 2020 2020 2020 2020  ated?",.        
+00005ed0: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
+00005ee0: 6e73 7765 7222 3a20 2259 6573 2c20 6672  nswer": "Yes, fr
+00005ef0: 6f6d 2076 302e 3137 2079 6f75 2063 616e  om v0.17 you can
+00005f00: 2061 6464 206d 6f72 6520 6461 7461 2063   add more data c
+00005f10: 6f6e 6e65 6374 696f 6e73 2074 6f20 616e  onnections to an
+00005f20: 2065 7869 7374 696e 6720 626c 7565 7072   existing bluepr
+00005f30: 696e 7422 2c0a 2020 2020 2020 2020 2020  int",.          
+00005f40: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
+00005f50: 7469 6573 223a 205b 5d2c 0a20 2020 2020  ties": [],.     
+00005f60: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
+00005f70: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00005f80: 2020 226c 6576 656c 223a 2022 6c6f 7722    "level": "low"
+00005f90: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00005fa0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00005fb0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00005fc0: 2269 6422 3a20 2264 6576 6c61 6b65 2d33  "id": "devlake-3
+00005fd0: 3622 2c0a 2020 2020 2020 2020 2020 2020  6",.            
+00005fe0: 2271 7565 7374 696f 6e22 3a20 2257 6865  "question": "Whe
+00005ff0: 6e20 7368 6f75 6c64 2049 2075 7365 2061  n should I use a
+00006000: 6476 616e 6365 6420 6d6f 6465 2066 6f72  dvanced mode for
+00006010: 2061 2062 6c75 6570 7269 6e74 3f22 2c0a   a blueprint?",.
+00006020: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
+00006030: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
+00006040: 2241 6476 616e 6365 6420 6d6f 6465 2061  "Advanced mode a
+00006050: 6c6c 6f77 7320 7573 6572 7320 746f 2063  llows users to c
+00006060: 7265 6174 6520 616e 7920 7069 7065 6c69  reate any pipeli
+00006070: 6e65 2062 7920 7772 6974 696e 6720 4a53  ne by writing JS
+00006080: 4f4e 2e20 5468 6973 2069 7320 7573 6566  ON. This is usef
+00006090: 756c 2066 6f72 2075 7365 7273 2077 686f  ul for users who
+000060a0: 2077 616e 7420 746f 2063 6f6c 6c65 6374   want to collect
+000060b0: 206d 756c 7469 706c 6520 4769 7448 7562   multiple GitHub
+000060c0: 2f47 6974 4c61 6220 7265 706f 7320 6f72  /GitLab repos or
+000060d0: 204a 6972 6120 7072 6f6a 6563 7473 2077   Jira projects w
+000060e0: 6974 6869 6e20 6120 7369 6e67 6c65 2070  ithin a single p
+000060f0: 6970 656c 696e 652c 2068 6176 6520 6669  ipeline, have fi
+00006100: 6e65 2d67 7261 696e 6564 2063 6f6e 7472  ne-grained contr
+00006110: 6f6c 206f 7665 7220 7768 6174 2065 6e74  ol over what ent
+00006120: 6974 6965 7320 746f 2063 6f6c 6c65 6374  ities to collect
+00006130: 206f 7220 7768 6174 2073 7562 7461 736b   or what subtask
+00006140: 7320 746f 2072 756e 2066 6f72 2065 6163  s to run for eac
+00006150: 6820 706c 7567 696e 2c20 616e 6420 6f72  h plugin, and or
+00006160: 6368 6573 7472 6174 6520 6120 636f 6d70  chestrate a comp
+00006170: 6c65 7820 7069 7065 6c69 6e65 2074 6861  lex pipeline tha
+00006180: 7420 636f 6e73 6973 7473 206f 6620 6d75  t consists of mu
+00006190: 6c74 6970 6c65 2073 7461 6765 7320 6f66  ltiple stages of
+000061a0: 2070 6c75 6769 6e73 2e20 596f 7520 6361   plugins. You ca
+000061b0: 6e20 7265 6665 7220 746f 206f 7572 2064  n refer to our d
+000061c0: 6f63 2066 6f72 206d 6f72 6520 6465 7461  oc for more deta
+000061d0: 696c 733a 2068 7474 7073 3a2f 2f64 6576  ils: https://dev
+000061e0: 6c61 6b65 2e61 7061 6368 652e 6f72 672f  lake.apache.org/
+000061f0: 646f 6373 2f43 6f6e 6669 6775 7261 7469  docs/Configurati
+00006200: 6f6e 2f41 6476 616e 6365 644d 6f64 6522  on/AdvancedMode"
+00006210: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+00006220: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
+00006230: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
+00006240: 2020 2022 6e6f 7465 7322 3a20 7b0a 2020     "notes": {.  
+00006250: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00006260: 6576 656c 223a 2022 6c6f 7722 0a20 2020  evel": "low".   
+00006270: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00006280: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00006290: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+000062a0: 3a20 2264 6576 6c61 6b65 2d33 3722 2c0a  : "devlake-37",.
+000062b0: 2020 2020 2020 2020 2020 2020 2271 7565              "que
+000062c0: 7374 696f 6e22 3a20 2248 6f77 2064 6f20  stion": "How do 
+000062d0: 4920 636f 6e66 6967 7572 6520 536f 6e61  I configure Sona
+000062e0: 7251 7562 653f 222c 0a20 2020 2020 2020  rQube?",.       
+000062f0: 2020 2020 2022 7265 6665 7265 6e63 655f       "reference_
+00006300: 616e 7377 6572 223a 2022 506c 6561 7365  answer": "Please
+00006310: 2066 6f6c 6c6f 7720 7468 6520 696e 7374   follow the inst
+00006320: 7275 6374 696f 6e20 696e 2074 6869 7320  ruction in this 
+00006330: 646f 633a 2068 7474 7073 3a2f 2f64 6576  doc: https://dev
+00006340: 6c61 6b65 2e61 7061 6368 652e 6f72 672f  lake.apache.org/
+00006350: 646f 6373 2f6e 6578 742f 436f 6e66 6967  docs/next/Config
+00006360: 7572 6174 696f 6e2f 536f 6e61 7251 7562  uration/SonarQub
+00006370: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00006380: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
+00006390: 6573 223a 205b 5d2c 0a20 2020 2020 2020  es": [],.       
+000063a0: 2020 2020 2022 6e6f 7465 7322 3a20 7b0a       "notes": {.
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 226c 6576 656c 223a 2022 6c6f 7722 0a20  "level": "low". 
+000063d0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000063e0: 2020 2020 207d 0a20 2020 205d 0a7d 0a         }.    ].}.
```

## chat/evaluation/qa/data/dataset/devlake_test_set_mini.json

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

```diff
@@ -1,772 +1,766 @@
-00000000: 7b0d 0a20 2020 2022 6e61 6d65 223a 2022  {..    "name": "
-00000010: 4465 764c 616b 6520 5265 706f 2051 7565  DevLake Repo Que
-00000020: 7374 696f 6e73 222c 0d0a 2020 2020 2264  stions",..    "d
-00000030: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00000040: 6573 6520 7175 6573 7469 6f6e 7320 636f  ese questions co
-00000050: 6d65 2066 726f 6d20 6465 766c 616b 655f  me from devlake_
-00000060: 7265 706f 5f71 7565 7374 696f 6e73 2e6a  repo_questions.j
-00000070: 736f 6e20 2877 6974 686f 7574 2044 5251  son (without DRQ
-00000080: 2d33 2c20 352c 2036 2c20 3134 2c20 3136  -3, 5, 6, 14, 16
-00000090: 292e 222c 0d0a 2020 2020 2263 6173 6573  ).",..    "cases
-000000a0: 223a 205b 0d0a 2020 2020 2020 2020 7b0d  ": [..        {.
-000000b0: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
-000000c0: 223a 2022 4452 512d 3122 2c0d 0a20 2020  ": "DRQ-1",..   
-000000d0: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
-000000e0: 6f6e 223a 2022 486f 7720 6973 2074 6865  on": "How is the
-000000f0: 206c 6561 6420 7469 6d65 2066 6f72 2063   lead time for c
-00000100: 6861 6e67 6573 2063 616c 6375 6c61 7465  hanges calculate
-00000110: 643f 222c 0d0a 2020 2020 2020 2020 2020  d?",..          
-00000120: 2020 2272 6566 6572 656e 6365 5f61 6e73    "reference_ans
-00000130: 7765 7222 3a20 2254 6865 206c 6561 6420  wer": "The lead 
-00000140: 7469 6d65 2066 6f72 2063 6861 6e67 6573  time for changes
-00000150: 2069 7320 6361 6c63 756c 6174 6564 2069   is calculated i
-00000160: 6e20 7468 6520 6043 616c 6375 6c61 7465  n the `Calculate
-00000170: 4368 616e 6765 4c65 6164 5469 6d65 6020  ChangeLeadTime` 
-00000180: 6675 6e63 7469 6f6e 2062 7920 666f 6c6c  function by foll
-00000190: 6f77 696e 6720 7468 6573 6520 7374 6570  owing these step
-000001a0: 733a 5c6e 5c6e 312e 2047 6574 2070 756c  s:\n\n1. Get pul
-000001b0: 6c20 7265 7175 6573 7473 2062 7920 7468  l requests by th
-000001c0: 6520 7072 6f6a 6563 7420 6e61 6d65 2e5c  e project name.\
-000001d0: 6e32 2e20 466f 7220 6561 6368 2070 756c  n2. For each pul
-000001e0: 6c20 7265 7175 6573 742c 2067 6574 2074  l request, get t
-000001f0: 6865 2066 6972 7374 2063 6f6d 6d69 7420  he first commit 
-00000200: 616e 6420 6361 6c63 756c 6174 6520 7468  and calculate th
-00000210: 6520 5052 2063 6f64 696e 6720 7469 6d65  e PR coding time
-00000220: 2061 7320 7468 6520 7469 6d65 2073 7061   as the time spa
-00000230: 6e20 6265 7477 6565 6e20 7468 6520 6669  n between the fi
-00000240: 7273 7420 636f 6d6d 6974 2773 2061 7574  rst commit's aut
-00000250: 686f 7265 6420 6461 7465 2061 6e64 2074  hored date and t
-00000260: 6865 2070 756c 6c20 7265 7175 6573 7427  he pull request'
-00000270: 7320 6372 6561 7465 6420 6461 7465 2e5c  s created date.\
-00000280: 6e33 2e20 4765 7420 7468 6520 6669 7273  n3. Get the firs
-00000290: 7420 7265 7669 6577 2066 6f72 2074 6865  t review for the
-000002a0: 2070 756c 6c20 7265 7175 6573 7420 2865   pull request (e
-000002b0: 7863 6c75 6469 6e67 2063 6f6d 6d65 6e74  xcluding comment
-000002c0: 7320 6672 6f6d 2074 6865 2050 5220 6372  s from the PR cr
-000002d0: 6561 746f 7229 2061 6e64 2063 616c 6375  eator) and calcu
-000002e0: 6c61 7465 2074 6865 2050 5220 7069 636b  late the PR pick
-000002f0: 7570 2074 696d 6520 6173 2074 6865 2074  up time as the t
-00000300: 696d 6520 7370 616e 2062 6574 7765 656e  ime span between
-00000310: 2074 6865 2070 756c 6c20 7265 7175 6573   the pull reques
-00000320: 7427 7320 6372 6561 7465 6420 6461 7465  t's created date
-00000330: 2061 6e64 2074 6865 2066 6972 7374 2072   and the first r
-00000340: 6576 6965 7727 7320 6372 6561 7465 6420  eview's created 
-00000350: 6461 7465 2e20 4361 6c63 756c 6174 6520  date. Calculate 
-00000360: 7468 6520 5052 2072 6576 6965 7720 7469  the PR review ti
-00000370: 6d65 2061 7320 7468 6520 7469 6d65 2073  me as the time s
-00000380: 7061 6e20 6265 7477 6565 6e20 7468 6520  pan between the 
-00000390: 6669 7273 7420 7265 7669 6577 2773 2063  first review's c
-000003a0: 7265 6174 6564 2064 6174 6520 616e 6420  reated date and 
-000003b0: 7468 6520 7075 6c6c 2072 6571 7565 7374  the pull request
-000003c0: 2773 206d 6572 6765 6420 6461 7465 2e5c  's merged date.\
-000003d0: 6e34 2e20 4765 7420 7468 6520 6465 706c  n4. Get the depl
-000003e0: 6f79 6d65 6e74 2066 6f72 2074 6865 2070  oyment for the p
-000003f0: 756c 6c20 7265 7175 6573 7420 7573 696e  ull request usin
-00000400: 6720 7468 6520 6d65 7267 6520 636f 6d6d  g the merge comm
-00000410: 6974 2053 4841 2061 6e64 2063 616c 6375  it SHA and calcu
-00000420: 6c61 7465 2074 6865 2050 5220 6465 706c  late the PR depl
-00000430: 6f79 2074 696d 6520 6173 2074 6865 2074  oy time as the t
-00000440: 696d 6520 7370 616e 2062 6574 7765 656e  ime span between
-00000450: 2074 6865 2070 756c 6c20 7265 7175 6573   the pull reques
-00000460: 7427 7320 6d65 7267 6564 2064 6174 6520  t's merged date 
-00000470: 616e 6420 7468 6520 6465 706c 6f79 6d65  and the deployme
-00000480: 6e74 2773 2066 696e 6973 6865 6420 6461  nt's finished da
-00000490: 7465 2e5c 6e35 2e20 4361 6c63 756c 6174  te.\n5. Calculat
-000004a0: 6520 7468 6520 5052 2063 7963 6c65 2074  e the PR cycle t
-000004b0: 696d 6520 6279 2061 6464 696e 6720 7468  ime by adding th
-000004c0: 6520 5052 2063 6f64 696e 6720 7469 6d65  e PR coding time
-000004d0: 2c20 5052 2064 7572 696e 6720 7469 6d65  , PR during time
-000004e0: 2028 7469 6d65 2073 7061 6e20 6265 7477   (time span betw
-000004f0: 6565 6e20 7468 6520 7075 6c6c 2072 6571  een the pull req
-00000500: 7565 7374 2773 2063 7265 6174 6564 2064  uest's created d
-00000510: 6174 6520 616e 6420 6d65 7267 6564 2064  ate and merged d
-00000520: 6174 6529 2c20 616e 6420 5052 2064 6570  ate), and PR dep
-00000530: 6c6f 7920 7469 6d65 2e5c 6e5c 6e54 6865  loy time.\n\nThe
-00000540: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
-00000550: 7320 6120 6050 726f 6a65 6374 5072 4d65  s a `ProjectPrMe
-00000560: 7472 6963 6020 6f62 6a65 6374 2063 6f6e  tric` object con
-00000570: 7461 696e 696e 6720 7468 6520 6361 6c63  taining the calc
-00000580: 756c 6174 6564 206c 6561 6420 7469 6d65  ulated lead time
-00000590: 7320 666f 7220 6561 6368 2070 756c 6c20  s for each pull 
-000005a0: 7265 7175 6573 7420 696e 2074 6865 2070  request in the p
-000005b0: 726f 6a65 6374 2e22 2c0d 0a20 2020 2020  roject.",..     
-000005c0: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
-000005d0: 726f 7065 7274 6965 7322 3a20 5b5d 2c0d  roperties": [],.
-000005e0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-000005f0: 7465 7322 3a20 7b0d 0a20 2020 2020 2020  tes": {..       
-00000600: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
-00000610: 3a20 226d 6964 220d 0a20 2020 2020 2020  : "mid"..       
-00000620: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000630: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00000640: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00000650: 2022 4452 512d 3222 2c0d 0a20 2020 2020   "DRQ-2",..     
-00000660: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
-00000670: 223a 2022 5768 7920 6361 6e20 7468 6520  ": "Why can the 
-00000680: 6c65 6164 2074 696d 6520 666f 7220 6368  lead time for ch
-00000690: 616e 6765 7320 6d65 7472 6963 2062 6520  anges metric be 
-000006a0: 6e75 6c6c 2073 6f6d 6574 696d 6573 3f22  null sometimes?"
-000006b0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000006c0: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
-000006d0: 223a 2022 5468 6520 6c65 6164 2074 696d  ": "The lead tim
-000006e0: 6520 666f 7220 6368 616e 6765 7320 6d65  e for changes me
-000006f0: 7472 6963 2063 616e 2062 6520 6e75 6c6c  tric can be null
-00000700: 2073 6f6d 6574 696d 6573 2062 6563 6175   sometimes becau
-00000710: 7365 2073 6f6d 6520 6f66 2074 6865 2074  se some of the t
-00000720: 696d 6520 7370 616e 7320 7573 6564 2074  ime spans used t
-00000730: 6f20 6361 6c63 756c 6174 6520 6974 206d  o calculate it m
-00000740: 6967 6874 2062 6520 6e75 6c6c 2e20 496e  ight be null. In
-00000750: 2074 6865 2060 4361 6c63 756c 6174 6543   the `CalculateC
-00000760: 6861 6e67 654c 6561 6454 696d 6560 2066  hangeLeadTime` f
-00000770: 756e 6374 696f 6e2c 2074 6865 2050 5220  unction, the PR 
-00000780: 636f 6469 6e67 2074 696d 652c 2050 5220  coding time, PR 
-00000790: 7069 636b 7570 2074 696d 652c 2050 5220  pickup time, PR 
-000007a0: 7265 7669 6577 2074 696d 652c 2061 6e64  review time, and
-000007b0: 2050 5220 6465 706c 6f79 2074 696d 6520   PR deploy time 
-000007c0: 6172 6520 6361 6c63 756c 6174 6564 2e20  are calculated. 
-000007d0: 4966 2061 6e79 206f 6620 7468 6573 6520  If any of these 
-000007e0: 7469 6d65 2073 7061 6e73 2061 7265 206e  time spans are n
-000007f0: 756c 6c20 6f72 2068 6176 6520 6e65 6761  ull or have nega
-00000800: 7469 7665 2076 616c 7565 732c 2074 6865  tive values, the
-00000810: 2066 696e 616c 2050 5220 6379 636c 6520   final PR cycle 
-00000820: 7469 6d65 2028 6c65 6164 2074 696d 6520  time (lead time 
-00000830: 666f 7220 6368 616e 6765 7329 206d 6967  for changes) mig
-00000840: 6874 206e 6f74 2062 6520 6361 6c63 756c  ht not be calcul
-00000850: 6174 6564 2c20 7265 7375 6c74 696e 6720  ated, resulting 
-00000860: 696e 2061 206e 756c 6c20 7661 6c75 652e  in a null value.
-00000870: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000880: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
-00000890: 6573 223a 205b 5d2c 0d0a 2020 2020 2020  es": [],..      
-000008a0: 2020 2020 2020 226e 6f74 6573 223a 207b        "notes": {
-000008b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008c0: 2020 226c 6576 656c 223a 2022 6c6f 7722    "level": "low"
-000008d0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-000008e0: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-000008f0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00000900: 2020 2020 2269 6422 3a20 2251 5244 2d34      "id": "QRD-4
-00000910: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000920: 2271 7565 7374 696f 6e22 3a20 2257 6861  "question": "Wha
-00000930: 7420 6461 7461 2064 6f65 7320 7468 6520  t data does the 
-00000940: 417a 7572 6520 4465 764f 7073 2070 6c75  Azure DevOps plu
-00000950: 6769 6e20 636f 6c6c 6563 743f 222c 0d0a  gin collect?",..
-00000960: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
-00000970: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
-00000980: 2254 6865 2041 7a75 7265 2044 6576 4f70  "The Azure DevOp
-00000990: 7320 706c 7567 696e 2063 6f6c 6c65 6374  s plugin collect
-000009a0: 7320 6461 7461 2072 656c 6174 6564 2074  s data related t
-000009b0: 6f20 4769 7420 7265 706f 7369 746f 7269  o Git repositori
-000009c0: 6573 2c20 4769 7420 7075 6c6c 2072 6571  es, Git pull req
-000009d0: 7565 7374 732c 2047 6974 2070 756c 6c20  uests, Git pull 
-000009e0: 7265 7175 6573 7420 636f 6d6d 6974 732c  request commits,
-000009f0: 2062 7569 6c64 732c 2061 6e64 206a 6f62   builds, and job
-00000a00: 732e 2053 7065 6369 6669 6361 6c6c 792c  s. Specifically,
-00000a10: 2069 7420 636f 6c6c 6563 7473 2069 6e66   it collects inf
-00000a20: 6f72 6d61 7469 6f6e 2073 7563 6820 6173  ormation such as
-00000a30: 3a5c 6e5c 6e31 2e20 4769 7450 756c 6c52  :\n\n1. GitPullR
-00000a40: 6571 7565 7374 733a 2042 6173 6520 7265  equests: Base re
-00000a50: 706f 7369 746f 7279 2049 442c 2068 6561  pository ID, hea
-00000a60: 6420 7265 706f 7369 746f 7279 2049 442c  d repository ID,
-00000a70: 2073 7461 7475 732c 206f 7269 6769 6e61   status, origina
-00000a80: 6c20 7374 6174 7573 2c20 7469 746c 652c  l status, title,
-00000a90: 2064 6573 6372 6970 7469 6f6e 2c20 5552   description, UR
-00000aa0: 4c2c 2061 7574 686f 7220 6e61 6d65 2c20  L, author name, 
-00000ab0: 6175 7468 6f72 2049 442c 2070 756c 6c20  author ID, pull 
-00000ac0: 7265 7175 6573 7420 6b65 792c 2063 7265  request key, cre
-00000ad0: 6174 6564 2064 6174 652c 206d 6572 6765  ated date, merge
-00000ae0: 6420 6461 7465 2c20 636c 6f73 6564 2064  d date, closed d
-00000af0: 6174 652c 2074 7970 652c 2063 6f6d 706f  ate, type, compo
-00000b00: 6e65 6e74 2c20 6d65 7267 6520 636f 6d6d  nent, merge comm
-00000b10: 6974 2053 4841 2c20 6865 6164 2072 6566  it SHA, head ref
-00000b20: 6572 656e 6365 2c20 6261 7365 2072 6566  erence, base ref
-00000b30: 6572 656e 6365 2c20 6865 6164 2063 6f6d  erence, head com
-00000b40: 6d69 7420 5348 412c 2061 6e64 2062 6173  mit SHA, and bas
-00000b50: 6520 636f 6d6d 6974 2053 4841 2e5c 6e5c  e commit SHA.\n\
-00000b60: 6e32 2e20 4769 7450 756c 6c52 6571 7565  n2. GitPullReque
-00000b70: 7374 436f 6d6d 6974 733a 2043 6f6d 6d69  stCommits: Commi
-00000b80: 7420 5348 4120 2863 6f6d 6d69 745f 6964  t SHA (commit_id
-00000b90: 292c 2070 756c 6c20 7265 7175 6573 7420  ), pull request 
-00000ba0: 4944 2c20 636f 6d6d 6974 2061 7574 686f  ID, commit autho
-00000bb0: 7220 6e61 6d65 2028 6175 7468 6f72 5f6e  r name (author_n
-00000bc0: 616d 6529 2c20 636f 6d6d 6974 2061 7574  ame), commit aut
-00000bd0: 686f 7220 656d 6169 6c20 2861 7574 686f  hor email (autho
-00000be0: 725f 656d 6169 6c29 2c20 616e 6420 636f  r_email), and co
-00000bf0: 6d6d 6974 2061 7574 686f 7265 6420 6461  mmit authored da
-00000c00: 7465 2028 6175 7468 6f72 5f64 6174 6529  te (author_date)
-00000c10: 2e5c 6e5c 6e33 2e20 4275 696c 6473 3a20  .\n\n3. Builds: 
-00000c20: 4275 696c 6427 7320 6e61 6d65 2c20 7374  Build's name, st
-00000c30: 6174 7573 2c20 6372 6561 7465 6420 6461  atus, created da
-00000c40: 7465 2c20 6669 6e69 7368 6564 2064 6174  te, finished dat
-00000c50: 652c 2072 6573 756c 742c 2064 7572 6174  e, result, durat
-00000c60: 696f 6e20 696e 2073 6563 6f6e 6473 2c20  ion in seconds, 
-00000c70: 656e 7669 726f 6e6d 656e 742c 2074 7970  environment, typ
-00000c80: 652c 2061 6e64 206f 7468 6572 2072 656c  e, and other rel
-00000c90: 6174 6564 2064 6574 6169 6c73 206c 696b  ated details lik
-00000ca0: 6520 636f 6d6d 6974 2053 4841 2c20 6272  e commit SHA, br
-00000cb0: 616e 6368 2c20 7265 706f 7369 746f 7279  anch, repository
-00000cc0: 2049 442c 2061 6e64 2072 6570 6f73 6974   ID, and reposit
-00000cd0: 6f72 7920 5552 4c2e 5c6e 5c6e 342e 204a  ory URL.\n\n4. J
-00000ce0: 6f62 733a 204a 6f62 2049 442c 206e 616d  obs: Job ID, nam
-00000cf0: 652c 2062 7569 6c64 2049 442c 2073 7461  e, build ID, sta
-00000d00: 7475 732c 2073 7461 7274 2074 696d 652c  tus, start time,
-00000d10: 2066 696e 6973 6820 7469 6d65 2c20 7265   finish time, re
-00000d20: 7375 6c74 2c20 7479 7065 2c20 6475 7261  sult, type, dura
-00000d30: 7469 6f6e 2069 6e20 7365 636f 6e64 732c  tion in seconds,
-00000d40: 2065 6e76 6972 6f6e 6d65 6e74 2c20 616e   environment, an
-00000d50: 6420 4349 4344 2073 636f 7065 2049 442e  d CICD scope ID.
-00000d60: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000d70: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
-00000d80: 6573 223a 205b 5d2c 0d0a 2020 2020 2020  es": [],..      
-00000d90: 2020 2020 2020 226e 6f74 6573 223a 207b        "notes": {
-00000da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000db0: 2020 226c 6576 656c 223a 2022 6d69 6422    "level": "mid"
-00000dc0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-00000dd0: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00000de0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00000df0: 2020 2020 2269 6422 3a20 2251 5244 2d37      "id": "QRD-7
-00000e00: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000e10: 2271 7565 7374 696f 6e22 3a20 2248 6f77  "question": "How
-00000e20: 2063 616e 2049 2063 6f6e 7472 6962 7574   can I contribut
-00000e30: 6520 746f 2044 6576 4c61 6b65 3f22 2c0d  e to DevLake?",.
-00000e40: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00000e50: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
-00000e60: 2022 596f 7520 6361 6e20 636f 6e74 7269   "You can contri
-00000e70: 6275 7465 2074 6f20 4465 764c 616b 6520  bute to DevLake 
-00000e80: 696e 2073 6576 6572 616c 2077 6179 733a  in several ways:
-00000e90: 5c6e 5c6e 312e 2043 7265 6174 6520 616e  \n\n1. Create an
-00000ea0: 2049 7373 7565 3a20 5265 706f 7274 2061   Issue: Report a
-00000eb0: 2062 7567 206f 7220 6665 6174 7572 6520   bug or feature 
-00000ec0: 7265 7175 6573 7420 746f 2041 7061 6368  request to Apach
-00000ed0: 6520 4465 764c 616b 652e 5c6e 322e 2053  e DevLake.\n2. S
-00000ee0: 7562 6d69 7420 6120 5052 2028 5075 6c6c  ubmit a PR (Pull
-00000ef0: 2052 6571 7565 7374 293a 2053 7461 7274   Request): Start
-00000f00: 2077 6974 6820 676f 6f64 2066 6972 7374   with good first
-00000f10: 2069 7373 7565 7320 6f72 2069 7373 7565   issues or issue
-00000f20: 7320 7769 7468 206e 6f20 6173 7369 676e  s with no assign
-00000f30: 6565 732e 2052 6561 6420 7468 726f 7567  ees. Read throug
-00000f40: 6820 7468 6520 5b43 6f6e 7472 6962 7574  h the [Contribut
-00000f50: 696e 6720 446f 6375 6d65 6e74 6174 696f  ing Documentatio
-00000f60: 6e5d 2868 7474 7073 3a2f 2f64 6576 6c61  n](https://devla
-00000f70: 6b65 2e61 7061 6368 652e 6f72 672f 636f  ke.apache.org/co
-00000f80: 6d6d 756e 6974 792f 292c 2061 6464 2072  mmunity/), add r
-00000f90: 656c 6576 616e 7420 7465 7374 732c 2064  elevant tests, d
-00000fa0: 6f63 756d 656e 7461 7469 6f6e 2c20 616e  ocumentation, an
-00000fb0: 6420 6c61 6265 6c73 2074 6f20 7468 6520  d labels to the 
-00000fc0: 5052 2e5c 6e33 2e20 4a6f 696e 204d 6169  PR.\n3. Join Mai
-00000fd0: 6c69 6e67 206c 6973 743a 2049 6e69 7469  ling list: Initi
-00000fe0: 6174 6520 6f72 2070 6172 7469 6369 7061  ate or participa
-00000ff0: 7465 2069 6e20 7072 6f6a 6563 7420 6469  te in project di
-00001000: 7363 7573 7369 6f6e 7320 6f6e 2074 6865  scussions on the
-00001010: 206d 6169 6c69 6e67 206c 6973 742e 5c6e   mailing list.\n
-00001020: 342e 2057 7269 7465 2061 2042 6c6f 673a  4. Write a Blog:
-00001030: 2057 7269 7465 2061 2062 6c6f 6720 746f   Write a blog to
-00001040: 2073 6861 7265 2079 6f75 7220 7573 6520   share your use 
-00001050: 6361 7365 7320 6162 6f75 7420 4170 6163  cases about Apac
-00001060: 6865 2044 6576 4c61 6b65 2e5c 6e35 2e20  he DevLake.\n5. 
-00001070: 436f 6e74 7269 6275 7465 2061 2050 6c75  Contribute a Plu
-00001080: 6769 6e3a 2041 6464 2061 2070 6c75 6769  gin: Add a plugi
-00001090: 6e20 746f 2069 6e74 6567 7261 7465 2041  n to integrate A
-000010a0: 7061 6368 6520 4465 764c 616b 6520 7769  pache DevLake wi
-000010b0: 7468 206d 6f72 6520 6461 7461 2073 6f75  th more data sou
-000010c0: 7263 6573 2066 6f72 2074 6865 2063 6f6d  rces for the com
-000010d0: 6d75 6e69 7479 2e5c 6e5c 6e50 6c65 6173  munity.\n\nPleas
-000010e0: 6520 7265 6164 2074 6865 205b 636f 6e74  e read the [cont
-000010f0: 7269 6275 7469 6f6e 2067 7569 6465 6c69  ribution guideli
-00001100: 6e65 735d 2868 7474 7073 3a2f 2f64 6576  nes](https://dev
-00001110: 6c61 6b65 2e61 7061 6368 652e 6f72 672f  lake.apache.org/
-00001120: 636f 6d6d 756e 6974 7929 2062 6566 6f72  community) befor
-00001130: 6520 796f 7520 6d61 6b65 2061 2063 6f6e  e you make a con
-00001140: 7472 6962 7574 696f 6e2e 222c 0d0a 2020  tribution.",..  
-00001150: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
-00001160: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
-00001170: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00001180: 226e 6f74 6573 223a 207b 0d0a 2020 2020  "notes": {..    
-00001190: 2020 2020 2020 2020 2020 2020 226c 6576              "lev
-000011a0: 656c 223a 2022 6c6f 7722 0d0a 2020 2020  el": "low"..    
-000011b0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-000011c0: 2020 207d 2c0d 0a20 2020 2020 2020 207b     },..        {
-000011d0: 0d0a 2020 2020 2020 2020 2020 2020 2269  ..            "i
-000011e0: 6422 3a20 2251 5244 2d38 222c 0d0a 2020  d": "QRD-8",..  
-000011f0: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
-00001200: 696f 6e22 3a20 2244 6f65 7320 4465 764c  ion": "Does DevL
-00001210: 616b 6527 7320 4769 7448 7562 2070 6c75  ake's GitHub plu
-00001220: 6769 6e20 7375 7070 6f72 7420 696e 6372  gin support incr
-00001230: 656d 656e 7461 6c20 7379 6e63 3f22 2c0d  emental sync?",.
-00001240: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00001250: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
-00001260: 2022 5965 732c 2044 6576 4c61 6b65 2773   "Yes, DevLake's
-00001270: 2047 6974 4875 6220 706c 7567 696e 2073   GitHub plugin s
-00001280: 7570 706f 7274 7320 696e 6372 656d 656e  upports incremen
-00001290: 7461 6c20 7379 6e63 2e20 496e 2074 6865  tal sync. In the
-000012a0: 2063 6f64 652c 2079 6f75 2063 616e 2073   code, you can s
-000012b0: 6565 2074 6865 2066 6f6c 6c6f 7769 6e67  ee the following
-000012c0: 206c 696e 653a 5c6e 5c6e 6069 6e63 7265   line:\n\n`incre
-000012d0: 6d65 6e74 616c 203a 3d20 636f 6c6c 6563  mental := collec
-000012e0: 746f 7257 6974 6853 7461 7465 2e49 7349  torWithState.IsI
-000012f0: 6e63 7265 6d65 6e74 616c 2829 605c 6e5c  ncremental()`\n\
-00001300: 6e54 6869 7320 6c69 6e65 2063 6865 636b  nThis line check
-00001310: 7320 6966 2074 6865 2063 6f6c 6c65 6374  s if the collect
-00001320: 6f72 2069 7320 7275 6e6e 696e 6720 696e  or is running in
-00001330: 2069 6e63 7265 6d65 6e74 616c 206d 6f64   incremental mod
-00001340: 652e 222c 0d0a 2020 2020 2020 2020 2020  e.",..          
-00001350: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
-00001360: 7469 6573 223a 205b 5d2c 0d0a 2020 2020  ties": [],..    
-00001370: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
-00001380: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00001390: 2020 2020 226c 6576 656c 223a 2022 6d69      "level": "mi
-000013a0: 6422 0d0a 2020 2020 2020 2020 2020 2020  d"..            
-000013b0: 7d0d 0a20 2020 2020 2020 207d 2c0d 0a20  }..        },.. 
-000013c0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-000013d0: 2020 2020 2020 2269 6422 3a20 2251 5244        "id": "QRD
-000013e0: 2d39 222c 0d0a 2020 2020 2020 2020 2020  -9",..          
-000013f0: 2020 2271 7565 7374 696f 6e22 3a20 2248    "question": "H
-00001400: 6f77 2063 616e 2049 2063 7265 6174 6520  ow can I create 
-00001410: 4465 764c 616b 6520 706c 7567 696e 7320  DevLake plugins 
-00001420: 696e 2050 7974 686f 6e3f 222c 0d0a 2020  in Python?",..  
-00001430: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
-00001440: 656e 6365 5f61 6e73 7765 7222 3a20 2254  ence_answer": "T
-00001450: 6f20 6372 6561 7465 2061 2044 6576 4c61  o create a DevLa
-00001460: 6b65 2070 6c75 6769 6e20 696e 2050 7974  ke plugin in Pyt
-00001470: 686f 6e2c 2066 6f6c 6c6f 7720 7468 6573  hon, follow thes
-00001480: 6520 7374 6570 733a 5c6e 5c6e 312e 204d  e steps:\n\n1. M
-00001490: 616b 6520 7375 7265 2079 6f75 2068 6176  ake sure you hav
-000014a0: 6520 5b50 6f65 7472 795d 2868 7474 7073  e [Poetry](https
-000014b0: 3a2f 2f70 7974 686f 6e2d 706f 6574 7279  ://python-poetry
-000014c0: 2e6f 7267 2f64 6f63 732f 2369 6e73 7461  .org/docs/#insta
-000014d0: 6c6c 6174 696f 6e29 2069 6e73 7461 6c6c  llation) install
-000014e0: 6564 2e5c 6e32 2e20 4d6f 7665 2074 6f20  ed.\n2. Move to 
-000014f0: 6070 7974 686f 6e2f 706c 7567 696e 7360  `python/plugins`
-00001500: 2061 6e64 2065 7865 6375 7465 2060 706f   and execute `po
-00001510: 6574 7279 206e 6577 206d 7970 6c75 6769  etry new myplugi
-00001520: 6e60 2e20 5468 6973 2077 696c 6c20 6765  n`. This will ge
-00001530: 6e65 7261 7465 2061 206e 6577 2064 6972  nerate a new dir
-00001540: 6563 746f 7279 2066 6f72 2079 6f75 7220  ectory for your 
-00001550: 706c 7567 696e 2e5c 6e33 2e20 496e 2074  plugin.\n3. In t
-00001560: 6865 2060 7079 7072 6f6a 6563 742e 746f  he `pyproject.to
-00001570: 6d6c 6020 6669 6c65 2c20 6164 6420 7468  ml` file, add th
-00001580: 6520 666f 6c6c 6f77 696e 6720 6c69 6e65  e following line
-00001590: 2061 7420 7468 6520 656e 6420 6f66 2074   at the end of t
-000015a0: 6865 2060 5b74 6f6f 6c2e 706f 6574 7279  he `[tool.poetry
-000015b0: 2e64 6570 656e 6465 6e63 6965 735d 6020  .dependencies]` 
-000015c0: 7365 6374 696f 6e3a 5c6e 6060 605c 6e70  section:\n```\np
-000015d0: 7964 6576 6c61 6b65 203d 207b 2070 6174  ydevlake = { pat
-000015e0: 6820 3d20 5c22 2e2e 2f2e 2e2f 7079 6465  h = \"../../pyde
-000015f0: 766c 616b 655c 222c 2064 6576 656c 6f70  vlake\", develop
-00001600: 203d 2074 7275 6520 7d5c 6e60 6060 5c6e   = true }\n```\n
-00001610: 342e 2052 756e 2060 706f 6574 7279 2069  4. Run `poetry i
-00001620: 6e73 7461 6c6c 602e 5c6e 352e 2043 7265  nstall`.\n5. Cre
-00001630: 6174 6520 6120 606d 6169 6e2e 7079 6020  ate a `main.py` 
-00001640: 6669 6c65 2077 6974 6820 7468 6520 6e65  file with the ne
-00001650: 6365 7373 6172 7920 636f 6e74 656e 742c  cessary content,
-00001660: 2069 6e63 6c75 6469 6e67 2063 6c61 7373   including class
-00001670: 6573 2066 6f72 2063 6f6e 6e65 6374 696f  es for connectio
-00001680: 6e2c 2074 7261 6e73 666f 726d 6174 696f  n, transformatio
-00001690: 6e20 7275 6c65 2c20 746f 6f6c 2073 636f  n rule, tool sco
-000016a0: 7065 2c20 616e 6420 706c 7567 696e 2e5c  pe, and plugin.\
-000016b0: 6e36 2e20 4372 6561 7465 2073 6865 6c6c  n6. Create shell
-000016c0: 2073 6372 6970 7473 2060 6275 696c 642e   scripts `build.
-000016d0: 7368 6020 616e 6420 6072 756e 2e73 6860  sh` and `run.sh`
-000016e0: 2069 6e20 7468 6520 706c 7567 696e 2072   in the plugin r
-000016f0: 6f6f 7420 6469 7265 6374 6f72 7920 746f  oot directory to
-00001700: 2062 7569 6c64 2061 6e64 2072 756e 2074   build and run t
-00001710: 6865 2070 6c75 6769 6e2e 5c6e 372e 2044  he plugin.\n7. D
-00001720: 6566 696e 6520 636f 6e6e 6563 7469 6f6e  efine connection
-00001730: 2070 6172 616d 6574 6572 732c 2074 7261   parameters, tra
-00001740: 6e73 666f 726d 6174 696f 6e20 7275 6c65  nsformation rule
-00001750: 2070 6172 616d 6574 6572 732c 2061 6e64   parameters, and
-00001760: 2074 6f6f 6c20 7363 6f70 6520 7479 7065   tool scope type
-00001770: 2e5c 6e38 2e20 496d 706c 656d 656e 7420  .\n8. Implement 
-00001780: 6d65 7468 6f64 7320 6c69 6b65 2060 646f  methods like `do
-00001790: 6d61 696e 5f73 636f 7065 7360 2c20 6072  main_scopes`, `r
-000017a0: 656d 6f74 655f 7363 6f70 6560 2c20 6072  emote_scope`, `r
-000017b0: 656d 6f74 655f 7363 6f70 655f 6772 6f75  emote_scope_grou
-000017c0: 7073 602c 2061 6e64 2060 7465 7374 5f63  ps`, and `test_c
-000017d0: 6f6e 6e65 6374 696f 6e60 2e5c 6e39 2e20  onnection`.\n9. 
-000017e0: 4164 6420 6120 6e65 7720 6461 7461 2073  Add a new data s
-000017f0: 7472 6561 6d20 6279 2063 7265 6174 696e  tream by creatin
-00001800: 6720 6120 746f 6f6c 206d 6f64 656c 2c20  g a tool model, 
-00001810: 7374 7265 616d 2063 6c61 7373 2c20 616e  stream class, an
-00001820: 6420 4150 4920 7772 6170 7065 722e 5c6e  d API wrapper.\n
-00001830: 3130 2e20 496d 706c 656d 656e 7420 6d65  10. Implement me
-00001840: 7468 6f64 7320 6c69 6b65 2060 636f 6c6c  thods like `coll
-00001850: 6563 7460 2c20 6065 7874 7261 6374 602c  ect`, `extract`,
-00001860: 2061 6e64 2060 636f 6e76 6572 7460 2066   and `convert` f
-00001870: 6f72 2074 6865 2073 7472 6561 6d20 636c  or the stream cl
-00001880: 6173 732e 5c6e 3131 2e20 4966 206e 6565  ass.\n11. If nee
-00001890: 6465 642c 2063 7265 6174 6520 7375 6273  ded, create subs
-000018a0: 7472 6561 6d73 2066 6f72 2068 6965 7261  treams for hiera
-000018b0: 7263 6869 6361 6c20 6461 7461 2073 6f75  rchical data sou
-000018c0: 7263 6573 2e5c 6e31 322e 2054 6573 7420  rces.\n12. Test 
-000018d0: 7468 6520 706c 7567 696e 2073 7461 6e64  the plugin stand
-000018e0: 616c 6f6e 6520 7573 696e 6720 7468 6520  alone using the 
-000018f0: 606d 6169 6e2e 7079 6020 6669 6c65 2077  `main.py` file w
-00001900: 6974 6820 6469 6666 6572 656e 7420 636f  ith different co
-00001910: 6d6d 616e 6473 2e5c 6e31 332e 2057 7269  mmands.\n13. Wri
-00001920: 7465 2075 6e69 742d 7465 7374 7320 666f  te unit-tests fo
-00001930: 7220 796f 7572 2070 6c75 6769 6e20 636f  r your plugin co
-00001940: 6465 2c20 7769 7468 2074 6573 7420 6669  de, with test fi
-00001950: 6c65 7320 656e 6469 6e67 2069 6e20 605f  les ending in `_
-00001960: 7465 7374 2e70 7960 2e5c 6e5c 6e48 6572  test.py`.\n\nHer
-00001970: 6527 7320 6120 6765 6e65 7261 6c20 6f75  e's a general ou
-00001980: 746c 696e 6520 6f66 2061 2044 6576 4c61  tline of a DevLa
-00001990: 6b65 2070 6c75 6769 6e20 636c 6173 733a  ke plugin class:
-000019a0: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e66  \n\n```python\nf
-000019b0: 726f 6d20 7079 6465 766c 616b 652e 706c  rom pydevlake.pl
-000019c0: 7567 696e 2069 6d70 6f72 7420 506c 7567  ugin import Plug
-000019d0: 696e 5c6e 5c6e 636c 6173 7320 4d79 4465  in\n\nclass MyDe
-000019e0: 764c 616b 6550 6c75 6769 6e28 506c 7567  vLakePlugin(Plug
-000019f0: 696e 293a 5c6e 2020 2020 2320 496d 706c  in):\n    # Impl
-00001a00: 656d 656e 7420 7265 7175 6972 6564 2070  ement required p
-00001a10: 726f 7065 7274 6965 7320 616e 6420 6d65  roperties and me
-00001a20: 7468 6f64 7320 6865 7265 5c6e 2020 2020  thods here\n    
-00001a30: 2320 652e 672e 2c20 6e61 6d65 2c20 6465  # e.g., name, de
-00001a40: 7363 7269 7074 696f 6e2c 2063 6f6e 6e65  scription, conne
-00001a50: 6374 696f 6e5f 7479 7065 2c20 746f 6f6c  ction_type, tool
-00001a60: 5f73 636f 7065 5f74 7970 652c 2074 7261  _scope_type, tra
-00001a70: 6e73 666f 726d 6174 696f 6e5f 7275 6c65  nsformation_rule
-00001a80: 5f74 7970 652c 2073 7472 6561 6d73 2c20  _type, streams, 
-00001a90: 6574 632e 5c6e 6060 605c 6e5c 6e59 6f75  etc.\n```\n\nYou
-00001aa0: 2077 6f75 6c64 2074 6865 6e20 6e65 6564   would then need
-00001ab0: 2074 6f20 696d 706c 656d 656e 7420 7468   to implement th
-00001ac0: 6520 7265 7175 6972 6564 2070 726f 7065  e required prope
-00001ad0: 7274 6965 7320 616e 6420 6d65 7468 6f64  rties and method
-00001ae0: 7320 666f 7220 796f 7572 2073 7065 6369  s for your speci
-00001af0: 6669 6320 706c 7567 696e 2c20 7375 6368  fic plugin, such
-00001b00: 2061 7320 606e 616d 6560 2c20 6064 6573   as `name`, `des
-00001b10: 6372 6970 7469 6f6e 602c 2060 636f 6e6e  cription`, `conn
-00001b20: 6563 7469 6f6e 5f74 7970 6560 2c20 6074  ection_type`, `t
-00001b30: 6f6f 6c5f 7363 6f70 655f 7479 7065 602c  ool_scope_type`,
-00001b40: 2060 7472 616e 7366 6f72 6d61 7469 6f6e   `transformation
-00001b50: 5f72 756c 655f 7479 7065 602c 2061 6e64  _rule_type`, and
-00001b60: 2060 7374 7265 616d 7360 2e20 596f 7520   `streams`. You 
-00001b70: 6361 6e20 7265 6665 7220 746f 2074 6865  can refer to the
-00001b80: 2070 726f 7669 6465 6420 636f 6465 2773   provided code's
-00001b90: 2074 6573 7420 6675 6e63 7469 6f6e 7320   test functions 
-00001ba0: 2865 2e67 2e2c 2060 6173 7365 7274 5f76  (e.g., `assert_v
-00001bb0: 616c 6964 5f6e 616d 6560 2c20 6061 7373  alid_name`, `ass
-00001bc0: 6572 745f 7661 6c69 645f 6465 7363 7269  ert_valid_descri
-00001bd0: 7074 696f 6e60 2c20 6061 7373 6572 745f  ption`, `assert_
-00001be0: 7661 6c69 645f 636f 6e6e 6563 7469 6f6e  valid_connection
-00001bf0: 5f74 7970 6560 2c20 6574 632e 2920 746f  _type`, etc.) to
-00001c00: 2075 6e64 6572 7374 616e 6420 7468 6520   understand the 
-00001c10: 7265 7175 6972 656d 656e 7473 2061 6e64  requirements and
-00001c20: 2063 6f6e 7374 7261 696e 7473 2066 6f72   constraints for
-00001c30: 2065 6163 6820 7072 6f70 6572 7479 2061   each property a
-00001c40: 6e64 206d 6574 686f 642e 5c6e 5c6e 4f6e  nd method.\n\nOn
-00001c50: 6365 2079 6f75 2068 6176 6520 696d 706c  ce you have impl
-00001c60: 656d 656e 7465 6420 796f 7572 2070 6c75  emented your plu
-00001c70: 6769 6e2c 2079 6f75 2063 616e 2075 7365  gin, you can use
-00001c80: 2074 6865 2070 726f 7669 6465 6420 7465   the provided te
-00001c90: 7374 2066 756e 6374 696f 6e73 2074 6f20  st functions to 
-00001ca0: 7661 6c69 6461 7465 2079 6f75 7220 706c  validate your pl
-00001cb0: 7567 696e 2061 6e64 2065 6e73 7572 6520  ugin and ensure 
-00001cc0: 6974 2077 6f72 6b73 2063 6f72 7265 6374  it works correct
-00001cd0: 6c79 2e22 2c0d 0a20 2020 2020 2020 2020  ly.",..         
-00001ce0: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
-00001cf0: 7274 6965 7322 3a20 5b5d 2c0d 0a20 2020  rties": [],..   
-00001d00: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
-00001d10: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00001d20: 2020 2020 2022 6c65 7665 6c22 3a20 226c       "level": "l
-00001d30: 6f77 220d 0a20 2020 2020 2020 2020 2020  ow"..           
-00001d40: 207d 0d0a 2020 2020 2020 2020 7d2c 0d0a   }..        },..
-00001d50: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00001d60: 2020 2020 2020 2022 6964 223a 2022 5152         "id": "QR
-00001d70: 442d 3130 222c 0d0a 2020 2020 2020 2020  D-10",..        
-00001d80: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
-00001d90: 2248 6f77 2064 6f20 4920 7265 736f 6c76  "How do I resolv
-00001da0: 6520 7468 6520 2770 616e 6963 3a20 696e  e the 'panic: in
-00001db0: 7661 6c69 6420 656e 634b 6579 2720 6572  valid encKey' er
-00001dc0: 726f 723f 222c 0d0a 2020 2020 2020 2020  ror?",..        
-00001dd0: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
-00001de0: 6e73 7765 7222 3a20 2254 6f20 7265 736f  nswer": "To reso
-00001df0: 6c76 6520 7468 6520 2770 616e 6963 3a20  lve the 'panic: 
-00001e00: 696e 7661 6c69 6420 656e 634b 6579 2720  invalid encKey' 
-00001e10: 6572 726f 722c 2079 6f75 206e 6565 6420  error, you need 
-00001e20: 746f 2065 6e73 7572 6520 7468 6174 2079  to ensure that y
-00001e30: 6f75 2068 6176 6520 6120 7661 6c69 6420  ou have a valid 
-00001e40: 656e 6372 7970 7469 6f6e 206b 6579 2073  encryption key s
-00001e50: 6574 2069 6e20 796f 7572 2065 6e76 6972  et in your envir
-00001e60: 6f6e 6d65 6e74 206f 7220 636f 6e66 6967  onment or config
-00001e70: 7572 6174 696f 6e2e 2048 6572 6520 6172  uration. Here ar
-00001e80: 6520 736f 6d65 2073 7465 7073 2079 6f75  e some steps you
-00001e90: 2063 616e 2066 6f6c 6c6f 773a 5c6e 5c6e   can follow:\n\n
-00001ea0: 312e 204d 616b 6520 7375 7265 2079 6f75  1. Make sure you
-00001eb0: 2068 6176 6520 6120 7661 6c69 6420 656e   have a valid en
-00001ec0: 6372 7970 7469 6f6e 206b 6579 2061 6e64  cryption key and
-00001ed0: 2069 7427 7320 6265 696e 6720 636f 7272   it's being corr
-00001ee0: 6563 746c 7920 6665 7463 6865 6420 7573  ectly fetched us
-00001ef0: 696e 6720 7468 6520 6070 6c75 6769 6e2e  ing the `plugin.
-00001f00: 456e 636f 6465 4b65 7945 6e76 5374 7260  EncodeKeyEnvStr`
-00001f10: 2063 6f6e 7374 616e 7420 6f72 2061 2073   constant or a s
-00001f20: 696d 696c 6172 206d 6574 686f 6420 696e  imilar method in
-00001f30: 2079 6f75 7220 636f 6465 2e5c 6e32 2e20   your code.\n2. 
-00001f40: 4966 2079 6f75 2061 7265 2075 7369 6e67  If you are using
-00001f50: 2061 2072 616e 646f 6d6c 7920 6765 6e65   a randomly gene
-00001f60: 7261 7465 6420 656e 6372 7970 7469 6f6e  rated encryption
-00001f70: 206b 6579 2c20 6d61 6b65 2073 7572 6520   key, make sure 
-00001f80: 746f 2073 746f 7265 2069 7420 7365 6375  to store it secu
-00001f90: 7265 6c79 2061 6e64 2075 7365 2074 6865  rely and use the
-00001fa0: 2073 616d 6520 6b65 7920 666f 7220 626f   same key for bo
-00001fb0: 7468 2065 6e63 7279 7074 696f 6e20 616e  th encryption an
-00001fc0: 6420 6465 6372 7970 7469 6f6e 2070 726f  d decryption pro
-00001fd0: 6365 7373 6573 2e5c 6e33 2e20 4368 6563  cesses.\n3. Chec
-00001fe0: 6b20 7468 6174 2074 6865 2065 6e76 6972  k that the envir
-00001ff0: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
-00002000: 7370 6563 6966 6965 6420 6279 2060 706c  specified by `pl
-00002010: 7567 696e 2e45 6e63 6f64 654b 6579 456e  ugin.EncodeKeyEn
-00002020: 7653 7472 6020 6f72 2061 2073 696d 696c  vStr` or a simil
-00002030: 6172 206d 6574 686f 6420 6973 2073 6574  ar method is set
-00002040: 2077 6974 6820 6120 7661 6c69 6420 656e   with a valid en
-00002050: 6372 7970 7469 6f6e 206b 6579 2e5c 6e34  cryption key.\n4
-00002060: 2e20 5665 7269 6679 2074 6861 7420 7468  . Verify that th
-00002070: 6520 656e 634b 6579 2069 7320 6265 696e  e encKey is bein
-00002080: 6720 7365 7420 616e 6420 7361 7665 6420  g set and saved 
-00002090: 746f 2074 6865 2063 6f6e 6669 6720 7072  to the config pr
-000020a0: 6f70 6572 6c79 2075 7369 6e67 2060 762e  operly using `v.
-000020b0: 5365 7428 706c 7567 696e 2e45 6e63 6f64  Set(plugin.Encod
-000020c0: 654b 6579 456e 7653 7472 2c20 656e 634b  eKeyEnvStr, encK
-000020d0: 6579 2960 2061 6e64 2060 636f 6e66 6967  ey)` and `config
-000020e0: 2e57 7269 7465 436f 6e66 6967 2876 2960  .WriteConfig(v)`
-000020f0: 206f 7220 7369 6d69 6c61 7220 6d65 7468   or similar meth
-00002100: 6f64 7320 696e 2079 6f75 7220 636f 6465  ods in your code
-00002110: 2e5c 6e5c 6e49 6620 7468 6520 6973 7375  .\n\nIf the issu
-00002120: 6520 7065 7273 6973 7473 2c20 796f 7520  e persists, you 
-00002130: 6d61 7920 6e65 6564 2074 6f20 7072 6f76  may need to prov
-00002140: 6964 6520 6d6f 7265 2063 6f6e 7465 7874  ide more context
-00002150: 206f 7220 7265 6665 7220 746f 2074 6865   or refer to the
-00002160: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
-00002170: 6620 7468 6520 7370 6563 6966 6963 2073  f the specific s
-00002180: 6f66 7477 6172 6520 796f 7520 6172 6520  oftware you are 
-00002190: 776f 726b 696e 6720 7769 7468 2e22 2c0d  working with.",.
-000021a0: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
-000021b0: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
-000021c0: 3a20 5b5d 2c0d 0a20 2020 2020 2020 2020  : [],..         
-000021d0: 2020 2022 6e6f 7465 7322 3a20 7b0d 0a20     "notes": {.. 
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000021f0: 6c65 7665 6c22 3a20 226d 6964 220d 0a20  level": "mid".. 
-00002200: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00002210: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00002220: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00002230: 2022 6964 223a 2022 5152 442d 3131 222c   "id": "QRD-11",
-00002240: 0d0a 2020 2020 2020 2020 2020 2020 2271  ..            "q
-00002250: 7565 7374 696f 6e22 3a20 2248 6f77 2064  uestion": "How d
-00002260: 6f65 7320 4465 764c 616b 6520 6765 6e65  oes DevLake gene
-00002270: 7261 7465 2061 2070 6970 656c 696e 6520  rate a pipeline 
-00002280: 6261 7365 6420 6f6e 2061 2062 6c75 6570  based on a bluep
-00002290: 7269 6e74 2773 2073 6574 7469 6e67 3f22  rint's setting?"
-000022a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000022b0: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
-000022c0: 223a 2022 4465 764c 616b 6520 6765 6e65  ": "DevLake gene
-000022d0: 7261 7465 7320 6120 7069 7065 6c69 6e65  rates a pipeline
-000022e0: 2062 6173 6564 206f 6e20 6120 626c 7565   based on a blue
-000022f0: 7072 696e 7427 7320 7365 7474 696e 6720  print's setting 
-00002300: 7468 726f 7567 6820 7468 6520 666f 6c6c  through the foll
-00002310: 6f77 696e 6720 7374 6570 733a 5c6e 5c6e  owing steps:\n\n
-00002320: 312e 2054 6865 2062 6c75 6570 7269 6e74  1. The blueprint
-00002330: 2073 6574 7469 6e67 7320 6172 6520 6465   settings are de
-00002340: 6669 6e65 6420 696e 2061 204a 534f 4e20  fined in a JSON 
-00002350: 666f 726d 6174 2c20 7768 6963 6820 696e  format, which in
-00002360: 636c 7564 6573 2074 6865 2076 6572 7369  cludes the versi
-00002370: 6f6e 2c20 636f 6e6e 6563 7469 6f6e 732c  on, connections,
-00002380: 2070 6c75 6769 6e2c 2063 6f6e 6e65 6374   plugin, connect
-00002390: 696f 6e49 642c 2061 6e64 2073 636f 7065  ionId, and scope
-000023a0: 732e 5c6e 5c6e 322e 2054 6865 2060 506c  s.\n\n2. The `Pl
-000023b0: 7567 696e 426c 7565 7072 696e 7456 3230  uginBlueprintV20
-000023c0: 302e 4d61 6b65 5069 7065 6c69 6e65 506c  0.MakePipelinePl
-000023d0: 616e 6020 6675 6e63 7469 6f6e 2069 7320  an` function is 
-000023e0: 6361 6c6c 6564 2077 6974 6820 616e 2061  called with an a
-000023f0: 7272 6179 206f 6620 7363 6f70 6573 2e20  rray of scopes. 
-00002400: 5468 6520 706c 7567 696e 2072 6574 7572  The plugin retur
-00002410: 6e73 2061 2060 5069 7065 6c69 6e65 506c  ns a `PipelinePl
-00002420: 616e 6020 696e 204a 534f 4e20 666f 726d  an` in JSON form
-00002430: 6174 2061 6e64 2061 6e20 6172 7261 7920  at and an array 
-00002440: 6f66 2060 5363 6f70 6560 2066 6f72 2070  of `Scope` for p
-00002450: 726f 6a65 6374 5f6d 6170 7069 6e67 2e5c  roject_mapping.\
-00002460: 6e5c 6e33 2e20 5468 6520 6672 616d 6577  n\n3. The framew
-00002470: 6f72 6b20 6d61 696e 7461 696e 7320 7468  ork maintains th
-00002480: 6520 7072 6f6a 6563 745f 6d61 7070 696e  e project_mappin
-00002490: 6720 7461 626c 6520 6261 7365 6420 6f6e  g table based on
-000024a0: 2074 6865 2060 5b5d 5363 6f70 6560 2061   the `[]Scope` a
-000024b0: 7272 6179 2e5c 6e5c 6e54 6865 7365 2073  rray.\n\nThese s
-000024c0: 7465 7073 2068 656c 7020 4465 764c 616b  teps help DevLak
-000024d0: 6520 6765 6e65 7261 7465 2061 2070 6970  e generate a pip
-000024e0: 656c 696e 6520 706c 616e 2062 6173 6564  eline plan based
-000024f0: 206f 6e20 7468 6520 626c 7565 7072 696e   on the blueprin
-00002500: 7427 7320 7365 7474 696e 6773 2c20 7768  t's settings, wh
-00002510: 6963 6820 6361 6e20 6265 2075 7365 6420  ich can be used 
-00002520: 746f 2065 7865 6375 7465 2074 6865 2070  to execute the p
-00002530: 6970 656c 696e 6520 616e 6420 636f 6c6c  ipeline and coll
-00002540: 6563 7420 6461 7461 2066 726f 6d20 7661  ect data from va
-00002550: 7269 6f75 7320 736f 7572 6365 732e 222c  rious sources.",
-00002560: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-00002570: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-00002580: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-00002590: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025b0: 226c 6576 656c 223a 2022 6c6f 7722 0d0a  "level": "low"..
-000025c0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-000025d0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000025e0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000025f0: 2020 2269 6422 3a20 2251 5244 2d31 3222    "id": "QRD-12"
-00002600: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002610: 7175 6573 7469 6f6e 223a 2022 486f 7720  question": "How 
-00002620: 646f 6573 2044 6576 4c61 6b65 2064 656c  does DevLake del
-00002630: 6574 6520 6120 7072 6f6a 6563 743f 222c  ete a project?",
-00002640: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00002650: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-00002660: 3a20 2244 6576 4c61 6b65 2064 656c 6574  : "DevLake delet
-00002670: 6573 2061 2070 726f 6a65 6374 2062 7920  es a project by 
-00002680: 666f 6c6c 6f77 696e 6720 7468 6573 6520  following these 
-00002690: 7374 6570 733a 5c6e 5c6e 312e 2056 6572  steps:\n\n1. Ver
-000026a0: 6966 7920 7468 6520 696e 7075 7420 7072  ify the input pr
-000026b0: 6f6a 6563 7420 6e61 6d65 2069 7320 6e6f  oject name is no
-000026c0: 7420 656d 7074 792e 5c6e 322e 2042 6567  t empty.\n2. Beg
-000026d0: 696e 2061 2064 6174 6162 6173 6520 7472  in a database tr
-000026e0: 616e 7361 6374 696f 6e2e 5c6e 332e 2047  ansaction.\n3. G
-000026f0: 6574 2074 6865 2070 726f 6a65 6374 2062  et the project b
-00002700: 7920 6974 7320 6e61 6d65 2075 7369 6e67  y its name using
-00002710: 2074 6865 2060 6765 7450 726f 6a65 6374   the `getProject
-00002720: 4279 4e61 6d65 6020 6675 6e63 7469 6f6e  ByName` function
-00002730: 2e5c 6e34 2e20 4465 6c65 7465 2074 6865  .\n4. Delete the
-00002740: 2070 726f 6a65 6374 2066 726f 6d20 7468   project from th
-00002750: 6520 606d 6f64 656c 732e 5072 6f6a 6563  e `models.Projec
-00002760: 7460 2074 6162 6c65 2075 7369 6e67 2074  t` table using t
-00002770: 6865 2070 726f 6a65 6374 206e 616d 652e  he project name.
-00002780: 5c6e 352e 2044 656c 6574 6520 7468 6520  \n5. Delete the 
-00002790: 7072 6f6a 6563 7420 6d61 7070 696e 6720  project mapping 
-000027a0: 6672 6f6d 2074 6865 2060 6372 6f73 7364  from the `crossd
-000027b0: 6f6d 6169 6e2e 5072 6f6a 6563 744d 6170  omain.ProjectMap
-000027c0: 7069 6e67 6020 7461 626c 6520 7573 696e  ping` table usin
-000027d0: 6720 7468 6520 7072 6f6a 6563 7420 6e61  g the project na
-000027e0: 6d65 2e5c 6e36 2e20 4465 6c65 7465 2074  me.\n6. Delete t
-000027f0: 6865 2070 726f 6a65 6374 206d 6574 7269  he project metri
-00002800: 6320 7365 7474 696e 6720 6672 6f6d 2074  c setting from t
-00002810: 6865 2060 6d6f 6465 6c73 2e50 726f 6a65  he `models.Proje
-00002820: 6374 4d65 7472 6963 5365 7474 696e 6760  ctMetricSetting`
-00002830: 2074 6162 6c65 2075 7369 6e67 2074 6865   table using the
-00002840: 2070 726f 6a65 6374 206e 616d 652e 5c6e   project name.\n
-00002850: 372e 2044 656c 6574 6520 7468 6520 7072  7. Delete the pr
-00002860: 6f6a 6563 7420 5052 206d 6574 7269 6320  oject PR metric 
-00002870: 6672 6f6d 2074 6865 2060 6372 6f73 7364  from the `crossd
-00002880: 6f6d 6169 6e2e 5072 6f6a 6563 7450 724d  omain.ProjectPrM
-00002890: 6574 7269 6360 2074 6162 6c65 2075 7369  etric` table usi
-000028a0: 6e67 2074 6865 2070 726f 6a65 6374 206e  ng the project n
-000028b0: 616d 652e 5c6e 382e 2044 656c 6574 6520  ame.\n8. Delete 
-000028c0: 7468 6520 7072 6f6a 6563 7420 6973 7375  the project issu
-000028d0: 6520 6d65 7472 6963 2066 726f 6d20 7468  e metric from th
-000028e0: 6520 6063 726f 7373 646f 6d61 696e 2e50  e `crossdomain.P
-000028f0: 726f 6a65 6374 4973 7375 654d 6574 7269  rojectIssueMetri
-00002900: 6360 2074 6162 6c65 2075 7369 6e67 2074  c` table using t
-00002910: 6865 2070 726f 6a65 6374 206e 616d 652e  he project name.
-00002920: 5c6e 392e 2043 6f6d 6d69 7420 7468 6520  \n9. Commit the 
-00002930: 7472 616e 7361 6374 696f 6e2e 5c6e 3130  transaction.\n10
-00002940: 2e20 4765 7420 7468 6520 626c 7565 7072  . Get the bluepr
-00002950: 696e 7420 6173 736f 6369 6174 6564 2077  int associated w
-00002960: 6974 6820 7468 6520 7072 6f6a 6563 7420  ith the project 
-00002970: 6e61 6d65 2075 7369 6e67 2074 6865 2060  name using the `
-00002980: 6270 4d61 6e61 6765 722e 4765 7444 6242  bpManager.GetDbB
-00002990: 6c75 6570 7269 6e74 4279 5072 6f6a 6563  lueprintByProjec
-000029a0: 744e 616d 6560 2066 756e 6374 696f 6e2e  tName` function.
-000029b0: 5c6e 3131 2e20 4465 6c65 7465 2074 6865  \n11. Delete the
-000029c0: 2062 6c75 6570 7269 6e74 2075 7369 6e67   blueprint using
-000029d0: 2074 6865 2060 6270 4d61 6e61 6765 722e   the `bpManager.
-000029e0: 4465 6c65 7465 426c 7565 7072 696e 7460  DeleteBlueprint`
-000029f0: 2066 756e 6374 696f 6e20 7769 7468 2074   function with t
-00002a00: 6865 2062 6c75 6570 7269 6e74 2049 442e  he blueprint ID.
-00002a10: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002a20: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
-00002a30: 6573 223a 205b 5d2c 0d0a 2020 2020 2020  es": [],..      
-00002a40: 2020 2020 2020 226e 6f74 6573 223a 207b        "notes": {
-00002a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002a60: 2020 226c 6576 656c 223a 2022 6869 6768    "level": "high
-00002a70: 220d 0a20 2020 2020 2020 2020 2020 207d  "..            }
-00002a80: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-00002a90: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00002aa0: 2020 2020 2022 6964 223a 2022 5152 442d       "id": "QRD-
-00002ab0: 3133 222c 0d0a 2020 2020 2020 2020 2020  13",..          
-00002ac0: 2020 2271 7565 7374 696f 6e22 3a20 2248    "question": "H
-00002ad0: 6f77 2064 6f65 7320 4465 764c 616b 6520  ow does DevLake 
-00002ae0: 6765 6e65 7261 7465 2074 6865 2074 656d  generate the tem
-00002af0: 706c 6174 6520 7573 6572 5f61 6363 6f75  plate user_accou
-00002b00: 6e74 5f6d 6170 7069 6e67 2e63 7376 2066  nt_mapping.csv f
-00002b10: 696c 653f 222c 0d0a 2020 2020 2020 2020  ile?",..        
-00002b20: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
-00002b30: 6e73 7765 7222 3a20 2244 6576 4c61 6b65  nswer": "DevLake
-00002b40: 2067 656e 6572 6174 6573 2074 6865 2074   generates the t
-00002b50: 656d 706c 6174 6520 7573 6572 5f61 6363  emplate user_acc
-00002b60: 6f75 6e74 5f6d 6170 7069 6e67 2e63 7376  ount_mapping.csv
-00002b70: 2066 696c 6520 7573 696e 6720 7468 6520   file using the 
-00002b80: 4765 7455 7365 7241 6363 6f75 6e74 4d61  GetUserAccountMa
-00002b90: 7070 696e 6720 6675 6e63 7469 6f6e 2e20  pping function. 
-00002ba0: 5468 6973 2066 756e 6374 696f 6e20 7265  This function re
-00002bb0: 7472 6965 7665 7320 616c 6c20 7573 6572  trieves all user
-00002bc0: 2f61 6363 6f75 6e74 206d 6170 7069 6e67  /account mapping
-00002bd0: 7320 6672 6f6d 2074 6865 2073 746f 7265  s from the store
-00002be0: 2c20 6d61 7273 6861 6c73 2074 6865 6d20  , marshals them 
-00002bf0: 696e 746f 2043 5356 2066 6f72 6d61 7420  into CSV format 
-00002c00: 7573 696e 6720 676f 6373 762e 4d61 7273  using gocsv.Mars
-00002c10: 6861 6c42 7974 6573 2861 6363 6f75 6e74  halBytes(account
-00002c20: 7329 2c20 616e 6420 7265 7475 726e 7320  s), and returns 
-00002c30: 7468 6520 4353 5620 6461 7461 2061 7320  the CSV data as 
-00002c40: 616e 204f 7574 7075 7446 696c 6520 7769  an OutputFile wi
-00002c50: 7468 2043 6f6e 7465 6e74 5479 7065 205c  th ContentType \
-00002c60: 2274 6578 742f 6373 765c 222e 222c 0d0a  "text/csv\".",..
-00002c70: 2020 2020 2020 2020 2020 2020 2261 6e73              "ans
-00002c80: 7765 725f 7072 6f70 6572 7469 6573 223a  wer_properties":
-00002c90: 205b 5d2c 0d0a 2020 2020 2020 2020 2020   [],..          
-00002ca0: 2020 226e 6f74 6573 223a 207b 0d0a 2020    "notes": {..  
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00002cc0: 6576 656c 223a 2022 6d69 6422 0d0a 2020  evel": "mid"..  
-00002cd0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00002ce0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00002cf0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00002d00: 2269 6422 3a20 2251 5244 2d31 3522 2c0d  "id": "QRD-15",.
-00002d10: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
-00002d20: 6573 7469 6f6e 223a 2022 486f 7720 6973  estion": "How is
-00002d30: 2074 6865 2068 2e73 746f 7265 2e66 696e   the h.store.fin
-00002d40: 6441 6c6c 4163 636f 756e 7473 2066 756e  dAllAccounts fun
-00002d50: 6374 696f 6e20 696d 706c 656d 656e 7465  ction implemente
-00002d60: 643f 222c 0d0a 2020 2020 2020 2020 2020  d?",..          
-00002d70: 2020 2272 6566 6572 656e 6365 5f61 6e73    "reference_ans
-00002d80: 7765 7222 3a20 2254 6865 2068 2e73 746f  wer": "The h.sto
-00002d90: 7265 2e66 696e 6441 6c6c 4163 636f 756e  re.findAllAccoun
-00002da0: 7473 2066 756e 6374 696f 6e20 6973 2069  ts function is i
-00002db0: 6d70 6c65 6d65 6e74 6564 2061 7320 666f  mplemented as fo
-00002dc0: 6c6c 6f77 733a 5c6e 5c6e 6060 6067 6f5c  llows:\n\n```go\
-00002dd0: 6e66 756e 6320 2864 202a 6462 5374 6f72  nfunc (d *dbStor
-00002de0: 6529 2066 696e 6441 6c6c 4163 636f 756e  e) findAllAccoun
-00002df0: 7473 2829 2028 5b5d 6163 636f 756e 742c  ts() ([]account,
-00002e00: 2065 7272 6f72 732e 4572 726f 7229 207b   errors.Error) {
-00002e10: 5c6e 5c74 7661 7220 6161 205b 5d63 726f  \n\tvar aa []cro
-00002e20: 7373 646f 6d61 696e 2e41 6363 6f75 6e74  ssdomain.Account
-00002e30: 5c6e 5c74 6572 7220 3a3d 2064 2e64 622e  \n\terr := d.db.
-00002e40: 416c 6c28 2661 6129 5c6e 5c74 6966 2065  All(&aa)\n\tif e
-00002e50: 7272 2021 3d20 6e69 6c20 7b5c 6e5c 745c  rr != nil {\n\t\
-00002e60: 7472 6574 7572 6e20 6e69 6c2c 2065 7272  treturn nil, err
-00002e70: 5c6e 5c74 7d5c 6e5c 7476 6172 2075 6120  \n\t}\n\tvar ua 
-00002e80: 5b5d 6372 6f73 7364 6f6d 6169 6e2e 5573  []crossdomain.Us
-00002e90: 6572 4163 636f 756e 745c 6e5c 7465 7272  erAccount\n\terr
-00002ea0: 203d 2064 2e64 622e 416c 6c28 2675 6129   = d.db.All(&ua)
-00002eb0: 5c6e 5c74 6966 2065 7272 2021 3d20 6e69  \n\tif err != ni
-00002ec0: 6c20 7b5c 6e5c 745c 7472 6574 7572 6e20  l {\n\t\treturn 
-00002ed0: 6e69 6c2c 2065 7272 5c6e 5c74 7d5c 6e5c  nil, err\n\t}\n\
-00002ee0: 7476 6172 2061 202a 6163 636f 756e 745c  tvar a *account\
-00002ef0: 6e5c 7472 6574 7572 6e20 612e 6672 6f6d  n\treturn a.from
-00002f00: 446f 6d61 696e 4c61 7965 7228 6161 2c20  DomainLayer(aa, 
-00002f10: 7561 292c 206e 696c 5c6e 7d5c 6e60 6060  ua), nil\n}\n```
-00002f20: 5c6e 5c6e 4974 2072 6574 7269 6576 6573  \n\nIt retrieves
-00002f30: 2061 6c6c 2061 6363 6f75 6e74 7320 616e   all accounts an
-00002f40: 6420 7573 6572 2061 6363 6f75 6e74 7320  d user accounts 
-00002f50: 6672 6f6d 2074 6865 2064 6174 6162 6173  from the databas
-00002f60: 652c 2061 6e64 2074 6865 6e20 6361 6c6c  e, and then call
-00002f70: 7320 7468 6520 6672 6f6d 446f 6d61 696e  s the fromDomain
-00002f80: 4c61 7965 7220 6675 6e63 7469 6f6e 2074  Layer function t
-00002f90: 6f20 636f 6e76 6572 7420 7468 656d 2069  o convert them i
-00002fa0: 6e74 6f20 7468 6520 6170 7072 6f70 7269  nto the appropri
-00002fb0: 6174 6520 666f 726d 6174 2e22 2c0d 0a20  ate format.",.. 
-00002fc0: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
-00002fd0: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
-00002fe0: 5b5d 2c0d 0a20 2020 2020 2020 2020 2020  [],..           
-00002ff0: 2022 6e6f 7465 7322 3a20 7b0d 0a20 2020   "notes": {..   
-00003000: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
-00003010: 7665 6c22 3a20 226c 6f77 220d 0a20 2020  vel": "low"..   
-00003020: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00003030: 2020 2020 7d0d 0a20 2020 205d 0d0a 7d        }..    ]..}
+00000000: 7b0a 2020 2020 226e 616d 6522 3a20 2244  {.    "name": "D
+00000010: 6576 4c61 6b65 2052 6570 6f20 5175 6573  evLake Repo Ques
+00000020: 7469 6f6e 7322 2c0a 2020 2020 2264 6573  tions",.    "des
+00000030: 6372 6970 7469 6f6e 223a 2022 5468 6573  cription": "Thes
+00000040: 6520 7175 6573 7469 6f6e 7320 636f 6d65  e questions come
+00000050: 2066 726f 6d20 6465 766c 616b 655f 7265   from devlake_re
+00000060: 706f 5f71 7565 7374 696f 6e73 2e6a 736f  po_questions.jso
+00000070: 6e20 2877 6974 686f 7574 2044 5251 2d33  n (without DRQ-3
+00000080: 2c20 352c 2036 2c20 3134 2c20 3136 292e  , 5, 6, 14, 16).
+00000090: 222c 0a20 2020 2022 6361 7365 7322 3a20  ",.    "cases": 
+000000a0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+000000b0: 2020 2020 2020 2020 2269 6422 3a20 2244          "id": "D
+000000c0: 5251 2d31 222c 0a20 2020 2020 2020 2020  RQ-1",.         
+000000d0: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
+000000e0: 486f 7720 6973 2074 6865 206c 6561 6420  How is the lead 
+000000f0: 7469 6d65 2066 6f72 2063 6861 6e67 6573  time for changes
+00000100: 2063 616c 6375 6c61 7465 643f 222c 0a20   calculated?",. 
+00000110: 2020 2020 2020 2020 2020 2022 7265 6665             "refe
+00000120: 7265 6e63 655f 616e 7377 6572 223a 2022  rence_answer": "
+00000130: 5468 6520 6c65 6164 2074 696d 6520 666f  The lead time fo
+00000140: 7220 6368 616e 6765 7320 6973 2063 616c  r changes is cal
+00000150: 6375 6c61 7465 6420 696e 2074 6865 2060  culated in the `
+00000160: 4361 6c63 756c 6174 6543 6861 6e67 654c  CalculateChangeL
+00000170: 6561 6454 696d 6560 2066 756e 6374 696f  eadTime` functio
+00000180: 6e20 6279 2066 6f6c 6c6f 7769 6e67 2074  n by following t
+00000190: 6865 7365 2073 7465 7073 3a5c 6e5c 6e31  hese steps:\n\n1
+000001a0: 2e20 4765 7420 7075 6c6c 2072 6571 7565  . Get pull reque
+000001b0: 7374 7320 6279 2074 6865 2070 726f 6a65  sts by the proje
+000001c0: 6374 206e 616d 652e 5c6e 322e 2046 6f72  ct name.\n2. For
+000001d0: 2065 6163 6820 7075 6c6c 2072 6571 7565   each pull reque
+000001e0: 7374 2c20 6765 7420 7468 6520 6669 7273  st, get the firs
+000001f0: 7420 636f 6d6d 6974 2061 6e64 2063 616c  t commit and cal
+00000200: 6375 6c61 7465 2074 6865 2050 5220 636f  culate the PR co
+00000210: 6469 6e67 2074 696d 6520 6173 2074 6865  ding time as the
+00000220: 2074 696d 6520 7370 616e 2062 6574 7765   time span betwe
+00000230: 656e 2074 6865 2066 6972 7374 2063 6f6d  en the first com
+00000240: 6d69 7427 7320 6175 7468 6f72 6564 2064  mit's authored d
+00000250: 6174 6520 616e 6420 7468 6520 7075 6c6c  ate and the pull
+00000260: 2072 6571 7565 7374 2773 2063 7265 6174   request's creat
+00000270: 6564 2064 6174 652e 5c6e 332e 2047 6574  ed date.\n3. Get
+00000280: 2074 6865 2066 6972 7374 2072 6576 6965   the first revie
+00000290: 7720 666f 7220 7468 6520 7075 6c6c 2072  w for the pull r
+000002a0: 6571 7565 7374 2028 6578 636c 7564 696e  equest (excludin
+000002b0: 6720 636f 6d6d 656e 7473 2066 726f 6d20  g comments from 
+000002c0: 7468 6520 5052 2063 7265 6174 6f72 2920  the PR creator) 
+000002d0: 616e 6420 6361 6c63 756c 6174 6520 7468  and calculate th
+000002e0: 6520 5052 2070 6963 6b75 7020 7469 6d65  e PR pickup time
+000002f0: 2061 7320 7468 6520 7469 6d65 2073 7061   as the time spa
+00000300: 6e20 6265 7477 6565 6e20 7468 6520 7075  n between the pu
+00000310: 6c6c 2072 6571 7565 7374 2773 2063 7265  ll request's cre
+00000320: 6174 6564 2064 6174 6520 616e 6420 7468  ated date and th
+00000330: 6520 6669 7273 7420 7265 7669 6577 2773  e first review's
+00000340: 2063 7265 6174 6564 2064 6174 652e 2043   created date. C
+00000350: 616c 6375 6c61 7465 2074 6865 2050 5220  alculate the PR 
+00000360: 7265 7669 6577 2074 696d 6520 6173 2074  review time as t
+00000370: 6865 2074 696d 6520 7370 616e 2062 6574  he time span bet
+00000380: 7765 656e 2074 6865 2066 6972 7374 2072  ween the first r
+00000390: 6576 6965 7727 7320 6372 6561 7465 6420  eview's created 
+000003a0: 6461 7465 2061 6e64 2074 6865 2070 756c  date and the pul
+000003b0: 6c20 7265 7175 6573 7427 7320 6d65 7267  l request's merg
+000003c0: 6564 2064 6174 652e 5c6e 342e 2047 6574  ed date.\n4. Get
+000003d0: 2074 6865 2064 6570 6c6f 796d 656e 7420   the deployment 
+000003e0: 666f 7220 7468 6520 7075 6c6c 2072 6571  for the pull req
+000003f0: 7565 7374 2075 7369 6e67 2074 6865 206d  uest using the m
+00000400: 6572 6765 2063 6f6d 6d69 7420 5348 4120  erge commit SHA 
+00000410: 616e 6420 6361 6c63 756c 6174 6520 7468  and calculate th
+00000420: 6520 5052 2064 6570 6c6f 7920 7469 6d65  e PR deploy time
+00000430: 2061 7320 7468 6520 7469 6d65 2073 7061   as the time spa
+00000440: 6e20 6265 7477 6565 6e20 7468 6520 7075  n between the pu
+00000450: 6c6c 2072 6571 7565 7374 2773 206d 6572  ll request's mer
+00000460: 6765 6420 6461 7465 2061 6e64 2074 6865  ged date and the
+00000470: 2064 6570 6c6f 796d 656e 7427 7320 6669   deployment's fi
+00000480: 6e69 7368 6564 2064 6174 652e 5c6e 352e  nished date.\n5.
+00000490: 2043 616c 6375 6c61 7465 2074 6865 2050   Calculate the P
+000004a0: 5220 6379 636c 6520 7469 6d65 2062 7920  R cycle time by 
+000004b0: 6164 6469 6e67 2074 6865 2050 5220 636f  adding the PR co
+000004c0: 6469 6e67 2074 696d 652c 2050 5220 6475  ding time, PR du
+000004d0: 7269 6e67 2074 696d 6520 2874 696d 6520  ring time (time 
+000004e0: 7370 616e 2062 6574 7765 656e 2074 6865  span between the
+000004f0: 2070 756c 6c20 7265 7175 6573 7427 7320   pull request's 
+00000500: 6372 6561 7465 6420 6461 7465 2061 6e64  created date and
+00000510: 206d 6572 6765 6420 6461 7465 292c 2061   merged date), a
+00000520: 6e64 2050 5220 6465 706c 6f79 2074 696d  nd PR deploy tim
+00000530: 652e 5c6e 5c6e 5468 6520 6675 6e63 7469  e.\n\nThe functi
+00000540: 6f6e 2072 6574 7572 6e73 2061 2060 5072  on returns a `Pr
+00000550: 6f6a 6563 7450 724d 6574 7269 6360 206f  ojectPrMetric` o
+00000560: 626a 6563 7420 636f 6e74 6169 6e69 6e67  bject containing
+00000570: 2074 6865 2063 616c 6375 6c61 7465 6420   the calculated 
+00000580: 6c65 6164 2074 696d 6573 2066 6f72 2065  lead times for e
+00000590: 6163 6820 7075 6c6c 2072 6571 7565 7374  ach pull request
+000005a0: 2069 6e20 7468 6520 7072 6f6a 6563 742e   in the project.
+000005b0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000005c0: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
+000005d0: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+000005e0: 2020 2020 226e 6f74 6573 223a 207b 0a20      "notes": {. 
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000600: 6c65 7665 6c22 3a20 226d 6964 220a 2020  level": "mid".  
+00000610: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000620: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+00000630: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
+00000640: 223a 2022 4452 512d 3222 2c0a 2020 2020  ": "DRQ-2",.    
+00000650: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00000660: 6e22 3a20 2257 6879 2063 616e 2074 6865  n": "Why can the
+00000670: 206c 6561 6420 7469 6d65 2066 6f72 2063   lead time for c
+00000680: 6861 6e67 6573 206d 6574 7269 6320 6265  hanges metric be
+00000690: 206e 756c 6c20 736f 6d65 7469 6d65 733f   null sometimes?
+000006a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000006b0: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
+000006c0: 223a 2022 5468 6520 6c65 6164 2074 696d  ": "The lead tim
+000006d0: 6520 666f 7220 6368 616e 6765 7320 6d65  e for changes me
+000006e0: 7472 6963 2063 616e 2062 6520 6e75 6c6c  tric can be null
+000006f0: 2073 6f6d 6574 696d 6573 2062 6563 6175   sometimes becau
+00000700: 7365 2073 6f6d 6520 6f66 2074 6865 2074  se some of the t
+00000710: 696d 6520 7370 616e 7320 7573 6564 2074  ime spans used t
+00000720: 6f20 6361 6c63 756c 6174 6520 6974 206d  o calculate it m
+00000730: 6967 6874 2062 6520 6e75 6c6c 2e20 496e  ight be null. In
+00000740: 2074 6865 2060 4361 6c63 756c 6174 6543   the `CalculateC
+00000750: 6861 6e67 654c 6561 6454 696d 6560 2066  hangeLeadTime` f
+00000760: 756e 6374 696f 6e2c 2074 6865 2050 5220  unction, the PR 
+00000770: 636f 6469 6e67 2074 696d 652c 2050 5220  coding time, PR 
+00000780: 7069 636b 7570 2074 696d 652c 2050 5220  pickup time, PR 
+00000790: 7265 7669 6577 2074 696d 652c 2061 6e64  review time, and
+000007a0: 2050 5220 6465 706c 6f79 2074 696d 6520   PR deploy time 
+000007b0: 6172 6520 6361 6c63 756c 6174 6564 2e20  are calculated. 
+000007c0: 4966 2061 6e79 206f 6620 7468 6573 6520  If any of these 
+000007d0: 7469 6d65 2073 7061 6e73 2061 7265 206e  time spans are n
+000007e0: 756c 6c20 6f72 2068 6176 6520 6e65 6761  ull or have nega
+000007f0: 7469 7665 2076 616c 7565 732c 2074 6865  tive values, the
+00000800: 2066 696e 616c 2050 5220 6379 636c 6520   final PR cycle 
+00000810: 7469 6d65 2028 6c65 6164 2074 696d 6520  time (lead time 
+00000820: 666f 7220 6368 616e 6765 7329 206d 6967  for changes) mig
+00000830: 6874 206e 6f74 2062 6520 6361 6c63 756c  ht not be calcul
+00000840: 6174 6564 2c20 7265 7375 6c74 696e 6720  ated, resulting 
+00000850: 696e 2061 206e 756c 6c20 7661 6c75 652e  in a null value.
+00000860: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000870: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
+00000880: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+00000890: 2020 2020 226e 6f74 6573 223a 207b 0a20      "notes": {. 
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000008b0: 6c65 7665 6c22 3a20 226c 6f77 220a 2020  level": "low".  
+000008c0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000008d0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+000008e0: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
+000008f0: 223a 2022 5152 442d 3422 2c0a 2020 2020  ": "QRD-4",.    
+00000900: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00000910: 6e22 3a20 2257 6861 7420 6461 7461 2064  n": "What data d
+00000920: 6f65 7320 7468 6520 417a 7572 6520 4465  oes the Azure De
+00000930: 764f 7073 2070 6c75 6769 6e20 636f 6c6c  vOps plugin coll
+00000940: 6563 743f 222c 0a20 2020 2020 2020 2020  ect?",.         
+00000950: 2020 2022 7265 6665 7265 6e63 655f 616e     "reference_an
+00000960: 7377 6572 223a 2022 5468 6520 417a 7572  swer": "The Azur
+00000970: 6520 4465 764f 7073 2070 6c75 6769 6e20  e DevOps plugin 
+00000980: 636f 6c6c 6563 7473 2064 6174 6120 7265  collects data re
+00000990: 6c61 7465 6420 746f 2047 6974 2072 6570  lated to Git rep
+000009a0: 6f73 6974 6f72 6965 732c 2047 6974 2070  ositories, Git p
+000009b0: 756c 6c20 7265 7175 6573 7473 2c20 4769  ull requests, Gi
+000009c0: 7420 7075 6c6c 2072 6571 7565 7374 2063  t pull request c
+000009d0: 6f6d 6d69 7473 2c20 6275 696c 6473 2c20  ommits, builds, 
+000009e0: 616e 6420 6a6f 6273 2e20 5370 6563 6966  and jobs. Specif
+000009f0: 6963 616c 6c79 2c20 6974 2063 6f6c 6c65  ically, it colle
+00000a00: 6374 7320 696e 666f 726d 6174 696f 6e20  cts information 
+00000a10: 7375 6368 2061 733a 5c6e 5c6e 312e 2047  such as:\n\n1. G
+00000a20: 6974 5075 6c6c 5265 7175 6573 7473 3a20  itPullRequests: 
+00000a30: 4261 7365 2072 6570 6f73 6974 6f72 7920  Base repository 
+00000a40: 4944 2c20 6865 6164 2072 6570 6f73 6974  ID, head reposit
+00000a50: 6f72 7920 4944 2c20 7374 6174 7573 2c20  ory ID, status, 
+00000a60: 6f72 6967 696e 616c 2073 7461 7475 732c  original status,
+00000a70: 2074 6974 6c65 2c20 6465 7363 7269 7074   title, descript
+00000a80: 696f 6e2c 2055 524c 2c20 6175 7468 6f72  ion, URL, author
+00000a90: 206e 616d 652c 2061 7574 686f 7220 4944   name, author ID
+00000aa0: 2c20 7075 6c6c 2072 6571 7565 7374 206b  , pull request k
+00000ab0: 6579 2c20 6372 6561 7465 6420 6461 7465  ey, created date
+00000ac0: 2c20 6d65 7267 6564 2064 6174 652c 2063  , merged date, c
+00000ad0: 6c6f 7365 6420 6461 7465 2c20 7479 7065  losed date, type
+00000ae0: 2c20 636f 6d70 6f6e 656e 742c 206d 6572  , component, mer
+00000af0: 6765 2063 6f6d 6d69 7420 5348 412c 2068  ge commit SHA, h
+00000b00: 6561 6420 7265 6665 7265 6e63 652c 2062  ead reference, b
+00000b10: 6173 6520 7265 6665 7265 6e63 652c 2068  ase reference, h
+00000b20: 6561 6420 636f 6d6d 6974 2053 4841 2c20  ead commit SHA, 
+00000b30: 616e 6420 6261 7365 2063 6f6d 6d69 7420  and base commit 
+00000b40: 5348 412e 5c6e 5c6e 322e 2047 6974 5075  SHA.\n\n2. GitPu
+00000b50: 6c6c 5265 7175 6573 7443 6f6d 6d69 7473  llRequestCommits
+00000b60: 3a20 436f 6d6d 6974 2053 4841 2028 636f  : Commit SHA (co
+00000b70: 6d6d 6974 5f69 6429 2c20 7075 6c6c 2072  mmit_id), pull r
+00000b80: 6571 7565 7374 2049 442c 2063 6f6d 6d69  equest ID, commi
+00000b90: 7420 6175 7468 6f72 206e 616d 6520 2861  t author name (a
+00000ba0: 7574 686f 725f 6e61 6d65 292c 2063 6f6d  uthor_name), com
+00000bb0: 6d69 7420 6175 7468 6f72 2065 6d61 696c  mit author email
+00000bc0: 2028 6175 7468 6f72 5f65 6d61 696c 292c   (author_email),
+00000bd0: 2061 6e64 2063 6f6d 6d69 7420 6175 7468   and commit auth
+00000be0: 6f72 6564 2064 6174 6520 2861 7574 686f  ored date (autho
+00000bf0: 725f 6461 7465 292e 5c6e 5c6e 332e 2042  r_date).\n\n3. B
+00000c00: 7569 6c64 733a 2042 7569 6c64 2773 206e  uilds: Build's n
+00000c10: 616d 652c 2073 7461 7475 732c 2063 7265  ame, status, cre
+00000c20: 6174 6564 2064 6174 652c 2066 696e 6973  ated date, finis
+00000c30: 6865 6420 6461 7465 2c20 7265 7375 6c74  hed date, result
+00000c40: 2c20 6475 7261 7469 6f6e 2069 6e20 7365  , duration in se
+00000c50: 636f 6e64 732c 2065 6e76 6972 6f6e 6d65  conds, environme
+00000c60: 6e74 2c20 7479 7065 2c20 616e 6420 6f74  nt, type, and ot
+00000c70: 6865 7220 7265 6c61 7465 6420 6465 7461  her related deta
+00000c80: 696c 7320 6c69 6b65 2063 6f6d 6d69 7420  ils like commit 
+00000c90: 5348 412c 2062 7261 6e63 682c 2072 6570  SHA, branch, rep
+00000ca0: 6f73 6974 6f72 7920 4944 2c20 616e 6420  ository ID, and 
+00000cb0: 7265 706f 7369 746f 7279 2055 524c 2e5c  repository URL.\
+00000cc0: 6e5c 6e34 2e20 4a6f 6273 3a20 4a6f 6220  n\n4. Jobs: Job 
+00000cd0: 4944 2c20 6e61 6d65 2c20 6275 696c 6420  ID, name, build 
+00000ce0: 4944 2c20 7374 6174 7573 2c20 7374 6172  ID, status, star
+00000cf0: 7420 7469 6d65 2c20 6669 6e69 7368 2074  t time, finish t
+00000d00: 696d 652c 2072 6573 756c 742c 2074 7970  ime, result, typ
+00000d10: 652c 2064 7572 6174 696f 6e20 696e 2073  e, duration in s
+00000d20: 6563 6f6e 6473 2c20 656e 7669 726f 6e6d  econds, environm
+00000d30: 656e 742c 2061 6e64 2043 4943 4420 7363  ent, and CICD sc
+00000d40: 6f70 6520 4944 2e22 2c0a 2020 2020 2020  ope ID.",.      
+00000d50: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00000d60: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00000d70: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00000d80: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00000d90: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+00000da0: 6d69 6422 0a20 2020 2020 2020 2020 2020  mid".           
+00000db0: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00000dc0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000dd0: 2020 2020 2269 6422 3a20 2251 5244 2d37      "id": "QRD-7
+00000de0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000df0: 7175 6573 7469 6f6e 223a 2022 486f 7720  question": "How 
+00000e00: 6361 6e20 4920 636f 6e74 7269 6275 7465  can I contribute
+00000e10: 2074 6f20 4465 764c 616b 653f 222c 0a20   to DevLake?",. 
+00000e20: 2020 2020 2020 2020 2020 2022 7265 6665             "refe
+00000e30: 7265 6e63 655f 616e 7377 6572 223a 2022  rence_answer": "
+00000e40: 596f 7520 6361 6e20 636f 6e74 7269 6275  You can contribu
+00000e50: 7465 2074 6f20 4465 764c 616b 6520 696e  te to DevLake in
+00000e60: 2073 6576 6572 616c 2077 6179 733a 5c6e   several ways:\n
+00000e70: 5c6e 312e 2043 7265 6174 6520 616e 2049  \n1. Create an I
+00000e80: 7373 7565 3a20 5265 706f 7274 2061 2062  ssue: Report a b
+00000e90: 7567 206f 7220 6665 6174 7572 6520 7265  ug or feature re
+00000ea0: 7175 6573 7420 746f 2041 7061 6368 6520  quest to Apache 
+00000eb0: 4465 764c 616b 652e 5c6e 322e 2053 7562  DevLake.\n2. Sub
+00000ec0: 6d69 7420 6120 5052 2028 5075 6c6c 2052  mit a PR (Pull R
+00000ed0: 6571 7565 7374 293a 2053 7461 7274 2077  equest): Start w
+00000ee0: 6974 6820 676f 6f64 2066 6972 7374 2069  ith good first i
+00000ef0: 7373 7565 7320 6f72 2069 7373 7565 7320  ssues or issues 
+00000f00: 7769 7468 206e 6f20 6173 7369 676e 6565  with no assignee
+00000f10: 732e 2052 6561 6420 7468 726f 7567 6820  s. Read through 
+00000f20: 7468 6520 5b43 6f6e 7472 6962 7574 696e  the [Contributin
+00000f30: 6720 446f 6375 6d65 6e74 6174 696f 6e5d  g Documentation]
+00000f40: 2868 7474 7073 3a2f 2f64 6576 6c61 6b65  (https://devlake
+00000f50: 2e61 7061 6368 652e 6f72 672f 636f 6d6d  .apache.org/comm
+00000f60: 756e 6974 792f 292c 2061 6464 2072 656c  unity/), add rel
+00000f70: 6576 616e 7420 7465 7374 732c 2064 6f63  evant tests, doc
+00000f80: 756d 656e 7461 7469 6f6e 2c20 616e 6420  umentation, and 
+00000f90: 6c61 6265 6c73 2074 6f20 7468 6520 5052  labels to the PR
+00000fa0: 2e5c 6e33 2e20 4a6f 696e 204d 6169 6c69  .\n3. Join Maili
+00000fb0: 6e67 206c 6973 743a 2049 6e69 7469 6174  ng list: Initiat
+00000fc0: 6520 6f72 2070 6172 7469 6369 7061 7465  e or participate
+00000fd0: 2069 6e20 7072 6f6a 6563 7420 6469 7363   in project disc
+00000fe0: 7573 7369 6f6e 7320 6f6e 2074 6865 206d  ussions on the m
+00000ff0: 6169 6c69 6e67 206c 6973 742e 5c6e 342e  ailing list.\n4.
+00001000: 2057 7269 7465 2061 2042 6c6f 673a 2057   Write a Blog: W
+00001010: 7269 7465 2061 2062 6c6f 6720 746f 2073  rite a blog to s
+00001020: 6861 7265 2079 6f75 7220 7573 6520 6361  hare your use ca
+00001030: 7365 7320 6162 6f75 7420 4170 6163 6865  ses about Apache
+00001040: 2044 6576 4c61 6b65 2e5c 6e35 2e20 436f   DevLake.\n5. Co
+00001050: 6e74 7269 6275 7465 2061 2050 6c75 6769  ntribute a Plugi
+00001060: 6e3a 2041 6464 2061 2070 6c75 6769 6e20  n: Add a plugin 
+00001070: 746f 2069 6e74 6567 7261 7465 2041 7061  to integrate Apa
+00001080: 6368 6520 4465 764c 616b 6520 7769 7468  che DevLake with
+00001090: 206d 6f72 6520 6461 7461 2073 6f75 7263   more data sourc
+000010a0: 6573 2066 6f72 2074 6865 2063 6f6d 6d75  es for the commu
+000010b0: 6e69 7479 2e5c 6e5c 6e50 6c65 6173 6520  nity.\n\nPlease 
+000010c0: 7265 6164 2074 6865 205b 636f 6e74 7269  read the [contri
+000010d0: 6275 7469 6f6e 2067 7569 6465 6c69 6e65  bution guideline
+000010e0: 735d 2868 7474 7073 3a2f 2f64 6576 6c61  s](https://devla
+000010f0: 6b65 2e61 7061 6368 652e 6f72 672f 636f  ke.apache.org/co
+00001100: 6d6d 756e 6974 7929 2062 6566 6f72 6520  mmunity) before 
+00001110: 796f 7520 6d61 6b65 2061 2063 6f6e 7472  you make a contr
+00001120: 6962 7574 696f 6e2e 222c 0a20 2020 2020  ibution.",.     
+00001130: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
+00001140: 726f 7065 7274 6965 7322 3a20 5b5d 2c0a  roperties": [],.
+00001150: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
+00001160: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
+00001170: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
+00001180: 226c 6f77 220a 2020 2020 2020 2020 2020  "low".          
+00001190: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+000011a0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000011b0: 2020 2020 2022 6964 223a 2022 5152 442d       "id": "QRD-
+000011c0: 3822 2c0a 2020 2020 2020 2020 2020 2020  8",.            
+000011d0: 2271 7565 7374 696f 6e22 3a20 2244 6f65  "question": "Doe
+000011e0: 7320 4465 764c 616b 6527 7320 4769 7448  s DevLake's GitH
+000011f0: 7562 2070 6c75 6769 6e20 7375 7070 6f72  ub plugin suppor
+00001200: 7420 696e 6372 656d 656e 7461 6c20 7379  t incremental sy
+00001210: 6e63 3f22 2c0a 2020 2020 2020 2020 2020  nc?",.          
+00001220: 2020 2272 6566 6572 656e 6365 5f61 6e73    "reference_ans
+00001230: 7765 7222 3a20 2259 6573 2c20 4465 764c  wer": "Yes, DevL
+00001240: 616b 6527 7320 4769 7448 7562 2070 6c75  ake's GitHub plu
+00001250: 6769 6e20 7375 7070 6f72 7473 2069 6e63  gin supports inc
+00001260: 7265 6d65 6e74 616c 2073 796e 632e 2049  remental sync. I
+00001270: 6e20 7468 6520 636f 6465 2c20 796f 7520  n the code, you 
+00001280: 6361 6e20 7365 6520 7468 6520 666f 6c6c  can see the foll
+00001290: 6f77 696e 6720 6c69 6e65 3a5c 6e5c 6e60  owing line:\n\n`
+000012a0: 696e 6372 656d 656e 7461 6c20 3a3d 2063  incremental := c
+000012b0: 6f6c 6c65 6374 6f72 5769 7468 5374 6174  ollectorWithStat
+000012c0: 652e 4973 496e 6372 656d 656e 7461 6c28  e.IsIncremental(
+000012d0: 2960 5c6e 5c6e 5468 6973 206c 696e 6520  )`\n\nThis line 
+000012e0: 6368 6563 6b73 2069 6620 7468 6520 636f  checks if the co
+000012f0: 6c6c 6563 746f 7220 6973 2072 756e 6e69  llector is runni
+00001300: 6e67 2069 6e20 696e 6372 656d 656e 7461  ng in incrementa
+00001310: 6c20 6d6f 6465 2e22 2c0a 2020 2020 2020  l mode.",.      
+00001320: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00001330: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00001340: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00001350: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00001360: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+00001370: 6d69 6422 0a20 2020 2020 2020 2020 2020  mid".           
+00001380: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00001390: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000013a0: 2020 2020 2269 6422 3a20 2251 5244 2d39      "id": "QRD-9
+000013b0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000013c0: 7175 6573 7469 6f6e 223a 2022 486f 7720  question": "How 
+000013d0: 6361 6e20 4920 6372 6561 7465 2044 6576  can I create Dev
+000013e0: 4c61 6b65 2070 6c75 6769 6e73 2069 6e20  Lake plugins in 
+000013f0: 5079 7468 6f6e 3f22 2c0a 2020 2020 2020  Python?",.      
+00001400: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
+00001410: 5f61 6e73 7765 7222 3a20 2254 6f20 6372  _answer": "To cr
+00001420: 6561 7465 2061 2044 6576 4c61 6b65 2070  eate a DevLake p
+00001430: 6c75 6769 6e20 696e 2050 7974 686f 6e2c  lugin in Python,
+00001440: 2066 6f6c 6c6f 7720 7468 6573 6520 7374   follow these st
+00001450: 6570 733a 5c6e 5c6e 312e 204d 616b 6520  eps:\n\n1. Make 
+00001460: 7375 7265 2079 6f75 2068 6176 6520 5b50  sure you have [P
+00001470: 6f65 7472 795d 2868 7474 7073 3a2f 2f70  oetry](https://p
+00001480: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
+00001490: 2f64 6f63 732f 2369 6e73 7461 6c6c 6174  /docs/#installat
+000014a0: 696f 6e29 2069 6e73 7461 6c6c 6564 2e5c  ion) installed.\
+000014b0: 6e32 2e20 4d6f 7665 2074 6f20 6070 7974  n2. Move to `pyt
+000014c0: 686f 6e2f 706c 7567 696e 7360 2061 6e64  hon/plugins` and
+000014d0: 2065 7865 6375 7465 2060 706f 6574 7279   execute `poetry
+000014e0: 206e 6577 206d 7970 6c75 6769 6e60 2e20   new myplugin`. 
+000014f0: 5468 6973 2077 696c 6c20 6765 6e65 7261  This will genera
+00001500: 7465 2061 206e 6577 2064 6972 6563 746f  te a new directo
+00001510: 7279 2066 6f72 2079 6f75 7220 706c 7567  ry for your plug
+00001520: 696e 2e5c 6e33 2e20 496e 2074 6865 2060  in.\n3. In the `
+00001530: 7079 7072 6f6a 6563 742e 746f 6d6c 6020  pyproject.toml` 
+00001540: 6669 6c65 2c20 6164 6420 7468 6520 666f  file, add the fo
+00001550: 6c6c 6f77 696e 6720 6c69 6e65 2061 7420  llowing line at 
+00001560: 7468 6520 656e 6420 6f66 2074 6865 2060  the end of the `
+00001570: 5b74 6f6f 6c2e 706f 6574 7279 2e64 6570  [tool.poetry.dep
+00001580: 656e 6465 6e63 6965 735d 6020 7365 6374  endencies]` sect
+00001590: 696f 6e3a 5c6e 6060 605c 6e70 7964 6576  ion:\n```\npydev
+000015a0: 6c61 6b65 203d 207b 2070 6174 6820 3d20  lake = { path = 
+000015b0: 5c22 2e2e 2f2e 2e2f 7079 6465 766c 616b  \"../../pydevlak
+000015c0: 655c 222c 2064 6576 656c 6f70 203d 2074  e\", develop = t
+000015d0: 7275 6520 7d5c 6e60 6060 5c6e 342e 2052  rue }\n```\n4. R
+000015e0: 756e 2060 706f 6574 7279 2069 6e73 7461  un `poetry insta
+000015f0: 6c6c 602e 5c6e 352e 2043 7265 6174 6520  ll`.\n5. Create 
+00001600: 6120 606d 6169 6e2e 7079 6020 6669 6c65  a `main.py` file
+00001610: 2077 6974 6820 7468 6520 6e65 6365 7373   with the necess
+00001620: 6172 7920 636f 6e74 656e 742c 2069 6e63  ary content, inc
+00001630: 6c75 6469 6e67 2063 6c61 7373 6573 2066  luding classes f
+00001640: 6f72 2063 6f6e 6e65 6374 696f 6e2c 2074  or connection, t
+00001650: 7261 6e73 666f 726d 6174 696f 6e20 7275  ransformation ru
+00001660: 6c65 2c20 746f 6f6c 2073 636f 7065 2c20  le, tool scope, 
+00001670: 616e 6420 706c 7567 696e 2e5c 6e36 2e20  and plugin.\n6. 
+00001680: 4372 6561 7465 2073 6865 6c6c 2073 6372  Create shell scr
+00001690: 6970 7473 2060 6275 696c 642e 7368 6020  ipts `build.sh` 
+000016a0: 616e 6420 6072 756e 2e73 6860 2069 6e20  and `run.sh` in 
+000016b0: 7468 6520 706c 7567 696e 2072 6f6f 7420  the plugin root 
+000016c0: 6469 7265 6374 6f72 7920 746f 2062 7569  directory to bui
+000016d0: 6c64 2061 6e64 2072 756e 2074 6865 2070  ld and run the p
+000016e0: 6c75 6769 6e2e 5c6e 372e 2044 6566 696e  lugin.\n7. Defin
+000016f0: 6520 636f 6e6e 6563 7469 6f6e 2070 6172  e connection par
+00001700: 616d 6574 6572 732c 2074 7261 6e73 666f  ameters, transfo
+00001710: 726d 6174 696f 6e20 7275 6c65 2070 6172  rmation rule par
+00001720: 616d 6574 6572 732c 2061 6e64 2074 6f6f  ameters, and too
+00001730: 6c20 7363 6f70 6520 7479 7065 2e5c 6e38  l scope type.\n8
+00001740: 2e20 496d 706c 656d 656e 7420 6d65 7468  . Implement meth
+00001750: 6f64 7320 6c69 6b65 2060 646f 6d61 696e  ods like `domain
+00001760: 5f73 636f 7065 7360 2c20 6072 656d 6f74  _scopes`, `remot
+00001770: 655f 7363 6f70 6560 2c20 6072 656d 6f74  e_scope`, `remot
+00001780: 655f 7363 6f70 655f 6772 6f75 7073 602c  e_scope_groups`,
+00001790: 2061 6e64 2060 7465 7374 5f63 6f6e 6e65   and `test_conne
+000017a0: 6374 696f 6e60 2e5c 6e39 2e20 4164 6420  ction`.\n9. Add 
+000017b0: 6120 6e65 7720 6461 7461 2073 7472 6561  a new data strea
+000017c0: 6d20 6279 2063 7265 6174 696e 6720 6120  m by creating a 
+000017d0: 746f 6f6c 206d 6f64 656c 2c20 7374 7265  tool model, stre
+000017e0: 616d 2063 6c61 7373 2c20 616e 6420 4150  am class, and AP
+000017f0: 4920 7772 6170 7065 722e 5c6e 3130 2e20  I wrapper.\n10. 
+00001800: 496d 706c 656d 656e 7420 6d65 7468 6f64  Implement method
+00001810: 7320 6c69 6b65 2060 636f 6c6c 6563 7460  s like `collect`
+00001820: 2c20 6065 7874 7261 6374 602c 2061 6e64  , `extract`, and
+00001830: 2060 636f 6e76 6572 7460 2066 6f72 2074   `convert` for t
+00001840: 6865 2073 7472 6561 6d20 636c 6173 732e  he stream class.
+00001850: 5c6e 3131 2e20 4966 206e 6565 6465 642c  \n11. If needed,
+00001860: 2063 7265 6174 6520 7375 6273 7472 6561   create substrea
+00001870: 6d73 2066 6f72 2068 6965 7261 7263 6869  ms for hierarchi
+00001880: 6361 6c20 6461 7461 2073 6f75 7263 6573  cal data sources
+00001890: 2e5c 6e31 322e 2054 6573 7420 7468 6520  .\n12. Test the 
+000018a0: 706c 7567 696e 2073 7461 6e64 616c 6f6e  plugin standalon
+000018b0: 6520 7573 696e 6720 7468 6520 606d 6169  e using the `mai
+000018c0: 6e2e 7079 6020 6669 6c65 2077 6974 6820  n.py` file with 
+000018d0: 6469 6666 6572 656e 7420 636f 6d6d 616e  different comman
+000018e0: 6473 2e5c 6e31 332e 2057 7269 7465 2075  ds.\n13. Write u
+000018f0: 6e69 742d 7465 7374 7320 666f 7220 796f  nit-tests for yo
+00001900: 7572 2070 6c75 6769 6e20 636f 6465 2c20  ur plugin code, 
+00001910: 7769 7468 2074 6573 7420 6669 6c65 7320  with test files 
+00001920: 656e 6469 6e67 2069 6e20 605f 7465 7374  ending in `_test
+00001930: 2e70 7960 2e5c 6e5c 6e48 6572 6527 7320  .py`.\n\nHere's 
+00001940: 6120 6765 6e65 7261 6c20 6f75 746c 696e  a general outlin
+00001950: 6520 6f66 2061 2044 6576 4c61 6b65 2070  e of a DevLake p
+00001960: 6c75 6769 6e20 636c 6173 733a 5c6e 5c6e  lugin class:\n\n
+00001970: 6060 6070 7974 686f 6e5c 6e66 726f 6d20  ```python\nfrom 
+00001980: 7079 6465 766c 616b 652e 706c 7567 696e  pydevlake.plugin
+00001990: 2069 6d70 6f72 7420 506c 7567 696e 5c6e   import Plugin\n
+000019a0: 5c6e 636c 6173 7320 4d79 4465 764c 616b  \nclass MyDevLak
+000019b0: 6550 6c75 6769 6e28 506c 7567 696e 293a  ePlugin(Plugin):
+000019c0: 5c6e 2020 2020 2320 496d 706c 656d 656e  \n    # Implemen
+000019d0: 7420 7265 7175 6972 6564 2070 726f 7065  t required prope
+000019e0: 7274 6965 7320 616e 6420 6d65 7468 6f64  rties and method
+000019f0: 7320 6865 7265 5c6e 2020 2020 2320 652e  s here\n    # e.
+00001a00: 672e 2c20 6e61 6d65 2c20 6465 7363 7269  g., name, descri
+00001a10: 7074 696f 6e2c 2063 6f6e 6e65 6374 696f  ption, connectio
+00001a20: 6e5f 7479 7065 2c20 746f 6f6c 5f73 636f  n_type, tool_sco
+00001a30: 7065 5f74 7970 652c 2074 7261 6e73 666f  pe_type, transfo
+00001a40: 726d 6174 696f 6e5f 7275 6c65 5f74 7970  rmation_rule_typ
+00001a50: 652c 2073 7472 6561 6d73 2c20 6574 632e  e, streams, etc.
+00001a60: 5c6e 6060 605c 6e5c 6e59 6f75 2077 6f75  \n```\n\nYou wou
+00001a70: 6c64 2074 6865 6e20 6e65 6564 2074 6f20  ld then need to 
+00001a80: 696d 706c 656d 656e 7420 7468 6520 7265  implement the re
+00001a90: 7175 6972 6564 2070 726f 7065 7274 6965  quired propertie
+00001aa0: 7320 616e 6420 6d65 7468 6f64 7320 666f  s and methods fo
+00001ab0: 7220 796f 7572 2073 7065 6369 6669 6320  r your specific 
+00001ac0: 706c 7567 696e 2c20 7375 6368 2061 7320  plugin, such as 
+00001ad0: 606e 616d 6560 2c20 6064 6573 6372 6970  `name`, `descrip
+00001ae0: 7469 6f6e 602c 2060 636f 6e6e 6563 7469  tion`, `connecti
+00001af0: 6f6e 5f74 7970 6560 2c20 6074 6f6f 6c5f  on_type`, `tool_
+00001b00: 7363 6f70 655f 7479 7065 602c 2060 7472  scope_type`, `tr
+00001b10: 616e 7366 6f72 6d61 7469 6f6e 5f72 756c  ansformation_rul
+00001b20: 655f 7479 7065 602c 2061 6e64 2060 7374  e_type`, and `st
+00001b30: 7265 616d 7360 2e20 596f 7520 6361 6e20  reams`. You can 
+00001b40: 7265 6665 7220 746f 2074 6865 2070 726f  refer to the pro
+00001b50: 7669 6465 6420 636f 6465 2773 2074 6573  vided code's tes
+00001b60: 7420 6675 6e63 7469 6f6e 7320 2865 2e67  t functions (e.g
+00001b70: 2e2c 2060 6173 7365 7274 5f76 616c 6964  ., `assert_valid
+00001b80: 5f6e 616d 6560 2c20 6061 7373 6572 745f  _name`, `assert_
+00001b90: 7661 6c69 645f 6465 7363 7269 7074 696f  valid_descriptio
+00001ba0: 6e60 2c20 6061 7373 6572 745f 7661 6c69  n`, `assert_vali
+00001bb0: 645f 636f 6e6e 6563 7469 6f6e 5f74 7970  d_connection_typ
+00001bc0: 6560 2c20 6574 632e 2920 746f 2075 6e64  e`, etc.) to und
+00001bd0: 6572 7374 616e 6420 7468 6520 7265 7175  erstand the requ
+00001be0: 6972 656d 656e 7473 2061 6e64 2063 6f6e  irements and con
+00001bf0: 7374 7261 696e 7473 2066 6f72 2065 6163  straints for eac
+00001c00: 6820 7072 6f70 6572 7479 2061 6e64 206d  h property and m
+00001c10: 6574 686f 642e 5c6e 5c6e 4f6e 6365 2079  ethod.\n\nOnce y
+00001c20: 6f75 2068 6176 6520 696d 706c 656d 656e  ou have implemen
+00001c30: 7465 6420 796f 7572 2070 6c75 6769 6e2c  ted your plugin,
+00001c40: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
+00001c50: 2070 726f 7669 6465 6420 7465 7374 2066   provided test f
+00001c60: 756e 6374 696f 6e73 2074 6f20 7661 6c69  unctions to vali
+00001c70: 6461 7465 2079 6f75 7220 706c 7567 696e  date your plugin
+00001c80: 2061 6e64 2065 6e73 7572 6520 6974 2077   and ensure it w
+00001c90: 6f72 6b73 2063 6f72 7265 6374 6c79 2e22  orks correctly."
+00001ca0: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+00001cb0: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
+00001cc0: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
+00001cd0: 2020 2022 6e6f 7465 7322 3a20 7b0a 2020     "notes": {.  
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00001cf0: 6576 656c 223a 2022 6c6f 7722 0a20 2020  evel": "low".   
+00001d00: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001d10: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00001d20: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00001d30: 3a20 2251 5244 2d31 3022 2c0a 2020 2020  : "QRD-10",.    
+00001d40: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00001d50: 6e22 3a20 2248 6f77 2064 6f20 4920 7265  n": "How do I re
+00001d60: 736f 6c76 6520 7468 6520 2770 616e 6963  solve the 'panic
+00001d70: 3a20 696e 7661 6c69 6420 656e 634b 6579  : invalid encKey
+00001d80: 2720 6572 726f 723f 222c 0a20 2020 2020  ' error?",.     
+00001d90: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
+00001da0: 655f 616e 7377 6572 223a 2022 546f 2072  e_answer": "To r
+00001db0: 6573 6f6c 7665 2074 6865 2027 7061 6e69  esolve the 'pani
+00001dc0: 633a 2069 6e76 616c 6964 2065 6e63 4b65  c: invalid encKe
+00001dd0: 7927 2065 7272 6f72 2c20 796f 7520 6e65  y' error, you ne
+00001de0: 6564 2074 6f20 656e 7375 7265 2074 6861  ed to ensure tha
+00001df0: 7420 796f 7520 6861 7665 2061 2076 616c  t you have a val
+00001e00: 6964 2065 6e63 7279 7074 696f 6e20 6b65  id encryption ke
+00001e10: 7920 7365 7420 696e 2079 6f75 7220 656e  y set in your en
+00001e20: 7669 726f 6e6d 656e 7420 6f72 2063 6f6e  vironment or con
+00001e30: 6669 6775 7261 7469 6f6e 2e20 4865 7265  figuration. Here
+00001e40: 2061 7265 2073 6f6d 6520 7374 6570 7320   are some steps 
+00001e50: 796f 7520 6361 6e20 666f 6c6c 6f77 3a5c  you can follow:\
+00001e60: 6e5c 6e31 2e20 4d61 6b65 2073 7572 6520  n\n1. Make sure 
+00001e70: 796f 7520 6861 7665 2061 2076 616c 6964  you have a valid
+00001e80: 2065 6e63 7279 7074 696f 6e20 6b65 7920   encryption key 
+00001e90: 616e 6420 6974 2773 2062 6569 6e67 2063  and it's being c
+00001ea0: 6f72 7265 6374 6c79 2066 6574 6368 6564  orrectly fetched
+00001eb0: 2075 7369 6e67 2074 6865 2060 706c 7567   using the `plug
+00001ec0: 696e 2e45 6e63 6f64 654b 6579 456e 7653  in.EncodeKeyEnvS
+00001ed0: 7472 6020 636f 6e73 7461 6e74 206f 7220  tr` constant or 
+00001ee0: 6120 7369 6d69 6c61 7220 6d65 7468 6f64  a similar method
+00001ef0: 2069 6e20 796f 7572 2063 6f64 652e 5c6e   in your code.\n
+00001f00: 322e 2049 6620 796f 7520 6172 6520 7573  2. If you are us
+00001f10: 696e 6720 6120 7261 6e64 6f6d 6c79 2067  ing a randomly g
+00001f20: 656e 6572 6174 6564 2065 6e63 7279 7074  enerated encrypt
+00001f30: 696f 6e20 6b65 792c 206d 616b 6520 7375  ion key, make su
+00001f40: 7265 2074 6f20 7374 6f72 6520 6974 2073  re to store it s
+00001f50: 6563 7572 656c 7920 616e 6420 7573 6520  ecurely and use 
+00001f60: 7468 6520 7361 6d65 206b 6579 2066 6f72  the same key for
+00001f70: 2062 6f74 6820 656e 6372 7970 7469 6f6e   both encryption
+00001f80: 2061 6e64 2064 6563 7279 7074 696f 6e20   and decryption 
+00001f90: 7072 6f63 6573 7365 732e 5c6e 332e 2043  processes.\n3. C
+00001fa0: 6865 636b 2074 6861 7420 7468 6520 656e  heck that the en
+00001fb0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00001fc0: 6c65 2073 7065 6369 6669 6564 2062 7920  le specified by 
+00001fd0: 6070 6c75 6769 6e2e 456e 636f 6465 4b65  `plugin.EncodeKe
+00001fe0: 7945 6e76 5374 7260 206f 7220 6120 7369  yEnvStr` or a si
+00001ff0: 6d69 6c61 7220 6d65 7468 6f64 2069 7320  milar method is 
+00002000: 7365 7420 7769 7468 2061 2076 616c 6964  set with a valid
+00002010: 2065 6e63 7279 7074 696f 6e20 6b65 792e   encryption key.
+00002020: 5c6e 342e 2056 6572 6966 7920 7468 6174  \n4. Verify that
+00002030: 2074 6865 2065 6e63 4b65 7920 6973 2062   the encKey is b
+00002040: 6569 6e67 2073 6574 2061 6e64 2073 6176  eing set and sav
+00002050: 6564 2074 6f20 7468 6520 636f 6e66 6967  ed to the config
+00002060: 2070 726f 7065 726c 7920 7573 696e 6720   properly using 
+00002070: 6076 2e53 6574 2870 6c75 6769 6e2e 456e  `v.Set(plugin.En
+00002080: 636f 6465 4b65 7945 6e76 5374 722c 2065  codeKeyEnvStr, e
+00002090: 6e63 4b65 7929 6020 616e 6420 6063 6f6e  ncKey)` and `con
+000020a0: 6669 672e 5772 6974 6543 6f6e 6669 6728  fig.WriteConfig(
+000020b0: 7629 6020 6f72 2073 696d 696c 6172 206d  v)` or similar m
+000020c0: 6574 686f 6473 2069 6e20 796f 7572 2063  ethods in your c
+000020d0: 6f64 652e 5c6e 5c6e 4966 2074 6865 2069  ode.\n\nIf the i
+000020e0: 7373 7565 2070 6572 7369 7374 732c 2079  ssue persists, y
+000020f0: 6f75 206d 6179 206e 6565 6420 746f 2070  ou may need to p
+00002100: 726f 7669 6465 206d 6f72 6520 636f 6e74  rovide more cont
+00002110: 6578 7420 6f72 2072 6566 6572 2074 6f20  ext or refer to 
+00002120: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00002130: 6e20 6f66 2074 6865 2073 7065 6369 6669  n of the specifi
+00002140: 6320 736f 6674 7761 7265 2079 6f75 2061  c software you a
+00002150: 7265 2077 6f72 6b69 6e67 2077 6974 682e  re working with.
+00002160: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00002170: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
+00002180: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+00002190: 2020 2020 226e 6f74 6573 223a 207b 0a20      "notes": {. 
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000021b0: 6c65 7665 6c22 3a20 226d 6964 220a 2020  level": "mid".  
+000021c0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000021d0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+000021e0: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
+000021f0: 223a 2022 5152 442d 3131 222c 0a20 2020  ": "QRD-11",.   
+00002200: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
+00002210: 6f6e 223a 2022 486f 7720 646f 6573 2044  on": "How does D
+00002220: 6576 4c61 6b65 2067 656e 6572 6174 6520  evLake generate 
+00002230: 6120 7069 7065 6c69 6e65 2062 6173 6564  a pipeline based
+00002240: 206f 6e20 6120 626c 7565 7072 696e 7427   on a blueprint'
+00002250: 7320 7365 7474 696e 673f 222c 0a20 2020  s setting?",.   
+00002260: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
+00002270: 6e63 655f 616e 7377 6572 223a 2022 4465  nce_answer": "De
+00002280: 764c 616b 6520 6765 6e65 7261 7465 7320  vLake generates 
+00002290: 6120 7069 7065 6c69 6e65 2062 6173 6564  a pipeline based
+000022a0: 206f 6e20 6120 626c 7565 7072 696e 7427   on a blueprint'
+000022b0: 7320 7365 7474 696e 6720 7468 726f 7567  s setting throug
+000022c0: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
+000022d0: 7374 6570 733a 5c6e 5c6e 312e 2054 6865  steps:\n\n1. The
+000022e0: 2062 6c75 6570 7269 6e74 2073 6574 7469   blueprint setti
+000022f0: 6e67 7320 6172 6520 6465 6669 6e65 6420  ngs are defined 
+00002300: 696e 2061 204a 534f 4e20 666f 726d 6174  in a JSON format
+00002310: 2c20 7768 6963 6820 696e 636c 7564 6573  , which includes
+00002320: 2074 6865 2076 6572 7369 6f6e 2c20 636f   the version, co
+00002330: 6e6e 6563 7469 6f6e 732c 2070 6c75 6769  nnections, plugi
+00002340: 6e2c 2063 6f6e 6e65 6374 696f 6e49 642c  n, connectionId,
+00002350: 2061 6e64 2073 636f 7065 732e 5c6e 5c6e   and scopes.\n\n
+00002360: 322e 2054 6865 2060 506c 7567 696e 426c  2. The `PluginBl
+00002370: 7565 7072 696e 7456 3230 302e 4d61 6b65  ueprintV200.Make
+00002380: 5069 7065 6c69 6e65 506c 616e 6020 6675  PipelinePlan` fu
+00002390: 6e63 7469 6f6e 2069 7320 6361 6c6c 6564  nction is called
+000023a0: 2077 6974 6820 616e 2061 7272 6179 206f   with an array o
+000023b0: 6620 7363 6f70 6573 2e20 5468 6520 706c  f scopes. The pl
+000023c0: 7567 696e 2072 6574 7572 6e73 2061 2060  ugin returns a `
+000023d0: 5069 7065 6c69 6e65 506c 616e 6020 696e  PipelinePlan` in
+000023e0: 204a 534f 4e20 666f 726d 6174 2061 6e64   JSON format and
+000023f0: 2061 6e20 6172 7261 7920 6f66 2060 5363   an array of `Sc
+00002400: 6f70 6560 2066 6f72 2070 726f 6a65 6374  ope` for project
+00002410: 5f6d 6170 7069 6e67 2e5c 6e5c 6e33 2e20  _mapping.\n\n3. 
+00002420: 5468 6520 6672 616d 6577 6f72 6b20 6d61  The framework ma
+00002430: 696e 7461 696e 7320 7468 6520 7072 6f6a  intains the proj
+00002440: 6563 745f 6d61 7070 696e 6720 7461 626c  ect_mapping tabl
+00002450: 6520 6261 7365 6420 6f6e 2074 6865 2060  e based on the `
+00002460: 5b5d 5363 6f70 6560 2061 7272 6179 2e5c  []Scope` array.\
+00002470: 6e5c 6e54 6865 7365 2073 7465 7073 2068  n\nThese steps h
+00002480: 656c 7020 4465 764c 616b 6520 6765 6e65  elp DevLake gene
+00002490: 7261 7465 2061 2070 6970 656c 696e 6520  rate a pipeline 
+000024a0: 706c 616e 2062 6173 6564 206f 6e20 7468  plan based on th
+000024b0: 6520 626c 7565 7072 696e 7427 7320 7365  e blueprint's se
+000024c0: 7474 696e 6773 2c20 7768 6963 6820 6361  ttings, which ca
+000024d0: 6e20 6265 2075 7365 6420 746f 2065 7865  n be used to exe
+000024e0: 6375 7465 2074 6865 2070 6970 656c 696e  cute the pipelin
+000024f0: 6520 616e 6420 636f 6c6c 6563 7420 6461  e and collect da
+00002500: 7461 2066 726f 6d20 7661 7269 6f75 7320  ta from various 
+00002510: 736f 7572 6365 732e 222c 0a20 2020 2020  sources.",.     
+00002520: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
+00002530: 726f 7065 7274 6965 7322 3a20 5b5d 2c0a  roperties": [],.
+00002540: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
+00002550: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
+00002560: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
+00002570: 226c 6f77 220a 2020 2020 2020 2020 2020  "low".          
+00002580: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+00002590: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000025a0: 2020 2020 2022 6964 223a 2022 5152 442d       "id": "QRD-
+000025b0: 3132 222c 0a20 2020 2020 2020 2020 2020  12",.           
+000025c0: 2022 7175 6573 7469 6f6e 223a 2022 486f   "question": "Ho
+000025d0: 7720 646f 6573 2044 6576 4c61 6b65 2064  w does DevLake d
+000025e0: 656c 6574 6520 6120 7072 6f6a 6563 743f  elete a project?
+000025f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00002600: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
+00002610: 223a 2022 4465 764c 616b 6520 6465 6c65  ": "DevLake dele
+00002620: 7465 7320 6120 7072 6f6a 6563 7420 6279  tes a project by
+00002630: 2066 6f6c 6c6f 7769 6e67 2074 6865 7365   following these
+00002640: 2073 7465 7073 3a5c 6e5c 6e31 2e20 5665   steps:\n\n1. Ve
+00002650: 7269 6679 2074 6865 2069 6e70 7574 2070  rify the input p
+00002660: 726f 6a65 6374 206e 616d 6520 6973 206e  roject name is n
+00002670: 6f74 2065 6d70 7479 2e5c 6e32 2e20 4265  ot empty.\n2. Be
+00002680: 6769 6e20 6120 6461 7461 6261 7365 2074  gin a database t
+00002690: 7261 6e73 6163 7469 6f6e 2e5c 6e33 2e20  ransaction.\n3. 
+000026a0: 4765 7420 7468 6520 7072 6f6a 6563 7420  Get the project 
+000026b0: 6279 2069 7473 206e 616d 6520 7573 696e  by its name usin
+000026c0: 6720 7468 6520 6067 6574 5072 6f6a 6563  g the `getProjec
+000026d0: 7442 794e 616d 6560 2066 756e 6374 696f  tByName` functio
+000026e0: 6e2e 5c6e 342e 2044 656c 6574 6520 7468  n.\n4. Delete th
+000026f0: 6520 7072 6f6a 6563 7420 6672 6f6d 2074  e project from t
+00002700: 6865 2060 6d6f 6465 6c73 2e50 726f 6a65  he `models.Proje
+00002710: 6374 6020 7461 626c 6520 7573 696e 6720  ct` table using 
+00002720: 7468 6520 7072 6f6a 6563 7420 6e61 6d65  the project name
+00002730: 2e5c 6e35 2e20 4465 6c65 7465 2074 6865  .\n5. Delete the
+00002740: 2070 726f 6a65 6374 206d 6170 7069 6e67   project mapping
+00002750: 2066 726f 6d20 7468 6520 6063 726f 7373   from the `cross
+00002760: 646f 6d61 696e 2e50 726f 6a65 6374 4d61  domain.ProjectMa
+00002770: 7070 696e 6760 2074 6162 6c65 2075 7369  pping` table usi
+00002780: 6e67 2074 6865 2070 726f 6a65 6374 206e  ng the project n
+00002790: 616d 652e 5c6e 362e 2044 656c 6574 6520  ame.\n6. Delete 
+000027a0: 7468 6520 7072 6f6a 6563 7420 6d65 7472  the project metr
+000027b0: 6963 2073 6574 7469 6e67 2066 726f 6d20  ic setting from 
+000027c0: 7468 6520 606d 6f64 656c 732e 5072 6f6a  the `models.Proj
+000027d0: 6563 744d 6574 7269 6353 6574 7469 6e67  ectMetricSetting
+000027e0: 6020 7461 626c 6520 7573 696e 6720 7468  ` table using th
+000027f0: 6520 7072 6f6a 6563 7420 6e61 6d65 2e5c  e project name.\
+00002800: 6e37 2e20 4465 6c65 7465 2074 6865 2070  n7. Delete the p
+00002810: 726f 6a65 6374 2050 5220 6d65 7472 6963  roject PR metric
+00002820: 2066 726f 6d20 7468 6520 6063 726f 7373   from the `cross
+00002830: 646f 6d61 696e 2e50 726f 6a65 6374 5072  domain.ProjectPr
+00002840: 4d65 7472 6963 6020 7461 626c 6520 7573  Metric` table us
+00002850: 696e 6720 7468 6520 7072 6f6a 6563 7420  ing the project 
+00002860: 6e61 6d65 2e5c 6e38 2e20 4465 6c65 7465  name.\n8. Delete
+00002870: 2074 6865 2070 726f 6a65 6374 2069 7373   the project iss
+00002880: 7565 206d 6574 7269 6320 6672 6f6d 2074  ue metric from t
+00002890: 6865 2060 6372 6f73 7364 6f6d 6169 6e2e  he `crossdomain.
+000028a0: 5072 6f6a 6563 7449 7373 7565 4d65 7472  ProjectIssueMetr
+000028b0: 6963 6020 7461 626c 6520 7573 696e 6720  ic` table using 
+000028c0: 7468 6520 7072 6f6a 6563 7420 6e61 6d65  the project name
+000028d0: 2e5c 6e39 2e20 436f 6d6d 6974 2074 6865  .\n9. Commit the
+000028e0: 2074 7261 6e73 6163 7469 6f6e 2e5c 6e31   transaction.\n1
+000028f0: 302e 2047 6574 2074 6865 2062 6c75 6570  0. Get the bluep
+00002900: 7269 6e74 2061 7373 6f63 6961 7465 6420  rint associated 
+00002910: 7769 7468 2074 6865 2070 726f 6a65 6374  with the project
+00002920: 206e 616d 6520 7573 696e 6720 7468 6520   name using the 
+00002930: 6062 704d 616e 6167 6572 2e47 6574 4462  `bpManager.GetDb
+00002940: 426c 7565 7072 696e 7442 7950 726f 6a65  BlueprintByProje
+00002950: 6374 4e61 6d65 6020 6675 6e63 7469 6f6e  ctName` function
+00002960: 2e5c 6e31 312e 2044 656c 6574 6520 7468  .\n11. Delete th
+00002970: 6520 626c 7565 7072 696e 7420 7573 696e  e blueprint usin
+00002980: 6720 7468 6520 6062 704d 616e 6167 6572  g the `bpManager
+00002990: 2e44 656c 6574 6542 6c75 6570 7269 6e74  .DeleteBlueprint
+000029a0: 6020 6675 6e63 7469 6f6e 2077 6974 6820  ` function with 
+000029b0: 7468 6520 626c 7565 7072 696e 7420 4944  the blueprint ID
+000029c0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+000029d0: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
+000029e0: 6573 223a 205b 5d2c 0a20 2020 2020 2020  es": [],.       
+000029f0: 2020 2020 2022 6e6f 7465 7322 3a20 7b0a       "notes": {.
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 226c 6576 656c 223a 2022 6869 6768 220a  "level": "high".
+00002a20: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00002a30: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00002a40: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002a50: 6964 223a 2022 5152 442d 3133 222c 0a20  id": "QRD-13",. 
+00002a60: 2020 2020 2020 2020 2020 2022 7175 6573             "ques
+00002a70: 7469 6f6e 223a 2022 486f 7720 646f 6573  tion": "How does
+00002a80: 2044 6576 4c61 6b65 2067 656e 6572 6174   DevLake generat
+00002a90: 6520 7468 6520 7465 6d70 6c61 7465 2075  e the template u
+00002aa0: 7365 725f 6163 636f 756e 745f 6d61 7070  ser_account_mapp
+00002ab0: 696e 672e 6373 7620 6669 6c65 3f22 2c0a  ing.csv file?",.
+00002ac0: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
+00002ad0: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
+00002ae0: 2244 6576 4c61 6b65 2067 656e 6572 6174  "DevLake generat
+00002af0: 6573 2074 6865 2074 656d 706c 6174 6520  es the template 
+00002b00: 7573 6572 5f61 6363 6f75 6e74 5f6d 6170  user_account_map
+00002b10: 7069 6e67 2e63 7376 2066 696c 6520 7573  ping.csv file us
+00002b20: 696e 6720 7468 6520 4765 7455 7365 7241  ing the GetUserA
+00002b30: 6363 6f75 6e74 4d61 7070 696e 6720 6675  ccountMapping fu
+00002b40: 6e63 7469 6f6e 2e20 5468 6973 2066 756e  nction. This fun
+00002b50: 6374 696f 6e20 7265 7472 6965 7665 7320  ction retrieves 
+00002b60: 616c 6c20 7573 6572 2f61 6363 6f75 6e74  all user/account
+00002b70: 206d 6170 7069 6e67 7320 6672 6f6d 2074   mappings from t
+00002b80: 6865 2073 746f 7265 2c20 6d61 7273 6861  he store, marsha
+00002b90: 6c73 2074 6865 6d20 696e 746f 2043 5356  ls them into CSV
+00002ba0: 2066 6f72 6d61 7420 7573 696e 6720 676f   format using go
+00002bb0: 6373 762e 4d61 7273 6861 6c42 7974 6573  csv.MarshalBytes
+00002bc0: 2861 6363 6f75 6e74 7329 2c20 616e 6420  (accounts), and 
+00002bd0: 7265 7475 726e 7320 7468 6520 4353 5620  returns the CSV 
+00002be0: 6461 7461 2061 7320 616e 204f 7574 7075  data as an Outpu
+00002bf0: 7446 696c 6520 7769 7468 2043 6f6e 7465  tFile with Conte
+00002c00: 6e74 5479 7065 205c 2274 6578 742f 6373  ntType \"text/cs
+00002c10: 765c 222e 222c 0a20 2020 2020 2020 2020  v\".",.         
+00002c20: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
+00002c30: 7274 6965 7322 3a20 5b5d 2c0a 2020 2020  rties": [],.    
+00002c40: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
+00002c50: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002c60: 2020 2022 6c65 7665 6c22 3a20 226d 6964     "level": "mid
+00002c70: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+00002c80: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002c90: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00002ca0: 2022 6964 223a 2022 5152 442d 3135 222c   "id": "QRD-15",
+00002cb0: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
+00002cc0: 6573 7469 6f6e 223a 2022 486f 7720 6973  estion": "How is
+00002cd0: 2074 6865 2068 2e73 746f 7265 2e66 696e   the h.store.fin
+00002ce0: 6441 6c6c 4163 636f 756e 7473 2066 756e  dAllAccounts fun
+00002cf0: 6374 696f 6e20 696d 706c 656d 656e 7465  ction implemente
+00002d00: 643f 222c 0a20 2020 2020 2020 2020 2020  d?",.           
+00002d10: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
+00002d20: 6572 223a 2022 5468 6520 682e 7374 6f72  er": "The h.stor
+00002d30: 652e 6669 6e64 416c 6c41 6363 6f75 6e74  e.findAllAccount
+00002d40: 7320 6675 6e63 7469 6f6e 2069 7320 696d  s function is im
+00002d50: 706c 656d 656e 7465 6420 6173 2066 6f6c  plemented as fol
+00002d60: 6c6f 7773 3a5c 6e5c 6e60 6060 676f 5c6e  lows:\n\n```go\n
+00002d70: 6675 6e63 2028 6420 2a64 6253 746f 7265  func (d *dbStore
+00002d80: 2920 6669 6e64 416c 6c41 6363 6f75 6e74  ) findAllAccount
+00002d90: 7328 2920 285b 5d61 6363 6f75 6e74 2c20  s() ([]account, 
+00002da0: 6572 726f 7273 2e45 7272 6f72 2920 7b5c  errors.Error) {\
+00002db0: 6e5c 7476 6172 2061 6120 5b5d 6372 6f73  n\tvar aa []cros
+00002dc0: 7364 6f6d 6169 6e2e 4163 636f 756e 745c  sdomain.Account\
+00002dd0: 6e5c 7465 7272 203a 3d20 642e 6462 2e41  n\terr := d.db.A
+00002de0: 6c6c 2826 6161 295c 6e5c 7469 6620 6572  ll(&aa)\n\tif er
+00002df0: 7220 213d 206e 696c 207b 5c6e 5c74 5c74  r != nil {\n\t\t
+00002e00: 7265 7475 726e 206e 696c 2c20 6572 725c  return nil, err\
+00002e10: 6e5c 747d 5c6e 5c74 7661 7220 7561 205b  n\t}\n\tvar ua [
+00002e20: 5d63 726f 7373 646f 6d61 696e 2e55 7365  ]crossdomain.Use
+00002e30: 7241 6363 6f75 6e74 5c6e 5c74 6572 7220  rAccount\n\terr 
+00002e40: 3d20 642e 6462 2e41 6c6c 2826 7561 295c  = d.db.All(&ua)\
+00002e50: 6e5c 7469 6620 6572 7220 213d 206e 696c  n\tif err != nil
+00002e60: 207b 5c6e 5c74 5c74 7265 7475 726e 206e   {\n\t\treturn n
+00002e70: 696c 2c20 6572 725c 6e5c 747d 5c6e 5c74  il, err\n\t}\n\t
+00002e80: 7661 7220 6120 2a61 6363 6f75 6e74 5c6e  var a *account\n
+00002e90: 5c74 7265 7475 726e 2061 2e66 726f 6d44  \treturn a.fromD
+00002ea0: 6f6d 6169 6e4c 6179 6572 2861 612c 2075  omainLayer(aa, u
+00002eb0: 6129 2c20 6e69 6c5c 6e7d 5c6e 6060 605c  a), nil\n}\n```\
+00002ec0: 6e5c 6e49 7420 7265 7472 6965 7665 7320  n\nIt retrieves 
+00002ed0: 616c 6c20 6163 636f 756e 7473 2061 6e64  all accounts and
+00002ee0: 2075 7365 7220 6163 636f 756e 7473 2066   user accounts f
+00002ef0: 726f 6d20 7468 6520 6461 7461 6261 7365  rom the database
+00002f00: 2c20 616e 6420 7468 656e 2063 616c 6c73  , and then calls
+00002f10: 2074 6865 2066 726f 6d44 6f6d 6169 6e4c   the fromDomainL
+00002f20: 6179 6572 2066 756e 6374 696f 6e20 746f  ayer function to
+00002f30: 2063 6f6e 7665 7274 2074 6865 6d20 696e   convert them in
+00002f40: 746f 2074 6865 2061 7070 726f 7072 6961  to the appropria
+00002f50: 7465 2066 6f72 6d61 742e 222c 0a20 2020  te format.",.   
+00002f60: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
+00002f70: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
+00002f80: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00002f90: 6f74 6573 223a 207b 0a20 2020 2020 2020  otes": {.       
+00002fa0: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
+00002fb0: 3a20 226c 6f77 220a 2020 2020 2020 2020  : "low".        
+00002fc0: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00002fd0: 2020 2020 5d0a 7d                            ].}
```

## chat/evaluation/qa/data/dataset/langchain_test_set.json

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

```diff
@@ -1,1144 +1,1132 @@
-00000000: 7b0d 0a20 2020 2022 6e61 6d65 223a 2022  {..    "name": "
-00000010: 4c61 6e67 6368 6169 6e53 6574 222c 0d0a  LangchainSet",..
-00000020: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00000030: 223a 2022 5465 7374 2073 7569 7465 206f  ": "Test suite o
-00000040: 6e20 7468 6520 6c61 6e67 6368 6169 6e20  n the langchain 
-00000050: 7072 6f6a 6563 742e 222c 0d0a 2020 2020  project.",..    
-00000060: 2263 6173 6573 223a 205b 0d0a 2020 2020  "cases": [..    
-00000070: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000080: 2020 2022 6964 223a 2022 6c61 6e67 6368     "id": "langch
-00000090: 6169 6e2d 3122 2c0d 0a20 2020 2020 2020  ain-1",..       
-000000a0: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
-000000b0: 2022 5768 6174 2069 7320 7468 6520 636c   "What is the cl
-000000c0: 6173 7320 6869 6572 6172 6368 793f 222c  ass hierarchy?",
-000000d0: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-000000e0: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-000000f0: 3a20 2254 6865 7265 2061 7265 2073 6576  : "There are sev
-00000100: 6572 616c 2063 6c61 7373 2068 6965 7261  eral class hiera
-00000110: 7263 6869 6573 2069 6e20 7468 6520 7072  rchies in the pr
-00000120: 6f76 6964 6564 2063 6f64 652c 2073 6f20  ovided code, so 
-00000130: 4927 6c6c 206c 6973 7420 6120 6665 773a  I'll list a few:
-00000140: 5c6e 5c6e 4261 7365 4d6f 6465 6cc2 a02d  \n\nBaseModel..-
-00000150: 3ec2 a043 6f6e 7374 6974 7574 696f 6e61  >..Constitutiona
-00000160: 6c50 7269 6e63 6970 6c65 3ac2 a043 6f6e  lPrinciple:..Con
-00000170: 7374 6974 7574 696f 6e61 6c50 7269 6e63  stitutionalPrinc
-00000180: 6970 6c65 c2a0 6973 2061 2073 7562 636c  iple..is a subcl
-00000190: 6173 7320 6f66 c2a0 4261 7365 4d6f 6465  ass of..BaseMode
-000001a0: 6c2e 5c6e 4261 7365 5072 6f6d 7074 5465  l.\nBasePromptTe
-000001b0: 6d70 6c61 7465 c2a0 2d3e c2a0 5374 7269  mplate..->..Stri
-000001c0: 6e67 5072 6f6d 7074 5465 6d70 6c61 7465  ngPromptTemplate
-000001d0: 2cc2 a041 494d 6573 7361 6765 5072 6f6d  ,..AIMessageProm
-000001e0: 7074 5465 6d70 6c61 7465 2cc2 a042 6173  ptTemplate,..Bas
-000001f0: 6543 6861 7450 726f 6d70 7454 656d 706c  eChatPromptTempl
-00000200: 6174 652c c2a0 4368 6174 4d65 7373 6167  ate,..ChatMessag
-00000210: 6550 726f 6d70 7454 656d 706c 6174 652c  ePromptTemplate,
-00000220: c2a0 4368 6174 5072 6f6d 7074 5465 6d70  ..ChatPromptTemp
-00000230: 6c61 7465 2cc2 a048 756d 616e 4d65 7373  late,..HumanMess
-00000240: 6167 6550 726f 6d70 7454 656d 706c 6174  agePromptTemplat
-00000250: 652c c2a0 4d65 7373 6167 6573 506c 6163  e,..MessagesPlac
-00000260: 6568 6f6c 6465 722c c2a0 5379 7374 656d  eholder,..System
-00000270: 4d65 7373 6167 6550 726f 6d70 7454 656d  MessagePromptTem
-00000280: 706c 6174 652c c2a0 4665 7753 686f 7450  plate,..FewShotP
-00000290: 726f 6d70 7454 656d 706c 6174 652c c2a0  romptTemplate,..
-000002a0: 4665 7753 686f 7450 726f 6d70 7457 6974  FewShotPromptWit
-000002b0: 6854 656d 706c 6174 6573 2cc2 a050 726f  hTemplates,..Pro
-000002c0: 6d70 742c c2a0 5072 6f6d 7074 5465 6d70  mpt,..PromptTemp
-000002d0: 6c61 7465 3a20 416c 6c20 6f66 2074 6865  late: All of the
-000002e0: 7365 2063 6c61 7373 6573 2061 7265 2073  se classes are s
-000002f0: 7562 636c 6173 7365 7320 6f66 c2a0 4261  ubclasses of..Ba
-00000300: 7365 5072 6f6d 7074 5465 6d70 6c61 7465  sePromptTemplate
-00000310: 2e5c 6e41 5049 4368 6169 6e2c c2a0 4368  .\nAPIChain,..Ch
-00000320: 6169 6e2c c2a0 4d61 7052 6564 7563 6544  ain,..MapReduceD
-00000330: 6f63 756d 656e 7473 4368 6169 6e2c c2a0  ocumentsChain,..
-00000340: 4d61 7052 6572 616e 6b44 6f63 756d 656e  MapRerankDocumen
-00000350: 7473 4368 6169 6e2c c2a0 5265 6669 6e65  tsChain,..Refine
-00000360: 446f 6375 6d65 6e74 7343 6861 696e 2cc2  DocumentsChain,.
-00000370: a053 7475 6666 446f 6375 6d65 6e74 7343  .StuffDocumentsC
-00000380: 6861 696e 2cc2 a048 7970 6f74 6865 7469  hain,..Hypotheti
-00000390: 6361 6c44 6f63 756d 656e 7445 6d62 6564  calDocumentEmbed
-000003a0: 6465 722c c2a0 4c4c 4d43 6861 696e 2cc2  der,..LLMChain,.
-000003b0: a04c 4c4d 4261 7368 4368 6169 6e2c c2a0  .LLMBashChain,..
-000003c0: 4c4c 4d43 6865 636b 6572 4368 6169 6e2c  LLMCheckerChain,
-000003d0: c2a0 4c4c 4d4d 6174 6843 6861 696e 2cc2  ..LLMMathChain,.
-000003e0: a04c 4c4d 5265 7175 6573 7473 4368 6169  .LLMRequestsChai
-000003f0: 6e2c c2a0 5041 4c43 6861 696e 2cc2 a051  n,..PALChain,..Q
-00000400: 4157 6974 6853 6f75 7263 6573 4368 6169  AWithSourcesChai
-00000410: 6e2c c2a0 5665 6374 6f72 4442 5141 5769  n,..VectorDBQAWi
-00000420: 7468 536f 7572 6365 7343 6861 696e 2cc2  thSourcesChain,.
-00000430: a056 6563 746f 7244 4251 412c c2a0 5351  .VectorDBQA,..SQ
-00000440: 4c44 6174 6162 6173 6543 6861 696e 3a20  LDatabaseChain: 
-00000450: 416c 6c20 6f66 2074 6865 7365 2063 6c61  All of these cla
-00000460: 7373 6573 2061 7265 2073 7562 636c 6173  sses are subclas
-00000470: 7365 7320 6f66 c2a0 4368 6169 6e2e 5c6e  ses of..Chain.\n
-00000480: 4261 7365 4c6f 6164 6572 3ac2 a042 6173  BaseLoader:..Bas
-00000490: 654c 6f61 6465 72c2 a069 7320 6120 7375  eLoader..is a su
-000004a0: 6263 6c61 7373 206f 66c2 a041 4243 2e5c  bclass of..ABC.\
-000004b0: 6e42 6173 6554 7261 6365 72c2 a02d 3ec2  nBaseTracer..->.
-000004c0: a043 6861 696e 5275 6e2c c2a0 4c4c 4d52  .ChainRun,..LLMR
-000004d0: 756e 2cc2 a053 6861 7265 6454 7261 6365  un,..SharedTrace
-000004e0: 722c c2a0 546f 6f6c 5275 6e2c c2a0 5472  r,..ToolRun,..Tr
-000004f0: 6163 6572 2cc2 a054 7261 6365 7245 7863  acer,..TracerExc
-00000500: 6570 7469 6f6e 2cc2 a054 7261 6365 7253  eption,..TracerS
-00000510: 6573 7369 6f6e 3a20 416c 6c20 6f66 2074  ession: All of t
-00000520: 6865 7365 2063 6c61 7373 6573 2061 7265  hese classes are
-00000530: 2073 7562 636c 6173 7365 7320 6f66 c2a0   subclasses of..
-00000540: 4261 7365 5472 6163 6572 2e5c 6e4f 7065  BaseTracer.\nOpe
-00000550: 6e41 4945 6d62 6564 6469 6e67 732c c2a0  nAIEmbeddings,..
-00000560: 4875 6767 696e 6746 6163 6545 6d62 6564  HuggingFaceEmbed
-00000570: 6469 6e67 732c c2a0 436f 6865 7265 456d  dings,..CohereEm
-00000580: 6265 6464 696e 6773 2cc2 a04a 696e 6145  beddings,..JinaE
-00000590: 6d62 6564 6469 6e67 732c c2a0 4c6c 616d  mbeddings,..Llam
-000005a0: 6143 7070 456d 6265 6464 696e 6773 2cc2  aCppEmbeddings,.
-000005b0: a048 7567 6769 6e67 4661 6365 4875 6245  .HuggingFaceHubE
-000005c0: 6d62 6564 6469 6e67 732c c2a0 5465 6e73  mbeddings,..Tens
-000005d0: 6f72 666c 6f77 4875 6245 6d62 6564 6469  orflowHubEmbeddi
-000005e0: 6e67 732c c2a0 5361 6765 6d61 6b65 7245  ngs,..SagemakerE
-000005f0: 6e64 706f 696e 7445 6d62 6564 6469 6e67  ndpointEmbedding
-00000600: 732c c2a0 4875 6767 696e 6746 6163 6549  s,..HuggingFaceI
-00000610: 6e73 7472 7563 7445 6d62 6564 6469 6e67  nstructEmbedding
-00000620: 732c c2a0 5365 6c66 486f 7374 6564 456d  s,..SelfHostedEm
-00000630: 6265 6464 696e 6773 2cc2 a053 656c 6648  beddings,..SelfH
-00000640: 6f73 7465 6448 7567 6769 6e67 4661 6365  ostedHuggingFace
-00000650: 456d 6265 6464 696e 6773 2cc2 a053 656c  Embeddings,..Sel
-00000660: 6648 6f73 7465 6448 7567 6769 6e67 4661  fHostedHuggingFa
-00000670: 6365 496e 7374 7275 6374 456d 6265 6464  ceInstructEmbedd
-00000680: 696e 6773 2cc2 a046 616b 6545 6d62 6564  ings,..FakeEmbed
-00000690: 6469 6e67 732c c2a0 416c 6570 6841 6c70  dings,..AlephAlp
-000006a0: 6861 4173 796d 6d65 7472 6963 5365 6d61  haAsymmetricSema
-000006b0: 6e74 6963 456d 6265 6464 696e 672c c2a0  nticEmbedding,..
-000006c0: 416c 6570 6841 6c70 6861 5379 6d6d 6574  AlephAlphaSymmet
-000006d0: 7269 6353 656d 616e 7469 6345 6d62 6564  ricSemanticEmbed
-000006e0: 6469 6e67 3a20 416c 6c20 6f66 2074 6865  ding: All of the
-000006f0: 7365 2063 6c61 7373 6573 2061 7265 2073  se classes are s
-00000700: 7562 636c 6173 7365 7320 6f66 c2a0 4261  ubclasses of..Ba
-00000710: 7365 4c4c 4d2e 222c 0d0a 2020 2020 2020  seLLM.",..      
-00000720: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
-00000730: 6f70 6572 7469 6573 223a 205b 5d2c 0d0a  operties": [],..
-00000740: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
-00000750: 6573 223a 207b 0d0a 2020 2020 2020 2020  es": {..        
-00000760: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
-00000770: 2022 6869 6768 220d 0a20 2020 2020 2020   "high"..       
-00000780: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000790: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-000007a0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-000007b0: 2022 6c61 6e67 6368 6169 6e2d 3222 2c0d   "langchain-2",.
-000007c0: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
-000007d0: 6573 7469 6f6e 223a 2022 5768 6174 2063  estion": "What c
-000007e0: 6c61 7373 6573 2061 7265 2064 6572 6976  lasses are deriv
-000007f0: 6564 2066 726f 6d20 7468 6520 6043 6861  ed from the `Cha
-00000800: 696e 6020 636c 6173 733f 222c 0d0a 2020  in` class?",..  
-00000810: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
-00000820: 656e 6365 5f61 6e73 7765 7222 3a20 2254  ence_answer": "T
-00000830: 6865 7265 2061 7265 206d 756c 7469 706c  here are multipl
-00000840: 6520 636c 6173 7365 7320 7468 6174 2061  e classes that a
-00000850: 7265 2064 6572 6976 6564 2066 726f 6d20  re derived from 
-00000860: 7468 6520 4368 6169 6e20 636c 6173 732e  the Chain class.
-00000870: 2053 6f6d 6520 6f66 2074 6865 6d20 6172   Some of them ar
-00000880: 653a 5c6e 5c6e 4150 4943 6861 696e 5c6e  e:\n\nAPIChain\n
-00000890: 416e 616c 797a 6544 6f63 756d 656e 7443  AnalyzeDocumentC
-000008a0: 6861 696e 5c6e 4368 6174 5665 6374 6f72  hain\nChatVector
-000008b0: 4442 4368 6169 6e5c 6e43 6f6d 6269 6e65  DBChain\nCombine
-000008c0: 446f 6375 6d65 6e74 7343 6861 696e 5c6e  DocumentsChain\n
-000008d0: 436f 6e73 7469 7475 7469 6f6e 616c 4368  ConstitutionalCh
-000008e0: 6169 6e5c 6e43 6f6e 7665 7273 6174 696f  ain\nConversatio
-000008f0: 6e43 6861 696e 5c6e 4772 6170 6851 4143  nChain\nGraphQAC
-00000900: 6861 696e 5c6e 4879 706f 7468 6574 6963  hain\nHypothetic
-00000910: 616c 446f 6375 6d65 6e74 456d 6265 6464  alDocumentEmbedd
-00000920: 6572 5c6e 4c4c 4d43 6861 696e 5c6e 4c4c  er\nLLMChain\nLL
-00000930: 4d43 6865 636b 6572 4368 6169 6e5c 6e4c  MCheckerChain\nL
-00000940: 4c4d 5265 7175 6573 7473 4368 6169 6e5c  LMRequestsChain\
-00000950: 6e4c 4c4d 5375 6d6d 6172 697a 6174 696f  nLLMSummarizatio
-00000960: 6e43 6865 636b 6572 4368 6169 6e5c 6e4d  nCheckerChain\nM
-00000970: 6170 5265 6475 6365 4368 6169 6e5c 6e4f  apReduceChain\nO
-00000980: 7065 6e41 5049 456e 6470 6f69 6e74 4368  penAPIEndpointCh
-00000990: 6169 6e5c 6e50 414c 4368 6169 6e5c 6e51  ain\nPALChain\nQ
-000009a0: 4157 6974 6853 6f75 7263 6573 4368 6169  AWithSourcesChai
-000009b0: 6e5c 6e52 6574 7269 6576 616c 5141 5c6e  n\nRetrievalQA\n
-000009c0: 5265 7472 6965 7661 6c51 4157 6974 6853  RetrievalQAWithS
-000009d0: 6f75 7263 6573 4368 6169 6e5c 6e53 6571  ourcesChain\nSeq
-000009e0: 7565 6e74 6961 6c43 6861 696e 5c6e 5351  uentialChain\nSQ
-000009f0: 4c44 6174 6162 6173 6543 6861 696e 5c6e  LDatabaseChain\n
-00000a00: 5472 616e 7366 6f72 6d43 6861 696e 5c6e  TransformChain\n
-00000a10: 5665 6374 6f72 4442 5141 5c6e 5665 6374  VectorDBQA\nVect
-00000a20: 6f72 4442 5141 5769 7468 536f 7572 6365  orDBQAWithSource
-00000a30: 7343 6861 696e 5c6e 5c6e 5468 6572 6520  sChain\n\nThere 
-00000a40: 6d69 6768 7420 6265 206d 6f72 6520 636c  might be more cl
-00000a50: 6173 7365 7320 7468 6174 2061 7265 2064  asses that are d
-00000a60: 6572 6976 6564 2066 726f 6d20 7468 6520  erived from the 
-00000a70: 4368 6169 6e20 636c 6173 7320 6173 2069  Chain class as i
-00000a80: 7420 6973 2070 6f73 7369 626c 6520 746f  t is possible to
-00000a90: 2063 7265 6174 6520 6375 7374 6f6d 2063   create custom c
-00000aa0: 6c61 7373 6573 2074 6861 7420 6578 7465  lasses that exte
-00000ab0: 6e64 2074 6865 2043 6861 696e 2063 6c61  nd the Chain cla
-00000ac0: 7373 2e22 2c0d 0a20 2020 2020 2020 2020  ss.",..         
-00000ad0: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
-00000ae0: 7274 6965 7322 3a20 5b5d 2c0d 0a20 2020  rties": [],..   
-00000af0: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
-00000b00: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00000b10: 2020 2020 2022 6c65 7665 6c22 3a20 2268       "level": "h
-00000b20: 6967 6822 0d0a 2020 2020 2020 2020 2020  igh"..          
-00000b30: 2020 7d0d 0a20 2020 2020 2020 207d 2c0d    }..        },.
-00000b40: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-00000b50: 2020 2020 2020 2020 2269 6422 3a20 226c          "id": "l
-00000b60: 616e 6763 6861 696e 2d33 222c 0d0a 2020  angchain-3",..  
-00000b70: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
-00000b80: 696f 6e22 3a20 2257 6861 7420 636c 6173  ion": "What clas
-00000b90: 7365 7320 616e 6420 6675 6e63 7469 6f6e  ses and function
-00000ba0: 7320 696e 2074 6865 2060 2e2f 6c61 6e67  s in the `./lang
-00000bb0: 6368 6169 6e2f 7574 696c 6974 6965 732f  chain/utilities/
-00000bc0: 6020 666f 726c 6465 7220 6172 6520 6e6f  ` forlder are no
-00000bd0: 7420 636f 7665 7265 6420 6279 2075 6e69  t covered by uni
-00000be0: 7420 7465 7374 733f 222c 0d0a 2020 2020  t tests?",..    
-00000bf0: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
-00000c00: 6365 5f61 6e73 7765 7222 3a20 2241 6c6c  ce_answer": "All
-00000c10: 2063 6c61 7373 6573 2061 6e64 2066 756e   classes and fun
-00000c20: 6374 696f 6e73 2069 6e20 7468 65c2 a02e  ctions in the...
-00000c30: 2f6c 616e 6763 6861 696e 2f75 7469 6c69  /langchain/utili
-00000c40: 7469 6573 2fc2 a066 6f6c 6465 7220 7365  ties/..folder se
-00000c50: 656d 2074 6f20 6861 7665 2075 6e69 7420  em to have unit 
-00000c60: 7465 7374 7320 7772 6974 7465 6e20 666f  tests written fo
-00000c70: 7220 7468 656d 2e22 2c0d 0a20 2020 2020  r them.",..     
-00000c80: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
-00000c90: 726f 7065 7274 6965 7322 3a20 5b5d 2c0d  roperties": [],.
-00000ca0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00000cb0: 7465 7322 3a20 7b0d 0a20 2020 2020 2020  tes": {..       
-00000cc0: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
-00000cd0: 3a20 226d 6964 220d 0a20 2020 2020 2020  : "mid"..       
-00000ce0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000cf0: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00000d00: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00000d10: 2022 6c61 6e67 6368 6169 6e2d 3422 2c0d   "langchain-4",.
-00000d20: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
-00000d30: 6573 7469 6f6e 223a 2022 5768 6174 2061  estion": "What a
-00000d40: 7265 2074 6865 2073 6f6d 6520 6f66 2074  re the some of t
-00000d50: 6865 206d 6169 6e20 6368 616c 6c65 6e67  he main challeng
-00000d60: 6573 2074 6861 7420 7468 6520 4c61 6e67  es that the Lang
-00000d70: 6368 6169 6e20 7072 6f6a 6563 7420 6861  chain project ha
-00000d80: 7320 746f 2064 6561 6c20 7769 7468 3f22  s to deal with?"
-00000d90: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000da0: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
-00000db0: 223a 2022 4261 7365 6420 6f6e 2074 6865  ": "Based on the
-00000dc0: 2063 6f6e 7465 7874 2070 726f 7669 6465   context provide
-00000dd0: 642c 2069 7420 7365 656d 7320 746f 2062  d, it seems to b
-00000de0: 6520 7265 6c61 7465 6420 746f 206e 6174  e related to nat
-00000df0: 7572 616c 206c 616e 6775 6167 6520 7072  ural language pr
-00000e00: 6f63 6573 7369 6e67 2061 6e64 2072 756e  ocessing and run
-00000e10: 6e69 6e67 206d 6f64 656c 7320 6f72 2063  ning models or c
-00000e20: 6861 696e 7320 6f6e 2064 6174 6173 6574  hains on dataset
-00000e30: 732e 2053 6f6d 6520 6765 6e65 7261 6c20  s. Some general 
-00000e40: 6368 616c 6c65 6e67 6573 2074 6861 7420  challenges that 
-00000e50: 636f 756c 6420 6265 2066 6163 6564 2069  could be faced i
-00000e60: 6e20 7375 6368 2070 726f 6a65 6374 7320  n such projects 
-00000e70: 6d61 7920 696e 636c 7564 653a 5c6e 5c6e  may include:\n\n
-00000e80: 312e 2048 616e 646c 696e 6720 6c61 7267  1. Handling larg
-00000e90: 6520 616e 6420 6469 7665 7273 6520 6461  e and diverse da
-00000ea0: 7461 7365 7473 3a20 5072 6f63 6573 7369  tasets: Processi
-00000eb0: 6e67 2061 6e64 206d 616e 6167 696e 6720  ng and managing 
-00000ec0: 6c61 7267 6520 6461 7461 7365 7473 2063  large datasets c
-00000ed0: 616e 2062 6520 636f 6d70 7574 6174 696f  an be computatio
-00000ee0: 6e61 6c6c 7920 6578 7065 6e73 6976 6520  nally expensive 
-00000ef0: 616e 6420 7469 6d65 2d63 6f6e 7375 6d69  and time-consumi
-00000f00: 6e67 2e20 456e 7375 7269 6e67 2065 6666  ng. Ensuring eff
-00000f10: 6963 6965 6e74 2064 6174 6120 7072 6f63  icient data proc
-00000f20: 6573 7369 6e67 2061 6e64 2073 746f 7261  essing and stora
-00000f30: 6765 2069 7320 6372 7563 6961 6c20 666f  ge is crucial fo
-00000f40: 7220 7468 6520 7072 6f6a 6563 7427 7320  r the project's 
-00000f50: 7375 6363 6573 732e 5c6e 5c6e 322e 204d  success.\n\n2. M
-00000f60: 6f64 656c 2070 6572 666f 726d 616e 6365  odel performance
-00000f70: 2061 6e64 2061 6363 7572 6163 793a 2044   and accuracy: D
-00000f80: 6576 656c 6f70 696e 6720 6d6f 6465 6c73  eveloping models
-00000f90: 2074 6861 7420 6361 6e20 6163 6375 7261   that can accura
-00000fa0: 7465 6c79 2075 6e64 6572 7374 616e 642c  tely understand,
-00000fb0: 2067 656e 6572 6174 652c 206f 7220 6d61   generate, or ma
-00000fc0: 6e69 7075 6c61 7465 206e 6174 7572 616c  nipulate natural
-00000fd0: 206c 616e 6775 6167 6520 6973 2063 6f6d   language is com
-00000fe0: 706c 6578 2e20 456e 7375 7269 6e67 2068  plex. Ensuring h
-00000ff0: 6967 6820 7065 7266 6f72 6d61 6e63 6520  igh performance 
-00001000: 616e 6420 6163 6375 7261 6379 2069 7320  and accuracy is 
-00001010: 616e 206f 6e67 6f69 6e67 2063 6861 6c6c  an ongoing chall
-00001020: 656e 6765 2069 6e20 7468 6520 6669 656c  enge in the fiel
-00001030: 6420 6f66 206e 6174 7572 616c 206c 616e  d of natural lan
-00001040: 6775 6167 6520 7072 6f63 6573 7369 6e67  guage processing
-00001050: 2e5c 6e5c 6e33 2e20 496e 7465 6772 6174  .\n\n3. Integrat
-00001060: 696f 6e20 7769 7468 2076 6172 696f 7573  ion with various
-00001070: 2074 6f6f 6c73 2061 6e64 2073 6572 7669   tools and servi
-00001080: 6365 733a 2054 6865 2070 726f 6a65 6374  ces: The project
-00001090: 206d 6967 6874 2072 6571 7569 7265 2069   might require i
-000010a0: 6e74 6567 7261 7469 6f6e 2077 6974 6820  ntegration with 
-000010b0: 6469 6666 6572 656e 7420 746f 6f6c 7320  different tools 
-000010c0: 616e 6420 7365 7276 6963 6573 2c20 7375  and services, su
-000010d0: 6368 2061 7320 6c61 6e67 7561 6765 206d  ch as language m
-000010e0: 6f64 656c 732c 2041 5049 732c 206f 7220  odels, APIs, or 
-000010f0: 6f74 6865 7220 6578 7465 726e 616c 2072  other external r
-00001100: 6573 6f75 7263 6573 2e20 456e 7375 7269  esources. Ensuri
-00001110: 6e67 2073 6561 6d6c 6573 7320 696e 7465  ng seamless inte
-00001120: 6772 6174 696f 6e20 6361 6e20 6265 2063  gration can be c
-00001130: 6861 6c6c 656e 6769 6e67 2e5c 6e5c 6e34  hallenging.\n\n4
-00001140: 2e20 5363 616c 6162 696c 6974 793a 2041  . Scalability: A
-00001150: 7320 7468 6520 7072 6f6a 6563 7420 6772  s the project gr
-00001160: 6f77 732c 2069 7420 6d61 7920 6e65 6564  ows, it may need
-00001170: 2074 6f20 6861 6e64 6c65 206d 6f72 6520   to handle more 
-00001180: 6461 7461 2c20 6d6f 7265 206d 6f64 656c  data, more model
-00001190: 732c 206f 7220 6d6f 7265 2075 7365 7273  s, or more users
-000011a0: 2e20 456e 7375 7269 6e67 2074 6861 7420  . Ensuring that 
-000011b0: 7468 6520 7072 6f6a 6563 7420 6361 6e20  the project can 
-000011c0: 7363 616c 6520 736d 6f6f 7468 6c79 2061  scale smoothly a
-000011d0: 6e64 2068 616e 646c 6520 696e 6372 6561  nd handle increa
-000011e0: 7365 6420 776f 726b 6c6f 6164 7320 6973  sed workloads is
-000011f0: 2069 6d70 6f72 7461 6e74 2066 6f72 206c   important for l
-00001200: 6f6e 672d 7465 726d 2073 7563 6365 7373  ong-term success
-00001210: 2e5c 6e5c 6e35 2e20 5365 6375 7269 7479  .\n\n5. Security
-00001220: 2061 6e64 2070 7269 7661 6379 3a20 4861   and privacy: Ha
-00001230: 6e64 6c69 6e67 2073 656e 7369 7469 7665  ndling sensitive
-00001240: 2064 6174 6120 616e 6420 656e 7375 7269   data and ensuri
-00001250: 6e67 2074 6865 2073 6563 7572 6974 7920  ng the security 
-00001260: 616e 6420 7072 6976 6163 7920 6f66 2075  and privacy of u
-00001270: 7365 7273 2061 6e64 2074 6865 6972 2069  sers and their i
-00001280: 6e66 6f72 6d61 7469 6f6e 2069 7320 616e  nformation is an
-00001290: 2065 7373 656e 7469 616c 2061 7370 6563   essential aspec
-000012a0: 7420 7468 6174 206e 6565 6473 2074 6f20  t that needs to 
-000012b0: 6265 2061 6464 7265 7373 6564 2e5c 6e5c  be addressed.\n\
-000012c0: 6e36 2e20 4d61 696e 7461 696e 696e 6720  n6. Maintaining 
-000012d0: 616e 6420 7570 6461 7469 6e67 206d 6f64  and updating mod
-000012e0: 656c 733a 204c 616e 6775 6167 6520 6d6f  els: Language mo
-000012f0: 6465 6c73 2061 6e64 206f 7468 6572 2063  dels and other c
-00001300: 6f6d 706f 6e65 6e74 7320 6f66 2074 6865  omponents of the
-00001310: 2070 726f 6a65 6374 206d 6179 206e 6565   project may nee
-00001320: 6420 746f 2062 6520 7570 6461 7465 6420  d to be updated 
-00001330: 6f72 206d 6169 6e74 6169 6e65 6420 6f76  or maintained ov
-00001340: 6572 2074 696d 6520 746f 2065 6e73 7572  er time to ensur
-00001350: 6520 636f 6e74 696e 7565 6420 6566 6665  e continued effe
-00001360: 6374 6976 656e 6573 7320 616e 6420 7265  ctiveness and re
-00001370: 6c65 7661 6e63 652e 5c6e 5c6e 372e 2043  levance.\n\n7. C
-00001380: 6f73 7420 6d61 6e61 6765 6d65 6e74 3a20  ost management: 
-00001390: 5275 6e6e 696e 6720 6c61 6e67 7561 6765  Running language
-000013a0: 206d 6f64 656c 732c 2065 7370 6563 6961   models, especia
-000013b0: 6c6c 7920 6c61 7267 6520 6f6e 6573 2c20  lly large ones, 
-000013c0: 6361 6e20 6265 2065 7870 656e 7369 7665  can be expensive
-000013d0: 2e20 4d61 6e61 6769 6e67 2074 6865 2063  . Managing the c
-000013e0: 6f73 7473 2061 7373 6f63 6961 7465 6420  osts associated 
-000013f0: 7769 7468 2072 756e 6e69 6e67 2073 7563  with running suc
-00001400: 6820 6d6f 6465 6c73 2c20 616c 6f6e 6720  h models, along 
-00001410: 7769 7468 206f 7468 6572 2069 6e66 7261  with other infra
-00001420: 7374 7275 6374 7572 6520 616e 6420 7265  structure and re
-00001430: 736f 7572 6365 732c 2069 7320 6120 6368  sources, is a ch
-00001440: 616c 6c65 6e67 6520 7468 6174 206e 6565  allenge that nee
-00001450: 6473 2074 6f20 6265 2061 6464 7265 7373  ds to be address
-00001460: 6564 2e5c 6e5c 6e50 6c65 6173 6520 6e6f  ed.\n\nPlease no
-00001470: 7465 2074 6861 7420 7468 6573 6520 6172  te that these ar
-00001480: 6520 6765 6e65 7261 6c20 6368 616c 6c65  e general challe
-00001490: 6e67 6573 2074 6861 7420 636f 756c 6420  nges that could 
-000014a0: 6265 2066 6163 6564 2069 6e20 6120 6e61  be faced in a na
-000014b0: 7475 7261 6c20 6c61 6e67 7561 6765 2070  tural language p
-000014c0: 726f 6365 7373 696e 6720 7072 6f6a 6563  rocessing projec
-000014d0: 742e 2054 6865 2073 7065 6369 6669 6320  t. The specific 
-000014e0: 6368 616c 6c65 6e67 6573 2066 6163 6564  challenges faced
-000014f0: 2062 7920 7468 6520 4c61 6e67 6368 6169   by the Langchai
-00001500: 6e20 7072 6f6a 6563 7420 6d69 6768 7420  n project might 
-00001510: 7661 7279 2062 6173 6564 206f 6e20 6974  vary based on it
-00001520: 7320 676f 616c 732c 2073 636f 7065 2c20  s goals, scope, 
-00001530: 616e 6420 696d 706c 656d 656e 7461 7469  and implementati
-00001540: 6f6e 2e22 2c0d 0a20 2020 2020 2020 2020  on.",..         
-00001550: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
-00001560: 7274 6965 7322 3a20 5b5d 2c0d 0a20 2020  rties": [],..   
-00001570: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
-00001580: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00001590: 2020 2020 2022 6c65 7665 6c22 3a20 2268       "level": "h
-000015a0: 6967 6822 0d0a 2020 2020 2020 2020 2020  igh"..          
-000015b0: 2020 7d0d 0a20 2020 2020 2020 207d 2c0d    }..        },.
-000015c0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-000015d0: 2020 2020 2020 2020 2269 6422 3a20 226c          "id": "l
-000015e0: 616e 6763 6861 696e 2d35 222c 0d0a 2020  angchain-5",..  
-000015f0: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
-00001600: 696f 6e22 3a20 2244 6f65 7320 6055 6e73  ion": "Does `Uns
-00001610: 7472 7563 7475 7265 644d 6172 6b64 6f77  tructuredMarkdow
-00001620: 6e4c 6f61 6465 7260 2061 6363 6570 7420  nLoader` accept 
-00001630: 6120 7374 7269 6e67 2072 6570 7265 7365  a string represe
-00001640: 6e74 6174 696f 6e20 6f66 2061 206d 6172  ntation of a mar
-00001650: 6b64 6f77 6e20 6669 6c65 3f22 2c0d 0a20  kdown file?",.. 
-00001660: 2020 2020 2020 2020 2020 2022 7265 6665             "refe
-00001670: 7265 6e63 655f 616e 7377 6572 223a 2022  rence_answer": "
-00001680: 4e6f 2c20 556e 7374 7275 6374 7572 6564  No, Unstructured
-00001690: 4d61 726b 646f 776e 4c6f 6164 6572 2064  MarkdownLoader d
-000016a0: 6f65 7320 6e6f 7420 6163 6365 7074 2061  oes not accept a
-000016b0: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
-000016c0: 7461 7469 6f6e 206f 6620 6120 6d61 726b  tation of a mark
-000016d0: 646f 776e 2066 696c 652e 2049 7420 7461  down file. It ta
-000016e0: 6b65 7320 6120 6669 6c65 2070 6174 6820  kes a file path 
-000016f0: 6173 2069 6e70 7574 2e22 2c0d 0a20 2020  as input.",..   
-00001700: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
-00001710: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
-00001720: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00001730: 6e6f 7465 7322 3a20 7b0d 0a20 2020 2020  notes": {..     
-00001740: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
-00001750: 6c22 3a20 226d 6964 220d 0a20 2020 2020  l": "mid"..     
-00001760: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00001770: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
-00001780: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
-00001790: 223a 2022 6c61 6e67 6368 6169 6e2d 3622  ": "langchain-6"
-000017a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000017b0: 7175 6573 7469 6f6e 223a 2022 5768 6174  question": "What
-000017c0: 2069 7320 7468 6520 7075 7270 6f73 6520   is the purpose 
-000017d0: 6f66 2074 6865 206c 616e 6763 6861 696e  of the langchain
-000017e0: 2070 726f 6a65 6374 3f22 2c0d 0a20 2020   project?",..   
-000017f0: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
-00001800: 6e63 655f 616e 7377 6572 223a 2022 5468  nce_answer": "Th
-00001810: 6520 7075 7270 6f73 6520 6f66 2074 6865  e purpose of the
-00001820: 204c 616e 6763 6861 696e 2070 726f 6a65   Langchain proje
-00001830: 6374 2069 7320 746f 2070 726f 7669 6465  ct is to provide
-00001840: 2061 2066 7261 6d65 776f 726b 2066 6f72   a framework for
-00001850: 2064 6576 656c 6f70 696e 6720 6170 706c   developing appl
-00001860: 6963 6174 696f 6e73 2070 6f77 6572 6564  ications powered
-00001870: 2062 7920 6c61 6e67 7561 6765 206d 6f64   by language mod
-00001880: 656c 732e 2049 7420 6169 6d73 2074 6f20  els. It aims to 
-00001890: 7369 6d70 6c69 6679 2074 6865 2063 7265  simplify the cre
-000018a0: 6174 696f 6e20 6f66 2061 7070 6c69 6361  ation of applica
-000018b0: 7469 6f6e 7320 7573 696e 6720 6c61 7267  tions using larg
-000018c0: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
-000018d0: 7320 284c 4c4d 7329 2061 6e64 206f 6666  s (LLMs) and off
-000018e0: 6572 7320 6120 7365 7420 6f66 2074 6f6f  ers a set of too
-000018f0: 6c73 2061 6e64 2073 6572 7669 6365 7320  ls and services 
-00001900: 746f 2061 7373 6973 7420 6465 7665 6c6f  to assist develo
-00001910: 7065 7273 2069 6e20 6275 696c 6469 6e67  pers in building
-00001920: 204e 4c50 2061 7070 6c69 6361 7469 6f6e   NLP application
-00001930: 732e 2054 6865 204c 616e 6763 6861 696e  s. The Langchain
-00001940: 2066 7261 6d65 776f 726b 2065 6e61 626c   framework enabl
-00001950: 6573 2064 6576 656c 6f70 6572 7320 746f  es developers to
-00001960: 2063 7265 6174 6520 7365 7175 656e 6365   create sequence
-00001970: 7320 6f66 2063 616c 6c73 2c20 636f 6e6e  s of calls, conn
-00001980: 6563 7420 6c61 6e67 7561 6765 206d 6f64  ect language mod
-00001990: 656c 7320 746f 206f 7468 6572 2064 6174  els to other dat
-000019a0: 6120 736f 7572 6365 732c 2061 6e64 2069  a sources, and i
-000019b0: 6e74 6572 6163 7420 7769 7468 2061 7070  nteract with app
-000019c0: 6c69 6361 7469 6f6e 2d73 7065 6369 6669  lication-specifi
-000019d0: 6320 6461 7461 2e20 4974 2061 6c73 6f20  c data. It also 
-000019e0: 7072 6f76 6964 6573 206f 6666 2d74 6865  provides off-the
-000019f0: 2d73 6865 6c66 2063 6861 696e 7320 666f  -shelf chains fo
-00001a00: 7220 7370 6563 6966 6963 2074 6173 6b73  r specific tasks
-00001a10: 2061 6e64 2061 6c6c 6f77 7320 666f 7220   and allows for 
-00001a20: 6375 7374 6f6d 697a 6174 696f 6e20 616e  customization an
-00001a30: 6420 6275 696c 6469 6e67 206e 6577 2063  d building new c
-00001a40: 6861 696e 732e 204f 7665 7261 6c6c 2c20  hains. Overall, 
-00001a50: 7468 6520 4c61 6e67 6368 6169 6e20 7072  the Langchain pr
-00001a60: 6f6a 6563 7420 6169 6d73 2074 6f20 7265  oject aims to re
-00001a70: 766f 6c75 7469 6f6e 697a 6520 7468 6520  volutionize the 
-00001a80: 7761 7920 7065 6f70 6c65 206c 6561 726e  way people learn
-00001a90: 206c 616e 6775 6167 6573 2061 6e64 2065   languages and e
-00001aa0: 6e68 616e 6365 2074 6865 2063 6170 6162  nhance the capab
-00001ab0: 696c 6974 6965 7320 6f66 206c 616e 6775  ilities of langu
-00001ac0: 6167 6520 6d6f 6465 6c73 2069 6e20 7661  age models in va
-00001ad0: 7269 6f75 7320 6170 706c 6963 6174 696f  rious applicatio
-00001ae0: 6e73 2e22 2c0d 0a20 2020 2020 2020 2020  ns.",..         
-00001af0: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
-00001b00: 7274 6965 7322 3a20 5b5d 2c0d 0a20 2020  rties": [],..   
-00001b10: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
-00001b20: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00001b30: 2020 2020 2022 6c65 7665 6c22 3a20 226d       "level": "m
-00001b40: 6964 220d 0a20 2020 2020 2020 2020 2020  id"..           
-00001b50: 207d 0d0a 2020 2020 2020 2020 7d2c 0d0a   }..        },..
-00001b60: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00001b70: 2020 2020 2020 2022 6964 223a 2022 6c61         "id": "la
-00001b80: 6e67 6368 6169 6e2d 3722 2c0d 0a20 2020  ngchain-7",..   
-00001b90: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
-00001ba0: 6f6e 223a 2022 4973 204f 7065 6e41 4927  on": "Is OpenAI'
-00001bb0: 7320 6067 7074 2d34 2d30 3631 3360 206d  s `gpt-4-0613` m
-00001bc0: 6f64 656c 2073 7570 706f 7274 6564 3f22  odel supported?"
-00001bd0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00001be0: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
-00001bf0: 223a 2022 4e6f 2c20 7468 6973 206d 6f64  ": "No, this mod
-00001c00: 656c 2069 7320 6e6f 7420 7375 7070 6f72  el is not suppor
-00001c10: 7465 642e 222c 0d0a 2020 2020 2020 2020  ted.",..        
-00001c20: 2020 2020 2261 6e73 7765 725f 7072 6f70      "answer_prop
-00001c30: 6572 7469 6573 223a 205b 5d2c 0d0a 2020  erties": [],..  
-00001c40: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
-00001c50: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00001c60: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
-00001c70: 6d69 6422 0d0a 2020 2020 2020 2020 2020  mid"..          
-00001c80: 2020 7d0d 0a20 2020 2020 2020 207d 2c0d    }..        },.
-00001c90: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-00001ca0: 2020 2020 2020 2020 2269 6422 3a20 226c          "id": "l
-00001cb0: 616e 6763 6861 696e 2d38 222c 0d0a 2020  angchain-8",..  
-00001cc0: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
-00001cd0: 696f 6e22 3a20 2248 6f77 2064 6f20 4920  ion": "How do I 
-00001ce0: 7573 6520 616e 2060 4c4c 4d43 6861 696e  use an `LLMChain
-00001cf0: 6020 7769 7468 2061 2063 6861 7420 6d6f  ` with a chat mo
-00001d00: 6465 6c3f 2050 6c65 6173 6520 7072 6f76  del? Please prov
-00001d10: 6964 6520 6578 616d 706c 6520 636f 6465  ide example code
-00001d20: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00001d30: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
-00001d40: 6572 223a 2022 5468 65c2 a04c 4c4d 4368  er": "The..LLMCh
-00001d50: 6169 6ec2 a063 616e 2062 6520 7573 6564  ain..can be used
-00001d60: 2077 6974 6820 6368 6174 206d 6f64 656c   with chat model
-00001d70: 7320 6173 2077 656c 6c3a 5c6e 6060 605c  s as well:\n```\
-00001d80: 6e66 726f 6d20 6c61 6e67 6368 6169 6e20  nfrom langchain 
-00001d90: 696d 706f 7274 204c 4c4d 4368 6169 6e5c  import LLMChain\
-00001da0: 6e66 726f 6d20 6c61 6e67 6368 6169 6e2e  nfrom langchain.
-00001db0: 6368 6174 5f6d 6f64 656c 7320 696d 706f  chat_models impo
-00001dc0: 7274 2043 6861 744f 7065 6e41 495c 6e66  rt ChatOpenAI\nf
-00001dd0: 726f 6d20 6c61 6e67 6368 6169 6e2e 7072  rom langchain.pr
-00001de0: 6f6d 7074 732e 6368 6174 2069 6d70 6f72  ompts.chat impor
-00001df0: 7420 285c 6e20 2020 2043 6861 7450 726f  t (\n    ChatPro
-00001e00: 6d70 7454 656d 706c 6174 652c 5c6e 2020  mptTemplate,\n  
-00001e10: 2020 5379 7374 656d 4d65 7373 6167 6550    SystemMessageP
-00001e20: 726f 6d70 7454 656d 706c 6174 652c 5c6e  romptTemplate,\n
-00001e30: 2020 2020 4875 6d61 6e4d 6573 7361 6765      HumanMessage
-00001e40: 5072 6f6d 7074 5465 6d70 6c61 7465 2c5c  PromptTemplate,\
-00001e50: 6e29 5c6e 5c6e 6368 6174 203d 2043 6861  n)\n\nchat = Cha
-00001e60: 744f 7065 6e41 4928 7465 6d70 6572 6174  tOpenAI(temperat
-00001e70: 7572 653d 3029 5c6e 5c6e 7465 6d70 6c61  ure=0)\n\ntempla
-00001e80: 7465 203d 205c 2259 6f75 2061 7265 2061  te = \"You are a
-00001e90: 2068 656c 7066 756c 2061 7373 6973 7461   helpful assista
-00001ea0: 6e74 2074 6861 7420 7472 616e 736c 6174  nt that translat
-00001eb0: 6573 207b 696e 7075 745f 6c61 6e67 7561  es {input_langua
-00001ec0: 6765 7d20 746f 207b 6f75 7470 7574 5f6c  ge} to {output_l
-00001ed0: 616e 6775 6167 657d 2e5c 225c 6e73 7973  anguage}.\"\nsys
-00001ee0: 7465 6d5f 6d65 7373 6167 655f 7072 6f6d  tem_message_prom
-00001ef0: 7074 203d 2053 7973 7465 6d4d 6573 7361  pt = SystemMessa
-00001f00: 6765 5072 6f6d 7074 5465 6d70 6c61 7465  gePromptTemplate
-00001f10: 2e66 726f 6d5f 7465 6d70 6c61 7465 2874  .from_template(t
-00001f20: 656d 706c 6174 6529 5c6e 6875 6d61 6e5f  emplate)\nhuman_
-00001f30: 7465 6d70 6c61 7465 203d 205c 227b 7465  template = \"{te
-00001f40: 7874 7d5c 225c 6e68 756d 616e 5f6d 6573  xt}\"\nhuman_mes
-00001f50: 7361 6765 5f70 726f 6d70 7420 3d20 4875  sage_prompt = Hu
-00001f60: 6d61 6e4d 6573 7361 6765 5072 6f6d 7074  manMessagePrompt
-00001f70: 5465 6d70 6c61 7465 2e66 726f 6d5f 7465  Template.from_te
-00001f80: 6d70 6c61 7465 2868 756d 616e 5f74 656d  mplate(human_tem
-00001f90: 706c 6174 6529 5c6e 6368 6174 5f70 726f  plate)\nchat_pro
-00001fa0: 6d70 7420 3d20 4368 6174 5072 6f6d 7074  mpt = ChatPrompt
-00001fb0: 5465 6d70 6c61 7465 2e66 726f 6d5f 6d65  Template.from_me
-00001fc0: 7373 6167 6573 285b 7379 7374 656d 5f6d  ssages([system_m
-00001fd0: 6573 7361 6765 5f70 726f 6d70 742c 2068  essage_prompt, h
-00001fe0: 756d 616e 5f6d 6573 7361 6765 5f70 726f  uman_message_pro
-00001ff0: 6d70 745d 295c 6e5c 6e63 6861 696e 203d  mpt])\n\nchain =
-00002000: 204c 4c4d 4368 6169 6e28 6c6c 6d3d 6368   LLMChain(llm=ch
-00002010: 6174 2c20 7072 6f6d 7074 3d63 6861 745f  at, prompt=chat_
-00002020: 7072 6f6d 7074 295c 6e63 6861 696e 2e72  prompt)\nchain.r
-00002030: 756e 2869 6e70 7574 5f6c 616e 6775 6167  un(input_languag
-00002040: 653d 5c22 456e 676c 6973 685c 222c 206f  e=\"English\", o
-00002050: 7574 7075 745f 6c61 6e67 7561 6765 3d5c  utput_language=\
-00002060: 2246 7265 6e63 685c 222c 2074 6578 743d  "French\", text=
-00002070: 5c22 4920 6c6f 7665 2070 726f 6772 616d  \"I love program
-00002080: 6d69 6e67 2e5c 2229 5c6e 6060 6022 2c0d  ming.\")\n```",.
-00002090: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
-000020a0: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
-000020b0: 3a20 5b5d 2c0d 0a20 2020 2020 2020 2020  : [],..         
-000020c0: 2020 2022 6e6f 7465 7322 3a20 7b0d 0a20     "notes": {.. 
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000020e0: 6c65 7665 6c22 3a20 2268 6967 6822 0d0a  level": "high"..
-000020f0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00002100: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00002110: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00002120: 2020 2269 6422 3a20 226c 616e 6763 6861    "id": "langcha
-00002130: 696e 2d39 222c 0d0a 2020 2020 2020 2020  in-9",..        
-00002140: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
-00002150: 2254 656c 6c20 6d65 2061 626f 7574 2074  "Tell me about t
-00002160: 6865 2060 5141 4765 6e65 7261 7469 6f6e  he `QAGeneration
-00002170: 4368 6169 6e60 2e22 2c0d 0a20 2020 2020  Chain`.",..     
-00002180: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
-00002190: 655f 616e 7377 6572 223a 2022 5468 6520  e_answer": "The 
-000021a0: 5141 4765 6e65 7261 7469 6f6e 4368 6169  QAGenerationChai
-000021b0: 6e20 6973 2061 2063 6861 696e 2069 6e20  n is a chain in 
-000021c0: 4c61 6e67 4368 6169 6e20 7468 6174 2067  LangChain that g
-000021d0: 656e 6572 6174 6573 2071 7565 7374 696f  enerates questio
-000021e0: 6e2d 616e 7377 6572 2070 6169 7273 206f  n-answer pairs o
-000021f0: 7665 7220 6120 7370 6563 6966 6963 2064  ver a specific d
-00002200: 6f63 756d 656e 742e 2049 7420 6973 2061  ocument. It is a
-00002210: 2075 7365 6675 6c20 746f 6f6c 2066 6f72   useful tool for
-00002220: 2067 656e 6572 6174 696e 6720 6576 616c   generating eval
-00002230: 7561 7469 6f6e 2064 6174 6120 666f 7220  uation data for 
-00002240: 7175 6573 7469 6f6e 2d61 6e73 7765 7269  question-answeri
-00002250: 6e67 2074 6173 6b73 2077 6865 6e20 796f  ng tasks when yo
-00002260: 7520 646f 6e27 7420 6861 7665 2061 206c  u don't have a l
-00002270: 6172 6765 2064 6174 6173 6574 206f 6620  arge dataset of 
-00002280: 6578 616d 706c 6573 2e20 5468 6520 5141  examples. The QA
-00002290: 4765 6e65 7261 7469 6f6e 4368 6169 6e20  GenerationChain 
-000022a0: 7461 6b65 7320 6120 646f 6375 6d65 6e74  takes a document
-000022b0: 2061 7320 696e 7075 7420 616e 6420 6765   as input and ge
-000022c0: 6e65 7261 7465 7320 7175 6573 7469 6f6e  nerates question
-000022d0: 2d61 6e73 7765 7220 7061 6972 7320 7468  -answer pairs th
-000022e0: 6174 2063 616e 2062 6520 7573 6564 2074  at can be used t
-000022f0: 6f20 6576 616c 7561 7465 2071 7565 7374  o evaluate quest
-00002300: 696f 6e2d 616e 7377 6572 696e 6720 7379  ion-answering sy
-00002310: 7374 656d 732e 2054 6869 7320 616c 6c6f  stems. This allo
-00002320: 7773 2079 6f75 2074 6f20 6576 616c 7561  ws you to evalua
-00002330: 7465 2074 6865 2070 6572 666f 726d 616e  te the performan
-00002340: 6365 206f 6620 796f 7572 2071 7565 7374  ce of your quest
-00002350: 696f 6e2d 616e 7377 6572 696e 6720 7379  ion-answering sy
-00002360: 7374 656d 2077 6974 686f 7574 2074 6865  stem without the
-00002370: 206e 6565 6420 666f 7220 6120 6c61 7267   need for a larg
-00002380: 6520 616d 6f75 6e74 206f 6620 7072 652d  e amount of pre-
-00002390: 6578 6973 7469 6e67 2064 6174 612e 222c  existing data.",
-000023a0: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-000023b0: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-000023c0: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-000023d0: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 226c 6576 656c 223a 2022 6c6f 7722 0d0a  "level": "low"..
-00002400: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00002410: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00002420: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00002430: 2020 2269 6422 3a20 226c 616e 6763 6861    "id": "langcha
-00002440: 696e 2d31 3022 2c0d 0a20 2020 2020 2020  in-10",..       
-00002450: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
-00002460: 2022 486f 7720 646f 2049 2072 6575 7365   "How do I reuse
-00002470: 2061 6e20 6578 6973 7469 6e67 2060 5164   an existing `Qd
-00002480: 7261 6e74 6020 636f 6c6c 6563 7469 6f6e  rant` collection
-00002490: 3f20 5072 6f76 6964 6520 616e 2065 7861  ? Provide an exa
-000024a0: 6d70 6c65 2e22 2c0d 0a20 2020 2020 2020  mple.",..       
-000024b0: 2020 2020 2022 7265 6665 7265 6e63 655f       "reference_
-000024c0: 616e 7377 6572 223a 2022 4966 2079 6f75  answer": "If you
-000024d0: 2077 616e 7420 746f 2072 6575 7365 2074   want to reuse t
-000024e0: 6865 2065 7869 7374 696e 6720 636f 6c6c  he existing coll
-000024f0: 6563 7469 6f6e 2c20 796f 7520 6361 6e20  ection, you can 
-00002500: 616c 7761 7973 2063 7265 6174 6520 616e  always create an
-00002510: 2069 6e73 7461 6e63 6520 6f66 c2a0 5164   instance of..Qd
-00002520: 7261 6e74 c2a0 6f6e 2079 6f75 7220 6f77  rant..on your ow
-00002530: 6e20 616e 6420 7061 7373 2074 6865 c2a0  n and pass the..
-00002540: 5164 7261 6e74 436c 6965 6e74 c2a0 696e  QdrantClient..in
-00002550: 7374 616e 6365 2077 6974 6820 7468 6520  stance with the 
-00002560: 636f 6e6e 6563 7469 6f6e 2064 6574 6169  connection detai
-00002570: 6c73 2e5c 6e5c 6e60 6060 7079 7468 6f6e  ls.\n\n```python
-00002580: 5c6e 696d 706f 7274 2071 6472 616e 745f  \nimport qdrant_
-00002590: 636c 6965 6e74 5c6e 5c6e 636c 6965 6e74  client\n\nclient
-000025a0: 203d 2071 6472 616e 745f 636c 6965 6e74   = qdrant_client
-000025b0: 2e51 6472 616e 7443 6c69 656e 7428 7061  .QdrantClient(pa
-000025c0: 7468 3d5c 222f 746d 702f 6c6f 6361 6c5f  th=\"/tmp/local_
-000025d0: 7164 7261 6e74 5c22 2c20 7072 6566 6572  qdrant\", prefer
-000025e0: 5f67 7270 633d 5472 7565 295c 6e71 6472  _grpc=True)\nqdr
-000025f0: 616e 7420 3d20 5164 7261 6e74 2863 6c69  ant = Qdrant(cli
-00002600: 656e 743d 636c 6965 6e74 2c20 636f 6c6c  ent=client, coll
-00002610: 6563 7469 6f6e 5f6e 616d 653d 5c22 6d79  ection_name=\"my
-00002620: 5f64 6f63 756d 656e 7473 5c22 2c20 656d  _documents\", em
-00002630: 6265 6464 696e 6773 3d65 6d62 6564 6469  beddings=embeddi
-00002640: 6e67 7329 5c6e 6060 6022 2c0d 0a20 2020  ngs)\n```",..   
-00002650: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
-00002660: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
-00002670: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002680: 6e6f 7465 7322 3a20 7b0d 0a20 2020 2020  notes": {..     
-00002690: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
-000026a0: 6c22 3a20 2268 6967 6822 0d0a 2020 2020  l": "high"..    
-000026b0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-000026c0: 2020 207d 2c0d 0a20 2020 2020 2020 207b     },..        {
-000026d0: 0d0a 2020 2020 2020 2020 2020 2020 2269  ..            "i
-000026e0: 6422 3a20 226c 616e 6763 6861 696e 2d31  d": "langchain-1
-000026f0: 3122 2c0d 0a20 2020 2020 2020 2020 2020  1",..           
-00002700: 2022 7175 6573 7469 6f6e 223a 2022 5768   "question": "Wh
-00002710: 6174 2064 6f65 7320 7468 6520 606d 6178  at does the `max
-00002720: 5f6d 6172 6769 6e61 6c5f 7265 6c65 7661  _marginal_releva
-00002730: 6e63 655f 7365 6172 6368 6020 6675 6e63  nce_search` func
-00002740: 7469 6f6e 2064 6f3f 222c 0d0a 2020 2020  tion do?",..    
-00002750: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
-00002760: 6365 5f61 6e73 7765 7222 3a20 2254 6865  ce_answer": "The
-00002770: 2060 6d61 785f 6d61 7267 696e 616c 5f72   `max_marginal_r
-00002780: 656c 6576 616e 6365 5f73 6561 7263 6860  elevance_search`
-00002790: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
-000027a0: 7320 6120 6c69 7374 206f 6620 646f 6375  s a list of docu
-000027b0: 6d65 6e74 7320 7365 6c65 6374 6564 2075  ments selected u
-000027c0: 7369 6e67 2074 6865 206d 6178 696d 616c  sing the maximal
-000027d0: 206d 6172 6769 6e61 6c20 7265 6c65 7661   marginal releva
-000027e0: 6e63 6520 616c 676f 7269 7468 6d2c 2077  nce algorithm, w
-000027f0: 6869 6368 206f 7074 696d 697a 6573 2066  hich optimizes f
-00002800: 6f72 2073 696d 696c 6172 6974 7920 746f  or similarity to
-00002810: 2074 6865 2071 7565 7279 2061 6e64 2064   the query and d
-00002820: 6976 6572 7369 7479 2061 6d6f 6e67 2074  iversity among t
-00002830: 6865 2073 656c 6563 7465 6420 646f 6375  he selected docu
-00002840: 6d65 6e74 732e 222c 0d0a 2020 2020 2020  ments.",..      
-00002850: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
-00002860: 6f70 6572 7469 6573 223a 205b 5d2c 0d0a  operties": [],..
-00002870: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
-00002880: 6573 223a 207b 0d0a 2020 2020 2020 2020  es": {..        
-00002890: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
-000028a0: 2022 6c6f 7722 0d0a 2020 2020 2020 2020   "low"..        
-000028b0: 2020 2020 7d0d 0a20 2020 2020 2020 207d      }..        }
-000028c0: 2c0d 0a20 2020 2020 2020 207b 0d0a 2020  ,..        {..  
-000028d0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-000028e0: 226c 616e 6763 6861 696e 2d31 3222 2c0d  "langchain-12",.
-000028f0: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
-00002900: 6573 7469 6f6e 223a 2022 5768 6174 2069  estion": "What i
-00002910: 7320 7468 6520 7075 7270 6f73 6520 6f66  s the purpose of
-00002920: 2074 6865 2060 5164 7261 6e74 6020 636c   the `Qdrant` cl
-00002930: 6173 733f 222c 0d0a 2020 2020 2020 2020  ass?",..        
-00002940: 2020 2020 2272 6566 6572 656e 6365 5f61      "reference_a
-00002950: 6e73 7765 7222 3a20 2254 6865 2070 7572  nswer": "The pur
-00002960: 706f 7365 206f 6620 7468 6520 5164 7261  pose of the Qdra
-00002970: 6e74 2063 6c61 7373 2069 7320 746f 2073  nt class is to s
-00002980: 6572 7665 2061 7320 6120 7772 6170 7065  erve as a wrappe
-00002990: 7220 6172 6f75 6e64 2074 6865 2051 6472  r around the Qdr
-000029a0: 616e 7420 7665 6374 6f72 2064 6174 6162  ant vector datab
-000029b0: 6173 652e 222c 0d0a 2020 2020 2020 2020  ase.",..        
-000029c0: 2020 2020 2261 6e73 7765 725f 7072 6f70      "answer_prop
-000029d0: 6572 7469 6573 223a 205b 5d2c 0d0a 2020  erties": [],..  
-000029e0: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
-000029f0: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00002a00: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
-00002a10: 6d69 6422 0d0a 2020 2020 2020 2020 2020  mid"..          
-00002a20: 2020 7d0d 0a20 2020 2020 2020 207d 2c0d    }..        },.
-00002a30: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-00002a40: 2020 2020 2020 2020 2269 6422 3a20 226c          "id": "l
-00002a50: 616e 6763 6861 696e 2d31 3322 2c0d 0a20  angchain-13",.. 
-00002a60: 2020 2020 2020 2020 2020 2022 7175 6573             "ques
-00002a70: 7469 6f6e 223a 2022 5768 6174 2064 6f65  tion": "What doe
-00002a80: 7320 7468 6520 6073 6176 655f 636f 6e74  s the `save_cont
-00002a90: 6578 7460 206d 6574 686f 6420 6f66 2043  ext` method of C
-00002aa0: 6f6e 7665 7273 6174 696f 6e45 6e74 6974  onversationEntit
-00002ab0: 794d 656d 6f72 7920 646f 3f22 2c0d 0a20  yMemory do?",.. 
-00002ac0: 2020 2020 2020 2020 2020 2022 7265 6665             "refe
-00002ad0: 7265 6e63 655f 616e 7377 6572 223a 2022  rence_answer": "
-00002ae0: 5468 6520 6073 6176 655f 636f 6e74 6578  The `save_contex
-00002af0: 7460 206d 6574 686f 6420 7361 7665 7320  t` method saves 
-00002b00: 7468 6520 636f 6e74 6578 7420 6672 6f6d  the context from
-00002b10: 2074 6865 2063 6f6e 7665 7273 6174 696f   the conversatio
-00002b20: 6e20 6869 7374 6f72 7920 746f 2074 6865  n history to the
-00002b30: 2065 6e74 6974 7920 7374 6f72 6520 6279   entity store by
-00002b40: 2067 656e 6572 6174 696e 6720 7375 6d6d   generating summ
-00002b50: 6172 6965 7320 666f 7220 6561 6368 2065  aries for each e
-00002b60: 6e74 6974 7920 696e 2074 6865 2065 6e74  ntity in the ent
-00002b70: 6974 7920 6361 6368 652e 222c 0d0a 2020  ity cache.",..  
-00002b80: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
-00002b90: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
-00002ba0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00002bb0: 226e 6f74 6573 223a 207b 0d0a 2020 2020  "notes": {..    
-00002bc0: 2020 2020 2020 2020 2020 2020 226c 6576              "lev
-00002bd0: 656c 223a 2022 6d69 6422 0d0a 2020 2020  el": "mid"..    
-00002be0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00002bf0: 2020 207d 2c0d 0a20 2020 2020 2020 207b     },..        {
-00002c00: 0d0a 2020 2020 2020 2020 2020 2020 2269  ..            "i
-00002c10: 6422 3a20 226c 616e 6763 6861 696e 2d31  d": "langchain-1
-00002c20: 3422 2c0d 0a20 2020 2020 2020 2020 2020  4",..           
-00002c30: 2022 7175 6573 7469 6f6e 223a 2022 5768   "question": "Wh
-00002c40: 6174 2069 7320 7468 6520 7573 6520 6f66  at is the use of
-00002c50: 2074 6865 2060 436f 6e76 6572 7361 7469   the `Conversati
-00002c60: 6f6e 4275 6666 6572 4d65 6d6f 7279 6020  onBufferMemory` 
-00002c70: 636c 6173 733f 222c 0d0a 2020 2020 2020  class?",..      
-00002c80: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
-00002c90: 5f61 6e73 7765 7222 3a20 2254 6865 2070  _answer": "The p
-00002ca0: 7572 706f 7365 206f 6620 7468 6520 436f  urpose of the Co
-00002cb0: 6e76 6572 7361 7469 6f6e 4275 6666 6572  nversationBuffer
-00002cc0: 4d65 6d6f 7279 2063 6c61 7373 2069 7320  Memory class is 
-00002cd0: 746f 2073 746f 7265 2063 6f6e 7665 7273  to store convers
-00002ce0: 6174 696f 6e20 6d65 6d6f 7279 2069 6e20  ation memory in 
-00002cf0: 6120 7374 7269 6e67 2062 7566 6665 722e  a string buffer.
-00002d00: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002d10: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
-00002d20: 6573 223a 205b 5d2c 0d0a 2020 2020 2020  es": [],..      
-00002d30: 2020 2020 2020 226e 6f74 6573 223a 207b        "notes": {
-00002d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002d50: 2020 226c 6576 656c 223a 2022 6d69 6422    "level": "mid"
-00002d60: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-00002d70: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00002d80: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00002d90: 2020 2020 2269 6422 3a20 226c 616e 6763      "id": "langc
-00002da0: 6861 696e 2d31 3522 2c0d 0a20 2020 2020  hain-15",..     
-00002db0: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
-00002dc0: 223a 2022 5768 6174 2069 7320 6120 7072  ": "What is a pr
-00002dd0: 6f6d 7074 2074 656d 706c 6174 653f 222c  ompt template?",
-00002de0: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-00002df0: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-00002e00: 3a20 2241 2070 726f 6d70 7420 7465 6d70  : "A prompt temp
-00002e10: 6c61 7465 2072 6566 6572 7320 746f 2061  late refers to a
-00002e20: 2072 6570 726f 6475 6369 626c 6520 7761   reproducible wa
-00002e30: 7920 746f 2067 656e 6572 6174 6520 6120  y to generate a 
-00002e40: 7072 6f6d 7074 2e20 4974 2063 6f6e 7461  prompt. It conta
-00002e50: 696e 7320 6120 7465 7874 2073 7472 696e  ins a text strin
-00002e60: 6720 285c 2274 6865 2074 656d 706c 6174  g (\"the templat
-00002e70: 655c 2229 2074 6861 7420 6361 6e20 7461  e\") that can ta
-00002e80: 6b65 2069 6e20 6120 7365 7420 6f66 2070  ke in a set of p
-00002e90: 6172 616d 6574 6572 7320 6672 6f6d 2074  arameters from t
-00002ea0: 6865 2065 6e64 2075 7365 7220 616e 6420  he end user and 
-00002eb0: 6765 6e65 7261 7465 7320 6120 7072 6f6d  generates a prom
-00002ec0: 7074 2e20 4120 7072 6f6d 7074 2074 656d  pt. A prompt tem
-00002ed0: 706c 6174 6520 6361 6e20 696e 636c 7564  plate can includ
-00002ee0: 6520 696e 7374 7275 6374 696f 6e73 2074  e instructions t
-00002ef0: 6f20 7468 6520 6c61 6e67 7561 6765 206d  o the language m
-00002f00: 6f64 656c 2c20 6120 7365 7420 6f66 2066  odel, a set of f
-00002f10: 6577 2d73 686f 7420 6578 616d 706c 6573  ew-shot examples
-00002f20: 2074 6f20 6865 6c70 2074 6865 206c 616e   to help the lan
-00002f30: 6775 6167 6520 6d6f 6465 6c20 6765 6e65  guage model gene
-00002f40: 7261 7465 2061 2062 6574 7465 7220 7265  rate a better re
-00002f50: 7370 6f6e 7365 2c20 616e 6420 6120 7175  sponse, and a qu
-00002f60: 6573 7469 6f6e 2074 6f20 7468 6520 6c61  estion to the la
-00002f70: 6e67 7561 6765 206d 6f64 656c 2e20 5072  nguage model. Pr
-00002f80: 6f6d 7074 2074 656d 706c 6174 6573 2063  ompt templates c
-00002f90: 616e 2062 6520 6372 6561 7465 6420 7573  an be created us
-00002fa0: 696e 6720 7468 65c2 a050 726f 6d70 7454  ing the..PromptT
-00002fb0: 656d 706c 6174 65c2 a063 6c61 7373 2069  emplate..class i
-00002fc0: 6e20 4c61 6e67 4368 6169 6e2e 222c 0d0a  n LangChain.",..
-00002fd0: 2020 2020 2020 2020 2020 2020 2261 6e73              "ans
-00002fe0: 7765 725f 7072 6f70 6572 7469 6573 223a  wer_properties":
-00002ff0: 205b 5d2c 0d0a 2020 2020 2020 2020 2020   [],..          
-00003000: 2020 226e 6f74 6573 223a 207b 0d0a 2020    "notes": {..  
-00003010: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00003020: 6576 656c 223a 2022 6d69 6422 0d0a 2020  evel": "mid"..  
-00003030: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00003040: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00003050: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00003060: 2269 6422 3a20 226c 616e 6763 6861 696e  "id": "langchain
-00003070: 2d31 3622 2c0d 0a20 2020 2020 2020 2020  -16",..         
-00003080: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
-00003090: 4973 2074 6865 7265 2061 2063 6163 6869  Is there a cachi
-000030a0: 6e67 206d 6563 6861 6e69 736d 2066 6f72  ng mechanism for
-000030b0: 204c 4c4d 733f 222c 0d0a 2020 2020 2020   LLMs?",..      
-000030c0: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
-000030d0: 5f61 6e73 7765 7222 3a20 2259 6573 2c20  _answer": "Yes, 
-000030e0: 7468 6572 6520 6973 2061 2063 6163 6869  there is a cachi
-000030f0: 6e67 206d 6563 6861 6e69 736d 2066 6f72  ng mechanism for
-00003100: 204c 4c4d 7320 284c 616e 6775 6167 6520   LLMs (Language 
-00003110: 4d6f 6465 6c73 292e 2043 6163 6869 6e67  Models). Caching
-00003120: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00003130: 7361 7665 206d 6f6e 6579 2062 7920 7265  save money by re
-00003140: 6475 6369 6e67 2074 6865 206e 756d 6265  ducing the numbe
-00003150: 7220 6f66 2041 5049 2063 616c 6c73 206d  r of API calls m
-00003160: 6164 6520 746f 2074 6865 204c 4c4d 2070  ade to the LLM p
-00003170: 726f 7669 6465 7220 616e 6420 746f 2073  rovider and to s
-00003180: 7065 6564 2075 7020 6170 706c 6963 6174  peed up applicat
-00003190: 696f 6e73 2062 7920 7265 6475 6369 6e67  ions by reducing
-000031a0: 2074 6865 206e 756d 6265 7220 6f66 2041   the number of A
-000031b0: 5049 2063 616c 6c73 2e20 5468 6572 6520  PI calls. There 
-000031c0: 6172 6520 6469 6666 6572 656e 7420 6361  are different ca
-000031d0: 6368 696e 6720 6f70 7469 6f6e 7320 6176  ching options av
-000031e0: 6169 6c61 626c 6520 7375 6368 2061 7320  ailable such as 
-000031f0: 496e 204d 656d 6f72 7920 4361 6368 652c  In Memory Cache,
-00003200: 2053 514c 6974 6520 4361 6368 652c 2052   SQLite Cache, R
-00003210: 6564 6973 2043 6163 6865 2c20 5365 6d61  edis Cache, Sema
-00003220: 6e74 6963 2043 6163 6865 2c20 4750 5443  ntic Cache, GPTC
-00003230: 6163 6865 2c20 4d6f 6d65 6e74 6f20 4361  ache, Momento Ca
-00003240: 6368 652c 2061 6e64 2053 514c 416c 6368  che, and SQLAlch
-00003250: 656d 7920 4361 6368 652e 2054 6865 7365  emy Cache. These
-00003260: 2063 6163 6869 6e67 206f 7074 696f 6e73   caching options
-00003270: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00003280: 6361 6368 6520 7072 6f6d 7074 7320 616e  cache prompts an
-00003290: 6420 7265 7370 6f6e 7365 732c 2061 6e64  d responses, and
-000032a0: 2073 6f6d 6520 6f66 2074 6865 6d20 6576   some of them ev
-000032b0: 656e 2073 7570 706f 7274 2063 6163 6869  en support cachi
-000032c0: 6e67 2062 6173 6564 206f 6e20 7365 6d61  ng based on sema
-000032d0: 6e74 6963 2073 696d 696c 6172 6974 792e  ntic similarity.
-000032e0: 2041 6464 6974 696f 6e61 6c6c 792c 2063   Additionally, c
-000032f0: 6163 6869 6e67 2063 616e 2062 6520 7475  aching can be tu
-00003300: 726e 6564 206f 6666 2066 6f72 2073 7065  rned off for spe
-00003310: 6369 6669 6320 4c4c 4d73 2069 6620 6465  cific LLMs if de
-00003320: 7369 7265 642e 222c 0d0a 2020 2020 2020  sired.",..      
-00003330: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
-00003340: 6f70 6572 7469 6573 223a 205b 5d2c 0d0a  operties": [],..
-00003350: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
-00003360: 6573 223a 207b 0d0a 2020 2020 2020 2020  es": {..        
-00003370: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
-00003380: 2022 6d69 6422 0d0a 2020 2020 2020 2020   "mid"..        
-00003390: 2020 2020 7d0d 0a20 2020 2020 2020 207d      }..        }
-000033a0: 2c0d 0a20 2020 2020 2020 207b 0d0a 2020  ,..        {..  
-000033b0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-000033c0: 226c 616e 6763 6861 696e 2d31 3722 2c0d  "langchain-17",.
-000033d0: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
-000033e0: 6573 7469 6f6e 223a 2022 4769 7665 206d  estion": "Give m
-000033f0: 6520 6120 6c69 7374 206f 6620 7468 6520  e a list of the 
-00003400: 6d61 696e 2063 6f6d 706f 6e65 6e74 7320  main components 
-00003410: 6f66 204c 616e 6763 6861 696e 2e22 2c0d  of Langchain.",.
-00003420: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00003430: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
-00003440: 2022 5468 6520 6d61 696e 2063 6f6d 706f   "The main compo
-00003450: 6e65 6e74 7320 6f66 204c 616e 6743 6861  nents of LangCha
-00003460: 696e 2061 7265 2061 7320 666f 6c6c 6f77  in are as follow
-00003470: 733a 5c6e 5c6e 4d6f 6465 6c73 3a20 4c61  s:\n\nModels: La
-00003480: 6e67 4368 6169 6e20 7375 7070 6f72 7473  ngChain supports
-00003490: 2076 6172 696f 7573 206d 6f64 656c 2074   various model t
-000034a0: 7970 6573 2061 6e64 206d 6f64 656c 2069  ypes and model i
-000034b0: 6e74 6567 7261 7469 6f6e 732e 5c6e 5072  ntegrations.\nPr
-000034c0: 6f6d 7074 733a 2054 6869 7320 6d6f 6475  ompts: This modu
-000034d0: 6c65 2069 6e63 6c75 6465 7320 7072 6f6d  le includes prom
-000034e0: 7074 206d 616e 6167 656d 656e 742c 2070  pt management, p
-000034f0: 726f 6d70 7420 6f70 7469 6d69 7a61 7469  rompt optimizati
-00003500: 6f6e 2c20 616e 6420 7072 6f6d 7074 2073  on, and prompt s
-00003510: 6572 6961 6c69 7a61 7469 6f6e 2e5c 6e4d  erialization.\nM
-00003520: 656d 6f72 793a 204c 616e 6743 6861 696e  emory: LangChain
-00003530: 2070 726f 7669 6465 7320 6120 7374 616e   provides a stan
-00003540: 6461 7264 2069 6e74 6572 6661 6365 2066  dard interface f
-00003550: 6f72 206d 656d 6f72 792c 2061 2063 6f6c  or memory, a col
-00003560: 6c65 6374 696f 6e20 6f66 206d 656d 6f72  lection of memor
-00003570: 7920 696d 706c 656d 656e 7461 7469 6f6e  y implementation
-00003580: 732c 2061 6e64 2065 7861 6d70 6c65 7320  s, and examples 
-00003590: 6f66 2063 6861 696e 732f 6167 656e 7473  of chains/agents
-000035a0: 2074 6861 7420 7573 6520 6d65 6d6f 7279   that use memory
-000035b0: 2e5c 6e49 6e64 6578 6573 3a20 5468 6973  .\nIndexes: This
-000035c0: 206d 6f64 756c 6520 636f 7665 7273 2062   module covers b
-000035d0: 6573 7420 7072 6163 7469 6365 7320 666f  est practices fo
-000035e0: 7220 636f 6d62 696e 696e 6720 6c61 6e67  r combining lang
-000035f0: 7561 6765 206d 6f64 656c 7320 7769 7468  uage models with
-00003600: 2079 6f75 7220 6f77 6e20 7465 7874 2064   your own text d
-00003610: 6174 612e 5c6e 4368 6169 6e73 3a20 4c61  ata.\nChains: La
-00003620: 6e67 4368 6169 6e20 7072 6f76 6964 6573  ngChain provides
-00003630: 2061 2073 7461 6e64 6172 6420 696e 7465   a standard inte
-00003640: 7266 6163 6520 666f 7220 6368 6169 6e73  rface for chains
-00003650: 2c20 696e 7465 6772 6174 696f 6e73 2077  , integrations w
-00003660: 6974 6820 6f74 6865 7220 746f 6f6c 732c  ith other tools,
-00003670: 2061 6e64 2065 6e64 2d74 6f2d 656e 6420   and end-to-end 
-00003680: 6368 6169 6e73 2066 6f72 2063 6f6d 6d6f  chains for commo
-00003690: 6e20 6170 706c 6963 6174 696f 6e73 2e5c  n applications.\
-000036a0: 6e41 6765 6e74 733a 204c 616e 6743 6861  nAgents: LangCha
-000036b0: 696e 2070 726f 7669 6465 7320 6120 7374  in provides a st
-000036c0: 616e 6461 7264 2069 6e74 6572 6661 6365  andard interface
-000036d0: 2066 6f72 2061 6765 6e74 732c 2061 2073   for agents, a s
-000036e0: 656c 6563 7469 6f6e 206f 6620 6167 656e  election of agen
-000036f0: 7473 2074 6f20 6368 6f6f 7365 2066 726f  ts to choose fro
-00003700: 6d2c 2061 6e64 2065 7861 6d70 6c65 7320  m, and examples 
-00003710: 6f66 2065 6e64 2d74 6f2d 656e 6420 6167  of end-to-end ag
-00003720: 656e 7473 2e5c 6e5c 6e54 6865 7365 2063  ents.\n\nThese c
-00003730: 6f6d 706f 6e65 6e74 7320 6361 6e20 6265  omponents can be
-00003740: 2075 7365 6420 696e 2076 6172 696f 7573   used in various
-00003750: 2077 6179 732c 2069 6e63 6c75 6469 6e67   ways, including
-00003760: 2066 6f72 2070 6572 736f 6e61 6c20 6173   for personal as
-00003770: 7369 7374 616e 7473 2c20 7175 6573 7469  sistants, questi
-00003780: 6f6e 2061 6e73 7765 7269 6e67 2c20 6368  on answering, ch
-00003790: 6174 626f 7473 2c20 7175 6572 7969 6e67  atbots, querying
-000037a0: 2074 6162 756c 6172 2064 6174 612c 2069   tabular data, i
-000037b0: 6e74 6572 6163 7469 6e67 2077 6974 6820  nteracting with 
-000037c0: 4150 4973 2c20 6578 7472 6163 7469 6f6e  APIs, extraction
-000037d0: 2c20 7375 6d6d 6172 697a 6174 696f 6e2c  , summarization,
-000037e0: 2061 6e64 2065 7661 6c75 6174 696f 6e2e   and evaluation.
-000037f0: 2041 6464 6974 696f 6e61 6c6c 792c 204c   Additionally, L
-00003800: 616e 6743 6861 696e 2070 726f 7669 6465  angChain provide
-00003810: 7320 7265 6665 7265 6e63 6520 646f 6375  s reference docu
-00003820: 6d65 6e74 6174 696f 6e20 666f 7220 616c  mentation for al
-00003830: 6c20 6974 7320 6665 6174 7572 6573 2061  l its features a
-00003840: 6e64 2061 6e20 6563 6f73 7973 7465 6d20  nd an ecosystem 
-00003850: 666f 7220 696e 7465 6772 6174 696e 6720  for integrating 
-00003860: 7769 7468 206f 7468 6572 2063 6f6d 7061  with other compa
-00003870: 6e69 6573 2f70 726f 6475 6374 732e 222c  nies/products.",
-00003880: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-00003890: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-000038a0: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-000038b0: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 226c 6576 656c 223a 2022 6869 6768 220d  "level": "high".
-000038e0: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-000038f0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00003900: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00003910: 2020 2022 6964 223a 2022 6c61 6e67 6368     "id": "langch
-00003920: 6169 6e2d 3138 222c 0d0a 2020 2020 2020  ain-18",..      
-00003930: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00003940: 3a20 2244 6966 6665 7265 6e63 6520 622f  : "Difference b/
-00003950: 7420 6120 7265 6163 7420 6167 656e 7420  t a react agent 
-00003960: 616e 6420 6120 706c 616e 2d61 6e64 2d65  and a plan-and-e
-00003970: 7865 6375 7465 2061 6765 6e74 3f22 2c0d  xecute agent?",.
-00003980: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-00003990: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
-000039a0: 2022 4120 5265 4163 7420 6167 656e 7420   "A ReAct agent 
-000039b0: 616e 6420 6120 706c 616e 2d61 6e64 2d65  and a plan-and-e
-000039c0: 7865 6375 7465 2061 6765 6e74 2061 7265  xecute agent are
-000039d0: 2074 776f 2064 6966 6665 7265 6e74 2074   two different t
-000039e0: 7970 6573 206f 6620 6167 656e 7473 2069  ypes of agents i
-000039f0: 6e20 7468 6520 4c61 6e67 4368 6169 6e20  n the LangChain 
-00003a00: 6672 616d 6577 6f72 6b2e 5c6e 5c6e 4120  framework.\n\nA 
-00003a10: 5265 4163 7420 6167 656e 742c 2077 6869  ReAct agent, whi
-00003a20: 6368 2073 7461 6e64 7320 666f 7220 5c22  ch stands for \"
-00003a30: 5265 6163 7469 6f6e 2041 6765 6e74 2c5c  Reaction Agent,\
-00003a40: 2220 7573 6573 2074 6865 2052 6541 6374  " uses the ReAct
-00003a50: 2066 7261 6d65 776f 726b 2074 6f20 6465   framework to de
-00003a60: 7465 726d 696e 6520 7768 6963 6820 746f  termine which to
-00003a70: 6f6c 2074 6f20 7573 6520 6261 7365 6420  ol to use based 
-00003a80: 6f6e 2074 6865 2074 6f6f 6c27 7320 6465  on the tool's de
-00003a90: 7363 7269 7074 696f 6e2e 2049 7420 6361  scription. It ca
-00003aa0: 6e20 7573 6520 6d75 6c74 6970 6c65 2074  n use multiple t
-00003ab0: 6f6f 6c73 2061 6e64 2069 7320 6465 7369  ools and is desi
-00003ac0: 676e 6564 2074 6f20 6265 2075 7365 6420  gned to be used 
-00003ad0: 696e 2063 6f6e 7665 7273 6174 696f 6e61  in conversationa
-00003ae0: 6c20 7365 7474 696e 6773 2e20 4974 2075  l settings. It u
-00003af0: 7365 7320 6d65 6d6f 7279 2074 6f20 7265  ses memory to re
-00003b00: 6d65 6d62 6572 2070 7265 7669 6f75 7320  member previous 
-00003b10: 636f 6e76 6572 7361 7469 6f6e 2069 6e74  conversation int
-00003b20: 6572 6163 7469 6f6e 7320 616e 6420 6465  eractions and de
-00003b30: 6369 6465 7320 7468 6520 6e65 7874 2073  cides the next s
-00003b40: 7465 7020 7573 696e 6720 7468 6520 6869  tep using the hi
-00003b50: 7374 6f72 7920 6f66 2074 6f6f 6c73 2c20  story of tools, 
-00003b60: 746f 6f6c 2069 6e70 7574 732c 2061 6e64  tool inputs, and
-00003b70: 206f 6273 6572 7661 7469 6f6e 732e 2052   observations. R
-00003b80: 6541 6374 2061 6765 6e74 7320 6172 6520  eAct agents are 
-00003b90: 7375 6974 6162 6c65 2066 6f72 2073 6d61  suitable for sma
-00003ba0: 6c6c 2074 6173 6b73 2061 6e64 2061 7265  ll tasks and are
-00003bb0: 2077 7261 7070 6564 2069 6e20 6167 656e   wrapped in agen
-00003bc0: 7420 6578 6563 7574 6f72 732e 5c6e 5c6e  t executors.\n\n
-00003bd0: 4f6e 2074 6865 206f 7468 6572 2068 616e  On the other han
-00003be0: 642c 2061 2070 6c61 6e2d 616e 642d 6578  d, a plan-and-ex
-00003bf0: 6563 7574 6520 6167 656e 7420 706c 616e  ecute agent plan
-00003c00: 7320 7468 6520 6675 6c6c 2073 6571 7565  s the full seque
-00003c10: 6e63 6520 6f66 2073 7465 7073 2074 6f20  nce of steps to 
-00003c20: 6163 636f 6d70 6c69 7368 2061 6e20 6f62  accomplish an ob
-00003c30: 6a65 6374 6976 6520 616e 6420 7468 656e  jective and then
-00003c40: 2065 7865 6375 7465 7320 7468 6f73 6520   executes those 
-00003c50: 7374 6570 7320 696e 206f 7264 6572 2e20  steps in order. 
-00003c60: 5468 6520 706c 616e 6e69 6e67 2069 7320  The planning is 
-00003c70: 7573 7561 6c6c 7920 646f 6e65 2062 7920  usually done by 
-00003c80: 6120 6c61 6e67 7561 6765 206d 6f64 656c  a language model
-00003c90: 2028 4c4c 4d29 2c20 616e 6420 7468 6520   (LLM), and the 
-00003ca0: 6578 6563 7574 696f 6e20 6973 2064 6f6e  execution is don
-00003cb0: 6520 6279 2061 2073 6570 6172 6174 6520  e by a separate 
-00003cc0: 6167 656e 7420 6571 7569 7070 6564 2077  agent equipped w
-00003cd0: 6974 6820 746f 6f6c 732e 2050 6c61 6e2d  ith tools. Plan-
-00003ce0: 616e 642d 6578 6563 7574 6520 6167 656e  and-execute agen
-00003cf0: 7473 2061 7265 2062 6574 7465 7220 7375  ts are better su
-00003d00: 6974 6564 2066 6f72 2063 6f6d 706c 6578  ited for complex
-00003d10: 206f 7220 6c6f 6e67 2d72 756e 6e69 6e67   or long-running
-00003d20: 2074 6173 6b73 2074 6861 7420 7265 7175   tasks that requ
-00003d30: 6972 6520 6d61 696e 7461 696e 696e 6720  ire maintaining 
-00003d40: 6c6f 6e67 2d74 6572 6d20 6f62 6a65 6374  long-term object
-00003d50: 6976 6573 2061 6e64 2066 6f63 7573 2e5c  ives and focus.\
-00003d60: 6e5c 6e49 6e20 7375 6d6d 6172 792c 2061  n\nIn summary, a
-00003d70: 2052 6541 6374 2061 6765 6e74 2075 7365   ReAct agent use
-00003d80: 7320 7468 6520 5265 4163 7420 6672 616d  s the ReAct fram
-00003d90: 6577 6f72 6b20 746f 2064 6563 6964 6520  ework to decide 
-00003da0: 7768 6963 6820 746f 6f6c 2074 6f20 7573  which tool to us
-00003db0: 6520 6261 7365 6420 6f6e 2074 6865 2074  e based on the t
-00003dc0: 6f6f 6c27 7320 6465 7363 7269 7074 696f  ool's descriptio
-00003dd0: 6e20 616e 6420 6973 2064 6573 6967 6e65  n and is designe
-00003de0: 6420 666f 7220 636f 6e76 6572 7361 7469  d for conversati
-00003df0: 6f6e 616c 2073 6574 7469 6e67 732e 2041  onal settings. A
-00003e00: 2070 6c61 6e2d 616e 642d 6578 6563 7574   plan-and-execut
-00003e10: 6520 6167 656e 7420 706c 616e 7320 7468  e agent plans th
-00003e20: 6520 6675 6c6c 2073 6571 7565 6e63 6520  e full sequence 
-00003e30: 6f66 2073 7465 7073 2061 6e64 2065 7865  of steps and exe
-00003e40: 6375 7465 7320 7468 656d 2069 6e20 6f72  cutes them in or
-00003e50: 6465 722c 206d 616b 696e 6720 6974 2073  der, making it s
-00003e60: 7569 7461 626c 6520 666f 7220 636f 6d70  uitable for comp
-00003e70: 6c65 7820 7461 736b 732e 222c 0d0a 2020  lex tasks.",..  
-00003e80: 2020 2020 2020 2020 2020 2261 6e73 7765            "answe
-00003e90: 725f 7072 6f70 6572 7469 6573 223a 205b  r_properties": [
-00003ea0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00003eb0: 226e 6f74 6573 223a 207b 0d0a 2020 2020  "notes": {..    
-00003ec0: 2020 2020 2020 2020 2020 2020 226c 6576              "lev
-00003ed0: 656c 223a 2022 6869 6768 220d 0a20 2020  el": "high"..   
-00003ee0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00003ef0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00003f00: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-00003f10: 6964 223a 2022 6c61 6e67 6368 6169 6e2d  id": "langchain-
-00003f20: 3139 222c 0d0a 2020 2020 2020 2020 2020  19",..          
-00003f30: 2020 2271 7565 7374 696f 6e22 3a20 2249    "question": "I
-00003f40: 7320 7468 6572 6520 6120 6053 656c 6651  s there a `SelfQ
-00003f50: 7565 7279 5265 7472 6965 7665 7260 2066  ueryRetriever` f
-00003f60: 6f72 2060 4d69 6c76 7573 603f 222c 0d0a  or `Milvus`?",..
-00003f70: 2020 2020 2020 2020 2020 2020 2272 6566              "ref
-00003f80: 6572 656e 6365 5f61 6e73 7765 7222 3a20  erence_answer": 
-00003f90: 224e 6f2e 2053 656c 6620 7175 6572 7969  "No. Self queryi
-00003fa0: 6e67 2066 6f72 204d 696c 7675 7320 6973  ng for Milvus is
-00003fb0: 206e 6f74 2073 7570 706f 7274 6564 2e22   not supported."
-00003fc0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00003fd0: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
-00003fe0: 7322 3a20 5b5d 2c0d 0a20 2020 2020 2020  s": [],..       
-00003ff0: 2020 2020 2022 6e6f 7465 7322 3a20 7b0d       "notes": {.
-00004000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004010: 2022 6c65 7665 6c22 3a20 226d 6964 220d   "level": "mid".
-00004020: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-00004030: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00004040: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00004050: 2020 2022 6964 223a 2022 6c61 6e67 6368     "id": "langch
-00004060: 6169 6e2d 3230 222c 0d0a 2020 2020 2020  ain-20",..      
-00004070: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00004080: 3a20 2248 6f77 2064 6f20 4920 6465 6669  : "How do I defi
-00004090: 6e65 2061 2063 7573 746f 6d20 746f 6f6c  ne a custom tool
-000040a0: 3f22 2c0d 0a20 2020 2020 2020 2020 2020  ?",..           
-000040b0: 2022 7265 6665 7265 6e63 655f 616e 7377   "reference_answ
-000040c0: 6572 223a 2022 546f 2064 6566 696e 6520  er": "To define 
-000040d0: 6120 6375 7374 6f6d 2074 6f6f 6c2c 2079  a custom tool, y
-000040e0: 6f75 2063 616e 2075 7365 2065 6974 6865  ou can use eithe
-000040f0: 7220 7468 6520 546f 6f6c 2064 6174 6163  r the Tool datac
-00004100: 6c61 7373 206f 7220 7375 6263 6c61 7373  lass or subclass
-00004110: 2074 6865 2042 6173 6554 6f6f 6c20 636c   the BaseTool cl
-00004120: 6173 732e 5c6e 5c6e 5573 696e 6720 7468  ass.\n\nUsing th
-00004130: 6520 546f 6f6c 2064 6174 6163 6c61 7373  e Tool dataclass
-00004140: 3a5c 6e49 6d70 6f72 7420 7468 6520 6e65  :\nImport the ne
-00004150: 6365 7373 6172 7920 6d6f 6475 6c65 733a  cessary modules:
-00004160: 2066 726f 6d20 6c61 6e67 6368 6169 6e20   from langchain 
-00004170: 696d 706f 7274 2054 6f6f 6c5c 6e44 6566  import Tool\nDef
-00004180: 696e 6520 7468 6520 746f 6f6c 2075 7369  ine the tool usi
-00004190: 6e67 2074 6865 2054 6f6f 6c20 6461 7461  ng the Tool data
-000041a0: 636c 6173 732c 2070 726f 7669 6469 6e67  class, providing
-000041b0: 2074 6865 2072 6571 7569 7265 6420 636f   the required co
-000041c0: 6d70 6f6e 656e 7473 2073 7563 6820 6173  mponents such as
-000041d0: 206e 616d 652c 2064 6573 6372 6970 7469   name, descripti
-000041e0: 6f6e 2c20 616e 6420 6675 6e63 7469 6f6e  on, and function
-000041f0: 2e5c 6e4f 7074 696f 6e61 6c6c 792c 2079  .\nOptionally, y
-00004200: 6f75 2063 616e 2064 6566 696e 6520 616e  ou can define an
-00004210: 2061 7267 735f 7363 6865 6d61 2074 6f20   args_schema to 
-00004220: 7072 6f76 6964 6520 6d6f 7265 2069 6e66  provide more inf
-00004230: 6f72 6d61 7469 6f6e 206f 7220 7661 6c69  ormation or vali
-00004240: 6461 7469 6f6e 2066 6f72 2065 7870 6563  dation for expec
-00004250: 7465 6420 7061 7261 6d65 7465 7273 2e5c  ted parameters.\
-00004260: 6e53 7562 636c 6173 7369 6e67 2074 6865  nSubclassing the
-00004270: 2042 6173 6554 6f6f 6c20 636c 6173 733a   BaseTool class:
-00004280: 5c6e 496d 706f 7274 2074 6865 206e 6563  \nImport the nec
-00004290: 6573 7361 7279 206d 6f64 756c 6573 3a20  essary modules: 
-000042a0: 6672 6f6d 206c 616e 6763 6861 696e 2069  from langchain i
-000042b0: 6d70 6f72 7420 4261 7365 546f 6f6c 5c6e  mport BaseTool\n
-000042c0: 4372 6561 7465 2061 2063 7573 746f 6d20  Create a custom 
-000042d0: 636c 6173 7320 7468 6174 2073 7562 636c  class that subcl
-000042e0: 6173 7365 7320 4261 7365 546f 6f6c 2e5c  asses BaseTool.\
-000042f0: 6e49 6d70 6c65 6d65 6e74 2074 6865 206e  nImplement the n
-00004300: 6563 6573 7361 7279 206d 6574 686f 6473  ecessary methods
-00004310: 2061 6e64 2069 6e73 7461 6e63 6520 7661   and instance va
-00004320: 7269 6162 6c65 7320 696e 2079 6f75 7220  riables in your 
-00004330: 6375 7374 6f6d 2063 6c61 7373 2e5c 6e41  custom class.\nA
-00004340: 6464 6974 696f 6e61 6c6c 792c 2074 6865  dditionally, the
-00004350: 7265 2069 7320 6120 4074 6f6f 6c20 6465  re is a @tool de
-00004360: 636f 7261 746f 7220 7072 6f76 6964 6564  corator provided
-00004370: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
-00004380: 6420 746f 2071 7569 636b 6c79 2063 7265  d to quickly cre
-00004390: 6174 6520 6120 546f 6f6c 2066 726f 6d20  ate a Tool from 
-000043a0: 6120 7369 6d70 6c65 2066 756e 6374 696f  a simple functio
-000043b0: 6e2e 2054 6865 2064 6563 6f72 6174 6f72  n. The decorator
-000043c0: 2075 7365 7320 7468 6520 6675 6e63 7469   uses the functi
-000043d0: 6f6e 206e 616d 6520 6173 2074 6865 2074  on name as the t
-000043e0: 6f6f 6c20 6e61 6d65 2062 7920 6465 6661  ool name by defa
-000043f0: 756c 7420 616e 6420 7468 6520 6675 6e63  ult and the func
-00004400: 7469 6f6e 2773 2064 6f63 7374 7269 6e67  tion's docstring
-00004410: 2061 7320 7468 6520 746f 6f6c 2773 2064   as the tool's d
-00004420: 6573 6372 6970 7469 6f6e 2e22 2c0d 0a20  escription.",.. 
-00004430: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
-00004440: 6572 5f70 726f 7065 7274 6965 7322 3a20  er_properties": 
-00004450: 5b5d 2c0d 0a20 2020 2020 2020 2020 2020  [],..           
-00004460: 2022 6e6f 7465 7322 3a20 7b0d 0a20 2020   "notes": {..   
-00004470: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
-00004480: 7665 6c22 3a20 226d 6964 220d 0a20 2020  vel": "mid"..   
-00004490: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-000044a0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-000044b0: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
-000044c0: 6964 223a 2022 6c61 6e67 6368 6169 6e2d  id": "langchain-
-000044d0: 3231 222c 0d0a 2020 2020 2020 2020 2020  21",..          
-000044e0: 2020 2271 7565 7374 696f 6e22 3a20 2249    "question": "I
-000044f0: 7320 7468 6572 6520 616e 2061 6765 6e74  s there an agent
-00004500: 2074 7970 6520 7468 6174 2073 7570 706f   type that suppo
-00004510: 7274 7320 4f70 656e 4149 2773 2066 756e  rts OpenAI's fun
-00004520: 6374 696f 6e20 6361 6c6c 696e 6720 696e  ction calling in
-00004530: 7465 7266 6163 653f 222c 0d0a 2020 2020  terface?",..    
-00004540: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
-00004550: 6365 5f61 6e73 7765 7222 3a20 2259 6573  ce_answer": "Yes
-00004560: 2c20 7468 6572 6520 6973 2061 6e20 6167  , there is an ag
-00004570: 656e 7420 7479 7065 2074 6861 7420 7375  ent type that su
-00004580: 7070 6f72 7473 204f 7065 6e41 4927 7320  pports OpenAI's 
-00004590: 6675 6e63 7469 6f6e 2063 616c 6c69 6e67  function calling
-000045a0: 2069 6e74 6572 6661 6365 2e20 4974 2069   interface. It i
-000045b0: 7320 6361 6c6c 6564 2074 6865 204f 7065  s called the Ope
-000045c0: 6e41 4920 4675 6e63 7469 6f6e 7320 4167  nAI Functions Ag
-000045d0: 656e 742e 2054 6869 7320 6167 656e 7420  ent. This agent 
-000045e0: 6973 2064 6573 6967 6e65 6420 746f 2077  is designed to w
-000045f0: 6f72 6b20 7769 7468 204f 7065 6e41 4920  ork with OpenAI 
-00004600: 6d6f 6465 6c73 2074 6861 7420 6861 7665  models that have
-00004610: 2062 6565 6e20 6669 6e65 2d74 756e 6564   been fine-tuned
-00004620: 2074 6f20 6465 7465 6374 2077 6865 6e20   to detect when 
-00004630: 6120 6675 6e63 7469 6f6e 2073 686f 756c  a function shoul
-00004640: 6420 6265 2063 616c 6c65 6420 616e 6420  d be called and 
-00004650: 7265 7370 6f6e 6420 7769 7468 2074 6865  respond with the
-00004660: 2069 6e70 7574 7320 7468 6174 2073 686f   inputs that sho
-00004670: 756c 6420 6265 2070 6173 7365 6420 746f  uld be passed to
-00004680: 2074 6865 2066 756e 6374 696f 6e2e 2054   the function. T
-00004690: 6865 204f 7065 6e41 4920 4675 6e63 7469  he OpenAI Functi
-000046a0: 6f6e 7320 4167 656e 7420 6973 2063 6170  ons Agent is cap
-000046b0: 6162 6c65 206f 6620 7265 7370 6f6e 6469  able of respondi
-000046c0: 6e67 2074 6f20 7072 6f6d 7074 7320 6672  ng to prompts fr
-000046d0: 6f6d 2074 6865 2075 7365 7220 7573 696e  om the user usin
-000046e0: 6720 6120 4c61 7267 6520 4c61 6e67 7561  g a Large Langua
-000046f0: 6765 204d 6f64 656c 2e22 2c0d 0a20 2020  ge Model.",..   
-00004700: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
-00004710: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
-00004720: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00004730: 6e6f 7465 7322 3a20 7b0d 0a20 2020 2020  notes": {..     
-00004740: 2020 2020 2020 2020 2020 2022 6c65 7665             "leve
-00004750: 6c22 3a20 226d 6964 220d 0a20 2020 2020  l": "mid"..     
-00004760: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00004770: 2020 7d0d 0a20 2020 205d 0d0a 7d           }..    ]..}
+00000000: 7b0a 2020 2020 226e 616d 6522 3a20 224c  {.    "name": "L
+00000010: 616e 6763 6861 696e 5365 7422 2c0a 2020  angchainSet",.  
+00000020: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00000030: 2022 5465 7374 2073 7569 7465 206f 6e20   "Test suite on 
+00000040: 7468 6520 6c61 6e67 6368 6169 6e20 7072  the langchain pr
+00000050: 6f6a 6563 742e 222c 0a20 2020 2022 6361  oject.",.    "ca
+00000060: 7365 7322 3a20 5b0a 2020 2020 2020 2020  ses": [.        
+00000070: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
+00000080: 6422 3a20 226c 616e 6763 6861 696e 2d31  d": "langchain-1
+00000090: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000000a0: 7175 6573 7469 6f6e 223a 2022 5768 6174  question": "What
+000000b0: 2069 7320 7468 6520 636c 6173 7320 6869   is the class hi
+000000c0: 6572 6172 6368 793f 222c 0a20 2020 2020  erarchy?",.     
+000000d0: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
+000000e0: 655f 616e 7377 6572 223a 2022 5468 6572  e_answer": "Ther
+000000f0: 6520 6172 6520 7365 7665 7261 6c20 636c  e are several cl
+00000100: 6173 7320 6869 6572 6172 6368 6965 7320  ass hierarchies 
+00000110: 696e 2074 6865 2070 726f 7669 6465 6420  in the provided 
+00000120: 636f 6465 2c20 736f 2049 276c 6c20 6c69  code, so I'll li
+00000130: 7374 2061 2066 6577 3a5c 6e5c 6e42 6173  st a few:\n\nBas
+00000140: 654d 6f64 656c c2a0 2d3e c2a0 436f 6e73  eModel..->..Cons
+00000150: 7469 7475 7469 6f6e 616c 5072 696e 6369  titutionalPrinci
+00000160: 706c 653a c2a0 436f 6e73 7469 7475 7469  ple:..Constituti
+00000170: 6f6e 616c 5072 696e 6369 706c 65c2 a069  onalPrinciple..i
+00000180: 7320 6120 7375 6263 6c61 7373 206f 66c2  s a subclass of.
+00000190: a042 6173 654d 6f64 656c 2e5c 6e42 6173  .BaseModel.\nBas
+000001a0: 6550 726f 6d70 7454 656d 706c 6174 65c2  ePromptTemplate.
+000001b0: a02d 3ec2 a053 7472 696e 6750 726f 6d70  .->..StringPromp
+000001c0: 7454 656d 706c 6174 652c c2a0 4149 4d65  tTemplate,..AIMe
+000001d0: 7373 6167 6550 726f 6d70 7454 656d 706c  ssagePromptTempl
+000001e0: 6174 652c c2a0 4261 7365 4368 6174 5072  ate,..BaseChatPr
+000001f0: 6f6d 7074 5465 6d70 6c61 7465 2cc2 a043  omptTemplate,..C
+00000200: 6861 744d 6573 7361 6765 5072 6f6d 7074  hatMessagePrompt
+00000210: 5465 6d70 6c61 7465 2cc2 a043 6861 7450  Template,..ChatP
+00000220: 726f 6d70 7454 656d 706c 6174 652c c2a0  romptTemplate,..
+00000230: 4875 6d61 6e4d 6573 7361 6765 5072 6f6d  HumanMessageProm
+00000240: 7074 5465 6d70 6c61 7465 2cc2 a04d 6573  ptTemplate,..Mes
+00000250: 7361 6765 7350 6c61 6365 686f 6c64 6572  sagesPlaceholder
+00000260: 2cc2 a053 7973 7465 6d4d 6573 7361 6765  ,..SystemMessage
+00000270: 5072 6f6d 7074 5465 6d70 6c61 7465 2cc2  PromptTemplate,.
+00000280: a046 6577 5368 6f74 5072 6f6d 7074 5465  .FewShotPromptTe
+00000290: 6d70 6c61 7465 2cc2 a046 6577 5368 6f74  mplate,..FewShot
+000002a0: 5072 6f6d 7074 5769 7468 5465 6d70 6c61  PromptWithTempla
+000002b0: 7465 732c c2a0 5072 6f6d 7074 2cc2 a050  tes,..Prompt,..P
+000002c0: 726f 6d70 7454 656d 706c 6174 653a 2041  romptTemplate: A
+000002d0: 6c6c 206f 6620 7468 6573 6520 636c 6173  ll of these clas
+000002e0: 7365 7320 6172 6520 7375 6263 6c61 7373  ses are subclass
+000002f0: 6573 206f 66c2 a042 6173 6550 726f 6d70  es of..BasePromp
+00000300: 7454 656d 706c 6174 652e 5c6e 4150 4943  tTemplate.\nAPIC
+00000310: 6861 696e 2cc2 a043 6861 696e 2cc2 a04d  hain,..Chain,..M
+00000320: 6170 5265 6475 6365 446f 6375 6d65 6e74  apReduceDocument
+00000330: 7343 6861 696e 2cc2 a04d 6170 5265 7261  sChain,..MapRera
+00000340: 6e6b 446f 6375 6d65 6e74 7343 6861 696e  nkDocumentsChain
+00000350: 2cc2 a052 6566 696e 6544 6f63 756d 656e  ,..RefineDocumen
+00000360: 7473 4368 6169 6e2c c2a0 5374 7566 6644  tsChain,..StuffD
+00000370: 6f63 756d 656e 7473 4368 6169 6e2c c2a0  ocumentsChain,..
+00000380: 4879 706f 7468 6574 6963 616c 446f 6375  HypotheticalDocu
+00000390: 6d65 6e74 456d 6265 6464 6572 2cc2 a04c  mentEmbedder,..L
+000003a0: 4c4d 4368 6169 6e2c c2a0 4c4c 4d42 6173  LMChain,..LLMBas
+000003b0: 6843 6861 696e 2cc2 a04c 4c4d 4368 6563  hChain,..LLMChec
+000003c0: 6b65 7243 6861 696e 2cc2 a04c 4c4d 4d61  kerChain,..LLMMa
+000003d0: 7468 4368 6169 6e2c c2a0 4c4c 4d52 6571  thChain,..LLMReq
+000003e0: 7565 7374 7343 6861 696e 2cc2 a050 414c  uestsChain,..PAL
+000003f0: 4368 6169 6e2c c2a0 5141 5769 7468 536f  Chain,..QAWithSo
+00000400: 7572 6365 7343 6861 696e 2cc2 a056 6563  urcesChain,..Vec
+00000410: 746f 7244 4251 4157 6974 6853 6f75 7263  torDBQAWithSourc
+00000420: 6573 4368 6169 6e2c c2a0 5665 6374 6f72  esChain,..Vector
+00000430: 4442 5141 2cc2 a053 514c 4461 7461 6261  DBQA,..SQLDataba
+00000440: 7365 4368 6169 6e3a 2041 6c6c 206f 6620  seChain: All of 
+00000450: 7468 6573 6520 636c 6173 7365 7320 6172  these classes ar
+00000460: 6520 7375 6263 6c61 7373 6573 206f 66c2  e subclasses of.
+00000470: a043 6861 696e 2e5c 6e42 6173 654c 6f61  .Chain.\nBaseLoa
+00000480: 6465 723a c2a0 4261 7365 4c6f 6164 6572  der:..BaseLoader
+00000490: c2a0 6973 2061 2073 7562 636c 6173 7320  ..is a subclass 
+000004a0: 6f66 c2a0 4142 432e 5c6e 4261 7365 5472  of..ABC.\nBaseTr
+000004b0: 6163 6572 c2a0 2d3e c2a0 4368 6169 6e52  acer..->..ChainR
+000004c0: 756e 2cc2 a04c 4c4d 5275 6e2c c2a0 5368  un,..LLMRun,..Sh
+000004d0: 6172 6564 5472 6163 6572 2cc2 a054 6f6f  aredTracer,..Too
+000004e0: 6c52 756e 2cc2 a054 7261 6365 722c c2a0  lRun,..Tracer,..
+000004f0: 5472 6163 6572 4578 6365 7074 696f 6e2c  TracerException,
+00000500: c2a0 5472 6163 6572 5365 7373 696f 6e3a  ..TracerSession:
+00000510: 2041 6c6c 206f 6620 7468 6573 6520 636c   All of these cl
+00000520: 6173 7365 7320 6172 6520 7375 6263 6c61  asses are subcla
+00000530: 7373 6573 206f 66c2 a042 6173 6554 7261  sses of..BaseTra
+00000540: 6365 722e 5c6e 4f70 656e 4149 456d 6265  cer.\nOpenAIEmbe
+00000550: 6464 696e 6773 2cc2 a048 7567 6769 6e67  ddings,..Hugging
+00000560: 4661 6365 456d 6265 6464 696e 6773 2cc2  FaceEmbeddings,.
+00000570: a043 6f68 6572 6545 6d62 6564 6469 6e67  .CohereEmbedding
+00000580: 732c c2a0 4a69 6e61 456d 6265 6464 696e  s,..JinaEmbeddin
+00000590: 6773 2cc2 a04c 6c61 6d61 4370 7045 6d62  gs,..LlamaCppEmb
+000005a0: 6564 6469 6e67 732c c2a0 4875 6767 696e  eddings,..Huggin
+000005b0: 6746 6163 6548 7562 456d 6265 6464 696e  gFaceHubEmbeddin
+000005c0: 6773 2cc2 a054 656e 736f 7266 6c6f 7748  gs,..TensorflowH
+000005d0: 7562 456d 6265 6464 696e 6773 2cc2 a053  ubEmbeddings,..S
+000005e0: 6167 656d 616b 6572 456e 6470 6f69 6e74  agemakerEndpoint
+000005f0: 456d 6265 6464 696e 6773 2cc2 a048 7567  Embeddings,..Hug
+00000600: 6769 6e67 4661 6365 496e 7374 7275 6374  gingFaceInstruct
+00000610: 456d 6265 6464 696e 6773 2cc2 a053 656c  Embeddings,..Sel
+00000620: 6648 6f73 7465 6445 6d62 6564 6469 6e67  fHostedEmbedding
+00000630: 732c c2a0 5365 6c66 486f 7374 6564 4875  s,..SelfHostedHu
+00000640: 6767 696e 6746 6163 6545 6d62 6564 6469  ggingFaceEmbeddi
+00000650: 6e67 732c c2a0 5365 6c66 486f 7374 6564  ngs,..SelfHosted
+00000660: 4875 6767 696e 6746 6163 6549 6e73 7472  HuggingFaceInstr
+00000670: 7563 7445 6d62 6564 6469 6e67 732c c2a0  uctEmbeddings,..
+00000680: 4661 6b65 456d 6265 6464 696e 6773 2cc2  FakeEmbeddings,.
+00000690: a041 6c65 7068 416c 7068 6141 7379 6d6d  .AlephAlphaAsymm
+000006a0: 6574 7269 6353 656d 616e 7469 6345 6d62  etricSemanticEmb
+000006b0: 6564 6469 6e67 2cc2 a041 6c65 7068 416c  edding,..AlephAl
+000006c0: 7068 6153 796d 6d65 7472 6963 5365 6d61  phaSymmetricSema
+000006d0: 6e74 6963 456d 6265 6464 696e 673a 2041  nticEmbedding: A
+000006e0: 6c6c 206f 6620 7468 6573 6520 636c 6173  ll of these clas
+000006f0: 7365 7320 6172 6520 7375 6263 6c61 7373  ses are subclass
+00000700: 6573 206f 66c2 a042 6173 654c 4c4d 2e22  es of..BaseLLM."
+00000710: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+00000720: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
+00000730: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
+00000740: 2020 2022 6e6f 7465 7322 3a20 7b0a 2020     "notes": {.  
+00000750: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00000760: 6576 656c 223a 2022 6869 6768 220a 2020  evel": "high".  
+00000770: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000780: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+00000790: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
+000007a0: 223a 2022 6c61 6e67 6368 6169 6e2d 3222  ": "langchain-2"
+000007b0: 2c0a 2020 2020 2020 2020 2020 2020 2271  ,.            "q
+000007c0: 7565 7374 696f 6e22 3a20 2257 6861 7420  uestion": "What 
+000007d0: 636c 6173 7365 7320 6172 6520 6465 7269  classes are deri
+000007e0: 7665 6420 6672 6f6d 2074 6865 2060 4368  ved from the `Ch
+000007f0: 6169 6e60 2063 6c61 7373 3f22 2c0a 2020  ain` class?",.  
+00000800: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
+00000810: 656e 6365 5f61 6e73 7765 7222 3a20 2254  ence_answer": "T
+00000820: 6865 7265 2061 7265 206d 756c 7469 706c  here are multipl
+00000830: 6520 636c 6173 7365 7320 7468 6174 2061  e classes that a
+00000840: 7265 2064 6572 6976 6564 2066 726f 6d20  re derived from 
+00000850: 7468 6520 4368 6169 6e20 636c 6173 732e  the Chain class.
+00000860: 2053 6f6d 6520 6f66 2074 6865 6d20 6172   Some of them ar
+00000870: 653a 5c6e 5c6e 4150 4943 6861 696e 5c6e  e:\n\nAPIChain\n
+00000880: 416e 616c 797a 6544 6f63 756d 656e 7443  AnalyzeDocumentC
+00000890: 6861 696e 5c6e 4368 6174 5665 6374 6f72  hain\nChatVector
+000008a0: 4442 4368 6169 6e5c 6e43 6f6d 6269 6e65  DBChain\nCombine
+000008b0: 446f 6375 6d65 6e74 7343 6861 696e 5c6e  DocumentsChain\n
+000008c0: 436f 6e73 7469 7475 7469 6f6e 616c 4368  ConstitutionalCh
+000008d0: 6169 6e5c 6e43 6f6e 7665 7273 6174 696f  ain\nConversatio
+000008e0: 6e43 6861 696e 5c6e 4772 6170 6851 4143  nChain\nGraphQAC
+000008f0: 6861 696e 5c6e 4879 706f 7468 6574 6963  hain\nHypothetic
+00000900: 616c 446f 6375 6d65 6e74 456d 6265 6464  alDocumentEmbedd
+00000910: 6572 5c6e 4c4c 4d43 6861 696e 5c6e 4c4c  er\nLLMChain\nLL
+00000920: 4d43 6865 636b 6572 4368 6169 6e5c 6e4c  MCheckerChain\nL
+00000930: 4c4d 5265 7175 6573 7473 4368 6169 6e5c  LMRequestsChain\
+00000940: 6e4c 4c4d 5375 6d6d 6172 697a 6174 696f  nLLMSummarizatio
+00000950: 6e43 6865 636b 6572 4368 6169 6e5c 6e4d  nCheckerChain\nM
+00000960: 6170 5265 6475 6365 4368 6169 6e5c 6e4f  apReduceChain\nO
+00000970: 7065 6e41 5049 456e 6470 6f69 6e74 4368  penAPIEndpointCh
+00000980: 6169 6e5c 6e50 414c 4368 6169 6e5c 6e51  ain\nPALChain\nQ
+00000990: 4157 6974 6853 6f75 7263 6573 4368 6169  AWithSourcesChai
+000009a0: 6e5c 6e52 6574 7269 6576 616c 5141 5c6e  n\nRetrievalQA\n
+000009b0: 5265 7472 6965 7661 6c51 4157 6974 6853  RetrievalQAWithS
+000009c0: 6f75 7263 6573 4368 6169 6e5c 6e53 6571  ourcesChain\nSeq
+000009d0: 7565 6e74 6961 6c43 6861 696e 5c6e 5351  uentialChain\nSQ
+000009e0: 4c44 6174 6162 6173 6543 6861 696e 5c6e  LDatabaseChain\n
+000009f0: 5472 616e 7366 6f72 6d43 6861 696e 5c6e  TransformChain\n
+00000a00: 5665 6374 6f72 4442 5141 5c6e 5665 6374  VectorDBQA\nVect
+00000a10: 6f72 4442 5141 5769 7468 536f 7572 6365  orDBQAWithSource
+00000a20: 7343 6861 696e 5c6e 5c6e 5468 6572 6520  sChain\n\nThere 
+00000a30: 6d69 6768 7420 6265 206d 6f72 6520 636c  might be more cl
+00000a40: 6173 7365 7320 7468 6174 2061 7265 2064  asses that are d
+00000a50: 6572 6976 6564 2066 726f 6d20 7468 6520  erived from the 
+00000a60: 4368 6169 6e20 636c 6173 7320 6173 2069  Chain class as i
+00000a70: 7420 6973 2070 6f73 7369 626c 6520 746f  t is possible to
+00000a80: 2063 7265 6174 6520 6375 7374 6f6d 2063   create custom c
+00000a90: 6c61 7373 6573 2074 6861 7420 6578 7465  lasses that exte
+00000aa0: 6e64 2074 6865 2043 6861 696e 2063 6c61  nd the Chain cla
+00000ab0: 7373 2e22 2c0a 2020 2020 2020 2020 2020  ss.",.          
+00000ac0: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
+00000ad0: 7469 6573 223a 205b 5d2c 0a20 2020 2020  ties": [],.     
+00000ae0: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
+00000af0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000b00: 2020 226c 6576 656c 223a 2022 6869 6768    "level": "high
+00000b10: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+00000b20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000b30: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000b40: 2022 6964 223a 2022 6c61 6e67 6368 6169   "id": "langchai
+00000b50: 6e2d 3322 2c0a 2020 2020 2020 2020 2020  n-3",.          
+00000b60: 2020 2271 7565 7374 696f 6e22 3a20 2257    "question": "W
+00000b70: 6861 7420 636c 6173 7365 7320 616e 6420  hat classes and 
+00000b80: 6675 6e63 7469 6f6e 7320 696e 2074 6865  functions in the
+00000b90: 2060 2e2f 6c61 6e67 6368 6169 6e2f 7574   `./langchain/ut
+00000ba0: 696c 6974 6965 732f 6020 666f 726c 6465  ilities/` forlde
+00000bb0: 7220 6172 6520 6e6f 7420 636f 7665 7265  r are not covere
+00000bc0: 6420 6279 2075 6e69 7420 7465 7374 733f  d by unit tests?
+00000bd0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000be0: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
+00000bf0: 223a 2022 416c 6c20 636c 6173 7365 7320  ": "All classes 
+00000c00: 616e 6420 6675 6e63 7469 6f6e 7320 696e  and functions in
+00000c10: 2074 6865 c2a0 2e2f 6c61 6e67 6368 6169   the.../langchai
+00000c20: 6e2f 7574 696c 6974 6965 732f c2a0 666f  n/utilities/..fo
+00000c30: 6c64 6572 2073 6565 6d20 746f 2068 6176  lder seem to hav
+00000c40: 6520 756e 6974 2074 6573 7473 2077 7269  e unit tests wri
+00000c50: 7474 656e 2066 6f72 2074 6865 6d2e 222c  tten for them.",
+00000c60: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
+00000c70: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
+00000c80: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+00000c90: 2020 226e 6f74 6573 223a 207b 0a20 2020    "notes": {.   
+00000ca0: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
+00000cb0: 7665 6c22 3a20 226d 6964 220a 2020 2020  vel": "mid".    
+00000cc0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000cd0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00000ce0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+00000cf0: 2022 6c61 6e67 6368 6169 6e2d 3422 2c0a   "langchain-4",.
+00000d00: 2020 2020 2020 2020 2020 2020 2271 7565              "que
+00000d10: 7374 696f 6e22 3a20 2257 6861 7420 6172  stion": "What ar
+00000d20: 6520 7468 6520 736f 6d65 206f 6620 7468  e the some of th
+00000d30: 6520 6d61 696e 2063 6861 6c6c 656e 6765  e main challenge
+00000d40: 7320 7468 6174 2074 6865 204c 616e 6763  s that the Langc
+00000d50: 6861 696e 2070 726f 6a65 6374 2068 6173  hain project has
+00000d60: 2074 6f20 6465 616c 2077 6974 683f 222c   to deal with?",
+00000d70: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00000d80: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+00000d90: 2022 4261 7365 6420 6f6e 2074 6865 2063   "Based on the c
+00000da0: 6f6e 7465 7874 2070 726f 7669 6465 642c  ontext provided,
+00000db0: 2069 7420 7365 656d 7320 746f 2062 6520   it seems to be 
+00000dc0: 7265 6c61 7465 6420 746f 206e 6174 7572  related to natur
+00000dd0: 616c 206c 616e 6775 6167 6520 7072 6f63  al language proc
+00000de0: 6573 7369 6e67 2061 6e64 2072 756e 6e69  essing and runni
+00000df0: 6e67 206d 6f64 656c 7320 6f72 2063 6861  ng models or cha
+00000e00: 696e 7320 6f6e 2064 6174 6173 6574 732e  ins on datasets.
+00000e10: 2053 6f6d 6520 6765 6e65 7261 6c20 6368   Some general ch
+00000e20: 616c 6c65 6e67 6573 2074 6861 7420 636f  allenges that co
+00000e30: 756c 6420 6265 2066 6163 6564 2069 6e20  uld be faced in 
+00000e40: 7375 6368 2070 726f 6a65 6374 7320 6d61  such projects ma
+00000e50: 7920 696e 636c 7564 653a 5c6e 5c6e 312e  y include:\n\n1.
+00000e60: 2048 616e 646c 696e 6720 6c61 7267 6520   Handling large 
+00000e70: 616e 6420 6469 7665 7273 6520 6461 7461  and diverse data
+00000e80: 7365 7473 3a20 5072 6f63 6573 7369 6e67  sets: Processing
+00000e90: 2061 6e64 206d 616e 6167 696e 6720 6c61   and managing la
+00000ea0: 7267 6520 6461 7461 7365 7473 2063 616e  rge datasets can
+00000eb0: 2062 6520 636f 6d70 7574 6174 696f 6e61   be computationa
+00000ec0: 6c6c 7920 6578 7065 6e73 6976 6520 616e  lly expensive an
+00000ed0: 6420 7469 6d65 2d63 6f6e 7375 6d69 6e67  d time-consuming
+00000ee0: 2e20 456e 7375 7269 6e67 2065 6666 6963  . Ensuring effic
+00000ef0: 6965 6e74 2064 6174 6120 7072 6f63 6573  ient data proces
+00000f00: 7369 6e67 2061 6e64 2073 746f 7261 6765  sing and storage
+00000f10: 2069 7320 6372 7563 6961 6c20 666f 7220   is crucial for 
+00000f20: 7468 6520 7072 6f6a 6563 7427 7320 7375  the project's su
+00000f30: 6363 6573 732e 5c6e 5c6e 322e 204d 6f64  ccess.\n\n2. Mod
+00000f40: 656c 2070 6572 666f 726d 616e 6365 2061  el performance a
+00000f50: 6e64 2061 6363 7572 6163 793a 2044 6576  nd accuracy: Dev
+00000f60: 656c 6f70 696e 6720 6d6f 6465 6c73 2074  eloping models t
+00000f70: 6861 7420 6361 6e20 6163 6375 7261 7465  hat can accurate
+00000f80: 6c79 2075 6e64 6572 7374 616e 642c 2067  ly understand, g
+00000f90: 656e 6572 6174 652c 206f 7220 6d61 6e69  enerate, or mani
+00000fa0: 7075 6c61 7465 206e 6174 7572 616c 206c  pulate natural l
+00000fb0: 616e 6775 6167 6520 6973 2063 6f6d 706c  anguage is compl
+00000fc0: 6578 2e20 456e 7375 7269 6e67 2068 6967  ex. Ensuring hig
+00000fd0: 6820 7065 7266 6f72 6d61 6e63 6520 616e  h performance an
+00000fe0: 6420 6163 6375 7261 6379 2069 7320 616e  d accuracy is an
+00000ff0: 206f 6e67 6f69 6e67 2063 6861 6c6c 656e   ongoing challen
+00001000: 6765 2069 6e20 7468 6520 6669 656c 6420  ge in the field 
+00001010: 6f66 206e 6174 7572 616c 206c 616e 6775  of natural langu
+00001020: 6167 6520 7072 6f63 6573 7369 6e67 2e5c  age processing.\
+00001030: 6e5c 6e33 2e20 496e 7465 6772 6174 696f  n\n3. Integratio
+00001040: 6e20 7769 7468 2076 6172 696f 7573 2074  n with various t
+00001050: 6f6f 6c73 2061 6e64 2073 6572 7669 6365  ools and service
+00001060: 733a 2054 6865 2070 726f 6a65 6374 206d  s: The project m
+00001070: 6967 6874 2072 6571 7569 7265 2069 6e74  ight require int
+00001080: 6567 7261 7469 6f6e 2077 6974 6820 6469  egration with di
+00001090: 6666 6572 656e 7420 746f 6f6c 7320 616e  fferent tools an
+000010a0: 6420 7365 7276 6963 6573 2c20 7375 6368  d services, such
+000010b0: 2061 7320 6c61 6e67 7561 6765 206d 6f64   as language mod
+000010c0: 656c 732c 2041 5049 732c 206f 7220 6f74  els, APIs, or ot
+000010d0: 6865 7220 6578 7465 726e 616c 2072 6573  her external res
+000010e0: 6f75 7263 6573 2e20 456e 7375 7269 6e67  ources. Ensuring
+000010f0: 2073 6561 6d6c 6573 7320 696e 7465 6772   seamless integr
+00001100: 6174 696f 6e20 6361 6e20 6265 2063 6861  ation can be cha
+00001110: 6c6c 656e 6769 6e67 2e5c 6e5c 6e34 2e20  llenging.\n\n4. 
+00001120: 5363 616c 6162 696c 6974 793a 2041 7320  Scalability: As 
+00001130: 7468 6520 7072 6f6a 6563 7420 6772 6f77  the project grow
+00001140: 732c 2069 7420 6d61 7920 6e65 6564 2074  s, it may need t
+00001150: 6f20 6861 6e64 6c65 206d 6f72 6520 6461  o handle more da
+00001160: 7461 2c20 6d6f 7265 206d 6f64 656c 732c  ta, more models,
+00001170: 206f 7220 6d6f 7265 2075 7365 7273 2e20   or more users. 
+00001180: 456e 7375 7269 6e67 2074 6861 7420 7468  Ensuring that th
+00001190: 6520 7072 6f6a 6563 7420 6361 6e20 7363  e project can sc
+000011a0: 616c 6520 736d 6f6f 7468 6c79 2061 6e64  ale smoothly and
+000011b0: 2068 616e 646c 6520 696e 6372 6561 7365   handle increase
+000011c0: 6420 776f 726b 6c6f 6164 7320 6973 2069  d workloads is i
+000011d0: 6d70 6f72 7461 6e74 2066 6f72 206c 6f6e  mportant for lon
+000011e0: 672d 7465 726d 2073 7563 6365 7373 2e5c  g-term success.\
+000011f0: 6e5c 6e35 2e20 5365 6375 7269 7479 2061  n\n5. Security a
+00001200: 6e64 2070 7269 7661 6379 3a20 4861 6e64  nd privacy: Hand
+00001210: 6c69 6e67 2073 656e 7369 7469 7665 2064  ling sensitive d
+00001220: 6174 6120 616e 6420 656e 7375 7269 6e67  ata and ensuring
+00001230: 2074 6865 2073 6563 7572 6974 7920 616e   the security an
+00001240: 6420 7072 6976 6163 7920 6f66 2075 7365  d privacy of use
+00001250: 7273 2061 6e64 2074 6865 6972 2069 6e66  rs and their inf
+00001260: 6f72 6d61 7469 6f6e 2069 7320 616e 2065  ormation is an e
+00001270: 7373 656e 7469 616c 2061 7370 6563 7420  ssential aspect 
+00001280: 7468 6174 206e 6565 6473 2074 6f20 6265  that needs to be
+00001290: 2061 6464 7265 7373 6564 2e5c 6e5c 6e36   addressed.\n\n6
+000012a0: 2e20 4d61 696e 7461 696e 696e 6720 616e  . Maintaining an
+000012b0: 6420 7570 6461 7469 6e67 206d 6f64 656c  d updating model
+000012c0: 733a 204c 616e 6775 6167 6520 6d6f 6465  s: Language mode
+000012d0: 6c73 2061 6e64 206f 7468 6572 2063 6f6d  ls and other com
+000012e0: 706f 6e65 6e74 7320 6f66 2074 6865 2070  ponents of the p
+000012f0: 726f 6a65 6374 206d 6179 206e 6565 6420  roject may need 
+00001300: 746f 2062 6520 7570 6461 7465 6420 6f72  to be updated or
+00001310: 206d 6169 6e74 6169 6e65 6420 6f76 6572   maintained over
+00001320: 2074 696d 6520 746f 2065 6e73 7572 6520   time to ensure 
+00001330: 636f 6e74 696e 7565 6420 6566 6665 6374  continued effect
+00001340: 6976 656e 6573 7320 616e 6420 7265 6c65  iveness and rele
+00001350: 7661 6e63 652e 5c6e 5c6e 372e 2043 6f73  vance.\n\n7. Cos
+00001360: 7420 6d61 6e61 6765 6d65 6e74 3a20 5275  t management: Ru
+00001370: 6e6e 696e 6720 6c61 6e67 7561 6765 206d  nning language m
+00001380: 6f64 656c 732c 2065 7370 6563 6961 6c6c  odels, especiall
+00001390: 7920 6c61 7267 6520 6f6e 6573 2c20 6361  y large ones, ca
+000013a0: 6e20 6265 2065 7870 656e 7369 7665 2e20  n be expensive. 
+000013b0: 4d61 6e61 6769 6e67 2074 6865 2063 6f73  Managing the cos
+000013c0: 7473 2061 7373 6f63 6961 7465 6420 7769  ts associated wi
+000013d0: 7468 2072 756e 6e69 6e67 2073 7563 6820  th running such 
+000013e0: 6d6f 6465 6c73 2c20 616c 6f6e 6720 7769  models, along wi
+000013f0: 7468 206f 7468 6572 2069 6e66 7261 7374  th other infrast
+00001400: 7275 6374 7572 6520 616e 6420 7265 736f  ructure and reso
+00001410: 7572 6365 732c 2069 7320 6120 6368 616c  urces, is a chal
+00001420: 6c65 6e67 6520 7468 6174 206e 6565 6473  lenge that needs
+00001430: 2074 6f20 6265 2061 6464 7265 7373 6564   to be addressed
+00001440: 2e5c 6e5c 6e50 6c65 6173 6520 6e6f 7465  .\n\nPlease note
+00001450: 2074 6861 7420 7468 6573 6520 6172 6520   that these are 
+00001460: 6765 6e65 7261 6c20 6368 616c 6c65 6e67  general challeng
+00001470: 6573 2074 6861 7420 636f 756c 6420 6265  es that could be
+00001480: 2066 6163 6564 2069 6e20 6120 6e61 7475   faced in a natu
+00001490: 7261 6c20 6c61 6e67 7561 6765 2070 726f  ral language pro
+000014a0: 6365 7373 696e 6720 7072 6f6a 6563 742e  cessing project.
+000014b0: 2054 6865 2073 7065 6369 6669 6320 6368   The specific ch
+000014c0: 616c 6c65 6e67 6573 2066 6163 6564 2062  allenges faced b
+000014d0: 7920 7468 6520 4c61 6e67 6368 6169 6e20  y the Langchain 
+000014e0: 7072 6f6a 6563 7420 6d69 6768 7420 7661  project might va
+000014f0: 7279 2062 6173 6564 206f 6e20 6974 7320  ry based on its 
+00001500: 676f 616c 732c 2073 636f 7065 2c20 616e  goals, scope, an
+00001510: 6420 696d 706c 656d 656e 7461 7469 6f6e  d implementation
+00001520: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00001530: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
+00001540: 6573 223a 205b 5d2c 0a20 2020 2020 2020  es": [],.       
+00001550: 2020 2020 2022 6e6f 7465 7322 3a20 7b0a       "notes": {.
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 226c 6576 656c 223a 2022 6869 6768 220a  "level": "high".
+00001580: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001590: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000015a0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000015b0: 6964 223a 2022 6c61 6e67 6368 6169 6e2d  id": "langchain-
+000015c0: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
+000015d0: 2271 7565 7374 696f 6e22 3a20 2244 6f65  "question": "Doe
+000015e0: 7320 6055 6e73 7472 7563 7475 7265 644d  s `UnstructuredM
+000015f0: 6172 6b64 6f77 6e4c 6f61 6465 7260 2061  arkdownLoader` a
+00001600: 6363 6570 7420 6120 7374 7269 6e67 2072  ccept a string r
+00001610: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00001620: 2061 206d 6172 6b64 6f77 6e20 6669 6c65   a markdown file
+00001630: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
+00001640: 2272 6566 6572 656e 6365 5f61 6e73 7765  "reference_answe
+00001650: 7222 3a20 224e 6f2c 2055 6e73 7472 7563  r": "No, Unstruc
+00001660: 7475 7265 644d 6172 6b64 6f77 6e4c 6f61  turedMarkdownLoa
+00001670: 6465 7220 646f 6573 206e 6f74 2061 6363  der does not acc
+00001680: 6570 7420 6120 7374 7269 6e67 2072 6570  ept a string rep
+00001690: 7265 7365 6e74 6174 696f 6e20 6f66 2061  resentation of a
+000016a0: 206d 6172 6b64 6f77 6e20 6669 6c65 2e20   markdown file. 
+000016b0: 4974 2074 616b 6573 2061 2066 696c 6520  It takes a file 
+000016c0: 7061 7468 2061 7320 696e 7075 742e 222c  path as input.",
+000016d0: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
+000016e0: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
+000016f0: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+00001700: 2020 226e 6f74 6573 223a 207b 0a20 2020    "notes": {.   
+00001710: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
+00001720: 7665 6c22 3a20 226d 6964 220a 2020 2020  vel": "mid".    
+00001730: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001740: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00001750: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+00001760: 2022 6c61 6e67 6368 6169 6e2d 3622 2c0a   "langchain-6",.
+00001770: 2020 2020 2020 2020 2020 2020 2271 7565              "que
+00001780: 7374 696f 6e22 3a20 2257 6861 7420 6973  stion": "What is
+00001790: 2074 6865 2070 7572 706f 7365 206f 6620   the purpose of 
+000017a0: 7468 6520 6c61 6e67 6368 6169 6e20 7072  the langchain pr
+000017b0: 6f6a 6563 743f 222c 0a20 2020 2020 2020  oject?",.       
+000017c0: 2020 2020 2022 7265 6665 7265 6e63 655f       "reference_
+000017d0: 616e 7377 6572 223a 2022 5468 6520 7075  answer": "The pu
+000017e0: 7270 6f73 6520 6f66 2074 6865 204c 616e  rpose of the Lan
+000017f0: 6763 6861 696e 2070 726f 6a65 6374 2069  gchain project i
+00001800: 7320 746f 2070 726f 7669 6465 2061 2066  s to provide a f
+00001810: 7261 6d65 776f 726b 2066 6f72 2064 6576  ramework for dev
+00001820: 656c 6f70 696e 6720 6170 706c 6963 6174  eloping applicat
+00001830: 696f 6e73 2070 6f77 6572 6564 2062 7920  ions powered by 
+00001840: 6c61 6e67 7561 6765 206d 6f64 656c 732e  language models.
+00001850: 2049 7420 6169 6d73 2074 6f20 7369 6d70   It aims to simp
+00001860: 6c69 6679 2074 6865 2063 7265 6174 696f  lify the creatio
+00001870: 6e20 6f66 2061 7070 6c69 6361 7469 6f6e  n of application
+00001880: 7320 7573 696e 6720 6c61 7267 6520 6c61  s using large la
+00001890: 6e67 7561 6765 206d 6f64 656c 7320 284c  nguage models (L
+000018a0: 4c4d 7329 2061 6e64 206f 6666 6572 7320  LMs) and offers 
+000018b0: 6120 7365 7420 6f66 2074 6f6f 6c73 2061  a set of tools a
+000018c0: 6e64 2073 6572 7669 6365 7320 746f 2061  nd services to a
+000018d0: 7373 6973 7420 6465 7665 6c6f 7065 7273  ssist developers
+000018e0: 2069 6e20 6275 696c 6469 6e67 204e 4c50   in building NLP
+000018f0: 2061 7070 6c69 6361 7469 6f6e 732e 2054   applications. T
+00001900: 6865 204c 616e 6763 6861 696e 2066 7261  he Langchain fra
+00001910: 6d65 776f 726b 2065 6e61 626c 6573 2064  mework enables d
+00001920: 6576 656c 6f70 6572 7320 746f 2063 7265  evelopers to cre
+00001930: 6174 6520 7365 7175 656e 6365 7320 6f66  ate sequences of
+00001940: 2063 616c 6c73 2c20 636f 6e6e 6563 7420   calls, connect 
+00001950: 6c61 6e67 7561 6765 206d 6f64 656c 7320  language models 
+00001960: 746f 206f 7468 6572 2064 6174 6120 736f  to other data so
+00001970: 7572 6365 732c 2061 6e64 2069 6e74 6572  urces, and inter
+00001980: 6163 7420 7769 7468 2061 7070 6c69 6361  act with applica
+00001990: 7469 6f6e 2d73 7065 6369 6669 6320 6461  tion-specific da
+000019a0: 7461 2e20 4974 2061 6c73 6f20 7072 6f76  ta. It also prov
+000019b0: 6964 6573 206f 6666 2d74 6865 2d73 6865  ides off-the-she
+000019c0: 6c66 2063 6861 696e 7320 666f 7220 7370  lf chains for sp
+000019d0: 6563 6966 6963 2074 6173 6b73 2061 6e64  ecific tasks and
+000019e0: 2061 6c6c 6f77 7320 666f 7220 6375 7374   allows for cust
+000019f0: 6f6d 697a 6174 696f 6e20 616e 6420 6275  omization and bu
+00001a00: 696c 6469 6e67 206e 6577 2063 6861 696e  ilding new chain
+00001a10: 732e 204f 7665 7261 6c6c 2c20 7468 6520  s. Overall, the 
+00001a20: 4c61 6e67 6368 6169 6e20 7072 6f6a 6563  Langchain projec
+00001a30: 7420 6169 6d73 2074 6f20 7265 766f 6c75  t aims to revolu
+00001a40: 7469 6f6e 697a 6520 7468 6520 7761 7920  tionize the way 
+00001a50: 7065 6f70 6c65 206c 6561 726e 206c 616e  people learn lan
+00001a60: 6775 6167 6573 2061 6e64 2065 6e68 616e  guages and enhan
+00001a70: 6365 2074 6865 2063 6170 6162 696c 6974  ce the capabilit
+00001a80: 6965 7320 6f66 206c 616e 6775 6167 6520  ies of language 
+00001a90: 6d6f 6465 6c73 2069 6e20 7661 7269 6f75  models in variou
+00001aa0: 7320 6170 706c 6963 6174 696f 6e73 2e22  s applications."
+00001ab0: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+00001ac0: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
+00001ad0: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
+00001ae0: 2020 2022 6e6f 7465 7322 3a20 7b0a 2020     "notes": {.  
+00001af0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00001b00: 6576 656c 223a 2022 6d69 6422 0a20 2020  evel": "mid".   
+00001b10: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001b20: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00001b30: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00001b40: 3a20 226c 616e 6763 6861 696e 2d37 222c  : "langchain-7",
+00001b50: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
+00001b60: 6573 7469 6f6e 223a 2022 4973 204f 7065  estion": "Is Ope
+00001b70: 6e41 4927 7320 6067 7074 2d34 2d30 3631  nAI's `gpt-4-061
+00001b80: 3360 206d 6f64 656c 2073 7570 706f 7274  3` model support
+00001b90: 6564 3f22 2c0a 2020 2020 2020 2020 2020  ed?",.          
+00001ba0: 2020 2272 6566 6572 656e 6365 5f61 6e73    "reference_ans
+00001bb0: 7765 7222 3a20 224e 6f2c 2074 6869 7320  wer": "No, this 
+00001bc0: 6d6f 6465 6c20 6973 206e 6f74 2073 7570  model is not sup
+00001bd0: 706f 7274 6564 2e22 2c0a 2020 2020 2020  ported.",.      
+00001be0: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00001bf0: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00001c00: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00001c10: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00001c20: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+00001c30: 6d69 6422 0a20 2020 2020 2020 2020 2020  mid".           
+00001c40: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00001c50: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001c60: 2020 2020 2269 6422 3a20 226c 616e 6763      "id": "langc
+00001c70: 6861 696e 2d38 222c 0a20 2020 2020 2020  hain-8",.       
+00001c80: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
+00001c90: 2022 486f 7720 646f 2049 2075 7365 2061   "How do I use a
+00001ca0: 6e20 604c 4c4d 4368 6169 6e60 2077 6974  n `LLMChain` wit
+00001cb0: 6820 6120 6368 6174 206d 6f64 656c 3f20  h a chat model? 
+00001cc0: 506c 6561 7365 2070 726f 7669 6465 2065  Please provide e
+00001cd0: 7861 6d70 6c65 2063 6f64 652e 222c 0a20  xample code.",. 
+00001ce0: 2020 2020 2020 2020 2020 2022 7265 6665             "refe
+00001cf0: 7265 6e63 655f 616e 7377 6572 223a 2022  rence_answer": "
+00001d00: 5468 65c2 a04c 4c4d 4368 6169 6ec2 a063  The..LLMChain..c
+00001d10: 616e 2062 6520 7573 6564 2077 6974 6820  an be used with 
+00001d20: 6368 6174 206d 6f64 656c 7320 6173 2077  chat models as w
+00001d30: 656c 6c3a 5c6e 6060 605c 6e66 726f 6d20  ell:\n```\nfrom 
+00001d40: 6c61 6e67 6368 6169 6e20 696d 706f 7274  langchain import
+00001d50: 204c 4c4d 4368 6169 6e5c 6e66 726f 6d20   LLMChain\nfrom 
+00001d60: 6c61 6e67 6368 6169 6e2e 6368 6174 5f6d  langchain.chat_m
+00001d70: 6f64 656c 7320 696d 706f 7274 2043 6861  odels import Cha
+00001d80: 744f 7065 6e41 495c 6e66 726f 6d20 6c61  tOpenAI\nfrom la
+00001d90: 6e67 6368 6169 6e2e 7072 6f6d 7074 732e  ngchain.prompts.
+00001da0: 6368 6174 2069 6d70 6f72 7420 285c 6e20  chat import (\n 
+00001db0: 2020 2043 6861 7450 726f 6d70 7454 656d     ChatPromptTem
+00001dc0: 706c 6174 652c 5c6e 2020 2020 5379 7374  plate,\n    Syst
+00001dd0: 656d 4d65 7373 6167 6550 726f 6d70 7454  emMessagePromptT
+00001de0: 656d 706c 6174 652c 5c6e 2020 2020 4875  emplate,\n    Hu
+00001df0: 6d61 6e4d 6573 7361 6765 5072 6f6d 7074  manMessagePrompt
+00001e00: 5465 6d70 6c61 7465 2c5c 6e29 5c6e 5c6e  Template,\n)\n\n
+00001e10: 6368 6174 203d 2043 6861 744f 7065 6e41  chat = ChatOpenA
+00001e20: 4928 7465 6d70 6572 6174 7572 653d 3029  I(temperature=0)
+00001e30: 5c6e 5c6e 7465 6d70 6c61 7465 203d 205c  \n\ntemplate = \
+00001e40: 2259 6f75 2061 7265 2061 2068 656c 7066  "You are a helpf
+00001e50: 756c 2061 7373 6973 7461 6e74 2074 6861  ul assistant tha
+00001e60: 7420 7472 616e 736c 6174 6573 207b 696e  t translates {in
+00001e70: 7075 745f 6c61 6e67 7561 6765 7d20 746f  put_language} to
+00001e80: 207b 6f75 7470 7574 5f6c 616e 6775 6167   {output_languag
+00001e90: 657d 2e5c 225c 6e73 7973 7465 6d5f 6d65  e}.\"\nsystem_me
+00001ea0: 7373 6167 655f 7072 6f6d 7074 203d 2053  ssage_prompt = S
+00001eb0: 7973 7465 6d4d 6573 7361 6765 5072 6f6d  ystemMessageProm
+00001ec0: 7074 5465 6d70 6c61 7465 2e66 726f 6d5f  ptTemplate.from_
+00001ed0: 7465 6d70 6c61 7465 2874 656d 706c 6174  template(templat
+00001ee0: 6529 5c6e 6875 6d61 6e5f 7465 6d70 6c61  e)\nhuman_templa
+00001ef0: 7465 203d 205c 227b 7465 7874 7d5c 225c  te = \"{text}\"\
+00001f00: 6e68 756d 616e 5f6d 6573 7361 6765 5f70  nhuman_message_p
+00001f10: 726f 6d70 7420 3d20 4875 6d61 6e4d 6573  rompt = HumanMes
+00001f20: 7361 6765 5072 6f6d 7074 5465 6d70 6c61  sagePromptTempla
+00001f30: 7465 2e66 726f 6d5f 7465 6d70 6c61 7465  te.from_template
+00001f40: 2868 756d 616e 5f74 656d 706c 6174 6529  (human_template)
+00001f50: 5c6e 6368 6174 5f70 726f 6d70 7420 3d20  \nchat_prompt = 
+00001f60: 4368 6174 5072 6f6d 7074 5465 6d70 6c61  ChatPromptTempla
+00001f70: 7465 2e66 726f 6d5f 6d65 7373 6167 6573  te.from_messages
+00001f80: 285b 7379 7374 656d 5f6d 6573 7361 6765  ([system_message
+00001f90: 5f70 726f 6d70 742c 2068 756d 616e 5f6d  _prompt, human_m
+00001fa0: 6573 7361 6765 5f70 726f 6d70 745d 295c  essage_prompt])\
+00001fb0: 6e5c 6e63 6861 696e 203d 204c 4c4d 4368  n\nchain = LLMCh
+00001fc0: 6169 6e28 6c6c 6d3d 6368 6174 2c20 7072  ain(llm=chat, pr
+00001fd0: 6f6d 7074 3d63 6861 745f 7072 6f6d 7074  ompt=chat_prompt
+00001fe0: 295c 6e63 6861 696e 2e72 756e 2869 6e70  )\nchain.run(inp
+00001ff0: 7574 5f6c 616e 6775 6167 653d 5c22 456e  ut_language=\"En
+00002000: 676c 6973 685c 222c 206f 7574 7075 745f  glish\", output_
+00002010: 6c61 6e67 7561 6765 3d5c 2246 7265 6e63  language=\"Frenc
+00002020: 685c 222c 2074 6578 743d 5c22 4920 6c6f  h\", text=\"I lo
+00002030: 7665 2070 726f 6772 616d 6d69 6e67 2e5c  ve programming.\
+00002040: 2229 5c6e 6060 6022 2c0a 2020 2020 2020  ")\n```",.      
+00002050: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00002060: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00002070: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00002080: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00002090: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+000020a0: 6869 6768 220a 2020 2020 2020 2020 2020  high".          
+000020b0: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+000020c0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000020d0: 2020 2020 2022 6964 223a 2022 6c61 6e67       "id": "lang
+000020e0: 6368 6169 6e2d 3922 2c0a 2020 2020 2020  chain-9",.      
+000020f0: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+00002100: 3a20 2254 656c 6c20 6d65 2061 626f 7574  : "Tell me about
+00002110: 2074 6865 2060 5141 4765 6e65 7261 7469   the `QAGenerati
+00002120: 6f6e 4368 6169 6e60 2e22 2c0a 2020 2020  onChain`.",.    
+00002130: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
+00002140: 6365 5f61 6e73 7765 7222 3a20 2254 6865  ce_answer": "The
+00002150: 2051 4147 656e 6572 6174 696f 6e43 6861   QAGenerationCha
+00002160: 696e 2069 7320 6120 6368 6169 6e20 696e  in is a chain in
+00002170: 204c 616e 6743 6861 696e 2074 6861 7420   LangChain that 
+00002180: 6765 6e65 7261 7465 7320 7175 6573 7469  generates questi
+00002190: 6f6e 2d61 6e73 7765 7220 7061 6972 7320  on-answer pairs 
+000021a0: 6f76 6572 2061 2073 7065 6369 6669 6320  over a specific 
+000021b0: 646f 6375 6d65 6e74 2e20 4974 2069 7320  document. It is 
+000021c0: 6120 7573 6566 756c 2074 6f6f 6c20 666f  a useful tool fo
+000021d0: 7220 6765 6e65 7261 7469 6e67 2065 7661  r generating eva
+000021e0: 6c75 6174 696f 6e20 6461 7461 2066 6f72  luation data for
+000021f0: 2071 7565 7374 696f 6e2d 616e 7377 6572   question-answer
+00002200: 696e 6720 7461 736b 7320 7768 656e 2079  ing tasks when y
+00002210: 6f75 2064 6f6e 2774 2068 6176 6520 6120  ou don't have a 
+00002220: 6c61 7267 6520 6461 7461 7365 7420 6f66  large dataset of
+00002230: 2065 7861 6d70 6c65 732e 2054 6865 2051   examples. The Q
+00002240: 4147 656e 6572 6174 696f 6e43 6861 696e  AGenerationChain
+00002250: 2074 616b 6573 2061 2064 6f63 756d 656e   takes a documen
+00002260: 7420 6173 2069 6e70 7574 2061 6e64 2067  t as input and g
+00002270: 656e 6572 6174 6573 2071 7565 7374 696f  enerates questio
+00002280: 6e2d 616e 7377 6572 2070 6169 7273 2074  n-answer pairs t
+00002290: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+000022a0: 746f 2065 7661 6c75 6174 6520 7175 6573  to evaluate ques
+000022b0: 7469 6f6e 2d61 6e73 7765 7269 6e67 2073  tion-answering s
+000022c0: 7973 7465 6d73 2e20 5468 6973 2061 6c6c  ystems. This all
+000022d0: 6f77 7320 796f 7520 746f 2065 7661 6c75  ows you to evalu
+000022e0: 6174 6520 7468 6520 7065 7266 6f72 6d61  ate the performa
+000022f0: 6e63 6520 6f66 2079 6f75 7220 7175 6573  nce of your ques
+00002300: 7469 6f6e 2d61 6e73 7765 7269 6e67 2073  tion-answering s
+00002310: 7973 7465 6d20 7769 7468 6f75 7420 7468  ystem without th
+00002320: 6520 6e65 6564 2066 6f72 2061 206c 6172  e need for a lar
+00002330: 6765 2061 6d6f 756e 7420 6f66 2070 7265  ge amount of pre
+00002340: 2d65 7869 7374 696e 6720 6461 7461 2e22  -existing data."
+00002350: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+00002360: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
+00002370: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
+00002380: 2020 2022 6e6f 7465 7322 3a20 7b0a 2020     "notes": {.  
+00002390: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+000023a0: 6576 656c 223a 2022 6c6f 7722 0a20 2020  evel": "low".   
+000023b0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+000023c0: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+000023d0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+000023e0: 3a20 226c 616e 6763 6861 696e 2d31 3022  : "langchain-10"
+000023f0: 2c0a 2020 2020 2020 2020 2020 2020 2271  ,.            "q
+00002400: 7565 7374 696f 6e22 3a20 2248 6f77 2064  uestion": "How d
+00002410: 6f20 4920 7265 7573 6520 616e 2065 7869  o I reuse an exi
+00002420: 7374 696e 6720 6051 6472 616e 7460 2063  sting `Qdrant` c
+00002430: 6f6c 6c65 6374 696f 6e3f 2050 726f 7669  ollection? Provi
+00002440: 6465 2061 6e20 6578 616d 706c 652e 222c  de an example.",
+00002450: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00002460: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+00002470: 2022 4966 2079 6f75 2077 616e 7420 746f   "If you want to
+00002480: 2072 6575 7365 2074 6865 2065 7869 7374   reuse the exist
+00002490: 696e 6720 636f 6c6c 6563 7469 6f6e 2c20  ing collection, 
+000024a0: 796f 7520 6361 6e20 616c 7761 7973 2063  you can always c
+000024b0: 7265 6174 6520 616e 2069 6e73 7461 6e63  reate an instanc
+000024c0: 6520 6f66 c2a0 5164 7261 6e74 c2a0 6f6e  e of..Qdrant..on
+000024d0: 2079 6f75 7220 6f77 6e20 616e 6420 7061   your own and pa
+000024e0: 7373 2074 6865 c2a0 5164 7261 6e74 436c  ss the..QdrantCl
+000024f0: 6965 6e74 c2a0 696e 7374 616e 6365 2077  ient..instance w
+00002500: 6974 6820 7468 6520 636f 6e6e 6563 7469  ith the connecti
+00002510: 6f6e 2064 6574 6169 6c73 2e5c 6e5c 6e60  on details.\n\n`
+00002520: 6060 7079 7468 6f6e 5c6e 696d 706f 7274  ``python\nimport
+00002530: 2071 6472 616e 745f 636c 6965 6e74 5c6e   qdrant_client\n
+00002540: 5c6e 636c 6965 6e74 203d 2071 6472 616e  \nclient = qdran
+00002550: 745f 636c 6965 6e74 2e51 6472 616e 7443  t_client.QdrantC
+00002560: 6c69 656e 7428 7061 7468 3d5c 222f 746d  lient(path=\"/tm
+00002570: 702f 6c6f 6361 6c5f 7164 7261 6e74 5c22  p/local_qdrant\"
+00002580: 2c20 7072 6566 6572 5f67 7270 633d 5472  , prefer_grpc=Tr
+00002590: 7565 295c 6e71 6472 616e 7420 3d20 5164  ue)\nqdrant = Qd
+000025a0: 7261 6e74 2863 6c69 656e 743d 636c 6965  rant(client=clie
+000025b0: 6e74 2c20 636f 6c6c 6563 7469 6f6e 5f6e  nt, collection_n
+000025c0: 616d 653d 5c22 6d79 5f64 6f63 756d 656e  ame=\"my_documen
+000025d0: 7473 5c22 2c20 656d 6265 6464 696e 6773  ts\", embeddings
+000025e0: 3d65 6d62 6564 6469 6e67 7329 5c6e 6060  =embeddings)\n``
+000025f0: 6022 2c0a 2020 2020 2020 2020 2020 2020  `",.            
+00002600: 2261 6e73 7765 725f 7072 6f70 6572 7469  "answer_properti
+00002610: 6573 223a 205b 5d2c 0a20 2020 2020 2020  es": [],.       
+00002620: 2020 2020 2022 6e6f 7465 7322 3a20 7b0a       "notes": {.
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 226c 6576 656c 223a 2022 6869 6768 220a  "level": "high".
+00002650: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00002660: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00002670: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002680: 6964 223a 2022 6c61 6e67 6368 6169 6e2d  id": "langchain-
+00002690: 3131 222c 0a20 2020 2020 2020 2020 2020  11",.           
+000026a0: 2022 7175 6573 7469 6f6e 223a 2022 5768   "question": "Wh
+000026b0: 6174 2064 6f65 7320 7468 6520 606d 6178  at does the `max
+000026c0: 5f6d 6172 6769 6e61 6c5f 7265 6c65 7661  _marginal_releva
+000026d0: 6e63 655f 7365 6172 6368 6020 6675 6e63  nce_search` func
+000026e0: 7469 6f6e 2064 6f3f 222c 0a20 2020 2020  tion do?",.     
+000026f0: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
+00002700: 655f 616e 7377 6572 223a 2022 5468 6520  e_answer": "The 
+00002710: 606d 6178 5f6d 6172 6769 6e61 6c5f 7265  `max_marginal_re
+00002720: 6c65 7661 6e63 655f 7365 6172 6368 6020  levance_search` 
+00002730: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
+00002740: 2061 206c 6973 7420 6f66 2064 6f63 756d   a list of docum
+00002750: 656e 7473 2073 656c 6563 7465 6420 7573  ents selected us
+00002760: 696e 6720 7468 6520 6d61 7869 6d61 6c20  ing the maximal 
+00002770: 6d61 7267 696e 616c 2072 656c 6576 616e  marginal relevan
+00002780: 6365 2061 6c67 6f72 6974 686d 2c20 7768  ce algorithm, wh
+00002790: 6963 6820 6f70 7469 6d69 7a65 7320 666f  ich optimizes fo
+000027a0: 7220 7369 6d69 6c61 7269 7479 2074 6f20  r similarity to 
+000027b0: 7468 6520 7175 6572 7920 616e 6420 6469  the query and di
+000027c0: 7665 7273 6974 7920 616d 6f6e 6720 7468  versity among th
+000027d0: 6520 7365 6c65 6374 6564 2064 6f63 756d  e selected docum
+000027e0: 656e 7473 2e22 2c0a 2020 2020 2020 2020  ents.",.        
+000027f0: 2020 2020 2261 6e73 7765 725f 7072 6f70      "answer_prop
+00002800: 6572 7469 6573 223a 205b 5d2c 0a20 2020  erties": [],.   
+00002810: 2020 2020 2020 2020 2022 6e6f 7465 7322           "notes"
+00002820: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00002830: 2020 2020 226c 6576 656c 223a 2022 6c6f      "level": "lo
+00002840: 7722 0a20 2020 2020 2020 2020 2020 207d  w".            }
+00002850: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00002860: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00002870: 2020 2269 6422 3a20 226c 616e 6763 6861    "id": "langcha
+00002880: 696e 2d31 3222 2c0a 2020 2020 2020 2020  in-12",.        
+00002890: 2020 2020 2271 7565 7374 696f 6e22 3a20      "question": 
+000028a0: 2257 6861 7420 6973 2074 6865 2070 7572  "What is the pur
+000028b0: 706f 7365 206f 6620 7468 6520 6051 6472  pose of the `Qdr
+000028c0: 616e 7460 2063 6c61 7373 3f22 2c0a 2020  ant` class?",.  
+000028d0: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
+000028e0: 656e 6365 5f61 6e73 7765 7222 3a20 2254  ence_answer": "T
+000028f0: 6865 2070 7572 706f 7365 206f 6620 7468  he purpose of th
+00002900: 6520 5164 7261 6e74 2063 6c61 7373 2069  e Qdrant class i
+00002910: 7320 746f 2073 6572 7665 2061 7320 6120  s to serve as a 
+00002920: 7772 6170 7065 7220 6172 6f75 6e64 2074  wrapper around t
+00002930: 6865 2051 6472 616e 7420 7665 6374 6f72  he Qdrant vector
+00002940: 2064 6174 6162 6173 652e 222c 0a20 2020   database.",.   
+00002950: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
+00002960: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
+00002970: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00002980: 6f74 6573 223a 207b 0a20 2020 2020 2020  otes": {.       
+00002990: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
+000029a0: 3a20 226d 6964 220a 2020 2020 2020 2020  : "mid".        
+000029b0: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
+000029c0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+000029d0: 2020 2020 2020 2022 6964 223a 2022 6c61         "id": "la
+000029e0: 6e67 6368 6169 6e2d 3133 222c 0a20 2020  ngchain-13",.   
+000029f0: 2020 2020 2020 2020 2022 7175 6573 7469           "questi
+00002a00: 6f6e 223a 2022 5768 6174 2064 6f65 7320  on": "What does 
+00002a10: 7468 6520 6073 6176 655f 636f 6e74 6578  the `save_contex
+00002a20: 7460 206d 6574 686f 6420 6f66 2043 6f6e  t` method of Con
+00002a30: 7665 7273 6174 696f 6e45 6e74 6974 794d  versationEntityM
+00002a40: 656d 6f72 7920 646f 3f22 2c0a 2020 2020  emory do?",.    
+00002a50: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
+00002a60: 6365 5f61 6e73 7765 7222 3a20 2254 6865  ce_answer": "The
+00002a70: 2060 7361 7665 5f63 6f6e 7465 7874 6020   `save_context` 
+00002a80: 6d65 7468 6f64 2073 6176 6573 2074 6865  method saves the
+00002a90: 2063 6f6e 7465 7874 2066 726f 6d20 7468   context from th
+00002aa0: 6520 636f 6e76 6572 7361 7469 6f6e 2068  e conversation h
+00002ab0: 6973 746f 7279 2074 6f20 7468 6520 656e  istory to the en
+00002ac0: 7469 7479 2073 746f 7265 2062 7920 6765  tity store by ge
+00002ad0: 6e65 7261 7469 6e67 2073 756d 6d61 7269  nerating summari
+00002ae0: 6573 2066 6f72 2065 6163 6820 656e 7469  es for each enti
+00002af0: 7479 2069 6e20 7468 6520 656e 7469 7479  ty in the entity
+00002b00: 2063 6163 6865 2e22 2c0a 2020 2020 2020   cache.",.      
+00002b10: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00002b20: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00002b30: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00002b40: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00002b50: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+00002b60: 6d69 6422 0a20 2020 2020 2020 2020 2020  mid".           
+00002b70: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00002b80: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00002b90: 2020 2020 2269 6422 3a20 226c 616e 6763      "id": "langc
+00002ba0: 6861 696e 2d31 3422 2c0a 2020 2020 2020  hain-14",.      
+00002bb0: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+00002bc0: 3a20 2257 6861 7420 6973 2074 6865 2075  : "What is the u
+00002bd0: 7365 206f 6620 7468 6520 6043 6f6e 7665  se of the `Conve
+00002be0: 7273 6174 696f 6e42 7566 6665 724d 656d  rsationBufferMem
+00002bf0: 6f72 7960 2063 6c61 7373 3f22 2c0a 2020  ory` class?",.  
+00002c00: 2020 2020 2020 2020 2020 2272 6566 6572            "refer
+00002c10: 656e 6365 5f61 6e73 7765 7222 3a20 2254  ence_answer": "T
+00002c20: 6865 2070 7572 706f 7365 206f 6620 7468  he purpose of th
+00002c30: 6520 436f 6e76 6572 7361 7469 6f6e 4275  e ConversationBu
+00002c40: 6666 6572 4d65 6d6f 7279 2063 6c61 7373  fferMemory class
+00002c50: 2069 7320 746f 2073 746f 7265 2063 6f6e   is to store con
+00002c60: 7665 7273 6174 696f 6e20 6d65 6d6f 7279  versation memory
+00002c70: 2069 6e20 6120 7374 7269 6e67 2062 7566   in a string buf
+00002c80: 6665 722e 222c 0a20 2020 2020 2020 2020  fer.",.         
+00002c90: 2020 2022 616e 7377 6572 5f70 726f 7065     "answer_prope
+00002ca0: 7274 6965 7322 3a20 5b5d 2c0a 2020 2020  rties": [],.    
+00002cb0: 2020 2020 2020 2020 226e 6f74 6573 223a          "notes":
+00002cc0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002cd0: 2020 2022 6c65 7665 6c22 3a20 226d 6964     "level": "mid
+00002ce0: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
+00002cf0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002d00: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00002d10: 2022 6964 223a 2022 6c61 6e67 6368 6169   "id": "langchai
+00002d20: 6e2d 3135 222c 0a20 2020 2020 2020 2020  n-15",.         
+00002d30: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
+00002d40: 5768 6174 2069 7320 6120 7072 6f6d 7074  What is a prompt
+00002d50: 2074 656d 706c 6174 653f 222c 0a20 2020   template?",.   
+00002d60: 2020 2020 2020 2020 2022 7265 6665 7265           "refere
+00002d70: 6e63 655f 616e 7377 6572 223a 2022 4120  nce_answer": "A 
+00002d80: 7072 6f6d 7074 2074 656d 706c 6174 6520  prompt template 
+00002d90: 7265 6665 7273 2074 6f20 6120 7265 7072  refers to a repr
+00002da0: 6f64 7563 6962 6c65 2077 6179 2074 6f20  oducible way to 
+00002db0: 6765 6e65 7261 7465 2061 2070 726f 6d70  generate a promp
+00002dc0: 742e 2049 7420 636f 6e74 6169 6e73 2061  t. It contains a
+00002dd0: 2074 6578 7420 7374 7269 6e67 2028 5c22   text string (\"
+00002de0: 7468 6520 7465 6d70 6c61 7465 5c22 2920  the template\") 
+00002df0: 7468 6174 2063 616e 2074 616b 6520 696e  that can take in
+00002e00: 2061 2073 6574 206f 6620 7061 7261 6d65   a set of parame
+00002e10: 7465 7273 2066 726f 6d20 7468 6520 656e  ters from the en
+00002e20: 6420 7573 6572 2061 6e64 2067 656e 6572  d user and gener
+00002e30: 6174 6573 2061 2070 726f 6d70 742e 2041  ates a prompt. A
+00002e40: 2070 726f 6d70 7420 7465 6d70 6c61 7465   prompt template
+00002e50: 2063 616e 2069 6e63 6c75 6465 2069 6e73   can include ins
+00002e60: 7472 7563 7469 6f6e 7320 746f 2074 6865  tructions to the
+00002e70: 206c 616e 6775 6167 6520 6d6f 6465 6c2c   language model,
+00002e80: 2061 2073 6574 206f 6620 6665 772d 7368   a set of few-sh
+00002e90: 6f74 2065 7861 6d70 6c65 7320 746f 2068  ot examples to h
+00002ea0: 656c 7020 7468 6520 6c61 6e67 7561 6765  elp the language
+00002eb0: 206d 6f64 656c 2067 656e 6572 6174 6520   model generate 
+00002ec0: 6120 6265 7474 6572 2072 6573 706f 6e73  a better respons
+00002ed0: 652c 2061 6e64 2061 2071 7565 7374 696f  e, and a questio
+00002ee0: 6e20 746f 2074 6865 206c 616e 6775 6167  n to the languag
+00002ef0: 6520 6d6f 6465 6c2e 2050 726f 6d70 7420  e model. Prompt 
+00002f00: 7465 6d70 6c61 7465 7320 6361 6e20 6265  templates can be
+00002f10: 2063 7265 6174 6564 2075 7369 6e67 2074   created using t
+00002f20: 6865 c2a0 5072 6f6d 7074 5465 6d70 6c61  he..PromptTempla
+00002f30: 7465 c2a0 636c 6173 7320 696e 204c 616e  te..class in Lan
+00002f40: 6743 6861 696e 2e22 2c0a 2020 2020 2020  gChain.",.      
+00002f50: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00002f60: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00002f70: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00002f80: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00002f90: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+00002fa0: 6d69 6422 0a20 2020 2020 2020 2020 2020  mid".           
+00002fb0: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00002fc0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00002fd0: 2020 2020 2269 6422 3a20 226c 616e 6763      "id": "langc
+00002fe0: 6861 696e 2d31 3622 2c0a 2020 2020 2020  hain-16",.      
+00002ff0: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
+00003000: 3a20 2249 7320 7468 6572 6520 6120 6361  : "Is there a ca
+00003010: 6368 696e 6720 6d65 6368 616e 6973 6d20  ching mechanism 
+00003020: 666f 7220 4c4c 4d73 3f22 2c0a 2020 2020  for LLMs?",.    
+00003030: 2020 2020 2020 2020 2272 6566 6572 656e          "referen
+00003040: 6365 5f61 6e73 7765 7222 3a20 2259 6573  ce_answer": "Yes
+00003050: 2c20 7468 6572 6520 6973 2061 2063 6163  , there is a cac
+00003060: 6869 6e67 206d 6563 6861 6e69 736d 2066  hing mechanism f
+00003070: 6f72 204c 4c4d 7320 284c 616e 6775 6167  or LLMs (Languag
+00003080: 6520 4d6f 6465 6c73 292e 2043 6163 6869  e Models). Cachi
+00003090: 6e67 2063 616e 2062 6520 7573 6564 2074  ng can be used t
+000030a0: 6f20 7361 7665 206d 6f6e 6579 2062 7920  o save money by 
+000030b0: 7265 6475 6369 6e67 2074 6865 206e 756d  reducing the num
+000030c0: 6265 7220 6f66 2041 5049 2063 616c 6c73  ber of API calls
+000030d0: 206d 6164 6520 746f 2074 6865 204c 4c4d   made to the LLM
+000030e0: 2070 726f 7669 6465 7220 616e 6420 746f   provider and to
+000030f0: 2073 7065 6564 2075 7020 6170 706c 6963   speed up applic
+00003100: 6174 696f 6e73 2062 7920 7265 6475 6369  ations by reduci
+00003110: 6e67 2074 6865 206e 756d 6265 7220 6f66  ng the number of
+00003120: 2041 5049 2063 616c 6c73 2e20 5468 6572   API calls. Ther
+00003130: 6520 6172 6520 6469 6666 6572 656e 7420  e are different 
+00003140: 6361 6368 696e 6720 6f70 7469 6f6e 7320  caching options 
+00003150: 6176 6169 6c61 626c 6520 7375 6368 2061  available such a
+00003160: 7320 496e 204d 656d 6f72 7920 4361 6368  s In Memory Cach
+00003170: 652c 2053 514c 6974 6520 4361 6368 652c  e, SQLite Cache,
+00003180: 2052 6564 6973 2043 6163 6865 2c20 5365   Redis Cache, Se
+00003190: 6d61 6e74 6963 2043 6163 6865 2c20 4750  mantic Cache, GP
+000031a0: 5443 6163 6865 2c20 4d6f 6d65 6e74 6f20  TCache, Momento 
+000031b0: 4361 6368 652c 2061 6e64 2053 514c 416c  Cache, and SQLAl
+000031c0: 6368 656d 7920 4361 6368 652e 2054 6865  chemy Cache. The
+000031d0: 7365 2063 6163 6869 6e67 206f 7074 696f  se caching optio
+000031e0: 6e73 2063 616e 2062 6520 7573 6564 2074  ns can be used t
+000031f0: 6f20 6361 6368 6520 7072 6f6d 7074 7320  o cache prompts 
+00003200: 616e 6420 7265 7370 6f6e 7365 732c 2061  and responses, a
+00003210: 6e64 2073 6f6d 6520 6f66 2074 6865 6d20  nd some of them 
+00003220: 6576 656e 2073 7570 706f 7274 2063 6163  even support cac
+00003230: 6869 6e67 2062 6173 6564 206f 6e20 7365  hing based on se
+00003240: 6d61 6e74 6963 2073 696d 696c 6172 6974  mantic similarit
+00003250: 792e 2041 6464 6974 696f 6e61 6c6c 792c  y. Additionally,
+00003260: 2063 6163 6869 6e67 2063 616e 2062 6520   caching can be 
+00003270: 7475 726e 6564 206f 6666 2066 6f72 2073  turned off for s
+00003280: 7065 6369 6669 6320 4c4c 4d73 2069 6620  pecific LLMs if 
+00003290: 6465 7369 7265 642e 222c 0a20 2020 2020  desired.",.     
+000032a0: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
+000032b0: 726f 7065 7274 6965 7322 3a20 5b5d 2c0a  roperties": [],.
+000032c0: 2020 2020 2020 2020 2020 2020 226e 6f74              "not
+000032d0: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
+000032e0: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
+000032f0: 226d 6964 220a 2020 2020 2020 2020 2020  "mid".          
+00003300: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+00003310: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00003320: 2020 2020 2022 6964 223a 2022 6c61 6e67       "id": "lang
+00003330: 6368 6169 6e2d 3137 222c 0a20 2020 2020  chain-17",.     
+00003340: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
+00003350: 223a 2022 4769 7665 206d 6520 6120 6c69  ": "Give me a li
+00003360: 7374 206f 6620 7468 6520 6d61 696e 2063  st of the main c
+00003370: 6f6d 706f 6e65 6e74 7320 6f66 204c 616e  omponents of Lan
+00003380: 6763 6861 696e 2e22 2c0a 2020 2020 2020  gchain.",.      
+00003390: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
+000033a0: 5f61 6e73 7765 7222 3a20 2254 6865 206d  _answer": "The m
+000033b0: 6169 6e20 636f 6d70 6f6e 656e 7473 206f  ain components o
+000033c0: 6620 4c61 6e67 4368 6169 6e20 6172 6520  f LangChain are 
+000033d0: 6173 2066 6f6c 6c6f 7773 3a5c 6e5c 6e4d  as follows:\n\nM
+000033e0: 6f64 656c 733a 204c 616e 6743 6861 696e  odels: LangChain
+000033f0: 2073 7570 706f 7274 7320 7661 7269 6f75   supports variou
+00003400: 7320 6d6f 6465 6c20 7479 7065 7320 616e  s model types an
+00003410: 6420 6d6f 6465 6c20 696e 7465 6772 6174  d model integrat
+00003420: 696f 6e73 2e5c 6e50 726f 6d70 7473 3a20  ions.\nPrompts: 
+00003430: 5468 6973 206d 6f64 756c 6520 696e 636c  This module incl
+00003440: 7564 6573 2070 726f 6d70 7420 6d61 6e61  udes prompt mana
+00003450: 6765 6d65 6e74 2c20 7072 6f6d 7074 206f  gement, prompt o
+00003460: 7074 696d 697a 6174 696f 6e2c 2061 6e64  ptimization, and
+00003470: 2070 726f 6d70 7420 7365 7269 616c 697a   prompt serializ
+00003480: 6174 696f 6e2e 5c6e 4d65 6d6f 7279 3a20  ation.\nMemory: 
+00003490: 4c61 6e67 4368 6169 6e20 7072 6f76 6964  LangChain provid
+000034a0: 6573 2061 2073 7461 6e64 6172 6420 696e  es a standard in
+000034b0: 7465 7266 6163 6520 666f 7220 6d65 6d6f  terface for memo
+000034c0: 7279 2c20 6120 636f 6c6c 6563 7469 6f6e  ry, a collection
+000034d0: 206f 6620 6d65 6d6f 7279 2069 6d70 6c65   of memory imple
+000034e0: 6d65 6e74 6174 696f 6e73 2c20 616e 6420  mentations, and 
+000034f0: 6578 616d 706c 6573 206f 6620 6368 6169  examples of chai
+00003500: 6e73 2f61 6765 6e74 7320 7468 6174 2075  ns/agents that u
+00003510: 7365 206d 656d 6f72 792e 5c6e 496e 6465  se memory.\nInde
+00003520: 7865 733a 2054 6869 7320 6d6f 6475 6c65  xes: This module
+00003530: 2063 6f76 6572 7320 6265 7374 2070 7261   covers best pra
+00003540: 6374 6963 6573 2066 6f72 2063 6f6d 6269  ctices for combi
+00003550: 6e69 6e67 206c 616e 6775 6167 6520 6d6f  ning language mo
+00003560: 6465 6c73 2077 6974 6820 796f 7572 206f  dels with your o
+00003570: 776e 2074 6578 7420 6461 7461 2e5c 6e43  wn text data.\nC
+00003580: 6861 696e 733a 204c 616e 6743 6861 696e  hains: LangChain
+00003590: 2070 726f 7669 6465 7320 6120 7374 616e   provides a stan
+000035a0: 6461 7264 2069 6e74 6572 6661 6365 2066  dard interface f
+000035b0: 6f72 2063 6861 696e 732c 2069 6e74 6567  or chains, integ
+000035c0: 7261 7469 6f6e 7320 7769 7468 206f 7468  rations with oth
+000035d0: 6572 2074 6f6f 6c73 2c20 616e 6420 656e  er tools, and en
+000035e0: 642d 746f 2d65 6e64 2063 6861 696e 7320  d-to-end chains 
+000035f0: 666f 7220 636f 6d6d 6f6e 2061 7070 6c69  for common appli
+00003600: 6361 7469 6f6e 732e 5c6e 4167 656e 7473  cations.\nAgents
+00003610: 3a20 4c61 6e67 4368 6169 6e20 7072 6f76  : LangChain prov
+00003620: 6964 6573 2061 2073 7461 6e64 6172 6420  ides a standard 
+00003630: 696e 7465 7266 6163 6520 666f 7220 6167  interface for ag
+00003640: 656e 7473 2c20 6120 7365 6c65 6374 696f  ents, a selectio
+00003650: 6e20 6f66 2061 6765 6e74 7320 746f 2063  n of agents to c
+00003660: 686f 6f73 6520 6672 6f6d 2c20 616e 6420  hoose from, and 
+00003670: 6578 616d 706c 6573 206f 6620 656e 642d  examples of end-
+00003680: 746f 2d65 6e64 2061 6765 6e74 732e 5c6e  to-end agents.\n
+00003690: 5c6e 5468 6573 6520 636f 6d70 6f6e 656e  \nThese componen
+000036a0: 7473 2063 616e 2062 6520 7573 6564 2069  ts can be used i
+000036b0: 6e20 7661 7269 6f75 7320 7761 7973 2c20  n various ways, 
+000036c0: 696e 636c 7564 696e 6720 666f 7220 7065  including for pe
+000036d0: 7273 6f6e 616c 2061 7373 6973 7461 6e74  rsonal assistant
+000036e0: 732c 2071 7565 7374 696f 6e20 616e 7377  s, question answ
+000036f0: 6572 696e 672c 2063 6861 7462 6f74 732c  ering, chatbots,
+00003700: 2071 7565 7279 696e 6720 7461 6275 6c61   querying tabula
+00003710: 7220 6461 7461 2c20 696e 7465 7261 6374  r data, interact
+00003720: 696e 6720 7769 7468 2041 5049 732c 2065  ing with APIs, e
+00003730: 7874 7261 6374 696f 6e2c 2073 756d 6d61  xtraction, summa
+00003740: 7269 7a61 7469 6f6e 2c20 616e 6420 6576  rization, and ev
+00003750: 616c 7561 7469 6f6e 2e20 4164 6469 7469  aluation. Additi
+00003760: 6f6e 616c 6c79 2c20 4c61 6e67 4368 6169  onally, LangChai
+00003770: 6e20 7072 6f76 6964 6573 2072 6566 6572  n provides refer
+00003780: 656e 6365 2064 6f63 756d 656e 7461 7469  ence documentati
+00003790: 6f6e 2066 6f72 2061 6c6c 2069 7473 2066  on for all its f
+000037a0: 6561 7475 7265 7320 616e 6420 616e 2065  eatures and an e
+000037b0: 636f 7379 7374 656d 2066 6f72 2069 6e74  cosystem for int
+000037c0: 6567 7261 7469 6e67 2077 6974 6820 6f74  egrating with ot
+000037d0: 6865 7220 636f 6d70 616e 6965 732f 7072  her companies/pr
+000037e0: 6f64 7563 7473 2e22 2c0a 2020 2020 2020  oducts.",.      
+000037f0: 2020 2020 2020 2261 6e73 7765 725f 7072        "answer_pr
+00003800: 6f70 6572 7469 6573 223a 205b 5d2c 0a20  operties": [],. 
+00003810: 2020 2020 2020 2020 2020 2022 6e6f 7465             "note
+00003820: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+00003830: 2020 2020 2020 226c 6576 656c 223a 2022        "level": "
+00003840: 6869 6768 220a 2020 2020 2020 2020 2020  high".          
+00003850: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+00003860: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00003870: 2020 2020 2022 6964 223a 2022 6c61 6e67       "id": "lang
+00003880: 6368 6169 6e2d 3138 222c 0a20 2020 2020  chain-18",.     
+00003890: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
+000038a0: 223a 2022 4469 6666 6572 656e 6365 2062  ": "Difference b
+000038b0: 2f74 2061 2072 6561 6374 2061 6765 6e74  /t a react agent
+000038c0: 2061 6e64 2061 2070 6c61 6e2d 616e 642d   and a plan-and-
+000038d0: 6578 6563 7574 6520 6167 656e 743f 222c  execute agent?",
+000038e0: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+000038f0: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+00003900: 2022 4120 5265 4163 7420 6167 656e 7420   "A ReAct agent 
+00003910: 616e 6420 6120 706c 616e 2d61 6e64 2d65  and a plan-and-e
+00003920: 7865 6375 7465 2061 6765 6e74 2061 7265  xecute agent are
+00003930: 2074 776f 2064 6966 6665 7265 6e74 2074   two different t
+00003940: 7970 6573 206f 6620 6167 656e 7473 2069  ypes of agents i
+00003950: 6e20 7468 6520 4c61 6e67 4368 6169 6e20  n the LangChain 
+00003960: 6672 616d 6577 6f72 6b2e 5c6e 5c6e 4120  framework.\n\nA 
+00003970: 5265 4163 7420 6167 656e 742c 2077 6869  ReAct agent, whi
+00003980: 6368 2073 7461 6e64 7320 666f 7220 5c22  ch stands for \"
+00003990: 5265 6163 7469 6f6e 2041 6765 6e74 2c5c  Reaction Agent,\
+000039a0: 2220 7573 6573 2074 6865 2052 6541 6374  " uses the ReAct
+000039b0: 2066 7261 6d65 776f 726b 2074 6f20 6465   framework to de
+000039c0: 7465 726d 696e 6520 7768 6963 6820 746f  termine which to
+000039d0: 6f6c 2074 6f20 7573 6520 6261 7365 6420  ol to use based 
+000039e0: 6f6e 2074 6865 2074 6f6f 6c27 7320 6465  on the tool's de
+000039f0: 7363 7269 7074 696f 6e2e 2049 7420 6361  scription. It ca
+00003a00: 6e20 7573 6520 6d75 6c74 6970 6c65 2074  n use multiple t
+00003a10: 6f6f 6c73 2061 6e64 2069 7320 6465 7369  ools and is desi
+00003a20: 676e 6564 2074 6f20 6265 2075 7365 6420  gned to be used 
+00003a30: 696e 2063 6f6e 7665 7273 6174 696f 6e61  in conversationa
+00003a40: 6c20 7365 7474 696e 6773 2e20 4974 2075  l settings. It u
+00003a50: 7365 7320 6d65 6d6f 7279 2074 6f20 7265  ses memory to re
+00003a60: 6d65 6d62 6572 2070 7265 7669 6f75 7320  member previous 
+00003a70: 636f 6e76 6572 7361 7469 6f6e 2069 6e74  conversation int
+00003a80: 6572 6163 7469 6f6e 7320 616e 6420 6465  eractions and de
+00003a90: 6369 6465 7320 7468 6520 6e65 7874 2073  cides the next s
+00003aa0: 7465 7020 7573 696e 6720 7468 6520 6869  tep using the hi
+00003ab0: 7374 6f72 7920 6f66 2074 6f6f 6c73 2c20  story of tools, 
+00003ac0: 746f 6f6c 2069 6e70 7574 732c 2061 6e64  tool inputs, and
+00003ad0: 206f 6273 6572 7661 7469 6f6e 732e 2052   observations. R
+00003ae0: 6541 6374 2061 6765 6e74 7320 6172 6520  eAct agents are 
+00003af0: 7375 6974 6162 6c65 2066 6f72 2073 6d61  suitable for sma
+00003b00: 6c6c 2074 6173 6b73 2061 6e64 2061 7265  ll tasks and are
+00003b10: 2077 7261 7070 6564 2069 6e20 6167 656e   wrapped in agen
+00003b20: 7420 6578 6563 7574 6f72 732e 5c6e 5c6e  t executors.\n\n
+00003b30: 4f6e 2074 6865 206f 7468 6572 2068 616e  On the other han
+00003b40: 642c 2061 2070 6c61 6e2d 616e 642d 6578  d, a plan-and-ex
+00003b50: 6563 7574 6520 6167 656e 7420 706c 616e  ecute agent plan
+00003b60: 7320 7468 6520 6675 6c6c 2073 6571 7565  s the full seque
+00003b70: 6e63 6520 6f66 2073 7465 7073 2074 6f20  nce of steps to 
+00003b80: 6163 636f 6d70 6c69 7368 2061 6e20 6f62  accomplish an ob
+00003b90: 6a65 6374 6976 6520 616e 6420 7468 656e  jective and then
+00003ba0: 2065 7865 6375 7465 7320 7468 6f73 6520   executes those 
+00003bb0: 7374 6570 7320 696e 206f 7264 6572 2e20  steps in order. 
+00003bc0: 5468 6520 706c 616e 6e69 6e67 2069 7320  The planning is 
+00003bd0: 7573 7561 6c6c 7920 646f 6e65 2062 7920  usually done by 
+00003be0: 6120 6c61 6e67 7561 6765 206d 6f64 656c  a language model
+00003bf0: 2028 4c4c 4d29 2c20 616e 6420 7468 6520   (LLM), and the 
+00003c00: 6578 6563 7574 696f 6e20 6973 2064 6f6e  execution is don
+00003c10: 6520 6279 2061 2073 6570 6172 6174 6520  e by a separate 
+00003c20: 6167 656e 7420 6571 7569 7070 6564 2077  agent equipped w
+00003c30: 6974 6820 746f 6f6c 732e 2050 6c61 6e2d  ith tools. Plan-
+00003c40: 616e 642d 6578 6563 7574 6520 6167 656e  and-execute agen
+00003c50: 7473 2061 7265 2062 6574 7465 7220 7375  ts are better su
+00003c60: 6974 6564 2066 6f72 2063 6f6d 706c 6578  ited for complex
+00003c70: 206f 7220 6c6f 6e67 2d72 756e 6e69 6e67   or long-running
+00003c80: 2074 6173 6b73 2074 6861 7420 7265 7175   tasks that requ
+00003c90: 6972 6520 6d61 696e 7461 696e 696e 6720  ire maintaining 
+00003ca0: 6c6f 6e67 2d74 6572 6d20 6f62 6a65 6374  long-term object
+00003cb0: 6976 6573 2061 6e64 2066 6f63 7573 2e5c  ives and focus.\
+00003cc0: 6e5c 6e49 6e20 7375 6d6d 6172 792c 2061  n\nIn summary, a
+00003cd0: 2052 6541 6374 2061 6765 6e74 2075 7365   ReAct agent use
+00003ce0: 7320 7468 6520 5265 4163 7420 6672 616d  s the ReAct fram
+00003cf0: 6577 6f72 6b20 746f 2064 6563 6964 6520  ework to decide 
+00003d00: 7768 6963 6820 746f 6f6c 2074 6f20 7573  which tool to us
+00003d10: 6520 6261 7365 6420 6f6e 2074 6865 2074  e based on the t
+00003d20: 6f6f 6c27 7320 6465 7363 7269 7074 696f  ool's descriptio
+00003d30: 6e20 616e 6420 6973 2064 6573 6967 6e65  n and is designe
+00003d40: 6420 666f 7220 636f 6e76 6572 7361 7469  d for conversati
+00003d50: 6f6e 616c 2073 6574 7469 6e67 732e 2041  onal settings. A
+00003d60: 2070 6c61 6e2d 616e 642d 6578 6563 7574   plan-and-execut
+00003d70: 6520 6167 656e 7420 706c 616e 7320 7468  e agent plans th
+00003d80: 6520 6675 6c6c 2073 6571 7565 6e63 6520  e full sequence 
+00003d90: 6f66 2073 7465 7073 2061 6e64 2065 7865  of steps and exe
+00003da0: 6375 7465 7320 7468 656d 2069 6e20 6f72  cutes them in or
+00003db0: 6465 722c 206d 616b 696e 6720 6974 2073  der, making it s
+00003dc0: 7569 7461 626c 6520 666f 7220 636f 6d70  uitable for comp
+00003dd0: 6c65 7820 7461 736b 732e 222c 0a20 2020  lex tasks.",.   
+00003de0: 2020 2020 2020 2020 2022 616e 7377 6572           "answer
+00003df0: 5f70 726f 7065 7274 6965 7322 3a20 5b5d  _properties": []
+00003e00: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00003e10: 6f74 6573 223a 207b 0a20 2020 2020 2020  otes": {.       
+00003e20: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
+00003e30: 3a20 2268 6967 6822 0a20 2020 2020 2020  : "high".       
+00003e40: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00003e50: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00003e60: 2020 2020 2020 2020 2269 6422 3a20 226c          "id": "l
+00003e70: 616e 6763 6861 696e 2d31 3922 2c0a 2020  angchain-19",.  
+00003e80: 2020 2020 2020 2020 2020 2271 7565 7374            "quest
+00003e90: 696f 6e22 3a20 2249 7320 7468 6572 6520  ion": "Is there 
+00003ea0: 6120 6053 656c 6651 7565 7279 5265 7472  a `SelfQueryRetr
+00003eb0: 6965 7665 7260 2066 6f72 2060 4d69 6c76  iever` for `Milv
+00003ec0: 7573 603f 222c 0a20 2020 2020 2020 2020  us`?",.         
+00003ed0: 2020 2022 7265 6665 7265 6e63 655f 616e     "reference_an
+00003ee0: 7377 6572 223a 2022 4e6f 2e20 5365 6c66  swer": "No. Self
+00003ef0: 2071 7565 7279 696e 6720 666f 7220 4d69   querying for Mi
+00003f00: 6c76 7573 2069 7320 6e6f 7420 7375 7070  lvus is not supp
+00003f10: 6f72 7465 642e 222c 0a20 2020 2020 2020  orted.",.       
+00003f20: 2020 2020 2022 616e 7377 6572 5f70 726f       "answer_pro
+00003f30: 7065 7274 6965 7322 3a20 5b5d 2c0a 2020  perties": [],.  
+00003f40: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
+00003f50: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00003f60: 2020 2020 2022 6c65 7665 6c22 3a20 226d       "level": "m
+00003f70: 6964 220a 2020 2020 2020 2020 2020 2020  id".            
+00003f80: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00003f90: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00003fa0: 2020 2022 6964 223a 2022 6c61 6e67 6368     "id": "langch
+00003fb0: 6169 6e2d 3230 222c 0a20 2020 2020 2020  ain-20",.       
+00003fc0: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
+00003fd0: 2022 486f 7720 646f 2049 2064 6566 696e   "How do I defin
+00003fe0: 6520 6120 6375 7374 6f6d 2074 6f6f 6c3f  e a custom tool?
+00003ff0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00004000: 7265 6665 7265 6e63 655f 616e 7377 6572  reference_answer
+00004010: 223a 2022 546f 2064 6566 696e 6520 6120  ": "To define a 
+00004020: 6375 7374 6f6d 2074 6f6f 6c2c 2079 6f75  custom tool, you
+00004030: 2063 616e 2075 7365 2065 6974 6865 7220   can use either 
+00004040: 7468 6520 546f 6f6c 2064 6174 6163 6c61  the Tool datacla
+00004050: 7373 206f 7220 7375 6263 6c61 7373 2074  ss or subclass t
+00004060: 6865 2042 6173 6554 6f6f 6c20 636c 6173  he BaseTool clas
+00004070: 732e 5c6e 5c6e 5573 696e 6720 7468 6520  s.\n\nUsing the 
+00004080: 546f 6f6c 2064 6174 6163 6c61 7373 3a5c  Tool dataclass:\
+00004090: 6e49 6d70 6f72 7420 7468 6520 6e65 6365  nImport the nece
+000040a0: 7373 6172 7920 6d6f 6475 6c65 733a 2066  ssary modules: f
+000040b0: 726f 6d20 6c61 6e67 6368 6169 6e20 696d  rom langchain im
+000040c0: 706f 7274 2054 6f6f 6c5c 6e44 6566 696e  port Tool\nDefin
+000040d0: 6520 7468 6520 746f 6f6c 2075 7369 6e67  e the tool using
+000040e0: 2074 6865 2054 6f6f 6c20 6461 7461 636c   the Tool datacl
+000040f0: 6173 732c 2070 726f 7669 6469 6e67 2074  ass, providing t
+00004100: 6865 2072 6571 7569 7265 6420 636f 6d70  he required comp
+00004110: 6f6e 656e 7473 2073 7563 6820 6173 206e  onents such as n
+00004120: 616d 652c 2064 6573 6372 6970 7469 6f6e  ame, description
+00004130: 2c20 616e 6420 6675 6e63 7469 6f6e 2e5c  , and function.\
+00004140: 6e4f 7074 696f 6e61 6c6c 792c 2079 6f75  nOptionally, you
+00004150: 2063 616e 2064 6566 696e 6520 616e 2061   can define an a
+00004160: 7267 735f 7363 6865 6d61 2074 6f20 7072  rgs_schema to pr
+00004170: 6f76 6964 6520 6d6f 7265 2069 6e66 6f72  ovide more infor
+00004180: 6d61 7469 6f6e 206f 7220 7661 6c69 6461  mation or valida
+00004190: 7469 6f6e 2066 6f72 2065 7870 6563 7465  tion for expecte
+000041a0: 6420 7061 7261 6d65 7465 7273 2e5c 6e53  d parameters.\nS
+000041b0: 7562 636c 6173 7369 6e67 2074 6865 2042  ubclassing the B
+000041c0: 6173 6554 6f6f 6c20 636c 6173 733a 5c6e  aseTool class:\n
+000041d0: 496d 706f 7274 2074 6865 206e 6563 6573  Import the neces
+000041e0: 7361 7279 206d 6f64 756c 6573 3a20 6672  sary modules: fr
+000041f0: 6f6d 206c 616e 6763 6861 696e 2069 6d70  om langchain imp
+00004200: 6f72 7420 4261 7365 546f 6f6c 5c6e 4372  ort BaseTool\nCr
+00004210: 6561 7465 2061 2063 7573 746f 6d20 636c  eate a custom cl
+00004220: 6173 7320 7468 6174 2073 7562 636c 6173  ass that subclas
+00004230: 7365 7320 4261 7365 546f 6f6c 2e5c 6e49  ses BaseTool.\nI
+00004240: 6d70 6c65 6d65 6e74 2074 6865 206e 6563  mplement the nec
+00004250: 6573 7361 7279 206d 6574 686f 6473 2061  essary methods a
+00004260: 6e64 2069 6e73 7461 6e63 6520 7661 7269  nd instance vari
+00004270: 6162 6c65 7320 696e 2079 6f75 7220 6375  ables in your cu
+00004280: 7374 6f6d 2063 6c61 7373 2e5c 6e41 6464  stom class.\nAdd
+00004290: 6974 696f 6e61 6c6c 792c 2074 6865 7265  itionally, there
+000042a0: 2069 7320 6120 4074 6f6f 6c20 6465 636f   is a @tool deco
+000042b0: 7261 746f 7220 7072 6f76 6964 6564 2074  rator provided t
+000042c0: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+000042d0: 746f 2071 7569 636b 6c79 2063 7265 6174  to quickly creat
+000042e0: 6520 6120 546f 6f6c 2066 726f 6d20 6120  e a Tool from a 
+000042f0: 7369 6d70 6c65 2066 756e 6374 696f 6e2e  simple function.
+00004300: 2054 6865 2064 6563 6f72 6174 6f72 2075   The decorator u
+00004310: 7365 7320 7468 6520 6675 6e63 7469 6f6e  ses the function
+00004320: 206e 616d 6520 6173 2074 6865 2074 6f6f   name as the too
+00004330: 6c20 6e61 6d65 2062 7920 6465 6661 756c  l name by defaul
+00004340: 7420 616e 6420 7468 6520 6675 6e63 7469  t and the functi
+00004350: 6f6e 2773 2064 6f63 7374 7269 6e67 2061  on's docstring a
+00004360: 7320 7468 6520 746f 6f6c 2773 2064 6573  s the tool's des
+00004370: 6372 6970 7469 6f6e 2e22 2c0a 2020 2020  cription.",.    
+00004380: 2020 2020 2020 2020 2261 6e73 7765 725f          "answer_
+00004390: 7072 6f70 6572 7469 6573 223a 205b 5d2c  properties": [],
+000043a0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+000043b0: 7465 7322 3a20 7b0a 2020 2020 2020 2020  tes": {.        
+000043c0: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
+000043d0: 2022 6d69 6422 0a20 2020 2020 2020 2020   "mid".         
+000043e0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+000043f0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00004400: 2020 2020 2020 2269 6422 3a20 226c 616e        "id": "lan
+00004410: 6763 6861 696e 2d32 3122 2c0a 2020 2020  gchain-21",.    
+00004420: 2020 2020 2020 2020 2271 7565 7374 696f          "questio
+00004430: 6e22 3a20 2249 7320 7468 6572 6520 616e  n": "Is there an
+00004440: 2061 6765 6e74 2074 7970 6520 7468 6174   agent type that
+00004450: 2073 7570 706f 7274 7320 4f70 656e 4149   supports OpenAI
+00004460: 2773 2066 756e 6374 696f 6e20 6361 6c6c  's function call
+00004470: 696e 6720 696e 7465 7266 6163 653f 222c  ing interface?",
+00004480: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00004490: 6665 7265 6e63 655f 616e 7377 6572 223a  ference_answer":
+000044a0: 2022 5965 732c 2074 6865 7265 2069 7320   "Yes, there is 
+000044b0: 616e 2061 6765 6e74 2074 7970 6520 7468  an agent type th
+000044c0: 6174 2073 7570 706f 7274 7320 4f70 656e  at supports Open
+000044d0: 4149 2773 2066 756e 6374 696f 6e20 6361  AI's function ca
+000044e0: 6c6c 696e 6720 696e 7465 7266 6163 652e  lling interface.
+000044f0: 2049 7420 6973 2063 616c 6c65 6420 7468   It is called th
+00004500: 6520 4f70 656e 4149 2046 756e 6374 696f  e OpenAI Functio
+00004510: 6e73 2041 6765 6e74 2e20 5468 6973 2061  ns Agent. This a
+00004520: 6765 6e74 2069 7320 6465 7369 676e 6564  gent is designed
+00004530: 2074 6f20 776f 726b 2077 6974 6820 4f70   to work with Op
+00004540: 656e 4149 206d 6f64 656c 7320 7468 6174  enAI models that
+00004550: 2068 6176 6520 6265 656e 2066 696e 652d   have been fine-
+00004560: 7475 6e65 6420 746f 2064 6574 6563 7420  tuned to detect 
+00004570: 7768 656e 2061 2066 756e 6374 696f 6e20  when a function 
+00004580: 7368 6f75 6c64 2062 6520 6361 6c6c 6564  should be called
+00004590: 2061 6e64 2072 6573 706f 6e64 2077 6974   and respond wit
+000045a0: 6820 7468 6520 696e 7075 7473 2074 6861  h the inputs tha
+000045b0: 7420 7368 6f75 6c64 2062 6520 7061 7373  t should be pass
+000045c0: 6564 2074 6f20 7468 6520 6675 6e63 7469  ed to the functi
+000045d0: 6f6e 2e20 5468 6520 4f70 656e 4149 2046  on. The OpenAI F
+000045e0: 756e 6374 696f 6e73 2041 6765 6e74 2069  unctions Agent i
+000045f0: 7320 6361 7061 626c 6520 6f66 2072 6573  s capable of res
+00004600: 706f 6e64 696e 6720 746f 2070 726f 6d70  ponding to promp
+00004610: 7473 2066 726f 6d20 7468 6520 7573 6572  ts from the user
+00004620: 2075 7369 6e67 2061 204c 6172 6765 204c   using a Large L
+00004630: 616e 6775 6167 6520 4d6f 6465 6c2e 222c  anguage Model.",
+00004640: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
+00004650: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
+00004660: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+00004670: 2020 226e 6f74 6573 223a 207b 0a20 2020    "notes": {.   
+00004680: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
+00004690: 7665 6c22 3a20 226d 6964 220a 2020 2020  vel": "mid".    
+000046a0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000046b0: 2020 7d0a 2020 2020 5d0a 7d                }.    ].}
```

## chat/evaluation/qa/data/dataset/mock.json

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

```diff
@@ -1,55 +1,53 @@
-00000000: 7b0d 0a20 2020 2022 6e61 6d65 223a 2022  {..    "name": "
-00000010: 4d6f 636b 5365 7422 2c0d 0a20 2020 2022  MockSet",..    "
-00000020: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
-00000030: 2074 6573 7420 7365 7420 746f 2072 756e   test set to run
-00000040: 2074 6865 2077 6f72 6b66 6c6f 7722 2c0d   the workflow",.
-00000050: 0a20 2020 2022 6361 7365 7322 3a20 5b0d  .    "cases": [.
-00000060: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-00000070: 2020 2020 2020 2020 2269 6422 3a20 226d          "id": "m
-00000080: 6b2d 3122 2c0d 0a20 2020 2020 2020 2020  k-1",..         
-00000090: 2020 2022 7175 6573 7469 6f6e 223a 2022     "question": "
-000000a0: 4172 6520 726f 7365 7320 7265 643f 222c  Are roses red?",
-000000b0: 0d0a 2020 2020 2020 2020 2020 2020 2272  ..            "r
-000000c0: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
-000000d0: 3a20 2259 6573 2e22 2c0d 0a20 2020 2020  : "Yes.",..     
-000000e0: 2020 2020 2020 2022 616e 7377 6572 5f70         "answer_p
-000000f0: 726f 7065 7274 6965 7322 3a20 5b5d 2c0d  roperties": [],.
-00000100: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00000110: 7465 7322 3a20 7b0d 0a20 2020 2020 2020  tes": {..       
-00000120: 2020 2020 2020 2020 2022 6c65 7665 6c22           "level"
-00000130: 3a20 226d 6964 220d 0a20 2020 2020 2020  : "mid"..       
-00000140: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000150: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00000160: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00000170: 2022 6d6b 2d32 222c 0d0a 2020 2020 2020   "mk-2",..      
-00000180: 2020 2020 2020 2271 7565 7374 696f 6e22        "question"
-00000190: 3a20 2241 7265 2076 696f 6c65 7473 2079  : "Are violets y
-000001a0: 656c 6c6f 773f 222c 0d0a 2020 2020 2020  ellow?",..      
-000001b0: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
-000001c0: 5f61 6e73 7765 7222 3a20 224e 6f2e 222c  _answer": "No.",
-000001d0: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
-000001e0: 6e73 7765 725f 7072 6f70 6572 7469 6573  nswer_properties
-000001f0: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
-00000200: 2020 2020 226e 6f74 6573 223a 207b 0d0a      "notes": {..
-00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 226c 6576 656c 223a 2022 6c6f 7722 0d0a  "level": "low"..
-00000230: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00000240: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00000250: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00000260: 2020 2269 6422 3a20 226d 6b2d 3322 2c0d    "id": "mk-3",.
-00000270: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
-00000280: 6573 7469 6f6e 223a 2022 5768 6174 2069  estion": "What i
-00000290: 7320 7468 6520 6361 7069 7461 6c20 6f66  s the capital of
-000002a0: 2043 6869 6e61 3f22 2c0d 0a20 2020 2020   China?",..     
-000002b0: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
-000002c0: 655f 616e 7377 6572 223a 2022 4265 696a  e_answer": "Beij
-000002d0: 696e 6720 6973 2074 6865 2063 6170 6974  ing is the capit
-000002e0: 616c 206f 6620 4368 696e 612e 222c 0d0a  al of China.",..
-000002f0: 2020 2020 2020 2020 2020 2020 2261 6e73              "ans
-00000300: 7765 725f 7072 6f70 6572 7469 6573 223a  wer_properties":
-00000310: 205b 5d2c 0d0a 2020 2020 2020 2020 2020   [],..          
-00000320: 2020 226e 6f74 6573 223a 207b 0d0a 2020    "notes": {..  
-00000330: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00000340: 6576 656c 223a 2022 6c6f 7722 0d0a 2020  evel": "low"..  
-00000350: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00000360: 2020 2020 207d 0d0a 2020 2020 5d0d 0a7d       }..    ]..}
+00000000: 7b0a 2020 2020 226e 616d 6522 3a20 224d  {.    "name": "M
+00000010: 6f63 6b53 6574 222c 0a20 2020 2022 6465  ockSet",.    "de
+00000020: 7363 7269 7074 696f 6e22 3a20 2241 2074  scription": "A t
+00000030: 6573 7420 7365 7420 746f 2072 756e 2074  est set to run t
+00000040: 6865 2077 6f72 6b66 6c6f 7722 2c0a 2020  he workflow",.  
+00000050: 2020 2263 6173 6573 223a 205b 0a20 2020    "cases": [.   
+00000060: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000070: 2020 2022 6964 223a 2022 6d6b 2d31 222c     "id": "mk-1",
+00000080: 0a20 2020 2020 2020 2020 2020 2022 7175  .            "qu
+00000090: 6573 7469 6f6e 223a 2022 4172 6520 726f  estion": "Are ro
+000000a0: 7365 7320 7265 643f 222c 0a20 2020 2020  ses red?",.     
+000000b0: 2020 2020 2020 2022 7265 6665 7265 6e63         "referenc
+000000c0: 655f 616e 7377 6572 223a 2022 5965 732e  e_answer": "Yes.
+000000d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000000e0: 616e 7377 6572 5f70 726f 7065 7274 6965  answer_propertie
+000000f0: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+00000100: 2020 2020 226e 6f74 6573 223a 207b 0a20      "notes": {. 
+00000110: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000120: 6c65 7665 6c22 3a20 226d 6964 220a 2020  level": "mid".  
+00000130: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000140: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+00000150: 0a20 2020 2020 2020 2020 2020 2022 6964  .            "id
+00000160: 223a 2022 6d6b 2d32 222c 0a20 2020 2020  ": "mk-2",.     
+00000170: 2020 2020 2020 2022 7175 6573 7469 6f6e         "question
+00000180: 223a 2022 4172 6520 7669 6f6c 6574 7320  ": "Are violets 
+00000190: 7965 6c6c 6f77 3f22 2c0a 2020 2020 2020  yellow?",.      
+000001a0: 2020 2020 2020 2272 6566 6572 656e 6365        "reference
+000001b0: 5f61 6e73 7765 7222 3a20 224e 6f2e 222c  _answer": "No.",
+000001c0: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
+000001d0: 7377 6572 5f70 726f 7065 7274 6965 7322  swer_properties"
+000001e0: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+000001f0: 2020 226e 6f74 6573 223a 207b 0a20 2020    "notes": {.   
+00000200: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
+00000210: 7665 6c22 3a20 226c 6f77 220a 2020 2020  vel": "low".    
+00000220: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000230: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00000240: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+00000250: 2022 6d6b 2d33 222c 0a20 2020 2020 2020   "mk-3",.       
+00000260: 2020 2020 2022 7175 6573 7469 6f6e 223a       "question":
+00000270: 2022 5768 6174 2069 7320 7468 6520 6361   "What is the ca
+00000280: 7069 7461 6c20 6f66 2043 6869 6e61 3f22  pital of China?"
+00000290: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+000002a0: 6566 6572 656e 6365 5f61 6e73 7765 7222  eference_answer"
+000002b0: 3a20 2242 6569 6a69 6e67 2069 7320 7468  : "Beijing is th
+000002c0: 6520 6361 7069 7461 6c20 6f66 2043 6869  e capital of Chi
+000002d0: 6e61 2e22 2c0a 2020 2020 2020 2020 2020  na.",.          
+000002e0: 2020 2261 6e73 7765 725f 7072 6f70 6572    "answer_proper
+000002f0: 7469 6573 223a 205b 5d2c 0a20 2020 2020  ties": [],.     
+00000300: 2020 2020 2020 2022 6e6f 7465 7322 3a20         "notes": 
+00000310: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000320: 2020 226c 6576 656c 223a 2022 6c6f 7722    "level": "low"
+00000330: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00000340: 2020 2020 2020 207d 0a20 2020 205d 0a7d         }.    ].}
```

## chat/evaluation/qa/README.md

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-# Evaluation
-
-A auto evaluation workflow for question answering application.
-
-## `cli.py`
-
-A cli tool for evaluation related tasks.
-
-```console
-$ python chat/evaluation/cli.py --help
-Usage: cli.py [OPTIONS] COMMAND [ARGS]...
-
-  CLI to run evaluations.
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  evaluate  Run evaluations.
-  markdown  Generate a markdown report from the json report in JSON_PATH.
-  resume    Resume an evaluation from the json report in JSON_PATH.
-  show      Show available evaluators and evaluable subjects.
-```
+# Evaluation
+
+A auto evaluation workflow for question answering application.
+
+## `cli.py`
+
+A cli tool for evaluation related tasks.
+
+```console
+$ python chat/evaluation/cli.py --help
+Usage: cli.py [OPTIONS] COMMAND [ARGS]...
+
+  CLI to run evaluations.
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  evaluate  Run evaluations.
+  markdown  Generate a markdown report from the json report in JSON_PATH.
+  resume    Resume an evaluation from the json report in JSON_PATH.
+  show      Show available evaluators and evaluable subjects.
+```
```

## chat/evaluation/retrieval/data/code_search_net_eval/README.md

 * *Ordering differences only*

```diff
@@ -1,138 +1,138 @@
-# CodeSearchNet_eval.json
-
-This dataset contains human evaluation of code snippet retrieval.
-This is the dataset used to evaluate the performance of the CodeSearchNet Challenge winners with a few modifications.
-First, we removed the snippets that were not accessible from GitHub anymore. Snippets that were too long (mostly minified JS) were removed.
-Then we merged the multiples evaluations of the same query/snippet pair into a single average score.
-You can find the original dataset [here](https://raw.githubusercontent.com/github/CodeSearchNet/bb121a/resources/annotationStore.csv).
-
-This dataset contains 2822 query/snippet/score triple over 99 different queries.
-Each entry is scored on a scale from 0 (irrelevant) to 3 (perfectly relevant).
-
-## Results
-
-The precision, recall and F1 score figures given here are lower bounds because non-annotated query/snippet pairs are considered as irrelevant (relevance score 0) but might in fact be relevant.
-They are calculated from the top 5 retrieved documents.
-The times are measured on a M1 Max MacBook Pro.
-
-
-## Model: "hkunlp/instructor-base"
-
-Here are the results for different instructions.
-Strangely, the default generic instructions perform slightly better than the task-specific ones.
-With the default instructions, base, large and xl models have same precision, recall and F1 scores.
-Only the indexing and retrieval time per query are different, so the base model is the best choice for this dataset.
-
-### Default instructions:
-
-Instructions:
-- query: "Represent the question for retrieving supporting documents: "
-- document: "Represent the document for retrieval: "
-
-Results:
-- Precision: 0.57
-- Recall: 0.68
-- F1: 0.62
-- Indexing time per doc (ms): 100
-- Retrieval time per query (ms): 102
-
-
-### Custom instructions 1:
-
-Instructions:
-- query: "Represent the code search query for retrieving supporting pieces of code: "
-- document: "Represent the piece of code for code retrieval: "
-
-Results:
-- Precision: 0.55
-- Recall: 0.65
-- F1: 0.59
-- Indexing time per doc (ms): 94
-- Retrieval time per query (ms): 63
-
-
-### Custom instructions 2:
-
-Instructions:
-- query: "Represent the query for retrieving supporting source code: "
-- document: "Represent the source code for retrieval: "
-
-Results:
-- Precision: 0.56
-- Recall: 0.67
-- F1: 0.61
-- Indexing time per doc (ms): 94
-- Retrieval time per query (ms): 73
-
-
-## Model: "hkunlp/instructor-large"
-
-### Default instructions:
-
-Instructions:
-- query: "Represent the question for retrieving supporting documents: "
-- document: "Represent the document for retrieval: "
-
-Results:
-- Precision: 0.57
-- Recall: 0.68
-- F1: 0.62
-- Indexing time per doc (ms): 285
-- Retrieval time per query (ms): 150
-
-
-## Model: "hkunlp/instructor-xl"
-
-Options:
-- embed_instruction="Represent this piece of code for retrieval: ",
-- query_instruction="Represent the coding question for retrieving supporting pieces of code: "
-
-Results:
-- Precision: 0.57
-- Recall: 0.68
-- F1: 0.62
-- Indexing time per doc (ms): 940
-- Retrieval time per query (ms): 402
-
-
-## Model: "sentence-transformers/all-mpnet-base-v2"
-
-Results:
-- Precision: 0.58
-- Recall: 0.69
-- F1: 0.63
-- Indexing time per doc (ms): 103
-- Retrieval time per query (ms): 150
-
-
-## Model: "text-embedding-ada-002"
-- Precision: 0.48
-- Recall: 0.57
-- F1: 0.52
-- Indexing time per doc (ms): 137
-- Retrieval time per query (ms): 281
-
-
-## Model: "intfloat/e5-large-v2"
-
-Results:
-- Precision: 0.57
-- Recall: 0.67
-- F1: 0.62
-- Indexing time per doc (ms): 337
-- Retrieval time per query (ms): 288
-
-# Summary
-
-| Model                                   | Precision | Recall | F1 score | Indexing time per doc (ms) | Retrieval time per query (ms) |
-| --------------------------------------- | --------- | ------ | -------- | -------------------------- | ----------------------------- |
-| sentence-transformers/all-mpnet-base-v2 |      0.58 |   0.69 |     0.63 |                        103 |                           150 |
-| hkunlp/instructor-base                  |      0.57 |   0.68 |     0.62 |                        100 |                           102 |
-| hkunlp/instructor-large                 |      0.57 |   0.68 |     0.62 |                        285 |                           150 |
-| hkunlp/instructor-xl                    |      0.57 |   0.68 |     0.62 |                        940 |                           402 |
-| intfloat/e5-large-v2                    |      0.57 |   0.67 |     0.62 |                        337 |                           288 |
-| text-embedding-ada-002                  |      0.48 |   0.57 |     0.52 |                        137 |                           281 |
-
-
-The first thing to notice is that, apart from the text-embedding-ada-002 model, which performs significantly worse than the others, all models have similar precision, recall and F1 scores.
-The sentence-transformers/all-mpnet-base-v2 model has the best precision, recall and F1 scores, but the hkunlp/instructor-base model is slightly faster to retrieve.
+# CodeSearchNet_eval.json
+
+This dataset contains human evaluation of code snippet retrieval.
+This is the dataset used to evaluate the performance of the CodeSearchNet Challenge winners with a few modifications.
+First, we removed the snippets that were not accessible from GitHub anymore. Snippets that were too long (mostly minified JS) were removed.
+Then we merged the multiples evaluations of the same query/snippet pair into a single average score.
+You can find the original dataset [here](https://raw.githubusercontent.com/github/CodeSearchNet/bb121a/resources/annotationStore.csv).
+
+This dataset contains 2822 query/snippet/score triple over 99 different queries.
+Each entry is scored on a scale from 0 (irrelevant) to 3 (perfectly relevant).
+
+## Results
+
+The precision, recall and F1 score figures given here are lower bounds because non-annotated query/snippet pairs are considered as irrelevant (relevance score 0) but might in fact be relevant.
+They are calculated from the top 5 retrieved documents.
+The times are measured on a M1 Max MacBook Pro.
+
+
+## Model: "hkunlp/instructor-base"
+
+Here are the results for different instructions.
+Strangely, the default generic instructions perform slightly better than the task-specific ones.
+With the default instructions, base, large and xl models have same precision, recall and F1 scores.
+Only the indexing and retrieval time per query are different, so the base model is the best choice for this dataset.
+
+### Default instructions:
+
+Instructions:
+- query: "Represent the question for retrieving supporting documents: "
+- document: "Represent the document for retrieval: "
+
+Results:
+- Precision: 0.57
+- Recall: 0.68
+- F1: 0.62
+- Indexing time per doc (ms): 100
+- Retrieval time per query (ms): 102
+
+
+### Custom instructions 1:
+
+Instructions:
+- query: "Represent the code search query for retrieving supporting pieces of code: "
+- document: "Represent the piece of code for code retrieval: "
+
+Results:
+- Precision: 0.55
+- Recall: 0.65
+- F1: 0.59
+- Indexing time per doc (ms): 94
+- Retrieval time per query (ms): 63
+
+
+### Custom instructions 2:
+
+Instructions:
+- query: "Represent the query for retrieving supporting source code: "
+- document: "Represent the source code for retrieval: "
+
+Results:
+- Precision: 0.56
+- Recall: 0.67
+- F1: 0.61
+- Indexing time per doc (ms): 94
+- Retrieval time per query (ms): 73
+
+
+## Model: "hkunlp/instructor-large"
+
+### Default instructions:
+
+Instructions:
+- query: "Represent the question for retrieving supporting documents: "
+- document: "Represent the document for retrieval: "
+
+Results:
+- Precision: 0.57
+- Recall: 0.68
+- F1: 0.62
+- Indexing time per doc (ms): 285
+- Retrieval time per query (ms): 150
+
+
+## Model: "hkunlp/instructor-xl"
+
+Options:
+- embed_instruction="Represent this piece of code for retrieval: ",
+- query_instruction="Represent the coding question for retrieving supporting pieces of code: "
+
+Results:
+- Precision: 0.57
+- Recall: 0.68
+- F1: 0.62
+- Indexing time per doc (ms): 940
+- Retrieval time per query (ms): 402
+
+
+## Model: "sentence-transformers/all-mpnet-base-v2"
+
+Results:
+- Precision: 0.58
+- Recall: 0.69
+- F1: 0.63
+- Indexing time per doc (ms): 103
+- Retrieval time per query (ms): 150
+
+
+## Model: "text-embedding-ada-002"
+- Precision: 0.48
+- Recall: 0.57
+- F1: 0.52
+- Indexing time per doc (ms): 137
+- Retrieval time per query (ms): 281
+
+
+## Model: "intfloat/e5-large-v2"
+
+Results:
+- Precision: 0.57
+- Recall: 0.67
+- F1: 0.62
+- Indexing time per doc (ms): 337
+- Retrieval time per query (ms): 288
+
+# Summary
+
+| Model                                   | Precision | Recall | F1 score | Indexing time per doc (ms) | Retrieval time per query (ms) |
+| --------------------------------------- | --------- | ------ | -------- | -------------------------- | ----------------------------- |
+| sentence-transformers/all-mpnet-base-v2 |      0.58 |   0.69 |     0.63 |                        103 |                           150 |
+| hkunlp/instructor-base                  |      0.57 |   0.68 |     0.62 |                        100 |                           102 |
+| hkunlp/instructor-large                 |      0.57 |   0.68 |     0.62 |                        285 |                           150 |
+| hkunlp/instructor-xl                    |      0.57 |   0.68 |     0.62 |                        940 |                           402 |
+| intfloat/e5-large-v2                    |      0.57 |   0.67 |     0.62 |                        337 |                           288 |
+| text-embedding-ada-002                  |      0.48 |   0.57 |     0.52 |                        137 |                           281 |
+
+
+The first thing to notice is that, apart from the text-embedding-ada-002 model, which performs significantly worse than the others, all models have similar precision, recall and F1 scores.
+The sentence-transformers/all-mpnet-base-v2 model has the best precision, recall and F1 scores, but the hkunlp/instructor-base model is slightly faster to retrieve.
```

## chat/README.md

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-# DevChat
-
+# DevChat
+
 Ask everything about your dev data beyond the code.
```

## Comparing `devchat_ask-0.0.7.dist-info/METADATA` & `devchat_ask-0.0.8.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat-ask
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: Hezheng Yin
 Author-email: hezheng@merico.dev
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: instructorembedding (>=1.0.1,<2.0.0)
```

