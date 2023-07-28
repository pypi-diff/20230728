# Comparing `tmp/chikpos-1.0.11.tar.gz` & `tmp/chikpos-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chikpos-1.0.11.tar", last modified: Sat Jul  8 04:27:00 2023, max compression
+gzip compressed data, was "chikpos-2.0.0rc1.tar", last modified: Fri Jul 28 01:48:03 2023, max compression
```

## Comparing `chikpos-1.0.11.tar` & `chikpos-2.0.0rc1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.515553 chikpos-1.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-08 04:26:51.000000 chikpos-1.0.11/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-08 04:26:51.000000 chikpos-1.0.11/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-08 04:26:51.000000 chikpos-1.0.11/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.491553 chikpos-1.0.11/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.495553 chikpos-1.0.11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-08 04:26:51.000000 chikpos-1.0.11/.github/workflows/build-test-cplusplus.yml.bak
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-08 04:26:51.000000 chikpos-1.0.11/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-08 04:26:51.000000 chikpos-1.0.11/.github/workflows/doc-html-pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-08 04:26:51.000000 chikpos-1.0.11/.github/workflows/manual-plot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-08 04:26:51.000000 chikpos-1.0.11/.github/workflows/plot-k27-no-bitfield.yaml.bak
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-08 04:26:51.000000 chikpos-1.0.11/.github/workflows/plot-k27.yaml.bak
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-08 04:26:51.000000 chikpos-1.0.11/.github/workflows/stale-issue.yml.bak
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-08 04:26:51.000000 chikpos-1.0.11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-08 04:26:51.000000 chikpos-1.0.11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-08 04:26:51.000000 chikpos-1.0.11/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 04:26:51.000000 chikpos-1.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-08 04:27:00.515553 chikpos-1.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-08 04:26:51.000000 chikpos-1.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.495553 chikpos-1.0.11/chikpos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-08 04:27:00.000000 chikpos-1.0.11/chikpos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-08 04:27:00.000000 chikpos-1.0.11/chikpos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 04:27:00.000000 chikpos-1.0.11/chikpos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 04:27:00.000000 chikpos-1.0.11/chikpos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 04:27:00.000000 chikpos-1.0.11/chikpos.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-07-08 04:26:51.000000 chikpos-1.0.11/docker-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-08 04:26:51.000000 chikpos-1.0.11/docker-test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.499553 chikpos-1.0.11/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/bucket_graph.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/code_documentation.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.499553 chikpos-1.0.11/documents/images/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/images/aesctr.png
--rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/images/beyondhellman.png
--rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/images/beyondhellman2.png
--rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/images/pointerformat.png
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/images/proofofspace.png
--rw-r--r--   0 runner    (1001) docker     (123)  1368329 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/proof_of_space.html
--rw-r--r--   0 runner    (1001) docker     (123)    75274 2023-07-08 04:26:51.000000 chikpos-1.0.11/documents/proof_of_space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/hellman_example/
--rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/Hellman attacks.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/aes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/cxxopts.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/hellman.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/sort_on_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-08 04:26:51.000000 chikpos-1.0.11/hellman_example/verifier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-08 04:26:51.000000 chikpos-1.0.11/lgtm.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.491553 chikpos-1.0.11/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/lib/FiniteStateEntropy/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.491553 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/FSE/
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/libfse/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/lib/FiniteStateEntropy/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.503553 chikpos-1.0.11/lib/FiniteStateEntropy/lib/Archives/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/Archives/hufx6.h
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/error_public.h
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/fseU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/fseU16.h
--rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/lib/mem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.507553 chikpos-1.0.11/lib/FiniteStateEntropy/programs/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/bench.c
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/bench.h
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/commandline.c
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fileio.c
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fileio.h
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fseDist.c
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fseDist.h
--rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fullbench.c
--rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/fuzzerU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/probaGenerator.c
--rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/zlibh.c
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/FiniteStateEntropy/programs/zlibh.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.507553 chikpos-1.0.11/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-08 04:26:51.000000 chikpos-1.0.11/lib/include/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 04:26:51.000000 chikpos-1.0.11/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-08 04:26:51.000000 chikpos-1.0.11/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.507553 chikpos-1.0.11/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-08 04:26:51.000000 chikpos-1.0.11/python-bindings/chikpos.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 04:27:00.515553 chikpos-1.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-08 04:26:51.000000 chikpos-1.0.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.511553 chikpos-1.0.11/src/
--rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b17phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b17phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b17phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b17sort_manager.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.511553 chikpos-1.0.11/src/b3/
--rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3.c
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3.h
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_avx2_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_avx512.c
--rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_avx512_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_dispatch.c
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_portable.c
--rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_sse41.c
--rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/b3/blake3_sse41_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/bitfield.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/bitfield_index.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/chacha8.c
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/chacha8.h
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/chik_filesystem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/entry_sizes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/exceptions.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/phase1.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/phases.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/progress.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/quicksort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/serialize.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/sort_manager.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/threading.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/uniformsort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-08 04:26:51.000000 chikpos-1.0.11/src/verifier.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.515553 chikpos-1.0.11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 04:26:51.000000 chikpos-1.0.11/tests/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:26:51.000000 chikpos-1.0.11/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-08 04:26:51.000000 chikpos-1.0.11/tests/plot-resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-08 04:26:51.000000 chikpos-1.0.11/tests/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-08 04:26:51.000000 chikpos-1.0.11/tests/test_python_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.515553 chikpos-1.0.11/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-08 04:26:51.000000 chikpos-1.0.11/tools/disk.gnuplot
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-08 04:26:51.000000 chikpos-1.0.11/tools/parse_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:00.515553 chikpos-1.0.11/uint128_t/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/endianness.h
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/uint128_t.build
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/uint128_t.h
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/uint128_t.include
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-08 04:26:51.000000 chikpos-1.0.11/uint128_t/uint128_t_config.include
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.092670 chikpos-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.068669 chikpos-2.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.072669 chikpos-2.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.github/workflows/build-test-cplusplus.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.github/workflows/doc-html-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.github/workflows/manual-plot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.github/workflows/plot-k27-no-bitfield.yaml.bak
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.github/workflows/plot-k27.yaml.bak
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.github/workflows/stale-issue.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-28 01:48:03.092670 chikpos-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.072669 chikpos-2.0.0rc1/chikpos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-28 01:48:03.000000 chikpos-2.0.0rc1/chikpos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-28 01:48:03.000000 chikpos-2.0.0rc1/chikpos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:48:03.000000 chikpos-2.0.0rc1/chikpos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:48:02.000000 chikpos-2.0.0rc1/chikpos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 01:48:03.000000 chikpos-2.0.0rc1/chikpos.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/docker-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/docker-test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.076670 chikpos-2.0.0rc1/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/bucket_graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/code_documentation.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.076670 chikpos-2.0.0rc1/documents/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/images/aesctr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/images/beyondhellman.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/images/beyondhellman2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/images/pointerformat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/images/proofofspace.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1368329 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/proof_of_space.html
+-rw-r--r--   0 runner    (1001) docker     (123)    75274 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/documents/proof_of_space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.080669 chikpos-2.0.0rc1/hellman_example/
+-rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/Hellman attacks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/aes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/cxxopts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/hellman.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/sort_on_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/hellman_example/verifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lgtm.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.068669 chikpos-2.0.0rc1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.080669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.068669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.080669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.080669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.080669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.080669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.084669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.084669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_public.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.084669 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/commandline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fullbench.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/probaGenerator.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.084669 chikpos-2.0.0rc1/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/lib/include/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.084669 chikpos-2.0.0rc1/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/python-bindings/chikpos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:48:03.092670 chikpos-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.088670 chikpos-2.0.0rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b17phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b17phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b17phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b17sort_manager.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.092670 chikpos-2.0.0rc1/src/b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_avx2_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_avx512.c
+-rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_avx512_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_dispatch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_portable.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_sse41.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/b3/blake3_sse41_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/bitfield.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/bitfield_index.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/chacha8.c
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/chacha8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/chik_filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/entry_sizes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/phase1.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/phases.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/progress.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49706 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/quicksort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/serialize.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/sort_manager.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/threading.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/uniformsort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/src/verifier.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.092670 chikpos-2.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/tests/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/tests/plot-resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/tests/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/tests/test_python_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.092670 chikpos-2.0.0rc1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/tools/disk.gnuplot
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/tools/parse_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:03.092670 chikpos-2.0.0rc1/uint128_t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/endianness.h
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/uint128_t.build
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/uint128_t.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/uint128_t.include
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 01:47:53.000000 chikpos-2.0.0rc1/uint128_t/uint128_t_config.include
```

### Comparing `chikpos-1.0.11/.github/workflows/build-test-cplusplus.yml.bak` & `chikpos-2.0.0rc1/.github/workflows/build-test-cplusplus.yml.bak`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/.github/workflows/build-wheels.yml` & `chikpos-2.0.0rc1/.github/workflows/build-wheels.yml`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/.github/workflows/doc-html-pdf.yml` & `chikpos-2.0.0rc1/.github/workflows/doc-html-pdf.yml`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/.github/workflows/manual-plot.yml` & `chikpos-2.0.0rc1/.github/workflows/manual-plot.yml`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/.github/workflows/plot-k27-no-bitfield.yaml.bak` & `chikpos-2.0.0rc1/.github/workflows/plot-k27-no-bitfield.yaml.bak`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/.github/workflows/plot-k27.yaml.bak` & `chikpos-2.0.0rc1/.github/workflows/plot-k27.yaml.bak`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/.github/workflows/stale-issue.yml.bak` & `chikpos-2.0.0rc1/.github/workflows/stale-issue.yml.bak`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/CMakeLists.txt` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,53 +12,40 @@
 endif()
 
 project(chikpos C CXX ASM)
 
 # CMake 3.14+
 include(FetchContent)
 
