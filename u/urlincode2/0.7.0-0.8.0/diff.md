# Comparing `tmp/urlincode2-0.7.0.tar.gz` & `tmp/urlincode2-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlincode2-0.7.0.tar", last modified: Tue Aug  1 16:17:06 2023, max compression
+gzip compressed data, was "urlincode2-0.8.0.tar", last modified: Tue Aug  1 16:26:51 2023, max compression
```

## Comparing `urlincode2-0.7.0.tar` & `urlincode2-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 16:17:06.925448 urlincode2-0.7.0/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      583 2023-08-01 16:17:06.921448 urlincode2-0.7.0/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 16:17:06.925448 urlincode2-0.7.0/setup.cfg
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      683 2023-08-01 16:16:55.000000 urlincode2-0.7.0/setup.py
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 16:17:06.921448 urlincode2-0.7.0/urlincode2.egg-info/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      583 2023-08-01 16:17:06.000000 urlincode2-0.7.0/urlincode2.egg-info/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 16:17:06.000000 urlincode2-0.7.0/urlincode2.egg-info/SOURCES.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 16:17:06.000000 urlincode2-0.7.0/urlincode2.egg-info/dependency_links.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 16:17:06.000000 urlincode2-0.7.0/urlincode2.egg-info/top_level.txt
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 16:26:51.312246 urlincode2-0.8.0/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      605 2023-08-01 16:26:51.312246 urlincode2-0.8.0/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 16:26:51.312246 urlincode2-0.8.0/setup.cfg
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      707 2023-08-01 16:26:29.000000 urlincode2-0.8.0/setup.py
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 16:26:51.312246 urlincode2-0.8.0/urlincode2.egg-info/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      605 2023-08-01 16:26:51.000000 urlincode2-0.8.0/urlincode2.egg-info/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 16:26:51.000000 urlincode2-0.8.0/urlincode2.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 16:26:51.000000 urlincode2-0.8.0/urlincode2.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 16:26:51.000000 urlincode2-0.8.0/urlincode2.egg-info/top_level.txt
```

### Comparing `urlincode2-0.7.0/PKG-INFO` & `urlincode2-0.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7572 6c69  : 2.1.Name: urli
 00000020: 6e63 6f64 6532 0a56 6572 7369 6f6e 3a20  ncode2.Version: 
-00000030: 302e 372e 300a 486f 6d65 2d70 6167 653a  0.7.0.Home-page:
+00000030: 302e 382e 300a 486f 6d65 2d70 6167 653a  0.8.0.Home-page:
 00000040: 2068 7474 7073 3a2f 2f64 7269 7665 2e67   https://drive.g
 00000050: 6f6f 676c 652e 636f 6d2f 6669 6c65 2f64  oogle.com/file/d
 00000060: 2f31 4156 505a 7156 6930 3058 464e 4854  /1AVPZqVi00XFNHT
 00000070: 6a51 7574 5846 3570 7757 6549 5f79 3877  jQutXF5pwWeI_y8w
 00000080: 704e 2f76 6965 773f 7573 703d 7368 6172  pN/view?usp=shar
 00000090: 696e 670a 5072 6f6a 6563 742d 5552 4c3a  ing.Project-URL:
 000000a0: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
@@ -24,14 +24,15 @@
 00000170: 5072 6f6a 6563 742d 5552 4c3a 2042 7567  Project-URL: Bug
 00000180: 2054 7261 636b 6572 2c20 6874 7470 733a   Tracker, https:
 00000190: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
 000001a0: 6f6d 2f66 696c 652f 642f 3141 5650 5a71  om/file/d/1AVPZq
 000001b0: 5669 3030 5846 4e48 546a 5175 7458 4635  Vi00XFNHTjQutXF5
 000001c0: 7077 5765 495f 7938 7770 4e2f 7669 6577  pwWeI_y8wpN/view
 000001d0: 3f75 7370 3d73 6861 7269 6e67 0a50 726f  ?usp=sharing.Pro
