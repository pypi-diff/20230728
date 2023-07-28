# Comparing `tmp/geohydrodemo-0.0.2.tar.gz` & `tmp/geohydrodemo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geohydrodemo-0.0.2.tar", last modified: Fri Jul 28 08:24:55 2023, max compression
+gzip compressed data, was "geohydrodemo-0.0.3.tar", last modified: Fri Jul 28 08:50:47 2023, max compression
```

## Comparing `geohydrodemo-0.0.2.tar` & `geohydrodemo-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 08:24:55.970279 geohydrodemo-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-28 06:46:16.000000 geohydrodemo-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-28 06:46:16.000000 geohydrodemo-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1203 2023-07-28 08:24:55.970279 geohydrodemo-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-07-28 08:16:25.000000 geohydrodemo-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 08:24:55.958275 geohydrodemo-0.0.2/geohydrodemo/
--rw-rw-rw-   0        0        0      137 2023-07-28 08:24:20.000000 geohydrodemo-0.0.2/geohydrodemo/__init__.py
--rw-rw-rw-   0        0        0      194 2023-07-28 06:46:16.000000 geohydrodemo-0.0.2/geohydrodemo/common.py
--rw-rw-rw-   0        0        0       20 2023-07-28 06:46:16.000000 geohydrodemo-0.0.2/geohydrodemo/geohydrodemo.py
-drwxrwxrwx   0        0        0        0 2023-07-28 08:24:55.966276 geohydrodemo-0.0.2/geohydrodemo.egg-info/
--rw-rw-rw-   0        0        0     1203 2023-07-28 08:24:55.000000 geohydrodemo-0.0.2/geohydrodemo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-28 08:24:55.000000 geohydrodemo-0.0.2/geohydrodemo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 08:24:55.000000 geohydrodemo-0.0.2/geohydrodemo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 07:08:13.000000 geohydrodemo-0.0.2/geohydrodemo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-07-28 08:24:55.000000 geohydrodemo-0.0.2/geohydrodemo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-28 06:46:16.000000 geohydrodemo-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0      420 2023-07-28 08:24:55.971278 geohydrodemo-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1775 2023-07-28 08:24:20.000000 geohydrodemo-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 08:24:55.968279 geohydrodemo-0.0.2/tests/
--rw-rw-rw-   0        0        0      433 2023-07-28 06:46:16.000000 geohydrodemo-0.0.2/tests/test_geohydrodemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/geohydrodemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/geohydrodemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/geohydrodemo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/geohydrodemo/geohydrodemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/geohydrodemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/setup.py
```

### Comparing `geohydrodemo-0.0.2/LICENSE` & `geohydrodemo-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Boji Chen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Boji Chen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `geohydrodemo-0.0.2/PKG-INFO` & `geohydrodemo-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1
-Name: geohydrodemo
-Version: 0.0.2
-Summary: A python package for interactive mapping
-Home-page: https://github.com/bojichen/geohydrodemo
-Author: Boji Chen
-Author-email: bojichen@connect.hku.hk
-License: MIT license
-Keywords: geohydrodemo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# geohydrodemo
-
-
-[![image](https://img.shields.io/pypi/v/geohydrodemo.svg)](https://pypi.python.org/pypi/geohydrodemo)
-[![image](https://img.shields.io/conda/vn/conda-forge/geohydrodemo.svg)](https://anaconda.org/conda-forge/geohydrodemo)
-
-
-**A python package for interactive mapping**
-
-
--   Free software: MIT license
--   Documentation: https://bojichen.github.io/geohydrodemo
--   This is just a practice 
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: geohydrodemo
+Version: 0.0.3
+Summary: A python package for interactive mapping
+Home-page: https://github.com/bojichen/geohydrodemo
+Author: Boji Chen
+Author-email: bojichen@connect.hku.hk
+License: MIT license
+Keywords: geohydrodemo
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# geohydrodemo
+
+
+[![image](https://img.shields.io/pypi/v/geohydrodemo.svg)](https://pypi.python.org/pypi/geohydrodemo)
+[![image](https://img.shields.io/conda/vn/conda-forge/geohydrodemo.svg)](https://anaconda.org/conda-forge/geohydrodemo)
+
+
+**A python package for interactive mapping**
+
+
+-   Free software: MIT license
+-   Documentation: https://bojichen.github.io/geohydrodemo
+-   This is just a practice 
+-   PyPI: <https://pypi.org/project/geohydrodemo/>
+    
+
+## Features
+
+-   TODO
+-   TODO 2
```

### Comparing `geohydrodemo-0.0.2/geohydrodemo.egg-info/PKG-INFO` & `geohydrodemo-0.0.3/geohydrodemo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1
-Name: geohydrodemo
-Version: 0.0.2
-Summary: A python package for interactive mapping
-Home-page: https://github.com/bojichen/geohydrodemo
-Author: Boji Chen
-Author-email: bojichen@connect.hku.hk
-License: MIT license
-Keywords: geohydrodemo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# geohydrodemo
-
-
-[![image](https://img.shields.io/pypi/v/geohydrodemo.svg)](https://pypi.python.org/pypi/geohydrodemo)
-[![image](https://img.shields.io/conda/vn/conda-forge/geohydrodemo.svg)](https://anaconda.org/conda-forge/geohydrodemo)
-
-
-**A python package for interactive mapping**
-
-
--   Free software: MIT license
--   Documentation: https://bojichen.github.io/geohydrodemo
--   This is just a practice 
-    
-
-## Features
-
--   TODO
+Metadata-Version: 2.1
+Name: geohydrodemo
+Version: 0.0.3
+Summary: A python package for interactive mapping
+Home-page: https://github.com/bojichen/geohydrodemo
+Author: Boji Chen
+Author-email: bojichen@connect.hku.hk
+License: MIT license
+Keywords: geohydrodemo
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# geohydrodemo
+
+
+[![image](https://img.shields.io/pypi/v/geohydrodemo.svg)](https://pypi.python.org/pypi/geohydrodemo)
+[![image](https://img.shields.io/conda/vn/conda-forge/geohydrodemo.svg)](https://anaconda.org/conda-forge/geohydrodemo)
+
+
+**A python package for interactive mapping**
+
+
+-   Free software: MIT license
+-   Documentation: https://bojichen.github.io/geohydrodemo
+-   This is just a practice 
+-   PyPI: <https://pypi.org/project/geohydrodemo/>
+    
+
+## Features
+
+-   TODO
+-   TODO 2
```

### Comparing `geohydrodemo-0.0.2/setup.py` & `geohydrodemo-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Boji Chen",
-    author_email='bojichen@connect.hku.hk',
-    python_requires='>=3.8',
-    classifiers=[
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-    description="A python package for interactive mapping",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='geohydrodemo',
-    name='geohydrodemo',
-    packages=find_packages(include=['geohydrodemo', 'geohydrodemo.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/bojichen/geohydrodemo',
-    version='0.0.2',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Boji Chen",
+    author_email='bojichen@connect.hku.hk',
+    python_requires='>=3.8',
+    classifiers=[
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+    description="A python package for interactive mapping",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='geohydrodemo',
+    name='geohydrodemo',
+    packages=find_packages(include=['geohydrodemo', 'geohydrodemo.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/bojichen/geohydrodemo',
+    version='0.0.3',
+    zip_safe=False,
+)
```

