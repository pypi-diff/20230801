# Comparing `tmp/molgenis_emx2_pyclient-8.209.5.tar.gz` & `tmp/molgenis_emx2_pyclient-8.210.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.209.5.tar", last modified: Mon Jul 31 13:41:03 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.210.0.tar", last modified: Tue Aug  1 15:11:24 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.209.5.tar` & `molgenis_emx2_pyclient-8.210.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:41:03.791214 molgenis_emx2_pyclient-8.209.5/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-07-31 13:29:18.000000 molgenis_emx2_pyclient-8.209.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-31 13:41:03.791214 molgenis_emx2_pyclient-8.209.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-31 13:29:19.000000 molgenis_emx2_pyclient-8.209.5/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-31 13:29:19.000000 molgenis_emx2_pyclient-8.209.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 13:29:19.000000 molgenis_emx2_pyclient-8.209.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 13:41:03.791214 molgenis_emx2_pyclient-8.209.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:41:03.787214 molgenis_emx2_pyclient-8.209.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:41:03.791214 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-31 13:29:19.000000 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-07-31 13:29:19.000000 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:41:03.791214 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-31 13:41:03.000000 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-31 13:41:03.000000 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 13:41:03.000000 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 13:41:03.000000 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 13:41:03.000000 molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 13:36:04.000000 molgenis_emx2_pyclient-8.209.5/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:11:24.517749 molgenis_emx2_pyclient-8.210.0/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-08-01 14:59:56.000000 molgenis_emx2_pyclient-8.210.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-08-01 15:11:24.517749 molgenis_emx2_pyclient-8.210.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-08-01 14:59:56.000000 molgenis_emx2_pyclient-8.210.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-08-01 14:59:56.000000 molgenis_emx2_pyclient-8.210.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-01 14:59:56.000000 molgenis_emx2_pyclient-8.210.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 15:11:24.517749 molgenis_emx2_pyclient-8.210.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:11:24.513749 molgenis_emx2_pyclient-8.210.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:11:24.517749 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-01 14:59:56.000000 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-08-01 14:59:56.000000 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:11:24.517749 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-08-01 15:11:24.000000 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-08-01 15:11:24.000000 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 15:11:24.000000 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-01 15:11:24.000000 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-01 15:11:24.000000 molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-01 15:06:24.000000 molgenis_emx2_pyclient-8.210.0/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.209.5/LICENSE` & `molgenis_emx2_pyclient-8.210.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.5/PKG-INFO` & `molgenis_emx2_pyclient-8.210.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.209.5
+Version: 8.210.0
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.209.5/README.md` & `molgenis_emx2_pyclient-8.210.0/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.5/pyproject.toml` & `molgenis_emx2_pyclient-8.210.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.209.5/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.210.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.209.5
+Version: 8.210.0
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

