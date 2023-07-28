# Comparing `tmp/xcsf-1.3.0.tar.gz` & `tmp/xcsf-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsf-1.3.0.tar", last modified: Thu Jul 20 10:56:30 2023, max compression
+gzip compressed data, was "xcsf-1.3.1.tar", last modified: Fri Jul 28 19:56:55 2023, max compression
```

## Comparing `xcsf-1.3.0.tar` & `xcsf-1.3.1.tar`

### file list

```diff
@@ -1,702 +1,704 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7267 2023-07-20 10:48:26.000000 xcsf-1.3.0/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    35149 2023-07-20 10:48:26.000000 xcsf-1.3.0/LICENSE.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      162 2023-07-20 10:48:26.000000 xcsf-1.3.0/MANIFEST.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-20 10:56:30.940587 xcsf-1.3.0/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3264 2023-07-20 10:48:26.000000 xcsf-1.3.0/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      428 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.editorconfig
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.git
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      340 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.gitattributes
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/.github/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2386 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.github/CONTRIBUTING.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/.github/workflows/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3308 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.github/workflows/CI.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      599 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.github/workflows/ci-fuzz.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      171 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      602 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/.travis.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    24882 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/CHANGELOG.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10330 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3903 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/CONTRIBUTORS.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1084 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/cJSON/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4650 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27632 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/README.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2284 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/appveyor.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    77959 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16193 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    40729 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON_Utils.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3938 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/cJSON_Utils.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/fuzzing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1169 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/CMakeLists.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      153 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/afl-prepare-linux.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/afl.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/afl.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1695 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/cjson_read_fuzzer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      992 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/fuzz_main.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      585 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       81 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test10
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      151 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test11
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      244 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.bu
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uf
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uu
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3465 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test4
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      875 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test5
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      487 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test6
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      401 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test7
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      249 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test8
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       52 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test9
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/json.dict
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      529 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/fuzzing/ossfuzz.sh
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/library_config/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      802 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/cJSONConfig.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      379 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/cJSONConfigVersion.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      304 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/libcjson.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      351 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/libcjson_utils.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      728 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/library_config/uninstall.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7711 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/test.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4530 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12775 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/cjson_add.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4166 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8588 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/compare_tests.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/inputs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      583 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      474 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test1.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       79 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test10
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       78 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test10.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      149 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test11
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test11.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      242 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      268 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test2.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test3
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      505 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test3.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3464 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test4
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3285 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test4.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      873 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test5
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      900 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test5.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      484 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test6
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test7
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      347 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test7.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      247 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test8
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      228 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test8.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       50 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test9
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/inputs/test9.expected
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      183 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/.editorconfig
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       25 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/.npmignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2306 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/README.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2659 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      393 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/package.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4031 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/spec_tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17205 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6776 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/json_patch_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5456 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/minify_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28328 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/misc_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/misc_utils_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7766 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/old_utils_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5068 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_array.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7999 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_examples.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3434 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_hex4.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3902 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_number.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5568 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_object.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4679 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_string.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3302 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_value.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4168 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/parse_with_opts.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3818 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_array.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4447 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_number.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4223 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_object.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2822 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_string.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3189 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/print_value.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6854 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/readme_examples.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      573 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/.gitattributes
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      212 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/.travis.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7806 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/auto/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3462 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_prompt.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_reporter.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1273 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_config.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11086 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_module.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18170 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_test_runner.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6995 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/parse_output.rb
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     7698 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/stylize_as_junit.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      766 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/test_file_filter.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/type_sanitizer.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5173 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4143 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5939 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_to_junit.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/docs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8092 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   144467 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28588 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18107 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8249 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9332 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1123 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/docs/license.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2237 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      139 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      862 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      335 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2393 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      567 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1998 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1768 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      175 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2453 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      664 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      271 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode2_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/all_tests.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/helper/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      405 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      483 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      884 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8367 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      696 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2357 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      565 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12322 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/examples/unity_config.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/eclipse/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1138 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1109 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6621 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      515 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.916587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3348 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1518 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1892 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2314 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/Makefile
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/main/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      653 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      722 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14403 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2593 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1206 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      628 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/release/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        5 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/release/build.info
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        7 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/release/version.info
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    49464 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    66485 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    69552 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/src/unity_internals.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/.rubocop.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2665 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/Makefile
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1271 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_def.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1242 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      333 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_head1.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1649 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1493 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1489 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      267 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1405 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1576 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3094 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8988 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile_helper.rb
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/spec/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4386 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_file.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_strict.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      917 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_32.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      942 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_64.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      856 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1139 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      854 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2960 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2060 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2274 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1898 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2244 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_msp430.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2052 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/CException.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/Defs.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      452 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/cmock.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      291 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/mockMock.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5137 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1356 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5844 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.920587 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    47428 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3442 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testparameterized.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   123592 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testunity.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      121 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/tests/unity_setup.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/cJSON/valgrind.supp
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.924587 xcsf-1.3.0/lib/dSFMT/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-07-20 10:48:45.000000 xcsf-1.3.0/lib/dSFMT/.git
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       30 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/.gitattributes
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       23 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2505 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/CHANGE-LOG.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1159 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/FILES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/LICENSE.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6429 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1022 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/Makefile.me
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2040 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/README.jp.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/README.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      368 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/check.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3482 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2437 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params11213.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params1279.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1474 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params132049.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params19937.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1476 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params216091.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params2203.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1460 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params4253.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params44497.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1452 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params521.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-params86243.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9492 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-ref.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   170957 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   196085 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   286679 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   319806 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   251845 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   280951 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41871 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.11213.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.1279.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41873 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.132049.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.19937.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41874 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.216091.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.2203.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41870 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.4253.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.44497.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41868 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.521.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.86243.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19933 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22620 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/dSFMT.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      332 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/debug.log
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76640 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/doxygen.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56023 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/doxygen.cfg.bak
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.924587 xcsf-1.3.0/lib/dSFMT/html/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/annotated.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/bc_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2825 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/classes.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/closed.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56903 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8c.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   121388 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    66996 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h_source.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/doxygen.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/doxygen.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2628 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/files.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2576 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/functions.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2468 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/functions_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11998 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3184 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_defs.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9926 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2320 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_type.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2536 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/globals_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11775 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/howto-compile.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9777 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/index.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/jquery.js
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1797 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/mainpage_8txt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/nav_f.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/nav_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/open.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5685 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/struct_d_s_f_m_t___t.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_a.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_b.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tab_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/tabs.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5509 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/html/union_w128___t.html
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/dSFMT/jump/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       35 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/CHANGE-LOG.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1438 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/FILES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/LICENSE.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3738 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1564 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/Makefile.me
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   387016 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   324452 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4265 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7578 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-old.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8670 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic.cpp
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   320872 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-jump
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1758 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/calc-jump.cpp
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      216 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/check-jump.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2242 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMT-calc-jump.hpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4493 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      596 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7761 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/dSFMText.hpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76359 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/debug.fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)  1078648 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/debug.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   316464 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/degree
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1281 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/degree.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    39223 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/degree.xlsx
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76620 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56003 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg.bak
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22586 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   264292 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.fix.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4473 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.fix.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   266939 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   436638 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4503 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.2203.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   366344 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/factorization
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/factorization.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2880 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    33093 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5064 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.19937.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      615 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11200 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.44497.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21652 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/fix.86243.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/dSFMT/jump/html/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2110 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/annotated.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/bc_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/bdwn.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2512 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/classes.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/closed.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4946 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8427 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10812 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2354 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/files.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2343 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/functions.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2235 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/functions_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2779 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/globals.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2527 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/globals_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2174 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/globals_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5241 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/index.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/jquery.js
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1880 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/mainpage_8txt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7747 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespacedsfmt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2503 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2382 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2123 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/namespaces.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/nav_f.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/nav_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/open.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3734 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/struct_f_i_x___t.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_a.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_b.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tab_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/html/tabs.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      839 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.1279.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   455421 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.132049.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   479378 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   124744 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2520 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.4253.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      358 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.521.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18059 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/lcm.86243.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1535 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/mainpage.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      100 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/memo.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      528 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/params.csv
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2883 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      385 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.1279.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    33388 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5089 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.19937.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    54080 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      598 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1114 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.4253.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11284 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.44497.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      176 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.521.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21836 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/poly.86243.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8246 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/readme-jp.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6265 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/readme.html
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)    26496 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1908 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample1.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)    18344 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2806 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/sample2.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M11213
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M1279
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   363792 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M132049
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M19937
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   376080 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M216091
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M2203
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M4253
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   351456 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M44497
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   339168 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M521
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   355600 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump-M86243
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6612 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/jump/test-jump.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3986 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/mainpage.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      557 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1642 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample3.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/sample4.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19611 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/dSFMT/test.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6491 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/doctest/examples/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/examples/all_features/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7948 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/all_features/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5086 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.932587 xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1556 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6731 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/executable_dll_and_plugin/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1184 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/dll/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      444 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/dll/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/executable/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      284 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/installed_doctest_cmake/executable/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/examples/mpi/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      311 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/examples/mpi/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/doctest/scripts/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/scripts/cmake/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      979 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/assemble_single_header.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8999 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/common.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7762 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/doctest.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3688 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/doctestAddTests.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2952 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/cmake/exec_test.cmake
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/scripts/how_stuff_works/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/how_stuff_works/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/doctest/scripts/playground/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      364 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/doctest/scripts/playground/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11983 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.912587 xcsf-1.3.0/lib/pybind11/include/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23959 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7069 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    65660 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8458 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      120 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2096 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28518 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    52930 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17869 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    26305 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    42613 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1625 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    31450 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18140 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      316 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13471 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4731 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5002 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8262 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8862 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    79416 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9103 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2734 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/options.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   126420 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    94641 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/include/pybind11/stl/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4185 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15337 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    29747 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21675 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2639 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1171 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1293 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1685 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1353 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1163 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1368 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tests/test_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tests/test_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/lib/pybind11/tools/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2350 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3105 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11190 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      817 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/JoinPaths.cmake
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1423 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/check-style.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      952 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1040 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1031 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/libsize.py
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1311 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/make_changelog.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      196 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14033 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8960 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8361 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       94 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/pyproject.toml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2104 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1234 2023-07-20 10:48:46.000000 xcsf-1.3.0/lib/pybind11/tools/setup_main.py.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-20 10:56:30.940587 xcsf-1.3.0/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4736 2023-07-20 10:48:26.000000 xcsf-1.3.0/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.936587 xcsf-1.3.0/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1432 2023-07-20 10:48:26.000000 xcsf-1.3.0/test/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/xcsf/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4641 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       20 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10726 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/__init__.pyi
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8230 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_integer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2787 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_integer.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9843 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2914 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/act_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5611 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/action.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9383 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/action.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7633 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/blas.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1579 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/blas.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19335 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cl.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3024 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23374 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2361 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6348 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1636 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/clset_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8819 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2878 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5977 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dummy.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2643 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_dummy.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13386 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ellipsoid.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3046 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ellipsoid.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8983 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_gp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2803 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_gp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11827 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3331 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15096 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_rectangle.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3097 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_rectangle.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13578 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ternary.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3221 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/cond_ternary.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13833 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/condition.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12061 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/condition.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2291 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/config.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/config.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23543 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3447 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16108 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/ea.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3096 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/ea.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1675 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3350 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7316 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_csv.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1679 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_csv.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7587 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_maze.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2018 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_maze.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4060 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_mux.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1720 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/env_mux.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18174 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/gp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3137 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/gp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4443 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/image.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1149 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/image.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/loss.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2531 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/loss.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2211 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/main.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14550 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3083 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6333 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_activations.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4420 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_activations.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17673 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12532 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22350 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_args.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3010 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_args.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8550 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_avgpool.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2595 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_avgpool.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15031 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_connected.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2669 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_connected.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21064 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_convolutional.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2869 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_convolutional.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8227 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_dropout.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2578 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_dropout.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    25430 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_lstm.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2479 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_lstm.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11181 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_maxpool.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2587 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_maxpool.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8094 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_noise.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2533 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_noise.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16764 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_recurrent.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2663 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_recurrent.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7627 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_softmax.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2577 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_softmax.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9233 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_upsample.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2620 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/neural_layer_upsample.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pa.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1168 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pa.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28009 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3520 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/param.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1486 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/perf.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      944 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/perf.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6703 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_constant.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2542 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_constant.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14958 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3441 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11945 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_nlms.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2918 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_nlms.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11788 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_rls.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3074 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pred_rls.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10334 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/prediction.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10375 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/prediction.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1113 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_callback.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3955 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_callback_checkpoint.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5460 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_callback_earlystop.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1465 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_utils.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    38402 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/pybind_wrapper.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7380 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4871 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7916 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5047 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/rule_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3796 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/sam.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1216 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/sam.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/xcsf/utils/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4045 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils/types.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5758 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils/viz.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3180 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4015 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/utils.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8322 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_rl.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1571 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_rl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7287 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_supervised.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1447 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcs_supervised.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6318 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcsf.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6927 2023-07-20 10:48:26.000000 xcsf-1.3.0/xcsf/xcsf.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:56:30.940587 xcsf-1.3.0/xcsf.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21726 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/not-zip-safe
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       15 2023-07-20 10:56:30.000000 xcsf-1.3.0/xcsf.egg-info/top_level.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.698229 xcsf-1.3.1/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8101 2023-07-28 19:49:07.000000 xcsf-1.3.1/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    35149 2023-07-20 10:48:26.000000 xcsf-1.3.1/LICENSE.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      162 2023-07-20 10:48:26.000000 xcsf-1.3.1/MANIFEST.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-28 19:56:55.698229 xcsf-1.3.1/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3264 2023-07-20 10:48:26.000000 xcsf-1.3.1/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.602228 xcsf-1.3.1/lib/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.602228 xcsf-1.3.1/lib/cJSON/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      428 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.editorconfig
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.git
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      340 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.gitattributes
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.602228 xcsf-1.3.1/lib/cJSON/.github/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2386 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.github/CONTRIBUTING.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.606228 xcsf-1.3.1/lib/cJSON/.github/workflows/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3308 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.github/workflows/CI.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      599 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.github/workflows/ci-fuzz.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      171 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      602 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/.travis.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    24882 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/CHANGELOG.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10330 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3903 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/CONTRIBUTORS.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1084 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/cJSON/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4650 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27632 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/README.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2284 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/appveyor.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    77959 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/cJSON.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16193 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/cJSON.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    40729 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/cJSON_Utils.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3938 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/cJSON_Utils.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.606228 xcsf-1.3.1/lib/cJSON/fuzzing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1169 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/CMakeLists.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      153 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/afl-prepare-linux.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4192 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/afl.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/afl.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1695 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/cjson_read_fuzzer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      992 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/fuzz_main.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.606228 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      585 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       81 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test10
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      151 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test11
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      244 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3.bu
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3.uf
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3.uu
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3465 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test4
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      875 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test5
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      487 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test6
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      401 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test7
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      249 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test8
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       52 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test9
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/json.dict
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      529 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/fuzzing/ossfuzz.sh
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.606228 xcsf-1.3.1/lib/cJSON/library_config/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      802 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/library_config/cJSONConfig.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      379 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/library_config/cJSONConfigVersion.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      304 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/library_config/libcjson.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      351 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/library_config/libcjson_utils.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      728 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/library_config/uninstall.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7711 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/test.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.610228 xcsf-1.3.1/lib/cJSON/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4530 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12775 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/cjson_add.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4166 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8588 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/compare_tests.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.614228 xcsf-1.3.1/lib/cJSON/tests/inputs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      583 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      474 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test1.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       79 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test10
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       78 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test10.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      149 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test11
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test11.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      242 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      268 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test2.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test3
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      505 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test3.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3464 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test4
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3285 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test4.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      873 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test5
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      900 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test5.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      484 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test6
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test7
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      347 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test7.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      247 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test8
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      228 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test8.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       50 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test9
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/inputs/test9.expected
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.618228 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      183 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/.editorconfig
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       25 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/.npmignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2306 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/README.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2659 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      393 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/package.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4031 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/spec_tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17205 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6776 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/json_patch_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5456 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/minify_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28328 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/misc_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3386 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/misc_utils_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7766 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/old_utils_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5068 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_array.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7999 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_examples.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3434 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_hex4.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3902 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_number.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5568 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_object.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4679 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_string.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3302 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_value.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4168 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/parse_with_opts.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3818 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/print_array.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4447 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/print_number.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4223 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/print_object.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2822 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/print_string.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3189 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/print_value.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6854 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/readme_examples.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.618228 xcsf-1.3.1/lib/cJSON/tests/unity/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      573 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/.gitattributes
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      212 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/.travis.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7806 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.618228 xcsf-1.3.1/lib/cJSON/tests/unity/auto/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3462 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/colour_prompt.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/colour_reporter.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1273 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/generate_config.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11086 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/generate_module.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18170 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/generate_test_runner.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6995 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/parse_output.rb
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     7698 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/stylize_as_junit.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      766 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/test_file_filter.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/type_sanitizer.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5173 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/unity_test_summary.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4143 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/unity_test_summary.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5939 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/auto/unity_to_junit.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.622228 xcsf-1.3.1/lib/cJSON/tests/unity/docs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8092 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   144467 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28588 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18107 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8249 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9332 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1123 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/docs/license.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.622228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.622228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2237 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      139 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.622228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      862 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      335 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.622228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2393 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      567 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.622228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/test_runners/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1998 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.622228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1768 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      175 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2453 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      664 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/test_runners/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      271 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode2_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/test_runners/all_tests.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/helper/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      405 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      483 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      884 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/rakefile.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8367 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      696 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2357 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      565 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12322 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/examples/unity_config.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.598228 xcsf-1.3.1/lib/cJSON/tests/unity/extras/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/extras/eclipse/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1138 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1109 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/rakefile.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6621 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      515 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.626228 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10386 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3348 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1518 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1892 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.630229 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2314 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/Makefile
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.630229 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/main/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      653 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      722 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14403 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2593 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1206 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      628 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.630229 xcsf-1.3.1/lib/cJSON/tests/unity/release/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        5 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/release/build.info
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        7 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/release/version.info
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.630229 xcsf-1.3.1/lib/cJSON/tests/unity/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    49464 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/src/unity.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    66485 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/src/unity.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    69552 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/src/unity_internals.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.630229 xcsf-1.3.1/lib/cJSON/tests/unity/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/.rubocop.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2665 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/Makefile
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.634229 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1271 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_def.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1242 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      333 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_head1.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1649 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1493 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1489 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      267 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1405 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1576 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3094 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/rakefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8988 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/rakefile_helper.rb
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.634229 xcsf-1.3.1/lib/cJSON/tests/unity/test/spec/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4386 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.638229 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/clang_file.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/clang_strict.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      917 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_32.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      942 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_64.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      856 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1139 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      854 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2960 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2060 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2274 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1898 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2244 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_msp430.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2052 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.638229 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/CException.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/Defs.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      452 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/cmock.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      291 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/mockMock.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5137 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1356 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5844 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.638229 xcsf-1.3.1/lib/cJSON/tests/unity/test/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    47428 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3442 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/tests/testparameterized.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   123592 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity/test/tests/testunity.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      121 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/tests/unity_setup.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/cJSON/valgrind.supp
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.650229 xcsf-1.3.1/lib/dSFMT/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-07-20 10:48:45.000000 xcsf-1.3.1/lib/dSFMT/.git
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       30 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/.gitattributes
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       23 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2505 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/CHANGE-LOG.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1159 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/FILES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/LICENSE.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6429 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1022 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/Makefile.me
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2040 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/README.jp.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/README.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      368 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/check.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3482 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2437 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params11213.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params1279.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1474 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params132049.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params19937.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1476 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params216091.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params2203.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1460 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params4253.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params44497.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1452 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params521.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-params86243.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9492 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-ref.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   170957 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.0.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   196085 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.0.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   286679 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.1.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   319806 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.1.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   251845 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   280951 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41871 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.11213.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.1279.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41873 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.132049.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.19937.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41874 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.216091.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.2203.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41870 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.4253.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.44497.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41868 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.521.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.86243.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19933 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22620 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/dSFMT.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      332 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/debug.log
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76640 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/doxygen.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56023 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/doxygen.cfg.bak
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.654229 xcsf-1.3.1/lib/dSFMT/html/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/annotated.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/bc_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2825 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/classes.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/closed.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56903 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/d_s_f_m_t_8c.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   121388 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/d_s_f_m_t_8h.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    66996 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/d_s_f_m_t_8h_source.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/doxygen.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/doxygen.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2628 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/files.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2576 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/functions.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2468 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/functions_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11998 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/globals.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3184 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/globals_defs.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9926 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/globals_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2320 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/globals_type.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2536 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/globals_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11775 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/howto-compile.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9777 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/index.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/jquery.js
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1797 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/mainpage_8txt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/nav_f.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/nav_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/open.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5685 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/struct_d_s_f_m_t___t.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/tab_a.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/tab_b.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/tab_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/tab_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/tabs.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5509 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/html/union_w128___t.html
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.674229 xcsf-1.3.1/lib/dSFMT/jump/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       35 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/CHANGE-LOG.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1438 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/FILES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/LICENSE.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3738 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1564 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/Makefile.me
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   387016 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   324452 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic-mpi
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4265 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic-mpi.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7578 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic-old.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8670 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic.cpp
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   320872 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/calc-jump
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1758 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/calc-jump.cpp
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      216 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/check-jump.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2242 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/dSFMT-calc-jump.hpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4493 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/dSFMT-jump.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      596 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/dSFMT-jump.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7761 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/dSFMText.hpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76359 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/debug.fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)  1078648 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/debug.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   316464 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/degree
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1281 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/degree.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    39223 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/degree.xlsx
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76620 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/doxygen.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56003 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/doxygen.cfg.bak
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22586 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fac.fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   264292 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fac.fix.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4473 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fac.fix.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   266939 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fac.lcm.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   436638 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fac.lcm.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4503 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fac.lcm.2203.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   366344 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/factorization
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/factorization.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2880 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    33093 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fix.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5064 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fix.19937.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      615 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fix.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11200 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fix.44497.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21652 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/fix.86243.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/dSFMT/jump/html/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2110 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/annotated.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/bc_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/bdwn.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2512 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/classes.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/closed.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4946 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8427 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10812 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/doxygen.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/doxygen.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2354 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/files.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2343 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/functions.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2235 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/functions_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2779 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/globals.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2527 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/globals_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2174 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/globals_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5241 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/index.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/jquery.js
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1880 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/mainpage_8txt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7747 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/namespacedsfmt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2503 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/namespacemembers.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2382 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/namespacemembers_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2123 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/namespaces.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/nav_f.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/nav_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/open.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3734 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/struct_f_i_x___t.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/tab_a.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/tab_b.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/tab_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/tab_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/html/tabs.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      839 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/lcm.1279.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   455421 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/lcm.132049.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   479378 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/lcm.216091.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   124744 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/lcm.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2520 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/lcm.4253.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      358 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/lcm.521.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18059 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/lcm.86243.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1535 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/mainpage.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      100 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/memo.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      528 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/params.csv
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2883 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      385 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.1279.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    33388 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5089 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.19937.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    54080 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      598 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1114 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.4253.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11284 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.44497.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      176 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.521.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21836 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/poly.86243.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8246 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/readme-jp.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6265 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/readme.html
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)    26496 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/sample1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1908 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/sample1.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)    18344 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/sample2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2806 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/sample2.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M11213
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M1279
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   363792 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M132049
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M19937
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   376080 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M216091
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M2203
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M4253
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   351456 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M44497
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   339168 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M521
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   355600 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump-M86243
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6612 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/jump/test-jump.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3986 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/mainpage.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      557 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/sample1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1642 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/sample2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/sample3.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/sample4.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19611 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/dSFMT/test.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6491 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.602228 xcsf-1.3.1/lib/doctest/examples/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/examples/all_features/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7948 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/all_features/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5086 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/examples/exe_with_static_libs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1556 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6731 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/examples/executable_dll_and_plugin/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1184 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.602228 xcsf-1.3.1/lib/doctest/examples/installed_doctest_cmake/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/examples/installed_doctest_cmake/dll/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      444 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/installed_doctest_cmake/dll/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/examples/installed_doctest_cmake/executable/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      284 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/installed_doctest_cmake/executable/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/examples/mpi/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      311 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/examples/mpi/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.602228 xcsf-1.3.1/lib/doctest/scripts/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/scripts/cmake/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      979 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/scripts/cmake/assemble_single_header.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8999 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/scripts/cmake/common.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7762 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/scripts/cmake/doctest.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3688 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/scripts/cmake/doctestAddTests.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2952 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/scripts/cmake/exec_test.cmake
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/scripts/how_stuff_works/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/scripts/how_stuff_works/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/doctest/scripts/playground/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      364 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/doctest/scripts/playground/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.682229 xcsf-1.3.1/lib/pybind11/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12067 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.602228 xcsf-1.3.1/lib/pybind11/include/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.686229 xcsf-1.3.1/lib/pybind11/include/pybind11/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    24334 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7750 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    67312 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8458 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      120 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2096 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.686229 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28518 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    53480 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5962 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17859 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28221 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    48364 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1625 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.686229 xcsf-1.3.1/lib/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      378 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/eigen/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    32135 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18442 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      316 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13459 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4731 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5002 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8262 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8862 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    79725 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9103 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2734 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   126706 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    98455 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.686229 xcsf-1.3.1/lib/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4185 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15477 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    29897 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/stl_bind.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1929 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21733 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2584 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1171 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1293 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1685 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1353 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1163 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1368 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tests/test_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tests/test_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/lib/pybind11/tools/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2449 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3105 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11190 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      817 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/JoinPaths.cmake
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1423 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/check-style.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      952 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1117 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1031 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/libsize.py
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1311 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      196 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14449 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7101 2023-07-28 19:46:37.000000 xcsf-1.3.1/lib/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8960 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8361 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       94 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2104 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1234 2023-07-20 10:48:46.000000 xcsf-1.3.1/lib/pybind11/tools/setup_main.py.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-28 19:56:55.698229 xcsf-1.3.1/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4736 2023-07-28 19:41:35.000000 xcsf-1.3.1/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.690229 xcsf-1.3.1/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1633 2023-07-26 13:11:45.000000 xcsf-1.3.1/test/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.698229 xcsf-1.3.1/xcsf/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4641 2023-07-25 09:54:11.000000 xcsf-1.3.1/xcsf/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       20 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10726 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/__init__.pyi
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8230 2023-07-21 15:46:57.000000 xcsf-1.3.1/xcsf/act_integer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2787 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/act_integer.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9843 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/act_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2914 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/act_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5611 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/action.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9383 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/action.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7633 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/blas.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1579 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/blas.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19360 2023-07-26 14:33:11.000000 xcsf-1.3.1/xcsf/cl.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3024 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23381 2023-07-28 17:50:59.000000 xcsf-1.3.1/xcsf/clset.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2361 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/clset.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6348 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/clset_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1636 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/clset_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8819 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2878 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5977 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_dummy.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2643 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_dummy.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13386 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_ellipsoid.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3046 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_ellipsoid.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8983 2023-07-23 18:54:02.000000 xcsf-1.3.1/xcsf/cond_gp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2803 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_gp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11827 2023-07-28 19:32:44.000000 xcsf-1.3.1/xcsf/cond_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3331 2023-07-28 19:33:02.000000 xcsf-1.3.1/xcsf/cond_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15096 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_rectangle.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3097 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_rectangle.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13578 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_ternary.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3221 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/cond_ternary.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13833 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/condition.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12061 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/condition.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2291 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/config.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/config.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23608 2023-07-26 14:33:06.000000 xcsf-1.3.1/xcsf/dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3447 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16230 2023-07-26 14:37:27.000000 xcsf-1.3.1/xcsf/ea.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3096 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/ea.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1675 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/env.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3350 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/env.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7316 2023-07-26 12:44:12.000000 xcsf-1.3.1/xcsf/env_csv.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1679 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/env_csv.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7587 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/env_maze.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2018 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/env_maze.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4060 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/env_mux.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1720 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/env_mux.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18174 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/gp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3137 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/gp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4469 2023-07-23 14:15:37.000000 xcsf-1.3.1/xcsf/image.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1149 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/image.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/loss.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2531 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/loss.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2211 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/main.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14550 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3083 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6333 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_activations.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4420 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_activations.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17673 2023-07-23 15:22:57.000000 xcsf-1.3.1/xcsf/neural_layer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12532 2023-07-26 22:34:30.000000 xcsf-1.3.1/xcsf/neural_layer.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22500 2023-07-26 14:35:17.000000 xcsf-1.3.1/xcsf/neural_layer_args.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3010 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_args.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8550 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_avgpool.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2595 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_avgpool.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15031 2023-07-28 19:40:40.000000 xcsf-1.3.1/xcsf/neural_layer_connected.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2669 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_connected.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21124 2023-07-28 19:40:40.000000 xcsf-1.3.1/xcsf/neural_layer_convolutional.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2869 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_convolutional.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8227 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_dropout.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2578 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_dropout.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    25430 2023-07-21 18:11:28.000000 xcsf-1.3.1/xcsf/neural_layer_lstm.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2479 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_lstm.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11181 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_maxpool.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2587 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_maxpool.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8094 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_noise.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2533 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_noise.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16764 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_recurrent.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2663 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_recurrent.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7627 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_softmax.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2577 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_softmax.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9233 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_upsample.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2620 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/neural_layer_upsample.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pa.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1168 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pa.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28296 2023-07-26 14:36:18.000000 xcsf-1.3.1/xcsf/param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3520 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/param.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1486 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/perf.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      944 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/perf.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6703 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pred_constant.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2542 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pred_constant.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14958 2023-07-28 19:40:40.000000 xcsf-1.3.1/xcsf/pred_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3441 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pred_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12010 2023-07-26 14:33:55.000000 xcsf-1.3.1/xcsf/pred_nlms.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2918 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pred_nlms.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11788 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pred_rls.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3074 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pred_rls.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10334 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/prediction.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10375 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/prediction.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1141 2023-07-23 14:14:12.000000 xcsf-1.3.1/xcsf/pybind_callback.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3955 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pybind_callback_checkpoint.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5460 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pybind_callback_earlystop.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1465 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/pybind_utils.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    38402 2023-07-24 15:22:22.000000 xcsf-1.3.1/xcsf/pybind_wrapper.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7380 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/rule_dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4871 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/rule_dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7916 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/rule_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5047 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/rule_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3796 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/sam.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1216 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/sam.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.698229 xcsf-1.3.1/xcsf/utils/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/utils/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4045 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/utils/types.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5758 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/utils/viz.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3180 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/utils.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4432 2023-07-23 13:24:16.000000 xcsf-1.3.1/xcsf/utils.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8322 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/xcs_rl.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1571 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/xcs_rl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7287 2023-07-26 13:07:59.000000 xcsf-1.3.1/xcsf/xcs_supervised.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1447 2023-07-20 10:48:26.000000 xcsf-1.3.1/xcsf/xcs_supervised.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6318 2023-07-23 13:15:02.000000 xcsf-1.3.1/xcsf/xcsf.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6927 2023-07-28 19:42:14.000000 xcsf-1.3.1/xcsf/xcsf.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-28 19:56:55.698229 xcsf-1.3.1/xcsf.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-28 19:56:55.000000 xcsf-1.3.1/xcsf.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21828 2023-07-28 19:56:55.000000 xcsf-1.3.1/xcsf.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-28 19:56:55.000000 xcsf-1.3.1/xcsf.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-20 10:56:30.000000 xcsf-1.3.1/xcsf.egg-info/not-zip-safe
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       15 2023-07-28 19:56:55.000000 xcsf-1.3.1/xcsf.egg-info/top_level.txt
```

### Comparing `xcsf-1.3.0/CMakeLists.txt` & `xcsf-1.3.1/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 cmake_minimum_required(VERSION 3.12)
 
 project(XCSF CXX C)
 set(PROJECT_VENDOR "Richard Preen")
 set(PROJECT_CONTACT "rpreen@gmail.com")
 set(PROJECT_URL "https://github.com/rpreen/xcsf")
 set(PROJECT_DESCRIPTION "XCSF: Learning Classifier System")
