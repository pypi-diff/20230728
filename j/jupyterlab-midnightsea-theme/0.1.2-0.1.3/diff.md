# Comparing `tmp/jupyterlab_midnightsea_theme-0.1.2.tar.gz` & `tmp/jupyterlab_midnightsea_theme-0.1.3.tar.gz`

## Comparing `jupyterlab_midnightsea_theme-0.1.2.tar` & `jupyterlab_midnightsea_theme-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/.copier-answers.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/RELEASE.md
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/install.json
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/tsconfig.json
--rw-r--r--   0        0        0   194546 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/yarn.lock
--rw-r--r--   0        0        0   354654 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/images/jupyterlab_midnightsea_1.png
--rw-r--r--   0        0        0   386722 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/images/jupyterlab_midnightsea_2.png
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/_version.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/package.json
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/static/568.0b757b367ff3fc9a0857.js
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/static/remoteEntry.0655a2cd4fb696bf5a8d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    12310 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/themes/jupyterlab_midnightsea_theme/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/themes/jupyterlab_midnightsea_theme/index.js
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/src/index.ts
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/style/index.css
--rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/style/variables.css
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/LICENSE
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/README.md
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/.copier-answers.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/TODO.md
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/install.json
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0   194546 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/yarn.lock
+-rw-r--r--   0        0        0   354654 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/images/jupyterlab_midnightsea_1.png
+-rw-r--r--   0        0        0   386722 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/images/jupyterlab_midnightsea_2.png
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/_version.py
+-rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/build_log.json
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/package.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/static/lib_index_js.0ed371c83de09a8940fe.js
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/static/lib_index_js.0ed371c83de09a8940fe.js.map
+-rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/static/remoteEntry.68012014eddafa0dad9c.js
+-rw-r--r--   0        0        0    26057 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/static/remoteEntry.68012014eddafa0dad9c.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/static/style.js
+-rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/themes/jupyterlab_midnightsea_theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/themes/jupyterlab_midnightsea_theme/index.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/src/index.ts
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/style/index.css
+-rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/style/variables.css
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/README.md
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 jupyterlab_midnightsea_theme-0.1.3/PKG-INFO
```

### Comparing `jupyterlab_midnightsea_theme-0.1.2/RELEASE.md` & `jupyterlab_midnightsea_theme-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/package.json` & `jupyterlab_midnightsea_theme-0.1.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -172,9 +172,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_midnightsea_theme-0.1.2/tsconfig.json` & `jupyterlab_midnightsea_theme-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/yarn.lock` & `jupyterlab_midnightsea_theme-0.1.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/images/jupyterlab_midnightsea_1.png` & `jupyterlab_midnightsea_theme-0.1.3/images/jupyterlab_midnightsea_1.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/images/jupyterlab_midnightsea_2.png` & `jupyterlab_midnightsea_theme-0.1.3/images/jupyterlab_midnightsea_2.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/__init__.py` & `jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/package.json` & `jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.68012014eddafa0dad9c.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -97,15 +97,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/eduardotlc/jupyterlab_midnightsea_theme",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.0655a2cd4fb696bf5a8d.js"
+            "load": "static/remoteEntry.68012014eddafa0dad9c.js"
         },
         "extension": true,
         "outputDir": "jupyterlab_midnightsea_theme/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -176,9 +176,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_midnightsea_theme-0.1.2/jupyterlab_midnightsea_theme/labextension/themes/jupyterlab_midnightsea_theme/index.css` & `jupyterlab_midnightsea_theme-0.1.3/style/variables.css`

 * *Files 1% similar despite different names*

```diff
@@ -348,18 +348,7 @@
 
   --jp-vega-background: #161724;
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
 }
-
-tt,
-code,
-kbd,
-samp,
-pre {
-  font-family: var(--jp-code-font-family);
-  font-size: var(--jp-code-font-size);
-  line-height: var(--jp-code-line-height);
-}
-
```

### Comparing `jupyterlab_midnightsea_theme-0.1.2/src/index.ts` & `jupyterlab_midnightsea_theme-0.1.3/src/index.ts`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   activate: (app: JupyterFrontEnd, manager: IThemeManager) => {
     console.log(
       'JupyterLab extension jupyterlab_midnightsea_theme is activated!'
     );
     const style = 'jupyterlab_midnightsea_theme/index.css';
 
     manager.register({
-      name: 'jupyterlab_midnightsea_theme',
+      name: 'Midnight Sea',
       isLight: false,
       load: () => manager.loadCSS(style),
       unload: () => Promise.resolve(undefined)
     });
   }
 };
```

### Comparing `jupyterlab_midnightsea_theme-0.1.2/style/variables.css` & `jupyterlab_midnightsea_theme-0.1.3/jupyterlab_midnightsea_theme/labextension/themes/jupyterlab_midnightsea_theme/index.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 :root {
   --jp-shadow-base-lightness: 0;
-  --jp-shadow-umbra-color: rgba(
-    var(--jp-shadow-base-lightness),
-    var(--jp-shadow-base-lightness),
-    var(--jp-shadow-base-lightness),
-    0.2
-  );
-  --jp-shadow-penumbra-color: rgba(
-    var(--jp-shadow-base-lightness),
-    var(--jp-shadow-base-lightness),
-    var(--jp-shadow-base-lightness),
-    0.14
-  );
+  --jp-shadow-umbra-color: #50f106; 
+  --jp-shadow-penumbra-color: #50f106;
   --jp-shadow-ambient-color: rgba(
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     0.12
   );
   --jp-elevation-z0: none;
@@ -348,7 +338,18 @@
 
   --jp-vega-background: #161724;
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
 }
