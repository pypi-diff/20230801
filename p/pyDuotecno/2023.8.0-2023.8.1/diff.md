# Comparing `tmp/pyDuotecno-2023.8.0.tar.gz` & `tmp/pyDuotecno-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDuotecno-2023.8.0.tar", last modified: Tue Aug  1 10:39:00 2023, max compression
+gzip compressed data, was "pyDuotecno-2023.8.1.tar", last modified: Tue Aug  1 18:30:04 2023, max compression
```

## Comparing `pyDuotecno-2023.8.0.tar` & `pyDuotecno-2023.8.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:39:00.976965 pyDuotecno-2023.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 10:39:00.976965 pyDuotecno-2023.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:39:00.976965 pyDuotecno-2023.8.0/duotecno/
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/duotecno/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/duotecno/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/duotecno/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/duotecno/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/duotecno/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:39:00.976965 pyDuotecno-2023.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/examples/read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:39:00.976965 pyDuotecno-2023.8.0/pyDuotecno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 10:39:00.000000 pyDuotecno-2023.8.0/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 10:39:00.000000 pyDuotecno-2023.8.0/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:39:00.000000 pyDuotecno-2023.8.0/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:39:00.000000 pyDuotecno-2023.8.0/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 10:39:00.000000 pyDuotecno-2023.8.0/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:39:00.976965 pyDuotecno-2023.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 10:38:49.000000 pyDuotecno-2023.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/duotecno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/duotecno/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/pyDuotecno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 18:30:04.000000 pyDuotecno-2023.8.1/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:30:04.904312 pyDuotecno-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 18:29:54.000000 pyDuotecno-2023.8.1/setup.py
```

### Comparing `pyDuotecno-2023.8.0/LICENSE` & `pyDuotecno-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.8.0/PKG-INFO` & `pyDuotecno-2023.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.8.0
+Version: 2023.8.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.8.0/duotecno/controller.py` & `pyDuotecno-2023.8.1/duotecno/controller.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.8.0/duotecno/node.py` & `pyDuotecno-2023.8.1/duotecno/node.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.8.0/duotecno/protocol.py` & `pyDuotecno-2023.8.1/duotecno/protocol.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.8.0/duotecno/unit.py` & `pyDuotecno-2023.8.1/duotecno/unit.py`

 * *Files 13% similar despite different names*

```diff
@@ -92,14 +92,35 @@
 
     async def handlePacket(self, packet) -> None:
         if isinstance(packet, EV_UNITDIMSTATUS_0):
             await self._update({"state": packet.state, "value": packet.dimValue})
             return
         await super().handlePacket(packet)
 
+    def is_on(self) -> int:
+        if self._state == 0:
+            return 0
+        return 1
+
+    def get_dimmer_state(self) -> int:
+        return self._value
+
+    async def set_dimmer_state(self, value: int | None = None) -> None:
+        # first send on
+        if value and value > 0:
+            # set state and turn on
+            await self.writer(f"[162,3,{self.node.address},{self.unit},{value}]")
+            await self.writer(f"[162,10,{self.node.address},{self.unit}]")
+        elif value or self._state == 1:
+            # turn off
+            await self.writer(f"[162,9,{self.node.address},{self.unit}]")
+        else:
+            # send turn on (restore state)
+            await self.writer(f"[162,10,{self.node.address},{self.unit}]")
+
 
 class SwitchUnit(BaseUnit):
     _unitType: final = 2
     _state: int = None
 
     async def handlePacket(self, packet) -> None:
         if isinstance(packet, EV_UNITSWITCHSTATUS_0):
```

### Comparing `pyDuotecno-2023.8.0/pyDuotecno.egg-info/PKG-INFO` & `pyDuotecno-2023.8.1/pyDuotecno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.8.0
+Version: 2023.8.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.8.0/pyproject.toml` & `pyDuotecno-2023.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "pyDuotecno"
 license = {text = "Apache"}
-version = "2023.8.0"
+version = "2023.8.1"
 description = "Open-source home automation platform running on Python 3."
 readme = "README.md"
 authors = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords = ["home", "duotecno", "automation"]
 classifiers = [
@@ -34,18 +34,18 @@
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
-exclude = ["tests", "tests.*"]
+exclude = ["tests", "tests.*", "examples", "examples/*"]
 
 [tool.bumpver]
-current_version = "2023.8.0"
+current_version = "2023.8.1"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

