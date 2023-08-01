# Comparing `tmp/lichenggong-0.5.1.0.tar.gz` & `tmp/lichenggong-0.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.5.1.0.tar", last modified: Mon Jul 31 02:05:36 2023, max compression
+gzip compressed data, was "lichenggong-0.5.1.1.tar", last modified: Tue Aug  1 12:16:27 2023, max compression
```

## Comparing `lichenggong-0.5.1.0.tar` & `lichenggong-0.5.1.1.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/
--rw-rw-rw-   0        0        0      785 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-07-19 23:28:27.000000 lichenggong-0.5.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.580387 lichenggong-0.5.1.0/lichenggong/
-drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.752262 lichenggong-0.5.1.0/lichenggong/Noodows/
--rw-rw-rw-   0        0        0     3162 2023-07-31 02:02:16.000000 lichenggong-0.5.1.0/lichenggong/Noodows/__bios__.py
--rw-rw-rw-   0        0        0        0 2023-07-18 10:50:27.000000 lichenggong-0.5.1.0/lichenggong/Noodows/__init__.py
--rw-rw-rw-   0        0        0    18219 2023-07-31 01:44:14.000000 lichenggong-0.5.1.0/lichenggong/Noodows/__noodows__.py
--rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.5.1.0/lichenggong/Noodows/first.txt
--rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.5.1.0/lichenggong/Noodows/practice.py
--rw-rw-rw-   0        0        0        0 2023-07-16 12:12:38.000000 lichenggong-0.5.1.0/lichenggong/Noodows/python.txt
--rw-rw-rw-   0        0        0     2370 2023-07-19 23:27:57.000000 lichenggong-0.5.1.0/lichenggong/Noodows/update.log
-drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.752262 lichenggong-0.5.1.0/lichenggong/Noodows/version/
--rw-rw-rw-   0        0        0        9 2023-07-19 12:24:31.000000 lichenggong-0.5.1.0/lichenggong/Noodows/version/build_version.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 02:03:53.000000 lichenggong-0.5.1.0/lichenggong/Noodows/version/version.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.564762 lichenggong-0.5.1.0/lichenggong/Program_Files/
-drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/lichenggong/Program_Files/System/
--rw-rw-rw-   0        0        0     5795 2023-07-19 23:22:45.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__calc__.py
--rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__logo__.py
--rw-rw-rw-   0        0        0        0 2023-07-18 06:49:18.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__n_explorer__.py
--rw-rw-rw-   0        0        0      233 2023-07-18 06:21:05.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__thanks__.py
--rw-rw-rw-   0        0        0    24951 2023-07-31 01:44:14.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__user__.py
--rw-rw-rw-   0        0        0      874 2023-07-18 08:47:14.000000 lichenggong-0.5.1.0/lichenggong/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.611641 lichenggong-0.5.1.0/lichenggong.egg-info/
--rw-rw-rw-   0        0        0      785 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      724 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-07-31 02:05:32.000000 lichenggong-0.5.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:16:27.813157 lichenggong-0.5.1.1/
+-rw-rw-rw-   0        0        0      785 2023-08-01 12:16:27.812157 lichenggong-0.5.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-07-19 23:28:27.000000 lichenggong-0.5.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 12:16:27.736153 lichenggong-0.5.1.1/lichenggong/
+drwxrwxrwx   0        0        0        0 2023-08-01 12:16:27.774152 lichenggong-0.5.1.1/lichenggong/Noodows/
+-rw-rw-rw-   0        0        0     2907 2023-08-01 12:04:39.000000 lichenggong-0.5.1.1/lichenggong/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 10:50:27.000000 lichenggong-0.5.1.1/lichenggong/Noodows/__init__.py
+-rw-rw-rw-   0        0        0    18219 2023-07-31 01:44:14.000000 lichenggong-0.5.1.1/lichenggong/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.5.1.1/lichenggong/Noodows/first.txt
+-rw-rw-rw-   0        0        0      798 2023-08-01 12:15:30.000000 lichenggong-0.5.1.1/lichenggong/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-08-01 12:16:27.779152 lichenggong-0.5.1.1/lichenggong/Noodows/version/
+-rw-rw-rw-   0        0        0        9 2023-07-19 12:24:31.000000 lichenggong-0.5.1.1/lichenggong/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 12:05:10.000000 lichenggong-0.5.1.1/lichenggong/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 12:16:27.731153 lichenggong-0.5.1.1/lichenggong/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-08-01 12:16:27.803153 lichenggong-0.5.1.1/lichenggong/Program_Files/System/
+-rw-rw-rw-   0        0        0     5795 2023-07-19 23:22:45.000000 lichenggong-0.5.1.1/lichenggong/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.5.1.1/lichenggong/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 06:49:18.000000 lichenggong-0.5.1.1/lichenggong/Program_Files/System/__n_explorer__.py
+-rw-rw-rw-   0        0        0      233 2023-07-18 06:21:05.000000 lichenggong-0.5.1.1/lichenggong/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    24951 2023-07-31 01:44:14.000000 lichenggong-0.5.1.1/lichenggong/Program_Files/System/__user__.py
+-rw-rw-rw-   0        0        0      874 2023-07-18 08:47:14.000000 lichenggong-0.5.1.1/lichenggong/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 12:16:27.745154 lichenggong-0.5.1.1/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      785 2023-08-01 12:16:27.000000 lichenggong-0.5.1.1/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-08-01 12:16:27.000000 lichenggong-0.5.1.1/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 12:16:27.000000 lichenggong-0.5.1.1/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-01 12:16:27.000000 lichenggong-0.5.1.1/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 12:16:27.814154 lichenggong-0.5.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-31 02:05:32.000000 lichenggong-0.5.1.1/setup.py
```

### Comparing `lichenggong-0.5.1.0/PKG-INFO` & `lichenggong-0.5.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.5.1.0
+Version: 0.5.1.1
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.5.1.0/lichenggong/Noodows/__bios__.py` & `lichenggong-0.5.1.1/lichenggong/Noodows/__bios__.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,33 +52,27 @@
     del file_list, total_code_num, code_num, total_blank_num, blank_num, total_annotate_num, annotate_num
     gc.collect()
     return files
 
 
 def bios():
     __logo__.logo3_0()
