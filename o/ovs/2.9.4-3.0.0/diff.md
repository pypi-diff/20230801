# Comparing `tmp/ovs-2.9.4.tar.gz` & `tmp/ovs-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ovs-2.9.4.tar", last modified: Tue Jun 25 14:05:47 2019, max compression
+gzip compressed data, was "ovs-3.0.0.tar", last modified: Tue Aug  1 18:47:51 2023, max compression
```

## Comparing `ovs-2.9.4.tar` & `ovs-3.0.0.tar`

### file list

```diff
@@ -1,51 +1,63 @@
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2019-06-25 14:05:47.000000 ovs-2.9.4/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs/compat/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs/compat/sortedcontainers/
--rw-rw-r--   0 terry     (1000) terry     (1000)     1603 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/compat/sortedcontainers/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    27200 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/compat/sortedcontainers/sorteddict.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    76797 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/compat/sortedcontainers/sortedlist.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    10093 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/compat/sortedcontainers/sortedset.py
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/compat/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs/db/
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/db/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     4856 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/db/custom_index.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    20446 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/db/data.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1160 2019-06-21 18:36:31.000000 ovs-2.9.4/ovs/db/error.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    75694 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/db/idl.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     3703 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/db/parser.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    12104 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/db/schema.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    23189 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/db/types.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs/unixctl/
--rw-rw-r--   0 terry     (1000) terry     (1000)     3086 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/unixctl/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     2049 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/unixctl/client.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     8223 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/unixctl/server.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     7459 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/_json.c
--rw-rw-r--   0 terry     (1000) terry     (1000)    20710 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/daemon.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1337 2019-03-19 22:35:03.000000 ovs-2.9.4/ovs/dirs.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     4608 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/fatal_signal.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1330 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/fcntl_win.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    17041 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/json.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    19748 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/jsonrpc.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1929 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/ovsuuid.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     9359 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/poller.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1467 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/process.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    24057 2019-06-21 18:36:31.000000 ovs-2.9.4/ovs/reconnect.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    11590 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/socket_util.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    30224 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/stream.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     2432 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/timeval.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     3119 2019-06-25 14:01:00.000000 ovs-2.9.4/ovs/util.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       93 2019-06-25 14:05:23.000000 ovs-2.9.4/ovs/version.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    16525 2019-06-25 14:03:20.000000 ovs-2.9.4/ovs/vlog.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     9226 2019-03-19 22:33:55.000000 ovs-2.9.4/ovs/winutils.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)      786 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      828 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       17 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        4 2019-06-25 14:05:47.000000 ovs-2.9.4/ovs.egg-info/top_level.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       45 2019-03-19 22:33:55.000000 ovs-2.9.4/README.rst
--rw-rw-r--   0 terry     (1000) terry     (1000)     3266 2019-06-21 18:36:31.000000 ovs-2.9.4/setup.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      786 2019-06-25 14:05:47.000000 ovs-2.9.4/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2019-06-25 14:05:47.000000 ovs-2.9.4/setup.cfg
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.685744 ovs-3.0.0/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 18:47:51.685744 ovs-3.0.0/PKG-INFO
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       45 2021-09-20 16:15:26.000000 ovs-3.0.0/README.rst
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.680744 ovs-3.0.0/ovs/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     7038 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/_json.c
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.681744 ovs-3.0.0/ovs/compat/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        0 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/compat/__init__.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.682744 ovs-3.0.0/ovs/compat/sortedcontainers/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     2131 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    22712 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/sorteddict.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    76293 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/sortedlist.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    19825 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/compat/sortedcontainers/sortedset.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    20710 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/daemon.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.683744 ovs-3.0.0/ovs/db/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/db/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4856 2021-11-05 13:35:58.000000 ovs-3.0.0/ovs/db/custom_index.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    21659 2023-06-14 20:52:13.000000 ovs-3.0.0/ovs/db/data.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1156 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/db/error.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    96770 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/db/idl.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3647 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/db/parser.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    11947 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/db/schema.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    23240 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/db/types.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1329 2023-08-01 18:44:12.000000 ovs-3.0.0/ovs/dirs.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4765 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/fatal_signal.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1330 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/fcntl_win.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.684744 ovs-3.0.0/ovs/flow/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      476 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    14382 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/decoders.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     7502 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/filter.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3772 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/flow/flow.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    10505 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/kv.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3819 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/list.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    26900 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/odp.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    13396 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/ofp.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     8786 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/flow/ofp_act.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     7348 2023-08-01 18:44:27.000000 ovs-3.0.0/ovs/flow/ofp_fields.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    16843 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/json.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    21087 2023-04-18 01:01:46.000000 ovs-3.0.0/ovs/jsonrpc.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1869 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/ovsuuid.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    10282 2023-01-27 14:27:10.000000 ovs-3.0.0/ovs/poller.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1467 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/process.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    26007 2023-05-17 03:37:46.000000 ovs-3.0.0/ovs/reconnect.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    11976 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/socket_util.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    32107 2023-08-01 15:27:48.000000 ovs-3.0.0/ovs/stream.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     2432 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/timeval.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.684744 ovs-3.0.0/ovs/unixctl/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3032 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/unixctl/__init__.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1999 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/unixctl/client.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     8121 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/unixctl/server.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     3120 2022-09-19 19:15:14.000000 ovs-3.0.0/ovs/util.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       93 2023-08-01 18:44:27.000000 ovs-3.0.0/ovs/version.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)    16694 2021-10-20 17:21:43.000000 ovs-3.0.0/ovs/vlog.py
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     9226 2021-09-20 16:15:26.000000 ovs-3.0.0/ovs/winutils.py
+drwxrwxr-x   0 twilson   (1000) twilson   (1000)        0 2023-08-01 18:47:51.681744 ovs-3.0.0/ovs.egg-info/
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)      670 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/PKG-INFO
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     1028 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/SOURCES.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        1 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/dependency_links.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       84 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/requires.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)        4 2023-08-01 18:47:51.000000 ovs-3.0.0/ovs.egg-info/top_level.txt
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       85 2022-04-28 18:38:11.000000 ovs-3.0.0/pyproject.toml
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)       38 2023-08-01 18:47:51.685744 ovs-3.0.0/setup.cfg
+-rw-rw-r--   0 twilson   (1000) twilson   (1000)     4350 2023-08-01 15:27:48.000000 ovs-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ovs-2.9.4/ovs/compat/sortedcontainers/sortedlist.py` & `ovs-3.0.0/ovs/compat/sortedcontainers/sortedlist.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,174 +1,309 @@
-"""Sorted list implementation.
+"""Sorted List
+==============
+
+:doc:`Sorted Containers<index>` is an Apache2 licensed Python sorted
+collections library, written in pure-Python, and fast as C-extensions. The
+:doc:`introduction<introduction>` is the best way to get started.
+
+Sorted list implementations:
+
+.. currentmodule:: sortedcontainers
+
+* :class:`SortedList`
+* :class:`SortedKeyList`
 
 """
-# pylint: disable=redefined-builtin, ungrouped-imports
+# pylint: disable=too-many-lines
 
-from __future__ import print_function
+import sys
+import traceback
 
 from bisect import bisect_left, bisect_right, insort
-from collections import Sequence, MutableSequence
-from functools import wraps
 from itertools import chain, repeat, starmap
-from math import log as log_e
-import operator as op
-from operator import iadd, add
+from math import log
+from operator import add, eq, ne, gt, ge, lt, le, iadd
+from textwrap import dedent
+
+###############################################################################
+# BEGIN Python 2/3 Shims
+###############################################################################
+
+try:
+    from collections.abc import Sequence, MutableSequence
+except ImportError:
+    from collections import Sequence, MutableSequence
+
+from functools import wraps
 from sys import hexversion
 
 if hexversion < 0x03000000:
-    from itertools import izip as zip  # pylint: disable=no-name-in-module
-    from itertools import imap as map  # pylint: disable=no-name-in-module
+    from itertools import imap as map  # pylint: disable=redefined-builtin
+    from itertools import izip as zip  # pylint: disable=redefined-builtin
     try:
         from thread import get_ident
     except ImportError:
         from dummy_thread import get_ident
 else:
     from functools import reduce
     try:
         from _thread import get_ident
     except ImportError:
-        from _dummy_thread import get_ident # pylint: disable=import-error
+        from _dummy_thread import get_ident
 
-LOAD = 1000
 
-def recursive_repr(func):
-    """Decorator to prevent infinite repr recursion."""
-    repr_running = set()
+def recursive_repr(fillvalue='...'):
+    "Decorator to make a repr function return fillvalue for a recursive call."
+    # pylint: disable=missing-docstring
+    # Copied from reprlib in Python 3
+    # https://hg.python.org/cpython/file/3.6/Lib/reprlib.py
+
+    def decorating_function(user_function):
+        repr_running = set()
+
+        @wraps(user_function)
+        def wrapper(self):
+            key = id(self), get_ident()
+            if key in repr_running:
+                return fillvalue
+            repr_running.add(key)
+            try:
+                result = user_function(self)
+            finally:
+                repr_running.discard(key)
+            return result
+
+        return wrapper
+
+    return decorating_function
+
+###############################################################################
+# END Python 2/3 Shims
+###############################################################################
 
-    @wraps(func)
-    def wrapper(self):
-        "Return ellipsis on recursive re-entry to function."
-        key = id(self), get_ident()
 
-        if key in repr_running:
-            return '...'
+class SortedList(MutableSequence):
+    """Sorted list is a sorted mutable sequence.
 
-        repr_running.add(key)
+    Sorted list values are maintained in sorted order.
 
-        try:
-            return func(self)
-        finally:
-            repr_running.discard(key)
+    Sorted list values must be comparable. The total ordering of values must
+    not change while they are stored in the sorted list.
 
-    return wrapper
+    Methods for adding values:
+
+    * :func:`SortedList.add`
+    * :func:`SortedList.update`
+    * :func:`SortedList.__add__`
+    * :func:`SortedList.__iadd__`
+    * :func:`SortedList.__mul__`
+    * :func:`SortedList.__imul__`
+
+    Methods for removing values:
+
+    * :func:`SortedList.clear`
+    * :func:`SortedList.discard`
+    * :func:`SortedList.remove`
+    * :func:`SortedList.pop`
+    * :func:`SortedList.__delitem__`
+
+    Methods for looking up values:
+
+    * :func:`SortedList.bisect_left`
+    * :func:`SortedList.bisect_right`
+    * :func:`SortedList.count`
+    * :func:`SortedList.index`
+    * :func:`SortedList.__contains__`
+    * :func:`SortedList.__getitem__`
+
+    Methods for iterating values:
+
+    * :func:`SortedList.irange`
+    * :func:`SortedList.islice`
+    * :func:`SortedList.__iter__`
+    * :func:`SortedList.__reversed__`
+
+    Methods for miscellany:
+
+    * :func:`SortedList.copy`
+    * :func:`SortedList.__len__`
+    * :func:`SortedList.__repr__`
+    * :func:`SortedList._check`
+    * :func:`SortedList._reset`
+
+    Sorted lists use lexicographical ordering semantics when compared to other
+    sequences.
+
+    Some methods of mutable sequences are not supported and will raise
+    not-implemented error.
 
-class SortedList(MutableSequence):
-    """
-    SortedList provides most of the same methods as a list but keeps the items
-    in sorted order.
     """
-    # pylint: disable=too-many-ancestors
-    def __init__(self, iterable=None):
-        """
-        SortedList provides most of the same methods as a list but keeps the
-        items in sorted order.
+    DEFAULT_LOAD_FACTOR = 1000
+
+
+    def __init__(self, iterable=None, key=None):
+        """Initialize sorted list instance.
+
+        Optional `iterable` argument provides an initial iterable of values to
+        initialize the sorted list.
+
+        Runtime complexity: `O(n*log(n))`
+
+        >>> sl = SortedList()
+        >>> sl
+        SortedList([])
+        >>> sl = SortedList([3, 1, 2, 5, 4])
+        >>> sl
+        SortedList([1, 2, 3, 4, 5])
+
+        :param iterable: initial values (optional)
 
-        An optional *iterable* provides an initial series of items to populate
-        the SortedList.
         """
+        assert key is None
         self._len = 0
+        self._load = self.DEFAULT_LOAD_FACTOR
         self._lists = []
         self._maxes = []
         self._index = []
-        self._load = LOAD
-        self._half = LOAD >> 1
-        self._dual = LOAD << 1
         self._offset = 0
 
         if iterable is not None:
             self._update(iterable)
 
+
     def __new__(cls, iterable=None, key=None):
-        """
-        SortedList provides most of the same methods as a list but keeps the
-        items in sorted order.
+        """Create new sorted list or sorted-key list instance.
+
+        Optional `key`-function argument will return an instance of subtype
+        :class:`SortedKeyList`.
 
-        An optional *iterable* provides an initial series of items to populate
-        the SortedList.
+        >>> sl = SortedList()
+        >>> isinstance(sl, SortedList)
+        True
+        >>> sl = SortedList(key=lambda x: -x)
+        >>> isinstance(sl, SortedList)
+        True
+        >>> isinstance(sl, SortedKeyList)
+        True
+
+        :param iterable: initial values (optional)
+        :param key: function used to extract comparison key (optional)
+        :return: sorted list or sorted-key list instance
 
-        An optional *key* argument will return an instance of subtype
-        SortedListWithKey.
         """
         # pylint: disable=unused-argument
         if key is None:
             return object.__new__(cls)
         else:
             if cls is SortedList:
-                return object.__new__(SortedListWithKey)
+                return object.__new__(SortedKeyList)
             else:
-                raise TypeError('inherit SortedListWithKey for key argument')
+                raise TypeError('inherit SortedKeyList for key argument')
+
 
     @property
-    def key(self):
-        """Key function used to extract comparison key for sorting."""
+    def key(self):  # pylint: disable=useless-return
+        """Function used to extract comparison key from values.
+
+        Sorted list compares values directly so the key function is none.
+
+        """
         return None
 
+
     def _reset(self, load):
-        """
-        Reset sorted list load.
+        """Reset sorted list load factor.
+
+        The `load` specifies the load-factor of the list. The default load
+        factor of 1000 works well for lists from tens to tens-of-millions of
+        values. Good practice is to use a value that is the cube root of the
+        list size. With billions of elements, the best load factor depends on
+        your usage. It's best to leave the load factor at the default until you
+        start benchmarking.
+
+        See :doc:`implementation` and :doc:`performance-scale` for more
+        information.
+
+        Runtime complexity: `O(n)`
+
+        :param int load: load-factor for sorted list sublists
 
-        The *load* specifies the load-factor of the list. The default load
-        factor of '1000' works well for lists from tens to tens of millions of
-        elements.  Good practice is to use a value that is the cube root of the
-        list size.  With billions of elements, the best load factor depends on
-        your usage.  It's best to leave the load factor at the default until
-        you start benchmarking.
         """
         values = reduce(iadd, self._lists, [])
         self._clear()
         self._load = load
-        self._half = load >> 1
-        self._dual = load << 1
         self._update(values)
 
+
     def clear(self):
-        """Remove all the elements from the list."""
+        """Remove all values from sorted list.
+
+        Runtime complexity: `O(n)`
+
+        """
         self._len = 0
         del self._lists[:]
         del self._maxes[:]
         del self._index[:]
+        self._offset = 0
 
     _clear = clear
 
-    def add(self, val):
-        """Add the element *val* to the list."""
+
+    def add(self, value):
+        """Add `value` to sorted list.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList()
+        >>> sl.add(3)
+        >>> sl.add(1)
+        >>> sl.add(2)
+        >>> sl
+        SortedList([1, 2, 3])
+
+        :param value: value to add to sorted list
+
+        """
         _lists = self._lists
         _maxes = self._maxes
 
         if _maxes:
-            pos = bisect_right(_maxes, val)
+            pos = bisect_right(_maxes, value)
 
             if pos == len(_maxes):
                 pos -= 1
-                _lists[pos].append(val)
-                _maxes[pos] = val
+                _lists[pos].append(value)
+                _maxes[pos] = value
             else:
-                insort(_lists[pos], val)
+                insort(_lists[pos], value)
 
             self._expand(pos)
         else:
-            _lists.append([val])
-            _maxes.append(val)
+            _lists.append([value])
+            _maxes.append(value)
 
         self._len += 1
 
+
     def _expand(self, pos):
-        """Splits sublists that are more than double the load level.
+        """Split sublists with length greater than double the load-factor.
 
         Updates the index when the sublist length is less than double the load
         level. This requires incrementing the nodes in a traversal from the
-        leaf node to the root. For an example traversal see self._loc.
+        leaf node to the root. For an example traversal see
+        ``SortedList._loc``.
 
         """
+        _load = self._load
         _lists = self._lists
         _index = self._index
 
-        if len(_lists[pos]) > self._dual:
+        if len(_lists[pos]) > (_load << 1):
             _maxes = self._maxes
-            _load = self._load
 
             _lists_pos = _lists[pos]
             half = _lists_pos[_load:]
             del _lists_pos[_load:]
             _maxes[pos] = _lists_pos[-1]
 
             _lists.insert(pos + 1, half)
@@ -179,23 +314,36 @@
             if _index:
                 child = self._offset + pos
                 while child:
                     _index[child] += 1
                     child = (child - 1) >> 1
                 _index[0] += 1
 
+
     def update(self, iterable):
-        """Update the list by adding all elements from *iterable*."""
+        """Update sorted list by adding all values from `iterable`.
+
+        Runtime complexity: `O(k*log(n))` -- approximate.
+
+        >>> sl = SortedList()
+        >>> sl.update([3, 1, 2])
+        >>> sl
+        SortedList([1, 2, 3])
+
+        :param iterable: iterable of values to add
+
+        """
         _lists = self._lists
         _maxes = self._maxes
         values = sorted(iterable)
 
         if _maxes:
             if len(values) * 4 >= self._len:
-                values.extend(chain.from_iterable(_lists))
+                _lists.append(values)
+                values = reduce(iadd, _lists, [])
                 values.sort()
                 self._clear()
             else:
                 _add = self.add
                 for val in values:
                     _add(val)
                 return
@@ -205,177 +353,222 @@
                       for pos in range(0, len(values), _load))
         _maxes.extend(sublist[-1] for sublist in _lists)
         self._len = len(values)
         del self._index[:]
 
     _update = update
 
-    def __contains__(self, val):
-        """Return True if and only if *val* is an element in the list."""
+
+    def __contains__(self, value):
+        """Return true if `value` is an element of the sorted list.
+
+        ``sl.__contains__(value)`` <==> ``value in sl``
+
+        Runtime complexity: `O(log(n))`
+
+        >>> sl = SortedList([1, 2, 3, 4, 5])
+        >>> 3 in sl
+        True
+
+        :param value: search for value in sorted list
+        :return: true if `value` in sorted list
+
+        """
         _maxes = self._maxes
 
         if not _maxes:
             return False
 
-        pos = bisect_left(_maxes, val)
+        pos = bisect_left(_maxes, value)
 
         if pos == len(_maxes):
             return False
 
         _lists = self._lists
-        idx = bisect_left(_lists[pos], val)
+        idx = bisect_left(_lists[pos], value)
 
-        return _lists[pos][idx] == val
+        return _lists[pos][idx] == value
 
-    def discard(self, val):
-        """
-        Remove the first occurrence of *val*.
 
-        If *val* is not a member, does nothing.
+    def discard(self, value):
+        """Remove `value` from sorted list if it is a member.
+
+        If `value` is not a member, do nothing.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList([1, 2, 3, 4, 5])
+        >>> sl.discard(5)
+        >>> sl.discard(0)
+        >>> sl == [1, 2, 3, 4]
+        True
+
+        :param value: `value` to discard from sorted list
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return
 
-        pos = bisect_left(_maxes, val)
+        pos = bisect_left(_maxes, value)
 
         if pos == len(_maxes):
             return
 
         _lists = self._lists
-        idx = bisect_left(_lists[pos], val)
+        idx = bisect_left(_lists[pos], value)
 
-        if _lists[pos][idx] == val:
+        if _lists[pos][idx] == value:
             self._delete(pos, idx)
 
-    def remove(self, val):
-        """
-        Remove first occurrence of *val*.
 
-        Raises ValueError if *val* is not present.
+    def remove(self, value):
+        """Remove `value` from sorted list; `value` must be a member.
+
+        If `value` is not a member, raise ValueError.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList([1, 2, 3, 4, 5])
+        >>> sl.remove(5)
+        >>> sl == [1, 2, 3, 4]
+        True
+        >>> sl.remove(0)
+        Traceback (most recent call last):
+          ...
+        ValueError: 0 not in list
+
+        :param value: `value` to remove from sorted list
+        :raises ValueError: if `value` is not in sorted list
+
         """
-        # pylint: disable=arguments-differ
         _maxes = self._maxes
 
         if not _maxes:
-            raise ValueError('{0!r} not in list'.format(val))
+            raise ValueError('{0!r} not in list'.format(value))
 
-        pos = bisect_left(_maxes, val)
+        pos = bisect_left(_maxes, value)
 
         if pos == len(_maxes):
-            raise ValueError('{0!r} not in list'.format(val))
+            raise ValueError('{0!r} not in list'.format(value))
 
         _lists = self._lists
-        idx = bisect_left(_lists[pos], val)
+        idx = bisect_left(_lists[pos], value)
 
-        if _lists[pos][idx] == val:
+        if _lists[pos][idx] == value:
             self._delete(pos, idx)
         else:
-            raise ValueError('{0!r} not in list'.format(val))
+            raise ValueError('{0!r} not in list'.format(value))
+
 
     def _delete(self, pos, idx):
-        """Delete the item at the given (pos, idx).
+        """Delete value at the given `(pos, idx)`.
 
         Combines lists that are less than half the load level.
 
         Updates the index when the sublist length is more than half the load
-        level. This requires decrementing the nodes in a traversal from the leaf
-        node to the root. For an example traversal see self._loc.
+        level. This requires decrementing the nodes in a traversal from the
+        leaf node to the root. For an example traversal see
+        ``SortedList._loc``.
+
+        :param int pos: lists index
+        :param int idx: sublist index
+
         """
         _lists = self._lists
         _maxes = self._maxes
         _index = self._index
 
         _lists_pos = _lists[pos]
 
         del _lists_pos[idx]
         self._len -= 1
 
         len_lists_pos = len(_lists_pos)
 
-        if len_lists_pos > self._half:
-
+        if len_lists_pos > (self._load >> 1):
             _maxes[pos] = _lists_pos[-1]
 
             if _index:
                 child = self._offset + pos
                 while child > 0:
                     _index[child] -= 1
                     child = (child - 1) >> 1
                 _index[0] -= 1
-
         elif len(_lists) > 1:
-
             if not pos:
                 pos += 1
 
             prev = pos - 1
             _lists[prev].extend(_lists[pos])
             _maxes[prev] = _lists[prev][-1]
 
             del _lists[pos]
             del _maxes[pos]
             del _index[:]
 
             self._expand(prev)
-
         elif len_lists_pos:
-
             _maxes[pos] = _lists_pos[-1]
-
         else:
-
             del _lists[pos]
             del _maxes[pos]
             del _index[:]
 
+
     def _loc(self, pos, idx):
-        """Convert an index pair (alpha, beta) into a single index that corresponds to
-        the position of the value in the sorted list.
+        """Convert an index pair (lists index, sublist index) into a single
+        index number that corresponds to the position of the value in the
+        sorted list.
 
-        Most queries require the index be built. Details of the index are
-        described in self._build_index.
+        Many queries require the index be built. Details of the index are
+        described in ``SortedList._build_index``.
 
         Indexing requires traversing the tree from a leaf node to the root. The
-        parent of each node is easily computable at (pos - 1) // 2.
+        parent of each node is easily computable at ``(pos - 1) // 2``.
 
         Left-child nodes are always at odd indices and right-child nodes are
         always at even indices.
 
         When traversing up from a right-child node, increment the total by the
         left-child node.
 
         The final index is the sum from traversal and the index in the sublist.
 
-        For example, using the index from self._build_index:
+        For example, using the index from ``SortedList._build_index``::
 
-        _index = 14 5 9 3 2 4 5
-        _offset = 3
+            _index = 14 5 9 3 2 4 5
+            _offset = 3
 
-        Tree:
+        Tree::
 
                  14
               5      9
             3   2  4   5
 
-        Converting index pair (2, 3) into a single index involves iterating like
-        so:
+        Converting an index pair (2, 3) into a single index involves iterating
+        like so:
 
         1. Starting at the leaf node: offset + alpha = 3 + 2 = 5. We identify
            the node as a left-child node. At such nodes, we simply traverse to
            the parent.
 
         2. At node 9, position 2, we recognize the node as a right-child node
            and accumulate the left-child in our total. Total is now 5 and we
            traverse to the parent at position 0.
 
         3. Iteration ends at the root.
 
-        Computing the index is the sum of the total and beta: 5 + 3 = 8.
+        The index is then the sum of the total and sublist index: 5 + 3 = 8.
+
+        :param int pos: lists index
+        :param int idx: sublist index
+        :return: index in sorted list
+
         """
         if not pos:
             return idx
 
         _index = self._index
 
         if not _index:
@@ -399,39 +592,41 @@
 
             # Advance pos to the parent node.
 
             pos = (pos - 1) >> 1
 
         return total + idx
 
+
     def _pos(self, idx):
-        """Convert an index into a pair (alpha, beta) that can be used to access
-        the corresponding _lists[alpha][beta] position.
+        """Convert an index into an index pair (lists index, sublist index)
+        that can be used to access the corresponding lists position.
 
-        Most queries require the index be built. Details of the index are
-        described in self._build_index.
+        Many queries require the index be built. Details of the index are
+        described in ``SortedList._build_index``.
 
-        Indexing requires traversing the tree to a leaf node. Each node has
-        two children which are easily computable. Given an index, pos, the
-        left-child is at pos * 2 + 1 and the right-child is at pos * 2 + 2.
+        Indexing requires traversing the tree to a leaf node. Each node has two
+        children which are easily computable. Given an index, pos, the
+        left-child is at ``pos * 2 + 1`` and the right-child is at ``pos * 2 +
+        2``.
 
         When the index is less than the left-child, traversal moves to the
         left sub-tree. Otherwise, the index is decremented by the left-child
         and traversal moves to the right sub-tree.
 
         At a child node, the indexing pair is computed from the relative
         position of the child node as compared with the offset and the remaining
         index.
 
-        For example, using the index from self._build_index:
+        For example, using the index from ``SortedList._build_index``::
 
-        _index = 14 5 9 3 2 4 5
-        _offset = 3
+            _index = 14 5 9 3 2 4 5
+            _offset = 3
 
-        Tree:
+        Tree::
 
                  14
               5      9
             3   2  4   5
 
         Indexing position 8 involves iterating like so:
 
@@ -448,14 +643,18 @@
 
         4. To compute the sublist index, we subtract the offset from the index
            of the leaf node: 5 - 3 = 2. To compute the index in the sublist, we
            simply use the index remaining from iteration. In this case, 3.
 
         The final index pair from our example is (2, 3) which corresponds to
         index 8 in the sorted list.
+
+        :param int idx: index in sorted list
+        :return: (lists index, sublist index) pair
+
         """
         if idx < 0:
             last_len = len(self._lists[-1])
 
             if (-idx) <= last_len:
                 return len(self._lists) - 1, last_len + idx
 
@@ -487,47 +686,50 @@
                 idx -= index_child
                 pos = child + 1
 
             child = (pos << 1) + 1
 
         return (pos - self._offset, idx)
 
+
     def _build_index(self):
-        """Build an index for indexing the sorted list.
+        """Build a positional index for indexing the sorted list.
 
         Indexes are represented as binary trees in a dense array notation
         similar to a binary heap.
 
-        For example, given a _lists representation storing integers:
+        For example, given a lists representation storing integers::
 
-        [0]: 1 2 3
-        [1]: 4 5
-        [2]: 6 7 8 9
-        [3]: 10 11 12 13 14
+            0: [1, 2, 3]
+            1: [4, 5]
+            2: [6, 7, 8, 9]
+            3: [10, 11, 12, 13, 14]
 
         The first transformation maps the sub-lists by their length. The
-        first row of the index is the length of the sub-lists.
+        first row of the index is the length of the sub-lists::
 
-        [0]: 3 2 4 5
+            0: [3, 2, 4, 5]
 
-        Each row after that is the sum of consecutive pairs of the previous row:
+        Each row after that is the sum of consecutive pairs of the previous
+        row::
 
-        [1]: 5 9
-        [2]: 14
+            1: [5, 9]
+            2: [14]
 
-        Finally, the index is built by concatenating these lists together:
+        Finally, the index is built by concatenating these lists together::
 
-        _index = 14 5 9 3 2 4 5
+            _index = [14, 5, 9, 3, 2, 4, 5]
 
-        An offset storing the start of the first row is also stored:
+        An offset storing the start of the first row is also stored::
 
-        _offset = 3
+            _offset = 3
 
         When built, the index can be used for efficient indexing into the list.
