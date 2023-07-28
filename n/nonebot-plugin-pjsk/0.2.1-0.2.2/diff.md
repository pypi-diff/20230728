# Comparing `tmp/nonebot_plugin_pjsk-0.2.1.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.1.tar", last modified: Wed Jul 26 16:22:00 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.2.tar", last modified: Fri Jul 28 16:21:00 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.1.tar` & `nonebot_plugin_pjsk-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-26 16:21:44.002201 nonebot_plugin_pjsk-0.2.1/LICENSE
--rw-r--r--   0        0        0     3412 2023-07-26 16:21:44.002201 nonebot_plugin_pjsk-0.2.1/README.md
--rw-r--r--   0        0        0      801 2023-07-26 16:21:44.062201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     6591 2023-07-26 16:21:44.062201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0      695 2023-07-26 16:21:44.062201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0     6407 2023-07-26 16:21:44.066201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     3553 2023-07-26 16:21:44.066201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2423 2023-07-26 16:21:44.066201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1086 2023-07-26 16:22:00.370602 nonebot_plugin_pjsk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-28 16:20:41.039194 nonebot_plugin_pjsk-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3764 2023-07-28 16:20:41.039194 nonebot_plugin_pjsk-0.2.2/README.md
+-rw-r--r--   0        0        0      889 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     7573 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0     1076 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0     7535 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     4002 2023-07-28 16:20:41.115195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2351 2023-07-28 16:20:41.119195 nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1811 2023-07-28 16:21:00.639484 nonebot_plugin_pjsk-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.1/LICENSE` & `nonebot_plugin_pjsk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.1/README.md` & `nonebot_plugin_pjsk-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
+<!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
@@ -10,15 +10,15 @@
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-PJSK
 
 _✨ Project Sekai 表情包制作 ✨_
 
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 <a href="https://pdm.fming.dev">
   <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
   <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange" alt="QQ Chat Group">
 </a>
 
@@ -34,14 +34,16 @@
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-pjsk" alt="pypi download">
 </a>
 
 </div>
 
 ## 📖 介绍
 
+### Wonderhoy!
+
 ![Wonderhoy](./readme/wonderhoy.png)
 
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
@@ -105,20 +107,28 @@
 
 ## ⚙️ 配置
 
 插件有配置项，但是一般情况下无需更改，请自行查看 [config.py](./nonebot_plugin_pjsk/config.py) 文件
 
 ## 🎉 使用
 
-使用指令 `pjsk -h` 查看插件帮助
+直接使用指令 `pjsk` 进入交互创建模式；  
+使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助
 
 ### 效果图
 
 <details>
-<summary>点击展开</summary>
+<summary>使用交互创建模式</summary>
+
+![example](./readme/example-interact.png)
+
+</details>
+
+<details>
+<summary>使用 Shell-Like 指令</summary>
 
 ![example](./readme/example.png)
 
 </details>
 
 ## 🙈 碎碎念
 
@@ -136,8 +146,19 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.2.2
+
+- 修改了 0.2.1 版的交互创建模式的触发方式
+- 试验性地支持了 Emoji
+
+### 0.2.1
+
+- 更改指令 `pjsk列表` 的交互方式
+
+### 0.2.0
+
+- 重构插件
```

#### html2text {}

```diff
@@ -1,31 +1,36 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» ![Wonderhoy](./readme/wonderhoy.png) ## ð¿ å®è£
-ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
-å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+## ð ä»ç» ### Wonderhoy! ![Wonderhoy](./readme/wonderhoy.png) ## ð¿
+å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
+å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-pjsk
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_pjsk" ] ```  ## âï¸ éç½®
 æä»¶æéç½®é¡¹ï¼ä½æ¯ä¸è¬æåµä¸æ éæ´æ¹ï¼è¯·èªè¡æ¥ç