-set(PROJECT_VERSION "1.3.0")
+set(PROJECT_VERSION "1.3.1")
 
 set(CMAKE_C_STANDARD 11)
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_C_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_VERBOSE_MAKEFILE OFF)
 
@@ -35,14 +35,29 @@
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wfatal-errors")
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wcast-qual")
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wredundant-decls")
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Winit-self")
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pedantic")
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wno-unused-function")
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pipe")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wformat")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wformat-security")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wformat-nonliteral")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wformat-y2k")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wformat=2")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wcast-align")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wlogical-op")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wmissing-declarations")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wmissing-prototypes")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wnested-externs")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wold-style-definition")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wpointer-arith")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wshadow")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wstrict-prototypes")
+  set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wundef")
 
   set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -W -Wall -Wextra ")
   set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wunused ")
   set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wfatal-errors")
   set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wcast-qual")
   set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wredundant-decls")
   set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Winit-self")
```

### Comparing `xcsf-1.3.0/LICENSE.md` & `xcsf-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/PKG-INFO` & `xcsf-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsf
-Version: 1.3.0
+Version: 1.3.1
 Summary: XCSF learning classifier system: rule-based evolutionary machine learning
 Home-page: https://github.com/rpreen/xcsf
 Maintainer: Richard Preen
 Maintainer-email: rpreen@gmail.com
 License: GPL-3.0
 Keywords: divide and conquer,evolutionary algorithm,genetic programming,learning classifier system,least squares,machine learning,neural networks,neuroevolution,reinforcement learning,rule-based,supervised learning,stochastic gradient descent,XCS,XCSF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xcsf-1.3.0/README.md` & `xcsf-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/.github/CONTRIBUTING.md` & `xcsf-1.3.1/lib/cJSON/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/.github/workflows/CI.yml` & `xcsf-1.3.1/lib/cJSON/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/.github/workflows/ci-fuzz.yml` & `xcsf-1.3.1/lib/cJSON/.github/workflows/ci-fuzz.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/.travis.yml` & `xcsf-1.3.1/lib/cJSON/.travis.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/CHANGELOG.md` & `xcsf-1.3.1/lib/cJSON/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/CMakeLists.txt` & `xcsf-1.3.1/lib/cJSON/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/CONTRIBUTORS.md` & `xcsf-1.3.1/lib/cJSON/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/LICENSE` & `xcsf-1.3.1/lib/cJSON/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/Makefile` & `xcsf-1.3.1/lib/cJSON/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/README.md` & `xcsf-1.3.1/lib/cJSON/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/appveyor.yml` & `xcsf-1.3.1/lib/cJSON/appveyor.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/cJSON.c` & `xcsf-1.3.1/lib/cJSON/cJSON.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/cJSON.h` & `xcsf-1.3.1/lib/cJSON/cJSON.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/cJSON_Utils.c` & `xcsf-1.3.1/lib/cJSON/cJSON_Utils.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/cJSON_Utils.h` & `xcsf-1.3.1/lib/cJSON/cJSON_Utils.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/CMakeLists.txt` & `xcsf-1.3.1/lib/cJSON/fuzzing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/afl.c` & `xcsf-1.3.1/lib/cJSON/fuzzing/afl.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/cjson_read_fuzzer.c` & `xcsf-1.3.1/lib/cJSON/fuzzing/cjson_read_fuzzer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/fuzz_main.c` & `xcsf-1.3.1/lib/cJSON/fuzzing/fuzz_main.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test1` & `xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test1`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3` & `xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.bu` & `xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3.bu`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uf` & `xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3.uf`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test3.uu` & `xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test3.uu`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test4` & `xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test4`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/inputs/test5` & `xcsf-1.3.1/lib/cJSON/fuzzing/inputs/test5`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/json.dict` & `xcsf-1.3.1/lib/cJSON/fuzzing/json.dict`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/fuzzing/ossfuzz.sh` & `xcsf-1.3.1/lib/cJSON/fuzzing/ossfuzz.sh`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/library_config/cJSONConfig.cmake.in` & `xcsf-1.3.1/lib/cJSON/library_config/cJSONConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/library_config/uninstall.cmake` & `xcsf-1.3.1/lib/cJSON/library_config/uninstall.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/test.c` & `xcsf-1.3.1/lib/cJSON/test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/CMakeLists.txt` & `xcsf-1.3.1/lib/cJSON/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/cjson_add.c` & `xcsf-1.3.1/lib/cJSON/tests/cjson_add.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/common.h` & `xcsf-1.3.1/lib/cJSON/tests/common.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/compare_tests.c` & `xcsf-1.3.1/lib/cJSON/tests/compare_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/inputs/test1` & `xcsf-1.3.1/lib/cJSON/tests/inputs/test1`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/inputs/test3` & `xcsf-1.3.1/lib/cJSON/tests/inputs/test3`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/inputs/test4` & `xcsf-1.3.1/lib/cJSON/tests/inputs/test4`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/inputs/test4.expected` & `xcsf-1.3.1/lib/cJSON/tests/inputs/test4.expected`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/inputs/test5` & `xcsf-1.3.1/lib/cJSON/tests/inputs/test5`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/inputs/test5.expected` & `xcsf-1.3.1/lib/cJSON/tests/inputs/test5.expected`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/README.md` & `xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json` & `xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/spec_tests.json` & `xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/spec_tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/json-patch-tests/tests.json` & `xcsf-1.3.1/lib/cJSON/tests/json-patch-tests/tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/json_patch_tests.c` & `xcsf-1.3.1/lib/cJSON/tests/json_patch_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/minify_tests.c` & `xcsf-1.3.1/lib/cJSON/tests/minify_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/misc_tests.c` & `xcsf-1.3.1/lib/cJSON/tests/misc_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/misc_utils_tests.c` & `xcsf-1.3.1/lib/cJSON/tests/misc_utils_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/old_utils_tests.c` & `xcsf-1.3.1/lib/cJSON/tests/old_utils_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_array.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_array.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_examples.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_examples.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_hex4.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_hex4.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_number.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_number.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_object.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_object.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_string.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_string.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_value.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_value.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/parse_with_opts.c` & `xcsf-1.3.1/lib/cJSON/tests/parse_with_opts.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/print_array.c` & `xcsf-1.3.1/lib/cJSON/tests/print_array.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/print_number.c` & `xcsf-1.3.1/lib/cJSON/tests/print_number.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/print_object.c` & `xcsf-1.3.1/lib/cJSON/tests/print_object.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/print_string.c` & `xcsf-1.3.1/lib/cJSON/tests/print_string.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/print_value.c` & `xcsf-1.3.1/lib/cJSON/tests/print_value.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/readme_examples.c` & `xcsf-1.3.1/lib/cJSON/tests/readme_examples.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/.gitattributes` & `xcsf-1.3.1/lib/cJSON/tests/unity/.gitattributes`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/.travis.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/.travis.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/README.md` & `xcsf-1.3.1/lib/cJSON/tests/unity/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_prompt.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/colour_prompt.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/colour_reporter.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/colour_reporter.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_config.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/generate_config.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_module.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/generate_module.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/generate_test_runner.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/generate_test_runner.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/parse_output.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/parse_output.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/stylize_as_junit.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/stylize_as_junit.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/test_file_filter.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/test_file_filter.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.py` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/unity_test_summary.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_test_summary.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/unity_test_summary.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/auto/unity_to_junit.py` & `xcsf-1.3.1/lib/cJSON/tests/unity/auto/unity_to_junit.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md` & `xcsf-1.3.1/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf` & `xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md` & `xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md` & `xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md` & `xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md` & `xcsf-1.3.1/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/docs/license.txt` & `xcsf-1.3.1/lib/cJSON/tests/unity/docs/license.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/makefile` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/makefile` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/rakefile.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/readme.txt` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/readme.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/examples/unity_config.h` & `xcsf-1.3.1/lib/cJSON/tests/unity/examples/unity_config.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/rakefile.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/readme.txt` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/readme.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/Makefile` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h` & `xcsf-1.3.1/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/src/unity.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/src/unity.h` & `xcsf-1.3.1/lib/cJSON/tests/unity/src/unity.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/src/unity_internals.h` & `xcsf-1.3.1/lib/cJSON/tests/unity/src/unity_internals.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/.rubocop.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/.rubocop.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/Makefile` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_def.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_def.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_param.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_param.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/rakefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/rakefile_helper.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_file.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/clang_file.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/clang_strict.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/clang_strict.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_32.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_32.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_64.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_64.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_msp430.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_msp430.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testparameterized.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/tests/testparameterized.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/cJSON/tests/unity/test/tests/testunity.c` & `xcsf-1.3.1/lib/cJSON/tests/unity/test/tests/testunity.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/CHANGE-LOG.txt` & `xcsf-1.3.1/lib/dSFMT/CHANGE-LOG.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/FILES.txt` & `xcsf-1.3.1/lib/dSFMT/FILES.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/LICENSE.txt` & `xcsf-1.3.1/lib/dSFMT/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/Makefile` & `xcsf-1.3.1/lib/dSFMT/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/Makefile.me` & `xcsf-1.3.1/lib/dSFMT/Makefile.me`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/README.jp.txt` & `xcsf-1.3.1/lib/dSFMT/README.jp.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/README.txt` & `xcsf-1.3.1/lib/dSFMT/README.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-common.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-common.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params11213.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params11213.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params1279.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params1279.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params132049.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params132049.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params19937.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params19937.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params216091.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params216091.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params2203.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params2203.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params4253.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params4253.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params44497.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params44497.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params521.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params521.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-params86243.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT-params86243.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-ref.c` & `xcsf-1.3.1/lib/dSFMT/dSFMT-ref.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.tar.gz` & `xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.0.zip` & `xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.0.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.tar.gz` & `xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.1.zip` & `xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.1.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.tar.gz` & `xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT-src-2.1.zip` & `xcsf-1.3.1/lib/dSFMT/dSFMT-src-2.1.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.11213.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.11213.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.1279.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.1279.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.132049.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.132049.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.19937.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.19937.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.216091.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.216091.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.2203.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.2203.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.4253.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.4253.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.44497.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.44497.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.521.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.521.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.86243.out.txt` & `xcsf-1.3.1/lib/dSFMT/dSFMT.86243.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.c` & `xcsf-1.3.1/lib/dSFMT/dSFMT.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/dSFMT.h` & `xcsf-1.3.1/lib/dSFMT/dSFMT.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/doxygen.cfg` & `xcsf-1.3.1/lib/dSFMT/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/doxygen.cfg.bak` & `xcsf-1.3.1/lib/dSFMT/doxygen.cfg.bak`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/annotated.html` & `xcsf-1.3.1/lib/dSFMT/html/annotated.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/bc_s.png` & `xcsf-1.3.1/lib/dSFMT/html/bc_s.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/classes.html` & `xcsf-1.3.1/lib/dSFMT/html/classes.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8c.html` & `xcsf-1.3.1/lib/dSFMT/html/d_s_f_m_t_8c.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h.html` & `xcsf-1.3.1/lib/dSFMT/html/d_s_f_m_t_8h.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/d_s_f_m_t_8h_source.html` & `xcsf-1.3.1/lib/dSFMT/html/d_s_f_m_t_8h_source.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/doxygen.css` & `xcsf-1.3.1/lib/dSFMT/html/doxygen.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/doxygen.png` & `xcsf-1.3.1/lib/dSFMT/html/doxygen.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/files.html` & `xcsf-1.3.1/lib/dSFMT/html/files.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/functions.html` & `xcsf-1.3.1/lib/dSFMT/html/functions.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/functions_vars.html` & `xcsf-1.3.1/lib/dSFMT/html/functions_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/globals.html` & `xcsf-1.3.1/lib/dSFMT/html/globals.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/globals_defs.html` & `xcsf-1.3.1/lib/dSFMT/html/globals_defs.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/globals_func.html` & `xcsf-1.3.1/lib/dSFMT/html/globals_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/globals_type.html` & `xcsf-1.3.1/lib/dSFMT/html/globals_type.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/globals_vars.html` & `xcsf-1.3.1/lib/dSFMT/html/globals_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/howto-compile.html` & `xcsf-1.3.1/lib/dSFMT/html/howto-compile.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/index.html` & `xcsf-1.3.1/lib/dSFMT/html/index.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/jquery.js` & `xcsf-1.3.1/lib/dSFMT/html/jquery.js`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/mainpage_8txt.html` & `xcsf-1.3.1/lib/dSFMT/html/mainpage_8txt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/struct_d_s_f_m_t___t.html` & `xcsf-1.3.1/lib/dSFMT/html/struct_d_s_f_m_t___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/tabs.css` & `xcsf-1.3.1/lib/dSFMT/html/tabs.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/html/union_w128___t.html` & `xcsf-1.3.1/lib/dSFMT/html/union_w128___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/FILES.txt` & `xcsf-1.3.1/lib/dSFMT/jump/FILES.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/LICENSE.txt` & `xcsf-1.3.1/lib/dSFMT/jump/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/Makefile` & `xcsf-1.3.1/lib/dSFMT/jump/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/Makefile.me` & `xcsf-1.3.1/lib/dSFMT/jump/Makefile.me`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic` & `xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi` & `xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic-mpi`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-mpi.cpp` & `xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic-mpi.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic-old.cpp` & `xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic-old.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/calc-characteristic.cpp` & `xcsf-1.3.1/lib/dSFMT/jump/calc-characteristic.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/calc-jump` & `xcsf-1.3.1/lib/dSFMT/jump/calc-jump`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/calc-jump.cpp` & `xcsf-1.3.1/lib/dSFMT/jump/calc-jump.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/dSFMT-calc-jump.hpp` & `xcsf-1.3.1/lib/dSFMT/jump/dSFMT-calc-jump.hpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.c` & `xcsf-1.3.1/lib/dSFMT/jump/dSFMT-jump.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/dSFMT-jump.h` & `xcsf-1.3.1/lib/dSFMT/jump/dSFMT-jump.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/dSFMText.hpp` & `xcsf-1.3.1/lib/dSFMT/jump/dSFMText.hpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/debug.fix.11213.txt` & `xcsf-1.3.1/lib/dSFMT/jump/debug.fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/debug.txt` & `xcsf-1.3.1/lib/dSFMT/jump/debug.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/degree` & `xcsf-1.3.1/lib/dSFMT/jump/degree`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/degree.cpp` & `xcsf-1.3.1/lib/dSFMT/jump/degree.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/degree.xlsx` & `xcsf-1.3.1/lib/dSFMT/jump/degree.xlsx`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg` & `xcsf-1.3.1/lib/dSFMT/jump/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/doxygen.cfg.bak` & `xcsf-1.3.1/lib/dSFMT/jump/doxygen.cfg.bak`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fac.fix.11213.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fac.fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fac.fix.132049.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fac.fix.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fac.fix.2203.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fac.fix.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.132049.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fac.lcm.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.216091.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fac.lcm.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fac.lcm.2203.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fac.lcm.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/factorization` & `xcsf-1.3.1/lib/dSFMT/jump/factorization`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/factorization.cpp` & `xcsf-1.3.1/lib/dSFMT/jump/factorization.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fix.11213.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fix.132049.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fix.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fix.19937.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fix.19937.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fix.2203.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fix.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fix.44497.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fix.44497.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/fix.86243.txt` & `xcsf-1.3.1/lib/dSFMT/jump/fix.86243.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/annotated.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/annotated.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/bc_s.png` & `xcsf-1.3.1/lib/dSFMT/jump/html/bc_s.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/classes.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/classes.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.css` & `xcsf-1.3.1/lib/dSFMT/jump/html/doxygen.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/doxygen.png` & `xcsf-1.3.1/lib/dSFMT/jump/html/doxygen.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/files.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/files.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/functions.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/functions.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/functions_vars.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/functions_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/globals.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/globals.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/globals_func.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/globals_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/globals_vars.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/globals_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/index.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/index.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/jquery.js` & `xcsf-1.3.1/lib/dSFMT/jump/html/jquery.js`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/mainpage_8txt.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/mainpage_8txt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/namespacedsfmt.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/namespacedsfmt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/namespacemembers.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/namespacemembers_func.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/namespacemembers_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/namespaces.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/namespaces.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/struct_f_i_x___t.html` & `xcsf-1.3.1/lib/dSFMT/jump/html/struct_f_i_x___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/html/tabs.css` & `xcsf-1.3.1/lib/dSFMT/jump/html/tabs.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/lcm.1279.txt` & `xcsf-1.3.1/lib/dSFMT/jump/lcm.1279.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/lcm.132049.tar.gz` & `xcsf-1.3.1/lib/dSFMT/jump/lcm.132049.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.tar.gz` & `xcsf-1.3.1/lib/dSFMT/jump/lcm.216091.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/lcm.216091.txt` & `xcsf-1.3.1/lib/dSFMT/jump/lcm.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/lcm.4253.txt` & `xcsf-1.3.1/lib/dSFMT/jump/lcm.4253.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/lcm.86243.tar.gz` & `xcsf-1.3.1/lib/dSFMT/jump/lcm.86243.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/mainpage.txt` & `xcsf-1.3.1/lib/dSFMT/jump/mainpage.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/params.csv` & `xcsf-1.3.1/lib/dSFMT/jump/params.csv`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.11213.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.132049.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.19937.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.19937.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.216091.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.2203.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.4253.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.4253.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.44497.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.44497.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/poly.86243.txt` & `xcsf-1.3.1/lib/dSFMT/jump/poly.86243.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/readme-jp.html` & `xcsf-1.3.1/lib/dSFMT/jump/readme-jp.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/readme.html` & `xcsf-1.3.1/lib/dSFMT/jump/readme.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/sample1` & `xcsf-1.3.1/lib/dSFMT/jump/sample1`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/sample1.c` & `xcsf-1.3.1/lib/dSFMT/jump/sample1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/sample2` & `xcsf-1.3.1/lib/dSFMT/jump/sample2`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/sample2.c` & `xcsf-1.3.1/lib/dSFMT/jump/sample2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M11213` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M11213`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M1279` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M1279`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M132049` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M132049`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M19937` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M19937`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M216091` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M216091`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M2203` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M2203`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M4253` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M4253`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M44497` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M44497`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M521` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M521`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump-M86243` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump-M86243`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/jump/test-jump.cpp` & `xcsf-1.3.1/lib/dSFMT/jump/test-jump.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/mainpage.txt` & `xcsf-1.3.1/lib/dSFMT/mainpage.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/sample1.c` & `xcsf-1.3.1/lib/dSFMT/sample1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/sample2.c` & `xcsf-1.3.1/lib/dSFMT/sample2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/sample3.c` & `xcsf-1.3.1/lib/dSFMT/sample3.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/sample4.c` & `xcsf-1.3.1/lib/dSFMT/sample4.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/dSFMT/test.c` & `xcsf-1.3.1/lib/dSFMT/test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/CMakeLists.txt` & `xcsf-1.3.1/lib/doctest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/examples/all_features/CMakeLists.txt` & `xcsf-1.3.1/lib/doctest/examples/all_features/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt` & `xcsf-1.3.1/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt` & `xcsf-1.3.1/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake` & `xcsf-1.3.1/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt` & `xcsf-1.3.1/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/scripts/cmake/assemble_single_header.cmake` & `xcsf-1.3.1/lib/doctest/scripts/cmake/assemble_single_header.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/scripts/cmake/common.cmake` & `xcsf-1.3.1/lib/doctest/scripts/cmake/common.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/scripts/cmake/doctest.cmake` & `xcsf-1.3.1/lib/doctest/scripts/cmake/doctest.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/scripts/cmake/doctestAddTests.cmake` & `xcsf-1.3.1/lib/doctest/scripts/cmake/doctestAddTests.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/doctest/scripts/cmake/exec_test.cmake` & `xcsf-1.3.1/lib/doctest/scripts/cmake/exec_test.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # CMakeLists.txt -- Build system for the pybind11 modules
 #
 # Copyright (c) 2015 Wenzel Jakob <wenzel@inf.ethz.ch>
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.22)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.22)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.22)
+  cmake_policy(VERSION 3.26)
 endif()
 
 # Avoid infinite recursion if tests include this as a subdirectory
 if(DEFINED PYBIND11_MASTER_PROJECT)
   return()
 endif()
 
