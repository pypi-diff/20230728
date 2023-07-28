# Comparing `tmp/transliter-0.3.6.tar.gz` & `tmp/transliter-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transliter-0.3.6.tar", last modified: Sun May 21 00:37:07 2023, max compression
+gzip compressed data, was "transliter-0.3.7.tar", last modified: Fri Jul 28 02:01:38 2023, max compression
```

## Comparing `transliter-0.3.6.tar` & `transliter-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-21 00:37:07.374472 transliter-0.3.6/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)    18092 2023-05-18 01:15:40.000000 transliter-0.3.6/LICENSE
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     7222 2023-05-21 00:37:07.374353 transliter-0.3.6/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     6883 2023-05-18 01:58:43.000000 transliter-0.3.6/README.md
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-05-21 00:37:07.374511 transliter-0.3.6/setup.cfg
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      656 2023-05-20 12:35:08.000000 transliter-0.3.6/setup.py
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-21 00:37:07.373449 transliter-0.3.6/transliter/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      155 2023-05-18 01:07:44.000000 transliter-0.3.6/transliter/__init__.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     6334 2023-05-21 00:08:23.000000 transliter-0.3.6/transliter/cyrillic_list.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     3414 2023-05-21 00:16:16.000000 transliter-0.3.6/transliter/jp_list.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1832 2023-05-13 04:20:03.000000 transliter-0.3.6/transliter/ko_jamo.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      370 2023-05-13 04:20:03.000000 transliter-0.3.6/transliter/spacing.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)    11042 2023-05-20 22:07:40.000000 transliter-0.3.6/transliter/transliter_cyrillic.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1920 2023-05-21 00:16:11.000000 transliter-0.3.6/transliter/transliter_jp.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     2990 2023-05-18 01:07:27.000000 transliter-0.3.6/transliter/transliter_ko.py
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-05-21 00:37:07.374138 transliter-0.3.6/transliter.egg-info/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     7222 2023-05-21 00:37:07.000000 transliter-0.3.6/transliter.egg-info/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      435 2023-05-21 00:37:07.000000 transliter-0.3.6/transliter.egg-info/SOURCES.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-05-21 00:37:07.000000 transliter-0.3.6/transliter.egg-info/dependency_links.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-05-21 00:37:07.000000 transliter-0.3.6/transliter.egg-info/not-zip-safe
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-05-21 00:37:07.000000 transliter-0.3.6/transliter.egg-info/requires.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-05-21 00:37:07.000000 transliter-0.3.6/transliter.egg-info/top_level.txt
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-07-28 02:01:38.249341 transliter-0.3.7/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)    18092 2023-05-18 01:15:40.000000 transliter-0.3.7/LICENSE
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     7183 2023-07-28 02:01:38.249219 transliter-0.3.7/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     6844 2023-07-28 01:51:47.000000 transliter-0.3.7/README.md
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-07-28 02:01:38.249382 transliter-0.3.7/setup.cfg
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      656 2023-07-28 01:53:07.000000 transliter-0.3.7/setup.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-07-28 02:01:38.248320 transliter-0.3.7/transliter/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      155 2023-05-18 01:07:44.000000 transliter-0.3.7/transliter/__init__.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     6334 2023-05-21 00:08:23.000000 transliter-0.3.7/transliter/cyrillic_list.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3414 2023-05-21 00:16:16.000000 transliter-0.3.7/transliter/jp_list.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1832 2023-05-13 04:20:03.000000 transliter-0.3.7/transliter/ko_jamo.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      426 2023-07-28 01:52:34.000000 transliter-0.3.7/transliter/spacing.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)    11852 2023-07-28 01:47:32.000000 transliter-0.3.7/transliter/transliter_cyrillic.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     2030 2023-07-28 01:42:38.000000 transliter-0.3.7/transliter/transliter_jp.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3100 2023-07-28 01:42:06.000000 transliter-0.3.7/transliter/transliter_ko.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-07-28 02:01:38.249041 transliter-0.3.7/transliter.egg-info/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     7183 2023-07-28 02:01:38.000000 transliter-0.3.7/transliter.egg-info/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      435 2023-07-28 02:01:38.000000 transliter-0.3.7/transliter.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-07-28 02:01:38.000000 transliter-0.3.7/transliter.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-07-28 02:01:38.000000 transliter-0.3.7/transliter.egg-info/not-zip-safe
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-07-28 02:01:38.000000 transliter-0.3.7/transliter.egg-info/requires.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-07-28 02:01:38.000000 transliter-0.3.7/transliter.egg-info/top_level.txt
```

### Comparing `transliter-0.3.6/LICENSE` & `transliter-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `transliter-0.3.6/PKG-INFO` & `transliter-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transliter
-Version: 0.3.6
+Version: 0.3.7
 Summary: TransLiter transliterates multilingual text into Latin script.
 Home-page: https://github.com/elibooklover/Transliter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: GPL-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -63,15 +63,15 @@
 urinara manse!
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 1-2. File Export (txt -> txt)
 
-The output is saved as `output_ko.txt` in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 > tl.txt_ko("test_ko.txt")
 안녕하세요.
 annyeonghaseyo.
 오늘 날씨 좋네요!
 oneul nalssi jotneyo!
@@ -82,15 +82,15 @@
 하루하루 재미있게 살아요.
 haruharu jaemiitge salayo.
 가족들과 저녁을 먹어요.gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ### 1-3. File Export (txt -> csv)
 
-The output is saved as `output_ko.csv` in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 > tl.csv_ko("test_ko.txt")
     Original Text                 Transliterated Text
 0          안녕하세요.                     annyeonghaseyo.
 1      오늘 날씨 좋네요!               oneul nalssi jotneyo!
 2     행복한 하루 되세요.           haengbokhan haru doeseyo.
@@ -123,15 +123,15 @@
 mainichiundouwoshimasu。
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 2-2. File Export (txt -> txt)
 
-The output is saved as `output_jp.txt` in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 > tl.txt_jp("test_jp.txt")
 気を付けて。
 kiwotsukete。
 良いニュースです。
 yoinyuーsudesu。
@@ -142,15 +142,15 @@
 気をつけてください。
 kiwotsuketekudasai。
 それはいい考えですね。sorehaiikangaedesune。
 ```
 
 ### 2-3. File Export (txt -> csv)
 
