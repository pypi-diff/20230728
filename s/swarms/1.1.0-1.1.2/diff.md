# Comparing `tmp/swarms-1.1.0.tar.gz` & `tmp/swarms-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-1.1.0.tar", last modified: Fri Jul 28 00:49:20 2023, max compression
+gzip compressed data, was "swarms-1.1.2.tar", last modified: Fri Jul 28 17:16:26 2023, max compression
```

## Comparing `swarms-1.1.0.tar` & `swarms-1.1.2.tar`

### file list

```diff
@@ -1,157 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 00:49:10.000000 swarms-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 00:49:20.778294 swarms-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-28 00:49:10.000000 swarms-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.762294 swarms-1.1.0/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-28 00:49:10.000000 swarms-1.1.0/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:49:20.778294 swarms-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-28 00:49:10.000000 swarms-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.762294 swarms-1.1.0/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/ocean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/petals_hf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/prompts/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/chains/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/tools/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/tools/core/code_interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/core/code_interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27430 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/core/code_interpreter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    73260 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/Calback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/ChatOpenAI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/ConversationalChatAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/agent_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/agent_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/boss/boss_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/orchestrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/embeddings/pegasus.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/character_generative.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/generative_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/worker_agent_ultra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/worker_ultra_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.485408 swarms-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 17:16:14.000000 swarms-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 17:16:26.485408 swarms-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-28 17:16:14.000000 swarms-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-28 17:16:14.000000 swarms-1.1.2/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:16:26.485408 swarms-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-28 17:16:14.000000 swarms-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/petals_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/agent_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/prompts/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/chains/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/tools/core/code_interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/core/code_interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/core/code_interpreter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73260 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/agent_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/boss/boss_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/orchestrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/embeddings/pegasus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/character_generative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/omni_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/worker_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/worker_ultra_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/top_level.txt
```

### Comparing `swarms-1.1.0/LICENSE` & `swarms-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/PKG-INFO` & `swarms-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.0
+Version: 1.1.2
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.0/README.md` & `swarms-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Swarming AI Agents (Swarms)
+## Swarms of Autonomous AI Agents 
 
 ![Swarming banner](images/swarms.png)
 
 Introducing Swarms, automating all digital activities with multi-agent collaboration, get started in 30 seconds in a seamless onboarding experience.
 
 ---
```

### Comparing `swarms-1.1.0/api/app.py` & `swarms-1.1.2/api/app.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/setup.py` & `swarms-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 ##
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '1.1.0',
+  version = '1.1.2',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-1.1.0/swarms/agents/agent.py` & `swarms-1.1.2/swarms/agents/agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/memory/base.py` & `swarms-1.1.2/swarms/agents/memory/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,38 +3,36 @@
 from __future__ import annotations
 
 import asyncio
 import math
 import warnings
 from abc import ABC, abstractmethod
 from functools import partial
-
 from typing import (
     Any,
     Callable,
     ClassVar,
     Collection,
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
 )
 
-from pydantic import Field, root_validator
-
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForRetrieverRun,
     CallbackManagerForRetrieverRun,
 )
 from langchain.docstore.document import Document
 from langchain.embeddings.base import Embeddings
 from langchain.schema import BaseRetriever
+from pydantic import Field, root_validator
 
 VST = TypeVar("VST", bound="VectorStore")
 
 
 class VectorStore(ABC):
     """Interface for vector stores."""
```

### Comparing `swarms-1.1.0/swarms/agents/memory/chroma.py` & `swarms-1.1.2/swarms/agents/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/memory/ocean.py` & `swarms-1.1.2/swarms/agents/memory/ocean.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/models/hf.py` & `swarms-1.1.2/swarms/agents/models/hf.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/models/llm.py` & `swarms-1.1.2/swarms/agents/models/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/prompts/chains/llm.py` & `swarms-1.1.2/swarms/agents/prompts/chains/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Chain that just formats a prompt and calls an LLM."""
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
-from pydantic import Extra, Field
-
+from langchain.base_language import BaseLanguageModel
 from langchain.callbacks.manager import (
     AsyncCallbackManager,
     AsyncCallbackManagerForChainRun,
     CallbackManager,
     CallbackManagerForChainRun,
     Callbacks,
 )
@@ -20,15 +19,15 @@
 from langchain.schema import (
     BaseLLMOutputParser,
     BasePromptTemplate,
     LLMResult,
     NoOpOutputParser,
     PromptValue,
 )
-from langchain.schema.language_model import BaseLanguageModel
+from pydantic import Extra, Field
 
 
 class LLMChain(Chain):
     """Chain to run queries against LLMs.
 
     Example:
         .. code-block:: python
