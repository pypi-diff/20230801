# Comparing `tmp/flappy-bird-env-0.1.5.tar.gz` & `tmp/flappy-bird-env-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flappy-bird-env-0.1.5.tar", last modified: Mon Jun 26 17:57:29 2023, max compression
+gzip compressed data, was "flappy-bird-env-0.1.6.tar", last modified: Tue Aug  1 12:03:31 2023, max compression
```

## Comparing `flappy-bird-env-0.1.5.tar` & `flappy-bird-env-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:57:29.127245 flappy-bird-env-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-26 17:57:29.127245 flappy-bird-env-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:57:29.127245 flappy-bird-env-0.1.5/flappy_bird_env/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/background.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/bird.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/drawable.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/flappy_bird.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:57:29.127245 flappy-bird-env-0.1.5/flappy_bird_env/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/images/background.png
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/images/base.png
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/images/downflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/images/midflap.png
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/images/pipe.png
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/images/upflap.png
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/movable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/flappy_bird_env/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:57:29.127245 flappy-bird-env-0.1.5/flappy_bird_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-26 17:57:29.000000 flappy-bird-env-0.1.5/flappy_bird_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-26 17:57:29.000000 flappy-bird-env-0.1.5/flappy_bird_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:57:29.000000 flappy-bird-env-0.1.5/flappy_bird_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 17:57:29.000000 flappy-bird-env-0.1.5/flappy_bird_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 17:57:29.000000 flappy-bird-env-0.1.5/flappy_bird_env.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-26 17:57:19.000000 flappy-bird-env-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:57:29.127245 flappy-bird-env-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:03:31.242448 flappy-bird-env-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 12:03:21.000000 flappy-bird-env-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 12:03:21.000000 flappy-bird-env-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-08-01 12:03:31.242448 flappy-bird-env-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-01 12:03:21.000000 flappy-bird-env-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:03:31.242448 flappy-bird-env-0.1.6/flappy_bird_env/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/bird.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/drawable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/flappy_bird_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:03:31.242448 flappy-bird-env-0.1.6/flappy_bird_env/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/images/background.png
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/images/base.png
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/images/downflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/images/midflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/images/pipe.png
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/images/upflap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/movable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/flappy_bird_env/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:03:31.242448 flappy-bird-env-0.1.6/flappy_bird_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-08-01 12:03:31.000000 flappy-bird-env-0.1.6/flappy_bird_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 12:03:31.000000 flappy-bird-env-0.1.6/flappy_bird_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:03:31.000000 flappy-bird-env-0.1.6/flappy_bird_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 12:03:31.000000 flappy-bird-env-0.1.6/flappy_bird_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 12:03:31.000000 flappy-bird-env-0.1.6/flappy_bird_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-01 12:03:22.000000 flappy-bird-env-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:03:31.242448 flappy-bird-env-0.1.6/setup.cfg
```

### Comparing `flappy-bird-env-0.1.5/LICENSE` & `flappy-bird-env-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flappy-bird-env-0.1.5/PKG-INFO` & `flappy-bird-env-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flappy-bird-env
-Version: 0.1.5
+Version: 0.1.6
 Summary: Flappy Bird as a Farama Gymnasium environment.
 Author-email: Roberto Schiavone <hello@robertoschiavone.io>
 Maintainer-email: Roberto Schiavone <hello@robertoschiavone.io>
 License: MIT License
         
         Copyright (c) 2023 Roberto Schiavone
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flappy-bird-env Version: 0.1.5 Summary: Flappy Bird
+Metadata-Version: 2.1 Name: flappy-bird-env Version: 0.1.6 Summary: Flappy Bird
 as a Farama Gymnasium environment. Author-email: Roberto Schiavone
 robertoschiavone.io> Maintainer-email: Roberto Schiavone
 robertoschiavone.io> License: MIT License Copyright (c) 2023 Roberto Schiavone
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `flappy-bird-env-0.1.5/README.md` & `flappy-bird-env-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env/base.py` & `flappy-bird-env-0.1.6/flappy_bird_env/base.py`

 * *Files identical despite different names*

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env/bird.py` & `flappy-bird-env-0.1.6/flappy_bird_env/bird.py`

 * *Files identical despite different names*

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env/flappy_bird.py` & `flappy-bird-env-0.1.6/flappy_bird_env/flappy_bird_env.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from typing import Any, Dict, List, SupportsFloat, Tuple
+from gymnasium.core import ActType, ObsType, RenderFrame
+
 import functools
 
 import gymnasium as gym
 import numpy as np
 import pygame
 
-from typing import Any, Dict, List, SupportsFloat, Tuple
-
-from gymnasium.core import ActType, ObsType, RenderFrame
 from gymnasium.spaces import Box, Discrete
 
 from .background import Background
 from .base import Base
 from .bird import Bird
 from .pipe import Pipe
```

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env/images/background.png` & `flappy-bird-env-0.1.6/flappy_bird_env/images/background.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env/images/pipe.png` & `flappy-bird-env-0.1.6/flappy_bird_env/images/pipe.png`

 * *Files identical despite different names*

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env/pipe.py` & `flappy-bird-env-0.1.6/flappy_bird_env/pipe.py`

 * *Files identical despite different names*

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env.egg-info/PKG-INFO` & `flappy-bird-env-0.1.6/flappy_bird_env.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flappy-bird-env
-Version: 0.1.5
+Version: 0.1.6
 Summary: Flappy Bird as a Farama Gymnasium environment.
 Author-email: Roberto Schiavone <hello@robertoschiavone.io>
 Maintainer-email: Roberto Schiavone <hello@robertoschiavone.io>
 License: MIT License
         
         Copyright (c) 2023 Roberto Schiavone
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flappy-bird-env Version: 0.1.5 Summary: Flappy Bird
+Metadata-Version: 2.1 Name: flappy-bird-env Version: 0.1.6 Summary: Flappy Bird
 as a Farama Gymnasium environment. Author-email: Roberto Schiavone
 robertoschiavone.io> Maintainer-email: Roberto Schiavone
 robertoschiavone.io> License: MIT License Copyright (c) 2023 Roberto Schiavone
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `flappy-bird-env-0.1.5/flappy_bird_env.egg-info/SOURCES.txt` & `flappy-bird-env-0.1.6/flappy_bird_env.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pyproject.toml
 flappy_bird_env/__init__.py
 flappy_bird_env/__main__.py
 flappy_bird_env/background.py
 flappy_bird_env/base.py
 flappy_bird_env/bird.py
 flappy_bird_env/drawable.py
-flappy_bird_env/flappy_bird.py
+flappy_bird_env/flappy_bird_env.py
 flappy_bird_env/movable.py
 flappy_bird_env/pipe.py
 flappy_bird_env.egg-info/PKG-INFO
 flappy_bird_env.egg-info/SOURCES.txt
 flappy_bird_env.egg-info/dependency_links.txt
 flappy_bird_env.egg-info/requires.txt
 flappy_bird_env.egg-info/top_level.txt
```

### Comparing `flappy-bird-env-0.1.5/pyproject.toml` & `flappy-bird-env-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flappy-bird-env"
-version = "0.1.5"
+version = "0.1.6"
 description = """Flappy Bird as a Farama Gymnasium environment."""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 authors = [
     { name = "Roberto Schiavone", email = "hello@robertoschiavone.io" },
 ]
@@ -14,17 +14,17 @@
 keywords = ["flappy-bird", "gymnasium", "reinforcement-learning"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries"
 ]
 dependencies = [
-    "gymnasium ~= 0.28.1",
-    "numpy ~= 1.25.0",
-    "pygame ~= 2.4.0"
+    "gymnasium ~= 0.29.0",
+    "numpy ~= 1.25.2",
+    "pygame ~= 2.5.0"
 ]
 
 [build-system]
 requires = ["setuptools ~= 65.5.0"]
 
 [project.urls]
 homepage = "https://github.com/robertoschiavone/flappy-bird-env"
```

