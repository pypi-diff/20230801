# Comparing `tmp/quiltcore-0.3.0.tar.gz` & `tmp/quiltcore-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltcore-0.3.0.tar", max compression
+gzip compressed data, was "quiltcore-0.3.1.tar", max compression
```

## Comparing `quiltcore-0.3.0.tar` & `quiltcore-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.3.0/LICENSE
--rw-r--r--   0        0        0     1573 2023-07-20 22:18:01.855543 quiltcore-0.3.0/README.md
--rw-r--r--   0        0        0     1115 2023-07-25 20:44:00.240364 quiltcore-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1291 2023-07-26 23:35:28.000000 quiltcore-0.3.0/quiltcore/__init__.py
--rw-r--r--   0        0        0     1765 2023-07-28 05:16:48.000000 quiltcore-0.3.0/quiltcore/builder.py
--rw-r--r--   0        0        0     1924 2023-07-28 05:16:48.000000 quiltcore-0.3.0/quiltcore/changes.py
--rw-r--r--   0        0        0     2063 2023-07-27 22:25:00.498998 quiltcore-0.3.0/quiltcore/delta.py
--rw-r--r--   0        0        0     2081 2023-07-27 20:11:29.346954 quiltcore-0.3.0/quiltcore/entry.py
--rw-r--r--   0        0        0     1451 2023-07-27 21:55:58.252178 quiltcore-0.3.0/quiltcore/header.py
--rw-r--r--   0        0        0     2532 2023-07-28 05:16:48.000000 quiltcore-0.3.0/quiltcore/manifest.py
--rw-r--r--   0        0        0      628 2023-07-26 15:49:28.518544 quiltcore-0.3.0/quiltcore/namespace.py
--rw-r--r--   0        0        0     1729 2023-07-27 01:48:38.308147 quiltcore-0.3.0/quiltcore/registry.py
--rw-r--r--   0        0        0     4832 2023-07-26 19:06:47.603824 quiltcore-0.3.0/quiltcore/resource.py
--rw-r--r--   0        0        0     3176 2023-07-25 20:35:00.181308 quiltcore-0.3.0/quiltcore/resource_key.py
--rw-r--r--   0        0        0     1516 2023-07-25 20:35:00.182089 quiltcore-0.3.0/quiltcore/resource_path.py
--rw-r--r--   0        0        0     1859 2023-07-27 20:11:40.022675 quiltcore-0.3.0/quiltcore/table.py
--rw-r--r--   0        0        0     6082 2023-07-27 20:22:02.254112 quiltcore-0.3.0/quiltcore/volume.py
--rw-r--r--   0        0        0     8926 2023-07-27 22:05:43.358147 quiltcore-0.3.0/quiltcore/yaml/codec.py
--rw-r--r--   0        0        0      848 2023-07-25 20:35:00.185720 quiltcore-0.3.0/quiltcore/yaml/config.py
--rw-r--r--   0        0        0     1217 2023-07-27 22:10:38.941860 quiltcore-0.3.0/quiltcore/yaml/quiltcore.yaml
--rw-r--r--   0        0        0      833 2023-07-27 22:07:49.354966 quiltcore-0.3.0/quiltcore/yaml/quiltspec.yaml
--rw-r--r--   0        0        0      160 2023-07-20 04:22:58.224611 quiltcore-0.3.0/quiltcore/yaml/schema.yaml
--rw-r--r--   0        0        0     1053 2023-07-20 22:23:12.863928 quiltcore-0.3.0/quiltcore/yaml/spec.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 quiltcore-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1573 2023-07-20 22:18:01.855543 quiltcore-0.3.1/README.md
+-rw-r--r--   0        0        0     1115 2023-07-30 04:14:15.411310 quiltcore-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1291 2023-07-26 23:35:28.000000 quiltcore-0.3.1/quiltcore/__init__.py
+-rw-r--r--   0        0        0     1765 2023-07-27 23:33:36.768064 quiltcore-0.3.1/quiltcore/builder.py
+-rw-r--r--   0        0        0     1924 2023-07-27 23:33:36.768534 quiltcore-0.3.1/quiltcore/changes.py
+-rw-r--r--   0        0        0     2063 2023-07-27 23:33:36.769027 quiltcore-0.3.1/quiltcore/delta.py
+-rw-r--r--   0        0        0     2081 2023-07-27 23:33:36.769455 quiltcore-0.3.1/quiltcore/entry.py
+-rw-r--r--   0        0        0     1451 2023-07-27 23:33:36.769904 quiltcore-0.3.1/quiltcore/header.py
+-rw-r--r--   0        0        0     2863 2023-07-29 05:16:43.683126 quiltcore-0.3.1/quiltcore/manifest.py
+-rw-r--r--   0        0        0      800 2023-08-01 16:27:18.649723 quiltcore-0.3.1/quiltcore/namespace.py
+-rw-r--r--   0        0        0     1812 2023-07-29 04:11:49.929380 quiltcore-0.3.1/quiltcore/registry.py
+-rw-r--r--   0        0        0     4881 2023-07-29 05:23:24.560119 quiltcore-0.3.1/quiltcore/resource.py
+-rw-r--r--   0        0        0     3176 2023-07-25 20:35:00.181308 quiltcore-0.3.1/quiltcore/resource_key.py
+-rw-r--r--   0        0        0     1609 2023-07-30 04:10:07.329505 quiltcore-0.3.1/quiltcore/resource_path.py
+-rw-r--r--   0        0        0     1859 2023-07-27 23:33:36.771096 quiltcore-0.3.1/quiltcore/table.py
+-rw-r--r--   0        0        0     6090 2023-08-01 18:44:37.119423 quiltcore-0.3.1/quiltcore/volume.py
+-rw-r--r--   0        0        0     8926 2023-07-27 23:33:36.772396 quiltcore-0.3.1/quiltcore/yaml/codec.py
+-rw-r--r--   0        0        0      848 2023-07-25 20:35:00.185720 quiltcore-0.3.1/quiltcore/yaml/config.py
+-rw-r--r--   0        0        0     1217 2023-07-27 23:33:36.772841 quiltcore-0.3.1/quiltcore/yaml/quiltcore.yaml
+-rw-r--r--   0        0        0      833 2023-07-27 22:07:49.354966 quiltcore-0.3.1/quiltcore/yaml/quiltspec.yaml
+-rw-r--r--   0        0        0      160 2023-07-20 04:22:58.224611 quiltcore-0.3.1/quiltcore/yaml/schema.yaml
+-rw-r--r--   0        0        0     1053 2023-07-20 22:23:12.863928 quiltcore-0.3.1/quiltcore/yaml/spec.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 quiltcore-0.3.1/PKG-INFO
```

### Comparing `quiltcore-0.3.0/LICENSE` & `quiltcore-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/README.md` & `quiltcore-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/pyproject.toml` & `quiltcore-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltcore"
-version = "0.3.0"
+version = "0.3.1"
 description = "low-level plubming to read/write Quilt packages"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `quiltcore-0.3.0/quiltcore/__init__.py` & `quiltcore-0.3.1/quiltcore/__init__.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/builder.py` & `quiltcore-0.3.1/quiltcore/builder.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/changes.py` & `quiltcore-0.3.1/quiltcore/changes.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/delta.py` & `quiltcore-0.3.1/quiltcore/delta.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/entry.py` & `quiltcore-0.3.1/quiltcore/entry.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/header.py` & `quiltcore-0.3.1/quiltcore/header.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/manifest.py` & `quiltcore-0.3.1/quiltcore/manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,19 +29,28 @@
                 for row in rows:
                     if not isinstance(row, Dict3):
                         raise ValueError("")
                     writer.write(asdict(row))
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
-        try:
-            self.table = Table(path, **kwargs)
-            self.head = self.table.head
-        except FileNotFoundError:
-            logging.warning(f"Manifest not found: {path}")
+        self._table: Table|None = None
+
+    def table(self) -> Table:
+        if not hasattr(self, "_table") or self._table is None:
+            try:
+                self._table = Table(self.path, **self.args)
+            except FileNotFoundError:
+                logging.warning(f"Manifest not found: {self.path}")
+        if not isinstance(self._table, Table):
+            raise TypeError(f"Expected Table, got {type(self._table)}")
+        return self._table
+    
+    def head(self):
+        return self.table().head
 
     #
     # Hash functions
     #
 
     def hash_quilt3(self) -> str:
         """Legacy quilt3 hash of the contents."""
@@ -49,15 +58,15 @@
 
     #
     # Private Methods for child resources
     #
 
     def _child_names(self, **kwargs) -> list[str]:
         """List all child resource names."""
-        return self.table.names()
+        return self.table().names()
 
     def _child_place(self, place: str) -> str:
         if self.IS_REL not in place:
             return place
         if self.IS_LOCAL.match(place) is not None:
             place = self.IS_LOCAL.sub("", place)
         if self.ARG_REG not in self.args:
@@ -65,15 +74,15 @@
         reg = self.args[self.ARG_REG]
         path = reg.root / place
         logging.debug(f"{place} -> {path} [{path.absolute()}]")
         return str(path)
 
     def _child_dict(self, key: str) -> dict:
         """Return the dict for a child resource."""
-        row = self.table.get_dict4(key)
+        row = self.table().get_dict4(key)
         place = row.place
         drow = asdict(row)
         drow[self.codec.K_PLC] = self._child_place(place)
         v = self.GetVersion(place)
         if len(v) > 0:
             drow[self.KEY_VER] = v
         return drow
```