+
+tt,
+code,
+kbd,
+samp,
+pre {
+  font-family: var(--jp-code-font-family);
+  font-size: var(--jp-code-font-size);
+  line-height: var(--jp-code-line-height);
+}
+
```

### Comparing `jupyterlab_midnightsea_theme-0.1.2/.gitignore` & `jupyterlab_midnightsea_theme-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/LICENSE` & `jupyterlab_midnightsea_theme-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/README.md` & `jupyterlab_midnightsea_theme-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,69 +24,108 @@
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlab_tranquilblue_theme
+pip install jupyterlab-midnightsea-theme
+```
+
+To check the installation, execute:
+
+```bash
+jupyter labextension list
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall jupyterlab_tranquilblue_theme
+pip uninstall jupyterlab-midnightsea-theme
 ```
 
 ## Contributing
 
+To make personal customizations to the theme, edit the [variables.css](./style/variables.css) file, and then run the development install steps listed bellow.
+
+Feel free to make [pending](./TODO.md) or other optimizations and pull requests, this theme is still under development and any contribution is very much appreciated.
+
+
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
+- Clone the repo to your local environment:
+
+```bash
+git clone https://github.com/eduardotlc/jupyterlab_midnightsea_theme
+```
+
+- Change directory to the jupyterlab_midnightsea_theme directory:
+
+```bash
+cd jupyterlab_midnightsea_theme
+```
+
+- Install package in development mode:
+
+```bash
+pip install -ve "."
+```
+
+- Link your development version of the extension with JupyterLab:
+
 ```bash
-# Clone the repo to your local environment
-# Change directory to the jupyterlab_tranquilblue_theme directory
-# Install package in development mode
-pip install -e "."
-# Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
-# Rebuild extension Typescript source after making changes
+```
+
+- Rebuild extension Typescript source after making changes:
+
+```bash
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
+- Watch the source directory in one terminal, automatically rebuilding when needed:
+
 ```bash
-# Watch the source directory in one terminal, automatically rebuilding when needed
 jlpm watch
-# Run JupyterLab in another terminal
+```
+
+- Run JupyterLab in another terminal:
+
+```bash
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-pip uninstall jupyterlab_tranquilblue_theme
+pip uninstall jupyterlab_midnightsea_theme
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `jupyterlab_tranquilblue_theme` within that folder.
+folder is located. Then you can remove the symlink named `jupyterlab_ariakedark_theme` within that folder.
+
+## Other themes
+
+See my other Jupyter Lab themes too
 
-### Packaging the extension
+[Ariake Dark](https://github.com/eduardotlc/jupyterlab_ariakedark_theme)
 
-See [RELEASE](RELEASE.md)
+[Material Darker](https://github.com/eduardotlc/jupyterlab_materialdarker_theme)
```

### Comparing `jupyterlab_midnightsea_theme-0.1.2/pyproject.toml` & `jupyterlab_midnightsea_theme-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_midnightsea_theme-0.1.2/PKG-INFO` & `jupyterlab_midnightsea_theme-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_midnightsea_theme
-Version: 0.1.2
+Version: 0.1.3
 Summary: A dark blue and purple JupyterLab theme extension.
 Project-URL: Homepage, https://github.com/eduardotlc/jupyterlab_midnightsea_theme
 Project-URL: Bug Tracker, https://github.com/eduardotlc/jupyterlab_midnightsea_theme/issues
 Project-URL: Repository, https://github.com/eduardotlc/jupyterlab_midnightsea_theme.git
 Author-email: Eduardo Campos <eduardotcampos@usp.br>
 License: BSD 3-Clause License
         
@@ -77,69 +77,108 @@
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlab_tranquilblue_theme
+pip install jupyterlab-midnightsea-theme
+```
+
+To check the installation, execute:
+
+```bash
+jupyter labextension list
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall jupyterlab_tranquilblue_theme
+pip uninstall jupyterlab-midnightsea-theme
 ```
 
 ## Contributing
 
+To make personal customizations to the theme, edit the [variables.css](./style/variables.css) file, and then run the development install steps listed bellow.
+
+Feel free to make [pending](./TODO.md) or other optimizations and pull requests, this theme is still under development and any contribution is very much appreciated.
+
+
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
+- Clone the repo to your local environment:
+
+```bash
+git clone https://github.com/eduardotlc/jupyterlab_midnightsea_theme
+```
+
+- Change directory to the jupyterlab_midnightsea_theme directory:
+
+```bash
+cd jupyterlab_midnightsea_theme
+```
+
+- Install package in development mode:
+
+```bash
+pip install -ve "."
+```
+
+- Link your development version of the extension with JupyterLab:
+
 ```bash
-# Clone the repo to your local environment
-# Change directory to the jupyterlab_tranquilblue_theme directory
-# Install package in development mode
-pip install -e "."
-# Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
-# Rebuild extension Typescript source after making changes
+```
+
+- Rebuild extension Typescript source after making changes:
+
+```bash
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
+- Watch the source directory in one terminal, automatically rebuilding when needed:
+
 ```bash
-# Watch the source directory in one terminal, automatically rebuilding when needed
 jlpm watch
-# Run JupyterLab in another terminal
+```
+
+- Run JupyterLab in another terminal:
+
+```bash
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-pip uninstall jupyterlab_tranquilblue_theme
+pip uninstall jupyterlab_midnightsea_theme
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `jupyterlab_tranquilblue_theme` within that folder.
+folder is located. Then you can remove the symlink named `jupyterlab_ariakedark_theme` within that folder.
+
+## Other themes
+
+See my other Jupyter Lab themes too
 
-### Packaging the extension
+[Ariake Dark](https://github.com/eduardotlc/jupyterlab_ariakedark_theme)
 
-See [RELEASE](RELEASE.md)
+[Material Darker](https://github.com/eduardotlc/jupyterlab_materialdarker_theme)
```