```

### Comparing `swarms-1.1.0/swarms/agents/prompts/prompts.py` & `swarms-1.1.2/swarms/agents/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/tools/base.py` & `swarms-1.1.2/swarms/agents/tools/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/tools/core/code_interpreter/main.py` & `swarms-1.1.2/swarms/agents/tools/core/code_interpreter/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import json
 import re
 import uuid
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
-from pydantic import BaseModel, BaseSettings, root_validator
-
 from langchain.agents import AgentExecutor, BaseSingleActionAgent
 from langchain.base_language import BaseLanguageModel
 from langchain.callbacks import AsyncIteratorCallbackHandler
 from langchain.callbacks.base import BaseCallbackManager
 from langchain.callbacks.manager import Callbacks
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
@@ -32,16 +30,15 @@
     FunctionMessage,
     HumanMessage,
     OutputParserException,
     SystemMessage,
 )
 from langchain.tools import BaseTool, StructuredTool
 from langchain.tools.convert_to_openai import format_tool_to_openai_function
-
-
+from pydantic import BaseModel, BaseSettings, root_validator
 
 remove_dl_link_prompt = ChatPromptTemplate(
     input_variables=["input_response"],
     messages=[
         SystemMessage(
             content="The user will send you a response and you need to remove the download link from it.\n"
             "Reformat the remaining message so no whitespace or half sentences are still there.\n"
@@ -291,15 +288,15 @@
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return f"File(name={self.name})"
 
 
-from langchain.schema import HumanMessage, AIMessage  # type: ignore
+from langchain.schema import AIMessage, HumanMessage  # type: ignore
 
 
 class UserRequest(HumanMessage):
     files: list[File] = []
 
     def __str__(self):
         return self.content
```

### Comparing `swarms-1.1.0/swarms/agents/tools/main.py` & `swarms-1.1.2/swarms/agents/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/utils/Agent.py` & `swarms-1.1.2/swarms/agents/utils/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import json
 import logging
 from abc import abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import yaml
-from pydantic import BaseModel, root_validator
-
 from langchain.agents.agent_types import AgentType
+from langchain.base_language import BaseLanguageModel
 from langchain.callbacks.base import BaseCallbackManager
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForToolRun,
     CallbackManagerForToolRun,
     Callbacks,
 )
 from langchain.chains.llm import LLMChain
@@ -22,17 +21,17 @@
 from langchain.prompts.prompt import PromptTemplate
 from langchain.schema import (
     AgentAction,
     AgentFinish,
     BaseOutputParser,
     BasePromptTemplate,
 )
-from langchain.schema.language_model import BaseLanguageModel
 from langchain.schema.messages import BaseMessage
 from langchain.tools.base import BaseTool
+from pydantic import BaseModel, root_validator
 
 logger = logging.getLogger(__name__)
 
 
 class BaseSingleActionAgent(BaseModel):
     """Base Agent class."""
```

### Comparing `swarms-1.1.0/swarms/agents/utils/Calback.py` & `swarms-1.1.2/swarms/agents/utils/Calback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Any, Dict, List, Optional, Union
 
+from celery import Task
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.schema import AgentAction, AgentFinish, LLMResult
-from celery import Task
+
+from swarms.utils.logger import logger
 
 # from ansi import ANSI, Color, Style, dim_multiline
 from swarms.utils.main import ANSI, Color, Style, dim_multiline
-from swarms.utils.logger import logger
 
 
 class EVALCallbackHandler(BaseCallbackHandler):
     @property
     def ignore_llm(self) -> bool:
         return False
```

### Comparing `swarms-1.1.0/swarms/agents/utils/ChatOpenAI.py` & `swarms-1.1.2/swarms/agents/utils/ChatOpenAI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 """OpenAI chat wrapper."""
 from __future__ import annotations
 
-import os
 import logging
+import os
 import sys
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple
 
 import openai
-
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import (
     AIMessage,
     BaseMessage,
     ChatGeneration,
     ChatMessage,
     ChatResult,
     HumanMessage,
     SystemMessage,
 )
-
 from langchain.utils import get_from_dict_or_env
-from swarms.utils.logger import logger
 from pydantic import BaseModel, Extra, Field, root_validator
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
+from swarms.utils.logger import logger
 
 # from ansi import ANSI, Color, Style
 from swarms.utils.main import ANSI, Color, Style
-import os
+
 
 def _create_retry_decorator(llm: ChatOpenAI) -> Callable[[Any], Any]:
     import openai
 
     min_seconds = 4
     max_seconds = 10
     # Wait 2^x * 1 second between each retry starting with
```

### Comparing `swarms-1.1.0/swarms/agents/utils/ConversationalChatAgent.py` & `swarms-1.1.2/swarms/agents/utils/ConversationalChatAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-from typing import Any, List, Optional, Sequence, Tuple
 import logging
+from typing import Any, List, Optional, Sequence, Tuple
 
-from swarms.agents.utils.Agent import Agent
+from langchain.agents.agent import AgentOutputParser
+from langchain.base_language import BaseLanguageModel
 from langchain.callbacks.base import BaseCallbackManager
 from langchain.chains import LLMChain
-from langchain.schema import BaseOutputParser
 from langchain.prompts.base import BasePromptTemplate
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     MessagesPlaceholder,
     SystemMessagePromptTemplate,
 )
 from langchain.schema import (
     AgentAction,
     AIMessage,
-    BaseLanguageModel,
     BaseMessage,
+    BaseOutputParser,
     HumanMessage,
 )
 from langchain.tools.base import BaseTool
 
-
-from langchain.agents.agent import AgentOutputParser
-from langchain.schema import AgentAction
-
-
 from swarms.agents.prompts.prompts import EVAL_TOOL_RESPONSE
-
-
+from swarms.agents.utils.Agent import Agent
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 class ConversationalChatAgent(Agent):
     """An agent designed to hold a conversation in addition to using tools."""
 
     output_parser: BaseOutputParser
```

### Comparing `swarms-1.1.0/swarms/agents/utils/agent_creator.py` & `swarms-1.1.2/swarms/agents/utils/agent_creator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/agents/utils/agent_setup.py` & `swarms-1.1.2/swarms/agents/utils/agent_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import os
 
-from swarms.agents.prompts.prompts import EVAL_PREFIX, EVAL_SUFFIX
-from swarms.agents.tools.main import BaseToolSet
-from swarms.agents.tools.main import ToolsFactory
-
+from langchain.callbacks.base import BaseCallbackManager
 
+# from .ChatOpenAI import ChatOpenAI
+from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import BaseOutputParser
-from langchain.callbacks.base import BaseCallbackManager
+
+from swarms.agents.prompts.prompts import EVAL_PREFIX, EVAL_SUFFIX
+from swarms.agents.tools.main import BaseToolSet, ToolsFactory
 
 from .ConversationalChatAgent import ConversationalChatAgent
-# from .ChatOpenAI import ChatOpenAI
-from langchain.chat_models import ChatOpenAI
 from .output_parser import EvalOutputParser
 
 
-
 class AgentSetup:
     def __init__(self, toolsets: list[BaseToolSet] = [], openai_api_key: str = None, serpapi_api_key: str = None, bing_search_url: str = None, bing_subscription_key: str = None):
         self.llm: BaseChatModel = None
         self.parser: BaseOutputParser = None
         self.global_tools: list = None
         self.toolsets = toolsets
         self.openai_api_key = openai_api_key or os.getenv("OPENAI_API_KEY")
```

### Comparing `swarms-1.1.0/swarms/agents/utils/prompts.py` & `swarms-1.1.2/swarms/agents/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/boss/boss_node.py` & `swarms-1.1.2/swarms/boss/boss_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/hivemind.py` & `swarms-1.1.2/swarms/hivemind.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/orchestrate.py` & `swarms-1.1.2/swarms/orchestrate.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/swarms.py` & `swarms-1.1.2/swarms/swarms.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from langchain.docstore import InMemoryDocstore
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.tools import DuckDuckGoSearchRun
 from langchain.tools.file_management.read import ReadFileTool
 from langchain.tools.file_management.write import WriteFileTool
 from langchain.vectorstores import FAISS
 
-from swarms.agents.models.hf import HuggingFaceLLM
 
 # from langchain.tools.human.tool import HumanInputRun
 from swarms.agents.tools.main import WebpageQATool, process_csv
 from swarms.boss.boss_node import BossNodeInitializer as BossNode
 from swarms.workers.worker_node import WorkerNodeInitializer
 
 # from langchain import LLMMathChain
@@ -34,37 +33,33 @@
 
 # ---------- Constants ----------
 ROOT_DIR = "./data/"
 
 class HierarchicalSwarm:
     def __init__(
         self, 
-        model_id: Optional[str] = None, 
         openai_api_key: Optional[str] = "", 
 
         use_vectorstore: Optional[bool] = True, 
         embedding_size: Optional[int] = None, 
         use_async: Optional[bool] = True, 
 
         human_in_the_loop: Optional[bool] = True, 
-        model_type: Optional[str] = None, 
         boss_prompt: Optional[str] = None,
 
         worker_prompt: Optional[str] = None,
         temperature: Optional[float] = None,
         max_iterations: Optional[int] = None,
         logging_enabled: Optional[bool] = True):
-        
-        self.model_id = model_id        
+            
         self.openai_api_key = openai_api_key
         self.use_vectorstore = use_vectorstore
 
         self.use_async = use_async
         self.human_in_the_loop = human_in_the_loop
-        self.model_type = model_type
 
         self.embedding_size = embedding_size
         self.boss_prompt = boss_prompt
         self.worker_prompt = worker_prompt
 
         self.temperature = temperature
         self.max_iterations = max_iterations
@@ -82,18 +77,15 @@
 
         Params:
             llm_class(class): The Language model class. Default is OpenAI.
             temperature (float): The Temperature for the language model. Default is 0.5
         """
         try: 
             # Initialize language model
-            if self.llm_class == 'openai':
-                return OpenAI(openai_api_key=self.openai_api_key, temperature=self.temperature)
-            elif self.model_type == "huggingface":
-                return HuggingFaceLLM(model_id=self.model_id, temperature=self.temperature)
+            return OpenAI(openai_api_key=self.openai_api_key, temperature=self.temperature)
         except Exception as e:
             logging.error(f"Failed to initialize language model: {e}")
 
     def initialize_tools(self, llm_class, extra_tools=None):
         """
         Init tools
         
@@ -193,15 +185,16 @@
             prefix = """You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n """
             
             prompt = ZeroShotAgent.create_prompt(tools, prefix=prefix, suffix=suffix, input_variables=["objective", "task", "context", "agent_scratchpad"],)
             llm_chain = LLMChain(llm=llm, prompt=prompt)
             agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=[tool.name for tool in tools])
 
             agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=tools, verbose=verbose)
