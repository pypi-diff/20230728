# Comparing `tmp/chrc-0.3.1.tar.gz` & `tmp/chrc-0.3.4.tar.gz`

## Comparing `chrc-0.3.1.tar` & `chrc-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chrc-0.3.1/languages_learn_source.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 chrc-0.3.1/languages_learn_source1.csv
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 chrc-0.3.1/test.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 chrc-0.3.1/update_to_pypi.bat
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 chrc-0.3.1/version_number_increase.py
--rw-r--r--   0        0        0    12064 2020-02-02 00:00:00.000000 chrc-0.3.1/chrc/Chinese_learn.py
--rw-r--r--   0        0        0    14696 2020-02-02 00:00:00.000000 chrc-0.3.1/chrc/QGUI_widget.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 chrc-0.3.1/chrc/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 chrc-0.3.1/chrc/gif_play.py
--rw-r--r--   0        0        0    43957 2020-02-02 00:00:00.000000 chrc-0.3.1/chrc/language_coach.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 chrc-0.3.1/chrc/playsound.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chrc-0.3.1/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 chrc-0.3.1/README.md
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 chrc-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 chrc-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chrc-0.3.4/languages_learn_source.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 chrc-0.3.4/languages_learn_source1.csv
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 chrc-0.3.4/test.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 chrc-0.3.4/update_to_pypi.bat
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 chrc-0.3.4/version_number_increase.py
+-rw-r--r--   0        0        0    12064 2020-02-02 00:00:00.000000 chrc-0.3.4/chrc/Chinese_learn.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chrc-0.3.4/chrc/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 chrc-0.3.4/chrc/gif_play.py
+-rw-r--r--   0        0        0    44441 2020-02-02 00:00:00.000000 chrc-0.3.4/chrc/language_coach.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 chrc-0.3.4/chrc/playsound.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chrc-0.3.4/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 chrc-0.3.4/README.md
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 chrc-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 chrc-0.3.4/PKG-INFO
```

### Comparing `chrc-0.3.1/version_number_increase.py` & `chrc-0.3.4/version_number_increase.py`

 * *Files identical despite different names*

### Comparing `chrc-0.3.1/chrc/Chinese_learn.py` & `chrc-0.3.4/chrc/Chinese_learn.py`

 * *Files identical despite different names*

### Comparing `chrc-0.3.1/chrc/gif_play.py` & `chrc-0.3.4/chrc/gif_play.py`

 * *Files identical despite different names*

### Comparing `chrc-0.3.1/chrc/language_coach.py` & `chrc-0.3.4/chrc/language_coach.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,17 +29,20 @@
 import multiprocessing
 import _thread
 import jieba
 print('import chlt.Chinese_learn')
 from chrc.Chinese_learn import *
 print(text_display_button)
 print('import chlt.gif_play')
-from chrc.gif_play import *
-print('import chlt.QGUI_widget')
-from chrc.QGUI_widget import *
+try:
+    from chrc.gif_play import *
+    from gif_play import *
+except:
+    print('fail to import gif play')
+
 
 def remove_str_punctuation(txt):
     punctuation_str = punctuation
     for i in punctuation_str:
         txt = txt.replace(i, '')
     punctuation_string = string.punctuation
     for i in punctuation_string:
@@ -553,33 +556,43 @@
             # i = self.problem_index
             if self.problem_index == 0:
                 self.initialize_widgets_for_start()
                 self.generate_problem_list_from_database()
                 # # print(self.report_dict)
 
             if self.problem_index < self.rounds_config:
+                # print('disable')
+                # self.button_record.config(state= "disabled")
                 r = int(self.rounds_val.get())-1
                 self.rounds_val.set(str(r))
                 txt = self.report_dict['problem'][self.problem_index]
                 self.input_text = txt
 
                 self.delete_privious_buttons()
                 self.creat_buttons()
+
+
+
                 self.label_word.configure(text='')
                 self.report_dict['time'][self.problem_index-1]=int(self.timer_config)-int(self.time_val.get())
