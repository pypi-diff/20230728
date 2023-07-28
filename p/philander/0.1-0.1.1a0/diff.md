# Comparing `tmp/philander-0.1.tar.gz` & `tmp/philander-0.1.1a0.tar.gz`

## Comparing `philander-0.1.tar` & `philander-0.1.1a0.tar`

### file list

```diff
@@ -1,145 +1,146 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 philander-0.1/.buildpath
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 philander-0.1/.project
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 philander-0.1/.pydevproject
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 philander-0.1/.externalToolBuilders/Sphinx API Doc.launch
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 philander-0.1/.externalToolBuilders/Sphinx Doc Build.launch
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 philander-0.1/.settings/org.eclipse.core.resources.prefs
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 philander-0.1/.settings/org.eclipse.ltk.core.refactoring.prefs
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 philander-0.1/doc/api/conf.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1/doc/api/index.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1/doc/api/modules.rst
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1/doc/api/philander.fastgait.rst
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 philander-0.1/doc/api/philander.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.buildinfo
--rw-r--r--   0        0        0   281164 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/genindex.html
--rw-r--r--   0        0        0    23481 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/gpio.html
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/index.html
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/interruptable.html
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/module.html
--rw-r--r--   0        0        0   447725 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/modules.html
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/objects.inv
--rw-r--r--   0        0        0    40495 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/philander.fastgait.html
--rw-r--r--   0        0        0  1291822 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/philander.html
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/py-modindex.html
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/search.html
--rw-r--r--   0        0        0   362002 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/searchindex.js
--rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/systypes.html
--rw-r--r--   0        0        0    29332 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/test.html
--rw-r--r--   0        0        0  1891795 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/environment.pickle
--rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/gpio.doctree
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/index.doctree
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/interruptable.doctree
--rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/module.doctree
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/modules.doctree
--rw-r--r--   0        0        0  3496468 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/philander.doctree
--rw-r--r--   0        0        0    97136 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/philander.fastgait.doctree
--rw-r--r--   0        0        0    50137 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/systypes.doctree
--rw-r--r--   0        0        0    76214 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/test.doctree
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/doc/api/index.doctree
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/doc/api/modules.doctree
--rw-r--r--   0        0        0   138640 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/.doctrees/doc/api/philander.doctree
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/dictionary.html
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/index.html
--rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/sensor.html
--rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/systypes.html
--rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/Configurable.html
--rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/Device.html
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/EventHandler.html
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/FuelGauge.html
--rw-r--r--   0        0        0    61382 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/Sensor.html
--rw-r--r--   0        0        0   115813 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/Serial_Bus.html
--rw-r--r--   0        0        0    13708 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/Watchdog.html
--rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/accelerometer.html
--rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/battery.html
--rw-r--r--   0        0        0   254368 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/bma456.html
--rw-r--r--   0        0        0   123528 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/bma456_reg.html
--rw-r--r--   0        0        0    38692 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/charger.html
--rw-r--r--   0        0        0    27268 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/dictionary.html
--rw-r--r--   0        0        0    28000 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/gasgauge.html
--rw-r--r--   0        0        0    81885 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/gpio.html
--rw-r--r--   0        0        0    60703 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/htu21d.html
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/hygrometer.html
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/imath.html
--rw-r--r--   0        0        0    30177 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/interruptable.html
--rw-r--r--   0        0        0   185929 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/max77960.html
--rw-r--r--   0        0        0   118450 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/max77960_reg.html
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/module.html
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/primitives.html
--rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/sbsimBMA456.html
--rw-r--r--   0        0        0   177744 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/serialbus.html
--rw-r--r--   0        0        0    48033 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/simBMA456.html
--rw-r--r--   0        0        0    44466 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/simbus.html
--rw-r--r--   0        0        0    50486 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/simdev.html
--rw-r--r--   0        0        0    13669 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/systypes.html
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/thermometer.html
--rw-r--r--   0        0        0    19223 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/voltmeter.html
--rw-r--r--   0        0        0    70844 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_modules/philander/fastgait/actorunit.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/gpio.rst.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/interruptable.rst.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/module.rst.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/philander.fastgait.rst.txt
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/philander.rst.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/systypes.rst.txt
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_sources/test.rst.txt
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/alabaster.css
--rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/doctools.js
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/file.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/plus.png
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 philander-0.1/doc/api/html/_static/underscore.js
--rw-r--r--   0        0        0   276792 2020-02-02 00:00:00.000000 philander-0.1/doc/uml/philander.aird
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 philander-0.1/doc/uml/philander.ecore
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 philander-0.1/philander/__init__.py
--rw-r--r--   0        0        0   116874 2020-02-02 00:00:00.000000 philander-0.1/philander/_bma456_feature.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 philander-0.1/philander/accelerometer.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 philander-0.1/philander/battery.py
--rw-r--r--   0        0        0    82541 2020-02-02 00:00:00.000000 philander-0.1/philander/bma456.py
--rw-r--r--   0        0        0    53191 2020-02-02 00:00:00.000000 philander-0.1/philander/bma456_reg.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 philander-0.1/philander/button.py
--rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 philander-0.1/philander/charger.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 philander-0.1/philander/configurable.py
--rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 philander-0.1/philander/dictionary.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 philander-0.1/philander/gasgauge.py
--rw-r--r--   0        0        0    23010 2020-02-02 00:00:00.000000 philander-0.1/philander/gpio.py
--rw-r--r--   0        0        0    16466 2020-02-02 00:00:00.000000 philander-0.1/philander/htu21d.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 philander-0.1/philander/hygrometer.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 philander-0.1/philander/imath.py
--rw-r--r--   0        0        0    10889 2020-02-02 00:00:00.000000 philander-0.1/philander/interruptable.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 philander-0.1/philander/led.py
--rw-r--r--   0        0        0    51549 2020-02-02 00:00:00.000000 philander-0.1/philander/max77960.py
--rw-r--r--   0        0        0    39765 2020-02-02 00:00:00.000000 philander-0.1/philander/max77960_reg.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 philander-0.1/philander/module.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 philander-0.1/philander/primitives.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 philander-0.1/philander/sensor.py
--rw-r--r--   0        0        0    59747 2020-02-02 00:00:00.000000 philander-0.1/philander/serialbus.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 philander-0.1/philander/simBMA456.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 philander-0.1/philander/simdev.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 philander-0.1/philander/systypes.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 philander-0.1/philander/thermometer.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 philander-0.1/philander/vibrasense.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 philander-0.1/philander/vibrasense2.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 philander-0.1/philander/voltmeter.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 philander-0.1/philander/watchdog.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 philander-0.1/philander/fastgait/__init__.py
--rw-r--r--   0        0        0    20466 2020-02-02 00:00:00.000000 philander-0.1/philander/fastgait/actorunit.py
--rw-r--r--   0        0        0    21356 2020-02-02 00:00:00.000000 philander-0.1/philander/fastgait/sysman.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 philander-0.1/test/utgpio.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 philander-0.1/test/utimath.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 philander-0.1/test/utserialbus.py
--rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 philander-0.1/LICENSE.txt
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 philander-0.1/pyproject.toml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 philander-0.1/readme.md
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 philander-0.1/PKG-INFO
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 philander-0.1.1a0/.buildpath
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 philander-0.1.1a0/.project
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.1a0/.pydevproject
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 philander-0.1.1a0/.pypirc
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 philander-0.1.1a0/.externalToolBuilders/Sphinx API Doc.launch
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 philander-0.1.1a0/.externalToolBuilders/Sphinx Doc Build.launch
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 philander-0.1.1a0/.settings/org.eclipse.core.resources.prefs
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 philander-0.1.1a0/.settings/org.eclipse.ltk.core.refactoring.prefs
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/conf.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/modules.rst
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/philander.fastgait.rst
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/philander.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.buildinfo
+-rw-r--r--   0        0        0   281164 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/genindex.html
+-rw-r--r--   0        0        0    23481 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/gpio.html
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/index.html
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/interruptable.html
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/module.html
+-rw-r--r--   0        0        0   447725 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/modules.html
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/objects.inv
+-rw-r--r--   0        0        0    40495 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/philander.fastgait.html
+-rw-r--r--   0        0        0  1291822 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/philander.html
+-rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/py-modindex.html
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/search.html
+-rw-r--r--   0        0        0   362002 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/searchindex.js
+-rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/systypes.html
+-rw-r--r--   0        0        0    29332 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/test.html
+-rw-r--r--   0        0        0  1891795 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/gpio.doctree
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/index.doctree
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/interruptable.doctree
+-rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/module.doctree
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/modules.doctree
+-rw-r--r--   0        0        0  3496468 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/philander.doctree
+-rw-r--r--   0        0        0    97136 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/philander.fastgait.doctree
+-rw-r--r--   0        0        0    50137 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/systypes.doctree
+-rw-r--r--   0        0        0    76214 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/test.doctree
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/doc/api/index.doctree
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/doc/api/modules.doctree
+-rw-r--r--   0        0        0   138640 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/.doctrees/doc/api/philander.doctree
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/dictionary.html
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/index.html
+-rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/sensor.html
+-rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/systypes.html
+-rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/Configurable.html
+-rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/Device.html
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/EventHandler.html
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/FuelGauge.html
+-rw-r--r--   0        0        0    61382 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/Sensor.html
+-rw-r--r--   0        0        0   115813 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/Serial_Bus.html
+-rw-r--r--   0        0        0    13708 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/Watchdog.html
+-rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/accelerometer.html
+-rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/battery.html
+-rw-r--r--   0        0        0   254368 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/bma456.html
+-rw-r--r--   0        0        0   123528 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/bma456_reg.html
+-rw-r--r--   0        0        0    38692 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/charger.html
+-rw-r--r--   0        0        0    27268 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/dictionary.html
+-rw-r--r--   0        0        0    28000 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/gasgauge.html
+-rw-r--r--   0        0        0    81885 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/gpio.html
+-rw-r--r--   0        0        0    60703 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/htu21d.html
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/hygrometer.html
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/imath.html
+-rw-r--r--   0        0        0    30177 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/interruptable.html
+-rw-r--r--   0        0        0   185929 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/max77960.html
+-rw-r--r--   0        0        0   118450 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/max77960_reg.html
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/module.html
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/primitives.html
+-rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/sbsimBMA456.html
+-rw-r--r--   0        0        0   177744 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/serialbus.html
+-rw-r--r--   0        0        0    48033 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/simBMA456.html
+-rw-r--r--   0        0        0    44466 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/simbus.html
+-rw-r--r--   0        0        0    50486 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/simdev.html
+-rw-r--r--   0        0        0    13669 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/systypes.html
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/thermometer.html
+-rw-r--r--   0        0        0    19223 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/voltmeter.html
+-rw-r--r--   0        0        0    70844 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_modules/philander/fastgait/actorunit.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/gpio.rst.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/interruptable.rst.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/module.rst.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/philander.fastgait.rst.txt
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/philander.rst.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/systypes.rst.txt
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_sources/test.rst.txt
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/doctools.js
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/file.png
+-rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/plus.png
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/api/html/_static/underscore.js
+-rw-r--r--   0        0        0   276792 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/uml/philander.aird
+-rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 philander-0.1.1a0/doc/uml/philander.ecore
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/__init__.py
+-rw-r--r--   0        0        0   116874 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/_bma456_feature.py
+-rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/accelerometer.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/battery.py
+-rw-r--r--   0        0        0    82541 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/bma456.py
+-rw-r--r--   0        0        0    53191 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/bma456_reg.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/button.py
+-rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/charger.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/configurable.py
+-rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/dictionary.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/gasgauge.py
+-rw-r--r--   0        0        0    23010 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/gpio.py
+-rw-r--r--   0        0        0    16466 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/htu21d.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/hygrometer.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/imath.py
+-rw-r--r--   0        0        0    10889 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/interruptable.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/led.py
+-rw-r--r--   0        0        0    51549 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/max77960.py
+-rw-r--r--   0        0        0    39765 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/max77960_reg.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/module.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/primitives.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/sensor.py
+-rw-r--r--   0        0        0    59747 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/serialbus.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/simBMA456.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/simdev.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/systypes.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/thermometer.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/vibrasense.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/vibrasense2.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/voltmeter.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/watchdog.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/fastgait/__init__.py
+-rw-r--r--   0        0        0    20466 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/fastgait/actorunit.py
+-rw-r--r--   0        0        0    21356 2020-02-02 00:00:00.000000 philander-0.1.1a0/philander/fastgait/sysman.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 philander-0.1.1a0/test/utgpio.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 philander-0.1.1a0/test/utimath.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 philander-0.1.1a0/test/utserialbus.py
+-rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 philander-0.1.1a0/LICENSE.txt
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 philander-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 philander-0.1.1a0/readme.md
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 philander-0.1.1a0/PKG-INFO
```