-        See the comment and notes on self._pos for details.
+        See the comment and notes on ``SortedList._pos`` for details.
+
         """
         row0 = list(map(len, self._lists))
 
         if len(row0) == 1:
             self._index[:] = row0
             self._offset = 0
             return
@@ -540,31 +742,51 @@
             row1.append(row0[-1])
 
         if len(row1) == 1:
             self._index[:] = row1 + row0
             self._offset = 1
             return
 
-        size = 2 ** (int(log_e(len(row1) - 1, 2)) + 1)
+        size = 2 ** (int(log(len(row1) - 1, 2)) + 1)
         row1.extend(repeat(0, size - len(row1)))
         tree = [row0, row1]
 
         while len(tree[-1]) > 1:
             head = iter(tree[-1])
             tail = iter(head)
             row = list(starmap(add, zip(head, tail)))
             tree.append(row)
 
         reduce(iadd, reversed(tree), self._index)
         self._offset = size * 2 - 1
 
-    def __delitem__(self, idx):
-        """Remove the element at *idx*. Supports slicing."""
-        if isinstance(idx, slice):
-            start, stop, step = idx.indices(self._len)
+
+    def __delitem__(self, index):
+        """Remove value at `index` from sorted list.
+
+        ``sl.__delitem__(index)`` <==> ``del sl[index]``
+
+        Supports slicing.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList('abcde')
+        >>> del sl[2]
+        >>> sl
+        SortedList(['a', 'b', 'd', 'e'])
+        >>> del sl[:2]
+        >>> sl
+        SortedList(['d', 'e'])
+
+        :param index: integer or slice for indexing
+        :raises IndexError: if index out of range
+
+        """
+        if isinstance(index, slice):
+            start, stop, step = index.indices(self._len)
 
             if step == 1 and start < stop:
                 if start == 0 and stop == self._len:
                     return self._clear()
                 elif self._len <= 8 * (stop - start):
                     values = self._getitem(slice(None, start))
                     if stop < self._len:
@@ -582,41 +804,68 @@
 
             _pos, _delete = self._pos, self._delete
 
             for index in indices:
                 pos, idx = _pos(index)
                 _delete(pos, idx)
         else:
-            pos, idx = self._pos(idx)
+            pos, idx = self._pos(index)
             self._delete(pos, idx)
 
-    _delitem = __delitem__
 
-    def __getitem__(self, idx):
-        """Return the element at *idx*. Supports slicing."""
+    def __getitem__(self, index):
+        """Lookup value at `index` in sorted list.
+
+        ``sl.__getitem__(index)`` <==> ``sl[index]``
+
+        Supports slicing.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList('abcde')
+        >>> sl[1]
+        'b'
+        >>> sl[-1]
+        'e'
+        >>> sl[2:5]
+        ['c', 'd', 'e']
+
+        :param index: integer or slice for indexing
+        :return: value or list of values
+        :raises IndexError: if index out of range
+
+        """
         _lists = self._lists
 
-        if isinstance(idx, slice):
-            start, stop, step = idx.indices(self._len)
+        if isinstance(index, slice):
+            start, stop, step = index.indices(self._len)
 
             if step == 1 and start < stop:
+                # Whole slice optimization: start to stop slices the whole
+                # sorted list.
+
                 if start == 0 and stop == self._len:
                     return reduce(iadd, self._lists, [])
 
                 start_pos, start_idx = self._pos(start)
+                start_list = _lists[start_pos]
+                stop_idx = start_idx + stop - start
+
+                # Small slice optimization: start index and stop index are
+                # within the start list.
+
+                if len(start_list) >= stop_idx:
+                    return start_list[start_idx:stop_idx]
 
                 if stop == self._len:
                     stop_pos = len(_lists) - 1
                     stop_idx = len(_lists[stop_pos])
                 else:
                     stop_pos, stop_idx = self._pos(stop)
 
-                if start_pos == stop_pos:
-                    return _lists[start_pos][start_idx:stop_idx]
-
                 prefix = _lists[start_pos][start_idx:]
                 middle = _lists[(start_pos + 1):stop_pos]
                 result = reduce(iadd, middle, prefix)
                 result += _lists[stop_pos][:stop_idx]
 
                 return result
 
@@ -629,229 +878,112 @@
             # reverse the order of the items and this could
             # be the desired behavior.
 
             indices = range(start, stop, step)
             return list(self._getitem(index) for index in indices)
         else:
             if self._len:
-                if idx == 0:
+                if index == 0:
                     return _lists[0][0]
-                elif idx == -1:
+                elif index == -1:
                     return _lists[-1][-1]
             else:
                 raise IndexError('list index out of range')
 
-            if 0 <= idx < len(_lists[0]):
-                return _lists[0][idx]
+            if 0 <= index < len(_lists[0]):
+                return _lists[0][index]
 
             len_last = len(_lists[-1])
 
-            if -len_last < idx < 0:
-                return _lists[-1][len_last + idx]
+            if -len_last < index < 0:
+                return _lists[-1][len_last + index]
 
-            pos, idx = self._pos(idx)
+            pos, idx = self._pos(index)
             return _lists[pos][idx]
 
     _getitem = __getitem__
 
-    def _check_order(self, idx, val):
-        _len = self._len
-        _lists = self._lists
-
-        pos, loc = self._pos(idx)
-
-        if idx < 0:
-            idx += _len
-
-        # Check that the inserted value is not less than the
-        # previous value.
-
-        if idx > 0:
-            idx_prev = loc - 1
-            pos_prev = pos
-
-            if idx_prev < 0:
-                pos_prev -= 1
-                idx_prev = len(_lists[pos_prev]) - 1
-
-            if _lists[pos_prev][idx_prev] > val:
-                msg = '{0!r} not in sort order at index {1}'.format(val, idx)
-                raise ValueError(msg)
-
-        # Check that the inserted value is not greater than
-        # the previous value.
-
-        if idx < (_len - 1):
-            idx_next = loc + 1
-            pos_next = pos
-
-            if idx_next == len(_lists[pos_next]):
-                pos_next += 1
-                idx_next = 0
-
-            if _lists[pos_next][idx_next] < val:
-                msg = '{0!r} not in sort order at index {1}'.format(val, idx)
-                raise ValueError(msg)
 
     def __setitem__(self, index, value):
-        """Replace item at position *index* with *value*.
-
-        Supports slice notation. Raises :exc:`ValueError` if the sort order
-        would be violated. When used with a slice and iterable, the
-        :exc:`ValueError` is raised before the list is mutated if the sort
-        order would be violated by the operation.
-
-        """
-        _lists = self._lists
-        _maxes = self._maxes
-        _check_order = self._check_order
-        _pos = self._pos
-
-        if isinstance(index, slice):
-            _len = self._len
-            start, stop, step = index.indices(_len)
-            indices = range(start, stop, step)
-
-            # Copy value to avoid aliasing issues with self and cases where an
-            # iterator is given.
-
-            values = tuple(value)
-
-            if step != 1:
-                if len(values) != len(indices):
-                    raise ValueError(
-                        'attempt to assign sequence of size %s'
-                        ' to extended slice of size %s'
-                        % (len(values), len(indices)))
-
-                # Keep a log of values that are set so that we can
-                # roll back changes if ordering is violated.
-
-                log = []
-                _append = log.append
-
-                for idx, val in zip(indices, values):
-                    pos, loc = _pos(idx)
-                    _append((idx, _lists[pos][loc], val))
-                    _lists[pos][loc] = val
-                    if len(_lists[pos]) == (loc + 1):
-                        _maxes[pos] = val
-
-                try:
-                    # Validate ordering of new values.
-
-                    for idx, _, newval in log:
-                        _check_order(idx, newval)
-
-                except ValueError:
-
-                    # Roll back changes from log.
-
-                    for idx, oldval, _ in log:
-                        pos, loc = _pos(idx)
-                        _lists[pos][loc] = oldval
-                        if len(_lists[pos]) == (loc + 1):
-                            _maxes[pos] = oldval
-
-                    raise
-            else:
-                if start == 0 and stop == _len:
-                    self._clear()
-                    return self._update(values)
-
-                if stop < start:
-                    # When calculating indices, stop may be less than start.
-                    # For example: ...[5:3:1] results in slice(5, 3, 1) which
-                    # is a valid but not useful stop index.
-                    stop = start
-
-                if values:
-
-                    # Check that given values are ordered properly.
+        """Raise not-implemented error.
 
-                    alphas = iter(values)
-                    betas = iter(values)
-                    next(betas)
-                    pairs = zip(alphas, betas)
+        ``sl.__setitem__(index, value)`` <==> ``sl[index] = value``
 
-                    if not all(alpha <= beta for alpha, beta in pairs):
-                        raise ValueError('given values not in sort order')
+        :raises NotImplementedError: use ``del sl[index]`` and
+            ``sl.add(value)`` instead
 
-                    # Check ordering in context of sorted list.
-
-                    if start and self._getitem(start - 1) > values[0]:
-                        message = '{0!r} not in sort order at index {1}'.format(
-                            values[0], start)
-                        raise ValueError(message)
-
-                    if stop != _len and self._getitem(stop) < values[-1]:
-                        message = '{0!r} not in sort order at index {1}'.format(
-                            values[-1], stop)
-                        raise ValueError(message)
-
-                # Delete the existing values.
+        """
+        message = 'use ``del sl[index]`` and ``sl.add(value)`` instead'
+        raise NotImplementedError(message)
 
-                self._delitem(index)
 
-                # Insert the new values.
+    def __iter__(self):
+        """Return an iterator over the sorted list.
 
-                _insert = self.insert
-                for idx, val in enumerate(values):
-                    _insert(start + idx, val)
-        else:
-            pos, loc = _pos(index)
-            _check_order(index, value)
-            _lists[pos][loc] = value
-            if len(_lists[pos]) == (loc + 1):
-                _maxes[pos] = value
+        ``sl.__iter__()`` <==> ``iter(sl)``
 
-    def __iter__(self):
-        """
-        Return an iterator over the Sequence.
+        Iterating the sorted list while adding or deleting values may raise a
+        :exc:`RuntimeError` or fail to iterate over all values.
 
-        Iterating the Sequence while adding or deleting values may raise a
-        `RuntimeError` or fail to iterate over all entries.
         """
         return chain.from_iterable(self._lists)
 
+
     def __reversed__(self):
-        """
-        Return an iterator to traverse the Sequence in reverse.
+        """Return a reverse iterator over the sorted list.
+
+        ``sl.__reversed__()`` <==> ``reversed(sl)``
+
+        Iterating the sorted list while adding or deleting values may raise a
+        :exc:`RuntimeError` or fail to iterate over all values.
 
-        Iterating the Sequence while adding or deleting values may raise a
-        `RuntimeError` or fail to iterate over all entries.
         """
         return chain.from_iterable(map(reversed, reversed(self._lists)))
 
+
     def reverse(self):
-        """Raise NotImplementedError
+        """Raise not-implemented error.
 
-        SortedList maintains values in ascending sort order. Values may not be
+        Sorted list maintains values in ascending sort order. Values may not be
         reversed in-place.
 
-        Use ``reversed(sorted_list)`` for a reverse iterator over values in
-        descending sort order.
+        Use ``reversed(sl)`` for an iterator over values in descending sort
+        order.
 
-        Implemented to override MutableSequence.reverse which provides an
+        Implemented to override `MutableSequence.reverse` which provides an
         erroneous default implementation.
 
+        :raises NotImplementedError: use ``reversed(sl)`` instead
+
         """
-        raise NotImplementedError('.reverse() not defined')
+        raise NotImplementedError('use ``reversed(sl)`` instead')
 
-    def islice(self, start=None, stop=None, reverse=False):
 
-        """
-        Returns an iterator that slices `self` from `start` to `stop` index,
-        inclusive and exclusive respectively.
+    def islice(self, start=None, stop=None, reverse=False):
+        """Return an iterator that slices sorted list from `start` to `stop`.
 
-        When `reverse` is `True`, values are yielded from the iterator in
-        reverse order.
+        The `start` and `stop` index are treated inclusive and exclusive,
+        respectively.
 
         Both `start` and `stop` default to `None` which is automatically
-        inclusive of the beginning and end.
+        inclusive of the beginning and end of the sorted list.
+
+        When `reverse` is `True` the values are yielded from the iterator in
+        reverse order; `reverse` defaults to `False`.
+
+        >>> sl = SortedList('abcdefghij')
+        >>> it = sl.islice(2, 6)
+        >>> list(it)
+        ['c', 'd', 'e', 'f']
+
+        :param int start: start index (inclusive)
+        :param int stop: stop index (exclusive)
+        :param bool reverse: yield values in reverse order
+        :return: iterator
+
         """
         _len = self._len
 
         if not _len:
             return iter(())
 
         start, stop, _ = slice(start, stop).indices(self._len)
@@ -867,68 +999,105 @@
             max_pos = len(self._lists) - 1
             max_idx = len(self._lists[-1])
         else:
             max_pos, max_idx = _pos(stop)
 
         return self._islice(min_pos, min_idx, max_pos, max_idx, reverse)
 
+
     def _islice(self, min_pos, min_idx, max_pos, max_idx, reverse):
-        """
-        Returns an iterator that slices `self` using two index pairs,
-        `(min_pos, min_idx)` and `(max_pos, max_idx)`; the first inclusive
-        and the latter exclusive. See `_pos` for details on how an index
-        is converted to an index pair.
+        """Return an iterator that slices sorted list using two index pairs.
+
+        The index pairs are (min_pos, min_idx) and (max_pos, max_idx), the
+        first inclusive and the latter exclusive. See `_pos` for details on how
+        an index is converted to an index pair.
 
         When `reverse` is `True`, values are yielded from the iterator in
         reverse order.
+
         """
         _lists = self._lists
 
         if min_pos > max_pos:
             return iter(())
-        elif min_pos == max_pos and not reverse:
-            return iter(_lists[min_pos][min_idx:max_idx])
-        elif min_pos == max_pos and reverse:
-            return reversed(_lists[min_pos][min_idx:max_idx])
-        elif min_pos + 1 == max_pos and not reverse:
-            return chain(_lists[min_pos][min_idx:], _lists[max_pos][:max_idx])
-        elif min_pos + 1 == max_pos and reverse:
+
+        if min_pos == max_pos:
+            if reverse:
+                indices = reversed(range(min_idx, max_idx))
+                return map(_lists[min_pos].__getitem__, indices)
+
+            indices = range(min_idx, max_idx)
+            return map(_lists[min_pos].__getitem__, indices)
+
+        next_pos = min_pos + 1
+
+        if next_pos == max_pos:
+            if reverse:
+                min_indices = range(min_idx, len(_lists[min_pos]))
+                max_indices = range(max_idx)
+                return chain(
+                    map(_lists[max_pos].__getitem__, reversed(max_indices)),
+                    map(_lists[min_pos].__getitem__, reversed(min_indices)),
+                )
+
+            min_indices = range(min_idx, len(_lists[min_pos]))
+            max_indices = range(max_idx)
             return chain(
-                reversed(_lists[max_pos][:max_idx]),
-                reversed(_lists[min_pos][min_idx:]),
+                map(_lists[min_pos].__getitem__, min_indices),
+                map(_lists[max_pos].__getitem__, max_indices),
             )
-        elif not reverse:
+
+        if reverse:
+            min_indices = range(min_idx, len(_lists[min_pos]))
+            sublist_indices = range(next_pos, max_pos)
+            sublists = map(_lists.__getitem__, reversed(sublist_indices))
+            max_indices = range(max_idx)
             return chain(
-                _lists[min_pos][min_idx:],
-                chain.from_iterable(_lists[(min_pos + 1):max_pos]),
-                _lists[max_pos][:max_idx],
+                map(_lists[max_pos].__getitem__, reversed(max_indices)),
+                chain.from_iterable(map(reversed, sublists)),
+                map(_lists[min_pos].__getitem__, reversed(min_indices)),
             )
 
-        temp = map(reversed, reversed(_lists[(min_pos + 1):max_pos]))
+        min_indices = range(min_idx, len(_lists[min_pos]))
+        sublist_indices = range(next_pos, max_pos)
+        sublists = map(_lists.__getitem__, sublist_indices)
+        max_indices = range(max_idx)
         return chain(
-            reversed(_lists[max_pos][:max_idx]),
-            chain.from_iterable(temp),
-            reversed(_lists[min_pos][min_idx:]),
+            map(_lists[min_pos].__getitem__, min_indices),
+            chain.from_iterable(sublists),
+            map(_lists[max_pos].__getitem__, max_indices),
         )
 
+
     def irange(self, minimum=None, maximum=None, inclusive=(True, True),
                reverse=False):
-        """
-        Create an iterator of values between `minimum` and `maximum`.
-
-        `inclusive` is a pair of booleans that indicates whether the minimum
-        and maximum ought to be included in the range, respectively. The
-        default is (True, True) such that the range is inclusive of both
-        minimum and maximum.
+        """Create an iterator of values between `minimum` and `maximum`.
 
         Both `minimum` and `maximum` default to `None` which is automatically
-        inclusive of the start and end of the list, respectively.
+        inclusive of the beginning and end of the sorted list.
+
+        The argument `inclusive` is a pair of booleans that indicates whether
+        the minimum and maximum ought to be included in the range,
+        respectively. The default is ``(True, True)`` such that the range is
+        inclusive of both minimum and maximum.
 
         When `reverse` is `True` the values are yielded from the iterator in
         reverse order; `reverse` defaults to `False`.
+
+        >>> sl = SortedList('abcdefghij')
+        >>> it = sl.irange('c', 'f')
+        >>> list(it)
+        ['c', 'd', 'e', 'f']
+
+        :param minimum: minimum value to start iterating
+        :param maximum: maximum value to stop iterating
+        :param inclusive: pair of booleans
+        :param bool reverse: yield values in reverse order
+        :return: iterator
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return iter(())
 
         _lists = self._lists
@@ -977,294 +1146,271 @@
                     max_pos -= 1
                     max_idx = len(_lists[max_pos])
                 else:
                     max_idx = bisect_left(_lists[max_pos], maximum)
 
         return self._islice(min_pos, min_idx, max_pos, max_idx, reverse)
 
+
     def __len__(self):
-        """Return the number of elements in the list."""
-        return self._len
+        """Return the size of the sorted list.
+
+        ``sl.__len__()`` <==> ``len(sl)``
+
+        :return: size of sorted list
 
-    def bisect_left(self, val):
         """
-        Similar to the *bisect* module in the standard library, this returns an
-        appropriate index to insert *val*. If *val* is already present, the
-        insertion point will be before (to the left of) any existing entries.
+        return self._len
+
+
+    def bisect_left(self, value):
+        """Return an index to insert `value` in the sorted list.
+
+        If the `value` is already present, the insertion point will be before
+        (to the left of) any existing values.
+
+        Similar to the `bisect` module in the standard library.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList([10, 11, 12, 13, 14])
+        >>> sl.bisect_left(12)
+        2
+
+        :param value: insertion index of value in sorted list
+        :return: index
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return 0
 
-        pos = bisect_left(_maxes, val)
+        pos = bisect_left(_maxes, value)
 
         if pos == len(_maxes):
             return self._len
 
-        idx = bisect_left(self._lists[pos], val)
-
+        idx = bisect_left(self._lists[pos], value)
         return self._loc(pos, idx)
 
-    def bisect_right(self, val):
-        """
-        Same as *bisect_left*, but if *val* is already present, the insertion
-        point will be after (to the right of) any existing entries.
+
+    def bisect_right(self, value):
+        """Return an index to insert `value` in the sorted list.
+
+        Similar to `bisect_left`, but if `value` is already present, the
+        insertion point will be after (to the right of) any existing values.
+
+        Similar to the `bisect` module in the standard library.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList([10, 11, 12, 13, 14])
+        >>> sl.bisect_right(12)
+        3
+
+        :param value: insertion index of value in sorted list
+        :return: index
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return 0
 
-        pos = bisect_right(_maxes, val)
+        pos = bisect_right(_maxes, value)
 
         if pos == len(_maxes):
             return self._len
 
-        idx = bisect_right(self._lists[pos], val)
-
+        idx = bisect_right(self._lists[pos], value)
         return self._loc(pos, idx)
 
     bisect = bisect_right
     _bisect_right = bisect_right
 
-    def count(self, val):
-        """Return the number of occurrences of *val* in the list."""
-        # pylint: disable=arguments-differ
+
+    def count(self, value):
+        """Return number of occurrences of `value` in the sorted list.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList([1, 2, 2, 3, 3, 3, 4, 4, 4, 4])
+        >>> sl.count(3)
+        3
+
+        :param value: value to count in sorted list
+        :return: count
+
+        """
         _maxes = self._maxes
 
         if not _maxes:
             return 0
 
-        pos_left = bisect_left(_maxes, val)
+        pos_left = bisect_left(_maxes, value)
 
         if pos_left == len(_maxes):
             return 0
 
         _lists = self._lists
-        idx_left = bisect_left(_lists[pos_left], val)
-        pos_right = bisect_right(_maxes, val)
+        idx_left = bisect_left(_lists[pos_left], value)
+        pos_right = bisect_right(_maxes, value)
 
         if pos_right == len(_maxes):
             return self._len - self._loc(pos_left, idx_left)
 
-        idx_right = bisect_right(_lists[pos_right], val)
+        idx_right = bisect_right(_lists[pos_right], value)
 
         if pos_left == pos_right:
             return idx_right - idx_left
 
         right = self._loc(pos_right, idx_right)
         left = self._loc(pos_left, idx_left)
-
         return right - left
 
+
     def copy(self):
-        """Return a shallow copy of the sorted list."""
-        return self.__class__(self)
+        """Return a shallow copy of the sorted list.
 
-    __copy__ = copy
+        Runtime complexity: `O(n)`
+
+        :return: new sorted list
 
-    def append(self, val):
-        """
-        Append the element *val* to the list. Raises a ValueError if the *val*
-        would violate the sort order.
         """
-        # pylint: disable=arguments-differ
-        _lists = self._lists
-        _maxes = self._maxes
+        return self.__class__(self)
 
-        if not _maxes:
-            _maxes.append(val)
-            _lists.append([val])
-            self._len = 1
-            return
+    __copy__ = copy
 
-        pos = len(_lists) - 1
 
-        if val < _lists[pos][-1]:
-            msg = '{0!r} not in sort order at index {1}'.format(val, self._len)
-            raise ValueError(msg)
+    def append(self, value):
+        """Raise not-implemented error.
 
-        _maxes[pos] = val
-        _lists[pos].append(val)
-        self._len += 1
-        self._expand(pos)
+        Implemented to override `MutableSequence.append` which provides an
+        erroneous default implementation.
+
+        :raises NotImplementedError: use ``sl.add(value)`` instead
 
-    def extend(self, values):
-        """
-        Extend the list by appending all elements from the *values*. Raises a
-        ValueError if the sort order would be violated.
         """
-        _lists = self._lists
-        _maxes = self._maxes
-        _load = self._load
+        raise NotImplementedError('use ``sl.add(value)`` instead')
 
-        if not isinstance(values, list):
-            values = list(values)
 
-        if not values:
-            return
+    def extend(self, values):
+        """Raise not-implemented error.
 
-        if any(values[pos - 1] > values[pos]
-               for pos in range(1, len(values))):
-            raise ValueError('given sequence not in sort order')
+        Implemented to override `MutableSequence.extend` which provides an
+        erroneous default implementation.
 
-        offset = 0
+        :raises NotImplementedError: use ``sl.update(values)`` instead
 
-        if _maxes:
-            if values[0] < _lists[-1][-1]:
-                msg = '{0!r} not in sort order at index {1}'.format(values[0], self._len)
-                raise ValueError(msg)
-
-            if len(_lists[-1]) < self._half:
-                _lists[-1].extend(values[:_load])
-                _maxes[-1] = _lists[-1][-1]
-                offset = _load
-
-        len_lists = len(_lists)
-
-        for idx in range(offset, len(values), _load):
-            _lists.append(values[idx:(idx + _load)])
-            _maxes.append(_lists[-1][-1])
+        """
+        raise NotImplementedError('use ``sl.update(values)`` instead')
 
-        _index = self._index
 
-        if len_lists == len(_lists):
-            len_index = len(_index)
-            if len_index > 0:
-                len_values = len(values)
-                child = len_index - 1
-                while child:
-                    _index[child] += len_values
-                    child = (child - 1) >> 1
-                _index[0] += len_values
-        else:
-            del _index[:]
+    def insert(self, index, value):
+        """Raise not-implemented error.
 
-        self._len += len(values)
+        :raises NotImplementedError: use ``sl.add(value)`` instead
 
-    def insert(self, idx, val):
-        """
-        Insert the element *val* into the list at *idx*. Raises a ValueError if
-        the *val* at *idx* would violate the sort order.
         """
-        # pylint: disable=arguments-differ
-        _len = self._len
-        _lists = self._lists
-        _maxes = self._maxes
+        raise NotImplementedError('use ``sl.add(value)`` instead')
 
-        if idx < 0:
-            idx += _len
-        if idx < 0:
-            idx = 0
-        if idx > _len:
-            idx = _len
 