@@ -122,28 +122,30 @@
     include/pybind11/buffer_info.h
     include/pybind11/cast.h
     include/pybind11/chrono.h
     include/pybind11/common.h
     include/pybind11/complex.h
     include/pybind11/options.h
     include/pybind11/eigen.h
+    include/pybind11/eigen/common.h
     include/pybind11/eigen/matrix.h
     include/pybind11/eigen/tensor.h
     include/pybind11/embed.h
     include/pybind11/eval.h
     include/pybind11/gil.h
     include/pybind11/iostream.h
     include/pybind11/functional.h
     include/pybind11/numpy.h
     include/pybind11/operators.h
     include/pybind11/pybind11.h
     include/pybind11/pytypes.h
     include/pybind11/stl.h
     include/pybind11/stl_bind.h
-    include/pybind11/stl/filesystem.h)
+    include/pybind11/stl/filesystem.h
+    include/pybind11/type_caster_pyobject_ptr.h)
 
 # Compare with grep and warn if mismatched
 if(PYBIND11_MASTER_PROJECT AND NOT CMAKE_VERSION VERSION_LESS 3.12)
   file(
     GLOB_RECURSE _pybind11_header_check
     LIST_DIRECTORIES false
     RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}"
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/attr.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/attr.h`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 /// Annotation for methods
 struct is_method {
     handle class_;
     explicit is_method(const handle &c) : class_(c) {}
 };
 
+/// Annotation for setters
+struct is_setter {};
+
 /// Annotation for operators
 struct is_operator {};
 
 /// Annotation for classes that cannot be subclassed
 struct is_final {};
 
 /// Annotation for parent scope
@@ -184,16 +187,16 @@
 };
 
 /// Internal data structure which holds metadata about a bound function (signature, overloads,
 /// etc.)
 struct function_record {
     function_record()
         : is_constructor(false), is_new_style_constructor(false), is_stateless(false),
-          is_operator(false), is_method(false), has_args(false), has_kwargs(false),
-          prepend(false) {}
+          is_operator(false), is_method(false), is_setter(false), has_args(false),
+          has_kwargs(false), prepend(false) {}
 
     /// Function name
     char *name = nullptr; /* why no C++ strings? They generate heavier code.. */
 
     // User-specified documentation string
     char *doc = nullptr;
 
@@ -226,14 +229,17 @@
 
     /// True if this is an operator (__add__), etc.
     bool is_operator : 1;
 
     /// True if this is a method
     bool is_method : 1;
 
+    /// True if this is a setter
+    bool is_setter : 1;
+
     /// True if the function has a '*args' argument
     bool has_args : 1;
 
     /// True if the function has a '**kwargs' argument
     bool has_kwargs : 1;
 
     /// True if this function is to be inserted at the beginning of the overload resolution chain
@@ -422,14 +428,20 @@
 struct process_attribute<is_method> : process_attribute_default<is_method> {
     static void init(const is_method &s, function_record *r) {
         r->is_method = true;
         r->scope = s.class_;
     }
 };
 
+/// Process an attribute which indicates that this function is a setter
+template <>
+struct process_attribute<is_setter> : process_attribute_default<is_setter> {
+    static void init(const is_setter &, function_record *r) { r->is_setter = true; }
+};
+
 /// Process an attribute which indicates the parent scope of a method
 template <>
 struct process_attribute<scope> : process_attribute_default<scope> {
     static void init(const scope &s, function_record *r) { r->scope = s.value; }
 };
 
 /// Process an attribute which indicates that this function is an operator
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/buffer_info.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     std::vector<ssize_t> strides(ndim, itemsize);
     for (size_t i = 1; i < ndim; ++i) {
         strides[i] = strides[i - 1] * shape[i - 1];
     }
     return strides;
 }
 
+template <typename T, typename SFINAE = void>
+struct compare_buffer_info;
+
 PYBIND11_NAMESPACE_END(detail)
 
 /// Information record describing a Python buffer object
 struct buffer_info {
     void *ptr = nullptr;          // Pointer to the underlying storage
     ssize_t itemsize = 0;         // Size of individual items in bytes
     ssize_t size = 0;             // Total number of entries
@@ -146,14 +149,25 @@
             delete m_view;
         }
     }
 
     Py_buffer *view() const { return m_view; }
     Py_buffer *&view() { return m_view; }
 
+    /* True if the buffer item type is equivalent to `T`. */
+    // To define "equivalent" by example:
+    // `buffer_info::item_type_is_equivalent_to<int>(b)` and
+    // `buffer_info::item_type_is_equivalent_to<long>(b)` may both be true
+    // on some platforms, but `int` and `unsigned` will never be equivalent.
+    // For the ground truth, please inspect `detail::compare_buffer_info<>`.
+    template <typename T>
+    bool item_type_is_equivalent_to() const {
+        return detail::compare_buffer_info<T>::compare(*this);
+    }
+
 private:
     struct private_ctr_tag {};
 
     buffer_info(private_ctr_tag,
                 void *ptr,
                 ssize_t itemsize,
                 const std::string &format,
@@ -166,17 +180,18 @@
 
     Py_buffer *m_view = nullptr;
     bool ownview = false;
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <typename T, typename SFINAE = void>
+template <typename T, typename SFINAE>
 struct compare_buffer_info {
     static bool compare(const buffer_info &b) {
+        // NOLINTNEXTLINE(bugprone-sizeof-expression) Needed for `PyObject *`
         return b.format == format_descriptor<T>::format() && b.itemsize == (ssize_t) sizeof(T);
     }
 };
 
 template <typename T>
 struct compare_buffer_info<T, detail::enable_if_t<std::is_integral<T>::value>> {
     static bool compare(const buffer_info &b) {
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/cast.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/cast.h`

 * *Files 2% similar despite different names*

