# Comparing `tmp/SOMcreator-1.1.7.5.tar.gz` & `tmp/SOMcreator-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.1.7.5.tar", last modified: Tue Aug  1 13:40:46 2023, max compression
+gzip compressed data, was "SOMcreator-1.1.8.tar", last modified: Tue Aug  1 15:29:36 2023, max compression
```

## Comparing `SOMcreator-1.1.7.5.tar` & `SOMcreator-1.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.143118 SOMcreator-1.1.7.5/
--rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.7.5/LICENSE
--rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.7.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1556 2023-08-01 13:40:46.143118 SOMcreator-1.1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.7.5/README.md
--rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.7.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 13:40:46.143118 SOMcreator-1.1.7.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:45.950706 SOMcreator-1.1.7.5/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:45.982642 SOMcreator-1.1.7.5/src/SOMcreator/
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.032310 SOMcreator-1.1.7.5/src/SOMcreator/Template/
--rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.046231 SOMcreator-1.1.7.5/src/SOMcreator/Template/__pyinstaller/
--rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/bookmark_template.txt
--rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/ifc.json
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.088393 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/
--rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/end_ungetestet.js
--rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/mapping_template.txt
--rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/Template/template.txt
--rw-rw-rw-   0        0        0      156 2023-08-01 12:16:35.000000 SOMcreator-1.1.7.5/src/SOMcreator/__init__.py
--rw-rw-rw-   0        0        0    25758 2023-08-01 13:40:29.000000 SOMcreator-1.1.7.5/src/SOMcreator/classes.py
--rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.5/src/SOMcreator/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.141953 SOMcreator-1.1.7.5/src/SOMcreator/external_software/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/allplan.py
--rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/card1.py
--rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/desite.py
--rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/excel.py
--rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/revit.py
--rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/external_software/vestra.py
--rw-rw-rw-   0        0        0     9379 2023-07-31 10:58:59.000000 SOMcreator-1.1.7.5/src/SOMcreator/filehandling.py
--rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.5/src/SOMcreator/quality_check.py
-drwxrwxrwx   0        0        0        0 2023-08-01 13:40:46.008357 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/
--rw-rw-rw-   0        0        0     1556 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 13:40:45.000000 SOMcreator-1.1.7.5/src/SOMcreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.344247 SOMcreator-1.1.8/
+-rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1554 2023-08-01 15:29:36.344247 SOMcreator-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.8/README.md
+-rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 15:29:36.344247 SOMcreator-1.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.154034 SOMcreator-1.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.183826 SOMcreator-1.1.8/src/SOMcreator/
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.251649 SOMcreator-1.1.8/src/SOMcreator/Template/
+-rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.8/src/SOMcreator/Template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.263422 SOMcreator-1.1.8/src/SOMcreator/Template/__pyinstaller/
+-rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/bookmark_template.txt
+-rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/ifc.json
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.294165 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/
+-rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/end_ungetestet.js
+-rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/mapping_template.txt
+-rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/template.txt
+-rw-rw-rw-   0        0        0      154 2023-08-01 15:29:19.000000 SOMcreator-1.1.8/src/SOMcreator/__init__.py
+-rw-rw-rw-   0        0        0    24554 2023-08-01 15:26:46.000000 SOMcreator-1.1.8/src/SOMcreator/classes.py
+-rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.8/src/SOMcreator/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.343251 SOMcreator-1.1.8/src/SOMcreator/external_software/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/__init__.py
+-rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/allplan.py
+-rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/card1.py
+-rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/desite.py
+-rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/excel.py
+-rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/revit.py
+-rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/vestra.py
+-rw-rw-rw-   0        0        0     9397 2023-08-01 15:25:56.000000 SOMcreator-1.1.8/src/SOMcreator/filehandling.py
+-rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/quality_check.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.217166 SOMcreator-1.1.8/src/SOMcreator.egg-info/
+-rw-rw-rw-   0        0        0     1554 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.1.7.5/LICENSE` & `SOMcreator-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/PKG-INFO` & `SOMcreator-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7.5
+Version: 1.1.8
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7.5/pyproject.toml` & `SOMcreator-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.1.8/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/end_ungetestet.js` & `SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/end_ungetestet.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.1.8/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/Template/template.txt` & `SOMcreator-1.1.8/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/classes.py` & `SOMcreator-1.1.8/src/SOMcreator/classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -568,15 +568,14 @@
 
     def __init__(self, name: str, ident_attrib: [Attribute, str], uuid: str = None,
                  ifc_mapping: set[str] | None = None, description: None | str = None,
                  optional: None | bool = None, abbreviation: None | str = None) -> None:
         super(Object, self).__init__(name, description, optional)
         self._registry.add(self)
 