-        if not _maxes:
-            # The idx must be zero by the inequalities above.
-            _maxes.append(val)
-            _lists.append([val])
-            self._len = 1
-            return
+    def pop(self, index=-1):
+        """Remove and return value at `index` in sorted list.
 
-        if not idx:
-            if val > _lists[0][0]:
-                msg = '{0!r} not in sort order at index {1}'.format(val, 0)
-                raise ValueError(msg)
-            else:
-                _lists[0].insert(0, val)
-                self._expand(0)
-                self._len += 1
-                return
+        Raise :exc:`IndexError` if the sorted list is empty or index is out of
+        range.
 
-        if idx == _len:
-            pos = len(_lists) - 1
-            if _lists[pos][-1] > val:
-                msg = '{0!r} not in sort order at index {1}'.format(val, _len)
-                raise ValueError(msg)
-            else:
-                _lists[pos].append(val)
-                _maxes[pos] = _lists[pos][-1]
-                self._expand(pos)
-                self._len += 1
-                return
+        Negative indices are supported.
 
-        pos, idx = self._pos(idx)
-        idx_before = idx - 1
-        if idx_before < 0:
-            pos_before = pos - 1
-            idx_before = len(_lists[pos_before]) - 1
-        else:
-            pos_before = pos
+        Runtime complexity: `O(log(n))` -- approximate.
 
-        before = _lists[pos_before][idx_before]
-        if before <= val <= _lists[pos][idx]:
-            _lists[pos].insert(idx, val)
-            self._expand(pos)
-            self._len += 1
-        else:
-            msg = '{0!r} not in sort order at index {1}'.format(val, idx)
-            raise ValueError(msg)
+        >>> sl = SortedList('abcde')
+        >>> sl.pop()
+        'e'
+        >>> sl.pop(2)
+        'c'
+        >>> sl
+        SortedList(['a', 'b', 'd'])
+
+        :param int index: index of value (default -1)
+        :return: value
+        :raises IndexError: if index is out of range
 
-    def pop(self, idx=-1):
-        """
-        Remove and return item at *idx* (default last).  Raises IndexError if
-        list is empty or index is out of range.  Negative indices are supported,
-        as for slice indices.
         """
-        # pylint: disable=arguments-differ
         if not self._len:
             raise IndexError('pop index out of range')
 
         _lists = self._lists
 
-        if idx == 0:
+        if index == 0:
             val = _lists[0][0]
             self._delete(0, 0)
             return val
 
-        if idx == -1:
+        if index == -1:
             pos = len(_lists) - 1
             loc = len(_lists[pos]) - 1
             val = _lists[pos][loc]
             self._delete(pos, loc)
             return val
 
-        if 0 <= idx < len(_lists[0]):
-            val = _lists[0][idx]
-            self._delete(0, idx)
+        if 0 <= index < len(_lists[0]):
+            val = _lists[0][index]
+            self._delete(0, index)
             return val
 
         len_last = len(_lists[-1])
 
-        if -len_last < idx < 0:
+        if -len_last < index < 0:
             pos = len(_lists) - 1
-            loc = len_last + idx
+            loc = len_last + index
             val = _lists[pos][loc]
             self._delete(pos, loc)
             return val
 
-        pos, idx = self._pos(idx)
+        pos, idx = self._pos(index)
         val = _lists[pos][idx]
         self._delete(pos, idx)
-
         return val
 
-    def index(self, val, start=None, stop=None):
-        """
-        Return the smallest *k* such that L[k] == val and i <= k < j`.  Raises
-        ValueError if *val* is not present.  *stop* defaults to the end of the
-        list. *start* defaults to the beginning. Negative indices are supported,
-        as for slice indices.
+
+    def index(self, value, start=None, stop=None):
+        """Return first index of value in sorted list.
+
+        Raise ValueError if `value` is not present.
+
+        Index must be between `start` and `stop` for the `value` to be
+        considered present. The default value, None, for `start` and `stop`
+        indicate the beginning and end of the sorted list.
+
+        Negative indices are supported.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> sl = SortedList('abcde')
+        >>> sl.index('d')
+        3
+        >>> sl.index('z')
+        Traceback (most recent call last):
+          ...
+        ValueError: 'z' is not in list
+
+        :param value: value in sorted list
+        :param int start: start index (default None, start of sorted list)
+        :param int stop: stop index (default None, end of sorted list)
+        :return: index of value
+        :raises ValueError: if value is not present
+
         """
-        # pylint: disable=arguments-differ
         _len = self._len
 
         if not _len:
-            raise ValueError('{0!r} is not in list'.format(val))
+            raise ValueError('{0!r} is not in list'.format(value))
 
         if start is None:
             start = 0
         if start < 0:
             start += _len
         if start < 0:
             start = 0
@@ -1273,307 +1419,423 @@
             stop = _len
         if stop < 0:
             stop += _len
         if stop > _len:
             stop = _len
 
         if stop <= start:
-            raise ValueError('{0!r} is not in list'.format(val))
+            raise ValueError('{0!r} is not in list'.format(value))
 
         _maxes = self._maxes
-        pos_left = bisect_left(_maxes, val)
+        pos_left = bisect_left(_maxes, value)
 
         if pos_left == len(_maxes):
-            raise ValueError('{0!r} is not in list'.format(val))
+            raise ValueError('{0!r} is not in list'.format(value))
 
         _lists = self._lists
-        idx_left = bisect_left(_lists[pos_left], val)
+        idx_left = bisect_left(_lists[pos_left], value)
 
-        if _lists[pos_left][idx_left] != val:
-            raise ValueError('{0!r} is not in list'.format(val))
+        if _lists[pos_left][idx_left] != value:
+            raise ValueError('{0!r} is not in list'.format(value))
 
         stop -= 1
         left = self._loc(pos_left, idx_left)
 
         if start <= left:
             if left <= stop:
                 return left
         else:
-            right = self._bisect_right(val) - 1
+            right = self._bisect_right(value) - 1
 
             if start <= right:
                 return start
 
-        raise ValueError('{0!r} is not in list'.format(val))
+        raise ValueError('{0!r} is not in list'.format(value))
+
+
+    def __add__(self, other):
+        """Return new sorted list containing all values in both sequences.
+
+        ``sl.__add__(other)`` <==> ``sl + other``
+
+        Values in `other` do not need to be in sorted order.
+
+        Runtime complexity: `O(n*log(n))`
+
+        >>> sl1 = SortedList('bat')
+        >>> sl2 = SortedList('cat')
+        >>> sl1 + sl2
+        SortedList(['a', 'a', 'b', 'c', 't', 't'])
+
+        :param other: other iterable
+        :return: new sorted list
 
-    def __add__(self, that):
-        """
-        Return a new sorted list containing all the elements in *self* and
-        *that*. Elements in *that* do not need to be properly ordered with
-        respect to *self*.
         """
         values = reduce(iadd, self._lists, [])
-        values.extend(that)
+        values.extend(other)
         return self.__class__(values)
 
-    def __iadd__(self, that):
-        """
-        Update *self* to include all values in *that*. Elements in *that* do not
-        need to be properly ordered with respect to *self*.
+    __radd__ = __add__
+
+
+    def __iadd__(self, other):
+        """Update sorted list with values from `other`.
+
+        ``sl.__iadd__(other)`` <==> ``sl += other``
+
+        Values in `other` do not need to be in sorted order.
+
+        Runtime complexity: `O(k*log(n))` -- approximate.
+
+        >>> sl = SortedList('bat')
+        >>> sl += 'cat'
+        >>> sl
+        SortedList(['a', 'a', 'b', 'c', 't', 't'])
+
+        :param other: other iterable
+        :return: existing sorted list
+
         """
-        self._update(that)
+        self._update(other)
         return self
 
-    def __mul__(self, that):
-        """
-        Return a new sorted list containing *that* shallow copies of each item
-        in SortedList.
+
+    def __mul__(self, num):
+        """Return new sorted list with `num` shallow copies of values.
+
+        ``sl.__mul__(num)`` <==> ``sl * num``
+
+        Runtime complexity: `O(n*log(n))`
+
+        >>> sl = SortedList('abc')
+        >>> sl * 3
+        SortedList(['a', 'a', 'a', 'b', 'b', 'b', 'c', 'c', 'c'])
+
+        :param int num: count of shallow copies
+        :return: new sorted list
+
         """
-        values = reduce(iadd, self._lists, []) * that
+        values = reduce(iadd, self._lists, []) * num
         return self.__class__(values)
 
-    def __imul__(self, that):
-        """
-        Increase the length of the list by appending *that* shallow copies of
-        each item.
+    __rmul__ = __mul__
+
+
+    def __imul__(self, num):
+        """Update the sorted list with `num` shallow copies of values.
+
+        ``sl.__imul__(num)`` <==> ``sl *= num``
+
+        Runtime complexity: `O(n*log(n))`
+
+        >>> sl = SortedList('abc')
+        >>> sl *= 3
+        >>> sl
+        SortedList(['a', 'a', 'a', 'b', 'b', 'b', 'c', 'c', 'c'])
+
+        :param int num: count of shallow copies
+        :return: existing sorted list
+
         """
-        values = reduce(iadd, self._lists, []) * that
+        values = reduce(iadd, self._lists, []) * num
         self._clear()
         self._update(values)
         return self
 
-    def _make_cmp(self, seq_op, doc):
+
+    def __make_cmp(seq_op, symbol, doc):
         "Make comparator method."
-        def comparer(self, that):
+        def comparer(self, other):
             "Compare method for sorted list and sequence."
-            # pylint: disable=protected-access
-            if not isinstance(that, Sequence):
+            if not isinstance(other, Sequence):
                 return NotImplemented
 
             self_len = self._len
-            len_that = len(that)
+            len_other = len(other)
 
-            if self_len != len_that:
-                if seq_op is op.eq:
+            if self_len != len_other:
+                if seq_op is eq:
                     return False
-                if seq_op is op.ne:
+                if seq_op is ne:
                     return True
 
-            for alpha, beta in zip(self, that):
+            for alpha, beta in zip(self, other):
                 if alpha != beta:
                     return seq_op(alpha, beta)
 
-            return seq_op(self_len, len_that)
+            return seq_op(self_len, len_other)
+
+        seq_op_name = seq_op.__name__
+        comparer.__name__ = '__{0}__'.format(seq_op_name)
+        doc_str = """Return true if and only if sorted list is {0} `other`.
+
+        ``sl.__{1}__(other)`` <==> ``sl {2} other``
 
-        comparer.__name__ = '__{0}__'.format(seq_op.__name__)
-        doc_str = 'Return `True` if and only if Sequence is {0} `that`.'
-        comparer.__doc__ = doc_str.format(doc)
+        Comparisons use lexicographical order as with sequences.
 
+        Runtime complexity: `O(n)`
+
+        :param other: `other` sequence
+        :return: true if sorted list is {0} `other`
+
+        """
+        comparer.__doc__ = dedent(doc_str.format(doc, seq_op_name, symbol))
         return comparer
 
-    __eq__ = _make_cmp(None, op.eq, 'equal to')
-    __ne__ = _make_cmp(None, op.ne, 'not equal to')
-    __lt__ = _make_cmp(None, op.lt, 'less than')
-    __gt__ = _make_cmp(None, op.gt, 'greater than')
-    __le__ = _make_cmp(None, op.le, 'less than or equal to')
-    __ge__ = _make_cmp(None, op.ge, 'greater than or equal to')
 
-    @recursive_repr
-    def __repr__(self):
-        """Return string representation of sequence."""
-        return '{0}({1!r})'.format(type(self).__name__, list(self))
+    __eq__ = __make_cmp(eq, '==', 'equal to')
+    __ne__ = __make_cmp(ne, '!=', 'not equal to')
+    __lt__ = __make_cmp(lt, '<', 'less than')
+    __gt__ = __make_cmp(gt, '>', 'greater than')
+    __le__ = __make_cmp(le, '<=', 'less than or equal to')
+    __ge__ = __make_cmp(ge, '>=', 'greater than or equal to')
+    __make_cmp = staticmethod(__make_cmp)
 
-    def _check(self):
-        try:
-            # Check load parameters.
 
-            assert self._load >= 4
-            assert self._half == (self._load >> 1)
-            assert self._dual == (self._load << 1)
+    def __reduce__(self):
+        values = reduce(iadd, self._lists, [])
+        return (type(self), (values,))
 
-            # Check empty sorted list case.
 
-            if self._maxes == []:
-                assert self._lists == []
-                return
+    @recursive_repr()
+    def __repr__(self):
+        """Return string representation of sorted list.
 
-            assert self._maxes and self._lists
+        ``sl.__repr__()`` <==> ``repr(sl)``
 
-            # Check all sublists are sorted.
+        :return: string representation
 
-            assert all(sublist[pos - 1] <= sublist[pos]
-                       for sublist in self._lists
-                       for pos in range(1, len(sublist)))
+        """
+        return '{0}({1!r})'.format(type(self).__name__, list(self))
 
-            # Check beginning/end of sublists are sorted.
 
-            for pos in range(1, len(self._lists)):
-                assert self._lists[pos - 1][-1] <= self._lists[pos][0]
+    def _check(self):
+        """Check invariants of sorted list.
 
-            # Check length of _maxes and _lists match.
+        Runtime complexity: `O(n)`
 
+        """
+        try:
+            assert self._load >= 4
             assert len(self._maxes) == len(self._lists)
+            assert self._len == sum(len(sublist) for sublist in self._lists)
 
-            # Check _maxes is a map of _lists.
+            # Check all sublists are sorted.
 
-            assert all(self._maxes[pos] == self._lists[pos][-1]
-                       for pos in range(len(self._maxes)))
+            for sublist in self._lists:
+                for pos in range(1, len(sublist)):
+                    assert sublist[pos - 1] <= sublist[pos]
 
-            # Check load level is less than _dual.
+            # Check beginning/end of sublists are sorted.
 
-            assert all(len(sublist) <= self._dual for sublist in self._lists)
+            for pos in range(1, len(self._lists)):
+                assert self._lists[pos - 1][-1] <= self._lists[pos][0]
 
-            # Check load level is greater than _half for all
-            # but the last sublist.
+            # Check _maxes index is the last value of each sublist.
 
-            assert all(len(self._lists[pos]) >= self._half
-                       for pos in range(0, len(self._lists) - 1))
+            for pos in range(len(self._maxes)):
+                assert self._maxes[pos] == self._lists[pos][-1]
 
-            # Check length.
+            # Check sublist lengths are less than double load-factor.
 
-            assert self._len == sum(len(sublist) for sublist in self._lists)
+            double = self._load << 1
+            assert all(len(sublist) <= double for sublist in self._lists)
+
+            # Check sublist lengths are greater than half load-factor for all
+            # but the last sublist.
 
-            # Check index.
+            half = self._load >> 1
+            for pos in range(0, len(self._lists) - 1):
+                assert len(self._lists[pos]) >= half
 
             if self._index:
-                assert len(self._index) == self._offset + len(self._lists)
                 assert self._len == self._index[0]
+                assert len(self._index) == self._offset + len(self._lists)
 
-                def test_offset_pos(pos):
-                    "Test positional indexing offset."
-                    from_index = self._index[self._offset + pos]
-                    return from_index == len(self._lists[pos])
+                # Check index leaf nodes equal length of sublists.
 
-                assert all(test_offset_pos(pos)
-                           for pos in range(len(self._lists)))
+                for pos in range(len(self._lists)):
+                    leaf = self._index[self._offset + pos]
+                    assert leaf == len(self._lists[pos])
+
+                # Check index branch nodes are the sum of their children.
 
                 for pos in range(self._offset):
                     child = (pos << 1) + 1
                     if child >= len(self._index):
                         assert self._index[pos] == 0
                     elif child + 1 == len(self._index):
                         assert self._index[pos] == self._index[child]
                     else:
                         child_sum = self._index[child] + self._index[child + 1]
-                        assert self._index[pos] == child_sum
-
+                        assert child_sum == self._index[pos]
         except:
-            import sys
-            import traceback
-
             traceback.print_exc(file=sys.stdout)
-
             print('len', self._len)
-            print('load', self._load, self._half, self._dual)
+            print('load', self._load)
             print('offset', self._offset)
             print('len_index', len(self._index))
             print('index', self._index)
             print('len_maxes', len(self._maxes))
             print('maxes', self._maxes)
             print('len_lists', len(self._lists))
             print('lists', self._lists)
-
             raise
 
+
 def identity(value):
     "Identity function."
     return value
 
-class SortedListWithKey(SortedList):
-    """
-    SortedListWithKey provides most of the same methods as a list but keeps
-    the items in sorted order.
+
+class SortedKeyList(SortedList):
+    """Sorted-key list is a subtype of sorted list.
+
+    The sorted-key list maintains values in comparison order based on the
+    result of a key function applied to every value.
+
+    All the same methods that are available in :class:`SortedList` are also
+    available in :class:`SortedKeyList`.
+
+    Additional methods provided:
+
+    * :attr:`SortedKeyList.key`
+    * :func:`SortedKeyList.bisect_key_left`
+    * :func:`SortedKeyList.bisect_key_right`
+    * :func:`SortedKeyList.irange_key`
+
+    Some examples below use:
+
+    >>> from operator import neg
+    >>> neg
+    <built-in function neg>
+    >>> neg(1)
+    -1
+
     """
-    # pylint: disable=too-many-ancestors,abstract-method
     def __init__(self, iterable=None, key=identity):
-        """SortedListWithKey provides most of the same methods as list but keeps the
-        items in sorted order.
+        """Initialize sorted-key list instance.
 
-        An optional *iterable* provides an initial series of items to populate
-        the SortedListWithKey.
+        Optional `iterable` argument provides an initial iterable of values to
+        initialize the sorted-key list.
 
-        An optional *key* argument defines a callable that, like the `key`
+        Optional `key` argument defines a callable that, like the `key`
         argument to Python's `sorted` function, extracts a comparison key from
-        each element. The default is the identity function.
+        each value. The default is the identity function.
+
+        Runtime complexity: `O(n*log(n))`
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList(key=neg)
+        >>> skl
+        SortedKeyList([], key=<built-in function neg>)
+        >>> skl = SortedKeyList([3, 1, 2], key=neg)
+        >>> skl
+        SortedKeyList([3, 2, 1], key=<built-in function neg>)
+
+        :param iterable: initial values (optional)
+        :param key: function used to extract comparison key (optional)
+
         """
-        # pylint: disable=super-init-not-called
+        self._key = key
         self._len = 0
+        self._load = self.DEFAULT_LOAD_FACTOR
         self._lists = []
         self._keys = []
         self._maxes = []
         self._index = []
-        self._key = key
-        self._load = LOAD
-        self._half = LOAD >> 1
-        self._dual = LOAD << 1
         self._offset = 0
 
         if iterable is not None:
             self._update(iterable)
 
+
     def __new__(cls, iterable=None, key=identity):
         return object.__new__(cls)
 
+
     @property
     def key(self):
-        """Key function used to extract comparison key for sorting."""
+        "Function used to extract comparison key from values."
         return self._key
 
+
     def clear(self):
-        """Remove all the elements from the list."""
+        """Remove all values from sorted-key list.
+
+        Runtime complexity: `O(n)`
+
+        """
         self._len = 0
         del self._lists[:]
         del self._keys[:]
         del self._maxes[:]
         del self._index[:]
 
     _clear = clear
 
-    def add(self, val):
-        """Add the element *val* to the list."""
+
+    def add(self, value):
+        """Add `value` to sorted-key list.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList(key=neg)
+        >>> skl.add(3)
+        >>> skl.add(1)
+        >>> skl.add(2)
+        >>> skl
+        SortedKeyList([3, 2, 1], key=<built-in function neg>)
+
+        :param value: value to add to sorted-key list
+
+        """
         _lists = self._lists
         _keys = self._keys
         _maxes = self._maxes
 
-        key = self._key(val)
+        key = self._key(value)
 
         if _maxes:
             pos = bisect_right(_maxes, key)
 
             if pos == len(_maxes):
                 pos -= 1
-                _lists[pos].append(val)
+                _lists[pos].append(value)
                 _keys[pos].append(key)
                 _maxes[pos] = key
             else:
                 idx = bisect_right(_keys[pos], key)
-                _lists[pos].insert(idx, val)
+                _lists[pos].insert(idx, value)
                 _keys[pos].insert(idx, key)
 
             self._expand(pos)
         else:
-            _lists.append([val])
+            _lists.append([value])
             _keys.append([key])
             _maxes.append(key)
 
         self._len += 1
 
+
     def _expand(self, pos):
-        """Splits sublists that are more than double the load level.
+        """Split sublists with length greater than double the load-factor.
 
         Updates the index when the sublist length is less than double the load
         level. This requires incrementing the nodes in a traversal from the
-        leaf node to the root. For an example traversal see self._loc.
+        leaf node to the root. For an example traversal see
+        ``SortedList._loc``.
 
         """
         _lists = self._lists
         _keys = self._keys
         _index = self._index
 
-        if len(_keys[pos]) > self._dual:
+        if len(_keys[pos]) > (self._load << 1):
             _maxes = self._maxes
             _load = self._load
 
             _lists_pos = _lists[pos]
             _keys_pos = _keys[pos]
             half = _lists_pos[_load:]
             half_keys = _keys_pos[_load:]
@@ -1590,24 +1852,38 @@
             if _index:
                 child = self._offset + pos
                 while child:
                     _index[child] += 1
                     child = (child - 1) >> 1
                 _index[0] += 1
 
+
     def update(self, iterable):
-        """Update the list by adding all elements from *iterable*."""
+        """Update sorted-key list by adding all values from `iterable`.
+
+        Runtime complexity: `O(k*log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList(key=neg)
+        >>> skl.update([3, 1, 2])
+        >>> skl
+        SortedKeyList([3, 2, 1], key=<built-in function neg>)
+
+        :param iterable: iterable of values to add
+
+        """
         _lists = self._lists
         _keys = self._keys
         _maxes = self._maxes
         values = sorted(iterable, key=self._key)
 
         if _maxes:
             if len(values) * 4 >= self._len:
-                values.extend(chain.from_iterable(_lists))
+                _lists.append(values)
+                values = reduce(iadd, _lists, [])
                 values.sort(key=self._key)
                 self._clear()
             else:
                 _add = self.add
                 for val in values:
                     _add(val)
                 return
@@ -1618,22 +1894,37 @@
         _keys.extend(list(map(self._key, _list)) for _list in _lists)
         _maxes.extend(sublist[-1] for sublist in _keys)
         self._len = len(values)
         del self._index[:]
 
     _update = update
 
-    def __contains__(self, val):
-        """Return True if and only if *val* is an element in the list."""
+
+    def __contains__(self, value):
+        """Return true if `value` is an element of the sorted-key list.
+
+        ``skl.__contains__(value)`` <==> ``value in skl``
+
+        Runtime complexity: `O(log(n))`
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([1, 2, 3, 4, 5], key=neg)
+        >>> 3 in skl
+        True
+
+        :param value: search for value in sorted-key list
+        :return: true if `value` in sorted-key list
+
+        """
         _maxes = self._maxes
 
         if not _maxes:
             return False
 
-        key = self._key(val)
+        key = self._key(value)
         pos = bisect_left(_maxes, key)
 
         if pos == len(_maxes):
             return False
 
         _lists = self._lists
         _keys = self._keys
@@ -1642,362 +1933,250 @@
 
         len_keys = len(_keys)
         len_sublist = len(_keys[pos])
 
         while True:
             if _keys[pos][idx] != key:
                 return False
-            if _lists[pos][idx] == val:
+            if _lists[pos][idx] == value:
                 return True
             idx += 1
             if idx == len_sublist:
                 pos += 1
                 if pos == len_keys:
                     return False
                 len_sublist = len(_keys[pos])
                 idx = 0
 
-    def discard(self, val):
-        """
-        Remove the first occurrence of *val*.
 
-        If *val* is not a member, does nothing.
+    def discard(self, value):
+        """Remove `value` from sorted-key list if it is a member.
+
+        If `value` is not a member, do nothing.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([5, 4, 3, 2, 1], key=neg)
+        >>> skl.discard(1)
+        >>> skl.discard(0)
+        >>> skl == [5, 4, 3, 2]
+        True
+
+        :param value: `value` to discard from sorted-key list
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return
 
-        key = self._key(val)
+        key = self._key(value)
         pos = bisect_left(_maxes, key)
 
         if pos == len(_maxes):
             return
 
         _lists = self._lists
         _keys = self._keys
         idx = bisect_left(_keys[pos], key)
         len_keys = len(_keys)
         len_sublist = len(_keys[pos])
 
         while True:
             if _keys[pos][idx] != key:
                 return
-            if _lists[pos][idx] == val:
+            if _lists[pos][idx] == value:
                 self._delete(pos, idx)
                 return
             idx += 1
             if idx == len_sublist:
                 pos += 1
                 if pos == len_keys:
                     return
                 len_sublist = len(_keys[pos])
                 idx = 0
 
-    def remove(self, val):
-        """
-        Remove first occurrence of *val*.
 
-        Raises ValueError if *val* is not present.
+    def remove(self, value):
+        """Remove `value` from sorted-key list; `value` must be a member.
+
+        If `value` is not a member, raise ValueError.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([1, 2, 3, 4, 5], key=neg)
+        >>> skl.remove(5)
+        >>> skl == [4, 3, 2, 1]
+        True
+        >>> skl.remove(0)
+        Traceback (most recent call last):
+          ...
+        ValueError: 0 not in list
+
+        :param value: `value` to remove from sorted-key list
+        :raises ValueError: if `value` is not in sorted-key list
+
         """
         _maxes = self._maxes
 
         if not _maxes:
-            raise ValueError('{0!r} not in list'.format(val))
+            raise ValueError('{0!r} not in list'.format(value))
 
-        key = self._key(val)
+        key = self._key(value)
         pos = bisect_left(_maxes, key)
 
         if pos == len(_maxes):
-            raise ValueError('{0!r} not in list'.format(val))
+            raise ValueError('{0!r} not in list'.format(value))
 
         _lists = self._lists
         _keys = self._keys
         idx = bisect_left(_keys[pos], key)
         len_keys = len(_keys)
         len_sublist = len(_keys[pos])
 
         while True:
             if _keys[pos][idx] != key:
-                raise ValueError('{0!r} not in list'.format(val))
-            if _lists[pos][idx] == val:
+                raise ValueError('{0!r} not in list'.format(value))
+            if _lists[pos][idx] == value:
                 self._delete(pos, idx)
                 return
             idx += 1
             if idx == len_sublist:
                 pos += 1
                 if pos == len_keys:
-                    raise ValueError('{0!r} not in list'.format(val))
+                    raise ValueError('{0!r} not in list'.format(value))
                 len_sublist = len(_keys[pos])
                 idx = 0
 
+
     def _delete(self, pos, idx):
-        """
-        Delete the item at the given (pos, idx).
+        """Delete value at the given `(pos, idx)`.
 
         Combines lists that are less than half the load level.
 
         Updates the index when the sublist length is more than half the load
-        level. This requires decrementing the nodes in a traversal from the leaf
-        node to the root. For an example traversal see self._loc.
+        level. This requires decrementing the nodes in a traversal from the
+        leaf node to the root. For an example traversal see
+        ``SortedList._loc``.
+
+        :param int pos: lists index
+        :param int idx: sublist index
+
         """
         _lists = self._lists
         _keys = self._keys
         _maxes = self._maxes
         _index = self._index
         keys_pos = _keys[pos]
         lists_pos = _lists[pos]
 
         del keys_pos[idx]
         del lists_pos[idx]
         self._len -= 1
 
         len_keys_pos = len(keys_pos)
 
-        if len_keys_pos > self._half:
-
+        if len_keys_pos > (self._load >> 1):
             _maxes[pos] = keys_pos[-1]
 
             if _index:
                 child = self._offset + pos
                 while child > 0:
                     _index[child] -= 1
                     child = (child - 1) >> 1
                 _index[0] -= 1
-
         elif len(_keys) > 1:
-
             if not pos:
                 pos += 1
 
             prev = pos - 1
             _keys[prev].extend(_keys[pos])
             _lists[prev].extend(_lists[pos])
             _maxes[prev] = _keys[prev][-1]
 
             del _lists[pos]
             del _keys[pos]
             del _maxes[pos]
             del _index[:]
 
             self._expand(prev)
-
         elif len_keys_pos:
-
             _maxes[pos] = keys_pos[-1]
-
         else:
-
             del _lists[pos]
             del _keys[pos]
             del _maxes[pos]
             del _index[:]
 
-    def _check_order(self, idx, key, val):
-        # pylint: disable=arguments-differ
-        _len = self._len
-        _keys = self._keys
-
-        pos, loc = self._pos(idx)
-
-        if idx < 0:
-            idx += _len
-
-        # Check that the inserted value is not less than the
-        # previous value.
-
-        if idx > 0:
-            idx_prev = loc - 1
-            pos_prev = pos
-
-            if idx_prev < 0:
-                pos_prev -= 1
-                idx_prev = len(_keys[pos_prev]) - 1
-
-            if _keys[pos_prev][idx_prev] > key:
-                msg = '{0!r} not in sort order at index {1}'.format(val, idx)
-                raise ValueError(msg)
-
-        # Check that the inserted value is not greater than
-        # the previous value.
-
-        if idx < (_len - 1):
-            idx_next = loc + 1
-            pos_next = pos
-
-            if idx_next == len(_keys[pos_next]):
-                pos_next += 1
-                idx_next = 0
-
-            if _keys[pos_next][idx_next] < key:
-                msg = '{0!r} not in sort order at index {1}'.format(val, idx)
-                raise ValueError(msg)
-
-    def __setitem__(self, index, value):
-        """Replace the item at position *index* with *value*.
-
-        Supports slice notation. Raises a :exc:`ValueError` if the sort order
-        would be violated. When used with a slice and iterable, the
-        :exc:`ValueError` is raised before the list is mutated if the sort
-        order would be violated by the operation.
-
-        """
-        # pylint: disable=too-many-locals
-        _lists = self._lists
-        _keys = self._keys
-        _maxes = self._maxes
-        _check_order = self._check_order
-        _pos = self._pos
-
-        if isinstance(index, slice):
-            _len = self._len
-            start, stop, step = index.indices(_len)
-            indices = range(start, stop, step)
-
-            # Copy value to avoid aliasing issues with self and cases where an
-            # iterator is given.
-
-            values = tuple(value)
-
-            if step != 1:
-                if len(values) != len(indices):
-                    raise ValueError(
-                        'attempt to assign sequence of size %s'
-                        ' to extended slice of size %s'
-                        % (len(values), len(indices)))
-
-                # Keep a log of values that are set so that we can
-                # roll back changes if ordering is violated.
-
-                log = []
-                _append = log.append
-
-                for idx, val in zip(indices, values):
-                    pos, loc = _pos(idx)
-                    key = self._key(val)
-                    _append((idx, _keys[pos][loc], key, _lists[pos][loc], val))
-                    _keys[pos][loc] = key
-                    _lists[pos][loc] = val
-                    if len(_keys[pos]) == (loc + 1):
-                        _maxes[pos] = key
-
-                try:
-                    # Validate ordering of new values.
-
-                    for idx, oldkey, newkey, oldval, newval in log:
-                        _check_order(idx, newkey, newval)
-
-                except ValueError:
-
-                    # Roll back changes from log.
-
-                    for idx, oldkey, newkey, oldval, newval in log:
-                        pos, loc = _pos(idx)
-                        _keys[pos][loc] = oldkey
-                        _lists[pos][loc] = oldval
-                        if len(_keys[pos]) == (loc + 1):
-                            _maxes[pos] = oldkey
-
-                    raise
-            else:
-                if start == 0 and stop == self._len:
-                    self._clear()
-                    return self._update(values)
-
-                if stop < start:
-                    # When calculating indices, stop may be less than start.
-                    # For example: ...[5:3:1] results in slice(5, 3, 1) which
-                    # is a valid but not useful stop index.
-                    stop = start
-
-                if values:
-
-                    # Check that given values are ordered properly.
-
-                    keys = tuple(map(self._key, values))
-                    alphas = iter(keys)
-                    betas = iter(keys)
-                    next(betas)
-                    pairs = zip(alphas, betas)
-
-                    if not all(alpha <= beta for alpha, beta in pairs):
-                        raise ValueError('given values not in sort order')
-
-                    # Check ordering in context of sorted list.
-
-                    if start:
-                        pos, loc = _pos(start - 1)
-                        if _keys[pos][loc] > keys[0]:
-                            msg = '{0!r} not in sort order at index {1}'.format(
-                                values[0], start)
-                            raise ValueError(msg)
-
-                    if stop != _len:
-                        pos, loc = _pos(stop)
-                        if _keys[pos][loc] < keys[-1]:
-                            msg = '{0!r} not in sort order at index {1}'.format(
-                                values[-1], stop)
-                            raise ValueError(msg)
-
-                # Delete the existing values.
-
-                self._delitem(index)
-
-                # Insert the new values.
-
-                _insert = self.insert
-                for idx, val in enumerate(values):
-                    _insert(start + idx, val)
-        else:
-            pos, loc = _pos(index)
-            key = self._key(value)
-            _check_order(index, key, value)
-            _lists[pos][loc] = value
-            _keys[pos][loc] = key
-            if len(_lists[pos]) == (loc + 1):
-                _maxes[pos] = key
 
     def irange(self, minimum=None, maximum=None, inclusive=(True, True),
                reverse=False):
-        """
-        Create an iterator of values between `minimum` and `maximum`.
-
-        `inclusive` is a pair of booleans that indicates whether the minimum
-        and maximum ought to be included in the range, respectively. The
-        default is (True, True) such that the range is inclusive of both
-        minimum and maximum.
+        """Create an iterator of values between `minimum` and `maximum`.
 
         Both `minimum` and `maximum` default to `None` which is automatically
-        inclusive of the start and end of the list, respectively.
+        inclusive of the beginning and end of the sorted-key list.
+
+        The argument `inclusive` is a pair of booleans that indicates whether
+        the minimum and maximum ought to be included in the range,
+        respectively. The default is ``(True, True)`` such that the range is
+        inclusive of both minimum and maximum.
 
         When `reverse` is `True` the values are yielded from the iterator in
         reverse order; `reverse` defaults to `False`.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([11, 12, 13, 14, 15], key=neg)
+        >>> it = skl.irange(14.5, 11.5)
+        >>> list(it)
+        [14, 13, 12]
+
+        :param minimum: minimum value to start iterating
+        :param maximum: maximum value to stop iterating
+        :param inclusive: pair of booleans
+        :param bool reverse: yield values in reverse order
+        :return: iterator
+
         """
-        minimum = self._key(minimum) if minimum is not None else None
-        maximum = self._key(maximum) if maximum is not None else None
+        min_key = self._key(minimum) if minimum is not None else None
+        max_key = self._key(maximum) if maximum is not None else None
         return self._irange_key(
-            min_key=minimum, max_key=maximum,
+            min_key=min_key, max_key=max_key,
             inclusive=inclusive, reverse=reverse,
         )
 
+
     def irange_key(self, min_key=None, max_key=None, inclusive=(True, True),
                    reverse=False):
-        """
-        Create an iterator of values between `min_key` and `max_key`.
-
-        `inclusive` is a pair of booleans that indicates whether the min_key
-        and max_key ought to be included in the range, respectively. The
-        default is (True, True) such that the range is inclusive of both
-        `min_key` and `max_key`.
+        """Create an iterator of values between `min_key` and `max_key`.
 
         Both `min_key` and `max_key` default to `None` which is automatically
-        inclusive of the start and end of the list, respectively.
+        inclusive of the beginning and end of the sorted-key list.
+
+        The argument `inclusive` is a pair of booleans that indicates whether
+        the minimum and maximum ought to be included in the range,
+        respectively. The default is ``(True, True)`` such that the range is
+        inclusive of both minimum and maximum.
 
         When `reverse` is `True` the values are yielded from the iterator in
         reverse order; `reverse` defaults to `False`.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([11, 12, 13, 14, 15], key=neg)
+        >>> it = skl.irange_key(-14, -12)
+        >>> list(it)
+        [14, 13, 12]
+
+        :param min_key: minimum key to start iterating
+        :param max_key: maximum key to stop iterating
+        :param inclusive: pair of booleans
+        :param bool reverse: yield values in reverse order
+        :return: iterator
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return iter(())
 
         _keys = self._keys
@@ -2048,37 +2227,79 @@
                 else:
                     max_idx = bisect_left(_keys[max_pos], max_key)
 
         return self._islice(min_pos, min_idx, max_pos, max_idx, reverse)
 
     _irange_key = irange_key
 
-    def bisect_left(self, val):
-        """
-        Similar to the *bisect* module in the standard library, this returns an
-        appropriate index to insert *val*. If *val* is already present, the
-        insertion point will be before (to the left of) any existing entries.
-        """
-        return self._bisect_key_left(self._key(val))
 
-    def bisect_right(self, val):
+    def bisect_left(self, value):
+        """Return an index to insert `value` in the sorted-key list.
+
+        If the `value` is already present, the insertion point will be before
+        (to the left of) any existing values.
+
+        Similar to the `bisect` module in the standard library.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([5, 4, 3, 2, 1], key=neg)
+        >>> skl.bisect_left(1)
+        4
+
+        :param value: insertion index of value in sorted-key list
+        :return: index
+
         """
-        Same as *bisect_left*, but if *val* is already present, the insertion
-        point will be after (to the right of) any existing entries.
+        return self._bisect_key_left(self._key(value))
+
+
+    def bisect_right(self, value):
+        """Return an index to insert `value` in the sorted-key list.
+
+        Similar to `bisect_left`, but if `value` is already present, the
+        insertion point will be after (to the right of) any existing values.
+
+        Similar to the `bisect` module in the standard library.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedList([5, 4, 3, 2, 1], key=neg)
+        >>> skl.bisect_right(1)
+        5
+
+        :param value: insertion index of value in sorted-key list
+        :return: index
+
         """
-        return self._bisect_key_right(self._key(val))
+        return self._bisect_key_right(self._key(value))
 
     bisect = bisect_right
 
+
     def bisect_key_left(self, key):
-        """
-        Similar to the *bisect* module in the standard library, this returns an
-        appropriate index to insert a value with a given *key*. If values with
-        *key* are already present, the insertion point will be before (to the
-        left of) any existing entries.
+        """Return an index to insert `key` in the sorted-key list.
+
+        If the `key` is already present, the insertion point will be before (to
+        the left of) any existing keys.
+
+        Similar to the `bisect` module in the standard library.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([5, 4, 3, 2, 1], key=neg)
+        >>> skl.bisect_key_left(-1)
+        4
+
+        :param key: insertion index of key in sorted-key list
+        :return: index
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return 0
 
         pos = bisect_left(_maxes, key)
@@ -2088,18 +2309,33 @@
 
         idx = bisect_left(self._keys[pos], key)
 
         return self._loc(pos, idx)
 
     _bisect_key_left = bisect_key_left
 
+
     def bisect_key_right(self, key):
-        """
-        Same as *bisect_key_left*, but if *key* is already present, the insertion
-        point will be after (to the right of) any existing entries.
+        """Return an index to insert `key` in the sorted-key list.
+
+        Similar to `bisect_key_left`, but if `key` is already present, the
+        insertion point will be after (to the right of) any existing keys.
+
+        Similar to the `bisect` module in the standard library.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedList([5, 4, 3, 2, 1], key=neg)
+        >>> skl.bisect_key_right(-1)
+        5
+
+        :param key: insertion index of key in sorted-key list
+        :return: index
+
         """
         _maxes = self._maxes
 
         if not _maxes:
             return 0
 
         pos = bisect_right(_maxes, key)
@@ -2110,22 +2346,35 @@
         idx = bisect_right(self._keys[pos], key)
 
         return self._loc(pos, idx)
 
     bisect_key = bisect_key_right
     _bisect_key_right = bisect_key_right
 
-    def count(self, val):
-        """Return the number of occurrences of *val* in the list."""
+
+    def count(self, value):
+        """Return number of occurrences of `value` in the sorted-key list.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([4, 4, 4, 4, 3, 3, 3, 2, 2, 1], key=neg)
+        >>> skl.count(2)
+        2
+
+        :param value: value to count in sorted-key list
+        :return: count
+
+        """
         _maxes = self._maxes
 
         if not _maxes:
             return 0
 
-        key = self._key(val)
+        key = self._key(value)
         pos = bisect_left(_maxes, key)
 
         if pos == len(_maxes):
             return 0
 
         _lists = self._lists
         _keys = self._keys
@@ -2133,194 +2382,71 @@
         total = 0
         len_keys = len(_keys)
         len_sublist = len(_keys[pos])
 
         while True:
             if _keys[pos][idx] != key:
                 return total
-            if _lists[pos][idx] == val:
+            if _lists[pos][idx] == value:
                 total += 1
             idx += 1
             if idx == len_sublist:
                 pos += 1
                 if pos == len_keys:
                     return total
                 len_sublist = len(_keys[pos])
                 idx = 0
 
-    def copy(self):
-        """Return a shallow copy of the sorted list."""
-        return self.__class__(self, key=self._key)
-
-    __copy__ = copy
-
-    def append(self, val):
-        """
-        Append the element *val* to the list. Raises a ValueError if the *val*
-        would violate the sort order.
-        """
-        # pylint: disable=arguments-differ
-        _lists = self._lists
-        _keys = self._keys
-        _maxes = self._maxes
-        key = self._key(val)
-
-        if not _maxes:
-            _maxes.append(key)
-            _keys.append([key])
-            _lists.append([val])
-            self._len = 1
-            return
-
-        pos = len(_keys) - 1
-
-        if key < _keys[pos][-1]:
-            msg = '{0!r} not in sort order at index {1}'.format(val, self._len)
-            raise ValueError(msg)
-
-        _lists[pos].append(val)
-        _keys[pos].append(key)
-        _maxes[pos] = key
-        self._len += 1
-        self._expand(pos)
 
-    def extend(self, values):
-        """
-        Extend the list by appending all elements from the *values*. Raises a
-        ValueError if the sort order would be violated.
-        """
-        _lists = self._lists
-        _keys = self._keys
-        _maxes = self._maxes
-        _load = self._load
-
-        if not isinstance(values, list):
-            values = list(values)
-
-        keys = list(map(self._key, values))
-
-        if any(keys[pos - 1] > keys[pos]
-               for pos in range(1, len(keys))):
-            raise ValueError('given sequence not in sort order')
-
-        offset = 0
-
-        if _maxes:
-            if keys[0] < _keys[-1][-1]:
-                msg = '{0!r} not in sort order at index {1}'.format(values[0], self._len)
-                raise ValueError(msg)
-
-            if len(_keys[-1]) < self._half:
-                _lists[-1].extend(values[:_load])
-                _keys[-1].extend(keys[:_load])
-                _maxes[-1] = _keys[-1][-1]
-                offset = _load
-
-        len_keys = len(_keys)
+    def copy(self):
+        """Return a shallow copy of the sorted-key list.
 
-        for idx in range(offset, len(keys), _load):
-            _lists.append(values[idx:(idx + _load)])
-            _keys.append(keys[idx:(idx + _load)])
-            _maxes.append(_keys[-1][-1])
+        Runtime complexity: `O(n)`
 
-        _index = self._index
+        :return: new sorted-key list
 
-        if len_keys == len(_keys):
-            len_index = len(_index)
-            if len_index > 0:
-                len_values = len(values)
-                child = len_index - 1
-                while child:
-                    _index[child] += len_values
-                    child = (child - 1) >> 1
-                _index[0] += len_values
-        else:
-            del _index[:]
-
-        self._len += len(values)
-
-    def insert(self, idx, val):
-        """
-        Insert the element *val* into the list at *idx*. Raises a ValueError if
-        the *val* at *idx* would violate the sort order.
         """
-        _len = self._len
-        _lists = self._lists
-        _keys = self._keys
-        _maxes = self._maxes
-
-        if idx < 0:
-            idx += _len
-        if idx < 0:
-            idx = 0
-        if idx > _len:
-            idx = _len
+        return self.__class__(self, key=self._key)
 
-        key = self._key(val)
+    __copy__ = copy
 
-        if not _maxes:
-            self._len = 1
-            _lists.append([val])
-            _keys.append([key])
-            _maxes.append(key)
-            return
 
-        if not idx:
-            if key > _keys[0][0]:
-                msg = '{0!r} not in sort order at index {1}'.format(val, 0)
-                raise ValueError(msg)
-            else:
-                self._len += 1
-                _lists[0].insert(0, val)
-                _keys[0].insert(0, key)
-                self._expand(0)
-                return
+    def index(self, value, start=None, stop=None):
+        """Return first index of value in sorted-key list.
 
-        if idx == _len:
-            pos = len(_keys) - 1
-            if _keys[pos][-1] > key:
-                msg = '{0!r} not in sort order at index {1}'.format(val, _len)
-                raise ValueError(msg)
-            else:
-                self._len += 1
-                _lists[pos].append(val)
-                _keys[pos].append(key)
-                _maxes[pos] = _keys[pos][-1]
-                self._expand(pos)
-                return
+        Raise ValueError if `value` is not present.
 
-        pos, idx = self._pos(idx)
-        idx_before = idx - 1
-        if idx_before < 0:
-            pos_before = pos - 1
-            idx_before = len(_keys[pos_before]) - 1
-        else:
-            pos_before = pos
+        Index must be between `start` and `stop` for the `value` to be
+        considered present. The default value, None, for `start` and `stop`
+        indicate the beginning and end of the sorted-key list.
+
+        Negative indices are supported.
+
+        Runtime complexity: `O(log(n))` -- approximate.
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([5, 4, 3, 2, 1], key=neg)
+        >>> skl.index(2)
+        3
+        >>> skl.index(0)
+        Traceback (most recent call last):
+          ...
+        ValueError: 0 is not in list
+
+        :param value: value in sorted-key list
+        :param int start: start index (default None, start of sorted-key list)
+        :param int stop: stop index (default None, end of sorted-key list)
+        :return: index of value
+        :raises ValueError: if value is not present
 
-        before = _keys[pos_before][idx_before]
-        if before <= key <= _keys[pos][idx]:
-            self._len += 1
-            _lists[pos].insert(idx, val)
-            _keys[pos].insert(idx, key)
-            self._expand(pos)
-        else:
-            msg = '{0!r} not in sort order at index {1}'.format(val, idx)
-            raise ValueError(msg)
-
-    def index(self, val, start=None, stop=None):
-        """
-        Return the smallest *k* such that L[k] == val and i <= k < j`.  Raises
-        ValueError if *val* is not present.  *stop* defaults to the end of the
-        list. *start* defaults to the beginning. Negative indices are supported,
-        as for slice indices.
         """
         _len = self._len
 
         if not _len:
-            raise ValueError('{0!r} is not in list'.format(val))
+            raise ValueError('{0!r} is not in list'.format(value))
 
         if start is None:
             start = 0
         if start < 0:
             start += _len
         if start < 0:
             start = 0
@@ -2329,180 +2455,191 @@
             stop = _len
         if stop < 0:
             stop += _len
         if stop > _len:
             stop = _len
 
         if stop <= start:
-            raise ValueError('{0!r} is not in list'.format(val))
+            raise ValueError('{0!r} is not in list'.format(value))
 
         _maxes = self._maxes
-        key = self._key(val)
+        key = self._key(value)
         pos = bisect_left(_maxes, key)
 
         if pos == len(_maxes):
-            raise ValueError('{0!r} is not in list'.format(val))
+            raise ValueError('{0!r} is not in list'.format(value))
 
         stop -= 1
         _lists = self._lists
         _keys = self._keys
         idx = bisect_left(_keys[pos], key)
         len_keys = len(_keys)
         len_sublist = len(_keys[pos])
 
         while True:
             if _keys[pos][idx] != key:
-                raise ValueError('{0!r} is not in list'.format(val))
-            if _lists[pos][idx] == val:
+                raise ValueError('{0!r} is not in list'.format(value))
+            if _lists[pos][idx] == value:
                 loc = self._loc(pos, idx)
                 if start <= loc <= stop:
                     return loc
                 elif loc > stop:
                     break
             idx += 1
             if idx == len_sublist:
                 pos += 1
                 if pos == len_keys:
-                    raise ValueError('{0!r} is not in list'.format(val))
+                    raise ValueError('{0!r} is not in list'.format(value))
                 len_sublist = len(_keys[pos])
                 idx = 0
 
-        raise ValueError('{0!r} is not in list'.format(val))
+        raise ValueError('{0!r} is not in list'.format(value))
+
+
+    def __add__(self, other):
+        """Return new sorted-key list containing all values in both sequences.
+
+        ``skl.__add__(other)`` <==> ``skl + other``
+
+        Values in `other` do not need to be in sorted-key order.
+
+        Runtime complexity: `O(n*log(n))`
+
+        >>> from operator import neg
+        >>> skl1 = SortedKeyList([5, 4, 3], key=neg)
+        >>> skl2 = SortedKeyList([2, 1, 0], key=neg)
+        >>> skl1 + skl2
+        SortedKeyList([5, 4, 3, 2, 1, 0], key=<built-in function neg>)
+
+        :param other: other iterable
+        :return: new sorted-key list
 
-    def __add__(self, that):
-        """
-        Return a new sorted list containing all the elements in *self* and
-        *that*. Elements in *that* do not need to be properly ordered with
-        respect to *self*.
         """
         values = reduce(iadd, self._lists, [])
-        values.extend(that)
+        values.extend(other)
         return self.__class__(values, key=self._key)
 
-    def __mul__(self, that):
-        """
-        Return a new sorted list containing *that* shallow copies of each item
-        in SortedListWithKey.
+    __radd__ = __add__
+
+
+    def __mul__(self, num):
+        """Return new sorted-key list with `num` shallow copies of values.
+
+        ``skl.__mul__(num)`` <==> ``skl * num``
+
+        Runtime complexity: `O(n*log(n))`
+
+        >>> from operator import neg
+        >>> skl = SortedKeyList([3, 2, 1], key=neg)
+        >>> skl * 2
+        SortedKeyList([3, 3, 2, 2, 1, 1], key=<built-in function neg>)
+
+        :param int num: count of shallow copies
+        :return: new sorted-key list
+
         """
-        values = reduce(iadd, self._lists, []) * that
+        values = reduce(iadd, self._lists, []) * num
         return self.__class__(values, key=self._key)
 
-    def __imul__(self, that):
-        """
-        Increase the length of the list by appending *that* shallow copies of
-        each item.
-        """
-        values = reduce(iadd, self._lists, []) * that
-        self._clear()
-        self._update(values)
-        return self
 
-    @recursive_repr
+    def __reduce__(self):
+        values = reduce(iadd, self._lists, [])
+        return (type(self), (values, self.key))
+
+
+    @recursive_repr()
     def __repr__(self):
-        """Return string representation of sequence."""
-        name = type(self).__name__
-        values = list(self)
-        _key = self._key
-        return '{0}({1!r}, key={2!r})'.format(name, values, _key)
+        """Return string representation of sorted-key list.
 
-    def _check(self):
-        try:
-            # Check load parameters.
+        ``skl.__repr__()`` <==> ``repr(skl)``
 
-            assert self._load >= 4
-            assert self._half == (self._load >> 1)
-            assert self._dual == (self._load << 1)
+        :return: string representation
 
-            # Check empty sorted list case.
+        """
+        type_name = type(self).__name__
+        return '{0}({1!r}, key={2!r})'.format(type_name, list(self), self._key)
 
-            if self._maxes == []:
-                assert self._keys == []
-                assert self._lists == []
-                return
 
-            assert self._maxes and self._keys and self._lists
+    def _check(self):
+        """Check invariants of sorted-key list.
+
+        Runtime complexity: `O(n)`
+
+        """
+        try:
+            assert self._load >= 4
+            assert len(self._maxes) == len(self._lists) == len(self._keys)
+            assert self._len == sum(len(sublist) for sublist in self._lists)
 
             # Check all sublists are sorted.
 
-            assert all(sublist[pos - 1] <= sublist[pos]
-                       for sublist in self._keys
-                       for pos in range(1, len(sublist)))
+            for sublist in self._keys:
+                for pos in range(1, len(sublist)):
+                    assert sublist[pos - 1] <= sublist[pos]
 
             # Check beginning/end of sublists are sorted.
 
             for pos in range(1, len(self._keys)):
                 assert self._keys[pos - 1][-1] <= self._keys[pos][0]
 
-            # Check length of _maxes and _lists match.
-
-            assert len(self._maxes) == len(self._lists) == len(self._keys)
-
             # Check _keys matches _key mapped to _lists.
 
-            assert all(len(val_list) == len(key_list)
-                       for val_list, key_list in zip(self._lists, self._keys))
-            assert all(self._key(val) == key for val, key in
-                       zip((_val for _val_list in self._lists for _val in _val_list),
-                           (_key for _key_list in self._keys for _key in _key_list)))
+            for val_sublist, key_sublist in zip(self._lists, self._keys):
+                assert len(val_sublist) == len(key_sublist)
+                for val, key in zip(val_sublist, key_sublist):
+                    assert self._key(val) == key
 
-            # Check _maxes is a map of _keys.
+            # Check _maxes index is the last value of each sublist.
 
-            assert all(self._maxes[pos] == self._keys[pos][-1]
-                       for pos in range(len(self._maxes)))
+            for pos in range(len(self._maxes)):
+                assert self._maxes[pos] == self._keys[pos][-1]
 
-            # Check load level is less than _dual.
+            # Check sublist lengths are less than double load-factor.
 
-            assert all(len(sublist) <= self._dual for sublist in self._lists)
+            double = self._load << 1
+            assert all(len(sublist) <= double for sublist in self._lists)
 
-            # Check load level is greater than _half for all
+            # Check sublist lengths are greater than half load-factor for all
             # but the last sublist.
 
-            assert all(len(self._lists[pos]) >= self._half
-                       for pos in range(0, len(self._lists) - 1))
-
-            # Check length.
-
-            assert self._len == sum(len(sublist) for sublist in self._lists)
-
-            # Check index.
+            half = self._load >> 1
+            for pos in range(0, len(self._lists) - 1):
+                assert len(self._lists[pos]) >= half
 
             if self._index:
-                assert len(self._index) == self._offset + len(self._lists)
                 assert self._len == self._index[0]
+                assert len(self._index) == self._offset + len(self._lists)
 
-                def test_offset_pos(pos):
-                    "Test positional indexing offset."
-                    from_index = self._index[self._offset + pos]
-                    return from_index == len(self._lists[pos])
+                # Check index leaf nodes equal length of sublists.
 
-                assert all(test_offset_pos(pos)
-                           for pos in range(len(self._lists)))
+                for pos in range(len(self._lists)):
+                    leaf = self._index[self._offset + pos]
+                    assert leaf == len(self._lists[pos])
+
+                # Check index branch nodes are the sum of their children.
 
                 for pos in range(self._offset):
                     child = (pos << 1) + 1
-                    if self._index[pos] == 0:
-                        assert child >= len(self._index)
+                    if child >= len(self._index):
+                        assert self._index[pos] == 0
                     elif child + 1 == len(self._index):
                         assert self._index[pos] == self._index[child]
                     else:
                         child_sum = self._index[child] + self._index[child + 1]
-                        assert self._index[pos] == child_sum
-
+                        assert child_sum == self._index[pos]
         except:
-            import sys
-            import traceback
-
             traceback.print_exc(file=sys.stdout)
-
             print('len', self._len)
-            print('load', self._load, self._half, self._dual)
+            print('load', self._load)
             print('offset', self._offset)
             print('len_index', len(self._index))
             print('index', self._index)
             print('len_maxes', len(self._maxes))
             print('maxes', self._maxes)
             print('len_keys', len(self._keys))
             print('keys', self._keys)
             print('len_lists', len(self._lists))
             print('lists', self._lists)
-
             raise
+
+
+SortedListWithKey = SortedKeyList
```

### Comparing `ovs-2.9.4/ovs/db/custom_index.py` & `ovs-3.0.0/ovs/db/custom_index.py`

 * *Files identical despite different names*

### Comparing `ovs-2.9.4/ovs/db/data.py` & `ovs-3.0.0/ovs/db/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 import ovs.json
 import ovs.jsonrpc
 import ovs.ovsuuid
 import ovs.poller
 import ovs.socket_util
 from ovs.db import error
 
-import six
-
 
 class ConstraintViolation(error.Error):
     def __init__(self, msg, json=None):
         error.Error.__init__(self, msg, json, tag="constraint violation")
 
 
 def escapeCString(src):
@@ -62,14 +60,16 @@
 
 def returnUnchanged(x):
     return x
 
 
 @functools.total_ordering
 class Atom(object):
+    __slots__ = ('value', 'type')
+
     def __init__(self, type_, value=None):
         self.type = type_
         if value is not None:
             self.value = value
         else:
             self.value = type_.default_atom()
 
@@ -115,24 +115,24 @@
     def is_default(self):
         return self == self.default(self.type)
 
     @staticmethod
     def from_json(base, json, symtab=None):
         type_ = base.type
         json = ovs.db.parser.float_to_int(json)
-        real_types = list(six.integer_types)
+        real_types = [int]
         real_types.extend([float])
         real_types = tuple(real_types)
         if ((type_ == ovs.db.types.IntegerType
-                and isinstance(json, six.integer_types))
+                and isinstance(json, int))
             or (type_ == ovs.db.types.RealType
                 and isinstance(json, real_types))
             or (type_ == ovs.db.types.BooleanType and isinstance(json, bool))
             or (type_ == ovs.db.types.StringType
-                and isinstance(json, six.string_types))):
+                and isinstance(json, str))):
             atom = Atom(type_, json)
         elif type_ == ovs.db.types.UuidType:
             atom = Atom(type_, ovs.ovsuuid.from_json(json, symtab))
         else:
             raise error.Error("expected %s" % type_.to_string(), json)
         atom.check_constraints(base)
         return atom