```diff
@@ -960,26 +960,26 @@
 struct move_always : std::false_type {};
 template <typename T>
 struct move_always<
     T,
     enable_if_t<
         all_of<move_is_plain_type<T>,
                negation<is_copy_constructible<T>>,
-               std::is_move_constructible<T>,
+               is_move_constructible<T>,
                std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
     : std::true_type {};
 template <typename T, typename SFINAE = void>
 struct move_if_unreferenced : std::false_type {};
 template <typename T>
 struct move_if_unreferenced<
     T,
     enable_if_t<
         all_of<move_is_plain_type<T>,
                negation<move_always<T>>,
-               std::is_move_constructible<T>,
+               is_move_constructible<T>,
                std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
     : std::true_type {};
 template <typename T>
 using move_never = none_of<move_always<T>, move_if_unreferenced<T>>;
 
 // Detect whether returning a `type` from a cast on type's type_caster is going to result in a
 // reference or pointer to a local variable of the type_caster.  Basically, only
@@ -1013,19 +1013,22 @@
 // Basic python -> C++ casting; throws if casting fails
 template <typename T, typename SFINAE>
 type_caster<T, SFINAE> &load_type(type_caster<T, SFINAE> &conv, const handle &handle) {
     static_assert(!detail::is_pyobject<T>::value,
                   "Internal error: type_caster should only be used for C++ types");
     if (!conv.load(handle, true)) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-        throw cast_error("Unable to cast Python instance to C++ type (#define "
-                         "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
+        throw cast_error(
+            "Unable to cast Python instance of type "
+            + str(type::handle_of(handle)).cast<std::string>()
+            + " to C++ type '?' (#define "
+              "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
 #else
         throw cast_error("Unable to cast Python instance of type "
-                         + (std::string) str(type::handle_of(handle)) + " to C++ type '"
+                         + str(type::handle_of(handle)).cast<std::string>() + " to C++ type '"
                          + type_id<T>() + "'");
 #endif
     }
     return conv;
 }
 // Wrapper around the above that also constructs and returns a type_caster
 template <typename T>
@@ -1034,28 +1037,60 @@
     load_type(conv, handle);
     return conv;
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 // pytype -> C++ type
-template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
+template <typename T,
+          detail::enable_if_t<!detail::is_pyobject<T>::value
+                                  && !detail::is_same_ignoring_cvref<T, PyObject *>::value,
+                              int>
+          = 0>
 T cast(const handle &handle) {
     using namespace detail;
     static_assert(!cast_is_temporary_value_reference<T>::value,
                   "Unable to cast type to reference: value is local to type caster");
     return cast_op<T>(load_type<T>(handle));
 }
 
 // pytype -> pytype (calls converting constructor)
 template <typename T, detail::enable_if_t<detail::is_pyobject<T>::value, int> = 0>
 T cast(const handle &handle) {
     return T(reinterpret_borrow<object>(handle));
 }
 
+// Note that `cast<PyObject *>(obj)` increments the reference count of `obj`.
+// This is necessary for the case that `obj` is a temporary, and could
+// not possibly be different, given
+// 1. the established convention that the passed `handle` is borrowed, and
+// 2. we don't want to force all generic code using `cast<T>()` to special-case
+//    handling of `T` = `PyObject *` (to increment the reference count there).
+// It is the responsibility of the caller to ensure that the reference count
+// is decremented.
+template <typename T,
+          typename Handle,
+          detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value
+                                  && detail::is_same_ignoring_cvref<Handle, handle>::value,
+                              int>
+          = 0>
+T cast(Handle &&handle) {
+    return handle.inc_ref().ptr();
+}
+// To optimize way an inc_ref/dec_ref cycle:
+template <typename T,
+          typename Object,
+          detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value
+                                  && detail::is_same_ignoring_cvref<Object, object>::value,
+                              int>
+          = 0>
+T cast(Object &&obj) {
+    return obj.release().ptr();
+}
+
 // C++ type -> py::object
 template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
 object cast(T &&value,
             return_value_policy policy = return_value_policy::automatic_reference,
             handle parent = handle()) {
     using no_ref_T = typename std::remove_reference<T>::type;
     if (policy == return_value_policy::automatic) {
@@ -1081,20 +1116,21 @@
 }
 
 template <typename T>
 detail::enable_if_t<!detail::move_never<T>::value, T> move(object &&obj) {
     if (obj.ref_count() > 1) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
         throw cast_error(
-            "Unable to cast Python instance to C++ rvalue: instance has multiple references"
-            " (#define PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
+            "Unable to cast Python " + str(type::handle_of(obj)).cast<std::string>()
+            + " instance to C++ rvalue: instance has multiple references"
+              " (#define PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
 #else
-        throw cast_error("Unable to move from Python " + (std::string) str(type::handle_of(obj))
-                         + " instance to C++ " + type_id<T>()
-                         + " instance: instance has multiple references");
+        throw cast_error("Unable to move from Python "
+                         + str(type::handle_of(obj)).cast<std::string>() + " instance to C++ "
+                         + type_id<T>() + " instance: instance has multiple references");
 #endif
     }
 
     // Move into a temporary and return that, because the reference may be a local value of `conv`
     T ret = std::move(detail::load_type<T>(obj).operator T &());
     return ret;
 }
@@ -1191,17 +1227,18 @@
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 // The overloads could coexist, i.e. the #if is not strictly speaking needed,
 // but it is an easy minor optimization.
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-inline cast_error cast_error_unable_to_convert_call_arg() {
-    return cast_error("Unable to convert call argument to Python object (#define "
-                      "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
+inline cast_error cast_error_unable_to_convert_call_arg(const std::string &name) {
+    return cast_error("Unable to convert call argument '" + name
+                      + "' to Python object (#define "
+                        "PYBIND11_DETAILED_ERROR_MESSAGES or compile in debug mode for details)");
 }
 #else
 inline cast_error cast_error_unable_to_convert_call_arg(const std::string &name,
                                                         const std::string &type) {
     return cast_error("Unable to convert call argument '" + name + "' of type '" + type
                       + "' to Python object");
 }
@@ -1216,15 +1253,15 @@
 tuple make_tuple(Args &&...args_) {
     constexpr size_t size = sizeof...(Args);
     std::array<object, size> args{{reinterpret_steal<object>(
         detail::make_caster<Args>::cast(std::forward<Args>(args_), policy, nullptr))...}};
     for (size_t i = 0; i < args.size(); i++) {
         if (!args[i]) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-            throw cast_error_unable_to_convert_call_arg();
+            throw cast_error_unable_to_convert_call_arg(std::to_string(i));
 #else
             std::array<std::string, size> argtypes{{type_id<Args>()...}};
             throw cast_error_unable_to_convert_call_arg(std::to_string(i), argtypes[i]);
 #endif
         }
     }
     tuple result(size);
@@ -1506,15 +1543,15 @@
 private:
     template <typename T>
     void process(list &args_list, T &&x) {
         auto o = reinterpret_steal<object>(
             detail::make_caster<T>::cast(std::forward<T>(x), policy, {}));
         if (!o) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-            throw cast_error_unable_to_convert_call_arg();
+            throw cast_error_unable_to_convert_call_arg(std::to_string(args_list.size()));
 #else
             throw cast_error_unable_to_convert_call_arg(std::to_string(args_list.size()),
                                                         type_id<T>());
 #endif
         }
         args_list.append(std::move(o));
     }
@@ -1538,15 +1575,15 @@
             multiple_values_error();
 #else
             multiple_values_error(a.name);
 #endif
         }
         if (!a.value) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
-            throw cast_error_unable_to_convert_call_arg();
+            throw cast_error_unable_to_convert_call_arg(a.name);
 #else
             throw cast_error_unable_to_convert_call_arg(a.name, a.type);
 #endif
         }
         m_kwargs[a.name] = std::move(a.value);
     }
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/chrono.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/complex.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/class.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/common.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/detail/common.h`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
-#define PYBIND11_VERSION_MINOR 10
-#define PYBIND11_VERSION_PATCH 4
+#define PYBIND11_VERSION_MINOR 11
+#define PYBIND11_VERSION_PATCH 1
 
 // Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
 // Additional convention: 0xD = dev
-#define PYBIND11_VERSION_HEX 0x020A0400
+#define PYBIND11_VERSION_HEX 0x020B0100
 
 // Define some generic pybind11 helper macros for warning management.
 //
 // Note that compiler-specific push/pop pairs are baked into the
 // PYBIND11_NAMESPACE_BEGIN/PYBIND11_NAMESPACE_END pair of macros. Therefore manual
 // PYBIND11_WARNING_PUSH/PYBIND11_WARNING_POP are usually only needed in `#include` sections.
 //
@@ -320,21 +320,17 @@
 
 // Must be after including <version> or one of the other headers specified by the standard
 #if defined(__cpp_lib_char8_t) && __cpp_lib_char8_t >= 201811L
 #    define PYBIND11_HAS_U8STRING
 #endif
 
 // See description of PR #4246:
-#if !defined(NDEBUG) && !defined(PY_ASSERT_GIL_HELD_INCREF_DECREF)                                \
-    && !(defined(PYPY_VERSION)                                                                    \
-         && defined(_MSC_VER)) /* PyPy Windows: pytest hangs indefinitely at the end of the       \
-                                  process (see PR #4268) */                                       \
-    && !defined(PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF)
-// The following define will be enabled by default in the 2.11 release
-// define PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+#if !defined(PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF) && !defined(NDEBUG)                       \
+    && !defined(PYPY_VERSION) && !defined(PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF)
+#    define PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
 #endif
 
 // #define PYBIND11_STR_LEGACY_PERMISSIVE
 // If DEFINED, pybind11::str can hold PyUnicodeObject or PyBytesObject
 //             (probably surprising and never documented, but this was the
 //             legacy behavior until and including v2.6.x). As a side-effect,
 //             pybind11::isinstance<str>() is true for both pybind11::str and
@@ -658,14 +654,18 @@
 struct remove_cvref {
     using type = remove_cv_t<remove_reference_t<T>>;
 };
 template <class T>
 using remove_cvref_t = typename remove_cvref<T>::type;
 #endif
 
+/// Example usage: is_same_ignoring_cvref<T, PyObject *>::value
+template <typename T, typename U>
+using is_same_ignoring_cvref = std::is_same<detail::remove_cvref_t<T>, U>;
+
 /// Index sequences
 #if defined(PYBIND11_CPP14)
 using std::index_sequence;
 using std::make_index_sequence;
 #else
 template <size_t...>
 struct index_sequence {};
@@ -751,15 +751,24 @@
 struct remove_class<R (C::*)(A...)> {
     using type = R(A...);
 };
 template <typename C, typename R, typename... A>
 struct remove_class<R (C::*)(A...) const> {
     using type = R(A...);
 };
-
+#ifdef __cpp_noexcept_function_type
+template <typename C, typename R, typename... A>
+struct remove_class<R (C::*)(A...) noexcept> {
+    using type = R(A...);
+};
+template <typename C, typename R, typename... A>
+struct remove_class<R (C::*)(A...) const noexcept> {
+    using type = R(A...);
+};
+#endif
 /// Helper template to strip away type modifiers
 template <typename T>
 struct intrinsic_type {
     using type = T;
 };
 template <typename T>
 struct intrinsic_type<const T> {
@@ -1009,14 +1018,23 @@
     assert(!PyErr_Occurred());
     throw std::runtime_error(reason);
 }
 
 template <typename T, typename SFINAE = void>
 struct format_descriptor {};
 
+template <typename T>
+struct format_descriptor<
+    T,
+    detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value>> {
+    static constexpr const char c = 'O';
+    static constexpr const char value[2] = {c, '\0'};
+    static std::string format() { return std::string(1, c); }
+};
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Returns the index of the given type in the type char array below, and in the list in numpy.h
 // The order here is: bool; 8 ints ((signed,unsigned)x(8,16,32,64)bits); float,double,long double;
 // complex float,double,long double.  Note that the long double types only participate when long
 // double is actually longer than double (it isn't under MSVC).
 // NB: not only the string below but also complex.h and numpy.h rely on this order.
 template <typename T, typename SFINAE = void>
@@ -1222,15 +1240,16 @@
 // test_kwargs_and_defaults.cpp:46:68: note: call 'std::move' explicitly to avoid copying
 //     m.def("args_function", [](py::args args) -> py::tuple { return args; });
 //                                                                    ^~~~
 //                                                                    std::move(args)
 #endif
 
 // Pybind offers detailed error messages by default for all builts that are debug (through the
-// negation of ndebug). This can also be manually enabled by users, for any builds, through
-// defining PYBIND11_DETAILED_ERROR_MESSAGES.
+// negation of NDEBUG). This can also be manually enabled by users, for any builds, through
+// defining PYBIND11_DETAILED_ERROR_MESSAGES. This information is primarily useful for those
+// who are writing (as opposed to merely using) libraries that use pybind11.
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES) && !defined(NDEBUG)
 #    define PYBIND11_DETAILED_ERROR_MESSAGES
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/descr.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files 4% similar despite different names*

```diff
@@ -139,19 +139,32 @@
 constexpr descr<0> concat() { return {}; }
 
 template <size_t N, typename... Ts>
 constexpr descr<N, Ts...> concat(const descr<N, Ts...> &descr) {
     return descr;
 }
 
+#ifdef __cpp_fold_expressions
+template <size_t N1, size_t N2, typename... Ts1, typename... Ts2>
+constexpr descr<N1 + N2 + 2, Ts1..., Ts2...> operator,(const descr<N1, Ts1...> &a,
+                                                       const descr<N2, Ts2...> &b) {
+    return a + const_name(", ") + b;
+}
+
+template <size_t N, typename... Ts, typename... Args>
+constexpr auto concat(const descr<N, Ts...> &d, const Args &...args) {
+    return (d, ..., args);
+}
+#else
 template <size_t N, typename... Ts, typename... Args>
 constexpr auto concat(const descr<N, Ts...> &d, const Args &...args)
     -> decltype(std::declval<descr<N + 2, Ts...>>() + concat(args...)) {
     return d + const_name(", ") + concat(args...);
 }
+#endif
 
 template <size_t N, typename... Ts>
 constexpr descr<N + 2, Ts...> type_descr(const descr<N, Ts...> &descr) {
     return const_name("{") + descr + const_name("}");
 }
 
 PYBIND11_NAMESPACE_END(detail)
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/init.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/detail/init.h`

 * *Files 0% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 // return-by-value version 1: returning a cpp class by value.  If the class has an alias and an
 // alias is required the alias must have an `Alias(Cpp &&)` constructor so that we can construct
 // the alias from the base when needed (i.e. because of Python-side inheritance).  When we don't
 // need it, we simply move-construct the cpp value into a new instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> &&result, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
-    static_assert(std::is_move_constructible<Cpp<Class>>::value,
+    static_assert(is_move_constructible<Cpp<Class>>::value,
                   "pybind11::init() return-by-value factory function requires a movable class");
     if (Class::has_alias && need_alias) {
         construct_alias_from_cpp<Class>(is_alias_constructible<Class>{}, v_h, std::move(result));
     } else {
         v_h.value_ptr() = new Cpp<Class>(std::move(result));
     }
 }
 
 // return-by-value version 2: returning a value of the alias type itself.  We move-construct an
 // Alias instance (even if no the python-side inheritance is involved).  The is intended for
 // cases where Alias initialization is always desired.
 template <typename Class>
 void construct(value_and_holder &v_h, Alias<Class> &&result, bool) {
     static_assert(
-        std::is_move_constructible<Alias<Class>>::value,
+        is_move_constructible<Alias<Class>>::value,
         "pybind11::init() return-by-alias-value factory function requires a movable alias class");
     v_h.value_ptr() = new Alias<Class>(std::move(result));
 }
 
 // Implementing class for py::init<...>()
 template <typename... Args>
 struct constructor {
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/internals.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,26 @@
 /// newer ABI.
 ///
 /// WARNING: If you choose to manually increase the ABI version, note that
 /// pybind11 may not be tested as thoroughly with a non-default ABI version, and
 /// further ABI-incompatible changes may be made before the ABI is officially
 /// changed to the new version.
 #ifndef PYBIND11_INTERNALS_VERSION
-#    define PYBIND11_INTERNALS_VERSION 4
+#    if PY_VERSION_HEX >= 0x030C0000
+// Version bump for Python 3.12+, before first 3.12 beta release.
+#        define PYBIND11_INTERNALS_VERSION 5
+#    else
+#        define PYBIND11_INTERNALS_VERSION 4
+#    endif
 #endif
 
+// This requirement is mainly to reduce the support burden (see PR #4570).
+static_assert(PY_VERSION_HEX < 0x030C0000 || PYBIND11_INTERNALS_VERSION >= 5,
+              "pybind11 ABI version 5 is the minimum for Python 3.12+");
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 using ExceptionTranslator = void (*)(std::exception_ptr);
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 constexpr const char *internals_function_record_capsule_name = "pybind11_function_record_capsule";
@@ -110,15 +119,16 @@
 
 // Python loads modules by default with dlopen with the RTLD_LOCAL flag; under libc++ and possibly
 // other STLs, this means `typeid(A)` from one module won't equal `typeid(A)` from another module
 // even when `A` is the same, non-hidden-visibility type (e.g. from a common include).  Under
 // libstdc++, this doesn't happen: equality and the type_index hash are based on the type name,
 // which works.  If not under a known-good stl, provide our own name-based hash and equality
 // functions that use the type name.
-#if defined(__GLIBCXX__)
+#if (PYBIND11_INTERNALS_VERSION <= 4 && defined(__GLIBCXX__))                                     \
+    || (PYBIND11_INTERNALS_VERSION >= 5 && !defined(_LIBCPP_VERSION))
 inline bool same_type(const std::type_info &lhs, const std::type_info &rhs) { return lhs == rhs; }
 using type_hash = std::hash<std::type_index>;
 using type_equal_to = std::equal_to<std::type_index>;
 #else
 inline bool same_type(const std::type_info &lhs, const std::type_info &rhs) {
     return lhs.name() == rhs.name() || std::strcmp(lhs.name(), rhs.name()) == 0;
 }
@@ -417,14 +427,46 @@
     } catch (const builtin_exception &e) {
         e.set_error();
         return;
     }
 }
 #endif
 
+inline object get_python_state_dict() {
+    object state_dict;
+#if PYBIND11_INTERNALS_VERSION <= 4 || PY_VERSION_HEX < 0x03080000 || defined(PYPY_VERSION)
+    state_dict = reinterpret_borrow<object>(PyEval_GetBuiltins());
+#else
+#    if PY_VERSION_HEX < 0x03090000
+    PyInterpreterState *istate = _PyInterpreterState_Get();
+#    else
+    PyInterpreterState *istate = PyInterpreterState_Get();
+#    endif
+    if (istate) {
+        state_dict = reinterpret_borrow<object>(PyInterpreterState_GetDict(istate));
+    }
+#endif
+    if (!state_dict) {
+        raise_from(PyExc_SystemError, "pybind11::detail::get_python_state_dict() FAILED");
+    }
+    return state_dict;
+}
+
+inline object get_internals_obj_from_state_dict(handle state_dict) {
+    return reinterpret_borrow<object>(dict_getitemstring(state_dict.ptr(), PYBIND11_INTERNALS_ID));
+}
+
+inline internals **get_internals_pp_from_capsule(handle obj) {
+    void *raw_ptr = PyCapsule_GetPointer(obj.ptr(), /*name=*/nullptr);
+    if (raw_ptr == nullptr) {
+        raise_from(PyExc_SystemError, "pybind11::detail::get_internals_pp_from_capsule() FAILED");
+    }
+    return static_cast<internals **>(raw_ptr);
+}
+
 /// Return a reference to the current `internals` data
 PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
     if (internals_pp && *internals_pp) {
         return **internals_pp;
     }
 
@@ -441,20 +483,20 @@
         ~gil_scoped_acquire_local() { PyGILState_Release(state); }
         const PyGILState_STATE state;
     } gil;
 #    endif
 #endif
     error_scope err_scope;
 
-    PYBIND11_STR_TYPE id(PYBIND11_INTERNALS_ID);
-    auto builtins = handle(PyEval_GetBuiltins());
-    if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
-        internals_pp = static_cast<internals **>(capsule(builtins[id]));
-
-        // We loaded builtins through python's builtins, which means that our `error_already_set`
+    dict state_dict = get_python_state_dict();
+    if (object internals_obj = get_internals_obj_from_state_dict(state_dict)) {
+        internals_pp = get_internals_pp_from_capsule(internals_obj);
+    }
+    if (internals_pp && *internals_pp) {
+        // We loaded the internals through `state_dict`, which means that our `error_already_set`
         // and `builtin_exception` may be different local classes than the ones set up in the
         // initial exception translator, below, so add another for our local exception classes.
         //
         // libstdc++ doesn't require this (types there are identified only by name)
         // libc++ with CPython doesn't require this (types are explicitly exported)
         // libc++ with PyPy still need it, awaiting further investigation
 #if !defined(__GLIBCXX__)
@@ -465,28 +507,30 @@
             internals_pp = new internals *();
         }
         auto *&internals_ptr = *internals_pp;
         internals_ptr = new internals();
 #if defined(WITH_THREAD)
 
         PyThreadState *tstate = PyThreadState_Get();
+        // NOLINTNEXTLINE(bugprone-assignment-in-if-condition)
         if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->tstate)) {
             pybind11_fail("get_internals: could not successfully initialize the tstate TSS key!");
         }
         PYBIND11_TLS_REPLACE_VALUE(internals_ptr->tstate, tstate);
 
 #    if PYBIND11_INTERNALS_VERSION > 4
