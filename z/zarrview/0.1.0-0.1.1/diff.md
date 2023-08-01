# Comparing `tmp/zarrview-0.1.0.tar.gz` & `tmp/zarrview-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrview-0.1.0.tar", last modified: Mon Jul 31 23:56:27 2023, max compression
+gzip compressed data, was "zarrview-0.1.1.tar", last modified: Tue Aug  1 20:15:51 2023, max compression
```

## Comparing `zarrview-0.1.0.tar` & `zarrview-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-07-31 23:56:27.547354 zarrview-0.1.0/
--rw-r--r--   0 marcel     (501) staff       (20)     1077 2023-07-31 23:47:54.000000 zarrview-0.1.0/LICENSE
--rw-r--r--   0 marcel     (501) staff       (20)      798 2023-07-31 23:56:27.546975 zarrview-0.1.0/PKG-INFO
--rw-r--r--   0 marcel     (501) staff       (20)       64 2023-07-31 23:47:54.000000 zarrview-0.1.0/README.md
--rw-r--r--   0 marcel     (501) staff       (20)       38 2023-07-31 23:56:27.547550 zarrview-0.1.0/setup.cfg
--rw-r--r--   0 marcel     (501) staff       (20)     1174 2023-07-31 23:32:05.000000 zarrview-0.1.0/setup.py
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-07-31 23:56:27.544311 zarrview-0.1.0/zarrview/
--rw-------   0 marcel     (501) staff       (20)    50449 2023-07-31 23:26:24.000000 zarrview-0.1.0/zarrview/ZarrViewer.py
--rw-r--r--   0 marcel     (501) staff       (20)        0 2023-07-10 21:49:49.000000 zarrview-0.1.0/zarrview/__init__.py
--rw-r--r--   0 marcel     (501) staff       (20)      364 2023-07-31 23:05:59.000000 zarrview-0.1.0/zarrview/__main__.py
--rw-------   0 marcel     (501) staff       (20)    22396 2023-07-31 23:00:32.000000 zarrview-0.1.0/zarrview/zarr_path_utils.py
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-07-31 23:56:27.546476 zarrview-0.1.0/zarrview.egg-info/
--rw-r--r--   0 marcel     (501) staff       (20)      798 2023-07-31 23:56:27.000000 zarrview-0.1.0/zarrview.egg-info/PKG-INFO
--rw-r--r--   0 marcel     (501) staff       (20)      278 2023-07-31 23:56:27.000000 zarrview-0.1.0/zarrview.egg-info/SOURCES.txt
--rw-r--r--   0 marcel     (501) staff       (20)        1 2023-07-31 23:56:27.000000 zarrview-0.1.0/zarrview.egg-info/dependency_links.txt
--rw-r--r--   0 marcel     (501) staff       (20)       36 2023-07-31 23:56:27.000000 zarrview-0.1.0/zarrview.egg-info/requires.txt
--rw-r--r--   0 marcel     (501) staff       (20)        9 2023-07-31 23:56:27.000000 zarrview-0.1.0/zarrview.egg-info/top_level.txt
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-01 20:15:51.800491 zarrview-0.1.1/
+-rw-r--r--   0 marcel     (501) staff       (20)     1077 2023-07-31 23:47:54.000000 zarrview-0.1.1/LICENSE
+-rw-r--r--   0 marcel     (501) staff       (20)     3916 2023-08-01 20:15:51.799972 zarrview-0.1.1/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)     3114 2023-08-01 19:54:02.000000 zarrview-0.1.1/README.md
+-rw-r--r--   0 marcel     (501) staff       (20)       38 2023-08-01 20:15:51.800588 zarrview-0.1.1/setup.cfg
+-rw-r--r--   0 marcel     (501) staff       (20)     1316 2023-08-01 20:14:16.000000 zarrview-0.1.1/setup.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-01 20:15:51.797314 zarrview-0.1.1/zarrview/
+-rw-------   0 marcel     (501) staff       (20)    50525 2023-08-01 17:00:31.000000 zarrview-0.1.1/zarrview/ZarrViewer.py
+-rw-r--r--   0 marcel     (501) staff       (20)        0 2023-07-10 21:49:49.000000 zarrview-0.1.1/zarrview/__init__.py
+-rw-r--r--   0 marcel     (501) staff       (20)      423 2023-08-01 18:30:36.000000 zarrview-0.1.1/zarrview/__main__.py
+-rw-------   0 marcel     (501) staff       (20)    22926 2023-08-01 16:57:00.000000 zarrview-0.1.1/zarrview/zarr_path_utils.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-01 20:15:51.799471 zarrview-0.1.1/zarrview.egg-info/
+-rw-r--r--   0 marcel     (501) staff       (20)     3916 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)      278 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/SOURCES.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        1 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/dependency_links.txt
+-rw-r--r--   0 marcel     (501) staff       (20)       78 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/requires.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        9 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/top_level.txt
```

### Comparing `zarrview-0.1.0/LICENSE` & `zarrview-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrview-0.1.0/zarrview/ZarrViewer.py` & `zarrview-0.1.1/zarrview/ZarrViewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     except ImportError:
         from PyQt5.QtCore import *
         from PyQt5.QtGui import *
         from PyQt5.QtWidgets import *
     Signal = pyqtSignal
     Slot = pyqtSlot
 
