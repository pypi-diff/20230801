# Comparing `tmp/sk_table_handler-0.0.1.tar.gz` & `tmp/sk_table_handler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_table_handler-0.0.1.tar", last modified: Fri Jul 28 16:11:41 2023, max compression
+gzip compressed data, was "sk_table_handler-0.0.2.tar", last modified: Tue Aug  1 17:21:10 2023, max compression
```

## Comparing `sk_table_handler-0.0.1.tar` & `sk_table_handler-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 16:11:41.845071 sk_table_handler-0.0.1/
--rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_table_handler-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     7595 2023-07-28 16:11:41.845071 sk_table_handler-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7117 2023-07-18 15:19:22.000000 sk_table_handler-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 16:11:41.845071 sk_table_handler-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-07-28 15:57:34.000000 sk_table_handler-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:11:41.845071 sk_table_handler-0.0.1/sk_table_handler.egg-info/
--rw-rw-rw-   0        0        0     7595 2023-07-28 16:11:41.000000 sk_table_handler-0.0.1/sk_table_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-28 16:11:41.000000 sk_table_handler-0.0.1/sk_table_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 16:11:41.000000 sk_table_handler-0.0.1/sk_table_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-28 16:11:41.000000 sk_table_handler-0.0.1/sk_table_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 16:11:41.000000 sk_table_handler-0.0.1/sk_table_handler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-28 16:11:41.845071 sk_table_handler-0.0.1/sk_table_hanlder/
--rw-rw-rw-   0        0        0     5041 2023-07-28 13:55:54.000000 sk_table_handler-0.0.1/sk_table_hanlder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:21:10.245469 sk_table_handler-0.0.2/
+-rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_table_handler-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     7595 2023-08-01 17:21:10.244471 sk_table_handler-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2023-07-18 15:19:22.000000 sk_table_handler-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:21:10.245469 sk_table_handler-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-08-01 17:21:00.000000 sk_table_handler-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:21:10.242474 sk_table_handler-0.0.2/sk_table_handler.egg-info/
+-rw-rw-rw-   0        0        0     7595 2023-08-01 17:21:10.000000 sk_table_handler-0.0.2/sk_table_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-08-01 17:21:10.000000 sk_table_handler-0.0.2/sk_table_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:21:10.000000 sk_table_handler-0.0.2/sk_table_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 17:21:10.000000 sk_table_handler-0.0.2/sk_table_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 17:21:10.000000 sk_table_handler-0.0.2/sk_table_handler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 17:21:10.243472 sk_table_handler-0.0.2/sk_table_hanlder/
+-rw-rw-rw-   0        0        0     5461 2023-08-01 17:11:04.000000 sk_table_handler-0.0.2/sk_table_hanlder/__init__.py
```

### Comparing `sk_table_handler-0.0.1/LICENSE.txt` & `sk_table_handler-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_table_handler-0.0.1/PKG-INFO` & `sk_table_handler-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk_table_handler
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_table_handler-0.0.1/README.md` & `sk_table_handler-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sk_table_handler-0.0.1/setup.py` & `sk_table_handler-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_table_handler',
-    version='0.0.1',
+    version='0.0.2',
     description='A simple calculator program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
     install_requires=['regex'],
```

### Comparing `sk_table_handler-0.0.1/sk_table_handler.egg-info/PKG-INFO` & `sk_table_handler-0.0.2/sk_table_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-table-handler
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_table_handler-0.0.1/sk_table_hanlder/__init__.py` & `sk_table_handler-0.0.2/sk_table_hanlder/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         self.data = {}
 
     def get_data(self,variable_declarations):
         data = {}
         pattern = '(\$\w+)\s*=\s*([^=;]+)\;'
         matches = re.findall(pattern,variable_declarations)
         for variable,value in matches:
-            data[variable] = eval(value)
+            data[variable] = eval(value) if 'eval' not in value else value
         return data
 
     def solve_table(self,data,declarations):
         pattern = r'(\$\w+)\s*=\s*((\$\w+)\s*\((\w+)\)\s*=>\s*(\((.*?)\))?\s*(\{(([^{}]|(?7))*)\}))'
 
         matches = re.findall(pattern,declarations)
         replace = ''
@@ -30,20 +30,22 @@
             value = self.get_table_value(data,template_variable,variable,placeholder,condition,return_value)
 
             declarations = re.sub(re.escape(replace),str(value),declarations)
 
         return declarations
 
 
-    def run(self,variable_declarations):
+    def process(self,variable_declarations):
+
+        procced_table = self.process_table(variable_declarations)
 
         data = self.get_data(variable_declarations)
 
 
-        declaration_text = self.solve_table(data,variable_declarations)
+        declaration_text = self.solve_table(data,procced_table)
 
 
         return declaration_text
 
 
     def get_table_value(self,data_stucture,template_variable,variable,placeholder,condition,return_value):
 
@@ -60,15 +62,16 @@
 
             exec(f"{placeholder} = value")
             if condition =='' or eval(f"{condition}"):
                 item =return_value
                 item = self.index_process(item)
                 item = self.process_ref(item,index,parent_index,list_len)
                 item = self.put_value(data_stucture,item)
-                item = eval(item)
+
+                item = eval(item) if 'eval' not in item else item
                 result.append(item)
                 data_stucture.update({variable : result})
                 index = index+1
 
 
         return result
 
@@ -100,19 +103,22 @@
         pattern = r'\[([^\[\]]+)\]'
         matches = re.findall(pattern,text)
         for match in matches:
             if eval(f"type({match})==int and ({match}<=-1 or {match}>={list_len})"):
                 return False
         return True
 
+    def process_table(self,declarations):
+        declarations  = re.sub(r'(\$)<(\w+)>',lambda catch: catch[1]+catch[2],declarations)
+        return declarations
+##$table3 = $<table1,table2>(x,y:x.item=y.item)=>{ 'name' : x.item , 'cost' : x.quantity*y.price ,'unit' : x.unit };
 
-
-
+##
 ##variables = '''
 ##        $table= [{'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}, {'number': 1}, {'number': 0}];
-##        $table2 = $table(x)=>{ {'number' : $table<[$parent_index-1].number|1>+$table<[$parent_index+1].number|1> } };'''
+##        $table2 = $<table>(x)=>{ {'number' : $table<[$parent_index-1].number|1>+$table<[$parent_index+1].number|1> } };'''
 ##table = TableHandler()
 ##
-##print(table.run(variables))
-##
+##print(table.process(variables))
+
```