### Comparing `quiltcore-0.3.0/quiltcore/namespace.py` & `quiltcore-0.3.1/quiltcore/namespace.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 
 
 class Namespace(ResourcePath):
     """
     Namespace of Manifests by Hash
     list/get returns a specific Manifest
     """
+    SEP = "/"
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         self.manifests = kwargs[self.KEY_MAN]
+        self.name = self.pkg_name()
 
     def hash(self, tag: str = ResourcePath.TAG_DEFAULT) -> str:
         hash_file = self.path / tag
         return hash_file.read_text()
 
     def _child_path(self, key: str) -> Path:
         """Return the path for a child resource."""
+        # TODO: match on partial hashes
         hash = self.hash(key)
         return self.manifests / hash
+
+    def pkg_name(self) -> str:
+        return self.SEP.join(self.path.parts[-2:])
```

### Comparing `quiltcore-0.3.0/quiltcore/registry.py` & `quiltcore-0.3.1/quiltcore/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class Registry(ResourcePath):
     """
     Top-level Resource reperesenting a Quilt Registry.
     Defines core paths containing Namespaces and Manifests.
     `list` and `get` return Namespace objects
+    TODO: Rename as "Domain"?
     """
 
     DIR_PREFIX = "quilt3/dirs/"
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         self.root = path
@@ -27,15 +28,18 @@
 
         dir = path / self.cf.get_path(self.DIR_PREFIX + key)
         if not dir.exists():
             dir.mkdir(parents=True, exist_ok=True)
         return dir
 
     def _child_args(self, key: str) -> dict:
-        return {self.KEY_MAN: self.manifests}
+        return {
+            self.KEY_MAN: self.manifests,
+            self.KEY_NS: key,
+        }
 
     def put(self, res: Resource, **kwargs) -> "Resource":
         """Link manifest into namespace"""
         if not isinstance(res, Manifest):
             raise TypeError(f"Expected Manifest, got {type(res)}")
         hash = res.hash_quilt3()
         name = kwargs[self.KEY_NS]
```

### Comparing `quiltcore-0.3.0/quiltcore/resource.py` & `quiltcore-0.3.1/quiltcore/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         self.class_key = self.class_name.lower()
         self.args[self.class_key] = self
         key = kwargs.get(self.KEY_KEY, None)
         if key is not None:
             self.args[f"{self.class_key}.{self.KEY_KEY}"] = key
         self.cf = Config()
         self._setup_params()
+        logging.debug(f"Resource: {repr(self)}")
 
     def __repr__(self):
         return f"<{self.class_name}({self.path}, {self.args})>"
 
     def __str__(self):
         return f"<{self.class_name}({self.path})>"
```

### Comparing `quiltcore-0.3.0/quiltcore/resource_key.py` & `quiltcore-0.3.1/quiltcore/resource_key.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/resource_path.py` & `quiltcore-0.3.1/quiltcore/resource_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,9 +46,11 @@
         """List all child resources."""
         return [self.child(x) for x in self._child_list()]
 
     def get(self, key: str, **kwargs) -> "Resource":
         """Get a child resource by name."""
         path = self._child_path(key)
         if not path.exists():
