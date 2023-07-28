# Comparing `tmp/hyd-0.1.5.tar.gz` & `tmp/hyd-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyd-0.1.5.tar", max compression
+gzip compressed data, was "hyd-0.1.6.tar", max compression
```

## Comparing `hyd-0.1.5.tar` & `hyd-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.5/LICENSE
--rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.5/README.md
--rw-r--r--   0        0        0     4467 2023-07-28 18:26:56.948007 hyd-0.1.5/hyd/HaukursYouTubeDownloader.py
--rw-r--r--   0        0        0      457 2023-07-28 18:40:09.865965 hyd-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 hyd-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.6/LICENSE
+-rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.6/README.md
+-rw-r--r--   0        0        0     4534 2023-07-28 18:45:13.440783 hyd-0.1.6/hyd/HaukursYouTubeDownloader.py
+-rw-r--r--   0        0        0      457 2023-07-28 18:51:46.885389 hyd-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 hyd-0.1.6/PKG-INFO
```

### Comparing `hyd-0.1.5/LICENSE` & `hyd-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyd-0.1.5/hyd/HaukursYouTubeDownloader.py` & `hyd-0.1.6/hyd/HaukursYouTubeDownloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,22 +53,24 @@
 
     # Window attribute locations and dimensions
     linkInputBox.place(relx=0.5, rely=0.45, anchor=CENTER)
     likeTextLabel.place(relx=0.87, rely=0.45, anchor=CENTER)
     downloadButtonMP4.place(relx=0.37, rely=0.7, anchor=CENTER)
     downloadButtonMP3.place(relx=0.63, rely=0.7, anchor=CENTER)
 
+
     def download(link, mp3IsClicked):
         print(f"The video link is {link}")
         print(f"Mp3 button was pushed: {mp3IsClicked}")
         try:
             fixedTitle = YouTube(link).title
             unwantedChars = ".$'%"
+            print("Removing unwanted characters from final file name...")
             for char in unwantedChars: # Removes unwanted characters from final file name to avoid errors
-                print("Removing unwanted chars from final file name...")
+                print(f"Removed {char} from final file name...")
                 fixedTitle = fixedTitle.replace(char, "")
             print("Finished removing unwanted characters!\nStarting time...")
             startTime = time()
             print("Downloading video...")
             YouTube(link).streams.get_highest_resolution().download(path) # Downloads video
             if os.path.exists(f"{path}/{fixedTitle}.mp4") and mp3IsClicked:
                 print("Mp3IsClicked is true; downloading converting mp4 download to mp3 download...")
```

### Comparing `hyd-0.1.5/PKG-INFO` & `hyd-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyd
-Version: 0.1.5
+Version: 0.1.6
 Summary: A basic python youtube downloader made using tkinter, moviepy and pytube.
 License: MIT
 Author: haukurlogi
 Author-email: haukurlogi2008@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

