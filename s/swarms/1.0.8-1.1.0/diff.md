# Comparing `tmp/swarms-1.0.8.tar.gz` & `tmp/swarms-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-1.0.8.tar", last modified: Sat Jul 22 19:42:49 2023, max compression
+gzip compressed data, was "swarms-1.1.0.tar", last modified: Fri Jul 28 00:49:20 2023, max compression
```

## Comparing `swarms-1.0.8.tar` & `swarms-1.1.0.tar`

### file list

```diff
@@ -1,152 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.445870 swarms-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 19:42:37.000000 swarms-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 19:42:49.445870 swarms-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-22 19:42:37.000000 swarms-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-22 19:42:37.000000 swarms-1.0.8/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 19:42:49.445870 swarms-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-22 19:42:37.000000 swarms-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/swarms/agents/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/memory/chroma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/swarms/agents/models/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/models/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/swarms/agents/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/swarms/agents/prompts/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/prompts/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/prompts/chains/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/agents/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/tools/agent_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/agents/tools/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/tools/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/agents/tools/core/code_interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/tools/core/code_interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/tools/core/code_interpreter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    73698 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/Calback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/ChatOpenAI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/ConversationalChatAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/agent_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/agent_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/agents/utils/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/boss/boss_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/utils/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/WorkerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/character_generative.py
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/generative_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.437870 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.441870 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.441870 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.441870 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.441870 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.441870 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.441870 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.441870 swarms-1.0.8/swarms/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-22 19:42:37.000000 swarms-1.0.8/swarms/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.445870 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.445870 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.445870 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/models/segment_anything/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/multi_modal_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.445870 swarms-1.0.8/swarms/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79542 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.445870 swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45875 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/worker_agent_ultra.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-22 19:42:38.000000 swarms-1.0.8/swarms/workers/worker_ultra_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:42:49.433869 swarms-1.0.8/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 19:42:49.000000 swarms-1.0.8/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-22 19:42:49.000000 swarms-1.0.8/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:42:49.000000 swarms-1.0.8/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-22 19:42:49.000000 swarms-1.0.8/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 19:42:49.000000 swarms-1.0.8/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 00:49:10.000000 swarms-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 00:49:20.778294 swarms-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-28 00:49:10.000000 swarms-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.762294 swarms-1.1.0/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-28 00:49:10.000000 swarms-1.1.0/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:49:20.778294 swarms-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-28 00:49:10.000000 swarms-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.762294 swarms-1.1.0/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/memory/ocean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/models/petals_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/prompts/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/chains/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms/agents/tools/core/code_interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/core/code_interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27430 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/core/code_interpreter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73260 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/agent_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/boss/boss_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/orchestrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/embeddings/pegasus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/character_generative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:10.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.770294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.774294 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/models/segment_anything/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.778294 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/omni_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/worker_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-28 00:49:11.000000 swarms-1.1.0/swarms/workers/worker_ultra_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:49:20.766294 swarms-1.1.0/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 00:49:20.000000 swarms-1.1.0/swarms.egg-info/top_level.txt
```

### Comparing `swarms-1.0.8/LICENSE` & `swarms-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/PKG-INFO` & `swarms-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.0.8
+Version: 1.1.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.0.8/README.md` & `swarms-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-# Agora 🏛️
-
-![Agora banner](images/Agora-Banner-blend.png)
-
-[Swarms](https://discord.gg/qUtxnK2NMf) is brought to you by Agora, the open source AI research organization. Join Agora and help create swarms and receive support to advance Humanity.
-
-![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)
-
----
-
 ## Swarming AI Agents (Swarms)
 
 ![Swarming banner](images/swarms.png)
 
-Welcome to Swarms - the future of AI, where we leverage the power of autonomous agents to create 'swarms' of Language Models (LLM) that work together, creating a dynamic and interactive AI system.
-
+Introducing Swarms, automating all digital activities with multi-agent collaboration, get started in 30 seconds in a seamless onboarding experience.
 
 ---
 
 ![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)
 
 
 [![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)
@@ -83,20 +72,17 @@
 
 * Create new python file and unleash superintelligence
 
 ```python
 
 from swarms import swarm
 
-api_key = "api key for openai"
-
 objective = "What is the capital of the Uk"
 
-result = swarm(api_key, objective)
-print(result)
+swarm(objective)
 ```
 
 ---
 
 # Method 2
 Download via Github, and install requirements. Simple example by:
 
@@ -107,33 +93,33 @@
 * `python3 -m pip install -r requirements.txt`
 
 * `python3 example.py`
 
 * or create a new file:
 
 ```python
-from swarms.swarms import Swarms
+from swarms.swarms import HierarchicalSwarm
 
 # Retrieve your API key from the environment or replace with your actual key
 api_key = "sksdsds"
 
 # Initialize Swarms with your API key
-swarm = Swarms(openai_api_key=api_key)
+swarm = HierarchicalSwarm(openai_api_key=api_key)
 
 # Define an objective
 objective = """
 Please develop and serve a simple community web service. 
 People can signup, login, post, comment. 
 Post and comment should be visible at once. 
 I want it to have neumorphism-style. 
 The ports you can use are 4500 and 6500.
 """
 
 # Run Swarms
-swarm.run_swarms(objective)
+swarm.run(objective)
 ```
 
 * Or just the worker no `BossNode`:
 
 ```python
 from swarms import worker_node
 
@@ -155,15 +141,15 @@
 # Various agents
 
 Here are some agents in the swarm you can use!
 
 | Agent        | Import Statement                                   | Example Usage                                           |
 |--------------|----------------------------------------------------|---------------------------------------------------------|
 | WorkerNode   | `from swarms import worker_node`                   | ```python api_key = "sksdsds" node = worker_node(api_key) objective = "Please make a web GUI for using HTTP API server..." task = node.run(objective) print(task)``` |
-| Swarms       | `from swarms.swarms import Swarms`                 | ```python import os from swarms.swarms import Swarms api_key = os.getenv("OPENAI_API_KEY") swarm = Swarms(openai_api_key=api_key) objective = "Please make a web GUI for using HTTP API server..." task = swarm.run_swarms(objective) print(task)``` |
+| Swarms       | `from swarms.swarms import Swarms`                 | ```python import os from swarms.swarms import Swarms api_key = os.getenv("OPENAI_API_KEY") swarm = Swarms(openai_api_key=api_key) objective = "Please make a web GUI for using HTTP API server..." task = swarm.run(objective) print(task)``` |
 
 
 ---
 
 
 # Docker Setup
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swarms-1.0.8/api/app.py` & `swarms-1.1.0/api/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,47 @@
+import logging
+import os
 from fastapi import FastAPI, HTTPException, Depends
 from fastapi_cache.decorator import cache
 from fastapi_cache.coder import JsonCoder
+
 from fastapi_cache import FastAPICache
+from fastapi_cache.backends.redis import RedisBackend
 from aioredis import Redis
+
 from pydantic import BaseModel
 from swarms.swarms import swarm
 from fastapi_limiter import FastAPILimiter
+
 from fastapi_limiter.depends import RateLimiter
+from dotenv import load_dotenv
+
+load_dotenv()
 
 class SwarmInput(BaseModel):
     api_key: str
     objective: str
 
 app = FastAPI()
 
 @app.on_event("startup")
 async def startup():
-    redis = Redis(host="localhost", port=6379)
+    redis_host = os.getenv("REDIS_HOST", "localhost")
+    redis_port = int(os.getenv("REDIS_PORT", 6379))
+    redis = await Redis.create(redis_host, redis_port)
     FastAPICache.init(RedisBackend(redis), prefix="fastapi-cache", coder=JsonCoder())
-    await FastAPILimiter.init("redis://localhost:6379")
+    await FastAPILimiter.init(f"redis://{redis_host}:{redis_port}")
 
 @app.post("/chat", dependencies=[Depends(RateLimiter(times=2, minutes=1))])
 @cache(expire=60)  # Cache results for 1 minute
-async def run_swarms(swarm_input: SwarmInput):
+async def run(swarm_input: SwarmInput):
     try:
         results = swarm(swarm_input.api_key, swarm_input.objective)
         if not results:
             raise HTTPException(status_code=500, detail="Failed to run swarms")
         return {"results": results}
     except ValueError as ve:
+        logging.error("A ValueError occurred", exc_info=True)
         raise HTTPException(status_code=400, detail=str(ve))
-    except Exception as e:
-        raise HTTPException(status_code=500, detail=str(e))
+    except Exception:
+        logging.error("An error occurred", exc_info=True)
+        raise HTTPException(status_code=500, detail="An unexpected error occurred")
```

### Comparing `swarms-1.0.8/setup.py` & `swarms-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 ##
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '1.0.8',
+  version = '1.1.0',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -23,19 +23,22 @@
         'langchain',
         'torch',
         'torchvision',
         'torchaudio',
         'asyncio',
         'nest_asyncio',
         'bs4',
+        'pegasusx',
+        'oceandb',
         'playwright',
         'duckduckgo_search',
         'faiss-cpu',
         'wget==3.2',
         'accelerate',
+        'sphinx_rtd_theme',
         'addict',
         'albumentations',
         'basicsr',
         'controlnet-aux',
         'diffusers',
         'einops',
         'gradio',
@@ -71,21 +74,21 @@
         'pydantic==1.10.6',
         'tenacity==8.2.2',
         'python-dotenv',
         'boto3',
         'uvicorn==0.21.1',
         'jinja2==3.1.2',
         'python-multipart==0.0.6',
-        'celery==5.2.7',
-        'redis==4.5.4',
+        'celery==5.3.1',
+        'redis==4.6.0',
         'sentencepiece',
-        'bitsandbytes==0.37.2',
+        'bitsandbytes==0.41.0',
         'psycopg2-binary==2.9.5',
         'google-search-results==2.4.2',
-        'black==23.1.0',
+        'black==23.7.0',
         'Pillow',
         'selenium',
         'diffusers',
         'controlnet_aux',
         'tiktoken',
         'espnet==202301',
         'espnet_model_zoo==0.1.7',
```

### Comparing `swarms-1.0.8/swarms/agents/memory/base.py` & `swarms-1.1.0/swarms/agents/memory/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/memory/chroma.py` & `swarms-1.1.0/swarms/agents/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/models/llm.py` & `swarms-1.1.0/swarms/agents/models/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/prompts/chains/llm.py` & `swarms-1.1.0/swarms/agents/prompts/chains/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/prompts/prompts.py` & `swarms-1.1.0/swarms/agents/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/tools/base.py` & `swarms-1.1.0/swarms/agents/tools/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, Awaitable, Callable, Dict, List, Optional, Type, Union
+from typing import Any, Callable, Optional, Type, Union
 from pydantic import BaseModel
 
 class ToolException(Exception):
     pass
 
 class BaseTool(ABC):
     name: str
```

### Comparing `swarms-1.0.8/swarms/agents/tools/core/code_interpreter/main.py` & `swarms-1.1.0/swarms/agents/tools/core/code_interpreter/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import asyncio
 import base64
 import json
 import re
 import uuid
 from dataclasses import dataclass
-from dotenv import load_dotenv
 from io import BytesIO
-from typing import Any, List, Optional, Sequence, Tuple, Union, TYPE_CHECKING
+from typing import Any, List, Optional, Sequence, Tuple, Union
 
 from pydantic import BaseModel, BaseSettings, root_validator
 
 from langchain.agents import AgentExecutor, BaseSingleActionAgent
 from langchain.base_language import BaseLanguageModel
 from langchain.callbacks import AsyncIteratorCallbackHandler
 from langchain.callbacks.base import BaseCallbackManager
@@ -723,17 +722,17 @@
         request.content += "**File(s) are now available in the cwd. **\n"
 
     async def output_handler(self, final_response: str) -> CodeInterpreterResponse:
         """Embed images in the response"""
         for file in self.output_files:
             if str(file.name) in final_response:
                 # rm ![Any](file.name) from the response
-                final_response = re.sub(rf"\n\n!\[.*\]\(.*\)", "", final_response)
+                final_response = re.sub(r"\n\n!\[.*\]\(.*\)", "", final_response)
 
-        if self.output_files and re.search(rf"\n\[.*\]\(.*\)", final_response):
+        if self.output_files and re.search(r"\n\[.*\]\(.*\)", final_response):
             final_response = await remove_download_link(final_response, self.llm)
 
         return CodeInterpreterResponse(content=final_response, files=self.output_files)
 
     async def generate_response(
         self,
         user_msg: str,
```

### Comparing `swarms-1.0.8/swarms/agents/tools/main.py` & `swarms-1.1.0/swarms/agents/tools/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from langchain.agents.tools import BaseTool, Tool
 from typing import Optional
 
 from langchain.agents import load_tools
 from langchain.agents.tools import BaseTool
 from langchain.llms.base import BaseLLM
 
-from langchain.chat_models import ChatOpenAI
 
 
 import requests
 from bs4 import BeautifulSoup
 
 from swarms.utils.logger import logger
 class ToolScope(Enum):
@@ -54,17 +53,16 @@
 
     def to_tool(
         self,
         get_session: SessionGetter = lambda: [],
     ) -> BaseTool:
         func = self.func
         if self.is_per_session():
-            func = lambda *args, **kwargs: self.func(
-                *args, **kwargs, get_session=get_session
-            )
+            def func(*args, **kwargs):
+                return self.func(*args, **kwargs, get_session=get_session)
 
         return Tool(
             name=self.name,
             description=self.description,
             func=func,
         )
 
@@ -166,15 +164,15 @@
         scope=ToolScope.SESSION,
     )
     def exit(self, message: str, get_session: SessionGetter) -> str:
         """Run the tool."""
         _, executor = get_session()
         del executor
 
-        logger.debug(f"\nProcessed ExitConversation.")
+        logger.debug("\nProcessed ExitConversation.")
 
         return message
     
 
 
 
 
@@ -418,16 +416,14 @@
 
 #         return (exitcode, output)
 
 ################## => stdout end
 
 import os
 import subprocess
-import time
-from datetime import datetime
 from typing import Dict, List
 
 from swarms.utils.main import ANSI, Color, Style # test
 
 class Terminal(BaseToolSet):
     def __init__(self):
         self.sessions: Dict[str, List[SyscallTracer]] = {}
@@ -936,15 +932,15 @@
 ###################### EDITOR// INIT.PY
 
 
 class CodeEditor(BaseToolSet):
     @tool(
         name="CodeEditor.READ",
         description="Read and understand code. "
-        f"Input should be filename and line number group. ex. test.py|1-10 "
+        "Input should be filename and line number group. ex. test.py|1-10 "
         "and the output will be code. ",
     )
     def read(self, inputs: str) -> str:
         try:
             output = CodeReader.read(inputs)
         except Exception as e:
             output = str(e)
@@ -1466,30 +1462,27 @@
 # General 
 import os
 import pandas as pd
 
 from langchain.agents.agent_toolkits.pandas.base import create_pandas_dataframe_agent
 from langchain.docstore.document import Document
 import asyncio
-import nest_asyncio
 
 # Tools
 from contextlib import contextmanager
 from typing import Optional
 from langchain.agents import tool
-from langchain.tools.file_management.read import ReadFileTool
-from langchain.tools.file_management.write import WriteFileTool
 
 ROOT_DIR = "./data/"
 
 from langchain.tools import BaseTool, DuckDuckGoSearchRun
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
 from pydantic import Field
-from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain, BaseCombineDocumentsChain
+from langchain.chains.qa_with_sources.loading import BaseCombineDocumentsChain
 
 
 
 @contextmanager
 def pushd(new_dir):
     """Context manager for changing the current working directory."""
     prev_dir = os.getcwd()
@@ -1783,22 +1776,14 @@
 
 
 
 
 
 ######################## ######################################################## file system
 
-from langchain.tools.file_management import (
-    ReadFileTool,
-    CopyFileTool,
-    DeleteFileTool,
-    MoveFileTool,
-    WriteFileTool,
-    ListDirectoryTool,
-)
 from langchain.agents.agent_toolkits import FileManagementToolkit
 from tempfile import TemporaryDirectory
 
 # We'll make a temporary directory to avoid clutter
 working_directory = TemporaryDirectory()
 
 toolkit = FileManagementToolkit(
```

### Comparing `swarms-1.0.8/swarms/agents/utils/Agent.py` & `swarms-1.1.0/swarms/agents/utils/Agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 """Chain that takes in an input and produces an action and action input."""
 from __future__ import annotations
 
-import asyncio
 import json
 import logging
-import time
 from abc import abstractmethod
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import yaml
 from pydantic import BaseModel, root_validator
 
 from langchain.agents.agent_types import AgentType
-from langchain.agents.tools import InvalidTool
 from langchain.callbacks.base import BaseCallbackManager
 from langchain.callbacks.manager import (
-    AsyncCallbackManagerForChainRun,
     AsyncCallbackManagerForToolRun,
-    CallbackManagerForChainRun,
     CallbackManagerForToolRun,
     Callbacks,
 )
-from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.input import get_color_mapping
 from langchain.prompts.few_shot import FewShotPromptTemplate
 from langchain.prompts.prompt import PromptTemplate
 from langchain.schema import (
     AgentAction,
     AgentFinish,
     BaseOutputParser,
     BasePromptTemplate,
-    OutputParserException,
 )
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.schema.messages import BaseMessage
 from langchain.tools.base import BaseTool
-from langchain.utilities.asyncio import asyncio_timeout
 
 logger = logging.getLogger(__name__)
 
 
 class BaseSingleActionAgent(BaseModel):
     """Base Agent class."""
```

### Comparing `swarms-1.0.8/swarms/agents/utils/Calback.py` & `swarms-1.1.0/swarms/agents/utils/Calback.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,25 @@
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> None:
         pass
 
     def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> None:
-        logger.info(ANSI(f"Entering new chain.").to(Color.green(), Style.italic()))
+        logger.info(ANSI("Entering new chain.").to(Color.green(), Style.italic()))
         logger.info(ANSI("Prompted Text").to(Color.yellow()) + f': {inputs["input"]}\n')
 
     def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
-        logger.info(ANSI(f"Finished chain.").to(Color.green(), Style.italic()))
+        logger.info(ANSI("Finished chain.").to(Color.green(), Style.italic()))
 
     def on_chain_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> None:
         logger.error(
-            ANSI(f"Chain Error").to(Color.red()) + ": " + dim_multiline(str(error))
+            ANSI("Chain Error").to(Color.red()) + ": " + dim_multiline(str(error))
         )
 
     def on_tool_start(
         self,
         serialized: Dict[str, Any],
         input_str: str,
         **kwargs: Any,
```

### Comparing `swarms-1.0.8/swarms/agents/utils/ChatOpenAI.py` & `swarms-1.1.0/swarms/agents/utils/ChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/utils/ConversationalChatAgent.py` & `swarms-1.1.0/swarms/agents/utils/ConversationalChatAgent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/utils/agent_creator.py` & `swarms-1.1.0/swarms/agents/utils/agent_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import os
 import logging
 from typing import Dict, Optional
 from celery import Task
 from langchain.agents.agent import AgentExecutor
 from langchain.callbacks.manager import CallbackManager
 from langchain.chains.conversation.memory import ConversationBufferMemory
 from langchain.memory.chat_memory import BaseChatMemory
 from swarms.agents.tools.main import BaseToolSet, ToolsFactory
-from swarms.agents.prompts.prompts import EVAL_PREFIX, EVAL_SUFFIX
 
 from swarms.agents.utils.agent_setup import AgentSetup
 # from .callback import EVALCallbackHandler, ExecutionTracingCallbackHandler
 from swarms.agents.utils.Calback import EVALCallbackHandler, ExecutionTracingCallbackHandler
 
 callback_manager_instance = CallbackManager(EVALCallbackHandler())
 
@@ -27,15 +25,15 @@
         return ConversationBufferMemory(memory_key="chat_history", return_messages=True)
 
     def get_or_create_memory(self, session: str) -> BaseChatMemory:
         if not isinstance(session, str):
             raise TypeError("Session must be a string")
         if not session:
             raise ValueError("Session is empty")
-        if not (session in self.memories):
+        if session not in self.memories:
             self.memories[session] = self.create_memory()
         return self.memories[session]
 
     def create_executor(self, session: str, execution: Optional[Task] = None, openai_api_key: str = None) -> AgentExecutor:
         try:
             builder = AgentSetup(self.toolsets)
             builder.setup_parser()
```

### Comparing `swarms-1.0.8/swarms/agents/utils/agent_setup.py` & `swarms-1.1.0/swarms/agents/utils/agent_setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/utils/output_parser.py` & `swarms-1.1.0/swarms/agents/utils/output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/agents/utils/prompts.py` & `swarms-1.1.0/swarms/agents/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/boss/boss_node.py` & `swarms-1.1.0/swarms/boss/boss_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
-from pydantic import ValidationError
 import logging
+import os
+
+import faiss
+from langchain import LLMChain, OpenAI, PromptTemplate
+from langchain.agents import AgentExecutor, Tool, ZeroShotAgent
+from langchain.docstore import InMemoryDocstore
+from langchain.embeddings import OpenAIEmbeddings
+from langchain.experimental import BabyAGI
+from langchain.vectorstores import FAISS
+from pydantic import ValidationError
+
 
-from swarms.agents.tools.agent_tools import *
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 # ---------- Boss Node ----------
 class BossNodeInitializer:
     """
     The BossNode class is responsible for creating and executing tasks using the BabyAGI model.
```

### Comparing `swarms-1.0.8/swarms/hivemind.py` & `swarms-1.1.0/swarms/hivemind.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# many boss + workers in unison
+#  workers in unison
 #kye gomez jul 13 4:01pm, can scale up the number of swarms working on a probkem with `hivemind(swarms=4, or swarms=auto which will scale the agents depending on the complexity)`
 
 import concurrent.futures
 import logging
 
-from swarms.swarms import Swarms
-
 #this needs to change, we need to specify exactly what needs to be imported
 from swarms.agents.tools.agent_tools import *
+from swarms.swarms import HierarchicalSwarm
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
-
 # add typechecking, documentation, and deeper error handling 
+# TODO: MANY WORKERS
 class HiveMind:
     def __init__(self, openai_api_key="", num_swarms=1, max_workers=None):
         self.openai_api_key = openai_api_key
         self.num_swarms = num_swarms
-        self.swarms = [Swarms(openai_api_key) for _ in range(num_swarms)]
+        self.swarms = [HierarchicalSwarm(openai_api_key) for _ in range(num_swarms)]
         self.vectorstore = self.initialize_vectorstore()
         self.max_workers = max_workers if max_workers else min(32, num_swarms)
 
     def initialize_vectorstore(self):
         try:
             embeddings_model = OpenAIEmbeddings(openai_api_key=self.openai_api_key)
             embedding_size = 1536
@@ -29,31 +28,31 @@
             return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
         except Exception as e:
             logging.error(f"Failed to initialize vector store: {e}")
             raise
 
     def run_swarm(self, swarm, objective):
         try:
-            return swarm.run_swarms(objective)
+            return swarm.run(objective)
         except Exception as e:
-            logging.error(f"An error occurred in run_swarms: {e}")
+            logging.error(f"An error occurred in run: {e}")
 
-    def run_swarms(self, objective, timeout=None):
+    def run(self, objective, timeout=None):
         with concurrent.futures.ThreadPoolExecutor(max_workers=self.max_workers) as executor:
             futures = {executor.submit(self.run_swarm, swarm, objective) for swarm in self.swarms}
             results = []
             for future in concurrent.futures.as_completed(futures, timeout=timeout):
                 try:
                     results.append(future.result())
                 except Exception as e:
                     logging.error(f"An error occurred in a swarm: {e}")
         return results
     
     def add_swarm(self):
-        self.swarms.append(Swarms(self.openai_api_key))
+        self.swarms.append(HierarchicalSwarm(self.openai_api_key))
 
     def remove_swarm(self, index):
         try:
             self.swarms.pop(index)
         except IndexError:
             logging.error(f"No swarm found at index {index}")
         
@@ -65,8 +64,8 @@
         try:
             self.swarms[index].cancel()
         except IndexError:
             logging.error(f"No swarm found at index {index}")
 
     def queue_tasks(self, tasks):
         for task in tasks:
-            self.run_swarms(task)
+            self.run(task)
```

### Comparing `swarms-1.0.8/swarms/swarms.py` & `swarms-1.1.0/swarms/swarms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,99 @@
-import logging
 import asyncio
+import logging
+from typing import Optional
 
-# from swarms.agents.tools.agent_tools import *
-from swarms.agents.tools.agent_tools import *
-from swarms.workers.WorkerNode import WorkerNodeInitializer, worker_node
-from swarms.boss.boss_node import BossNodeInitializer as BossNode
-from swarms.workers.worker_ultra_node import WorkerUltra
+import faiss
+from langchain import LLMChain, OpenAI, PromptTemplate
+from langchain.agents import AgentExecutor, Tool, ZeroShotAgent
+from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain
+from langchain.chat_models import ChatOpenAI
+from langchain.docstore import InMemoryDocstore
+from langchain.embeddings import OpenAIEmbeddings
+from langchain.tools import DuckDuckGoSearchRun
+from langchain.tools.file_management.read import ReadFileTool
+from langchain.tools.file_management.write import WriteFileTool
+from langchain.vectorstores import FAISS
 
-from langchain import LLMMathChain
+from swarms.agents.models.hf import HuggingFaceLLM
 
+# from langchain.tools.human.tool import HumanInputRun
+from swarms.agents.tools.main import WebpageQATool, process_csv
+from swarms.boss.boss_node import BossNodeInitializer as BossNode
+from swarms.workers.worker_node import WorkerNodeInitializer
 
+# from langchain import LLMMathChain
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
-from swarms.utils.task import Task
-
-# TODO: Pass in abstract LLM class that can utilize Hf or Anthropic models
-# TODO: Move away from OPENAI
-class Swarms:
-    def __init__(self, openai_api_key="", use_vectorstore=True, use_async=True, human_in_the_loop=True):
-        #openai_api_key: the openai key. Default is empty
-        if not openai_api_key:
-            logging.error("OpenAI key is not provided")
-            raise ValueError("OpenAI API key is required")
+# TODO: Pass in abstract LLM class that can utilize Hf or Anthropic models, Move away from OPENAI
+# TODO: ADD Universal Communication Layer, a ocean vectorstore instance
+# TODO: BE MORE EXPLICIT ON TOOL USE, TASK DECOMPOSITION AND TASK COMPLETETION AND ALLOCATION
+# TODO: Add RLHF Data collection, ask user how the swarm is performing
+# TODO: Create an onboarding process if not settings are preconfigured like `from swarms import Swarm, Swarm()` => then initiate onboarding name your swarm + provide purpose + etc 
+
+
+# ---------- Constants ----------
+ROOT_DIR = "./data/"
+
+class HierarchicalSwarm:
+    def __init__(
+        self, 
+        model_id: Optional[str] = None, 
+        openai_api_key: Optional[str] = "", 
+
+        use_vectorstore: Optional[bool] = True, 
+        embedding_size: Optional[int] = None, 
+        use_async: Optional[bool] = True, 
+
+        human_in_the_loop: Optional[bool] = True, 
+        model_type: Optional[str] = None, 
+        boss_prompt: Optional[str] = None,
+
+        worker_prompt: Optional[str] = None,
+        temperature: Optional[float] = None,
+        max_iterations: Optional[int] = None,
+        logging_enabled: Optional[bool] = True):
         
+        self.model_id = model_id        
         self.openai_api_key = openai_api_key
         self.use_vectorstore = use_vectorstore
+
         self.use_async = use_async
         self.human_in_the_loop = human_in_the_loop
+        self.model_type = model_type
+
+        self.embedding_size = embedding_size
+        self.boss_prompt = boss_prompt
+        self.worker_prompt = worker_prompt
+
+        self.temperature = temperature
+        self.max_iterations = max_iterations
+        self.logging_enabled = logging_enabled
+
+        self.logger = logging.getLogger()
+        if not logging_enabled:
+            self.logger.disabled = True
+
 
-    def initialize_llm(self, llm_class, temperature=0.5):
+
+    def initialize_llm(self, llm_class: str = None):
         """
         Init LLM 
 
         Params:
             llm_class(class): The Language model class. Default is OpenAI.
             temperature (float): The Temperature for the language model. Default is 0.5
         """
         try: 
             # Initialize language model
-            return llm_class(openai_api_key=self.openai_api_key, temperature=temperature)
+            if self.llm_class == 'openai':
+                return OpenAI(openai_api_key=self.openai_api_key, temperature=self.temperature)
+            elif self.model_type == "huggingface":
+                return HuggingFaceLLM(model_id=self.model_id, temperature=self.temperature)
         except Exception as e:
             logging.error(f"Failed to initialize language model: {e}")
 
     def initialize_tools(self, llm_class, extra_tools=None):
         """
         Init tools
         
@@ -65,64 +115,59 @@
                 process_csv,
                 WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
             ]
 
             if extra_tools:
                 tools.extend(extra_tools)
 
-
-
             assert tools is not None, "tools is not initialized"
             return tools
 
         except Exception as e:
             logging.error(f"Failed to initialize tools: {e}")
             raise
 
     def initialize_vectorstore(self):
         """
         Init vector store
         """
-
-        try:
-                
+        try:     
             embeddings_model = OpenAIEmbeddings(openai_api_key=self.openai_api_key)
-            embedding_size = 1536
+            embedding_size = self.embedding_size
             index = faiss.IndexFlatL2(embedding_size)
 
             return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
         except Exception as e:
             logging.error(f"Failed to initialize vector store: {e}")
             return None
 
-    def initialize_worker_node(self, worker_tools, vectorstore, llm_class=ChatOpenAI, ai_name="Swarm Worker AI Assistant", human_in_the_loop=True):
+    def initialize_worker_node(self, worker_tools, vectorstore, llm_class=ChatOpenAI, ai_name="Swarm Worker AI Assistant",):
         """
         Init WorkerNode
 
         Params:
             worker_tools (list): The list of worker tools.
             vectorstore (object): The vector store object
             llm_class (class): The Language model class. Default is ChatOpenAI
             ai_name (str): The AI name. Default is "Swarms worker AI assistant"        
         """
-
-        try:
-                
+        try:    
             # Initialize worker node
             llm = self.initialize_llm(ChatOpenAI)
             worker_node = WorkerNodeInitializer(llm=llm, tools=worker_tools, vectorstore=vectorstore)
             worker_node.create_agent(ai_name=ai_name, ai_role="Assistant", search_kwargs={}, human_in_the_loop=self.human_in_the_loop) # add search kwargs
+            worker_description = self.worker_prompt
 
-            worker_node_tool = Tool(name="WorkerNode AI Agent", func=worker_node.run, description="Input: an objective with a todo list for that objective. Output: your task completed: Please be very clear what the objective and task instructions are. The Swarm worker agent is Useful for when you need to spawn an autonomous agent instance as a worker to accomplish any complex tasks, it can search the internet or write code or spawn child multi-modality models to process and generate images and text or audio and so on")
+            worker_node_tool = Tool(name="WorkerNode AI Agent", func=worker_node.run, description= worker_description or "Input: an objective with a todo list for that objective. Output: your task completed: Please be very clear what the objective and task instructions are. The Swarm worker agent is Useful for when you need to spawn an autonomous agent instance as a worker to accomplish any complex tasks, it can search the internet or write code or spawn child multi-modality models to process and generate images and text or audio and so on")
             return worker_node_tool
         except Exception as e:
             logging.error(f"Failed to initialize worker node: {e}")
             raise
 
-    def initialize_boss_node(self, vectorstore, worker_node, llm_class=OpenAI, max_iterations=5, verbose=False):
+    def initialize_boss_node(self, vectorstore, worker_node, llm_class=OpenAI, max_iterations=None, verbose=False):
         """
         Init BossNode
 
         Params:
             vectorstore (object): the vector store object.
             worker_node (object): the worker node object
             llm_class (class): the language model class. Default is OpenAI
@@ -130,43 +175,41 @@
             verbose(bool): Debug mode. Default is False
         
         """
         try:
 
             # Initialize boss node
             llm = self.initialize_llm(llm_class)
-            todo_prompt = PromptTemplate.from_template("You are a boss planer in a swarm who is an expert at coming up with a todo list for a given objective and then creating an worker to help you accomplish your task. Rate every task on the importance of it's probability to complete the main objective on a scale from 0 to 1, an integer. Come up with a todo list for this objective: {objective} and then spawn a worker agent to complete the task for you. Always spawn an worker agent after creating a plan and pass the objective and plan to the worker agent.")
+            
+            # prompt = self.boss_prompt
+            todo_prompt = PromptTemplate.from_template({self.boss_prompt} or "You are a boss planer in a swarm who is an expert at coming up with a todo list for a given objective and then creating an worker to help you accomplish your task. Rate every task on the importance of it's probability to complete the main objective on a scale from 0 to 1, an integer. Come up with a todo list for this objective: {objective} and then spawn a worker agent to complete the task for you. Always spawn an worker agent after creating a plan and pass the objective and plan to the worker agent.")
             todo_chain = LLMChain(llm=llm, prompt=todo_prompt)
 
-            #math tool
-            # llm_math_chain = LLMMathChain.from_llm(llm=llm, verbose=True)
-
             tools = [
                 Tool(name="TODO", func=todo_chain.run, description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for your objective. Note create a todo list then assign a ranking from 0.0 to 1.0 to each task, then sort the tasks based on the tasks most likely to achieve the objective. The Output: a todo list for that objective with rankings for each step from 0.1 Please be very clear what the objective is!"),
                 worker_node,
-                # Tool(name="Calculator", func=llm_math_chain.run, description="useful for when you need to answer questions about math")
             ]
 
             suffix = """Question: {task}\n{agent_scratchpad}"""
             prefix = """You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n """
             
             prompt = ZeroShotAgent.create_prompt(tools, prefix=prefix, suffix=suffix, input_variables=["objective", "task", "context", "agent_scratchpad"],)
             llm_chain = LLMChain(llm=llm, prompt=prompt)
             agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=[tool.name for tool in tools])
 
             agent_executor = AgentExecutor.from_agent_and_tools(agent=agent, tools=tools, verbose=verbose)
-            return BossNode(llm, vectorstore, agent_executor, max_iterations=max_iterations)
+            return BossNode(llm, vectorstore, agent_executor, max_iterations=self.max_iterations)
         except Exception as e:
             logging.error(f"Failed to initialize boss node: {e}")
             raise
 
 
 
 
-    def run_swarms(self, objective):
+    def run(self, objective):
         """
         Run the swarm with the given objective
 
         Params:
             objective(str): The task
         """
         try:
@@ -185,19 +228,24 @@
                 loop = asyncio.get_event_loop()
                 result = loop.run_until_complete(boss_node.run(task))
             else:
                 result = boss_node.run(task)
             logging.info(f"Completed tasks: {task}")
             return result
         except Exception as e:
-            logging.error(f"An error occurred in run_swarms: {e}")
+            logging.error(f"An error occurred in run: {e}")
             return None
         
 # usage-# usage-
-def swarm(api_key="", objective=""):
+def swarm(
+    api_key: Optional[str]="", 
+    objective: Optional[str]="", 
+    model_type: Optional[str]="", 
+    model_id: Optional[str]=""
+    ):
     """
     Run the swarm with the given API key and objective.
 
     Parameters:
     api_key (str): The OpenAI API key. Default is an empty string.
     objective (str): The objective. Default is an empty string.
 
@@ -208,19 +256,18 @@
     if not api_key or not isinstance(api_key, str):
         logging.error("Invalid OpenAI key")
         raise ValueError("A valid OpenAI API key is required")
     if not objective or not isinstance(objective, str):
         logging.error("Invalid objective")
         raise ValueError("A valid objective is required")
     try:
-        swarms = Swarms(api_key, use_async=False) # Turn off async
-        result = swarms.run_swarms(objective)
+        swarms = HierarchicalSwarm(api_key, model_id=model_type, use_async=False, model_type=model_type) #logging_enabled=logging_enabled) # Turn off async
+        result = swarms.run(objective)
         if result is None:
             logging.error("Failed to run swarms")
         else:
             logging.info(f"Successfully ran swarms with results: {result}")
         return result
     except Exception as e:
         logging.error(f"An error occured in swarm: {e}")
         return None
 
-
```

### Comparing `swarms-1.0.8/swarms/utils/embeddings/base.py` & `swarms-1.1.0/swarms/utils/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/utils/main.py` & `swarms-1.1.0/swarms/utils/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/utils/static.py` & `swarms-1.1.0/swarms/utils/static.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/WorkerNode.py` & `swarms-1.1.0/swarms/workers/worker_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,34 @@
-from swarms.agents.tools.agent_tools import *
-from langchain.tools import BaseTool
-from typing import Optional, Type
-
-from langchain.callbacks.manager import (
-    AsyncCallbackManagerForToolRun,
-    CallbackManagerForToolRun,
-)
-from typing import List, Any, Dict, Optional
+import logging
+
+import faiss
+from langchain.agents import Tool
+from langchain.chains.qa_with_sources.loading import load_qa_with_sources_chain
+from langchain.chat_models import ChatOpenAI
+from langchain.docstore import InMemoryDocstore
+from langchain.embeddings import OpenAIEmbeddings
+from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
 from langchain.memory.chat_message_histories import FileChatMessageHistory
+from langchain.tools import DuckDuckGoSearchRun
+from langchain.tools.file_management.read import ReadFileTool
+from langchain.tools.file_management.write import WriteFileTool
+from langchain.vectorstores import FAISS
+
+# from langchain.tools.human.tool import HumanInputRun
+from swarms.agents.tools.main import WebpageQATool, process_csv
+
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+
+
+ROOT_DIR = "./data/"
 
-import logging
-from pydantic import BaseModel, Extra
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
-from swarms.agents.tools.main import Terminal
 
 class WorkerNodeInitializer:
     """Useful for when you need to spawn an autonomous agent instance as a worker to accomplish complex tasks, it can search the internet or spawn child multi-modality models to process and generate images and text or audio and so on"""
 
     def __init__(self, llm, tools, vectorstore):
         if not llm or not tools or not vectorstore:
             logging.error("llm, tools, and vectorstore cannot be None.")
@@ -104,15 +115,14 @@
 
             tools = [
                 web_search,
                 WriteFileTool(root_dir=ROOT_DIR),
                 ReadFileTool(root_dir=ROOT_DIR),
                 process_csv,
                 WebpageQATool(qa_chain=load_qa_with_sources_chain(llm)),
-                Terminal,
             ]
             if not tools:
                 logging.error("Tools are not initialized")
                 raise ValueError("Tools are not initialized")
             return tools
         except Exception as e:
             logging.error(f"Failed to initialize tools: {e}")
```

### Comparing `swarms-1.0.8/swarms/workers/character_generative.py` & `swarms-1.1.0/swarms/workers/character_generative.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 # Copyright (c) 2021 Microsoft. All Rights Reserved.
 # Licensed under the Apache License, Version 2.0 [see LICENSE for details]
 # ------------------------------------------------------------------------
 # Copied from DETR (https://github.com/facebookresearch/detr)
 # Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved.
 # ------------------------------------------------------------------------
 
-from .groundingdino import build_groundingdino
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import torch
 import torch.nn.functional as F
 import torchvision
 from torch import nn
 from torchvision.models._utils import IntermediateLayerGetter
 
-from groundingdino.util.misc import NestedTensor, clean_state_dict, is_main_process
+from groundingdino.util.misc import NestedTensor, is_main_process
 
 from .position_encoding import build_position_encoding
 from .swin_transformer import build_swin_transformer
 
 
 class FrozenBatchNorm2d(torch.nn.Module):
     """
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 # Grounding DINO
 # url: https://github.com/IDEA-Research/GroundingDINO
 # Copyright (c) 2023 IDEA. All Rights Reserved.
 # Licensed under the Apache License, Version 2.0 [see LICENSE for details]
 # ------------------------------------------------------------------------
 
 import torch
-import torch.nn.functional as F
-import torch.utils.checkpoint as checkpoint
-from torch import Tensor, nn
-from torchvision.ops.boxes import nms
-from transformers import BertConfig, BertModel, BertPreTrainedModel
+from torch import nn
 from transformers.modeling_outputs import BaseModelOutputWithPoolingAndCrossAttentions
 
 
 class BertModelWarper(nn.Module):
     def __init__(self, bert_model):
         super().__init__()
         # self.bert = bert_modelc
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,40 +16,30 @@
 # ------------------------------------------------------------------------
 import copy
 from typing import List
 
 import torch
 import torch.nn.functional as F
 from torch import nn
-from torchvision.ops.boxes import nms
-from transformers import AutoTokenizer, BertModel, BertTokenizer, RobertaModel, RobertaTokenizerFast
 
-from groundingdino.util import box_ops, get_tokenlizer
+from groundingdino.util import get_tokenlizer
 from groundingdino.util.misc import (
     NestedTensor,
-    accuracy,
-    get_world_size,
-    interpolate,
     inverse_sigmoid,
-    is_dist_avail_and_initialized,
     nested_tensor_from_tensor_list,
 )
-from groundingdino.util.utils import get_phrases_from_posmap
-from groundingdino.util.visualizer import COCOVisualizer
-from groundingdino.util.vl_utils import create_positive_map_from_span
 
 from ..registry import MODULE_BUILD_FUNCS
 from .backbone import build_backbone
 from .bertwarper import (
     BertModelWarper,
-    generate_masks_with_special_tokens,
     generate_masks_with_special_tokens_and_transfer_map,
 )
 from .transformer import build_transformer
-from .utils import MLP, ContrastiveEmbed, sigmoid_focal_loss
+from .utils import MLP, ContrastiveEmbed
 
 
 class GroundingDINO(nn.Module):
     """This is the Cross-Attention Detector module that performs object detection"""
 
     def __init__(
         self,
@@ -148,15 +138,15 @@
                         nn.GroupNorm(32, hidden_dim),
                     )
                 ]
             )
 
         self.backbone = backbone
         self.aux_loss = aux_loss
-        self.box_pred_damping = box_pred_damping = None
+        self.box_pred_damping = None
 
         self.iter_update = iter_update
         assert iter_update, "Why not iter_update?"
 
         # prepare pred layers
         self.dec_pred_bbox_embed_share = dec_pred_bbox_embed_share
         # prepare class & box embed
@@ -304,15 +294,15 @@
                 m = samples.mask
                 mask = F.interpolate(m[None].float(), size=src.shape[-2:]).to(torch.bool)[0]
                 pos_l = self.backbone[1](NestedTensor(src, mask)).to(src.dtype)
                 srcs.append(src)
                 masks.append(mask)
                 poss.append(pos_l)
 
-        input_query_bbox = input_query_label = attn_mask = dn_meta = None
+        input_query_bbox = input_query_label = attn_mask = None
         hs, reference, hs_enc, ref_enc, init_box_proposal = self.transformer(
             srcs, masks, input_query_bbox, poss, input_query_label, attn_mask, text_dict
         )
 
         # deformable-detr-like anchor update
         outputs_coord_list = []
         for dec_lid, (layer_ref_sig, layer_bbox_embed, layer_hs) in enumerate(
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,14 @@
         )
         level_start_index = torch.cat(
             (spatial_shapes.new_zeros((1,)), spatial_shapes.prod(1).cumsum(0)[:-1])
         )
         valid_ratios = torch.stack([self.get_valid_ratio(m) for m in masks], 1)
 
         # two stage
-        enc_topk_proposals = enc_refpoint_embed = None
 
         #########################################################
         # Begin Encoder
         #########################################################
         memory, memory_text = self.encoder(
             src_flatten,
             pos=lvl_pos_embed_flatten,
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,19 @@
     * positional encodings are passed in MHattention
     * extra LN at the end of encoder is removed
     * decoder returns a stack of activations from all decoding layers
 """
 from typing import Optional
 
 import torch
-import torch.nn.functional as F
 from torch import Tensor, nn
 
 from .utils import (
-    MLP,
     _get_activation_fn,
     _get_clones,
-    gen_encoder_output_proposals,
-    gen_sineembed_for_position,
-    sigmoid_focal_loss,
 )
 
 
 class TextTransformer(nn.Module):
     def __init__(self, num_layers, d_model=256, nheads=8, dim_feedforward=2048, dropout=0.1):
         super().__init__()
         self.num_layers = num_layers
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from transformers import AutoTokenizer, BertModel, BertTokenizer, RobertaModel, RobertaTokenizerFast
+from transformers import AutoTokenizer, BertModel, RobertaModel
 import os
 
 def get_tokenlizer(text_encoder_type):
     if not isinstance(text_encoder_type, str):
         # print("text_encoder_type is not a str")
         if hasattr(text_encoder_type, "text_encoder_type"):
             text_encoder_type = text_encoder_type.text_encoder_type
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,16 @@
         "max_freq_log2": multires - 1,
         "num_freqs": multires,
         "log_sampling": True,
         "periodic_fns": [torch.sin, torch.cos],
     }
 
     embedder_obj = Embedder(**embed_kwargs)
-    embed = lambda x, eo=embedder_obj: eo.embed(x)
+    def embed(x, eo=embedder_obj):
+        return eo.embed(x)
     return embed, embedder_obj.out_dim
 
 
 class APOPMeter:
     def __init__(self) -> None:
         self.tp = 0
         self.fp = 0
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 @Author  :   Shilong Liu 
 @Contact :   slongliu86@gmail.com
 """
 
 import datetime
 import os
 
-import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from matplotlib import transforms
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Polygon
 from pycocotools import mask as maskUtils
@@ -130,15 +129,15 @@
         print("savename: {}".format(savename))
         os.makedirs(os.path.dirname(savename), exist_ok=True)
         plt.savefig(savename)
         plt.close()
 
     def addtgt(self, tgt):
         """ """
-        if tgt is None or not "boxes" in tgt:
+        if tgt is None or "boxes" not in tgt:
             ax = plt.gca()
 
             if "caption" in tgt:
                 ax.set_title(tgt["caption"], wrap=True)
 
             ax.set_axis_off()
             return
```

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/GroundingDINO/setup.py` & `swarms-1.1.0/swarms/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/models/segment_anything/setup.py` & `swarms-1.1.0/swarms/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/multi_modal_worker.py` & `swarms-1.1.0/swarms/workers/multi_modal_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-1.1.0/swarms/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,62 @@
 # coding: utf-8
+import argparse
+import inspect
+import math
 import os
-import gradio as gr
 import random
-import torch
-import cv2
 import re
 import uuid
-from PIL import Image, ImageDraw, ImageOps, ImageFont
-import math
+
+import cv2
+import gradio as gr
+import matplotlib.pyplot as plt
 import numpy as np
-import argparse
-import inspect
-import tempfile
-from transformers import CLIPSegProcessor, CLIPSegForImageSegmentation
-from transformers import pipeline, BlipProcessor, BlipForConditionalGeneration, BlipForQuestionAnswering
-from transformers import AutoImageProcessor, UperNetForSemanticSegmentation
-
-from diffusers import StableDiffusionPipeline, StableDiffusionInpaintPipeline, StableDiffusionInstructPix2PixPipeline
-from diffusers import EulerAncestralDiscreteScheduler
-from diffusers import StableDiffusionControlNetPipeline, ControlNetModel, UniPCMultistepScheduler
+import torch
+import wget
+from controlnet_aux import HEDdetector, MLSDdetector, OpenposeDetector
+from diffusers import (
+    ControlNetModel,
+    EulerAncestralDiscreteScheduler,
+    StableDiffusionControlNetPipeline,
+    StableDiffusionInpaintPipeline,
+    StableDiffusionInstructPix2PixPipeline,
+    StableDiffusionPipeline,
+    UniPCMultistepScheduler,
+)
 from diffusers.pipelines.stable_diffusion import StableDiffusionSafetyChecker
-
-from controlnet_aux import OpenposeDetector, MLSDdetector, HEDdetector
-
 from langchain.agents.initialize import initialize_agent
 from langchain.agents.tools import Tool
 from langchain.chains.conversation.memory import ConversationBufferMemory
 from langchain.llms.openai import OpenAI
+from PIL import Image, ImageDraw, ImageFont, ImageOps
+from transformers import (
+    BlipForConditionalGeneration,
+    BlipForQuestionAnswering,
+    BlipProcessor,
+    pipeline,
+)
 
 # Grounding DINO
 # import groundingdino.datasets.transforms as T
 from swarms.workers.models import (
     Compose,
     Normalize,
-    ToTensor,
-    crop,
-    hflip,
-    resize,
-    pad,
-    ResizeDebug,
-    RandomCrop,
-    RandomSizeCrop,
-    CenterCrop,
-    RandomHorizontalFlip,
     RandomResize,
-    RandomPad,
-    RandomSelect
+    SLConfig,
+    ToTensor,
+    build_model,
+    clean_state_dict,
+    get_phrases_from_posmap,
+)
+from swarms.workers.models.segment_anything import (
+    SamAutomaticMaskGenerator,
+    SamPredictor,
+    build_sam,
 )
-
-from swarms.workers.models import build_model
-from swarms.workers.models  import box_ops
-from swarms.workers.models import SLConfig
-from swarms.workers.models import clean_state_dict, get_phrases_from_posmap
-
-from swarms.workers.models.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
-import cv2
-import numpy as np
-import matplotlib.pyplot as plt
-import wget
 
 VISUAL_AGENT_PREFIX = """Worker Multi-Modal Agent is designed to be able to assist with a wide range of text and visual related tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. Worker Multi-Modal Agent is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
 
 Worker Multi-Modal Agent is able to process and understand large amounts of text and images. As a language model, Worker Multi-Modal Agent can not directly read images, but it has a list of tools to finish different visual tasks. Each image will have a file name formed as "image/xxx.png", and Worker Multi-Modal Agent can invoke different tools to indirectly understand pictures. When talking about images, Worker Multi-Modal Agent is very strict to the file name and will never fabricate nonexistent files. When using tools to generate new image files, Worker Multi-Modal Agent is also known that the image may not be the same as the user's demand, and will use other visual question answering tools or description tools to observe the real image. Worker Multi-Modal Agent is able to use tools in a sequence, and is loyal to the tool observation outputs rather than faking the image content and image file name. It will remember to provide the file name from the last tool observation, if a new image is generated.
 
 Human may provide new figures to Worker Multi-Modal Agent with a description. The description helps Worker Multi-Modal Agent to understand this image, but Worker Multi-Modal Agent should use tools to finish following tasks, rather than directly imagine from the description.
 
@@ -1015,16 +1010,14 @@
         plt.figure(figsize=(20,20))
         plt.imshow(image)
         if len(masks) == 0:
             return
         sorted_anns = sorted(masks, key=(lambda x: x['area']), reverse=True)
         ax = plt.gca()
         ax.set_autoscale_on(False)
-        polygons = []
-        color = []
         for ann in sorted_anns:
             m = ann['segmentation']
             img = np.ones((m.shape[0], m.shape[1], 3))
             color_mask = np.random.random((1, 3)).tolist()[0]
             for i in range(3):
                 img[:,:,i] = color_mask[i]
             ax.imshow(np.dstack((img, m)))
@@ -1359,23 +1352,23 @@
         merged_mask = self.merge_masks(masks)
         # draw output image
 
         for mask in masks:
             image = self.sam.show_mask(mask[0].cpu().numpy(), image, random_color=True, transparency=0.3)
 
 
-        merged_mask_image = Image.fromarray(merged_mask)
+        Image.fromarray(merged_mask)
 
         return merged_mask
 
 
 class ImageEditing:
     template_model = True
     def __init__(self, Text2Box:Text2Box, Segmenting:Segmenting, Inpainting:Inpainting):
-        print(f"Initializing ImageEditing")
+        print("Initializing ImageEditing")
         self.sam = Segmenting
         self.grounding = Text2Box
         self.inpaint = Inpainting
 
     def pad_edge(self,mask,padding):
         #mask Tensor [H,W]
         mask = mask.numpy()
```

### Comparing `swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,26 @@
 import uuid
 import numpy as np
 from transformers import pipeline
 from diffusers import DiffusionPipeline, StableDiffusionControlNetPipeline, ControlNetModel, UniPCMultistepScheduler
 from diffusers.utils import load_image
 from diffusers import DiffusionPipeline, DPMSolverMultistepScheduler
 from diffusers.utils import export_to_video
-from transformers import SpeechT5Processor, SpeechT5ForTextToSpeech, SpeechT5HifiGan, SpeechT5ForSpeechToSpeech
-from transformers import BlipProcessor, BlipForConditionalGeneration
-from transformers import TrOCRProcessor, VisionEncoderDecoderModel, ViTImageProcessor, AutoTokenizer
+from transformers import SpeechT5Processor, SpeechT5HifiGan, SpeechT5ForSpeechToSpeech
+from transformers import VisionEncoderDecoderModel, ViTImageProcessor, AutoTokenizer
 from datasets import load_dataset
 from PIL import Image
 # import flask
 # from flask import request, jsonify
 import waitress
 # from flask_cors import CORS
-import io
 from torchvision import transforms
 import torch
 import torchaudio
-from speechbrain.pretrained import WaveformEnhancement
-import joblib
-from huggingface_hub import hf_hub_url, cached_download
-from transformers import AutoImageProcessor, TimesformerForVideoClassification
-from transformers import MaskFormerFeatureExtractor, MaskFormerForInstanceSegmentation, AutoFeatureExtractor
+from transformers import MaskFormerFeatureExtractor, MaskFormerForInstanceSegmentation
 from controlnet_aux import OpenposeDetector, MLSDdetector, HEDdetector, CannyDetector, MidasDetector
 from controlnet_aux.open_pose.body import Body
 from controlnet_aux.mlsd.models.mbv2_mlsd_large import MobileV2_MLSD_Large
 from controlnet_aux.hed import Network
 from transformers import DPTForDepthEstimation, DPTFeatureExtractor
 import warnings
 import time
@@ -115,15 +109,15 @@
             #     "device": device
             # },
             "JorisCos/DCCRNet_Libri1Mix_enhsingle_16k": {
                 "model": BaseModel.from_pretrained("JorisCos/DCCRNet_Libri1Mix_enhsingle_16k"),
                 "device": device
             },
             "espnet/kan-bayashi_ljspeech_vits": {
-                "model": Text2Speech.from_pretrained(f"espnet/kan-bayashi_ljspeech_vits"),
+                "model": Text2Speech.from_pretrained("espnet/kan-bayashi_ljspeech_vits"),
                 "device": device
             },
             "lambdalabs/sd-image-variations-diffusers": {
                 "model": DiffusionPipeline.from_pretrained(f"{local_fold}/lambdalabs/sd-image-variations-diffusers"), #torch_dtype=torch.float16
                 "device": device
             },
             # "CompVis/stable-diffusion-v1-4": {
```

### Comparing `swarms-1.0.8/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-1.1.0/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 from PIL import Image, ImageDraw
 from diffusers.utils import load_image
 from pydub import AudioSegment
 import threading
 from queue import Queue
 # import flask
 # from flask import request, jsonify
-import waitress
 # from flask_cors import CORS, cross_origin
 from swarms.workers.multi_modal_workers.omni_agent.get_token_ids import get_token_ids_for_task_parsing, get_token_ids_for_choose_model, count_tokens, get_max_context_length
 from huggingface_hub.inference_api import InferenceApi
-from huggingface_hub.inference_api import ALL_TASKS
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--config", type=str, default="swarms/agents/workers/multi_modal_workers/omni_agent/config.yml")
 parser.add_argument("--mode", type=str, default="cli")
 args = parser.parse_args()
 
 if __name__ != "__main__":
@@ -249,15 +247,15 @@
         f = open("logs/log_fail.jsonl", "a")
     log = args
     f.write(json.dumps(log) + "\n")
     f.close()
 
 def image_to_bytes(img_url):
     img_byte = io.BytesIO()
-    type = img_url.split(".")[-1]
+    img_url.split(".")[-1]
     load_image(img_url).save(img_byte, format="png")
     img_data = img_byte.getvalue()
     return img_data
 
 def resource_has_dep(command):
     args = command["args"]
     for _, v in args.items():
@@ -805,15 +803,15 @@
             hosted_on = "local"
             reason = "ControlNet is the best model for this task."
             choose = {"id": best_model_id, "reason": reason}
             logger.debug(f"chosen model: {choose}")
         else:
             logger.warning(f"Task {command['task']} is not available. ControlNet need to be deployed locally.")
             record_case(success=False, **{"input": input, "task": command, "reason": f"Task {command['task']} is not available. ControlNet need to be deployed locally.", "op":"message"})
-            inference_result = {"error": f"service related to ControlNet is not available."}
+            inference_result = {"error": "service related to ControlNet is not available."}
             results[id] = collect_result(command, "", inference_result)
             return False
     elif task in ["summarization", "translation", "conversational", "text-generation", "text2text-generation"]: # ChatGPT Can do
         best_model_id = "ChatGPT"
         reason = "ChatGPT performs well on some NLP tasks as well."
         choose = {"id": best_model_id, "reason": reason}
         messages = [{
@@ -868,15 +866,15 @@
             choose_str = choose_model(input, command, cand_models_info, api_key, api_type, api_endpoint)
             logger.debug(f"chosen model: {choose_str}")
             try:
                 choose = json.loads(choose_str)
                 reason = choose["reason"]
                 best_model_id = choose["id"]
                 hosted_on = "local" if best_model_id in all_avaliable_models["local"] else "huggingface"
-            except Exception as e:
+            except Exception:
                 logger.warning(f"the response [ {choose_str} ] is not a valid JSON, try to find the model id and reason in the response.")
                 choose_str = find_json(choose_str)
                 best_model_id, reason, choose  = get_id_reason(choose_str)
                 hosted_on = "local" if best_model_id in all_avaliable_models["local"] else "huggingface"
     inference_result = model_inference(best_model_id, args, hosted_on, command['task'])
 
     if "error" in inference_result:
```

### Comparing `swarms-1.0.8/swarms/workers/omni_worker.py` & `swarms-1.1.0/swarms/workers/omni_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms/workers/worker_agent_ultra.py` & `swarms-1.1.0/swarms/workers/worker_agent_ultra.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-import os
 import logging
-from typing import Optional, Type
-from langchain.callbacks.manager import (
-    AsyncCallbackManagerForToolRun,
-    CallbackManagerForToolRun,
-)
+import os
+from typing import Dict, List
 
+from langchain.memory.chat_message_histories import FileChatMessageHistory
 
 from swarms.agents.tools.agent_tools import *
-from typing import List, Any, Dict, Optional
-from langchain.memory.chat_message_histories import FileChatMessageHistory
 
-import logging
-from pydantic import BaseModel, Extra
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 
 
-from typing import List, Any, Dict, Optional
+from typing import Dict, List
+
 from langchain.memory.chat_message_histories import FileChatMessageHistory
-from swarms.utils.main import BaseHandler, FileHandler, FileType
-from swarms.agents.tools.main import ExitConversation, RequestsGet, CodeEditor, Terminal
-from swarms.utils.main import CsvToDataframe
-from swarms.agents.tools.main import BaseToolSet
-from swarms.utils.main import StaticUploader
+
+from swarms.agents.tools.main import (
+    BaseToolSet,
+    CodeEditor,
+    ExitConversation,
+    RequestsGet,
+    Terminal,
+)
+from swarms.utils.main import BaseHandler, CsvToDataframe, FileType
 
 
 class WorkerUltraNode:
     """Useful for when you need to spawn an autonomous agent instance as a worker to accomplish complex tasks, it can search the internet or spawn child multi-modality models to process and generate images and text or audio and so on"""
 
     def __init__(self, llm, toolsets, vectorstore):
         if not llm or not toolsets or not vectorstore:
@@ -108,16 +106,22 @@
                 RequestsGet(),
                 ExitConversation(),
             ]
             handlers: Dict[FileType, BaseHandler] = {FileType.DATAFRAME: CsvToDataframe()}
 
             if os.environ.get("USE_GPU", False):
                 import torch
-                from swarms.agents.tools.main import ImageCaptioning
-                from swarms.agents.tools.main import ImageEditing, InstructPix2Pix, Text2Image, VisualQuestionAnswering
+
+                from swarms.agents.tools.main import (
+                    ImageCaptioning,
+                    ImageEditing,
+                    InstructPix2Pix,
+                    Text2Image,
+                    VisualQuestionAnswering,
+                )
 
                 if torch.cuda.is_available():
                     toolsets.extend(
                         [
                             Text2Image("cuda"),
                             ImageEditing("cuda"),
                             InstructPix2Pix("cuda"),
```

### Comparing `swarms-1.0.8/swarms/workers/worker_ultra_node.py` & `swarms-1.1.0/swarms/workers/worker_ultra_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.8/swarms.egg-info/PKG-INFO` & `swarms-1.1.0/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.0.8
+Version: 1.1.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.0.8/swarms.egg-info/SOURCES.txt` & `swarms-1.1.0/swarms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 LICENSE
 README.md
 setup.py
 api/__init__.py
 api/app.py
 swarms/__init__.py
 swarms/hivemind.py
+swarms/orchestrate.py
 swarms/swarms.py
 swarms.egg-info/PKG-INFO
 swarms.egg-info/SOURCES.txt
 swarms.egg-info/dependency_links.txt
 swarms.egg-info/requires.txt
 swarms.egg-info/top_level.txt
 swarms/agents/__init__.py
+swarms/agents/agent.py
 swarms/agents/memory/__init__.py
 swarms/agents/memory/base.py
 swarms/agents/memory/chroma.py
+swarms/agents/memory/ocean.py
 swarms/agents/models/__init__.py
+swarms/agents/models/hf.py
 swarms/agents/models/llm.py
+swarms/agents/models/petals_hf.py
 swarms/agents/prompts/__init__.py
 swarms/agents/prompts/prompts.py
 swarms/agents/prompts/chains/__init__.py
 swarms/agents/prompts/chains/llm.py
 swarms/agents/tools/__init__.py
-swarms/agents/tools/agent_tools.py
 swarms/agents/tools/base.py
 swarms/agents/tools/main.py
 swarms/agents/tools/core/__init__.py
 swarms/agents/tools/core/code_interpreter/__init__.py
 swarms/agents/tools/core/code_interpreter/main.py
 swarms/agents/utils/Agent.py
 swarms/agents/utils/Calback.py
@@ -42,23 +46,24 @@
 swarms/utils/__init__.py
 swarms/utils/logger.py
 swarms/utils/main.py
 swarms/utils/static.py
 swarms/utils/task.py
 swarms/utils/embeddings/__init__.py
 swarms/utils/embeddings/base.py
+swarms/utils/embeddings/pegasus.py
 swarms/utils/schema/__init__.py
 swarms/utils/schema/base.py
-swarms/workers/WorkerNode.py
 swarms/workers/__init__.py
 swarms/workers/character_generative.py
 swarms/workers/generative_worker.py
 swarms/workers/multi_modal_worker.py
 swarms/workers/omni_worker.py
 swarms/workers/worker_agent_ultra.py
+swarms/workers/worker_node.py
 swarms/workers/worker_ultra_node.py
 swarms/workers/models/__init__.py
 swarms/workers/models/GroundingDINO/__init__.py
 swarms/workers/models/GroundingDINO/setup.py
 swarms/workers/models/GroundingDINO/groundingdino/__init__.py
 swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
 swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
```

### Comparing `swarms-1.0.8/swarms.egg-info/requires.txt` & `swarms-1.1.0/swarms.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 langchain
 torch
 torchvision
 torchaudio
 asyncio
 nest_asyncio
 bs4
+pegasusx
+oceandb
 playwright
 duckduckgo_search
 faiss-cpu
 wget==3.2
 accelerate
+sphinx_rtd_theme
 addict
 albumentations
 basicsr
 controlnet-aux
 diffusers
 einops
 gradio
@@ -51,21 +54,21 @@
 pydantic==1.10.6
 tenacity==8.2.2
 python-dotenv
 boto3
 uvicorn==0.21.1
 jinja2==3.1.2
 python-multipart==0.0.6
-celery==5.2.7
-redis==4.5.4
+celery==5.3.1
+redis==4.6.0
 sentencepiece
-bitsandbytes==0.37.2
+bitsandbytes==0.41.0
 psycopg2-binary==2.9.5
 google-search-results==2.4.2
-black==23.1.0
+black==23.7.0
 Pillow
 selenium
 diffusers
 controlnet_aux
 tiktoken
 espnet==202301
 espnet_model_zoo==0.1.7
```