-        self._scripts: list[Script] = list()
         self._property_sets: list[PropertySet] = list()
         self._ident_attrib = ident_attrib
         self._aggregations: set[Aggregation] = set()
         self.custom_attribues = {}
 
         self._abbreviation = abbreviation
         if abbreviation is None:
@@ -621,22 +620,22 @@
     def add_ifc_map(self, value: str) -> None:
         self._ifc_mapping.add(value)
 
     def remove_ifc_map(self, value: str) -> None:
         self._ifc_mapping.remove(value)
 
     @property
-    def aggregation_representations(self) -> set[Aggregation]:  # Todo: add nodes functionality to graphs_window
+    def aggregations(self) -> set[Aggregation]:
         return self._aggregations
 
-    def add_aggregation_representation(self, node: Aggregation) -> None:
+    def add_aggregation(self, node: Aggregation) -> None:
         self._aggregations.add(node)
 
-    def remove_aggregation_representation(self, node: Aggregation) -> None:
-        self.aggregation_representations.remove(node)
+    def remove_aggregation(self, node: Aggregation) -> None:
+        self.aggregations.remove(node)
 
     @property
     def inherited_property_sets(self) -> dict[Object, list[PropertySet]]:
         def recursion(recursion_property_sets, recursion_obj: Object):
             psets = recursion_obj.property_sets
 
             if psets:
@@ -699,31 +698,21 @@
             attributes += property_set.attributes
 
         if inherit:
             attributes += self.parent.get_attributes(inherit=True)
 
         return attributes
 
-    @property
-    def scripts(self) -> list[Script]:
-        return self._scripts
-
-    def add_script(self, script: Script) -> None:
-        self._scripts.append(script)
-
-    def delete_script(self, script: Script) -> None:
-        self._scripts.remove(script)
-
     def delete(self) -> None:
         Object._registry.remove(self)
         pset: PropertySet
         for pset in self.property_sets:
             pset.delete()
 
-        for aggregation in self.aggregation_representations.copy():
+        for aggregation in self.aggregations.copy():
             aggregation.delete()
 
     def get_property_set_by_name(self, property_set_name: str) -> PropertySet | None:
         for property_set in self.property_sets:
             if property_set.name == property_set_name:
                 return property_set
         return None
@@ -737,45 +726,57 @@
 
 class Aggregation(Hirarchy):
     _registry: set[Aggregation] = set()
 
     def __str__(self):
         return self.name
 
-    def __init__(self, obj: Object, uuid: str | None = None, description: None | str = None,
-                 optional: None | bool = None):
+    def __init__(self, obj: Object, parent_connection=constants.AGGREGATION, uuid: str | None = None,
+                 description: None | str = None,
+                 optional: None | bool = None, ):
         super(Aggregation, self).__init__(obj.name, description, optional)
         self._registry.add(self)
         if uuid is None:
             self.uuid = str(uuid4())
         else:
             self.uuid = str(uuid)
         self.object = obj
         self._parent: Aggregation | None = None
-        self.connection_dict: dict[Aggregation, int] = dict()
-
-        self.object.add_aggregation_representation(self)
+        self._parent_connection = parent_connection
+        self.object.add_aggregation(self)
 
     def delete(self) -> None:
         super(Aggregation, self).delete()
-        self.object.remove_aggregation_representation(self)
+        self.object.remove_aggregation(self)
+        self.parent.children.remove(self)
+        for child in self.children:
+            child.parent = None
 
     @property