+        // NOLINTNEXTLINE(bugprone-assignment-in-if-condition)
         if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->loader_life_support_tls_key)) {
             pybind11_fail("get_internals: could not successfully initialize the "
                           "loader_life_support TSS key!");
         }
 #    endif
         internals_ptr->istate = tstate->interp;
 #endif
-        builtins[id] = capsule(internals_pp);
+        state_dict[PYBIND11_INTERNALS_ID] = capsule(internals_pp);
         internals_ptr->registered_exception_translators.push_front(&translate_exception);
         internals_ptr->static_property_type = make_static_property_type();
         internals_ptr->default_metaclass = make_default_metaclass();
         internals_ptr->instance_base = make_object_base_type(internals_ptr->default_metaclass);
     }
     return **internals_pp;
 }
@@ -510,14 +554,15 @@
     // plausible number).
     PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
 
     // Holds the shared TLS key for the loader_life_support stack.
     struct shared_loader_life_support_data {
         PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
         shared_loader_life_support_data() {
+            // NOLINTNEXTLINE(bugprone-assignment-in-if-condition)
             if (!PYBIND11_TLS_KEY_CREATE(loader_life_support_tls_key)) {
                 pybind11_fail("local_internals: could not successfully initialize the "
                               "loader_life_support TLS key!");
             }
         }
         // We can't help but leak the TLS key, because Python never unloads extension modules.
     };
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files 7% similar despite different names*

```diff
@@ -254,17 +254,17 @@
     instance *inst = nullptr;
     size_t index = 0u;
     const detail::type_info *type = nullptr;
     void **vh = nullptr;
 
     // Main constructor for a found value/holder:
     value_and_holder(instance *i, const detail::type_info *type, size_t vpos, size_t index)
-        : inst{i}, index{index}, type{type}, vh{inst->simple_layout
-                                                    ? inst->simple_value_holder
-                                                    : &inst->nonsimple.values_and_holders[vpos]} {}
+        : inst{i}, index{index}, type{type},
+          vh{inst->simple_layout ? inst->simple_value_holder
+                                 : &inst->nonsimple.values_and_holders[vpos]} {}
 
     // Default constructor (used to signal a value-and-holder not found by get_value_and_holder())
     value_and_holder() = default;
 
     // Used for past-the-end iterator
     explicit value_and_holder(size_t index) : index{index} {}
 
@@ -818,49 +818,207 @@
 using movable_cast_op_type
     = conditional_t<std::is_pointer<typename std::remove_reference<T>::type>::value,
                     typename std::add_pointer<intrinsic_t<T>>::type,
                     conditional_t<std::is_rvalue_reference<T>::value,
                                   typename std::add_rvalue_reference<intrinsic_t<T>>::type,
                                   typename std::add_lvalue_reference<intrinsic_t<T>>::type>>;
 
-// std::is_copy_constructible isn't quite enough: it lets std::vector<T> (and similar) through when
-// T is non-copyable, but code containing such a copy constructor fails to actually compile.
-template <typename T, typename SFINAE = void>
-struct is_copy_constructible : std::is_copy_constructible<T> {};
+// Does the container have a mapped type and is it recursive?
+// Implemented by specializations below.
+template <typename Container, typename SFINAE = void>
+struct container_mapped_type_traits {
+    static constexpr bool has_mapped_type = false;
+    static constexpr bool has_recursive_mapped_type = false;
+};
+
+template <typename Container>
+struct container_mapped_type_traits<
+    Container,
+    typename std::enable_if<
+        std::is_same<typename Container::mapped_type, Container>::value>::type> {
+    static constexpr bool has_mapped_type = true;
+    static constexpr bool has_recursive_mapped_type = true;
+};
+
+template <typename Container>
+struct container_mapped_type_traits<
+    Container,
+    typename std::enable_if<
+        negation<std::is_same<typename Container::mapped_type, Container>>::value>::type> {
+    static constexpr bool has_mapped_type = true;
+    static constexpr bool has_recursive_mapped_type = false;
+};
+
+// Does the container have a value type and is it recursive?
+// Implemented by specializations below.
+template <typename Container, typename SFINAE = void>
+struct container_value_type_traits : std::false_type {
+    static constexpr bool has_value_type = false;
+    static constexpr bool has_recursive_value_type = false;
+};
+
+template <typename Container>
+struct container_value_type_traits<
+    Container,
+    typename std::enable_if<
+        std::is_same<typename Container::value_type, Container>::value>::type> {
+    static constexpr bool has_value_type = true;
+    static constexpr bool has_recursive_value_type = true;
+};
+
+template <typename Container>
+struct container_value_type_traits<
+    Container,
+    typename std::enable_if<
+        negation<std::is_same<typename Container::value_type, Container>>::value>::type> {
+    static constexpr bool has_value_type = true;
+    static constexpr bool has_recursive_value_type = false;
+};
+
+/*
+ * Tag to be used for representing the bottom of recursively defined types.
+ * Define this tag so we don't have to use void.
+ */
+struct recursive_bottom {};
+
+/*
+ * Implementation detail of `recursive_container_traits` below.
+ * `T` is the `value_type` of the container, which might need to be modified to
+ * avoid recursive types and const types.
+ */
+template <typename T, bool is_this_a_map>
+struct impl_type_to_check_recursively {
+    /*
+     * If the container is recursive, then no further recursion should be done.
+     */
+    using if_recursive = recursive_bottom;
+    /*
+     * Otherwise yield `T` unchanged.
+     */
+    using if_not_recursive = T;
+};
+
+/*
+ * For pairs - only as value type of a map -, the first type should remove the `const`.
+ * Also, if the map is recursive, then the recursive checking should consider
+ * the first type only.
+ */
+template <typename A, typename B>
+struct impl_type_to_check_recursively<std::pair<A, B>, /* is_this_a_map = */ true> {
+    using if_recursive = typename std::remove_const<A>::type;
+    using if_not_recursive = std::pair<typename std::remove_const<A>::type, B>;
+};
+
+/*
+ * Implementation of `recursive_container_traits` below.
+ */
+template <typename Container, typename SFINAE = void>
+struct impl_recursive_container_traits {
+    using type_to_check_recursively = recursive_bottom;
+};
 
-// Specialization for types that appear to be copy constructible but also look like stl containers
-// (we specifically check for: has `value_type` and `reference` with `reference = value_type&`): if
-// so, copy constructability depends on whether the value_type is copy constructible.
 template <typename Container>
-struct is_copy_constructible<
+struct impl_recursive_container_traits<
     Container,
-    enable_if_t<
-        all_of<std::is_copy_constructible<Container>,
-               std::is_same<typename Container::value_type &, typename Container::reference>,
-               // Avoid infinite recursion
-               negation<std::is_same<Container, typename Container::value_type>>>::value>>
-    : is_copy_constructible<typename Container::value_type> {};
+    typename std::enable_if<container_value_type_traits<Container>::has_value_type>::type> {
+    static constexpr bool is_recursive
+        = container_mapped_type_traits<Container>::has_recursive_mapped_type
+          || container_value_type_traits<Container>::has_recursive_value_type;
+    /*
+     * This member dictates which type Pybind11 should check recursively in traits
+     * such as `is_move_constructible`, `is_copy_constructible`, `is_move_assignable`, ...
+     * Direct access to `value_type` should be avoided:
+     * 1. `value_type` might recursively contain the type again
+     * 2. `value_type` of STL map types is `std::pair<A const, B>`, the `const`
+     *    should be removed.
+     *
+     */
+    using type_to_check_recursively = typename std::conditional<
+        is_recursive,
+        typename impl_type_to_check_recursively<
+            typename Container::value_type,
+            container_mapped_type_traits<Container>::has_mapped_type>::if_recursive,
+        typename impl_type_to_check_recursively<
+            typename Container::value_type,
+            container_mapped_type_traits<Container>::has_mapped_type>::if_not_recursive>::type;
+};
+
+/*
+ * This trait defines the `type_to_check_recursively` which is needed to properly
+ * handle recursively defined traits such as `is_move_constructible` without going
+ * into an infinite recursion.
+ * Should be used instead of directly accessing the `value_type`.
+ * It cancels the recursion by returning the `recursive_bottom` tag.
+ *
+ * The default definition of `type_to_check_recursively` is as follows:
+ *
+ * 1. By default, it is `recursive_bottom`, so that the recursion is canceled.
+ * 2. If the type is non-recursive and defines a `value_type`, then the `value_type` is used.
+ *    If the `value_type` is a pair and a `mapped_type` is defined,
+ *    then the `const` is removed from the first type.
+ * 3. If the type is recursive and `value_type` is not a pair, then `recursive_bottom` is returned.
+ * 4. If the type is recursive and `value_type` is a pair and a `mapped_type` is defined,
+ *    then `const` is removed from the first type and the first type is returned.
+ *
+ * This behavior can be extended by the user as seen in test_stl_binders.cpp.
+ *
+ * This struct is exactly the same as impl_recursive_container_traits.
+ * The duplication achieves that user-defined specializations don't compete
+ * with internal specializations, but take precedence.
+ */
+template <typename Container, typename SFINAE = void>
+struct recursive_container_traits : impl_recursive_container_traits<Container> {};
+
+template <typename T>
+struct is_move_constructible
+    : all_of<std::is_move_constructible<T>,
+             is_move_constructible<
+                 typename recursive_container_traits<T>::type_to_check_recursively>> {};
+
+template <>
+struct is_move_constructible<recursive_bottom> : std::true_type {};
+
+// Likewise for std::pair
+// (after C++17 it is mandatory that the move constructor not exist when the two types aren't
+// themselves move constructible, but this can not be relied upon when T1 or T2 are themselves
+// containers).
+template <typename T1, typename T2>
+struct is_move_constructible<std::pair<T1, T2>>
+    : all_of<is_move_constructible<T1>, is_move_constructible<T2>> {};
+
+// std::is_copy_constructible isn't quite enough: it lets std::vector<T> (and similar) through when
+// T is non-copyable, but code containing such a copy constructor fails to actually compile.
+template <typename T>
+struct is_copy_constructible
+    : all_of<std::is_copy_constructible<T>,
+             is_copy_constructible<
+                 typename recursive_container_traits<T>::type_to_check_recursively>> {};
+
+template <>
+struct is_copy_constructible<recursive_bottom> : std::true_type {};
 
 // Likewise for std::pair
 // (after C++17 it is mandatory that the copy constructor not exist when the two types aren't
 // themselves copy constructible, but this can not be relied upon when T1 or T2 are themselves
 // containers).
 template <typename T1, typename T2>
 struct is_copy_constructible<std::pair<T1, T2>>
     : all_of<is_copy_constructible<T1>, is_copy_constructible<T2>> {};
 
 // The same problems arise with std::is_copy_assignable, so we use the same workaround.
-template <typename T, typename SFINAE = void>
-struct is_copy_assignable : std::is_copy_assignable<T> {};
-template <typename Container>
-struct is_copy_assignable<Container,
-                          enable_if_t<all_of<std::is_copy_assignable<Container>,
-                                             std::is_same<typename Container::value_type &,
-                                                          typename Container::reference>>::value>>
-    : is_copy_assignable<typename Container::value_type> {};
+template <typename T>
+struct is_copy_assignable
+    : all_of<
+          std::is_copy_assignable<T>,
+          is_copy_assignable<typename recursive_container_traits<T>::type_to_check_recursively>> {
+};
+
+template <>
+struct is_copy_assignable<recursive_bottom> : std::true_type {};
+
 template <typename T1, typename T2>
 struct is_copy_assignable<std::pair<T1, T2>>
     : all_of<is_copy_assignable<T1>, is_copy_assignable<T2>> {};
 
 PYBIND11_NAMESPACE_END(detail)
 
 // polymorphic_type_hook<itype>::get(src, tinfo) determines whether the object pointed
@@ -990,15 +1148,15 @@
        decltype argument to apply SFINAE to the public copy/move constructors.*/
     template <typename T, typename = enable_if_t<is_copy_constructible<T>::value>>
     static auto make_copy_constructor(const T *)
         -> decltype(new T(std::declval<const T>()), Constructor{}) {
         return [](const void *arg) -> void * { return new T(*reinterpret_cast<const T *>(arg)); };
     }
 
-    template <typename T, typename = enable_if_t<std::is_move_constructible<T>::value>>
+    template <typename T, typename = enable_if_t<is_move_constructible<T>::value>>
     static auto make_move_constructor(const T *)
         -> decltype(new T(std::declval<T &&>()), Constructor{}) {
         return [](const void *arg) -> void * {
             return new T(std::move(*const_cast<T *>(reinterpret_cast<const T *>(arg))));
         };
     }
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/detail/typeid.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/matrix.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/eigen/matrix.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "../numpy.h"
+#include "common.h"
 
 /* HINT: To suppress warnings originating from the Eigen headers, use -isystem.
    See also:
        https://stackoverflow.com/questions/2579576/i-dir-vs-isystem-dir
        https://stackoverflow.com/questions/1741816/isystem-for-ms-visual-studio-c-compiler
 */
 PYBIND11_WARNING_PUSH
@@ -283,14 +284,16 @@
 }
 
 // Type caster for regular, dense matrix types (e.g. MatrixXd), but not maps/refs/etc. of dense
 // types.
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_dense_plain<Type>::value>> {
     using Scalar = typename Type::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using props = EigenProps<Type>;
 
     bool load(handle src, bool convert) {
         // If we're in no-convert mode, only load if given an array of the correct type
         if (!convert && !isinstance<array_t<Scalar>>(src)) {
             return false;
         }
@@ -401,14 +404,17 @@
 private:
     Type value;
 };
 
 // Base class for casting reference/map/block/etc. objects back to python.
 template <typename MapType>
 struct eigen_map_caster {
+    static_assert(!std::is_pointer<typename MapType::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
+
 private:
     using props = EigenProps<MapType>;
 
 public:
     // Directly referencing a ref/map's data is a bit dangerous (whatever the map/ref points to has
     // to stay around), but we'll allow it under the assumption that you know what you're doing
     // (and have an appropriate keep_alive in place).  We return a numpy array pointing directly at
@@ -453,14 +459,16 @@
     Eigen::Ref<PlainObjectType, 0, StrideType>,
     enable_if_t<is_eigen_dense_map<Eigen::Ref<PlainObjectType, 0, StrideType>>::value>>
     : public eigen_map_caster<Eigen::Ref<PlainObjectType, 0, StrideType>> {
 private:
     using Type = Eigen::Ref<PlainObjectType, 0, StrideType>;
     using props = EigenProps<Type>;
     using Scalar = typename props::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using MapType = Eigen::Map<PlainObjectType, 0, StrideType>;
     using Array
         = array_t<Scalar,
                   array::forcecast
                       | ((props::row_major ? props::inner_stride : props::outer_stride) == 1
                              ? array::c_style
                          : (props::row_major ? props::outer_stride : props::inner_stride) == 1
@@ -600,14 +608,17 @@
 
 // type_caster for special matrix types (e.g. DiagonalMatrix), which are EigenBase, but not
 // EigenDense (i.e. they don't have a data(), at least not with the usual matrix layout).
 // load() is not supported, but we can cast them into the python domain by first copying to a
 // regular Eigen::Matrix, then casting that.
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_other<Type>::value>> {
+    static_assert(!std::is_pointer<typename Type::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
+
 protected:
     using Matrix
         = Eigen::Matrix<typename Type::Scalar, Type::RowsAtCompileTime, Type::ColsAtCompileTime>;
     using props = EigenProps<Matrix>;
 
 public:
     static handle cast(const Type &src, return_value_policy /* policy */, handle /* parent */) {
@@ -628,14 +639,16 @@
     template <typename>
     using cast_op_type = Type;
 };
 
 template <typename Type>
 struct type_caster<Type, enable_if_t<is_eigen_sparse<Type>::value>> {
     using Scalar = typename Type::Scalar;
+    static_assert(!std::is_pointer<Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using StorageIndex = remove_reference_t<decltype(*std::declval<Type>().outerIndexPtr())>;
     using Index = typename Type::Index;
     static constexpr bool rowMajor = Type::IsRowMajor;
 
     bool load(handle src, bool) {
         if (!src) {
             return false;
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/eigen/tensor.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/eigen/tensor.h`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "../numpy.h"
+#include "common.h"
 
 #if defined(__GNUC__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
 static_assert(__GNUC__ > 5, "Eigen Tensor support in pybind11 requires GCC > 5.0");
 #endif
 
 // Disable warnings for Eigen
 PYBIND11_WARNING_PUSH
