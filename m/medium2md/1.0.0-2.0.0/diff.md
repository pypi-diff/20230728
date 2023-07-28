# Comparing `tmp/medium2md-1.0.0.tar.gz` & `tmp/medium2md-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium2md-1.0.0.tar", last modified: Mon Jul 24 04:08:17 2023, max compression
+gzip compressed data, was "medium2md-2.0.0.tar", last modified: Fri Jul 28 16:02:24 2023, max compression
```

## Comparing `medium2md-1.0.0.tar` & `medium2md-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 siddharthsah   (501) staff       (20)        0 2023-07-24 04:08:17.108862 medium2md-1.0.0/
--rw-r--r--   0 siddharthsah   (501) staff       (20)     1076 2023-07-23 18:22:32.000000 medium2md-1.0.0/LICENSE.txt
--rw-r--r--   0 siddharthsah   (501) staff       (20)     5008 2023-07-24 04:08:17.108676 medium2md-1.0.0/PKG-INFO
--rw-r--r--   0 siddharthsah   (501) staff       (20)     4041 2023-07-24 04:02:10.000000 medium2md-1.0.0/README.md
-drwxr-xr-x   0 siddharthsah   (501) staff       (20)        0 2023-07-24 04:08:17.105602 medium2md-1.0.0/medium2md.egg-info/
--rw-r--r--   0 siddharthsah   (501) staff       (20)     5008 2023-07-24 04:08:17.000000 medium2md-1.0.0/medium2md.egg-info/PKG-INFO
--rw-r--r--   0 siddharthsah   (501) staff       (20)      369 2023-07-24 04:08:17.000000 medium2md-1.0.0/medium2md.egg-info/SOURCES.txt
--rw-r--r--   0 siddharthsah   (501) staff       (20)        1 2023-07-24 04:08:17.000000 medium2md-1.0.0/medium2md.egg-info/dependency_links.txt
--rw-r--r--   0 siddharthsah   (501) staff       (20)       44 2023-07-24 04:08:17.000000 medium2md-1.0.0/medium2md.egg-info/entry_points.txt
--rw-r--r--   0 siddharthsah   (501) staff       (20)      405 2023-07-24 04:08:17.000000 medium2md-1.0.0/medium2md.egg-info/requires.txt
--rw-r--r--   0 siddharthsah   (501) staff       (20)        4 2023-07-24 04:08:17.000000 medium2md-1.0.0/medium2md.egg-info/top_level.txt
--rw-r--r--   0 siddharthsah   (501) staff       (20)       38 2023-07-24 04:08:17.108911 medium2md-1.0.0/setup.cfg
--rw-r--r--   0 siddharthsah   (501) staff       (20)     2010 2023-07-24 03:35:58.000000 medium2md-1.0.0/setup.py
-drwxr-xr-x   0 siddharthsah   (501) staff       (20)        0 2023-07-24 04:08:17.108258 medium2md-1.0.0/src/
--rw-r--r--   0 siddharthsah   (501) staff       (20)        0 2023-07-23 06:31:10.000000 medium2md-1.0.0/src/__init__.py
--rw-r--r--   0 siddharthsah   (501) staff       (20)     4601 2023-07-23 16:22:13.000000 medium2md-1.0.0/src/clean_md.py
--rw-r--r--   0 siddharthsah   (501) staff       (20)      246 2023-07-23 16:41:26.000000 medium2md-1.0.0/src/clean_unnecessary_data.py
--rw-r--r--   0 siddharthsah   (501) staff       (20)     4090 2023-07-24 03:49:39.000000 medium2md-1.0.0/src/download_with_media.py
--rw-r--r--   0 siddharthsah   (501) staff       (20)     1680 2023-07-23 16:35:16.000000 medium2md-1.0.0/src/html_to_md.py
--rw-r--r--   0 siddharthsah   (501) staff       (20)     6066 2023-07-23 17:53:28.000000 medium2md-1.0.0/src/main.py
--rw-r--r--   0 siddharthsah   (501) staff       (20)     3507 2023-07-23 16:42:02.000000 medium2md-1.0.0/src/url_to_local.py
+drwxr-xr-x   0 siddharthsah   (501) staff       (20)        0 2023-07-28 16:02:24.228957 medium2md-2.0.0/
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     1076 2023-07-28 15:56:07.000000 medium2md-2.0.0/LICENSE.txt
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     5022 2023-07-28 16:02:24.228803 medium2md-2.0.0/PKG-INFO
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     4055 2023-07-28 15:56:07.000000 medium2md-2.0.0/README.md
+drwxr-xr-x   0 siddharthsah   (501) staff       (20)        0 2023-07-28 16:02:24.227712 medium2md-2.0.0/medium2md.egg-info/
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     5022 2023-07-28 16:02:24.000000 medium2md-2.0.0/medium2md.egg-info/PKG-INFO
+-rw-r--r--   0 siddharthsah   (501) staff       (20)      369 2023-07-28 16:02:24.000000 medium2md-2.0.0/medium2md.egg-info/SOURCES.txt
+-rw-r--r--   0 siddharthsah   (501) staff       (20)        1 2023-07-28 16:02:24.000000 medium2md-2.0.0/medium2md.egg-info/dependency_links.txt
+-rw-r--r--   0 siddharthsah   (501) staff       (20)       44 2023-07-28 16:02:24.000000 medium2md-2.0.0/medium2md.egg-info/entry_points.txt
+-rw-r--r--   0 siddharthsah   (501) staff       (20)      405 2023-07-28 16:02:24.000000 medium2md-2.0.0/medium2md.egg-info/requires.txt
+-rw-r--r--   0 siddharthsah   (501) staff       (20)        4 2023-07-28 16:02:24.000000 medium2md-2.0.0/medium2md.egg-info/top_level.txt
+-rw-r--r--   0 siddharthsah   (501) staff       (20)       38 2023-07-28 16:02:24.229005 medium2md-2.0.0/setup.cfg
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     2010 2023-07-28 16:02:10.000000 medium2md-2.0.0/setup.py
+drwxr-xr-x   0 siddharthsah   (501) staff       (20)        0 2023-07-28 16:02:24.228602 medium2md-2.0.0/src/
+-rw-r--r--   0 siddharthsah   (501) staff       (20)        0 2023-07-28 15:56:07.000000 medium2md-2.0.0/src/__init__.py
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     4601 2023-07-28 15:56:07.000000 medium2md-2.0.0/src/clean_md.py
+-rw-r--r--   0 siddharthsah   (501) staff       (20)      246 2023-07-28 15:56:07.000000 medium2md-2.0.0/src/clean_unnecessary_data.py
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     4090 2023-07-28 15:56:07.000000 medium2md-2.0.0/src/download_with_media.py
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     1680 2023-07-28 15:56:07.000000 medium2md-2.0.0/src/html_to_md.py
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     6188 2023-07-28 15:56:07.000000 medium2md-2.0.0/src/main.py
+-rw-r--r--   0 siddharthsah   (501) staff       (20)     3507 2023-07-28 15:56:07.000000 medium2md-2.0.0/src/url_to_local.py
```

### Comparing `medium2md-1.0.0/LICENSE.txt` & `medium2md-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `medium2md-1.0.0/PKG-INFO` & `medium2md-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium2md
-Version: 1.0.0
+Version: 2.0.0
 Summary: Download and convert Medium articles to markdown with images
 Home-page: https://github.com/siddharthksah/medium2md
 Author: Siddharth Kumar
 Author-email: siddharth123sk@gmail.com
 Project-URL: Bug Tracker, https://github.com/siddharthksah/medium2md/issues
 Project-URL: Documentation, https://github.com/siddharthksah/medium2md#readme
 Project-URL: Source Code, https://github.com/siddharthksah/medium2md
@@ -17,29 +17,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Medium2md
-
-<p align="center">
-  <img src="demo.png" alt="Medium2md Demo">
-</p>
-
+![Header](./header.png)
 <p align="center">
   <a href="https://github.com/siddharthksah/medium2md/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/blob/main/LICENSE.txt"><img alt="GitHub license" src="https://img.shields.io/github/license/siddharthksah/medium2md"></a>
 </p>
 
 Convert your favorite Medium articles into markdown files using `Medium2md`, a powerful and user-friendly command-line tool. Designed in Python, it extends beyond simple conversion to download all images within the article, saving them locally and integrating them into your markdown file seamlessly.
 
+<p align="center">
+  <img src="demo.png" alt="Medium2md Demo">
+</p>
+
 ## Table of Contents
 
 - [Features](#features)
 - [Getting Started](#getting-started)
 - [Usage](#usage)
 - [Project Structure](#project-structure)
 - [Contributing](#contributing)
@@ -72,15 +71,15 @@
     ```bash
     cd medium2md
     ```
 
 3. Create a new conda environment and activate it:
 
     ```bash
