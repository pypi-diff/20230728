# Comparing `tmp/dara_core-0.0.1-py3-none-any.whl.zip` & `tmp/dara_core-1.0.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,103 @@
-Zip file size: 1644 bytes, number of entries: 6
--rw-r--r--  2.0 unx      551 b- defN 80-Jan-01 00:00 dara/core/logo.py
--rw-r--r--  2.0 unx      100 b- defN 80-Jan-01 00:00 dara/core/main.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_core-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 dara_core-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      310 b- defN 80-Jan-01 00:00 dara_core-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx      454 b- defN 16-Jan-01 00:00 dara_core-0.0.1.dist-info/RECORD
-6 files, 1547 bytes uncompressed, 820 bytes compressed:  47.0%
+Zip file size: 3214575 bytes, number of entries: 101
+-rw-r--r--  2.0 unx     1994 b- defN 80-Jan-01 00:00 dara/core/__init__.py
+-rw-r--r--  2.0 unx      868 b- defN 80-Jan-01 00:00 dara/core/actions.py
+-rw-r--r--  2.0 unx      851 b- defN 80-Jan-01 00:00 dara/core/auth/__init__.py
+-rw-r--r--  2.0 unx     2638 b- defN 80-Jan-01 00:00 dara/core/auth/base.py
+-rw-r--r--  2.0 unx     4692 b- defN 80-Jan-01 00:00 dara/core/auth/basic.py
+-rw-r--r--  2.0 unx     3482 b- defN 80-Jan-01 00:00 dara/core/auth/definitions.py
+-rw-r--r--  2.0 unx     4155 b- defN 80-Jan-01 00:00 dara/core/auth/routes.py
+-rw-r--r--  2.0 unx     2855 b- defN 80-Jan-01 00:00 dara/core/auth/utils.py
+-rw-r--r--  2.0 unx     7764 b- defN 80-Jan-01 00:00 dara/core/base_definitions.py
+-rw-r--r--  2.0 unx     6583 b- defN 80-Jan-01 00:00 dara/core/cli.py
+-rw-r--r--  2.0 unx    16584 b- defN 80-Jan-01 00:00 dara/core/configuration.py
+-rw-r--r--  2.0 unx     1771 b- defN 80-Jan-01 00:00 dara/core/css.py
+-rw-r--r--  2.0 unx    12601 b- defN 80-Jan-01 00:00 dara/core/data_utils.py
+-rw-r--r--  2.0 unx     4205 b- defN 80-Jan-01 00:00 dara/core/defaults.py
+-rw-r--r--  2.0 unx    19836 b- defN 80-Jan-01 00:00 dara/core/definitions.py
+-rw-r--r--  2.0 unx     4658 b- defN 80-Jan-01 00:00 dara/core/http.py
+-rw-r--r--  2.0 unx     2552 b- defN 80-Jan-01 00:00 dara/core/interactivity/__init__.py
+-rw-r--r--  2.0 unx    20409 b- defN 80-Jan-01 00:00 dara/core/interactivity/actions.py
+-rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 dara/core/interactivity/any_data_variable.py
+-rw-r--r--  2.0 unx    11455 b- defN 80-Jan-01 00:00 dara/core/interactivity/any_variable.py
+-rw-r--r--  2.0 unx     1424 b- defN 80-Jan-01 00:00 dara/core/interactivity/condition.py
+-rw-r--r--  2.0 unx     8526 b- defN 80-Jan-01 00:00 dara/core/interactivity/data_variable.py
+-rw-r--r--  2.0 unx    12366 b- defN 80-Jan-01 00:00 dara/core/interactivity/derived_data_variable.py
+-rw-r--r--  2.0 unx    20482 b- defN 80-Jan-01 00:00 dara/core/interactivity/derived_variable.py
+-rw-r--r--  2.0 unx     8494 b- defN 80-Jan-01 00:00 dara/core/interactivity/filtering.py
+-rw-r--r--  2.0 unx     1147 b- defN 80-Jan-01 00:00 dara/core/interactivity/non_data_variable.py
+-rw-r--r--  2.0 unx     4037 b- defN 80-Jan-01 00:00 dara/core/interactivity/plain_variable.py
+-rw-r--r--  2.0 unx     2191 b- defN 80-Jan-01 00:00 dara/core/interactivity/url_variable.py
+-rw-r--r--  2.0 unx      577 b- defN 80-Jan-01 00:00 dara/core/internal/__init__.py
+-rw-r--r--  2.0 unx     3061 b- defN 80-Jan-01 00:00 dara/core/internal/cgroup.py
+-rw-r--r--  2.0 unx     4987 b- defN 80-Jan-01 00:00 dara/core/internal/dependency_resolution.py
+-rw-r--r--  2.0 unx     2491 b- defN 80-Jan-01 00:00 dara/core/internal/devtools.py
+-rw-r--r--  2.0 unx     2385 b- defN 80-Jan-01 00:00 dara/core/internal/download.py
+-rw-r--r--  2.0 unx     3522 b- defN 80-Jan-01 00:00 dara/core/internal/execute_action.py
+-rw-r--r--  2.0 unx     1098 b- defN 80-Jan-01 00:00 dara/core/internal/hashing.py
+-rw-r--r--  2.0 unx     7491 b- defN 80-Jan-01 00:00 dara/core/internal/import_discovery.py
+-rw-r--r--  2.0 unx     6608 b- defN 80-Jan-01 00:00 dara/core/internal/normalization.py
+-rw-r--r--  2.0 unx     1427 b- defN 80-Jan-01 00:00 dara/core/internal/pandas_utils.py
+-rw-r--r--  2.0 unx      657 b- defN 80-Jan-01 00:00 dara/core/internal/pool/__init__.py
+-rw-r--r--  2.0 unx     4948 b- defN 80-Jan-01 00:00 dara/core/internal/pool/channel.py
+-rw-r--r--  2.0 unx     4645 b- defN 80-Jan-01 00:00 dara/core/internal/pool/definitions.py
+-rw-r--r--  2.0 unx    17452 b- defN 80-Jan-01 00:00 dara/core/internal/pool/task_pool.py
+-rw-r--r--  2.0 unx     5230 b- defN 80-Jan-01 00:00 dara/core/internal/pool/utils.py
+-rw-r--r--  2.0 unx     6778 b- defN 80-Jan-01 00:00 dara/core/internal/pool/worker.py
+-rw-r--r--  2.0 unx     1655 b- defN 80-Jan-01 00:00 dara/core/internal/port_utils.py
+-rw-r--r--  2.0 unx     2435 b- defN 80-Jan-01 00:00 dara/core/internal/registries.py
+-rw-r--r--  2.0 unx     3610 b- defN 80-Jan-01 00:00 dara/core/internal/registry.py
+-rw-r--r--  2.0 unx    19385 b- defN 80-Jan-01 00:00 dara/core/internal/routing.py
+-rw-r--r--  2.0 unx    12906 b- defN 80-Jan-01 00:00 dara/core/internal/scheduler.py
+-rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 dara/core/internal/settings.py
+-rw-r--r--  2.0 unx    10656 b- defN 80-Jan-01 00:00 dara/core/internal/store.py
+-rw-r--r--  2.0 unx    24524 b- defN 80-Jan-01 00:00 dara/core/internal/tasks.py
+-rw-r--r--  2.0 unx     4406 b- defN 80-Jan-01 00:00 dara/core/internal/utils.py
+-rw-r--r--  2.0 unx     9539 b- defN 80-Jan-01 00:00 dara/core/internal/websocket.py
+-rw-r--r--  2.0 unx      726 b- defN 80-Jan-01 00:00 dara/core/jinja/index.html
+-rw-r--r--  2.0 unx     1253 b- defN 80-Jan-01 00:00 dara/core/jinja/index_autojs.html
+-rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 dara/core/js_tooling/custom_js_scaffold/index.tsx
+-rw-r--r--  2.0 unx      676 b- defN 80-Jan-01 00:00 dara/core/js_tooling/custom_js_scaffold/local-js-component.tsx
+-rw-r--r--  2.0 unx    22612 b- defN 80-Jan-01 00:00 dara/core/js_tooling/js_utils.py
+-rw-r--r--  2.0 unx    47068 b- defN 80-Jan-01 00:00 dara/core/js_tooling/statics/favicon.ico
+-rw-r--r--  2.0 unx      446 b- defN 80-Jan-01 00:00 dara/core/js_tooling/statics/tsconfig.json
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 dara/core/js_tooling/templates/.npmrc
+-rw-r--r--  2.0 unx      161 b- defN 80-Jan-01 00:00 dara/core/js_tooling/templates/_entry.template.tsx
+-rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 dara/core/js_tooling/templates/_entry_autojs.template.tsx
+-rw-r--r--  2.0 unx       84 b- defN 80-Jan-01 00:00 dara/core/js_tooling/templates/cldp.config.json
+-rw-r--r--  2.0 unx      538 b- defN 80-Jan-01 00:00 dara/core/js_tooling/templates/vite.config.template.ts
+-rw-r--r--  2.0 unx      706 b- defN 80-Jan-01 00:00 dara/core/log_configs/logging.yaml
+-rw-r--r--  2.0 unx    13093 b- defN 80-Jan-01 00:00 dara/core/logging.py
+-rw-r--r--  2.0 unx    16787 b- defN 80-Jan-01 00:00 dara/core/main.py
+-rw-r--r--  2.0 unx      823 b- defN 80-Jan-01 00:00 dara/core/metrics/__init__.py
+-rw-r--r--  2.0 unx     2580 b- defN 80-Jan-01 00:00 dara/core/metrics/cache.py
+-rw-r--r--  2.0 unx     1833 b- defN 80-Jan-01 00:00 dara/core/metrics/runtime.py
+-rw-r--r--  2.0 unx     2231 b- defN 80-Jan-01 00:00 dara/core/metrics/utils.py
+-rw-r--r--  2.0 unx  4287787 b- defN 80-Jan-01 00:00 dara/core/umd/dara.core.umd.js
+-rw-r--r--  2.0 unx  4082283 b- defN 80-Jan-01 00:00 dara/core/umd/style.css
+-rw-r--r--  2.0 unx      577 b- defN 80-Jan-01 00:00 dara/core/visual/__init__.py
+-rw-r--r--  2.0 unx     1652 b- defN 80-Jan-01 00:00 dara/core/visual/components/__init__.py
+-rw-r--r--  2.0 unx     3378 b- defN 80-Jan-01 00:00 dara/core/visual/components/fallback.py
+-rw-r--r--  2.0 unx     6600 b- defN 80-Jan-01 00:00 dara/core/visual/components/for_cmp.py
+-rw-r--r--  2.0 unx      866 b- defN 80-Jan-01 00:00 dara/core/visual/components/invalid_component.py
+-rw-r--r--  2.0 unx      893 b- defN 80-Jan-01 00:00 dara/core/visual/components/menu.py
+-rw-r--r--  2.0 unx     1669 b- defN 80-Jan-01 00:00 dara/core/visual/components/progress_tracker.py
+-rw-r--r--  2.0 unx      886 b- defN 80-Jan-01 00:00 dara/core/visual/components/raw_string.py
+-rw-r--r--  2.0 unx      943 b- defN 80-Jan-01 00:00 dara/core/visual/components/router_content.py
+-rw-r--r--  2.0 unx     1207 b- defN 80-Jan-01 00:00 dara/core/visual/components/sidebar_frame.py
+-rw-r--r--  2.0 unx     1220 b- defN 80-Jan-01 00:00 dara/core/visual/components/topbar_frame.py
+-rw-r--r--  2.0 unx      686 b- defN 80-Jan-01 00:00 dara/core/visual/components/types.py
+-rw-r--r--  2.0 unx    43028 b- defN 80-Jan-01 00:00 dara/core/visual/css/Property.py
+-rw-r--r--  2.0 unx   367298 b- defN 80-Jan-01 00:00 dara/core/visual/css/__init__.py
+-rw-r--r--  2.0 unx    13460 b- defN 80-Jan-01 00:00 dara/core/visual/dynamic_component.py
+-rw-r--r--  2.0 unx     5840 b- defN 80-Jan-01 00:00 dara/core/visual/progress_updater.py
+-rw-r--r--  2.0 unx     5794 b- defN 80-Jan-01 00:00 dara/core/visual/template.py
+-rw-r--r--  2.0 unx      794 b- defN 80-Jan-01 00:00 dara/core/visual/themes/__init__.py
+-rw-r--r--  2.0 unx     1942 b- defN 80-Jan-01 00:00 dara/core/visual/themes/dark.py
+-rw-r--r--  2.0 unx     2744 b- defN 80-Jan-01 00:00 dara/core/visual/themes/definitions.py
+-rw-r--r--  2.0 unx     1944 b- defN 80-Jan-01 00:00 dara/core/visual/themes/light.py
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_core-1.0.0a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1741 b- defN 80-Jan-01 00:00 dara_core-1.0.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_core-1.0.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 dara_core-1.0.0a1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     9105 b- defN 16-Jan-01 00:00 dara_core-1.0.0a1.dist-info/RECORD
+101 files, 9323718 bytes uncompressed, 3200069 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,19 +1,304 @@
-Filename: dara/core/logo.py
+Filename: dara/core/__init__.py
+Comment: 
+
+Filename: dara/core/actions.py
+Comment: 
+
+Filename: dara/core/auth/__init__.py
+Comment: 
+
+Filename: dara/core/auth/base.py
+Comment: 
+
+Filename: dara/core/auth/basic.py
+Comment: 
+
+Filename: dara/core/auth/definitions.py
+Comment: 
+
+Filename: dara/core/auth/routes.py
+Comment: 
+
+Filename: dara/core/auth/utils.py
+Comment: 
+
+Filename: dara/core/base_definitions.py
+Comment: 
+
+Filename: dara/core/cli.py
+Comment: 
+
+Filename: dara/core/configuration.py
+Comment: 
+
+Filename: dara/core/css.py
+Comment: 
+
+Filename: dara/core/data_utils.py
+Comment: 
+
+Filename: dara/core/defaults.py
+Comment: 
+
+Filename: dara/core/definitions.py
+Comment: 
+
+Filename: dara/core/http.py
+Comment: 
+
+Filename: dara/core/interactivity/__init__.py
+Comment: 
+
+Filename: dara/core/interactivity/actions.py
+Comment: 
+
+Filename: dara/core/interactivity/any_data_variable.py
+Comment: 
+
+Filename: dara/core/interactivity/any_variable.py
+Comment: 
+
+Filename: dara/core/interactivity/condition.py
+Comment: 
+
+Filename: dara/core/interactivity/data_variable.py
+Comment: 
+
+Filename: dara/core/interactivity/derived_data_variable.py
+Comment: 
+
+Filename: dara/core/interactivity/derived_variable.py
+Comment: 
+
+Filename: dara/core/interactivity/filtering.py
+Comment: 
+
+Filename: dara/core/interactivity/non_data_variable.py
+Comment: 
+
+Filename: dara/core/interactivity/plain_variable.py
+Comment: 
+
+Filename: dara/core/interactivity/url_variable.py
+Comment: 
+
+Filename: dara/core/internal/__init__.py
+Comment: 
+
+Filename: dara/core/internal/cgroup.py
+Comment: 
+
+Filename: dara/core/internal/dependency_resolution.py
+Comment: 
+
+Filename: dara/core/internal/devtools.py
+Comment: 
+
+Filename: dara/core/internal/download.py
+Comment: 
+
+Filename: dara/core/internal/execute_action.py
+Comment: 
+
+Filename: dara/core/internal/hashing.py
+Comment: 
+
+Filename: dara/core/internal/import_discovery.py
+Comment: 
+
+Filename: dara/core/internal/normalization.py
+Comment: 
+
+Filename: dara/core/internal/pandas_utils.py
+Comment: 
+
+Filename: dara/core/internal/pool/__init__.py
+Comment: 
+
+Filename: dara/core/internal/pool/channel.py
+Comment: 
+
+Filename: dara/core/internal/pool/definitions.py
+Comment: 
+
+Filename: dara/core/internal/pool/task_pool.py
+Comment: 
+
+Filename: dara/core/internal/pool/utils.py
+Comment: 
+
+Filename: dara/core/internal/pool/worker.py
+Comment: 
+
+Filename: dara/core/internal/port_utils.py
+Comment: 
+
+Filename: dara/core/internal/registries.py
+Comment: 
+
+Filename: dara/core/internal/registry.py
+Comment: 
+
+Filename: dara/core/internal/routing.py
+Comment: 
+
+Filename: dara/core/internal/scheduler.py
+Comment: 
+
+Filename: dara/core/internal/settings.py
+Comment: 
+
+Filename: dara/core/internal/store.py
+Comment: 
+
+Filename: dara/core/internal/tasks.py
+Comment: 
+
+Filename: dara/core/internal/utils.py
+Comment: 
+
+Filename: dara/core/internal/websocket.py
+Comment: 
+
+Filename: dara/core/jinja/index.html
+Comment: 
+
+Filename: dara/core/jinja/index_autojs.html
+Comment: 
+
+Filename: dara/core/js_tooling/custom_js_scaffold/index.tsx
+Comment: 
+
+Filename: dara/core/js_tooling/custom_js_scaffold/local-js-component.tsx
+Comment: 
+
+Filename: dara/core/js_tooling/js_utils.py
+Comment: 
+
+Filename: dara/core/js_tooling/statics/favicon.ico
+Comment: 
+
+Filename: dara/core/js_tooling/statics/tsconfig.json
+Comment: 
+
+Filename: dara/core/js_tooling/templates/.npmrc
+Comment: 
+
+Filename: dara/core/js_tooling/templates/_entry.template.tsx
+Comment: 
+
+Filename: dara/core/js_tooling/templates/_entry_autojs.template.tsx
+Comment: 
+
+Filename: dara/core/js_tooling/templates/cldp.config.json
+Comment: 
+
+Filename: dara/core/js_tooling/templates/vite.config.template.ts
+Comment: 
+
+Filename: dara/core/log_configs/logging.yaml
+Comment: 
+
+Filename: dara/core/logging.py
 Comment: 
 
 Filename: dara/core/main.py
 Comment: 
 