@@ -160,14 +161,16 @@
     return result;
 }
 
 PYBIND11_WARNING_POP
 
 template <typename Type>
 struct type_caster<Type, typename eigen_tensor_helper<Type>::ValidType> {
+    static_assert(!std::is_pointer<typename Type::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using Helper = eigen_tensor_helper<Type>;
     static constexpr auto temp_name = get_tensor_descriptor<Type, false>::value;
     PYBIND11_TYPE_CASTER(Type, temp_name);
 
     bool load(handle src, bool convert) {
         if (!convert) {
             if (!isinstance<array>(src)) {
@@ -355,14 +358,16 @@
 struct get_storage_pointer_type<MapType, void_t<typename MapType::PointerArgType>> {
     using SPT = typename MapType::PointerArgType;
 };
 
 template <typename Type, int Options>
 struct type_caster<Eigen::TensorMap<Type, Options>,
                    typename eigen_tensor_helper<remove_cv_t<Type>>::ValidType> {
+    static_assert(!std::is_pointer<typename Type::Scalar>::value,
+                  PYBIND11_EIGEN_MESSAGE_POINTER_TYPES_ARE_NOT_SUPPORTED);
     using MapType = Eigen::TensorMap<Type, Options>;
     using Helper = eigen_tensor_helper<remove_cv_t<Type>>;
 
     bool load(handle src, bool /*convert*/) {
         // Note that we have a lot more checks here as we want to make sure to avoid copies
         if (!isinstance<array>(src)) {
             return false;
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/embed.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/embed.h`

 * *Files 2% similar despite different names*

```diff
@@ -194,17 +194,18 @@
                                    const char *const *argv = nullptr,
                                    bool add_program_dir_to_path = true) {
 #if PY_VERSION_HEX < PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
     detail::initialize_interpreter_pre_pyconfig(
         init_signal_handlers, argc, argv, add_program_dir_to_path);
 #else
     PyConfig config;
-    PyConfig_InitIsolatedConfig(&config);
-    config.isolated = 0;
-    config.use_environment = 1;
+    PyConfig_InitPythonConfig(&config);
+    // See PR #4473 for background
+    config.parse_argv = 0;
+
     config.install_signal_handlers = init_signal_handlers ? 1 : 0;
     initialize_interpreter(&config, argc, argv, add_program_dir_to_path);
 #endif
 }
 
 /** \rst
     Shut down the Python interpreter. No pybind11 or CPython API functions can be called
@@ -238,24 +239,22 @@
         itself cannot completely unload binary extension modules and there are several
         caveats with regard to interpreter restarting. All the details can be found
         in the CPython documentation. In short, not all interpreter memory may be
         freed, either due to reference cycles or user-created global data.
 
  \endrst */
 inline void finalize_interpreter() {
-    handle builtins(PyEval_GetBuiltins());
-    const char *id = PYBIND11_INTERNALS_ID;
-
     // Get the internals pointer (without creating it if it doesn't exist).  It's possible for the
     // internals to be created during Py_Finalize() (e.g. if a py::capsule calls `get_internals()`
     // during destruction), so we get the pointer-pointer here and check it after Py_Finalize().
     detail::internals **internals_ptr_ptr = detail::get_internals_pp();
-    // It could also be stashed in builtins, so look there too:
-    if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
-        internals_ptr_ptr = capsule(builtins[id]);
+    // It could also be stashed in state_dict, so look there too:
+    if (object internals_obj
+        = get_internals_obj_from_state_dict(detail::get_python_state_dict())) {
+        internals_ptr_ptr = detail::get_internals_pp_from_capsule(internals_obj);
     }
     // Local internals contains data managed by the current interpreter, so we must clear them to
     // avoid undefined behaviors when initializing another interpreter
     detail::get_local_internals().registered_types_cpp.clear();
     detail::get_local_internals().registered_exception_translators.clear();
 
     Py_Finalize();
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/eval.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/functional.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/gil.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/iostream.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/numpy.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/numpy.h`

 * *Files 2% similar despite different names*

```diff
@@ -560,14 +560,16 @@
         args["names"] = std::move(names);
         args["formats"] = std::move(formats);
         args["offsets"] = std::move(offsets);
         args["itemsize"] = pybind11::int_(itemsize);
         m_ptr = from_args(args).release().ptr();
     }
 
+    /// Return dtype for the given typenum (one of the NPY_TYPES).
+    /// https://numpy.org/devdocs/reference/c-api/array.html#c.PyArray_DescrFromType
     explicit dtype(int typenum)
         : object(detail::npy_api::get().PyArray_DescrFromType_(typenum), stolen_t{}) {
         if (m_ptr == nullptr) {
             throw error_already_set();
         }
     }
 
@@ -1279,20 +1281,24 @@
                                              npy_api::NPY_CFLOAT_,
                                              npy_api::NPY_CDOUBLE_,
                                              npy_api::NPY_CLONGDOUBLE_};
 
 public:
     static constexpr int value = values[detail::is_fmt_numeric<T>::index];
 
-    static pybind11::dtype dtype() {
-        if (auto *ptr = npy_api::get().PyArray_DescrFromType_(value)) {
-            return reinterpret_steal<pybind11::dtype>(ptr);
-        }
-        pybind11_fail("Unsupported buffer format!");
-    }
+    static pybind11::dtype dtype() { return pybind11::dtype(/*typenum*/ value); }
+};
+
+template <typename T>
+struct npy_format_descriptor<T, enable_if_t<is_same_ignoring_cvref<T, PyObject *>::value>> {
+    static constexpr auto name = const_name("object");
+
+    static constexpr int value = npy_api::NPY_OBJECT_;
+
+    static pybind11::dtype dtype() { return pybind11::dtype(/*typenum*/ value); }
 };
 
 #define PYBIND11_DECL_CHAR_FMT                                                                    \
     static constexpr auto name = const_name("S") + const_name<N>();                               \
     static pybind11::dtype dtype() {                                                              \
         return pybind11::dtype(std::string("S") + std::to_string(N));                             \
     }
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/operators.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/options.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/pybind11.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/pybind11.h`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 /// Wraps an arbitrary C++ function/method/lambda function/.. into a callable Python object
 class cpp_function : public function {
 public:
     cpp_function() = default;
     // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(std::nullptr_t) {}
+    cpp_function(std::nullptr_t, const is_setter &) {}
 
     /// Construct a cpp_function from a vanilla function pointer
     template <typename Return, typename... Args, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (*f)(Args...), const Extra &...extra) {
         initialize(f, f, extra...);
     }
@@ -240,18 +241,24 @@
             return_value_policy policy
                 = return_value_policy_override<Return>::policy(call.func.policy);
 
             /* Function scope guard -- defaults to the compile-to-nothing `void_type` */
             using Guard = extract_guard_t<Extra...>;
 
             /* Perform the function call */
-            handle result
-                = cast_out::cast(std::move(args_converter).template call<Return, Guard>(cap->f),
-                                 policy,
-                                 call.parent);
+            handle result;
+            if (call.func.is_setter) {
+                (void) std::move(args_converter).template call<Return, Guard>(cap->f);
+                result = none().release();
+            } else {
+                result = cast_out::cast(
+                    std::move(args_converter).template call<Return, Guard>(cap->f),
+                    policy,
+                    call.parent);
+            }
 
             /* Invoke call policy post-call hook */
             process_attributes<Extra...>::postcall(call, result);
 
             return result;
         };
 
@@ -497,16 +504,16 @@
             std::memset(rec->def, 0, sizeof(PyMethodDef));
             rec->def->ml_name = rec->name;
             rec->def->ml_meth
                 = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*)()>(dispatcher));
             rec->def->ml_flags = METH_VARARGS | METH_KEYWORDS;
 
             capsule rec_capsule(unique_rec.release(),
+                                detail::get_function_record_capsule_name(),
                                 [](void *ptr) { destruct((detail::function_record *) ptr); });
-            rec_capsule.set_name(detail::get_function_record_capsule_name());
             guarded_strdup.release();
 
             object scope_module;
             if (rec->scope) {
                 if (hasattr(rec->scope, "__module__")) {
                     scope_module = rec->scope.attr("__module__");
                 } else if (hasattr(rec->scope, "__name__")) {
@@ -1725,15 +1732,16 @@
         return def_property_static(name, fget, nullptr, extra...);
     }
 
     /// Uses return_value_policy::reference_internal by default
     template <typename Getter, typename Setter, typename... Extra>
     class_ &
     def_property(const char *name, const Getter &fget, const Setter &fset, const Extra &...extra) {
-        return def_property(name, fget, cpp_function(method_adaptor<type>(fset)), extra...);
+        return def_property(
+            name, fget, cpp_function(method_adaptor<type>(fset), is_setter()), extra...);
     }
     template <typename Getter, typename... Extra>
     class_ &def_property(const char *name,
                          const Getter &fget,
                          const cpp_function &fset,
                          const Extra &...extra) {
         return def_property(name,
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/pytypes.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/pytypes.h`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,20 @@
 private:
 #ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
     void throw_gilstate_error(const std::string &function_name) const {
         fprintf(
             stderr,
             "%s is being called while the GIL is either not held or invalid. Please see "
             "https://pybind11.readthedocs.io/en/stable/advanced/"
-            "misc.html#common-sources-of-global-interpreter-lock-errors for debugging advice.\n",
+            "misc.html#common-sources-of-global-interpreter-lock-errors for debugging advice.\n"
+            "If you are convinced there is no bug in your code, you can #define "
+            "PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF"
+            "to disable this check. In that case you have to ensure this #define is consistently "
+            "used for all translation units linked into a given pybind11 extension, otherwise "
+            "there will be ODR violations.",
             function_name.c_str());
         fflush(stderr);
         if (Py_TYPE(m_ptr)->tp_name != nullptr) {
             fprintf(stderr,
                     "The failing %s call was triggered on a %s object.\n",
                     function_name.c_str(),
                     Py_TYPE(m_ptr)->tp_name);
@@ -467,66 +472,86 @@
         return reinterpret_cast<PyTypeObject *>(obj)->tp_name;
     }
     return Py_TYPE(obj)->tp_name;
 }
 
 std::string error_string();
 
+// The code in this struct is very unusual, to minimize the chances of
+// masking bugs (elsewhere) by errors during the error handling (here).
+// This is meant to be a lifeline for troubleshooting long-running processes
+// that crash under conditions that are virtually impossible to reproduce.
+// Low-level implementation alternatives are preferred to higher-level ones
+// that might raise cascading exceptions. Last-ditch-kind-of attempts are made
+// to report as much of the original error as possible, even if there are
+// secondary issues obtaining some of the details.
 struct error_fetch_and_normalize {
-    // Immediate normalization is long-established behavior (starting with
-    // https://github.com/pybind/pybind11/commit/135ba8deafb8bf64a15b24d1513899eb600e2011
-    // from Sep 2016) and safest. Normalization could be deferred, but this could mask
-    // errors elsewhere, the performance gain is very minor in typical situations
-    // (usually the dominant bottleneck is EH unwinding), and the implementation here
-    // would be more complex.
+    // This comment only applies to Python <= 3.11:
+    //     Immediate normalization is long-established behavior (starting with
+    //     https://github.com/pybind/pybind11/commit/135ba8deafb8bf64a15b24d1513899eb600e2011
+    //     from Sep 2016) and safest. Normalization could be deferred, but this could mask
+    //     errors elsewhere, the performance gain is very minor in typical situations
+    //     (usually the dominant bottleneck is EH unwinding), and the implementation here
+    //     would be more complex.
+    // Starting with Python 3.12, PyErr_Fetch() normalizes exceptions immediately.
+    // Any errors during normalization are tracked under __notes__.
     explicit error_fetch_and_normalize(const char *called) {
         PyErr_Fetch(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
         if (!m_type) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " called while "
                             "Python error indicator not set.");
         }
         const char *exc_type_name_orig = detail::obj_class_name(m_type.ptr());
         if (exc_type_name_orig == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to obtain the name "
                             "of the original active exception type.");
         }
         m_lazy_error_string = exc_type_name_orig;
+#if PY_VERSION_HEX >= 0x030C0000
+        // The presence of __notes__ is likely due to exception normalization
+        // errors, although that is not necessarily true, therefore insert a
+        // hint only:
+        if (PyObject_HasAttrString(m_value.ptr(), "__notes__")) {
+            m_lazy_error_string += "[WITH __notes__]";
+        }
+#else
         // PyErr_NormalizeException() may change the exception type if there are cascading
         // failures. This can potentially be extremely confusing.
         PyErr_NormalizeException(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
         if (m_type.ptr() == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to normalize the "
                             "active exception.");
         }
         const char *exc_type_name_norm = detail::obj_class_name(m_type.ptr());
         if (exc_type_name_norm == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to obtain the name "
                             "of the normalized active exception type.");
         }
-#if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x07030a00
+#    if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x07030a00
         // This behavior runs the risk of masking errors in the error handling, but avoids a
         // conflict with PyPy, which relies on the normalization here to change OSError to
         // FileNotFoundError (https://github.com/pybind/pybind11/issues/4075).
         m_lazy_error_string = exc_type_name_norm;
-#else
+#    else
         if (exc_type_name_norm != m_lazy_error_string) {
             std::string msg = std::string(called)
                               + ": MISMATCH of original and normalized "
                                 "active exception types: ";
             msg += "ORIGINAL ";
             msg += m_lazy_error_string;
             msg += " REPLACED BY ";
             msg += exc_type_name_norm;
             msg += ": " + format_value_and_trace();
             pybind11_fail(msg);
         }
+#    endif
 #endif
     }
 
     error_fetch_and_normalize(const error_fetch_and_normalize &) = delete;
     error_fetch_and_normalize(error_fetch_and_normalize &&) = delete;
 
     std::string format_value_and_trace() const {
@@ -554,14 +579,48 @@
                         message_error_string = detail::error_string();
                         result = message_unavailable_exc;
                     } else {
                         result = std::string(buffer, static_cast<std::size_t>(length));
                     }
                 }
             }
+#if PY_VERSION_HEX >= 0x030B0000
+            auto notes
+                = reinterpret_steal<object>(PyObject_GetAttrString(m_value.ptr(), "__notes__"));
+            if (!notes) {
+                PyErr_Clear(); // No notes is good news.
+            } else {
+                auto len_notes = PyList_Size(notes.ptr());
+                if (len_notes < 0) {
+                    result += "\nFAILURE obtaining len(__notes__): " + detail::error_string();
+                } else {
+                    result += "\n__notes__ (len=" + std::to_string(len_notes) + "):";
+                    for (ssize_t i = 0; i < len_notes; i++) {
+                        PyObject *note = PyList_GET_ITEM(notes.ptr(), i);
+                        auto note_bytes = reinterpret_steal<object>(
+                            PyUnicode_AsEncodedString(note, "utf-8", "backslashreplace"));
+                        if (!note_bytes) {
+                            result += "\nFAILURE obtaining __notes__[" + std::to_string(i)
+                                      + "]: " + detail::error_string();
+                        } else {
+                            char *buffer = nullptr;
+                            Py_ssize_t length = 0;
+                            if (PyBytes_AsStringAndSize(note_bytes.ptr(), &buffer, &length)
+                                == -1) {
+                                result += "\nFAILURE formatting __notes__[" + std::to_string(i)
+                                          + "]: " + detail::error_string();
+                            } else {
+                                result += '\n';
+                                result += std::string(buffer, static_cast<std::size_t>(length));
+                            }
+                        }
+                    }
+                }
+            }
+#endif
         } else {
             result = "<MESSAGE UNAVAILABLE>";
         }
         if (result.empty()) {
             result = "<EMPTY MESSAGE>";
         }
 
@@ -1867,36 +1926,21 @@
     capsule(const void *value, PyCapsule_Destructor destructor)
         : object(PyCapsule_New(const_cast<void *>(value), nullptr, destructor), stolen_t{}) {
         if (!m_ptr) {
             throw error_already_set();
         }
     }
 
+    /// Capsule name is nullptr.
     capsule(const void *value, void (*destructor)(void *)) {
-        m_ptr = PyCapsule_New(const_cast<void *>(value), nullptr, [](PyObject *o) {
-            // guard if destructor called while err indicator is set
-            error_scope error_guard;
-            auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
-            if (destructor == nullptr && PyErr_Occurred()) {
-                throw error_already_set();
-            }
-            const char *name = get_name_in_error_scope(o);
-            void *ptr = PyCapsule_GetPointer(o, name);
-            if (ptr == nullptr) {
-                throw error_already_set();
-            }
-
-            if (destructor != nullptr) {
-                destructor(ptr);
-            }
-        });
+        initialize_with_void_ptr_destructor(value, nullptr, destructor);
+    }
 
-        if (!m_ptr || PyCapsule_SetContext(m_ptr, reinterpret_cast<void *>(destructor)) != 0) {
-            throw error_already_set();
-        }
+    capsule(const void *value, const char *name, void (*destructor)(void *)) {
+        initialize_with_void_ptr_destructor(value, name, destructor);
     }
 
     explicit capsule(void (*destructor)()) {
         m_ptr = PyCapsule_New(reinterpret_cast<void *>(destructor), nullptr, [](PyObject *o) {
             const char *name = get_name_in_error_scope(o);
             auto destructor = reinterpret_cast<void (*)()>(PyCapsule_GetPointer(o, name));
             if (destructor == nullptr) {
@@ -1956,14 +2000,40 @@
         if ((name == nullptr) && PyErr_Occurred()) {
             // write out and consume error raised by call to PyCapsule_GetName
             PyErr_WriteUnraisable(o);
         }
 
         return name;
     }
+
+    void initialize_with_void_ptr_destructor(const void *value,
+                                             const char *name,
+                                             void (*destructor)(void *)) {
+        m_ptr = PyCapsule_New(const_cast<void *>(value), name, [](PyObject *o) {
+            // guard if destructor called while err indicator is set
+            error_scope error_guard;
+            auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
+            if (destructor == nullptr && PyErr_Occurred()) {
+                throw error_already_set();
+            }
+            const char *name = get_name_in_error_scope(o);
+            void *ptr = PyCapsule_GetPointer(o, name);
+            if (ptr == nullptr) {
+                throw error_already_set();
+            }
+
+            if (destructor != nullptr) {
+                destructor(ptr);
+            }
+        });
+
+        if (!m_ptr || PyCapsule_SetContext(m_ptr, reinterpret_cast<void *>(destructor)) != 0) {
+            throw error_already_set();
+        }
+    }
 };
 
 class tuple : public object {
 public:
     PYBIND11_OBJECT_CVT(tuple, object, PyTuple_Check, PySequence_Tuple)
     template <typename SzType = ssize_t,
               detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/stl/filesystem.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/stl.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/stl.h`

 * *Files 2% similar despite different names*

```diff
@@ -269,19 +269,19 @@
             }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
     PYBIND11_TYPE_CASTER(ArrayType,
-                         const_name("List[") + value_conv::name
+                         const_name<Resizable>(const_name(""), const_name("Annotated["))
+                             + const_name("List[") + value_conv::name + const_name("]")
                              + const_name<Resizable>(const_name(""),
-                                                     const_name("[") + const_name<Size>()
-                                                         + const_name("]"))
-                             + const_name("]"));
+                                                     const_name(", FixedSize(")
+                                                         + const_name<Size>() + const_name(")]")));
 };
 
 template <typename Type, size_t Size>
 struct type_caster<std::array<Type, Size>>
     : array_caster<std::array<Type, Size>, Type, false, Size> {};
 
 template <typename Type>
@@ -312,14 +312,15 @@
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         if (!src) {
             return none().release();
         }
         if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Value>::policy(policy);
         }
+        // NOLINTNEXTLINE(bugprone-unchecked-optional-access)
         return value_conv::cast(*std::forward<T>(src), policy, parent);
     }
 
     bool load(handle src, bool convert) {
         if (!src) {
             return false;
         }
```

### Comparing `xcsf-1.3.0/lib/pybind11/include/pybind11/stl_bind.h` & `xcsf-1.3.1/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,19 @@
     T,
     enable_if_t<container_traits<T>::is_element && container_traits<T>::is_comparable>>
     : std::true_type {};
 
 /* For a vector/map data structure, recursively check the value type
    (which is std::pair for maps) */
 template <typename T>
-struct is_comparable<T, enable_if_t<container_traits<T>::is_vector>> {
-    static constexpr const bool value = is_comparable<typename T::value_type>::value;
-};
+struct is_comparable<T, enable_if_t<container_traits<T>::is_vector>>
+    : is_comparable<typename recursive_container_traits<T>::type_to_check_recursively> {};
+
+template <>
+struct is_comparable<recursive_bottom> : std::true_type {};
 
 /* For pairs, recursively check the two data types */
 template <typename T>
 struct is_comparable<T, enable_if_t<container_traits<T>::is_pair>> {
     static constexpr const bool value = is_comparable<typename T::first_type>::value
                                         && is_comparable<typename T::second_type>::value;
 };
@@ -351,21 +353,25 @@
 template <typename Vector, typename Class_>
 void vector_accessor(enable_if_t<vector_needs_copy<Vector>::value, Class_> &cl) {
     using T = typename Vector::value_type;
     using SizeType = typename Vector::size_type;
     using DiffType = typename Vector::difference_type;
     using ItType = typename Vector::iterator;
     cl.def("__getitem__", [](const Vector &v, DiffType i) -> T {
-        if (i < 0 && (i += v.size()) < 0) {
-            throw index_error();
+        if (i < 0) {
+            i += v.size();
+            if (i < 0) {
+                throw index_error();
+            }
         }
-        if ((SizeType) i >= v.size()) {
+        auto i_st = static_cast<SizeType>(i);
+        if (i_st >= v.size()) {
             throw index_error();
         }
-        return v[(SizeType) i];
+        return v[i_st];
     });
 
     cl.def(
         "__iter__",
         [](Vector &v) {
             return make_iterator<return_value_policy::copy, ItType, ItType, T>(v.begin(), v.end());
         },
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # CMakeLists.txt -- Build system for the pybind11 test suite
 #
 # Copyright (c) 2015 Wenzel Jakob <wenzel@inf.ethz.ch>
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.21)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.21)
+  cmake_policy(VERSION 3.26)
 endif()
 
-# Only needed for CMake < 3.5 support
-include(CMakeParseArguments)
-
 # Filter out items; print an optional message if any items filtered. This ignores extensions.
 #
 # Usage:
 #   pybind11_filter_tests(LISTNAME file1.cpp file2.cpp ... MESSAGE "")
 #
 macro(pybind11_filter_tests LISTNAME)
   cmake_parse_arguments(ARG "" "MESSAGE" "" ${ARGN})
@@ -150,15 +147,19 @@
     test_pytypes
     test_sequences_and_iterators
     test_smart_ptr
     test_stl
     test_stl_binders
     test_tagbased_polymorphic
     test_thread
+    test_type_caster_pyobject_ptr
     test_union
+    test_unnamed_namespace_a
+    test_unnamed_namespace_b
+    test_vector_unique_ptr_member
     test_virtual_functions)
 
 # Invoking cmake with something like:
 #     cmake -DPYBIND11_TEST_OVERRIDE="test_callbacks.cpp;test_pickling.cpp" ..
 # lets you override the tests that get compiled and run.  You can restore to all tests with:
 #     cmake -DPYBIND11_TEST_OVERRIDE= ..
 if(PYBIND11_TEST_OVERRIDE)
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# Built-in in CMake 3.5+
-include(CMakeParseArguments)
-
 add_custom_target(test_cmake_build)
 
 function(pybind11_add_build_test name)
   cmake_parse_arguments(ARG "INSTALL" "" "" ${ARGN})
 
   set(build_options "-DCMAKE_CXX_COMPILER=${CMAKE_CXX_COMPILER}")
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.18)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.18)
+  cmake_policy(VERSION 3.26)
 endif()
 
 project(test_installed_embed CXX)
 
 find_package(pybind11 CONFIG REQUIRED)
 message(STATUS "Found pybind11 v${pybind11_VERSION}: ${pybind11_INCLUDE_DIRS}")
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 project(test_installed_module CXX)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.18)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.18)
+  cmake_policy(VERSION 3.26)
 endif()
 
 project(test_installed_function CXX)
 
 find_package(pybind11 CONFIG REQUIRED)
 message(
   STATUS "Found pybind11 v${pybind11_VERSION} ${pybind11_VERSION_TYPE}: ${pybind11_INCLUDE_DIRS}")
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.18)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.18)
+  cmake_policy(VERSION 3.26)
 endif()
 
 project(test_installed_target CXX)
 
 find_package(pybind11 CONFIG REQUIRED)
 message(STATUS "Found pybind11 v${pybind11_VERSION}: ${pybind11_INCLUDE_DIRS}")
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.18)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.18)
+  cmake_policy(VERSION 3.26)
 endif()
 
 project(test_subdirectory_embed CXX)
 
 set(PYBIND11_INSTALL
     ON
     CACHE BOOL "")
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.18)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.18)
+  cmake_policy(VERSION 3.26)
 endif()
 
 project(test_subdirectory_function CXX)
 
 add_subdirectory("${pybind11_SOURCE_DIR}" pybind11)
 pybind11_add_module(test_subdirectory_function ../main.cpp)
 set_target_properties(test_subdirectory_function PROPERTIES OUTPUT_NAME test_cmake_build)
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.18)
+if(${CMAKE_VERSION} VERSION_LESS 3.26)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.18)
+  cmake_policy(VERSION 3.26)
 endif()
 
 project(test_subdirectory_target CXX)
 
 add_subdirectory("${pybind11_SOURCE_DIR}" pybind11)
 
 add_library(test_subdirectory_target MODULE ../main.cpp)