-    conda create --name medium2md python=3.8
+    conda create --name medium2md python=3.8 -y
     conda activate medium2md
     ```
 
 4. Install the package and its dependencies using `setup.py`:
 
     ```bash
     python3 setup.py install
```

#### html2text {}

```diff
@@ -1,49 +1,50 @@
-Metadata-Version: 2.1 Name: medium2md Version: 1.0.0 Summary: Download and
+Metadata-Version: 2.1 Name: medium2md Version: 2.0.0 Summary: Download and
 convert Medium articles to markdown with images Home-page: https://github.com/
 siddharthksah/medium2md Author: Siddharth Kumar Author-email:
 siddharth123sk@gmail.com Project-URL: Bug Tracker, https://github.com/
 siddharthksah/medium2md/issues Project-URL: Documentation, https://github.com/
 siddharthksah/medium2md#readme Project-URL: Source Code, https://github.com/
 siddharthksah/medium2md Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
 Text Processing Classifier: Topic :: Utilities Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.txt # Medium2md
-                               [Medium2md Demo]
+Description-Content-Type: text/markdown License-File: LICENSE.txt ![Header](./
+header.png)
         [GitHub_issues] [GitHub_forks] [GitHub_stars] [GitHub_license]
 Convert your favorite Medium articles into markdown files using `Medium2md`, a
 powerful and user-friendly command-line tool. Designed in Python, it extends
 beyond simple conversion to download all images within the article, saving them
