# Comparing `tmp/recorder-viz-0.4.7.tar.gz` & `tmp/recorder-viz-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recorder-viz-0.4.7.tar", last modified: Wed Mar 22 23:19:06 2023, max compression
+gzip compressed data, was "dist/recorder-viz-0.4.8.tar", last modified: Tue Aug  1 16:49:31 2023, max compression
```

## Comparing `recorder-viz-0.4.7.tar` & `recorder-viz-0.4.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 wangchen  (1000) wangchen  (1000)        0 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/
-drwxr-xr-x   0 wangchen  (1000) wangchen  (1000)        0 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/recorder_viz.egg-info/
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)     3692 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/recorder_viz.egg-info/PKG-INFO
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)       36 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/recorder_viz.egg-info/top_level.txt
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)        1 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/recorder_viz.egg-info/dependency_links.txt
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)      408 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/recorder_viz.egg-info/SOURCES.txt
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)     2469 2021-10-07 01:02:07.000000 recorder-viz-0.4.7/README.md
-drwxr-xr-x   0 wangchen  (1000) wangchen  (1000)        0 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/recorder_viz/
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)      144 2023-03-22 23:18:54.000000 recorder-viz-0.4.7/recorder_viz/__init__.py
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)     4940 2021-10-15 18:23:19.000000 recorder-viz-0.4.7/recorder_viz/html_writer.py
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)    19894 2022-09-13 15:47:03.000000 recorder-viz-0.4.7/recorder_viz/reporter.py
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)    10134 2023-03-22 22:07:47.000000 recorder-viz-0.4.7/recorder_viz/recorder-logger.h
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)    12342 2023-03-22 23:15:11.000000 recorder-viz-0.4.7/recorder_viz/reader.c
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)    73928 2021-10-07 00:52:49.000000 recorder-viz-0.4.7/recorder_viz/uthash.h
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)     8633 2021-10-15 15:57:51.000000 recorder-viz-0.4.7/recorder_viz/build_offset_intervals.py
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)     4203 2023-03-22 23:15:25.000000 recorder-viz-0.4.7/recorder_viz/reader.h
--rw-rw-r--   0 wangchen  (1000) wangchen  (1000)     3991 2023-03-22 23:15:34.000000 recorder-viz-0.4.7/recorder_viz/creader_wrapper.py
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)     3692 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/PKG-INFO
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)       38 2023-03-22 23:19:06.000000 recorder-viz-0.4.7/setup.cfg
--rw-r--r--   0 wangchen  (1000) wangchen  (1000)     1753 2023-03-22 23:18:44.000000 recorder-viz-0.4.7/setup.py
+drwxr-xr-x   0 wangchen  (1000) wangchen  (1000)        0 2023-08-01 16:49:31.000000 recorder-viz-0.4.8/
+drwxr-xr-x   0 wangchen  (1000) wangchen  (1000)        0 2023-08-01 16:49:31.000000 recorder-viz-0.4.8/recorder_viz.egg-info/
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)     3692 2023-08-01 16:49:30.000000 recorder-viz-0.4.8/recorder_viz.egg-info/PKG-INFO
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)       36 2023-08-01 16:49:30.000000 recorder-viz-0.4.8/recorder_viz.egg-info/top_level.txt
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)        1 2023-08-01 16:49:30.000000 recorder-viz-0.4.8/recorder_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)      408 2023-08-01 16:49:30.000000 recorder-viz-0.4.8/recorder_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)     2469 2021-10-07 01:02:07.000000 recorder-viz-0.4.8/README.md
+drwxr-xr-x   0 wangchen  (1000) wangchen  (1000)        0 2023-08-01 16:49:31.000000 recorder-viz-0.4.8/recorder_viz/
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)      144 2023-08-01 16:48:02.000000 recorder-viz-0.4.8/recorder_viz/__init__.py
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)     4940 2021-10-15 18:23:19.000000 recorder-viz-0.4.8/recorder_viz/html_writer.py
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)    19894 2022-09-13 15:47:03.000000 recorder-viz-0.4.8/recorder_viz/reporter.py
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)    10134 2023-03-22 22:07:47.000000 recorder-viz-0.4.8/recorder_viz/recorder-logger.h
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)    12342 2023-08-01 16:48:36.000000 recorder-viz-0.4.8/recorder_viz/reader.c
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)    73928 2021-10-07 00:52:49.000000 recorder-viz-0.4.8/recorder_viz/uthash.h
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)     8633 2021-10-15 15:57:51.000000 recorder-viz-0.4.8/recorder_viz/build_offset_intervals.py
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)     3984 2023-08-01 16:48:17.000000 recorder-viz-0.4.8/recorder_viz/reader.h
+-rw-rw-r--   0 wangchen  (1000) wangchen  (1000)     3991 2023-03-22 23:15:34.000000 recorder-viz-0.4.8/recorder_viz/creader_wrapper.py
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)     3692 2023-08-01 16:49:31.000000 recorder-viz-0.4.8/PKG-INFO
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)       38 2023-08-01 16:49:31.000000 recorder-viz-0.4.8/setup.cfg
+-rw-r--r--   0 wangchen  (1000) wangchen  (1000)     1753 2023-08-01 16:47:43.000000 recorder-viz-0.4.8/setup.py
```

### Comparing `recorder-viz-0.4.7/recorder_viz.egg-info/PKG-INFO` & `recorder-viz-0.4.8/recorder_viz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recorder-viz
-Version: 0.4.7
+Version: 0.4.8
 Summary: Utilities for processing Recorder traces
 Home-page: https://github.com/wangvsa/recorder-viz
 Author: Chen Wang
 Author-email: wangvsa@gmail.com
 License: UNKNOWN
 Description: recorder-viz
         =============