```

### Comparing `xcsf-1.3.0/lib/pybind11/tests/test_embed/CMakeLists.txt` & `xcsf-1.3.1/lib/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/FindCatch.cmake` & `xcsf-1.3.1/lib/pybind11/tools/FindCatch.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,22 @@
   endif()
 endfunction()
 
 # Download the single-header version of Catch
 function(_download_catch version destination_dir)
   message(STATUS "Downloading catch v${version}...")
   set(url https://github.com/philsquared/Catch/releases/download/v${version}/catch.hpp)
-  file(DOWNLOAD ${url} "${destination_dir}/catch.hpp" STATUS status)
+  file(
+    DOWNLOAD ${url} "${destination_dir}/catch.hpp"
+    STATUS status
+    LOG log)
   list(GET status 0 error)
   if(error)
-    message(FATAL_ERROR "Could not download ${url}")
+    string(REPLACE "\n" "\n  " log "  ${log}")
+    message(FATAL_ERROR "Could not download URL:\n" "  ${url}\n" "Log:\n" "${log}")
   endif()
   set(CATCH_INCLUDE_DIR
       "${destination_dir}"
       CACHE INTERNAL "")
 endfunction()
 
 # Look for catch locally
```

### Comparing `xcsf-1.3.0/lib/pybind11/tools/FindEigen3.cmake` & `xcsf-1.3.1/lib/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/FindPythonLibsNew.cmake` & `xcsf-1.3.1/lib/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/JoinPaths.cmake` & `xcsf-1.3.1/lib/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/check-style.sh` & `xcsf-1.3.1/lib/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/cmake_uninstall.cmake.in` & `xcsf-1.3.1/lib/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/codespell_ignore_lines_from_errors.py` & `xcsf-1.3.1/lib/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 from typing import List
 
 
 def run(args: List[str]) -> None:
     assert len(args) == 1, "codespell_errors.txt"
     cache = {}
     done = set()
-    for line in sorted(open(args[0]).read().splitlines()):
+    with open(args[0]) as f:
+        lines = f.read().splitlines()
+
+    for line in sorted(lines):
         i = line.find(" ==> ")
         if i > 0:
             flds = line[:i].split(":")
             if len(flds) >= 2:
                 filename, line_num = flds[:2]
                 if filename not in cache:
-                    cache[filename] = open(filename).read().splitlines()
+                    with open(filename) as f:
+                        cache[filename] = f.read().splitlines()
                 supp = cache[filename][int(line_num) - 1]
                 if supp not in done:
                     print(supp)
                     done.add(supp)
 
 
 if __name__ == "__main__":
```

### Comparing `xcsf-1.3.0/lib/pybind11/tools/libsize.py` & `xcsf-1.3.1/lib/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/make_changelog.py` & `xcsf-1.3.1/lib/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/pybind11Common.cmake` & `xcsf-1.3.1/lib/pybind11/tools/pybind11Common.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #[======================================================[.rst
 
 Adds the following targets::
 
     pybind11::pybind11 - link to headers and pybind11
     pybind11::module - Adds module links
     pybind11::embed - Adds embed links
-    pybind11::lto - Link time optimizations (manual selection)
-    pybind11::thin_lto - Link time optimizations (manual selection)
+    pybind11::lto - Link time optimizations (only if CMAKE_INTERPROCEDURAL_OPTIMIZATION is not set)
+    pybind11::thin_lto - Link time optimizations (only if CMAKE_INTERPROCEDURAL_OPTIMIZATION is not set)
     pybind11::python_link_helper - Adds link to Python libraries
     pybind11::windows_extras - MSVC bigobj and mp for building multithreaded
     pybind11::opt_size - avoid optimizations that increase code size
 
 Adds the following functions::
 
     pybind11_strip(target) - strip target after building on linux/macOS
     pybind11_find_import(module) - See if a module is installed.
 
 #]======================================================]
 
 # CMake 3.10 has an include_guard command, but we can't use that yet
 # include_guard(global) (pre-CMake 3.10)
-if(TARGET pybind11::lto)
+if(TARGET pybind11::pybind11)
   return()
 endif()
 
 # If we are in subdirectory mode, all IMPORTED targets must be GLOBAL. If we
 # are in CONFIG mode, they should be "normal" targets instead.
 # In CMake 3.11+ you can promote a target to global after you create it,
 # which might be simpler than this check.
@@ -159,19 +159,27 @@
                           "(last two chars: ${VAL} not understood as a valid CXX std)")
     endif()
   endif()
 endif()
 
 # --------------------- Python specifics -------------------------
 
+# CMake 3.27 removes the classic FindPythonInterp if CMP0148 is NEW
+if(CMAKE_VERSION VERSION_LESS "3.27")
+  set(_pybind11_missing_old_python "OLD")
+else()
+  cmake_policy(GET CMP0148 _pybind11_missing_old_python)
+endif()
+
 # Check to see which Python mode we are in, new, old, or no python
 if(PYBIND11_NOPYTHON)
   set(_pybind11_nopython ON)
 elseif(
-  PYBIND11_FINDPYTHON
+  _pybind11_missing_old_python STREQUAL "NEW"
+  OR PYBIND11_FINDPYTHON
   OR Python_FOUND
   OR Python2_FOUND
   OR Python3_FOUND)
   # New mode
   include("${CMAKE_CURRENT_LIST_DIR}/pybind11NewTools.cmake")
 
 else()
@@ -368,19 +376,21 @@
         TARGET ${target}
         APPEND
         PROPERTY INTERFACE_LINK_OPTIONS "$<${not_debug}:${PYBIND11_LTO_LINKER_FLAGS}>")
     endif()
   endif()
 endfunction()
 
-add_library(pybind11::lto IMPORTED INTERFACE ${optional_global})
-_pybind11_generate_lto(pybind11::lto FALSE)
+if(NOT DEFINED CMAKE_INTERPROCEDURAL_OPTIMIZATION)
+  add_library(pybind11::lto IMPORTED INTERFACE ${optional_global})
+  _pybind11_generate_lto(pybind11::lto FALSE)
 
-add_library(pybind11::thin_lto IMPORTED INTERFACE ${optional_global})
-_pybind11_generate_lto(pybind11::thin_lto TRUE)
+  add_library(pybind11::thin_lto IMPORTED INTERFACE ${optional_global})
+  _pybind11_generate_lto(pybind11::thin_lto TRUE)
+endif()
 
 # ---------------------- pybind11_strip -----------------------------
 
 function(pybind11_strip target_name)
   # Strip unnecessary sections of the binary on Linux/macOS
   if(CMAKE_STRIP)
     if(APPLE)
```

### Comparing `xcsf-1.3.0/lib/pybind11/tools/pybind11Config.cmake.in` & `xcsf-1.3.1/lib/pybind11/tools/pybind11Config.cmake.in`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,17 @@
   Adds bigobj and mp for MSVC.
 
 Modes
 =====
 
 There are two modes provided; classic, which is built on the old Python
 discovery packages in CMake, or the new FindPython mode, which uses FindPython
-from 3.12+ forward (3.15+ _highly_ recommended).
+from 3.12+ forward (3.15+ _highly_ recommended). If you set the minimum or
+maximum version of CMake to 3.27+, then FindPython is the default (since
+FindPythonInterp/FindPythonLibs has been removed via policy `CMP0148`).
 
 New FindPython mode
 ^^^^^^^^^^^^^^^^^^^
 
 To activate this mode, either call ``find_package(Python COMPONENTS Interpreter Development)``
 before finding this package, or set the ``PYBIND11_FINDPYTHON`` variable to ON. In this mode,
 you can either use the basic targets, or use the FindPython tools:
```

### Comparing `xcsf-1.3.0/lib/pybind11/tools/pybind11NewTools.cmake` & `xcsf-1.3.1/lib/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/pybind11Tools.cmake` & `xcsf-1.3.1/lib/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/setup_global.py.in` & `xcsf-1.3.1/lib/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/lib/pybind11/tools/setup_main.py.in` & `xcsf-1.3.1/lib/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/setup.py` & `xcsf-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="xcsf",
-    version="1.3.0",
+    version="1.3.1",
     license="GPL-3.0",
     maintainer="Richard Preen",
     maintainer_email="rpreen@gmail.com",
     description="XCSF learning classifier system: rule-based evolutionary machine learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rpreen/xcsf",
```

### Comparing `xcsf-1.3.0/test/CMakeLists.txt` & `xcsf-1.3.1/test/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,31 +14,39 @@
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 set(XCSF_TESTS
+    act_integer_test.cpp
+    cl_test.cpp
     clset_test.cpp
+    cond_gp_test.cpp
+    cond_dgp_test.cpp
     cond_ellipsoid_test.cpp
     cond_rectangle_test.cpp
     cond_ternary_test.cpp
     loss_test.cpp
+    neural_activations_test.cpp
+    neural_layer_args_test.cpp
+    neural_layer_test.cpp
     neural_layer_connected_test.cpp
     neural_layer_convolutional_test.cpp
     neural_layer_lstm_test.cpp
     neural_layer_maxpool_test.cpp
     neural_layer_recurrent_test.cpp
     neural_test.cpp
     pa_test.cpp
     pred_nlms_test.cpp
     pred_rls_test.cpp
     serialization_test.cpp
     util_test.cpp
-    unit_tests.cpp)
+    unit_tests.cpp
+    xcs_supervised_test.cpp)
 
 add_definitions(-DDSFMT_MEXP=19937)
 
 add_executable(tests ${XCSF_TESTS})
 target_link_libraries(tests xcs)
 
 add_test(NAME xcsf COMMAND tests)
```

### Comparing `xcsf-1.3.0/xcsf/CMakeLists.txt` & `xcsf-1.3.1/xcsf/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/__init__.pyi` & `xcsf-1.3.1/xcsf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/act_integer.c` & `xcsf-1.3.1/xcsf/act_integer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/act_integer.h` & `xcsf-1.3.1/xcsf/act_integer.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/act_neural.c` & `xcsf-1.3.1/xcsf/act_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/act_neural.h` & `xcsf-1.3.1/xcsf/act_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/action.c` & `xcsf-1.3.1/xcsf/action.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/action.h` & `xcsf-1.3.1/xcsf/action.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/blas.c` & `xcsf-1.3.1/xcsf/blas.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/blas.h` & `xcsf-1.3.1/xcsf/blas.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cl.c` & `xcsf-1.3.1/xcsf/cl.c`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /**
  * @file cl.c
  * @author Richard Preen <rpreen@gmail.com>
  * @copyright The Authors.
- * @date 2015--2021.
+ * @date 2015--2023.
  * @brief Functions operating on classifiers.
  */
 
 #include "cl.h"
 #include "action.h"
 #include "condition.h"
 #include "ea.h"
@@ -574,15 +574,15 @@
  * @param [in] json cJSON object.
  */
 static void
 cl_json_import_current(const struct XCSF *xcsf, struct Cl *c, const cJSON *json)
 {
     const cJSON *item = cJSON_GetObjectItem(json, "current_match");
     if (item != NULL && cJSON_IsBool(item)) {
-        c->m = item->valueint;
+        c->m = true ? item->type == cJSON_True : false;
     }
     item = cJSON_GetObjectItem(json, "current_action");
     if (item != NULL && cJSON_IsNumber(item)) {
         c->action = item->valueint;
     }
     item = cJSON_GetObjectItem(json, "current_prediction");
     if (item != NULL && cJSON_IsArray(item)) {
```

### Comparing `xcsf-1.3.0/xcsf/cl.h` & `xcsf-1.3.1/xcsf/cl.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/clset.c` & `xcsf-1.3.1/xcsf/clset.c`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     while (iter != NULL) {
         sum += iter->cl->time * iter->cl->num;
         iter = iter->next;
     }
     return sum;
 }
 
-void
+static void
 clset_load_pop_file(struct XCSF *xcsf)
 {
     FILE *f = fopen(xcsf->population_file, "rt");
     if (f == NULL) {
         printf("Error opening JSON file: %s\n", xcsf->population_file);
         exit(EXIT_FAILURE);
     }
```

### Comparing `xcsf-1.3.0/xcsf/clset.h` & `xcsf-1.3.1/xcsf/clset.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/clset_neural.c` & `xcsf-1.3.1/xcsf/clset_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/clset_neural.h` & `xcsf-1.3.1/xcsf/clset_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_dgp.c` & `xcsf-1.3.1/xcsf/cond_dgp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_dgp.h` & `xcsf-1.3.1/xcsf/cond_dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_dummy.c` & `xcsf-1.3.1/xcsf/cond_dummy.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_dummy.h` & `xcsf-1.3.1/xcsf/cond_dummy.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_ellipsoid.c` & `xcsf-1.3.1/xcsf/cond_ellipsoid.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_ellipsoid.h` & `xcsf-1.3.1/xcsf/cond_ellipsoid.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_gp.c` & `xcsf-1.3.1/xcsf/cond_gp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_gp.h` & `xcsf-1.3.1/xcsf/cond_gp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_neural.c` & `xcsf-1.3.1/xcsf/cond_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_neural.h` & `xcsf-1.3.1/xcsf/cond_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_rectangle.c` & `xcsf-1.3.1/xcsf/cond_rectangle.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_rectangle.h` & `xcsf-1.3.1/xcsf/cond_rectangle.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_ternary.c` & `xcsf-1.3.1/xcsf/cond_ternary.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/cond_ternary.h` & `xcsf-1.3.1/xcsf/cond_ternary.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/condition.c` & `xcsf-1.3.1/xcsf/condition.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/condition.h` & `xcsf-1.3.1/xcsf/condition.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/config.c` & `xcsf-1.3.1/xcsf/config.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/config.h` & `xcsf-1.3.1/xcsf/config.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/dgp.c` & `xcsf-1.3.1/xcsf/dgp.c`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /**
  * @file dgp.c
  * @author Richard Preen <rpreen@gmail.com>
  * @copyright The Authors.
- * @date 2016--2022.
+ * @date 2016--2023.
  * @brief An implementation of dynamical GP graphs with fuzzy activations.
  */
 
 #include "dgp.h"
 #include "sam.h"
 #include "utils.h"
 
@@ -662,15 +662,16 @@
                    cJSON_IsNumber(iter)) {
             graph_param_set_max_t(args, iter->valueint);
         } else if (strncmp(iter->string, "n\0", 2) == 0 &&
                    cJSON_IsNumber(iter)) {
             graph_param_set_n(args, iter->valueint);
         } else if (strncmp(iter->string, "evolve_cycles\0", 14) == 0 &&
                    cJSON_IsBool(iter)) {
-            graph_param_set_evolve_cycles(args, iter->valueint);
+            const bool evolve = true ? iter->type == cJSON_True : false;
+            graph_param_set_evolve_cycles(args, evolve);
         } else {
             return iter->string;
         }
     }
     return NULL;
 }
```

### Comparing `xcsf-1.3.0/xcsf/dgp.h` & `xcsf-1.3.1/xcsf/dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/ea.c` & `xcsf-1.3.1/xcsf/ea.c`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /**
  * @file ea.c
  * @author Richard Preen <rpreen@gmail.com>
  * @copyright The Authors.
- * @date 2015--2022.
+ * @date 2015--2023.
  * @brief Evolutionary algorithm functions.
  */
 
 #include "ea.h"
 #include "cl.h"
 #include "clset.h"
 #include "utils.h"
@@ -306,18 +306,20 @@
                    cJSON_IsNumber(iter)) {
             catch_error(ea_param_set_err_reduc(xcsf, iter->valuedouble));
         } else if (strncmp(iter->string, "fit_reduc\0", 10) == 0 &&
                    cJSON_IsNumber(iter)) {
             catch_error(ea_param_set_fit_reduc(xcsf, iter->valuedouble));
         } else if (strncmp(iter->string, "subsumption\0", 12) == 0 &&
                    cJSON_IsBool(iter)) {
-            catch_error(ea_param_set_subsumption(xcsf, iter->valueint));
+            const bool sub = true ? iter->type == cJSON_True : false;
+            catch_error(ea_param_set_subsumption(xcsf, sub));
         } else if (strncmp(iter->string, "pred_reset\0", 11) == 0 &&
                    cJSON_IsBool(iter)) {
-            catch_error(ea_param_set_pred_reset(xcsf, iter->valueint));
+            const bool reset = true ? iter->type == cJSON_True : false;
+            catch_error(ea_param_set_pred_reset(xcsf, reset));
         } else {
             printf("Error importing EA parameter %s\n", iter->string);
             exit(EXIT_FAILURE);
         }
     }
 }
```

### Comparing `xcsf-1.3.0/xcsf/ea.h` & `xcsf-1.3.1/xcsf/ea.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env.c` & `xcsf-1.3.1/xcsf/env.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env.h` & `xcsf-1.3.1/xcsf/env.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env_csv.c` & `xcsf-1.3.1/xcsf/env_csv.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env_csv.h` & `xcsf-1.3.1/xcsf/env_csv.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env_maze.c` & `xcsf-1.3.1/xcsf/env_maze.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env_maze.h` & `xcsf-1.3.1/xcsf/env_maze.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env_mux.c` & `xcsf-1.3.1/xcsf/env_mux.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/env_mux.h` & `xcsf-1.3.1/xcsf/env_mux.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/gp.c` & `xcsf-1.3.1/xcsf/gp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/gp.h` & `xcsf-1.3.1/xcsf/gp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/image.c` & `xcsf-1.3.1/xcsf/image.c`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /**
  * @file image.c
  * @author Richard Preen <rpreen@gmail.com>
  * @copyright The Authors.
- * @date 2020.
+ * @date 2020--2023.
  * @brief Image handling functions.
  */
 
+#include "image.h"
+
 static void
 col2im_add_pixel(double *im, const int height, const int width, int row,
                  int col, const int channel, const int pad, const double val)
 {
     row -= pad;
     col -= pad;
     if (row < 0 || col < 0 || row >= height || col >= width) {
```

