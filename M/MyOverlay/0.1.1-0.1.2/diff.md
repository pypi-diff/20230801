# Comparing `tmp/MyOverlay-0.1.1.tar.gz` & `tmp/MyOverlay-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.1.1.tar", last modified: Tue Aug  1 08:49:25 2023, max compression
+gzip compressed data, was "MyOverlay-0.1.2.tar", last modified: Tue Aug  1 09:05:09 2023, max compression
```

## Comparing `MyOverlay-0.1.1.tar` & `MyOverlay-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:49:25.358170 MyOverlay-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-08-01 08:49:25.356171 MyOverlay-0.1.1/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      712 2023-08-01 08:49:25.000000 MyOverlay-0.1.1/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-08-01 08:49:25.000000 MyOverlay-0.1.1/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:49:25.000000 MyOverlay-0.1.1/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-08-01 08:49:25.000000 MyOverlay-0.1.1/MyOverlay.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:49:25.000000 MyOverlay-0.1.1/MyOverlay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      712 2023-08-01 08:49:25.357127 MyOverlay-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-01 08:49:25.358170 MyOverlay-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 09:05:09.309264 MyOverlay-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-08-01 09:05:09.308255 MyOverlay-0.1.2/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      712 2023-08-01 09:05:09.000000 MyOverlay-0.1.2/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-08-01 09:05:09.000000 MyOverlay-0.1.2/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:05:09.000000 MyOverlay-0.1.2/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-01 09:05:09.000000 MyOverlay-0.1.2/MyOverlay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:05:09.000000 MyOverlay-0.1.2/MyOverlay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      712 2023-08-01 09:05:09.309264 MyOverlay-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:05:09.310221 MyOverlay-0.1.2/setup.cfg
```

### Comparing `MyOverlay-0.1.1/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.1.2/MyOverlay.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.1
+Version: 0.1.2
 Summary: Customized Only Text Screen Overlay
 Home-page: https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Author: Erik Reimann
 Author-email: erikreimann28@gmail.com
 License: General Public 3.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `MyOverlay-0.1.1/PKG-INFO` & `MyOverlay-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.1.1
+Version: 0.1.2
 Summary: Customized Only Text Screen Overlay
 Home-page: https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Author: Erik Reimann
 Author-email: erikreimann28@gmail.com
 License: General Public 3.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

