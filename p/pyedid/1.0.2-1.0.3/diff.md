# Comparing `tmp/pyedid-1.0.2.tar.gz` & `tmp/pyedid-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedid-1.0.2.tar", last modified: Tue Mar 28 12:30:48 2023, max compression
+gzip compressed data, was "pyedid-1.0.3.tar", last modified: Tue Aug  1 09:17:27 2023, max compression
```

## Comparing `pyedid-1.0.2.tar` & `pyedid-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:30:48.912657 pyedid-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 12:30:34.000000 pyedid-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-28 12:30:48.912657 pyedid-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-28 12:30:34.000000 pyedid-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:30:48.908657 pyedid-1.0.2/pyedid/
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-28 12:30:34.000000 pyedid-1.0.2/pyedid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:30:48.912657 pyedid-1.0.2/pyedid/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-28 12:30:34.000000 pyedid-1.0.2/pyedid/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:30:48.912657 pyedid-1.0.2/pyedid/types/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-28 12:30:34.000000 pyedid-1.0.2/pyedid/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95651 2023-03-28 12:30:34.000000 pyedid-1.0.2/pyedid/types/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-28 12:30:34.000000 pyedid-1.0.2/pyedid/types/edid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-03-28 12:30:34.000000 pyedid-1.0.2/pyedid/types/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:30:48.912657 pyedid-1.0.2/pyedid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-28 12:30:48.000000 pyedid-1.0.2/pyedid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-28 12:30:48.000000 pyedid-1.0.2/pyedid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:30:48.000000 pyedid-1.0.2/pyedid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 12:30:48.000000 pyedid-1.0.2/pyedid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 12:30:48.000000 pyedid-1.0.2/pyedid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:30:48.912657 pyedid-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-28 12:30:34.000000 pyedid-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:27.967919 pyedid-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 09:17:16.000000 pyedid-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-01 09:17:27.967919 pyedid-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-01 09:17:16.000000 pyedid-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:27.963919 pyedid-1.0.3/pyedid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-01 09:17:16.000000 pyedid-1.0.3/pyedid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:27.967919 pyedid-1.0.3/pyedid/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-01 09:17:16.000000 pyedid-1.0.3/pyedid/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:27.967919 pyedid-1.0.3/pyedid/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-01 09:17:16.000000 pyedid-1.0.3/pyedid/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95651 2023-08-01 09:17:16.000000 pyedid-1.0.3/pyedid/types/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-01 09:17:16.000000 pyedid-1.0.3/pyedid/types/edid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-08-01 09:17:16.000000 pyedid-1.0.3/pyedid/types/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:17:27.967919 pyedid-1.0.3/pyedid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-01 09:17:27.000000 pyedid-1.0.3/pyedid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-01 09:17:27.000000 pyedid-1.0.3/pyedid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:17:27.000000 pyedid-1.0.3/pyedid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 09:17:27.000000 pyedid-1.0.3/pyedid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 09:17:27.000000 pyedid-1.0.3/pyedid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:17:27.967919 pyedid-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-01 09:17:16.000000 pyedid-1.0.3/setup.py
```

### Comparing `pyedid-1.0.2/LICENSE` & `pyedid-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyedid-1.0.2/PKG-INFO` & `pyedid-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyedid
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to parse extended display identification data (EDID)
 Home-page: https://github.com/dd4e/pyedid
 Author: Davydov Denis, Jonas Lieb
 Author-email: dadmoscow@gmail.com
 License: MIT
 Keywords: edid,xrandr,display,monitor
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyedid-1.0.2/README.md` & `pyedid-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyedid-1.0.2/pyedid/__init__.py` & `pyedid-1.0.3/pyedid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'Edid',
     'Registry',
     'DEFAULT_REGISTRY',
     'get_edid_from_xrandr_verbose',
     'parse_edid'
 )
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 
 def parse_edid(raw: Union[bytes, str], registry: Registry = DEFAULT_REGISTRY) -> Edid:
     '''Parse raw EDID and return parsed object
 
     :param raw: Raw edid value
     :param registry: Edid registry, default uses the DEFAULT_REGISTRY
@@ -84,14 +84,15 @@
                     serial = text
                 elif timing_type == 0xFC:
                     name = text
 
     return Edid(
         manufacturer_id = raw_edid.manu_id,
         manufacturer = registry.get_company_by_raw(raw_edid.manu_id),
+        manufacturer_pnp_id = registry.get_company_pnp_id(raw_edid.manu_id),
         product_id = raw_edid.prod_id,
         year = raw_edid.manu_year + 1990,
         week = raw_edid.manu_week,
         edid_version = '{:d}.{:d}'.format(raw_edid.edid_version, raw_edid.edid_revision),
         type = 'digital' if (raw_edid.input_type & 0xFF) else 'analog',
         width = float(raw_edid.width),
         height = float(raw_edid.height),
```

### Comparing `pyedid-1.0.2/pyedid/helpers/__init__.py` & `pyedid-1.0.3/pyedid/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedid-1.0.2/pyedid/types/default.py` & `pyedid-1.0.3/pyedid/types/default.py`

 * *Files identical despite different names*

### Comparing `pyedid-1.0.2/pyedid/types/edid.py` & `pyedid-1.0.3/pyedid/types/edid.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import List, NamedTuple, Optional, Tuple, Union
 
 
 class Edid(NamedTuple):
     '''Parsed EDID object'''
     manufacturer_id: int
     manufacturer: str
+    manufacturer_pnp_id: str
     product_id: int
     year: int
     week: int
     edid_version: str
     type: str
     width: float
     height: float
```

### Comparing `pyedid-1.0.2/pyedid/types/registry.py` & `pyedid-1.0.3/pyedid/types/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,15 +144,19 @@
             writer = csv.writer(f)
             writer.writerows(self.items())
 
     def get_company_by_pnp(self, pnp_id: str) -> str:
         '''Convert PNP id to company name or 'Unknown' if not found'''
         return self.get(pnp_id, self.__DEFAULT_NAME)
 
-    def get_company_by_raw(self, raw_id: int) -> str:
+    def get_company_pnp_id(self, raw_id: int) -> str:
         '''Convert raw edid value to company name or 'Unknown' if not found'''
         tmp = [(raw_id >> 10) & 31, (raw_id >> 5) & 31, raw_id & 31]
         try:
-            pnp_id = ''.join(string.ascii_uppercase[n-1] for n in tmp)
-            return self.get_company_by_pnp(pnp_id)
+            return ''.join(string.ascii_uppercase[n-1] for n in tmp)
         except IndexError:
             return self.__DEFAULT_NAME
+
+    def get_company_by_raw(self, raw_id: int) -> str:
+        '''Convert raw edid value to PNP ID or 'Unknown' if not found'''
+        pnp_id = self.get_company_pnp_id(raw_id)
+        return self.get_company_by_pnp(pnp_id)
```

### Comparing `pyedid-1.0.2/pyedid.egg-info/PKG-INFO` & `pyedid-1.0.3/pyedid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyedid
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to parse extended display identification data (EDID)
 Home-page: https://github.com/dd4e/pyedid
 Author: Davydov Denis, Jonas Lieb
 Author-email: dadmoscow@gmail.com
 License: MIT
 Keywords: edid,xrandr,display,monitor
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyedid-1.0.2/setup.py` & `pyedid-1.0.3/setup.py`

 * *Files identical despite different names*

