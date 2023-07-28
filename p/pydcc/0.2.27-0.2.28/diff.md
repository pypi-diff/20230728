# Comparing `tmp/pydcc-0.2.27.tar.gz` & `tmp/pydcc-0.2.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydcc-0.2.27.tar", last modified: Fri Jul 28 11:19:02 2023, max compression
+gzip compressed data, was "pydcc-0.2.28.tar", last modified: Fri Jul 28 11:49:44 2023, max compression
```

## Comparing `pydcc-0.2.27.tar` & `pydcc-0.2.28.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:19:02.865615 pydcc-0.2.27/
--rw-rw-rw-   0        0        0     1057 2023-03-14 11:13:43.000000 pydcc-0.2.27/LICENSE
--rw-rw-rw-   0        0        0       97 2023-04-21 08:04:52.000000 pydcc-0.2.27/MANIFEST.in
--rw-rw-rw-   0        0        0     4793 2023-07-28 11:19:02.864615 pydcc-0.2.27/PKG-INFO
--rw-rw-rw-   0        0        0     4107 2023-07-21 11:07:01.000000 pydcc-0.2.27/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 11:19:02.827514 pydcc-0.2.27/dcc/
--rw-rw-rw-   0        0        0      313 2023-07-10 14:47:54.000000 pydcc-0.2.27/dcc/__init__.py
--rw-rw-rw-   0        0        0    24633 2023-07-28 11:12:48.000000 pydcc-0.2.27/dcc/dcc.py
--rw-rw-rw-   0        0        0    15345 2023-07-12 15:33:45.000000 pydcc-0.2.27/dcc/dcc_xml_validator.py
--rw-rw-rw-   0        0        0        6 2023-07-28 11:18:48.000000 pydcc-0.2.27/next_version.txt
-drwxrwxrwx   0        0        0        0 2023-07-28 11:19:02.861614 pydcc-0.2.27/pydcc.egg-info/
--rw-rw-rw-   0        0        0     4793 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-28 11:19:02.000000 pydcc-0.2.27/pydcc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 11:19:02.865615 pydcc-0.2.27/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-07-11 09:46:25.000000 pydcc-0.2.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:49:44.283613 pydcc-0.2.28/
+-rw-rw-rw-   0        0        0     1057 2023-03-14 11:13:43.000000 pydcc-0.2.28/LICENSE
+-rw-rw-rw-   0        0        0       97 2023-04-21 08:04:52.000000 pydcc-0.2.28/MANIFEST.in
+-rw-rw-rw-   0        0        0     4846 2023-07-28 11:49:44.282617 pydcc-0.2.28/PKG-INFO
+-rw-rw-rw-   0        0        0     4160 2023-07-28 11:47:34.000000 pydcc-0.2.28/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 11:49:44.258614 pydcc-0.2.28/dcc/
+-rw-rw-rw-   0        0        0      313 2023-07-10 14:47:54.000000 pydcc-0.2.28/dcc/__init__.py
+-rw-rw-rw-   0        0        0    24633 2023-07-28 11:12:48.000000 pydcc-0.2.28/dcc/dcc.py
+-rw-rw-rw-   0        0        0    15345 2023-07-12 15:33:45.000000 pydcc-0.2.28/dcc/dcc_xml_validator.py
+-rw-rw-rw-   0        0        0        6 2023-07-28 11:48:51.000000 pydcc-0.2.28/next_version.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 11:49:44.279614 pydcc-0.2.28/pydcc.egg-info/
+-rw-rw-rw-   0        0        0     4846 2023-07-28 11:49:44.000000 pydcc-0.2.28/pydcc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-28 11:49:44.000000 pydcc-0.2.28/pydcc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:49:44.000000 pydcc-0.2.28/pydcc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-28 11:49:44.000000 pydcc-0.2.28/pydcc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-28 11:49:44.000000 pydcc-0.2.28/pydcc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:49:44.283613 pydcc-0.2.28/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-07-11 09:46:25.000000 pydcc-0.2.28/setup.py
```

### Comparing `pydcc-0.2.27/LICENSE` & `pydcc-0.2.28/LICENSE`

 * *Files identical despite different names*

### Comparing `pydcc-0.2.27/PKG-INFO` & `pydcc-0.2.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydcc
-Version: 0.2.27
+Version: 0.2.28
 Summary: Library for handling digital calibration certificates (DCC). 
 Home-page: https://gitlab.com/gemimeg/pydcc
 Author: Andreas Tobola
 Author-email: pydcc.t@siemens.com
 License: MIT License
 Keywords: digital calibration certificate measurement uncertainty precision GUM DCC
 Classifier: Development Status :: 3 - Alpha