### Comparing `xcsf-1.3.0/xcsf/image.h` & `xcsf-1.3.1/xcsf/image.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/loss.c` & `xcsf-1.3.1/xcsf/loss.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/loss.h` & `xcsf-1.3.1/xcsf/loss.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/main.c` & `xcsf-1.3.1/xcsf/main.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural.c` & `xcsf-1.3.1/xcsf/neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural.h` & `xcsf-1.3.1/xcsf/neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_activations.c` & `xcsf-1.3.1/xcsf/neural_activations.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_activations.h` & `xcsf-1.3.1/xcsf/neural_activations.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer.c` & `xcsf-1.3.1/xcsf/neural_layer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer.h` & `xcsf-1.3.1/xcsf/neural_layer.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_args.c` & `xcsf-1.3.1/xcsf/neural_layer_args.c`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /**
  * @file neural_layer_args.c
  * @author Richard Preen <rpreen@gmail.com>
  * @copyright The Authors.
- * @date 2020--2022.
+ * @date 2020--2023.
  * @brief Functions operating on neural network arguments/constants.
  */
 
 #include "neural_activations.h"
 #include "neural_layer_avgpool.h"
 #include "neural_layer_connected.h"
 #include "neural_layer_convolutional.h"
@@ -198,20 +198,20 @@
  * @param [in] json cJSON object.
  * @return Whether a parameter was found.
  */
 static bool
 layer_args_json_import_sgd(struct ArgsLayer *args, const cJSON *json)
 {
     if (strncmp(json->string, "sgd_weights\0", 12) == 0 && cJSON_IsBool(json)) {
-        args->sgd_weights = json->valueint;
+        args->sgd_weights = true ? json->type == cJSON_True : false;
     } else if (strncmp(json->string, "eta\0", 4) == 0 && cJSON_IsNumber(json)) {
         args->eta = json->valuedouble;
     } else if (strncmp(json->string, "evolve_eta\0", 11) == 0 &&
                cJSON_IsBool(json)) {
-        args->evolve_eta = json->valueint;
+        args->evolve_eta = true ? json->type == cJSON_True : false;
     } else if (strncmp(json->string, "eta_min\0", 8) == 0 &&
                cJSON_IsNumber(json)) {
         args->eta_min = json->valuedouble;
     } else if (strncmp(json->string, "momentum\0", 9) == 0 &&
                cJSON_IsNumber(json)) {
         args->momentum = json->valuedouble;
     } else if (strncmp(json->string, "decay\0", 6) == 0 &&
@@ -248,24 +248,24 @@
  * @return Whether a parameter was found.
  */
 static bool
 layer_args_json_import_evo(struct ArgsLayer *args, const cJSON *json)
 {
     if (strncmp(json->string, "evolve_weights\0", 15) == 0 &&
         cJSON_IsBool(json)) {
-        args->evolve_weights = json->valueint;
+        args->evolve_weights = true ? json->type == cJSON_True : false;
     } else if (strncmp(json->string, "evolve_functions\0", 17) == 0 &&
                cJSON_IsBool(json)) {
-        args->evolve_functions = json->valueint;
+        args->evolve_functions = true ? json->type == cJSON_True : false;
     } else if (strncmp(json->string, "evolve_connect\0", 15) == 0 &&
                cJSON_IsBool(json)) {
-        args->evolve_connect = json->valueint;
+        args->evolve_connect = true ? json->type == cJSON_True : false;
     } else if (strncmp(json->string, "evolve_neurons\0", 15) == 0 &&
                cJSON_IsBool(json)) {
-        args->evolve_neurons = json->valueint;
+        args->evolve_neurons = true ? json->type == cJSON_True : false;
     } else if (strncmp(json->string, "n_max\0", 6) == 0 &&
                cJSON_IsNumber(json)) {
         args->n_max = json->valueint;
     } else if (strncmp(json->string, "max_neuron_grow\0", 16) == 0 &&
                cJSON_IsNumber(json)) {
         args->max_neuron_grow = json->valueint;
     } else {
```

### Comparing `xcsf-1.3.0/xcsf/neural_layer_args.h` & `xcsf-1.3.1/xcsf/neural_layer_args.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_avgpool.c` & `xcsf-1.3.1/xcsf/neural_layer_avgpool.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_avgpool.h` & `xcsf-1.3.1/xcsf/neural_layer_avgpool.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_connected.c` & `xcsf-1.3.1/xcsf/neural_layer_connected.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_connected.h` & `xcsf-1.3.1/xcsf/neural_layer_connected.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_convolutional.c` & `xcsf-1.3.1/xcsf/neural_layer_convolutional.c`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,16 @@
     l->out_w = src->out_w;
     l->out_c = src->out_c;
     l->n_outputs = src->n_outputs;
     l->n_inputs = src->n_inputs;
     l->max_outputs = src->max_outputs;
     l->max_neuron_grow = src->max_neuron_grow;
     l->n_biases = src->n_biases;
+    l->momentum = src->momentum;
+    l->decay = src->decay;
     l->eta = src->eta;
     l->eta_max = src->eta_max;
     l->eta_min = src->eta_min;
     malloc_layer_arrays(l);
     memcpy(l->weights, src->weights, sizeof(double) * src->n_weights);
     memcpy(l->weight_active, src->weight_active, sizeof(bool) * src->n_weights);
     memcpy(l->biases, src->biases, sizeof(double) * src->n_biases);
```

### Comparing `xcsf-1.3.0/xcsf/neural_layer_convolutional.h` & `xcsf-1.3.1/xcsf/neural_layer_convolutional.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_dropout.c` & `xcsf-1.3.1/xcsf/neural_layer_dropout.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_dropout.h` & `xcsf-1.3.1/xcsf/neural_layer_dropout.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_lstm.c` & `xcsf-1.3.1/xcsf/neural_layer_lstm.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_lstm.h` & `xcsf-1.3.1/xcsf/neural_layer_lstm.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_maxpool.c` & `xcsf-1.3.1/xcsf/neural_layer_maxpool.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_maxpool.h` & `xcsf-1.3.1/xcsf/neural_layer_maxpool.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_noise.c` & `xcsf-1.3.1/xcsf/neural_layer_noise.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_noise.h` & `xcsf-1.3.1/xcsf/neural_layer_noise.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_recurrent.c` & `xcsf-1.3.1/xcsf/neural_layer_recurrent.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_recurrent.h` & `xcsf-1.3.1/xcsf/neural_layer_recurrent.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_softmax.c` & `xcsf-1.3.1/xcsf/neural_layer_softmax.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_softmax.h` & `xcsf-1.3.1/xcsf/neural_layer_softmax.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_upsample.c` & `xcsf-1.3.1/xcsf/neural_layer_upsample.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/neural_layer_upsample.h` & `xcsf-1.3.1/xcsf/neural_layer_upsample.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pa.c` & `xcsf-1.3.1/xcsf/pa.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pa.h` & `xcsf-1.3.1/xcsf/pa.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/param.c` & `xcsf-1.3.1/xcsf/param.c`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,16 @@
                cJSON_IsNumber(json)) {
         catch_error(param_set_pop_size(xcsf, json->valueint));
     } else if (strncmp(json->string, "max_trials\0", 11) == 0 &&
                cJSON_IsNumber(json)) {
         catch_error(param_set_max_trials(xcsf, json->valueint));
     } else if (strncmp(json->string, "pop_init\0", 9) == 0 &&
                cJSON_IsBool(json)) {
-        catch_error(param_set_pop_init(xcsf, json->valueint));
+        const bool init = true ? json->type == cJSON_True : false;
+        catch_error(param_set_pop_init(xcsf, init));
     } else if (strncmp(json->string, "perf_trials\0", 12) == 0 &&
                cJSON_IsNumber(json)) {
         catch_error(param_set_perf_trials(xcsf, json->valueint));
     } else if (strncmp(json->string, "loss_func\0", 10) == 0 &&
                cJSON_IsString(json)) {
         if (param_set_loss_func_string(xcsf, json->valuestring) ==
             PARAM_INVALID) {
@@ -274,15 +275,16 @@
  *
  */
 static bool
 param_json_import_subsump(struct XCSF *xcsf, const cJSON *json)
 {
     if (strncmp(json->string, "set_subsumption\0", 16) == 0 &&
         cJSON_IsBool(json)) {
-        catch_error(param_set_set_subsumption(xcsf, json->valueint));
+        const bool sub = true ? json->type == cJSON_True : false;
+        catch_error(param_set_set_subsumption(xcsf, sub));
     } else if (strncmp(json->string, "theta_sub\0", 10) == 0 &&
                cJSON_IsNumber(json)) {
         catch_error(param_set_theta_sub(xcsf, json->valueint));
     } else {
         return false;
     }
     return true;
@@ -320,18 +322,20 @@
     } else if (strncmp(json->string, "e0\0", 3) == 0 && cJSON_IsNumber(json)) {
         catch_error(param_set_e0(xcsf, json->valuedouble));
     } else if (strncmp(json->string, "m_probation\0", 12) == 0 &&
                cJSON_IsNumber(json)) {
         catch_error(param_set_m_probation(xcsf, json->valueint));
     } else if (strncmp(json->string, "stateful\0", 9) == 0 &&
                cJSON_IsBool(json)) {
-        catch_error(param_set_stateful(xcsf, json->valueint));
+        const bool stateful = true ? json->type == cJSON_True : false;
+        catch_error(param_set_stateful(xcsf, stateful));
     } else if (strncmp(json->string, "compaction\0", 11) == 0 &&
                cJSON_IsBool(json)) {
-        catch_error(param_set_compaction(xcsf, json->valueint));
+        const bool compact = true ? json->type == cJSON_True : false;
+        catch_error(param_set_compaction(xcsf, compact));
     } else {
         return false;
     }
     return true;
 }
 
 /**
@@ -472,17 +476,17 @@
  * @param [in] fp Pointer to the output file.
  * @return The total number of elements written.
  */
 size_t
 param_save(const struct XCSF *xcsf, FILE *fp)
 {
     size_t s = 0;
-    size_t len = sizeof(xcsf->population_file);
+    size_t len = strnlen(xcsf->population_file, MAX_LEN);
     s += fwrite(&len, sizeof(size_t), 1, fp);
-    s += fwrite(xcsf->population_file, len, 1, fp);
+    s += fwrite(xcsf->population_file, sizeof(char), len, fp);
     s += fwrite(&xcsf->time, sizeof(int), 1, fp);
     s += fwrite(&xcsf->error, sizeof(double), 1, fp);
     s += fwrite(&xcsf->mset_size, sizeof(double), 1, fp);
     s += fwrite(&xcsf->aset_size, sizeof(double), 1, fp);
     s += fwrite(&xcsf->mfrac, sizeof(double), 1, fp);
     s += fwrite(&xcsf->explore, sizeof(bool), 1, fp);
     s += fwrite(&xcsf->x_dim, sizeof(int), 1, fp);
@@ -528,16 +532,16 @@
 size_t
 param_load(struct XCSF *xcsf, FILE *fp)
 {
     size_t s = 0;
     size_t len = 0;
     s += fread(&len, sizeof(size_t), 1, fp);
     free(xcsf->population_file);
-    xcsf->population_file = malloc(len);
-    s += fread(xcsf->population_file, len, 1, fp);
+    xcsf->population_file = malloc(sizeof(char) * len);
+    s += fread(xcsf->population_file, sizeof(char), len, fp);
     s += fread(&xcsf->time, sizeof(int), 1, fp);
     s += fread(&xcsf->error, sizeof(double), 1, fp);
     s += fread(&xcsf->mset_size, sizeof(double), 1, fp);
     s += fread(&xcsf->aset_size, sizeof(double), 1, fp);
     s += fread(&xcsf->mfrac, sizeof(double), 1, fp);
     s += fread(&xcsf->explore, sizeof(bool), 1, fp);
     s += fread(&xcsf->x_dim, sizeof(int), 1, fp);
```

### Comparing `xcsf-1.3.0/xcsf/param.h` & `xcsf-1.3.1/xcsf/param.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/perf.c` & `xcsf-1.3.1/xcsf/perf.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/perf.h` & `xcsf-1.3.1/xcsf/perf.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pred_constant.c` & `xcsf-1.3.1/xcsf/pred_constant.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pred_constant.h` & `xcsf-1.3.1/xcsf/pred_constant.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pred_neural.c` & `xcsf-1.3.1/xcsf/pred_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pred_neural.h` & `xcsf-1.3.1/xcsf/pred_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pred_nlms.c` & `xcsf-1.3.1/xcsf/pred_nlms.c`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 /**
  * @file pred_nlms.c
  * @author Richard Preen <rpreen@gmail.com>
  * @copyright The Authors.
- * @date 2015--2022.
+ * @date 2015--2023.
  * @brief Normalised least mean squares prediction functions.
  */
 
 #include "pred_nlms.h"
 #include "blas.h"
 #include "sam.h"
 #include "utils.h"
@@ -344,15 +344,16 @@
         if (strncmp(iter->string, "x0\0", 3) == 0 && cJSON_IsNumber(iter)) {
             pred_param_set_x0(xcsf, iter->valuedouble);
         } else if (strncmp(iter->string, "eta\0", 4) == 0 &&
                    cJSON_IsNumber(iter)) {
             pred_param_set_eta(xcsf, iter->valuedouble);
         } else if (strncmp(iter->string, "evolve_eta\0", 11) == 0 &&
                    cJSON_IsBool(iter)) {
-            pred_param_set_evolve_eta(xcsf, iter->valueint);
+            const bool evolve = true ? iter->type == cJSON_True : false;
+            pred_param_set_evolve_eta(xcsf, evolve);
         } else if (strncmp(iter->string, "eta_min\0", 8) == 0 &&
                    cJSON_IsNumber(iter)) {
             pred_param_set_eta_min(xcsf, iter->valuedouble);
         } else {
             return iter->string;
         }
     }
```

### Comparing `xcsf-1.3.0/xcsf/pred_nlms.h` & `xcsf-1.3.1/xcsf/pred_nlms.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pred_rls.c` & `xcsf-1.3.1/xcsf/pred_rls.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pred_rls.h` & `xcsf-1.3.1/xcsf/pred_rls.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/prediction.c` & `xcsf-1.3.1/xcsf/prediction.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/prediction.h` & `xcsf-1.3.1/xcsf/prediction.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pybind_callback.h` & `xcsf-1.3.1/xcsf/pybind_callback.h`

 * *Files 19% similar despite different names*

```diff
@@ -32,13 +32,15 @@
 extern "C" {
 #include "xcsf.h"
 }
 
 class Callback
 {
   public:
+    virtual ~Callback() {}
+
     virtual bool
     run(struct XCSF *xcsf, py::dict metrics) = 0;
 
     virtual void
     finish(struct XCSF *xcsf) = 0;
 };
```

### Comparing `xcsf-1.3.0/xcsf/pybind_callback_checkpoint.h` & `xcsf-1.3.1/xcsf/pybind_callback_checkpoint.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pybind_callback_earlystop.h` & `xcsf-1.3.1/xcsf/pybind_callback_earlystop.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pybind_utils.h` & `xcsf-1.3.1/xcsf/pybind_utils.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/pybind_wrapper.cpp` & `xcsf-1.3.1/xcsf/pybind_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/rule_dgp.c` & `xcsf-1.3.1/xcsf/rule_dgp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/rule_dgp.h` & `xcsf-1.3.1/xcsf/rule_dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/rule_neural.c` & `xcsf-1.3.1/xcsf/rule_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/rule_neural.h` & `xcsf-1.3.1/xcsf/rule_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/sam.c` & `xcsf-1.3.1/xcsf/sam.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/sam.h` & `xcsf-1.3.1/xcsf/sam.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/utils/types.py` & `xcsf-1.3.1/xcsf/utils/types.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/utils/viz.py` & `xcsf-1.3.1/xcsf/utils/viz.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/utils.c` & `xcsf-1.3.1/xcsf/utils.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/utils.h` & `xcsf-1.3.1/xcsf/utils.h`

 * *Files 4% similar despite different names*

```diff
@@ -153,7 +153,25 @@
     for (int i = 0; i < size; ++i) {
         if (arr1[i] < arr2[i] - tol || arr1[i] > arr2[i] + tol) {
             return false;
         }
     }
     return true;
 }
+
+/**
+ * @brief Checks whether two integer arrays are equal.
+ * @param [in] arr1 Array.
+ * @param [in] arr2 Array.
+ * @param [in] size Length of the arrays.
+ * @return Whether the arrays are equal.
+ */
+static inline bool
+check_array_eq_int(const int *arr1, const int *arr2, int size)
+{
+    for (int i = 0; i < size; ++i) {
+        if (arr1[i] != arr2[i]) {
+            return false;
+        }
+    }
+    return true;
+}
```

### Comparing `xcsf-1.3.0/xcsf/xcs_rl.c` & `xcsf-1.3.1/xcsf/xcs_rl.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/xcs_rl.h` & `xcsf-1.3.1/xcsf/xcs_rl.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/xcs_supervised.c` & `xcsf-1.3.1/xcsf/xcs_supervised.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/xcs_supervised.h` & `xcsf-1.3.1/xcsf/xcs_supervised.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/xcsf.c` & `xcsf-1.3.1/xcsf/xcsf.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.3.0/xcsf/xcsf.h` & `xcsf-1.3.1/xcsf/xcsf.h`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 #include <stdint.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
 static const int VERSION_MAJOR = 1; //!< XCSF major version number
 static const int VERSION_MINOR = 3; //!< XCSF minor version number
-static const int VERSION_BUILD = 0; //!< XCSF build version number
+static const int VERSION_BUILD = 1; //!< XCSF build version number
 
 /**
  * @brief Classifier data structure.
  */
 struct Cl {
     struct CondVtbl const *cond_vptr; //!< Functions acting on conditions
     struct PredVtbl const *pred_vptr; //!< Functions acting on predictions
```

### Comparing `xcsf-1.3.0/xcsf.egg-info/PKG-INFO` & `xcsf-1.3.1/xcsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsf
-Version: 1.3.0
+Version: 1.3.1
 Summary: XCSF learning classifier system: rule-based evolutionary machine learning
 Home-page: https://github.com/rpreen/xcsf
 Maintainer: Richard Preen
 Maintainer-email: rpreen@gmail.com
 License: GPL-3.0
 Keywords: divide and conquer,evolutionary algorithm,genetic programming,learning classifier system,least squares,machine learning,neural networks,neuroevolution,reinforcement learning,rule-based,supervised learning,stochastic gradient descent,XCS,XCSF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xcsf-1.3.0/xcsf.egg-info/SOURCES.txt` & `xcsf-1.3.1/xcsf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -453,21 +453,23 @@
 lib/pybind11/include/pybind11/numpy.h
 lib/pybind11/include/pybind11/operators.h
 lib/pybind11/include/pybind11/options.h
 lib/pybind11/include/pybind11/pybind11.h
 lib/pybind11/include/pybind11/pytypes.h
 lib/pybind11/include/pybind11/stl.h
 lib/pybind11/include/pybind11/stl_bind.h
+lib/pybind11/include/pybind11/type_caster_pyobject_ptr.h
 lib/pybind11/include/pybind11/detail/class.h
 lib/pybind11/include/pybind11/detail/common.h
 lib/pybind11/include/pybind11/detail/descr.h
 lib/pybind11/include/pybind11/detail/init.h
 lib/pybind11/include/pybind11/detail/internals.h
 lib/pybind11/include/pybind11/detail/type_caster_base.h
 lib/pybind11/include/pybind11/detail/typeid.h
+lib/pybind11/include/pybind11/eigen/common.h
 lib/pybind11/include/pybind11/eigen/matrix.h
 lib/pybind11/include/pybind11/eigen/tensor.h
 lib/pybind11/include/pybind11/stl/filesystem.h
 lib/pybind11/tests/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
```

