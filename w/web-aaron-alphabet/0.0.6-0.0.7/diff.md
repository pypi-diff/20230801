# Comparing `tmp/web-aaron-alphabet-0.0.6.tar.gz` & `tmp/web-aaron-alphabet-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-aaron-alphabet-0.0.6.tar", last modified: Sun Mar 26 23:11:02 2023, max compression
+gzip compressed data, was "web-aaron-alphabet-0.0.7.tar", last modified: Tue Aug  1 11:49:04 2023, max compression
```

## Comparing `web-aaron-alphabet-0.0.6.tar` & `web-aaron-alphabet-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/
--rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 web-aaron-alphabet-0.0.6/LICENSE
--rw-rw-r--   0 lk        (1002) lk        (1002)     1463 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/PKG-INFO
--rwxrwxrwx   0 lk        (1002) lk        (1002)      602 2023-03-26 10:30:10.000000 web-aaron-alphabet-0.0.6/pyproject.toml
--rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/setup.cfg
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/src/
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/
--rwxrwxrwx   0 lk        (1002) lk        (1002)        0 2023-03-25 18:29:15.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/__init__.py
--rw-rw-r--   0 lk        (1002) lk        (1002)     2723 2023-03-26 12:33:36.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/__main__.py
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/converting/
--rwxrwxrwx   0 lk        (1002) lk        (1002)       94 2023-03-25 22:36:43.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/converting/__init__.py
--rw-rw-r--   0 lk        (1002) lk        (1002)      286 2023-03-25 21:45:07.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/converting/htmldocx.py
--rw-rw-r--   0 lk        (1002) lk        (1002)       63 2023-03-25 21:23:25.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/converting/pdfkit.py
--rw-rw-r--   0 lk        (1002) lk        (1002)       77 2023-03-25 22:30:15.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/converting/weasyprint.py
--rw-rw-r--   0 lk        (1002) lk        (1002)      141 2023-03-25 21:36:34.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/converting/wkhtmltopdf.py
--rw-rw-r--   0 lk        (1002) lk        (1002)     1240 2023-03-26 10:30:00.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/harvesting.py
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/merging/
--rw-rw-r--   0 lk        (1002) lk        (1002)      347 2023-03-25 20:37:59.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/merging/PyPDF2.py
--rw-rw-r--   0 lk        (1002) lk        (1002)       58 2023-03-25 21:19:57.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/merging/__init__.py
--rw-rw-r--   0 lk        (1002) lk        (1002)      164 2023-03-25 21:19:06.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/merging/pypdf.py
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-03-26 23:11:02.106520 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/
--rw-rw-r--   0 lk        (1002) lk        (1002)     1463 2023-03-26 23:11:02.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 lk        (1002) lk        (1002)      725 2023-03-26 23:11:02.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-03-26 23:11:02.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       61 2023-03-26 23:11:02.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/requires.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       19 2023-03-26 23:11:02.000000 web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/top_level.txt
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:49:04.361804 web-aaron-alphabet-0.0.7/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     1065 2023-08-01 11:48:10.000000 web-aaron-alphabet-0.0.7/LICENSE
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1466 2023-08-01 11:49:04.361804 web-aaron-alphabet-0.0.7/PKG-INFO
+-rwxrwxrwx   0 jo        (1000) jo        (1000)      606 2023-08-01 11:48:47.000000 web-aaron-alphabet-0.0.7/pyproject.toml
+-rwxrwxrwx   0 jo        (1000) jo        (1000)       38 2023-08-01 11:49:04.361804 web-aaron-alphabet-0.0.7/setup.cfg
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:49:04.357804 web-aaron-alphabet-0.0.7/src/
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:49:04.357804 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)        0 2023-03-25 18:29:15.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/__init__.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)     2694 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/__main__.py
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:49:04.361804 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/converting/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)       56 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/converting/__init__.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)      287 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/converting/htmldocx.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)       64 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/converting/pdfkit.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)       78 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/converting/weasyprint.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)      141 2023-03-25 21:36:34.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/converting/wkhtmltopdf.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1241 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/harvesting.py
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:49:04.361804 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/merging/
+-rw-rw-r--   0 jo        (1000) jo        (1000)      348 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/merging/PyPDF2.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)       46 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/merging/__init__.py
+-rw-rw-r--   0 jo        (1000) jo        (1000)      165 2023-08-01 11:48:58.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/merging/pypdf.py
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:49:04.361804 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1466 2023-08-01 11:49:04.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 jo        (1000) jo        (1000)      725 2023-08-01 11:49:04.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)        1 2023-08-01 11:49:04.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       61 2023-08-01 11:49:04.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/requires.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       19 2023-08-01 11:49:04.000000 web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/top_level.txt
```

### Comparing `web-aaron-alphabet-0.0.6/LICENSE` & `web-aaron-alphabet-0.0.7/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 Johannes Horler
+Copyright © 2023 Aaron Alphabet
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `web-aaron-alphabet-0.0.6/PKG-INFO` & `web-aaron-alphabet-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: web-aaron-alphabet
-Version: 0.0.6
+Version: 0.0.7
 Summary: Websites to PDFs. 
-Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
-License: Copyright © 2022 Johannes Horler
+Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
+License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `web-aaron-alphabet-0.0.6/pyproject.toml` & `web-aaron-alphabet-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "web-aaron-alphabet"
-version = "0.0.6"
+version = "0.0.7"
 description = "Websites to PDFs. "
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

### Comparing `web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/__main__.py` & `web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-from argparse import ArgumentParser
+import inspect
 import os
-import tempfile
 import string
-import inspect
 import sys
+import tempfile
+from argparse import ArgumentParser
 from contextlib import contextmanager, redirect_stderr, redirect_stdout
 
-from . import harvesting
-from . import converting
-from . import merging
-
-
-
+from . import converting, harvesting, merging
 
 engines = dict()
 for n, m in inspect.getmembers(converting):
     if not n.startswith('_'):
         engines[n] = m
 
 parser = ArgumentParser(fromfile_prefix_chars='@')
```

### Comparing `web-aaron-alphabet-0.0.6/src/web_aaron_alphabet/harvesting.py` & `web-aaron-alphabet-0.0.7/src/web_aaron_alphabet/harvesting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 
+
 class _Harvester:
     @classmethod
     def from_namespace(cls, ns):
         sig = inspect.signature(cls.__init__)
         parameters = list(dict(sig.parameters).items())
         n, m = parameters.pop(0)
         assert n == 'self'
```

### Comparing `web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/PKG-INFO` & `web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: web-aaron-alphabet
-Version: 0.0.6
+Version: 0.0.7
 Summary: Websites to PDFs. 
-Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
-License: Copyright © 2022 Johannes Horler
+Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
+License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `web-aaron-alphabet-0.0.6/src/web_aaron_alphabet.egg-info/SOURCES.txt` & `web-aaron-alphabet-0.0.7/src/web_aaron_alphabet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