@@ -202,15 +202,15 @@
             return '.real = %.15g' % self.value
         elif self.type == ovs.db.types.BooleanType:
             if self.value:
                 return '.boolean = true'
             else:
                 return '.boolean = false'
         elif self.type == ovs.db.types.StringType:
-            return '.string = "%s"' % escapeCString(self.value)
+            return '.s = %s' % escapeCString(self.value)
         elif self.type == ovs.db.types.UuidType:
             return '.uuid = %s' % ovs.ovsuuid.to_c_assignment(self.value)
 
     def toEnglish(self, escapeLiteral=returnUnchanged):
         if self.type == ovs.db.types.IntegerType:
             return '%d' % self.value
         elif self.type == ovs.db.types.RealType:
@@ -247,31 +247,33 @@
             else:
                 return self.value
         elif self.type == ovs.db.types.UuidType:
             return str(self.value)
 
     @staticmethod
     def new(x):
-        if isinstance(x, six.integer_types):
+        if isinstance(x, int):
             t = ovs.db.types.IntegerType
         elif isinstance(x, float):
             t = ovs.db.types.RealType
         elif isinstance(x, bool):
             t = ovs.db.types.BooleanType
-        elif isinstance(x, six.string_types):
+        elif isinstance(x, str):
             t = ovs.db.types.StringType
         elif isinstance(x, uuid):
             t = ovs.db.types.UuidType
         else:
             raise TypeError
         return Atom(t, x)
 
 
 @functools.total_ordering
 class Datum(object):
+    __slots__ = ('type', 'values')
+
     def __init__(self, type_, values={}):
         self.type = type_
         self.values = values
 
     def __eq__(self, other):
         if not isinstance(other, Datum):
             return NotImplemented
@@ -316,15 +318,15 @@
     def check_constraints(self):
         """Checks that each of the atoms in 'datum' conforms to the constraints
         specified by its 'type' and raises an ovs.db.error.Error.
 
         This function is not commonly useful because the most ordinary way to
         obtain a datum is ultimately via Datum.from_json() or Atom.from_json(),
         which check constraints themselves."""
-        for keyAtom, valueAtom in six.iteritems(self.values):
+        for keyAtom, valueAtom in self.values.items():
             keyAtom.check_constraints(self.type.key)
             if valueAtom is not None:
                 valueAtom.check_constraints(self.type.value)
 
     @staticmethod
     def from_json(type_, json, symtab=None):
         """Parses 'json' as a datum of the type described by 'type'.  If
@@ -377,15 +379,15 @@
             return Datum(type_, {keyAtom: None})
 
     def to_json(self):
         if self.type.is_map():
             return ["map", [[k.to_json(), v.to_json()]
                             for k, v in sorted(self.values.items())]]
         elif len(self.values) == 1:
-            key = next(six.iterkeys(self.values))
+            key = next(iter(self.values.keys()))
             return key.to_json()
         else:
             return ["set", [k.to_json() for k in sorted(self.values.keys())]]
 
     def to_string(self):
         head = tail = None
         if self.type.n_max > 1 or len(self.values) == 0:
@@ -411,40 +413,40 @@
 
         if tail:
             s.append(tail)
         return ''.join(s)
 
     def diff(self, datum):
         if self.type.n_max > 1 or len(self.values) == 0:
-            for k, v in six.iteritems(datum.values):
+            for k, v in datum.values.items():
                 if k in self.values and v == self.values[k]:
                     del self.values[k]
                 else:
                     self.values[k] = v
         else:
             return datum
 
         return self
 
     def as_list(self):
         if self.type.is_map():
-            return [[k.value, v.value] for k, v in six.iteritems(self.values)]
+            return [[k.value, v.value] for k, v in self.values.items()]
         else:
-            return [k.value for k in six.iterkeys(self.values)]
+            return [k.value for k in self.values.keys()]
 
     def as_dict(self):
         return dict(self.values)
 
     def as_scalar(self):
         if len(self.values) == 1:
             if self.type.is_map():
-                k, v = next(six.iteritems(self.values))
+                k, v = next(iter(self.values.items()))
                 return [k.value, v.value]
             else:
-                return next(six.iterkeys(self.values)).value
+                return next(iter(self.values.keys())).value
         else:
             return None
 
     def to_python(self, uuid_to_row):
         """Returns this datum's value converted into a natural Python
         representation of this datum's type, according to the following
         rules:
@@ -483,15 +485,15 @@
             value = uuid_to_row(self.as_scalar(), self.type.key)
             if value is None:
                 return self.type.key.default()
             else:
                 return value
         elif self.type.is_map():
             value = {}
-            for k, v in six.iteritems(self.values):
+            for k, v in self.values.items():
                 dk = uuid_to_row(k.value, self.type.key)
                 dv = uuid_to_row(v.value, self.type.value)
                 if dk is not None and dv is not None:
                     value[dk] = dv
             return value
         else:
             s = set()
@@ -511,15 +513,15 @@
         'row_to_uuid', which should convert objects that represent rows (if
         any) into uuid.UUID objects and return other data unchanged.
 
         Raises ovs.db.error.Error if 'value' is not in an appropriate form for
         'type_'."""
         d = {}
         if isinstance(value, dict):
-            for k, v in six.iteritems(value):
+            for k, v in value.items():
                 ka = Atom.from_python(type_.key, row_to_uuid(k))
                 va = Atom.from_python(type_.value, row_to_uuid(v))
                 d[ka] = va
         elif isinstance(value, (list, set, tuple)):
             for k in value:
                 ka = Atom.from_python(type_.key, row_to_uuid(k))
                 d[ka] = None
@@ -561,24 +563,51 @@
         return self.type.n_min <= n <= self.type.n_max
 
     def cDeclareDatum(self, name):
         n = len(self.values)
         if n == 0:
             return ["static struct ovsdb_datum %s = { .n = 0 };"]
 
-        s = ["static union ovsdb_atom %s_keys[%d] = {" % (name, n)]
-        for key in sorted(self.values):
-            s += ["    { %s }," % key.cInitAtom(key)]
-        s += ["};"]
+        s = []
+        if self.type.key.type == ovs.db.types.StringType:
+            s += ["static struct json %s_key_strings[%d] = {"
+                  % (name, n)]
+            for key in sorted(self.values):
+                s += ['    { .type = JSON_STRING, '
+                      '.string = "%s", .count = 2 },'
+                      % escapeCString(key.value)]
+            s += ["};"]
+            s += ["static union ovsdb_atom %s_keys[%d] = {" % (name, n)]
+            for i in range(n):
+                s += ["    { .s = &%s_key_strings[%d] }," % (name, i)]
+            s += ["};"]
+        else:
+            s = ["static union ovsdb_atom %s_keys[%d] = {" % (name, n)]
+            for key in sorted(self.values):
+                s += ["    { %s }," % key.cInitAtom(key)]
+            s += ["};"]
 
         if self.type.value:
-            s = ["static union ovsdb_atom %s_values[%d] = {" % (name, n)]
-            for k, v in sorted(self.values.items()):
-                s += ["    { %s }," % v.cInitAtom(v)]
-            s += ["};"]
+            if self.type.value.type == ovs.db.types.StringType:
+                s += ["static struct json %s_val_strings[%d] = {"
+                      % (name, n)]
+                for k, v in sorted(self.values):
+                    s += ['    { .type = JSON_STRING, '
+                          '.string = "%s", .count = 2 },'
+                          % escapeCString(v.value)]
+                s += ["};"]
+                s += ["static union ovsdb_atom %s_values[%d] = {" % (name, n)]
+                for i in range(n):
+                    s += ["    { .s = &%s_val_strings[%d] }," % (name, i)]
+                s += ["};"]
+            else:
+                s = ["static union ovsdb_atom %s_values[%d] = {" % (name, n)]
+                for k, v in sorted(self.values.items()):
+                    s += ["    { %s }," % v.cInitAtom(v)]
+                s += ["};"]
 
         s += ["static struct ovsdb_datum %s = {" % name]
         s += ["    .n = %d," % n]
         s += ["    .keys = %s_keys," % name]
         if self.type.value:
             s += ["    .values = %s_values," % name]
         s += ["};"]
```

### Comparing `ovs-2.9.4/ovs/db/error.py` & `ovs-3.0.0/ovs/db/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,9 +26,9 @@
                 self.tag = "syntax error"
         else:
             self.tag = tag
 
         # Compose message.
         syntax = ""
         if self.json is not None:
-                syntax = 'syntax "%s": ' % ovs.json.to_string(self.json)
+            syntax = 'syntax "%s": ' % ovs.json.to_string(self.json)
         Exception.__init__(self, "%s%s: %s" % (syntax, self.tag, self.msg))
```

### Comparing `ovs-2.9.4/ovs/db/idl.py` & `ovs-3.0.0/ovs/db/idl.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,39 +8,181 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import collections
+import enum
 import functools
 import uuid
 
 import ovs.db.data as data
 import ovs.db.parser
 import ovs.db.schema
 import ovs.jsonrpc
 import ovs.ovsuuid
 import ovs.poller
 import ovs.vlog
 from ovs.db import custom_index
 from ovs.db import error
 
-import six
-
 vlog = ovs.vlog.Vlog("idl")
 
 __pychecker__ = 'no-classattr no-objattrs'
 
 ROW_CREATE = "create"
 ROW_UPDATE = "update"
 ROW_DELETE = "delete"
 
 OVSDB_UPDATE = 0
 OVSDB_UPDATE2 = 1
+OVSDB_UPDATE3 = 2
+
+CLUSTERED = "clustered"
+RELAY = "relay"
+
+
+Notice = collections.namedtuple('Notice', ('event', 'row', 'updates'))
+Notice.__new__.__defaults__ = (None,)  # default updates=None
+
+
+class ColumnDefaultDict(dict):
+    """A column dictionary with on-demand generated default values
+
+    This object acts like the Row._data column dictionary, but without the
+    necessity of populating column default values. These values are generated
+    on-demand and therefore only use memory once they are accessed.
+    """
+    __slots__ = ('_table', )
+
+    def __init__(self, table):
+        self._table = table
+        super().__init__()
+
+    def __missing__(self, column):
+        column = self._table.columns[column]
+        return ovs.db.data.Datum.default(column.type)
+
+    def keys(self):
+        return self._table.columns.keys()
+
+    def values(self):
+        return iter(self[k] for k in self)
+
+    def __iter__(self):
+        return iter(self.keys())
+
+    def __contains__(self, item):
+        return item in self.keys()
+
+
+class Monitor(enum.IntEnum):
+    monitor = OVSDB_UPDATE
+    monitor_cond = OVSDB_UPDATE2
+    monitor_cond_since = OVSDB_UPDATE3
+
+
+class ConditionState(object):
+    def __init__(self):
+        self._ack_cond = None
+        self._req_cond = None
+        self._new_cond = [True]
+
+    def __iter__(self):
+        return iter([self._new_cond, self._req_cond, self._ack_cond])
+
+    @property
+    def new(self):
+        """The latest freshly initialized condition change"""
+        return self._new_cond
+
+    @property
+    def acked(self):
+        """The last condition change that has been accepted by the server"""
+        return self._ack_cond
+
+    @property
+    def requested(self):
+        """A condition that's been requested, but not acked by the server"""
+        return self._req_cond
+
+    @property
+    def latest(self):
+        """The most recent condition change"""
+        return next(cond for cond in self if cond is not None)
+
+    @staticmethod
+    def is_true(condition):
+        return condition == [True]
+
+    def init(self, cond):
+        """Signal that a condition change is being initiated"""
+        self._new_cond = cond
+
+    def ack(self):
+        """Signal that a condition change has been acked"""
+        if self._req_cond is not None:
+            self._ack_cond, self._req_cond = (self._req_cond, None)
+
+    def request(self):
+        """Signal that a condition change has been requested"""
+        if self._new_cond is not None:
+            self._req_cond, self._new_cond = (self._new_cond, None)
+
+    def reset(self):
+        """Reset a requested condition change back to new"""
+        if self._req_cond is not None:
+            if self._new_cond is None:
+                self._new_cond = self._req_cond
+            self._req_cond = None
+            return True
+        return False
+
+
+class IdlTable(object):
+    def __init__(self, idl, table):
+        assert isinstance(table, ovs.db.schema.TableSchema)
+        self._table = table
+        self.need_table = False
+        self.rows = custom_index.IndexedRows(self)
+        self.idl = idl
+        self._condition_state = ConditionState()
+        self.columns = {k: IdlColumn(v) for k, v in table.columns.items()}
+
+    def __getattr__(self, attr):
+        return getattr(self._table, attr)
+
+    @property
+    def condition_state(self):
+        # read-only, no setter
+        return self._condition_state
+
+    @property
+    def condition(self):
+        return self.condition_state.latest
+
+    @condition.setter
+    def condition(self, condition):
+        assert isinstance(condition, list)
+        self.idl.cond_change(self.name, condition)
+
+    @classmethod
+    def schema_tables(cls, idl, schema):
+        return {k: cls(idl, v) for k, v in schema.tables.items()}
+
+
+class IdlColumn(object):
+    def __init__(self, column):
+        self._column = column
+        self.alert = True
+
+    def __getattr__(self, attr):
+        return getattr(self._column, attr)
 
 
 class Idl(object):
     """Open vSwitch Database Interface Definition Language (OVSDB IDL).
 
     The OVSDB IDL maintains an in-memory replica of a database.  It issues RPC
     requests to an OVSDB database server and parses the responses, converting
@@ -88,75 +230,121 @@
       requested lock, and False otherwise.
 
     - 'txn': The ovs.db.idl.Transaction object for the database transaction
       currently being constructed, if there is one, or None otherwise.
 """
 
     IDL_S_INITIAL = 0
-    IDL_S_MONITOR_REQUESTED = 1
-    IDL_S_MONITOR_COND_REQUESTED = 2
+    IDL_S_SERVER_SCHEMA_REQUESTED = 1
+    IDL_S_SERVER_MONITOR_REQUESTED = 2
+    IDL_S_DATA_MONITOR_REQUESTED = 3
+    IDL_S_DATA_MONITOR_COND_REQUESTED = 4
+    IDL_S_DATA_MONITOR_COND_SINCE_REQUESTED = 5
+    IDL_S_MONITORING = 6
+
+    monitor_map = {
+        Monitor.monitor: IDL_S_SERVER_MONITOR_REQUESTED,
+        Monitor.monitor_cond: IDL_S_DATA_MONITOR_COND_REQUESTED,
+        Monitor.monitor_cond_since: IDL_S_DATA_MONITOR_COND_SINCE_REQUESTED}
 
-    def __init__(self, remote, schema, probe_interval=None):
+    def __init__(self, remote, schema_helper, probe_interval=None,
+                 leader_only=True):
         """Creates and returns a connection to the database named 'db_name' on
         'remote', which should be in a form acceptable to
         ovs.jsonrpc.session.open().  The connection will maintain an in-memory
         replica of the remote database.
 
-        'schema' should be the schema for the remote database.  The caller may
-        have cut it down by removing tables or columns that are not of
-        interest.  The IDL will only replicate the tables and columns that
-        remain.  The caller may also add a attribute named 'alert' to selected
-        remaining columns, setting its value to False; if so, then changes to
-        those columns will not be considered changes to the database for the
-        purpose of the return value of Idl.run() and Idl.change_seqno.  This is
-        useful for columns that the IDL's client will write but not read.
+        'remote' can be comma separated multiple remotes and each remote
+        should be in a form acceptable to ovs.jsonrpc.session.open().
+
+        'schema_helper' should be an instance of the SchemaHelper class which
+        generates schema for the remote database. The caller may have cut it
+        down by removing tables or columns that are not of interest.  The IDL
+        will only replicate the tables and columns that remain.  The caller may
+        also add an attribute named 'alert' to selected remaining columns,
+        setting its value to False; if so, then changes to those columns will
+        not be considered changes to the database for the purpose of the return
+        value of Idl.run() and Idl.change_seqno.  This is useful for columns
+        that the IDL's client will write but not read.
 
         As a convenience to users, 'schema' may also be an instance of the
         SchemaHelper class.
 
         The IDL uses and modifies 'schema' directly.
 
+        If 'leader_only' is set to True (default value) the IDL will only
+        monitor and transact with the leader of the cluster.
+
         If "probe_interval" is zero it disables the connection keepalive
         feature. If non-zero the value will be forced to at least 1000
         milliseconds. If None it will just use the default value in OVS.
         """
 
-        assert isinstance(schema, SchemaHelper)
-        schema = schema.get_idl_schema()
+        assert isinstance(schema_helper, SchemaHelper)
+        schema = schema_helper.get_idl_schema()
 
-        self.tables = schema.tables
+        self.tables = IdlTable.schema_tables(self, schema)
         self.readonly = schema.readonly
         self._db = schema
