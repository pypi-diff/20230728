# Comparing `tmp/seeeye-0.0.2-py3-none-any.whl.zip` & `tmp/seeeye-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,67 +1,73 @@
-Zip file size: 34504 bytes, number of entries: 65
--rw-r--r--  2.0 unx      174 b- defN 23-Jun-30 04:32 cicd/core/action.py
--rw-r--r--  2.0 unx     3100 b- defN 23-Jun-30 04:32 cicd/core/client.py
--rw-r--r--  2.0 unx      131 b- defN 23-Jun-30 04:32 cicd/core/env.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Jun-30 04:32 cicd/core/logger.py
--rw-r--r--  2.0 unx      333 b- defN 23-Jun-30 04:32 cicd/core/_cli/opts.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jun-30 04:32 cicd/core/mixin/core.py
--rw-r--r--  2.0 unx      282 b- defN 23-Jun-30 04:32 cicd/core/mixin/git.py
--rw-r--r--  2.0 unx      115 b- defN 23-Jun-30 04:32 cicd/core/mixin/logger.py
--rw-r--r--  2.0 unx     1552 b- defN 23-Jun-30 04:32 cicd/core/mixin/provider.py
--rw-r--r--  2.0 unx      261 b- defN 23-Jun-30 04:32 cicd/core/mixin/step.py
--rw-r--r--  2.0 unx     1237 b- defN 23-Jun-30 04:32 cicd/core/provider/client.py
--rw-r--r--  2.0 unx     1261 b- defN 23-Jun-30 04:32 cicd/core/provider/info.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jun-30 04:32 cicd/core/provider/models/api.py
--rw-r--r--  2.0 unx     1878 b- defN 23-Jun-30 04:32 cicd/core/provider/models/base.py
--rw-r--r--  2.0 unx      158 b- defN 23-Jun-30 04:32 cicd/core/provider/models/pr.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-30 04:32 cicd/core/provider/models/project.py
--rw-r--r--  2.0 unx     1929 b- defN 23-Jun-30 04:32 cicd/core/syntax/data_represented.py
--rw-r--r--  2.0 unx      563 b- defN 23-Jun-30 04:32 cicd/core/syntax/json.py
--rw-r--r--  2.0 unx      253 b- defN 23-Jun-30 04:32 cicd/core/syntax/yaml.py
--rw-r--r--  2.0 unx      827 b- defN 23-Jun-30 04:32 cicd/core/utils/cli_group.py
--rw-r--r--  2.0 unx     1570 b- defN 23-Jun-30 04:32 cicd/core/utils/sh.py
--rw-r--r--  2.0 unx      369 b- defN 23-Jun-30 04:32 cicd/core/utils/step.py
--rw-r--r--  2.0 unx      970 b- defN 23-Jun-30 04:32 cicd/core/utils/timeout.py
--rw-r--r--  2.0 unx     2844 b- defN 23-Jun-30 04:32 cicd/ios/cli.py
--rw-r--r--  2.0 unx     1489 b- defN 23-Jun-30 04:32 cicd/ios/actions/base.py
--rw-r--r--  2.0 unx      690 b- defN 23-Jun-30 04:32 cicd/ios/actions/cov.py
--rw-r--r--  2.0 unx     1170 b- defN 23-Jun-30 04:32 cicd/ios/actions/test_extraction.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jun-30 04:32 cicd/ios/actions/xcodebuild/__init__.py
--rw-r--r--  2.0 unx     5052 b- defN 23-Jun-30 04:32 cicd/ios/actions/xcodebuild/base.py
--rw-r--r--  2.0 unx      591 b- defN 23-Jun-30 04:32 cicd/ios/actions/xcodebuild/build.py
--rw-r--r--  2.0 unx     1110 b- defN 23-Jun-30 04:32 cicd/ios/actions/xcodebuild/test.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jun-30 04:32 cicd/ios/cov/__init__.py
--rw-r--r--  2.0 unx      378 b- defN 23-Jun-30 04:32 cicd/ios/cov/config.py
--rw-r--r--  2.0 unx      767 b- defN 23-Jun-30 04:32 cicd/ios/cov/cov.py
--rw-r--r--  2.0 unx     2273 b- defN 23-Jun-30 04:32 cicd/ios/cov/report.py
--rw-r--r--  2.0 unx      560 b- defN 23-Jun-30 04:32 cicd/ios/mixin/base_ios.py
--rw-r--r--  2.0 unx      389 b- defN 23-Jun-30 04:32 cicd/ios/mixin/build.py
--rw-r--r--  2.0 unx      566 b- defN 23-Jun-30 04:32 cicd/ios/mixin/cocoapods.py
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-30 04:32 cicd/ios/mixin/cov.py
--rw-r--r--  2.0 unx      186 b- defN 23-Jun-30 04:32 cicd/ios/mixin/metadata.py
--rw-r--r--  2.0 unx      160 b- defN 23-Jun-30 04:32 cicd/ios/mixin/mono.py
--rw-r--r--  2.0 unx      461 b- defN 23-Jun-30 04:32 cicd/ios/mixin/simulator.py
--rw-r--r--  2.0 unx      603 b- defN 23-Jun-30 04:32 cicd/ios/mixin/test.py
--rw-r--r--  2.0 unx     1267 b- defN 23-Jun-30 04:32 cicd/ios/mixin/test_sharding.py
--rw-r--r--  2.0 unx     2022 b- defN 23-Jun-30 04:32 cicd/ios/project/metadata.py
--rw-r--r--  2.0 unx     1967 b- defN 23-Jun-30 04:32 cicd/ios/runner/base.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jun-30 04:32 cicd/ios/runner/xcodebuild/__init__.py
--rw-r--r--  2.0 unx      279 b- defN 23-Jun-30 04:32 cicd/ios/runner/xcodebuild/build.py
--rw-r--r--  2.0 unx      623 b- defN 23-Jun-30 04:32 cicd/ios/runner/xcodebuild/test.py
--rw-r--r--  2.0 unx       25 b- defN 23-Jun-30 04:32 cicd/ios/simulator/__init__.py
--rw-r--r--  2.0 unx     5181 b- defN 23-Jun-30 04:32 cicd/ios/simulator/simulator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 04:32 cicd/ios/syntax/__init__.py
--rw-r--r--  2.0 unx     4600 b- defN 23-Jun-30 04:32 cicd/ios/syntax/xcresult.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 04:32 cicd/providers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 04:32 cicd/providers/github/__init__.py
--rw-r--r--  2.0 unx      929 b- defN 23-Jun-30 04:32 cicd/providers/github/client.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jun-30 04:32 cicd/providers/github/env.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 04:32 cicd/providers/gitlab/__init__.py
--rw-r--r--  2.0 unx      134 b- defN 23-Jun-30 04:32 cicd/providers/gitlab/client.py
--rw-r--r--  2.0 unx       63 b- defN 23-Jun-30 04:32 cicd/providers/gitlab/env.py
--rw-r--r--  2.0 unx     1092 b- defN 23-Jun-30 04:32 seeeye-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2941 b- defN 23-Jun-30 04:32 seeeye-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 04:32 seeeye-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-30 04:32 seeeye-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5365 b- defN 23-Jun-30 04:32 seeeye-0.0.2.dist-info/RECORD
-65 files, 65877 bytes uncompressed, 25994 bytes compressed:  60.5%
+Zip file size: 38033 bytes, number of entries: 71
+-rw-r--r--  2.0 unx      165 b- defN 23-Jul-28 01:25 cicd/cli.py
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-28 01:25 cicd/core/action.py
+-rw-r--r--  2.0 unx     3100 b- defN 23-Jul-28 01:25 cicd/core/client.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jul-28 01:25 cicd/core/env.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-28 01:25 cicd/core/logger.py
+-rw-r--r--  2.0 unx      333 b- defN 23-Jul-28 01:25 cicd/core/_cli/opts.py
+-rw-r--r--  2.0 unx      163 b- defN 23-Jul-28 01:25 cicd/core/mixin/core.py
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-28 01:25 cicd/core/mixin/git.py
+-rw-r--r--  2.0 unx      115 b- defN 23-Jul-28 01:25 cicd/core/mixin/logger.py
+-rw-r--r--  2.0 unx     1552 b- defN 23-Jul-28 01:25 cicd/core/mixin/provider.py
+-rw-r--r--  2.0 unx      261 b- defN 23-Jul-28 01:25 cicd/core/mixin/step.py
+-rw-r--r--  2.0 unx     1237 b- defN 23-Jul-28 01:25 cicd/core/provider/client.py
+-rw-r--r--  2.0 unx     1261 b- defN 23-Jul-28 01:25 cicd/core/provider/info.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jul-28 01:25 cicd/core/provider/models/api.py
+-rw-r--r--  2.0 unx     1878 b- defN 23-Jul-28 01:25 cicd/core/provider/models/base.py
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-28 01:25 cicd/core/provider/models/pr.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-28 01:25 cicd/core/provider/models/project.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Jul-28 01:25 cicd/core/syntax/data_represented.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Jul-28 01:25 cicd/core/syntax/json.py
+-rw-r--r--  2.0 unx      253 b- defN 23-Jul-28 01:25 cicd/core/syntax/yaml.py
+-rw-r--r--  2.0 unx      827 b- defN 23-Jul-28 01:25 cicd/core/utils/cli_group.py
+-rw-r--r--  2.0 unx      534 b- defN 23-Jul-28 01:25 cicd/core/utils/file.py
+-rw-r--r--  2.0 unx     1708 b- defN 23-Jul-28 01:25 cicd/core/utils/sh.py
+-rw-r--r--  2.0 unx      369 b- defN 23-Jul-28 01:25 cicd/core/utils/step.py
+-rw-r--r--  2.0 unx      970 b- defN 23-Jul-28 01:25 cicd/core/utils/timeout.py
+-rw-r--r--  2.0 unx     3352 b- defN 23-Jul-28 01:25 cicd/ios/cli.py
+-rw-r--r--  2.0 unx     2482 b- defN 23-Jul-28 01:25 cicd/ios/actions/base.py
+-rw-r--r--  2.0 unx      690 b- defN 23-Jul-28 01:25 cicd/ios/actions/cov.py
+-rw-r--r--  2.0 unx     1170 b- defN 23-Jul-28 01:25 cicd/ios/actions/test_extraction.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/__init__.py
+-rw-r--r--  2.0 unx     3413 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/archive.py
+-rw-r--r--  2.0 unx     5150 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/base.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/build.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Jul-28 01:25 cicd/ios/actions/xcodebuild/test.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-28 01:25 cicd/ios/cov/__init__.py
+-rw-r--r--  2.0 unx      378 b- defN 23-Jul-28 01:25 cicd/ios/cov/config.py
+-rw-r--r--  2.0 unx      767 b- defN 23-Jul-28 01:25 cicd/ios/cov/cov.py
+-rw-r--r--  2.0 unx     2273 b- defN 23-Jul-28 01:25 cicd/ios/cov/report.py
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-28 01:25 cicd/ios/mixin/archive.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-28 01:25 cicd/ios/mixin/base_ios.py
+-rw-r--r--  2.0 unx      389 b- defN 23-Jul-28 01:25 cicd/ios/mixin/build.py
+-rw-r--r--  2.0 unx      566 b- defN 23-Jul-28 01:25 cicd/ios/mixin/cocoapods.py
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-28 01:25 cicd/ios/mixin/cov.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Jul-28 01:25 cicd/ios/mixin/metadata.py
+-rw-r--r--  2.0 unx      212 b- defN 23-Jul-28 01:25 cicd/ios/mixin/mono.py
+-rw-r--r--  2.0 unx      469 b- defN 23-Jul-28 01:25 cicd/ios/mixin/simulator.py
+-rw-r--r--  2.0 unx      603 b- defN 23-Jul-28 01:25 cicd/ios/mixin/test.py
+-rw-r--r--  2.0 unx     1267 b- defN 23-Jul-28 01:25 cicd/ios/mixin/test_sharding.py
+-rw-r--r--  2.0 unx     2022 b- defN 23-Jul-28 01:25 cicd/ios/project/metadata.py
+-rw-r--r--  2.0 unx     1967 b- defN 23-Jul-28 01:25 cicd/ios/runner/base.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/__init__.py
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/archive.py
+-rw-r--r--  2.0 unx      279 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/build.py
+-rw-r--r--  2.0 unx      623 b- defN 23-Jul-28 01:25 cicd/ios/runner/xcodebuild/test.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-28 01:25 cicd/ios/simulator/__init__.py
+-rw-r--r--  2.0 unx     5181 b- defN 23-Jul-28 01:25 cicd/ios/simulator/simulator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/ios/syntax/__init__.py
+-rw-r--r--  2.0 unx     4600 b- defN 23-Jul-28 01:25 cicd/ios/syntax/xcresult.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/providers/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/providers/github/__init__.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Jul-28 01:25 cicd/providers/github/client.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-28 01:25 cicd/providers/github/env.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 01:25 cicd/providers/gitlab/__init__.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Jul-28 01:25 cicd/providers/gitlab/client.py
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-28 01:25 cicd/providers/gitlab/env.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2941 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5874 b- defN 23-Jul-28 01:26 seeeye-0.0.3.dist-info/RECORD
+71 files, 73171 bytes uncompressed, 28721 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: cicd/cli.py
+Comment: 
+
 Filename: cicd/core/action.py
 Comment: 
 
 Filename: cicd/core/client.py
 Comment: 
 
 Filename: cicd/core/env.py