-            raise KeyError(f"Key {key} not found in {self.path}")
+            if not kwargs.get(self.KEY_FRC, False):
+                raise KeyError(f"Key {key} not found in {self.path}")
+            path.mkdir(parents=True)
         return self.child(path, key)
```

### Comparing `quiltcore-0.3.0/quiltcore/table.py` & `quiltcore-0.3.1/quiltcore/table.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/volume.py` & `quiltcore-0.3.1/quiltcore/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,35 +143,35 @@
         """Insert/Replace and return a child resource."""
         logging.debug(f"Volume.put: {res} [{kwargs}]]")
         if not isinstance(res, Manifest):
             raise TypeError(f"Volume.put requires a Manifest, not {type(res)}")
         man: Manifest = res
         hash = man.hash_quilt3()
         stage_path = self._stage_path(hash)
-        Manifest.WriteToPath(man.head, man.list(), stage_path)  # type: ignore
+        Manifest.WriteToPath(man.head(), man.list(), stage_path)  # type: ignore
 
         new_path = self._man_path(hash)
         if new_path.exists() and not kwargs.get(self.KEY_FRC, False):
             raise FileExistsError(f"Manifest {new_path} already exists")
 
         ns_name = (
             kwargs.get(self.KEY_NS)
             or man.args.get(self.KEY_NS)
             or f"unknown/{self.Now()}"
         )
         kwargs[self.KEY_NS] = ns_name
         if self.KEY_META in kwargs:
-            man.head.user_meta = kwargs[self.KEY_META]
+            man.head().user_meta = kwargs[self.KEY_META]
         if self.KEY_MSG in kwargs:
-            man.head.message = kwargs[self.KEY_MSG]
+            man.head().message = kwargs[self.KEY_MSG]
 
         if not kwargs.get(self.KEY_NCP, False):
             man = self.translate_manifest(man, new_path, ns_name)
         self.registry.put(man, **kwargs)
         return man
 
     def translate_manifest(self, man: ResourceKey, path: Path, name: str) -> Manifest:
         """Translate entries from manifest into this Volume"""
         dest = str(self.path / name)
         entries = [entry.get(dest) for entry in man.list()]
-        Manifest.WriteToPath(man.head, entries, path)  # type: ignore
+        Manifest.WriteToPath(man.head(), entries, path)  # type: ignore
         return Manifest(path, **self.args)
```

### Comparing `quiltcore-0.3.0/quiltcore/yaml/codec.py` & `quiltcore-0.3.1/quiltcore/yaml/codec.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/yaml/config.py` & `quiltcore-0.3.1/quiltcore/yaml/config.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/yaml/quiltcore.yaml` & `quiltcore-0.3.1/quiltcore/yaml/quiltcore.yaml`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/yaml/quiltspec.yaml` & `quiltcore-0.3.1/quiltcore/yaml/quiltspec.yaml`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/quiltcore/yaml/spec.py` & `quiltcore-0.3.1/quiltcore/yaml/spec.py`

 * *Files identical despite different names*

### Comparing `quiltcore-0.3.0/PKG-INFO` & `quiltcore-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltcore
-Version: 0.3.0
+Version: 0.3.1
 Summary: low-level plubming to read/write Quilt packages
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