+
+
+                # self.button_record.configure(background="#d9d9d9")
                 self.read(self.input_text)
 
-            if self.problem_index == self.rounds_config:
+                print('normal')
+
+            if self.problem_index >= self.rounds_config:
                 self.button_start['text'] = 'Submit'
                 self.delete_privious_buttons()
                 self.label_word.configure(text='Press Submit button to submit')
 
             self.problem_index+=1
-            if self.problem_index > self.rounds_config:
-                self.problem_index = self.rounds_config+1
+            # if self.problem_index > self.rounds_config:
+            #     self.problem_index = self.rounds_config+1
 
 
         elif self.button_start['text'] == 'Submit':
             self.button_start['text'] = 'Start'
             self.report_dict['time'][self.problem_index-2]=int(self.timer_config)-int(self.time_val.get())
             self.problem_index = 0
             self.initialize_widgets_for_stop()
@@ -954,22 +967,28 @@
         var = gTTS(text = read_text,lang = language_type,slow = True)
 
         audio_fname = os.path.join(self.source_path,read_text+'.mp3')
         # print(os.path.isfile(fname))
 
         if not os.path.isfile(audio_fname):
             # soundfile.write(audio_fname, var, 44100)
-            var.save(audio_fname)
+            try:
+                var.save(audio_fname)
+            except:
+                print('not a available text!')
 
         try:
             self.mp3_playing_processing.terminate()
 
         except:
             print('No mp3 playing processing is running.')
-        _thread.start_new_thread(playsound, (audio_fname,))
+        try:
+            _thread.start_new_thread(playsound, (audio_fname,))
+        except:
+            print(r'Exception ignored in thread started by: <function _playsoundWin at 0x000001CDBA23E5F0>aceback ')
         # self.mp3_playing_processing = multiprocessing.Process(target=playsound, args=(audio_fname,))
         # self.mp3_playing_processing.start()
         # p.terminate()
 
         # playsound(audio_fname)
         # playsound(fname)
         # os.system('\"'+audio_fname+'\"')
```

### Comparing `chrc-0.3.1/chrc/playsound.py` & `chrc-0.3.4/chrc/playsound.py`

 * *Files identical despite different names*

### Comparing `chrc-0.3.1/LICENSE` & `chrc-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chrc-0.3.1/pyproject.toml` & `chrc-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6368 7263 220d 0a76 6572 7369 6f6e   "chrc"..version
-00000070: 203d 2022 302e 332e 3122 0d0a 6175 7468   = "0.3.1"..auth
+00000070: 203d 2022 302e 332e 3422 0d0a 6175 7468   = "0.3.4"..auth
 00000080: 6f72 7320 3d20 5b0d 0a20 207b 206e 616d  ors = [..  { nam
 00000090: 653d 2273 6861 776e 2079 616e 2077 616e  e="shawn yan wan
 000000a0: 6722 2c20 656d 6169 6c3d 2273 6861 776e  g", email="shawn
 000000b0: 7961 6e77 616e 6740 676d 6169 6c2e 636f  yanwang@gmail.co
 000000c0: 6d22 207d 2c0d 0a5d 0d0a 6465 7363 7269  m" },..]..descri
 000000d0: 7074 696f 6e20 3d20 2249 7420 6973 2061  ption = "It is a
 000000e0: 2074 6f6f 6c20 746f 206c 6561 726e 2043   tool to learn C
```

### Comparing `chrc-0.3.1/PKG-INFO` & `chrc-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: chrc
-Version: 0.3.1
+Version: 0.3.4
 Summary: It is a tool to learn Chinese.
 Project-URL: Homepage, https://gitee.com/shawnyanwang/chinese-learning-tool
 Project-URL: Bug Tracker, https://gitee.com/shawnyanwang/chinese-learning-tool/issues
 Author-email: shawn yan wang <shawnyanwang@gmail.com>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: gtts>=2.2.4
 Requires-Dist: jieba>=0.42.1
```

