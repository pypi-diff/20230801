# Comparing `tmp/mangapy-2.0.1.tar.gz` & `tmp/mangapy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangapy-2.0.1.tar", last modified: Tue Aug  1 19:23:11 2023, max compression
+gzip compressed data, was "mangapy-2.0.2.tar", last modified: Tue Aug  1 19:27:13 2023, max compression
```

## Comparing `mangapy-2.0.1.tar` & `mangapy-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.892252 mangapy-2.0.1/
--rw-r--r--   0 alessandro   (501) staff       (20)     1067 2019-12-11 18:08:50.000000 mangapy-2.0.1/LICENSE
--rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-08-01 19:23:11.891668 mangapy-2.0.1/PKG-INFO
--rw-r--r--   0 alessandro   (501) staff       (20)     1946 2023-07-31 15:59:06.000000 mangapy-2.0.1/README.md
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.887820 mangapy-2.0.1/mangapy/
--rw-r--r--   0 alessandro   (501) staff       (20)       51 2020-03-13 14:35:31.000000 mangapy-2.0.1/mangapy/__init__.py
--rw-r--r--   0 alessandro   (501) staff       (20)     4524 2023-07-31 15:59:06.000000 mangapy-2.0.1/mangapy/chapter_archiver.py
--rw-r--r--   0 alessandro   (501) staff       (20)     9061 2023-07-31 15:59:06.000000 mangapy-2.0.1/mangapy/cli.py
--rw-r--r--   0 alessandro   (501) staff       (20)     7412 2023-08-01 12:42:26.000000 mangapy-2.0.1/mangapy/fanfox.py
--rw-r--r--   0 alessandro   (501) staff       (20)      994 2023-07-31 15:59:06.000000 mangapy-2.0.1/mangapy/mangarepository.py
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.890642 mangapy-2.0.1/mangapy.egg-info/
--rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/PKG-INFO
--rw-r--r--   0 alessandro   (501) staff       (20)      358 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/SOURCES.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        1 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/dependency_links.txt
--rw-r--r--   0 alessandro   (501) staff       (20)       45 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/entry_points.txt
--rw-r--r--   0 alessandro   (501) staff       (20)       32 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/requires.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        8 2023-08-01 19:23:11.000000 mangapy-2.0.1/mangapy.egg-info/top_level.txt
--rw-r--r--   0 alessandro   (501) staff       (20)      100 2021-03-23 11:11:45.000000 mangapy-2.0.1/pyproject.toml
--rw-r--r--   0 alessandro   (501) staff       (20)       38 2023-08-01 19:23:11.892384 mangapy-2.0.1/setup.cfg
--rw-r--r--   0 alessandro   (501) staff       (20)     1109 2023-08-01 13:03:22.000000 mangapy-2.0.1/setup.py
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:23:11.891037 mangapy-2.0.1/tests/
--rw-r--r--   0 alessandro   (501) staff       (20)     2962 2023-08-01 13:03:12.000000 mangapy-2.0.1/tests/test_fanfox.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:27:13.537517 mangapy-2.0.2/
+-rw-r--r--   0 alessandro   (501) staff       (20)     1067 2019-12-11 18:08:50.000000 mangapy-2.0.2/LICENSE
+-rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-08-01 19:27:13.537032 mangapy-2.0.2/PKG-INFO
+-rw-r--r--   0 alessandro   (501) staff       (20)     1946 2023-07-31 15:59:06.000000 mangapy-2.0.2/README.md
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:27:13.530289 mangapy-2.0.2/mangapy/
+-rw-r--r--   0 alessandro   (501) staff       (20)       51 2020-03-13 14:35:31.000000 mangapy-2.0.2/mangapy/__init__.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     4527 2023-08-01 19:26:27.000000 mangapy-2.0.2/mangapy/chapter_archiver.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     9061 2023-07-31 15:59:06.000000 mangapy-2.0.2/mangapy/cli.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     7412 2023-08-01 12:42:26.000000 mangapy-2.0.2/mangapy/fanfox.py
+-rw-r--r--   0 alessandro   (501) staff       (20)      994 2023-07-31 15:59:06.000000 mangapy-2.0.2/mangapy/mangarepository.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:27:13.535005 mangapy-2.0.2/mangapy.egg-info/
+-rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-08-01 19:27:13.000000 mangapy-2.0.2/mangapy.egg-info/PKG-INFO
+-rw-r--r--   0 alessandro   (501) staff       (20)      358 2023-08-01 19:27:13.000000 mangapy-2.0.2/mangapy.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        1 2023-08-01 19:27:13.000000 mangapy-2.0.2/mangapy.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)       45 2023-08-01 19:27:13.000000 mangapy-2.0.2/mangapy.egg-info/entry_points.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)       32 2023-08-01 19:27:13.000000 mangapy-2.0.2/mangapy.egg-info/requires.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        8 2023-08-01 19:27:13.000000 mangapy-2.0.2/mangapy.egg-info/top_level.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)      100 2021-03-23 11:11:45.000000 mangapy-2.0.2/pyproject.toml
+-rw-r--r--   0 alessandro   (501) staff       (20)       38 2023-08-01 19:27:13.537617 mangapy-2.0.2/setup.cfg
+-rw-r--r--   0 alessandro   (501) staff       (20)     1109 2023-08-01 19:26:52.000000 mangapy-2.0.2/setup.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-08-01 19:27:13.535769 mangapy-2.0.2/tests/
+-rw-r--r--   0 alessandro   (501) staff       (20)     2962 2023-08-01 13:03:12.000000 mangapy-2.0.2/tests/test_fanfox.py
```

### Comparing `mangapy-2.0.1/LICENSE` & `mangapy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.1/PKG-INFO` & `mangapy-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangapy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Manga downloader
 Home-page: https://github.com/alemar11/mangapy
 Author: Alessandro Marzoli
 Author-email: me@alessandromarzoli.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mangapy-2.0.1/README.md` & `mangapy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.1/mangapy/chapter_archiver.py` & `mangapy-2.0.2/mangapy/chapter_archiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         description = ('Chapter {0}'.format(chapter_name))
         func = partial(self._save_image, chapter_images_path, headers)  # currying
 
         if pdf:
             pdf_path = self.path.joinpath('pdf')
             chapter_pdf_file_path = pdf_path.joinpath(chapter_name + '.pdf')
             if os.path.isfile(chapter_pdf_file_path):
