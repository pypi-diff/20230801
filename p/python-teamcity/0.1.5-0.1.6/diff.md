# Comparing `tmp/python-teamcity-0.1.5.tar.gz` & `tmp/python-teamcity-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-teamcity-0.1.5.tar", last modified: Thu May 25 11:37:58 2023, max compression
+gzip compressed data, was "python-teamcity-0.1.6.tar", last modified: Tue Aug  1 07:49:08 2023, max compression
```

## Comparing `python-teamcity-0.1.5.tar` & `python-teamcity-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:37:58.871059 python-teamcity-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-05-25 11:37:58.820411 python-teamcity-0.1.5/.github/
-drwxrwxrwx   0        0        0        0 2023-05-25 11:37:58.840675 python-teamcity-0.1.5/.github/workflows/
--rw-rw-rw-   0        0        0     2852 2022-11-24 14:11:30.000000 python-teamcity-0.1.5/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0       68 2023-05-25 11:37:58.000000 python-teamcity-0.1.5/AUTHORS
--rw-rw-rw-   0        0        0      685 2023-05-25 11:37:57.000000 python-teamcity-0.1.5/ChangeLog
--rw-rw-rw-   0        0        0     1093 2023-05-25 11:37:21.000000 python-teamcity-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1020 2023-05-25 11:37:58.871059 python-teamcity-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       67 2022-11-22 12:21:06.000000 python-teamcity-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 11:37:58.844187 python-teamcity-0.1.5/examples/
--rw-rw-rw-   0        0        0        0 2022-11-22 12:26:55.000000 python-teamcity-0.1.5/examples/__init__.py
--rw-rw-rw-   0        0        0      561 2023-05-25 11:37:22.000000 python-teamcity-0.1.5/examples/sample.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:37:58.860019 python-teamcity-0.1.5/python_teamcity.egg-info/
--rw-rw-rw-   0        0        0     1020 2023-05-25 11:37:58.000000 python-teamcity-0.1.5/python_teamcity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-05-25 11:37:58.000000 python-teamcity-0.1.5/python_teamcity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 11:37:58.000000 python-teamcity-0.1.5/python_teamcity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-01 12:33:48.000000 python-teamcity-0.1.5/python_teamcity.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-05-25 11:37:58.000000 python-teamcity-0.1.5/python_teamcity.egg-info/pbr.json
--rw-rw-rw-   0        0        0        9 2023-05-25 11:37:58.000000 python-teamcity-0.1.5/python_teamcity.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 11:37:58.000000 python-teamcity-0.1.5/python_teamcity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        8 2022-11-22 12:28:41.000000 python-teamcity-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0      880 2023-05-25 11:37:58.872059 python-teamcity-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      133 2022-11-24 14:11:30.000000 python-teamcity-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:37:58.867019 python-teamcity-0.1.5/teamcity/
--rw-rw-rw-   0        0        0       31 2022-12-28 09:42:30.000000 python-teamcity-0.1.5/teamcity/__init__.py
--rw-rw-rw-   0        0        0    13561 2023-05-25 11:37:21.000000 python-teamcity-0.1.5/teamcity/teamcity.py
--rw-rw-rw-   0        0        0      237 2022-11-24 14:11:30.000000 python-teamcity-0.1.5/teamcity/teamcity_const.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:37:58.869054 python-teamcity-0.1.5/tests/
--rw-rw-rw-   0        0        0        0 2022-11-22 12:27:14.000000 python-teamcity-0.1.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:49:08.844932 python-teamcity-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-08-01 07:49:08.775424 python-teamcity-0.1.6/.github/
+drwxrwxrwx   0        0        0        0 2023-08-01 07:49:08.801915 python-teamcity-0.1.6/.github/workflows/
+-rw-rw-rw-   0        0        0     2852 2022-11-24 14:11:30.000000 python-teamcity-0.1.6/.github/workflows/codeql.yml
+-rw-rw-rw-   0        0        0       68 2023-08-01 07:49:07.000000 python-teamcity-0.1.6/AUTHORS
+-rw-rw-rw-   0        0        0      751 2023-08-01 07:49:07.000000 python-teamcity-0.1.6/ChangeLog
+-rw-rw-rw-   0        0        0     1093 2023-05-25 11:37:21.000000 python-teamcity-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      992 2023-08-01 07:49:08.845932 python-teamcity-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2022-11-22 12:21:06.000000 python-teamcity-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 07:49:08.807915 python-teamcity-0.1.6/examples/
+-rw-rw-rw-   0        0        0        0 2022-11-22 12:26:55.000000 python-teamcity-0.1.6/examples/__init__.py
+-rw-rw-rw-   0        0        0      658 2023-07-20 10:09:23.000000 python-teamcity-0.1.6/examples/sample.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:49:08.830157 python-teamcity-0.1.6/python_teamcity.egg-info/
+-rw-rw-rw-   0        0        0      992 2023-08-01 07:49:08.000000 python-teamcity-0.1.6/python_teamcity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-08-01 07:49:08.000000 python-teamcity-0.1.6/python_teamcity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 07:49:08.000000 python-teamcity-0.1.6/python_teamcity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-01 12:33:48.000000 python-teamcity-0.1.6/python_teamcity.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-08-01 07:49:08.000000 python-teamcity-0.1.6/python_teamcity.egg-info/pbr.json
+-rw-rw-rw-   0        0        0        9 2023-08-01 07:49:08.000000 python-teamcity-0.1.6/python_teamcity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 07:49:08.000000 python-teamcity-0.1.6/python_teamcity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        8 2022-11-22 12:28:41.000000 python-teamcity-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0      852 2023-08-01 07:49:08.846933 python-teamcity-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      133 2022-11-24 14:11:30.000000 python-teamcity-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:49:08.839423 python-teamcity-0.1.6/teamcity/
+-rw-rw-rw-   0        0        0       31 2022-12-28 09:42:30.000000 python-teamcity-0.1.6/teamcity/__init__.py
+-rw-rw-rw-   0        0        0    13697 2023-08-01 07:46:27.000000 python-teamcity-0.1.6/teamcity/teamcity.py
+-rw-rw-rw-   0        0        0      237 2022-11-24 14:11:30.000000 python-teamcity-0.1.6/teamcity/teamcity_const.py
+drwxrwxrwx   0        0        0        0 2023-08-01 07:49:08.841935 python-teamcity-0.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-22 12:27:14.000000 python-teamcity-0.1.6/tests/__init__.py
```

### Comparing `python-teamcity-0.1.5/.github/workflows/codeql.yml` & `python-teamcity-0.1.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.1.5/ChangeLog` & `python-teamcity-0.1.6/ChangeLog`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v0.1.6
+------
+
+* Optimize get\_build\_dependencies function
+
 v0.1.5
 ------
 
 * Fix get\_builds\_by\_since\_build issue
 
 v0.1.4
 ------
```

