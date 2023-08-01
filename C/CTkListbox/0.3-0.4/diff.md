# Comparing `tmp/CTkListbox-0.3.tar.gz` & `tmp/CTkListbox-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkListbox-0.3.tar", last modified: Mon Jul 10 16:29:18 2023, max compression
+gzip compressed data, was "CTkListbox-0.4.tar", last modified: Tue Aug  1 15:19:16 2023, max compression
```

## Comparing `CTkListbox-0.3.tar` & `CTkListbox-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 16:29:18.140320 CTkListbox-0.3/
-drwxrwxrwx   0        0        0        0 2023-07-10 16:29:18.073315 CTkListbox-0.3/CTkListbox/
--rw-rw-rw-   0        0        0      190 2023-07-10 16:27:56.000000 CTkListbox-0.3/CTkListbox/__init__.py
--rw-rw-rw-   0        0        0     6599 2023-07-10 16:26:42.000000 CTkListbox-0.3/CTkListbox/ctk_listbox.py
-drwxrwxrwx   0        0        0        0 2023-07-10 16:29:18.137319 CTkListbox-0.3/CTkListbox.egg-info/
--rw-rw-rw-   0        0        0     2764 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-10 16:29:18.000000 CTkListbox-0.3/CTkListbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 16:29:17.000000 CTkListbox-0.3/CTkListbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkListbox-0.3/LICENSE
--rw-rw-rw-   0        0        0     2764 2023-07-10 16:29:18.140320 CTkListbox-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2187 2023-07-06 12:24:22.000000 CTkListbox-0.3/README.md
--rw-rw-rw-   0        0        0      527 2023-07-10 16:29:18.146322 CTkListbox-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-07-10 16:28:10.000000 CTkListbox-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:19:16.076705 CTkListbox-0.4/
+drwxrwxrwx   0        0        0        0 2023-08-01 15:19:16.061076 CTkListbox-0.4/CTkListbox/
+-rw-rw-rw-   0        0        0      190 2023-08-01 15:14:46.000000 CTkListbox-0.4/CTkListbox/__init__.py
+-rw-rw-rw-   0        0        0     7640 2023-08-01 15:12:29.000000 CTkListbox-0.4/CTkListbox/ctk_listbox.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:19:16.076705 CTkListbox-0.4/CTkListbox.egg-info/
+-rw-rw-rw-   0        0        0     2917 2023-08-01 15:19:15.000000 CTkListbox-0.4/CTkListbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-08-01 15:19:16.000000 CTkListbox-0.4/CTkListbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 15:19:15.000000 CTkListbox-0.4/CTkListbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-01 15:19:15.000000 CTkListbox-0.4/CTkListbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-01 15:19:15.000000 CTkListbox-0.4/CTkListbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkListbox-0.4/LICENSE
+-rw-rw-rw-   0        0        0     2917 2023-08-01 15:19:16.076705 CTkListbox-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2334 2023-08-01 15:18:27.000000 CTkListbox-0.4/README.md
+-rw-rw-rw-   0        0        0      527 2023-08-01 15:19:16.076705 CTkListbox-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2023-08-01 15:18:48.000000 CTkListbox-0.4/setup.py
```

### Comparing `CTkListbox-0.3/CTkListbox.egg-info/PKG-INFO` & `CTkListbox-0.4/CTkListbox.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkListbox
-Version: 0.3
+Version: 0.4
 Summary: Customtkinter Listbox widget
 Home-page: https://github.com/Akascape/CTkListbox
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,listbox-widget,listbox,modern-listbox,option menu,list-box
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -66,16 +66,22 @@
 | multiple_selection | select multiple options in the listbox, `default=False`|
 | *other_parameters | _all other parameters of ctk_scrollable frame can be passed_ |
 
 ## Methods
 - **.insert(index, option)**
    add a option to the listbox
 - **.get()**
-   get the selected/index option
+   get the selected options
 - **.delete(index)**
    delete a option from the listbox
 - **.size()**
    get the size of the listbox
+- **.activate(index)**
+  activate an option
+- **.deactivae(index)**
+  deactivate any option
+- **.curselection()**
+  returns indexes of selected options
 - **.configure()**
    change some parameters for the listbox
   
 ### Thanks for visiting! Hope it will help :)
```

### Comparing `CTkListbox-0.3/LICENSE` & `CTkListbox-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkListbox-0.3/PKG-INFO` & `CTkListbox-0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkListbox
-Version: 0.3
+Version: 0.4
 Summary: Customtkinter Listbox widget
 Home-page: https://github.com/Akascape/CTkListbox
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,listbox-widget,listbox,modern-listbox,option menu,list-box
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
@@ -66,16 +66,22 @@
 | multiple_selection | select multiple options in the listbox, `default=False`|
 | *other_parameters | _all other parameters of ctk_scrollable frame can be passed_ |
 
 ## Methods
 - **.insert(index, option)**
    add a option to the listbox
 - **.get()**
-   get the selected/index option
+   get the selected options
 - **.delete(index)**
    delete a option from the listbox
 - **.size()**
    get the size of the listbox
+- **.activate(index)**
+  activate an option
+- **.deactivae(index)**
+  deactivate any option
+- **.curselection()**
+  returns indexes of selected options
 - **.configure()**
    change some parameters for the listbox
   
 ### Thanks for visiting! Hope it will help :)
```

### Comparing `CTkListbox-0.3/README.md` & `CTkListbox-0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -51,16 +51,22 @@
 | multiple_selection | select multiple options in the listbox, `default=False`|
 | *other_parameters | _all other parameters of ctk_scrollable frame can be passed_ |
 
 ## Methods
 - **.insert(index, option)**
    add a option to the listbox
 - **.get()**
-   get the selected/index option
+   get the selected options
 - **.delete(index)**
    delete a option from the listbox
 - **.size()**
    get the size of the listbox
+- **.activate(index)**
+  activate an option
+- **.deactivae(index)**
+  deactivate any option
+- **.curselection()**
+  returns indexes of selected options
 - **.configure()**
    change some parameters for the listbox
   
 ### Thanks for visiting! Hope it will help :)
```

### Comparing `CTkListbox-0.3/setup.cfg` & `CTkListbox-0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4c69 7374 626f 780d 0a76   = CTkListbox..v
-00000020: 6572 7369 6f6e 203d 2030 2e33 0d0a 6465  ersion = 0.3..de
+00000020: 6572 7369 6f6e 203d 2030 2e34 0d0a 6465  ersion = 0.4..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 4c69 7374 626f  omtkinter Listbo
 00000050: 7820 7769 6467 6574 0d0a 6c6f 6e67 5f64  x widget..long_d
 00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000090: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
```

### Comparing `CTkListbox-0.3/setup.py` & `CTkListbox-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkListbox',
-    version = '0.3',
+    version = '0.4',
     description = "Customtkinter Listbox widget",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkListbox",
```