-The output is saved as `output_jp.csv` in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 > tl.csv_jp("test_jp.txt")
   Original Text    Transliterated Text
 0        気を付けて。           kiwotsukete。
 1     良いニュースです。         yoinyuーsudesu。
 2      おやすみなさい。          oyasuminasai。
@@ -164,15 +164,15 @@
 Some languages such as Japanese don't have spacing between words. If there is spacing between the characters or words for text in those languages, you might bump into errors. To avoid the errors, the spacing needs to be removed.
 
 ```
 > tl.spacing("良 い ニ ュ ー ス で す。")
 良いニュースです。
 ```
 
-If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `spacing_removed.txt`.
+If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `filename_rmspace.txt`.
 
 ```
 > tl.spacing_file("test.txt")
 ```
 
 ## 4. Cyrillic
 
@@ -212,15 +212,15 @@
 Dobro jutro
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 4-2. File Export (txt -> txt)
 
-The output is saved as `output_ru.txt` (Russian) / `output_sr.txt` (Serbian) in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 # Russian
 > tl.txt_ru("test_ru.txt")
 Доброе утро.
 Dobroe utro.
 Меня зовут Мандли.
@@ -240,15 +240,15 @@
 Не разумем
 Ne razumem
 Извините!Izvinite!
 ```
 
 ### 4-3. File Export (txt -> csv)
 
-The output is saved as `output_ru.csv` (Russian) / `output_sr.csv` (Serbian) in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 # Russian
 > tl.csv_ru("test_ru.txt")
                 Original Text          Transliterated Text
 0                Доброе утро.                 Dobroe utro.
 1          Меня зовут Мандли.          Menya zovut Mandli.
```

### Comparing `transliter-0.3.6/README.md` & `transliter-0.3.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 urinara manse!
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 1-2. File Export (txt -> txt)
 
-The output is saved as `output_ko.txt` in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 > tl.txt_ko("test_ko.txt")
 안녕하세요.
 annyeonghaseyo.
 오늘 날씨 좋네요!
 oneul nalssi jotneyo!
@@ -70,15 +70,15 @@
 하루하루 재미있게 살아요.
 haruharu jaemiitge salayo.
 가족들과 저녁을 먹어요.gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ### 1-3. File Export (txt -> csv)
 
