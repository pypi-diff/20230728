# Comparing `tmp/parsetypes-0.3.1.tar.gz` & `tmp/parsetypes-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsetypes-0.3.1.tar", last modified: Fri Jun 16 23:41:07 2023, max compression
+gzip compressed data, was "parsetypes-0.3.2.tar", last modified: Fri Jul 28 16:13:26 2023, max compression
```

## Comparing `parsetypes-0.3.1.tar` & `parsetypes-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.264475 parsetypes-0.3.1/
--rw-rw-rw-   0        0        0     1548 2023-06-16 23:39:36.000000 parsetypes-0.3.1/CHANGELOG.md
--rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7436 2023-06-16 23:41:07.264475 parsetypes-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4183 2023-05-28 23:00:42.000000 parsetypes-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.249449 parsetypes-0.3.1/docs/
-drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.257476 parsetypes-0.3.1/docs/html/
--rw-rw-rw-   0        0        0     1729 2023-06-16 23:40:58.000000 parsetypes-0.3.1/docs/html/favicon.png
--rw-rw-rw-   0        0        0      141 2023-06-16 23:40:57.000000 parsetypes-0.3.1/docs/html/index.html
--rw-rw-rw-   0        0        0   593363 2023-06-16 23:40:57.000000 parsetypes-0.3.1/docs/html/parsetypes.html
--rw-rw-rw-   0        0        0   228557 2023-06-16 23:40:58.000000 parsetypes-0.3.1/docs/html/search.js
--rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:55.000000 parsetypes-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 23:41:07.264475 parsetypes-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.250452 parsetypes-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.260476 parsetypes-0.3.1/src/parsetypes/
--rw-rw-rw-   0        0        0      633 2023-06-16 23:40:42.000000 parsetypes-0.3.1/src/parsetypes/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-05-30 01:37:10.000000 parsetypes-0.3.1/src/parsetypes/_common.py
--rw-rw-rw-   0        0        0      348 2023-05-28 04:48:55.000000 parsetypes-0.3.1/src/parsetypes/_compat.py
--rw-rw-rw-   0        0        0    44629 2023-06-16 23:29:21.000000 parsetypes-0.3.1/src/parsetypes/_parser.py
--rw-rw-rw-   0        0        0     5201 2023-05-30 01:28:26.000000 parsetypes-0.3.1/src/parsetypes/_reduce_types.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.262476 parsetypes-0.3.1/src/parsetypes.egg-info/
--rw-rw-rw-   0        0        0     7436 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 23:41:07.000000 parsetypes-0.3.1/src/parsetypes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 23:41:07.263476 parsetypes-0.3.1/tests/
--rw-rw-rw-   0        0        0    71380 2023-06-16 23:35:10.000000 parsetypes-0.3.1/tests/test_parser.py
--rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:55.000000 parsetypes-0.3.1/tests/test_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:13:26.272661 parsetypes-0.3.2/
+-rw-rw-rw-   0        0        0     1589 2023-07-28 16:03:10.000000 parsetypes-0.3.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0       22 2023-05-28 02:54:36.000000 parsetypes-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5746 2023-07-28 16:13:26.271662 parsetypes-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2452 2023-07-28 16:01:02.000000 parsetypes-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 16:13:26.247664 parsetypes-0.3.2/docs/
+drwxrwxrwx   0        0        0        0 2023-07-28 16:13:26.258661 parsetypes-0.3.2/docs/html/
+-rw-rw-rw-   0        0        0     1729 2023-07-28 16:13:17.000000 parsetypes-0.3.2/docs/html/favicon.png
+-rw-rw-rw-   0        0        0      141 2023-07-28 16:13:16.000000 parsetypes-0.3.2/docs/html/index.html
+-rw-rw-rw-   0        0        0   593363 2023-07-28 16:13:16.000000 parsetypes-0.3.2/docs/html/parsetypes.html
+-rw-rw-rw-   0        0        0   228557 2023-07-28 16:13:16.000000 parsetypes-0.3.2/docs/html/search.js
+-rw-rw-rw-   0        0        0     2297 2023-05-28 04:48:56.000000 parsetypes-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 16:13:26.272661 parsetypes-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 16:13:26.248661 parsetypes-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 16:13:26.263661 parsetypes-0.3.2/src/parsetypes/
+-rw-rw-rw-   0        0        0      633 2023-07-28 16:03:35.000000 parsetypes-0.3.2/src/parsetypes/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-05-30 01:37:10.000000 parsetypes-0.3.2/src/parsetypes/_common.py
+-rw-rw-rw-   0        0        0      348 2023-05-28 04:48:56.000000 parsetypes-0.3.2/src/parsetypes/_compat.py
+-rw-rw-rw-   0        0        0    44629 2023-06-16 23:42:18.000000 parsetypes-0.3.2/src/parsetypes/_parser.py
+-rw-rw-rw-   0        0        0     5201 2023-05-30 01:28:26.000000 parsetypes-0.3.2/src/parsetypes/_reduce_types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:13:26.268661 parsetypes-0.3.2/src/parsetypes.egg-info/
+-rw-rw-rw-   0        0        0     5746 2023-07-28 16:13:26.000000 parsetypes-0.3.2/src/parsetypes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-07-28 16:13:26.000000 parsetypes-0.3.2/src/parsetypes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 16:13:26.000000 parsetypes-0.3.2/src/parsetypes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      296 2023-07-28 16:13:26.000000 parsetypes-0.3.2/src/parsetypes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 16:13:26.000000 parsetypes-0.3.2/src/parsetypes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 16:13:26.270661 parsetypes-0.3.2/tests/
+-rw-rw-rw-   0        0        0    71380 2023-06-16 23:42:18.000000 parsetypes-0.3.2/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8837 2023-05-28 04:48:56.000000 parsetypes-0.3.2/tests/test_reduce_types.py
```

### Comparing `parsetypes-0.3.1/CHANGELOG.md` & `parsetypes-0.3.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ## Changelog
 
 This project follows [PEP 440](https://peps.python.org/pep-0440/) and [Semantic Versioning (SemVer)](https://semver.org/spec/v2.0.0.html). In addition to the guarantees specified by SemVer, for versions before 1.0, this project guarantees backwards compatibility of the API for patch version updates (0.<var>y</var>.<b><var>z</var></b>).
 
 The recommended version specifier is <code>parsetypes ~= <var>x</var>.<var>y</var></code> for version 1.0 and later, and <code>parsetypes ~= <var>0</var>.<var>y</var>.<var>z</var></code> for versions prior to 1.0.
 
+### 0.3.2
+
+- Improved documentation
+
 ### 0.3.1
 
 - Added the arguments `allow_negative` and `allow_sign` (both `True` by default) to <code><var>parser</var>.parse_int()</code>, for parity with <code><var>parser</var>.is_int()</code> which already had these arguments
 
 ### 0.3
 
 - Made the previously public but undocumented instance variables of TypeParser that corresponded to the constructor arguments private instead
```

### Comparing `parsetypes-0.3.1/docs/html/favicon.png` & `parsetypes-0.3.2/docs/html/favicon.png`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/docs/html/parsetypes.html` & `parsetypes-0.3.2/docs/html/parsetypes.html`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">	- treat `inf` as either a float or a normal string</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">	- give exact Decimal values instead of floats</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">	- detect inline lists</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.3.1&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;0.3.2&quot;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">._common</span> <span class="kn">import</span> <span class="n">AnyScalar</span><span class="p">,</span> <span class="n">AnyScalarType</span><span class="p">,</span> <span class="n">AnyValue</span><span class="p">,</span> <span class="n">AnyValueType</span><span class="p">,</span> <span class="n">GenericValue</span><span class="p">,</span> <span class="n">Nullable</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">._parser</span> <span class="kn">import</span> <span class="n">TypeParser</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">._reduce_types</span> <span class="kn">import</span> <span class="n">reduce_types</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">(</span><span class="s1">&#39;TypeParser&#39;</span><span class="p">,</span> <span class="s1">&#39;reduce_types&#39;</span><span class="p">,</span> <span class="s1">&#39;Nullable&#39;</span><span class="p">)</span>
 </span></pre></div>
```

#### html2text {}

```diff
@@ -48,15 +48,15 @@
 _6
 - give exact Decimal values instead of floats
 _7
 - detect inline lists
 _8"""
 _9
 10
-11__version__ = "0.3.1"
+11__version__ = "0.3.2"
 12
 13from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType,
 GenericValue, Nullable
 14from ._parser import TypeParser
 15from ._reduce_types import reduce_types
 16
 17__all__ = ('TypeParser', 'reduce_types', 'Nullable')
```

### Comparing `parsetypes-0.3.1/docs/html/search.js` & `parsetypes-0.3.2/docs/html/search.js`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/pyproject.toml` & `parsetypes-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/src/parsetypes/__init__.py` & `parsetypes-0.3.2/src/parsetypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 	The `TypeParser` class provides configurable type inference and parsing. This can be initialised with different settings to, for example:
 	- treat `inf` as either a float or a normal string
 	- give exact Decimal values instead of floats
 	- detect inline lists
 """
 
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 from ._common import AnyScalar, AnyScalarType, AnyValue, AnyValueType, GenericValue, Nullable
 from ._parser import TypeParser
 from ._reduce_types import reduce_types
 
 __all__ = ('TypeParser', 'reduce_types', 'Nullable')
```

### Comparing `parsetypes-0.3.1/src/parsetypes/_common.py` & `parsetypes-0.3.2/src/parsetypes/_common.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/src/parsetypes/_parser.py` & `parsetypes-0.3.2/src/parsetypes/_parser.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/src/parsetypes/_reduce_types.py` & `parsetypes-0.3.2/src/parsetypes/_reduce_types.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/src/parsetypes.egg-info/SOURCES.txt` & `parsetypes-0.3.2/src/parsetypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/tests/test_parser.py` & `parsetypes-0.3.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `parsetypes-0.3.1/tests/test_reduce_types.py` & `parsetypes-0.3.2/tests/test_reduce_types.py`

 * *Files identical despite different names*

