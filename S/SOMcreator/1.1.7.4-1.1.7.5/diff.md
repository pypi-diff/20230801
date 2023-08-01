# Comparing `tmp/SOMcreator-1.1.7.4.tar.gz` & `tmp/SOMcreator-1.1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.1.7.4.tar", last modified: Mon Jul 31 11:01:39 2023, max compression
+gzip compressed data, was "SOMcreator-1.1.7.5.tar", last modified: Tue Aug  1 13:40:46 2023, max compression
```

## Comparing `SOMcreator-1.1.7.4.tar` & `SOMcreator-1.1.7.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.561345 SOMcreator-1.1.7.4/
--rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.7.4/LICENSE
--rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.7.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1556 2023-07-31 11:01:39.561345 SOMcreator-1.1.7.4/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.7.4/README.md
--rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 11:01:39.562292 SOMcreator-1.1.7.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.325697 SOMcreator-1.1.7.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.355883 SOMcreator-1.1.7.4/src/SOMcreator/
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.446789 SOMcreator-1.1.7.4/src/SOMcreator/Template/
--rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.457950 SOMcreator-1.1.7.4/src/SOMcreator/Template/__pyinstaller/
--rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/bookmark_template.txt
--rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/ifc.json
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.511437 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/
--rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/end_ungetestet.js
--rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/mapping_template.txt
--rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/template.txt
--rw-rw-rw-   0        0        0      156 2023-07-31 10:59:21.000000 SOMcreator-1.1.7.4/src/SOMcreator/__init__.py
--rw-rw-rw-   0        0        0    24958 2023-07-26 15:19:58.000000 SOMcreator-1.1.7.4/src/SOMcreator/classes.py
--rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.4/src/SOMcreator/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.560329 SOMcreator-1.1.7.4/src/SOMcreator/external_software/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/allplan.py
--rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/card1.py
--rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/desite.py
--rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/excel.py
--rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/revit.py
--rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/vestra.py
--rw-rw-rw-   0        0        0     9379 2023-07-31 10:58:59.000000 SOMcreator-1.1.7.4/src/SOMcreator/filehandling.py
--rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/quality_check.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.398561 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/
--rw-rw-rw-   0        0        0     1556 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.143118 SOMcreator-1.1.7.5/
+-rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.7.5/LICENSE
+-rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.7.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1556 2023-08-01 13:40:46.143118 SOMcreator-1.1.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.7.5/README.md
+-rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 13:40:46.143118 SOMcreator-1.1.7.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:45.950706 SOMcreator-1.1.7.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:45.982642 SOMcreator-1.1.7.5/src/SOMcreator/
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.032310 SOMcreator-1.1.7.5/src/SOMcreator/Template/
+-rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.046231 SOMcreator-1.1.7.5/src/SOMcreator/Template/__pyinstaller/
+-rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/bookmark_template.txt
+-rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/ifc.json
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.088393 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/
+-rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/end_ungetestet.js
+-rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/mapping_template.txt
+-rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/template.txt
+-rw-rw-rw-   0        0        0      156 2023-08-01 12:16:35.000000 SOMcreator-1.1.7.5/src/SOMcreator/__init__.py
+-rw-rw-rw-   0        0        0    25758 2023-08-01 13:40:29.000000 SOMcreator-1.1.7.5/src/SOMcreator/classes.py
+-rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.5/src/SOMcreator/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.141953 SOMcreator-1.1.7.5/src/SOMcreator/external_software/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/__init__.py
+-rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/allplan.py
+-rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/card1.py
+-rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/desite.py
+-rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/excel.py
+-rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/revit.py
+-rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/vestra.py
+-rw-rw-rw-   0        0        0     9379 2023-07-31 10:58:59.000000 SOMcreator-1.1.7.5/src/SOMcreator/filehandling.py
+-rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/quality_check.py
+drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.008357 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/
+-rw-rw-rw-   0        0        0     1556 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.1.7.4/LICENSE` & `SOMcreator-1.1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/PKG-INFO` & `SOMcreator-1.1.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7.4
+Version: 1.1.7.5
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7.4/pyproject.toml` & `SOMcreator-1.1.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.1.7.5/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/end_ungetestet.js` & `SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/end_ungetestet.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.1.7.5/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/Template/template.txt` & `SOMcreator-1.1.7.5/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/classes.py` & `SOMcreator-1.1.7.5/src/SOMcreator/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,43 +20,44 @@
         return iter(sorted(list(self._registry), key=lambda x: x.name))
 
     def __len__(self) -> int:
         return len(self._registry)
 
 
 class Project(object):
-    def __init__(self, name: str = "", author: str|None = None) -> None:
+    def __init__(self, name: str = "", author: str | None = None) -> None:
         self._name = ""
         self._author = author
         self._version = "1.0.0"
