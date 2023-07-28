# Comparing `tmp/streamdeck_linux_gui-3.0.0.tar.gz` & `tmp/streamdeck_linux_gui-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeck_linux_gui-3.0.0.tar", max compression
+gzip compressed data, was "streamdeck_linux_gui-3.0.1.tar", max compression
```

## Comparing `streamdeck_linux_gui-3.0.0.tar` & `streamdeck_linux_gui-3.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1072 2023-07-25 14:47:47.596712 streamdeck_linux_gui-3.0.0/LICENSE
--rw-r--r--   0        0        0     6971 2023-07-27 13:01:44.079668 streamdeck_linux_gui-3.0.0/README.md
--rw-r--r--   0        0        0     1455 2023-07-27 19:37:52.914647 streamdeck_linux_gui-3.0.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/__init__.py
--rw-r--r--   0        0        0    22758 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/api.py
--rw-r--r--   0        0        0      496 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/config.py
--rw-r--r--   0        0        0     3252 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/dimmer.py
--rw-r--r--   0        0        0        0 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/__init__.py
--rw-r--r--   0        0        0    10958 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/display_grid.py
--rw-r--r--   0        0        0     1283 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/empty_filter.py
--rw-r--r--   0        0        0     2394 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/filter.py
--rw-r--r--   0        0        0     4381 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/image_filter.py
--rw-r--r--   0        0        0     1763 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/keypress_filter.py
--rw-r--r--   0        0        0     2754 2023-07-26 22:20:00.861250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/pipeline.py
--rw-r--r--   0        0        0     1427 2023-07-26 22:20:00.862250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/pulse_filter.py
--rw-r--r--   0        0        0     3324 2023-07-26 22:20:00.862250 streamdeck_linux_gui-3.0.0/streamdeck_ui/display/text_filter.py
--rw-r--r--   0        0        0    11560 2023-07-26 22:20:00.862250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/LICENSE.txt
--rw-r--r--   0        0        0   171072 2023-07-26 22:20:00.862250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   177120 2023-07-26 22:20:00.863250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   170348 2023-07-26 22:20:00.863250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   174520 2023-07-26 22:20:00.864250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   173516 2023-07-26 22:20:00.865250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   170012 2023-07-26 22:20:00.865250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   176184 2023-07-26 22:20:00.866250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   171656 2023-07-26 22:20:00.866250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   176428 2023-07-26 22:20:00.867250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   171272 2023-07-26 22:20:00.867250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   171500 2023-07-26 22:20:00.868250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   175872 2023-07-26 22:20:00.868250 streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0    33374 2023-07-27 13:01:18.448668 streamdeck_linux_gui-3.0.0/streamdeck_ui/gui.py
--rw-r--r--   0        0        0     1081 2023-07-26 22:20:00.869250 streamdeck_linux_gui-3.0.0/streamdeck_ui/icons/cross.png
--rw-r--r--   0        0        0     1341 2023-07-26 22:20:00.869250 streamdeck_linux_gui-3.0.0/streamdeck_ui/icons/gear.png
--rw-r--r--   0        0        0      236 2023-07-26 22:20:00.869250 streamdeck_linux_gui-3.0.0/streamdeck_ui/icons/vertical-align.png
--rw-r--r--   0        0        0    17681 2023-07-26 22:20:00.869250 streamdeck_linux_gui-3.0.0/streamdeck_ui/logo.png
--rw-r--r--   0        0        0    18321 2023-07-26 22:20:00.869250 streamdeck_linux_gui-3.0.0/streamdeck_ui/main.ui
--rw-r--r--   0        0        0     6301 2023-07-26 22:20:00.869250 streamdeck_linux_gui-3.0.0/streamdeck_ui/mock_streamdeck.py
--rw-r--r--   0        0        0      181 2023-07-26 22:20:00.869250 streamdeck_linux_gui-3.0.0/streamdeck_ui/resources.qrc
--rw-r--r--   0        0        0     9432 2023-07-27 13:00:54.596668 streamdeck_linux_gui-3.0.0/streamdeck_ui/resources_rc.py
--rw-r--r--   0        0        0     1007 2023-07-26 22:20:00.876250 streamdeck_linux_gui-3.0.0/streamdeck_ui/semaphore.py
--rw-r--r--   0        0        0     4118 2023-07-26 22:20:00.876250 streamdeck_linux_gui-3.0.0/streamdeck_ui/settings.ui
--rw-r--r--   0        0        0     6700 2023-07-26 22:20:00.876250 streamdeck_linux_gui-3.0.0/streamdeck_ui/stream_deck_monitor.py
--rw-r--r--   0        0        0    18654 2023-07-27 13:00:54.596668 streamdeck_linux_gui-3.0.0/streamdeck_ui/ui_main.py
--rw-r--r--   0        0        0     5184 2023-07-27 13:00:54.596668 streamdeck_linux_gui-3.0.0/streamdeck_ui/ui_settings.py
--rw-r--r--   0        0        0     7921 1970-01-01 00:00:00.000000 streamdeck_linux_gui-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-28 20:26:47.134493 streamdeck_linux_gui-3.0.1/LICENSE
+-rw-r--r--   0        0        0     7643 2023-07-28 20:26:47.134493 streamdeck_linux_gui-3.0.1/README.md
+-rw-r--r--   0        0        0     1455 2023-07-28 20:26:47.142494 streamdeck_linux_gui-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-07-28 20:26:47.142494 streamdeck_linux_gui-3.0.1/streamdeck_ui/__init__.py
+-rw-r--r--   0        0        0    22758 2023-07-28 20:26:47.142494 streamdeck_linux_gui-3.0.1/streamdeck_ui/api.py
+-rw-r--r--   0        0        0      496 2023-07-28 20:26:47.142494 streamdeck_linux_gui-3.0.1/streamdeck_ui/config.py
+-rw-r--r--   0        0        0     3252 2023-07-28 20:26:47.142494 streamdeck_linux_gui-3.0.1/streamdeck_ui/dimmer.py
+-rw-r--r--   0        0        0        0 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/__init__.py
+-rw-r--r--   0        0        0    10958 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/display_grid.py
+-rw-r--r--   0        0        0     1283 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/empty_filter.py
+-rw-r--r--   0        0        0     2394 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/filter.py
+-rw-r--r--   0        0        0     4381 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/image_filter.py
+-rw-r--r--   0        0        0     1761 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/keypress_filter.py
+-rw-r--r--   0        0        0     2754 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/pipeline.py
+-rw-r--r--   0        0        0     1427 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/pulse_filter.py
+-rw-r--r--   0        0        0     3336 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/display/text_filter.py
+-rw-r--r--   0        0        0    11560 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/LICENSE.txt
+-rw-r--r--   0        0        0   171072 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   177120 2023-07-28 20:26:47.146494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   170348 2023-07-28 20:26:47.150494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   174520 2023-07-28 20:26:47.150494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   173516 2023-07-28 20:26:47.150494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   170012 2023-07-28 20:26:47.154494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   176184 2023-07-28 20:26:47.154494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   171656 2023-07-28 20:26:47.154494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   176428 2023-07-28 20:26:47.154494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   171272 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   171500 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   175872 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0    33374 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/gui.py
+-rw-r--r--   0        0        0     1081 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/icons/cross.png
+-rw-r--r--   0        0        0     1341 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/icons/gear.png
+-rw-r--r--   0        0        0      236 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/icons/vertical-align.png
+-rw-r--r--   0        0        0    17681 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/logo.png
+-rw-r--r--   0        0        0    18321 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/main.ui
+-rw-r--r--   0        0        0     6301 2023-07-28 20:26:47.158494 streamdeck_linux_gui-3.0.1/streamdeck_ui/mock_streamdeck.py
+-rw-r--r--   0        0        0      181 2023-07-28 20:26:47.162494 streamdeck_linux_gui-3.0.1/streamdeck_ui/resources.qrc
+-rw-r--r--   0        0        0     9432 2023-07-28 20:26:47.162494 streamdeck_linux_gui-3.0.1/streamdeck_ui/resources_rc.py
+-rw-r--r--   0        0        0     1007 2023-07-28 20:26:47.162494 streamdeck_linux_gui-3.0.1/streamdeck_ui/semaphore.py
+-rw-r--r--   0        0        0     4118 2023-07-28 20:26:47.162494 streamdeck_linux_gui-3.0.1/streamdeck_ui/settings.ui
+-rw-r--r--   0        0        0     6700 2023-07-28 20:26:47.162494 streamdeck_linux_gui-3.0.1/streamdeck_ui/stream_deck_monitor.py
+-rw-r--r--   0        0        0    18654 2023-07-28 20:26:47.162494 streamdeck_linux_gui-3.0.1/streamdeck_ui/ui_main.py
+-rw-r--r--   0        0        0     5184 2023-07-28 20:26:47.162494 streamdeck_linux_gui-3.0.1/streamdeck_ui/ui_settings.py
+-rw-r--r--   0        0        0     8593 1970-01-01 00:00:00.000000 streamdeck_linux_gui-3.0.1/PKG-INFO
```

### Comparing `streamdeck_linux_gui-3.0.0/LICENSE` & `streamdeck_linux_gui-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/README.md` & `streamdeck_linux_gui-3.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -59,28 +59,39 @@
 ### Precooked Scripts
 There are scripts for setting up streamdeck_ui on [Debian/Ubuntu](scripts/ubuntu_install.sh) and [Fedora](scripts/fedora_install.sh).
 
 ## Updating Documentation
 
 Documentation is powered by mkdocs-material, and its on the [docs](docs/) folder. Install it with `pip install mkdocs-material` and run `mkdocs serve` to see the changes locally, before submitting a PR.
 
