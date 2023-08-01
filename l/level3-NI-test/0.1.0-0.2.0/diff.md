# Comparing `tmp/level3_NI_test-0.1.0.tar.gz` & `tmp/level3_NI_test-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "level3_NI_test-0.1.0.tar", last modified: Tue Aug  1 06:25:31 2023, max compression
+gzip compressed data, was "level3_NI_test-0.2.0.tar", last modified: Tue Aug  1 08:40:01 2023, max compression
```

## Comparing `level3_NI_test-0.1.0.tar` & `level3_NI_test-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 06:25:29.943503 level3_NI_test-0.1.0/
--rw-rw-rw-   0        0        0      486 2023-08-01 06:25:31.197996 level3_NI_test-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-01 06:19:42.000000 level3_NI_test-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 06:25:29.987137 level3_NI_test-0.1.0/level3_NI_test/
--rw-rw-rw-   0        0        0        0 2023-08-01 06:20:01.000000 level3_NI_test-0.1.0/level3_NI_test/__init__.py
--rw-rw-rw-   0        0        0     3891 2023-08-01 06:23:36.000000 level3_NI_test-0.1.0/level3_NI_test/level3.py
-drwxrwxrwx   0        0        0        0 2023-08-01 06:25:30.019170 level3_NI_test-0.1.0/level3_NI_test.egg-info/
--rw-rw-rw-   0        0        0      486 2023-08-01 06:25:29.000000 level3_NI_test-0.1.0/level3_NI_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-08-01 06:25:29.000000 level3_NI_test-0.1.0/level3_NI_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 06:25:29.000000 level3_NI_test-0.1.0/level3_NI_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-01 06:25:29.000000 level3_NI_test-0.1.0/level3_NI_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 06:25:31.230850 level3_NI_test-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-08-01 06:21:56.000000 level3_NI_test-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:39:59.729738 level3_NI_test-0.2.0/
+-rw-rw-rw-   0        0        0      504 2023-08-01 08:40:01.281919 level3_NI_test-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-01 06:19:42.000000 level3_NI_test-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 08:39:59.768567 level3_NI_test-0.2.0/level3_NI_test/
+-rw-rw-rw-   0        0        0      250 2023-07-28 16:44:59.000000 level3_NI_test-0.2.0/level3_NI_test/Level1.py
+-rw-rw-rw-   0        0        0      966 2023-08-01 08:39:09.000000 level3_NI_test-0.2.0/level3_NI_test/Level2.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 06:20:01.000000 level3_NI_test-0.2.0/level3_NI_test/__init__.py
+-rw-rw-rw-   0        0        0     3868 2023-08-01 08:36:57.000000 level3_NI_test-0.2.0/level3_NI_test/level3.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:39:59.800428 level3_NI_test-0.2.0/level3_NI_test.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-01 08:39:59.000000 level3_NI_test-0.2.0/level3_NI_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:40:01.321744 level3_NI_test-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-08-01 08:39:41.000000 level3_NI_test-0.2.0/setup.py
```

### Comparing `level3_NI_test-0.1.0/level3_NI_test/level3.py` & `level3_NI_test-0.2.0/level3_NI_test/level3.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,9 +105,8 @@
                 toWrite += '4,'
         last += ',None\n'
         toWrite = f'{toWrite[:-1]}\n'
     convert_to_hex(last)
     with open('output003.csv','w') as csvF:
         csvF.write(toWrite[:-1])
 
-    main_file.close()
-main('sample003.csv')
+    main_file.close()
```

### Comparing `level3_NI_test-0.1.0/setup.py` & `level3_NI_test-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='level3_NI_test',
-    version='0.1.0',
-    description='description',
+    version='0.2.0',
+    description='Test uploading module to PyPi',
     author='Hamza Daoud',
     author_email='hamzadaoud99@gmail.com',
     packages=find_packages(),
     install_requires=[],  # List any dependencies your package needs
     classifiers=[
         'Development Status :: 3 - Alpha',  # Choose an appropriate status
         'Intended Audience :: Developers',
```

