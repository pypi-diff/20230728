# Comparing `tmp/wheezy.security-3.0.1.tar.gz` & `tmp/wheezy.security-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheezy.security-3.0.1.tar", last modified: Sat Dec 19 15:12:17 2020, max compression
+gzip compressed data, was "wheezy.security-3.2.0.tar", last modified: Fri Jul 28 10:58:29 2023, max compression
```

## Comparing `wheezy.security-3.0.1.tar` & `wheezy.security-3.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 15:12:17.253202 wheezy.security-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3895 2020-12-19 15:12:17.249202 wheezy.security-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2361 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-19 15:12:17.253202 wheezy.security-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2254 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 15:12:17.249202 wheezy.security-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 15:12:17.249202 wheezy.security-3.0.1/src/wheezy/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 15:12:17.249202 wheezy.security-3.0.1/src/wheezy/security/
--rw-r--r--   0 runner    (1001) docker     (116)      253 2020-12-19 15:12:16.000000 wheezy.security-3.0.1/src/wheezy/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1687 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/security/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 15:12:17.249202 wheezy.security-3.0.1/src/wheezy/security/crypto/
--rw-r--r--   0 runner    (1001) docker     (116)      117 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/security/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4733 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/security/crypto/comp.py
--rw-r--r--   0 runner    (1001) docker     (116)      847 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/security/crypto/padding.py
--rw-r--r--   0 runner    (1001) docker     (116)     4116 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/security/crypto/ticket.py
--rw-r--r--   0 runner    (1001) docker     (116)      221 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/security/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)      647 2020-12-19 15:12:03.000000 wheezy.security-3.0.1/src/wheezy/security/principal.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-19 15:12:17.249202 wheezy.security-3.0.1/src/wheezy.security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3895 2020-12-19 15:12:16.000000 wheezy.security-3.0.1/src/wheezy.security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      608 2020-12-19 15:12:17.000000 wheezy.security-3.0.1/src/wheezy.security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-19 15:12:16.000000 wheezy.security-3.0.1/src/wheezy.security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-19 15:12:16.000000 wheezy.security-3.0.1/src/wheezy.security.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-19 15:12:16.000000 wheezy.security-3.0.1/src/wheezy.security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-12-19 15:12:16.000000 wheezy.security-3.0.1/src/wheezy.security.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/src/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/src/wheezy/security/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 10:58:27.000000 wheezy.security-3.2.0/src/wheezy/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/security/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/src/wheezy/security/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/security/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/security/crypto/comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/security/crypto/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/security/crypto/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/security/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-28 10:58:20.000000 wheezy.security-3.2.0/src/wheezy/security/principal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:58:29.206792 wheezy.security-3.2.0/src/wheezy.security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-28 10:58:29.000000 wheezy.security-3.2.0/src/wheezy.security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-28 10:58:29.000000 wheezy.security-3.2.0/src/wheezy.security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:29.000000 wheezy.security-3.2.0/src/wheezy.security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:29.000000 wheezy.security-3.2.0/src/wheezy.security.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:58:29.000000 wheezy.security-3.2.0/src/wheezy.security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:58:29.000000 wheezy.security-3.2.0/src/wheezy.security.egg-info/top_level.txt
```

### Comparing `wheezy.security-3.0.1/LICENSE` & `wheezy.security-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wheezy.security-3.0.1/PKG-INFO` & `wheezy.security-3.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 Metadata-Version: 2.1
 Name: wheezy.security
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight security/cryptography library
 Home-page: https://github.com/akornatskyy/wheezy.security
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.security
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.security.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.security)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.security/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.security?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezysecurity/badge/?version=latest)](https://wheezysecurity.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.security.svg)](https://badge.fury.io/py/wheezy.security)
-        
-        [wheezy.security](https://pypi.org/project/wheezy.security/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        is a lightweight security library that provides integration with:
-        
-        - [pycrypto](https://www.dlitz.net/software/pycrypto) - The Python
-          Cryptography Toolkit.
-        - [pycryptodome](https://www.pycryptodome.org) - PyCryptodome
-          is a fork of PyCrypto. It brings several enhancements.
-        - [pycryptodomex](https://www.pycryptodome.org) - PyCryptodomex
-          is a library independent of the PyCrypto.
-        - [cryptography](https://pypi.org/project/cryptography/) - cryptography
-          is a package which provides cryptographic recipes and primitives to
-          Python developers.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.security),
-          and [issues](https://github.com/akornatskyy/wheezy.security/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.security)
-        - [documentation](https://wheezysecurity.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.security](https://pypi.org/project/wheezy.security/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.security/) site:
-        
-        ```sh
-        pip install -U wheezy.security
-        ```
-        
-        If you would like take benefit of one of cryptography library that has
-        built-in support specify extra requirements:
-        
-        ```sh
-        pip install wheezy.security[pycrypto]
-        pip install wheezy.security[pycryptodome]
-        pip install wheezy.security[pycryptodomex]
-        pip install wheezy.security[cryptography]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.security).
-        
 Keywords: security ticket encryption pycrypto
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.security
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.security.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.security)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.security/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.security?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezysecurity/badge/?version=latest)](https://wheezysecurity.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.security.svg)](https://badge.fury.io/py/wheezy.security)
+
+[wheezy.security](https://pypi.org/project/wheezy.security/) is a
+[python](https://www.python.org) package written in pure Python code. It
+is a lightweight security library that provides integration with:
+
+- [pycrypto](https://www.dlitz.net/software/pycrypto) - The Python
+  Cryptography Toolkit.
+- [pycryptodome](https://www.pycryptodome.org) - PyCryptodome
+  is a fork of PyCrypto. It brings several enhancements.
+- [pycryptodomex](https://www.pycryptodome.org) - PyCryptodomex
+  is a library independent of the PyCrypto.
+- [cryptography](https://pypi.org/project/cryptography/) - cryptography
+  is a package which provides cryptographic recipes and primitives to
+  Python developers.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.security),
+  and [issues](https://github.com/akornatskyy/wheezy.security/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.security)
+- [documentation](https://wheezysecurity.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.security](https://pypi.org/project/wheezy.security/) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.security/) site:
+
+```sh
+pip install -U wheezy.security
+```
+
+If you would like take benefit of one of cryptography library that has
+built-in support specify extra requirements:
+
+```sh
+pip install wheezy.security[pycrypto]
+pip install wheezy.security[pycryptodome]
+pip install wheezy.security[pycryptodomex]
+pip install wheezy.security[cryptography]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.security).
```

### Comparing `wheezy.security-3.0.1/README.md` & `wheezy.security-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   tracker are available on
   [github](https://github.com/akornatskyy/wheezy.security)
 - [documentation](https://wheezysecurity.readthedocs.io/en/latest/)
 
 ## Install
 
 [wheezy.security](https://pypi.org/project/wheezy.security/) requires
-[python](https://www.python.org) version 3.6+. It is independent of operating
+[python](https://www.python.org) version 3.8+. It is independent of operating
 system. You can install it from
 [pypi](https://pypi.org/project/wheezy.security/) site:
 
 ```sh
 pip install -U wheezy.security
 ```
```

### Comparing `wheezy.security-3.0.1/setup.py` & `wheezy.security-3.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,32 +34,32 @@
     .group(1)
     .strip()
 )
 
 setup(
     name="wheezy.security",
     version=VERSION,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     description="A lightweight security/cryptography library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/akornatskyy/wheezy.security",
     author="Andriy Kornatskyy",
     author_email="andriy.kornatskyy@live.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Security",
         "Topic :: Security :: Cryptography",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="security ticket encryption pycrypto",
```

### Comparing `wheezy.security-3.0.1/src/wheezy/security/authorization.py` & `wheezy.security-3.2.0/src/wheezy/security/authorization.py`

 * *Files identical despite different names*

### Comparing `wheezy.security-3.0.1/src/wheezy/security/crypto/comp.py` & `wheezy.security-3.2.0/src/wheezy/security/crypto/comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     def ripemd160():
         return openssl_hash("ripemd160")  # pragma: nocover
 
     def whirlpool():
         return openssl_hash("whirlpool")  # pragma: nocover
 
-
 except ValueError:  # pragma: nocover
     ripemd160 = None
     whirlpool = None
 
 
 # Encryption interface
 
@@ -81,15 +80,14 @@
         assert len(key) >= key_size
         if len(key) < key_size + 16:  # pragma: nocover
             warn("AES%d: key and iv overlap." % (key_size * 8))
         key = key[-key_size:]
         iv = key[:16]
         return lambda: AES.new(key, AES.MODE_CBC, iv)
 
-
 except ImportError:  # pragma: nocover
     try:  # pragma: nocover
         from cryptography.hazmat.backends import default_backend
         from cryptography.hazmat.primitives.ciphers import (
             Cipher,
             algorithms,
             modes,
```

### Comparing `wheezy.security-3.0.1/src/wheezy/security/crypto/padding.py` & `wheezy.security-3.2.0/src/wheezy/security/crypto/padding.py`

 * *Files identical despite different names*

### Comparing `wheezy.security-3.0.1/src/wheezy/security/crypto/ticket.py` & `wheezy.security-3.2.0/src/wheezy/security/crypto/ticket.py`

 * *Files identical despite different names*

### Comparing `wheezy.security-3.0.1/src/wheezy/security/principal.py` & `wheezy.security-3.2.0/src/wheezy/security/principal.py`

 * *Files identical despite different names*

### Comparing `wheezy.security-3.0.1/src/wheezy.security.egg-info/PKG-INFO` & `wheezy.security-3.2.0/src/wheezy.security.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 Metadata-Version: 2.1
 Name: wheezy.security
-Version: 3.0.1
+Version: 3.2.0
 Summary: A lightweight security/cryptography library
 Home-page: https://github.com/akornatskyy/wheezy.security
 Author: Andriy Kornatskyy
 Author-email: andriy.kornatskyy@live.com
 License: MIT
-Description: # wheezy.security
-        
-        [![Build Status](https://travis-ci.org/akornatskyy/wheezy.security.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.security)
-        [![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.security/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.security?branch=master)
-        [![Documentation Status](https://readthedocs.org/projects/wheezysecurity/badge/?version=latest)](https://wheezysecurity.readthedocs.io/en/latest/?badge=latest)
-        [![pypi version](https://badge.fury.io/py/wheezy.security.svg)](https://badge.fury.io/py/wheezy.security)
-        
-        [wheezy.security](https://pypi.org/project/wheezy.security/) is a
-        [python](https://www.python.org) package written in pure Python code. It
-        is a lightweight security library that provides integration with:
-        
-        - [pycrypto](https://www.dlitz.net/software/pycrypto) - The Python
-          Cryptography Toolkit.
-        - [pycryptodome](https://www.pycryptodome.org) - PyCryptodome
-          is a fork of PyCrypto. It brings several enhancements.
-        - [pycryptodomex](https://www.pycryptodome.org) - PyCryptodomex
-          is a library independent of the PyCrypto.
-        - [cryptography](https://pypi.org/project/cryptography/) - cryptography
-          is a package which provides cryptographic recipes and primitives to
-          Python developers.
-        
-        It is optimized for performance, well tested and documented.
-        
-        Resources:
-        
-        - [source code](https://github.com/akornatskyy/wheezy.security),
-          and [issues](https://github.com/akornatskyy/wheezy.security/issues)
-          tracker are available on
-          [github](https://github.com/akornatskyy/wheezy.security)
-        - [documentation](https://wheezysecurity.readthedocs.io/en/latest/)
-        
-        ## Install
-        
-        [wheezy.security](https://pypi.org/project/wheezy.security/) requires
-        [python](https://www.python.org) version 3.6+. It is independent of operating
-        system. You can install it from
-        [pypi](https://pypi.org/project/wheezy.security/) site:
-        
-        ```sh
-        pip install -U wheezy.security
-        ```
-        
-        If you would like take benefit of one of cryptography library that has
-        built-in support specify extra requirements:
-        
-        ```sh
-        pip install wheezy.security[pycrypto]
-        pip install wheezy.security[pycryptodome]
-        pip install wheezy.security[pycryptodomex]
-        pip install wheezy.security[cryptography]
-        ```
-        
-        If you run into any issue or have comments, go ahead and add on
-        [github](https://github.com/akornatskyy/wheezy.security).
-        
 Keywords: security ticket encryption pycrypto
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# wheezy.security
+
+[![Build Status](https://travis-ci.org/akornatskyy/wheezy.security.svg?branch=master)](https://travis-ci.org/akornatskyy/wheezy.security)
+[![Coverage Status](https://coveralls.io/repos/github/akornatskyy/wheezy.security/badge.svg?branch=master)](https://coveralls.io/github/akornatskyy/wheezy.security?branch=master)
+[![Documentation Status](https://readthedocs.org/projects/wheezysecurity/badge/?version=latest)](https://wheezysecurity.readthedocs.io/en/latest/?badge=latest)
+[![pypi version](https://badge.fury.io/py/wheezy.security.svg)](https://badge.fury.io/py/wheezy.security)
+
+[wheezy.security](https://pypi.org/project/wheezy.security/) is a
+[python](https://www.python.org) package written in pure Python code. It
+is a lightweight security library that provides integration with:
+
+- [pycrypto](https://www.dlitz.net/software/pycrypto) - The Python
+  Cryptography Toolkit.
+- [pycryptodome](https://www.pycryptodome.org) - PyCryptodome
+  is a fork of PyCrypto. It brings several enhancements.
+- [pycryptodomex](https://www.pycryptodome.org) - PyCryptodomex
+  is a library independent of the PyCrypto.
+- [cryptography](https://pypi.org/project/cryptography/) - cryptography
+  is a package which provides cryptographic recipes and primitives to
+  Python developers.
+
+It is optimized for performance, well tested and documented.
+
+Resources:
+
+- [source code](https://github.com/akornatskyy/wheezy.security),
+  and [issues](https://github.com/akornatskyy/wheezy.security/issues)
+  tracker are available on
+  [github](https://github.com/akornatskyy/wheezy.security)
+- [documentation](https://wheezysecurity.readthedocs.io/en/latest/)
+
+## Install
+
+[wheezy.security](https://pypi.org/project/wheezy.security/) requires
+[python](https://www.python.org) version 3.8+. It is independent of operating
+system. You can install it from
+[pypi](https://pypi.org/project/wheezy.security/) site:
+
+```sh
+pip install -U wheezy.security
+```
+
+If you would like take benefit of one of cryptography library that has
+built-in support specify extra requirements:
+
+```sh
+pip install wheezy.security[pycrypto]
+pip install wheezy.security[pycryptodome]
+pip install wheezy.security[pycryptodomex]
+pip install wheezy.security[cryptography]
+```
+
+If you run into any issue or have comments, go ahead and add on
+[github](https://github.com/akornatskyy/wheezy.security).
```

### Comparing `wheezy.security-3.0.1/src/wheezy.security.egg-info/SOURCES.txt` & `wheezy.security-3.2.0/src/wheezy.security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

