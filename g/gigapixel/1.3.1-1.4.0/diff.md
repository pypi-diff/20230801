# Comparing `tmp/gigapixel-1.3.1.tar.gz` & `tmp/gigapixel-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigapixel-1.3.1.tar", last modified: Sat Apr 29 09:16:55 2023, max compression
+gzip compressed data, was "gigapixel-1.4.0.tar", last modified: Mon Jul 31 22:14:22 2023, max compression
```

## Comparing `gigapixel-1.3.1.tar` & `gigapixel-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:16:55.413786 gigapixel-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 09:16:42.000000 gigapixel-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-29 09:16:55.413786 gigapixel-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-29 09:16:42.000000 gigapixel-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:16:55.413786 gigapixel-1.3.1/gigapixel/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/gigapixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-29 09:16:42.000000 gigapixel-1.3.1/gigapixel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 09:16:55.413786 gigapixel-1.3.1/gigapixel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 09:16:55.000000 gigapixel-1.3.1/gigapixel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-29 09:16:42.000000 gigapixel-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-29 09:16:55.417786 gigapixel-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-29 09:16:42.000000 gigapixel-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:22.380162 gigapixel-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 22:14:08.000000 gigapixel-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-31 22:14:22.380162 gigapixel-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-31 22:14:08.000000 gigapixel-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:22.380162 gigapixel-1.4.0/gigapixel/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-31 22:14:08.000000 gigapixel-1.4.0/gigapixel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-31 22:14:08.000000 gigapixel-1.4.0/gigapixel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-31 22:14:08.000000 gigapixel-1.4.0/gigapixel/gigapixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-31 22:14:08.000000 gigapixel-1.4.0/gigapixel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:14:22.380162 gigapixel-1.4.0/gigapixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-31 22:14:22.000000 gigapixel-1.4.0/gigapixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-31 22:14:22.000000 gigapixel-1.4.0/gigapixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:14:22.000000 gigapixel-1.4.0/gigapixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 22:14:22.000000 gigapixel-1.4.0/gigapixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 22:14:22.000000 gigapixel-1.4.0/gigapixel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 22:14:08.000000 gigapixel-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 22:14:22.380162 gigapixel-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-31 22:14:08.000000 gigapixel-1.4.0/setup.py
```

### Comparing `gigapixel-1.3.1/LICENSE` & `gigapixel-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gigapixel-1.3.1/PKG-INFO` & `gigapixel-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigapixel
-Version: 1.3.1
+Version: 1.4.0
 Summary: Topaz Gigapixel AI automation tool
 Home-page: https://github.com/TimNekk/Gigapixel
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
   <a href="#usage">Usage</a> •
   <a href="#contributing">Contributing</a> •
   <a href="#license">License</a>
 </p>
 
 ## Requirements
 