-        self._changed = True        # indecates if project was modified -> used for close dialog
+        self._changed = True  # indecates if project was modified -> used for close dialog
         self.name = name
 
-    def get_uuid_dict(self) -> dict[str,Object|PropertySet|Attribute|Aggregation]:
+    def get_uuid_dict(self) -> dict[str, Object | PropertySet | Attribute | Aggregation]:
         pset_dict = {pset.uuid: pset for pset in PropertySet}
         object_dict = {obj.uuid: obj for obj in Object}
         attribute_dict = {attribute.uuid: attribute for attribute in Attribute}
         aggregation_dict = {aggreg.uuid: aggreg for aggreg in Aggregation}
         full_dict = pset_dict | object_dict | attribute_dict | aggregation_dict
         if None in full_dict:
             full_dict.pop(None)
         return full_dict
 
-    def get_element_by_uuid(self,uuid:str) -> Attribute|PropertySet|Object|Aggregation|None:
+    def get_element_by_uuid(self, uuid: str) -> Attribute | PropertySet | Object | Aggregation | None:
         if uuid is None:
             return None
         return self.get_uuid_dict().get(uuid)
 
-    def open(self,path) -> dict:
-        json_dict = filehandling.import_json(self,path)
+    def open(self, path) -> dict:
+        json_dict = filehandling.import_json(self, path)
         return json_dict
 
-    def save(self,path) -> dict:
-        json_dict = filehandling.export_json(self,path)
+    def save(self, path) -> dict:
+        json_dict = filehandling.export_json(self, path)
         return json_dict
+
     @property
     def changed(self) -> bool:
         def check_data():
             for obj in Object:
                 if obj.changed:
                     return True
             return False
@@ -142,14 +143,15 @@
         for n in root_objects:
             create_childen(n)
         return base
 
     def get_predefined_psets(self) -> set[PropertySet]:
         return set(pset for pset in PropertySet if pset.object == None)
 
+
 class Hirarchy(object, metaclass=IterRegistry):
 
     def __init__(self, name: str, description: str | None = None, optional: bool | None = None) -> None:
 
         self._parent = None
         self._children = set()
         self._name = name
@@ -163,15 +165,15 @@
             self.description = description
 
         self._optional = False
         if optional is not None:
             self._optional = optional
 
     @property
-    def optional_wo_hirarchy(self) ->bool:
+    def optional_wo_hirarchy(self) -> bool:
         return self._optional
 
     @property
     def optional(self) -> bool:
         if self.parent is not None:
             if self.parent.optional:
                 return True
@@ -188,14 +190,15 @@
         if self._description:
             return self._description
         return self.parent.description
 
     @description.setter
     def description(self, value):
         self._description = value
+
     @property
     def mapping_dict(self) -> dict[str, bool]:
         return self._mapping_dict
 
     @mapping_dict.setter
     def mapping_dict(self, value: dict[str, bool]) -> None:
         self._mapping_dict = value
@@ -255,17 +258,17 @@
 class PropertySet(Hirarchy):
     _registry: set[PropertySet] = set()
 
     def __init__(self, name: str, obj: Object = None, uuid: str = None, description: None | str = None,
                  optional: None | bool = None) -> None:
         super(PropertySet, self).__init__(name, description, optional)
         self._attributes = set()
-        self._object  = None
+        self._object = None
         if obj is not None:
-            obj.add_property_set(self)  #adds Pset to Object and sets pset.object = obj
+            obj.add_property_set(self)  # adds Pset to Object and sets pset.object = obj
         self._registry.add(self)
         self.uuid = uuid
         if self.uuid is None:
             self.uuid = str(uuid4())
         self.changed = True
 
     def __lt__(self, other):
@@ -389,26 +392,26 @@
 
 class Attribute(Hirarchy):
     _registry: set[Attribute] = set()
 
     def __init__(self, property_set: PropertySet | None, name: str, value: list, value_type: int,
                  data_type: str = "xs:string",
                  child_inherits_values: bool = False, uuid: str = None, description: None | str = None,
-                 optional: None | bool = None, revit_mapping: None|str = None):
+                 optional: None | bool = None, revit_mapping: None | str = None):
 
         super(Attribute, self).__init__(name, description, optional)
         self._value = value
         self._property_set = property_set
         self._value_type = value_type
         self._data_type = data_type
         self._registry.add(self)
         if revit_mapping is None:
             self._revit_name = name
         else:
-            self._revit_name  = revit_mapping
+            self._revit_name = revit_mapping
 
         self.changed = True
         self._child_inherits_values = child_inherits_values
         self.uuid = uuid
 
         if self.uuid is None:
             self.uuid = str(uuid4())