-The output is saved as `output_ko.csv` in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 > tl.csv_ko("test_ko.txt")
     Original Text                 Transliterated Text
 0          안녕하세요.                     annyeonghaseyo.
 1      오늘 날씨 좋네요!               oneul nalssi jotneyo!
 2     행복한 하루 되세요.           haengbokhan haru doeseyo.
@@ -111,15 +111,15 @@
 mainichiundouwoshimasu。
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 2-2. File Export (txt -> txt)
 
-The output is saved as `output_jp.txt` in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 > tl.txt_jp("test_jp.txt")
 気を付けて。
 kiwotsukete。
 良いニュースです。
 yoinyuーsudesu。
@@ -130,15 +130,15 @@
 気をつけてください。
 kiwotsuketekudasai。
 それはいい考えですね。sorehaiikangaedesune。
 ```
 
 ### 2-3. File Export (txt -> csv)
 
-The output is saved as `output_jp.csv` in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 > tl.csv_jp("test_jp.txt")
   Original Text    Transliterated Text
 0        気を付けて。           kiwotsukete。
 1     良いニュースです。         yoinyuーsudesu。
 2      おやすみなさい。          oyasuminasai。
@@ -152,15 +152,15 @@
 Some languages such as Japanese don't have spacing between words. If there is spacing between the characters or words for text in those languages, you might bump into errors. To avoid the errors, the spacing needs to be removed.
 
 ```
 > tl.spacing("良 い ニ ュ ー ス で す。")
 良いニュースです。
 ```
 
-If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `spacing_removed.txt`.
+If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `filename_rmspace.txt`.
 
 ```
 > tl.spacing_file("test.txt")
 ```
 
 ## 4. Cyrillic
 
@@ -200,15 +200,15 @@
 Dobro jutro
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 4-2. File Export (txt -> txt)
 
-The output is saved as `output_ru.txt` (Russian) / `output_sr.txt` (Serbian) in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 # Russian
 > tl.txt_ru("test_ru.txt")
 Доброе утро.
 Dobroe utro.
 Меня зовут Мандли.
@@ -228,15 +228,15 @@
 Не разумем
 Ne razumem
 Извините!Izvinite!
 ```
 
 ### 4-3. File Export (txt -> csv)
 
-The output is saved as `output_ru.csv` (Russian) / `output_sr.csv` (Serbian) in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 # Russian
 > tl.csv_ru("test_ru.txt")
                 Original Text          Transliterated Text
 0                Доброе утро.                 Dobroe utro.
 1          Меня зовут Мандли.          Menya zovut Mandli.
```

### Comparing `transliter-0.3.6/setup.py` & `transliter-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='transliter',
     python_requires='>=3.6',
-    version='0.3.6',
+    version='0.3.7',
     url='https://github.com/elibooklover/Transliter',
     license='GPL-2.0',
     author='Hoyeol Kim',
     author_email='elibooklover@gmail.com',
     description='TransLiter transliterates multilingual text into Latin script.',
     packages=['transliter', ],
     long_description=long_description,
```

### Comparing `transliter-0.3.6/transliter/cyrillic_list.py` & `transliter-0.3.7/transliter/cyrillic_list.py`

 * *Files identical despite different names*

### Comparing `transliter-0.3.6/transliter/jp_list.py` & `transliter-0.3.7/transliter/jp_list.py`

 * *Files identical despite different names*

### Comparing `transliter-0.3.6/transliter/ko_jamo.py` & `transliter-0.3.7/transliter/ko_jamo.py`

 * *Files identical despite different names*

### Comparing `transliter-0.3.6/transliter/transliter_cyrillic.py` & `transliter-0.3.7/transliter/transliter_cyrillic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from transliter.cyrillic_list import *
 import pandas as pd
+import os
 
 # Russian
 def ru(text):
     transliterated_text = ""
     for letter in text:
         try: 
             if letter in RUSSIAN_LIST:
@@ -19,42 +20,44 @@
         input_text = input("Please enter Russian text: ")
         print(ru(input_text))
         if input_text == "": 
             break
 
 def txt_ru(file):
     f = open(file, 'r')
