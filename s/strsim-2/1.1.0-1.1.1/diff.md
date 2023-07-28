# Comparing `tmp/strsim_2-1.1.0.tar.gz` & `tmp/strsim_2-1.1.1.tar.gz`

## Comparing `strsim_2-1.1.0.tar` & `strsim_2-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 strsim_2-1.1.0/Cargo.toml
--rw-r--r--   0     1001      123     3271 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.github/workflows/build.sh
--rw-r--r--   0     1001      123     3060 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      123     2641 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.github/workflows/pydiscovery.py
--rw-r--r--   0     1001      123      575 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.gitignore
--rw-r--r--   0     1001      123     1064 2023-07-18 17:29:19.000000 strsim_2-1.1.0/LICENSE
--rw-r--r--   0     1001      123       54 2023-07-18 17:29:19.000000 strsim_2-1.1.0/README.md
--rw-r--r--   0     1001      123       10 2023-07-18 17:29:54.000000 strsim_2-1.1.0/dist/strsim_2-1.1.0.tar.gz
--rw-r--r--   0     1001      123      709 2023-07-18 17:29:19.000000 strsim_2-1.1.0/pyproject.toml
--rw-r--r--   0     1001      123     1301 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/error.rs
--rw-r--r--   0     1001      123      275 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/helper.rs
--rw-r--r--   0     1001      123     4752 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/hybrid_jaccard.rs
--rw-r--r--   0     1001      123     2533 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/jaro.rs
--rw-r--r--   0     1001      123     2154 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/jaro_winkler.rs
--rw-r--r--   0     1001      123     6878 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/levenshtein.rs
--rw-r--r--   0     1001      123     5145 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/lib.rs
--rw-r--r--   0     1001      123     3779 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/monge_elkan.rs
--rw-r--r--   0     1001      123     2840 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/python.rs
--rw-r--r--   0     1001      123     6454 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/tokenizers.rs
--rw-r--r--   0     1001      123      115 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/wrapped_strsim/mod.rs
--rw-r--r--   0     1001      123     2502 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/wrapped_strsim/seq_strsim.rs
--rw-r--r--   0     1001      123     2554 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/wrapped_strsim/set_strsim.rs
--rw-r--r--   0     1001      123      161 2023-07-18 17:29:19.000000 strsim_2-1.1.0/strsim/__init__.py
--rw-r--r--   0     1001      123      798 2023-07-18 17:29:19.000000 strsim_2-1.1.0/strsim/__init__.pyi
--rw-r--r--   0     1001      123        0 2023-07-18 17:29:19.000000 strsim_2-1.1.0/strsim/py.typed
--rw-r--r--   0     1001      123        0 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/__init__.py
--rw-r--r--   0     1001      123      929 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/common/mod.rs
--rw-r--r--   0     1001      123      967 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/hybrid_jaccard.rs
--rw-r--r--   0     1001      123      977 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/jaro.rs
--rw-r--r--   0     1001      123     1527 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/jaro_winkler.rs
--rw-r--r--   0     1001      123     1781 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/levenshtein.rs
--rw-r--r--   0     1001      123     1167 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/monge_elkan.rs
--rw-r--r--   0     1001      123      554 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/resources/rltk_check.py
--rw-r--r--   0     1001      123    10981 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/resources/strsim_check.ipynb
--rw-r--r--   0     1001      123     1944 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/resources/test_linear_sum_assignment.ipynb
--rw-r--r--   0     1001      123      896 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/test_python.py
--rw-r--r--   0     1001      123    11543 2023-07-18 17:29:21.000000 strsim_2-1.1.0/Cargo.lock
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 strsim_2-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 strsim_2-1.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     3271 2023-07-28 03:00:52.000000 strsim_2-1.1.1/.github/workflows/build.sh
+-rw-r--r--   0     1001      123     3393 2023-07-28 03:00:52.000000 strsim_2-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     2641 2023-07-28 03:00:52.000000 strsim_2-1.1.1/.github/workflows/pydiscovery.py
+-rw-r--r--   0     1001      123      575 2023-07-28 03:00:52.000000 strsim_2-1.1.1/.gitignore
+-rw-r--r--   0     1001      123     1064 2023-07-28 03:00:52.000000 strsim_2-1.1.1/LICENSE
+-rw-r--r--   0     1001      123       54 2023-07-28 03:00:52.000000 strsim_2-1.1.1/README.md
+-rw-r--r--   0     1001      123       10 2023-07-28 03:01:22.000000 strsim_2-1.1.1/dist/strsim_2-1.1.1.tar.gz
+-rw-r--r--   0     1001      123      726 2023-07-28 03:00:52.000000 strsim_2-1.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     1301 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/error.rs
+-rw-r--r--   0     1001      123      275 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/helper.rs
+-rw-r--r--   0     1001      123     4752 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/hybrid_jaccard.rs
+-rw-r--r--   0     1001      123     2533 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/jaro.rs
+-rw-r--r--   0     1001      123     2154 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/jaro_winkler.rs
+-rw-r--r--   0     1001      123     6878 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/levenshtein.rs
+-rw-r--r--   0     1001      123     5145 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     3779 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/monge_elkan.rs
+-rw-r--r--   0     1001      123     2840 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/python.rs
+-rw-r--r--   0     1001      123     6454 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/tokenizers.rs
+-rw-r--r--   0     1001      123      115 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/wrapped_strsim/mod.rs
+-rw-r--r--   0     1001      123     2502 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/wrapped_strsim/seq_strsim.rs
+-rw-r--r--   0     1001      123     2554 2023-07-28 03:00:52.000000 strsim_2-1.1.1/src/wrapped_strsim/set_strsim.rs
+-rw-r--r--   0     1001      123      161 2023-07-28 03:00:52.000000 strsim_2-1.1.1/strsim/__init__.py
+-rw-r--r--   0     1001      123      798 2023-07-28 03:00:52.000000 strsim_2-1.1.1/strsim/__init__.pyi
+-rw-r--r--   0     1001      123        0 2023-07-28 03:00:52.000000 strsim_2-1.1.1/strsim/py.typed
+-rw-r--r--   0     1001      123        0 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/__init__.py
+-rw-r--r--   0     1001      123      929 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/common/mod.rs
+-rw-r--r--   0     1001      123      967 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/hybrid_jaccard.rs
+-rw-r--r--   0     1001      123      977 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/jaro.rs
+-rw-r--r--   0     1001      123     1527 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/jaro_winkler.rs
+-rw-r--r--   0     1001      123     1781 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/levenshtein.rs
+-rw-r--r--   0     1001      123     1167 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/monge_elkan.rs
+-rw-r--r--   0     1001      123      554 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/resources/rltk_check.py
+-rw-r--r--   0     1001      123    10981 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/resources/strsim_check.ipynb
+-rw-r--r--   0     1001      123     1944 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/resources/test_linear_sum_assignment.ipynb
+-rw-r--r--   0     1001      123      896 2023-07-28 03:00:52.000000 strsim_2-1.1.1/tests/test_python.py
+-rw-r--r--   0     1001      123    11544 2023-07-28 03:00:54.000000 strsim_2-1.1.1/Cargo.lock
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 strsim_2-1.1.1/PKG-INFO
```

### Comparing `strsim_2-1.1.0/Cargo.toml` & `strsim_2-1.1.1/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "yass-2"
-version = "1.1.0"
+version = "1.1.1"
 edition = "2021"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/strsim"
 repository = "https://github.com/binh-vu/strsim"
 license-file = "LICENSE"
 description = "Yet another string similarity library"
 keywords = ["string-similarity", "strsim", "levenshtein", "jaro-winkler"]
