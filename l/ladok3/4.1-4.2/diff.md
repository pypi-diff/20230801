# Comparing `tmp/ladok3-4.1.tar.gz` & `tmp/ladok3-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladok3-4.1.tar", max compression
+gzip compressed data, was "ladok3-4.2.tar", max compression
```

## Comparing `ladok3-4.1.tar` & `ladok3-4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-4.1/LICENSE
--rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-4.1/README.md
--rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-4.1/doc/Makefile
--rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-4.1/doc/abstract.tex
--rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-4.1/doc/ladok3.tex
--rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-4.1/doc/preamble.tex
--rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-4.1/makefiles/doc.mk
--rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-4.1/makefiles/exam.mk
--rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/haskell.mk
--rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-4.1/makefiles/miun.course.mk
--rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/miun.depend.mk
--rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/miun.docs.mk
--rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/miun.port.mk
--rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/miun.pub.mk
--rw-r--r--   0        0        0     2912 2023-06-09 13:33:51.987944 ladok3-4.1/makefiles/noweb.mk
--rw-r--r--   0        0        0     2363 2023-06-09 13:33:51.611939 ladok3-4.1/makefiles/pkg.mk
--rw-r--r--   0        0        0     1225 2023-06-09 13:33:51.971944 ladok3-4.1/makefiles/portability.mk
--rw-r--r--   0        0        0     4827 2023-06-09 13:33:51.579938 ladok3-4.1/makefiles/pub.mk
--rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/results.mk
--rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/subdir.mk
--rw-r--r--   0        0        0     6376 2023-06-09 13:33:51.979944 ladok3-4.1/makefiles/tex.mk
--rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-4.1/makefiles/transform.mk
--rw-r--r--   0        0        0     1766 2023-06-27 20:00:54.564702 ladok3-4.1/pyproject.toml
--rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-4.1/src/ladok3/.gitignore
--rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-4.1/src/ladok3/Makefile
--rw-r--r--   0        0        0    43304 2023-06-27 12:08:54.288682 ladok3-4.1/src/ladok3/api.nw
--rw-r--r--   0        0        0    20641 2023-06-21 18:24:44.772562 ladok3-4.1/src/ladok3/cli.nw
--rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-4.1/src/ladok3/data.nw
--rw-r--r--   0        0        0    50196 2023-06-27 12:08:54.288682 ladok3-4.1/src/ladok3/ladok3.nw
--rw-r--r--   0        0        0     8972 2023-06-27 18:22:41.616669 ladok3-4.1/src/ladok3/report.nw
--rw-r--r--   0        0        0     3747 2023-06-08 20:54:19.896194 ladok3-4.1/src/ladok3/student.nw
--rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-4.1/src/ladok3/undoc.nw
--rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-4.1/PKG-INFO
+-rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-4.2/LICENSE
+-rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-4.2/README.md
+-rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-4.2/doc/Makefile
+-rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-4.2/doc/abstract.tex
+-rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-4.2/doc/ladok3.tex
+-rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-4.2/doc/preamble.tex
+-rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-4.2/makefiles/doc.mk
+-rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-4.2/makefiles/exam.mk
+-rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/haskell.mk
+-rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-4.2/makefiles/miun.course.mk
+-rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/miun.depend.mk
+-rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/miun.docs.mk
+-rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/miun.port.mk
+-rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/miun.pub.mk
+-rw-r--r--   0        0        0     2912 2023-06-09 13:33:51.987944 ladok3-4.2/makefiles/noweb.mk
+-rw-r--r--   0        0        0     2363 2023-06-09 13:33:51.611939 ladok3-4.2/makefiles/pkg.mk
+-rw-r--r--   0        0        0     1225 2023-06-09 13:33:51.971944 ladok3-4.2/makefiles/portability.mk
+-rw-r--r--   0        0        0     4827 2023-06-09 13:33:51.579938 ladok3-4.2/makefiles/pub.mk
+-rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/results.mk
+-rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/subdir.mk
+-rw-r--r--   0        0        0     6376 2023-06-09 13:33:51.979944 ladok3-4.2/makefiles/tex.mk
+-rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-4.2/makefiles/transform.mk
+-rw-r--r--   0        0        0     1766 2023-08-01 18:56:09.757357 ladok3-4.2/pyproject.toml
+-rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-4.2/src/ladok3/.gitignore
+-rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-4.2/src/ladok3/Makefile
+-rw-r--r--   0        0        0    43304 2023-06-27 12:08:54.288682 ladok3-4.2/src/ladok3/api.nw
+-rw-r--r--   0        0        0    20641 2023-06-21 18:24:44.772562 ladok3-4.2/src/ladok3/cli.nw
+-rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-4.2/src/ladok3/data.nw
+-rw-r--r--   0        0        0    50196 2023-06-27 12:08:54.288682 ladok3-4.2/src/ladok3/ladok3.nw
+-rw-r--r--   0        0        0     8972 2023-06-27 18:22:41.616669 ladok3-4.2/src/ladok3/report.nw
+-rw-r--r--   0        0        0     3747 2023-06-08 20:54:19.896194 ladok3-4.2/src/ladok3/student.nw
+-rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-4.2/src/ladok3/undoc.nw
+-rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-4.2/PKG-INFO
```

### Comparing `ladok3-4.1/LICENSE` & `ladok3-4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/README.md` & `ladok3-4.2/README.md`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/doc/Makefile` & `ladok3-4.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/doc/ladok3.tex` & `ladok3-4.2/doc/ladok3.tex`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/doc/preamble.tex` & `ladok3-4.2/doc/preamble.tex`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/doc.mk` & `ladok3-4.2/makefiles/doc.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/exam.mk` & `ladok3-4.2/makefiles/exam.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/miun.course.mk` & `ladok3-4.2/makefiles/miun.course.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/miun.depend.mk` & `ladok3-4.2/makefiles/miun.depend.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/miun.docs.mk` & `ladok3-4.2/makefiles/miun.docs.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/miun.port.mk` & `ladok3-4.2/makefiles/miun.port.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/miun.pub.mk` & `ladok3-4.2/makefiles/miun.pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/noweb.mk` & `ladok3-4.2/makefiles/noweb.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/pkg.mk` & `ladok3-4.2/makefiles/pkg.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/portability.mk` & `ladok3-4.2/makefiles/portability.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/pub.mk` & `ladok3-4.2/makefiles/pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/results.mk` & `ladok3-4.2/makefiles/results.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/tex.mk` & `ladok3-4.2/makefiles/tex.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/makefiles/transform.mk` & `ladok3-4.2/makefiles/transform.mk`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/pyproject.toml` & `ladok3-4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ladok3"
-version = "4.1"
+version = "4.2"
 description = "Python wrapper and CLI for the LADOK3 REST API."
 authors = [
   "Daniel Bosk <dbosk@kth.se>",
   "Alexander Baltatzis",
   "Gerald Q. Maguire Jr"
 ]
 license = "MIT"