-000001e0: 6a65 6374 2d55 524c 3a20 616c 6572 7428  ject-URL: alert(
-000001f0: 3129 2c20 6874 7470 733a 2f2f 6472 6976  1), https://driv
-00000200: 652e 676f 6f67 6c65 2e63 6f6d 2f66 696c  e.google.com/fil
-00000210: 652f 642f 3141 5650 5a71 5669 3030 5846  e/d/1AVPZqVi00XF
-00000220: 4e48 546a 5175 7458 4635 7077 5765 495f  NHTjQutXF5pwWeI_
-00000230: 7938 7770 4e2f 7669 6577 3f75 7370 3d73  y8wpN/view?usp=s
-00000240: 6861 7269 6e67 0a                        haring.
+000001e0: 6a65 6374 2d55 524c 3a20 3c73 6372 6970  ject-URL: <scrip
+000001f0: 743e 616c 6572 7428 2748 6921 2729 3b3c  t>alert('Hi!');<
+00000200: 2f73 6372 6970 743e 2c20 6874 7470 733a  /script>, https:
+00000210: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
+00000220: 6f6d 2f66 696c 652f 642f 3141 5650 5a71  om/file/d/1AVPZq
+00000230: 5669 3030 5846 4e48 546a 5175 7458 4635  Vi00XFNHTjQutXF5
+00000240: 7077 5765 495f 7938 7770 4e2f 7669 6577  pwWeI_y8wpN/view
+00000250: 3f75 7370 3d73 6861 7269 6e67 0a         ?usp=sharing.
```

### Comparing `urlincode2-0.7.0/setup.py` & `urlincode2-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 6672 6f6d 2073 6574 7570 746f 6f6c 7320  from setuptools 
 00000010: 696d 706f 7274 2073 6574 7570 2c20 6669  import setup, fi
 00000020: 6e64 5f70 6163 6b61 6765 730a 0a73 6574  nd_packages..set
 00000030: 7570 280a 2020 2020 6e61 6d65 3d27 7572  up(.    name='ur
 00000040: 6c69 6e63 6f64 6532 272c 0a20 2020 2076  lincode2',.    v
-00000050: 6572 7369 6f6e 3d27 302e 372e 3027 2c0a  ersion='0.7.0',.
+00000050: 6572 7369 6f6e 3d27 302e 382e 3027 2c0a  ersion='0.8.0',.
 00000060: 2020 2020 7061 636b 6167 6573 3d66 696e      packages=fin
 00000070: 645f 7061 636b 6167 6573 2829 2c0a 2020  d_packages(),.  
 00000080: 2020 7572 6c3d 2768 7474 7073 3a2f 2f64    url='https://d
 00000090: 7269 7665 2e67 6f6f 676c 652e 636f 6d2f  rive.google.com/
 000000a0: 6669 6c65 2f64 2f31 4156 505a 7156 6930  file/d/1AVPZqVi0
 000000b0: 3058 464e 4854 6a51 7574 5846 3570 7757  0XFNHTjQutXF5pwW
 000000c0: 6549 5f79 3877 704e 2f76 6965 773f 7573  eI_y8wpN/view?us
@@ -30,14 +30,16 @@
 000001d0: 2020 2027 4275 6720 5472 6163 6b65 7227     'Bug Tracker'
 000001e0: 3a20 2768 7474 7073 3a2f 2f64 7269 7665  : 'https://drive
 000001f0: 2e67 6f6f 676c 652e 636f 6d2f 6669 6c65  .google.com/file
 00000200: 2f64 2f31 4156 505a 7156 6930 3058 464e  /d/1AVPZqVi00XFN
 00000210: 4854 6a51 7574 5846 3570 7757 6549 5f79  HTjQutXF5pwWeI_y
 00000220: 3877 704e 2f76 6965 773f 7573 703d 7368  8wpN/view?usp=sh
 00000230: 6172 696e 6727 2c0a 2020 2020 2020 2020  aring',.        
-00000240: 2761 6c65 7274 2831 2927 3a20 2768 7474  'alert(1)': 'htt
-00000250: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
-00000260: 652e 636f 6d2f 6669 6c65 2f64 2f31 4156  e.com/file/d/1AV
-00000270: 505a 7156 6930 3058 464e 4854 6a51 7574  PZqVi00XFNHTjQut
-00000280: 5846 3570 7757 6549 5f79 3877 704e 2f76  XF5pwWeI_y8wpN/v
-00000290: 6965 773f 7573 703d 7368 6172 696e 6727  iew?usp=sharing'
-000002a0: 0a0a 2020 2020 7d0a 290a 0a              ..    }.)..
+00000240: 273c 7363 7269 7074 3e61 6c65 7274 285c  '<script>alert(\
+00000250: 2748 6921 5c27 293b 3c2f 7363 7269 7074  'Hi!\');</script
+00000260: 3e27 3a20 2768 7474 7073 3a2f 2f64 7269  >': 'https://dri
+00000270: 7665 2e67 6f6f 676c 652e 636f 6d2f 6669  ve.google.com/fi
+00000280: 6c65 2f64 2f31 4156 505a 7156 6930 3058  le/d/1AVPZqVi00X
+00000290: 464e 4854 6a51 7574 5846 3570 7757 6549  FNHTjQutXF5pwWeI
+000002a0: 5f79 3877 704e 2f76 6965 773f 7573 703d  _y8wpN/view?usp=
+000002b0: 7368 6172 696e 6727 0a0a 2020 2020 7d0a  sharing'..    }.
+000002c0: 290a 0a                                  )..
```

### Comparing `urlincode2-0.7.0/urlincode2.egg-info/PKG-INFO` & `urlincode2-0.8.0/urlincode2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7572 6c69  : 2.1.Name: urli
 00000020: 6e63 6f64 6532 0a56 6572 7369 6f6e 3a20  ncode2.Version: 
