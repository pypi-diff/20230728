# Comparing `tmp/jupyterlab_nodeeditor-1.0.7.tar.gz` & `tmp/jupyterlab_nodeeditor-1.0.8.tar.gz`

## Comparing `jupyterlab_nodeeditor-1.0.7.tar` & `jupyterlab_nodeeditor-1.0.8.tar`

### file list

```diff
@@ -1,444 +1,444 @@
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.copier-answers.yml
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.gitmodules
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/CHANGELOG.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/RELEASE.md
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/dev.sh
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/init.sh
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/install.json
--rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/package.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/setup.py
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/tsconfig.json
--rwxr-xr-x   0        0        0   215696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/yarn.lock
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.vscode/settings.json
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.copier-answers.yml
--rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.gitignore
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/CHANGELOG.md
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/LICENSE
--rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/README.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/RELEASE.md
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/install.json
--rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/package.json
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/pyproject.toml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/setup.py
--rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/tsconfig.json
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/schema/plugin.json
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/src/index.ts
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/style/base.css
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/style/index.js
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.babelrc
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.editorconfig
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.eslintrc
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.git
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.gitignore
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.npmignore
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.nvmrc
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.travis.yml
--rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/LICENSE
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/README.md
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress.json
--rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/logo.ai
--rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/logo.png
--rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/logo.svg
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/package.json
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/rollup.config.js
--rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/yarn.lock
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/fixtures/example.json
--rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/integration/NodeEditorSpec.js
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/plugins/index.js
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/support/commands.js
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/support/index.js
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/.gitignore
--rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/README.md
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/babel.config.js
--rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docusaurus.config.js
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/package.json
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/sidebars.js
--rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/yarn.lock
--rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/blog/2019-05-28-hola.md
--rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/blog/2019-05-29-hello-world.md
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/blog/2019-05-30-welcome.md
--rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/AnatomyExample.js
--rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/Colors.js
--rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/ControlExamples.js
--rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicNodesExamples.js
--rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicThemingExample.js
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/FlexRow.js
--rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/GettingStartedExample.js
--rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/NodeEditor.mdx
--rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/RootEngine.mdx
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/anatomy.mdx
--rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/basic-config.mdx
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/colors.mdx
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/comments.mdx
--rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/controls.mdx
--rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/defining-nodes.mdx
--rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc1.md
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc2.md
--rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc3.md
--rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/dynamic-nodes.mdx
--rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/faq.mdx
--rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/flume-config.mdx
--rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/logic-nodes.mdx
--rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/mdx.md
--rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/node-editor.mdx
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/overview.mdx
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/quick-start.mdx
--rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-engine.mdx
--rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-node.mdx
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/running-logic.mdx
--rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/saving-nodes.mdx
--rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/theming.mdx
--rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/type-safety.mdx
--rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-with-react.mdx
--rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-without-react.mdx
--rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/exampleFlumeConfig.js
--rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/components/TypeSafe.js
--rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/css/custom.css
--rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/index.js
--rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/styles.module.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/.nojekyll
--rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/60fps.svg
--rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-192x192.png
--rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-512x512.png
--rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/apple-touch-icon.png
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-blue.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-green.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-red.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-red_1.svg
--rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right.svg
--rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/controls.svg
--rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/example_editors.png
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon-16x16.png
--rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon-32x32.png
--rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon.ico
--rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/fb-img.png
--rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/flume-short-web.mp4
--rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/friends-graph.svg
--rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/hero-nodes.svg
--rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo-dark.svg
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo.svg
--rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/netlify.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/page-curve-blue.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/page-curve-dark.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/page-curve.svg
--rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/performance-tile.svg
--rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/play-icon.svg
--rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/react-tile.svg
--rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/size-tile.svg
--rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme-tile.svg
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme.svg
--rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-node.svg
--rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-nodes.svg
--rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_mountain.svg
--rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_react.svg
--rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_tree.svg
--rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/valid_port_types.png
--rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/wordmark_white.svg
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/.eslintrc
--rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/README.md
--rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/package.json
--rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/yarn.lock
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/public/index.html
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/public/manifest.json
--rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/App.js
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/index.css
--rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/index.js
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/TestEditor.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/nodes.js
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Checkbox.js
--rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/FloatingNavigation.js
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Header.js
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/LogicEditor.js
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Modal.js
--rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/OptionsEditor.js
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/BoxIcon.js
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/FormIcon.js
--rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/GearIcon.js
--rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Attributes.js
--rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Body.js
--rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Field.js
--rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.css
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.js
--rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/InputTypes.js
--rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/NodeTypes.js
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/PreviewField.js
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Sidebar.js
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/defaultNodes.js
--rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/designerReducer.js
--rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldTypes.js
--rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldsReducer.js
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/formHandler.js
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/previewFieldsReducer.js
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/resolveLogic.js
--rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/wizardLogic/logicTypes.js
--rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.css
--rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.js
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.css
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.js
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/.eslintrc
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/Cache.js
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/RootEngine.js
--rwxr-xr-x   0        0        0     2060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/commentsReducer.js
--rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/connectionCalculator.js
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/constants.js
--rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/context.js
--rwxr-xr-x   0        0        0     9649 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/index.js
--rwxr-xr-x   0        0        0    14282 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/nodesReducer.js
--rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/stageReducer.js
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/styles.css
--rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/toastsReducer.js
--rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/typeBuilders.js
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/utilities.js
--rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Checkbox/Checkbox.css
--rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Checkbox/Checkbox.js
--rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.css
--rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.js
--rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.css
--rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.js
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connection/Connection.css
--rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connection/Connection.js
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connections/Connections.css
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connections/Connections.js
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.css
--rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.js
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Control/Control.css
--rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Control/Control.js
--rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Draggable/Draggable.js
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.css
--rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.js
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Node/Node.css
--rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Node/Node.js
--rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.css
--rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.js
--rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.css
--rwxr-xr-x   0        0        0     9421 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.js
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/TextInput/TextInput.css
--rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/TextInput/TextInput.js
--rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.css
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.js
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/hooks/usePrevious.js
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/img/grid.png
--rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/dynamic.test.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/nodes.js
--rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/ssr.test.js
--rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/test.js
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/_version.py
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/select.py
--rwxr-xr-x   0        0        0     3962 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/utils.py
--rwxr-xr-x   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/package.json
--rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
--rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
--rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
--rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
--rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
--rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
--rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js
--rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js
--rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
--rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
--rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
--rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
--rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
--rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
--rwxr-xr-x   0        0        0   220449 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8863.6ed3cbfeea198a6b6e21.js
--rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
--rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
--rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    13292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/remoteEntry.05ee5c7186d725a070e5.js
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/style.js
--rwxr-xr-x   0        0        0     9868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
--rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/schema/plugin.json
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/ReRunIcon.tsx
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/arrownIcon.tsx
--rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/clearIcon.tsx
--rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/deleteIcon.tsx
--rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/exportIcon.tsx
--rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/factory.ts
--rwxr-xr-x   0        0        0    51346 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/flumeConfig.tsx
--rwxr-xr-x   0        0        0     8089 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/imageViewer.tsx
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/index.ts
--rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/lockIcon.tsx
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/model.ts
--rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/newIcon.tsx
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/runIcon.tsx
--rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/utils.tsx
--rwxr-xr-x   0        0        0   182475 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/widget.tsx
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/yesIcon.tsx
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/style/base.css
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/style/index.js
--rwxr-xr-x   0        0        0   254494 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/1.jpeg
--rwxr-xr-x   0        0        0   153675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/2.jpeg
--rwxr-xr-x   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/main.ipynb
--rwxr-xr-x   0        0        0   546624 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/testlib.ipynb
--rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.gitignore
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/LICENSE
--rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/README.md
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/.copier-answers.yml
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/.gitmodules
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/CHANGELOG.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/RELEASE.md
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/dev.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/init.sh
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/install.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/package.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/setup.py
+-rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/tsconfig.json
+-rwxr-xr-x   0        0        0   215696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/yarn.lock
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/.vscode/settings.json
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/.copier-answers.yml
+-rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/.gitignore
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/LICENSE
+-rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/README.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/RELEASE.md
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/install.json
+-rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/package.json
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/setup.py
+-rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/tsconfig.json
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/schema/plugin.json
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/src/index.ts
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/style/base.css
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/_temp_extension/style/index.js
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.babelrc
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.editorconfig
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.eslintrc
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.git
+-rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.gitignore
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.npmignore
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.nvmrc
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/.travis.yml
+-rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/LICENSE
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/README.md
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/cypress.json
+-rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/logo.ai
+-rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/logo.png
+-rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/logo.svg
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/package.json
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/rollup.config.js
+-rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/yarn.lock
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/cypress/fixtures/example.json
+-rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/cypress/integration/NodeEditorSpec.js
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/cypress/plugins/index.js
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/cypress/support/commands.js
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/cypress/support/index.js
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/.gitignore
+-rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/README.md
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/babel.config.js
+-rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docusaurus.config.js
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/package.json
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/sidebars.js
+-rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/yarn.lock
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/blog/2019-05-28-hola.md
+-rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/blog/2019-05-29-hello-world.md
+-rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/blog/2019-05-30-welcome.md
+-rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/components/AnatomyExample.js
+-rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/components/Colors.js
+-rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/components/ControlExamples.js
+-rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/components/DynamicNodesExamples.js
+-rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/components/DynamicThemingExample.js
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/components/FlexRow.js
+-rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/components/GettingStartedExample.js
+-rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/NodeEditor.mdx
+-rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/RootEngine.mdx
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/anatomy.mdx
+-rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/basic-config.mdx
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/colors.mdx
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/comments.mdx
+-rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/controls.mdx
+-rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/defining-nodes.mdx
+-rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/doc1.md
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/doc2.md
+-rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/doc3.md
+-rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/dynamic-nodes.mdx
+-rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/faq.mdx
+-rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/flume-config.mdx
+-rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/logic-nodes.mdx
+-rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/mdx.md
+-rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/node-editor.mdx
+-rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/overview.mdx
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/quick-start.mdx
+-rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/root-engine.mdx
+-rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/root-node.mdx
+-rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/running-logic.mdx
+-rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/saving-nodes.mdx
+-rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/theming.mdx
+-rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/type-safety.mdx
+-rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/using-with-react.mdx
+-rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/docs/using-without-react.mdx
+-rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/src/exampleFlumeConfig.js
+-rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/src/components/TypeSafe.js
+-rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/src/css/custom.css
+-rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/src/pages/index.js
+-rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/src/pages/styles.module.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/.nojekyll
+-rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/60fps.svg
+-rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/android-chrome-192x192.png
+-rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/android-chrome-512x512.png
+-rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/apple-touch-icon.png
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/arrow-right-blue.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/arrow-right-green.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/arrow-right-red.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/arrow-right-red_1.svg
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/arrow-right.svg
+-rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/controls.svg
+-rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/example_editors.png
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/favicon-16x16.png
+-rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/favicon-32x32.png
+-rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/favicon.ico
+-rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/fb-img.png
+-rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/flume-short-web.mp4
+-rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/friends-graph.svg
+-rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/hero-nodes.svg
+-rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/logo-dark.svg
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/logo.svg
+-rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/netlify.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/page-curve-blue.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/page-curve-dark.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/page-curve.svg
+-rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/performance-tile.svg
+-rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/play-icon.svg
+-rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/react-tile.svg
+-rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/size-tile.svg
+-rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/theme-tile.svg
+-rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/theme.svg
+-rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/type-safe-node.svg
+-rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/type-safe-nodes.svg
+-rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/undraw_docusaurus_mountain.svg
+-rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/undraw_docusaurus_react.svg
+-rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/undraw_docusaurus_tree.svg
+-rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/valid_port_types.png
+-rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/wordmark_white.svg
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/.eslintrc
+-rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/README.md
+-rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/package.json
+-rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/yarn.lock
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/public/index.html
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/public/manifest.json
+-rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/App.js
+-rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/index.css
+-rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/index.js
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/TestRoutes/TestEditor.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/TestRoutes/nodes.js
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/components/Checkbox.js
+-rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/components/FloatingNavigation.js
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/components/Header.js
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/components/LogicEditor.js
+-rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/components/Modal.js
+-rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/components/OptionsEditor.js
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/icons/BoxIcon.js
+-rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/icons/FormIcon.js
+-rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/icons/GearIcon.js
+-rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Attributes.js
+-rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Body.js
+-rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Field.js
+-rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Form.css
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Form.js
+-rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/InputTypes.js
+-rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/NodeTypes.js
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/PreviewField.js
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Sidebar.js
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/defaultNodes.js
+-rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/designerReducer.js
+-rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/fieldTypes.js
+-rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/fieldsReducer.js
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/formHandler.js
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/previewFieldsReducer.js
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/resolveLogic.js
+-rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/wizardLogic/logicTypes.js
+-rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Forms/Forms.css
+-rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Forms/Forms.js
+-rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Records/Records.css
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Records/Records.js
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/.eslintrc
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/Cache.js
+-rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/RootEngine.js
+-rwxr-xr-x   0        0        0     2060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/commentsReducer.js
+-rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/connectionCalculator.js
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/constants.js
+-rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/context.js
+-rwxr-xr-x   0        0        0     9649 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/index.js
+-rwxr-xr-x   0        0        0    14282 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/nodesReducer.js
+-rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/stageReducer.js
+-rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/styles.css
+-rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/toastsReducer.js
+-rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/typeBuilders.js
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/utilities.js
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Checkbox/Checkbox.css
+-rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Checkbox/Checkbox.js
+-rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/ColorPicker/ColorPicker.css
+-rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/ColorPicker/ColorPicker.js
+-rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Comment/Comment.css
+-rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Comment/Comment.js
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Connection/Connection.css
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Connection/Connection.js
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Connections/Connections.css
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Connections/Connections.js
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/ContextMenu/ContextMenu.css
+-rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/ContextMenu/ContextMenu.js
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Control/Control.css
+-rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Control/Control.js
+-rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Draggable/Draggable.js
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/IoPorts/IoPorts.css
+-rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/IoPorts/IoPorts.js
+-rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Node/Node.css
+-rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Node/Node.js
+-rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Select/Select.css
+-rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Select/Select.js
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Stage/Stage.css
+-rwxr-xr-x   0        0        0     9421 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Stage/Stage.js
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/TextInput/TextInput.css
+-rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/TextInput/TextInput.js
+-rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Toaster/Toaster.css
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/components/Toaster/Toaster.js
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/hooks/usePrevious.js
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/img/grid.png
+-rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/tests/dynamic.test.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/tests/nodes.js
+-rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/tests/ssr.test.js
+-rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/flume/src/tests/test.js
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/_version.py
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/select.py
+-rwxr-xr-x   0        0        0     4328 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/utils.py
+-rwxr-xr-x   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/package.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
+-rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
+-rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
+-rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
+-rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js
+-rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js
+-rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
+-rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
+-rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0   220723 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8863.20e858ad3b69492ea869.js
+-rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
+-rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
+-rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    13292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/remoteEntry.eca8ee7dca148406f024.js
+-rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/style.js
+-rwxr-xr-x   0        0        0     9868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
+-rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/schema/plugin.json
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/ReRunIcon.tsx
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/arrownIcon.tsx
+-rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/clearIcon.tsx
+-rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/deleteIcon.tsx
+-rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/exportIcon.tsx
+-rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/factory.ts
+-rwxr-xr-x   0        0        0    51346 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/flumeConfig.tsx
+-rwxr-xr-x   0        0        0     8089 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/imageViewer.tsx
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/index.ts
+-rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/lockIcon.tsx
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/model.ts
+-rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/newIcon.tsx
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/runIcon.tsx
+-rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/utils.tsx
+-rwxr-xr-x   0        0        0   183214 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/widget.tsx
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/src/yesIcon.tsx
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/style/base.css
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/style/index.js
+-rwxr-xr-x   0        0        0   254494 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/test_ext/1.jpeg
+-rwxr-xr-x   0        0        0   153675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/test_ext/2.jpeg
+-rwxr-xr-x   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/test_ext/main.ipynb
+-rwxr-xr-x   0        0        0   546624 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/test_ext/testlib.ipynb
+-rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/.gitignore
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/LICENSE
+-rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/README.md
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.8/PKG-INFO
```

