# Comparing `tmp/nasti-0.1.4.tar.gz` & `tmp/nasti-0.1.6.tar.gz`

## Comparing `nasti-0.1.4.tar` & `nasti-0.1.6.tar`

### file list

```diff
@@ -1,45 +1,53 @@
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 nasti-0.1.4/Makefile
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nasti-0.1.4/Pipfile
--rw-r--r--   0        0        0    28335 2020-02-02 00:00:00.000000 nasti-0.1.4/Pipfile.lock
--rw-r--r--   0        0        0    70731 2020-02-02 00:00:00.000000 nasti-0.1.4/logo.png
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nasti-0.1.4/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nasti-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/cli.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/exceptions.py
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/mutation.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/nasti.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/nastifile.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/source_handlers.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 nasti-0.1.4/nasti/validation.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/mocks.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_mutation.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_nastifile.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_source_handlers.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/test_validation.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/bad_yaml/nasti.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_empty_files/nasti.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/nasti.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/test.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_files_dont_exist/nasti.yaml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_misconfigured_validation/nasti.yaml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_no_files/nasti.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_run/nasti.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_text_replacement_fails/nasti.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_text_replacement_fails/test.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unknown_keys/nasti.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/nasti.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/.dontsearch
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/ref.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/unmentioned
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/nested/searchbutnotfind
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/mutation_unmentioned_files/files/nested/unmentioned
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/no_mutations/nasti.yaml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.4/tests/nastifiles/valid/nasti.yaml
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nasti-0.1.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nasti-0.1.4/LICENSE
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 nasti-0.1.4/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 nasti-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 nasti-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 nasti-0.1.6/Makefile
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 nasti-0.1.6/Pipfile
+-rw-r--r--   0        0        0    33354 2020-02-02 00:00:00.000000 nasti-0.1.6/Pipfile.lock
+-rw-r--r--   0        0        0    70731 2020-02-02 00:00:00.000000 nasti-0.1.6/logo.png
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nasti-0.1.6/reference.yaml
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nasti-0.1.6/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nasti-0.1.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/cli.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/exceptions.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/globals.py
+-rw-r--r--   0        0        0     8256 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/mutation.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/nasti.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/nastifile.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/source_handlers.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 nasti-0.1.6/nasti/validation.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/mocks.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/test_globals.py
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/test_mutation.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/test_nastifile.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/test_source_handlers.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/test_validation.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/bad_yaml/nasti.yaml
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_default_and_globals_complex/nasti.yaml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_default_and_globals_simple/nasti.yaml
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_default_exception/nasti.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_empty_files/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/nasti.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_file_doesnt_contain_replacement_text/test.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_files_dont_exist/nasti.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_misconfigured_validation/nasti.yaml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_no_files/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_run/nasti.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_text_replacement_fails/nasti.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_text_replacement_fails/test.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_unknown_keys/nasti.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_unmentioned_files/nasti.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_unmentioned_files/files/.dontsearch
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_unmentioned_files/files/ref.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_unmentioned_files/files/unmentioned
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_unmentioned_files/files/nested/searchbutnotfind
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/mutation_unmentioned_files/files/nested/unmentioned
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/nastifile_default/nasti.yaml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/nastifile_globals/nasti.yaml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/no_mutations/nasti.yaml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nasti-0.1.6/tests/nastifiles/valid/nasti.yaml
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nasti-0.1.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nasti-0.1.6/LICENSE
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 nasti-0.1.6/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nasti-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 nasti-0.1.6/PKG-INFO
```

### Comparing `nasti-0.1.4/Pipfile.lock` & `nasti-0.1.6/Pipfile.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9592803030303031%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'975153968901e2b8046a5aea431ecabe8cd662efb881a967c3e544464595945b'}}",*

 * * "'default'": "{'jinja2': OrderedDict([('hashes', "*

 * *              "['sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852', "*

 * *              "'sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61']), "*

 * *              "('index', 'pypi'), ('version', '==3.1.2')]), 'markupsafe': OrderedDict([('hashes', "*

 * *              "['sha256:05fb21170423db021895e1ea1e1f3a […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "838ecd7d4e984f86fc68c9c6387307f36b8264d23e30bff69b380bd32f43881f"
