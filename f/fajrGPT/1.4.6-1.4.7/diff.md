# Comparing `tmp/fajrGPT-1.4.6.tar.gz` & `tmp/fajrGPT-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.4.6.tar", last modified: Wed Jul 26 10:48:41 2023, max compression
+gzip compressed data, was "fajrGPT-1.4.7.tar", last modified: Fri Jul 28 11:26:05 2023, max compression
```

## Comparing `fajrGPT-1.4.6.tar` & `fajrGPT-1.4.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-26 10:48:41.474101 fajrGPT-1.4.6/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.6/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-26 10:48:41.473473 fajrGPT-1.4.6/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.6/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-26 10:48:41.472072 fajrGPT-1.4.6/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.6/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.6/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    19125 2023-07-26 10:47:03.000000 fajrGPT-1.4.6/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-26 10:48:41.473280 fajrGPT-1.4.6/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-26 10:48:41.000000 fajrGPT-1.4.6/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-26 10:48:41.474165 fajrGPT-1.4.6/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-26 10:47:18.000000 fajrGPT-1.4.6/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-28 11:26:05.870977 fajrGPT-1.4.7/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.7/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-28 11:26:05.870793 fajrGPT-1.4.7/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.7/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-28 11:26:05.869193 fajrGPT-1.4.7/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.7/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.7/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    19455 2023-07-27 10:48:53.000000 fajrGPT-1.4.7/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-28 11:26:05.870581 fajrGPT-1.4.7/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-28 11:26:05.000000 fajrGPT-1.4.7/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-28 11:26:05.000000 fajrGPT-1.4.7/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-28 11:26:05.000000 fajrGPT-1.4.7/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-28 11:26:05.000000 fajrGPT-1.4.7/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-28 11:26:05.000000 fajrGPT-1.4.7/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-28 11:26:05.000000 fajrGPT-1.4.7/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-28 11:26:05.871020 fajrGPT-1.4.7/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-28 11:25:21.000000 fajrGPT-1.4.7/setup.py
```

### Comparing `fajrGPT-1.4.6/LICENSE` & `fajrGPT-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.6/PKG-INFO` & `fajrGPT-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.6
+Version: 1.4.7
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.6/README.md` & `fajrGPT-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.6/fajrGPT/quran_metadata.py` & `fajrGPT-1.4.7/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.6/fajrGPT/wake.py` & `fajrGPT-1.4.7/fajrGPT/wake.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,34 +74,39 @@
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
     # return back to the main thread
     play_audio_thread.join()
 
 def download_surah(surah, output):
-    # obtain the number of verses in the surah
-    num_verses = quran_chapter_to_verse[int(surah)]
-    
-    # loop over all the verses in the surah and construct the urls
-    urls = [quran_verse_to_mp3_url(f'{surah}:{verse}') for verse in range(1,num_verses+1)]
+    # check if the output file already exists
+    if os.path.exists(f'{output}.mp3'):
+        # if the output file exists, then return True
+        return True
+    else:
+        # obtain the number of verses in the surah
+        num_verses = quran_chapter_to_verse[int(surah)] + 1 # +1 corresponds to the basmalah
+        
+        # loop over all the verses in the surah and construct the urls
+        urls = [quran_verse_to_mp3_url("1:1")] + [quran_verse_to_mp3_url(f'{surah}:{verse}') for verse in range(1,num_verses+1)]
 
-    # download the verse audio and sleep for 0.5 seconds between each download
-    file_paths = [download_file_and_sleep(url,0.5) for url in urls]
+        # download the verse audio and sleep for 0.5 seconds between each download
+        file_paths = [download_file_and_sleep(url,0.5) for url in urls]
 
-    # combine the audio files
-    combined_audio = AudioSegment.empty()
-    for file_path in file_paths:
-        combined_audio += AudioSegment.from_mp3(file_path)
-    
-    # save the mp3 to the output file
-    combined_audio.export(f'{output}.mp3', format="mp3")
+        # combine the audio files
+        combined_audio = AudioSegment.empty()
+        for file_path in file_paths:
+            combined_audio += AudioSegment.from_mp3(file_path)
+        
+        # save the mp3 to the output file
+        combined_audio.export(f'{output}.mp3', format="mp3")
 
-    # delete the temporary files
-    for file_path in file_paths:
-        os.remove(file_path)
+        # delete the temporary files
+        for file_path in file_paths:
+            os.remove(file_path)
 
     return True    
 
 def play_quran_verses_audio(verses,transition_time=0.5):
     # convert verses to urls
     urls = [quran_verse_to_mp3_url(verse) for verse in verses]
 
@@ -274,15 +279,15 @@
     # initialize the verse_texts output and explanations output
     verse_texts = []
     explanations = []
 
     # Get the explanations
     for i, verse_info in enumerate(zip(verses_Quran_Module, verses)):
         verse_QM, verse = verse_info
-        verse_text = Project_Quran().Get_Ayah_English(verse_QM).split('"')[1][0:-1].replace("&quot;",'"')
+        verse_text = Project_Quran().Get_Ayah_English(verse_QM).split('"')[1][0:-1].replace("&quot;",'"').replace("&quot",'"')
         chapter_number = verse.split(':')[0]
         if i == 0:
             prompt2 = f"""
             I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
             You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
             I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
```

### Comparing `fajrGPT-1.4.6/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.4.7/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.6
+Version: 1.4.7
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.6/setup.py` & `fajrGPT-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.4.6",
+    version="1.4.7",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