-locally and integrating them into your markdown file seamlessly. ## Table of
-Contents - [Features](#features) - [Getting Started](#getting-started) -
-[Usage](#usage) - [Project Structure](#project-structure) - [Contributing]
-(#contributing) - [License](#license) ## Features - **Efficient Conversion**:
-Download Medium articles as HTML and convert them into clean, readable Markdown
-files. - **Image Handling**: Download images from the article, save them
-locally, and update image URLs in the markdown files to point to local paths. -
-**Post-Processing**: Automatically clean up unnecessary data after conversion.
-- **User-Friendly**: Interactive CLI interface with progress bars and prompts
-for an enhanced user experience. ## Getting Started ### Prerequisites - Python
-3.8 or later - Conda ### Installation 1. Clone the repository: ```bash git
-clone https://github.com/siddharthksah/medium2md.git ``` 2. Navigate into the
-project directory: ```bash cd medium2md ``` 3. Create a new conda environment
-and activate it: ```bash conda create --name medium2md python=3.8 conda
-activate medium2md ``` 4. Install the package and its dependencies using
-`setup.py`: ```bash python3 setup.py install playwright install ``` This will
-automatically install all required packages listed in `setup.py`'s
-`install_requires` section. ## Usage Run `medium2md` with: ```bash python3 src/
-main.py -u  ``` Replace  with the URL of the Medium article you wish to
-download. If no URL is provided, the script will prompt you to input one. When
-the process is complete, the script will ask if you wish to open the downloaded
-markdown file in your default editor. ## Output The converted articles are
-stored in the output directory, which is created in the project's root
-directory. ## Unittests ### Running Unittests To run the unittests for the
+locally and integrating them into your markdown file seamlessly.
+                               [Medium2md Demo]
+## Table of Contents - [Features](#features) - [Getting Started](#getting-
+started) - [Usage](#usage) - [Project Structure](#project-structure) -
+[Contributing](#contributing) - [License](#license) ## Features - **Efficient
+Conversion**: Download Medium articles as HTML and convert them into clean,
+readable Markdown files. - **Image Handling**: Download images from the
+article, save them locally, and update image URLs in the markdown files to
+point to local paths. - **Post-Processing**: Automatically clean up unnecessary
+data after conversion. - **User-Friendly**: Interactive CLI interface with
+progress bars and prompts for an enhanced user experience. ## Getting Started
+### Prerequisites - Python 3.8 or later - Conda ### Installation 1. Clone the
+repository: ```bash git clone https://github.com/siddharthksah/medium2md.git
+``` 2. Navigate into the project directory: ```bash cd medium2md ``` 3. Create
+a new conda environment and activate it: ```bash conda create --name medium2md
+python=3.8 -y conda activate medium2md ``` 4. Install the package and its
+dependencies using `setup.py`: ```bash python3 setup.py install playwright
+install ``` This will automatically install all required packages listed in
+`setup.py`'s `install_requires` section. ## Usage Run `medium2md` with: ```bash
+python3 src/main.py -u  ``` Replace  with the URL of the Medium article you
+wish to download. If no URL is provided, the script will prompt you to input
+one. When the process is complete, the script will ask if you wish to open the
+downloaded markdown file in your default editor. ## Output The converted
+articles are stored in the output directory, which is created in the project's
+root directory. ## Unittests ### Running Unittests To run the unittests for the
 `Medium2md` project, navigate to the root directory of the project and use the
 following command: ```bash python -m unittest discover unittests ``` This will
 automatically discover and run all the unittests in the unittests directory.
 Please ensure that you have installed the required packages for the project by
 following the installation instructions in the `Getting Started` section. ##
 ð Project Structure ```markdown . âââ LICENSE.txt âââ README.md
 âââ docs âââ output âââ requirements.txt âââ src
```

### Comparing `medium2md-1.0.0/README.md` & `medium2md-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# Medium2md
-
-<p align="center">
-  <img src="demo.png" alt="Medium2md Demo">
-</p>
-
+![Header](./header.png)
 <p align="center">
   <a href="https://github.com/siddharthksah/medium2md/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/blob/main/LICENSE.txt"><img alt="GitHub license" src="https://img.shields.io/github/license/siddharthksah/medium2md"></a>
 </p>
 
 Convert your favorite Medium articles into markdown files using `Medium2md`, a powerful and user-friendly command-line tool. Designed in Python, it extends beyond simple conversion to download all images within the article, saving them locally and integrating them into your markdown file seamlessly.
 
+<p align="center">
+  <img src="demo.png" alt="Medium2md Demo">
+</p>
+
 ## Table of Contents
 
 - [Features](#features)
 - [Getting Started](#getting-started)
 - [Usage](#usage)
 - [Project Structure](#project-structure)
 - [Contributing](#contributing)
@@ -49,15 +48,15 @@
     ```bash
     cd medium2md
     ```
 
 3. Create a new conda environment and activate it:
 
     ```bash
-    conda create --name medium2md python=3.8
+    conda create --name medium2md python=3.8 -y
     conda activate medium2md
     ```
 
 4. Install the package and its dependencies using `setup.py`:
 
     ```bash
     python3 setup.py install
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-# Medium2md
-                               [Medium2md Demo]
+![Header](./header.png)
         [GitHub_issues] [GitHub_forks] [GitHub_stars] [GitHub_license]
 Convert your favorite Medium articles into markdown files using `Medium2md`, a
 powerful and user-friendly command-line tool. Designed in Python, it extends
 beyond simple conversion to download all images within the article, saving them
-locally and integrating them into your markdown file seamlessly. ## Table of
-Contents - [Features](#features) - [Getting Started](#getting-started) -
-[Usage](#usage) - [Project Structure](#project-structure) - [Contributing]
-(#contributing) - [License](#license) ## Features - **Efficient Conversion**:
-Download Medium articles as HTML and convert them into clean, readable Markdown
-files. - **Image Handling**: Download images from the article, save them
-locally, and update image URLs in the markdown files to point to local paths. -
-**Post-Processing**: Automatically clean up unnecessary data after conversion.
-- **User-Friendly**: Interactive CLI interface with progress bars and prompts
-for an enhanced user experience. ## Getting Started ### Prerequisites - Python
-3.8 or later - Conda ### Installation 1. Clone the repository: ```bash git
-clone https://github.com/siddharthksah/medium2md.git ``` 2. Navigate into the
-project directory: ```bash cd medium2md ``` 3. Create a new conda environment
-and activate it: ```bash conda create --name medium2md python=3.8 conda
-activate medium2md ``` 4. Install the package and its dependencies using
-`setup.py`: ```bash python3 setup.py install playwright install ``` This will
-automatically install all required packages listed in `setup.py`'s
-`install_requires` section. ## Usage Run `medium2md` with: ```bash python3 src/
-main.py -u  ``` Replace  with the URL of the Medium article you wish to
-download. If no URL is provided, the script will prompt you to input one. When
-the process is complete, the script will ask if you wish to open the downloaded
-markdown file in your default editor. ## Output The converted articles are
-stored in the output directory, which is created in the project's root
-directory. ## Unittests ### Running Unittests To run the unittests for the
+locally and integrating them into your markdown file seamlessly.
+                               [Medium2md Demo]
+## Table of Contents - [Features](#features) - [Getting Started](#getting-
+started) - [Usage](#usage) - [Project Structure](#project-structure) -
+[Contributing](#contributing) - [License](#license) ## Features - **Efficient
+Conversion**: Download Medium articles as HTML and convert them into clean,
+readable Markdown files. - **Image Handling**: Download images from the
+article, save them locally, and update image URLs in the markdown files to
+point to local paths. - **Post-Processing**: Automatically clean up unnecessary
+data after conversion. - **User-Friendly**: Interactive CLI interface with
+progress bars and prompts for an enhanced user experience. ## Getting Started
+### Prerequisites - Python 3.8 or later - Conda ### Installation 1. Clone the
+repository: ```bash git clone https://github.com/siddharthksah/medium2md.git
+``` 2. Navigate into the project directory: ```bash cd medium2md ``` 3. Create
+a new conda environment and activate it: ```bash conda create --name medium2md
+python=3.8 -y conda activate medium2md ``` 4. Install the package and its
+dependencies using `setup.py`: ```bash python3 setup.py install playwright
+install ``` This will automatically install all required packages listed in
+`setup.py`'s `install_requires` section. ## Usage Run `medium2md` with: ```bash
+python3 src/main.py -u  ``` Replace  with the URL of the Medium article you
+wish to download. If no URL is provided, the script will prompt you to input
+one. When the process is complete, the script will ask if you wish to open the
+downloaded markdown file in your default editor. ## Output The converted
+articles are stored in the output directory, which is created in the project's
+root directory. ## Unittests ### Running Unittests To run the unittests for the
 `Medium2md` project, navigate to the root directory of the project and use the
 following command: ```bash python -m unittest discover unittests ``` This will
 automatically discover and run all the unittests in the unittests directory.
 Please ensure that you have installed the required packages for the project by
 following the installation instructions in the `Getting Started` section. ##
 ð Project Structure ```markdown . âââ LICENSE.txt âââ README.md
 âââ docs âââ output âââ requirements.txt âââ src
```

### Comparing `medium2md-1.0.0/medium2md.egg-info/PKG-INFO` & `medium2md-2.0.0/medium2md.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium2md
-Version: 1.0.0
+Version: 2.0.0
 Summary: Download and convert Medium articles to markdown with images
 Home-page: https://github.com/siddharthksah/medium2md
 Author: Siddharth Kumar
 Author-email: siddharth123sk@gmail.com
 Project-URL: Bug Tracker, https://github.com/siddharthksah/medium2md/issues
 Project-URL: Documentation, https://github.com/siddharthksah/medium2md#readme
 Project-URL: Source Code, https://github.com/siddharthksah/medium2md
@@ -17,29 +17,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Medium2md
-
-<p align="center">
-  <img src="demo.png" alt="Medium2md Demo">
-</p>
-
+![Header](./header.png)
 <p align="center">
   <a href="https://github.com/siddharthksah/medium2md/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/siddharthksah/medium2md"></a>
   <a href="https://github.com/siddharthksah/medium2md/blob/main/LICENSE.txt"><img alt="GitHub license" src="https://img.shields.io/github/license/siddharthksah/medium2md"></a>
 </p>
 
 Convert your favorite Medium articles into markdown files using `Medium2md`, a powerful and user-friendly command-line tool. Designed in Python, it extends beyond simple conversion to download all images within the article, saving them locally and integrating them into your markdown file seamlessly.
 
+<p align="center">
+  <img src="demo.png" alt="Medium2md Demo">
+</p>
+
 ## Table of Contents
 
 - [Features](#features)
 - [Getting Started](#getting-started)
 - [Usage](#usage)
 - [Project Structure](#project-structure)
 - [Contributing](#contributing)
@@ -72,15 +71,15 @@
     ```bash
     cd medium2md
     ```
 
 3. Create a new conda environment and activate it:
 
     ```bash
-    conda create --name medium2md python=3.8
+    conda create --name medium2md python=3.8 -y
     conda activate medium2md
     ```
 
 4. Install the package and its dependencies using `setup.py`:
 
     ```bash
     python3 setup.py install
```

#### html2text {}

```diff
@@ -1,49 +1,50 @@
-Metadata-Version: 2.1 Name: medium2md Version: 1.0.0 Summary: Download and
+Metadata-Version: 2.1 Name: medium2md Version: 2.0.0 Summary: Download and
 convert Medium articles to markdown with images Home-page: https://github.com/
 siddharthksah/medium2md Author: Siddharth Kumar Author-email:
 siddharth123sk@gmail.com Project-URL: Bug Tracker, https://github.com/
 siddharthksah/medium2md/issues Project-URL: Documentation, https://github.com/
 siddharthksah/medium2md#readme Project-URL: Source Code, https://github.com/
 siddharthksah/medium2md Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
 Text Processing Classifier: Topic :: Utilities Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.txt # Medium2md
-                               [Medium2md Demo]
+Description-Content-Type: text/markdown License-File: LICENSE.txt ![Header](./
+header.png)
         [GitHub_issues] [GitHub_forks] [GitHub_stars] [GitHub_license]
 Convert your favorite Medium articles into markdown files using `Medium2md`, a
 powerful and user-friendly command-line tool. Designed in Python, it extends
 beyond simple conversion to download all images within the article, saving them
-locally and integrating them into your markdown file seamlessly. ## Table of
-Contents - [Features](#features) - [Getting Started](#getting-started) -
-[Usage](#usage) - [Project Structure](#project-structure) - [Contributing]
-(#contributing) - [License](#license) ## Features - **Efficient Conversion**:
-Download Medium articles as HTML and convert them into clean, readable Markdown
-files. - **Image Handling**: Download images from the article, save them
-locally, and update image URLs in the markdown files to point to local paths. -
-**Post-Processing**: Automatically clean up unnecessary data after conversion.
-- **User-Friendly**: Interactive CLI interface with progress bars and prompts
-for an enhanced user experience. ## Getting Started ### Prerequisites - Python
-3.8 or later - Conda ### Installation 1. Clone the repository: ```bash git
-clone https://github.com/siddharthksah/medium2md.git ``` 2. Navigate into the
-project directory: ```bash cd medium2md ``` 3. Create a new conda environment
-and activate it: ```bash conda create --name medium2md python=3.8 conda
-activate medium2md ``` 4. Install the package and its dependencies using
-`setup.py`: ```bash python3 setup.py install playwright install ``` This will
-automatically install all required packages listed in `setup.py`'s
-`install_requires` section. ## Usage Run `medium2md` with: ```bash python3 src/
-main.py -u  ``` Replace  with the URL of the Medium article you wish to
-download. If no URL is provided, the script will prompt you to input one. When
-the process is complete, the script will ask if you wish to open the downloaded
-markdown file in your default editor. ## Output The converted articles are
-stored in the output directory, which is created in the project's root
-directory. ## Unittests ### Running Unittests To run the unittests for the
+locally and integrating them into your markdown file seamlessly.
+                               [Medium2md Demo]
+## Table of Contents - [Features](#features) - [Getting Started](#getting-
+started) - [Usage](#usage) - [Project Structure](#project-structure) -
+[Contributing](#contributing) - [License](#license) ## Features - **Efficient
+Conversion**: Download Medium articles as HTML and convert them into clean,
+readable Markdown files. - **Image Handling**: Download images from the
+article, save them locally, and update image URLs in the markdown files to
+point to local paths. - **Post-Processing**: Automatically clean up unnecessary
+data after conversion. - **User-Friendly**: Interactive CLI interface with
+progress bars and prompts for an enhanced user experience. ## Getting Started
+### Prerequisites - Python 3.8 or later - Conda ### Installation 1. Clone the
+repository: ```bash git clone https://github.com/siddharthksah/medium2md.git
+``` 2. Navigate into the project directory: ```bash cd medium2md ``` 3. Create
+a new conda environment and activate it: ```bash conda create --name medium2md
+python=3.8 -y conda activate medium2md ``` 4. Install the package and its
+dependencies using `setup.py`: ```bash python3 setup.py install playwright
+install ``` This will automatically install all required packages listed in
+`setup.py`'s `install_requires` section. ## Usage Run `medium2md` with: ```bash
+python3 src/main.py -u  ``` Replace  with the URL of the Medium article you
+wish to download. If no URL is provided, the script will prompt you to input
+one. When the process is complete, the script will ask if you wish to open the
+downloaded markdown file in your default editor. ## Output The converted
+articles are stored in the output directory, which is created in the project's
+root directory. ## Unittests ### Running Unittests To run the unittests for the
 `Medium2md` project, navigate to the root directory of the project and use the
 following command: ```bash python -m unittest discover unittests ``` This will
 automatically discover and run all the unittests in the unittests directory.
 Please ensure that you have installed the required packages for the project by
 following the installation instructions in the `Getting Started` section. ##
 ð Project Structure ```markdown . âââ LICENSE.txt âââ README.md
 âââ docs âââ output âââ requirements.txt âââ src
```

### Comparing `medium2md-1.0.0/setup.py` & `medium2md-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="medium2md",
-    version="1.0.0",
+    version="2.0.0",
     author="Siddharth Kumar",
     author_email="siddharth123sk@gmail.com",
     description="Download and convert Medium articles to markdown with images",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/siddharthksah/medium2md",
     packages=setuptools.find_packages(),
```

### Comparing `medium2md-1.0.0/src/clean_md.py` & `medium2md-2.0.0/src/clean_md.py`

 * *Files identical despite different names*

### Comparing `medium2md-1.0.0/src/download_with_media.py` & `medium2md-2.0.0/src/download_with_media.py`

 * *Files identical despite different names*

### Comparing `medium2md-1.0.0/src/html_to_md.py` & `medium2md-2.0.0/src/html_to_md.py`

 * *Files identical despite different names*

### Comparing `medium2md-1.0.0/src/main.py` & `medium2md-2.0.0/src/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 def main():
     """
     The main function to execute the script.
     """
     # Parse arguments
     parser = argparse.ArgumentParser(description='Download Medium articles with images and convert them into markdown files.')
     parser.add_argument('-u', '--url', type=str, help='URL of the Medium article')
+    parser.add_argument('-h', '--help', action='help', default=argparse.SUPPRESS, help='Show this help message and exit')
     args = parser.parse_args()
 
     # If no URL is given, prompt the user to enter it
     if not args.url:
         args.url = prompt_input("Enter the URL of the Medium article:")
 
     # If the URL is not valid, prompt the user to enter it again
```

### Comparing `medium2md-1.0.0/src/url_to_local.py` & `medium2md-2.0.0/src/url_to_local.py`

 * *Files identical despite different names*

