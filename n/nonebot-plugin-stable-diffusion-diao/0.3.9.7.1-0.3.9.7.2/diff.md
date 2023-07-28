# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.7.1.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.7.1.tar", last modified: Mon Jul 24 18:36:01 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.7.2.tar", last modified: Fri Jul 28 08:34:13 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    27623 2023-07-24 16:34:03.348175 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6215 2023-07-24 16:31:49.508822 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    16209 2023-07-24 18:35:40.523775 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6967 2023-07-24 18:35:51.029539 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    19049 2023-07-24 18:32:19.159565 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    10785 2023-07-24 18:01:54.559680 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    44350 2023-07-24 18:32:07.735950 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      730 2023-07-24 18:36:01.278393 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    27633 2023-07-27 04:38:23.778936 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6188 2023-07-28 08:33:16.986476 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    16209 2023-07-24 18:35:40.523775 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     6967 2023-07-24 18:35:51.029539 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    19049 2023-07-24 18:32:19.159565 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    10785 2023-07-25 03:34:42.018245 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    44380 2023-07-27 04:38:58.160130 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      730 2023-07-28 08:34:13.810804 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,16 +339,16 @@
         if not args.override:
             global pre_tags
             pre_tags = basetag + await config.get_value(group_id, "tags")
             pre_ntags = lowQuality + await config.get_value(group_id, "ntags")
         else:
             pre_tags = ""
             pre_ntags = ""
-        fifo.tags = pre_tags + "," + tags_list + "," + ",".join(new_tags_list) + style_tag + random_tags
-        fifo.ntags = pre_ntags + fifo.ntags + style_ntag
+        fifo.tags = pre_tags + "," + tags_list + "," + ",".join(new_tags_list) + str(style_tag) + random_tags
+        fifo.ntags = pre_ntags + fifo.ntags + str(style_ntag)
         if redis_client:
             tags_list_ = tags_to_list(tags_list)
             r1 = redis_client[0]
             pipe = r1.pipeline()
             pipe.rpush("prompts", str(tags_list_))
             pipe.rpush(fifo.user_id, str(dict(fifo)))
             pipe.execute()
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,15 @@
     user_msg = msg.extract_plain_text().strip()
     to_openai = user_msg + "prompt"
     prompt = await get_user_session(event.get_session_id()).main(to_openai)
 
     await risk_control(
                     bot, 
                     event, 
-                    "这是chatgpt为你生成的prompt"+prompt, 
-                    True
+                    "这是chatgpt为你生成的prompt"+prompt 
     )
     
     tags = config.novelai_tags + basetag + prompt
     ntags = config.novelai_ntags + lowQuality
 
     fifo = AIDRAW(
                 tags=tags,
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 后端 
 # 查看所有后端的工作状态
 emb 
 # 直接发送emb获取emb文件
 emb2_原  # 查找2号后端所有带有"原"的emb模型
 例如: 绘画 hutao 返回 原神胡桃的画面(如果有这个emb的话)
 lora
-# 同emb，直接发送lora获取所有的lora模型 使用 -lora 模型1编号_模型2权重,模型2编号_模型2权重，例如 -lora 341_1,233_0.9
+# 同emb，直接发送lora获取所有的lora模型 使用 -lora 模型1编号_模型1权重,模型2编号_模型2权重，例如 -lora 341_1,233_0.9
 ```
 ```
 采样器
 # 获取当前后端可用采样器
 分析
 # 分析出图像的tags, 分析 [图片], [回复图片消息] 分析,都是可以的
 审核
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -931,15 +931,15 @@
                 await risk_control(bot, event, [f"预设名称: {name}\n正面提示词: {tags}\n负面提示词: {ntags}\n"], True)
                 break
         if not find_style:
             await style_.finish(f"没有找到预设{args.find_style_name}")
     if len(args.tags) != 0:
         if args.tags and args.style_name:
             tags = await prepocess_tags(args.tags, False)
-            ntags = args.ntags
+            ntags = "" if args.ntags is None else args.ntags
             style_dict["name"] = args.style_name
             style_dict["prompt"] = tags
             style_dict["negative_prompt"] = ntags
             r.rpush("user_style", str(style_dict))
             await style_.finish(f"添加预设: {args.style_name}成功!")
         else:
             await style_.finish("参数不完整, 请检查后重试")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.1/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.7.1"
+version = "0.3.9.7.2"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