-import numpy as np
 import zarr
 from zarrview import zarr_path_utils as zpu
 import qtawesome as qta
 
 
 class ZarrTreeItem:
     """ Each tree item corresponds to a zarr group, array, or attr.
@@ -937,17 +936,21 @@
             result += self._repr_recursion(child, indent + 2)
         return result
 
     def __repr__(self) -> str:
         return self._repr_recursion(self.root_item)
     
     def max_depth(self) -> int:
+        max_depth = 0
         items = self.root_item.subtree_itemlist()
-        depths = [item.depth() for item in items]
-        return np.max(depths)
+        for item in items:
+            depth = item.depth()
+            if depth > max_depth:
+                max_depth = depth
+        return max_depth
 
     def dump(self):
         self.root_item.dump()
 
 
 class ZarrTreeView(QTreeView):
     def __init__(self, parent: QWidget = None):
```

### Comparing `zarrview-0.1.0/zarrview/zarr_path_utils.py` & `zarrview-0.1.1/zarrview/zarr_path_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """zarr_path_utils.py
 """
 
 
 import re
-import numpy as np
 import zarr
 
 
 def index_exp(exp: str) -> tuple[int | list[int] | slice]:
     """ Convert index expression string to tuple of slices or index lists for each dimension.
 
     exp: Index expression string (i.e., what you would put inside [] for indexing as in numpy).
@@ -46,32 +45,36 @@
             # single index
             slices.append(
                 int(part)
             )
     return tuple(slices)
 
 def test_index_exp():
-    ok = []
+    all_ok = True
+
     for exp, slices in [
         ['5', (5,)],
         [':5', (slice(None, 5),)],
         ['::2', (slice(None, None, 2),)],
         ['5::2', (slice(5, None, 2),)],
         [':', (slice(None),)],
         [' : ', (slice(None),)],
         [':2, [5, 7, 8], 1:3, :', (slice(None, 2), [5, 7, 8], slice(1, 3), slice(None))],
         ['[5, 7, 8]', ([5, 7, 8],)],
         ['[5, 7, 8], 6', ([5, 7, 8], 6)],
         [':, [5, 7, 8]', (slice(None), [5, 7, 8])],
         ['5, 7, 8', (5, 7, 8)]
     ]:
         ind = index_exp(exp)