-[config.py](./nonebot_plugin_pjsk/config.py) æä»¶ ## ð ä½¿ç¨ ä½¿ç¨æä»¤
-`pjsk -h` æ¥çæä»¶å¸®å© ### ææå¾  ç¹å»å±å¼ ![example](./readme/
-example.png)  ## ð ç¢ç¢å¿µ - ~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
+[config.py](./nonebot_plugin_pjsk/config.py) æä»¶ ## ð ä½¿ç¨
+ç´æ¥ä½¿ç¨æä»¤ `pjsk` è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h`
+äºè§£ä½¿ç¨ Shell-Like æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾
+ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example](./readme/example-interact.png)   ä½¿ç¨
+Shell-Like æä»¤ ![example](./readme/example.png)  ## ð ç¢ç¢å¿µ -
+~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
 å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æ issue æè [å ç¾¤](https://
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.2
+- ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
+è¯éªæ§å°æ¯æäº Emoji ### 0.2.1 - æ´æ¹æä»¤ `pjskåè¡¨`
+çäº¤äºæ¹å¼ ### 0.2.0 - éææä»¶
```

### Comparing `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __plugin_meta__ = PluginMetadata(
     name="Sekai Stickers",
     description="基于 NoneBot2 的 Project Sekai 表情包制作插件",
-    usage="使用指令 `pjsk -h` 获取指令帮助",
+    usage="直接使用指令 `pjsk` 进入交互创建模式；\n使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     config=ConfigModel,
     supported_adapters={
         "~onebot.v11",
         "~onebot.v12",
         "~kaiheila",
```

### Comparing `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+from imagetext_py import EmojiSource
 from nonebot import get_driver
 from pydantic import BaseModel, validator
 
 
 class ConfigModel(BaseModel):
     pjsk_assets_prefix: str = (
         "https://raw.gitmirror.com/TheOriginalAyaka/sekai-stickers/main/"
     )
-    pjsk_repo_prefix: str = (
-        "https://raw.gitmirror.com/Agnes4m/nonebot_plugin_pjsk/main/"
-    )
+    pjsk_repo_prefix: str = "https://raw.gitmirror.com/Agnes4m/nonebot_plugin_pjsk/main/"
+
+    pjsk_emoji_source: str = "Apple"
+    """Emoji 来源，可选值见 https://github.com/nathanielfernandes/imagetext-py/blob/master/imagetext_py/imagetext_py.pyi#L217"""
 
     @validator("pjsk_assets_prefix", "pjsk_repo_prefix")
     def check_url(cls, v):  # noqa: N805
         if not v.startswith(("http://", "https://")):
             raise ValueError("URL must start with http:// or https://")
         if not v.endswith("/"):
             v = f"{v}/"
         return v
 
+    @validator("pjsk_emoji_source")
+    def check_emoji_source(cls, v):  # noqa: N805
+        if not getattr(EmojiSource, v, None):
+            raise ValueError("Invalid emoji source")
+
 
 config: ConfigModel = ConfigModel.parse_obj(get_driver().config.dict())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/draw.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 import asyncio
+from functools import partial
 from io import BytesIO
-from typing import Any, Awaitable, Callable, Coroutine, Dict, List, Optional, overload
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Coroutine,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    overload,
+)
+from typing_extensions import ParamSpec
 
 import anyio
 from imagetext_py import (
     Canvas,
     Color,
+    EmojiOptions,
+    EmojiSource,
     Font,
     Paint,
     TextAlign,
     draw_text_multiline,
     text_size_multiline,
 )
 from numpy import rad2deg
 from PIL import Image
 from pil_utils import BuildImage
 from pil_utils.types import ColorType
-from typing_extensions import ParamSpec
 
+from .config import config
 from .resource import (
     CACHE_FOLDER,
     FONT_PATHS,
     LOADED_STICKER_INFO,
     RESOURCE_FOLDER,
     StickerInfo,
 )
@@ -36,59 +50,78 @@
 DEFAULT_STROKE_WIDTH = 9
 DEFAULT_LINE_SPACING = 1.3
 
 
 def ensure_font() -> Font:
     global FONT
     if not FONT:
-        FONT = Font(str(FONT_PATHS[0]), [str(x) for x in FONT_PATHS[1:]])
+        FONT = Font(
+            str(FONT_PATHS[0]),
+            [str(x) for x in FONT_PATHS[1:]],
+            emoji_options=EmojiOptions(
+                source=getattr(EmojiSource, config.pjsk_emoji_source),
+            ),
+        )
     return FONT
 
 
 def hex_to_color(hex_color: str) -> Color:
     if hex_color.startswith("#"):
         hex_color = hex_color[1:]
     return Color.from_hex(hex_color)
 
 
