# Comparing `tmp/philander-0.1.8.tar.gz` & `tmp/philander-0.1.9.tar.gz`

## Comparing `philander-0.1.8.tar` & `philander-0.1.9.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 philander-0.1.8/.buildpath
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 philander-0.1.8/.project
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.8/.pydevproject
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 philander-0.1.8/.externalToolBuilders/Build Dist.launch
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 philander-0.1.8/.externalToolBuilders/Sphinx API Doc.launch
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 philander-0.1.8/.externalToolBuilders/Sphinx Doc Build.launch
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 philander-0.1.8/.settings/org.eclipse.core.resources.prefs
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 philander-0.1.8/.settings/org.eclipse.ltk.core.refactoring.prefs
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/conf.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/index.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/modules.rst
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/philander.fastgait.rst
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/philander.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.buildinfo
--rw-r--r--   0        0        0   281311 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/genindex.html
--rw-r--r--   0        0        0    23481 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/gpio.html
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/index.html
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/interruptable.html
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/module.html
--rw-r--r--   0        0        0   457028 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/modules.html
--rw-r--r--   0        0        0    10531 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/objects.inv
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/philander.fastgait.html
--rw-r--r--   0        0        0  1347605 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/philander.html
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/py-modindex.html
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/search.html
--rw-r--r--   0        0        0   362717 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/searchindex.js
--rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/systypes.html
--rw-r--r--   0        0        0    29332 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/test.html
--rw-r--r--   0        0        0  1894041 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/environment.pickle
--rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/gpio.doctree
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/index.doctree
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/interruptable.doctree
--rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/module.doctree
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/modules.doctree
--rw-r--r--   0        0        0  3592562 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/philander.doctree
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/philander.fastgait.doctree
--rw-r--r--   0        0        0    50137 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/systypes.doctree
--rw-r--r--   0        0        0    76214 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/test.doctree
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/doc/api/index.doctree
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/doc/api/modules.doctree
--rw-r--r--   0        0        0   138640 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/.doctrees/doc/api/philander.doctree
--rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/dictionary.html
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/index.html
--rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/sensor.html
--rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/systypes.html
--rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/Configurable.html
--rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/Device.html
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/EventHandler.html
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/FuelGauge.html
--rw-r--r--   0        0        0    61389 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/Sensor.html
--rw-r--r--   0        0        0   115813 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/Serial_Bus.html
--rw-r--r--   0        0        0    13711 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/Watchdog.html
--rw-r--r--   0        0        0    23313 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/accelerometer.html
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/battery.html
--rw-r--r--   0        0        0   260186 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/bma456.html
--rw-r--r--   0        0        0   123528 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/bma456_reg.html
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/button.html
--rw-r--r--   0        0        0    38699 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/charger.html
--rw-r--r--   0        0        0    27732 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/dictionary.html
--rw-r--r--   0        0        0    28007 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/gasgauge.html
--rw-r--r--   0        0        0    81813 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/gpio.html
--rw-r--r--   0        0        0    60743 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/htu21d.html
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/hygrometer.html
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/imath.html
--rw-r--r--   0        0        0    30184 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/interruptable.html
--rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/led.html
--rw-r--r--   0        0        0   186098 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/max77960.html
--rw-r--r--   0        0        0   118450 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/max77960_reg.html
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/module.html
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/primitives.html
--rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/sbsimBMA456.html
--rw-r--r--   0        0        0   181688 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/serialbus.html
--rw-r--r--   0        0        0    48037 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/simBMA456.html
--rw-r--r--   0        0        0    44466 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/simbus.html
--rw-r--r--   0        0        0    50492 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/simdev.html
--rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/systypes.html
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/thermometer.html
--rw-r--r--   0        0        0    19853 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/vibrasense.html
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/vibrasense2.html
--rw-r--r--   0        0        0    19228 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/voltmeter.html
--rw-r--r--   0        0        0    70844 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_modules/philander/fastgait/actorunit.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/gpio.rst.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/index.rst.txt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/interruptable.rst.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/module.rst.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/philander.fastgait.rst.txt
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/philander.rst.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/systypes.rst.txt
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_sources/test.rst.txt
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/alabaster.css
--rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/doctools.js
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/file.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/plus.png
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 philander-0.1.8/doc/api/html/_static/underscore.js
--rw-r--r--   0        0        0   276792 2020-02-02 00:00:00.000000 philander-0.1.8/doc/uml/philander.aird
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 philander-0.1.8/doc/uml/philander.ecore
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 philander-0.1.8/philander/__init__.py
--rw-r--r--   0        0        0   116874 2020-02-02 00:00:00.000000 philander-0.1.8/philander/_bma456_feature.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 philander-0.1.8/philander/accelerometer.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 philander-0.1.8/philander/battery.py
--rw-r--r--   0        0        0    82563 2020-02-02 00:00:00.000000 philander-0.1.8/philander/bma456.py
--rw-r--r--   0        0        0    53191 2020-02-02 00:00:00.000000 philander-0.1.8/philander/bma456_reg.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 philander-0.1.8/philander/button.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 philander-0.1.8/philander/charger.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 philander-0.1.8/philander/configurable.py
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 philander-0.1.8/philander/dictionary.py
--rw-r--r--   0        0        0     9178 2020-02-02 00:00:00.000000 philander-0.1.8/philander/gasgauge.py
--rw-r--r--   0        0        0    23143 2020-02-02 00:00:00.000000 philander-0.1.8/philander/gpio.py
--rw-r--r--   0        0        0    16476 2020-02-02 00:00:00.000000 philander-0.1.8/philander/htu21d.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 philander-0.1.8/philander/hygrometer.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 philander-0.1.8/philander/imath.py
--rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 philander-0.1.8/philander/interruptable.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 philander-0.1.8/philander/led.py
--rw-r--r--   0        0        0    51566 2020-02-02 00:00:00.000000 philander-0.1.8/philander/max77960.py
--rw-r--r--   0        0        0    39765 2020-02-02 00:00:00.000000 philander-0.1.8/philander/max77960_reg.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 philander-0.1.8/philander/module.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 philander-0.1.8/philander/primitives.py
--rw-r--r--   0        0        0    26759 2020-02-02 00:00:00.000000 philander-0.1.8/philander/sensor.py
--rw-r--r--   0        0        0    59754 2020-02-02 00:00:00.000000 philander-0.1.8/philander/serialbus.py
--rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 philander-0.1.8/philander/simBMA456.py
--rw-r--r--   0        0        0    18518 2020-02-02 00:00:00.000000 philander-0.1.8/philander/simdev.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 philander-0.1.8/philander/systypes.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 philander-0.1.8/philander/thermometer.py
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 philander-0.1.8/philander/vibrasense.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 philander-0.1.8/philander/vibrasense2.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 philander-0.1.8/philander/voltmeter.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 philander-0.1.8/philander/watchdog.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 philander-0.1.8/philander/fastgait/__init__.py
--rw-r--r--   0        0        0    20466 2020-02-02 00:00:00.000000 philander-0.1.8/philander/fastgait/actorunit.py
--rw-r--r--   0        0        0    21356 2020-02-02 00:00:00.000000 philander-0.1.8/philander/fastgait/sysman.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 philander-0.1.8/test/utgpio.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 philander-0.1.8/test/utimath.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 philander-0.1.8/test/utserialbus.py
--rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 philander-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 philander-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 philander-0.1.8/readme.md
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 philander-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 philander-0.1.9/.buildpath
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 philander-0.1.9/.project
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.9/.pydevproject
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 philander-0.1.9/.externalToolBuilders/Build Dist.launch
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 philander-0.1.9/.externalToolBuilders/Sphinx API Doc.launch
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 philander-0.1.9/.externalToolBuilders/Sphinx Doc Build.launch
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 philander-0.1.9/.settings/org.eclipse.core.resources.prefs
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 philander-0.1.9/.settings/org.eclipse.ltk.core.refactoring.prefs
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/conf.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/modules.rst
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/philander.fastgait.rst
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/philander.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.buildinfo
+-rw-r--r--   0        0        0   281311 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/genindex.html
+-rw-r--r--   0        0        0    23481 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/gpio.html
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/index.html
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/interruptable.html
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/module.html
+-rw-r--r--   0        0        0   457028 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/modules.html
+-rw-r--r--   0        0        0    10531 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/objects.inv
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/philander.fastgait.html
+-rw-r--r--   0        0        0  1347605 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/philander.html
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/py-modindex.html
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/search.html
+-rw-r--r--   0        0        0   362717 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/searchindex.js
+-rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/systypes.html
+-rw-r--r--   0        0        0    29332 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/test.html
+-rw-r--r--   0        0        0  1894126 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    61929 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/gpio.doctree
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/index.doctree
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/interruptable.doctree
+-rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/module.doctree
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/modules.doctree
+-rw-r--r--   0        0        0  3592562 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/philander.doctree
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/philander.fastgait.doctree
+-rw-r--r--   0        0        0    50137 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/systypes.doctree
+-rw-r--r--   0        0        0    76214 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/test.doctree
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/doc/api/index.doctree
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/doc/api/modules.doctree
+-rw-r--r--   0        0        0   138640 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/.doctrees/doc/api/philander.doctree
+-rw-r--r--   0        0        0    26728 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/dictionary.html
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/index.html
+-rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/sensor.html
+-rw-r--r--   0        0        0    13313 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/systypes.html
+-rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/Configurable.html
+-rw-r--r--   0        0        0    21369 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/Device.html
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/EventHandler.html
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/FuelGauge.html
+-rw-r--r--   0        0        0    61389 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/Sensor.html
+-rw-r--r--   0        0        0   115813 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/Serial_Bus.html
+-rw-r--r--   0        0        0    13711 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/Watchdog.html
+-rw-r--r--   0        0        0    23313 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/accelerometer.html
+-rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/battery.html
+-rw-r--r--   0        0        0   260186 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/bma456.html
+-rw-r--r--   0        0        0   123528 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/bma456_reg.html
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/button.html
+-rw-r--r--   0        0        0    38699 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/charger.html
+-rw-r--r--   0        0        0    27732 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/dictionary.html
+-rw-r--r--   0        0        0    28007 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/gasgauge.html
+-rw-r--r--   0        0        0    81813 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/gpio.html
+-rw-r--r--   0        0        0    60743 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/htu21d.html
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/hygrometer.html
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/imath.html
+-rw-r--r--   0        0        0    30184 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/interruptable.html
+-rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/led.html
+-rw-r--r--   0        0        0   186098 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/max77960.html
+-rw-r--r--   0        0        0   118450 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/max77960_reg.html
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/module.html
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/primitives.html
+-rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/sbsimBMA456.html
+-rw-r--r--   0        0        0   181688 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/serialbus.html
+-rw-r--r--   0        0        0    48037 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/simBMA456.html
+-rw-r--r--   0        0        0    44466 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/simbus.html
+-rw-r--r--   0        0        0    50492 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/simdev.html
+-rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/systypes.html
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/thermometer.html
+-rw-r--r--   0        0        0    19853 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/vibrasense.html
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/vibrasense2.html
+-rw-r--r--   0        0        0    19228 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/voltmeter.html
+-rw-r--r--   0        0        0    70844 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_modules/philander/fastgait/actorunit.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/gpio.rst.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/interruptable.rst.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/module.rst.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/philander.fastgait.rst.txt
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/philander.rst.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/systypes.rst.txt
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_sources/test.rst.txt
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/doctools.js
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/file.png
+-rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/plus.png
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 philander-0.1.9/doc/api/html/_static/underscore.js
+-rw-r--r--   0        0        0   276792 2020-02-02 00:00:00.000000 philander-0.1.9/doc/uml/philander.aird
+-rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 philander-0.1.9/doc/uml/philander.ecore
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 philander-0.1.9/philander/__init__.py
+-rw-r--r--   0        0        0   116874 2020-02-02 00:00:00.000000 philander-0.1.9/philander/_bma456_feature.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 philander-0.1.9/philander/accelerometer.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 philander-0.1.9/philander/battery.py
+-rw-r--r--   0        0        0    82563 2020-02-02 00:00:00.000000 philander-0.1.9/philander/bma456.py
+-rw-r--r--   0        0        0    53191 2020-02-02 00:00:00.000000 philander-0.1.9/philander/bma456_reg.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 philander-0.1.9/philander/button.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 philander-0.1.9/philander/charger.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 philander-0.1.9/philander/configurable.py
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 philander-0.1.9/philander/dictionary.py
+-rw-r--r--   0        0        0     9178 2020-02-02 00:00:00.000000 philander-0.1.9/philander/gasgauge.py
+-rw-r--r--   0        0        0    23143 2020-02-02 00:00:00.000000 philander-0.1.9/philander/gpio.py
+-rw-r--r--   0        0        0    16476 2020-02-02 00:00:00.000000 philander-0.1.9/philander/htu21d.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 philander-0.1.9/philander/hygrometer.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 philander-0.1.9/philander/imath.py
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 philander-0.1.9/philander/interruptable.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 philander-0.1.9/philander/led.py
+-rw-r--r--   0        0        0    51566 2020-02-02 00:00:00.000000 philander-0.1.9/philander/max77960.py
+-rw-r--r--   0        0        0    39765 2020-02-02 00:00:00.000000 philander-0.1.9/philander/max77960_reg.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 philander-0.1.9/philander/module.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 philander-0.1.9/philander/primitives.py
+-rw-r--r--   0        0        0    26759 2020-02-02 00:00:00.000000 philander-0.1.9/philander/sensor.py
+-rw-r--r--   0        0        0    59754 2020-02-02 00:00:00.000000 philander-0.1.9/philander/serialbus.py
+-rw-r--r--   0        0        0    14379 2020-02-02 00:00:00.000000 philander-0.1.9/philander/simBMA456.py
+-rw-r--r--   0        0        0    18518 2020-02-02 00:00:00.000000 philander-0.1.9/philander/simdev.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 philander-0.1.9/philander/systypes.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 philander-0.1.9/philander/thermometer.py
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 philander-0.1.9/philander/vibrasense.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 philander-0.1.9/philander/vibrasense2.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 philander-0.1.9/philander/voltmeter.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 philander-0.1.9/philander/watchdog.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 philander-0.1.9/philander/fastgait/__init__.py
+-rw-r--r--   0        0        0    20466 2020-02-02 00:00:00.000000 philander-0.1.9/philander/fastgait/actorunit.py
+-rw-r--r--   0        0        0    21356 2020-02-02 00:00:00.000000 philander-0.1.9/philander/fastgait/sysman.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 philander-0.1.9/test/utgpio.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 philander-0.1.9/test/utimath.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 philander-0.1.9/test/utserialbus.py
+-rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 philander-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 philander-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 philander-0.1.9/readme.md
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 philander-0.1.9/PKG-INFO
```

### Comparing `philander-0.1.8/.project` & `philander-0.1.9/.project`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/.pydevproject` & `philander-0.1.9/.pydevproject`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/.externalToolBuilders/Build Dist.launch` & `philander-0.1.9/.externalToolBuilders/Build Dist.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/.externalToolBuilders/Sphinx API Doc.launch` & `philander-0.1.9/.externalToolBuilders/Sphinx API Doc.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/.externalToolBuilders/Sphinx Doc Build.launch` & `philander-0.1.9/.externalToolBuilders/Sphinx Doc Build.launch`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/conf.py` & `philander-0.1.9/doc/api/conf.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/philander.fastgait.rst` & `philander-0.1.9/doc/api/philander.fastgait.rst`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/philander.rst` & `philander-0.1.9/doc/api/philander.rst`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/genindex.html` & `philander-0.1.9/doc/api/html/genindex.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/gpio.html` & `philander-0.1.9/doc/api/html/gpio.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/index.html` & `philander-0.1.9/doc/api/html/index.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/interruptable.html` & `philander-0.1.9/doc/api/html/interruptable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/module.html` & `philander-0.1.9/doc/api/html/module.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/modules.html` & `philander-0.1.9/doc/api/html/modules.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/objects.inv` & `philander-0.1.9/doc/api/html/objects.inv`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/philander.fastgait.html` & `philander-0.1.9/doc/api/html/philander.fastgait.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/philander.html` & `philander-0.1.9/doc/api/html/philander.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/py-modindex.html` & `philander-0.1.9/doc/api/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/search.html` & `philander-0.1.9/doc/api/html/search.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/searchindex.js` & `philander-0.1.9/doc/api/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/systypes.html` & `philander-0.1.9/doc/api/html/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/test.html` & `philander-0.1.9/doc/api/html/test.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/gpio.doctree` & `philander-0.1.9/doc/api/html/.doctrees/gpio.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/index.doctree` & `philander-0.1.9/doc/api/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/interruptable.doctree` & `philander-0.1.9/doc/api/html/.doctrees/interruptable.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/module.doctree` & `philander-0.1.9/doc/api/html/.doctrees/module.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/modules.doctree` & `philander-0.1.9/doc/api/html/.doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/philander.doctree` & `philander-0.1.9/doc/api/html/.doctrees/philander.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/philander.fastgait.doctree` & `philander-0.1.9/doc/api/html/.doctrees/philander.fastgait.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/systypes.doctree` & `philander-0.1.9/doc/api/html/.doctrees/systypes.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/test.doctree` & `philander-0.1.9/doc/api/html/.doctrees/test.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/doc/api/index.doctree` & `philander-0.1.9/doc/api/html/.doctrees/doc/api/index.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/doc/api/modules.doctree` & `philander-0.1.9/doc/api/html/.doctrees/doc/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/.doctrees/doc/api/philander.doctree` & `philander-0.1.9/doc/api/html/.doctrees/doc/api/philander.doctree`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/dictionary.html` & `philander-0.1.9/doc/api/html/_modules/dictionary.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/index.html` & `philander-0.1.9/doc/api/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/sensor.html` & `philander-0.1.9/doc/api/html/_modules/sensor.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/systypes.html` & `philander-0.1.9/doc/api/html/_modules/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/Configurable.html` & `philander-0.1.9/doc/api/html/_modules/philander/Configurable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/Device.html` & `philander-0.1.9/doc/api/html/_modules/philander/Device.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/EventHandler.html` & `philander-0.1.9/doc/api/html/_modules/philander/EventHandler.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/FuelGauge.html` & `philander-0.1.9/doc/api/html/_modules/philander/FuelGauge.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/Sensor.html` & `philander-0.1.9/doc/api/html/_modules/philander/Sensor.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/Serial_Bus.html` & `philander-0.1.9/doc/api/html/_modules/philander/Serial_Bus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/Watchdog.html` & `philander-0.1.9/doc/api/html/_modules/philander/Watchdog.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/accelerometer.html` & `philander-0.1.9/doc/api/html/_modules/philander/accelerometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/battery.html` & `philander-0.1.9/doc/api/html/_modules/philander/battery.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/bma456.html` & `philander-0.1.9/doc/api/html/_modules/philander/bma456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/bma456_reg.html` & `philander-0.1.9/doc/api/html/_modules/philander/bma456_reg.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/button.html` & `philander-0.1.9/doc/api/html/_modules/philander/button.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/charger.html` & `philander-0.1.9/doc/api/html/_modules/philander/charger.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/dictionary.html` & `philander-0.1.9/doc/api/html/_modules/philander/dictionary.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/gasgauge.html` & `philander-0.1.9/doc/api/html/_modules/philander/gasgauge.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/gpio.html` & `philander-0.1.9/doc/api/html/_modules/philander/gpio.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/htu21d.html` & `philander-0.1.9/doc/api/html/_modules/philander/htu21d.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/hygrometer.html` & `philander-0.1.9/doc/api/html/_modules/philander/hygrometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/imath.html` & `philander-0.1.9/doc/api/html/_modules/philander/imath.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/interruptable.html` & `philander-0.1.9/doc/api/html/_modules/philander/interruptable.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/led.html` & `philander-0.1.9/doc/api/html/_modules/philander/led.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/max77960.html` & `philander-0.1.9/doc/api/html/_modules/philander/max77960.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/max77960_reg.html` & `philander-0.1.9/doc/api/html/_modules/philander/max77960_reg.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/module.html` & `philander-0.1.9/doc/api/html/_modules/philander/module.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/primitives.html` & `philander-0.1.9/doc/api/html/_modules/philander/primitives.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/sbsimBMA456.html` & `philander-0.1.9/doc/api/html/_modules/philander/sbsimBMA456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/serialbus.html` & `philander-0.1.9/doc/api/html/_modules/philander/serialbus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/simBMA456.html` & `philander-0.1.9/doc/api/html/_modules/philander/simBMA456.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/simbus.html` & `philander-0.1.9/doc/api/html/_modules/philander/simbus.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/simdev.html` & `philander-0.1.9/doc/api/html/_modules/philander/simdev.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/systypes.html` & `philander-0.1.9/doc/api/html/_modules/philander/systypes.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/thermometer.html` & `philander-0.1.9/doc/api/html/_modules/philander/thermometer.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/vibrasense.html` & `philander-0.1.9/doc/api/html/_modules/philander/vibrasense.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/vibrasense2.html` & `philander-0.1.9/doc/api/html/_modules/philander/vibrasense2.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/voltmeter.html` & `philander-0.1.9/doc/api/html/_modules/philander/voltmeter.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_modules/philander/fastgait/actorunit.html` & `philander-0.1.9/doc/api/html/_modules/philander/fastgait/actorunit.html`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_sources/philander.fastgait.rst.txt` & `philander-0.1.9/doc/api/html/_sources/philander.fastgait.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_sources/philander.rst.txt` & `philander-0.1.9/doc/api/html/_sources/philander.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_sources/test.rst.txt` & `philander-0.1.9/doc/api/html/_sources/test.rst.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js` & `philander-0.1.9/doc/api/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/alabaster.css` & `philander-0.1.9/doc/api/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/basic.css` & `philander-0.1.9/doc/api/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/doctools.js` & `philander-0.1.9/doc/api/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/jquery-3.6.0.js` & `philander-0.1.9/doc/api/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/jquery.js` & `philander-0.1.9/doc/api/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/language_data.js` & `philander-0.1.9/doc/api/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/pygments.css` & `philander-0.1.9/doc/api/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/searchtools.js` & `philander-0.1.9/doc/api/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/sphinx_highlight.js` & `philander-0.1.9/doc/api/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/underscore-1.13.1.js` & `philander-0.1.9/doc/api/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/api/html/_static/underscore.js` & `philander-0.1.9/doc/api/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/uml/philander.aird` & `philander-0.1.9/doc/uml/philander.aird`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/doc/uml/philander.ecore` & `philander-0.1.9/doc/uml/philander.ecore`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/__init__.py` & `philander-0.1.9/philander/__init__.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/_bma456_feature.py` & `philander-0.1.9/philander/_bma456_feature.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/accelerometer.py` & `philander-0.1.9/philander/accelerometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/battery.py` & `philander-0.1.9/philander/battery.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/bma456.py` & `philander-0.1.9/philander/bma456.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/bma456_reg.py` & `philander-0.1.9/philander/bma456_reg.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/button.py` & `philander-0.1.9/philander/button.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/charger.py` & `philander-0.1.9/philander/charger.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/configurable.py` & `philander-0.1.9/philander/configurable.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/dictionary.py` & `philander-0.1.9/philander/dictionary.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/gasgauge.py` & `philander-0.1.9/philander/gasgauge.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/gpio.py` & `philander-0.1.9/philander/gpio.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/htu21d.py` & `philander-0.1.9/philander/htu21d.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/hygrometer.py` & `philander-0.1.9/philander/hygrometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/imath.py` & `philander-0.1.9/philander/imath.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/interruptable.py` & `philander-0.1.9/philander/interruptable.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/led.py` & `philander-0.1.9/philander/led.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/max77960.py` & `philander-0.1.9/philander/max77960.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/max77960_reg.py` & `philander-0.1.9/philander/max77960_reg.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/module.py` & `philander-0.1.9/philander/module.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/primitives.py` & `philander-0.1.9/philander/primitives.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/sensor.py` & `philander-0.1.9/philander/sensor.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/serialbus.py` & `philander-0.1.9/philander/serialbus.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/simBMA456.py` & `philander-0.1.9/philander/simBMA456.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/simdev.py` & `philander-0.1.9/philander/simdev.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/systypes.py` & `philander-0.1.9/philander/systypes.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/thermometer.py` & `philander-0.1.9/philander/thermometer.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/vibrasense.py` & `philander-0.1.9/philander/vibrasense.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/vibrasense2.py` & `philander-0.1.9/philander/vibrasense2.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/voltmeter.py` & `philander-0.1.9/philander/voltmeter.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/watchdog.py` & `philander-0.1.9/philander/watchdog.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/fastgait/__init__.py` & `philander-0.1.9/philander/fastgait/__init__.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/fastgait/actorunit.py` & `philander-0.1.9/philander/fastgait/actorunit.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/philander/fastgait/sysman.py` & `philander-0.1.9/philander/fastgait/sysman.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/test/utgpio.py` & `philander-0.1.9/test/utgpio.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/test/utimath.py` & `philander-0.1.9/test/utimath.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/test/utserialbus.py` & `philander-0.1.9/test/utserialbus.py`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/LICENSE.txt` & `philander-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `philander-0.1.8/pyproject.toml` & `philander-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "philander"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Oliver Maye", email="maye@ihp-microelectronics.com" },
 ]
 description = "Sensor and other parts driver collection"
 readme = "readme.md"
 requires-python = ">=3.0"
 classifiers = [
@@ -28,9 +28,8 @@
 
 [project.optional-dependencies]
 optSerial = [
   "smbus2",
 ]
 optGPIO = [
   "RPi.GPIO",
-  "gpiozero",
 ]
```

### Comparing `philander-0.1.8/PKG-INFO` & `philander-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: philander
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sensor and other parts driver collection
 Project-URL: Homepage, https://www.ihp-microelectronics.com/
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Oliver Maye <maye@ihp-microelectronics.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Requires-Dist: pymitter
 Requires-Dist: python-periphery
 Requires-Dist: smbus2
 Provides-Extra: optgpio
-Requires-Dist: gpiozero; extra == 'optgpio'
 Requires-Dist: rpi-gpio; extra == 'optgpio'
 Provides-Extra: optserial
 Requires-Dist: smbus2; extra == 'optserial'
 Description-Content-Type: text/markdown
 
 # The philander package
```