-        self._session = ovs.jsonrpc.Session.open(remote,
+        remotes = self._parse_remotes(remote)
+        self._session = ovs.jsonrpc.Session.open_multiple(remotes,
             probe_interval=probe_interval)
+        self._request_id = None
         self._monitor_request_id = None
         self._last_seqno = None
         self.change_seqno = 0
         self.uuid = uuid.uuid1()
+        self.last_id = str(uuid.UUID(int=0))
+
+        # Server monitor.
+        self._server_schema_request_id = None
+        self._server_monitor_request_id = None
+        self._db_change_aware_request_id = None
+        self._server_db_name = '_Server'
+        self._server_db_table = 'Database'
+        self.server_tables = None
+        self._server_db = None
+        self.server_monitor_uuid = uuid.uuid1()
+        self.leader_only = leader_only
+        self.cluster_id = None
+        self._min_index = 0
+
         self.state = self.IDL_S_INITIAL
 
         # Database locking.
         self.lock_name = None          # Name of lock we need, None if none.
         self.has_lock = False          # Has db server said we have the lock?
         self.is_lock_contended = False  # Has db server said we can't get lock?
         self._lock_request_id = None   # JSON-RPC ID of in-flight lock request.
 
         # Transaction support.
         self.txn = None
         self._outstanding_txns = {}
 
-        for table in six.itervalues(schema.tables):
-            for column in six.itervalues(table.columns):
-                if not hasattr(column, 'alert'):
-                    column.alert = True
-            table.need_table = False
-            table.rows = custom_index.IndexedRows(table)
-            table.idl = self
-            table.condition = [True]
-            table.cond_changed = False
+        self.cond_changed = False
+        self.cond_seqno = 0
+
+    def _parse_remotes(self, remote):
+        # If remote is -
+        # "tcp:10.0.0.1:6641,unix:/tmp/db.sock,t,s,tcp:10.0.0.2:6642"
+        # this function returns
+        # ["tcp:10.0.0.1:6641", "unix:/tmp/db.sock,t,s", tcp:10.0.0.2:6642"]
+        remotes = []
+        for r in remote.split(','):
+            if remotes and r.find(":") == -1:
+                remotes[-1] += "," + r
+            else:
+                remotes.append(r)
+        return remotes
+
+    def set_cluster_id(self, cluster_id):
+        """Set the id of the cluster that this idl must connect to."""
+        self.cluster_id = cluster_id
+        if self.state != self.IDL_S_INITIAL:
+            self.force_reconnect()
 
     def index_create(self, table, name):
         """Create a named multi-column index on a table"""
         return self.tables[table].rows.index_create(name)
 
     def index_irange(self, table, name, start, end):
         """Return items in a named index between start/end inclusive"""
@@ -167,14 +355,63 @@
         return self.tables[table].rows.indexes[name].irange(value, value)
 
     def close(self):
         """Closes the connection to the database.  The IDL will no longer
         update."""
         self._session.close()
 
+    def ack_conditions(self):
+        """Mark all requested table conditions as acked"""
+        for table in self.tables.values():
+            table.condition_state.ack()
+
+    def sync_conditions(self):
+        """Synchronize condition state when the FSM is restarted
+
+        If a non-zero last_id is available for the DB, then upon reconnect
+        the IDL should first request acked conditions to avoid missing updates
+        about records that were added before the transaction with
+        txn-id == last_id. If there were requested condition changes in flight
+        and the IDL client didn't set new conditions, then reset the requested
+        conditions to new to trigger a follow-up monitor_cond_change request.
+
+        If there were changes in flight then there are two cases:
+        a. either the server already processed the requested monitor condition
+           change but the FSM was restarted before the client was notified.
+           In this case the client should clear its local cache because it's
+           out of sync with the monitor view on the server side.
+
+        b. OR the server hasn't processed the requested monitor condition
+           change yet.
+
+        As there's no easy way to differentiate between the two, and given that
+        this condition should be rare, reset the 'last_id', essentially
+        flushing the local cached DB contents.
+        """
+        ack_all = self.last_id == str(uuid.UUID(int=0))
+        if ack_all:
+            self.cond_changed = False
+
+        for table in self.tables.values():
+            if ack_all:
+                table.condition_state.request()
+                table.condition_state.ack()
+            else:
+                if table.condition_state.reset():
+                    self.last_id = str(uuid.UUID(int=0))
+                    self.cond_changed = True
+
+    def restart_fsm(self):
+        # Resync data DB table conditions to avoid missing updated due to
+        # conditions that were in flight or changed locally while the
+        # connection was down.
+        self.sync_conditions()
+        self.__send_server_schema_request()
+        self.state = self.IDL_S_SERVER_SCHEMA_REQUESTED
+
     def run(self):
         """Processes a batch of messages from the database server.  Returns
         True if the database as seen through the IDL changed, False if it did
         not change.  The initial fetch of the entire contents of the remote
         database is considered to be one kind of change.  If the IDL has been
         configured to acquire a database lock (with Idl.set_lock()), then
         successfully acquiring the lock is also considered to be a change.
@@ -193,58 +430,138 @@
         initial_change_seqno = self.change_seqno
 
         self.send_cond_change()
         self._session.run()
         i = 0
         while i < 50:
             i += 1
+            previous_change_seqno = self.change_seqno
             if not self._session.is_connected():
                 break
 
             seqno = self._session.get_seqno()
             if seqno != self._last_seqno:
                 self._last_seqno = seqno
                 self.__txn_abort_all()
-                self.__send_monitor_request()
+                self.restart_fsm()
                 if self.lock_name:
                     self.__send_lock_request()
                 break
 
             msg = self._session.recv()
             if msg is None:
                 break
+            is_response = msg.type in (ovs.jsonrpc.Message.T_REPLY,
+                                       ovs.jsonrpc.Message.T_ERROR)
+
+            if is_response and self._request_id and self._request_id == msg.id:
+                self._request_id = None
+                # process_response follows
+
             if (msg.type == ovs.jsonrpc.Message.T_NOTIFY
+                    and msg.method == "update3"
+                    and len(msg.params) == 3):
+                # Database contents changed.
+                self.__parse_update(msg.params[2], OVSDB_UPDATE3)
+                self.last_id = msg.params[1]
+            elif (msg.type == ovs.jsonrpc.Message.T_NOTIFY
                     and msg.method == "update2"
                     and len(msg.params) == 2):
                 # Database contents changed.
                 self.__parse_update(msg.params[1], OVSDB_UPDATE2)
             elif (msg.type == ovs.jsonrpc.Message.T_NOTIFY
                     and msg.method == "update"
                     and len(msg.params) == 2):
                 # Database contents changed.
-                self.__parse_update(msg.params[1], OVSDB_UPDATE)
+                if msg.params[0] == str(self.server_monitor_uuid):
+                    self.__parse_update(msg.params[1], OVSDB_UPDATE,
+                                        tables=self.server_tables)
+                    self.change_seqno = previous_change_seqno
+                    if not self.__check_server_db():
+                        self.force_reconnect()
+                        break
+                else:
+                    self.__parse_update(msg.params[1], OVSDB_UPDATE)
             elif (msg.type == ovs.jsonrpc.Message.T_REPLY
                   and self._monitor_request_id is not None
                   and self._monitor_request_id == msg.id):
                 # Reply to our "monitor" request.
                 try:
                     self.change_seqno += 1
                     self._monitor_request_id = None
-                    self.__clear()
-                    if self.state == self.IDL_S_MONITOR_COND_REQUESTED:
+                    if (self.state ==
+                            self.IDL_S_DATA_MONITOR_COND_SINCE_REQUESTED):
+                        # If 'found' is false, clear table rows for new dump
+                        if not msg.result[0]:
+                            self.__clear()
+                        self.__parse_update(msg.result[2], OVSDB_UPDATE3)
+                    elif self.state == self.IDL_S_DATA_MONITOR_COND_REQUESTED:
+                        self.__clear()
                         self.__parse_update(msg.result, OVSDB_UPDATE2)
                     else:
-                        assert self.state == self.IDL_S_MONITOR_REQUESTED
+                        assert self.state == self.IDL_S_DATA_MONITOR_REQUESTED
+                        self.__clear()
                         self.__parse_update(msg.result, OVSDB_UPDATE)
+                    self.state = self.IDL_S_MONITORING
 
                 except error.Error as e:
                     vlog.err("%s: parse error in received schema: %s"
                              % (self._session.get_name(), e))
                     self.__error()
             elif (msg.type == ovs.jsonrpc.Message.T_REPLY
+                  and self._server_schema_request_id is not None
+                  and self._server_schema_request_id == msg.id):
+                # Reply to our "get_schema" of _Server request.
+                try:
+                    self._server_schema_request_id = None
+                    sh = SchemaHelper(None, msg.result)
+                    sh.register_table(self._server_db_table)
+                    schema = sh.get_idl_schema()
+                    self._server_db = schema
+                    self.server_tables = IdlTable.schema_tables(self, schema)
+                    self.__send_server_monitor_request()
+                except error.Error as e:
+                    vlog.err("%s: error receiving server schema: %s"
+                             % (self._session.get_name(), e))
+                    if self.cluster_id:
+                        self.__error()
+                        break
+                    else:
+                        self.change_seqno = previous_change_seqno
+                        self.__send_monitor_request()
+            elif (msg.type == ovs.jsonrpc.Message.T_REPLY
+                  and self._server_monitor_request_id is not None
+                  and self._server_monitor_request_id == msg.id):
+                # Reply to our "monitor" of _Server request.
+                try:
+                    self._server_monitor_request_id = None
+                    self.__parse_update(msg.result, OVSDB_UPDATE,
+                                        tables=self.server_tables)
+                    self.change_seqno = previous_change_seqno
+                    if self.__check_server_db():
+                        self.__send_monitor_request()
+                        self.__send_db_change_aware()
+                    else:
+                        self.force_reconnect()
+                        break
+                except error.Error as e:
+                    vlog.err("%s: parse error in received schema: %s"
+                             % (self._session.get_name(), e))
+                    if self.cluster_id:
+                        self.__error()
+                        break
+                    else:
+                        self.change_seqno = previous_change_seqno
+                        self.__send_monitor_request()
+            elif (msg.type == ovs.jsonrpc.Message.T_REPLY
+                  and self._db_change_aware_request_id is not None
+                  and self._db_change_aware_request_id == msg.id):
+                # Reply to us notifying the server of our change awarness.
+                self._db_change_aware_request_id = None
+            elif (msg.type == ovs.jsonrpc.Message.T_REPLY
                   and self._lock_request_id is not None
                   and self._lock_request_id == msg.id):
                 # Reply to our "lock" request.
                 self.__parse_lock_reply(msg.result)
             elif (msg.type == ovs.jsonrpc.Message.T_NOTIFY
                   and msg.method == "locked"):
                 # We got our lock.
@@ -253,40 +570,85 @@
                   and msg.method == "stolen"):
                 # Someone else stole our lock.
                 self.__parse_lock_notify(msg.params, False)
             elif msg.type == ovs.jsonrpc.Message.T_NOTIFY and msg.id == "echo":
                 # Reply to our echo request.  Ignore it.
                 pass
             elif (msg.type == ovs.jsonrpc.Message.T_ERROR and
-                  self.state == self.IDL_S_MONITOR_COND_REQUESTED and
+                  self.state == (
+                      self.IDL_S_DATA_MONITOR_COND_SINCE_REQUESTED) and
+                      self._monitor_request_id == msg.id):
+                if msg.error == "unknown method":
+                    self.__send_monitor_request(Monitor.monitor_cond)
+            elif (msg.type == ovs.jsonrpc.Message.T_ERROR and
+                  self.state == self.IDL_S_DATA_MONITOR_COND_REQUESTED and
                   self._monitor_request_id == msg.id):
                 if msg.error == "unknown method":
+                    self.__send_monitor_request(Monitor.monitor)
+            elif (msg.type == ovs.jsonrpc.Message.T_ERROR and
+                  self._server_schema_request_id is not None and
+                  self._server_schema_request_id == msg.id):
+                self._server_schema_request_id = None
+                if self.cluster_id:
+                    self.force_reconnect()
+                    break
+                else:
+                    self.change_seqno = previous_change_seqno
                     self.__send_monitor_request()
             elif (msg.type in (ovs.jsonrpc.Message.T_ERROR,
                                ovs.jsonrpc.Message.T_REPLY)
                   and self.__txn_process_reply(msg)):
                 # __txn_process_reply() did everything needed.
                 pass
+            elif (msg.type == ovs.jsonrpc.Message.T_REPLY and
+                  self.state == self.IDL_S_MONITORING):
+                # Mark the last requested conditions as acked and if further
+                # condition changes were pending, send them now.
+                self.ack_conditions()
+                self.send_cond_change()
+                self.cond_seqno += 1
             else:
                 # This can happen if a transaction is destroyed before we
                 # receive the reply, so keep the log level low.
                 vlog.dbg("%s: received unexpected %s message"
                          % (self._session.get_name(),
                              ovs.jsonrpc.Message.type_to_string(msg.type)))
 
         return initial_change_seqno != self.change_seqno
 
+    def compose_cond_change(self):
+        if not self.cond_changed:
+            return
+
+        change_requests = {}
+        for table in self.tables.values():
+            # Always use the most recent conditions set by the IDL client when
+            # requesting monitor_cond_change
+            if table.condition_state.new is not None:
+                change_requests[table.name] = [
+                    {"where": table.condition_state.new}]
+                table.condition_state.request()
+
+        if not change_requests:
+            return
+
+        self.cond_changed = False
+        old_uuid = str(self.uuid)
+        self.uuid = uuid.uuid1()
+        params = [old_uuid, str(self.uuid), change_requests]
+        return ovs.jsonrpc.Message.create_request(
+            "monitor_cond_change", params)
+
     def send_cond_change(self):
-        if not self._session.is_connected():
+        if not self._session.is_connected() or self._request_id is not None:
             return
 
-        for table in six.itervalues(self.tables):
-            if table.cond_changed:
-                self.__send_cond_change(table, table.condition)
-                table.cond_changed = False
+        msg = self.compose_cond_change()
+        if msg:
+            self.send_request(msg)
 
     def cond_change(self, table_name, cond):
         """Sets the condition for 'table_name' to 'cond', which should be a
         conditional expression suitable for use directly in the OVSDB
         protocol, with the exception that the empty condition []
         matches no rows (instead of matching every row).  That is, []
         is equivalent to [False], not to [True].
@@ -294,21 +656,37 @@
 
         table = self.tables.get(table_name)
         if not table:
             raise error.Error('Unknown table "%s"' % table_name)
 
         if cond == []:
             cond = [False]
-        if table.condition != cond:
-            table.condition = cond
-            table.cond_changed = True
+
+        # Compare the new condition to the last known condition
+        if table.condition_state.latest != cond:
+            table.condition_state.init(cond)
+            self.cond_changed = True
+
+        # New condition will be sent out after all already requested ones
+        # are acked.
+        if table.condition_state.new:
+            any_reqs = any(t.condition_state.request
+                           for t in self.tables.values())
+            return self.cond_seqno + int(any_reqs) + 1
+
+        # Already requested conditions should be up to date at
+        # self.cond_seqno + 1 while acked conditions are already up to date
+        return self.cond_seqno + int(bool(table.condition_state.requested))
 
     def wait(self, poller):
         """Arranges for poller.block() to wake up when self.run() has something
         to do or when activity occurs on a transaction on 'self'."""
+        if self.cond_changed:
+            poller.immediate_wake()
+            return
         self._session.wait(poller)
         self._session.recv_wait(poller)
 
     def has_ever_connected(self):
         """Returns True, if the IDL successfully connected to the remote
         database and retrieved its contents (even if the connection
         subsequently dropped and is in the process of reconnecting).  If so,
@@ -318,16 +696,28 @@
         Returns False if the IDL has never connected or retrieved the
         database's contents.  If so, the IDL is empty."""
         return self.change_seqno != 0
 
     def force_reconnect(self):
         """Forces the IDL to drop its connection to the database and reconnect.
         In the meantime, the contents of the IDL will not change."""
+        if self.state == self.IDL_S_MONITORING:
+            # The IDL was in MONITORING state, so we either had data
+            # inconsistency on this server, or it stopped being the cluster
+            # leader, or the user requested to re-connect.  Avoiding backoff
+            # in these cases, as we need to re-connect as soon as possible.
+            # Connections that are not in MONITORING state should have their
+            # backoff to avoid constant flood of re-connection attempts in
+            # case there is no suitable database server.
+            self._session.reset_backoff()
         self._session.force_reconnect()
 
+    def session_name(self):
+        return self._session.get_name()
+
     def set_lock(self, lock_name):
         """If 'lock_name' is not None, configures the IDL to obtain the named
         lock from the database server and to avoid modifying the database when
         the lock cannot be acquired (that is, when another client has the same
         lock).
 
         If 'lock_name' is None, drops the locking requirement and releases the
@@ -354,30 +744,33 @@
         :param row:     The row as it is after the operation has occured
         :type row:      Row
         :param updates: For updates, row with only old values of the changed
                         columns
         :type updates:  Row
         """
 
-    def __send_cond_change(self, table, cond):
-        monitor_cond_change = {table.name: [{"where": cond}]}
-        old_uuid = str(self.uuid)
-        self.uuid = uuid.uuid1()
-        params = [old_uuid, str(self.uuid), monitor_cond_change]
-        msg = ovs.jsonrpc.Message.create_request("monitor_cond_change", params)
-        self._session.send(msg)
+    def cooperative_yield(self):
+        """Hook for cooperatively yielding to eventlet/gevent/asyncio/etc.
+
+        When a block of code is going to spend a lot of time cpu-bound without
+        doing any I/O, it can cause greenthread/coroutine libraries to block.
+        This call should be added to code where this can happen, but defaults
+        to doing nothing to avoid overhead where it is not needed.
+        """
 
     def __clear(self):
         changed = False
 
-        for table in six.itervalues(self.tables):
+        for table in self.tables.values():
             if table.rows:
                 changed = True
                 table.rows = custom_index.IndexedRows(table)
 
+        self.cond_seqno = 0
+
         if changed:
             self.change_seqno += 1
 
     def __update_has_lock(self, new_has_lock):
         if new_has_lock and not self.has_lock:
             if self._monitor_request_id is None:
                 self.change_seqno += 1
@@ -418,102 +811,156 @@
             and isinstance(params, (list, tuple))
             and params
             and params[0] == self.lock_name):
             self.__update_has_lock(new_has_lock)
             if not new_has_lock:
                 self.is_lock_contended = True
 
-    def __send_monitor_request(self):
+    def __send_db_change_aware(self):
+        msg = ovs.jsonrpc.Message.create_request("set_db_change_aware",
+                                                 [True])
+        self._db_change_aware_request_id = msg.id
+        self._session.send(msg)
+
+    def send_request(self, request):
+        self._request_id = request.id
+        if self._session.is_connected():
+            return self._session.send(request)
+
+    def __send_monitor_request(self, max_version=Monitor.monitor_cond_since):
         if self.state == self.IDL_S_INITIAL:
-            self.state = self.IDL_S_MONITOR_COND_REQUESTED
+            self.state = self.IDL_S_DATA_MONITOR_COND_REQUESTED
             method = "monitor_cond"
+        elif self.state == self.IDL_S_SERVER_MONITOR_REQUESTED:
+            self.state = self.monitor_map[Monitor(max_version)]
+            method = Monitor(max_version).name
         else:
-            self.state = self.IDL_S_MONITOR_REQUESTED
+            self.state = self.IDL_S_DATA_MONITOR_REQUESTED
             method = "monitor"
 
         monitor_requests = {}
-        for table in six.itervalues(self.tables):
+        for table in self.tables.values():
             columns = []
-            for column in six.iterkeys(table.columns):
+            for column in table.columns.keys():
                 if ((table.name not in self.readonly) or
                         (table.name in self.readonly) and
                         (column not in self.readonly[table.name])):
                     columns.append(column)
             monitor_request = {"columns": columns}
-            if method == "monitor_cond" and table.condition != [True]:
-                monitor_request["where"] = table.condition
-                table.cond_change = False
+            if method in ("monitor_cond", "monitor_cond_since") and (
+                    not ConditionState.is_true(table.condition_state.acked)):
+                monitor_request["where"] = table.condition_state.acked
             monitor_requests[table.name] = [monitor_request]
 
-        msg = ovs.jsonrpc.Message.create_request(
-            method, [self._db.name, str(self.uuid), monitor_requests])
+        args = [self._db.name, str(self.uuid), monitor_requests]
+        if method == "monitor_cond_since":
+            args.append(str(self.last_id))
+        msg = ovs.jsonrpc.Message.create_request(method, args)
         self._monitor_request_id = msg.id
-        self._session.send(msg)
+        self.send_request(msg)
+
+    def __send_server_schema_request(self):
+        self.state = self.IDL_S_SERVER_SCHEMA_REQUESTED
+        msg = ovs.jsonrpc.Message.create_request(
+            "get_schema", [self._server_db_name, str(self.uuid)])
+        self._server_schema_request_id = msg.id
+        self.send_request(msg)
 
-    def __parse_update(self, update, version):
+    def __send_server_monitor_request(self):
+        self.state = self.IDL_S_SERVER_MONITOR_REQUESTED
+        monitor_requests = {}
+        table = self.server_tables[self._server_db_table]
+        columns = [column for column in table.columns.keys()]
+        for column in table.columns.values():
+            if not hasattr(column, 'alert'):
+                column.alert = True
+        table.rows = custom_index.IndexedRows(table)
+        table.need_table = False
+        table.idl = self
+        monitor_request = {"columns": columns}
+        monitor_requests[table.name] = [monitor_request]
+        msg = ovs.jsonrpc.Message.create_request(
+            'monitor', [self._server_db.name,
+                             str(self.server_monitor_uuid),
+                             monitor_requests])
+        self._server_monitor_request_id = msg.id
+        self.send_request(msg)
+
+    def __parse_update(self, update, version, tables=None):
         try:
-            self.__do_parse_update(update, version)
+            if not tables:
+                self.__do_parse_update(update, version, self.tables)
+            else:
+                self.__do_parse_update(update, version, tables)
         except error.Error as e:
             vlog.err("%s: error parsing update: %s"
                      % (self._session.get_name(), e))
 
-    def __do_parse_update(self, table_updates, version):
+    def __do_parse_update(self, table_updates, version, tables):
         if not isinstance(table_updates, dict):
             raise error.Error("<table-updates> is not an object",
                               table_updates)
 
-        for table_name, table_update in six.iteritems(table_updates):
-            table = self.tables.get(table_name)
+        notices = []
+        for table_name, table_update in table_updates.items():
+            table = tables.get(table_name)
             if not table:
                 raise error.Error('<table-updates> includes unknown '
                                   'table "%s"' % table_name)
 
             if not isinstance(table_update, dict):
                 raise error.Error('<table-update> for table "%s" is not '
                                   'an object' % table_name, table_update)
 
-            for uuid_string, row_update in six.iteritems(table_update):
+            for uuid_string, row_update in table_update.items():
                 if not ovs.ovsuuid.is_valid_string(uuid_string):
                     raise error.Error('<table-update> for table "%s" '
                                       'contains bad UUID "%s" as member '
                                       'name' % (table_name, uuid_string),
                                       table_update)
                 uuid = ovs.ovsuuid.from_string(uuid_string)
 
                 if not isinstance(row_update, dict):
                     raise error.Error('<table-update> for table "%s" '
                                       'contains <row-update> for %s that '
                                       'is not an object'
                                       % (table_name, uuid_string))
 
-                if version == OVSDB_UPDATE2:
-                    if self.__process_update2(table, uuid, row_update):
+                self.cooperative_yield()
+
+                if version in (OVSDB_UPDATE2, OVSDB_UPDATE3):
+                    changes = self.__process_update2(table, uuid, row_update)
+                    if changes:
+                        notices.append(changes)
                         self.change_seqno += 1
                     continue
 
                 parser = ovs.db.parser.Parser(row_update, "row-update")
                 old = parser.get_optional("old", [dict])
                 new = parser.get_optional("new", [dict])
                 parser.finish()
 
                 if not old and not new:
                     raise error.Error('<row-update> missing "old" and '
                                       '"new" members', row_update)
 
-                if self.__process_update(table, uuid, old, new):
+                changes = self.__process_update(table, uuid, old, new)
+                if changes:
+                    notices.append(changes)
                     self.change_seqno += 1
+        for notice in notices:
+            self.notify(*notice)
 
     def __process_update2(self, table, uuid, row_update):
+        """Returns Notice if a column changed, False otherwise."""
         row = table.rows.get(uuid)
-        changed = False
         if "delete" in row_update:
             if row:
                 del table.rows[uuid]
-                self.notify(ROW_DELETE, row)
-                changed = True
+                return Notice(ROW_DELETE, row)
             else:
                 # XXX rate-limit
                 vlog.warn("cannot delete missing row %s from table"
                           "%s" % (uuid, table.name))
         elif "insert" in row_update or "initial" in row_update:
             if row:
                 vlog.warn("cannot add existing row %s from table"
@@ -524,37 +971,35 @@
                 row_update = row_update['insert']
             else:
                 row_update = row_update['initial']
             self.__add_default(table, row_update)
             changed = self.__row_update(table, row, row_update)
             table.rows[uuid] = row
             if changed:
-                self.notify(ROW_CREATE, row)
+                return Notice(ROW_CREATE, row)
         elif "modify" in row_update:
             if not row:
                 raise error.Error('Modify non-existing row')
 
             old_row = self.__apply_diff(table, row, row_update['modify'])
-            self.notify(ROW_UPDATE, row, Row(self, table, uuid, old_row))
-            changed = True
+            return Notice(ROW_UPDATE, row, Row(self, table, uuid, old_row))
         else:
             raise error.Error('<row-update> unknown operation',
                               row_update)
-        return changed
+        return False
 
     def __process_update(self, table, uuid, old, new):
-        """Returns True if a column changed, False otherwise."""
+        """Returns Notice if a column changed, False otherwise."""
         row = table.rows.get(uuid)
         changed = False
         if not new:
             # Delete row.
             if row:
                 del table.rows[uuid]
-                changed = True
-                self.notify(ROW_DELETE, row)
+                return Notice(ROW_DELETE, row)
             else:
                 # XXX rate-limit
                 vlog.warn("cannot delete missing row %s from table %s"
                           % (uuid, table.name))
         elif not old:
             # Insert row.
             op = ROW_CREATE
@@ -566,49 +1011,115 @@
                 op = ROW_UPDATE
                 vlog.warn("cannot add existing row %s to table %s"
                           % (uuid, table.name))
             changed |= self.__row_update(table, row, new)
             if op == ROW_CREATE:
                 table.rows[uuid] = row
             if changed:
-                self.notify(ROW_CREATE, row)
+                return Notice(ROW_CREATE, row)
         else:
             op = ROW_UPDATE
             if not row:
                 row = self.__create_row(table, uuid)
                 changed = True
                 op = ROW_CREATE
                 # XXX rate-limit
                 vlog.warn("cannot modify missing row %s in table %s"
                           % (uuid, table.name))
             changed |= self.__row_update(table, row, new)
             if op == ROW_CREATE:
                 table.rows[uuid] = row
             if changed:
-                self.notify(op, row, Row.from_json(self, table, uuid, old))
-        return changed
+                return Notice(op, row, Row.from_json(self, table, uuid, old))
+        return False
+
+    def __check_server_db(self):
+        """Returns True if this is a valid server database, False otherwise."""
+        session_name = self.session_name()
+
+        if self._server_db_table not in self.server_tables:
+            vlog.info("%s: server does not have %s table in its %s database"
+                      % (session_name, self._server_db_table,
+                         self._server_db_name))
+            return False
+
+        rows = self.server_tables[self._server_db_table].rows
+
+        database = None
+        for row in rows.values():
+            if self.cluster_id:
+                if self.cluster_id in \
+                   map(lambda x: str(x)[:4], row.cid):
+                    database = row
+                    break
+            elif row.name == self._db.name:
+                database = row
+                break
+
+        if not database:
+            vlog.info("%s: server does not have %s database"
+                      % (session_name, self._db.name))
+            return False
+
+        if database.model == CLUSTERED:
+            if not database.schema:
+                vlog.info('%s: clustered database server has not yet joined '
+                          'cluster; trying another server' % session_name)
+                return False
+            if not database.connected:
+                vlog.info('%s: clustered database server is disconnected '
+                          'from cluster; trying another server' % session_name)
+                return False
+            if (self.leader_only and
+                not database.leader):
+                vlog.info('%s: clustered database server is not cluster '
+                          'leader; trying another server' % session_name)
+                return False
+            if database.index:
+                if database.index[0] < self._min_index:
+                    vlog.warn('%s: clustered database server has stale data; '
+                              'trying another server' % session_name)
+                    return False
+                self._min_index = database.index[0]
+        elif database.model == RELAY:
+            if not database.schema:
+                vlog.info('%s: relay database server has not yet connected '
+                          'to the relay source; trying another server'
+                          % session_name)
+                return False
+            if not database.connected:
+                vlog.info('%s: relay database server is disconnected '
+                          'from the relay source; trying another server'
+                          % session_name)
+                return False
+            if self.leader_only:
+                vlog.info('%s: relay database server cannot be a leader; '
+                          'trying another server' % session_name)
+                return False
+
+        return True
 
     def __column_name(self, column):
         if column.type.key.type == ovs.db.types.UuidType:
             return ovs.ovsuuid.to_json(column.type.key.type.default)
         else:
             return column.type.key.type.default
 
     def __add_default(self, table, row_update):
-        for column in six.itervalues(table.columns):
+        for column in table.columns.values():
             if column.name not in row_update:
                 if ((table.name not in self.readonly) or
                         (table.name in self.readonly) and
                         (column.name not in self.readonly[table.name])):
                     if column.type.n_min != 0 and not column.type.is_map():
                         row_update[column.name] = self.__column_name(column)
 
     def __apply_diff(self, table, row, row_diff):
         old_row = {}
-        for column_name, datum_diff_json in six.iteritems(row_diff):
+        for column_name, datum_diff_json in row_diff.items():
             column = table.columns.get(column_name)
             if not column:
                 # XXX rate-limit
                 vlog.warn("unknown column %s updating table %s"
                           % (column_name, table.name))
                 continue
 
@@ -625,15 +1136,15 @@
             if datum != row._data[column_name]:
                 row._data[column_name] = datum
 
         return old_row
 
     def __row_update(self, table, row, row_json):
         changed = False
-        for column_name, datum_json in six.iteritems(row_json):
+        for column_name, datum_json in row_json.items():
             column = table.columns.get(column_name)
             if not column:
                 # XXX rate-limit
                 vlog.warn("unknown column %s updating table %s"
                           % (column_name, table.name))
                 continue
 
@@ -652,18 +1163,15 @@
             else:
                 # Didn't really change but the OVSDB monitor protocol always
                 # includes every value in a row.
                 pass
         return changed
 
     def __create_row(self, table, uuid):
-        data = {}
-        for column in six.itervalues(table.columns):
-            data[column.name] = ovs.db.data.Datum.default(column.type)
-        return Row(self, table, uuid, data)
+        return Row(self, table, uuid, ColumnDefaultDict(table))
 
     def __error(self):
         self._session.force_reconnect()
 
     def __txn_abort_all(self):
         while self._outstanding_txns:
             txn = self._outstanding_txns.popitem()[1]
@@ -672,21 +1180,14 @@
     def __txn_process_reply(self, msg):
         txn = self._outstanding_txns.pop(msg.id, None)
         if txn:
             txn._process_reply(msg)
             return True
 
 
-def _uuid_to_row(atom, base):
-    if base.ref_table:
-        return base.ref_table.rows.get(atom)
-    else:
-        return atom
-
-
 def _row_to_uuid(value):
     if isinstance(value, Row):
         return value.uuid
     else:
         return value
 
 
@@ -786,14 +1287,31 @@
         if not isinstance(other, Row):
             return NotImplemented
         return bool(self.__dict__['uuid'] == other.__dict__['uuid'])
 
     def __hash__(self):
         return int(self.__dict__['uuid'])
 
+    def __str__(self):
+        return "{table}({data})".format(
+            table=self._table.name,
+            data=", ".join("{col}={val}".format(col=c, val=getattr(self, c))
+                           for c in sorted(self._table.columns)))
+
+    def _uuid_to_row(self, atom, base):
+        if base.ref_table:
+            try:
+                table = self._idl.tables[base.ref_table.name]
+            except KeyError as e:
+                msg = "Table {} is not registered".format(base.ref_table.name)
+                raise AttributeError(msg) from e
+            return table.rows.get(atom)
+        else:
+            return atom
+
     def __getattr__(self, column_name):
         assert self._changes is not None
         assert self._mutations is not None
 
         try:
             column = self._table.columns[column_name]
         except KeyError:
@@ -827,15 +1345,15 @@
                                                               removes,
                                                               _row_to_uuid)
                         removes_list = removes_datum.as_list()
                         dlist = [x for x in dlist if x not in removes_list]
                     datum = data.Datum.from_python(column.type, dlist,
                                                    _row_to_uuid)
                 elif column.type.is_map():