### Comparing `philander-0.1/.project` & `philander-0.1.1a0/.project`

 * *Files identical despite different names*

### Comparing `philander-0.1/.pydevproject` & `philander-0.1.1a0/.pydevproject`

 * *Files 18% similar despite different names*

#### Comparing `philander-0.1/.pydevproject` & `philander-0.1.1a0/.pydevproject`

```diff
@@ -1,10 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?eclipse-pydev version="1.0"?>
 <pydev_project>
   <pydev_property name="org.python.pydev.PYTHON_PROJECT_INTERPRETER">Default</pydev_property>
   <pydev_property name="org.python.pydev.PYTHON_PROJECT_VERSION">python interpreter</pydev_property>
   <pydev_pathproperty name="org.python.pydev.PROJECT_SOURCE_PATH">
-    <path>/${PROJECT_DIR_NAME}/philander</path>
     <path>/${PROJECT_DIR_NAME}/test</path>
   </pydev_pathproperty>
 </pydev_project>
```

### Comparing `philander-0.1/.externalToolBuilders/Sphinx API Doc.launch` & `philander-0.1.1a0/.externalToolBuilders/Sphinx API Doc.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1/.externalToolBuilders/Sphinx Doc Build.launch` & `philander-0.1.1a0/.externalToolBuilders/Sphinx Doc Build.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/conf.py` & `philander-0.1.1a0/doc/api/conf.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/philander.fastgait.rst` & `philander-0.1.1a0/doc/api/philander.fastgait.rst`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/philander.rst` & `philander-0.1.1a0/doc/api/philander.rst`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/genindex.html` & `philander-0.1.1a0/doc/api/html/genindex.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/gpio.html` & `philander-0.1.1a0/doc/api/html/gpio.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/index.html` & `philander-0.1.1a0/doc/api/html/index.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/interruptable.html` & `philander-0.1.1a0/doc/api/html/interruptable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/module.html` & `philander-0.1.1a0/doc/api/html/module.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/modules.html` & `philander-0.1.1a0/doc/api/html/modules.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/objects.inv` & `philander-0.1.1a0/doc/api/html/objects.inv`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/philander.fastgait.html` & `philander-0.1.1a0/doc/api/html/philander.fastgait.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/philander.html` & `philander-0.1.1a0/doc/api/html/philander.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/py-modindex.html` & `philander-0.1.1a0/doc/api/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/search.html` & `philander-0.1.1a0/doc/api/html/search.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/searchindex.js` & `philander-0.1.1a0/doc/api/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/systypes.html` & `philander-0.1.1a0/doc/api/html/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/test.html` & `philander-0.1.1a0/doc/api/html/test.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/environment.pickle` & `philander-0.1.1a0/doc/api/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/gpio.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/gpio.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/index.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/interruptable.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/interruptable.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/module.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/module.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/modules.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/philander.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/philander.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/philander.fastgait.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/philander.fastgait.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/systypes.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/systypes.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/test.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/test.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/doc/api/index.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/doc/api/index.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/doc/api/modules.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/doc/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/.doctrees/doc/api/philander.doctree` & `philander-0.1.1a0/doc/api/html/.doctrees/doc/api/philander.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/dictionary.html` & `philander-0.1.1a0/doc/api/html/_modules/dictionary.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/index.html` & `philander-0.1.1a0/doc/api/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/sensor.html` & `philander-0.1.1a0/doc/api/html/_modules/sensor.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/systypes.html` & `philander-0.1.1a0/doc/api/html/_modules/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/Configurable.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/Configurable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/Device.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/Device.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/EventHandler.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/EventHandler.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/FuelGauge.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/FuelGauge.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/Sensor.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/Sensor.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/Serial_Bus.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/Serial_Bus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/Watchdog.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/Watchdog.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/accelerometer.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/accelerometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/battery.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/battery.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/bma456.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/bma456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/bma456_reg.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/bma456_reg.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/charger.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/charger.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/dictionary.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/dictionary.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/gasgauge.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/gasgauge.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/gpio.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/gpio.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/htu21d.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/htu21d.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/hygrometer.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/hygrometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/imath.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/imath.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/interruptable.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/interruptable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/max77960.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/max77960.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/max77960_reg.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/max77960_reg.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/module.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/module.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/primitives.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/primitives.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/sbsimBMA456.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/sbsimBMA456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/serialbus.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/serialbus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/simBMA456.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/simBMA456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/simbus.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/simbus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/simdev.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/simdev.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/systypes.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/thermometer.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/thermometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/voltmeter.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/voltmeter.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_modules/philander/fastgait/actorunit.html` & `philander-0.1.1a0/doc/api/html/_modules/philander/fastgait/actorunit.html`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_sources/philander.fastgait.rst.txt` & `philander-0.1.1a0/doc/api/html/_sources/philander.fastgait.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_sources/philander.rst.txt` & `philander-0.1.1a0/doc/api/html/_sources/philander.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_sources/test.rst.txt` & `philander-0.1.1a0/doc/api/html/_sources/test.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js` & `philander-0.1.1a0/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/alabaster.css` & `philander-0.1.1a0/doc/api/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/basic.css` & `philander-0.1.1a0/doc/api/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/doctools.js` & `philander-0.1.1a0/doc/api/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/jquery-3.6.0.js` & `philander-0.1.1a0/doc/api/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/jquery.js` & `philander-0.1.1a0/doc/api/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/language_data.js` & `philander-0.1.1a0/doc/api/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/pygments.css` & `philander-0.1.1a0/doc/api/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/searchtools.js` & `philander-0.1.1a0/doc/api/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/sphinx_highlight.js` & `philander-0.1.1a0/doc/api/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/underscore-1.13.1.js` & `philander-0.1.1a0/doc/api/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/api/html/_static/underscore.js` & `philander-0.1.1a0/doc/api/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/uml/philander.aird` & `philander-0.1.1a0/doc/uml/philander.aird`

 * *Files identical despite different names*

