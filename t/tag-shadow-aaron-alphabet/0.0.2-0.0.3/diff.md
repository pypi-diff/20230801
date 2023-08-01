# Comparing `tmp/tag-shadow-aaron-alphabet-0.0.2.tar.gz` & `tmp/tag-shadow-aaron-alphabet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tag-shadow-aaron-alphabet-0.0.2.tar", last modified: Thu Mar 30 22:10:41 2023, max compression
+gzip compressed data, was "tag-shadow-aaron-alphabet-0.0.3.tar", last modified: Tue Aug  1 12:14:12 2023, max compression
```

## Comparing `tag-shadow-aaron-alphabet-0.0.2.tar` & `tag-shadow-aaron-alphabet-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-30 22:10:41.935930 tag-shadow-aaron-alphabet-0.0.2/
--rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 tag-shadow-aaron-alphabet-0.0.2/LICENSE
--rw-rw-r--   0 lk        (1002) lk        (1002)     1479 2023-03-30 22:10:41.935930 tag-shadow-aaron-alphabet-0.0.2/PKG-INFO
--rwxrwxrwx   0 lk        (1002) lk        (1002)      530 2023-03-29 22:05:53.000000 tag-shadow-aaron-alphabet-0.0.2/pyproject.toml
--rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-03-30 22:10:41.935930 tag-shadow-aaron-alphabet-0.0.2/setup.cfg
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-30 22:10:41.931930 tag-shadow-aaron-alphabet-0.0.2/src/
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-30 22:10:41.935930 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/
--rwxrwxrwx   0 lk        (1002) lk        (1002)     2083 2023-03-30 21:47:47.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/__init__.py
--rwxrwxrwx   0 lk        (1002) lk        (1002)       82 2023-03-29 22:10:30.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/__main__.py
--rwxrwxrwx   0 lk        (1002) lk        (1002)     2314 2023-03-30 20:27:14.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/_conditions.py
--rwxrwxrwx   0 lk        (1002) lk        (1002)     1382 2023-03-30 21:48:32.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/_tasking.py
--rwxrwxrwx   0 lk        (1002) lk        (1002)     2792 2023-03-30 19:47:00.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/utils.py
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-30 22:10:41.935930 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet.egg-info/
--rw-rw-r--   0 lk        (1002) lk        (1002)     1479 2023-03-30 22:10:41.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 lk        (1002) lk        (1002)      506 2023-03-30 22:10:41.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-03-30 22:10:41.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       15 2023-03-30 22:10:41.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet.egg-info/requires.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       26 2023-03-30 22:10:41.000000 tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet.egg-info/top_level.txt
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:14:12.546499 tag-shadow-aaron-alphabet-0.0.3/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     1065 2023-08-01 12:13:34.000000 tag-shadow-aaron-alphabet-0.0.3/LICENSE
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1482 2023-08-01 12:14:12.546499 tag-shadow-aaron-alphabet-0.0.3/PKG-INFO
+-rwxrwxrwx   0 jo        (1000) jo        (1000)      534 2023-08-01 12:13:21.000000 tag-shadow-aaron-alphabet-0.0.3/pyproject.toml
+-rwxrwxrwx   0 jo        (1000) jo        (1000)       38 2023-08-01 12:14:12.546499 tag-shadow-aaron-alphabet-0.0.3/setup.cfg
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:14:12.546499 tag-shadow-aaron-alphabet-0.0.3/src/
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:14:12.546499 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     2071 2023-08-01 12:13:53.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/__init__.py
+-rwxrwxrwx   0 jo        (1000) jo        (1000)       83 2023-08-01 12:13:53.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/__main__.py
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     2314 2023-08-01 12:13:53.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/_conditions.py
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     1375 2023-08-01 12:13:53.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/_tasking.py
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     2792 2023-08-01 12:13:53.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/utils.py
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 12:14:12.546499 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet.egg-info/
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1482 2023-08-01 12:14:12.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 jo        (1000) jo        (1000)      506 2023-08-01 12:14:12.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)        1 2023-08-01 12:14:12.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       15 2023-08-01 12:14:12.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet.egg-info/requires.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       26 2023-08-01 12:14:12.000000 tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet.egg-info/top_level.txt
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/LICENSE` & `tag-shadow-aaron-alphabet-0.0.3/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 Johannes Horler
+Copyright © 2023 Aaron Alphabet
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/PKG-INFO` & `tag-shadow-aaron-alphabet-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tag-shadow-aaron-alphabet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tagging with shadow-files. 
-Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
-License: Copyright © 2022 Johannes Horler
+Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
+License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/pyproject.toml` & `tag-shadow-aaron-alphabet-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tag-shadow-aaron-alphabet"
-version = "0.0.2"
+version = "0.0.3"
 description = "Tagging with shadow-files. "
 license = { file = "LICENSE" }
-authors = [{ name = "Aaron Alphabet", email = "aaron.alphabet@gmx.ch" }]
+authors = [{ name = "Aaron Alphabet", email = "aaron.alphabet@posteo.org" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/__init__.py` & `tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse as _argparse
-from . import _tasking
-from . import _conditions
+
+from . import _conditions, _tasking
 
 parser = _argparse.ArgumentParser(
     fromfile_prefix_chars='@',
     allow_abbrev=False,
 )
 _subparsers = parser.add_subparsers(dest='task', required=True)
 _subparser = _subparsers.add_parser('tag')
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/_conditions.py` & `tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/_conditions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import os
 import string
-from . import utils
 
+from . import utils
 
 
 class Get:
     def __init__(self, key):
         self._key = utils.tag(key)
     def __call__(self, data):
         ans = data.get(self._key, False)
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/_tasking.py` & `tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/_tasking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import os as _os 
-import tomllib as _tomllib
-import tomli_w as _tomli_w
+import os as _os
 import shutil as _shutil
 import subprocess
 import sys
+import tomllib as _tomllib
 
-from . import utils
-
+import tomli_w as _tomli_w
 
-    
+from . import utils
 
 
 def _file_decorator(oldfunc):
     def newfunc(*, targets, **kwargs):
         if len(targets) == 0:
             targets = ['.']
         files = utils.walk(*targets)
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet/utils.py` & `tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import os as _os 
-import tomllib as _tomllib
-import tomli_w as _tomli_w
+import os as _os
 import shutil as _shutil
 import string as _string
+import tomllib as _tomllib
+
+import tomli_w as _tomli_w
 
 _tagchars = _string.ascii_lowercase + _string.digits + '_'
 
 def tag(value):
 	value = str(value).lower()
 	ans = ""
 	for x in value:
```

### Comparing `tag-shadow-aaron-alphabet-0.0.2/src/tag_shadow_aaron_alphabet.egg-info/PKG-INFO` & `tag-shadow-aaron-alphabet-0.0.3/src/tag_shadow_aaron_alphabet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tag-shadow-aaron-alphabet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tagging with shadow-files. 
-Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
-License: Copyright © 2022 Johannes Horler
+Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
+License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

