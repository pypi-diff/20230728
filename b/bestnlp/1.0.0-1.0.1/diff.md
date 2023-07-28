# Comparing `tmp/bestnlp-1.0.0-py3-none-any.whl.zip` & `tmp/bestnlp-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3806 bytes, number of entries: 6
+Zip file size: 3511 bytes, number of entries: 6
 -rw-r--r--  2.0 unx      113 b- defN 23-Jul-21 08:28 bestnlp/__init__.py
--rw-r--r--  2.0 unx     8916 b- defN 23-Jul-21 08:23 bestnlp/new_word_discovery.py
--rw-r--r--  2.0 unx      213 b- defN 23-Jul-21 08:30 bestnlp-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 08:30 bestnlp-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-21 08:30 bestnlp-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      457 b- defN 23-Jul-21 08:30 bestnlp-1.0.0.dist-info/RECORD
-6 files, 9799 bytes uncompressed, 2976 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     7561 b- defN 23-Jul-28 09:00 bestnlp/new_word_discovery.py
+-rw-r--r--  2.0 unx      213 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      457 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/RECORD
+6 files, 8444 bytes uncompressed, 2681 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: bestnlp/__init__.py
 Comment: 
 
 Filename: bestnlp/new_word_discovery.py
 Comment: 
 
-Filename: bestnlp-1.0.0.dist-info/METADATA
+Filename: bestnlp-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: bestnlp-1.0.0.dist-info/WHEEL
+Filename: bestnlp-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: bestnlp-1.0.0.dist-info/top_level.txt
+Filename: bestnlp-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bestnlp-1.0.0.dist-info/RECORD
+Filename: bestnlp-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestnlp/new_word_discovery.py