### Comparing `jupyterlab_nodeeditor-1.0.7/RELEASE.md` & `jupyterlab_nodeeditor-1.0.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/package.json` & `jupyterlab_nodeeditor-1.0.8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.8'"}*

```diff
@@ -175,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.7"
+    "version": "1.0.8"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.7/tsconfig.json` & `jupyterlab_nodeeditor-1.0.8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/yarn.lock` & `jupyterlab_nodeeditor-1.0.8/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/.gitignore` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/LICENSE` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/README.md` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/RELEASE.md` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/package.json` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/pyproject.toml` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/tsconfig.json` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/jupyterlab_nodeeditor/__init__.py` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/jupyterlab_nodeeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/_temp_extension/src/index.ts` & `jupyterlab_nodeeditor-1.0.8/_temp_extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/CODE_OF_CONDUCT.md` & `jupyterlab_nodeeditor-1.0.8/flume/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/LICENSE` & `jupyterlab_nodeeditor-1.0.8/flume/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/README.md` & `jupyterlab_nodeeditor-1.0.8/flume/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/logo.ai` & `jupyterlab_nodeeditor-1.0.8/flume/logo.ai`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/logo.png` & `jupyterlab_nodeeditor-1.0.8/flume/logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/logo.svg` & `jupyterlab_nodeeditor-1.0.8/flume/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/package.json` & `jupyterlab_nodeeditor-1.0.8/flume/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/rollup.config.js` & `jupyterlab_nodeeditor-1.0.8/flume/rollup.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/yarn.lock` & `jupyterlab_nodeeditor-1.0.8/flume/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/cypress/integration/NodeEditorSpec.js` & `jupyterlab_nodeeditor-1.0.8/flume/cypress/integration/NodeEditorSpec.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/cypress/plugins/index.js` & `jupyterlab_nodeeditor-1.0.8/flume/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/cypress/support/commands.js` & `jupyterlab_nodeeditor-1.0.8/flume/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/cypress/support/index.js` & `jupyterlab_nodeeditor-1.0.8/flume/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/README.md` & `jupyterlab_nodeeditor-1.0.8/flume/docs/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docusaurus.config.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/package.json` & `jupyterlab_nodeeditor-1.0.8/flume/docs/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/yarn.lock` & `jupyterlab_nodeeditor-1.0.8/flume/docs/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/components/AnatomyExample.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/components/AnatomyExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/components/Colors.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/components/Colors.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/components/ControlExamples.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/components/ControlExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicNodesExamples.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/components/DynamicNodesExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicThemingExample.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/components/DynamicThemingExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/components/GettingStartedExample.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/components/GettingStartedExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/NodeEditor.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/NodeEditor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/RootEngine.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/RootEngine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/anatomy.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/anatomy.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/basic-config.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/basic-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/colors.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/colors.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/comments.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/comments.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/controls.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/controls.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/defining-nodes.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/defining-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc1.md` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/doc1.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc3.md` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/doc3.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/dynamic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/dynamic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/faq.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/faq.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/flume-config.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/flume-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/logic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/logic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/mdx.md` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/mdx.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/node-editor.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/node-editor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/overview.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/overview.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/quick-start.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/quick-start.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-engine.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/root-engine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-node.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/root-node.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/running-logic.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/running-logic.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/saving-nodes.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/saving-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/theming.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/theming.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/type-safety.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/type-safety.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-with-react.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/using-with-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-without-react.mdx` & `jupyterlab_nodeeditor-1.0.8/flume/docs/docs/using-without-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/src/exampleFlumeConfig.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/src/exampleFlumeConfig.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/src/components/TypeSafe.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/src/components/TypeSafe.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/src/css/custom.css` & `jupyterlab_nodeeditor-1.0.8/flume/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/index.js` & `jupyterlab_nodeeditor-1.0.8/flume/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/styles.module.css` & `jupyterlab_nodeeditor-1.0.8/flume/docs/src/pages/styles.module.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/60fps.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/60fps.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-192x192.png` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-512x512.png` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/apple-touch-icon.png` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/controls.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/controls.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/example_editors.png` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/example_editors.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon-32x32.png` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon.ico` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/fb-img.png` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/fb-img.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/flume-short-web.mp4` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/flume-short-web.mp4`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/friends-graph.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/friends-graph.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/hero-nodes.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/hero-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo-dark.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/netlify.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/netlify.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/performance-tile.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/performance-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/react-tile.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/react-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/size-tile.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/size-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme-tile.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/theme-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/theme.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-node.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/type-safe-node.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-nodes.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/type-safe-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_mountain.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_react.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_tree.svg` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/valid_port_types.png` & `jupyterlab_nodeeditor-1.0.8/flume/docs/static/img/valid_port_types.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/README.md` & `jupyterlab_nodeeditor-1.0.8/flume/example/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/package.json` & `jupyterlab_nodeeditor-1.0.8/flume/example/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/yarn.lock` & `jupyterlab_nodeeditor-1.0.8/flume/example/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/public/index.html` & `jupyterlab_nodeeditor-1.0.8/flume/example/public/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/App.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/App.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/index.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/TestEditor.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/TestRoutes/TestEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/nodes.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/TestRoutes/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Checkbox.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/components/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/FloatingNavigation.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/components/FloatingNavigation.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/LogicEditor.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/components/LogicEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/OptionsEditor.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/components/OptionsEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/BoxIcon.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/icons/BoxIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/FormIcon.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/icons/FormIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/GearIcon.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/icons/GearIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Attributes.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Attributes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Body.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Body.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Field.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Field.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.css` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Form.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Form.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/InputTypes.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/InputTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/NodeTypes.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/NodeTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/PreviewField.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/PreviewField.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Sidebar.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/Sidebar.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/designerReducer.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/designerReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldTypes.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/fieldTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldsReducer.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/fieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/previewFieldsReducer.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/previewFieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/resolveLogic.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/resolveLogic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/wizardLogic/logicTypes.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Form/wizardLogic/logicTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.css` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Forms/Forms.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Forms/Forms.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.css` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Records/Records.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.js` & `jupyterlab_nodeeditor-1.0.8/flume/example/src/pages/Records/Records.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/RootEngine.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/RootEngine.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/commentsReducer.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/commentsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/connectionCalculator.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/connectionCalculator.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/context.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/context.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/index.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/nodesReducer.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/nodesReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/toastsReducer.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/toastsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/typeBuilders.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/typeBuilders.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/utilities.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/utilities.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Checkbox/Checkbox.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Checkbox/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.css` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/ColorPicker/ColorPicker.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/ColorPicker/ColorPicker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.css` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Comment/Comment.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Comment/Comment.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Connection/Connection.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Connection/Connection.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.css` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/ContextMenu/ContextMenu.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/ContextMenu/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Control/Control.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Control/Control.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Draggable/Draggable.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Draggable/Draggable.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.css` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/IoPorts/IoPorts.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/IoPorts/IoPorts.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Node/Node.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Node/Node.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.css` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Select/Select.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Select/Select.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.css` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Stage/Stage.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Stage/Stage.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/TextInput/TextInput.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/TextInput/TextInput.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.css` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Toaster/Toaster.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/components/Toaster/Toaster.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/tests/dynamic.test.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/tests/dynamic.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/tests/nodes.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/tests/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/tests/ssr.test.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/tests/ssr.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/flume/src/tests/test.js` & `jupyterlab_nodeeditor-1.0.8/flume/src/tests/test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/select.py` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/select.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/utils.py` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import io
+import os
 import base64
 
 def get_instance_info(v):
     from .select import select, mselect
     t = type(v)
     d = None
     if isinstance(v, int) \
@@ -18,18 +19,25 @@
     return json.dumps({"type": str(t), "value": d})
 
 
 def get_urls(urls):
     # 如果urls是字符串
     if isinstance(urls, str):
         try:
-            ret = json.loads(urls)
-            if not isinstance(ret, list):
-                raise TypeError('Expecting a list')
-            return json.dumps(ret)
+            if urls.startswith('http'):
+                ret = json.loads(urls)
+                if not isinstance(ret, list):
+                    raise TypeError('Expecting a list')
+                return json.dumps(ret)
+            elif os.path.exists(urls) and os.path.isfile(urls):
+                with open(urls, 'rb') as fp:
+                    data = fp.read()
+                    data = base64.b64encode(data).decode()
+                url = 'data:image/png;base64,' + data
+                return json.dumps([url])
         except ValueError as e:
             return json.dumps([urls])
         except TypeError as e:
             raise TypeError('Invalid input type')
     
     # 如果urls是列表
     if isinstance(urls, list):
```

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/package.json` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.eca8ee7dca148406f024.js'}}",*

 * * "'version'": "'1.0.8'"}*

```diff
@@ -107,15 +107,15 @@
         "schema/**/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_nodeeditor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.05ee5c7186d725a070e5.js",