@@ -561,15 +564,15 @@
 
 
 class Object(Hirarchy):
     _registry: set[Object] = set()
 
     def __init__(self, name: str, ident_attrib: [Attribute, str], uuid: str = None,
                  ifc_mapping: set[str] | None = None, description: None | str = None,
-                 optional: None | bool = None,abbreviation:None|str = None) -> None:
+                 optional: None | bool = None, abbreviation: None | str = None) -> None:
         super(Object, self).__init__(name, description, optional)
         self._registry.add(self)
 
         self._scripts: list[Script] = list()
         self._property_sets: list[PropertySet] = list()
         self._ident_attrib = ident_attrib
         self._aggregations: set[Aggregation] = set()
@@ -592,19 +595,19 @@
     def __str__(self):
         return f"Object {self.name}"
 
     def __lt__(self, other: Object):
         return self.ident_value < other.ident_value
 
     @property
-    def abbreviation(self)-> str:
+    def abbreviation(self) -> str:
         return self._abbreviation
 
     @abbreviation.setter
-    def abbreviation(self,value)-> None:
+    def abbreviation(self, value) -> None:
         self._abbreviation = value
 
     @property
     def ifc_mapping(self) -> set[str]:
         return self._ifc_mapping
 
     @ifc_mapping.setter
@@ -734,16 +737,17 @@
 
 class Aggregation(Hirarchy):
     _registry: set[Aggregation] = set()
 
     def __str__(self):
         return self.name
 
-    def __init__(self, obj: Object, uuid: str | None = None, description: None | str = None,optional: None | bool = None):
-        super(Aggregation, self).__init__(obj.name, description,optional)
+    def __init__(self, obj: Object, uuid: str | None = None, description: None | str = None,
+                 optional: None | bool = None):
+        super(Aggregation, self).__init__(obj.name, description, optional)
         self._registry.add(self)
         if uuid is None:
             self.uuid = str(uuid4())
         else:
             self.uuid = str(uuid)
         self.object = obj
         self._parent: Aggregation | None = None
@@ -765,41 +769,68 @@
         :return:
         """
         if self.parent is None:
             return 0
 
         return self.parent.connection_dict[self]
 
-    def add_child(self, child: Aggregation, connection_type: int = constants.AGGREGATION) -> Aggregation:
+    def add_child(self, child: Aggregation, connection_type: int = constants.AGGREGATION) -> bool:
+        """returns if adding child is allowed"""
+
+        def loop_parents(element, search_value):
+            if element.parent is None:
+                return True
+            if element.parent.object == search_value:
+                return False
+            else:
+                return loop_parents(element.parent, search_value)
+
+        if child.object == self.object:
+            return False
+
+        if not loop_parents(self, child.object):
+            return False
+
+        if not child.set_parent(self, connection_type):
+            return False
+
         self.children.add(child)
-        child.set_parent(self, connection_type)
         self.connection_dict[child] = connection_type
-        return child
+        return True
 
     @property
     def parent(self) -> Aggregation:
         return self._parent
 
-    def set_parent(self, value: Aggregation, connection_type: int) -> None:
-        if self.parent is not None:
-            self.connection_dict.pop(self.parent)
+    def set_parent(self, value: Aggregation, connection_type: int) -> bool:
+        if self.parent is not None and value != self._parent:
+            return False
+            # self.connection_dict.pop(self.parent)
+
         self._parent = value
         self.connection_dict[value] = connection_type
+        return True
+
+    def remove_parent(self):
+        if self in self.parent.children:
+            self.parent.children.remove(self)
+        self._parent = None
 
     @property
     def is_root(self):
         return not self.parent
 
     def id_group(self) -> str:
         own_text = f"{self.object.abbreviation}_xxx"
         if self.is_root:
             return own_text
         else:
             return f"{self.parent.id_group()}_{own_text}"
 
+
 class Script():
     def __init__(self, title: str, obj: Object) -> None:
         self.code = str()
         self.changed = True
         self._object = obj
         obj.add_script(self)
         self._name = title
```

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/constants.py` & `SOMcreator-1.1.7.5/src/SOMcreator/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.1.7.5/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.1.7.5/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/external_software/desite.py` & `SOMcreator-1.1.7.5/src/SOMcreator/external_software/desite.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.1.7.5/src/SOMcreator/external_software/excel.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.1.7.5/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.1.7.5/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/filehandling.py` & `SOMcreator-1.1.7.5/src/SOMcreator/filehandling.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator/quality_check.py` & `SOMcreator-1.1.7.5/src/SOMcreator/quality_check.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.1.7.5/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7.4
+Version: 1.1.7.5
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7.4/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.1.7.5/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