-                print("⏺  {0} already downloaded and it will skipped.".format(chapter_name))
+                print("⏺  {0} already downloaded and it will be skipped.".format(chapter_name))
                 return  # early exit if the file is already on disk
 
         with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
             list(tqdm(executor.map(func, pages), total=len(pages), desc=description, unit='pages', ncols=100))
 
         if pdf:
             pdf_path = self.path.joinpath('pdf')
```

### Comparing `mangapy-2.0.1/mangapy/cli.py` & `mangapy-2.0.2/mangapy/cli.py`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.1/mangapy/fanfox.py` & `mangapy-2.0.2/mangapy/fanfox.py`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.1/mangapy/mangarepository.py` & `mangapy-2.0.2/mangapy/mangarepository.py`

 * *Files identical despite different names*

### Comparing `mangapy-2.0.1/mangapy.egg-info/PKG-INFO` & `mangapy-2.0.2/mangapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangapy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Manga downloader
 Home-page: https://github.com/alemar11/mangapy
 Author: Alessandro Marzoli
 Author-email: me@alessandromarzoli.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mangapy-2.0.1/setup.py` & `mangapy-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     author="Alessandro Marzoli",
     author_email="me@alessandromarzoli.com",
     name='mangapy',
     license="MIT",
     description='Manga downloader',
-    version='2.0.1',
+    version='2.0.2',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/alemar11/mangapy',
     packages=find_packages(),
     python_requires=">=3.11",
     install_requires=['bs4', 'pillow', 'pyyaml', 'requests', 'tqdm'],
     classifiers=[
```

### Comparing `mangapy-2.0.1/tests/test_fanfox.py` & `mangapy-2.0.2/tests/test_fanfox.py`

 * *Files identical despite different names*