-if (${CMAKE_SYSTEM_NAME} MATCHES "FreeBSD")
-include(${CMAKE_INSTALL_PREFIX}/share/cmake/pybind11/pybind11Config.cmake)
-else()
 FetchContent_Declare(
   pybind11-src
   GIT_REPOSITORY https://github.com/pybind/pybind11.git
-  GIT_TAG        v2.10.0
+  GIT_TAG        v2.6.2
 )
 FetchContent_MakeAvailable(pybind11-src)
-endif()
-
-FetchContent_Declare(
-  cxxopts
-  GIT_REPOSITORY https://github.com/jarro2783/cxxopts.git
-  GIT_TAG        v2.2.1
-)
-FetchContent_MakeAvailable(cxxopts)
 
 FetchContent_Declare(
-  gulrak
-  GIT_REPOSITORY https://github.com/gulrak/filesystem.git
-  GIT_TAG        v1.5.6
+  fse
+  GIT_REPOSITORY https://github.com/Cyan4973/FiniteStateEntropy.git
+  GIT_TAG        510d22b221c8c02f281c35f9edeb606baacef27b
 )
-FetchContent_MakeAvailable(gulrak)
+FetchContent_MakeAvailable(fse)
 
-set(FSE_LIB ${CMAKE_CURRENT_SOURCE_DIR}/lib/FiniteStateEntropy/lib)
+set(FSE_LIB ${fse_SOURCE_DIR}/lib)
 set(FSE_FILES
     ${FSE_LIB}/fse_compress.c
     ${FSE_LIB}/fse_decompress.c
     ${FSE_LIB}/entropy_common.c
     ${FSE_LIB}/hist.c
 )
 
 include_directories(
   ${INCLUDE_DIRECTORIES}
   ${CMAKE_CURRENT_SOURCE_DIR}/../lib/include
-  ${cxxopts_SOURCE_DIR}/include
-  ${gulrak_SOURCE_DIR}/include/ghc
-  ${CMAKE_CURRENT_SOURCE_DIR}/../lib/FiniteStateEntropy/lib
+  ${FSE_LIB}
   ${CMAKE_CURRENT_SOURCE_DIR}/src
   ${CMAKE_CURRENT_SOURCE_DIR}/test
   )
 
 add_library(fse ${FSE_FILES})
 
 IF (MSVC)
@@ -84,22 +71,22 @@
 
 set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -g")
 set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -g")
 
 ENDIF()
 
 IF (CMAKE_BUILD_TYPE STREQUAL "ASAN")
-set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O1 -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
-set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -O1 -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
+set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
+set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
 set (CMAKE_LINKER_FLAGS "${CMAKE_LINKER_FLAGS} -fno-omit-frame-pointer -fsanitize=address -fsanitize=undefined")
 ENDIF()
 
 IF (CMAKE_BUILD_TYPE STREQUAL "TSAN")