### Comparing `python-teamcity-0.1.5/LICENSE` & `python-teamcity-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.1.5/PKG-INFO` & `python-teamcity-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
-License: GPLv3
+License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `python-teamcity-0.1.5/examples/sample.py` & `python-teamcity-0.1.6/examples/sample.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,10 +9,12 @@
 logging.basicConfig(level=logging.DEBUG)
 
 if __name__ == '__main__':
     tc = TeamCity(server=TEAMCITY_SERVER, tokens=TEAMCITY_TOKENS)
     # s = tc.get_build_details(1)
     # print(tc.get_build_details(23929740))
     # print(tc.get_all_builds(build_type_id='Hk4eAsset_Streaming_38devAssignerTools'))
-    test = tc.get_builds_by_since_build(23948144,count = 50)
+    # single = tc.get_builds_by_since_build(25954043,count = 50)
+    test = tc.get_build_dependencies(25954059)
+    single = tc.get_build_details(25954043)
 
     pass
```

### Comparing `python-teamcity-0.1.5/python_teamcity.egg-info/PKG-INFO` & `python-teamcity-0.1.6/python_teamcity.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
-License: GPLv3
+License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `python-teamcity-0.1.5/setup.cfg` & `python-teamcity-0.1.6/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 686f 6e2d 7465 616d 6369   = python-teamci
 00000020: 7479 0d0a 7665 7273 696f 6e20 3d20 302e  ty..version = 0.
-00000030: 312e 350d 0a61 7574 686f 7220 3d20 5975  1.5..author = Yu
+00000030: 312e 360d 0a61 7574 686f 7220 3d20 5975  1.6..author = Yu
 00000040: 6e6c 696e 2054 616e 0d0a 6175 7468 6f72  nlin Tan..author
 00000050: 5f65 6d61 696c 203d 2074 616e 7975 6e6c  _email = tanyunl
 00000060: 696e 3230 3033 406e 6f72 6272 6561 642e  in2003@norbread.
 00000070: 636f 6d0d 0a73 756d 6d61 7279 203d 2050  com..summary = P
 00000080: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
 00000090: 7220 7472 6967 6765 7269 6e67 2054 6561  r triggering Tea
 000000a0: 6d43 6974 7920 6279 2052 4553 5420 4150  mCity by REST AP
 000000b0: 490d 0a64 6573 6372 6970 7469 6f6e 2d66  I..description-f
 000000c0: 696c 6520 3d20 5245 4144 4d45 2e6d 640d  ile = README.md.
-000000d0: 0a6c 6963 656e 7365 203d 2047 504c 7633  .license = GPLv3
-000000e0: 0d0a 686f 6d65 2d70 6167 6520 3d20 6874  ..home-page = ht
-000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000100: 2f6e 6f72 6272 6561 6432 3030 332f 7079  /norbread2003/py
-00000110: 7468 6f6e 2d74 6561 6d63 6974 790d 0a63  thon-teamcity..c
-00000120: 6c61 7373 6966 6965 7220 3d20 0d0a 0954  lassifier = ...T
-00000130: 6f70 6963 203a 3a20 5574 696c 6974 6965  opic :: Utilitie
-00000140: 730d 0a09 496e 7465 6e64 6564 2041 7564  s...Intended Aud
-00000150: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000160: 6572 730d 0a09 456e 7669 726f 6e6d 656e  ers...Environmen
-00000170: 7420 3a3a 2043 6f6e 736f 6c65 0d0a 094c  t :: Console...L
-00000180: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000190: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
-000001a0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-000001b0: 656e 7365 2076 3320 2847 504c 7633 290d  ense v3 (GPLv3).
-000001c0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-000001d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000001e0: 6465 6e74 0d0a 0950 726f 6772 616d 6d69  dent...Programmi
-000001f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000200: 7974 686f 6e0d 0a09 5072 6f67 7261 6d6d  ython...Programm
-00000210: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000220: 5079 7468 6f6e 203a 3a20 332e 350d 0a09  Python :: 3.5...
-00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000250: 3a20 332e 360d 0a09 5072 6f67 7261 6d6d  : 3.6...Programm
-00000260: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000270: 5079 7468 6f6e 203a 3a20 332e 370d 0a09  Python :: 3.7...
-00000280: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000290: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002a0: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
-000002b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002c0: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-000002d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002f0: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
-00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000310: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
-00000320: 0a0d 0a5b 6669 6c65 735d 0d0a 7061 636b  ...[files]..pack
-00000330: 6167 6573 203d 200d 0a09 7465 616d 6369  ages = ...teamci
-00000340: 7479 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ty....[egg_info]
-00000350: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000360: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000000d0: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
+000000e0: 686f 6d65 2d70 6167 6520 3d20 6874 7470  home-page = http
+000000f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
+00000100: 6f72 6272 6561 6432 3030 332f 7079 7468  orbread2003/pyth
+00000110: 6f6e 2d74 6561 6d63 6974 790d 0a63 6c61  on-teamcity..cla
+00000120: 7373 6966 6965 7220 3d20 0d0a 0954 6f70  ssifier = ...Top
+00000130: 6963 203a 3a20 5574 696c 6974 6965 730d  ic :: Utilities.
+00000140: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+00000150: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000160: 730d 0a09 456e 7669 726f 6e6d 656e 7420  s...Environment 
+00000170: 3a3a 2043 6f6e 736f 6c65 0d0a 094c 6963  :: Console...Lic
+00000180: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000190: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000001a0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
+000001b0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001c0: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
+000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001e0: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
+000001f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000200: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000210: 350d 0a09 5072 6f67 7261 6d6d 696e 6720  5...Programming 
+00000220: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000230: 6f6e 203a 3a20 332e 360d 0a09 5072 6f67  on :: 3.6...Prog
+00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000260: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
+00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000280: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
+00000290: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002a0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002b0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
+000002c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002d0: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+000002e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000300: 2e31 310d 0a0d 0a5b 6669 6c65 735d 0d0a  .11....[files]..
+00000310: 7061 636b 6167 6573 203d 200d 0a09 7465  packages = ...te
+00000320: 616d 6369 7479 0d0a 0d0a 5b65 6767 5f69  amcity....[egg_i
+00000330: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000340: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000350: 0d0a 0d0a                                ....
```

