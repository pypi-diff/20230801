# Comparing `tmp/human_readable_time-0.1.3.tar.gz` & `tmp/human_readable_time-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human_readable_time-0.1.3.tar", last modified: Tue Aug  1 15:00:40 2023, max compression
+gzip compressed data, was "human_readable_time-0.1.4.tar", last modified: Tue Aug  1 15:41:02 2023, max compression
```

## Comparing `human_readable_time-0.1.3.tar` & `human_readable_time-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 15:00:40.012851 human_readable_time-0.1.3/
--rw-rw-rw-   0        0        0     3683 2023-08-01 15:00:39.598847 human_readable_time-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2254 2023-08-01 14:59:45.000000 human_readable_time-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 15:00:38.334848 human_readable_time-0.1.3/human_readable_time/
--rw-rw-rw-   0        0        0      422 2023-07-31 17:26:38.000000 human_readable_time-0.1.3/human_readable_time/human_readable_time.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:00:39.369848 human_readable_time-0.1.3/human_readable_time.egg-info/
--rw-rw-rw-   0        0        0     3683 2023-08-01 15:00:35.000000 human_readable_time-0.1.3/human_readable_time.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-01 15:00:36.000000 human_readable_time-0.1.3/human_readable_time.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 15:00:35.000000 human_readable_time-0.1.3/human_readable_time.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-01 15:00:35.000000 human_readable_time-0.1.3/human_readable_time.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 15:00:40.013850 human_readable_time-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3822 2023-08-01 14:59:26.000000 human_readable_time-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:41:02.000079 human_readable_time-0.1.4/
+-rw-rw-rw-   0        0        0     3683 2023-08-01 15:41:01.972078 human_readable_time-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2254 2023-08-01 14:59:45.000000 human_readable_time-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 15:40:55.338822 human_readable_time-0.1.4/human_readable_time/
+-rw-rw-rw-   0        0        0      578 2023-08-01 15:39:58.000000 human_readable_time-0.1.4/human_readable_time/human_readable_time.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:41:01.969082 human_readable_time-0.1.4/human_readable_time.egg-info/
+-rw-rw-rw-   0        0        0     3683 2023-08-01 15:40:52.000000 human_readable_time-0.1.4/human_readable_time.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-01 15:40:52.000000 human_readable_time-0.1.4/human_readable_time.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 15:40:52.000000 human_readable_time-0.1.4/human_readable_time.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 15:40:52.000000 human_readable_time-0.1.4/human_readable_time.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 15:41:02.001081 human_readable_time-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3822 2023-08-01 15:40:34.000000 human_readable_time-0.1.4/setup.py
```

### Comparing `human_readable_time-0.1.3/PKG-INFO` & `human_readable_time-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: human_readable_time
-Version: 0.1.3
+Version: 0.1.4
 Summary: A utility package for human-readable time conversion.
 Home-page: https://github.com/MuGhasemi/human_readable_time
 Author: Muhammad Ghasemi
 Author-email: mughasemi2008@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `human_readable_time-0.1.3/README.md` & `human_readable_time-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `human_readable_time-0.1.3/human_readable_time.egg-info/PKG-INFO` & `human_readable_time-0.1.4/human_readable_time.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: human-readable-time
-Version: 0.1.3
+Version: 0.1.4
 Summary: A utility package for human-readable time conversion.
 Home-page: https://github.com/MuGhasemi/human_readable_time
 Author: Muhammad Ghasemi
 Author-email: mughasemi2008@email.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `human_readable_time-0.1.3/setup.py` & `human_readable_time-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='human_readable_time',
-    version='0.1.3',
+    version='0.1.4',
     description='A utility package for human-readable time conversion.',
     long_description='''
                     # زمان خوانا
 
                     این یک تابع پایتون است که عددی غیر منفی (ثانیه) را به عنوان ورودی می‌گیرد و زمان را با 
                     فرمت خوانا (ساعت:دقیقه:ثانیه) برمی‌گرداند.
```