-    f2 = open("output_ru.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + ru(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_ru(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = ru(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_ru.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Ukrainian
 def ua(text):
     transliterated_text = ""
     for letter in text:
@@ -72,42 +75,44 @@
         input_text = input("Please enter Ukrainian text: ")
         print(ua(input_text))
         if input_text == "": 
             break
 
 def txt_ua(file):
     f = open(file, 'r')
-    f2 = open("output_ua.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + ua(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_ua(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = ua(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_ua.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Bulgarian
 def bg(text):
     transliterated_text = ""
     for letter in text:
@@ -125,42 +130,44 @@
         input_text = input("Please enter Bulgarian text: ")
         print(bg(input_text))
         if input_text == "": 
             break
 
 def txt_bg(file):
     f = open(file, 'r')
-    f2 = open("output_bg.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + bg(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_bg(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = bg(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_bg.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Macedonian
 def mk(text):
     transliterated_text = ""
     for letter in text:
@@ -178,42 +185,44 @@
         input_text = input("Please enter Macedonian text: ")
         print(mk(input_text))
         if input_text == "": 
             break
 
 def txt_mk(file):
     f = open(file, 'r')
-    f2 = open("output_mk.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + mk(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_mk(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = mk(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_mk.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Mongolian
 def mn(text):
     transliterated_text = ""
     for letter in text:
@@ -231,42 +240,44 @@
         input_text = input("Please enter Mongolian text: ")
         print(me(input_text))
         if input_text == "": 
             break
 
 def txt_mn(file):
     f = open(file, 'r')
-    f2 = open("output_mn.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + mn(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_mn(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = mn(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_mn.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 
 # Montenegrin
 def me(text):
     transliterated_text = ""
@@ -285,42 +296,44 @@
         input_text = input("Please enter Montenegrin text: ")
         print(me(input_text))
         if input_text == "": 
             break
 
 def txt_me(file):
     f = open(file, 'r')
-    f2 = open("output_me.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + me(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_me(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = me(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_me.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Serbian
 def sr(text):
     transliterated_text = ""
     for letter in text:
@@ -338,42 +351,44 @@
         input_text = input("Please enter Serbian text: ")
         print(sr(input_text))
         if input_text == "": 
             break
 
 def txt_sr(file):
     f = open(file, 'r')
-    f2 = open("output_sr.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + sr(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_sr(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = sr(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_sr.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
 
 # Tajiki
 def tj(text):
     transliterated_text = ""
     for letter in text:
@@ -391,37 +406,39 @@
         input_text = input("Please enter Tajiki text: ")
         print(tj(input_text))
         if input_text == "": 
             break
 
 def txt_tj(file):
     f = open(file, 'r')
-    f2 = open("output_tj.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + tj(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_tj(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = tj(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_tj.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
```

### Comparing `transliter-0.3.6/transliter/transliter_jp.py` & `transliter-0.3.7/transliter/transliter_jp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from transliter.jp_list import *
 import pykakasi
 import pandas as pd
+import os
 
 def kanji_to_hiragana(text):
     kks = pykakasi.kakasi()
     hiragana_text = ''
     for result in kks.convert(text):
         if result['hira']:
             hiragana_text += result['hira']
@@ -34,37 +35,39 @@
         input_text = input("Please enter Japanese text: ")
         print(jp(input_text))
         if input_text == "": 
             break
 
 def txt_jp(file):
     f = open(file, 'r')
-    f2 = open("output_jp.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + jp(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_jp(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = jp(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_jp.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
```

### Comparing `transliter-0.3.6/transliter/transliter_ko.py` & `transliter-0.3.7/transliter/transliter_ko.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from transliter.ko_jamo import *
 import re
 import pandas as pd
+import os
 
 def convert(Ko_words):
     split_word_list = list(Ko_words)
     jamo_result = []
     for keyword in split_word_list:
         if re.match('.*[가-힣]+.*', keyword) is not None:
             char_code = ord(keyword) - BASE_CODE
@@ -53,37 +54,39 @@
         input_text = input("Please enter Korean text: ")
         print(ko(input_text))
         if input_text == "": 
             break
 
 def txt_ko(file):
     f = open(file, 'r')
-    f2 = open("output_ko.txt", 'w')
+    new_file = os.path.splitext(file)[0]
+    f2 = open(f"{new_file}_output.txt", 'w')
     result = ""
     while True:
         line = f.readline()
         result += line + ko(line)
         if not line: 
             break
     print(result)
     f2.write(result)
     f.close()
     f2.close()
 
 def csv_ko(file):
     data = pd.DataFrame(columns=['Original Text', 'Transliterated Text'])
     f = open(file, 'r')
+    new_file = os.path.splitext(file)[0]
     lines = f.readlines()
     
     index_list = list(range(len(lines)))
     sentence_list = []
     transliter_list = []
     for sentence in lines:
         st = sentence.strip()
         tr = ko(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_ko.csv", encoding="utf-8-sig")
+    data.to_csv(f"{new_file}_output.csv", encoding="utf-8-sig")
     print(data)
     f.close()
```

### Comparing `transliter-0.3.6/transliter.egg-info/PKG-INFO` & `transliter-0.3.7/transliter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transliter
-Version: 0.3.6
+Version: 0.3.7
 Summary: TransLiter transliterates multilingual text into Latin script.
 Home-page: https://github.com/elibooklover/Transliter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: GPL-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -63,15 +63,15 @@
 urinara manse!
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 1-2. File Export (txt -> txt)
 
-The output is saved as `output_ko.txt` in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 > tl.txt_ko("test_ko.txt")
 안녕하세요.
 annyeonghaseyo.
 오늘 날씨 좋네요!
 oneul nalssi jotneyo!
@@ -82,15 +82,15 @@
 하루하루 재미있게 살아요.
 haruharu jaemiitge salayo.
 가족들과 저녁을 먹어요.gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ### 1-3. File Export (txt -> csv)
 
-The output is saved as `output_ko.csv` in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 > tl.csv_ko("test_ko.txt")
     Original Text                 Transliterated Text
 0          안녕하세요.                     annyeonghaseyo.
 1      오늘 날씨 좋네요!               oneul nalssi jotneyo!
 2     행복한 하루 되세요.           haengbokhan haru doeseyo.
@@ -123,15 +123,15 @@
 mainichiundouwoshimasu。
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 2-2. File Export (txt -> txt)
 
-The output is saved as `output_jp.txt` in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 > tl.txt_jp("test_jp.txt")
 気を付けて。
 kiwotsukete。
 良いニュースです。
 yoinyuーsudesu。
@@ -142,15 +142,15 @@
 気をつけてください。
 kiwotsuketekudasai。
 それはいい考えですね。sorehaiikangaedesune。
 ```
 
 ### 2-3. File Export (txt -> csv)
 
-The output is saved as `output_jp.csv` in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 > tl.csv_jp("test_jp.txt")
   Original Text    Transliterated Text
 0        気を付けて。           kiwotsukete。
 1     良いニュースです。         yoinyuーsudesu。
 2      おやすみなさい。          oyasuminasai。
@@ -164,15 +164,15 @@
 Some languages such as Japanese don't have spacing between words. If there is spacing between the characters or words for text in those languages, you might bump into errors. To avoid the errors, the spacing needs to be removed.
 
 ```
 > tl.spacing("良 い ニ ュ ー ス で す。")
 良いニュースです。
 ```
 
-If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `spacing_removed.txt`.
+If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `filename_rmspace.txt`.
 
 ```
 > tl.spacing_file("test.txt")
 ```
 
 ## 4. Cyrillic
 
@@ -212,15 +212,15 @@
 Dobro jutro
 ```
 
 To exit Transliter, please press enter without any text.
 
 ### 4-2. File Export (txt -> txt)
 
-The output is saved as `output_ru.txt` (Russian) / `output_sr.txt` (Serbian) in your current directory.
+The output is saved as `filename_output.txt` in your current directory.
 
 ```
 # Russian
 > tl.txt_ru("test_ru.txt")
 Доброе утро.
 Dobroe utro.
 Меня зовут Мандли.
@@ -240,15 +240,15 @@
 Не разумем
 Ne razumem
 Извините!Izvinite!
 ```
 
 ### 4-3. File Export (txt -> csv)
 
-The output is saved as `output_ru.csv` (Russian) / `output_sr.csv` (Serbian) in your current directory.
+The output is saved as `filename_output.csv` in your current directory.
 
 ```
 # Russian
 > tl.csv_ru("test_ru.txt")
                 Original Text          Transliterated Text
 0                Доброе утро.                 Dobroe utro.
 1          Меня зовут Мандли.          Menya zovut Mandli.
```