-    file_name = r'../'
-    scale = 20
+    scale = 10
     start = t.perf_counter()
     for i in range(scale + 1):
-        a = "|" * i
-        b = "-" * (scale - i)
+        a = "-" * i
+        b = " " * (scale - i)
         c = (i / scale) * 100
         dur = t.perf_counter() - start
         print("Loading {:^3.0f}%[{}{}]{:.2f}s Noodows is coming".format(c, a, b, dur))
     print()
     a = file_dir('../')
     print('代码行: {}'.format(a[0][0]))  # 返回代码行数
     print('空行数: {}'.format(a[0][1]))  # 返回空行数
     print('注释行: {}'.format(a[0][2]))  # 返回注释行数
-    for root, dirs, file in os.walk(file_name):
-        print('File folder：{0}'.format(root))
-        print('Sub folders：{0}'.format(dirs))
-        print('Files:{0}'.format(file))
-        print('|' * 25)
     print('files:', a[1])
     print('large(MB)', a[2] / (1024 ** 2))
     print('hallo,world =) ')
     print()
-    del a, root, dirs, file
+    del a
     del i, scale, start, dur, b, c
     gc.collect()
```

### Comparing `lichenggong-0.5.1.0/lichenggong/Noodows/__noodows__.py` & `lichenggong-0.5.1.1/lichenggong/Noodows/__noodows__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.1.0/lichenggong/Noodows/update.log` & `lichenggong-0.5.1.1/lichenggong/Noodows/update.log`

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,68 @@
->>before version 0.2.2.1 and at version 0.2.2.1
-'''
-
-all things goes on
-
-it's so far that i even forgot what it been updated
-
-'''
->>at version 0.2.2.3
+>>at version 0.2.2.3 - 0.2.2.9
 '''
 
 language update
 
-Chinese(繁體中文) and English(US and UK)
-
-'''
->>at version 0.2.2.5
-'''
+繁體中文 and English
 
 streamline content update
 
 delete some game in the __lidao__.py
 
 delete some Irrelevant content in the __lidao__.py
 
-if you want to play\delete them go to .\无用程序\废弃程序\ikun21(小游戏).py and .\无用程序\恶搞程序\梗.py
+create file update.log
 
 '''
->>at version 0.2.2.6
-'''
-
-streamline content update
-
-delete some Irrelevant content
-
-'''
->>at version 0.2.2.9
-'''
-
-streamline content update
-files changes
-
-change file--update log.txt to update.log.txt to update.log
-
-Availability upgrade!
-
-fix version 0.2.2.5 version 0.2.2.6,version 0.2.2.7 and version 0.2.2.8 "THE VERSION ERROR"
-
-we saw that version have ERROR
-
-it made the module cannot use
-
-fix it!
-'''
->>at version 0.2.2.10
-'''
-
-practicability update
-
-you can Shutdown the while Ture
-
-'''
->>at version 0.2.2.11
-'''
-
-streamline content update
-
-'''
->>at version 0.2.2.12
+>>at version 0.2.2.10 - 0.2.2.14
 '''
 
 practicability update
 
-fix ikun missing
-
-'''
->>at version 0.2.2.13
-'''
+you can Exit it
 
 practicability update
 
 fix loading too long
 
 '''
->>at version 0.2.2.14
+>>at version 0.2.3.1 -0.2.3.4
 '''
-
 practicability update
 
-fix password
-
-'''
->>at version 0.2.3.1
-'''
-
-logo upgrade
-
 make logo more and more modern
 
-'''
->>at version 0.2.3.2
-'''
-
-file control update
-
-make the __file__.py,it can do the file read
-
-'''
->>at version 0.2.3.3
-'''
-
-23333333333333333
-
-streamline content update
-
-delete the __file__.py and in its integration in another file--__lidao__.py
-
-practicability update
-
 make the loading more useful
 
-'''
->>at version 0.2.3.4
-'''
-
 streamline content update
 
-delete the Cutscenes at the time of the change password
-
-because it is too long
-
 practicability update
 
 fix calc is error
 
 file control update
 
-folder kun change to System
-
 '''
->>at version 0.2.4.0 build_version 10.7.1.19920
+>>at version 0.3.*.*
 '''
-version change
-
-there is the latest 0.2 version
+big change
 
 '''
->>at version 0.3.1.0 build_version 33.17.81919
+>>at version 0.4.*.*
 '''
-big change
 
-I can't wait fighting with my computer and dividing it into two piece
+big change
 
 '''
->>at version 0.4.*.*
+>>at version 0.5.0.0
 '''
 
-change some things
+[doge]
 
 '''
->>at version 0.5.0.0
+>>at version 0.5.1.0 -0.5.1.1
 '''
 
 [doge]
 
 '''
```