@@ -54,14 +57,17 @@
 
 Filename: cicd/core/syntax/yaml.py
 Comment: 
 
 Filename: cicd/core/utils/cli_group.py
 Comment: 
 
+Filename: cicd/core/utils/file.py
+Comment: 
+
 Filename: cicd/core/utils/sh.py
 Comment: 
 
 Filename: cicd/core/utils/step.py
 Comment: 
 
 Filename: cicd/core/utils/timeout.py
@@ -78,14 +84,17 @@
 
 Filename: cicd/ios/actions/test_extraction.py
 Comment: 
 
 Filename: cicd/ios/actions/xcodebuild/__init__.py
 Comment: 
 
+Filename: cicd/ios/actions/xcodebuild/archive.py
+Comment: 
+
 Filename: cicd/ios/actions/xcodebuild/base.py
 Comment: 
 
 Filename: cicd/ios/actions/xcodebuild/build.py
 Comment: 
 
 Filename: cicd/ios/actions/xcodebuild/test.py
@@ -99,14 +108,17 @@
 
 Filename: cicd/ios/cov/cov.py
 Comment: 
 
 Filename: cicd/ios/cov/report.py
 Comment: 
 
+Filename: cicd/ios/mixin/archive.py
+Comment: 
+
 Filename: cicd/ios/mixin/base_ios.py
 Comment: 
 
 Filename: cicd/ios/mixin/build.py
 Comment: 
 
 Filename: cicd/ios/mixin/cocoapods.py