+            "load": "static/remoteEntry.eca8ee7dca148406f024.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_nodeeditor/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -180,9 +180,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.7"
+    "version": "1.0.8"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.8'"}*

```diff
@@ -175,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.7"
+    "version": "1.0.8"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8863.6ed3cbfeea198a6b6e21.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8863.20e858ad3b69492ea869.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6823,15 +6823,14 @@
                                         break
                                     } i || n.push((0, _flume__WEBPACK_IMPORTED_MODULE_7__.a2)(e)), o(n = r(t, n))
                             }
                     }
                     return i
                 }
                 async buildNodeTypeByCompleteMatch(match, filter) {
-                    var _a, _b;
                     let node_types = [],
                         node_type_name = "",
                         filters = filter.split(".");
                     if (filters.length > 1) {
                         filters.pop();
                         for (const e of filters) node_type_name = node_type_name + "." + e.trim();
                         node_type_name = node_type_name + "." + match.text.trim(), node_type_name = node_type_name.slice(1, node_type_name.length)
@@ -6855,63 +6854,67 @@
                                     target_type,
                                     target_value
                                 }
                             } catch (e) {}
                         }
                         break;
                         case "function": {
-                            let e = this._buildInputPortsFromSignature(match.signature);
-                            node_types = this._buildCommonNodeTypes(node_type_name, e), this._nodeTypes[node_type_name] = {
+                            let e = match.signature;
+                            if (-1 != e.indexOf("...")) {
+                                let t = await this._getFunctionSignature(node_type_name);
+                                t && (e = t)
+                            }
+                            let t = this._buildInputPortsFromSignature(e);
+                            node_types = this._buildCommonNodeTypes(node_type_name, t), this._nodeTypes[node_type_name] = {
                                 type: "function",
                                 node_type_name,
-                                in_ports: e
+                                in_ports: t
                             }
                         }
                         break;
                         case "module":
                         case "keywork":
                             break;
                         case "class": {
-                            let e = await (null === (_b = null === (_a = this._context.sessionContext.session) || void 0 === _a ? void 0 : _a.kernel) || void 0 === _b ? void 0 : _b.requestInspect({
-                                code: node_type_name,
-                                cursor_pos: node_type_name.length,
-                                detail_level: 1
-                            }));
-                            if (e && "ok" == e.content.status) {
-                                let t = e.content.data["text/plain"];
-                                t = (0, _utils__WEBPACK_IMPORTED_MODULE_22__.cc)(t);
-                                let n = /Init\ssignature:(.*?)(\(.*\))/g.exec(t);
-                                if (n) {
-                                    let e = this._buildInputPortsFromSignature(n[2], !0);
-                                    node_types = this._buildCommonNodeTypes(node_type_name, e, "class"), this._nodeTypes[node_type_name] = {
-                                        type: "class",
-                                        node_type_name,
-                                        in_ports: e
-                                    }
+                            let e = await this._getFunctionSignature(node_type_name);
+                            if (null != e) {
+                                let t = this._buildInputPortsFromSignature(e, !0);
+                                node_types = this._buildCommonNodeTypes(node_type_name, t, "class"), this._nodeTypes[node_type_name] = {
+                                    type: "class",
+                                    node_type_name,
+                                    in_ports: t
                                 }
                             }
                         }
                     }
                     return node_types
                 }
                 _buildInputPortsFromSignature(signature, isClass = !1) {
-                    signature = signature.replace(/->.*/g, ""), signature = signature.trim(), signature = signature.slice(1, signature.length - 1);
+                    signature = signature.replace(/->.*/g, ""), signature = signature.replace(/\s/g, ""), signature = signature.trim(), signature = signature.slice(1, signature.length - 1);
                     let in_ports = [],
                         state = "read_name",
                         arg_name = "",
                         arg_in_type = "keyword",
                         arg_type = "any",
                         arg_default = "None",
                         stateStack = [],
                         starFlag = !1;
 
                     function tryPushPortAndResetState() {
+                        switch (arg_type) {
+                            case "str":
+                            case "int":
+                            case "float":
+                            case "bool":
+                                break;
+                            default:
+                                arg_type = "any"
+                        }
                         if (starFlag || "/" != arg_name) {
                             if ("*" == arg_name) arg_in_type = "keyword", starFlag = !0;
-                            else if (isClass && 0 == in_ports.length);
                             else if (arg_name.length > 0) {
                                 let ret = /\*{2}\s*([_\w]+)/g.exec(arg_name);
                                 if (ret) {
                                     try {
                                         arg_name = "**" + ret[1].trim() + "(dict)"
                                     } catch (e) {}
                                     arg_type = "dict"
@@ -8715,14 +8718,29 @@
                     for (const o of Object.values(e)) null == t && (t = o), n == o.id && (t = o);
                     return null == t || await this._loadNodes(t, !1)
                 }
                 async _runStartNode() {
                     for (const e of Object.values(this.editorNodes))
                         if ("start" == e.type) return void await this.runNode(e.id, !0)
                 }
+                async _getFunctionSignature(e) {
+                    var t, n;
+                    let o = await (null === (n = null === (t = this._context.sessionContext.session) || void 0 === t ? void 0 : t.kernel) || void 0 === n ? void 0 : n.requestInspect({
+                        code: e,
+                        cursor_pos: e.length,
+                        detail_level: 1
+                    }));
+                    if (o && "ok" == o.content.status) {
+                        let e = o.content.data["text/plain"];
+                        e = (0, _utils__WEBPACK_IMPORTED_MODULE_22__.cc)(e);
+                        let t = /ignature:([\s\S]*?)(\([\s\S]*?\))/g.exec(e);
+                        if (t) return t[2]
+                    }
+                    return null
+                }
                 _createCommands() {
                     try {
                         this._createCommand("nd-load", "加载", (() => {
                             this._openLoadMenu()
                         })), this._createCommand("nd-create", "创建", (() => this.createNewNodes())), this._createCommand("nd-delete", "删除", (() => this.deleteNodes())), this._createCommand("nd-rename", "重命名", (() => this._renameNodes())), this._createCommand("nd-copy", "复制", (() => this._copyNodes())), this._createCommand("nd-run-all-cells", "执行所有的cell", (() => this.runAllCells())), this._createCommand("nd-clear-run-cache", "清除运行缓存", (() => this._clearRunCache())), this._createCommand("nd-undo", "恢复", (() => this.redo(-1))), this._createCommand("nd-redo", "重做", (() => this.redo(1))), this._createCommand("nd-reset-viewport", "重置视口", (() => this._focusToAllNodes())), this._createCommand("nd-toggle-output-area", "切换输出面板", (() => this._toggleOutputArea())), this._createCommand("nd-clear-output-area", "清空输出面板", (() => {
                             this._clearOutput()
                         })), this._createCommand("nd-open-code-editor", "打开编辑器", (() => this._openCellEditor())), this._createCommand("nd-kernel-interrupt", "中断内核", (() => this._interuptKernel())), this._createCommand("nd-kernel-restart", "重启内核", (() => this._restartKernel())), this._createCommand("nd-kernel-change", "更换内核", (() => this._selectKernel())), this._createCommand("nd-select-all", "选中所有节点", (() => this._selectAllNodes())), this._createCommand("nd-delete-selected-nodes", "删除选中的节点", (() => this._removeSelectedNodes())), this._createCommand("nd-copy-selected-nodes", "复制选中的节点", (() => this._copySelectedNodes())), this._createCommand("nd-paste-selected-nodes", "粘贴选中的节点", (() => this._pasteSelectedNodes())), this._createCommand("nd-focus-to-selected-nodes", "聚焦选中的节点", (() => this._focusToSelectedNodes())), this._createCommand("nd-close-image-viewer", "关闭图片浏览器", (() => this.setShowImg(!1))), this._createCommand("nd-run-cucrrent-cell", "运行当前的Cell", (() => this._editorRun())), this._createCommand("nd-insert-cell", "插入Cell", (() => {
```

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/remoteEntry.05ee5c7186d725a070e5.js` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/remoteEntry.eca8ee7dca148406f024.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -123,15 +123,15 @@
         8084: "dda9b009ce099df0bb96",
         8180: "a3d01aa0d2f10b552dd3",
         8401: "d14444e38cb7aa24efdd",
         8424: "3938b0f02a27846d3fcd",
         8670: "e60df217bf8cf5c38364",
         8715: "815f4104f6ed5438c593",
         8719: "e05fefc4bcc2bc7ab0d6",
-        8863: "6ed3cbfeea198a6b6e21",
+        8863: "20e858ad3b69492ea869",
         8906: "b9ef8e8fbada8f634ff8",
         8946: "e37c54e493ef0fcd3129",
         9343: "68df0c5454cb71b71ac8",
         9398: "e709c53f5309c556391b",
         9400: "af8212185e81be7c179c",
         9537: "5b34dc2ee55a5048c2a8",
         9684: "31d4865e5191437dcb69",
@@ -215,15 +215,15 @@
         8084: "dda9b009ce099df0bb96",
         8180: "a3d01aa0d2f10b552dd3",
         8401: "d14444e38cb7aa24efdd",
         8424: "3938b0f02a27846d3fcd",
         8670: "e60df217bf8cf5c38364",
         8715: "815f4104f6ed5438c593",
         8719: "e05fefc4bcc2bc7ab0d6",
-        8863: "6ed3cbfeea198a6b6e21",
+        8863: "20e858ad3b69492ea869",
         8906: "b9ef8e8fbada8f634ff8",
         8946: "e37c54e493ef0fcd3129",
         9343: "68df0c5454cb71b71ac8",
         9398: "e709c53f5309c556391b",
         9400: "af8212185e81be7c179c",
         9537: "5b34dc2ee55a5048c2a8",
         9684: "31d4865e5191437dcb69",
@@ -285,15 +285,15 @@
                         (!b || !b.loaded && (!f != !b.eager ? f : t > b.from)) && (c[a] = {
                             get: d,
                             from: t,
                             eager: !!f
                         })
                     },
                     o = [];
-                return "default" === d && (b("jupyterlab_nodeeditor", "1.0.7", (() => Promise.all([E.e(2602), E.e(8863)]).then((() => () => E(8863))))), b("monaco-editor", "0.39.0", (() => Promise.all([E.e(3837), E.e(8)]).then((() => () => E(3837))))), b("react-portal", "4.2.2", (() => Promise.all([E.e(2602), E.e(5600)]).then((() => () => E(5600))))), b("uuid", "9.0.0", (() => E.e(9687).then((() => () => E(9687)))))), e[d] = o.length ? Promise.all(o).then((() => e[d] = 1)) : 1
+                return "default" === d && (b("jupyterlab_nodeeditor", "1.0.8", (() => Promise.all([E.e(2602), E.e(8863)]).then((() => () => E(8863))))), b("monaco-editor", "0.39.0", (() => Promise.all([E.e(3837), E.e(8)]).then((() => () => E(3837))))), b("react-portal", "4.2.2", (() => Promise.all([E.e(2602), E.e(5600)]).then((() => () => E(5600))))), b("uuid", "9.0.0", (() => E.e(9687).then((() => () => E(9687)))))), e[d] = o.length ? Promise.all(o).then((() => e[d] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var a = E.g.document;
         if (!e && a && (a.currentScript && (e = a.currentScript.src), !e)) {
```