-                    dmap = datum.to_python(_uuid_to_row)
+                    dmap = datum.to_python(self._uuid_to_row)
                     if inserts is not None:
                         dmap.update(inserts)
                     if removes is not None:
                         for key in removes:
                             if key not in (inserts or {}):
                                 dmap.pop(key, None)
                     datum = data.Datum.from_python(column.type, dmap,
@@ -844,15 +1362,15 @@
                 if inserts is None:
                     raise AttributeError("%s instance has no attribute '%s'" %
                                          (self.__class__.__name__,
                                           column_name))
                 else:
                     datum = inserts
 
-        return datum.to_python(_uuid_to_row)
+        return datum.to_python(self._uuid_to_row)
 
     def __setattr__(self, column_name, value):
         assert self._changes is not None
         assert self._idl.txn
 
         if ((self._table.name in self._idl.readonly) and
                 (column_name in self._idl.readonly[self._table.name])):
@@ -928,30 +1446,30 @@
         column_value[key] = value
 
     def delkey(self, column_name, key, value=None):
         self._idl.txn._txn_rows[self.uuid] = self
         if value:
             try:
                 old_value = data.Datum.to_python(self._data[column_name],
-                                                 _uuid_to_row)
+                                                 self._uuid_to_row)
             except error.Error:
                 return
             if key not in old_value:
                 return
             if old_value[key] != value:
                 return
         removes = self._mutations.setdefault('_removes', {})
         column_value = removes.setdefault(column_name, set())
         column_value.add(key)
         return
 
     @classmethod
     def from_json(cls, idl, table, uuid, row_json):
         data = {}
-        for column_name, datum_json in six.iteritems(row_json):
+        for column_name, datum_json in row_json.items():
             column = table.columns.get(column_name)
             if not column:
                 # XXX rate-limit
                 vlog.warn("unknown column %s in table %s"
                           % (column_name, table.name))
                 continue
             try:
@@ -987,15 +1505,15 @@
 
         Because of the latter property, always call Row.verify() *before*
         modifying the column, for a given read-modify-write.
 
         A transaction must be in progress."""
         assert self._idl.txn
         assert self._changes is not None
-        if not self._data or column_name in self._changes:
+        if self._data is None or column_name in self._changes:
             return
 
         self._prereqs[column_name] = None
 
     def delete(self):
         """Deletes this row from its table.
 
@@ -1173,15 +1691,15 @@
             else:
                 return [self._substitute_uuids(elem) for elem in json]
         return json
 
     def __disassemble(self):
         self.idl.txn = None
 
-        for row in six.itervalues(self._txn_rows):
+        for row in self._txn_rows.values():
             if row._changes is None:
                 # If we add the deleted row back to rows with _changes == None
                 # then __getattr__ will not work for the indexes
                 row.__dict__["_changes"] = {}
                 row.__dict__["_mutations"] = {}
                 row._table.rows[row.uuid] = row
             elif row._data is None:
@@ -1243,29 +1761,34 @@
         successfully, then the database server will send an update and, thus,
         the IDL will be updated with the committed changes."""
         # The status can only change if we're the active transaction.
         # (Otherwise, our status will change only in Idl.run().)
         if self != self.idl.txn:
             return self._status
 
+        if self.idl.state != Idl.IDL_S_MONITORING:
+            self._status = Transaction.TRY_AGAIN
+            self.__disassemble()
+            return self._status
+
         # If we need a lock but don't have it, give up quickly.
         if self.idl.lock_name and not self.idl.has_lock:
             self._status = Transaction.NOT_LOCKED
             self.__disassemble()
             return self._status
 
         operations = [self.idl._db.name]
 
         # Assert that we have the required lock (avoiding a race).
         if self.idl.lock_name:
             operations.append({"op": "assert",
                                "lock": self.idl.lock_name})
 
         # Add prerequisites and declarations of new rows.
-        for row in six.itervalues(self._txn_rows):
+        for row in self._txn_rows.values():
             if row._prereqs:
                 rows = {}
                 columns = []
                 for column_name in row._prereqs:
                     columns.append(column_name)
                     rows[column_name] = row._data[column_name].to_json()
                 operations.append({"op": "wait",
@@ -1274,15 +1797,15 @@
                                    "where": _where_uuid_equals(row.uuid),
                                    "until": "==",
                                    "columns": columns,
                                    "rows": [rows]})
 
         # Add updates.
         any_updates = False
-        for row in six.itervalues(self._txn_rows):
+        for row in self._txn_rows.values():
             if row._changes is None:
                 if row._table.is_root:
                     operations.append({"op": "delete",
                                        "table": row._table.name,
                                        "where": _where_uuid_equals(row.uuid)})
                     any_updates = True
                 else:
@@ -1300,15 +1823,15 @@
                 else:
                     op["op"] = "update"
                     op["where"] = _where_uuid_equals(row.uuid)
 
                 row_json = {}
                 op["row"] = row_json
 
-                for column_name, datum in six.iteritems(row._changes):
+                for column_name, datum in row._changes.items():
                     if row._data is not None or not datum.is_default():
                         row_json[column_name] = (
                             self._substitute_uuids(datum.to_json()))
 
                         # If anything really changed, consider it an update.
                         # We can't suppress not-really-changed values earlier
                         # or transactions would become nonatomic (see the big
@@ -1328,15 +1851,15 @@
                     op["where"] = self._substitute_uuids(
                         _where_uuid_equals(row.uuid))
                 else:
                     # Existing row
                     op["where"] = _where_uuid_equals(row.uuid)
                 op["mutations"] = []
                 if '_removes' in row._mutations.keys():
-                    for col, dat in six.iteritems(row._mutations['_removes']):
+                    for col, dat in row._mutations['_removes'].items():
                         column = row._table.columns[col]
                         if column.type.is_map():
                             opdat = ["set"]
                             opdat.append(list(dat))
                         else:
                             opdat = ["set"]
                             inner_opdat = []
@@ -1349,21 +1872,20 @@
                                 inner_opdat.append(
                                     self._substitute_uuids(datum.to_json()))
                             opdat.append(inner_opdat)
                         mutation = [col, "delete", opdat]
                         op["mutations"].append(mutation)
                         addop = True
                 if '_inserts' in row._mutations.keys():
-                    for col, val in six.iteritems(row._mutations['_inserts']):
+                    for col, val in row._mutations['_inserts'].items():
                         column = row._table.columns[col]
                         if column.type.is_map():
-                            opdat = ["map"]
                             datum = data.Datum.from_python(column.type, val,
                                                            _row_to_uuid)
-                            opdat.append(datum.as_list())
+                            opdat = self._substitute_uuids(datum.to_json())
                         else:
                             opdat = ["set"]
                             inner_opdat = []
                             for ele in val:
                                 try:
                                     datum = data.Datum.from_python(column.type,
                                         ele, _row_to_uuid)
@@ -1516,15 +2038,15 @@
         #
         # We don't do this for read/write columns because that would break
         # atomicity of transactions--some other client might have written a
         # different value in that column since we read it.  (But if a whole
         # transaction only does writes of existing values, without making any
         # real changes, we will drop the whole transaction later in
         # ovsdb_idl_txn_commit().)
-        if (not column.alert and row._data and
+        if (not column.alert and row._data is not None and
                 row._data.get(column.name) == datum):
             new_value = row._changes.get(column.name)
             if new_value is None or new_value == datum:
                 return
 
         txn._txn_rows[row.uuid] = row
         if '_inserts' in row._mutations:
@@ -1592,15 +2114,15 @@
                     hard_errors = True
                 if self._fetch_requests:
                     if self.__process_fetch_reply(ops):
                         self.idl.change_seqno += 1
                     else:
                         hard_errors = True
 
-                for insert in six.itervalues(self._inserted_rows):
+                for insert in self._inserted_rows.values():
                     if not self.__process_insert_reply(insert, ops):
                         hard_errors = True
 
             if hard_errors:
                 self._status = Transaction.ERROR
             elif lock_errors:
                 self._status = Transaction.NOT_LOCKED
@@ -1661,15 +2183,15 @@
                       "increment (has %d, needs %d)" %
                       (len(ops), self._inc_index + 2))
 
         # We know that this is a JSON object because the loop in
         # __process_reply() already checked.
         mutate = ops[self._inc_index]
         count = mutate.get("count")
-        if not Transaction.__check_json_type(count, six.integer_types,
+        if not Transaction.__check_json_type(count, (int,),
                                              '"mutate" reply "count"'):
             return False
         if count != 1:
             # XXX rate-limit
             vlog.warn('"mutate" reply "count" is %d instead of 1' % count)
             return False
 
@@ -1684,15 +2206,15 @@
                       'instead of 1' % len(rows))
             return False
         row = rows[0]
         if not Transaction.__check_json_type(row, (dict,),
                                              '"select" reply row'):
             return False
         column = row.get(self._inc_column)
-        if not Transaction.__check_json_type(column, six.integer_types,
+        if not Transaction.__check_json_type(column, (int,),
                                              '"select" reply inc column'):
             return False
         self._inc_new_value = column
         return True
 
     def __process_insert_reply(self, insert, ops):
         if insert.op_index >= len(ops):
@@ -1762,28 +2284,28 @@
         with Row.fetch().
 
         'table' must be a string.
         'columns' must be a list of strings.
         'readonly' must be a list of strings.
         """
 
-        assert isinstance(table, six.string_types)
+        assert isinstance(table, str)
         assert isinstance(columns, list)
 
         columns = set(columns) | self._tables.get(table, set())
         self._tables[table] = columns
         self._readonly[table] = readonly
 
     def register_table(self, table):
         """Registers interest in the given all columns of 'table'. Future calls
         to get_idl_schema() will include all columns of 'table'.
 
         'table' must be a string
         """
-        assert isinstance(table, six.string_types)
+        assert isinstance(table, str)
         self._tables[table] = set()  # empty set means all columns in the table
 
     def register_all(self):
         """Registers interest in every column of every table."""
         self._all = True
 
     def get_idl_schema(self):
@@ -1792,15 +2314,15 @@
         function."""
 
         schema = ovs.db.schema.DbSchema.from_json(self.schema_json)
         self.schema_json = None
 
         if not self._all:
             schema_tables = {}
-            for table, columns in six.iteritems(self._tables):
+            for table, columns in self._tables.items():
                 schema_tables[table] = (
                     self._keep_table_columns(schema, table, columns))
 
             schema.tables = schema_tables
         schema.readonly = self._readonly
         return schema
 
@@ -1810,14 +2332,14 @@
 
         if not columns:
             # empty set means all columns in the table
             return table
 
         new_columns = {}
         for column_name in columns:
-            assert isinstance(column_name, six.string_types)
+            assert isinstance(column_name, str)
             assert column_name in table.columns
 
             new_columns[column_name] = table.columns[column_name]
 
         table.columns = new_columns
         return table
```

### Comparing `ovs-2.9.4/ovs/db/parser.py` & `ovs-3.0.0/ovs/db/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 
 from ovs.db import error
 
-import six
-
 
 class Parser(object):
     def __init__(self, json, name):
         self.name = name
         self.json = json
         if not isinstance(json, dict):
             self.__raise_error("Object expected.")
@@ -77,32 +75,32 @@
     return x
 
 
 id_re = re.compile("[_a-zA-Z][_a-zA-Z0-9]*$")
 
 
 def is_identifier(s):
-    return isinstance(s, six.string_types) and id_re.match(s)
+    return isinstance(s, str) and id_re.match(s)
 
 
 def json_type_to_string(type_):
-    number_types = list(six.integer_types)
+    number_types = [int]
     number_types.extend([float])
     number_types = tuple(number_types)
     if type_ is None:
         return "null"
     elif issubclass(type_, bool):
         return "boolean"
     elif issubclass(type_, dict):
         return "object"
     elif issubclass(type_, list):
         return "array"
     elif issubclass(type_, number_types):
         return "number"
-    elif issubclass(type_, six.string_types):
+    elif issubclass(type_, str):
         return "string"
     else:
         return "<invalid>"
 
 
 def unwrap_json(json, name, types, desc):
     if (not isinstance(json, (list, tuple))
```

### Comparing `ovs-2.9.4/ovs/db/schema.py` & `ovs-3.0.0/ovs/db/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 import re
 import sys
 
 import ovs.db.parser
 import ovs.db.types
 from ovs.db import error
 
-import six
-
 
 def _check_id(name, json):
     if name.startswith('_'):
         raise error.Error('names beginning with "_" are reserved', json)
     elif not ovs.db.parser.is_identifier(name):
         raise error.Error("name must be a valid id", json)
 
@@ -38,66 +36,66 @@
         self.tables = tables
 
         # "isRoot" was not part of the original schema definition.  Before it
         # was added, there was no support for garbage collection.  So, for
         # backward compatibility, if the root set is empty then assume that
         # every table is in the root set.
         if self.__root_set_size() == 0:
-            for table in six.itervalues(self.tables):
+            for table in self.tables.values():
                 table.is_root = True
 
         # Find the "ref_table"s referenced by "ref_table_name"s.
         #
         # Also force certain columns to be persistent, as explained in
         # __check_ref_table().  This requires 'is_root' to be known, so this
         # must follow the loop updating 'is_root' above.
-        for table in six.itervalues(self.tables):
-            for column in six.itervalues(table.columns):
+        for table in self.tables.values():
+            for column in table.columns.values():
                 self.__follow_ref_table(column, column.type.key, "key")
                 self.__follow_ref_table(column, column.type.value, "value")
 
     def __root_set_size(self):
         """Returns the number of tables in the schema's root set."""
         n_root = 0
-        for table in six.itervalues(self.tables):
+        for table in self.tables.values():
             if table.is_root:
                 n_root += 1
         return n_root
 
     @staticmethod
     def from_json(json, allow_extensions=False):
         parser = ovs.db.parser.Parser(json, "database schema")
         name = parser.get("name", ['id'])
-        version = parser.get_optional("version", six.string_types)
-        parser.get_optional("cksum", six.string_types)
+        version = parser.get_optional("version", (str,))
+        parser.get_optional("cksum", (str,))
         tablesJson = parser.get("tables", [dict])
         parser.finish()
 
         if (version is not None and
-            not re.match('[0-9]+\.[0-9]+\.[0-9]+$', version)):
+            not re.match(r'[0-9]+\.[0-9]+\.[0-9]+$', version)):
             raise error.Error('schema version "%s" not in format x.y.z'
                               % version)
 
         tables = {}
-        for tableName, tableJson in six.iteritems(tablesJson):
+        for tableName, tableJson in tablesJson.items():
             _check_id(tableName, json)
             tables[tableName] = TableSchema.from_json(tableJson, tableName,
                                                       allow_extensions)
 
         return DbSchema(name, version, tables)
 
     def to_json(self):
         # "isRoot" was not part of the original schema definition.  Before it
         # was added, there was no support for garbage collection.  So, for
         # backward compatibility, if every table is in the root set then do not
         # output "isRoot" in table schemas.
         default_is_root = self.__root_set_size() == len(self.tables)
 
         tables = {}
-        for table in six.itervalues(self.tables):
+        for table in self.tables.values():
             tables[table.name] = table.to_json(default_is_root)
         json = {"name": self.name, "tables": tables}
         if self.version:
             json["version"] = self.version
         return json
 
     def copy(self):
@@ -133,18 +131,18 @@
         self.idlHeader = idlHeader
         self.cDecls = cDecls
         self.hDecls = hDecls
 
     @staticmethod
     def from_json(json):
         parser = ovs.db.parser.Parser(json, "IDL schema")
-        idlPrefix = parser.get("idlPrefix", six.string_types)
-        idlHeader = parser.get("idlHeader", six.string_types)
-        cDecls = parser.get_optional("cDecls", six.string_types, "")
-        hDecls = parser.get_optional("hDecls", six.string_types, "")
+        idlPrefix = parser.get("idlPrefix", (str,))
+        idlHeader = parser.get("idlHeader", (str,))
+        cDecls = parser.get_optional("cDecls", (str,), "")
+        hDecls = parser.get_optional("hDecls", (str,), "")
 
         subjson = dict(json)
         del subjson["idlPrefix"]
         del subjson["idlHeader"]
         subjson.pop("cDecls", None)
         subjson.pop("hDecls", None)
         schema = DbSchema.from_json(subjson, allow_extensions=True)
@@ -156,15 +154,15 @@
 def column_set_from_json(json, columns):
     if json is None:
         return tuple(columns)
     elif not isinstance(json, list):
         raise error.Error("array of distinct column names expected", json)
     else:
         for column_name in json:
-            if not isinstance(column_name, six.string_types):
+            if not isinstance(column_name, str):
                 raise error.Error("array of distinct column names expected",
                                   json)
             elif column_name not in columns:
                 raise error.Error("%s is not a valid column name"
                                   % column_name, json)
         if len(set(json)) != len(json):
             # Duplicate.
@@ -202,15 +200,15 @@
         elif max_rows <= 0:
             raise error.Error("maxRows must be at least 1", json)
 
         if not columns_json:
             raise error.Error("table must have at least one column", json)
 
         columns = {}
-        for column_name, column_json in six.iteritems(columns_json):
+        for column_name, column_json in columns_json.items():
             _check_id(column_name, json)
             columns[column_name] = ColumnSchema.from_json(column_json,
                                                           column_name,
                                                           allow_extensions)
 
         indexes = []
         for index_json in indexes_json:
@@ -243,15 +241,15 @@
         json = {}
         if not self.mutable:
             json["mutable"] = False
         if default_is_root != self.is_root:
             json["isRoot"] = self.is_root
 
         json["columns"] = columns = {}
-        for column in six.itervalues(self.columns):
+        for column in self.columns.values():
             if not column.name.startswith("_"):
                 columns[column.name] = column.to_json()
 
         if self.max_rows != sys.maxsize:
             json["maxRows"] = self.max_rows
 
         if self.indexes:
@@ -272,15 +270,15 @@
         self.extensions = extensions
 
     @staticmethod
     def from_json(json, name, allow_extensions=False):
         parser = ovs.db.parser.Parser(json, "schema for column %s" % name)
         mutable = parser.get_optional("mutable", [bool], True)
         ephemeral = parser.get_optional("ephemeral", [bool], False)
-        _types = list(six.string_types)
+        _types = [str]
         _types.extend([dict])
         type_ = ovs.db.types.Type.from_json(parser.get("type", _types))
         if allow_extensions:
             extensions = parser.get_optional("extensions", [dict], {})
         else:
             extensions = {}
         parser.finish()
```

### Comparing `ovs-2.9.4/ovs/db/types.py` & `ovs-3.0.0/ovs/db/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 import uuid
 
 import ovs.db.data
 import ovs.db.parser
 import ovs.ovsuuid
 from ovs.db import error
 
-import six
-
 
 class AtomicType(object):
     def __init__(self, name, default, python_types):
         self.name = name
         self.default = default
         self.python_types = python_types
 
@@ -35,41 +33,51 @@
             for atomic_type in ATOMIC_TYPES:
                 if s == atomic_type.name:
                     return atomic_type
         raise error.Error('"%s" is not an atomic-type' % s, s)
 
     @staticmethod
     def from_json(json):
-        if not isinstance(json, six.string_types):
+        if not isinstance(json, str):
             raise error.Error("atomic-type expected", json)
         else:
             return AtomicType.from_string(json)
 
     def __str__(self):
         return self.name
 
     def to_string(self):
         return self.name
 
+    def to_rvalue_string(self):
+        if self == StringType:
+            return 's->' + self.name
+        return self.name
+
+    def to_lvalue_string(self):
+        if self == StringType:
+            return 's'
+        return self.name
+
     def to_json(self):
         return self.name
 
     def default_atom(self):
         return ovs.db.data.Atom(self, self.default)
 
 
-REAL_PYTHON_TYPES = list(six.integer_types)
+REAL_PYTHON_TYPES = [int]
 REAL_PYTHON_TYPES.extend([float])
 REAL_PYTHON_TYPES = tuple(REAL_PYTHON_TYPES)
 
 VoidType = AtomicType("void", None, ())
-IntegerType = AtomicType("integer", 0, six.integer_types)
+IntegerType = AtomicType("integer", 0, (int,))
 RealType = AtomicType("real", 0.0, REAL_PYTHON_TYPES)
 BooleanType = AtomicType("boolean", False, (bool,))
-StringType = AtomicType("string", "", six.string_types)
+StringType = AtomicType("string", "", (str,))
 UuidType = AtomicType("uuid", ovs.ovsuuid.zero(), (uuid.UUID,))
 
 ATOMIC_TYPES = [VoidType, IntegerType, RealType, BooleanType, StringType,
                 UuidType]
 
 
 def escapeCString(src):
@@ -151,42 +159,41 @@
         if not isinstance(other, BaseType):
             return NotImplemented
         else:
             return not (self == other)
 
     @staticmethod
     def __parse_uint(parser, name, default):
-        value = parser.get_optional(name, six.integer_types)
+        value = parser.get_optional(name, (int,))
         if value is None:
             value = default
         else:
             max_value = 2 ** 32 - 1
             if not (0 <= value <= max_value):
                 raise error.Error("%s out of valid range 0 to %d"
                                   % (name, max_value), value)
         return value
 
     @staticmethod
     def from_json(json):
-        if isinstance(json, six.string_types):
+        if isinstance(json, str):
             return BaseType(AtomicType.from_json(json))
 
         parser = ovs.db.parser.Parser(json, "ovsdb type")
-        atomic_type = AtomicType.from_json(parser.get("type",
-                                                      six.string_types))
+        atomic_type = AtomicType.from_json(parser.get("type", (str,)))
 
         base = BaseType(atomic_type)
 
         enum = parser.get_optional("enum", [])
         if enum is not None:
             base.enum = ovs.db.data.Datum.from_json(
                     BaseType.get_enum_type(base.type), enum)
         elif base.type == IntegerType:
-            base.min = parser.get_optional("minInteger", six.integer_types)
-            base.max = parser.get_optional("maxInteger", six.integer_types)
+            base.min = parser.get_optional("minInteger", (int,))
+            base.max = parser.get_optional("maxInteger", (int,))
             if (base.min is not None and base.max is not None
                     and base.min > base.max):
                 raise error.Error("minInteger exceeds maxInteger", json)
         elif base.type == RealType:
             base.min = parser.get_optional("minReal", REAL_PYTHON_TYPES)
             base.max = parser.get_optional("maxReal", REAL_PYTHON_TYPES)
             if (base.min is not None and base.max is not None
@@ -198,15 +205,15 @@
                                                     sys.maxsize)
             if base.min_length > base.max_length:
                 raise error.Error("minLength exceeds maxLength", json)
         elif base.type == UuidType:
             base.ref_table_name = parser.get_optional("refTable", ['id'])
             if base.ref_table_name:
                 base.ref_type = parser.get_optional("refType",
-                                                    six.string_types,
+                                                    (str,),
                                                    "strong")
                 if base.ref_type not in ['strong', 'weak']:
                     raise error.Error('refType must be "strong" or "weak" '
                                       '(not "%s")' % base.ref_type)
         parser.finish()
 
         return base
@@ -372,26 +379,15 @@
     def copyCValue(self, dst, src, refTable=True):
         args = {'dst': dst, 'src': src}
         if self.ref_table_name:
             if not refTable:
                 return "%(dst)s = *%(src)s;" % args
             return ("%(dst)s = %(src)s->header_.uuid;") % args
         elif self.type == StringType:
-            return "%(dst)s = xstrdup(%(src)s);" % args
-        else:
-            return "%(dst)s = %(src)s;" % args
-
-    def assign_c_value_casting_away_const(self, dst, src, refTable=True):
-        args = {'dst': dst, 'src': src}
-        if self.ref_table_name:
-            if not refTable:
-                return "%(dst)s = *%(src)s;" % args
-            return ("%(dst)s = %(src)s->header_.uuid;") % args
-        elif self.type == StringType:
-            return "%(dst)s = CONST_CAST(char *, %(src)s);" % args
+            return "%(dst)s = ovsdb_atom_string_create(%(src)s);" % args
         else:
             return "%(dst)s = %(src)s;" % args
 
     def initCDefault(self, var, is_optional):
         if self.ref_table_name:
             return "%s = NULL;" % var
         elif self.type == StringType and not is_optional:
@@ -415,39 +411,39 @@
                 low = "INT64_MIN"
             else:
                 low = "INT64_C(%d)" % self.min
             if self.max is None:
                 high = "INT64_MAX"
             else:
                 high = "INT64_C(%d)" % self.max
-            init.append(".u.integer = { .min = %s, .max = %s }," % (low, high))
+            init.append(".integer = { .min = %s, .max = %s }," % (low, high))
         elif self.type == RealType:
             if self.min is None:
                 low = "-DBL_MAX"
             else:
                 low = self.min
             if self.max is None:
                 high = "DBL_MAX"
             else:
                 high = self.max
-            init.append(".u.real = { .min = %s, .max = %s }," % (low, high))
+            init.append(".real = { .min = %s, .max = %s }," % (low, high))
         elif self.type == StringType:
             if self.min is None:
                 low = 0
             else:
                 low = self.min_length
             if self.max is None:
                 high = "UINT_MAX"
             else:
                 high = self.max_length
