# Comparing `tmp/prr-0.3.1.tar.gz` & `tmp/prr-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prr-0.3.1.tar", max compression
+gzip compressed data, was "prr-0.4.0.tar", max compression
```

## Comparing `prr-0.3.1.tar` & `prr-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,190 @@
--rw-r--r--   0        0        0     1074 2023-05-07 19:46:47.449469 prr-0.3.1/LICENSE
--rw-r--r--   0        0        0    20237 2023-05-30 10:52:02.806517 prr-0.3.1/README.md
--rwxr-xr-x   0        0        0        0 2023-05-13 08:47:25.401520 prr-0.3.1/prr/__init__.py
--rwxr-xr-x   0        0        0     3697 2023-05-23 10:57:14.414579 prr-0.3.1/prr/__main__.py
--rwxr-xr-x   0        0        0     4385 2023-05-23 10:57:14.414734 prr-0.3.1/prr/commands/run.py
--rwxr-xr-x   0        0        0     2395 2023-05-23 10:57:14.414830 prr-0.3.1/prr/commands/watch.py
--rw-r--r--   0        0        0      376 2023-05-23 10:57:14.415002 prr-0.3.1/prr/prompt/__init__.py
--rw-r--r--   0        0        0     1744 2023-05-23 10:57:14.415110 prr-0.3.1/prr/prompt/model_options.py
--rw-r--r--   0        0        0     6538 2023-05-23 10:57:14.415244 prr-0.3.1/prr/prompt/prompt_config.py
--rw-r--r--   0        0        0     1980 2023-05-23 10:57:14.415364 prr-0.3.1/prr/prompt/prompt_loader.py
--rw-r--r--   0        0        0     3165 2023-05-23 10:57:14.415488 prr-0.3.1/prr/prompt/prompt_template.py
--rw-r--r--   0        0        0      834 2023-05-23 10:57:14.415581 prr-0.3.1/prr/prompt/service_config.py
--rw-r--r--   0        0        0     1393 2023-05-23 10:57:14.415747 prr-0.3.1/prr/runner/__init__.py
--rw-r--r--   0        0        0      654 2023-05-23 10:57:14.415829 prr-0.3.1/prr/runner/prompt_run.py
--rw-r--r--   0        0        0      954 2023-05-23 10:57:14.416098 prr-0.3.1/prr/runner/prompt_run_result.py
--rw-r--r--   0        0        0      767 2023-05-23 10:57:14.416178 prr-0.3.1/prr/runner/request.py
--rw-r--r--   0        0        0      810 2023-05-23 10:57:14.416439 prr-0.3.1/prr/runner/response.py
--rw-r--r--   0        0        0     2874 2023-05-23 10:57:14.416540 prr-0.3.1/prr/runner/saver.py
--rw-r--r--   0        0        0     2436 2023-05-23 10:57:14.416727 prr-0.3.1/prr/services/providers/anthropic/complete.py
--rw-r--r--   0        0        0     1507 2023-05-30 10:52:02.808566 prr-0.3.1/prr/services/providers/bigcode/starcoder.py
--rw-r--r--   0        0        0     2941 2023-05-23 10:57:14.416885 prr-0.3.1/prr/services/providers/google/chat.py
--rw-r--r--   0        0        0     1951 2023-05-23 10:57:14.417015 prr-0.3.1/prr/services/providers/google/complete.py
--rw-r--r--   0        0        0     1429 2023-05-23 10:57:14.417158 prr-0.3.1/prr/services/providers/openai/chat.py
--rw-r--r--   0        0        0     1073 2023-05-30 10:52:02.808827 prr-0.3.1/prr/services/service_registry.py
--rw-r--r--   0        0        0      143 2023-05-23 10:57:14.417498 prr-0.3.1/prr/utils/config.py
--rw-r--r--   0        0        0      907 2023-05-30 10:52:39.886565 prr-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    21127 1970-01-01 00:00:00.000000 prr-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-19 13:16:07.000000 prr-0.4.0/LICENSE
+-rw-r--r--   0        0        0    20618 2023-07-28 09:44:55.543477 prr-0.4.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-19 13:16:07.000000 prr-0.4.0/prr/__init__.py
+-rwxr-xr-x   0        0        0     4266 2023-07-28 09:44:55.543477 prr-0.4.0/prr/__main__.py
+-rwxr-xr-x   0        0        0     4635 2023-07-28 09:44:55.543477 prr-0.4.0/prr/commands/run.py
+-rw-r--r--   0        0        0     2074 2023-07-28 09:44:55.543477 prr-0.4.0/prr/commands/ui.py
+-rwxr-xr-x   0        0        0     2395 2023-05-19 20:06:32.000000 prr-0.4.0/prr/commands/watch.py
+-rw-r--r--   0        0        0      156 2023-07-28 09:44:55.543477 prr-0.4.0/prr/prompt/__init__.py
+-rw-r--r--   0        0        0     2045 2023-07-28 09:44:55.543477 prr-0.4.0/prr/prompt/model_options.py
+-rw-r--r--   0        0        0     6510 2023-07-28 09:44:55.543477 prr-0.4.0/prr/prompt/prompt_config.py
+-rw-r--r--   0        0        0     1980 2023-05-19 20:06:32.000000 prr-0.4.0/prr/prompt/prompt_loader.py
+-rw-r--r--   0        0        0     3416 2023-07-28 09:44:55.543477 prr-0.4.0/prr/prompt/prompt_template.py
+-rw-r--r--   0        0        0      842 2023-06-18 14:49:17.616167 prr-0.4.0/prr/prompt/service_config.py
+-rw-r--r--   0        0        0      607 2023-07-28 09:44:55.543477 prr-0.4.0/prr/prompt_template.yaml
+-rw-r--r--   0        0        0     2919 2023-07-28 09:44:55.543477 prr-0.4.0/prr/runner/__init__.py
+-rw-r--r--   0        0        0     1042 2023-07-28 09:44:55.543477 prr-0.4.0/prr/runner/prompt_run.py
+-rw-r--r--   0        0        0     1664 2023-07-28 09:44:55.543477 prr-0.4.0/prr/runner/prompt_run_result.py
+-rw-r--r--   0        0        0     3087 2023-07-28 09:44:55.543477 prr-0.4.0/prr/runner/run_collection.py
+-rw-r--r--   0        0        0     2309 2023-07-28 09:44:55.543477 prr-0.4.0/prr/runner/saved_prompt_run.py
+-rw-r--r--   0        0        0     2347 2023-07-28 09:44:55.543477 prr-0.4.0/prr/runner/saved_service_run.py
+-rw-r--r--   0        0        0     2595 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/providers/anthropic/complete.py
+-rw-r--r--   0        0        0     1457 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/providers/bigcode/starcoder.py
+-rw-r--r--   0        0        0      796 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/providers/elevenlabs/tts.py
+-rw-r--r--   0        0        0     2606 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/providers/google/chat.py
+-rw-r--r--   0        0        0     1499 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/providers/google/complete.py
+-rw-r--r--   0        0        0     1473 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/providers/openai/chat.py
+-rw-r--r--   0        0        0     1006 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/providers/test/test_service.py
+-rw-r--r--   0        0        0      650 2023-06-18 14:49:17.616167 prr-0.4.0/prr/services/service_base.py
+-rw-r--r--   0        0        0     1341 2023-07-28 09:44:55.543477 prr-0.4.0/prr/services/service_registry.py
+-rw-r--r--   0        0        0     1105 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/prompt_files.py
+-rw-r--r--   0        0        0     5286 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/routers/diff.py
+-rw-r--r--   0        0        0     2653 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/routers/edit.py
+-rw-r--r--   0        0        0     3869 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/routers/runs.py
+-rw-r--r--   0        0        0     1044 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/routers/state.py
+-rw-r--r--   0        0        0     7606 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/css/index.css
+-rw-r--r--   0        0        0   104601 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/CHANGELOG.md
+-rw-r--r--   0        0        0     1098 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/LICENSE
+-rw-r--r--   0        0        0     5479 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/README.md
+-rw-r--r--   0        0        0    63064 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/ThirdPartyNotices.txt
+-rw-r--r--   0        0        0    73464 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/browser/ui/codicons/codicon/codicon.ttf
+-rw-r--r--   0        0        0      537 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.de.js
+-rw-r--r--   0        0        0      537 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.es.js
+-rw-r--r--   0        0        0      537 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.fr.js
+-rw-r--r--   0        0        0      537 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.it.js
+-rw-r--r--   0        0        0      537 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.ja.js
+-rw-r--r--   0        0        0      531 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.js
+-rw-r--r--   0        0        0      537 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.ko.js
+-rw-r--r--   0        0        0      537 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.ru.js
+-rw-r--r--   0        0        0      543 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.zh-cn.js
+-rw-r--r--   0        0        0      543 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/common/worker/simpleWorker.nls.zh-tw.js
+-rw-r--r--   0        0        0   310019 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/base/worker/workerMain.js
+-rw-r--r--   0        0        0    14986 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/abap/abap.js
+-rw-r--r--   0        0        0     4775 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/apex/apex.js
+-rw-r--r--   0        0        0     1673 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/azcli/azcli.js
+-rw-r--r--   0        0        0     2666 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/bat/bat.js
+-rw-r--r--   0        0        0     3361 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/bicep/bicep.js
+-rw-r--r--   0        0        0     3016 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/cameligo/cameligo.js
+-rw-r--r--   0        0        0    10472 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/clojure/clojure.js
+-rw-r--r--   0        0        0     4417 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/coffee/coffee.js
+-rw-r--r--   0        0        0     6299 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/cpp/cpp.js
+-rw-r--r--   0        0        0     5351 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/csharp/csharp.js
+-rw-r--r--   0        0        0     2240 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/csp/csp.js
+-rw-r--r--   0        0        0     5331 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/css/css.js
+-rw-r--r--   0        0        0     4212 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/cypher/cypher.js
+-rw-r--r--   0        0        0     5073 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/dart/dart.js
+-rw-r--r--   0        0        0     2704 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/dockerfile/dockerfile.js
+-rw-r--r--   0        0        0     6163 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/ecl/ecl.js
+-rw-r--r--   0        0        0    11053 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/elixir/elixir.js
+-rw-r--r--   0        0        0     2635 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/flow9/flow9.js
+-rw-r--r--   0        0        0    17189 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/freemarker2/freemarker2.js
+-rw-r--r--   0        0        0     3810 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/fsharp/fsharp.js
+-rw-r--r--   0        0        0     3476 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/go/go.js
+-rw-r--r--   0        0        0     3089 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/graphql/graphql.js
+-rw-r--r--   0        0        0     7867 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/handlebars/handlebars.js
+-rw-r--r--   0        0        0     4411 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/hcl/hcl.js
+-rw-r--r--   0        0        0     6095 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/html/html.js
+-rw-r--r--   0        0        0     1922 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/ini/ini.js
+-rw-r--r--   0        0        0     4044 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/java/java.js
+-rw-r--r--   0        0        0     7177 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/javascript/javascript.js
+-rw-r--r--   0        0        0     8052 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/julia/julia.js
+-rw-r--r--   0        0        0     4266 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/kotlin/kotlin.js
+-rw-r--r--   0        0        0     4721 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/less/less.js
+-rw-r--r--   0        0        0     3262 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/lexon/lexon.js
+-rw-r--r--   0        0        0     5045 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/liquid/liquid.js
+-rw-r--r--   0        0        0     2944 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/lua/lua.js
+-rw-r--r--   0        0        0     3636 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/m3/m3.js
+-rw-r--r--   0        0        0     4619 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/markdown/markdown.js
+-rw-r--r--   0        0        0     3402 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/mips/mips.js
+-rw-r--r--   0        0        0     5737 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/msdax/msdax.js
+-rw-r--r--   0        0        0    12099 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/mysql/mysql.js
+-rw-r--r--   0        0        0     3239 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/objective-c/objective-c.js
+-rw-r--r--   0        0        0     3822 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/pascal/pascal.js
+-rw-r--r--   0        0        0     2833 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/pascaligo/pascaligo.js
+-rw-r--r--   0        0        0     9078 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/perl/perl.js
+-rw-r--r--   0        0        0    14289 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/pgsql/pgsql.js
+-rw-r--r--   0        0        0     8848 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/php/php.js
+-rw-r--r--   0        0        0     2504 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/pla/pla.js
+-rw-r--r--   0        0        0     8687 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/postiats/postiats.js
+-rw-r--r--   0        0        0    17774 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/powerquery/powerquery.js
+-rw-r--r--   0        0        0     4104 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/powershell/powershell.js
+-rw-r--r--   0        0        0     9877 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/protobuf/protobuf.js
+-rw-r--r--   0        0        0     5649 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/pug/pug.js
+-rw-r--r--   0        0        0     4702 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/python/python.js
+-rw-r--r--   0        0        0     3762 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/qsharp/qsharp.js
+-rw-r--r--   0        0        0     3948 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/r/r.js
+-rw-r--r--   0        0        0     9861 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/razor/razor.js
+-rw-r--r--   0        0        0     4381 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/redis/redis.js
+-rw-r--r--   0        0        0    12631 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/redshift/redshift.js
+-rw-r--r--   0        0        0     4740 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/restructuredtext/restructuredtext.js
+-rw-r--r--   0        0        0     9327 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/ruby/ruby.js
+-rw-r--r--   0        0        0     4983 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/rust/rust.js
+-rw-r--r--   0        0        0     2648 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/sb/sb.js
+-rw-r--r--   0        0        0     8143 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/scala/scala.js
+-rw-r--r--   0        0        0     2594 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/scheme/scheme.js
+-rw-r--r--   0        0        0     7232 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/scss/scss.js
+-rw-r--r--   0        0        0     3898 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/shell/shell.js
+-rw-r--r--   0        0        0    19428 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/solidity/solidity.js
+-rw-r--r--   0        0        0     3591 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/sophia/sophia.js
+-rw-r--r--   0        0        0     3379 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/sparql/sparql.js
+-rw-r--r--   0        0        0    11118 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/sql/sql.js
+-rw-r--r--   0        0        0     8209 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/st/st.js
+-rw-r--r--   0        0        0     5997 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/swift/swift.js
+-rw-r--r--   0        0        0     8444 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/systemverilog/systemverilog.js
+-rw-r--r--   0        0        0     4392 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/tcl/tcl.js
+-rw-r--r--   0        0        0     6795 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/twig/twig.js
+-rw-r--r--   0        0        0     6500 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/typescript/typescript.js
+-rw-r--r--   0        0        0     6610 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/vb/vb.js
+-rw-r--r--   0        0        0     8146 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/wgsl/wgsl.js
+-rw-r--r--   0        0        0     3492 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/xml/xml.js
+-rw-r--r--   0        0        0     5096 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/basic-languages/yaml/yaml.js
+-rw-r--r--   0        0        0   107356 2023-07-28 09:44:55.583478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.css
+-rw-r--r--   0        0        0  3329321 2023-07-28 09:44:55.590144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.js
+-rw-r--r--   0        0        0   114926 2023-07-28 09:44:55.590144 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.de.js
+-rw-r--r--   0        0        0   115058 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.es.js
+-rw-r--r--   0        0        0   126358 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.fr.js
+-rw-r--r--   0        0        0   116969 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.it.js
+-rw-r--r--   0        0        0   236069 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.ja.js
+-rw-r--r--   0        0        0    91639 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.js
+-rw-r--r--   0        0        0   195409 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.ko.js
+-rw-r--r--   0        0        0   485940 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.ru.js
+-rw-r--r--   0        0        0   148711 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.zh-cn.js
+-rw-r--r--   0        0        0   151610 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/editor/editor.main.nls.zh-tw.js
+-rw-r--r--   0        0        0    34290 2023-07-28 09:44:55.593478 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/css/cssMode.js
+-rw-r--r--   0        0        0   776551 2023-07-28 09:44:55.596811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/css/cssWorker.js
+-rw-r--r--   0        0        0    34826 2023-07-28 09:44:55.596811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/html/htmlMode.js
+-rw-r--r--   0        0        0   445890 2023-07-28 09:44:55.596811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/html/htmlWorker.js
+-rw-r--r--   0        0        0    40280 2023-07-28 09:44:55.596811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/json/jsonMode.js
+-rw-r--r--   0        0        0   128871 2023-07-28 09:44:55.596811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/json/jsonWorker.js
+-rw-r--r--   0        0        0    23674 2023-07-28 09:44:55.596811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/typescript/tsMode.js
+-rw-r--r--   0        0        0  4602226 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/language/typescript/tsWorker.js
+-rw-r--r--   0        0        0    30027 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/static/monaco-editor/min/vs/loader.js
+-rw-r--r--   0        0        0      719 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.de.js.map
+-rw-r--r--   0        0        0      719 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.es.js.map
+-rw-r--r--   0        0        0      719 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.fr.js.map
+-rw-r--r--   0        0        0      719 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.it.js.map
+-rw-r--r--   0        0        0      719 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.ja.js.map
+-rw-r--r--   0        0        0      894 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.js.map
+-rw-r--r--   0        0        0      719 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.ko.js.map
+-rw-r--r--   0        0        0      719 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.ru.js.map
+-rw-r--r--   0        0        0      728 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.zh-cn.js.map
+-rw-r--r--   0        0        0      728 2023-07-28 09:44:55.543477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/common/worker/simpleWorker.nls.zh-tw.js.map
+-rw-r--r--   0        0        0  1215904 2023-07-28 09:44:55.573477 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/base/worker/workerMain.js.map
+-rw-r--r--   0        0        0 11809964 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.js.map
+-rw-r--r--   0        0        0   139641 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.de.js.map
+-rw-r--r--   0        0        0   139848 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.es.js.map
+-rw-r--r--   0        0        0   148094 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.fr.js.map
+-rw-r--r--   0        0        0   144710 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.it.js.map
+-rw-r--r--   0        0        0   155200 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.ja.js.map
+-rw-r--r--   0        0        0   118593 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.js.map
+-rw-r--r--   0        0        0   139049 2023-07-28 09:44:55.576811 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.ko.js.map
+-rw-r--r--   0        0        0   210324 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.ru.js.map
+-rw-r--r--   0        0        0   110864 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.zh-cn.js.map
+-rw-r--r--   0        0        0   112848 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/editor/editor.main.nls.zh-tw.js.map
+-rw-r--r--   0        0        0   124034 2023-07-28 09:44:55.580144 prr-0.4.0/prr/ui/static/monaco-editor/min-maps/vs/loader.js.map
+-rw-r--r--   0        0        0   321062 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/static/monaco-editor/monaco.d.ts
+-rw-r--r--   0        0        0     2935 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/static/monaco-editor/package.json
+-rw-r--r--   0        0        0     1906 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/_footer.html
+-rw-r--r--   0        0        0      268 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/_header.html
+-rw-r--r--   0        0        0      426 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/_menu.html
+-rw-r--r--   0        0        0     5527 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/_run_helpers.html
+-rw-r--r--   0        0        0     4305 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/diff.html
+-rw-r--r--   0        0        0     2140 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/edit.html
+-rw-r--r--   0        0        0      278 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/error.html
+-rw-r--r--   0        0        0     3246 2023-07-28 09:44:55.606811 prr-0.4.0/prr/ui/templates/run.html
+-rw-r--r--   0        0        0      416 2023-07-28 09:44:55.606811 prr-0.4.0/prr/utils/config.py
+-rw-r--r--   0        0        0      827 2023-06-18 14:49:17.616167 prr-0.4.0/prr/utils/request.py
+-rw-r--r--   0        0        0     1319 2023-07-28 09:44:55.606811 prr-0.4.0/prr/utils/response.py
+-rw-r--r--   0        0        0      971 2023-07-28 09:44:55.610145 prr-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    21638 1970-01-01 00:00:00.000000 prr-0.4.0/PKG-INFO
```

### Comparing `prr-0.3.1/LICENSE` & `prr-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prr-0.3.1/README.md` & `prr-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ## Note
 
 **prr** is in very early stages of development, so things might still change unexpectedly or explode embarrasingly.
 
 ## Features
 