@@ -135,14 +147,17 @@
 
 Filename: cicd/ios/runner/base.py
 Comment: 
 
 Filename: cicd/ios/runner/xcodebuild/__init__.py
 Comment: 
 
+Filename: cicd/ios/runner/xcodebuild/archive.py
+Comment: 
+
 Filename: cicd/ios/runner/xcodebuild/build.py
 Comment: 
 
 Filename: cicd/ios/runner/xcodebuild/test.py
 Comment: 
 
 Filename: cicd/ios/simulator/__init__.py
@@ -174,23 +189,26 @@
 
 Filename: cicd/providers/gitlab/client.py
 Comment: 
 
 Filename: cicd/providers/gitlab/env.py
 Comment: 
 
-Filename: seeeye-0.0.2.dist-info/LICENSE
+Filename: seeeye-0.0.3.dist-info/LICENSE
+Comment: 
+
+Filename: seeeye-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: seeeye-0.0.2.dist-info/METADATA
+Filename: seeeye-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: seeeye-0.0.2.dist-info/WHEEL
+Filename: seeeye-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: seeeye-0.0.2.dist-info/top_level.txt
+Filename: seeeye-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: seeeye-0.0.2.dist-info/RECORD
+Filename: seeeye-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cicd/core/utils/sh.py