-            init.append(".u.string = { .minLen = %s, .maxLen = %s }," % (
+            init.append(".string = { .minLen = %s, .maxLen = %s }," % (
                 low, high))
         elif self.type == UuidType:
             if self.ref_table_name is not None:
-                init.append(".u.uuid = { .refTableName = \"%s\", "
+                init.append(".uuid = { .refTableName = \"%s\", "
                             ".refType = OVSDB_REF_%s }," % (
                                 escapeCString(self.ref_table_name),
                                 self.ref_type.upper()))
         return init
 
 
 class Type(object):
@@ -516,24 +512,24 @@
         elif isinstance(json, int) and 0 <= json <= sys.maxsize:
             return json
         else:
             raise error.Error("bad min or max value", json)
 
     @staticmethod
     def from_json(json):
-        if isinstance(json, six.string_types):
+        if isinstance(json, str):
             return Type(BaseType.from_json(json))
 
         parser = ovs.db.parser.Parser(json, "ovsdb type")
-        _types = list(six.string_types)
+        _types = [str]
         _types.extend([dict])
         key_json = parser.get("key", _types)
         value_json = parser.get_optional("value", _types)
         min_json = parser.get_optional("min", [int])
-        _types = list(six.string_types)
+        _types = [str]
         _types.extend([int])
         max_json = parser.get_optional("max", _types)
         parser.finish()
 
         key = BaseType.from_json(key_json)
         if value_json:
             value = BaseType.from_json(value_json)
@@ -590,15 +586,24 @@
                                           commafy(self.n_max))
             else:
                 quantity = "up to %s " % commafy(self.n_max)
 
             if self.value:
                 return "map of %s%s-%s pairs" % (quantity, keyName, valueName)
             else:
-                if keyName.endswith('s'):
+                # Extract the last word from 'keyName' so we can make it
+                # plural.  For linguistic analysis, turn it into English
+                # without formatting so that we don't consider any prefix or
+                # suffix added by escapeLiteral.
+                plainKeyName = (self.key.toEnglish(returnUnchanged)
+                                .rpartition(' ')[2].lower())
+
+                if plainKeyName == 'chassis':
+                    plural = keyName
+                elif plainKeyName.endswith('s'):
                     plural = keyName + "es"
                 else:
                     plural = keyName + "s"
                 return "set of %s%s" % (quantity, plural)
 
     def constraintsToEnglish(self, escapeLiteral=returnUnchanged,
                              escapeNumber=returnUnchanged):
```

### Comparing `ovs-2.9.4/ovs/unixctl/__init__.py` & `ovs-3.0.0/ovs/unixctl/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 import ovs.util
 
-import six
-
 commands = {}
-strtypes = six.string_types
 
 
 class _UnixctlCommand(object):
     def __init__(self, usage, min_args, max_args, callback, aux):
         self.usage = usage
         self.min_args = min_args
         self.max_args = max_args
@@ -55,29 +52,29 @@
     'aux'.  Normally 'callback' should reply by calling
     UnixctlConnection.reply() or UnixctlConnection.reply_error() before it
     returns, but if the command cannot be handled immediately, then it can
     defer the reply until later.  A given connection can only process a single
     request at a time, so a reply must be made eventually to avoid blocking
     that connection."""
 
-    assert isinstance(name, strtypes)
-    assert isinstance(usage, strtypes)
+    assert isinstance(name, str)
+    assert isinstance(usage, str)
     assert isinstance(min_args, int)
     assert isinstance(max_args, int)
     assert callable(callback)
 
     if name not in commands:
         commands[name] = _UnixctlCommand(usage, min_args, max_args, callback,
                                          aux)
 
 
 def socket_name_from_target(target):
-    assert isinstance(target, strtypes)
+    assert isinstance(target, str)
 
-    """ On Windows an absolute path contains ':' ( i.e: C:\ ) """
+    """ On Windows an absolute path contains ':' ( i.e: C:\\ ) """
     if target.startswith('/') or target.find(':') > -1:
         return 0, target
 
     pidfile_name = "%s/%s.pid" % (ovs.dirs.RUNDIR, target)
     pid = ovs.daemon.read_pidfile(pidfile_name)
     if pid < 0:
         return -pid, "cannot read pidfile \"%s\"" % pidfile_name
```

### Comparing `ovs-2.9.4/ovs/unixctl/client.py` & `ovs-3.0.0/ovs/unixctl/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,30 +14,27 @@
 
 import os
 
 import ovs.jsonrpc
 import ovs.stream
 import ovs.util
 
-import six
-
 vlog = ovs.vlog.Vlog("unixctl_client")
-strtypes = six.string_types
 
 
 class UnixctlClient(object):
     def __init__(self, conn):
         assert isinstance(conn, ovs.jsonrpc.Connection)
         self._conn = conn
 
     def transact(self, command, argv):
-        assert isinstance(command, strtypes)
+        assert isinstance(command, str)
         assert isinstance(argv, list)
         for arg in argv:
-            assert isinstance(arg, strtypes)
+            assert isinstance(arg, str)
 
         request = ovs.jsonrpc.Message.create_request(command, argv)
         error, reply = self._conn.transact_block(request)
 
         if error:
             vlog.warn("error communicating with %s: %s"
                       % (self._conn.name, os.strerror(error)))
```

### Comparing `ovs-2.9.4/ovs/unixctl/server.py` & `ovs-3.0.0/ovs/unixctl/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,17 @@
 import ovs.jsonrpc
 import ovs.stream
 import ovs.unixctl
 import ovs.util
 import ovs.version
 import ovs.vlog
 
-import six
-from six.moves import range
 
 Message = ovs.jsonrpc.Message
 vlog = ovs.vlog.Vlog("unixctl_server")
-strtypes = six.string_types
 
 
 class UnixctlConnection(object):
     def __init__(self, rpc):
         assert isinstance(rpc, ovs.jsonrpc.Connection)
         self._rpc = rpc
         self._request_id = None
@@ -79,15 +76,15 @@
     def _wait(self, poller):
         self._rpc.wait(poller)
         if not self._rpc.get_backlog():
             self._rpc.recv_wait(poller)
 
     def _reply_impl(self, success, body):
         assert isinstance(success, bool)
-        assert body is None or isinstance(body, strtypes)
+        assert body is None or isinstance(body, str)
 
         assert self._request_id is not None
 
         if body is None:
             body = ""
 
         if body and not body.endswith("\n"):
@@ -117,20 +114,20 @@
             error = '"%s" command requires at least %d arguments' \
                     % (method, command.min_args)
         elif len(params) > command.max_args:
             error = '"%s" command takes at most %d arguments' \
                     % (method, command.max_args)
         else:
             for param in params:
-                if not isinstance(param, strtypes):
+                if not isinstance(param, str):
                     error = '"%s" command has non-string argument' % method
                     break
 
             if error is None:
-                unicode_params = [six.text_type(p) for p in params]
+                unicode_params = [str(p) for p in params]
                 command.callback(self, unicode_params, command.aux)
 
         if error:
             self.reply_error(error)
 
 
 def _unixctl_version(conn, unused_argv, version):
@@ -184,15 +181,15 @@
     @staticmethod
     def create(path, version=None):
         """Creates a new UnixctlServer which listens on a unixctl socket
         created at 'path'.  If 'path' is None, the default path is chosen.
         'version' contains the version of the server as reported by the unixctl
         version command.  If None, ovs.version.VERSION is used."""
 
-        assert path is None or isinstance(path, strtypes)
+        assert path is None or isinstance(path, str)
 
         if path is not None:
             path = "punix:%s" % ovs.util.abs_file_name(ovs.dirs.RUNDIR, path)
         else:
             if sys.platform == "win32":
                 path = "punix:%s/%s.ctl" % (ovs.dirs.RUNDIR,
                                             ovs.util.PROGRAM_NAME)
@@ -218,18 +215,18 @@
 
 class UnixctlClient(object):
     def __init__(self, conn):
         assert isinstance(conn, ovs.jsonrpc.Connection)
         self._conn = conn
 
     def transact(self, command, argv):
-        assert isinstance(command, strtypes)
+        assert isinstance(command, str)
         assert isinstance(argv, list)
         for arg in argv:
-            assert isinstance(arg, strtypes)
+            assert isinstance(arg, str)
 
         request = Message.create_request(command, argv)
         error, reply = self._conn.transact_block(request)
 
         if error:
             vlog.warn("error communicating with %s: %s"
                       % (self._conn.name, os.strerror(error)))
```

### Comparing `ovs-2.9.4/ovs/_json.c` & `ovs-3.0.0/ovs/_json.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 #include "Python.h"
 #include <openvswitch/json.h>
 #include "structmember.h"
 
-#if PY_MAJOR_VERSION >= 3
-#define IS_PY3K
-#endif
-
 typedef struct {
     PyObject_HEAD
     struct json_parser *_parser;
 } json_ParserObject;
 
 static void
 Parser_dealloc(json_ParserObject * p)
@@ -50,38 +46,30 @@
 
 static PyObject *
 Parser_feed(json_ParserObject * self, PyObject * args)
 {
     Py_ssize_t input_sz;
     PyObject *input;
     size_t rd;
-    char *input_str;
+    const char *input_str;
 
     if (self->_parser == NULL) {
         return NULL;
     }
 
     if (!PyArg_UnpackTuple(args, "input", 1, 1, &input)) {
         return NULL;
     }
-#ifdef IS_PY3K
     if ((input_str = PyUnicode_AsUTF8AndSize(input, &input_sz)) == NULL) {
-#else
-    if (PyString_AsStringAndSize(input, &input_str, &input_sz) < 0) {
-#endif
         return NULL;
     }
 
     rd = json_parser_feed(self->_parser, input_str, (size_t) input_sz);
 
-#ifdef IS_PY3K
     return PyLong_FromSize_t(rd);
-#else
-    return PyInt_FromSize_t(rd);
-#endif
 }
 
 static PyObject *
 Parser_is_done(json_ParserObject * self)
 {
     if (self->_parser == NULL) {
         return NULL;
@@ -102,15 +90,15 @@
     case JSON_OBJECT:{
             struct shash_node *node;
             PyObject *dict = PyDict_New();
 
             if (dict == NULL) {
                 return PyErr_NoMemory();
             }
-            SHASH_FOR_EACH(node, json->u.object) {
+            SHASH_FOR_EACH (node, json->object) {
                 PyObject *key = PyUnicode_FromString(node->name);
                 PyObject *val = json_to_python(node->data);
 
                 if (!(key && val) || PyDict_SetItem(dict, key, val)) {
                     Py_XDECREF(key);
                     Py_XDECREF(val);
                     Py_XDECREF(dict);
@@ -119,43 +107,39 @@
 
                 Py_XDECREF(key);
                 Py_XDECREF(val);
             }
             return dict;
         }
     case JSON_ARRAY:{
-            int i;
-            PyObject *arr = PyList_New(json->u.array.n);
+            size_t i;
+            PyObject *arr = PyList_New(json->array.n);
 
             if (arr == NULL) {
                 return PyErr_NoMemory();
             }
-            for (i = 0; i < json->u.array.n; i++) {
-                PyObject *item = json_to_python(json->u.array.elems[i]);
+            for (i = 0; i < json->array.n; i++) {
+                PyObject *item = json_to_python(json->array.elems[i]);
 
                 if (!item || PyList_SetItem(arr, i, item)) {
                     Py_XDECREF(arr);
                     return NULL;
                 }
             }
             return arr;
         }
     case JSON_REAL:
-        if (json->u.real != 0) {
-            return PyFloat_FromDouble(json->u.real);
+        if (json->real != 0) {
+            return PyFloat_FromDouble(json->real);
         } /* fall through to treat 0 as int */
     case JSON_INTEGER:
-#ifdef IS_PY3K
-        return PyLong_FromLong((long) json->u.integer);
-#else
-        return PyInt_FromLong((long) json->u.integer);
-#endif
+        return PyLong_FromLong((long) json->integer);
 
     case JSON_STRING:
-        return PyUnicode_FromString(json->u.string);
+        return PyUnicode_FromString(json->string);
     default:
         return NULL;
     }
 }
 
 static PyObject *
 Parser_finish(json_ParserObject * self)
@@ -221,49 +205,41 @@
     0,                          /* tp_descr_set */
     0,                          /* tp_dictoffset */
     0,                          /* tp_init */
     0,                          /* tp_alloc */
     Parser_new,                 /* tp_new */
 };
 
-#ifdef IS_PY3K
 static struct PyModuleDef moduledef = {
     PyModuleDef_HEAD_INIT,
     "ovs._json",                /* m_name */
     "OVS JSON Parser module",   /* m_doc */
     0,                          /* m_size */
     0,                          /* m_methods */
     0,                          /* m_slots */
     0,                          /* m_traverse */
     0,                          /* m_clear */
     0,                          /* m_free */
 };
 
-#define INITERROR return NULL
-#else /* !IS_PY3K */
-#define INITERROR return
-#endif
-
 PyMODINIT_FUNC
-#ifdef IS_PY3K
 PyInit__json(void)
-#else
-init_json(void)
-#endif
 {
     PyObject *m;
 
     if (PyType_Ready(&json_ParserType) < 0) {
-        INITERROR;
+        return NULL;
     }
-#ifdef IS_PY3K
+
     m = PyModule_Create(&moduledef);
-#else
-    m = Py_InitModule3("ovs._json", NULL, "OVS JSON Parser module");
-#endif
+    if (!m) {
+        return NULL;
+    }
 
     Py_INCREF(&json_ParserType);
-    PyModule_AddObject(m, "Parser", (PyObject *) & json_ParserType);
-#ifdef IS_PY3K
+    if (PyModule_AddObject(m, "Parser", (PyObject *) &json_ParserType) < 0) {
+        Py_DECREF(&json_ParserType);
+        Py_DECREF(m);
+        return NULL;
+    }
     return m;
-#endif
 }
```

### Comparing `ovs-2.9.4/ovs/daemon.py` & `ovs-3.0.0/ovs/daemon.py`

 * *Files identical despite different names*

### Comparing `ovs-2.9.4/ovs/dirs.py` & `ovs-3.0.0/ovs/dirs.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # The @variables@ in this file are replaced by default directories for
 # use in python/ovs/dirs.py in the source directory and replaced by the
 # configured directories for use in the installed python/ovs/dirs.py.
 #
 import os
 
 # Note that the use of """ is to aid in dealing with paths with quotes in them.
-PKGDATADIR = os.environ.get("OVS_PKGDATADIR", """/usr/local/share/openvswitch""")
-RUNDIR = os.environ.get("OVS_RUNDIR", """/var/run""")
-LOGDIR = os.environ.get("OVS_LOGDIR", """/usr/local/var/log""")
-BINDIR = os.environ.get("OVS_BINDIR", """/usr/local/bin""")
+PKGDATADIR = os.environ.get("OVS_PKGDATADIR", """/usr/share/openvswitch""")
+RUNDIR = os.environ.get("OVS_RUNDIR", """/var/run/openvswitch""")
+LOGDIR = os.environ.get("OVS_LOGDIR", """/var/log/openvswitch""")
+BINDIR = os.environ.get("OVS_BINDIR", """/usr/bin""")
 
 DBDIR = os.environ.get("OVS_DBDIR")
 if not DBDIR:
     sysconfdir = os.environ.get("OVS_SYSCONFDIR")
     if sysconfdir:
         DBDIR = "%s/openvswitch" % sysconfdir
     else:
-        DBDIR = """/usr/local/etc/openvswitch"""
+        DBDIR = """/etc/openvswitch"""
```

### Comparing `ovs-2.9.4/ovs/fatal_signal.py` & `ovs-3.0.0/ovs/fatal_signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,16 +152,22 @@
         for signr in signals:
             if signal.getsignal(signr) == signal.SIG_DFL:
                 signal.signal(signr, _signal_handler)
         atexit.register(_atexit_handler)
 
 
 def signal_alarm(timeout):
+    if not timeout:
+        env_timeout = os.environ.get('OVS_CTL_TIMEOUT')
+        if env_timeout:
+            timeout = int(env_timeout)
+    if not timeout:
+        return
+
     if sys.platform == "win32":
-        import os
         import time
         import threading
 
         class Alarm (threading.Thread):
             def __init__(self, timeout):
                 super(Alarm, self).__init__()
                 self.timeout = timeout
```

### Comparing `ovs-2.9.4/ovs/fcntl_win.py` & `ovs-3.0.0/ovs/fcntl_win.py`

 * *Files identical despite different names*

### Comparing `ovs-2.9.4/ovs/json.py` & `ovs-3.0.0/ovs/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,34 +15,26 @@
 from __future__ import absolute_import
 
 import functools
 import json
 import re
 import sys
 
-import six
-
 PARSER_C = 'C'
 PARSER_PY = 'PYTHON'
 try:
     import ovs._json
     PARSER = PARSER_C
 except ImportError:
     PARSER = PARSER_PY
 
 __pychecker__ = 'no-stringiter'
 
 SPACES_PER_LEVEL = 2
-_dumper = functools.partial(json.dumps, separators=(",", ":"))
-
-if six.PY2:
-    def dumper(*args, **kwargs):
-        return _dumper(*args, **kwargs).decode('raw-unicode-escape')
-else:
-    dumper = _dumper
+dumper = functools.partial(json.dumps, separators=(",", ":"))
 
 
 def to_stream(obj, stream, pretty=False, sort_keys=True):
     stream.write(dumper(obj, indent=SPACES_PER_LEVEL if pretty else None,
                         sort_keys=sort_keys))
 
 
@@ -70,20 +62,20 @@
     try:
         return from_stream(stream)
     finally:
         stream.close()
 
 
 def from_string(s):
-    if not isinstance(s, six.text_type):
+    if not isinstance(s, str):
         # We assume the input is a string.  We will only hit this case for a
         # str in Python 2 which is not unicode, so we need to go ahead and
         # decode it.
         try:
-            s = six.text_type(s, 'utf-8')
+            s = str(s, 'utf-8')
         except UnicodeDecodeError as e:
             seq = ' '.join(["0x%2x" % ord(c)
                            for c in e.object[e.start:e.end] if ord(c) >= 0x80])
             return "not a valid UTF-8 string: invalid UTF-8 sequence %s" % seq
     p = Parser(check_trailer=True)
     p.feed(s)
     return p.finish()
@@ -175,15 +167,15 @@
             self.buffer += c
             return True
         else:
             self.__lex_finish_keyword()
             return False
 
     __number_re = re.compile("(-)?(0|[1-9][0-9]*)"
-            "(?:\.([0-9]+))?(?:[eE]([-+]?[0-9]+))?$")
+            r"(?:\.([0-9]+))?(?:[eE]([-+]?[0-9]+))?$")
 
     def __lex_finish_number(self):
         s = self.buffer
         m = Parser.__number_re.match(s)
         if m:
             sign, integer, fraction, exp = m.groups()
             if (exp is not None and
@@ -232,15 +224,15 @@
                 # Suppress negative zero.
                 value = 0
             self.__parser_input(value)
         elif re.match("-?0[0-9]", s):
             self.__error("leading zeros not allowed")
         elif re.match("-([^0-9]|$)", s):
             self.__error("'-' must be followed by digit")
-        elif re.match("-?(0|[1-9][0-9]*)\.([^0-9]|$)", s):
+        elif re.match(r"-?(0|[1-9][0-9]*)\.([^0-9]|$)", s):
             self.__error("decimal point must be followed by digit")
         elif re.search("e[-+]?([^0-9]|$)", s):
             self.__error("exponent must contain at least one digit")
         else:
             self.__error("syntax error in number")
 
     def __lex_number(self, c):
@@ -337,15 +329,15 @@
                     self.__error("second half of escaped surrogate pair is "
                                  "not trailing surrogate")
                     return
                 code_point = Parser.__utf16_decode_surrogate_pair(c0, c1)
                 inp = inp[6:]
             else:
                 code_point = c0
-            out += six.unichr(code_point)
+            out += chr(code_point)
         self.__parser_input('string', out)
 
     def __lex_string_escape(self, c):
         self.buffer += c
         self.lex_state = Parser.__lex_string
         return True
 
@@ -462,15 +454,15 @@
             top = self.stack[-1]
             if isinstance(top, list):
                 self.parse_state = Parser.__parse_array_next
             else:
                 self.parse_state = Parser.__parse_object_next
 
     def __parse_value(self, token, string, next_state):
-        number_types = list(six.integer_types)
+        number_types = [int]
         number_types.extend([float])
         number_types = tuple(number_types)
         if token in [False, None, True] or isinstance(token, number_types):
             self.__put_value(token)
         elif token == 'string':
             self.__put_value(string)
         else:
```

### Comparing `ovs-2.9.4/ovs/jsonrpc.py` & `ovs-3.0.0/ovs/jsonrpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import codecs
 import errno
 import os
+import random
 import sys
 
 import ovs.json
 import ovs.poller
 import ovs.reconnect
 import ovs.stream
 import ovs.timeval
 import ovs.util
 import ovs.vlog
 
-import six
-
 EOF = ovs.util.EOF
 vlog = ovs.vlog.Vlog("jsonrpc")
 
 
 class Message(object):
     T_REQUEST = 0               # Request.
     T_NOTIFY = 1                # Notification.
@@ -114,15 +113,15 @@
             return "message is not a JSON object"
 
         # Make a copy to avoid modifying the caller's dict.
         json = dict(json)
 
         if "method" in json:
             method = json.pop("method")
-            if not isinstance(method, six.string_types):
+            if not isinstance(method, str):
                 return "method is not a JSON string"
         else:
             method = None
 
         params = json.pop("params", None)
         result = json.pop("result", None)
         error = json.pop("error", None)
@@ -267,16 +266,15 @@
             if not self.input:
                 error, data = self.stream.recv(4096)
                 # Python 3 has separate types for strings and bytes.  We
                 # received bytes from a socket.  We expect it to be string
                 # data, so we convert it here as soon as possible.
                 if data and not error:
                     try:
-                        if six.PY3 or ovs.json.PARSER == ovs.json.PARSER_PY:
-                            data = decoder.decode(data)
+                        data = decoder.decode(data)
                     except UnicodeError:
                         error = errno.EILSEQ
                 if error:
                     if (sys.platform == "win32" and
                             error == errno.WSAEWOULDBLOCK):
                         # WSAEWOULDBLOCK would be the equivalent on Windows
                         # for EAGAIN on Unix.
@@ -294,15 +292,15 @@
                     return EOF, None
                 else:
                     self.input += data
                     self.received_bytes += len(data)
             else:
                 if self.parser is None:
                     self.parser = ovs.json.Parser()
-                if six.PY3 and ovs.json.PARSER == ovs.json.PARSER_C:
+                if ovs.json.PARSER == ovs.json.PARSER_C:
                     self.input = self.input.encode('utf-8')[
                         self.parser.feed(self.input):].decode()
                 else:
                     self.input = self.input[self.parser.feed(self.input):]
                 if self.parser.is_done():
                     msg = self.__process_msg()
                     if msg:
@@ -336,15 +334,15 @@
                 and reply.id == id_):
                 break
         return error, reply
 
     def __process_msg(self):
         json = self.parser.finish()
         self.parser = None
-        if isinstance(json, six.string_types):
+        if isinstance(json, str):
             # XXX rate-limit
             vlog.warn("%s: error parsing stream: %s" % (self.name, json))
             self.error(errno.EPROTO)
             return
 
         msg = Message.from_json(json)
         if not isinstance(msg, Message):
@@ -369,20 +367,25 @@
             self.stream.close()
             self.output = ""
 
 
 class Session(object):
     """A JSON-RPC session with reconnection."""
 
-    def __init__(self, reconnect, rpc):
+    def __init__(self, reconnect, rpc, remotes):
         self.reconnect = reconnect
         self.rpc = rpc
         self.stream = None
         self.pstream = None
         self.seqno = 0
+        if type(remotes) != list:
+            remotes = [remotes]
+        self.remotes = remotes
+        random.shuffle(self.remotes)
+        self.next_remote = 0
 
     @staticmethod
     def open(name, probe_interval=None):
         """Creates and returns a Session that maintains a JSON-RPC session to
         'name', which should be a string acceptable to ovs.stream.Stream or
         ovs.stream.PassiveStream's initializer.
 
@@ -394,36 +397,46 @@
         at any given time.  Any new connection causes the previous one (if any)
         to be dropped.
 
         If "probe_interval" is zero it disables the connection keepalive
         feature. If non-zero the value will be forced to at least 1000
         milliseconds. If None it will just use the default value in OVS.
         """
+        return Session.open_multiple([name], probe_interval=probe_interval)
+
+    @staticmethod
+    def open_multiple(remotes, probe_interval=None):
         reconnect = ovs.reconnect.Reconnect(ovs.timeval.msec())
-        reconnect.set_name(name)
+        session = Session(reconnect, None, remotes)
+        session.pick_remote()
         reconnect.enable(ovs.timeval.msec())
-
-        if ovs.stream.PassiveStream.is_valid_name(name):
+        reconnect.set_backoff_free_tries(len(remotes))
+        if ovs.stream.PassiveStream.is_valid_name(reconnect.get_name()):
             reconnect.set_passive(True, ovs.timeval.msec())
 
-        if not ovs.stream.stream_or_pstream_needs_probes(name):
+        if not ovs.stream.stream_or_pstream_needs_probes(reconnect.get_name()):
             reconnect.set_probe_interval(0)
         elif probe_interval is not None:
             reconnect.set_probe_interval(probe_interval)
 
-        return Session(reconnect, None)
+        return session
 
     @staticmethod
     def open_unreliably(jsonrpc):
         reconnect = ovs.reconnect.Reconnect(ovs.timeval.msec())
+        session = Session(reconnect, None, [jsonrpc.name])
         reconnect.set_quiet(True)
-        reconnect.set_name(jsonrpc.name)
+        session.pick_remote()
         reconnect.set_max_tries(0)
         reconnect.connected(ovs.timeval.msec())
-        return Session(reconnect, jsonrpc)
+        return session
+
+    def pick_remote(self):
+        self.reconnect.set_name(self.remotes[self.next_remote])
+        self.next_remote = (self.next_remote + 1) % len(self.remotes)
 
     def close(self):
         if self.rpc is not None:
             self.rpc.close()
             self.rpc = None
         if self.stream is not None:
             self.stream.close()
@@ -433,36 +446,42 @@
             self.pstream = None
 
     def __disconnect(self):
         if self.rpc is not None:
             self.rpc.error(EOF)
             self.rpc.close()
             self.rpc = None
-            self.seqno += 1
         elif self.stream is not None:
             self.stream.close()
             self.stream = None
-            self.seqno += 1
+        else:
+            return
+
+        self.seqno += 1
+        self.pick_remote()
 
     def __connect(self):
         self.__disconnect()
 
         name = self.reconnect.get_name()
         if not self.reconnect.is_passive():
             error, self.stream = ovs.stream.Stream.open(name)
             if not error:
                 self.reconnect.connecting(ovs.timeval.msec())
             else:
                 self.reconnect.connect_failed(ovs.timeval.msec(), error)
+                self.stream = None
+                self.pick_remote()
         elif self.pstream is None:
             error, self.pstream = ovs.stream.PassiveStream.open(name)
             if not error:
                 self.reconnect.listening(ovs.timeval.msec())
             else:
                 self.reconnect.connect_failed(ovs.timeval.msec(), error)
+                self.pick_remote()
 
         self.seqno += 1
 
     def run(self):
         if self.pstream is not None:
             error, stream = self.pstream.accept()
             if error == 0:
@@ -500,14 +519,15 @@
             error = self.stream.connect()
             if error == 0:
                 self.reconnect.connected(ovs.timeval.msec())
                 self.rpc = Connection(self.stream)
                 self.stream = None
             elif error != errno.EAGAIN:
                 self.reconnect.connect_failed(ovs.timeval.msec(), error)
+                self.pick_remote()
                 self.stream.close()
                 self.stream = None
 
         action = self.reconnect.run(ovs.timeval.msec())
         if action == ovs.reconnect.CONNECT:
             self.__connect()
         elif action == ovs.reconnect.DISCONNECT:
@@ -546,21 +566,24 @@
         else:
             return errno.ENOTCONN
 
     def recv(self):
         if self.rpc is not None:
             received_bytes = self.rpc.get_received_bytes()
             error, msg = self.rpc.recv()
+
+            now = ovs.timeval.msec()
+            self.reconnect.receive_attempted(now)
             if received_bytes != self.rpc.get_received_bytes():
                 # Data was successfully received.
                 #
                 # Previously we only counted receiving a full message as
                 # activity, but with large messages or a slow connection that
                 # policy could time out the session mid-message.
-                self.reconnect.activity(ovs.timeval.msec())
+                self.reconnect.activity(now)
 
             if not error:
                 if msg.type == Message.T_REQUEST and msg.method == "echo":
                     # Echo request.  Send reply.
                     self.send(Message.create_reply(msg.params, msg.id))
                 elif msg.type == Message.T_REPLY and msg.id == "echo":
                     # It's a reply to our echo request.  Suppress it.
@@ -584,7 +607,23 @@
         return self.rpc is not None
 
     def get_seqno(self):
         return self.seqno
 
     def force_reconnect(self):
         self.reconnect.force_reconnect(ovs.timeval.msec())
+
+    def reset_backoff(self):
+        """ Resets the reconnect backoff by allowing as many free tries as the
+        number of configured remotes.  This is to be used by upper layers
+        before calling force_reconnect() if backoff is undesirable."""
+        free_tries = len(self.remotes)
+
+        if self.is_connected():
+            # The extra free try will be consumed when the current remote
+            # is disconnected.
+            free_tries += 1
+
+        self.reconnect.set_backoff_free_tries(free_tries)
+
+    def get_num_of_remotes(self):
+        return len(self.remotes)
```

### Comparing `ovs-2.9.4/ovs/ovsuuid.py` & `ovs-3.0.0/ovs/ovsuuid.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 import re
 import uuid
 
 import ovs.db.parser
 from ovs.db import error
 
-import six
-from six.moves import range
-
 uuidRE = re.compile("^xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx$"
                     .replace('x', '[0-9a-fA-F]'))
 
 
 def zero():
     return uuid.UUID(int=0)
 
@@ -37,24 +34,24 @@
     if not is_valid_string(s):
         raise error.Error("%s is not a valid UUID" % s)
     return uuid.UUID(s)
 
 
 def from_json(json, symtab=None):
     try:
-        s = ovs.db.parser.unwrap_json(json, "uuid", six.string_types, "string")
+        s = ovs.db.parser.unwrap_json(json, "uuid", (str,), "string")
         if not uuidRE.match(s):
             raise error.Error("\"%s\" is not a valid UUID" % s, json)
         return uuid.UUID(s)
     except error.Error as e:
         if not symtab:
             raise e
         try:
             name = ovs.db.parser.unwrap_json(json, "named-uuid",
-                                             six.string_types, "string")
+                                             (str,), "string")
         except error.Error:
             raise e
 
         if name not in symtab:
             symtab[name] = uuid.uuid4()
         return symtab[name]
```

### Comparing `ovs-2.9.4/ovs/poller.py` & `ovs-3.0.0/ovs/poller.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,35 @@
 import ovs.timeval
 import ovs.vlog
 
 if sys.platform == "win32":
     import ovs.winutils as winutils
 
 try:
-    from OpenSSL import SSL
+    import ssl
 except ImportError:
-    SSL = None
+    ssl = None
 
 try:
-    import eventlet.patcher
+    from eventlet import patcher as eventlet_patcher
 
     def _using_eventlet_green_select():
-        return eventlet.patcher.is_monkey_patched(select)
+        return eventlet_patcher.is_monkey_patched(select)
 except:
+    eventlet_patcher = None
+
     def _using_eventlet_green_select():
         return False
 
+try:
+    from gevent import monkey as gevent_monkey
+except:
+    gevent_monkey = None
+
+
 vlog = ovs.vlog.Vlog("poller")
 
 POLLIN = 0x001
 POLLOUT = 0x004
 POLLERR = 0x008
 POLLHUP = 0x010
 POLLNVAL = 0x020
@@ -61,15 +69,15 @@
         self.rlist = []
         self.wlist = []
         self.xlist = []
 
     def register(self, fd, events):
         if isinstance(fd, socket.socket):
             fd = fd.fileno()
-        if SSL and isinstance(fd, SSL.Connection):
+        if ssl and isinstance(fd, ssl.SSLSocket):
             fd = fd.fileno()
 
         if sys.platform != 'win32':
             # Skip this on Windows, it also register events
             assert isinstance(fd, int)
         if events & POLLIN:
             self.rlist.append(fd)
@@ -103,15 +111,15 @@
             # Wait until any of the events is set to signaled
             try:
                 retval = winutils.win32event.WaitForMultipleObjects(
                     events,
                     False,  # Wait all
                     timeout)
             except winutils.pywintypes.error:
-                    return [(0, POLLERR)]
+                return [(0, POLLERR)]
 
             if retval == winutils.winerror.WAIT_TIMEOUT:
                 return []
 
             if events[retval] in self.rlist:
                 revent = POLLIN
             elif events[retval] in self.wlist:
@@ -253,7 +261,30 @@
                     if revents & POLLNVAL:
                         s += "[POLLNVAL]"
                     vlog.dbg("%s on fd %d" % (s, fd))
 
     def __reset(self):
         self.poll = SelectPoll()
         self.timeout = -1
+
+
+def get_system_poll():
+    """Returns the original select.poll() object. If select.poll is
+    monkey patched by eventlet or gevent library, it gets the original
+    select.poll and returns an object of it using the
+    eventlet.patcher.original/gevent.monkey.get_original functions.
+
+    As a last resort, if there is any exception it returns the
+    SelectPoll() object.
+    """
+    try:
+        if _using_eventlet_green_select():
+            _system_poll = eventlet_patcher.original("select").poll
+        elif gevent_monkey and gevent_monkey.is_object_patched(
+                'select', 'poll'):
+            _system_poll = gevent_monkey.get_original('select', 'poll')
+        else:
+            _system_poll = select.poll
+    except:
+        _system_poll = SelectPoll
+
+    return _system_poll()
```

### Comparing `ovs-2.9.4/ovs/process.py` & `ovs-3.0.0/ovs/process.py`

 * *Files identical despite different names*

### Comparing `ovs-2.9.4/ovs/reconnect.py` & `ovs-3.0.0/ovs/reconnect.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,66 +40,80 @@
     later.)"""
 
     class Void(object):
         name = "VOID"
         is_connected = False
 
         @staticmethod
-        def deadline(fsm):
+        def deadline(fsm, now):
             return None
 
         @staticmethod
         def run(fsm, now):
             return None
 
     class Listening(object):
         name = "LISTENING"
         is_connected = False
 
         @staticmethod
-        def deadline(fsm):
+        def deadline(fsm, now):
             return None
 
         @staticmethod
         def run(fsm, now):
             return None
 
     class Backoff(object):
         name = "BACKOFF"
         is_connected = False
 
         @staticmethod
-        def deadline(fsm):
+        def deadline(fsm, now):
             return fsm.state_entered + fsm.backoff
 
         @staticmethod
         def run(fsm, now):
             return CONNECT
 
     class ConnectInProgress(object):
         name = "CONNECTING"
         is_connected = False
 
         @staticmethod
-        def deadline(fsm):
+        def deadline(fsm, now):
             return fsm.state_entered + max(1000, fsm.backoff)
 
         @staticmethod
         def run(fsm, now):
             return DISCONNECT
 
     class Active(object):
         name = "ACTIVE"
         is_connected = True
 
         @staticmethod
-        def deadline(fsm):
+        def deadline(fsm, now):
             if fsm.probe_interval:
                 base = max(fsm.last_activity, fsm.state_entered)
-                return base + fsm.probe_interval
+                expiration = base + fsm.probe_interval
+                if (now < expiration or
+                    fsm.last_receive_attempt is None or
+                    fsm.last_receive_attempt >= expiration):
+                    # We still have time before the expiration or the time has
+                    # already passed and there was no activity.  In the first
+                    # case we need to wait for the expiration, in the second -
+                    # we're already past the deadline. */
+                    return expiration
+                else:
+                    # Time has already passed, but we didn't attempt to receive
+                    # anything.  We need to wake up and try to receive even if
+                    # nothing is pending, so we can update the expiration time
+                    # or transition to a different state.
+                    return now + 1
             return None
 
         @staticmethod
         def run(fsm, now):
             vlog.dbg("%s: idle %d ms, sending inactivity probe"
                      % (fsm.name,
                         now - max(fsm.last_activity, fsm.state_entered)))
@@ -107,32 +121,38 @@
             return PROBE
 
     class Idle(object):
         name = "IDLE"
         is_connected = True
 
         @staticmethod
-        def deadline(fsm):
+        def deadline(fsm, now):
             if fsm.probe_interval:
-                return fsm.state_entered + fsm.probe_interval
+                expiration = fsm.state_entered + fsm.probe_interval
+                if (now < expiration or
+                    fsm.last_receive_attempt is None or
+                    fsm.last_receive_attempt >= expiration):
+                    return expiration
+                else:
+                    return now + 1
             return None
 
         @staticmethod
         def run(fsm, now):
             vlog.err("%s: no response to inactivity probe after %.3g "
                      "seconds, disconnecting"
                       % (fsm.name, (now - fsm.state_entered) / 1000.0))
             return DISCONNECT
 
     class Reconnect(object):
         name = "RECONNECT"
         is_connected = False
 
         @staticmethod
-        def deadline(fsm):
+        def deadline(fsm, now):
             return fsm.state_entered
 
         @staticmethod
         def run(fsm, now):
             return DISCONNECT
 
     def __init__(self, now):
@@ -149,14 +169,15 @@
 
         self.state = Reconnect.Void
         self.state_entered = now
         self.backoff = 0
         self.last_activity = now
         self.last_connected = None
         self.last_disconnected = None
+        self.last_receive_attempt = now
         self.max_tries = None
         self.backoff_free_tries = 0
 
         self.creation_time = now
         self.n_attempted_connections = 0
         self.n_successful_connections = 0
         self.total_connected_duration = 0
@@ -237,15 +258,15 @@
         else:
             self.max_backoff = 8000
         if self.min_backoff > self.max_backoff:
             self.max_backoff = self.min_backoff
 
         if (self.state == Reconnect.Backoff and
             self.backoff > self.max_backoff):
-                self.backoff = self.max_backoff
+            self.backoff = self.max_backoff
 
     def set_backoff_free_tries(self, backoff_free_tries):
         """Sets the number of connection attempts that will be made without
         backoff to 'backoff_free_tries'.  Values 0 and 1 both
         represent a single attempt."""
         self.backoff_free_tries = backoff_free_tries
 
@@ -340,14 +361,17 @@
             elif self.state == Reconnect.Listening:
                 if error > 0:
                     vlog.warn("%s: error listening for connections (%s)"
                               % (self.name, os.strerror(error)))
                 else:
                     self.info_level("%s: error listening for connections"
                                     % self.name)
+            elif self.state == Reconnect.Reconnect:
+                self.info_level("%s: connection closed by client"
+                                % self.name)
             elif self.backoff < self.max_backoff:
                 if self.passive:
                     type_ = "listen"
                 else:
                     type_ = "connection"
                 if error > 0:
                     vlog.warn("%s: %s attempt failed (%s)"
@@ -465,14 +489,24 @@
         """Tell this FSM that some activity occurred on the connection.  This
         resets the probe interval timer, so that the connection is known not to
         be idle."""
         if self.state != Reconnect.Active:
             self._transition(now, Reconnect.Active)
         self.last_activity = now
 
+    def receive_attempted(self, now):
+        """Tell 'fsm' that some attempt to receive data on the connection was
+        made at 'now'.  The FSM only allows probe interval timer to expire when
+        some attempt to receive data on the connection was received after the
+        time when it should have expired.  This helps in the case where there's
+        a long delay in the poll loop and then reconnect_run() executes before
+        the code to try to receive anything from the remote runs.  (To disable
+        this feature, pass None for 'now'.)"""
+        self.last_receive_attempt = now
+
     def _transition(self, now, state):
         if self.state == Reconnect.ConnectInProgress:
             self.n_attempted_connections += 1
             if state == Reconnect.Active:
                 self.n_successful_connections += 1
 
         connected_before = self.state.is_connected
@@ -521,15 +555,15 @@
 
             - ovs.reconnect.PROBE: The client should send some kind of request
               to the peer that will elicit a response, to ensure that the
               connection is indeed in working order.  (This will only be
               returned if the "probe interval" is nonzero--see
               self.set_probe_interval())."""
 