+            "sha256": "975153968901e2b8046a5aea431ecabe8cd662efb881a967c3e544464595945b"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_full_version": "3.11.4",
             "python_version": "3.11"
         },
         "sources": [
@@ -103,14 +103,78 @@
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
+        "jinja2": {
+            "hashes": [
+                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
+                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
+            ],
+            "index": "pypi",
+            "version": "==3.1.2"
+        },
+        "markupsafe": {
+            "hashes": [
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.1.3"
+        },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
```

### Comparing `nasti-0.1.4/logo.png` & `nasti-0.1.6/logo.png`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/.github/workflows/coverage.yml` & `nasti-0.1.6/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/.github/workflows/tests.yml` & `nasti-0.1.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/nasti/cli.py` & `nasti-0.1.6/nasti/cli.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/nasti/exceptions.py` & `nasti-0.1.6/nasti/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 class MutationTooManyInputTriesException(Exception):
     pass
 
 class MutationTextReplacementFailedException(Exception):
     pass
 
+class MutationDefaultTemplateInvalidException(Exception):
+    pass
+
 class ValidationConfigMissingException(Exception):
     pass
 
 class ValidationConfigInvalidException(Exception):
     pass
 
 class ValidationUnknownKindException(Exception):
@@ -43,8 +46,17 @@
 class NastiFileInvalidYamlException(Exception):
     pass
 
 class NastiFileNoMutationsException(Exception):
     pass
 
 class NastiFileUnknownKeysException(Exception):
+    pass
+
+class NastiFileGlobalNotFoundException(Exception):
+    pass
+
+class GlobalRequiredKeysMissingException(Exception):
+    pass
+
+class GlobalTooManyInputTriesException(Exception):
     pass
```

### Comparing `nasti-0.1.4/nasti/mutation.py` & `nasti-0.1.6/nasti/mutation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import os
 import re
 from nasti.validation import Validation
 import nasti.exceptions as exceptions
-
+from jinja2 import Template
 
 class Mutation:
     prompt = ""
     help = False
     validation = False
     replace = ""
     files = []
     path = ""
+    default = False
+    globals = {}
 
     HELP_KEY = "help"
     VALIDATION_KEY = "validation"
     NAME_KEY = "name"
     PROMPT_KEY = "prompt"
     REPLACE_KEY = "replace"
     FILES_KEY = "files"
+    DEFAULT_KEY = "default"
+    GLOBALS_KEY = "globals"
 
-    def __init__(self, mutation_config, path, os_dep=os, open_dep=open, input_dep=input, print_dep=print):
+    def __init__(self, mutation_config: dict, path, os_dep=os, open_dep=open, input_dep=input, print_dep=print):
         # Dependency injection
         self.os_dep = os_dep
         self.open_dep = open_dep
         self.input_dep = input_dep
         self.print_dep = print_dep
         # Required fields
         try:
@@ -32,14 +36,18 @@
             self.replace     = mutation_config[self.REPLACE_KEY]
             self.files       = mutation_config[self.FILES_KEY]
         except Exception as e:
             raise exceptions.MutationRequiredKeysMissingException(f"Error: Invalid mutation config: {mutation_config} required field missing missing {e}")
         # Optional fields
         if self.HELP_KEY in mutation_config:
             self.help        = mutation_config[self.HELP_KEY]
+        if self.GLOBALS_KEY in mutation_config:
+            self.globals     = mutation_config[self.GLOBALS_KEY]
+        if self.DEFAULT_KEY in mutation_config:
+            self.default     = mutation_config[self.DEFAULT_KEY]
         if self.VALIDATION_KEY in mutation_config:
             try:
                 self.validation = Validation(mutation_config[self.VALIDATION_KEY])
             except Exception as e:
                 raise e(f"Error: Invalid vaidation config in mutation: {mutation_config} {e}")
         self.path = path
 
@@ -100,31 +108,51 @@
 
     # Validate the nastifile syntax
     # Raises exceptions if there are any problems
     def validate(self):
         # verify files isn't empty
         if len(self.files) == 0:
             raise exceptions.MutationEmptyFilesException(f"Error: mutation {self.name} does not contain any files.")
+        # If there's a default template verify it renders
+        if self.default:
+            self.render_default_template()
         for file in self.files:
             # verify file exists
             file_with_path = self.__get_file_full_path(file)
             if not self.os_dep.path.isfile(file_with_path):
                 raise exceptions.MutationFileDoesNotExistException(f"Error: mutation: {self.name} file: {file} at: {file_with_path} does not exist.")
             # verify the file contains the text to be replaced
             with self.open_dep(file_with_path, 'r') as f:
                 # search for at least one instance of the text to be replaced
                 if not re.search(self.replace, f.read()):
                     raise exceptions.MutationFileDoesNotContainReplacementStringException(f"Error: mutation {self.name} file: {file} at: {file_with_path} does not contain {self.replace} ")
 
+    def render_default_template(self):
+        default_value = ""
+        if not self.default:
+            return
+        try:
+            template = Template(self.default)
+            default_value = template.render(**self.globals)
+        except Exception as e:
+            raise exceptions.MutationDefaultTemplateInvalidException(f"Error: Unable to render default template: {e}")
+        return default_value
+        
 
     def run(self):
         # Prompt the user for input
         if self.help:
             self.print_dep(self.help)
+        # If there is a default value, print it
+        if self.default:
+            default = self.render_default_template()
+            self.print_dep(f"Enter for Default: {default}")
         user_input = self.__get_user_input()
+        if user_input == "":
+            user_input = self.render_default_template()
         try:
             self.__replace_text_in_files(user_input)
         except Exception as e:
             raise exceptions.MutationTextReplacementFailedException(f"Error: Unable to replace text in files: {e}")
 
     def __get_user_input(self):
         tries = 0
```

### Comparing `nasti-0.1.4/nasti/nasti.py` & `nasti-0.1.6/nasti/nasti.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/nasti/source_handlers.py` & `nasti-0.1.6/nasti/source_handlers.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/nasti/validation.py` & `nasti-0.1.6/nasti/validation.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/tests/mocks.py` & `nasti-0.1.6/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/tests/test_mutation.py` & `nasti-0.1.6/tests/test_mutation.py`

 * *Files 20% similar despite different names*

```diff
@@ -62,14 +62,20 @@
         mutation_config = config["mutations"][0]
         # Validations raise multiple exceptions
         # We only test for an exception here
         # The validation tests cover all of the various kinds of failures
         with self.assertRaises(Exception):
             Mutation(mutation_config, "tests/nastifiles/mutation_misconfigured_validation")
 
+    def test_mutation_with_missing_required_config(self):
+        mutation_config = {
+            "prompt": "test prompt",
+        }
+        with self.assertRaises(exceptions.MutationRequiredKeysMissingException):
+            Mutation(mutation_config, "")
 
     def test_file_doesnt_contain_replacement_text(self):
         input_dep = func = lambda x: "bogus_slug"
         print_dep = func = lambda x: None
         #open the yaml file
         with open("tests/nastifiles/mutation_file_doesnt_contain_replacement_text/nasti.yaml", "r") as f:
             config = yaml.safe_load(f)
@@ -103,7 +109,43 @@
         mutation.run()
         #open the file we replaced stuff in
         with open("tests/nastifiles/mutation_run/test.txt", "r") as f:
             file_contents = f.read()
         assert file_contents == "just bogus_slug please"
         #delete the file we replaced stuff in
         os.remove("tests/nastifiles/mutation_run/test.txt")
+
+    def test_mutation_default_and_globals_simple(self):
+        input_dep = func = lambda x: "bogus_slug"
+        print_dep = func = lambda x: None
+        #open the yaml file
+        with open("tests/nastifiles/mutation_default_and_globals_simple/nasti.yaml", "r") as f:
+            config = yaml.safe_load(f)
+        mutation_config = config["mutations"][0]
+        mutation_config["globals"] = {config["globals"][0]["name"]: "Test App"}
+        mutation = Mutation(mutation_config, "tests/nastifiles/mutation_default_and_globals_simple", os, open, input_dep, print_dep)
+        default_value = mutation.render_default_template()
+        assert default_value == "Test App"
+
+    def test_mutation_default_and_globals_complex(self):
+        input_dep = func = lambda x: "bogus_slug"
+        print_dep = func = lambda x: None
+        #open the yaml file
+        with open("tests/nastifiles/mutation_default_and_globals_complex/nasti.yaml", "r") as f:
+            config = yaml.safe_load(f)
+        mutation_config = config["mutations"][0]
+        mutation_config["globals"] = {config["globals"][0]["name"]: "Test App"}
+        mutation = Mutation(mutation_config, "tests/nastifiles/mutation_default_and_globals_complex", os, open, input_dep, print_dep)
+        default_value = mutation.render_default_template()
+        assert default_value == "test_app"
+
+    def test_mutation_default_exception(self):
+        input_dep = func = lambda x: "bogus_slug"
+        print_dep = func = lambda x: None
+        #open the yaml file
+        with open("tests/nastifiles/mutation_default_exception/nasti.yaml", "r") as f:
+            config = yaml.safe_load(f)
+        mutation_config = config["mutations"][0]
+        mutation_config["globals"] = {config["globals"][0]["name"]: "Test App"}
+        mutation = Mutation(mutation_config, "tests/nastifiles/mutation_default_exception", os, open, input_dep, print_dep)
+        with self.assertRaises(exceptions.MutationDefaultTemplateInvalidException):
+            mutation.render_default_template()
```

### Comparing `nasti-0.1.4/tests/test_nastifile.py` & `nasti-0.1.6/tests/test_nastifile.py`

 * *Files 26% similar despite different names*

```diff
@@ -77,7 +77,36 @@
             "path": "tests/nastifiles/valid",
             "os_dep": os,
             "open_dep": open,
         })
         unmentioned_files = nasti_file.find_unmentioned_files()
         assert len(unmentioned_files.get_results()) == 0
         assert len(unmentioned_files.get_report()) == 0
