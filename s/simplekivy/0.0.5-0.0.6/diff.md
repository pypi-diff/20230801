# Comparing `tmp/simplekivy-0.0.5.tar.gz` & `tmp/simplekivy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplekivy-0.0.5.tar", last modified: Thu Jul 20 16:19:01 2023, max compression
+gzip compressed data, was "simplekivy-0.0.6.tar", last modified: Tue Aug  1 13:28:26 2023, max compression
```

## Comparing `simplekivy-0.0.5.tar` & `simplekivy-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1058 2023-07-13 13:38:06.000000 simplekivy-0.0.5/LICENSE
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3383 2023-07-20 16:19:01.579148 simplekivy-0.0.5/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2830 2023-07-20 16:18:11.000000 simplekivy-0.0.5/README.md
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-20 16:10:44.000000 simplekivy-0.0.5/pyproject.toml
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-20 16:19:01.579148 simplekivy-0.0.5/setup.cfg
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/simplekivy/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.5/simplekivy/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      912 2023-07-16 11:59:18.000000 simplekivy-0.0.5/simplekivy/simplekivy.py
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/simplekivy/widgets/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       37 2023-07-16 11:58:18.000000 simplekivy-0.0.5/simplekivy/widgets/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3222 2023-07-20 16:06:46.000000 simplekivy-0.0.5/simplekivy/widgets/app.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.5/simplekivy/widgets/main.kv
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-20 16:19:01.579148 simplekivy-0.0.5/simplekivy.egg-info/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3383 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/SOURCES.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/dependency_links.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-20 16:19:01.000000 simplekivy-0.0.5/simplekivy.egg-info/top_level.txt
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-08-01 13:28:26.152305 simplekivy-0.0.6/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1058 2023-07-13 13:38:06.000000 simplekivy-0.0.6/LICENSE
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3383 2023-08-01 13:28:26.152305 simplekivy-0.0.6/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2830 2023-07-20 16:18:11.000000 simplekivy-0.0.6/README.md
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-08-01 13:22:58.000000 simplekivy-0.0.6/pyproject.toml
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-08-01 13:28:26.152305 simplekivy-0.0.6/setup.cfg
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-08-01 13:28:26.144305 simplekivy-0.0.6/simplekivy/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.6/simplekivy/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      912 2023-07-16 11:59:18.000000 simplekivy-0.0.6/simplekivy/simplekivy.py
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-08-01 13:28:26.152305 simplekivy-0.0.6/simplekivy/widgets/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       37 2023-07-16 11:58:18.000000 simplekivy-0.0.6/simplekivy/widgets/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3364 2023-08-01 13:24:48.000000 simplekivy-0.0.6/simplekivy/widgets/app.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.6/simplekivy/widgets/main.kv
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-08-01 13:28:26.152305 simplekivy-0.0.6/simplekivy.egg-info/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3383 2023-08-01 13:28:26.000000 simplekivy-0.0.6/simplekivy.egg-info/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-08-01 13:28:26.000000 simplekivy-0.0.6/simplekivy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-08-01 13:28:26.000000 simplekivy-0.0.6/simplekivy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-08-01 13:28:26.000000 simplekivy-0.0.6/simplekivy.egg-info/top_level.txt
```

### Comparing `simplekivy-0.0.5/LICENSE` & `simplekivy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.5/PKG-INFO` & `simplekivy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.5
+Version: 0.0.6
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplekivy-0.0.5/README.md` & `simplekivy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.5/pyproject.toml` & `simplekivy-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "simplekivy"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="yousuf", email="yosefmahmoud356@gmail.com" },
 ]
 description = "the idea is inspired by PySimpleGui , to quickly create simple kivy apps "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplekivy-0.0.5/simplekivy/simplekivy.py` & `simplekivy-0.0.6/simplekivy/simplekivy.py`

 * *Files identical despite different names*

### Comparing `simplekivy-0.0.5/simplekivy/widgets/app.py` & `simplekivy-0.0.6/simplekivy/widgets/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 file_path = os.path.abspath(os.path.dirname(__file__))
 print(file_path)
 Builder.load_file(os.path.join(file_path, "main.kv"))
 
 
 class AppMethods:
-    def freeze(self, wid, parent = None):
+    def freeze(self, wid, parent=None):
         type_wid = type(wid)
         
         #list for boxlayout
         if type_wid is list:
             parent = F.BoxLayout(orientation="horizontal")
             self.row_widget_adder(wid, parent)
             return parent
@@ -22,27 +22,25 @@
         elif type_wid is tuple:
             parent = F.FloatLayout()
             self.row_widget_adder(wid, parent) 
             return parent
 
         elif type_wid is dict:
             if parent:
-                self.row_widget_adder([wid], parent)
+                self.row_widget_adder_dict(wid, parent)
 
             else:
-                widgets = self.row_widget_adder([wid])
+                widgets = self.row_widget_adder_dict(wid)
                 return widgets
             
         elif type_wid is set:
-            
             if not parent:
                 return wid
             for i in wid:
-                if parent:
-                    self.row_widget_adder([i], parent)
+                self.row_widget_adder([i], parent)
 
         elif type_wid is str:
             widget = Builder.load_string(wid)
             return widget
 
         else:
             return wid
@@ -54,42 +52,53 @@
 
     def add_to_widget(self, widget, parent):
         try:
             parent.add_widget(widget()) 
         except TypeError:
             parent.add_widget(widget) 
 
+
+    def row_widget_adder_dict(self, item, parent=None):
+        if not parent:
+            dict_keys = []
+        items = item.copy().items()
+        for key, value in items:
+            if type(key) is not str :
+                try:keyI = key()  #keyI => keyInstance
+                except: keyI = key
+                wid = self.freeze(value, parent = keyI)
+                if wid:
+                    self.add_to_widget(wid, keyI)
+
+                if parent:
+                    self.add_to_widget(keyI, parent)
+                else:
+                    dict_keys.append(keyI)
+
+                del item[key]
+
+        parent.__init__(**item)
+        if not parent:
+            return dict_keys
+
+    def row_widget_adder_lists_str(self, item, parent=None):
+        wid = self.freeze(item)
+        self.add_to_widget(wid, parent)  
+
     def row_widget_adder(self, widofmainlist, parent=None):
         if not parent:
             dict_keys = []
         for item in widofmainlist:
             item_type = type(item)
+            
             if item_type is dict:
-                items = item.copy().items()
-                for key, value in items:
-                    if type(key) is not str :
-                        try:keyI = key()  #keyI => keyInstance
-                        except: keyI = key
-                        wid = self.freeze(value, parent = keyI)
-                        if wid:
-                            self.add_to_widget(wid, keyI)
-
-                        if parent:
-                            self.add_to_widget(keyI, parent)
-                        else:
-                            dict_keys.append(keyI)
-
-                        del item[key]
-
-                parent.__init__(**item)
-                if not parent:
-                    return dict_keys
+                wid = self.row_widget_adder_dict(item, parent=parent)
+
             elif item_type in (list, tuple, str):
-                wid = self.freeze(item)
-                self.add_to_widget(wid, parent)
+                self.row_widget_adder_lists_str(item, parent=parent)
 
             elif item_type is set:
                 self.freeze(item, parent=parent)
                     
 
             else:self.add_to_widget(item, parent)
 
@@ -100,11 +109,12 @@
         for widofmainlist in self.widgets:
             if type(widofmainlist) in (list, tuple,  str):
                 wid = self.freeze(widofmainlist)
                 self.add_to_root(wid)
 
             elif type(widofmainlist) is dict or set:
                 self.freeze(widofmainlist, parent=self.root)
+
             else:
                 self.add_to_root(widofmainlist)
```

### Comparing `simplekivy-0.0.5/simplekivy.egg-info/PKG-INFO` & `simplekivy-0.0.6/simplekivy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.5
+Version: 0.0.6
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

