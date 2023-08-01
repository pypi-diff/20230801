# Comparing `tmp/momos-helper-0.0.1.tar.gz` & `tmp/momos-helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/momos-helper-0.0.1.tar", last modified: Tue Aug  1 05:32:23 2023, max compression
+gzip compressed data, was "dist/momos-helper-0.0.2.tar", last modified: Tue Aug  1 05:53:29 2023, max compression
```

## Comparing `momos-helper-0.0.1.tar` & `momos-helper-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwx------   0 shaunchew   (501) staff       (20)        0 2023-08-01 05:32:23.000000 momos-helper-0.0.1/
--rwx------   0 shaunchew   (501) staff       (20)      508 2023-08-01 05:32:23.000000 momos-helper-0.0.1/PKG-INFO
-drwx------   0 shaunchew   (501) staff       (20)        0 2023-08-01 05:32:23.000000 momos-helper-0.0.1/momos-helper/
--rwx------   0 shaunchew   (501) staff       (20)       32 2023-08-01 05:20:34.000000 momos-helper-0.0.1/momos-helper/__init__.py
--rwx------   0 shaunchew   (501) staff       (20)     6075 2023-08-01 05:26:22.000000 momos-helper-0.0.1/momos-helper/postgres_psycopg2.py
-drwx------   0 shaunchew   (501) staff       (20)        0 2023-08-01 05:32:23.000000 momos-helper-0.0.1/momos_helper.egg-info/
--rwx------   0 shaunchew   (501) staff       (20)      508 2023-08-01 05:32:23.000000 momos-helper-0.0.1/momos_helper.egg-info/PKG-INFO
--rwx------   0 shaunchew   (501) staff       (20)      246 2023-08-01 05:32:23.000000 momos-helper-0.0.1/momos_helper.egg-info/SOURCES.txt
--rwx------   0 shaunchew   (501) staff       (20)        1 2023-08-01 05:32:23.000000 momos-helper-0.0.1/momos_helper.egg-info/dependency_links.txt
--rwx------   0 shaunchew   (501) staff       (20)       37 2023-08-01 05:32:23.000000 momos-helper-0.0.1/momos_helper.egg-info/requires.txt
--rwx------   0 shaunchew   (501) staff       (20)       13 2023-08-01 05:32:23.000000 momos-helper-0.0.1/momos_helper.egg-info/top_level.txt
--rwx------   0 shaunchew   (501) staff       (20)       38 2023-08-01 05:32:23.000000 momos-helper-0.0.1/setup.cfg
--rwx------   0 shaunchew   (501) staff       (20)      984 2023-08-01 05:24:11.000000 momos-helper-0.0.1/setup.py
+drwx------   0 shaunchew   (501) staff       (20)        0 2023-08-01 05:53:29.000000 momos-helper-0.0.2/
+-rwx------   0 shaunchew   (501) staff       (20)      502 2023-08-01 05:53:29.000000 momos-helper-0.0.2/PKG-INFO
+drwx------   0 shaunchew   (501) staff       (20)        0 2023-08-01 05:53:29.000000 momos-helper-0.0.2/momos-helper/
+-rwx------   0 shaunchew   (501) staff       (20)       32 2023-08-01 05:20:34.000000 momos-helper-0.0.2/momos-helper/__init__.py
+-rwx------   0 shaunchew   (501) staff       (20)     6075 2023-08-01 05:26:22.000000 momos-helper-0.0.2/momos-helper/postgres_psycopg2.py
+-rwx------   0 shaunchew   (501) staff       (20)     1076 2023-08-01 05:51:14.000000 momos-helper-0.0.2/momos-helper/read_gs.py
+drwx------   0 shaunchew   (501) staff       (20)        0 2023-08-01 05:53:29.000000 momos-helper-0.0.2/momos_helper.egg-info/
+-rwx------   0 shaunchew   (501) staff       (20)      502 2023-08-01 05:53:29.000000 momos-helper-0.0.2/momos_helper.egg-info/PKG-INFO
+-rwx------   0 shaunchew   (501) staff       (20)      270 2023-08-01 05:53:29.000000 momos-helper-0.0.2/momos_helper.egg-info/SOURCES.txt
+-rwx------   0 shaunchew   (501) staff       (20)        1 2023-08-01 05:53:29.000000 momos-helper-0.0.2/momos_helper.egg-info/dependency_links.txt
+-rwx------   0 shaunchew   (501) staff       (20)       72 2023-08-01 05:53:29.000000 momos-helper-0.0.2/momos_helper.egg-info/requires.txt
+-rwx------   0 shaunchew   (501) staff       (20)       13 2023-08-01 05:53:29.000000 momos-helper-0.0.2/momos_helper.egg-info/top_level.txt
+-rwx------   0 shaunchew   (501) staff       (20)       38 2023-08-01 05:53:29.000000 momos-helper-0.0.2/setup.cfg
+-rwx------   0 shaunchew   (501) staff       (20)     1005 2023-08-01 05:53:07.000000 momos-helper-0.0.2/setup.py
```

### Comparing `momos-helper-0.0.1/momos-helper/postgres_psycopg2.py` & `momos-helper-0.0.2/momos-helper/postgres_psycopg2.py`

 * *Files identical despite different names*

### Comparing `momos-helper-0.0.1/setup.py` & `momos-helper-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Momos Helper Package'
 LONG_DESCRIPTION = 'This package is to help increase standardisation & speed of development for Momos internal teams'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="momos-helper",
         version=VERSION,
         author="Shaun Chew",
         author_email="shaun@momos.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['psycopg2-binary==2.8.6','pandas==2.0.3'], # add any additional packages that
-        # needs to be installed along with your package. Eg: 'caer'
+        install_requires=['psycopg2-binary==2.8.6','pandas==2.0.3','gspread==4.0.1','oauth2client==4.1.3'], # add any additional packages that needs to be installed along with your package. Eg: 'caer'
 
-        keywords=['python', 'momos','internal','postgres','boto3','googlesheet'],
+        keywords=['python', 'momos','internal','postgres','googlesheet'],
         classifiers= [
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