-        ok.append(ind == slices)
-        print('OK' if ok[-1] else 'FAIL', exp, '->', ind)
-    return np.all(ok)
+        ok = ind == slices
+        print('OK' if ok else 'FAIL', exp, '->', ind)
+        if not ok:
+            all_ok = False
+    
+    return all_ok
 
 
 def name_index_exp(exp: str) -> tuple[str, tuple[int | list[int] | slice]]:
     """ parse name[index_exp] string for name and slices/indices
     
     e.g.,
         exp = 'group[1:3, 14, [5, 7, 8]]'
@@ -82,19 +85,24 @@
         if pos != -1:
             name = exp[:pos].strip()
             ind = exp[pos+1:-1]
             return name, index_exp(ind)
     return exp, ()
 
 def test_name_index_exp():
+    all_ok = True
+
     exp = 'group[:, 1:3, 2, [5, 7, 8]]'
     name, slices = name_index_exp(exp)
     ok = name == 'group' and slices == (slice(None), slice(1, 3), 2, [5, 7, 8])
     print('OK' if ok else 'FAIL', exp, '->', name, slices)
-    return ok
+    if not ok:
+        all_ok = False
+    
+    return all_ok
 
 
 def slice_path(path: str) -> tuple[tuple[str, tuple[int | list[int] | slice]]]:
     """ return path parts and slices/indices from path string
 
     e.g. path = 'project/run[0]/sweep[:2,3]/channel[[1,4,6]]/trace[:]'
         -> (
@@ -104,35 +112,39 @@
             ('channel', ([1,4,6],)), 
             ('trace', (slice(None, None, None),))
             )
     """
     return tuple(name_index_exp(part.strip()) for part in path.strip('/').split('/'))
 
 def test_slice_path():
-    ok = []
+    all_ok = True
 
     path = 'project/run[0]/sweep[:2,3]/channel[[1,4,6]]/trace[:]'
     pathslices = slice_path(path)
-    ok.append(pathslices == (
+    ok = pathslices == (
         ('project', ()), 
         ('run', (0,)), 
         ('sweep', (slice(None, 2), 3)), 
         ('channel', ([1,4,6],)), 
         ('trace', (slice(None),))
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', pathslices)
+    )
+    print('OK' if ok else 'FAIL', path, '->', pathslices)
+    if not ok:
+        all_ok = False
 
     path = 'project'
     pathslices = slice_path(path)
-    ok.append(pathslices == (
+    ok = pathslices == (
         ('project', ()),
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', pathslices)
+    )
+    print('OK' if ok else 'FAIL', path, '->', pathslices)
+    if not ok:
+        all_ok = False
 
-    return np.all(ok)
+    return all_ok
 
 
 def path_slice_regex(path: str | tuple[tuple[str, tuple[int | list[int] | slice]]]
                      ) -> tuple[str, list[slice]]:
     """ Constructs a regex for matching paths in the input path slice.
 
         Returns the regex plus all slices associated with capture groups in the regex.
@@ -195,83 +207,105 @@
     for group, group_slice in zip(result.groups(), group_slices):
         index = int(group)
         if index not in range(*group_slice.indices(index + 1)):
             return False
     return True
 
 def test_path_in_slice():
-    ok = []
+    all_ok = True
 
     path_slice = 'run[0]/sweep[:]/channel[1:]/trace[:]'
     path = 'run.0/sweep.1/channel.1'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == False)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == False
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = '.../channel[1:]/...'
     path = 'run.0/sweep.1/channel.1/trace.2'
     isin = path_in_slice(path, path_slice_regex(path_slice))
-    ok.append(isin == True)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == True
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = '.../channel[1:]/...'
     path = 'run.0/sweep.1/channel.1/trace.2'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == True)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == True
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = '.../channel[1:]/...'
     path = 'run.0/sweep.1/channel.0/trace.2'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == False)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == False
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = 'run[0]/sweep.1/channel[1:]/trace[:]'
     path = 'run.0/sweep.1/channel.1/trace.2'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == True)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == True
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = 'run[0]/sweep[:]/channel[1:]/trace[:]'
     path = 'run.0/sweep.1/channel.1/trace.2'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == True)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == True
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = 'run[0]/sweep[:]/channel[1:]/trace[:]'
     path = 'run.0/sweep.1/channel.0/trace.2'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == False)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == False
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = 'run[0]/sweep[:,3,4:]/channel[1:]/trace[:]'
     path = 'run.0/sweep.1.3.6/channel.2/trace.8'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == True)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == True
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = 'run[0]/sweep[:,3,4:]/channel[1:]/trace[:]'
     path = 'run.0/sweep.1.3/channel.2/trace.8'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == False)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == False
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = 'run[0]/sweep[:,3,4:]/channel[1:]/trace[:]'
     path = 'run.0/sweep.1.3.6/channel.2/'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == False)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == False
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
     path_slice = 'run[0]/sweep[0]/channel[0]/trace[:]'
     path = 'run.0/sweep.0/channel.0/trace.0/ydata'
     isin = path_in_slice(path, path_slice)