-set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O2 -fno-omit-frame-pointer -fsanitize=thread")
-set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -O2 -fno-omit-frame-pointer -fsanitize=thread")
+set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fno-omit-frame-pointer -fsanitize=thread")
+set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fno-omit-frame-pointer -fsanitize=thread")
 set (CMAKE_LINKER_FLAGS "${CMAKE_LINKER_FLAGS} -fno-omit-frame-pointer -fsanitize=thread")
 ENDIF()
 
 IF (APPLE)
 # on macOS "uname -m" returns the architecture (x86_64 or arm64)
 execute_process(
     COMMAND uname -m
@@ -138,63 +125,47 @@
 
 add_executable(ProofOfSpace
     src/cli.cpp
     src/chacha8.c
     ${BLAKE3_SRC}
 )
 
-option(BUILD_PROOF_OF_SPACE_STATICALLY "Build ProofOfSpace target statically" OFF)
-IF (BUILD_PROOF_OF_SPACE_STATICALLY)
-  message("Statically build ProofOfSpace")
-  target_link_libraries(ProofOfSpace -static -Wl,--whole-archive -lrt -lpthread -Wl,--no-whole-archive)
-ENDIF()
-
-FetchContent_Declare(
-  Catch2
-  GIT_REPOSITORY https://github.com/catchorg/Catch2.git
-  GIT_TAG        v3.3.2
-)
-FetchContent_MakeAvailable(Catch2)
-
 add_executable(RunTests
+    tests/test-main.cpp
     tests/test.cpp
     src/chacha8.c
     ${BLAKE3_SRC}
 )
 
-target_link_libraries(RunTests
-  PRIVATE
-    fse
-    Threads::Threads
-    Catch2::Catch2
-)
-
 find_package(Threads REQUIRED)
 
 add_library(uint128 STATIC uint128_t/uint128_t.cpp)
 target_include_directories(uint128 PUBLIC uint128_t)
 
 target_compile_features(fse PUBLIC cxx_std_17)
 target_compile_features(chikpos PUBLIC cxx_std_17)
 target_compile_features(RunTests PUBLIC cxx_std_17)
 
 if (${CMAKE_SYSTEM_NAME} MATCHES "Darwin")
   target_link_libraries(chikpos PRIVATE fse Threads::Threads)
   target_link_libraries(ProofOfSpace fse Threads::Threads)
+  target_link_libraries(RunTests fse Threads::Threads)
 elseif (${CMAKE_SYSTEM_NAME} MATCHES "OpenBSD")
   target_link_libraries(chikpos PRIVATE fse Threads::Threads)
   target_link_libraries(ProofOfSpace fse Threads::Threads)
+  target_link_libraries(RunTests fse Threads::Threads)
 elseif (${CMAKE_SYSTEM_NAME} MATCHES "FreeBSD")
   target_link_libraries(chikpos PRIVATE fse Threads::Threads)
   target_link_libraries(ProofOfSpace fse Threads::Threads)
+  target_link_libraries(RunTests fse Threads::Threads)
 elseif (MSVC)
   target_link_libraries(chikpos PRIVATE fse Threads::Threads uint128)
   target_link_libraries(ProofOfSpace fse Threads::Threads uint128)
-  target_link_libraries(RunTests PRIVATE uint128)
+  target_link_libraries(RunTests fse Threads::Threads uint128)
 else()
   target_link_libraries(chikpos PRIVATE fse stdc++fs Threads::Threads)
   target_link_libraries(ProofOfSpace fse stdc++fs Threads::Threads)
-  target_link_libraries(RunTests PRIVATE stdc++fs)
+  target_link_libraries(RunTests fse stdc++fs Threads::Threads)
 endif()
 
 enable_testing()
 add_test(NAME RunTests COMMAND RunTests)
```

### Comparing `chikpos-1.0.11/Dockerfile` & `chikpos-2.0.0rc1/Dockerfile`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/LICENSE` & `chikpos-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/PKG-INFO` & `chikpos-2.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chikpos
-Version: 1.0.11
+Version: 2.0.0rc1
 Summary: Chik proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chik-Network/chikpos
 Author: Mariano Sorgente
 Author-email: mariano@chiknetwork.com
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chikpos-1.0.11/README.md` & `chikpos-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/chikpos.egg-info/PKG-INFO` & `chikpos-2.0.0rc1/chikpos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chikpos
-Version: 1.0.11
+Version: 2.0.0rc1
 Summary: Chik proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chik-Network/chikpos
 Author: Mariano Sorgente
 Author-email: mariano@chiknetwork.com
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chikpos-1.0.11/chikpos.egg-info/SOURCES.txt` & `chikpos-2.0.0rc1/chikpos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/bucket_graph.pdf` & `chikpos-2.0.0rc1/documents/bucket_graph.pdf`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/code_documentation.pdf` & `chikpos-2.0.0rc1/documents/code_documentation.pdf`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/images/aesctr.png` & `chikpos-2.0.0rc1/documents/images/aesctr.png`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/images/beyondhellman.png` & `chikpos-2.0.0rc1/documents/images/beyondhellman.png`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/images/beyondhellman2.png` & `chikpos-2.0.0rc1/documents/images/beyondhellman2.png`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/images/pointerformat.png` & `chikpos-2.0.0rc1/documents/images/pointerformat.png`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/images/proofofspace.png` & `chikpos-2.0.0rc1/documents/images/proofofspace.png`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/proof_of_space.html` & `chikpos-2.0.0rc1/documents/proof_of_space.html`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/documents/proof_of_space.md` & `chikpos-2.0.0rc1/documents/proof_of_space.md`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/Hellman attacks.pdf` & `chikpos-2.0.0rc1/hellman_example/Hellman attacks.pdf`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/aes.hpp` & `chikpos-2.0.0rc1/hellman_example/aes.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/bits.hpp` & `chikpos-2.0.0rc1/hellman_example/bits.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/calculate_bucket.hpp` & `chikpos-2.0.0rc1/hellman_example/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/cli.cpp` & `chikpos-2.0.0rc1/hellman_example/cli.cpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/cxxopts.hpp` & `chikpos-2.0.0rc1/hellman_example/cxxopts.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/encoding.hpp` & `chikpos-2.0.0rc1/hellman_example/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/hellman.hpp` & `chikpos-2.0.0rc1/hellman_example/hellman.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/picosha2.hpp` & `chikpos-2.0.0rc1/hellman_example/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/plotter_disk.hpp` & `chikpos-2.0.0rc1/hellman_example/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/pos_constants.hpp` & `chikpos-2.0.0rc1/hellman_example/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/prover_disk.hpp` & `chikpos-2.0.0rc1/hellman_example/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/sort_on_disk.hpp` & `chikpos-2.0.0rc1/hellman_example/sort_on_disk.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/util.hpp` & `chikpos-2.0.0rc1/hellman_example/util.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/hellman_example/verifier.hpp` & `chikpos-2.0.0rc1/hellman_example/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/LICENSE` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/LICENSE`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/README.md` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/README.md`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/Archives/hufx6.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/README.md` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/README.md`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/bitstream.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/bitstream.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/compiler.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/compiler.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/debug.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/debug.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/entropy_common.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/entropy_common.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/error_private.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_private.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/error_public.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_public.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/fse.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/fseU16.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/fseU16.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/fse_compress.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_compress.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/fse_decompress.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/hist.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/hist.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/huf.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/huf_compress.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_compress.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/huf_decompress.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/lib/mem.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/lib/mem.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/COPYING` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/COPYING`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/bench.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/bench.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/commandline.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/commandline.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/cpu.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/cpu.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fileio.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fileio.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fseDist.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fseDist.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fullbench.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fullbench.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fuzzer.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzer.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fuzzerHuff0.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerHuff0.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/fuzzerU16.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerU16.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/probaGenerator.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/probaGenerator.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/xxhash.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/xxhash.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/zlibh.c` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/FiniteStateEntropy/programs/zlibh.h` & `chikpos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/lib/include/picosha2.hpp` & `chikpos-2.0.0rc1/lib/include/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/python-bindings/chikpos.cpp` & `chikpos-2.0.0rc1/python-bindings/chikpos.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         .def(
             "get_id",
             [](DiskProver &dp) {
                 const std::vector<uint8_t>& id = dp.GetId();
                 return py::bytes(reinterpret_cast<const char*>(id.data()), id.size());
             })
         .def("get_size", [](DiskProver &dp) { return dp.GetSize(); })
+        .def("get_compression_level", [](DiskProver &dp) { return dp.GetCompressionLevel(); })
         .def("get_filename", [](DiskProver &dp) { return dp.GetFilename(); })
         .def(
             "get_qualities_for_challenge",
             [](DiskProver &dp, const py::bytes &challenge) {
                 if (len(challenge) != 32) {
                     throw std::invalid_argument("Challenge must be exactly 32 bytes");
                 }
@@ -175,10 +176,14 @@
                 }
                 uint8_t *quality_buf = new uint8_t[32];
                 quality.ToBytes(quality_buf);
                 py::bytes quality_py = py::bytes(reinterpret_cast<char *>(quality_buf), 32);
                 delete[] quality_buf;
                 return stdx::optional<py::bytes>(quality_py);
             });
+
+    py::class_<ContextQueue>(m, "ContextQueue")
+        .def("init", &ContextQueue::init);
+    m.attr("decompressor_context_queue") = &decompressor_context_queue;
 }
 
 #endif  // PYTHON_BINDINGS_PYTHON_BINDINGS_HPP_
```

### Comparing `chikpos-1.0.11/setup.py` & `chikpos-2.0.0rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 import os
 import re
+import shutil
 import sys
 import platform
 import subprocess
 
 from setuptools import setup, setuptools, Extension
 from setuptools.command.build_ext import build_ext
 from distutils.version import LooseVersion
@@ -40,14 +41,17 @@
     def build_extension(self, ext):
         extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
         cmake_args = [
             "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + str(extdir),
             "-DPYTHON_EXECUTABLE=" + sys.executable,
         ]
 
+        if os.getenv("CP_USE_GREEN_REAPER") == "1":
+            cmake_args.append("-DCP_LINK_BLADEBIT_HARVESTER=ON")
+
         cfg = "Debug" if self.debug else "Release"
         build_args = ["--config", cfg]
 
         if platform.system() == "Windows":
             cmake_args += [
                 "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}".format(cfg.upper(), extdir)
             ]
@@ -173,19 +177,32 @@
         if ct == "unix":
             opts.append('-DVERSION_INFO="%s"' % self.distribution.get_version())
             opts.append(cpp_flag(self.compiler))
             if has_flag(self.compiler, "-fvisibility=hidden"):
                 opts.append("-fvisibility=hidden")
         elif ct == "msvc":
             opts.append('/DVERSION_INFO=\\"%s\\"' % self.distribution.get_version())
+
+            # Link bladebit_harvester
+            if os.getenv("CP_USE_GREEN_REAPER") == "1":
+                opts.append("/DUSE_GREEN_REAPER=1")
+                opts.append("/DBLADEBIT_HARVESTER_LINKED=1")
+                opts.append("/Ilibs/green_reaper/include")
+                link_opts.append("libs/green_reaper/lib/bladebit_harvester.lib")
+
         for ext in self.extensions:
             ext.extra_compile_args = opts
             ext.extra_link_args = link_opts
         build_ext.build_extensions(self)
 