@@ -48,17 +48,17 @@
 "Releases" = "https://github.com/dbosk/ladok3/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 appdirs = "^1.4.4"
 argcomplete = "^2.0.0"
 cachetools = "^5.2.0"
-cryptography = "^37.0.3"
+cryptography = "^38.0.3"
 keyring = "^23.6.0"
-requests = "^2.28.0"
+requests = "^2.31.0"
 urllib3 = "^1.26.9"
 weblogin = "^1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 numpy = "^1.23.4"
 pandas = "^1.5.1"
```

### Comparing `ladok3-4.1/src/ladok3/Makefile` & `ladok3-4.2/src/ladok3/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/src/ladok3/api.nw` & `ladok3-4.2/src/ladok3/api.nw`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/src/ladok3/cli.nw` & `ladok3-4.2/src/ladok3/cli.nw`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/src/ladok3/data.nw` & `ladok3-4.2/src/ladok3/data.nw`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/src/ladok3/ladok3.nw` & `ladok3-4.2/src/ladok3/ladok3.nw`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/src/ladok3/report.nw` & `ladok3-4.2/src/ladok3/report.nw`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/src/ladok3/student.nw` & `ladok3-4.2/src/ladok3/student.nw`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/src/ladok3/undoc.nw` & `ladok3-4.2/src/ladok3/undoc.nw`

 * *Files identical despite different names*

### Comparing `ladok3-4.1/PKG-INFO` & `ladok3-4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladok3
-Version: 4.1
+Version: 4.2
 Summary: Python wrapper and CLI for the LADOK3 REST API.
 Home-page: https://github.com/dbosk/ladok3
 License: MIT
 Keywords: ladok3,ladok
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: argcomplete (>=2.0.0,<3.0.0)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
-Requires-Dist: cryptography (>=37.0.3,<38.0.0)
+Requires-Dist: cryptography (>=38.0.3,<39.0.0)
 Requires-Dist: keyring (>=23.6.0,<24.0.0)
-Requires-Dist: requests (>=2.28.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
 Requires-Dist: weblogin (>=1.5,<2.0)
 Project-URL: Bug Tracker, https://github.com/dbosk/ladok3/issues
 Project-URL: Repository, https://github.com/dbosk/ladok3
 Project-URL: Releases, https://github.com/dbosk/ladok3/releases
 Description-Content-Type: text/markdown
```