```diff
@@ -1,10 +1,12 @@
 import os
+import shlex
 import signal
 import subprocess
+import typing as t
 
 from cicd.core.logger import logger
 
 
 class Shell:
     class ExecError(Exception):
         pass
@@ -39,9 +41,12 @@
         except (subprocess.TimeoutExpired, TimeoutError) as e:
             # Clean up process group. For some long-running (shell) commands such as `xcodebuild foo | bar`,
             # the child processes are not getting cleaned up properly.
             # --> Kill the process group to clean up them all.
             os.killpg(os.getpgid(proc.pid), signal.SIGTERM)
             raise e
 
+    def quote(self, s) -> t.Optional[str]:
+        return shlex.quote(str(s)) if s is not None else None
+
 
 sh = Shell()
```

## cicd/ios/cli.py

```diff
@@ -58,39 +58,53 @@
     'timeout',
     'shards',
     'shard_idx',
 )
 
 
 @click.group()
-def cli():
+def main():
     pass
 
 
-@cli.command()
+@main.command()
 @click.option('--build-for-testing', is_flag=True, help='Build for testing')
 @click.option('--cocoapods', is_flag=True, help='Run pod install beforehand')
 @xcodebuild_opts
 def build(**kwargs):
     Mixin(**kwargs).start_building()
 
 
-@cli.command()
+@main.command()
 @click.option('--retries', type=int, help='Number of test retries')
 @click.option('--only-testing', multiple=True, help='Run only these tests')
 @click.option('--test-without-building', is_flag=True, help='Test without building')
 @click.option('--cocoapods', is_flag=True, help='Run pod install beforehand')
 @xcodebuild_opts
 def test(**kwargs):
     Mixin(**kwargs).start_testing()
 
 
-@cli.command()
+@main.command()
+@click.option(
+    '--profiles',
+    help='Profiles mapping used for exporting to .ipa (format: <bundle_id>:<profile_name>)',
+)
+@click.option('--export-method', help='Export method (Ex: app-store, ad-hoc...)')
+@click.option('--output-path', help='Where the ipa should be in')
+@click.option('--archive-path', help='Archive path')
+@click.option('--cocoapods', is_flag=True, help='Run pod install beforehand')
+@xcodebuild_opts
+def archive(**kwargs):
+    Mixin(**kwargs).start_archiving()
+
+
+@main.command()
 @click.option('--config', help='Path to config file (default: .cov.yml)')
 @click.option('--export', help='Path to export cov json data')
 @opts.use('timeout', 'derived_data_path')
 def cov(**kwargs):
     Mixin(**kwargs).start_parsing_cov()
 
 
 if __name__ == '__main__':
-    cli()
+    main()
```

## cicd/ios/actions/base.py

```diff
@@ -5,36 +5,76 @@
 
 from cicd.core.action import Action
 from cicd.ios.mixin.metadata import MetadataMixin
 from cicd.ios.syntax.xcresult import XCResult
 
 
 class IOSAction(Action, MetadataMixin):
-    xcresult: XCResult
+    xcresult: t.Optional[XCResult]
+    xcarchive_path: t.Optional[Path]
 
     @cached_property
     def derived_data_path(self) -> Path:
         path = self.kwargs.get('derived_data_path')
         return Path(path) if path else self.metadata.default_derived_data_path
 
-    def xcresult_paths(self) -> t.List[Path]:
-        return sorted(self.derived_data_path.glob('Logs/Test/*.xcresult'), reverse=True)
+    @cached_property
+    def archive_path(self) -> Path:
+        path = self.kwargs.get('archive_path') or '~/Library/Developer/Xcode/Archives'
+        return Path(path).expanduser()
 
     @contextmanager
-    def collect_xcresults(self, new_only=True) -> XCResult:
-        '''Collect the xcresults generated after an action.'''
-        before = self.xcresult_paths() if new_only else []
+    def collect_artifacts(
+        self,
+        name: str,
+        base_path: Path,
+        pattern: str,
+        on_detected: t.Callable[[t.List[Path]], None],
+        new_only=True,
+    ) -> t.List[Path]:
+        def find_paths() -> t.List[Path]:
+            return sorted(base_path.glob(pattern), reverse=True)
+
+        before = find_paths() if new_only else []
         try:
             yield
         finally:
-            after = self.xcresult_paths()
+            after = find_paths()
             paths = list(set(after).difference(before))
             if len(paths) == 0:
                 raise RuntimeError(
-                    f'Cannot detect any xcresult bundle. DerivedData: {self.derived_data_path}'
+                    f'Cannot detect any {name} matching: {base_path / pattern}'
                 )
             elif len(paths) > 1:
-                self.logger.warning(f'Detected more than one xcresult bundle: {paths}')
-                # TODO: Merge xcresult bundles
+                self.logger.warning(f'Detected more than one {name}: {paths}')
             else:
-                self.logger.info(f'Detected xcresult bundles: {paths}')
-            self.xcresult = XCResult(path=paths[0])
+                self.logger.info(f'Detected {name}: {paths}')
+            on_detected(paths)
+
+    @contextmanager
+    def collect_xcresults(self, new_only=True) -> XCResult:
+        '''Collect the xcresults generated after an action.'''
+
+        def save(paths):
+            self.xcresult = XCResult(paths[0])
+
+        with self.collect_artifacts(
+            name='xcresult',
+            base_path=self.derived_data_path,
+            pattern='Logs/Test/*.xcresult',
+            on_detected=save,
+            new_only=new_only,
+        ):
+            yield
+
+    @contextmanager
+    def collect_xcarchives(self, new_only=True) -> t.List[Path]:
+        def save(paths):
+            self.xcarchive_path = paths[0]
+
+        with self.collect_artifacts(
+            name='xcarchive',
+            base_path=self.archive_path,
+            pattern='**/*.xcarchive',
+            on_detected=save,
+        ):
+            yield
```