+        # Copy bladebit_harvester.dll on windows to the target build directory
+        # in order to package it into the root directory of the wheel
+        if os.getenv("CP_USE_GREEN_REAPER") == "1" and sys.platform == "win32":
+            shutil.copy2("libs/green_reaper/lib/bladebit_harvester.dll", self.build_lib + "/bladebit_harvester.dll")
+
 
 if platform.system() == "Windows":
     setup(
         name="chikpos",
         author="Mariano Sorgente",
         author_email="mariano@chiknetwork.com",
         description="Chik proof of space plotting, proving, and verifying (wraps C++)",
```

### Comparing `chikpos-1.0.11/src/b17phase2.hpp` & `chikpos-2.0.0rc1/src/b17phase2.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b17phase3.hpp` & `chikpos-2.0.0rc1/src/b17phase3.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b17phase4.hpp` & `chikpos-2.0.0rc1/src/b17phase4.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b17sort_manager.hpp` & `chikpos-2.0.0rc1/src/b17sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3.c` & `chikpos-2.0.0rc1/src/b3/blake3.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3.h` & `chikpos-2.0.0rc1/src/b3/blake3.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_avx2.c` & `chikpos-2.0.0rc1/src/b3/blake3_avx2.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_avx2_x86-64_unix.S` & `chikpos-2.0.0rc1/src/b3/blake3_avx2_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_avx512.c` & `chikpos-2.0.0rc1/src/b3/blake3_avx512.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_avx512_x86-64_unix.S` & `chikpos-2.0.0rc1/src/b3/blake3_avx512_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_dispatch.c` & `chikpos-2.0.0rc1/src/b3/blake3_dispatch.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_impl.h` & `chikpos-2.0.0rc1/src/b3/blake3_impl.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_portable.c` & `chikpos-2.0.0rc1/src/b3/blake3_portable.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_sse41.c` & `chikpos-2.0.0rc1/src/b3/blake3_sse41.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/b3/blake3_sse41_x86-64_unix.S` & `chikpos-2.0.0rc1/src/b3/blake3_sse41_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/bitfield.hpp` & `chikpos-2.0.0rc1/src/bitfield.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/bitfield_index.hpp` & `chikpos-2.0.0rc1/src/bitfield_index.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/bits.hpp` & `chikpos-2.0.0rc1/src/bits.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/calculate_bucket.hpp` & `chikpos-2.0.0rc1/src/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/chacha8.c` & `chikpos-2.0.0rc1/src/chacha8.c`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/chik_filesystem.hpp` & `chikpos-2.0.0rc1/src/chik_filesystem.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/cli.cpp` & `chikpos-2.0.0rc1/src/cli.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,25 @@
     cout << "./ProofOfSpace create" << endl;
     cout << "./ProofOfSpace prove <challenge>" << endl;
     cout << "./ProofOfSpace verify <proof> <challenge>" << endl;
     cout << "./ProofOfSpace check" << endl;
     exit(0);
 }
 
+// Not thread safe
+inline void InitDecompresserQueueDefault(bool no_cuda = false)
+{
+    static bool initialized = false;
+    if (initialized) {
+        return;
+    }
+    decompressor_context_queue.init(1, (uint32_t)std::thread::hardware_concurrency(), false, 9, !no_cuda, 0, false);
+    initialized = true;
+}
+
 int main(int argc, char *argv[]) try {
     cxxopts::Options options(
         "ProofOfSpace", "Utility for plotting, generating and verifying proofs of space.");
     options.positional_help("(create/prove/verify/check) param1 param2 ")
         .show_positional_help();
 
     // Default values
@@ -157,14 +168,16 @@
                 id_bytes.size(),
                 buffmegabytes,
                 num_buckets,
                 num_stripes,
                 num_threads,
                 phases_flags);
     } else if (operation == "prove") {
+        InitDecompresserQueueDefault();
+
         if (argc < 3) {
             HelpAndQuit(options);
         }
         cout << "Proving using filename=" << filename << " challenge=" << argv[2] << endl
              << endl;
         string challenge = Strip0x(argv[2]);
         if (challenge.size() != 64) {
@@ -234,64 +247,71 @@
             cout << "Proof verification suceeded. Quality: " << quality << endl;
         } else {
             cout << "Proof verification failed." << endl;
             exit(1);
         }
         delete[] proof_bytes;
     } else if (operation == "check") {
+        InitDecompresserQueueDefault();
+
         uint32_t iterations = 1000;
         if (argc == 3) {
             iterations = std::stoi(argv[2]);
         }
 
         DiskProver prover(filename);
         Verifier verifier = Verifier();
 
         uint32_t success = 0;
+        uint32_t failures = 0;
+        uint32_t exceptions = 0;
         std::vector<uint8_t> id_bytes = prover.GetId();
         k = prover.GetSize();
 
         for (uint32_t num = 0; num < iterations; num++) {
             vector<unsigned char> hash_input = intToBytes(num, 4);
             hash_input.insert(hash_input.end(), id_bytes.begin(), id_bytes.end());
 
             vector<unsigned char> hash(picosha2::k_digest_size);
             picosha2::hash256(hash_input.begin(), hash_input.end(), hash.begin(), hash.end());
 
-            try {
-                vector<LargeBits> qualities = prover.GetQualitiesForChallenge(hash.data());
+            vector<LargeBits> qualities = prover.GetQualitiesForChallenge(hash.data());
 
-                for (uint32_t i = 0; i < qualities.size(); i++) {
+            for (uint32_t i = 0; i < qualities.size(); i++) {
+                try {
                     LargeBits proof = prover.GetFullProof(hash.data(), i, parallel_read);
                     uint8_t *proof_data = new uint8_t[proof.GetSize() / 8];
                     proof.ToBytes(proof_data);
                     cout << "i: " << num << std::endl;
                     cout << "challenge: 0x" << Util::HexStr(hash.data(), 256 / 8) << endl;
                     cout << "proof: 0x" << Util::HexStr(proof_data, k * 8) << endl;
                     LargeBits quality =
                         verifier.ValidateProof(id_bytes.data(), k, hash.data(), proof_data, k * 8);
                     if (quality.GetSize() == 256 && quality == qualities[i]) {
                         cout << "quality: " << quality << endl;
                         cout << "Proof verification succeeded. k = " << static_cast<int>(k) << endl;
                         success++;
                     } else {
                         cout << "Proof verification failed." << endl;
+                        failures += 1;
                     }
                     delete[] proof_data;
+                } catch (const std::exception& error) {
+                    cout << "Threw: " << error.what() << endl;
+                    exceptions += 1;
                 }
-            } catch (const std::exception& error) {
-                cout << "Threw: " << error.what() << endl;
-                continue;
             }
         }
         std::cout << "Total success: " << success << "/" << iterations << ", "
                   << (success * 100 / static_cast<double>(iterations)) << "%." << std::endl;
+        std::cout << "Total failures: " << failures << std::endl;
+        std::cout << "Exceptions: " << exceptions << std::endl;
         if (show_progress) { progress(4, 1, 1); }
     } else {
-        cout << "Invalid operation. Use create/prove/verify/check" << endl;
+        cout << "Invalid operation '" << operation << "'. Use create/prove/verify/check" << endl;
     }
     return 0;
 } catch (const cxxopts::OptionException &e) {
     cout << "error parsing options: " << e.what() << endl;
     return 1;
 } catch (const std::exception &e) {
     std::cerr << "Caught exception: " << e.what() << endl;
```

### Comparing `chikpos-1.0.11/src/disk.hpp` & `chikpos-2.0.0rc1/src/disk.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/encoding.hpp` & `chikpos-2.0.0rc1/src/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/entry_sizes.hpp` & `chikpos-2.0.0rc1/src/entry_sizes.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/exceptions.hpp` & `chikpos-2.0.0rc1/src/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/phase1.hpp` & `chikpos-2.0.0rc1/src/phase1.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/phase2.hpp` & `chikpos-2.0.0rc1/src/phase2.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/phase3.hpp` & `chikpos-2.0.0rc1/src/phase3.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/phase4.hpp` & `chikpos-2.0.0rc1/src/phase4.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/phases.hpp` & `chikpos-2.0.0rc1/src/phases.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/plotter_disk.hpp` & `chikpos-2.0.0rc1/src/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/pos_constants.hpp` & `chikpos-2.0.0rc1/src/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/prover_disk.hpp` & `chikpos-2.0.0rc1/src/prover_disk.hpp`

 * *Files 25% similar despite different names*

```diff
@@ -20,45 +20,278 @@
 #endif
 #include <stdio.h>
 
 #include <algorithm>  // std::min
 #include <fstream>
 #include <future>
 #include <iostream>
-#include <mutex>
 #include <string>
 #include <utility>
 #include <vector>
+#include <mutex>
+#include <condition_variable>
 
 #include "../lib/include/picosha2.hpp"
 #include "calculate_bucket.hpp"
 #include "encoding.hpp"
 #include "entry_sizes.hpp"
 #include "serialize.hpp"
 #include "util.hpp"
 
+#if USE_GREEN_REAPER
+    #include "GreenReaperPortable.h"
+#endif
+
+#define CHIK_PLOT_V2_MAGIC       0x544F4C50ul   // "PLOT"
+#define CHIK_PLOT_VERSION_2_0_0  2
+
+
 struct plot_header {
     uint8_t magic[19];
     uint8_t id[32];
     uint8_t k;
     uint8_t fmt_desc_len[2];
     uint8_t fmt_desc[50];
 };
 
+#if USE_GREEN_REAPER
+static GRApi _grApi{};
+static bool _dcompressor_queue_initialized = false;
+class ContextQueue {
+public:
+    ContextQueue() {}
+
+    bool init(
+        uint32_t context_count,
+        uint32_t thread_count,
+        bool no_cpu_affinity,
+        const uint32_t max_compression_level,
+        bool use_gpu_harvesting,
+        uint32_t gpu_index,
+        bool enforce_gpu_index
+    ) {
+        assert(!_dcompressor_queue_initialized);
+        _dcompressor_queue_initialized = true;
+
+        // Populate the API
+        #if _WIN32
+            #define GR_LIB_PREFIX ""
+            #define GR_LIB_EXT ".dll"
+        #else
+            #define GR_LIB_PREFIX "lib"
+
+            #if __APPLE__
+                #define GR_LIB_EXT ".dylib"
+            #else
+                #define GR_LIB_EXT ".so"
+            #endif
+        #endif
+
+        // void* lib = grLoadModule(GR_LIB_PREFIX "bladebit_harvester" GR_LIB_EXT);
+
+        // if (lib == nullptr) {
+        //     int code;
+        //     #if _WIN32
+        //         code = (int)::GetLastError();
+        //     #else
+        //         code = (int)dlerror();
+        //     #endif
+
+        //     std::stringstream err; err << "Failed to load bladebit_harvester with error: '" << code << "'";
+        //     throw std::runtime_error(err.str());
+        // }
+        // #undef GR_LIB_PREFIX
+        // #undef GR_LIB_EXT
+
+        // // Init GR API
+        // {
+        //     const auto r = grPopulateApiFromModule(lib, &_grApi, sizeof(GRApi), GR_API_VERSION);
+        //     if (r != GRResult_OK) {
+        //         std::stringstream err; err << "Failed to initialize GR API with error " << r;
+        //         throw std::runtime_error(err.str());
+        //     }
+        // }
+
+        GreenReaperConfig cfg = {};
+        cfg.apiVersion = GR_API_VERSION;
+        cfg.threadCount = thread_count;
+        cfg.disableCpuAffinity = no_cpu_affinity;
+        if (!use_gpu_harvesting) {
+            cfg.gpuRequest = GRGpuRequestKind_None;
+        } else {
+            if (enforce_gpu_index) {
+                cfg.gpuRequest = GRGpuRequestKind_ExactDevice;
+            } else {
+                cfg.gpuRequest = GRGpuRequestKind_FirstAvailable;
+            }
+        }
+        cfg.gpuDeviceIndex = gpu_index;
+
+        for (uint32_t i = 0; i < context_count; i++) {
+            
+            cfg.cpuOffset = i * thread_count;
+            GreenReaperContext* gr = nullptr;
+            auto result = grCreateContext(&gr, &cfg, sizeof(cfg));
+
+            std::string error_msg;
+
+            if (result == GRResult_OK) {
+                assert(gr);
+                queue.push(gr);
+
+                // Preallocate memory required fot the maximum compression level we are supporting initially
+                result = grPreallocateForCompressionLevel(gr, 32, max_compression_level);
+                if (result != GRResult_OK) {
+                    std::stringstream err; err << "Failed to preallocate memory for contexts with result " << result;
+                    error_msg = err.str();
+                }
+            }
+            if (result != GRResult_OK) {
+                // Destroy contexts that were already created
+                while (!queue.empty()) {
+                    grDestroyContext( queue.front() );
+                    queue.pop();
+                }
+                if (error_msg.length() < 1) {
+                    std::stringstream err; err << "Failed to create GRContext with result " << result;
+                    error_msg = err.str();
+                }
+                throw std::runtime_error(error_msg);
+            }
+
+            if (i == 0 && use_gpu_harvesting) {
+                if (grHasGpuDecompressor(gr) == GR_TRUE) {
+                    return true;
+                } else {
+                    // default to CPU
+                    cfg.gpuRequest = GRGpuRequestKind_None;
+                }
+            }
+        }
+        return false;
+    }
+
+    void push(GreenReaperContext* gr) {
+        std::unique_lock<std::mutex> lock(mutex);
+        queue.push(gr);
+        lock.unlock();
+        condition.notify_one();
+    }
+
+    GreenReaperContext* pop() {
+        std::unique_lock<std::mutex> lock(mutex);
+        while (queue.empty()) {
+            condition.wait(lock);
+        }
+        GreenReaperContext* gr = queue.front();
+        queue.pop();
+        return gr;
+    }
+
+private:
+    std::queue<GreenReaperContext*> queue;
+    std::mutex mutex;
+    std::condition_variable condition;
+};
+
+class ProofCache {
+    static constexpr uint32_t MAX_ENTRIES = 64;
+
+    struct Entry {
+        alignas(16) uint8_t challenge[32];
+        uint32_t index;
+    };
+
+    uint32_t cache_entry_proof_position = 0;
+    std::vector<Entry> challenges;
+    std::vector<LargeBits> full_proofs;
+    mutable std::mutex lock;
+
+public:
+    inline ProofCache() = default;
+    inline ProofCache(ProofCache&& other)
+        : cache_entry_proof_position(other.cache_entry_proof_position)
+        , challenges(std::move(other.challenges))
+        , full_proofs(std::move(other.full_proofs))
+    {
+        other.cache_entry_proof_position = 0;
+    }
+
+    inline ProofCache(ProofCache const& other) = delete;
+
+    inline bool FoundCachedProof(const uint32_t index, const uint8_t* challenge, LargeBits& out_full_proof) {
+        std::lock_guard<std::mutex> l(lock);
+
+        Entry entry;
+        memcpy(entry.challenge, challenge, sizeof(entry.challenge));
+        entry.index = index;
+
+        for (uint32_t i = 0; i < challenges.size(); i++) {
+            if (memcmp(&challenges[i], &entry, sizeof(Entry)) == 0) {
+                out_full_proof = full_proofs[i];
+                return true;
+            }
+        }
+        return false;
+    }
+
+    inline void CacheProof(const uint32_t index, const uint8_t* challenge, const LargeBits& full_proof) {
+        std::lock_guard<std::mutex> l(lock);
+
+        Entry entry;
+        memcpy(entry.challenge, challenge, sizeof(entry.challenge));
+        entry.index = index;
+
+        if (challenges.size() < MAX_ENTRIES) {
+            challenges.emplace_back(entry);
+            full_proofs.emplace_back(full_proof);
+        } else {
+            challenges[cache_entry_proof_position] = entry;
+            full_proofs[cache_entry_proof_position] = full_proof;
+        }
+        cache_entry_proof_position = (cache_entry_proof_position + 1) % MAX_ENTRIES;
+    }
+
+    static_assert(alignof(ProofCache::Entry) == 16);
+};
+#else
+// Dummy one for python
+class ContextQueue {
+public:
+    inline ContextQueue() {}
+
+    inline bool init(
+        uint32_t context_count,
+        uint32_t thread_count,
+        bool no_cpu_affinity,
+        const uint32_t max_compression_level,
+        bool use_gpu_harvesting,
+        uint32_t gpu_index,
+        bool enforce_gpu_index
+    ) 
+    {
+        return false;
+    }
+};
+#endif // USE_GREEN_REAPER
+
+ContextQueue decompressor_context_queue;
+
 
 // The DiskProver, given a correctly formatted plot file, can efficiently generate valid proofs
 // of space, for a given challenge.
 class DiskProver {
 public:
     static const uint16_t VERSION{1};
     // The constructor opens the file, and reads the contents of the file header. The table pointers
     // will be used to find and seek to all seven tables, at the time of proving.
     explicit DiskProver(const std::string& filename) : id(kIdLen)
     {
         struct plot_header header{};
+        this->compression_level = 0;
         this->filename = filename;
 
         std::ifstream disk_file(filename, std::ios::in | std::ios::binary);
 
         if (!disk_file.is_open()) {
             throw std::invalid_argument("Invalid file " + filename);
         }
@@ -66,35 +299,84 @@
         // 32 bytes  - unique plot id
         // 1 byte    - k
         // 2 bytes   - format description length
         // x bytes   - format description
         // 2 bytes   - memo length
         // x bytes   - memo
 
-        SafeRead(disk_file, (uint8_t*)&header, sizeof(header));
-        if (memcmp(header.magic, "Proof of Space Plot", sizeof(header.magic)) != 0)
-            throw std::invalid_argument("Invalid plot header magic");
-
-        uint16_t fmt_desc_len = Util::TwoBytesToInt(header.fmt_desc_len);
-
-        if (fmt_desc_len == kFormatDescription.size() &&
-            !memcmp(header.fmt_desc, kFormatDescription.c_str(), fmt_desc_len)) {
-            // OK
+        // Check for V2 Magic.
+        uint8_t magic_2_bytes[4];
+        SafeRead(disk_file, magic_2_bytes, 4);
+        uint32_t magic_2_result;
+        memcpy(&magic_2_result, magic_2_bytes, sizeof(magic_2_result));
+        if (magic_2_result == CHIK_PLOT_V2_MAGIC) {
+            uint8_t version_bytes[4];
+            SafeRead(disk_file, version_bytes, 4);
+            uint32_t version_result;
+            memcpy(&version_result, version_bytes, sizeof(version_result));
+            if (version_result == CHIK_PLOT_VERSION_2_0_0) {
+                version = 2;
+            }
+            else {
+                throw std::invalid_argument("Unsupported version.");
+            }
         } else {
-            throw std::invalid_argument("Invalid plot file format");
+            // V1
+            version = 1;
+            memcpy(header.magic, magic_2_bytes, sizeof(magic_2_bytes));
+            uint8_t tmp_magic_buff[15];
+            SafeRead(disk_file, tmp_magic_buff, sizeof(header.magic) - 4);
+            memcpy(header.magic + 4, tmp_magic_buff, sizeof(tmp_magic_buff));
+            if (memcmp(header.magic, "Proof of Space Plot", sizeof(header.magic)) != 0) {
+                throw std::invalid_argument("Invalid plot header magic: " + Util::HexStr(header.magic, 19));
+            }
+        }
+
+        SafeRead(disk_file, (uint8_t*)&header.id, sizeof(header.id));
+        SafeRead(disk_file, (uint8_t*)&header.k, sizeof(header.k));
+
+        if (version == 1) {
+            SafeRead(disk_file, (uint8_t*)&header.fmt_desc_len, sizeof(header.fmt_desc_len));
+            SafeRead(disk_file, (uint8_t*)&header.fmt_desc, sizeof(header.fmt_desc));
+
+            uint16_t fmt_desc_len = Util::TwoBytesToInt(header.fmt_desc_len);
+
+            if (fmt_desc_len == kFormatDescription.size() &&
+                !memcmp(header.fmt_desc, kFormatDescription.c_str(), fmt_desc_len)) {
+                // OK
+            } else {
+                throw std::invalid_argument("Invalid plot file format");
+            }
+            SafeSeek(disk_file, offsetof(struct plot_header, fmt_desc) + fmt_desc_len);
         }
+
         memcpy(id.data(), header.id, sizeof(header.id));
         this->k = header.k;
-        SafeSeek(disk_file, offsetof(struct plot_header, fmt_desc) + fmt_desc_len);
 
         uint8_t size_buf[2];
         SafeRead(disk_file, size_buf, 2);
         memo.resize(Util::TwoBytesToInt(size_buf));
         SafeRead(disk_file, memo.data(), memo.size());
 
+        if (version == 2) {
+            uint8_t flags_bytes[4];
+            SafeRead(disk_file, flags_bytes, sizeof(flags_bytes));
+            uint32_t flags;
+            memcpy(&flags, flags_bytes, sizeof(flags));
+            if (flags & 1) {
+                uint8_t compression_level;
+                SafeRead(disk_file, &compression_level, sizeof(compression_level));
+                this->compression_level = compression_level;
+            }
+        }
+        #if !defined( USE_GREEN_REAPER )
+            if (this->compression_level > 0)
+                throw std::logic_error("Harvester does not support compressed plots.");
+        #endif
+
         this->table_begin_pointers = std::vector<uint64_t>(11, 0);
         this->C2 = std::vector<uint64_t>();
 
         uint8_t pointer_buf[8];
         for (uint8_t i = 1; i < 11; i++) {
             SafeRead(disk_file, pointer_buf, 8);
             this->table_begin_pointers[i] = Util::EightBytesToInt(pointer_buf);
@@ -130,34 +412,48 @@
         delete[] c2_buf;
     }
 
     explicit DiskProver(const std::vector<uint8_t>& vecBytes)
     {
         Deserializer deserializer(vecBytes);
         deserializer >> version;
-        if (version != VERSION) {
+        if (version != 1 && version != 2) {
             // TODO: Migrate to new version if we change something related to the data structure
             throw std::invalid_argument("DiskProver: Invalid version.");
         }
         deserializer >> filename;
         deserializer >> memo;
         deserializer >> id;
         deserializer >> k;
         deserializer >> table_begin_pointers;
         deserializer >> C2;
+        if (version == 2) {
+            deserializer >> compression_level;
+        } else {
+            compression_level = 0;
+        }
+
+        #if !defined( USE_GREEN_REAPER )
+            if (compression_level > 0)
+                throw std::runtime_error("Harvester does not support compressed plots.");
+        #endif
     }
 
     DiskProver(DiskProver const&) = delete;
 
     DiskProver(DiskProver&& other) noexcept
+        #if USE_GREEN_REAPER
+            : cached_proofs(std::move(other.cached_proofs))
+        #endif
     {
         filename = std::move(other.filename);
         memo = std::move(other.memo);
         id = std::move(other.id);
         k = other.k;
+        compression_level = other.compression_level;
         table_begin_pointers = std::move(other.table_begin_pointers);
         C2 = std::move(other.C2);
         version = std::move(other.version);
     }
 
     ~DiskProver()
     {
@@ -176,79 +472,194 @@
 
     const std::vector<uint64_t>& GetC2() const noexcept { return C2; }
 
     const std::string& GetFilename() const noexcept { return filename; }
 
     uint8_t GetSize() const noexcept { return k; }
 
+    uint8_t GetCompressionLevel() const noexcept { return compression_level; }
+
+    bool CompareProofBits(const LargeBits& left, const LargeBits& right, uint8_t k)
+    {
+        uint16_t size = left.GetSize() / k;
+        assert(left.GetSize() == right.GetSize());
+        for (int16_t i = size - 1; i >= 0; i--) {
+            LargeBits left_val = left.Slice(k * i, k * (i + 1));
+            LargeBits right_val = right.Slice(k * i, k * (i + 1));
+            if (left_val < right_val) {
+                return true;
+            }
+            if (left_val > right_val) {
+                return false;
+            }
+        }
+        return false;
+    }
+
+    LargeBits GetQualityStringFromProof(
+        LargeBits proof,
+        const uint8_t* challenge)
+    {
+        Bits challenge_bits = Bits(challenge, 256 / 8, 256);
+        uint16_t quality_index = challenge_bits.Slice(256 - 5).GetValue() << 1;
+
+        // Converts the proof from proof ordering to plot ordering
+        for (uint8_t table_index = 1; table_index < 7; table_index++) {
+            LargeBits new_proof;
+            uint16_t size = k * (1 << (table_index - 1));
+            for (int j = 0; j < (1 << (7 - table_index)); j += 2) {
+                LargeBits L = proof.Slice(j * size, (j + 1) * size);
+                LargeBits R = proof.Slice((j + 1) * size, (j + 2) * size);
+                if (CompareProofBits(L, R, k)) {
+                    new_proof += (L + R);
+                } else {
+                    new_proof += (R + L);
+                }
+            }
+            proof = new_proof;
+        }
+        // Hashes two of the x values, based on the quality index
+        std::vector<unsigned char> hash_input(32 + Util::ByteAlign(2 * k) / 8, 0);
+        memcpy(hash_input.data(), challenge, 32);
+        proof.Slice(k * quality_index, k * (quality_index + 2)).ToBytes(hash_input.data() + 32);
+        std::vector<unsigned char> hash(picosha2::k_digest_size);
+        picosha2::hash256(hash_input.begin(), hash_input.end(), hash.begin(), hash.end());
+        return LargeBits(hash.data(), 32, 256);
+    }
+
     // Given a challenge, returns a quality string, which is sha256(challenge + 2 adjecent x
     // values), from the 64 value proof. Note that this is more efficient than fetching all 64 x
     // values, which are in different parts of the disk.
     std::vector<LargeBits> GetQualitiesForChallenge(const uint8_t* challenge)
     {
         std::vector<LargeBits> qualities;
 
-        std::lock_guard<std::mutex> l(_mtx);
+        uint32_t p7_entries_size = 0;
 
         {
+            std::lock_guard<std::mutex> l(_mtx);
             std::ifstream disk_file(filename, std::ios::in | std::ios::binary);
 
             if (!disk_file.is_open()) {
                 throw std::invalid_argument("Invalid file " + filename);
             }
 
             // This tells us how many f7 outputs (and therefore proofs) we have for this
             // challenge. The expected value is one proof.
             std::vector<uint64_t> p7_entries = GetP7Entries(disk_file, challenge);
 
             if (p7_entries.empty()) {
                 return std::vector<LargeBits>();
             }
+            p7_entries_size = p7_entries.size();
 
             // The last 5 bits of the challenge determine which route we take to get to
             // our two x values in the leaves.
             uint8_t last_5_bits = challenge[31] & 0x1f;
 
             for (uint64_t position : p7_entries) {
+                #if USE_GREEN_REAPER
+                    if (compression_level >= 9) {
+                        break;
+                    }
+                #endif
                 // This inner loop goes from table 6 to table 1, getting the two backpointers,
                 // and following one of them.
-                for (uint8_t table_index = 6; table_index > 1; table_index--) {
+                uint64_t alt_position;
+                for (uint8_t table_index = 6; table_index > GetEndTable(); table_index--) {
                     uint128_t line_point = ReadLinePoint(disk_file, table_index, position);
 
                     auto xy = Encoding::LinePointToSquare(line_point);
                     assert(xy.first >= xy.second);
 
                     if (((last_5_bits >> (table_index - 2)) & 1) == 0) {
                         position = xy.second;
+                        alt_position = xy.first;
                     } else {
                         position = xy.first;
+                        alt_position = xy.second;
                     }
                 }
-                uint128_t new_line_point = ReadLinePoint(disk_file, 1, position);
-                auto x1x2 = Encoding::LinePointToSquare(new_line_point);
-
+                uint128_t new_line_point = ReadLinePoint(disk_file, GetEndTable(), position);
+                std::pair<uint64_t, uint64_t> x1x2;
+                
+                #if USE_GREEN_REAPER
+                    if (compression_level > 0) {
+                        GRCompressedQualitiesRequest req;
+                        req.compressionLevel = compression_level;
+                        req.plotId = id.data();
+                        req.challenge = challenge;
+                        req.xLinePoints[0].hi = (uint64_t)(new_line_point >> 64);
+                        req.xLinePoints[0].lo = (uint64_t)new_line_point;
+                        if (compression_level >= 6) {
+                            uint128_t alt_line_point = ReadLinePoint(disk_file, GetEndTable(), alt_position);
+                            req.xLinePoints[1].hi = (uint64_t)(alt_line_point >> 64);
+                            req.xLinePoints[1].lo = (uint64_t)alt_line_point;
+                        }
+
+                        GreenReaperContext* gr = decompressor_context_queue.pop();
+                        assert(gr);
+
+                        auto res = grGetFetchQualitiesXPair(gr, &req);
+                        decompressor_context_queue.push(gr);
+
+                        if (res != GRResult_OK) {
+                            // Expect this will result in failure in a later step.
+                            x1x2.first = x1x2.second = 0;
+                        } else {
+                            x1x2.first = req.x1;
+                            x1x2.second = req.x2;
+                        }
+                    } else 
+                #endif // #if USE_GREEN_REAPER
+                {
+                    x1x2 = Encoding::LinePointToSquare(new_line_point);
+                }
                 // The final two x values (which are stored in the same location) are hashed
                 std::vector<unsigned char> hash_input(32 + Util::ByteAlign(2 * k) / 8, 0);
                 memcpy(hash_input.data(), challenge, 32);
                 (LargeBits(x1x2.second, k) + LargeBits(x1x2.first, k))
                     .ToBytes(hash_input.data() + 32);
                 std::vector<unsigned char> hash(picosha2::k_digest_size);
                 picosha2::hash256(hash_input.begin(), hash_input.end(), hash.begin(), hash.end());
                 qualities.emplace_back(hash.data(), 32, 256);
             }
         }  // Scope for disk_file
+
+        #if USE_GREEN_REAPER
+            if (compression_level >= 9) {
+                uint8_t failure_bytes[32];
+                for (int i = 0; i < 32; i++) {
+                    failure_bytes[i] = 255;
+                }
+                for (uint32_t i = 0; i < p7_entries_size; i++) {
+                    try {
+                        auto proof = GetFullProof(challenge, i);
+                        qualities.push_back(GetQualityStringFromProof(proof, challenge));
+                    } catch (const std::exception& error) {
+                        qualities.emplace_back(failure_bytes, 32, 256);
+                    }
+                }
+            }
+        #endif
         return qualities;
     }
 
     // Given a challenge, and an index, returns a proof of space. This assumes GetQualities was
     // called, and there are actually proofs present. The index represents which proof to fetch,
     // if there are multiple.
     LargeBits GetFullProof(const uint8_t* challenge, uint32_t index, bool parallel_read = true)
     {
         LargeBits full_proof;
+        
+        #if USE_GREEN_REAPER
+            if (compression_level >= 9 && cached_proofs.FoundCachedProof(index, challenge, full_proof)) {
+                return full_proof;
+            }
+        #endif
 
         std::lock_guard<std::mutex> l(_mtx);
         {
             std::ifstream disk_file(filename, std::ios::in | std::ios::binary);
 
             if (!disk_file.is_open()) {
                 throw std::invalid_argument("Invalid file " + filename);
@@ -258,47 +669,104 @@
             if (p7_entries.empty() || index >= p7_entries.size()) {
                 throw std::logic_error("No proof of space for this challenge");
             }
 
             // Gets the 64 leaf x values, concatenated together into a k*64 bit string.
             std::vector<Bits> xs;
             if (parallel_read) {
-                xs = GetInputs(p7_entries[index], 6);
+                xs = GetInputs(p7_entries[index], 6, nullptr);
             } else {
                 xs = GetInputs(p7_entries[index], 6, &disk_file); // Passing in a disk_file disabled the parallel reads
             }
 
+            #if USE_GREEN_REAPER
+                if (compression_level > 0) {
+                    auto gr = decompressor_context_queue.pop();
+
+                    GRCompressedProofRequest req{};
+                    req.compressionLevel = compression_level;
+                    req.plotId = id.data();
+
+                    uint8_t compressed_proof_size = (compression_level <= 8 ? GR_POST_PROOF_CMP_X_COUNT : (GR_POST_PROOF_CMP_X_COUNT / 2));
+                    for (int i = 0; i < compressed_proof_size; i++) {
+                        req.compressedProof[i] = xs[i].GetValue();
+                    }
+
+                    GRResult res = grFetchProofForChallenge(gr, &req);
+                    decompressor_context_queue.push(gr);
+
+                    if (res != GRResult_OK) {
+                        if (res == GRResult_NoProof) {
+                            throw std::runtime_error("GRResult_NoProof received");
+                        }
+                        if (res == GRResult_Failed) {
+                            throw std::runtime_error("GRResult is not GRResult_OK, received GRResult_Failed");
+                        }
+                        if (res == GRResult_OutOfMemory) {
+                            throw std::runtime_error("GRResult is not GRResult_OK, received GRResult_OutOfMemory");
+                        }
+                        if (res == GRResult_WrongVersion) {
+                            throw std::runtime_error("GRResult is not GRResult_OK, received GRResult_WrongVersion");
+                        }
+                        if (res == GRResult_InvalidGPU) {
+                            throw std::runtime_error("GRResult is not GRResult_OK, received GRResult_InvalidGPU");
+                        }
+                        if (res == GRResult_InvalidArg) {
+                            throw std::runtime_error("GRResult is not GRResult_OK, received GRResult_InvalidArg");
+                        }
+                    }
+                    std::vector<Bits> uncompressed_xs;
+                    for (int i = 0; i < GR_POST_PROOF_X_COUNT; i++) {
+                        uncompressed_xs.push_back(Bits(req.fullProof[i], k));
+                    }
+                    xs = uncompressed_xs;
+                }
+            #endif
+
             // Sorts them according to proof ordering, where
             // f1(x0) m= f1(x1), f2(x0, x1) m= f2(x2, x3), etc. On disk, they are not stored in
             // proof ordering, they're stored in plot ordering, due to the sorting in the Compress
             // phase.
             std::vector<LargeBits> xs_sorted = ReorderProof(xs);
             for (const auto& x : xs_sorted) {
                 full_proof += x;
             }
         }  // Scope for disk_file
+
+        #if USE_GREEN_REAPER
+            if (compression_level >= 9) {
+                cached_proofs.CacheProof(index, challenge, full_proof);
+            }
+        #endif
         return full_proof;
     }
 
     std::vector<uint8_t> ToBytes() const
     {
         Serializer serializer;
         serializer << version << filename << memo << id << k << table_begin_pointers << C2;
+        if (version == 2) {
+            serializer << compression_level;
+        }
         return serializer.Data();
     }
 
 private:
     uint16_t version{VERSION};
     mutable std::mutex _mtx;
     std::string filename;
     std::vector<uint8_t> memo;
     std::vector<uint8_t> id;  // Unique plot id
     uint8_t k;
+    uint8_t compression_level;
     std::vector<uint64_t> table_begin_pointers;
     std::vector<uint64_t> C2;
+    #if USE_GREEN_REAPER
+        ProofCache cached_proofs;
+    #endif
 
     // Using this method instead of simply seeking will prevent segfaults that would arise when
     // continuing the process of looking up qualities.
     static void SafeSeek(std::ifstream& disk_file, uint64_t seek_location) {
         disk_file.seekg(seek_location);
 
         if (disk_file.fail()) {
@@ -324,38 +792,77 @@
                       << (disk_file.rdstate() & std::ifstream::eofbit)
                       << std::endl;
             throw std::runtime_error("badbit or failbit after reading size " +
                     std::to_string(size) + " at position " + std::to_string(pos));
         }
     }
 
+    uint8_t GetEndTable() {
+        if (compression_level == 0) {
+            return 1;
+        }
+        if (compression_level <= 8) {
+            return 2;
+        }
+        return 3;
+    }
+
     // Reads exactly one line point (pair of two k bit back-pointers) from the given table.
     // The entry at index "position" is read. First, the park index is calculated, then
     // the park is read, and finally, entry deltas are added up to the position that we
     // are looking for.
-    uint128_t ReadLinePoint(std::ifstream& disk_file, uint8_t table_index, uint64_t position)
-    {
+    uint128_t ReadLinePoint(
+        std::ifstream& disk_file,
+        uint8_t table_index,
+        uint64_t position
+    ) {
+        size_t compressed_park_size = 0;
+        uint32_t compressed_stub_size_bits = 0;
+        double compressed_ans_r_value = 0;
+
+        const bool is_compressed = compression_level > 0 && table_index == GetEndTable();
+        (void)is_compressed;
+
+        #if USE_GREEN_REAPER
+            if (is_compressed) {
+                GRCompressionInfo info{};
+                const auto r = grGetCompressionInfo(&info, sizeof(info), k, compression_level);
+                if (r != GRResult_OK) {
+                    std::stringstream err; err << "Failed to obtain compression info with error " << r;
+                    throw std::runtime_error(err.str());
+                }
+                
+                compressed_park_size = info.tableParkSize;;
+                compressed_stub_size_bits = info.subtSizeBits;
+                compressed_ans_r_value = info.ansRValue;
+            }
+        #else
+            (void)compressed_stub_size_bits;
+            (void)compressed_ans_r_value;
+            (void)compressed_park_size;
+        #endif
+
         uint64_t park_index = position / kEntriesPerPark;
-        uint32_t park_size_bits = EntrySizes::CalculateParkSize(k, table_index) * 8;
+        uint32_t park_size_bits = (is_compressed ? compressed_park_size : EntrySizes::CalculateParkSize(k, table_index)) * 8;
 
         SafeSeek(disk_file, table_begin_pointers[table_index] + (park_size_bits / 8) * park_index);
 
         // This is the checkpoint at the beginning of the park
         uint16_t line_point_size = EntrySizes::CalculateLinePointSize(k);
         auto* line_point_bin = new uint8_t[line_point_size + 7];
         SafeRead(disk_file, line_point_bin, line_point_size);
         uint128_t line_point = Util::SliceInt128FromBytes(line_point_bin, 0, k * 2);
 
         // Reads EPP stubs
-        uint32_t stubs_size_bits = EntrySizes::CalculateStubsSize(k) * 8;
+        uint32_t stubs_size_bits = (is_compressed ? (Util::ByteAlign((kEntriesPerPark - 1) * compressed_stub_size_bits) / 8) : EntrySizes::CalculateStubsSize(k)) * 8;
         auto* stubs_bin = new uint8_t[stubs_size_bits / 8 + 7];
         SafeRead(disk_file, stubs_bin, stubs_size_bits / 8);
 
-        // Reads EPP deltas
-        uint32_t max_deltas_size_bits = EntrySizes::CalculateMaxDeltasSize(k, table_index) * 8;
+        // Reads EPP deltas        
+        uint32_t max_deltas_size_bits = (is_compressed ? compressed_park_size - (line_point_size + stubs_size_bits) : EntrySizes::CalculateMaxDeltasSize(k, table_index)) * 8;
         auto* deltas_bin = new uint8_t[max_deltas_size_bits / 8];
 
         // Reads the size of the encoded deltas object
         uint16_t encoded_deltas_size = 0;
         SafeRead(disk_file, (uint8_t*)&encoded_deltas_size, sizeof(uint16_t));
 
         if (encoded_deltas_size * 8 > max_deltas_size_bits) {
@@ -370,21 +877,21 @@
             deltas.resize(encoded_deltas_size);
             SafeRead(disk_file, deltas.data(), encoded_deltas_size);
         } else {
             // Compressed
             SafeRead(disk_file, deltas_bin, encoded_deltas_size);
 
             // Decodes the deltas
-            double R = kRValues[table_index - 1];
+            double R = (is_compressed ? compressed_ans_r_value : kRValues[table_index - 1]);
             deltas =
                 Encoding::ANSDecodeDeltas(deltas_bin, encoded_deltas_size, kEntriesPerPark - 1, R);
         }
 
         uint32_t start_bit = 0;
-        uint8_t stub_size = k - kStubMinusBits;
+        uint8_t stub_size = (uint8_t)(is_compressed ? compressed_stub_size_bits : k - kStubMinusBits);
         uint64_t sum_deltas = 0;
         uint64_t sum_stubs = 0;
         for (uint32_t i = 0;
              i < std::min((uint32_t)(position % kEntriesPerPark), (uint32_t)deltas.size());
              i++) {
             uint64_t stub = Util::EightBytesToInt(stubs_bin + start_bit / 8);
             stub <<= start_bit % 8;
@@ -720,15 +1227,15 @@
             std::ifstream disk_file_parallel(filename, std::ios::in | std::ios::binary);
             line_point = ReadLinePoint(disk_file_parallel, depth, position);
         } else {
             line_point = ReadLinePoint(*disk_file, depth, position);
         }
         std::pair<uint64_t, uint64_t> xy = Encoding::LinePointToSquare(line_point);
 
-        if (depth == 1) {
+        if (depth == GetEndTable()) {
             // For table P1, the line point represents two concatenated x values.
             std::vector<Bits> ret;
             ret.emplace_back(xy.second, k);  // y
             ret.emplace_back(xy.first, k);   // x
             return ret;
         } else {
             std::vector<Bits> left, right;
```

### Comparing `chikpos-1.0.11/src/quicksort.hpp` & `chikpos-2.0.0rc1/src/quicksort.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/serialize.hpp` & `chikpos-2.0.0rc1/src/serialize.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/sort_manager.hpp` & `chikpos-2.0.0rc1/src/sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/threading.hpp` & `chikpos-2.0.0rc1/src/threading.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/uniformsort.hpp` & `chikpos-2.0.0rc1/src/uniformsort.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/util.hpp` & `chikpos-2.0.0rc1/src/util.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/src/verifier.hpp` & `chikpos-2.0.0rc1/src/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/tests/plot-resources.py` & `chikpos-2.0.0rc1/tests/plot-resources.py`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/tests/test.cpp` & `chikpos-2.0.0rc1/tests/test.cpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/tests/test_python_bindings.py` & `chikpos-2.0.0rc1/tests/test_python_bindings.py`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/tools/disk.gnuplot` & `chikpos-2.0.0rc1/tools/disk.gnuplot`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/tools/parse_disk.py` & `chikpos-2.0.0rc1/tools/parse_disk.py`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/uint128_t/LICENSE` & `chikpos-2.0.0rc1/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/uint128_t/README.md` & `chikpos-2.0.0rc1/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/uint128_t/endianness.h` & `chikpos-2.0.0rc1/uint128_t/endianness.h`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/uint128_t/uint128_t.cpp` & `chikpos-2.0.0rc1/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/uint128_t/uint128_t.include` & `chikpos-2.0.0rc1/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chikpos-1.0.11/uint128_t/uint128_t_config.include` & `chikpos-2.0.0rc1/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