@@ -38,26 +38,32 @@
 
 [Data examples](data) included in this repository may contain other licenses. Please refer to the license declarations within the data examples.
 
 ## Background to DCC
 
 The digital calibration certificate (DCC) is the machine-readable counterpart of the previous calibration certificate. The DCC was released by the Physikalisch-Technische Bundesanstalt (PTB) [1]. The DCC has a hierarchical structure comprising regulated areas whose information must meet specific requirements. The DCC exists in Extensible Markup Language (XML). 
 
-## Official Repository
-
-We are moving our repository to another site. We will announce the new site until August 2023.
-
 ## Aim of this software library
 
 Python is a programming language widely used in science and cloud computing applications. This software library extends Python by capabilities of handling DCC, in particular, loading DCCs from XML-Files, and operating on regulated areas of the DCC. Regulated areas in DCC are (1) administrative data and (2) measurement results. 
 
 Consider reading the [user guide](doc/pydcc.md) for more details, including API documentation.
 
 Further, the [contibution guide](CONTRIBUTING.md) explains how one can contribute to this software module.
 
+## Installation
+
+```
+pip install pydcc
+```
+
+## Official Code Repository
+
+We are moving our repository to another site. We will announce the new site until August 2023.
+
 ## Initial Contributors
 
 This project was started in January 2021 with an initial team of developers.
 
 * [Andreas Tobola](@tobola), [Siemens AG](https://siemens.com)
 * [Kai Mienert](@mienertPTB), [PTB](https://www.ptb.de)
 * [Katharina Janzen](@katharina.janzen), [PTB](https://www.ptb.de)
@@ -69,15 +75,14 @@
 
 Besides coding, the weekly team discussions were essential for achieving our goals. 
 Additional discussion supporters were:
 
 * Daniel HeiÃŸelmann, [PTB](https://www.ptb.de)
 * Benjamin Gloger, [PTB](https://www.ptb.de)
 
-
 ## References
 
 [1] The official release of the digital calibration certificate (DCC) in version 2.4.0 https://www.ptb.de/dcc/v2.4.0/de/
 
 [2] Current XML schema for DCCs https://www.ptb.de/dcc/dcc.xsd
 
 [3] The official release of the digital calibration certificate (DCC) in version 3.0.0 https://www.ptb.de/dcc/v3.0.0/
```

### Comparing `pydcc-0.2.27/README.md` & `pydcc-0.2.28/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,32 @@
 
 [Data examples](data) included in this repository may contain other licenses. Please refer to the license declarations within the data examples.
 
 ## Background to DCC
 
 The digital calibration certificate (DCC) is the machine-readable counterpart of the previous calibration certificate. The DCC was released by the Physikalisch-Technische Bundesanstalt (PTB) [1]. The DCC has a hierarchical structure comprising regulated areas whose information must meet specific requirements. The DCC exists in Extensible Markup Language (XML). 
 
-## Official Repository
-
-We are moving our repository to another site. We will announce the new site until August 2023.
-
 ## Aim of this software library
 
 Python is a programming language widely used in science and cloud computing applications. This software library extends Python by capabilities of handling DCC, in particular, loading DCCs from XML-Files, and operating on regulated areas of the DCC. Regulated areas in DCC are (1) administrative data and (2) measurement results. 
 
 Consider reading the [user guide](doc/pydcc.md) for more details, including API documentation.
 
 Further, the [contibution guide](CONTRIBUTING.md) explains how one can contribute to this software module.
 
+## Installation
+
+```
+pip install pydcc
+```
+
+## Official Code Repository
+
+We are moving our repository to another site. We will announce the new site until August 2023.
+
 ## Initial Contributors
 
 This project was started in January 2021 with an initial team of developers.
 
 * [Andreas Tobola](@tobola), [Siemens AG](https://siemens.com)
 * [Kai Mienert](@mienertPTB), [PTB](https://www.ptb.de)
 * [Katharina Janzen](@katharina.janzen), [PTB](https://www.ptb.de)
@@ -51,15 +57,14 @@
 
 Besides coding, the weekly team discussions were essential for achieving our goals. 
 Additional discussion supporters were:
 
 * Daniel Heißelmann, [PTB](https://www.ptb.de)
 * Benjamin Gloger, [PTB](https://www.ptb.de)
 
-
 ## References
 
 [1] The official release of the digital calibration certificate (DCC) in version 2.4.0 https://www.ptb.de/dcc/v2.4.0/de/
 
 [2] Current XML schema for DCCs https://www.ptb.de/dcc/dcc.xsd
 
 [3] The official release of the digital calibration certificate (DCC) in version 3.0.0 https://www.ptb.de/dcc/v3.0.0/
```

### Comparing `pydcc-0.2.27/dcc/dcc.py` & `pydcc-0.2.28/dcc/dcc.py`

 * *Files identical despite different names*

### Comparing `pydcc-0.2.27/dcc/dcc_xml_validator.py` & `pydcc-0.2.28/dcc/dcc_xml_validator.py`

 * *Files identical despite different names*

### Comparing `pydcc-0.2.27/pydcc.egg-info/PKG-INFO` & `pydcc-0.2.28/pydcc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydcc
-Version: 0.2.27
+Version: 0.2.28
 Summary: Library for handling digital calibration certificates (DCC). 
 Home-page: https://gitlab.com/gemimeg/pydcc
 Author: Andreas Tobola
 Author-email: pydcc.t@siemens.com
 License: MIT License
 Keywords: digital calibration certificate measurement uncertainty precision GUM DCC
 Classifier: Development Status :: 3 - Alpha
@@ -38,26 +38,32 @@
 
 [Data examples](data) included in this repository may contain other licenses. Please refer to the license declarations within the data examples.
 
 ## Background to DCC
 
 The digital calibration certificate (DCC) is the machine-readable counterpart of the previous calibration certificate. The DCC was released by the Physikalisch-Technische Bundesanstalt (PTB) [1]. The DCC has a hierarchical structure comprising regulated areas whose information must meet specific requirements. The DCC exists in Extensible Markup Language (XML). 
 
-## Official Repository
-
-We are moving our repository to another site. We will announce the new site until August 2023.
-
 ## Aim of this software library
 
 Python is a programming language widely used in science and cloud computing applications. This software library extends Python by capabilities of handling DCC, in particular, loading DCCs from XML-Files, and operating on regulated areas of the DCC. Regulated areas in DCC are (1) administrative data and (2) measurement results. 
 
 Consider reading the [user guide](doc/pydcc.md) for more details, including API documentation.
 
 Further, the [contibution guide](CONTRIBUTING.md) explains how one can contribute to this software module.
 
+## Installation
+
+```
+pip install pydcc
+```
+
+## Official Code Repository
+
+We are moving our repository to another site. We will announce the new site until August 2023.
+
 ## Initial Contributors
 
 This project was started in January 2021 with an initial team of developers.
 
 * [Andreas Tobola](@tobola), [Siemens AG](https://siemens.com)
 * [Kai Mienert](@mienertPTB), [PTB](https://www.ptb.de)
 * [Katharina Janzen](@katharina.janzen), [PTB](https://www.ptb.de)
@@ -69,15 +75,14 @@
 
 Besides coding, the weekly team discussions were essential for achieving our goals. 
 Additional discussion supporters were:
 
 * Daniel HeiÃŸelmann, [PTB](https://www.ptb.de)
 * Benjamin Gloger, [PTB](https://www.ptb.de)
 
-
 ## References
 
 [1] The official release of the digital calibration certificate (DCC) in version 2.4.0 https://www.ptb.de/dcc/v2.4.0/de/
 
 [2] Current XML schema for DCCs https://www.ptb.de/dcc/dcc.xsd
 
 [3] The official release of the digital calibration certificate (DCC) in version 3.0.0 https://www.ptb.de/dcc/v3.0.0/
```

### Comparing `pydcc-0.2.27/setup.py` & `pydcc-0.2.28/setup.py`

 * *Files identical despite different names*