## cicd/ios/actions/xcodebuild/__init__.py

```diff
@@ -1,3 +1,4 @@
+from .archive import *
 from .base import *
 from .build import *
 from .test import *
```

## cicd/ios/actions/xcodebuild/base.py

```diff
@@ -1,9 +1,8 @@
 import typing as t
-from shlex import quote
 
 from cicd.core.utils.sh import sh
 from cicd.ios.actions.base import IOSAction
 from cicd.ios.mixin.metadata import MetadataMixin
 
 __all__ = ['XCBAction']
 
@@ -11,25 +10,31 @@
 class CmdMaker(MetadataMixin):
     def __init__(self, **kwargs) -> None:
         self.kwargs = kwargs
 
     def make(self) -> t.Optional[str]:
         raise NotImplementedError
 
-    def quote(self, s) -> t.Optional[str]:
-        return quote(str(s)) if s is not None else None
+    def args_from_dict(self, ds: t.Dict[str, t.Any]) -> t.List[str]:
+        return [
+            x for (k, v) in ds.items() for x in [f'-{k}', sh.quote(v)] if v is not None
+        ]
 
 
 class XCBCmdMaker(CmdMaker):
     def make(self) -> t.Optional[str]:
         xctestrun = self.kwargs.get('xctestrun')
         workspace = self.kwargs.get('workspace')
         scheme = self.kwargs.get('scheme')
         project = self.kwargs.get('project')
         target = self.kwargs.get('target')
+        xcargs = self.kwargs.get('xcargs', {})
+        actions = self.kwargs.get('actions', [])
+        tests = self.kwargs.get('only_testing', [])
+
         if xctestrun:
             workspace, scheme = None, None
             project, target = None, None
         elif workspace or scheme:
             workspace = workspace or self.metadata.xcworkspace_path  # prefill
             scheme = scheme or self.metadata.scheme  # prefill
             project, target = None, None
@@ -39,65 +44,59 @@
             workspace, scheme = None, None
         elif self.metadata.xcworkspace_path:
             workspace = self.metadata.xcworkspace_path
             scheme = self.metadata.scheme
         elif self.metadata.xcodeproj_path:
             project = self.metadata.xcodeproj_path
 
-        simulator = self.kwargs.pop('_simulator')
+        simulator = self.kwargs.pop('_simulator', None)
         if simulator:
             default_destination = f'id={simulator.identifier}'
+        elif 'archive' in actions:
+            default_destination = 'generic/platform=iOS'
         else:
             default_destination = 'platform=iOS Simulator,name=Seeeye'
         xcb_kwargs = {
             'derivedDataPath': self.kwargs.get('derived_data_path'),
             'xctestrun': xctestrun,
             'workspace': workspace,
             'scheme': scheme,
             'project': project,
             'target': target,
             'configuration': self.kwargs.get('configuration'),
             'sdk': self.kwargs.get('sdk'),
             'destination': self.kwargs.get('destination') or default_destination,
+            'archivePath': self.kwargs.get('archive_path'),
         }
-        xcargs = self.kwargs.get('xcargs', {})
-        actions = self.kwargs.get('actions', [])
-        tests = self.kwargs.get('only_testing', [])
         if self.kwargs.get('clean'):
             actions.insert(0, 'clean')
 
-        cmps = ['xcodebuild'] + actions
-        cmps += [
-            x
-            for (k, v) in xcb_kwargs.items()
-            for x in [f'-{k}', self.quote(v)]
-            if v is not None
-        ]
+        cmps = ['xcodebuild'] + actions + self.args_from_dict(xcb_kwargs)
         cmps += [x for test in tests for x in ['-only-testing', test]]
         if isinstance(xcargs, str):
             cmps += [xcargs]
         elif isinstance(xcargs, (tuple, list)):
             cmps += list(xcargs)
         elif isinstance(xcargs, dict):
-            cmps += [f'{k}={quote(v)}' for (k, v) in xcargs.items()]
+            cmps += [f'{k}={sh.quote(v)}' for (k, v) in xcargs.items()]
         return ' '.join(cmps)
 
 
 class LogCmdMaker(CmdMaker):
     def make(self) -> t.Optional[str]:
         return self.kwargs.get('log_formatter') or self.metadata.resolve_program(
             'xcpretty'
         )
 
 
 class TeeCmdMaker(CmdMaker):
     def make(self) -> t.Optional[str]:
         log_path = self.kwargs.get('log_path')
         if log_path:
-            return f'tee {quote(log_path)}'
+            return f'tee {sh.quote(log_path)}'
 
 
 class XCBAction(IOSAction, MetadataMixin):
     '''A class that interacts with the xcodebuild command.
 
     It is up to subclasses to guarantee params are passed valid.
     For example, ``only_testing`` and ``build_for_testing`` should not co-exist.
```

