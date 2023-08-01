# Comparing `tmp/dosmaster-1.4.tar.gz` & `tmp/dosmaster-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.4.tar", last modified: Tue Aug  1 20:31:06 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.4.1.tar", last modified: Tue Aug  1 20:36:03 2023, max compression
```

## Comparing `dosmaster-1.4.tar` & `dosmaster-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:31:06.000000 dosmaster-1.4/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      625 2023-08-01 20:31:06.000000 dosmaster-1.4/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1431 2023-08-01 20:28:57.000000 dosmaster-1.4/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:31:06.000000 dosmaster-1.4/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      625 2023-08-01 20:31:06.000000 dosmaster-1.4/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      253 2023-08-01 20:31:06.000000 dosmaster-1.4/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-01 20:31:06.000000 dosmaster-1.4/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       50 2023-08-01 20:31:06.000000 dosmaster-1.4/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       43 2023-08-01 20:31:06.000000 dosmaster-1.4/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        5 2023-08-01 20:31:06.000000 dosmaster-1.4/dosmaster.egg-info/top_level.txt
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:31:06.000000 dosmaster-1.4/main/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      151 2023-08-01 20:29:55.000000 dosmaster-1.4/main/__init__.py
--rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)    52858 2023-08-01 20:30:05.000000 dosmaster-1.4/main/dosmaster.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-01 20:31:06.000000 dosmaster-1.4/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1703 2023-08-01 20:27:19.000000 dosmaster-1.4/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:36:03.000000 dosmaster-1.4.1/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      627 2023-08-01 20:36:03.000000 dosmaster-1.4.1/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1433 2023-08-01 20:35:35.000000 dosmaster-1.4.1/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:36:03.000000 dosmaster-1.4.1/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      627 2023-08-01 20:36:03.000000 dosmaster-1.4.1/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      253 2023-08-01 20:36:03.000000 dosmaster-1.4.1/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-01 20:36:03.000000 dosmaster-1.4.1/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       50 2023-08-01 20:36:03.000000 dosmaster-1.4.1/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       43 2023-08-01 20:36:03.000000 dosmaster-1.4.1/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        5 2023-08-01 20:36:03.000000 dosmaster-1.4.1/dosmaster.egg-info/top_level.txt
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:36:03.000000 dosmaster-1.4.1/main/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-01 20:35:24.000000 dosmaster-1.4.1/main/__init__.py
+-rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)    52897 2023-08-01 20:35:48.000000 dosmaster-1.4.1/main/dosmaster.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-01 20:36:03.000000 dosmaster-1.4.1/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1703 2023-08-01 20:27:19.000000 dosmaster-1.4.1/setup.py
```

### Comparing `dosmaster-1.4/PKG-INFO` & `dosmaster-1.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.4
+Version: 1.4.1
 Summary: DOS(Density Of States) Plot Smartly
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.4/README.md` & `dosmaster-1.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ver.1.1 : 재시작 시 loading 속도 향상 (by Jaesun Kim)
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
-ver.1.4 : PyPI에 올릴 수 있도록 수정
+ver.1.4.1 : PyPI에 올릴 수 있도록 수정
 
 
 ## Source Code Download
 
    1) 서버의 ssh-key를 복사 : 다음의 명령어를 git clone할 서버에서 입력하면 나옴.
```

### Comparing `dosmaster-1.4/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.4.1/dosmaster.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.4
+Version: 1.4.1
 Summary: DOS(Density Of States) Plot Smartly
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.4/main/dosmaster.py` & `dosmaster-1.4.1/main/dosmaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #======================================================================================================
-#Script Name : dosmaster Program(ver.1.4)
+#Script Name : dosmaster Program(ver.1.4.1)
 #Made by Youngjun Park (yjpark29@postech.ac.kr)
 #Inspired by Jaesun Kim
 #Edit Date : 23/06/21
 #======================================================================================================
 #Description : DOS Plot Smartly
 #======================================================================================================
 #: 1) Add Atom DOS
@@ -1097,8 +1097,9 @@
         elif Input_Work == '4':
             graph_config = graph_editor(DOS_list, Labellist, graph_config, color_dict)
         elif Input_Work == '5':
             graph_config = change_sign(graph_config, dos_object_total_dos)
         
         graph_config = DOSplot(DOS_list, Color_list, Labellist, graph_config, color_dict, dos_object_total_dos, dos_object_list, orbital_list, is_save)
 
-
+if __name__ == "__main__":
+    main()
```

### Comparing `dosmaster-1.4/setup.py` & `dosmaster-1.4.1/setup.py`

 * *Files identical despite different names*