### Comparing `philander-0.1/doc/uml/philander.ecore` & `philander-0.1.1a0/doc/uml/philander.ecore`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/__init__.py` & `philander-0.1.1a0/philander/__init__.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/_bma456_feature.py` & `philander-0.1.1a0/philander/_bma456_feature.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/accelerometer.py` & `philander-0.1.1a0/philander/accelerometer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 """
 __author__ = "Oliver Maye"
 __version__ = "0.1"
 __all__ = ["Activity", "AxesSign", "Orientation", "Tap",\
            "SamplingMode", \
            "EventSource", "EventContext", "Configuration", "StatusID", "Data",\
            "Accelerometer"]
-from configurable import Configuration
+from .configurable import Configuration
+from .interruptable import EventContext as IntEventContext
+from .sensor import Sensor
+
 from dataclasses import dataclass
 from enum import Enum, Flag, unique, auto
-from interruptable import EventContext as IntEventContext
-from sensor import Sensor
 
 @unique
 class Activity(Enum):
     """Identifies general types of human walking activities, that an\
     accelerometer is possibly able to detect or distinguish.
     """
     unknown      = auto()
```

### Comparing `philander-0.1/philander/battery.py` & `philander-0.1.1a0/philander/battery.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/bma456.py` & `philander-0.1.1a0/philander/bma456.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/bma456_reg.py` & `philander-0.1.1a0/philander/bma456_reg.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/button.py` & `philander-0.1.1a0/philander/button.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/charger.py` & `philander-0.1.1a0/philander/charger.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/configurable.py` & `philander-0.1.1a0/philander/configurable.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/dictionary.py` & `philander-0.1.1a0/philander/dictionary.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/gasgauge.py` & `philander-0.1.1a0/philander/gasgauge.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/gpio.py` & `philander-0.1.1a0/philander/gpio.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/htu21d.py` & `philander-0.1.1a0/philander/htu21d.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/hygrometer.py` & `philander-0.1.1a0/philander/hygrometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/imath.py` & `philander-0.1.1a0/philander/imath.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/interruptable.py` & `philander-0.1.1a0/philander/interruptable.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/led.py` & `philander-0.1.1a0/philander/led.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/max77960.py` & `philander-0.1.1a0/philander/max77960.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/max77960_reg.py` & `philander-0.1.1a0/philander/max77960_reg.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/module.py` & `philander-0.1.1a0/philander/module.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/primitives.py` & `philander-0.1.1a0/philander/primitives.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/sensor.py` & `philander-0.1.1a0/philander/sensor.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/serialbus.py` & `philander-0.1.1a0/philander/serialbus.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/simBMA456.py` & `philander-0.1.1a0/philander/simBMA456.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/simdev.py` & `philander-0.1.1a0/philander/simdev.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/systypes.py` & `philander-0.1.1a0/philander/systypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Data types commonly used throughout the system and not associated with any specific module.
 """
 __author__ = "Oliver Maye"
 __version__ = "0.1"
 __all__ = ["ErrorCode", "RunLevel", "Info",]
 from enum import Enum
+from dataclasses import dataclass
 
 class ErrorCode(Enum):
     """Data type to indicate either a successful completion or the\
     reason why some function or operation failed.
     """
     errOk				= 0		# No error, success.
     errInvalidParameter	= 1		# Parameter is NULL or out of range.
```

### Comparing `philander-0.1/philander/thermometer.py` & `philander-0.1.1a0/philander/thermometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/vibrasense.py` & `philander-0.1.1a0/philander/vibrasense.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/vibrasense2.py` & `philander-0.1.1a0/philander/vibrasense2.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/voltmeter.py` & `philander-0.1.1a0/philander/voltmeter.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/watchdog.py` & `philander-0.1.1a0/philander/watchdog.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/fastgait/__init__.py` & `philander-0.1.1a0/philander/fastgait/__init__.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/fastgait/actorunit.py` & `philander-0.1.1a0/philander/fastgait/actorunit.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/philander/fastgait/sysman.py` & `philander-0.1.1a0/philander/fastgait/sysman.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/test/utgpio.py` & `philander-0.1.1a0/test/utgpio.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/test/utimath.py` & `philander-0.1.1a0/test/utimath.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/test/utserialbus.py` & `philander-0.1.1a0/test/utserialbus.py`

 * *Files identical despite different names*

### Comparing `philander-0.1/LICENSE.txt` & `philander-0.1.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1/pyproject.toml` & `philander-0.1.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "philander"
-version = "0.1"
+version = "0.1.1a"
 authors = [
   { name="Oliver Maye", email="maye@ihp-microelectronics.com" },
 ]
 description = "Sensor and other parts driver collection"
 readme = "readme.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `philander-0.1/PKG-INFO` & `philander-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philander
-Version: 0.1
+Version: 0.1.1a0
 Summary: Sensor and other parts driver collection
 Project-URL: Homepage, https://www.ihp-microelectronics.com/
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Oliver Maye <maye@ihp-microelectronics.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
```

