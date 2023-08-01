# Comparing `tmp/argparse-aaron-alphabet-0.0.2.tar.gz` & `tmp/argparse-aaron-alphabet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-aaron-alphabet-0.0.2.tar", last modified: Sun May  7 09:37:40 2023, max compression
+gzip compressed data, was "argparse-aaron-alphabet-0.0.3.tar", last modified: Tue Aug  1 11:59:23 2023, max compression
```

## Comparing `argparse-aaron-alphabet-0.0.2.tar` & `argparse-aaron-alphabet-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/
--rwxrwxrwx   0 lk        (1002) lk        (1002)     1066 2023-03-01 20:28:52.000000 argparse-aaron-alphabet-0.0.2/LICENSE
--rw-rw-r--   0 lk        (1002) lk        (1002)     1472 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/PKG-INFO
--rwxrwxrwx   0 lk        (1002) lk        (1002)      501 2023-05-07 09:37:29.000000 argparse-aaron-alphabet-0.0.2/pyproject.toml
--rwxrwxrwx   0 lk        (1002) lk        (1002)       38 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/setup.cfg
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/src/
-drwxrwxr-x   0 lk        (1002) lk        (1002)        0 2023-05-07 09:37:40.365091 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/
--rw-rw-r--   0 lk        (1002) lk        (1002)     1472 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 lk        (1002) lk        (1002)      267 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)        1 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)       24 2023-05-07 09:37:40.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/top_level.txt
--rw-rw-r--   0 lk        (1002) lk        (1002)      184 2023-05-07 09:37:18.000000 argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.py
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:59:23.887538 argparse-aaron-alphabet-0.0.3/
+-rwxrwxrwx   0 jo        (1000) jo        (1000)     1065 2023-08-01 11:58:53.000000 argparse-aaron-alphabet-0.0.3/LICENSE
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1475 2023-08-01 11:59:23.887538 argparse-aaron-alphabet-0.0.3/PKG-INFO
+-rwxrwxrwx   0 jo        (1000) jo        (1000)      505 2023-08-01 11:58:38.000000 argparse-aaron-alphabet-0.0.3/pyproject.toml
+-rwxrwxrwx   0 jo        (1000) jo        (1000)       38 2023-08-01 11:59:23.887538 argparse-aaron-alphabet-0.0.3/setup.cfg
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:59:23.887538 argparse-aaron-alphabet-0.0.3/src/
+drwxrwxr-x   0 jo        (1000) jo        (1000)        0 2023-08-01 11:59:23.887538 argparse-aaron-alphabet-0.0.3/src/argparse_aaron_alphabet.egg-info/
+-rw-rw-r--   0 jo        (1000) jo        (1000)     1475 2023-08-01 11:59:23.000000 argparse-aaron-alphabet-0.0.3/src/argparse_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 jo        (1000) jo        (1000)      267 2023-08-01 11:59:23.000000 argparse-aaron-alphabet-0.0.3/src/argparse_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)        1 2023-08-01 11:59:23.000000 argparse-aaron-alphabet-0.0.3/src/argparse_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)       24 2023-08-01 11:59:23.000000 argparse-aaron-alphabet-0.0.3/src/argparse_aaron_alphabet.egg-info/top_level.txt
+-rw-rw-r--   0 jo        (1000) jo        (1000)      185 2023-08-01 11:59:19.000000 argparse-aaron-alphabet-0.0.3/src/argparse_aaron_alphabet.py
```

### Comparing `argparse-aaron-alphabet-0.0.2/LICENSE` & `argparse-aaron-alphabet-0.0.3/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright © 2022 Johannes Horler
+Copyright © 2023 Aaron Alphabet
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `argparse-aaron-alphabet-0.0.2/PKG-INFO` & `argparse-aaron-alphabet-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: argparse-aaron-alphabet
-Version: 0.0.2
+Version: 0.0.3
 Summary: os-library-extension. 
-Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
-License: Copyright © 2022 Johannes Horler
+Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
+License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `argparse-aaron-alphabet-0.0.2/src/argparse_aaron_alphabet.egg-info/PKG-INFO` & `argparse-aaron-alphabet-0.0.3/src/argparse_aaron_alphabet.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: argparse-aaron-alphabet
-Version: 0.0.2
+Version: 0.0.3
 Summary: os-library-extension. 
-Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
-License: Copyright © 2022 Johannes Horler
+Author-email: Aaron Alphabet <aaron.alphabet@posteo.org>
+License: Copyright © 2023 Aaron Alphabet
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

