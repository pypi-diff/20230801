# Comparing `tmp/ciopath-1.1.0-py2.py3-none-any.whl.zip` & `tmp/ciopath-1.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15998 bytes, number of entries: 16
--rw-r--r--  2.0 unx     1079 b- defN 23-Jul-19 15:58 ciopath/LICENSE
--rw-r--r--  2.0 unx      267 b- defN 23-Jul-19 15:58 ciopath/README.md
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-19 15:58 ciopath/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:57 ciopath/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 23-Jul-19 15:57 ciopath/gpath.py
--rw-r--r--  2.0 unx     8118 b- defN 23-Jul-19 15:57 ciopath/gpath_list.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:57 tests/__init__.py
--rw-r--r--  2.0 unx    18769 b- defN 23-Jul-19 15:57 tests/test_gpath.py
--rw-r--r--  2.0 unx    17802 b- defN 23-Jul-19 15:57 tests/test_gpath_list.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:57 tests/mocks/__init__.py
--rw-r--r--  2.0 unx      215 b- defN 23-Jul-19 15:57 tests/mocks/glob.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jul-19 15:58 ciopath-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      686 b- defN 23-Jul-19 15:58 ciopath-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-19 15:58 ciopath-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-19 15:58 ciopath-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1206 b- defN 23-Jul-19 15:58 ciopath-1.1.0.dist-info/RECORD
-16 files, 57936 bytes uncompressed, 14032 bytes compressed:  75.8%
+Zip file size: 16012 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     1079 b- defN 23-Aug-01 01:25 ciopath/LICENSE
+-rw-r--r--  2.0 unx      267 b- defN 23-Aug-01 01:25 ciopath/README.md
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-01 01:25 ciopath/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 01:24 ciopath/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 23-Aug-01 01:24 ciopath/gpath.py
+-rw-r--r--  2.0 unx     8046 b- defN 23-Aug-01 01:24 ciopath/gpath_list.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 01:24 tests/__init__.py
+-rw-r--r--  2.0 unx    18817 b- defN 23-Aug-01 01:24 tests/test_gpath.py
+-rw-r--r--  2.0 unx    17831 b- defN 23-Aug-01 01:24 tests/test_gpath_list.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 01:24 tests/mocks/__init__.py
+-rw-r--r--  2.0 unx      215 b- defN 23-Aug-01 01:24 tests/mocks/glob.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Aug-01 01:25 ciopath-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      686 b- defN 23-Aug-01 01:25 ciopath-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Aug-01 01:25 ciopath-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Aug-01 01:25 ciopath-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1206 b- defN 23-Aug-01 01:25 ciopath-1.1.1.dist-info/RECORD
+16 files, 57941 bytes uncompressed, 14046 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: tests/mocks/__init__.py
 Comment: 
 
 Filename: tests/mocks/glob.py
 Comment: 
 
-Filename: ciopath-1.1.0.dist-info/LICENSE
+Filename: ciopath-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ciopath-1.1.0.dist-info/METADATA
+Filename: ciopath-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ciopath-1.1.0.dist-info/WHEEL
+Filename: ciopath-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ciopath-1.1.0.dist-info/top_level.txt
+Filename: ciopath-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ciopath-1.1.0.dist-info/RECORD
+Filename: ciopath-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ciopath/VERSION

```diff
@@ -1 +1 @@
-1.1.0
+1.1.1
```

## ciopath/gpath_list.py

```diff
@@ -167,16 +167,15 @@
                 continue
             if stats["is_file"]:
                 result.append(entry)
             elif stats["is_dir"]:
                 for root, _, files in os.walk(entry.fslash()):
                     for file_name in files:
                         file_path = os.path.join(root, file_name)
-                        resolved_path = os.path.realpath(file_path)
-                        result.append(Path(resolved_path))
+                        result.append(Path(file_path))
 
         self._entries = result
         self._clean = False
         self._current = 0
 
     def __iter__(self):
         """Get an iterator to entries.
```

## tests/test_gpath.py

```diff
@@ -123,15 +123,17 @@
     def test_many_to_single_backslashes_bslash_out(self):
         self.p = Path("C:\\\\a\\b///c")
         self.assertEqual(self.p.bslash(), "C:\\a\\b\\c")
 
 
 class PathExpansionTest(unittest.TestCase):
     def setUp(self):
+
         self.env = {
+            "USERPROFILE": "/users/joebloggs",
             "HOME": "/users/joebloggs",
             "SHOT": "/metropolis/shot01",
             "DEPT": "texturing",
         }
 
     def test_posix_tilde_input(self):
         with mock.patch.dict("os.environ", self.env):
```

## tests/test_gpath_list.py

```diff
@@ -28,14 +28,15 @@
 # Now import glob because we need to populate it.
 import glob  # isort:skip
 
 
 class PathListTest(unittest.TestCase):
     def setUp(self):
         self.env = {
+            "USERPROFILE": "/users/joebloggs",
             "HOME": "/users/joebloggs",
             "SHOT": "/metropolis/shot01",
             "DEPT": "texturing",
         }
 
         self.other_files_on_disk = [
             "/other/file.0001.exr",
@@ -528,33 +529,33 @@
         self.assertEqual(len(d), 3)
         d.remove_pattern("*")
         self.assertEqual(len(d), 0)
 
 
 class RealFilesTest(unittest.TestCase):
     @patch("os.walk")
-    @patch("os.path.realpath")
+    # @patch("os.path.realpath")
     @patch.object(PathList, "glob")
     @patch.object(Path, "stat")
-    def test_expands_a_folder(self, mock_stat, mock_glob, mock_realpath, mock_walk):
-        mock_realpath.side_effect = lambda x: f"/real{x}"
+    def test_expands_a_folder(self, mock_stat, mock_glob,  mock_walk):
+        # mock_realpath.side_effect = lambda x: f"/real{x}"
         mock_walk.return_value = [
             ("/tmp", ["dir1", "dir2"], ["file1.txt", "file2.txt"]),
             ("/tmp/dir1", [], ["file3.txt", "file4.txt"]),
             ("/tmp/dir2", [], []),
         ]
         mock_stat.return_value = {"is_dir": True, "is_file": False}
         p = PathList()
         p.add("/tmp")
         p.real_files()
         self.assertEqual(len(p), 4)
         self.assertEqual(mock_glob.call_count, 1)
-        self.assertIn("/real/tmp/file1.txt", p)
-        self.assertIn("/real/tmp/dir1/file3.txt", p)
-        self.assertNotIn("/tmp", p)
+        self.assertIn("/tmp/file1.txt", p)
+        self.assertIn("/tmp/dir1/file3.txt", p)
+        # self.assertNotIn("/tmp", p)
 
         # ensure it doesn't add files that are already there
         p.add("/tmp")
         p.real_files()
         self.assertEqual(len(p), 4)
```

## Comparing `ciopath-1.1.0.dist-info/LICENSE` & `ciopath-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ciopath-1.1.0.dist-info/METADATA` & `ciopath-1.1.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciopath
-Version: 1.1.0
+Version: 1.1.1
 Summary: Object-oriented platform-transparent path manipulations.
 Home-page: https://github.com/ConductorTechnologies/sequence
 Author: conductor
 Author-email: info@conductortech.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