## cicd/ios/actions/xcodebuild/build.py

```diff
@@ -2,17 +2,15 @@
 
 
 class BuildError(Exception):
     pass
 
 
 class XCBBuildAction(XCBAction):
-    '''A class that iteracts with the xcodebuild command,
-    particularly for build actions.
-    '''
+    '''A class that interacts with the xcodebuild command, particularly for build actions.'''
 
     def run(self):
         kwargs = self.kwargs
         try:
             if not kwargs.get('actions'):
                 if kwargs.get('build_for_testing'):
                     kwargs['actions'] = ['build-for-testing']
```

## cicd/ios/actions/xcodebuild/test.py

```diff
@@ -8,17 +8,15 @@
 
     def __init__(self, xcresult: XCResult, *args: object) -> None:
         super().__init__(*args)
         self.xcresult = xcresult
 
 
 class XCBTestAction(XCBAction):
-    '''A class that iteracts with the xcodebuild command,
-    particularly for test actions.
-    '''
+    '''A class that interacts with the xcodebuild command, particularly for test actions.'''
 
     def run(self) -> XCResult:
         '''Execute the action
 
         :raises: The ``TestError`` embedding the xcresult of the test session.
         :return: The ``XCResult`` object corresponding to the test session.
         :rtype: XCResult
```

## cicd/ios/mixin/base_ios.py

```diff
@@ -11,13 +11,14 @@
 ):
     def __init__(self, **kwargs) -> None:
         self.kwargs = kwargs
         super().__init__()
 
     def pre_run(self):
         self.prepare_cocoapods(**self.kwargs)
-        self.prepare_simulator(**self.kwargs)
-        # Workaround: For children to use simulator info
-        self.kwargs['_simulator'] = self.simulator
+        if self.kwargs.get('prepare_simulator', True):
+            self.prepare_simulator(**self.kwargs)
+            # Workaround: For children to use simulator info
+            self.kwargs['_simulator'] = self.simulator
 
     def post_run(self):
         pass
```

## cicd/ios/mixin/mono.py

```diff
@@ -1,11 +1,13 @@
+from .archive import ArchiveMixin
 from .build import BuildMixin
 from .cov import CovMixin
 from .test import TestMixin
 
 
 class MonoMixin(
+    ArchiveMixin,
     BuildMixin,
     TestMixin,
     CovMixin,
 ):
     pass
```

## cicd/ios/mixin/simulator.py

```diff
@@ -1,14 +1,15 @@
 import typing as t
 
 from cicd.ios.simulator import Simulator
 
 
 class SimulatorMixin:
-    simulator: t.Optional[Simulator]
+    simulator: t.Optional[Simulator] = None
+
     def prepare_simulator(self, **kwargs):
         destination = kwargs.get('destination')
         if destination:
             self.simulator = Simulator.from_xcodebuild_destination(destination)
         else:
             self.simulator = Simulator(**kwargs)
         if self.simulator:
```

## cicd/ios/runner/xcodebuild/__init__.py

```diff
@@ -1,2 +1,3 @@
+from .archive import *
 from .build import *
 from .test import *
```

## Comparing `seeeye-0.0.2.dist-info/LICENSE` & `seeeye-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `seeeye-0.0.2.dist-info/METADATA` & `seeeye-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeeye
-Version: 0.0.2
+Version: 0.0.3
 Summary: CI/CD toolkits for mobile apps
 Author-email: Thuyen Trinh <trinhngocthuyen@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/trinhngocthuyen/seeeye
 Keywords: ci,cd,ci/cd,mobile,ios
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

## Comparing `seeeye-0.0.2.dist-info/RECORD` & `seeeye-0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+cicd/cli.py,sha256=0fjlMdwR2DZ1OgvsJFvoyHv5T002KDDtnhcSq0-mqZA,165
 cicd/core/action.py,sha256=XeqZCDSZdcDsdZ2OwiiceoDrzqs5X_b9XdftyksIT3Y,174
 cicd/core/client.py,sha256=PznhG9LAlpXJ3g9ekdDoaYL0rOpZPAk0RVwBosBwqnA,3100
 cicd/core/env.py,sha256=r2u3vcAb_M2eiwDNXCgk-vWojfqqezM0J8-94_4HUL4,131
 cicd/core/logger.py,sha256=ldpHJEMlOdTd3KdOW8szewaNt1u6DEjNcerOay3_5t4,1071
 cicd/core/_cli/opts.py,sha256=rcLrpeopmU95fFDnNIWLg59BBgyq74-8HJa-mymqblU,333
 cicd/core/mixin/core.py,sha256=LSNMmW3YGsqehkw-zuhqwjziOczsqnA6Wk4JfvbIZMY,163
 cicd/core/mixin/git.py,sha256=3EdZJDDXZH2hYjXJj65awwcqErOWzWAPLupQ4Va8_aM,282