```diff
@@ -1,29 +1,27 @@
 import random
 import math
-from collections import Counter
 import pandas as pd
 import jieba.posseg as jieba
 import re
 import os
 
 _get_module_path = lambda path: os.path.normpath(os.path.join(os.getcwd(),
                                                  os.path.dirname(__file__), path))
 
 
-
 class NewWordDiscovery():
 
     def __init__(self):
         self.jieba_dict = self._read_jieba_dict()
 
 
-    def _read_jieba_dict(self, filename=_get_module_path("dict.txt")):
+    def _read_jieba_dict(self):
         di = dict()
-        with open(filename, "r") as f:
+        with open(_get_module_path("dict.txt"), "r") as f:
             for line in f:
                 temp = line.strip().split()
                 word, freq = temp[0], int(temp[1])
                 di[word] = freq
         return di
 
 
@@ -85,16 +83,14 @@
                     if word not in freq_di:
                         freq_di[word] = {"freq": 0, "left": dict(), "right": dict(), "pos": []}
                     freq_di[word]["freq"] += 1
                     left_tmp = words[i - 1] if i - 1 >= 0 else ""
                     freq_di[word]["left"][left_tmp] = freq_di[word]["left"].get(left_tmp, 0) + 1
                     right_tmp = words[i + j] if i + j < l else ""
                     freq_di[word]["right"][right_tmp] = freq_di[word]["right"].get(right_tmp, 0) + 1
-                    #freq_di[word]["left"].append(words[i - 1] if i - 1 >= 0 else "")
-                    #freq_di[word]["right"].append(words[i + j] if i + j < l else "")
                     freq_di[word]["pos"] = flags[i: i + j]
             idf_list.append(sentence_set)
         idf_di = self.calculate_idf(idf_list)
         return freq_di, word_num, idf_di
 
 
     def ami(self, freq_di, word_num, threshold=0, percent=10):
@@ -107,15 +103,14 @@
                 val = math.log2(val)
                 #val *= freq_di[word]["freq"]/word_num/len(word)
                 val /= len(word)
                 if val > threshold:
                     di[word] = val
         di = sorted(di.items(), key=lambda x: x[1], reverse=True)
         di = di[:int(len(freq_di) * percent / 100)]
-        #print(di[0][1], di[-1][1])
         di = {key: value for key, value in di}
         return di
 
 
     def structure(self, freq_di, threshold=1.9):
         di = dict()
         for word in freq_di:
@@ -133,57 +128,43 @@
                     val *= 0.1
 
                 if val > threshold:
                     di[word] = val
         return di
 
 
-
-
-
     def entropy(self, di):
        num = sum(di.values())
        res = 0
        for word, freq in di.items():
            if word == "":
-               #res -= (1/num * math.log2(1/num)) * math.sqrt(freq)
-               #res -= 1/num * math.log2(1/num)
                res -= freq/num * math.log2(freq/num)
            else:
                res -= freq/num * math.log2(freq/num)
-           #res -= freq / num * math.log2(freq / num)
-       if res < 0:
-           print("res < 0", res, di)
        return res
 
 
 
 
     def L_entropy(self, freq_di, threshold=0, percent=10):
         di = dict()
         for word in freq_di:
             if len(word) > 1:
                 l_e = self.entropy(freq_di[word]["left"])
                 r_e = self.entropy(freq_di[word]["right"])
-                #final_entropy = math.log((l_e * 2 ** r_e + r_e * 2 ** l_e + 0.00001) / (abs(l_e - r_e) + 1), 1.5)
-                #final_entropy = (min(r_e, l_e) ** 2) * (math.sqrt(max(r_e, l_e)))
-                #final_entropy = min(l_e, r_e) * math.sqrt(max(l_e, r_e))
                 final_entropy = min(l_e, r_e) * math.log(max(l_e, r_e) + math.e, math.e)
                 if final_entropy > threshold:
-                    #di[word] = final_entropy
                     di[word] = [final_entropy, l_e, r_e]
-        #di = sorted(di.items(), key=lambda x: x[1], reverse=True)
         di = sorted(di.items(), key=lambda x: x[1][0], reverse=True)
         di = di[:int(len(freq_di) * percent / 100)]
         di = {key: value for key, value in di}
         return di
 
 
-
-    def extract_keyword(self, filename, k_min=2, k_max=5, mode="word", min_freq=5, entropy_percent=15, ami_percent=15, write_mode=True, write_name="details.csv"):
+    def extract_keyword(self, filename, k_min=2, k_max=5, mode="word", min_freq=5, entropy_percent=20, ami_percent=20, write_mode=True, write_name="details.csv"):
         sentences = self.read_txt(filename)
         write_df = {"word":[], "ami":[], "entropy":[], "l_e":[], "r_e":[], "pos":[], "freq":[], "idf":[], "score":[]}
         freq_di, word_num, idf_di = self.calculate_frequency(sentences, k_min, k_max, mode)
         entropy_di = self.L_entropy(freq_di, percent=entropy_percent)
         print(len(entropy_di))
         ami_di = self.ami(freq_di, word_num, percent=ami_percent)
         print(len(ami_di))
@@ -191,41 +172,32 @@
         filter_words = self.get_filter_word(freq_di)
         final_di = dict()
         for name in entropy_di:
             complete_name = "".join(name)
             if (complete_name not in filter_words) and (name in ami_di) and (name in structure_di) and (freq_di[name]["freq"] >= min_freq):
                 idf = [idf_di[w] for w in name]
                 idf = sum(idf)/len(idf)
-                #final_di[name] = (math.sqrt(entropy_di[name]) + 5 * ami_di[name]) * structure_di[name] * math.sqrt(freq_di[name]["freq"]) * idf
                 final_di[name] = entropy_di[name][0] * ami_di[name] * structure_di[name] * idf * math.sqrt(freq_di[name]["freq"])
                 write_df["word"].append(complete_name)
                 write_df["ami"].append(ami_di[name])
                 write_df["entropy"].append(entropy_di[name][0])
                 write_df["l_e"].append(entropy_di[name][1])
                 write_df["r_e"].append(entropy_di[name][2])
                 write_df["pos"].append("_".join(freq_di[name]["pos"]))
                 write_df["freq"].append(freq_di[name]["freq"])
                 write_df["idf"].append(idf)
                 write_df["score"].append(final_di[name])
-        #final_di = sorted(final_di.items(), key=lambda x: x[1], reverse=True)
-        #final_list = ["".join(elem[0]) for elem in final_di]
         if write_mode:
             pd.DataFrame.from_dict(write_df).to_csv(write_name)
 
 
 
 
-
-
-# sentences = utils.read_txt("三体.txt")
 # nwd = NewWordDiscovery()
 # nwd.extract_keyword("三体.txt", k_min=2, k_max=7, mode="char", min_freq=7, entropy_percent=20, ami_percent=20, write_name="char.csv", write_mode=True)
-#extract_keyword(sentences, k_min=2, k_max=5, mode="word", min_freq=7, entropy_percent=20, ami_percent=20, write_name="word.csv", write_mode=True)
-
-
```