-        deadline = self.state.deadline(self)
+        deadline = self.state.deadline(self, now)
         if deadline is not None and now >= deadline:
             return self.state.run(self, now)
         else:
             return None
 
     def wait(self, poller, now):
         """Causes the next call to poller.block() to wake up when self.run()
@@ -538,15 +572,15 @@
         if timeout is not None and timeout >= 0:
             poller.timer_wait(timeout)
 
     def timeout(self, now):
         """Returns the number of milliseconds after which self.run() should be
         called if nothing else notable happens in the meantime, or None if this
         is currently unnecessary."""
-        deadline = self.state.deadline(self)
+        deadline = self.state.deadline(self, now)
         if deadline is not None:
             remaining = deadline - now
             return max(0, remaining)
         else:
             return None
 
     def is_connected(self):
```

### Comparing `ovs-2.9.4/ovs/socket_util.py` & `ovs-3.0.0/ovs/socket_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 import socket
 import sys
 
 import ovs.fatal_signal
 import ovs.poller
 import ovs.vlog
 
-import six
-from six.moves import range
+try:
+    import ssl
+except ImportError:
+    ssl = None
 
 if sys.platform == 'win32':
     import ovs.winutils as winutils
     import win32file
 
 vlog = ovs.vlog.Vlog("socket_util")
 
@@ -86,15 +88,15 @@
                     return e.errno, None
 
             ovs.fatal_signal.add_file_to_unlink(bind_path)
             sock.bind(bind_path)
 
             try:
                 os.fchmod(sock.fileno(), 0o700)
-            except OSError as e:
+            except OSError:
                 pass
         if connect_path is not None:
             try:
                 sock.connect(connect_path)
             except socket.error as e:
                 if get_exception_errno(e) != errno.EINPROGRESS:
                     raise
@@ -158,33 +160,39 @@
                 free_short_name(short_bind_path)
                 free_short_name(short_connect_path)
         else:
             return get_exception_errno(e), None
 
 
 def check_connection_completion(sock):
-    p = ovs.poller.SelectPoll()
     if sys.platform == "win32":
+        p = ovs.poller.SelectPoll()
         event = winutils.get_new_event(None, False, True, None)
         # Receive notification of readiness for writing, of completed
         # connection or multipoint join operation, and of socket closure.
         win32file.WSAEventSelect(sock, event,
                                  win32file.FD_WRITE |
                                  win32file.FD_CONNECT |
                                  win32file.FD_CLOSE)
         p.register(event, ovs.poller.POLLOUT)
     else:
+        p = ovs.poller.get_system_poll()
         p.register(sock, ovs.poller.POLLOUT)
     pfds = p.poll(0)
     if len(pfds) == 1:
         revents = pfds[0][1]
-        if revents & ovs.poller.POLLERR:
+        if revents & ovs.poller.POLLERR or revents & ovs.poller.POLLHUP:
             try:
                 # The following should raise an exception.
-                socket.send("\0", socket.MSG_DONTWAIT)
+                if ssl and isinstance(sock, ssl.SSLSocket):
+                    # SSL wrapped socket does not allow
+                    # non-zero optional flag.
+                    sock.send("\0".encode())
+                else:
+                    sock.send("\0".encode(), socket.MSG_DONTWAIT)
 
                 # (Here's where we end up if it didn't.)
                 # XXX rate-limit
                 vlog.err("poll return POLLERR but send succeeded")
                 return errno.EPROTO
             except socket.error as e:
                 return get_exception_errno(e)
@@ -220,44 +228,52 @@
             raise ValueError("%s: port number must be specified" % target)
         host_name = address[0]
     if not host_name:
         raise ValueError("%s: bad peer name format" % target)
     return (host_name, port)
 
 
-def inet_open_active(style, target, default_port, dscp):
-    address = inet_parse_active(target, default_port)
+def inet_create_socket_active(style, address):
     try:
         is_addr_inet = is_valid_ipv4_address(address[0])
         if is_addr_inet:
             sock = socket.socket(socket.AF_INET, style, 0)
             family = socket.AF_INET
         else:
             sock = socket.socket(socket.AF_INET6, style, 0)
             family = socket.AF_INET6
     except socket.error as e:
         return get_exception_errno(e), None
 
+    return family, sock
+
+
+def inet_connect_active(sock, address, family, dscp):
     try:
         set_nonblocking(sock)
         set_dscp(sock, family, dscp)
-        try:
-            sock.connect(address)
-        except socket.error as e:
-            error = get_exception_errno(e)
-            if sys.platform == 'win32' and error == errno.WSAEWOULDBLOCK:
-                # WSAEWOULDBLOCK would be the equivalent on Windows
-                # for EINPROGRESS on Unix.
-                error = errno.EINPROGRESS
-            if error != errno.EINPROGRESS:
-                raise
-        return 0, sock
+        error = sock.connect_ex(address)
+        if error not in (0, errno.EINPROGRESS, errno.EWOULDBLOCK):
+            sock.close()
+            return error
+        return 0
     except socket.error as e:
         sock.close()
-        return get_exception_errno(e), None
+        return get_exception_errno(e)
+
+
+def inet_open_active(style, target, default_port, dscp):
+    address = inet_parse_active(target, default_port)
+    family, sock = inet_create_socket_active(style, address)
+    if sock is None:
+        return family, sock
+    error = inet_connect_active(sock, address, family, dscp)
+    if error:
+        return error, None
+    return 0, sock
 
 
 def get_exception_errno(e):
     """A lot of methods on Python socket objects raise socket.error, but that
     exception is documented as having two completely different forms of
     arguments: either a string or a (errno, string) tuple.  We only want the
     errno."""
@@ -291,16 +307,16 @@
     """Returns an (error, bytes_written) tuple where 'error' is 0 on success,
     otherwise a positive errno value, and 'bytes_written' is the number of
     bytes that were written before the error occurred.  'error' is 0 if and
     only if 'bytes_written' is len(buf)."""
     bytes_written = 0
     if len(buf) == 0:
         return 0, 0
-    if six.PY3 and not isinstance(buf, six.binary_type):
-        buf = six.binary_type(buf, 'utf-8')
+    if not isinstance(buf, bytes):
+        buf = bytes(buf, 'utf-8')
     while True:
         try:
             retval = os.write(fd, buf)
             assert retval >= 0
             if retval == len(buf):
                 return 0, bytes_written + len(buf)
             elif retval == 0:
```

### Comparing `ovs-2.9.4/ovs/stream.py` & `ovs-3.0.0/ovs/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 import socket
 import sys
 
 import ovs.poller
 import ovs.socket_util
 import ovs.vlog
 
-import six
-
 try:
-    from OpenSSL import SSL
+    import ssl
 except ImportError:
-    SSL = None
+    ssl = None
 
 if sys.platform == 'win32':
     import ovs.winutils as winutils
     import pywintypes
     import win32event
     import win32file
     import win32pipe
@@ -82,15 +80,15 @@
 
     @staticmethod
     def register_method(method, cls):
         Stream._SOCKET_METHODS[method + ":"] = cls
 
     @staticmethod
     def _find_method(name):
-        for method, cls in six.iteritems(Stream._SOCKET_METHODS):
+        for method, cls in Stream._SOCKET_METHODS.items():
             if name.startswith(method):
                 return cls
         return None
 
     @staticmethod
     def is_valid_name(name):
         """Returns True if 'name' is a stream name in the form "TYPE:ARGS" and
@@ -131,14 +129,18 @@
     # Default value of dscp bits for connection between controller and manager.
     # Value of IPTOS_PREC_INTERNETCONTROL = 0xc0 which is defined
     # in <netinet/ip.h> is used.
     IPTOS_PREC_INTERNETCONTROL = 0xc0
     DSCP_DEFAULT = IPTOS_PREC_INTERNETCONTROL >> 2
 
     @staticmethod
+    def check_connection_completion(sock):
+        return ovs.socket_util.check_connection_completion(sock)
+
+    @staticmethod
     def open(name, dscp=DSCP_DEFAULT):
         """Attempts to connect a stream to a remote peer.  'name' is a
         connection name in the form "TYPE:ARGS", where TYPE is an active stream
         class's name and ARGS are stream class-specific.  The supported TYPEs
         include "unix", "tcp", and "ssl".
 
         Returns (error, stream): on success 'error' is 0 and 'stream' is the
@@ -170,15 +172,15 @@
                     return errno.ENOENT, None
 
                 try:
                     npipe = winutils.create_file(pipename)
                     try:
                         winutils.set_pipe_mode(npipe,
                                                win32pipe.PIPE_READMODE_BYTE)
-                    except pywintypes.error as e:
+                    except pywintypes.error:
                         return errno.ENOENT, None
                 except pywintypes.error as e:
                     if e.winerror == winutils.winerror.ERROR_PIPE_BUSY:
                         # Pipe is busy, set the retry flag to true and retry
                         # again during the connect function.
                         Stream.retry_connect = True
                         return 0, cls(None, name, errno.EAGAIN,
@@ -187,45 +189,62 @@
                     return errno.ENOENT, None
                 return 0, cls(None, name, 0, pipe=npipe, is_server=False)
 
         error, sock = cls._open(suffix, dscp)
         if error:
             return error, None
         else:
-            status = ovs.socket_util.check_connection_completion(sock)
-            return 0, cls(sock, name, status)
+            err = cls.check_connection_completion(sock)
+            if err == errno.EAGAIN or err == errno.EINPROGRESS:
+                status = errno.EAGAIN
+                err = 0
+            elif err == 0:
+                status = 0
+            else:
+                status = err
+            return err, cls(sock, name, status)
 
     @staticmethod
     def _open(suffix, dscp):
         raise NotImplementedError("This method must be overrided by subclass")
 
     @staticmethod
-    def open_block(error_stream):
+    def open_block(error_stream, timeout=None):
         """Blocks until a Stream completes its connection attempt, either
-        succeeding or failing.  (error, stream) should be the tuple returned by
-        Stream.open().  Returns a tuple of the same form.
+        succeeding or failing, but no more than 'timeout' milliseconds.
+        (error, stream) should be the tuple returned by Stream.open().
+        Negative value of 'timeout' means infinite waiting.
+        Returns a tuple of the same form.
 
         Typical usage:
         error, stream = Stream.open_block(Stream.open("unix:/tmp/socket"))"""
 
         # Py3 doesn't support tuple parameter unpacking - PEP 3113
         error, stream = error_stream
         if not error:
+            deadline = None
+            if timeout is not None and timeout >= 0:
+                deadline = ovs.timeval.msec() + timeout
             while True:
                 error = stream.connect()
                 if sys.platform == 'win32' and error == errno.WSAEWOULDBLOCK:
                     # WSAEWOULDBLOCK would be the equivalent on Windows
                     # for EAGAIN on Unix.
                     error = errno.EAGAIN
                 if error != errno.EAGAIN:
                     break
+                if deadline is not None and ovs.timeval.msec() > deadline:
+                    error = errno.ETIMEDOUT
+                    break
                 stream.run()
                 poller = ovs.poller.Poller()
                 stream.run_wait(poller)
                 stream.connect_wait(poller)
+                if deadline is not None:
+                    poller.timer_wait_until(deadline)
                 poller.block()
             if stream.socket is not None:
                 assert error != errno.EINPROGRESS
 
         if error and stream:
             stream.close()
             stream = None
@@ -242,15 +261,15 @@
                 win32pipe.DisconnectNamedPipe(self.pipe)
             winutils.close_handle(self.pipe, vlog.warn)
             winutils.close_handle(self._read.hEvent, vlog.warn)
             winutils.close_handle(self._write.hEvent, vlog.warn)
 
     def __scs_connecting(self):
         if self.socket is not None:
-            retval = ovs.socket_util.check_connection_completion(self.socket)
+            retval = self.check_connection_completion(self.socket)
             assert retval != errno.EINPROGRESS
         elif sys.platform == 'win32':
             if self.retry_connect:
                 try:
                     self.pipe = winutils.create_file(self._pipename)
                     self._retry_connect = False
                     retval = 0
@@ -299,27 +318,30 @@
 
             - If the connection has been closed in the normal fashion or if 'n'
               is 0, the tuple is (0, "").
 
         The recv function will not block waiting for data to arrive.  If no
         data have been received, it returns (errno.EAGAIN, "") immediately."""
 
+        try:
+            return self._recv(n)
+        except socket.error as e:
+            return (ovs.socket_util.get_exception_errno(e), "")
+
+    def _recv(self, n):
         retval = self.connect()
         if retval != 0:
             return (retval, "")
         elif n == 0:
             return (0, "")
 
         if sys.platform == 'win32' and self.socket is None:
             return self.__recv_windows(n)
 
-        try:
-            return (0, self.socket.recv(n))
-        except socket.error as e:
-            return (ovs.socket_util.get_exception_errno(e), "")
+        return (0, self.socket.recv(n))
 
     def __recv_windows(self, n):
         if self._read_pending:
             try:
                 nBytesRead = winutils.get_overlapped_result(self.pipe,
                                                             self._read,
                                                             False)
@@ -373,34 +395,34 @@
         len(buf).  0 is only a valid return value if len(buf) is 0.
 
         On error, returns a negative errno value.
 
         Will not block.  If no bytes can be immediately accepted for
         transmission, returns -errno.EAGAIN immediately."""
 
+        try:
+            return self._send(buf)
+        except socket.error as e:
+            return -ovs.socket_util.get_exception_errno(e)
+
+    def _send(self, buf):
         retval = self.connect()
         if retval != 0:
             return -retval
         elif len(buf) == 0:
             return 0
 
-        # Python 3 has separate types for strings and bytes.  We must have
-        # bytes here.
-        if six.PY3 and not isinstance(buf, bytes):
-            buf = bytes(buf, 'utf-8')
-        elif six.PY2:
+        # We must have bytes for sending.
+        if isinstance(buf, str):
             buf = buf.encode('utf-8')
 
         if sys.platform == 'win32' and self.socket is None:
             return self.__send_windows(buf)
 
-        try:
-            return self.socket.send(buf)
-        except socket.error as e:
-            return -ovs.socket_util.get_exception_errno(e)
+        return self.socket.send(buf)
 
     def __send_windows(self, buf):
         if self._write_pending:
             try:
                 nBytesWritten = winutils.get_overlapped_result(self.pipe,
                                                                self._write,
                                                                False)
@@ -701,16 +723,16 @@
                 winutils.close_handle(self._read.hEvent)
 
 
 def usage(name):
     return """
 Active %s connection methods:
   unix:FILE               Unix domain socket named FILE
-  tcp:IP:PORT             TCP socket to IP with port no of PORT
-  ssl:IP:PORT             SSL socket to IP with port no of PORT
+  tcp:HOST:PORT           TCP socket to HOST with port no of PORT
+  ssl:HOST:PORT           SSL socket to HOST with port no of PORT
 
 Passive %s connection methods:
   punix:FILE              Listen on Unix domain socket FILE""" % (name, name)
 
 
 class UnixStream(Stream):
     @staticmethod
@@ -746,72 +768,98 @@
 
 
 Stream.register_method("tcp", TCPStream)
 
 
 class SSLStream(Stream):
     @staticmethod
-    def needs_probes():
-        return True
+    def check_connection_completion(sock):
+        try:
+            return Stream.check_connection_completion(sock)
+        except ssl.SSLSyscallError as e:
+            return ovs.socket_util.get_exception_errno(e)
 
     @staticmethod
-    def verify_cb(conn, cert, errnum, depth, ok):
-        return ok
+    def needs_probes():
+        return True
 
     @staticmethod
     def _open(suffix, dscp):
-        error, sock = TCPStream._open(suffix, dscp)
-        if error:
-            return error, None
+        address = ovs.socket_util.inet_parse_active(suffix, 0)
+        family, sock = ovs.socket_util.inet_create_socket_active(
+                socket.SOCK_STREAM, address)
+        if sock is None:
+            return family, sock
 
         # Create an SSL context
-        ctx = SSL.Context(SSL.SSLv23_METHOD)
-        ctx.set_verify(SSL.VERIFY_PEER, SSLStream.verify_cb)
-        ctx.set_options(SSL.OP_NO_SSLv2 | SSL.OP_NO_SSLv3)
+        ctx = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
+        ctx.verify_mode = ssl.CERT_REQUIRED
+        ctx.options |= ssl.OP_NO_SSLv2
+        ctx.options |= ssl.OP_NO_SSLv3
         # If the client has not set the SSL configuration files
         # exception would be raised.
-        ctx.use_privatekey_file(Stream._SSL_private_key_file)
-        ctx.use_certificate_file(Stream._SSL_certificate_file)
         ctx.load_verify_locations(Stream._SSL_ca_cert_file)
-
-        ssl_sock = SSL.Connection(ctx, sock)
-        ssl_sock.set_connect_state()
+        ctx.load_cert_chain(Stream._SSL_certificate_file,
+                            Stream._SSL_private_key_file)
+        ssl_sock = ctx.wrap_socket(sock, do_handshake_on_connect=False)
+
+        # Connect
+        error = ovs.socket_util.inet_connect_active(ssl_sock, address, family,
+                                                    dscp)
+        if not error:
+            try:
+                ssl_sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+            except socket.error as e:
+                ssl_sock.close()
+                return ovs.socket_util.get_exception_errno(e), None
         return error, ssl_sock
 
     def connect(self):
         retval = super(SSLStream, self).connect()
 
         if retval:
             return retval
 
         # TCP Connection is successful. Now do the SSL handshake
         try:
             self.socket.do_handshake()
-        except SSL.WantReadError:
+        except ssl.SSLWantReadError:
             return errno.EAGAIN
-        except SSL.SysCallError as e:
+        except ssl.SSLSyscallError as e:
             return ovs.socket_util.get_exception_errno(e)
 
         return 0
 
     def recv(self, n):
         try:
-            return super(SSLStream, self).recv(n)
-        except SSL.WantReadError:
+            return super(SSLStream, self)._recv(n)
+        except ssl.SSLWantReadError:
             return (errno.EAGAIN, "")
-        except SSL.SysCallError as e:
+        except ssl.SSLSyscallError as e:
             return (ovs.socket_util.get_exception_errno(e), "")
-        except SSL.ZeroReturnError:
+        except ssl.SSLZeroReturnError:
             return (0, "")
+        except socket.error as e:
+            return (ovs.socket_util.get_exception_errno(e), "")
 
     def send(self, buf):
         try:
-            return super(SSLStream, self).send(buf)
-        except SSL.WantWriteError:
+            return super(SSLStream, self)._send(buf)
+        except ssl.SSLWantWriteError:
             return -errno.EAGAIN
-        except SSL.SysCallError as e:
+        except ssl.SSLSyscallError as e:
             return -ovs.socket_util.get_exception_errno(e)
+        except socket.error as e:
+            return -ovs.socket_util.get_exception_errno(e)
+
+    def close(self):
+        if self.socket:
+            try:
+                self.socket.shutdown(socket.SHUT_RDWR)
+            except socket.error:
+                pass
+        return super(SSLStream, self).close()
 
 
-if SSL:
+if ssl:
     # Register SSL only if the OpenSSL module is available
     Stream.register_method("ssl", SSLStream)
```

### Comparing `ovs-2.9.4/ovs/timeval.py` & `ovs-3.0.0/ovs/timeval.py`

 * *Files identical despite different names*

### Comparing `ovs-2.9.4/ovs/util.py` & `ovs-3.0.0/ovs/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     string, in which case the current working directory is used.
 
     Returns None if 'dir_' is None and getcwd() fails.
 
     This differs from os.path.abspath() in that it will never change the
     meaning of a file name.
 
-    On Windows an absolute path contains ':' ( i.e: C:\ ) """
+    On Windows an absolute path contains ':' ( i.e: C:\\ ) """
     if file_name.startswith('/') or file_name.find(':') > -1:
         return file_name
     else:
         if dir_ is None or dir_ == "":
             try:
                 dir_ = os.getcwd()
             except OSError:
```

### Comparing `ovs-2.9.4/ovs/vlog.py` & `ovs-3.0.0/ovs/vlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 import sys
 import threading
 
 import ovs.dirs
 import ovs.unixctl
 import ovs.util
 
-import six
-from six.moves import range
-
 DESTINATIONS = {"console": "info", "file": "info", "syslog": "info"}
 PATTERNS = {
     "console": "%D{%Y-%m-%dT%H:%M:%SZ}|%05N|%c%T|%p|%m",
     "file": "%D{%Y-%m-%dT%H:%M:%S.###Z}|%05N|%c%T|%p|%m",
     "syslog": "ovs|%05N|%c%T|%p|%m",
 }
 LEVELS = {
@@ -77,15 +74,15 @@
         if not Vlog.__inited:
             return
 
         level_num = LEVELS.get(level.lower(), logging.DEBUG)
         msg_num = Vlog.__msg_num
         Vlog.__msg_num += 1
 
-        for f, f_level in six.iteritems(Vlog.__mfl[self.name]):
+        for f, f_level in Vlog.__mfl[self.name].items():
             f_level = LEVELS.get(f_level, logging.CRITICAL)
             if level_num >= f_level:
                 msg = self._build_message(message, f, level, msg_num)
                 logging.getLogger(f).log(level_num, msg, **kwargs)
 
     def _build_message(self, message, destination, level, msg_num):
         pattern = self.__log_patterns[destination]
@@ -138,15 +135,15 @@
         if matches.group(2):
             min_width = int(matches.group(2))
             if len(replace) < min_width:
                 replace = replace.center(min_width)
         return re.sub(match, replace.replace('\\', r'\\'), tmp)
 
     def _format_time(self, tmp):
-        date_regex = re.compile('(%(0?[1-9]?[dD])(\{(.*)\})?)')
+        date_regex = re.compile(r'(%(0?[1-9]?[dD])(\{(.*)\})?)')
         match = date_regex.search(tmp)
 
         if match is None:
             return tmp
 
         # UTC date or Local TZ?
         if match.group(2) == "d":
@@ -181,15 +178,15 @@
         self.__log("INFO", message, **kwargs)
 
     def dbg(self, message, **kwargs):
         self.__log("DBG", message, **kwargs)
 
     def __is_enabled(self, level):
         level = LEVELS.get(level.lower(), logging.DEBUG)
-        for f, f_level in six.iteritems(Vlog.__mfl[self.name]):
+        for f, f_level in Vlog.__mfl[self.name].items():
             f_level = LEVELS.get(f_level, logging.CRITICAL)
             if level >= f_level:
                 return True
         return False
 
     def emer_is_enabled(self):
         return self.__is_enabled("EMER")
@@ -233,15 +230,15 @@
                     logger.addHandler(logging.StreamHandler(sys.stderr))
                 elif f == "syslog":
                     Vlog.add_syslog_handler()
                 elif f == "file" and Vlog.__log_file:
                     Vlog.__file_handler = logging.FileHandler(Vlog.__log_file)
                     logger.addHandler(Vlog.__file_handler)
             except (IOError, socket.error):
-                logger.setLevel(logging.CRITICAL)
+                logger.disabled = True
 
         ovs.unixctl.command_register("vlog/reopen", "", 0, 0,
                                      Vlog._unixctl_vlog_reopen, None)
         ovs.unixctl.command_register("vlog/close", "", 0, 0,
                                      Vlog._unixctl_vlog_close, None)
         try:
             # Windows limitation on Python 2, sys.maxsize is a long number
@@ -301,28 +298,32 @@
 
         # If handler is already added and there is no change in 'facility',
         # there is nothing to do.
         if (not facility or facility == syslog_facility) and syslog_handler:
             return
 
         logger = logging.getLogger('syslog')
-        # If there is no infrastructure to support python syslog, disable
-        # the logger to avoid repeated errors.
-        if not os.path.exists("/dev/log"):
+        # Disable the logger if the "null" syslog method requested
+        # by environment.
+        if os.environ.get('OVS_SYSLOG_METHOD') == "null":
             logger.disabled = True
             return
 
+        if facility is None:
+            facility = syslog_facility
+
+        new_handler = logging.handlers.SysLogHandler(address="/dev/log",
+                                                     facility=facility)
+
         if syslog_handler:
             logger.removeHandler(syslog_handler)
 
-        if facility:
-            syslog_facility = facility
+        syslog_handler = new_handler
+        syslog_facility = facility
 
-        syslog_handler = logging.handlers.SysLogHandler(address="/dev/log",
-                                                    facility=syslog_facility)
         logger.addHandler(syslog_handler)
         return
 
     @staticmethod
     def set_levels_from_string(s):
         module = None
         level = None
@@ -338,15 +339,19 @@
                     return
                 else:
                     return "Destination %s does not exist" % words[1]
             except IndexError:
                 return "Please supply a valid pattern and destination"
         elif words[0] == "FACILITY":
             if words[1] in FACILITIES:
-                Vlog.add_syslog_handler(words[1])
+                try:
+                    Vlog.add_syslog_handler(words[1])
+                except (IOError, socket.error):
+                    logger = logging.getLogger('syslog')
+                    logger.disabled = True
                 return
             else:
                 return "Facility %s is invalid" % words[1]
 
         for word in [w.lower() for w in words]:
             if word == "any":
                 pass
```

### Comparing `ovs-2.9.4/ovs/winutils.py` & `ovs-3.0.0/ovs/winutils.py`

 * *Files identical despite different names*

### Comparing `ovs-2.9.4/ovs.egg-info/PKG-INFO` & `ovs-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ovs
-Version: 2.9.4
+Version: 3.0.0
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
-Description: UNKNOWN
 Keywords: openvswitch,ovs,OVSDB
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Provides-Extra: flow
```

### Comparing `ovs-2.9.4/ovs.egg-info/SOURCES.txt` & `ovs-3.0.0/ovs.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.rst
+pyproject.toml
 setup.py
 ovs/__init__.py
 ovs/_json.c
 ovs/daemon.py
 ovs/dirs.py
 ovs/fatal_signal.py
 ovs/fcntl_win.py
@@ -33,10 +34,20 @@
 ovs/db/custom_index.py
 ovs/db/data.py
 ovs/db/error.py
 ovs/db/idl.py
 ovs/db/parser.py
 ovs/db/schema.py
 ovs/db/types.py
+ovs/flow/__init__.py
+ovs/flow/decoders.py
+ovs/flow/filter.py
+ovs/flow/flow.py
+ovs/flow/kv.py
+ovs/flow/list.py
+ovs/flow/odp.py
+ovs/flow/ofp.py
+ovs/flow/ofp_act.py
+ovs/flow/ofp_fields.py
 ovs/unixctl/__init__.py
 ovs/unixctl/client.py
 ovs/unixctl/server.py
```

### Comparing `ovs-2.9.4/setup.py` & `ovs-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,35 +6,47 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from __future__ import print_function
-
+import os
 import sys
 
-from distutils.command.build_ext import build_ext
-from distutils.errors import CCompilerError, DistutilsExecError, \
-    DistutilsPlatformError
+from setuptools.command.build_ext import build_ext
+try:
+    from setuptools.errors import CCompilerError, ExecError, PlatformError
+except ImportError:  # Needed for setuptools < 59.0
+    from distutils.errors import CCompilerError
+    from distutils.errors import DistutilsExecError as ExecError
+    from distutils.errors import DistutilsPlatformError as PlatformError
 
 import setuptools
 
 VERSION = "unknown"
 
 try:
     # Try to set the version from the generated ovs/version.py
     exec(open("ovs/version.py").read())
 except IOError:
     print("Ensure version.py is created by running make python/ovs/version.py",
           file=sys.stderr)
     sys.exit(-1)
 
-ext_errors = (CCompilerError, DistutilsExecError, DistutilsPlatformError)
+try:
+    # Try to open generated ovs/dirs.py. However, in this case we
+    # don't need to exec()
+    open("ovs/dirs.py")
+except IOError:
+    print("Ensure dirs.py is created by running make python/ovs/dirs.py",
+          file=sys.stderr)
+    sys.exit(-1)
+
+ext_errors = (CCompilerError, ExecError, PlatformError)
 if sys.platform == 'win32':
     ext_errors += (IOError, ValueError)
 
 
 class BuildFailed(Exception):
     pass
 
@@ -42,60 +54,76 @@
 class try_build_ext(build_ext):
     # This class allows C extension building to fail
     # NOTE: build_ext is not a new-style class
 
     def run(self):
         try:
             build_ext.run(self)
-        except DistutilsPlatformError:
+        except PlatformError:
             raise BuildFailed()
 
     def build_extension(self, ext):
         try:
             build_ext.build_extension(self, ext)
         except ext_errors:
             raise BuildFailed()
 
 
+# Allow caller of setup.py to pass in libopenvswitch.a as an object for linking
+# plus all the dependencies through the use of 'extra_cflags' and 'extra_libs'
+# environment variables when not building a shared openvswitch library.
+
+if os.environ.get('enable_shared', '') == 'no':
+    libraries = []
+else:
+    libraries = ['openvswitch']
+
+extra_cflags = os.environ.get('extra_cflags', '').split()
+extra_libs = os.environ.get('extra_libs', '').split()
+
+
 setup_args = dict(
     name='ovs',
     description='Open vSwitch library',
     version=VERSION,
     url='http://www.openvswitch.org/',
     author='Open vSwitch',
     author_email='dev@openvswitch.org',
     packages=['ovs', 'ovs.compat', 'ovs.compat.sortedcontainers',
-              'ovs.db', 'ovs.unixctl'],
+              'ovs.db', 'ovs.unixctl', 'ovs.flow'],
     keywords=['openvswitch', 'ovs', 'OVSDB'],
     license='Apache 2.0',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Topic :: Database :: Front-Ends',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Networking',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
     ],
-    ext_modules=[setuptools.Extension("ovs._json", sources=["ovs/_json.c"],
-                                      libraries=['openvswitch'])],
+    ext_modules=[setuptools.Extension("ovs._json",
+                                      sources=["ovs/_json.c"],
+                                      libraries=libraries,
+                                      extra_compile_args=extra_cflags,
+                                      extra_link_args=extra_libs)],
     cmdclass={'build_ext': try_build_ext},
     install_requires=['sortedcontainers'],
+    extras_require={':sys_platform == "win32"': ['pywin32 >= 1.0'],
+                    'flow': ['netaddr', 'pyparsing']},
 )
 
 try:
     setuptools.setup(**setup_args)
 except BuildFailed:
     BUILD_EXT_WARNING = ("WARNING: The C extension could not be compiled, "
                          "speedups are not enabled.")
     print("*" * 75)
     print(BUILD_EXT_WARNING)
     print("Failure information, if any, is above.")
     print("Retrying the build without the C extension.")
     print("*" * 75)
 
-    del(setup_args['cmdclass'])
-    del(setup_args['ext_modules'])
+    del setup_args['cmdclass']
+    del setup_args['ext_modules']
     setuptools.setup(**setup_args)
```

### Comparing `ovs-2.9.4/PKG-INFO` & `ovs-3.0.0/ovs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ovs
-Version: 2.9.4
+Version: 3.0.0
 Summary: Open vSwitch library
 Home-page: http://www.openvswitch.org/
 Author: Open vSwitch
 Author-email: dev@openvswitch.org
 License: Apache 2.0
-Description: UNKNOWN
 Keywords: openvswitch,ovs,OVSDB
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Provides-Extra: flow
```