-[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.3.3** or **newer** required
+[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.1.0** or **newer** required
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/gigapixel/)
 
 ```bash
 pip install -U gigapixel
@@ -76,20 +76,33 @@
 output_suffix = '-gigapixel'
 
 # Create Gigapixel instance.
 app = Gigapixel(exe_path, output_suffix)
 
 # Process image.
 image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+output_path = app.process(image)
 
 # Print output path.
 print(output_path)
 ```
 
+Additional parameters can be passed to `process()` method **(Takes additional time)**:
+```python
+from gigapixel import Scale, Mode, OutputFormat
+
+output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+```
+
+> **Warning!**
+> Using parameters (`scale`, `mode`, `output_format`, `delete_from_history`) will take **additional time** to process single image.
+> Consider using them only when needed.
+> To get the best performance, use `app.process(image)`
+
+
 ## Contributing
 
 Bug reports and/or pull requests are welcome
 
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gigapixel Version: 1.3.1 Summary: Topaz Gigapixel
+Metadata-Version: 2.1 Name: gigapixel Version: 1.4.0 Summary: Topaz Gigapixel
 AI automation tool Home-page: https://github.com/TimNekk/Gigapixel Author:
 TimNekk Author-email: herew26@gmail.com License: Apache License, Version 2.0,
 see LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -16,23 +16,28 @@
                                  [Gigapixel]
                                   Gigapixel
                                      ******
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
-**v6.3.3** or **newer** required ## Installation Install the current version
+**v6.1.0** or **newer** required ## Installation Install the current version
 with [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -
 U gigapixel ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()`
 method to enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
 OutputFormat from pathlib import Path # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
 Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
 You should set same value inside Gigapixel (File -> Preferences -> Default
 filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
 = Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
-image.jpg') output_path = app.process(image, scale=Scale.X2,
-mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG) #
-Print output path. print(output_path) ``` ## Contributing Bug reports and/or
-pull requests are welcome ## License The module is available as open source
-under the terms of the [Apache License, Version 2.0](https://opensource.org/
-licenses/Apache-2.0)
+image.jpg') output_path = app.process(image) # Print output path. print
+(output_path) ``` Additional parameters can be passed to `process()` method **
+(Takes additional time)**: ```python from gigapixel import Scale, Mode,
+OutputFormat output_path = app.process(image, scale=Scale.X2,
+mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+``` > **Warning!** > Using parameters (`scale`, `mode`, `output_format`,
+`delete_from_history`) will take **additional time** to process single image. >
+Consider using them only when needed. > To get the best performance, use
+`app.process(image)` ## Contributing Bug reports and/or pull requests are
+welcome ## License The module is available as open source under the terms of
+the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `gigapixel-1.3.1/README.md` & `gigapixel-1.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   <a href="#usage">Usage</a> •
   <a href="#contributing">Contributing</a> •
   <a href="#license">License</a>
 </p>
 
 ## Requirements
 
-[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.3.3** or **newer** required
+[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.1.0** or **newer** required
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/gigapixel/)
 
 ```bash
 pip install -U gigapixel
@@ -51,20 +51,33 @@
 output_suffix = '-gigapixel'
 
 # Create Gigapixel instance.
 app = Gigapixel(exe_path, output_suffix)
 
 # Process image.
 image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+output_path = app.process(image)
 
 # Print output path.
 print(output_path)
 ```
 
+Additional parameters can be passed to `process()` method **(Takes additional time)**:
+```python
+from gigapixel import Scale, Mode, OutputFormat
+
+output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+```
+
+> **Warning!**
+> Using parameters (`scale`, `mode`, `output_format`, `delete_from_history`) will take **additional time** to process single image.
+> Consider using them only when needed.
+> To get the best performance, use `app.process(image)`
+
+
 ## Contributing
 
 Bug reports and/or pull requests are welcome
 
 
 ## License
```

#### html2text {}

```diff
@@ -2,23 +2,28 @@
                                  [Gigapixel]
                                   Gigapixel
                                      ******
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
-**v6.3.3** or **newer** required ## Installation Install the current version
+**v6.1.0** or **newer** required ## Installation Install the current version
 with [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -
 U gigapixel ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()`
 method to enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
 OutputFormat from pathlib import Path # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
 Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
 You should set same value inside Gigapixel (File -> Preferences -> Default
 filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
 = Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
-image.jpg') output_path = app.process(image, scale=Scale.X2,
-mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG) #
-Print output path. print(output_path) ``` ## Contributing Bug reports and/or
-pull requests are welcome ## License The module is available as open source
-under the terms of the [Apache License, Version 2.0](https://opensource.org/
-licenses/Apache-2.0)
+image.jpg') output_path = app.process(image) # Print output path. print
+(output_path) ``` Additional parameters can be passed to `process()` method **
+(Takes additional time)**: ```python from gigapixel import Scale, Mode,
+OutputFormat output_path = app.process(image, scale=Scale.X2,
+mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+``` > **Warning!** > Using parameters (`scale`, `mode`, `output_format`,
+`delete_from_history`) will take **additional time** to process single image. >
+Consider using them only when needed. > To get the best performance, use
+`app.process(image)` ## Contributing Bug reports and/or pull requests are
+welcome ## License The module is available as open source under the terms of
+the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `gigapixel-1.3.1/gigapixel/logging.py` & `gigapixel-1.4.0/gigapixel/logging.py`

 * *Files identical despite different names*

### Comparing `gigapixel-1.3.1/gigapixel.egg-info/PKG-INFO` & `gigapixel-1.4.0/gigapixel.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigapixel
-Version: 1.3.1
+Version: 1.4.0
 Summary: Topaz Gigapixel AI automation tool
 Home-page: https://github.com/TimNekk/Gigapixel
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
   <a href="#usage">Usage</a> •
   <a href="#contributing">Contributing</a> •
   <a href="#license">License</a>
 </p>
 
 ## Requirements
 
-[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.3.3** or **newer** required
+[Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai) **v6.1.0** or **newer** required
 
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/gigapixel/)
 
 ```bash
 pip install -U gigapixel
@@ -76,20 +76,33 @@
 output_suffix = '-gigapixel'
 
 # Create Gigapixel instance.
 app = Gigapixel(exe_path, output_suffix)
 
 # Process image.
 image = Path('path/to/image.jpg')
-output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+output_path = app.process(image)
 
 # Print output path.
 print(output_path)
 ```
 
+Additional parameters can be passed to `process()` method **(Takes additional time)**:
+```python
+from gigapixel import Scale, Mode, OutputFormat
+
+output_path = app.process(image, scale=Scale.X2, mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+```
+
+> **Warning!**
+> Using parameters (`scale`, `mode`, `output_format`, `delete_from_history`) will take **additional time** to process single image.
+> Consider using them only when needed.
+> To get the best performance, use `app.process(image)`
+
+
 ## Contributing
 
 Bug reports and/or pull requests are welcome
 
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gigapixel Version: 1.3.1 Summary: Topaz Gigapixel
+Metadata-Version: 2.1 Name: gigapixel Version: 1.4.0 Summary: Topaz Gigapixel
 AI automation tool Home-page: https://github.com/TimNekk/Gigapixel Author:
 TimNekk Author-email: herew26@gmail.com License: Apache License, Version 2.0,
 see LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -16,23 +16,28 @@
                                  [Gigapixel]
                                   Gigapixel
                                      ******
                   *** Topaz Gigapixel AI automation tool ***
                            [PyPI] [Python 3] [Tests]
      Requirements â¢ Installation â¢ Usage â¢ Contributing â¢ License
 ## Requirements [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
-**v6.3.3** or **newer** required ## Installation Install the current version
+**v6.1.0** or **newer** required ## Installation Install the current version
 with [PyPI](https://pypi.org/project/gigapixel/) ```bash pip install -
 U gigapixel ``` ## Usage 1. Create `Gigapixel` instance 2. Use `.process()`
 method to enhance image ```python from gigapixel import Gigapixel, Scale, Mode,
 OutputFormat from pathlib import Path # Path to Gigapixel executable file.
 exe_path = Path('C:\Program Files\Topaz Labs LLC\Topaz Gigapixel AI\Topaz
 Gigapixel AI.exe') # Output file suffix. (e.g. pic.jpg -> pic-gigapixel.jpg) #
 You should set same value inside Gigapixel (File -> Preferences -> Default
 filename suffix). output_suffix = '-gigapixel' # Create Gigapixel instance. app
 = Gigapixel(exe_path, output_suffix) # Process image. image = Path('path/to/
-image.jpg') output_path = app.process(image, scale=Scale.X2,
-mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG) #
-Print output path. print(output_path) ``` ## Contributing Bug reports and/or
-pull requests are welcome ## License The module is available as open source
-under the terms of the [Apache License, Version 2.0](https://opensource.org/
-licenses/Apache-2.0)
+image.jpg') output_path = app.process(image) # Print output path. print
+(output_path) ``` Additional parameters can be passed to `process()` method **
+(Takes additional time)**: ```python from gigapixel import Scale, Mode,
+OutputFormat output_path = app.process(image, scale=Scale.X2,
+mode=Mode.STANDARD, delete_from_history=True, output_format=OutputFormat.PNG)
+``` > **Warning!** > Using parameters (`scale`, `mode`, `output_format`,
+`delete_from_history`) will take **additional time** to process single image. >
+Consider using them only when needed. > To get the best performance, use
+`app.process(image)` ## Contributing Bug reports and/or pull requests are
+welcome ## License The module is available as open source under the terms of
+the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `gigapixel-1.3.1/setup.py` & `gigapixel-1.4.0/setup.py`

 * *Files identical despite different names*