@@ -14,52 +15,57 @@
 cicd/core/provider/models/base.py,sha256=ViBnjKvXC1yMq3rhGwZoUFZ71F7-6AVN4UnMtr_9T7c,1878
 cicd/core/provider/models/pr.py,sha256=d_-2EezDN4zUQHUOEwAu2i1SyrFK6iLf7rMOH3mE0Gw,158
 cicd/core/provider/models/project.py,sha256=t-M-75onuYW8FVDHlqh8-HouWBy7d6M7J09kewIET5A,982
 cicd/core/syntax/data_represented.py,sha256=ZxVUffqNaWW4lYNZvoNMj5F3HTr0XeuOIbg2nwcTWrE,1929
 cicd/core/syntax/json.py,sha256=w4JcdxFFXf2GhQOHhZSBI7cM_QIDMhaueSLrpGPtejU,563
 cicd/core/syntax/yaml.py,sha256=XXra6E7hHdnri-y470kp3DQ7BTT6iXz5m0a0UES76ZA,253
 cicd/core/utils/cli_group.py,sha256=fPwV3Ry4ni49P5f_eph-_roX-KJh0DodrdwZ0_RMEYo,827
-cicd/core/utils/sh.py,sha256=odGwGLRG92D1SIusc7CjUlu0UEujikHXsoQ_FecaCNQ,1570
+cicd/core/utils/file.py,sha256=mA8OLqAolOHdp_AbIRecqqHDeHbh4IHdqoW_cbi8LrI,534
+cicd/core/utils/sh.py,sha256=GdeTxGmHnE6U24_AiZPHmJkuoJ7_VWQYMg52XZSrfak,1708
 cicd/core/utils/step.py,sha256=em3xuJLvkZJf1T9muYpkvcm2QnxPWNGajRjSZ92w3yY,369
 cicd/core/utils/timeout.py,sha256=OX4Cd6BedrAC8eHuM4wyBlYgnXYgtZTU7nTax6lpifo,970
-cicd/ios/cli.py,sha256=FaLFUu4JsRwG0dgxDq1SX2P6TkFUZfW2RI-hXpVJ7bE,2844
-cicd/ios/actions/base.py,sha256=LRLgvuYcyf1efu8PToPm7q4gKO3d_30waMxeCRonOgI,1489
+cicd/ios/cli.py,sha256=r0PuM9Pos34RwQD-OZXj5Hpkbu2HPC5IQG6X2nBiqJI,3352
+cicd/ios/actions/base.py,sha256=KLux4boKXXq_LUItu47IXHGpQhBUb7FOBGPLRewL8EU,2482
 cicd/ios/actions/cov.py,sha256=3iPTg0Q17o8XRoNd3e_qw2E7L_EkjTR3l_VQncjRwOo,690
 cicd/ios/actions/test_extraction.py,sha256=YuYhVrCDxD7PHY9GKp3mInLP5-5pf03Y4jaGK3dLLIU,1170
-cicd/ios/actions/xcodebuild/__init__.py,sha256=IiqQuaNQlEe0O1nd2i0mibAhvlpdjUz-GxhIK-50Ig4,61
-cicd/ios/actions/xcodebuild/base.py,sha256=5gdWLLFBCDQBwCOloH8HFQTuZ6PkZuKh2p0M8-NBrso,5052
-cicd/ios/actions/xcodebuild/build.py,sha256=9DmvDDfo5qKFRCgDx4hDBmMgr_8VH65YkLgdkT3_b5g,591
-cicd/ios/actions/xcodebuild/test.py,sha256=dxYaLrVl2igURPJ2Ah5BViMkOycHZr3R4FC9a4Kococ,1110
+cicd/ios/actions/xcodebuild/__init__.py,sha256=8R3lS89ufp3xSOvEafgApMLdd3_jU2Ays43VjX702mI,84
+cicd/ios/actions/xcodebuild/archive.py,sha256=6mc48ds277X_v9zw5HIuGJsY6jYa9KF5Rlce8WWP7bQ,3413
+cicd/ios/actions/xcodebuild/base.py,sha256=ikZ3PYgAASoZC2oHR8o7ngQ7XSLlKNnqo-3XDfUM6Qs,5150
+cicd/ios/actions/xcodebuild/build.py,sha256=D5G9Wg2JELzgLs9x9ktaaNitPQ-Z_QMAC0g5RLeIXb4,583
+cicd/ios/actions/xcodebuild/test.py,sha256=qwW73vYxEzHBNZtvSGjEmjxauxrA85APnIlwjPRBbyQ,1102
 cicd/ios/cov/__init__.py,sha256=V73S1UnY2lzUJitrRRLF3a4lhb0igeVFASBgh_QlCKs,63
 cicd/ios/cov/config.py,sha256=S8i9exRBS39LVVjxKYYCUiN3sNUKywv3FwkBtL3WsNA,378
 cicd/ios/cov/cov.py,sha256=grPe6FXhBvguAIk9E25xyl7t9O-g-KxZZ5mNHbwA0K0,767
 cicd/ios/cov/report.py,sha256=K5UvOngLDYZXH8J_8SnAx1vRez6_gVbE_Ef7L1JVizg,2273
-cicd/ios/mixin/base_ios.py,sha256=kt_67Fc-7qw4RvepoBMVih3zqVqAL0j43haP0FYPR4Y,560
+cicd/ios/mixin/archive.py,sha256=uqf1EQ1kQI7RVFs1nklD3xo0E9KAiRxIZ2LNt6wE-bQ,449
+cicd/ios/mixin/base_ios.py,sha256=chc8YCy36Y6EzjznbnJPedpHPjkKASmZacR1_AlK5OQ,627
 cicd/ios/mixin/build.py,sha256=wbCzckqLVS5OcuYEXTEdlr8N8_pLQEHje0oWj26IZn4,389
 cicd/ios/mixin/cocoapods.py,sha256=8ojhBaGOR0GK1gGEjNoRG8BI14BEBgkr8PDcXihfNuY,566
 cicd/ios/mixin/cov.py,sha256=XvIkennIfDC5s_RctySyOIaWdy62KQjZ91hVH82uFWI,190
 cicd/ios/mixin/metadata.py,sha256=Csuw7PLQqsxWuFBm4R2zu71lpkFtdBY5CYOTo2l0vkc,186
