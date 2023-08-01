# Comparing `tmp/perplexityai-1.0.0.tar.gz` & `tmp/perplexityai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perplexityai-1.0.0.tar", last modified: Tue Aug  1 16:14:05 2023, max compression
+gzip compressed data, was "perplexityai-1.0.1.tar", last modified: Tue Aug  1 16:28:02 2023, max compression
```

## Comparing `perplexityai-1.0.0.tar` & `perplexityai-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 16:14:05.876328 perplexityai-1.0.0/
--rw-rw-rw-   0        0        0    18092 2023-08-01 16:12:32.000000 perplexityai-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2171 2023-08-01 16:14:05.875344 perplexityai-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      955 2023-08-01 16:12:32.000000 perplexityai-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 16:14:05.855335 perplexityai-1.0.0/perplexityai/
--rw-rw-rw-   0        0        0      103 2023-08-01 16:12:32.000000 perplexityai-1.0.0/perplexityai/__init__.py
--rw-rw-rw-   0        0        0     6380 2023-08-01 16:12:32.000000 perplexityai-1.0.0/perplexityai/perplexity.py
-drwxrwxrwx   0        0        0        0 2023-08-01 16:14:05.873338 perplexityai-1.0.0/perplexityai.egg-info/
--rw-rw-rw-   0        0        0     2171 2023-08-01 16:14:05.000000 perplexityai-1.0.0/perplexityai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-08-01 16:14:05.000000 perplexityai-1.0.0/perplexityai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 16:14:05.000000 perplexityai-1.0.0/perplexityai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-08-01 16:14:05.000000 perplexityai-1.0.0/perplexityai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-01 16:14:05.000000 perplexityai-1.0.0/perplexityai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 16:14:05.877329 perplexityai-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-08-01 16:12:32.000000 perplexityai-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:28:02.920453 perplexityai-1.0.1/
+-rw-rw-rw-   0        0        0    18092 2023-08-01 16:26:58.000000 perplexityai-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2479 2023-08-01 16:28:02.920453 perplexityai-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-08-01 16:26:58.000000 perplexityai-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 16:28:02.920453 perplexityai-1.0.1/perplexityai/
+-rw-rw-rw-   0        0        0     6424 2023-08-01 16:26:58.000000 perplexityai-1.0.1/perplexityai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:28:02.920453 perplexityai-1.0.1/perplexityai.egg-info/
+-rw-rw-rw-   0        0        0     2479 2023-08-01 16:28:02.000000 perplexityai-1.0.1/perplexityai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-01 16:28:02.000000 perplexityai-1.0.1/perplexityai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 16:28:02.000000 perplexityai-1.0.1/perplexityai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-08-01 16:28:02.000000 perplexityai-1.0.1/perplexityai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 16:28:02.000000 perplexityai-1.0.1/perplexityai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 16:28:02.920453 perplexityai-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1578 2023-08-01 16:26:58.000000 perplexityai-1.0.1/setup.py
```

### Comparing `perplexityai-1.0.0/LICENSE` & `perplexityai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perplexityai-1.0.0/PKG-INFO` & `perplexityai-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: perplexityai
-Version: 1.0.0
+Version: 1.0.1
 Summary: A better, simpler and faster version of nathanrchn's perplexityai.
 Home-page: https://github.com/Ruu3f/perplexityai
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/perplexityai
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
-Keywords: artificial-intelligence,machine-learning,deep-learning,perplexityai,python,ai
+Keywords: artificial-intelligence,machine-learning,deep-learning,perplexityai,perplexity,python,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,15 +20,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PerplexityAI
+[![PyPI](https://img.shields.io/pypi/v/perplexityai)](https://pypi.org/project/perplexityai)
+[![Downloads](https://static.pepy.tech/badge/perplexityai)](https://pypi.org/project/perplexityai)
+[![Status](https://img.shields.io/pypi/status/perplexityai)](https://pypi.org/project/perplexityai)
+
+# perplexityai
 
 A better, simpler, and faster version of nathanrchn's PerplexityAI.
 
 ## Get started:
 
 ```
 python -m pip install -U perplexityai
```

### Comparing `perplexityai-1.0.0/README.md` & `perplexityai-1.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# PerplexityAI
+[![PyPI](https://img.shields.io/pypi/v/perplexityai)](https://pypi.org/project/perplexityai)
+[![Downloads](https://static.pepy.tech/badge/perplexityai)](https://pypi.org/project/perplexityai)
+[![Status](https://img.shields.io/pypi/status/perplexityai)](https://pypi.org/project/perplexityai)
+
+# perplexityai
 
 A better, simpler, and faster version of nathanrchn's PerplexityAI.
 
 ## Get started:
 
 ```
 python -m pip install -U perplexityai
```

### Comparing `perplexityai-1.0.0/perplexityai/perplexity.py` & `perplexityai-1.0.1/perplexityai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+__author__ = "Ruu3f"
+__version__ = "1.0.1"
+
 from time import sleep
 from uuid import uuid4
 from requests import Session
 from threading import Thread
 from json import loads, dumps
 from random import getrandbits
 from websocket import WebSocketApp
```

### Comparing `perplexityai-1.0.0/perplexityai.egg-info/PKG-INFO` & `perplexityai-1.0.1/perplexityai.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: perplexityai
-Version: 1.0.0
+Version: 1.0.1
 Summary: A better, simpler and faster version of nathanrchn's perplexityai.
 Home-page: https://github.com/Ruu3f/perplexityai
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/perplexityai
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
-Keywords: artificial-intelligence,machine-learning,deep-learning,perplexityai,python,ai
+Keywords: artificial-intelligence,machine-learning,deep-learning,perplexityai,perplexity,python,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,15 +20,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PerplexityAI
+[![PyPI](https://img.shields.io/pypi/v/perplexityai)](https://pypi.org/project/perplexityai)
+[![Downloads](https://static.pepy.tech/badge/perplexityai)](https://pypi.org/project/perplexityai)
+[![Status](https://img.shields.io/pypi/status/perplexityai)](https://pypi.org/project/perplexityai)
+
+# perplexityai
 
 A better, simpler, and faster version of nathanrchn's PerplexityAI.
 
 ## Get started:
 
 ```
 python -m pip install -U perplexityai
```

### Comparing `perplexityai-1.0.0/setup.py` & `perplexityai-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="perplexityai",
-    version="1.0.0",
+    version="1.0.1",
     description="A better, simpler and faster version of nathanrchn's perplexityai.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/perplexityai",
     author="Ruu3f",
     license="GPLv2",
     keywords=[
         "artificial-intelligence",
         "machine-learning",
         "deep-learning",
         "perplexityai",
+        "perplexity",
         "python",
         "ai",
     ],
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