-    ok.append(isin == False)
-    print('OK' if ok[-1] else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    ok = isin == False
+    print('OK' if ok else 'FAIL', path, 'in' if isin else 'not in', path_slice)
+    if not ok:
+        all_ok = False
 
-    return np.all(ok)
+    return all_ok
 
 
 def find_first(root: zarr.hierarchy.Group, name: str, include_arrays: bool = True, include_groups: bool = True) -> zarr.hierarchy.Group | zarr.core.Array | None:
     def _find_first(obj):
         if isinstance(obj, zarr.core.Array) and not include_arrays:
             return
         if isinstance(obj, zarr.hierarchy.Group) and not include_groups:
@@ -280,47 +314,55 @@
         if name == objname or name == objname.split('.')[0]:
             return obj
     
     return root.visitvalues(_find_first)
 
 def test_find_first():
     root = zarr.group()
-    root.create_dataset('run.0/sweep.0/channel.0/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.0/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.0/trace.2/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.2/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.0/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.0/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.1/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.1/trace.1/ydata', data=np.random.random(1000))
+    root.create_dataset('run.0/sweep.0/channel.0/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.0/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.0/trace.2/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.2/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.0/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.0/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.1/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.1/trace.1/ydata', shape=1000)
     print(root.tree())
 
-    ok = []
+    all_ok = True
 
     obj = find_first(root, 'ydata')
     trueobj = root['run.0/sweep.0/channel.0/trace.0/ydata']
-    ok.append(obj == trueobj)
-    print('OK' if ok[-1] else 'FAIL', 'ydata', '->', obj)
+    ok = obj == trueobj
+    print('OK' if all_ok else 'FAIL', 'ydata', '->', obj)
+    if not ok:
+        all_ok = False
 
     obj = find_first(root, 'channel.1')
     trueobj = root['run.0/sweep.0/channel.1']
-    ok.append(obj == trueobj)
-    print('OK' if ok[-1] else 'FAIL', 'channel.1', '->', obj)
+    ok = obj == trueobj
+    print('OK' if ok else 'FAIL', 'channel.1', '->', obj)
+    if not ok:
+        all_ok = False
 
     obj = find_first(root, 'ydata', include_arrays=False)
-    ok.append(obj is None)
-    print('OK' if ok[-1] else 'FAIL', 'ydata include_arrays=False', '->', obj)
+    ok = obj is None
+    print('OK' if ok else 'FAIL', 'ydata include_arrays=False', '->', obj)
+    if not ok:
+        all_ok = False
 
     obj = find_first(root, 'channel.1', include_groups=False)
-    ok.append(obj is None)
-    print('OK' if ok[-1] else 'FAIL', 'channel.1 include_groups=False', '->', obj)
+    ok = obj is None
+    print('OK' if ok else 'FAIL', 'channel.1 include_groups=False', '->', obj)
+    if not ok:
+        all_ok = False
     
-    return np.all(ok)
+    return all_ok
 
 
 def find_all(root: zarr.hierarchy.Group, name: str, include_arrays: bool = True, include_groups: bool = True) -> list[zarr.hierarchy.Group | zarr.core.Array]:
     objects = []
 
     def _find_all(obj):
         if isinstance(obj, zarr.core.Array) and not include_arrays:
@@ -332,58 +374,66 @@
             objects.append(obj)
     
     root.visitvalues(_find_all)
     return objects
 
 def test_find_all():
     root = zarr.group()
-    root.create_dataset('run.0/sweep.0/channel.0/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.0/trace.0/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.0/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.0/trace.2/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.2/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.0/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.0/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.1/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.1/trace.1/ydata', data=np.random.random(1000))
+    root.create_dataset('run.0/sweep.0/channel.0/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.0/trace.0/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.0/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.0/trace.2/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.2/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.0/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.0/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.1/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.1/trace.1/ydata', shape=1000)
     print(root.tree())
 
-    ok = []
+    all_ok = True
 
     objs = find_all(root['run.0/sweep.0/channel.0'], 'trace')
     trueobjs = (
         root['run.0/sweep.0/channel.0/trace.0'],
         root['run.0/sweep.0/channel.0/trace.0/trace.0'],
         root['run.0/sweep.0/channel.0/trace.1'],
         root['run.0/sweep.0/channel.0/trace.2']
     )
-    ok.append(tuple(objs) == trueobjs)
-    print('OK' if ok[-1] else 'FAIL', 'run.0/sweep.0/channel.0', 'trace', '->', objs)
+    ok = tuple(objs) == trueobjs
+    print('OK' if ok else 'FAIL', 'run.0/sweep.0/channel.0', 'trace', '->', objs)
+    if not ok:
+        all_ok = False
 
     objs = find_all(root['run.0/sweep.0/channel.0'], 'ydata')
     trueobjs = (
         root['run.0/sweep.0/channel.0/trace.0/trace.0/ydata'],
         root['run.0/sweep.0/channel.0/trace.0/ydata'],
         root['run.0/sweep.0/channel.0/trace.1/ydata'],
         root['run.0/sweep.0/channel.0/trace.2/ydata']
     )
-    ok.append(tuple(objs) == trueobjs)
-    print('OK' if ok[-1] else 'FAIL', 'run.0/sweep.0/channel.0', 'ydata', '->', objs)
+    ok = tuple(objs) == trueobjs
+    print('OK' if ok else 'FAIL', 'run.0/sweep.0/channel.0', 'ydata', '->', objs)
+    if not ok:
+        all_ok = False
 
     objs = find_all(root['run.0/sweep.0/channel.0'], 'trace', include_groups=False)
-    ok.append(tuple(objs) == ())
-    print('OK' if ok[-1] else 'FAIL', 'run.0/sweep.0/channel.0', 'trace include_groups=False', '->', objs)
+    ok = tuple(objs) == ()
+    print('OK' if ok else 'FAIL', 'run.0/sweep.0/channel.0', 'trace include_groups=False', '->', objs)
+    if not ok:
+        all_ok = False
 
     objs = find_all(root['run.0/sweep.0/channel.0'], 'ydata', include_arrays=False)
-    ok.append(tuple(objs) == ())
-    print('OK' if ok[-1] else 'FAIL', 'run.0/sweep.0/channel.0', 'ydata include_arrays=False', '->', objs)
+    ok = tuple(objs) == ()
+    print('OK' if ok else 'FAIL', 'run.0/sweep.0/channel.0', 'ydata include_arrays=False', '->', objs)
+    if not ok:
+        all_ok = False
     
-    return np.all(ok)
+    return all_ok
 
 
 def find_leaves(root: zarr.hierarchy.Group, path_slice: str, 
                 include_arrays: bool = True, include_groups: bool = True
                 ) -> list[zarr.hierarchy.Group | zarr.core.Array]:
     regex, group_slices = path_slice_regex(path_slice)
     objects = []
@@ -402,155 +452,181 @@
                 objects.append(obj)
     
     root.visitvalues(_find_leaves)
     return objects
 
 def test_find_leaves():
     root = zarr.group()
-    root.create_dataset('run.0/sweep.0/channel.0/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.0/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.0/trace.2/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.0/channel.1/trace.2/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.0/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.0/trace.1/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.1/trace.0/ydata', data=np.random.random(1000))
-    root.create_dataset('run.0/sweep.1/channel.1/trace.1/ydata', data=np.random.random(1000))
+    root.create_dataset('run.0/sweep.0/channel.0/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.0/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.0/trace.2/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.0/channel.1/trace.2/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.0/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.0/trace.1/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.1/trace.0/ydata', shape=1000)
+    root.create_dataset('run.0/sweep.1/channel.1/trace.1/ydata', shape=1000)
     print(root.tree())
 
-    ok = []
+    all_ok = True
 
     path = '.../channel[0]/trace[:]'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.0/trace.0'],
         root['run.0/sweep.0/channel.0/trace.1'],
         root['run.0/sweep.0/channel.0/trace.2'],
         root['run.0/sweep.1/channel.0/trace.0'],
         root['run.0/sweep.1/channel.0/trace.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run[0]/sweep[1]/...'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.1/channel.0/trace.0/ydata'],
         root['run.0/sweep.1/channel.0/trace.1/ydata'],
         root['run.0/sweep.1/channel.1/trace.0/ydata'],
         root['run.0/sweep.1/channel.1/trace.1/ydata']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run[0]/.../trace.1'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.0/trace.1'],
         root['run.0/sweep.0/channel.1/trace.1'],
         root['run.0/sweep.1/channel.0/trace.1'],
         root['run.0/sweep.1/channel.1/trace.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = '.../channel[0]/...'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.0/trace.0/ydata'],
         root['run.0/sweep.0/channel.0/trace.1/ydata'],
         root['run.0/sweep.0/channel.0/trace.2/ydata'],
         root['run.0/sweep.1/channel.0/trace.0/ydata'],
         root['run.0/sweep.1/channel.0/trace.1/ydata']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run[0]/sweep[0]/channel[0]/trace[:]'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.0/trace.0'],
         root['run.0/sweep.0/channel.0/trace.1'],
         root['run.0/sweep.0/channel.0/trace.2']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run[0]/sweep[:]/channel[1:2]/trace[1]'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.1/trace.1'],
         root['run.0/sweep.1/channel.1/trace.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run[0]/sweep[1]/channel[:]/trace[:]'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.1/channel.0/trace.0'],
         root['run.0/sweep.1/channel.0/trace.1'],
         root['run.0/sweep.1/channel.1/trace.0'],
         root['run.0/sweep.1/channel.1/trace.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run.0/sweep[:]/channel[1]/trace[:]'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.1/trace.0'],
         root['run.0/sweep.0/channel.1/trace.1'],
         root['run.0/sweep.0/channel.1/trace.2'],
         root['run.0/sweep.1/channel.1/trace.0'],
         root['run.0/sweep.1/channel.1/trace.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run.0/sweep.1/channel[1]/trace[:]'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.1/channel.1/trace.0'],
         root['run.0/sweep.1/channel.1/trace.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run.0/*/channel[1]/trace[:]'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.1/trace.0'],
         root['run.0/sweep.0/channel.1/trace.1'],
         root['run.0/sweep.0/channel.1/trace.2'],
         root['run.0/sweep.1/channel.1/trace.0'],
         root['run.0/sweep.1/channel.1/trace.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run.0/*/channel[1]/trace[:]/ydata'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0/channel.1/trace.0/ydata'],
         root['run.0/sweep.0/channel.1/trace.1/ydata'],
         root['run.0/sweep.0/channel.1/trace.2/ydata'],
         root['run.0/sweep.1/channel.1/trace.0/ydata'],
         root['run.0/sweep.1/channel.1/trace.1/ydata']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run.0/*'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0'],
         root['run.0/sweep.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
     path = 'run[:]/*'
     leaves = find_leaves(root, path)
-    ok.append(tuple(leaves) == (
+    ok = tuple(leaves) == (
         root['run.0/sweep.0'],
         root['run.0/sweep.1']
-    ))
-    print('OK' if ok[-1] else 'FAIL', path, '->', leaves)
+    )
+    print('OK' if ok else 'FAIL', path, '->', leaves)
+    if not ok:
+        all_ok = False
 
-    return np.all(ok)
+    return all_ok
 
 
 def tests():
     test_funcs = [
         test_index_exp,
         test_name_index_exp,
         test_slice_path,
```