-cicd/ios/mixin/mono.py,sha256=DMwD2umDB3uA3hMytwMbQP32BlfejP-aDT39kPjGVlk,160
-cicd/ios/mixin/simulator.py,sha256=WPiSm8hT7mGTmgeSq0xfgd5LN-6ZamyalnAvoQpuoBw,461
+cicd/ios/mixin/mono.py,sha256=aM58kda67VduecJOXmxqYgIdOucXmSk6_QBhlOJfK_0,212
+cicd/ios/mixin/simulator.py,sha256=aqzikkoaqAg8EDI4jZM9LqmoLXWHtnZC-DaS2ZzLe6s,469
 cicd/ios/mixin/test.py,sha256=2Lq4LMT_RX-1Ft2ugR4Xywm3NOdHuUU2gUxNyTEpV-k,603
 cicd/ios/mixin/test_sharding.py,sha256=zMN1XevkCFdxp9YrcFZScWDg98N4cSL21nHLbbywaFM,1267
 cicd/ios/project/metadata.py,sha256=ykWn6YQBcoxdZEXjlgdyx0J8vMVcx6vgcRE8jfbAEaY,2022
 cicd/ios/runner/base.py,sha256=EGwf3WhmQd6IDrtgLBEYAQj5hq4SKwYW9S2JxfE3tAg,1967
-cicd/ios/runner/xcodebuild/__init__.py,sha256=w6dBhoHTvBItle4FtD2rqnrwC5MnDQIAe5GyN2oMKk8,41
+cicd/ios/runner/xcodebuild/__init__.py,sha256=bWQXCY47-0ASN06yAQwd_oz3eNE7F6AANqEQ-xK8QBo,64
+cicd/ios/runner/xcodebuild/archive.py,sha256=BgoHRV61qs8G9L1KZ8jfpHh5zcv4SJ67QYmMN1vb8bg,291
 cicd/ios/runner/xcodebuild/build.py,sha256=8R991GaJtY14i-1FVr980Pc6PXf7hPmtVtgVJaB1f4k,279
 cicd/ios/runner/xcodebuild/test.py,sha256=9mLglBoXiwAhg3NzGLORcY8JFMQgaxtfhMtiARfZZDA,623
 cicd/ios/simulator/__init__.py,sha256=Q9Ql1qnoRmUXXWW_XL7QFR86jfZD9Ld9ZKxT6QdN5X8,25
 cicd/ios/simulator/simulator.py,sha256=NeLa_K5ItLVU9O9WIULFfn2gdMu4B7mF7ZQkmKLSVZI,5181
 cicd/ios/syntax/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cicd/ios/syntax/xcresult.py,sha256=-o4RiOjskIFRwj5ktZAxzdNSwgK8_APrdS_BVpbg6pE,4600
 cicd/providers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cicd/providers/github/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cicd/providers/github/client.py,sha256=uhfzAn8LFYqlfXxVzwOMcj_XnEM8RaTgr1E9sndK6YI,929
 cicd/providers/github/env.py,sha256=6d0JqBare1z_hILN-RG3fhEaD1QQ2udcp3nI1mZc5oM,63
 cicd/providers/gitlab/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cicd/providers/gitlab/client.py,sha256=VFM96sLw-QIB50h6k_swV1GMftv-IgXMUqbUeyCvv78,134
 cicd/providers/gitlab/env.py,sha256=8oTranPx1OS5skABEHkuBVmtLfjYP5radk1SpTWFODc,63
-seeeye-0.0.2.dist-info/LICENSE,sha256=kVdhDldPTgkI0N-t0mNlqix21PXulpLy6pT71bkscTQ,1092
-seeeye-0.0.2.dist-info/METADATA,sha256=6Od2gYYMICoie981Qkra-OvmNbt9NoZ5whRXwr6TE_E,2941
-seeeye-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-seeeye-0.0.2.dist-info/top_level.txt,sha256=JqUP3rOzYUVQV4g4zKPF7kt3EoB7tiVgcWDINQmDIW4,5
-seeeye-0.0.2.dist-info/RECORD,,
+seeeye-0.0.3.dist-info/LICENSE,sha256=kVdhDldPTgkI0N-t0mNlqix21PXulpLy6pT71bkscTQ,1092
+seeeye-0.0.3.dist-info/METADATA,sha256=9UvlhB0H96JTczrUSCgweKddFSlwAAPROITDhN8U_nE,2941
+seeeye-0.0.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+seeeye-0.0.3.dist-info/entry_points.txt,sha256=AvnV-B3vp5CsY752DIbcr0s22d3VA3XHzdZHT5WcniQ,39
+seeeye-0.0.3.dist-info/top_level.txt,sha256=JqUP3rOzYUVQV4g4zKPF7kt3EoB7tiVgcWDINQmDIW4,5
+seeeye-0.0.3.dist-info/RECORD,,
```