@@ -25,8 +25,7 @@
 
 [dev-dependencies]
 approx = "0.5.1"
 maplit = "1.0.2"
 
 [features]
 extension-module = ["pyo3/extension-module"]
-default = ["extension-module"]
```

### Comparing `strsim_2-1.1.0/.github/workflows/build.sh` & `strsim_2-1.1.1/.github/workflows/build.sh`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/.github/workflows/ci.yml` & `strsim_2-1.1.1/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,38 @@
   pull_request:
 
 jobs:
   build:
     strategy:
       matrix:
         python: ["3.8", "3.9", "3.10", "3.11"]
-        platform: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        # python: ["3.8"]
-        # platform: ["ubuntu-latest"]
+        platform: ["ubuntu-22.04", "macos-12", "windows-2022"]
     runs-on: ${{ matrix.platform }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
+      - name: Cache Rust target directory
+        uses: actions/cache@v3
+        with:
+          key: ${{ runner.os }}
+          path: |
+            ~/.cargo  
+            target
       - name: Run test
         if: matrix.python == '3.8'
         run: cargo test --no-default-features --features pyo3/auto-initialize
       - uses: messense/maturin-action@v1
+        env:
+          MACOSX_DEPLOYMENT_TARGET: 10.14
         with:
           command: build
-          args: --release ${{ startsWith(matrix.platform, 'ubuntu') && startsWith(matrix.python, '3.8') && '--sdist' || '' }} -o dist -i python ${{ startsWith(matrix.platform, 'macos') && '--universal2' || '' }}
+          args: --release ${{ startsWith(matrix.platform, 'ubuntu') && startsWith(matrix.python, '3.8') && '--sdist' || '' }} -o dist -i python ${{ startsWith(matrix.platform, 'macos') && '--target universal2-apple-darwin' || '' }}
       - name: Run test
         if: matrix.python == '3.8' && !startsWith(matrix.platform, 'windows')
         run: |
           python -c "import subprocess, glob, os; file = glob.glob(os.path.join('dist', '*cp38*.whl'))[0]; subprocess.check_output(['pip', 'install', file])"
           pip install pytest
           mv strsim strsim2
           pytest -xs tests/
@@ -39,14 +46,19 @@
           name: wheels
           path: dist
 
   build-manylinux:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
+      - name: Cache Rust target directory
+        uses: actions/cache@v3
+        with:
+          key: ${{ runner.os }}-manylinux
+          path: target
       - name: Build wheels
         run: |
           docker run --rm -w /project -v $(pwd):/project \
             -e EXTRA_PATH=/opt/python/cp38-cp38/bin \
             -e PYTHON_HOMES=/opt/python \
             -e CARGO_NET_GIT_FETCH_WITH_CLI=false \
             quay.io/pypa/manylinux2014_x86_64:latest \
@@ -55,29 +67,29 @@
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   release-crate:
     name: Release Crates.io
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
     if: startsWith(github.ref, 'refs/tags/') || startsWith(github.ref, 'refs/heads/master') || startsWith(github.ref, 'refs/heads/dev-ci')
     needs: [build, build-manylinux]
     steps:
       - uses: actions/checkout@v3
       - name: Publish to Crates
         env:
           CARGO_REGISTRY_TOKEN: ${{ secrets.CRATES_TOKEN }}
         run: |
           cargo publish --dry-run
           cargo publish --no-verify || echo 'crate is already published'
 
   release-pypi:
     name: Release PyPI.org
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
     if: startsWith(github.ref, 'refs/tags/') || startsWith(github.ref, 'refs/heads/master') || startsWith(github.ref, 'refs/heads/dev-ci')
     needs: [build, build-manylinux]
     steps:
       - uses: actions/download-artifact@v2
         with:
           name: wheels
       - name: Publish to PyPI
```