### Comparing `python-teamcity-0.1.5/teamcity/teamcity.py` & `python-teamcity-0.1.6/teamcity/teamcity.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     None
 
 Update Record
 -------------
 0.1.0.1122   11/22/2022   Yunlin Tan([None])            Python API for triggering TeamCity by REST API.
 0.1.1        11/25/2022   Yunlin Tan([None])            Add more functions by requests.
 0.1.5        5/25/2023    Yunlin Tan([None])            Multiple features added.
+0.1.6        5/26/2023    Yunlin Tan([None])            Optimize get_build_dependencies function.
 
 Depends On
 ----------
 **Python Dependencies:**
     - requests
 
 **Other Dependencies:**
@@ -240,15 +241,16 @@
               f'relativeUrl))),snapshot-dependencies(count,build(id)),running-info(percentageComplete,' \
               f'elapsedSeconds,estimatedTotalSeconds,leftSeconds,probablyHanging,lastActivityTime,outdated,' \
               f'outdatedReasonBuild(number,links(link(type,relativeUrl)))),waitReason,queuePosition,' \
               f'startEstimate,finishEstimate,plannedAgent(name,id,environment(osType),typeId,pool(id,name)),' \
               f'delayedByBuild(id,number,status,state,failedToStart,personal,canceledInfo,buildType(id)),' \
               f'triggered(date,displayText,buildType(id,paused,internalId,projectId,name,type,links(' \
               f'link(type,relativeUrl)))))'
-        return self.get_request(url)['build']
+        data = self.get_request(url)['build']
+        return data if data else []
 
     def get_user(self, username='') -> dict:
         """Get user by username from TeamCity.
 
         :param username: username, if empty - get current user
         :return: user dict, for example:
```