```

### Comparing `recorder-viz-0.4.7/README.md` & `recorder-viz-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/recorder_viz/html_writer.py` & `recorder-viz-0.4.8/recorder_viz/html_writer.py`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/recorder_viz/reporter.py` & `recorder-viz-0.4.8/recorder_viz/reporter.py`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/recorder_viz/recorder-logger.h` & `recorder-viz-0.4.8/recorder_viz/recorder-logger.h`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/recorder_viz/reader.c` & `recorder-viz-0.4.8/recorder_viz/reader.c`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/recorder_viz/uthash.h` & `recorder-viz-0.4.8/recorder_viz/uthash.h`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/recorder_viz/build_offset_intervals.py` & `recorder-viz-0.4.8/recorder_viz/build_offset_intervals.py`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/recorder_viz/reader.h` & `recorder-viz-0.4.8/recorder_viz/reader.h`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #define _RECORDER_READER_H_
 #include <stdbool.h>
 #include "recorder-logger.h"
 
 // keep in sync with VERSION_STR in lib/recorder-logger.c
 // equal (major, minor) is needed for compatibility
 #define VERSION_MAJOR 		2
-#define VERSION_MINOR 		4
+#define VERSION_MINOR 		5
 #define VERSION_PATCH 		0
 
 #define POSIX_SEMANTICS 	0
 #define COMMIT_SEMANTICS 	1
 #define SESSION_SEMANTICS	2
 
 #ifdef __cplusplus
@@ -24,26 +24,21 @@
     int seqId;              // The sequence id of the I/O call
     double tstart;
     size_t offset;
     size_t count;
     bool isRead;
 } Interval;
 
+/* Per-file intervals
+ * <filename, intervals>
+ */
 typedef struct IntervalsMap_t {
     char* filename;
     size_t num_intervals;
     Interval *intervals;    // Pointer to Interval, copied from vector<Interval>
-
-    int *num_opens;         // num_opens[rank] is list of number of opens for rank
-    int *num_closes;
-    int *num_commits;
-
-    double **topens;        // topens[rank] is a list of open timestamps for rank
-    double **tcloses;
-    double **tcommits;
 } IntervalsMap;
 
 typedef struct CST_t {
     int rank;
     int entries;
     CallSignature *cs_list; // CallSignature is defined in recorder-logger.h
 } CST;
@@ -154,14 +149,14 @@
  *  - RECORDER_MPI
  *  - RECORDER_HDF5
  *  - RECORDER_FTRACE
  */
 int recorder_get_func_type(RecorderReader* reader, Record* record);
 
 
-IntervalsMap* build_offset_intervals(RecorderReader *reader, int semantics, int *num_files);
+IntervalsMap* build_offset_intervals(RecorderReader *reader, int *num_files);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif
```

### Comparing `recorder-viz-0.4.7/recorder_viz/creader_wrapper.py` & `recorder-viz-0.4.8/recorder_viz/creader_wrapper.py`

 * *Files identical despite different names*

### Comparing `recorder-viz-0.4.7/PKG-INFO` & `recorder-viz-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recorder-viz
-Version: 0.4.7
+Version: 0.4.8
 Summary: Utilities for processing Recorder traces
 Home-page: https://github.com/wangvsa/recorder-viz
 Author: Chen Wang
 Author-email: wangvsa@gmail.com
 License: UNKNOWN
 Description: recorder-viz
         =============
```

### Comparing `recorder-viz-0.4.7/setup.py` & `recorder-viz-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="recorder-viz",                # Package name, e.g., pip install recorder-viz
-    version="0.4.7",
+    version="0.4.8",
     author="Chen Wang",
     author_email="wangvsa@gmail.com",
     description="Utilities for processing Recorder traces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wangvsa/recorder-viz",
     packages=['recorder_viz'],                  # package for import: after installaion, import recorder_viz
```