### Comparing `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json` & `jupyterlab_nodeeditor-1.0.8/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/schema/plugin.json` & `jupyterlab_nodeeditor-1.0.8/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/ReRunIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/ReRunIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/arrownIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/arrownIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/clearIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/clearIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/deleteIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/deleteIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/exportIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/exportIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/factory.ts` & `jupyterlab_nodeeditor-1.0.8/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/flumeConfig.tsx` & `jupyterlab_nodeeditor-1.0.8/src/flumeConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/imageViewer.tsx` & `jupyterlab_nodeeditor-1.0.8/src/imageViewer.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/index.ts` & `jupyterlab_nodeeditor-1.0.8/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/lockIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/lockIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/newIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/newIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/runIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/runIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/utils.tsx` & `jupyterlab_nodeeditor-1.0.8/src/utils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/src/widget.tsx` & `jupyterlab_nodeeditor-1.0.8/src/widget.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -1839,55 +1839,54 @@
                         target_type,
                         target_value
                     }
                 } catch (error) { }
             } break;
             case "function": {
                 // 1.解析signature (a:int, b, c:str= "123", *args, **kwargs)
-                let in_ports: any[] = this._buildInputPortsFromSignature(match.signature)
+                let signature = match.signature as string
+                if (signature.indexOf("...") != -1) {
+                    let ret = await this._getFunctionSignature(node_type_name)
+                    if (ret) {
+                        signature = ret as string
+                    }
+                }
+                let in_ports: any[] = this._buildInputPortsFromSignature(signature)
                 // 2.构建nodeType
                 node_types = this._buildCommonNodeTypes(node_type_name, in_ports)
                 // 3.记录下来
                 this._nodeTypes[node_type_name] = {
                     type: "function",
                     node_type_name,
                     in_ports,
                 }
             } break;
             case "module": { } break;
             case "class": {
-                let ret = await this._context.sessionContext.session?.kernel?.requestInspect({
-                    code: node_type_name,
-                    cursor_pos: node_type_name.length,
-                    detail_level: 1
-                })
-                if (ret && ret.content.status == "ok") {
-                    let content = ret.content.data['text/plain'] as string
-                    content = removeAnsi(content)
-                    let execRet = /Init\ssignature:(.*?)(\(.*\))/g.exec(content)
-                    if (execRet) {
-                        let in_ports: any[] = this._buildInputPortsFromSignature(execRet[2], true)
-                        // 2.构建nodeType
-                        node_types = this._buildCommonNodeTypes(node_type_name, in_ports, "class")
-                        // 3.记录下来
-                        this._nodeTypes[node_type_name] = {
-                            type: "class",
-                            node_type_name,
-                            in_ports,
-                        }
+                let signature = await this._getFunctionSignature(node_type_name)
+                if (signature != null) {
+                    let in_ports: any[] = this._buildInputPortsFromSignature(signature, true)
+                    // 2.构建nodeType
+                    node_types = this._buildCommonNodeTypes(node_type_name, in_ports, "class")
+                    // 3.记录下来
+                    this._nodeTypes[node_type_name] = {
+                        type: "class",
+                        node_type_name,
+                        in_ports,
                     }
                 }
             } break;
             case "keywork": { } break;
         }
         return node_types
     }
 
     private _buildInputPortsFromSignature(signature: String, isClass = false) {
         signature = signature.replace(/->.*/g, "")
+        signature = signature.replace(/\s/g, "")
         signature = signature.trim()
         signature = signature.slice(1, signature.length - 1)
         let in_ports: any[] = []
         // 2.用 ", "分割
         let state: 'read_name'
             | 'read_type'
             | 'read_default'
@@ -1901,23 +1900,35 @@
         let arg_name = ''
         let arg_in_type = 'keyword'
         let arg_type = 'any'
         let arg_default: any = 'None'
         let stateStack: any[] = []
         let starFlag = false
         function tryPushPortAndResetState() {
+            switch (arg_type) {
+                case 'str':
+                    break;
+                case 'int':
+                    break;
+                case 'float':
+                    break;
+                case 'bool':
+                    break;
+                default:
+                    arg_type = 'any'
+            }
             if (!starFlag && arg_name == "/") {
                 arg_in_type = "keyword"
                 for (let port of in_ports) {
                     port.arg_in_type = "positional"
                 }
             } else if (arg_name == "*") {
                 arg_in_type = "keyword"
                 starFlag = true
-            } else if (isClass && in_ports.length == 0) {
+                // } else if (isClass && in_ports.length == 0) {
             } else if (arg_name.length > 0) {
                 // 判断是否是dict
                 let ret = /\*{2}\s*([_\w]+)/g.exec(arg_name)
                 if (ret) {
                     try { arg_name = "**" + ret[1].trim() + "(dict)" } catch (error) { }
                     arg_type = "dict"
                 } else {
@@ -2051,16 +2062,14 @@
                                     break;
                                 case 'float':
                                     arg_default = 0
                                     break;
                                 case 'bool':
                                     arg_default = false
                                     break;
-                                default:
-                                    break;
                             }
                             tryPushPortAndResetState()
                         } break
                         default: {
                             arg_type += c
                         } break
                     }
@@ -5100,14 +5109,31 @@
             if ((node as any).type == "start") {
                 await this.runNode((node as any).id, true)
                 return
             }
         }
     }
 