### Comparing `strsim_2-1.1.0/.github/workflows/pydiscovery.py` & `strsim_2-1.1.1/.github/workflows/pydiscovery.py`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/.gitignore` & `strsim_2-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/LICENSE` & `strsim_2-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/pyproject.toml` & `strsim_2-1.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 [project]
 name = "strsim-2"
-version = "1.1.0"
+version = "1.1.1"
 description = "Yet another string similarity library (implemented in Rust)"
 readme = "README.md"
-authors = [
-    { name = "Binh Vu", email = "binh@toan2.com" },
-]
+authors = [{ name = "Binh Vu", email = "binh@toan2.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 requires-python = ">=3.8"
@@ -17,17 +15,16 @@
 dependencies = []
 
 [project.urls]
 homepage = "https://github.com/binh-vu/strsim"
 repository = "https://github.com/binh-vu/strsim"
 
 [project.optional-dependencies]
-dev = [
-    'pytest >= 7.1.3, < 8.0.0',
-]
+dev = ['pytest >= 7.1.3, < 8.0.0']
 
 [tool.maturin]
 module-name = "strsim"
+features = ["extension-module"]
 
 [build-system]
-requires = ["maturin>=0.15,<0.16"]
-build-backend = "maturin"
+requires = ["maturin>=1.0,<2.0"]
+build-backend = "maturin"
```

### Comparing `strsim_2-1.1.0/src/error.rs` & `strsim_2-1.1.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/hybrid_jaccard.rs` & `strsim_2-1.1.1/src/hybrid_jaccard.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/jaro.rs` & `strsim_2-1.1.1/src/jaro.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/jaro_winkler.rs` & `strsim_2-1.1.1/src/jaro_winkler.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/levenshtein.rs` & `strsim_2-1.1.1/src/levenshtein.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/lib.rs` & `strsim_2-1.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/monge_elkan.rs` & `strsim_2-1.1.1/src/monge_elkan.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/python.rs` & `strsim_2-1.1.1/src/python.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/tokenizers.rs` & `strsim_2-1.1.1/src/tokenizers.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/wrapped_strsim/seq_strsim.rs` & `strsim_2-1.1.1/src/wrapped_strsim/seq_strsim.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/src/wrapped_strsim/set_strsim.rs` & `strsim_2-1.1.1/src/wrapped_strsim/set_strsim.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/strsim/__init__.pyi` & `strsim_2-1.1.1/strsim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/common/mod.rs` & `strsim_2-1.1.1/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/hybrid_jaccard.rs` & `strsim_2-1.1.1/tests/hybrid_jaccard.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/jaro.rs` & `strsim_2-1.1.1/tests/jaro.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/jaro_winkler.rs` & `strsim_2-1.1.1/tests/jaro_winkler.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/levenshtein.rs` & `strsim_2-1.1.1/tests/levenshtein.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/monge_elkan.rs` & `strsim_2-1.1.1/tests/monge_elkan.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/resources/rltk_check.py` & `strsim_2-1.1.1/tests/resources/rltk_check.py`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/resources/strsim_check.ipynb` & `strsim_2-1.1.1/tests/resources/strsim_check.ipynb`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/resources/test_linear_sum_assignment.ipynb` & `strsim_2-1.1.1/tests/resources/test_linear_sum_assignment.ipynb`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/tests/test_python.py` & `strsim_2-1.1.1/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `strsim_2-1.1.0/Cargo.lock` & `strsim_2-1.1.1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -63,17 +63,17 @@
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "hashbrown"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
@@ -84,17 +84,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inventory"
-version = "0.3.9"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25b1d6b4b9fb75fc419bdef998b689df5080a32931cb3395b86202046b56a9ea"
+checksum = "a53088c87cf71c9d4f3372a2cb9eea1e7b8a0b1bf8b7f7d23fe5b76dbb07e63b"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
@@ -139,17 +139,17 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
@@ -248,17 +248,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.31"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
@@ -304,47 +304,47 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.26"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
@@ -416,15 +416,15 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "yass-2"
-version = "1.1.0"
+version = "1.1.1"
 dependencies = [
  "anyhow",
  "approx",
  "derive_more",
  "hashbrown",
  "itertools",
  "lsap",
```

### Comparing `strsim_2-1.1.0/PKG-INFO` & `strsim_2-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strsim-2
-Version: 1.1.0
+Version: 1.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 License-File: LICENSE
 Summary: Yet another string similarity library (implemented in Rust)
```