-Filename: dara_core-0.0.1.dist-info/WHEEL
+Filename: dara/core/metrics/__init__.py
+Comment: 
+
+Filename: dara/core/metrics/cache.py
+Comment: 
+
+Filename: dara/core/metrics/runtime.py
+Comment: 
+
+Filename: dara/core/metrics/utils.py
+Comment: 
+
+Filename: dara/core/umd/dara.core.umd.js
+Comment: 
+
+Filename: dara/core/umd/style.css
+Comment: 
+
+Filename: dara/core/visual/__init__.py
+Comment: 
+
+Filename: dara/core/visual/components/__init__.py
+Comment: 
+
+Filename: dara/core/visual/components/fallback.py
+Comment: 
+
+Filename: dara/core/visual/components/for_cmp.py
+Comment: 
+
+Filename: dara/core/visual/components/invalid_component.py
+Comment: 
+
+Filename: dara/core/visual/components/menu.py
+Comment: 
+
+Filename: dara/core/visual/components/progress_tracker.py
+Comment: 
+
+Filename: dara/core/visual/components/raw_string.py
+Comment: 
+
+Filename: dara/core/visual/components/router_content.py
+Comment: 
+
+Filename: dara/core/visual/components/sidebar_frame.py
+Comment: 
+
+Filename: dara/core/visual/components/topbar_frame.py
+Comment: 
+
+Filename: dara/core/visual/components/types.py
+Comment: 
+
+Filename: dara/core/visual/css/Property.py
+Comment: 
+
+Filename: dara/core/visual/css/__init__.py
+Comment: 
+
+Filename: dara/core/visual/dynamic_component.py
+Comment: 
+
+Filename: dara/core/visual/progress_updater.py
+Comment: 
+
+Filename: dara/core/visual/template.py
+Comment: 
+
+Filename: dara/core/visual/themes/__init__.py
+Comment: 
+
+Filename: dara/core/visual/themes/dark.py
+Comment: 
+
+Filename: dara/core/visual/themes/definitions.py
+Comment: 
+
+Filename: dara/core/visual/themes/light.py
+Comment: 
+
+Filename: dara_core-1.0.0a1.dist-info/LICENSE
+Comment: 
+
+Filename: dara_core-1.0.0a1.dist-info/METADATA
 Comment: 
 
