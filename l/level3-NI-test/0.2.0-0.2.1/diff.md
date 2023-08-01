# Comparing `tmp/level3_NI_test-0.2.0.tar.gz` & `tmp/level3_NI_test-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "level3_NI_test-0.2.0.tar", last modified: Tue Aug  1 08:40:01 2023, max compression
+gzip compressed data, was "level3_NI_test-0.2.1.tar", last modified: Tue Aug  1 08:47:13 2023, max compression
```

## Comparing `level3_NI_test-0.2.0.tar` & `level3_NI_test-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:39:59.729738 level3_NI_test-0.2.0/
--rw-rw-rw-   0        0        0      504 2023-08-01 08:40:01.281919 level3_NI_test-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-01 06:19:42.000000 level3_NI_test-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:39:59.768567 level3_NI_test-0.2.0/level3_NI_test/
--rw-rw-rw-   0        0        0      250 2023-07-28 16:44:59.000000 level3_NI_test-0.2.0/level3_NI_test/Level1.py
--rw-rw-rw-   0        0        0      966 2023-08-01 08:39:09.000000 level3_NI_test-0.2.0/level3_NI_test/Level2.py
--rw-rw-rw-   0        0        0        0 2023-08-01 06:20:01.000000 level3_NI_test-0.2.0/level3_NI_test/__init__.py
--rw-rw-rw-   0        0        0     3868 2023-08-01 08:36:57.000000 level3_NI_test-0.2.0/level3_NI_test/level3.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:39:59.800428 level3_NI_test-0.2.0/level3_NI_test.egg-info/
--rw-rw-rw-   0        0        0      504 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 08:40:01.321744 level3_NI_test-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-08-01 08:39:41.000000 level3_NI_test-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:47:12.013982 level3_NI_test-0.2.1/
+-rw-rw-rw-   0        0        0      504 2023-08-01 08:47:13.714512 level3_NI_test-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-01 06:19:42.000000 level3_NI_test-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:47:12.064758 level3_NI_test-0.2.1/level3_NI_test/
+-rw-rw-rw-   0        0        0      298 2023-08-01 08:38:37.000000 level3_NI_test-0.2.1/level3_NI_test/Level1.py
+-rw-rw-rw-   0        0        0      832 2023-07-31 05:59:13.000000 level3_NI_test-0.2.1/level3_NI_test/Level2.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 06:20:01.000000 level3_NI_test-0.2.1/level3_NI_test/__init__.py
+-rw-rw-rw-   0        0        0     3868 2023-08-01 08:36:57.000000 level3_NI_test-0.2.1/level3_NI_test/level3.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:47:12.097613 level3_NI_test-0.2.1/level3_NI_test.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-08-01 08:47:11.000000 level3_NI_test-0.2.1/level3_NI_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-08-01 08:47:11.000000 level3_NI_test-0.2.1/level3_NI_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:47:11.000000 level3_NI_test-0.2.1/level3_NI_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-01 08:47:11.000000 level3_NI_test-0.2.1/level3_NI_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:47:13.767279 level3_NI_test-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-08-01 08:47:06.000000 level3_NI_test-0.2.1/setup.py
```

### Comparing `level3_NI_test-0.2.0/level3_NI_test/Level2.py` & `level3_NI_test-0.2.1/level3_NI_test/Level2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-def main(fileName):
-    main_file = open(fileName)
-    content = main_file.read()
-    lines = content.split('\n')
-    for line in lines[1:]:
-        fields = []
-        to_append = ""
-        split_flag = True
-        for c in range(len(line)):
-            if line[c] == ',' and split_flag:
-                fields.append(to_append)
-                to_append = ''
-            elif line[c] == '"':
-                if line[c-1] == '"':
-                    to_append += '"'
-                elif line[c+1] == '"':
-                    continue
-                else:
-                    split_flag = not split_flag
+main_file = open('sample002.csv')
+content = main_file.read()
+lines = content.split('\n')
+for line in lines[1:]:
+    fields = []
+    to_append = ""
+    split_flag = True
+    for c in range(len(line)):
+        if line[c] == ',' and split_flag:
+            fields.append(to_append)
+            to_append = ''
+        elif line[c] == '"':
+            if line[c-1] == '"':
+                to_append += '"'
+            elif line[c+1] == '"':
+                continue
             else:
-                to_append += line[c]
-        fields.append(to_append)
-        for f in range(1,6):
-            try:
-                print(f'{fields[f]}',end='')
-            except:
-                print(None, end='')
-            if f < 5:
-                print(";",end='')
-        print()
-    main_file.close()
+                split_flag = not split_flag
+        else:
+            to_append += line[c]
+    fields.append(to_append)
+    for f in range(1,6):
+        try:
+            print(f'{fields[f]}',end='')
+        except:
+            print(None, end='')
+        if f < 5:
+            print(";",end='')
+    print()
+main_file.close()
```

### Comparing `level3_NI_test-0.2.0/level3_NI_test/level3.py` & `level3_NI_test-0.2.1/level3_NI_test/level3.py`

 * *Files identical despite different names*

### Comparing `level3_NI_test-0.2.0/setup.py` & `level3_NI_test-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='level3_NI_test',
-    version='0.2.0',
+    version='0.2.1',
     description='Test uploading module to PyPi',
     author='Hamza Daoud',
     author_email='hamzadaoud99@gmail.com',
     packages=find_packages(),
     install_requires=[],  # List any dependencies your package needs
     classifiers=[
         'Development Status :: 3 - Alpha',  # Choose an appropriate status
```