+    
+    def test_globals(self):
+        input_dep = func = lambda x: "test_global_value"
+        print_dep = func = lambda x: None
+        nasti_file = NastiFile({
+            "path": "tests/nastifiles/nastifile_globals",
+            "os_dep": os,
+            "open_dep": open,
+            "input_dep": input_dep,
+            "print_dep": print_dep
+        })
+        nasti_file.load()
+        nasti_file.run()
+        global_obj = nasti_file.get_global("app_name")
+        assert global_obj  == "test_global_value"
+    
+    def test_default(self):
+        input_dep = func = lambda x: "input_from_user"
+        print_dep = func = lambda x: None
+        nasti_file = NastiFile({
+            "path": "tests/nastifiles/nastifile_default",
+            "os_dep": os,
+            "open_dep": open,
+            "input_dep": input_dep,
+            "print_dep": print_dep
+        })
+        nasti_file.load()
+        nasti_file.run()
+
```

### Comparing `nasti-0.1.4/tests/test_source_handlers.py` & `nasti-0.1.6/tests/test_source_handlers.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/tests/test_validation.py` & `nasti-0.1.6/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/.gitignore` & `nasti-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/LICENSE` & `nasti-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nasti-0.1.4/README.md` & `nasti-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: NASTI
+Version: 0.1.6
+Summary: NASTI's A Strange Templating Implementation
+Project-URL: Homepage, https://github.com/adamrdrew/nasti
+Project-URL: Bug Tracker, https://github.com/adamrdrew/nasti/issues
+Author-email: Adam Drew <adamrdrew@live.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 [![Build Status](https://github.com/adamrdrew/nasti/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/adamrdrew/nasti/actions)
 [![codecov](https://codecov.io/gh/adamrdrew/nasti/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/adamrdrew/nasti?branch=master)
 
  <center><img src="logo.png"></center>
 
 # NASTI
 NASTI is A Strange Templating Implementation.
@@ -34,15 +48,15 @@
 # Let NASTI greate your new project's repo
 $ nasti process --git ~/Development/some-template
 ```
 
 ## Template Creation
 All you need to get started is a project you that want to be available as a template. It can be in any language, with any project layout. 
 
-Simply add a nastifile called `nasti.yaml` to the root of your project and add some mutations:
+Simply add a nastifile called `nasti.yaml` to the root of your project and add some mutations. Mutations are definition of text replacement operations.
 
 ```yaml
 ---
 mutations:
     # Name is an ID used internally and will appear in error messages
   - name: "github"
     # Prompt to present to the template user
@@ -123,14 +137,68 @@
     "ip_address":   validators.ip_address,
     "slug":         validators.slug,
     "url":          validators.url,
     "uuid":         validators.uuid,
 }
 ```
 
+### Globals and Default Templates
+You may want to make the same input available to multiple mutations. Globals allow you to gather information from the user and then reference that input in mutations. Globals are accessed through mutation features called default templates. Default templates use Jina2 template syntax allowing you to create derived values such as converting "App Name" to "app_name" or combine mutliple globals.
+
+Example:
+```yaml
+---
+globals:
+  - name: "app_name"
+    prompt: "App Name"
+    help: "The name of your application"
+mutations:
+  - name: "example_mutation"
+    prompt: "Example Mutation"
+    help: "Help for an example mutation"
+    replace: "example text to replace"
+    default: "{{ app_name }}"
+    files: []
+    validation:
+      kind: "slug"
+```
+
+In the above example the user will first be prompted to enter data for the global called "app_name". Whatever the user enters will be used as the default value for the mutation "example_mutation". If a default is presented to the user they'll have the option to hit enter without entering any input to use the default.
+
+A more complex example showing the Jinja2 template syntax:
+```yaml
+---
+globals:
+  - name: "app_name"
+    prompt: "App Name"
+    help: "The name of your application"
+mutations:
+  - name: "example_mutation"
+    prompt: "Example Mutation"
+    help: "Help for an example mutation"
+    replace: "example text to replace"
+    default: "{{ app_name.lower().split(' ') | join('_') }}"
+    files: []
+    validation:
+      kind: "slug"
+```
+
+In that example if the user entered "My Great App" for the "app_name" global the "example_mutation" would have a default value of "my_great_app". Jinja2 syntax is extremely power, allowing you to use built in filters, call native Python methods, and more. [Check out their documentaiton](https://jinja.palletsprojects.com/en/2.10.x/templates/) for more info. 
+
+Also, note that globals support validations using exactly the same syntax as mutaitons:
+
+```yaml
+globals:
+  - name: "route_prefix"
+    prompt: "Route Prefix"
+    help: "Your route prefix"
+    validation:
+      kind: slug
+```
+
 ## Development
 
 ### Dependency Management & Virtual Environment
 This project uses [pipenv](https://github.com/pypa/pipenv) to manage dependencies and the virtual environment. You'll want to make sure you have pipenv installed. Then after you pull down the NASTI code run `pipenv install`. You can then enter the virtual environment and get to hacking with `pipenv shell`.
 
 ### Running from Source
 If you are hacking on the app and you want to run the version you have in the source tree enter the venv with `pipenv shell` and then run the app directly:
```

### Comparing `nasti-0.1.4/pyproject.toml` & `nasti-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "NASTI"
-version = "0.1.4"
+version = "0.1.6"
 authors = [
   { name="Adam Drew", email="adamrdrew@live.com" },
 ]
-description = "NASTI is Not A Starndard Templating Implementation"
+description = "NASTI's A Strange Templating Implementation"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `nasti-0.1.4/PKG-INFO` & `nasti-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: NASTI
-Version: 0.1.4
-Summary: NASTI is Not A Starndard Templating Implementation
-Project-URL: Homepage, https://github.com/adamrdrew/nasti
-Project-URL: Bug Tracker, https://github.com/adamrdrew/nasti/issues
-Author-email: Adam Drew <adamrdrew@live.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 [![Build Status](https://github.com/adamrdrew/nasti/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/adamrdrew/nasti/actions)
 [![codecov](https://codecov.io/gh/adamrdrew/nasti/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/adamrdrew/nasti?branch=master)
 
  <center><img src="logo.png"></center>
 
 # NASTI
 NASTI is A Strange Templating Implementation.
@@ -48,15 +34,15 @@
 # Let NASTI greate your new project's repo
 $ nasti process --git ~/Development/some-template
 ```
 
 ## Template Creation
 All you need to get started is a project you that want to be available as a template. It can be in any language, with any project layout. 
 
-Simply add a nastifile called `nasti.yaml` to the root of your project and add some mutations:
+Simply add a nastifile called `nasti.yaml` to the root of your project and add some mutations. Mutations are definition of text replacement operations.
 
 ```yaml
 ---
 mutations:
     # Name is an ID used internally and will appear in error messages
   - name: "github"
     # Prompt to present to the template user
@@ -137,14 +123,68 @@
     "ip_address":   validators.ip_address,
     "slug":         validators.slug,
     "url":          validators.url,
     "uuid":         validators.uuid,
 }
 ```
 
+### Globals and Default Templates
+You may want to make the same input available to multiple mutations. Globals allow you to gather information from the user and then reference that input in mutations. Globals are accessed through mutation features called default templates. Default templates use Jina2 template syntax allowing you to create derived values such as converting "App Name" to "app_name" or combine mutliple globals.
+
+Example:
+```yaml
+---
+globals:
+  - name: "app_name"
+    prompt: "App Name"
+    help: "The name of your application"
+mutations:
+  - name: "example_mutation"
+    prompt: "Example Mutation"
+    help: "Help for an example mutation"
+    replace: "example text to replace"
+    default: "{{ app_name }}"
+    files: []
+    validation:
+      kind: "slug"
+```
+
+In the above example the user will first be prompted to enter data for the global called "app_name". Whatever the user enters will be used as the default value for the mutation "example_mutation". If a default is presented to the user they'll have the option to hit enter without entering any input to use the default.
+
+A more complex example showing the Jinja2 template syntax:
+```yaml
+---
+globals:
+  - name: "app_name"
+    prompt: "App Name"
+    help: "The name of your application"
+mutations:
+  - name: "example_mutation"
+    prompt: "Example Mutation"
+    help: "Help for an example mutation"
+    replace: "example text to replace"
+    default: "{{ app_name.lower().split(' ') | join('_') }}"
+    files: []
+    validation:
+      kind: "slug"
+```
+
+In that example if the user entered "My Great App" for the "app_name" global the "example_mutation" would have a default value of "my_great_app". Jinja2 syntax is extremely power, allowing you to use built in filters, call native Python methods, and more. [Check out their documentaiton](https://jinja.palletsprojects.com/en/2.10.x/templates/) for more info. 
+
+Also, note that globals support validations using exactly the same syntax as mutaitons:
+
+```yaml
+globals:
+  - name: "route_prefix"
+    prompt: "Route Prefix"
+    help: "Your route prefix"
+    validation:
+      kind: slug
+```
+
 ## Development
 
 ### Dependency Management & Virtual Environment
 This project uses [pipenv](https://github.com/pypa/pipenv) to manage dependencies and the virtual environment. You'll want to make sure you have pipenv installed. Then after you pull down the NASTI code run `pipenv install`. You can then enter the virtual environment and get to hacking with `pipenv shell`.
 
 ### Running from Source
 If you are hacking on the app and you want to run the version you have in the source tree enter the venv with `pipenv shell` and then run the app directly:
```