-            return BossNode(llm, vectorstore, agent_executor, max_iterations=self.max_iterations)
+            return BossNode(llm, vectorstore, 
+            agent_executor, max_iterations=self.max_iterations)
         except Exception as e:
             logging.error(f"Failed to initialize boss node: {e}")
             raise
 
 
 
 
@@ -235,16 +228,14 @@
             logging.error(f"An error occurred in run: {e}")
             return None
         
 # usage-# usage-
 def swarm(
     api_key: Optional[str]="", 
     objective: Optional[str]="", 
-    model_type: Optional[str]="", 
-    model_id: Optional[str]=""
     ):
     """
     Run the swarm with the given API key and objective.
 
     Parameters:
     api_key (str): The OpenAI API key. Default is an empty string.
     objective (str): The objective. Default is an empty string.
@@ -256,15 +247,15 @@
     if not api_key or not isinstance(api_key, str):
         logging.error("Invalid OpenAI key")
         raise ValueError("A valid OpenAI API key is required")
     if not objective or not isinstance(objective, str):
         logging.error("Invalid objective")
         raise ValueError("A valid objective is required")
     try:
-        swarms = HierarchicalSwarm(api_key, model_id=model_type, use_async=False, model_type=model_type) #logging_enabled=logging_enabled) # Turn off async
+        swarms = HierarchicalSwarm(api_key, use_async=False) #logging_enabled=logging_enabled) # Turn off async
         result = swarms.run(objective)
         if result is None:
             logging.error("Failed to run swarms")
         else:
             logging.info(f"Successfully ran swarms with results: {result}")
         return result
     except Exception as e:
```

### Comparing `swarms-1.1.0/swarms/utils/embeddings/base.py` & `swarms-1.1.2/swarms/utils/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/utils/embeddings/pegasus.py` & `swarms-1.1.2/swarms/utils/embeddings/pegasus.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/utils/main.py` & `swarms-1.1.2/swarms/utils/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/utils/static.py` & `swarms-1.1.2/swarms/utils/static.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/character_generative.py` & `swarms-1.1.2/swarms/workers/character_generative.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/generative_worker.py` & `swarms-1.1.2/swarms/workers/generative_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import logging
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
+from langchain import LLMChain
+from langchain.base_language import BaseLanguageModel
+
 ############
 from langchain.prompts import PromptTemplate
 from langchain.retrievers import TimeWeightedVectorStoreRetriever
 from langchain.schema import BaseMemory, Document
-
-from langchain.schema.language_model import BaseLanguageModel
 from langchain.utils import mock_now
-from langchain import LLMChain
-from langchain.schema.language_model import BaseLanguageModel
-
 
 logger = logging.getLogger(__name__)
 
 
 #######################
```

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/GroundingDINO/setup.py` & `swarms-1.1.2/swarms/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/models/segment_anything/setup.py` & `swarms-1.1.2/swarms/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/multi_modal_worker.py` & `swarms-1.1.2/swarms/workers/multi_modal_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-1.1.2/swarms/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/omni_worker.py` & `swarms-1.1.2/swarms/workers/omni_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/worker_agent_ultra.py` & `swarms-1.1.2/swarms/workers/worker_agent_ultra.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/worker_node.py` & `swarms-1.1.2/swarms/workers/worker_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms/workers/worker_ultra_node.py` & `swarms-1.1.2/swarms/workers/worker_ultra_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.0/swarms.egg-info/PKG-INFO` & `swarms-1.1.2/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.0
+Version: 1.1.2
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.0/swarms.egg-info/SOURCES.txt` & `swarms-1.1.2/swarms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 swarms.egg-info/PKG-INFO
 swarms.egg-info/SOURCES.txt
 swarms.egg-info/dependency_links.txt
 swarms.egg-info/requires.txt
 swarms.egg-info/top_level.txt
 swarms/agents/__init__.py
 swarms/agents/agent.py
+swarms/agents/base.py
+swarms/agents/memory.py
 swarms/agents/memory/__init__.py
 swarms/agents/memory/base.py
 swarms/agents/memory/chroma.py
 swarms/agents/memory/ocean.py
 swarms/agents/models/__init__.py
 swarms/agents/models/hf.py
 swarms/agents/models/llm.py
 swarms/agents/models/petals_hf.py
 swarms/agents/prompts/__init__.py
+swarms/agents/prompts/agent_prompt.py
 swarms/agents/prompts/prompts.py
 swarms/agents/prompts/chains/__init__.py
 swarms/agents/prompts/chains/llm.py
 swarms/agents/tools/__init__.py
 swarms/agents/tools/base.py
 swarms/agents/tools/main.py
 swarms/agents/tools/core/__init__.py
```

### Comparing `swarms-1.1.0/swarms.egg-info/requires.txt` & `swarms-1.1.2/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