+    private async _getFunctionSignature(targetFunction) {
+        let ret = await this._context.sessionContext.session?.kernel?.requestInspect({
+            code: targetFunction,
+            cursor_pos: targetFunction.length,
+            detail_level: 1
+        })
+        if (ret && ret.content.status == "ok") {
+            let content = ret.content.data['text/plain'] as string
+            content = removeAnsi(content)
+            let execRet = /ignature:([\s\S]*?)(\([\s\S]*?\))/g.exec(content)
+            if (execRet) {
+                return execRet[2]
+            }
+        }
+        return null
+    }
+
     private _createCommands() {
         try {
             this._createCommand("nd-load", "加载", () => { this._openLoadMenu() })
             this._createCommand("nd-create", "创建", () => this.createNewNodes())
             this._createCommand("nd-delete", "删除", () => this.deleteNodes())
             this._createCommand("nd-rename", "重命名", () => this._renameNodes())
             this._createCommand("nd-copy", "复制", () => this._copyNodes())
```

### Comparing `jupyterlab_nodeeditor-1.0.7/src/yesIcon.tsx` & `jupyterlab_nodeeditor-1.0.8/src/yesIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/test_ext/1.jpeg` & `jupyterlab_nodeeditor-1.0.8/test_ext/1.jpeg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/test_ext/2.jpeg` & `jupyterlab_nodeeditor-1.0.8/test_ext/2.jpeg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/test_ext/main.ipynb` & `jupyterlab_nodeeditor-1.0.8/test_ext/main.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/test_ext/testlib.ipynb` & `jupyterlab_nodeeditor-1.0.8/test_ext/testlib.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/.gitignore` & `jupyterlab_nodeeditor-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/LICENSE` & `jupyterlab_nodeeditor-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/README.md` & `jupyterlab_nodeeditor-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/pyproject.toml` & `jupyterlab_nodeeditor-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.7/PKG-INFO` & `jupyterlab_nodeeditor-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nodeeditor
-Version: 1.0.7
+Version: 1.0.8
 Summary: 一个节点编辑器
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_nodeeditor
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_nodeeditor/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_nodeeditor.git
 Author-email: l0n0l <cenlan@hotmail.com>
 License: BSD 3-Clause License
```