-
 ## Development & Contributions
 
 Contributuions encouraged and very welcome, however some rules and guidelines must be followed! 
 
 ### General Guidelines
 
 - The project is versioned according to [Semantic Versioning](https://semver.org/).
 - When writing your commit messages, please follow the [Angular commit message](https://gist.github.com/brianclements/841ea7bffdb01346392c).
 - Pull requests should be made against the `develop` branch, so please make sure you check out the `develop` branch.
 - Pull requests should include tests and documentation as appropriate.
 - When opening a pull request, if possible, attach a screenshot or GIF of the changes.
-- Please read the [contributing guide](https://www.notion.so/cfcolaco/docs/contributing.md) for more information and instructions on how to get started.
+- Please read the [contributing guide](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/blob/main/docs/contributing/contributing-guide.md) for more information and instructions on how to get started.
+
+### Feature Requests
+
+Open a new discussion with the `feature request` tag and describe the feature you would like to see implemented. If you have a screenshot or GIF of the feature, please attach it to the discussion.
+
+### Bug Reports
+
+Open a bug report [here](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/issues) and follow the template. Please include as much information as possible.
+
+### Have a Question?
+
+If you need any help, have a question, or just want to discuss something related to the project, please feel free to open a [discussion](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/discussions).
 
 ## Known issues
 
 - pip package is not yet available for the current state of the project. Please install from source, currently trying to find a better way to provide the package.
-- Streamdeck uses [pynput](https://github.com/moses-palmer/pynput) for simulating **Key Presses** but it lacks proper [support for Wayland](https://github.com/moses-palmer/pynput/issues/189). Generally your results will be good when using X (Ubuntu/Linux Mint). [This thread](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/issues/47) may be useful.
+- Streamdeck uses [pynput](https://github.com/moses-palmer/pynput) for simulating **Key Presses** but it lacks proper [support for Wayland](https://github.com/moses-palmer/pynput/issues/189). Generally your results will be good when using X (Ubuntu/Linux Mint). [This thread](https://github.com/timothycrosley/streamdeck-ui/issues/47) may be useful.
 - **Key Press** or **Write Text** does not work on Fedora (outside of the streamdeck itself), which is not particularly useful. However, still do a lot with the **Command** feature.
-- Some users have reported that the Stream Deck device does not work on all on specific USB ports, as it draws quite a bit of power and/or has [strict bandwidth requirements](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/issues/69#issuecomment-715887397). Try a different port.
+- Some users have reported that the Stream Deck device does not work on all on specific USB ports, as it draws quite a bit of power and/or has [strict bandwidth requirements](https://github.com/timothycrosley/streamdeck-ui/issues/69#issuecomment-715887397). Try a different port.
 - If you are executing a shell script from the Command feature - remember to add the shebang at the top of your file, for the language in question. `#!/bin/bash` or `#!/usr/bin/python3` etc. The streamdeck may appear to lock up if you don't under some distros.
```

### Comparing `streamdeck_linux_gui-3.0.0/pyproject.toml` & `streamdeck_linux_gui-3.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamdeck-linux-gui"
-version = "3.0.0"
+version = "3.0.1"
 description = "A service, Web Interface, and UI for interacting with your computer using a Stream Deck"
 authors = ["Timothy Crosley <timothy.crosley@gmail.com>"]
 maintainers = ["4s3ti <4s3ti@4s3ti.net>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "streamdeck_ui"}
```

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/api.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/api.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/dimmer.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/dimmer.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/display_grid.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/display_grid.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/empty_filter.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/empty_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/filter.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/image_filter.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/image_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/keypress_filter.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/keypress_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             if image:
                 return (image, frame_hash)
 
             input = get_input()
             if self.active:
                 input = get_input()
                 background = self.blank_image.copy()
-                input.thumbnail((self.size[0] - 10, self.size[1] - 10), Image.ANTIALIAS)
+                input.thumbnail((self.size[0] - 10, self.size[1] - 10), Image.LANCZOS)
                 # Reduce the image by 10px
 
                 enhancer = ImageEnhance.Brightness(input)
                 input = enhancer.enhance(2)
                 # Light it up a bit
 
                 background.paste(input, (5, 5))
```

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/pipeline.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/pipeline.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/pulse_filter.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/pulse_filter.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/display/text_filter.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/display/text_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,21 @@
         self.hashcode = hash((self.__class__, text, font, vertical_align))
 
     def initialize(self, size: Tuple[int, int]):
         self.image = Image.new("RGBA", size)
         backdrop_draw = ImageDraw.Draw(self.image)
 
         # Calculate the height and width of the text we're drawing, using the font itself
-        label_w, _ = backdrop_draw.textsize(self.text, font=self.true_font)
-
+        label_w = backdrop_draw.textlength(self.text, font=self.true_font)
         # Calculate dimensions for text that include ascender (above the line)
         # and below the line  (descender) characters. This is used to adust the
         # font placement and should allow for button text to horizontally align
         # across buttons. Basically we want to figure out what is the tallest
         # text we will need to draw.
-        _, label_h = backdrop_draw.textsize("lLpgyL|", font=self.true_font)
+        _, _, _, label_h = backdrop_draw.textbbox((0, 0), "lLpgyL|", font=self.true_font)
 
         gap = (size[1] - 5 * label_h) // 4
 
         if self.vertical_align == "top":
             label_y = 0
         elif self.vertical_align == "middle-top":
             label_y = gap + label_h
```

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/LICENSE.txt` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Black.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Light.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/fonts/roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/gui.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/gui.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/icons/cross.png` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/icons/cross.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/icons/gear.png` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/icons/gear.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/logo.png` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/logo.png`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/main.ui` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/main.ui`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/mock_streamdeck.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/mock_streamdeck.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/resources_rc.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/resources_rc.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/semaphore.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/semaphore.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/settings.ui` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/settings.ui`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/stream_deck_monitor.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/stream_deck_monitor.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/ui_main.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/ui_main.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/streamdeck_ui/ui_settings.py` & `streamdeck_linux_gui-3.0.1/streamdeck_ui/ui_settings.py`

 * *Files identical despite different names*

### Comparing `streamdeck_linux_gui-3.0.0/PKG-INFO` & `streamdeck_linux_gui-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeck-linux-gui
-Version: 3.0.0
+Version: 3.0.1
 Summary: A service, Web Interface, and UI for interacting with your computer using a Stream Deck
 License: MIT
 Author: Timothy Crosley
 Author-email: timothy.crosley@gmail.com
 Maintainer: 4s3ti
 Maintainer-email: 4s3ti@4s3ti.net
 Requires-Python: >=3.8,<3.12
@@ -84,29 +84,40 @@
 ### Precooked Scripts
 There are scripts for setting up streamdeck_ui on [Debian/Ubuntu](scripts/ubuntu_install.sh) and [Fedora](scripts/fedora_install.sh).
 
 ## Updating Documentation
 
 Documentation is powered by mkdocs-material, and its on the [docs](docs/) folder. Install it with `pip install mkdocs-material` and run `mkdocs serve` to see the changes locally, before submitting a PR.
 
-
 ## Development & Contributions
 
 Contributuions encouraged and very welcome, however some rules and guidelines must be followed! 
 
 ### General Guidelines
 
 - The project is versioned according to [Semantic Versioning](https://semver.org/).
 - When writing your commit messages, please follow the [Angular commit message](https://gist.github.com/brianclements/841ea7bffdb01346392c).
 - Pull requests should be made against the `develop` branch, so please make sure you check out the `develop` branch.
 - Pull requests should include tests and documentation as appropriate.
 - When opening a pull request, if possible, attach a screenshot or GIF of the changes.
-- Please read the [contributing guide](https://www.notion.so/cfcolaco/docs/contributing.md) for more information and instructions on how to get started.
+- Please read the [contributing guide](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/blob/main/docs/contributing/contributing-guide.md) for more information and instructions on how to get started.
+
+### Feature Requests
+
+Open a new discussion with the `feature request` tag and describe the feature you would like to see implemented. If you have a screenshot or GIF of the feature, please attach it to the discussion.
+
+### Bug Reports
+
+Open a bug report [here](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/issues) and follow the template. Please include as much information as possible.
+
+### Have a Question?
+
+If you need any help, have a question, or just want to discuss something related to the project, please feel free to open a [discussion](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/discussions).
 
 ## Known issues
 
 - pip package is not yet available for the current state of the project. Please install from source, currently trying to find a better way to provide the package.
-- Streamdeck uses [pynput](https://github.com/moses-palmer/pynput) for simulating **Key Presses** but it lacks proper [support for Wayland](https://github.com/moses-palmer/pynput/issues/189). Generally your results will be good when using X (Ubuntu/Linux Mint). [This thread](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/issues/47) may be useful.
+- Streamdeck uses [pynput](https://github.com/moses-palmer/pynput) for simulating **Key Presses** but it lacks proper [support for Wayland](https://github.com/moses-palmer/pynput/issues/189). Generally your results will be good when using X (Ubuntu/Linux Mint). [This thread](https://github.com/timothycrosley/streamdeck-ui/issues/47) may be useful.
 - **Key Press** or **Write Text** does not work on Fedora (outside of the streamdeck itself), which is not particularly useful. However, still do a lot with the **Command** feature.
-- Some users have reported that the Stream Deck device does not work on all on specific USB ports, as it draws quite a bit of power and/or has [strict bandwidth requirements](https://github.com/streamdeck-linux-gui/streamdeck-linux-gui/issues/69#issuecomment-715887397). Try a different port.
+- Some users have reported that the Stream Deck device does not work on all on specific USB ports, as it draws quite a bit of power and/or has [strict bandwidth requirements](https://github.com/timothycrosley/streamdeck-ui/issues/69#issuecomment-715887397). Try a different port.
 - If you are executing a shell script from the Command feature - remember to add the shebang at the top of your file, for the language in question. `#!/bin/bash` or `#!/usr/bin/python3` etc. The streamdeck may appear to lock up if you don't under some distros.
```