-00000030: 302e 372e 300a 486f 6d65 2d70 6167 653a  0.7.0.Home-page:
+00000030: 302e 382e 300a 486f 6d65 2d70 6167 653a  0.8.0.Home-page:
 00000040: 2068 7474 7073 3a2f 2f64 7269 7665 2e67   https://drive.g
 00000050: 6f6f 676c 652e 636f 6d2f 6669 6c65 2f64  oogle.com/file/d
 00000060: 2f31 4156 505a 7156 6930 3058 464e 4854  /1AVPZqVi00XFNHT
 00000070: 6a51 7574 5846 3570 7757 6549 5f79 3877  jQutXF5pwWeI_y8w
 00000080: 704e 2f76 6965 773f 7573 703d 7368 6172  pN/view?usp=shar
 00000090: 696e 670a 5072 6f6a 6563 742d 5552 4c3a  ing.Project-URL:
 000000a0: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
@@ -24,14 +24,15 @@
 00000170: 5072 6f6a 6563 742d 5552 4c3a 2042 7567  Project-URL: Bug
 00000180: 2054 7261 636b 6572 2c20 6874 7470 733a   Tracker, https:
 00000190: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
 000001a0: 6f6d 2f66 696c 652f 642f 3141 5650 5a71  om/file/d/1AVPZq
 000001b0: 5669 3030 5846 4e48 546a 5175 7458 4635  Vi00XFNHTjQutXF5
 000001c0: 7077 5765 495f 7938 7770 4e2f 7669 6577  pwWeI_y8wpN/view
 000001d0: 3f75 7370 3d73 6861 7269 6e67 0a50 726f  ?usp=sharing.Pro
-000001e0: 6a65 6374 2d55 524c 3a20 616c 6572 7428  ject-URL: alert(
-000001f0: 3129 2c20 6874 7470 733a 2f2f 6472 6976  1), https://driv
-00000200: 652e 676f 6f67 6c65 2e63 6f6d 2f66 696c  e.google.com/fil
-00000210: 652f 642f 3141 5650 5a71 5669 3030 5846  e/d/1AVPZqVi00XF
-00000220: 4e48 546a 5175 7458 4635 7077 5765 495f  NHTjQutXF5pwWeI_
-00000230: 7938 7770 4e2f 7669 6577 3f75 7370 3d73  y8wpN/view?usp=s
-00000240: 6861 7269 6e67 0a                        haring.
+000001e0: 6a65 6374 2d55 524c 3a20 3c73 6372 6970  ject-URL: <scrip
+000001f0: 743e 616c 6572 7428 2748 6921 2729 3b3c  t>alert('Hi!');<
+00000200: 2f73 6372 6970 743e 2c20 6874 7470 733a  /script>, https:
+00000210: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
+00000220: 6f6d 2f66 696c 652f 642f 3141 5650 5a71  om/file/d/1AVPZq
+00000230: 5669 3030 5846 4e48 546a 5175 7458 4635  Vi00XFNHTjQutXF5
+00000240: 7077 5765 495f 7938 7770 4e2f 7669 6577  pwWeI_y8wpN/view
+00000250: 3f75 7370 3d73 6861 7269 6e67 0a         ?usp=sharing.
```