-    def parent_connection(self) -> int:
-        """
-        NO PARENT = 0
-        AGGREGATION = 1
-        INHERITANCE = 2
-        AGGREGATION+INHERITANCE =3
-        :return:
-        """
-        if self.parent is None:
-            return 0
+    def parent_connection(self):
+        return self._parent_connection
+
+    @parent_connection.setter
+    def parent_connection(self, value):
+        self._parent_connection = value
+
+    @property
+    def parent(self) -> Aggregation:
+        return self._parent
+
+    def set_parent(self, value, connection_type):
+        if self.parent is not None and value != self.parent:
+            return False
+        self._parent = value
+        self._parent_connection = connection_type
+        return True
 
-        return self.parent.connection_dict[self]
+    def remove_parent(self):
+        self.parent.children.remove(self)
+        self._parent = None
 
     def add_child(self, child: Aggregation, connection_type: int = constants.AGGREGATION) -> bool:
         """returns if adding child is allowed"""
 
         def loop_parents(element, search_value):
             if element.parent is None:
                 return True
@@ -790,67 +791,22 @@
         if not loop_parents(self, child.object):
             return False
 
         if not child.set_parent(self, connection_type):
             return False
 
         self.children.add(child)
-        self.connection_dict[child] = connection_type
-        return True
-
-    @property
-    def parent(self) -> Aggregation:
-        return self._parent
-
-    def set_parent(self, value: Aggregation, connection_type: int) -> bool:
-        if self.parent is not None and value != self._parent:
-            return False
-            # self.connection_dict.pop(self.parent)
-
-        self._parent = value
-        self.connection_dict[value] = connection_type
+        child.parent_connection = connection_type
         return True
 
-    def remove_parent(self):
-        if self in self.parent.children:
-            self.parent.children.remove(self)
-        self._parent = None
-
     @property
     def is_root(self):
-        return not self.parent
+        if self.parent is None:
+            return True
+        return False
 
     def id_group(self) -> str:
         own_text = f"{self.object.abbreviation}_xxx"
         if self.is_root:
             return own_text
         else:
-            return f"{self.parent.id_group()}_{own_text}"
-
-
-class Script():
-    def __init__(self, title: str, obj: Object) -> None:
-        self.code = str()
-        self.changed = True
-        self._object = obj
-        obj.add_script(self)
-        self._name = title
-
-    @property
-    def object(self) -> Object:
-        return self._object
-
-    @object.setter
-    def object(self, value: Object) -> None:
-        self._object.delete_script(self)
-        self._object = value
-        value.add_script(self)
-        self.changed = True
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @name.setter
-    def name(self, value: str) -> None:
-        self._name = value
-        self.changed = True
+            return f"{self.parent.id_group()}_{own_text}"
```

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/constants.py` & `SOMcreator-1.1.8/src/SOMcreator/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.1.8/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.1.8/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/external_software/desite.py` & `SOMcreator-1.1.8/src/SOMcreator/external_software/desite.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.1.8/src/SOMcreator/external_software/excel.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.1.8/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.1.8/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/filehandling.py` & `SOMcreator-1.1.8/src/SOMcreator/filehandling.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 uuid_dict[uuid].add_child(element)
 
     def load_aggregation(aggregation_dict: dict, identifier: str, ):
         name, description, optional, parent = load_basics(aggregation_dict)
         object_uuid = aggregation_dict[constants.OBJECT]
         obj = project.get_element_by_uuid(object_uuid)
         parent_connection = aggregation_dict[constants.CONNECTION]
-        aggregation = classes.Aggregation(obj, identifier, description, optional)
+        aggregation = classes.Aggregation(obj,parent_connection, identifier, description, optional)
         aggregation_parent_dict[aggregation] = (parent, parent_connection)
 
     def build_aggregation_structure():
         for aggregation, (uuid, connection_type) in aggregation_parent_dict.items():
             parent = project.get_element_by_uuid(uuid)
             if parent is not None:
                 parent.add_child(aggregation,connection_type)
```

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator/quality_check.py` & `SOMcreator-1.1.8/src/SOMcreator/quality_check.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.1.8/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7.5
+Version: 1.1.8
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7.5/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.1.8/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