-- Command-line execution of prompts
+- Command-line execution of prompts (now with web UI!)
 - Quick iteration on prompt design and paramter refinement with `watch` command
 - YAML configuration ties prompts to models and their configurations
 - Write prompt-scripts with #!/usr/bin/prr shebang and execute them directly
 - All prompts can optionally use templating language ([Jinja](https://jinja.palletsprojects.com/en/3.1.x/)) for flow control, partials and others
 - Execute multiple models, or configurations against the same prompt
 - Expandable to other LLM providers (current integrations are <100 lines of code each)
 - Each prompt run across models gives you stats on model response times and token counts used to work across performance, quality and cost factors
@@ -99,17 +99,29 @@
 ```bash
 # https://platform.openai.com/account/api-keys
 OPENAI_API_KEY="sk-..."
 
 # https://console.anthropic.com/account/keys
 ANTHROPIC_API_KEY="sk-ant-..."
 
+ELEVEN_LABS_API_KEY="9db0...."
+
 DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo"
 ```
 
+### Running web user interface
+
+Simply run prr with 'ui' command and your prompt path (if it doesn't exist, it will be created), like so:
+
+```sh
+$ prr ui ~/Desktop/my-prompt
+```
+
+Web browser will be launched with the UI connected to your command that you will use to launch the runs.
+
 #### For Google PaLM, you need to install the following dependencies:
 You need to install [Google Cloud SDK](https://cloud.google.com/sdk/docs/install) and you need to have access to a Vertex AI with Generative AI enabled.
 `prr` assumes you're logged in into your Google Cloud account and have access to the project you want to use.
 
 ```sh
 gcloud auth login
 ```
@@ -119,14 +131,16 @@
 ```
 
 ```sh
 gcloud auth application-default login
 ```
 
 
+
+
 ### Code completion
 Using Starcoder model you can get code completion for a variety of languages. Here's a quick example of how to use it (check out the content of `examples/code/completion.yaml`):
 
 ```sh
 $ prr run ./examples/code/completion.yaml
 ```
 
@@ -424,14 +438,15 @@
 
 ### Current integrations
 
 * OpenAI/chat - https://platform.openai.com/docs/guides/chat
 * Anthropic/complete - https://console.anthropic.com/docs/api
 * Google Vertex AI PaLM - https://cloud.google.com/vertex-ai/docs/generative-ai/learn/overview
 * Starcoder - https://huggingface.co/bigcode/starcoder
+* Eleven Labs - https://beta.elevenlabs.io
 
 ## Development
 
 1. Clone the repo
 
 ```sh
 $ git clone https://github.com/Forward-Operators/prr.git
```

#### html2text {}

```diff
@@ -4,20 +4,20 @@
 APIs. Easily refine your parameters, prompts and model choices to achieve the
 best results while iterating smoothly with a quick feedback loop. **prr** is
 released as an open-source project under the MIT License. Made by [Forward
 Operators](https://fwdoperators.com/). We work on LLM and ML-related projects
 with some awesome human beings and cool companies. Everyone is welcome to
 contribute! ## Note **prr** is in very early stages of development, so things
 might still change unexpectedly or explode embarrasingly. ## Features -
-Command-line execution of prompts - Quick iteration on prompt design and
-paramter refinement with `watch` command - YAML configuration ties prompts to
-models and their configurations - Write prompt-scripts with #!/usr/bin/prr
-shebang and execute them directly - All prompts can optionally use templating
-language ([Jinja](https://jinja.palletsprojects.com/en/3.1.x/)) for flow
-control, partials and others - Execute multiple models, or configurations
+Command-line execution of prompts (now with web UI!) - Quick iteration on
+prompt design and paramter refinement with `watch` command - YAML configuration
+ties prompts to models and their configurations - Write prompt-scripts with #!/
+usr/bin/prr shebang and execute them directly - All prompts can optionally use
+templating language ([Jinja](https://jinja.palletsprojects.com/en/3.1.x/)) for
+flow control, partials and others - Execute multiple models, or configurations
 against the same prompt - Expandable to other LLM providers (current
 integrations are <100 lines of code each) - Each prompt run across models gives
 you stats on model response times and token counts used to work across
 performance, quality and cost factors - Each prompt run is recorded in detail
 for later analysis including raw rendered prompt and raw completion ## TODO As
 this is early stage work, there's lots improvements that can be done in the
 future and you're welcome to contribute! - [x] Get rix of Python 3.10
@@ -47,19 +47,23 @@
 [Watch_the_video] #### Prompt configuration Let's configure a bunch of models
 to run our prompt on. This time, we're asking the LLMs to generate a React
 boilerplate code. [Watch_the_video] ### Installation & configuration Install it
 via `pip` ```sh $ pip install -U prr ``` Check `.env.example` - and save it as
 `~/.prr_rc`. Fill in your API keys for OpenAI, Anthropic and others: ```bash #
 https://platform.openai.com/account/api-keys OPENAI_API_KEY="sk-..." # https://
 console.anthropic.com/account/keys ANTHROPIC_API_KEY="sk-ant-..."
-DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo" ``` #### For Google PaLM, you need
-to install the following dependencies: You need to install [Google Cloud SDK]
-(https://cloud.google.com/sdk/docs/install) and you need to have access to a
-Vertex AI with Generative AI enabled. `prr` assumes you're logged in into your
-Google Cloud account and have access to the project you want to use. ```sh
+ELEVEN_LABS_API_KEY="9db0...." DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo" ```
+### Running web user interface Simply run prr with 'ui' command and your prompt
+path (if it doesn't exist, it will be created), like so: ```sh $ prr ui ~/
+Desktop/my-prompt ``` Web browser will be launched with the UI connected to
+your command that you will use to launch the runs. #### For Google PaLM, you
+need to install the following dependencies: You need to install [Google Cloud
+SDK](https://cloud.google.com/sdk/docs/install) and you need to have access to
+a Vertex AI with Generative AI enabled. `prr` assumes you're logged in into
+your Google Cloud account and have access to the project you want to use. ```sh
 gcloud auth login ``` ```sh gcloud config set project  ``` ```sh gcloud auth
 application-default login ``` ### Code completion Using Starcoder model you can
 get code completion for a variety of languages. Here's a quick example of how
 to use it (check out the content of `examples/code/completion.yaml`): ```sh $
 prr run ./examples/code/completion.yaml ``` ### Run a prompt from a simple text
 file containing just a prompt Let's create a simple text file and call it
 `dingo` with the following content: ```text What are key traits of a Dingo dog?
@@ -198,24 +202,25 @@
 e4ec82a710f780100ccf671f85254bcf prompt_tokens: 43 stop_reason: stop_sequence
 tokens_used: 71 total_tokens: 71 truncated: false stats: elapsed_time:
 1.1589760780334473 end_time: 1683471638.6106346 start_time: 1683471637.4516585
 ``` ## Available models ### Current integrations * OpenAI/chat - https://
 platform.openai.com/docs/guides/chat * Anthropic/complete - https://
 console.anthropic.com/docs/api * Google Vertex AI PaLM - https://
 cloud.google.com/vertex-ai/docs/generative-ai/learn/overview * Starcoder -
-https://huggingface.co/bigcode/starcoder ## Development 1. Clone the repo ```sh
-$ git clone https://github.com/Forward-Operators/prr.git ``` 2. Make sure you
-have Python 3.9 or 3.10 installed. If you need to have multiple Python versions
-in your system, consider using [asdf](https://github.com/asdf-vm/asdf). 3.
-Install the required packages: This project uses Poetry. See [how to install]
-(https://python-poetry.org/docs/#installation) it. ```sh poetry shell poetry
-install ``` It will install `prr` executable file in your active python
-environment. 4. Setup your API keys Copy `.env.example` - and save it as
-`~/.prr_rc`. Fill in your API keys for OpenAI, Anthropic and others: ```bash #
-https://platform.openai.com/account/api-keys OPENAI_API_KEY="sk-..." # https://
+https://huggingface.co/bigcode/starcoder * Eleven Labs - https://
+beta.elevenlabs.io ## Development 1. Clone the repo ```sh $ git clone https://
+github.com/Forward-Operators/prr.git ``` 2. Make sure you have Python 3.9 or
+3.10 installed. If you need to have multiple Python versions in your system,
+consider using [asdf](https://github.com/asdf-vm/asdf). 3. Install the required
+packages: This project uses Poetry. See [how to install](https://python-
+poetry.org/docs/#installation) it. ```sh poetry shell poetry install ``` It
+will install `prr` executable file in your active python environment. 4. Setup
+your API keys Copy `.env.example` - and save it as `~/.prr_rc`. Fill in your
+API keys for OpenAI, Anthropic and others: ```bash # https://
+platform.openai.com/account/api-keys OPENAI_API_KEY="sk-..." # https://
 console.anthropic.com/account/keys ANTHROPIC_API_KEY="sk-ant-..."
 DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo" # https://console.cloud.google.com
 GOOGLE_PROJECT="gcp-project-id" GOOGLE_LOCATION="us-central1" # https://
 huggingface.co/settings/tokens HF_TOKEN="hf_..." ``` You can also use
 DEFAULT_SERVICE to specify the model you want to use by default, but otherwise
 you're good to go! If you'd like to run this code during developmnent, you can
 use `python -m prr` to load the module. ## Contributing We'd love your help in
```

### Comparing `prr-0.3.1/prr/__main__.py` & `prr-0.4.0/prr/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python
 
 import argparse
 import os
-import sys
 
 from prr.commands.run import RunPromptCommand
+from prr.commands.ui import UIPromptCommand
 from prr.commands.watch import WatchPromptCommand
-from prr.prompt.model_options import ModelOptions
 from prr.utils.config import load_config
 
 config = load_config()
 
 
+def check_if_prompt_exists(prompt_path):
+    return os.path.exists(prompt_path) or os.path.exists(prompt_path + ".yaml")
+
+
 def main():
     parser = argparse.ArgumentParser(
         description="Run a prompt against configured models.",
         prog="prr",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
@@ -26,14 +29,17 @@
     )
     watch_parser = sub_parsers.add_parser(
         "watch", help="watch prompts/config changes to launch re-runs"
     )
     script_parser = sub_parsers.add_parser(
         "script", help="prompt script mode for use with #!/usr/bin/prr"
     )
+    ui_parser = sub_parsers.add_parser(
+        "ui", help="launch a web UI to analyze saved runs"
+    )
 
     def add_common_args(_parser):
         _parser.add_argument(
             "--abbrev",
             help="Abbreviate prompts and completions",
             action="store_true",
             default=False,
@@ -85,37 +91,47 @@
         _parser.add_argument(
             "--log",
             "-l",
             help="Save each run in <prompt>.runs directory",
             action="store_true",
             default=False,
         )
+
         _parser.add_argument("prompt_path", help="Path to prompt to run")
 
     add_common_args(run_parser)
     add_common_args(watch_parser)
     add_common_args(script_parser)
 
+    ui_parser.add_argument("prompt_path", help="Path to prompt to analyze")
+
     watch_parser.add_argument(
         "--cooldown", "-c", type=int, help="How much to wait after a re-run", default=5
     )
 
     args, prompt_args = parser.parse_known_args()
     parsed_args = vars(args)
 
+    if parsed_args["command"] == "ui":
+        if not check_if_prompt_exists(parsed_args["prompt_path"]):
+            raise Exception(f"Prompt file {parsed_args['prompt_path']} does not exist")
+        command = UIPromptCommand(parsed_args)
+        command.start()
+
     if parsed_args["command"] == "script":
         parsed_args["quiet"] = True
         parsed_args["abbrev"] = False
+
         command = RunPromptCommand(parsed_args, prompt_args)
         command.run_prompt()
 
     if parsed_args["command"] == "run":
         command = RunPromptCommand(parsed_args)
         command.run_prompt()
 
     if parsed_args["command"] == "watch":
-        command = WatchPromptCommand(parsed_args)
+        command = WatchPromptCommand(parsed_args, prompt_args)
         command.watch_prompt()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `prr-0.3.1/prr/commands/run.py` & `prr-0.4.0/prr/commands/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,102 +22,122 @@
         self.prompt_config = None
 
         if self.args["quiet"]:
             self.console = Console(file=StringIO())
         else:
             self.console = Console(log_time=False, log_path=False)
 
+        if self.args["log"]:
+            self.save_run = True
+        else:
+            self.save_run = False
+
         self.load_prompt_for_path()
-        self.runner = Runner(self.prompt_config)
+        self.runner = Runner(self.prompt_config, self.save_run, self.prompt_args)
+
+    def print_prompt(self, request):
+        if self.args["abbrev"]:
+            self.console.log(
+                "Prompt:      "
+                + "[yellow]"
+                + request.prompt_text(25).strip()
+                + f"[/yellow] ({len(request.prompt_text())} chars)"
+            )
+        else:
+            self.console.log(
+                Panel("[yellow]" + request.prompt_text().strip() + "[/yellow]")
+            )
+
+    def print_completion(self, response):
+        if self.args["abbrev"]:
+            self.console.log(
+                "Completion:  "
+                + "[green]"
+                + response.response_text(25).strip()
+                + f"[/green] ({len(response.response_content)} chars)"
+            )
+        else:
+            self.console.log(
+                Panel("[green]" + str(response.response_text()).strip() + "[/green]")
+            )
+
+    def print_basic_stats(self, result):
+        response = result.response
+
+        completion = (
+            f"[blue]Completion length[/blue]: {len(response.response_content)} bytes"
+        )
+        tokens_used = f"[blue]Tokens used[/blue]: {response.tokens_used()}"
+        elapsed_time = f"[blue]Elapsed time[/blue]: {round(result.elapsed_time, 2)}s"
+
+        self.console.log(f"{completion} {tokens_used} {elapsed_time}")
+
+    def print_run_parameters(self, service_name, request):
+        self.console.log(
+            f"🤖 [magenta]{service_name}[/magenta] {request.options.description()}",
+            style="frame",
+        )
 
     def print_run_results(self, result, run_save_directory):
         request = result.request
         response = result.response
 
         if self.args["quiet"]:
-            print(response.response_content)
-        else:
-            if self.args["abbrev"]:
-                self.console.log(
-                    "Prompt:      "
-                    + "[yellow]"
-                    + request.prompt_text(25).strip()
-                    + f"[/yellow] ({len(request.prompt_text())} chars)"
-                )
-                self.console.log(
-                    "Completion:  "
-                    + "[green]"
-                    + response.response_abbrev(25).strip()
-                    + f"[/green] ({len(response.response_content)} chars)"
-                )
+            # just print out the output verbatim
+            if isinstance(response.response_content, str):
+                print(response.response_content)
             else:
-                self.console.log(
-                    Panel("[yellow]" + request.prompt_text().strip() + "[/yellow]")
-                )
-                self.console.log(
-                    Panel("[green]" + response.response_content.strip() + "[/green]")
-                )
-
-            completion = f"[blue]Completion length[/blue]: {len(response.response_content)} bytes"
-            tokens_used = f"[blue]Tokens used[/blue]: {response.tokens_used()}"
-            elapsed_time = (
-                f"[blue]Elapsed time[/blue]: {round(result.elapsed_time, 2)}s"
-            )
-
-            self.console.log(f"{completion} {tokens_used} {elapsed_time}")
+                sys.stdout.buffer.write(response.response_content)
+        else:
+            self.print_completion(response)
+            self.print_basic_stats(result)
 
             if run_save_directory:
                 self.console.log(f"💾 {run_save_directory}")
+                self.console.log("")
 
-    def run_prompt_on_service(self, service_name, save=False):
-        # TODO/FIXME: doing all this here just to get the actual options
-        #             calculated after command line, defaults, config, etc
-        service_config = self.prompt_config.service_with_name(service_name)
-        service_config.process_option_overrides(self.args)
-        options = service_config.options
-
-        with self.console.status(
-            f":robot: [bold green]{service_name}[/bold green]"
-        ) as status:
-            self.console.log(
-                f"\n🤖 [bold]{service_name}[/bold] {options.description()}",
-                style="frame",
-            )
-
-            status.update(status="running model", spinner="dots8Bit")
-
-            result, run_save_directory = self.runner.run_service(
-                service_name, self.args, save
-            )
-
-            self.print_run_results(result, run_save_directory)
+    def on_request(self, service_name, request):
+        self.print_run_parameters(service_name, request)
+        self.print_prompt(request)
 
     def load_prompt_for_path(self):
         prompt_path = self.args["prompt_path"]
 
         self.console.log(f":magnifying_glass_tilted_left: Reading {prompt_path}")
 
         loader = PromptConfigLoader()
         self.prompt_config = loader.load_from_path(prompt_path)
 
-    def run_prompt(self):
-        services_to_run = self.prompt_config.configured_services()
+    def services_to_run(self):
+        _services = self.prompt_config.configured_services()
 
-        if services_to_run == []:
+        if _services == []:
             if self.args["service"]:
-                services_to_run = [self.args["service"]]
+                _services = [self.args["service"]]
                 self.console.log(
-                    f":racing_car:  Running service {self.args['service']} with default options."
+                    f":racing_car:  Running service {self.args['service']}."
                 )
             else:
                 self.console.log(
                     f":x: No services configured for prompt {self.args['prompt_path']}, in ~/.prr_rc nor given in command-line."
                 )
                 exit(-1)
         else:
-            self.console.log(f":racing_car:  Running services: {services_to_run}")
+            self.console.log(f":racing_car:  Running services: {_services}")
 
-        if not self.args["abbrev"]:
-            self.console.log(Panel(self.prompt_config.template_text()))
+        return _services
+
+    def run_prompt(self):
+        services = self.services_to_run()
 
-        for service_name in services_to_run:
-            self.run_prompt_on_service(service_name, self.args["log"])
+        self.runner.run_services(
+            services,
+            self.args,
+            {
+                "on_request": lambda service_name, request: self.on_request(
+                    service_name, request
+                ),
+                "on_result": lambda service_name, result, run_save_directory: self.print_run_results(
+                    result, run_save_directory
+                ),
+            },
+        )
```

### Comparing `prr-0.3.1/prr/commands/watch.py` & `prr-0.4.0/prr/commands/watch.py`

 * *Files identical despite different names*

### Comparing `prr-0.3.1/prr/prompt/prompt_config.py` & `prr-0.4.0/prr/prompt/prompt_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 
         # services: (ServiceConfig)
         self.services = {}
 
         # version: 1
         self.version = None
 
-    def template_text(self):
-        return self.template.render_text()
+    def render_text(self, prompt_args=None):
+        return self.template.render_text(prompt_args)
+
+    def render_messages(self, prompt_args=None):
+        return self.template.render_messages(prompt_args)
 
     # raw YAML file
     def load_from_config_contents(self, raw_config_content):
         # raw YAML string
         self.raw_config_content = raw_config_content
 
         # parse raw YAML content into a dictionary
@@ -68,24 +71,21 @@
             return ServiceConfig(service_name, service_name)
 
     # returns options for specific service, already includes all option inheritance
     def options_for_service(self, service_name):
         return self.service_with_name(service_name).options
 
     def option_for_service(self, service_name, option_name):
-        return self.options_for_service(service_name).option(option_name)
+        return self.options_for_service(service_name).value(option_name)
 
     def file_dependencies(self):
-        _dependencies = []
-        for message in self.template.messages:
-            for dependency in message.file_dependencies:
-                if dependency not in _dependencies:
-                    _dependencies.append(dependency)
+        if self.template:
+            return self.template.file_dependencies()
 
-        return _dependencies
+        return []
 
     ####################################################
 
     def __parse(self):
         self.__parse_version()
         self.__parse_prompt()
         self.__parse_services()
@@ -125,15 +125,15 @@
 
     # high level "services:" parsing
     def __parse_services(self):
         if self.config_content:
             _services = self.config_content.get("services")
 
             if _services:
-                options_for_all_services = _services.get("options")
+                options_for_all_services = _services.get("options") or {}
 
                 #
                 # if we have models + prompt-level model options
                 #
                 # services:
                 #   models:
                 #     - 'openai/chat/gpt-4'
```

### Comparing `prr-0.3.1/prr/prompt/prompt_loader.py` & `prr-0.4.0/prr/prompt/prompt_loader.py`

 * *Files identical despite different names*

### Comparing `prr-0.3.1/prr/prompt/prompt_template.py` & `prr-0.4.0/prr/prompt/prompt_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
 import jinja2
+from jinja2 import meta
 
 
 class PromptMessage:
     def __init__(
         self, content_template_string, search_path=".", role="user", name=None
     ):
         self.content_template_string = content_template_string
@@ -21,19 +22,28 @@
         )
 
         self.template_env = jinja2.Environment(loader=template_loader)
         self.__add_dependency_files_from_jinja_template(content_template_string)
 
         self.template = self.template_env.from_string(self.content_template_string)
 
-    def render_text(self, args=[]):
-        return self.template.render({"prompt_args": args})
+    def is_system(self):
+        return self.role == "system"
 
-    def render_message(self, args=[]):
-        _message = {"role": self.role, "content": self.render_text(args)}
+    def is_user(self):
+        return self.role == "user"
+
+    def is_assistant(self):
+        return self.role == "assistant"
+
+    def render_text(self, prompt_args=None):
+        return self.template.render({"prompt_args": prompt_args})
+
+    def render_message(self, prompt_args=None):
+        _message = {"role": self.role, "content": self.render_text(prompt_args)}
 
         if self.name:
             _message.update({"name": self.name})
 
         return _message
 
     def __add_dependency_files_from_jinja_template(self, jinja_template_content):
@@ -44,20 +54,20 @@
 
 
 # base class
 class PromptTemplate:
     def __init__(self):
         self.messages = []
 
-    def render_text(self, args=[]):
+    def render_text(self, args=None):
         rendered_texts = [message.render_text(args) for message in self.messages]
 
         return "\n".join(rendered_texts)
 
-    def render_messages(self, args=[]):
+    def render_messages(self, args=None):
         return [message.render_message(args) for message in self.messages]
 
     def file_dependencies(self):
         _dependencies = []
         for message in self.messages:
             for dependency in message.file_dependencies:
                 if dependency not in _dependencies:
```

### Comparing `prr-0.3.1/prr/prompt/service_config.py` & `prr-0.4.0/prr/prompt/service_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
         self.model = model  # full model path, e.g. "openai/chat/gpt-5"
         self.options = ModelOptions(options or {})
 
     def process_option_overrides(self, option_overrides):
         self.options.update_options(option_overrides)
 
     # which model to use with the service
-    # like gpt-4.5-turbo or claude-v1.3-100k
+    # like "gpt-4.5-turbo" or "claude-v1.3-100k"
     def model_name(self):
         return self.model.split("/")[-1]
 
     # which service so use
-    # like openai/chat or anthropic/complete
+    # like "openai/chat" or "anthropic/complete"
     def service_key(self):
         return "/".join(self.model.split("/")[:-1])
 
     def to_dict(self):
         return {"model": self.config_name(), "options": self.options.to_dict()}
```

### Comparing `prr-0.3.1/prr/runner/prompt_run_result.py` & `prr-0.4.0/prr/runner/prompt_run_result.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,31 +6,42 @@
         self.prompt = prompt
         self.config = config
         self.start_time = None
         self.end_time = None
         self.elapsed_time = None
         self.request = None
         self.response = None
+        self.tokens_per_second = None
+        self.tokens_generated = None
 
     def before_run(self):
         self.start_time = time.time()
 
     def after_run(self):
         self.end_time = time.time()
         self.elapsed_time = self.end_time - self.start_time
 
     def update_with_response(self, response):
         self.response = response
+        self.tokens_generated = self.response.tokens_generated()
+
+        if self.tokens_generated != None:
+            self.tokens_per_second = self.tokens_generated / self.elapsed_time
 
     def update_with_request(self, request):
         self.request = request
 
     def metrics(self):
         return {
             "stats": {
                 "start_time": self.start_time,
                 "end_time": self.end_time,
                 "elapsed_time": self.elapsed_time,
+                "tokens_per_second": self.tokens_per_second,
+                "tokens_generated": self.tokens_generated,
             },
             "request": self.request.to_dict(),
             "response": self.response.to_dict(),
         }
+
+    def __str__(self):
+        return f"PromptRunResult(prompt={self.prompt}, config={self.config}, start_time={self.start_time}, end_time={self.end_time}, elapsed_time={self.elapsed_time}, request={self.request}, response={self.response}, tokens_per_second={self.tokens_per_second}, tokens_generated={self.tokens_generated})"
```

### Comparing `prr-0.3.1/prr/runner/request.py` & `prr-0.4.0/prr/utils/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import yaml
 
 
-# request we're sending to the service
+# request we're sending to the service - prompts rendered, options parsed
 class ServiceRequest:
-    def __init__(self, service_config, rendered_prompt_content):
+    def __init__(self, service_config, rendered_prompt_content, options):
         self.service_config = service_config
         self.prompt_content = rendered_prompt_content
+        self.options = options
 
     def to_dict(self):
         return {
             "model": self.service_config.model,
-            "options": self.service_config.options.to_dict(),
+            "options": self.options.to_dict(),
         }
 
     def prompt_text(self, max_len=0):
         if isinstance(self.prompt_content, str):
             text = self.prompt_content
         else:
             text = yaml.dump(self.prompt_content)
```

### Comparing `prr-0.3.1/prr/runner/saver.py` & `prr-0.4.0/prr/runner/saved_service_run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,74 @@
 import os
-from datetime import datetime
 
 import yaml
 
 
-class PromptRunSaver:
-    def __init__(self, prompt_config):
-        self.prompt_config = prompt_config
-        self.run_time = datetime.now()
-        self.runs_subdir = self.run_root_directory_path()
+class SavedServiceRun:
+    def __init__(self, saved_service_run_path):
+        self.saved_service_run_path = saved_service_run_path
 
-    def run_root_directory_path_for_runs_dir(self, runs_dir):
-        try:
-            previous_runs = os.listdir(runs_dir)
-        except FileNotFoundError:
-            return os.path.join(runs_dir, "1")
+    def name(self):
+        return os.path.basename(self.saved_service_run_path)
 
-        run_id = 1
-        while True:
-            run_dir = os.path.join(runs_dir, str(run_id))
+    def prompt_content(self):
+        return self.read_file(["prompt.yaml", "prompt"])
 
-            if not os.path.exists(run_dir):
-                return run_dir
+    def read_file(self, filenames):
+        for filename in filenames:
+            filename_path = os.path.join(self.saved_service_run_path, filename)
 
-            run_id += 1
+            if os.path.isfile(filename_path) and os.access(filename_path, os.R_OK):
+                return open(filename_path, "r").read()
 
-    def run_root_directory_path(self):
-        dirname = self.prompt_config.search_path
+    def output_content(self):
+        # "completion" is old style
+        return self.read_file(["output", "completion"])
 
-        if self.prompt_config.filename:
-            basename = os.path.basename(self.prompt_config.filename)
-        else:
-            basename = "prr"
+    def run_details(self):
+        #  try-catch on yaml load here
+        content = self.run_details_content()
 
-        root, extension = os.path.splitext(basename)
+        if content:
+            yaml_content = yaml.safe_load(content)
+            return yaml_content
 
-        if extension == ".yaml":
-            basename = root
+        return {}
 
-        runs_dir = os.path.join(dirname, f"{basename}.runs")
+    def run_details_content(self):
+        return self.read_file(["run.yaml"])
 
-        return self.run_root_directory_path_for_runs_dir(runs_dir)
-
-    def run_directory_path(self, service_or_model_name):
-        model_name_part = service_or_model_name.replace("/", "-")
-
-        return os.path.join(self.runs_subdir, model_name_part)
-
-    def prepare_run_directory(self, service_or_model_name):
-        run_dir = self.run_directory_path(service_or_model_name)
-
-        os.makedirs(run_dir, exist_ok=True)
-
-        return run_dir
-
-    def save_prompt(self, run_directory, request):
+    def save_prompt(self, request):
         prompt_content = request.prompt_content
 
         if prompt_content:
             if isinstance(prompt_content, str):
-                prompt_file = os.path.join(run_directory, f"prompt")
+                prompt_file = os.path.join(self.saved_service_run_path, f"prompt")
 
                 with open(prompt_file, "w") as f:
                     f.write(prompt_content)
             else:
-                prompt_file = os.path.join(run_directory, f"prompt.yaml")
+                prompt_file = os.path.join(self.saved_service_run_path, f"prompt.yaml")
 
                 with open(prompt_file, "w") as f:
                     yaml.dump(prompt_content, f, default_flow_style=False)
 
-    def save_completion(self, run_directory, response):
-        completion_file = os.path.join(run_directory, f"completion")
+    def save_completion(self, response):
+        completion_file = os.path.join(self.saved_service_run_path, f"output")
 
         with open(completion_file, "w") as f:
             f.write(response.response_content)
 
-    def save_run(self, run_directory, result):
-        run_file = os.path.join(run_directory, f"run.yaml")
+    def save_run(self, result):
+        run_file = os.path.join(self.saved_service_run_path, f"run.yaml")
         run_data = result.metrics()
 
         with open(run_file, "w") as f:
             yaml.dump(run_data, f, default_flow_style=False)
 
-    def save(self, service_or_model_name, result):
-        run_directory = self.prepare_run_directory(service_or_model_name)
-
-        self.save_prompt(run_directory, result.request)
-        self.save_completion(run_directory, result.response)
-        self.save_run(run_directory, result)
-
-        return run_directory
+    def save(self, result):
+        if not os.path.exists(self.saved_service_run_path):
+            os.makedirs(self.saved_service_run_path)
+
+        self.save_prompt(result.request)
+        self.save_completion(result.response)
+        self.save_run(result)
```

### Comparing `prr-0.3.1/prr/services/providers/bigcode/starcoder.py` & `prr-0.4.0/prr/services/providers/bigcode/starcoder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 from huggingface_hub import Repository
 from text_generation import Client
 
-from prr.runner.request import ServiceRequest
-from prr.runner.response import ServiceResponse
-from prr.utils.config import load_config
+from prr.services.service_base import ServiceBase
+from prr.utils.config import ensure_api_key, load_config
+from prr.utils.request import ServiceRequest
+from prr.utils.response import ServiceResponse
 
 config = load_config()
 
-HF_TOKEN = config.get("HF_TOKEN", None)
 API_URL = "https://api-inference.huggingface.co/models/bigcode/starcoder"
 
 FIM_PREFIX = "<fim_prefix>"
 FIM_MIDDLE = "<fim_middle>"
 FIM_SUFFIX = "<fim_suffix>"
 
 FIM_INDICATOR = "<FILL_HERE>"
 
 
-class ServiceBigcodeStarcoder:
+class ServiceBigcodeStarcoder(ServiceBase):
     provider = "bigcode"
     service = "starcoder"
+    options = ["temperature", "max_tokens", "top_p", "repetition_penalty"]
 
-    def run(self, prompt, service_config):
-        self.service_config = service_config
-        self.prompt = prompt
+    def run(self):
+        HF_TOKEN = ensure_api_key(config, "HF_TOKEN")
 
         client = Client(
             API_URL,
             headers={"Authorization": f"Bearer {HF_TOKEN}"},
         )
 
-        options = self.service_config.options
-
-        prompt_text = prompt.template_text()
-
-        service_request = ServiceRequest(service_config, prompt_text)
-
-        response = client.generate(
-            prompt_text,
-            temperature=options.temperature,
-            max_new_tokens=options.max_tokens,
-            top_p=options.top_p,
-            # repetition_penalty=options.repetition_penalty,
+        completion = client.generate(
+            self.request.prompt_content,
+            temperature=self.option("temperature"),
+            max_new_tokens=self.option("max_tokens"),
+            top_p=self.option("top_p"),
+            repetition_penalty=self.option("repetition_penalty"),
         )
 
-        service_response = ServiceResponse(
-            response.generated_text,
+        self.response = ServiceResponse(
+            completion.generated_text,
             {
-                "tokens_used": response.details.generated_tokens,
-                "stop_reason": response.details.finish_reason,
+                "tokens_used": completion.details.generated_tokens,
+                "stop_reason": str(completion.details.finish_reason),
             },
         )
 
-        return service_request, service_response
+        return self.request, self.response
```

### Comparing `prr-0.3.1/prr/services/providers/google/chat.py` & `prr-0.4.0/prr/services/providers/google/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,79 @@
 from google.cloud import aiplatform
 from vertexai.preview.language_models import ChatModel, InputOutputTextPair
 
-from prr.runner.request import ServiceRequest
-from prr.runner.response import ServiceResponse
-from prr.utils.config import load_config
+from prr.services.service_base import ServiceBase
+from prr.utils.config import ensure_api_key, load_config
+from prr.utils.response import ServiceResponse
 
 config = load_config()
 
-aiplatform.init(
-    # your Google Cloud Project ID or number
-    # environment default used is not set
-    project=config.get("GOOGLE_PROJECT"),
-    # the Vertex AI region you will use
-    # defaults to us-central1
-    location=config.get("GOOGLE_LOCATION"),
-    # custom google.auth.credentials.Credentials
-    # environment default creds used if not set
-    # credentials=config[my_credentials],
-)
 
-
-class ServiceGoogleChat:
+class ServiceGoogleChat(ServiceBase):
     provider = "google"
     service = "chat"
+    options = ["max_tokens", "temperature", "top_k", "top_p"]
 
-    def run(self, prompt, service_config):
-        self.service_config = service_config
-        options = self.service_config.options
-        self.prompt = prompt
-
-        messages = self.messages_from_prompt()
+    def run(self):
+        aiplatform.init(
+            # your Google Cloud Project ID or number
+            # environment default used is not set
+            project=ensure_api_key(config, "GOOGLE_PROJECT"),
+            # the Vertex AI region you will use
+            # defaults to us-central1
+            location=ensure_api_key(config, "GOOGLE_LOCATION"),
+            # custom google.auth.credentials.Credentials
+            # environment default creds used if not set
+            # credentials=config[my_credentials],
+        )
 
         model = ChatModel.from_pretrained(self.service_config.model_name())
 
-        service_request = ServiceRequest(self.service_config, {"messages": messages})
-
         parameters = {
-            "temperature": options.temperature,
-            "max_output_tokens": options.max_tokens,
-            "top_p": options.top_p,
-            "top_k": options.top_k,
+            "temperature": self.option("temperature"),
+            "max_output_tokens": self.option("max_tokens"),
+            "top_p": self.option("top_p"),
+            "top_k": self.option("top_k"),
         }
 
+        # TODO: support examples
         chat = model.start_chat(
-            context=f"""{self.context_from_messages()}""",
+            context=self.request.prompt_content["context"],
             examples=[],
         )
 
         response = chat.send_message(
-            f"""{self.message_from_messages()}""", **parameters
+            self.request.prompt_content["messages"], **parameters
         )
 
-        service_response = ServiceResponse(response.text, {})
-
-        return service_request, service_response
-
-    def messages_from_prompt(self):
-        messages = self.prompt.messages
-
-        # prefer messages in prompt if they exist
-        if messages:
-            return messages
-
-        return [{"role": "user", "content": self.prompt.text()}]
+        self.response = ServiceResponse(response.text, {})
 
-    def context_from_messages(self):
-        messages = self.prompt.messages
+        return self.request, self.response
 
-        if messages:
-            for message in messages:
-                if message["role"] == "system":
-                    context = message["content"]
-        else:
-            context = None
-
-        return context
-
-    def examples_from_messages(self):
-        messages = self.prompt.messages
-
-        if messages:
-            examples = []
-            for message in messages:
-                if message["role"] == "examples":
-                    examples.append(
-                        InputOutputTextPair(message["input"], message["output"])
-                    )
-        else:
-            examples = []
-
-        return examples
+    def render_message(self, message):
+        return {
+            "author": "bot" if message.is_assistant() else "user",
+            "content": message.render_text(self.prompt_args),
+        }
 
-    def message_from_messages(self):
-        messages = self.prompt.messages
+    # define render prompt to change how the prompt is rendered
+    def render_prompt(self):
+        context_messages = []
+        chat_messages = []
+
+        # TODO: this should not reach so deep
+        if self.prompt.template.messages:
+            for message in self.prompt.template.messages:
+                if message.is_system():
+                    context_messages.append(message)
+                else:
+                    chat_messages.append(message)
 
-        if messages:
-            for message in messages:
-                if message["role"] == "user":
-                    message = message["content"]
-        else:
-            message = None
+        context_text = "\n".join(
+            [m.render_text(self.prompt_args) for m in context_messages]
+        )
+        messages = [self.render_message(m) for m in chat_messages]
 
-        return message
+        return {
+            "context": context_text,
+            "messages": messages,
+        }
```

### Comparing `prr-0.3.1/prr/services/providers/google/complete.py` & `prr-0.4.0/prr/services/providers/google/complete.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,46 @@
 from google.cloud import aiplatform
 from vertexai.preview.language_models import TextGenerationModel
 
-from prr.runner.request import ServiceRequest
-from prr.runner.response import ServiceResponse
-from prr.utils.config import load_config
+from prr.services.service_base import ServiceBase
+from prr.utils.config import ensure_api_key, load_config
+from prr.utils.response import ServiceResponse
 
 config = load_config()
 
-aiplatform.init(
-    # your Google Cloud Project ID or number
-    # environment default used is not set
-    project=config.get("GOOGLE_PROJECT", None),
-    # the Vertex AI region you will use
-    # defaults to us-central1
-    location=config.get("GOOGLE_LOCATION", None),
-    # custom google.auth.credentials.Credentials
-    # environment default creds used if not set
-    # credentials=config[my_credentials],
-)
 
-
-class ServiceGoogleComplete:
+class ServiceGoogleComplete(ServiceBase):
     provider = "google"
     service = "complete"
+    options = ["max_tokens", "temperature", "top_k", "top_p"]
 
-    def run(self, prompt, service_config):
-        self.service_config = service_config
-        options = self.service_config.options
-        self.prompt = prompt
-
-        prompt_text = self.prompt_text()
+    def run(self):
+        aiplatform.init(
+            # your Google Cloud Project ID or number
+            # environment default used is not set
+            project=ensure_api_key(config, "GOOGLE_PROJECT"),
+            # the Vertex AI region you will use
+            # defaults to us-central1
+            location=ensure_api_key(config, "GOOGLE_LOCATION"),
+            # custom google.auth.credentials.Credentials
+            # environment default creds used if not set
+            # credentials=config[my_credentials],
+        )
 
         client = TextGenerationModel.from_pretrained(self.service_config.model_name())
 
-        service_request = ServiceRequest(self.service_config, prompt_text)
-
-        options = self.service_config.options
-
-        response = client.predict(
+        result = client.predict(
             prompt_text,
-            max_output_tokens=options.max_tokens,
-            temperature=options.temperature,
-            top_k=options.top_k,
-            top_p=options.top_p,
+            max_output_tokens=self.option("max_tokens"),
+            temperature=self.option("temperature"),
+            top_k=self.option("top_k"),
+            top_p=self.option("top_p"),
         )
 
-        service_response = ServiceResponse(
-            str(response),
+        self.response = ServiceResponse(
+            str(result),
             {
-                "details": response,
+                "details": result,
             },
         )
 
-        return service_request, service_response
-
-    def prompt_text(self):
-        messages = self.prompt.messages
-
-        prompt_text = ""
-
-        if messages:
-            for message in messages:
-                if message["role"] != "assistant":
-                    prompt_text += " " + message["content"]
-
-        else:
-            prompt_text = self.prompt.text()
-
-        return messages
+        return self.request, self.response
```

### Comparing `prr-0.3.1/prr/services/providers/openai/chat.py` & `prr-0.4.0/prr/services/providers/openai/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import openai
 
-from prr.runner.request import ServiceRequest
-from prr.runner.response import ServiceResponse
-from prr.utils.config import load_config
+from prr.services.service_base import ServiceBase
+from prr.utils.config import ensure_api_key, load_config
+from prr.utils.response import ServiceResponse
 
 config = load_config()
-openai.api_key = config.get("OPENAI_API_KEY", None)
 
 
 # OpenAI model provider class
-class ServiceOpenAIChat:
+class ServiceOpenAIChat(ServiceBase):
     provider = "openai"
     service = "chat"
 
-    def run(self, prompt, service_config):
-        messages = prompt.template.render_messages()
+    # options we take into account
+    options = ["max_tokens", "temperature"]
 
-        service_request = ServiceRequest(service_config, {"messages": messages})
-
-        options = service_config.options
+    def run(self):
+        openai.api_key = ensure_api_key(config, "OPENAI_API_KEY")
 
         completion = openai.ChatCompletion.create(
-            model=service_config.model_name(),
-            messages=messages,
-            temperature=options.temperature,
-            max_tokens=options.max_tokens,
+            model=self.service_config.model_name(),
+            messages=self.request.prompt_content,
+            temperature=self.option("temperature"),
+            max_tokens=self.option("max_tokens"),
         )
 
         usage = completion.usage
-
         choices = completion.choices
-        first_choice = choices[0]
 
+        first_choice = choices[0]
         completion_content = first_choice.message.content
 
-        service_response = ServiceResponse(
+        self.response = ServiceResponse(
             completion_content,
             {
                 "choices": len(choices),
                 "tokens_used": usage.total_tokens,
                 "completion_tokens": usage.completion_tokens,
                 "prompt_tokens": usage.prompt_tokens,
                 "total_tokens": usage.total_tokens,
                 "finish_reason": first_choice.finish_reason,
             },
         )
 
-        return service_request, service_response
+        return self.request, self.response
+
+    def render_prompt(self):
+        return self.prompt.render_messages(self.prompt_args)
```

### Comparing `prr-0.3.1/prr/services/service_registry.py` & `prr-0.4.0/prr/services/service_registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from prr.services.providers.anthropic.complete import ServiceAnthropicComplete
-from prr.services.providers.bigcode.starcoder import ServiceBigcodeStarcoder
-from prr.services.providers.google.chat import ServiceGoogleChat
-from prr.services.providers.google.complete import ServiceGoogleComplete
-from prr.services.providers.openai.chat import ServiceOpenAIChat
-
-
 # main registry, where services are being... registered
 # and looked up for upon execution
 class ServiceRegistry:
     def __init__(self):
         self.services = {}
 
     def register(self, service_class):
         key = f"{service_class.provider}/{service_class.service}"
-        self.services[key] = service_class()
+        self.services[key] = service_class
 
     def register_all_services(self):
+        from prr.services.providers.anthropic.complete import ServiceAnthropicComplete
+        from prr.services.providers.bigcode.starcoder import ServiceBigcodeStarcoder
+        from prr.services.providers.elevenlabs.tts import ServiceElevenLabsTTS
+        from prr.services.providers.google.chat import ServiceGoogleChat
+        from prr.services.providers.google.complete import ServiceGoogleComplete
+        from prr.services.providers.openai.chat import ServiceOpenAIChat
+        from prr.services.providers.test.test_service import ServiceTest
+
         self.register(ServiceOpenAIChat)
         self.register(ServiceAnthropicComplete)
         self.register(ServiceBigcodeStarcoder)
         self.register(ServiceGoogleComplete)
         self.register(ServiceGoogleChat)
+        self.register(ServiceElevenLabsTTS)
+        self.register(ServiceTest)
 
     def service_for_service_config(self, service_config):
         key = service_config.service_key()
         return self.services[key]
```

### Comparing `prr-0.3.1/pyproject.toml` & `prr-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prr"
-version = "0.3.1"
+version = "0.4.0"
 description = "prr - command-line LLM prompt runner"
 authors = [ "Zbigniew Sobiecki <zbigniew@fwdoperators.com>" , "Mateusz Kozak <mateusz@fwdoperators.com>" ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -13,14 +13,17 @@
 anthropic = "^0.2.7"
 rich = "^13.3.5"
 Jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 google-cloud-aiplatform = "^1.25.0"
 huggingface-hub = "^0.14.1"
 text-generation = "^0.5.2"
+uvicorn = "^0.22.0"
+elevenlabs = "^0.2.21"
+fastapi = "^0.100.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.12.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
```

### Comparing `prr-0.3.1/PKG-INFO` & `prr-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: prr
-Version: 0.3.1
+Version: 0.4.0
 Summary: prr - command-line LLM prompt runner
 License: MIT
 Author: Zbigniew Sobiecki
 Author-email: zbigniew@fwdoperators.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: anthropic (>=0.2.7,<0.3.0)
+Requires-Dist: elevenlabs (>=0.2.21,<0.3.0)
+Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: google-cloud-aiplatform (>=1.25.0,<2.0.0)
 Requires-Dist: huggingface-hub (>=0.14.1,<0.15.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: text-generation (>=0.5.2,<0.6.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 # prr - The Prompt Runner
 
 Welcome to **prr - The Prompt Runner**!
 
 **prr** is a simple toolchain designed to help you run prompts across multiple Large Language Models (LLMs), whether they are hosted locally or accessible through APIs. Easily refine your parameters, prompts and model choices to achieve the best results while iterating smoothly with a quick feedback loop.
@@ -36,15 +39,15 @@
 
 ## Note
 
 **prr** is in very early stages of development, so things might still change unexpectedly or explode embarrasingly.
 
 ## Features
 
-- Command-line execution of prompts
+- Command-line execution of prompts (now with web UI!)
 - Quick iteration on prompt design and paramter refinement with `watch` command
 - YAML configuration ties prompts to models and their configurations
 - Write prompt-scripts with #!/usr/bin/prr shebang and execute them directly
 - All prompts can optionally use templating language ([Jinja](https://jinja.palletsprojects.com/en/3.1.x/)) for flow control, partials and others
 - Execute multiple models, or configurations against the same prompt
 - Expandable to other LLM providers (current integrations are <100 lines of code each)
 - Each prompt run across models gives you stats on model response times and token counts used to work across performance, quality and cost factors
@@ -123,17 +126,29 @@
 ```bash
 # https://platform.openai.com/account/api-keys
 OPENAI_API_KEY="sk-..."
 
 # https://console.anthropic.com/account/keys
 ANTHROPIC_API_KEY="sk-ant-..."
 
+ELEVEN_LABS_API_KEY="9db0...."
+
 DEFAULT_SERVICE="openai/chat/gpt-3.5-turbo"
 ```
 
+### Running web user interface
+
+Simply run prr with 'ui' command and your prompt path (if it doesn't exist, it will be created), like so:
+
+```sh
+$ prr ui ~/Desktop/my-prompt
+```
+
+Web browser will be launched with the UI connected to your command that you will use to launch the runs.
+
 #### For Google PaLM, you need to install the following dependencies:
 You need to install [Google Cloud SDK](https://cloud.google.com/sdk/docs/install) and you need to have access to a Vertex AI with Generative AI enabled.
 `prr` assumes you're logged in into your Google Cloud account and have access to the project you want to use.
 
 ```sh
 gcloud auth login
 ```
@@ -143,14 +158,16 @@
 ```
 
 ```sh
 gcloud auth application-default login
 ```
 
 
+
+
 ### Code completion
 Using Starcoder model you can get code completion for a variety of languages. Here's a quick example of how to use it (check out the content of `examples/code/completion.yaml`):
 
 ```sh
 $ prr run ./examples/code/completion.yaml
 ```
 
@@ -448,14 +465,15 @@
 
 ### Current integrations
 
 * OpenAI/chat - https://platform.openai.com/docs/guides/chat
 * Anthropic/complete - https://console.anthropic.com/docs/api
 * Google Vertex AI PaLM - https://cloud.google.com/vertex-ai/docs/generative-ai/learn/overview
 * Starcoder - https://huggingface.co/bigcode/starcoder
+* Eleven Labs - https://beta.elevenlabs.io
 
 ## Development
 
 1. Clone the repo
 
 ```sh
 $ git clone https://github.com/Forward-Operators/prr.git
```