-def render_text(
+async def render_text(
     text: str,
     color: str,
     font_size: int,
     font_weight: int,
     stoke_width: int,
     line_spacing: float,
 ) -> Image.Image:
     font = ensure_font()
 
     text_lines = text.splitlines()
     padding = stoke_width
 
-    actual_size = text_size_multiline(text_lines, font_size, font, line_spacing)
+    actual_size = await anyio.to_thread.run_sync(
+        partial(
+            text_size_multiline,
+            lines=text_lines,
+            size=font_size,
+            font=font,
+            line_spacing=line_spacing,
+            draw_emojis=True,
+        ),
+    )
     size = (
         actual_size[0] + padding * 2,
         actual_size[1] + padding * 2 + font_size // 2,  # 更多纵向 padding 防止文字被裁
     )
 
     canvas = Canvas(*size, Color(255, 255, 255, 0))
-    draw_text_multiline(
-        canvas,
-        text_lines,  # type: ignore 这里是源代码有问题
-        size[0] // 2,
-        size[1] // 2,
-        0.5,
-        0.5,
-        font_weight,
-        font_size,
-        font,
-        Paint(hex_to_color(color)),
-        line_spacing,
-        TextAlign.Center,
-        stoke_width,  # type: ignore same
-        Paint(Color(255, 255, 255)),
+    await anyio.to_thread.run_sync(
+        partial(
+            draw_text_multiline,
+            canvas=canvas,
+            lines=text_lines,
+            x=size[0] // 2,
+            y=size[1] // 2,
+            ax=0.5,
+            ay=0.5,
+            width=font_weight,
+            size=font_size,
+            font=font,
+            fill=Paint(hex_to_color(color)),
+            line_spacing=line_spacing,
+            align=TextAlign.Center,
+            stroke=stoke_width,  # type: ignore 源码 type 有问题
+            stroke_color=Paint(Color(255, 255, 255)),
+            draw_emojis=True,
+        ),
     )
 
     return canvas.to_image().convert("RGBA")
 
 
 def paste_text_on_image(
     image: Image.Image,
@@ -124,15 +157,15 @@
     rotate: Optional[int] = None,
     font_size: Optional[int] = None,
     stroke_width: Optional[int] = None,
     line_spacing: Optional[float] = None,
     font_weight: Optional[int] = None,
 ) -> Image.Image:
     sticker_img = await anyio.Path(RESOURCE_FOLDER / info.img).read_bytes()
-    text_img = render_text(
+    text_img = await render_text(
         text or info.default_text.text,
         info.color,
         font_size or info.default_text.s,
         font_weight or DEFAULT_FONT_WEIGHT,
         stroke_width or DEFAULT_STROKE_WIDTH,
         line_spacing or DEFAULT_LINE_SPACING,
     )
@@ -167,40 +200,26 @@
             bg.paste(item, (x_offset, y_offset), item)
             x_offset += item.size[0] + padding
         y_offset += max([x.size[1] for x in line]) + padding
 
     return bg
 
 
-async def render_all_characters() -> Image.Image:
-    characters: Dict[str, StickerInfo] = {}
-    for info in LOADED_STICKER_INFO:
-        if info.character not in characters:
-            characters[info.character] = info
-
-    tasks: List[Coroutine[Any, Any, Image.Image]] = [
-        draw_sticker(info, info.character.capitalize()) for info in characters.values()
-    ]
-    images: List[Image.Image] = await asyncio.gather(*tasks)
-    return render_summary_picture(images)
-
-
-async def render_character_stickers(character: str) -> Optional[Image.Image]:
-    character = character.lower()
-
-    tasks: List[Coroutine[Any, Any, Image.Image]] = [
-        draw_sticker(info, info.sticker_id)
-        for info in LOADED_STICKER_INFO
-        if info.character.lower() == character
-    ]
-    if not tasks:
-        return None
-
-    images: List[Image.Image] = await asyncio.gather(*tasks)
-    return render_summary_picture(images)
+async def render_summary_from_tasks(
+    tasks: Iterable[Awaitable[Image.Image]],
+    padding: int = 15,
+    line_max: int = 5,
+    background: Optional[ColorType] = None,
+) -> Image.Image:
+    return render_summary_picture(
+        await asyncio.gather(*tasks),
+        padding,
+        line_max,
+        background,
+    )
 
 
 @overload
 def use_image_cache(
     func: Callable[P, Awaitable[Image.Image]],
     filename: str,
     image_format: str = "JPEG",
@@ -232,7 +251,35 @@
             return None
 
         image = i2b(raw_image, image_format)
         await path.write_bytes(image)
         return image
 
     return wrapper
+
+
+async def render_all_characters() -> Image.Image:
+    characters: Dict[str, StickerInfo] = {}
+    for info in LOADED_STICKER_INFO:
+        if info.character not in characters:
+            characters[info.character] = info
+    return await render_summary_from_tasks(
+        draw_sticker(info, info.character.capitalize()) for info in characters.values()
+    )
+
+
+async def get_all_characters() -> bytes:
+    return await use_image_cache(render_all_characters, "all_characters")()
+
+
+async def render_character_stickers(character: str) -> Optional[Image.Image]:
+    character = character.lower()
+    tasks: List[Coroutine[Any, Any, Image.Image]] = [
+        draw_sticker(info, info.sticker_id)
+        for info in LOADED_STICKER_INFO
+        if info.character.lower() == character
+    ]
+    return (await render_summary_from_tasks(tasks)) if tasks else None
+
+
+async def get_character_stickers(character: str) -> Optional[bytes]:
+    return await use_image_cache(render_character_stickers, character)(character)
```

### Comparing `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/resource.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
+import random
 import shutil
 from pathlib import Path
-from typing import Coroutine, List
+from typing import Coroutine, List, Optional, overload
 
 import anyio
-from loguru import logger
-from nonebot import get_driver
+from nonebot import get_driver, logger
 from pydantic import BaseModel, Field, parse_raw_as
 
 from .config import config
 from .utils import ResponseType, async_request, with_semaphore
 
 DATA_FOLDER = Path.cwd() / "data" / "pjsk"
 FONT_FOLDER = DATA_FOLDER / "fonts"
@@ -47,14 +47,32 @@
     color: str
     default_text: StickerText = Field(..., alias="defaultText")
 
 
 LOADED_STICKER_INFO: List[StickerInfo] = []
 
 
+@overload
+def select_or_get_random(sticker_id: None = None) -> StickerInfo:
+    ...
+
+
+@overload
+def select_or_get_random(sticker_id: str) -> Optional[StickerInfo]:
+    ...
+
+
+def select_or_get_random(sticker_id: Optional[str] = None) -> Optional[StickerInfo]:
+    return (
+        next((x for x in LOADED_STICKER_INFO if sticker_id == x.sticker_id), None)
+        if sticker_id
+        else random.choice(LOADED_STICKER_INFO)
+    )
+
+
 async def check_and_download_font():
     async def download(font_name: str):
         logger.opt(colors=True).info(f"Downloading font <y>{font_name}</y>")
         path = anyio.Path(FONT_FOLDER) / font_name
         await path.write_bytes(
             await async_request(f"fonts/{font_name}", prefix=config.pjsk_repo_prefix),
         )
```

### Comparing `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.2/nonebot_plugin_pjsk/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import math
 from asyncio import Semaphore
 from enum import Enum, auto
 from typing import Any, Iterable, List, Literal, Optional, Type, TypeVar, overload
 
 from httpx import AsyncClient
 
 from .config import config
@@ -68,18 +67,14 @@
                 return await func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
-def rad2deg(rad: float) -> float:
-    return rad * 180 / math.pi
-
-
 def split_list(li: Iterable[T], length: int) -> List[List[T]]:
     latest = []
     tmp = []
     for n, i in enumerate(li):
         tmp.append(i)
         if (n + 1) % length == 0:
             latest.append(tmp)
@@ -101,8 +96,8 @@
     if not value:
         return default
     try:
         if value.startswith("^"):
             return default + expected_type(value[1:])
         return expected_type(value)  # type: ignore pylance 抽风
     except Exception as e:
-        raise ResolveValueError from e
+        raise ResolveValueError(value) from e
```

### Comparing `nonebot_plugin_pjsk-0.2.1/pyproject.toml` & `nonebot_plugin_pjsk-0.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.1"
+version = "0.2.2"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
-    "nonebot-adapter-onebot>=2.2.0",
     "nonebot-plugin-send-anything-anywhere>=0.2.7",
-    "imagetext-py>=1.0.2",
+    "imagetext-py>=2.1.3",
     "pil-utils>=0.1.7",
+    "httpx>=0.24.1",
+    "numpy>=1.25.1",
+    "anyio>=3.7.1",
 ]
-requires-python = ">=3.8,<4.0"
+requires-python = ">=3.9,<4.0"
 keywords = [
     "pjsk",
     "nonebot2",
     "plugin",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -35,12 +37,73 @@
 
 [project.urls]
 homepage = "https://github.com/Agnes4m/nonebot_plugin_pjsk"
 
 [tool.pdm.build]
 includes = []
 
+[tool.pyright]
+pythonVersion = "3.8"
+
+[tool.black]
+line-length = 89
+target-version = [
+    "py39",
+    "py310",
+    "py311",
+]
+include = "\\.pyi?$"
+
+[tool.ruff]
+ignore = [
+    "B008",
+    "B905",
+    "E501",
+    "FBT002",
+    "PGH003",
+    "RUF001",
+    "RUF002",
+    "RUF003",
+    "RUF006",
+    "RUF100",
+    "SIM117",
+    "TRY002",
+    "TRY003",
+]
+select = [
+    "A",
+    "ARG",
+    "ASYNC",
+    "B",
+    "C4",
+    "COM",
+    "E",
+    "F",
+    "FBT",
+    "FLY",
+    "I",
+    "ISC",
+    "N",
+    "PIE",
+    "PGH",
+    "PTH",
+    "PYI",
+    "Q",
+    "RET",
+    "RSE",
+    "RUF",
+    "SIM",
+    "SLF",
+    "SLOT",
+    "TRY",
+]
+
+[tool.ruff.isort]
+extra-standard-library = [
+    "typing_extensions",
+]
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_pjsk-0.2.1/PKG-INFO` & `nonebot_plugin_pjsk-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk
-Requires-Python: <4.0,>=3.8
+Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.0.0
-Requires-Dist: nonebot-adapter-onebot>=2.2.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
-Requires-Dist: imagetext-py>=1.0.2
+Requires-Dist: imagetext-py>=2.1.3
 Requires-Dist: pil-utils>=0.1.7
+Requires-Dist: httpx>=0.24.1
+Requires-Dist: numpy>=1.25.1
+Requires-Dist: anyio>=3.7.1
 Description-Content-Type: text/markdown
 
-<!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
+<!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
@@ -34,15 +36,15 @@
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
 # NoneBot-Plugin-PJSK
 
 _✨ Project Sekai 表情包制作 ✨_
 
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 <a href="https://pdm.fming.dev">
   <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
   <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange" alt="QQ Chat Group">
 </a>
 
@@ -58,14 +60,16 @@
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-pjsk" alt="pypi download">
 </a>
 
 </div>
 
 ## 📖 介绍
 
+### Wonderhoy!
+
 ![Wonderhoy](./readme/wonderhoy.png)
 
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
@@ -129,20 +133,28 @@
 
 ## ⚙️ 配置
 
 插件有配置项，但是一般情况下无需更改，请自行查看 [config.py](./nonebot_plugin_pjsk/config.py) 文件
 
 ## 🎉 使用
 
-使用指令 `pjsk -h` 查看插件帮助
+直接使用指令 `pjsk` 进入交互创建模式；  
+使用指令 `pjsk -h` 了解使用 Shell-Like 指令创建表情的帮助
 
 ### 效果图
 
 <details>
-<summary>点击展开</summary>
+<summary>使用交互创建模式</summary>
+
+![example](./readme/example-interact.png)
+
+</details>
+
+<details>
+<summary>使用 Shell-Like 指令</summary>
 
 ![example](./readme/example.png)
 
 </details>
 
 ## 🙈 碎碎念
 
@@ -160,8 +172,19 @@
 
 感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
 - [爱发电](https://afdian.net/a/agnes_digital)
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.2.2
+
+- 修改了 0.2.1 版的交互创建模式的触发方式
+- 试验性地支持了 Emoji
+
+### 0.2.1
+
+- 更改指令 `pjsk列表` 的交互方式
+
+### 0.2.0
+
+- 重构插件
```

#### html2text {}

```diff
@@ -1,45 +1,50 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.1 Summary: Project
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.2 Summary: Project
 Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
 https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Project-URL:
 Homepage, https://github.com/Agnes4m/nonebot_plugin_pjsk Requires-Python:
-<4.0,>=3.8 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-
-onebot>=2.2.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
-Requires-Dist: imagetext-py>=1.0.2 Requires-Dist: pil-utils>=0.1.7 Description-
-Content-Type: text/markdown
+<4.0,>=3.9 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-
+anything-anywhere>=0.2.7 Requires-Dist: imagetext-py>=2.1.3 Requires-Dist: pil-
+utils>=0.1.7 Requires-Dist: httpx>=0.24.1 Requires-Dist: numpy>=1.25.1
+Requires-Dist: anyio>=3.7.1 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» ![Wonderhoy](./readme/wonderhoy.png) ## ð¿ å®è£
-ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
-å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+## ð ä»ç» ### Wonderhoy! ![Wonderhoy](./readme/wonderhoy.png) ## ð¿
+å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
+å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-pjsk
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
 ```bash conda install nonebot-plugin-pjsk ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_pjsk" ] ```  ## âï¸ éç½®
 æä»¶æéç½®é¡¹ï¼ä½æ¯ä¸è¬æåµä¸æ éæ´æ¹ï¼è¯·èªè¡æ¥ç
-[config.py](./nonebot_plugin_pjsk/config.py) æä»¶ ## ð ä½¿ç¨ ä½¿ç¨æä»¤
-`pjsk -h` æ¥çæä»¶å¸®å© ### ææå¾  ç¹å»å±å¼ ![example](./readme/
-example.png)  ## ð ç¢ç¢å¿µ - ~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
+[config.py](./nonebot_plugin_pjsk/config.py) æä»¶ ## ð ä½¿ç¨
+ç´æ¥ä½¿ç¨æä»¤ `pjsk` è¿å¥äº¤äºåå»ºæ¨¡å¼ï¼ ä½¿ç¨æä»¤ `pjsk -h`
+äºè§£ä½¿ç¨ Shell-Like æä»¤åå»ºè¡¨æçå¸®å© ### ææå¾
+ä½¿ç¨äº¤äºåå»ºæ¨¡å¼ ![example](./readme/example-interact.png)   ä½¿ç¨
+Shell-Like æä»¤ ![example](./readme/example.png)  ## ð ç¢ç¢å¿µ -
+~~ç±äºæ¬äººæ²¡ç©è¿å¤éç§ç¤ï¼~~
 å¯è½åºç°ä¸äºå°é®é¢ï¼å¯ä»¥æ issue æè [å ç¾¤](https://
 jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦ ~~æèåçº¯è¿æ¥ç©~~ -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨éï¼åæ¬¢è¯¥é¡¹ç®å¯ä»¥
 Star æèæä¾ PRï¼å¦æææä¾µæå°å¨ 24 å°æ¶åå é¤ -
 [ç±åçµ](https://afdian.net/a/agnes_digital) ## ð¡ é¸£è°¢ ###
 [TheOriginalAyaka/sekai-stickers](https://github.com/TheOriginalAyaka/sekai-
 stickers) - åé¡¹ç® & ç´ ææ¥æº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+[ç±åçµ](https://afdian.net/a/agnes_digital) ## ð æ´æ°æ¥å¿ ### 0.2.2
+- ä¿®æ¹äº 0.2.1 ççäº¤äºåå»ºæ¨¡å¼çè§¦åæ¹å¼ -
+è¯éªæ§å°æ¯æäº Emoji ### 0.2.1 - æ´æ¹æä»¤ `pjskåè¡¨`
+çäº¤äºæ¹å¼ ### 0.2.0 - éææä»¶
```