### Comparing `lichenggong-0.5.1.0/lichenggong/Program_Files/System/__calc__.py` & `lichenggong-0.5.1.1/lichenggong/Program_Files/System/__calc__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.1.0/lichenggong/Program_Files/System/__logo__.py` & `lichenggong-0.5.1.1/lichenggong/Program_Files/System/__logo__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.1.0/lichenggong/Program_Files/System/__user__.py` & `lichenggong-0.5.1.1/lichenggong/Program_Files/System/__user__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.1.0/lichenggong/__init__.py` & `lichenggong-0.5.1.1/lichenggong/__init__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.1.0/lichenggong.egg-info/PKG-INFO` & `lichenggong-0.5.1.1/lichenggong.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.5.1.0
+Version: 0.5.1.1
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `lichenggong-0.5.1.0/lichenggong.egg-info/SOURCES.txt` & `lichenggong-0.5.1.1/lichenggong.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 lichenggong.egg-info/SOURCES.txt
 lichenggong.egg-info/dependency_links.txt
 lichenggong.egg-info/top_level.txt
 lichenggong/Noodows/__bios__.py
 lichenggong/Noodows/__init__.py
 lichenggong/Noodows/__noodows__.py
 lichenggong/Noodows/first.txt
-lichenggong/Noodows/practice.py
-lichenggong/Noodows/python.txt
 lichenggong/Noodows/update.log
 lichenggong/Noodows/version/build_version.txt
 lichenggong/Noodows/version/version.txt
 lichenggong/Program_Files/System/__calc__.py
 lichenggong/Program_Files/System/__logo__.py
 lichenggong/Program_Files/System/__n_explorer__.py
 lichenggong/Program_Files/System/__thanks__.py
```

### Comparing `lichenggong-0.5.1.0/setup.py` & `lichenggong-0.5.1.1/setup.py`

 * *Files identical despite different names*