-Filename: dara_core-0.0.1.dist-info/entry_points.txt
+Filename: dara_core-1.0.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: dara_core-0.0.1.dist-info/METADATA
+Filename: dara_core-1.0.0a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: dara_core-0.0.1.dist-info/RECORD
+Filename: dara_core-1.0.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dara/core/main.py

```diff
@@ -1,7 +1,411 @@
-from dara.core.logo import LOGO
+"""
+Copyright 2023 Impulse Innovations Limited
 
-def main():
-    print(LOGO)
 
-if __name__ == '__main__':
-    main()
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+import asyncio
+import os
+import sys
+from concurrent.futures import ThreadPoolExecutor
+from contextlib import asynccontextmanager
+from importlib.util import find_spec
+from pathlib import Path
+from typing import Optional
+
+from anyio import create_task_group
+from fastapi import FastAPI, HTTPException, Request
+from fastapi.responses import HTMLResponse
+from fastapi.staticfiles import StaticFiles
+from prometheus_client import start_http_server
+from starlette.templating import Jinja2Templates, _TemplateResponse
+
+from dara.core.auth import auth_router
+from dara.core.configuration import Configuration, ConfigurationBuilder
+from dara.core.defaults import (
+    blank_template,
+    default_template,
+    top_menu_template,
+    top_template,
+)
+from dara.core.internal.cgroup import get_cpu_count, set_memory_limit
+from dara.core.internal.devtools import send_error_for_session
+from dara.core.internal.pool import TaskPool
+from dara.core.internal.registries import (
+    action_def_registry,
+    auth_registry,
+    component_registry,
+    config_registry,
+    latest_value_registry,
+    sessions_registry,
+    template_registry,
+    utils_registry,
+    websocket_registry,
+)
+from dara.core.internal.routing import create_router, error_decorator
+from dara.core.internal.settings import get_settings
+from dara.core.internal.store import Store
+from dara.core.internal.tasks import TaskManager
+from dara.core.internal.utils import enforce_sso, import_config
+from dara.core.internal.websocket import WebsocketManager
+from dara.core.js_tooling.js_utils import (
+    BuildMode,
+    build_autojs_template,
+    get_build_config,
+    rebuild_js,
+    require_js_build,
+)
+from dara.core.logging import LoggingMiddleware, dev_logger, eng_logger, http_logger
+
+
+def _start_application(config: Configuration):
+    """
+    Helper to start the application with a config passed. This is split out from main so that it can be used directly
+    for testing purposes.
+
+    :param config: the app configuration
+    """
+    # Clear env cache in case we're re-running the app and get_settings was called too early
+    get_settings.cache_clear()
+
+    # Check we have a config
+    if isinstance(config, Configuration) is False:
+        raise ValueError('Invalid Configuration class passed to Dara Core. Did you forget to call _to_configuration()?')
+
+    # Setup the main template to work with Vite
+    os.environ['VITE_MANIFEST_PATH'] = f'{config.static_files_dir}/manifest.json'
+    import fastapi_vite
+
+    if len(config.pages) > 0:
+        BASE_DIR = Path(__file__).parent
+        jinja_templates = Jinja2Templates(directory=str((Path(BASE_DIR, 'jinja'))))
+        jinja_templates.env.globals['vite_hmr_client'] = fastapi_vite.vite_hmr_client
+        jinja_templates.env.globals['vite_asset'] = fastapi_vite.vite_asset
+        jinja_templates.env.globals['entry'] = '_entry.tsx'
+
+        # If dev mode enabled, set live reload to true
+        if os.environ.get('VITE_SERVE_MODE') or os.environ.get('DARA_LIVE_RELOAD'):
+            config.live_reload = True
+
+    # Configure the default executor for threads run via the async loop
+    loop = asyncio.get_event_loop()
+    loop.set_default_executor(ThreadPoolExecutor(max_workers=int(os.environ.get('DARA_NUM_COMPONENT_THREADS', 8))))
+
+    is_production = os.environ.get('DARA_DOCKER_MODE') == 'TRUE'
+
+    # Setup registries:
+    # 1) cleanup ones which store results etc so if Dara is ran in a thread and restarted we get a fresh state
+    # 2) cleanup utils registry so we get a fresh set of internals
+    # We're explicitly not cleaning up components etc as components are registered beforehand
+    # so cleaning them up here would result in an error
+    latest_value_registry.replace({}, deepcopy=False)
+    websocket_registry.replace({}, deepcopy=False)
+    sessions_registry.replace({}, deepcopy=False)
+    config_registry.replace({}, deepcopy=False)
+
+    @asynccontextmanager
+    async def lifespan(app: FastAPI):
+        # STARTUP
+
+        # Retrieve the existing Store instance for the application
+        # Store must exist before the app starts as instantiating e.g. Variables
+        # requires a store existing
+        store: Store = utils_registry.get('Store')
+
+        # Create a task group for the application so we can kick off tasks in the background
+        async with create_task_group() as task_group:
+            ws_manager = WebsocketManager()
+            task_manager = TaskManager(task_group, ws_manager, store)
+
+            # Add other internals
+            utils_registry.set('TaskGroup', task_group)
+            utils_registry.set('WebsocketManager', ws_manager)
+            utils_registry.set('TaskManager', task_manager)
+
+            utils_registry.set('TaskPool', None)
+
+            task_pool: Optional[TaskPool] = None
+
+            # Only initialize the pool if a task module is configured
+            if config.task_module:
+                # Verify task module exists
+                task_module_spec = find_spec(config.task_module)
+                if task_module_spec is None or not task_module_spec.name.endswith('.tasks'):
+                    raise RuntimeError(
+                        f'Task module {config.task_module} does not exist or is invalid. Set config.task_module path to a tasks.py module'
+                    )
+
+                # Default to number of CPUs - 1 (with minimum of 1)
+                cpu_count = get_cpu_count()
+                max_workers = int(os.environ.get('DARA_POOL_MAX_WORKERS', max(1, cpu_count - 1)))
+                dev_logger.info(
+                    'Initializing task pool...',
+                    {
+                        'max_workers': max_workers,
+                        'task_module': config.task_module,
+                    },
+                )
+                task_pool = TaskPool(
+                    task_group=task_group,
+                    worker_parameters={'task_module': config.task_module},
+                    max_workers=max_workers,
+                )
+                await task_pool.start(60)   # timeout after 60s
+                utils_registry.set('TaskPool', task_pool)
+                dev_logger.info('Task pool initialized')
+
+            # Yield back to the app
+            yield
+
+            # SHUTDOWN
+            eng_logger.debug('App shutting down, attempting to cancel all tasks and shut down the task pool')
+            await task_manager.cancel_all_tasks()
+
+            if task_pool is not None:
+                eng_logger.debug('Shutting down task pool...')
+                await task_pool.join(5)
+                eng_logger.debug('Task pool shut down')
+
+    app = FastAPI(
+        lifespan=lifespan, docs_url=None if is_production else '/docs', redoc_url=None if is_production else '/redoc'
+    )
+
+    # Define catch-all mechanisms
+    @app.middleware('http')
+    async def catchall_middleware(req: Request, call_next):
+        try:
+            return await call_next(req)
+        except Exception as e:
+            try:
+                ws_mgr: WebsocketManager = utils_registry.get('WebsocketManager')
+                session_id = req.state.session_id
+                await send_error_for_session(ws_mgr, session_id)
+            except AttributeError:
+                # i.e. unauthenticated endpoint
+                eng_logger.debug('Error could not be sent as no session was found in the request state')
+            raise e
+
+    # Setup http logger
+    if os.environ.get('DARA_TEST_FLAG', None) is None:
+        app.add_middleware(LoggingMiddleware, logger=http_logger)
+
+    # Loop over scheduled jobs and start them
+    eng_logger.info(f'Starting {len(config.scheduled_jobs)} local scheduled jobs')
+    for job, func, args in config.scheduled_jobs:
+        job.do(func, args)
+
+    route_urls = [f'"/api/{route.url}"' for route in config.routes]
+    eng_logger.info(f'Registering local routes [{", ".join(route_urls)}]')
+
+    # Add endpoint configurations to registry
+    for conf in config.endpoint_configurations:
+        config_registry.register(conf.__class__.__name__, conf)
+
+    # Register collected endpoints
+    for route in config.routes:
+        clean_url = f'/api/{route.url}'.replace('//', '/')
+        app.add_api_route(
+            path=clean_url,
+            endpoint=error_decorator(route.handler),
+            dependencies=route.dependencies,
+            methods=[route.method.value],
+        )
+
+    # Check which JS build mode the app is ran in
+    build_config = get_build_config()
+
+    # Check if we need to build any JS
+    if len(config.pages) > 0 and require_js_build(config, build_config):
+        dev_logger.info('JS Requires a rebuild. Rebuilding...')
+        rebuild_js(config=config, build_config=build_config)
+        dev_logger.info('JS rebuilt successfully!')
+
+    # Loop over registered components and add to the registry
+    eng_logger.info(f'Registering components [{", ".join([c.name for c in config.components])}]')
+    for component in config.components:
+        component_registry.register(component.name, component)
+
+    # Loop over registered actions and add to the registry
+    eng_logger.info(f'Registering actions [{", ".join([a.name for a in config.actions])}]')
+    for action in config.actions:
+        action_def_registry.register(action.name, action)
+
+    dev_logger.info(f'Using {config.auth_config.__class__.__name__} auth configuration')
+    auth_registry.register('auth_config', config.auth_config)
+
+    try:
+        eng_logger.info('Registering template')
+
+        # Add the default templates
+        if config.template == 'default':
+            eng_logger.info('Registering template "default"')
+            template_registry.register('default', default_template(config))
+        elif config.template == 'blank':
+            eng_logger.info('Registering template "blank"')
+            template_registry.register('blank', blank_template(config))
+        elif config.template == 'top':
+            eng_logger.info('Registering template "top"')
+            template_registry.register('top', top_template(config))
+        elif config.template == 'top-menu':
+            eng_logger.info('Registering template "top-menu"')
+            template_registry.register('top-menu', top_menu_template(config))
+        else:
+            # Loop over user defined templates and add to the registry
+            for name, renderer in config.template_renderers.items():
+                if name == config.template:
+                    eng_logger.info(f'Registering custom template "{name}"')
+                    template_registry.register(name, renderer(config))
+
+    except Exception as e:
+        dev_logger.error(
+            'Something went wrong when building application template, there is most likely an issue in the application logic',
+            e,
+        )
+        sys.exit(1)
+
+    # Root routes
+
+    @app.get('/status')
+    async def status():
+        """
+        Used by liveness probes to check application responds to HTTP requests
+        """
+        return {'status': 'ok'}
+
+    # Register the core routes of the application
+    core_api_router = create_router(config)
+
+    # Start metrics server in a daemon thread
+    if os.environ.get('DARA_DISABLE_METRICS') != 'TRUE' and os.environ.get('DARA_TEST_FLAG', None) is None:
+        port = int(os.environ.get('DARA_METRICS_PORT', 10000))
+        start_http_server(port)
+
+    # Start profiling server in a daemon thread if explicitly enabled (only works on linux)
+    if os.environ.get('DARA_PYPPROF_PORT', None) is not None:
+        profiling_port = int(os.environ.get('DARA_PYPPROF_PORT', 10001))
+        dev_logger.warning('Starting cpu/memory profiling server', extra={'port': profiling_port})
+
+        from pypprof.net_http import start_pprof_server
+
+        start_pprof_server(port=profiling_port)
+
+    # Serve statics, only if we have any pages defined
+    if len(config.pages) > 0:
+        app.mount('/static', StaticFiles(directory=config.static_files_dir), name='static')
+
+    # Mount Routers
+    app.include_router(auth_router, prefix='/api/auth')
+    app.include_router(core_api_router, prefix='/api/core')
+
+    @app.get('/api/{rest_of_path:path}')
+    async def not_found():  # pylint: disable=unused-variable
+        raise HTTPException(status_code=404, detail='API endpoint not found')
+
+    if len(config.pages) > 0:
+        dev_logger.info(f'Registering pages: [{", ".join(list(config.pages.keys()))}]')
+        # For any unmatched route then serve the app to the user if we have any pages to serve
+        # (Required for the chosen routing system in the UI)
+
+        # Auto-js mode - serve the built template with UMDs
+        if build_config.mode == BuildMode.AUTO_JS:
+            # Load template
+            with open(os.path.join(Path(BASE_DIR, 'jinja'), 'index_autojs.html'), 'r', encoding='utf-8') as fp:
+                template = fp.read()
+
+            # Generate tags for the template
+            template = build_autojs_template(template, config)
+
+            @app.get('/{full_path:path}', include_in_schema=False, response_class=HTMLResponse)
+            async def serve_app(request: Request):  # pylint: disable=unused-variable
+                return HTMLResponse(template)
+
+        else:
+            # Otherwise serve the Vite template
+
+            @app.get('/{full_path:path}', include_in_schema=False, response_class=_TemplateResponse)
+            async def serve_app(request: Request):  # pylint: disable=unused-variable
+                return jinja_templates.TemplateResponse('index.html', {'request': request})
+
+    # App is now ready, call user-defined startup functions
+    eng_logger.info(f'Running {len(config.startup_functions)} local startup functions')
+    for startup_function in config.startup_functions:
+        startup_function()
+
+    return app
+
+
+def main(extra=None):
+    """
+    Deprecated since v1.12.4
+
+    Dara applications should not call main directly as the CLI automatically picks up `config` from the entry file
+    """
+    print(
+        'Call to deprecated function `main` detected. Your application should not call the main function directly, please remove any calls to `main` from your code.'
+    )
+    sys.exit(1)
+
+
+def start(extra=None):
+    """
+    The start function reads the Configuration for an application from DARA_CONFIG_PATH env var
+    and creates an ASGI instance of FastAPI to serve the app. See the project docs for more
+    details
+
+    Note: start takes an extra param in case `uvicorn` passes extra data here. It's not currently used but
+    it's necessary to prevent errors such as `start() takes 0 positional arguments but 1 was given` happening
+    which prevent real errors from showing up in the console.
+    """
+    # Set debug logging level based on the environment variable set by CLI
+    debug_level = os.environ.get('DARA_DEBUG_LOG_LEVEL', 'NONE')
+    if debug_level != 'NONE':
+        eng_logger._logger.setLevel(debug_level)
+
+        # In DEBUG mode also enable detailed http logs
+        if debug_level == 'DEBUG':
+            http_logger._logger.setLevel('DEBUG')
+    else:
+        eng_logger._logger.disabled = True
+
+    # Set dev logging level based on the environment variable set by CLI
+    dev_level = os.environ.get('DARA_DEV_LOG_LEVEL', 'NONE')
+    if dev_level != 'NONE':
+        dev_logger._logger.setLevel(dev_level)
+    else:
+        dev_logger._logger.setLevel('INFO')
+
+    # First load the configuration based on the environment variable
+    config_path = os.environ.get('DARA_CONFIG_PATH')
+    dev_logger.info(f'Loading configuration from {config_path}')
+
+    if config_path is None:
+        raise ValueError(
+            'Missing config path. Please start the application via the cli or set the DARA_CONFIG_PATH env var'
+        )
+
+    if get_settings().cgroup_memory_limit_enabled:
+        set_memory_limit()
+
+    config_module, config = import_config(config_path)
+
+    if not isinstance(config, ConfigurationBuilder):
+        raise ValueError(f'"config" object in {config_path} is not an instance of ConfigurationBuilder')
+
+    # Enforce SSO at this point - this runs on each reload
+    if os.environ.get('DARA_ENFORCE_SSO') == 'TRUE':
+        enforce_sso(config)
+
+    config._run_discovery(config_module)
+
+    return _start_application(config=config._to_configuration())
```

