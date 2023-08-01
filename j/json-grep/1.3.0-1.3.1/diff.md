# Comparing `tmp/json-grep-1.3.0.tar.gz` & `tmp/json-grep-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-grep-1.3.0.tar", last modified: Wed Jul 26 09:41:31 2023, max compression
+gzip compressed data, was "json-grep-1.3.1.tar", last modified: Tue Aug  1 12:48:37 2023, max compression
```

## Comparing `json-grep-1.3.0.tar` & `json-grep-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.3.0/MANIFEST.in
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1974 2023-07-26 09:41:31.294892 json-grep-1.3.0/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1553 2023-07-26 09:40:21.000000 json-grep-1.3.0/README.md
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/json_grep.egg-info/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1974 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      396 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/SOURCES.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/dependency_links.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/entry_points.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/not-zip-safe
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/top_level.txt
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/jsongrep/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-07-26 09:39:26.000000 json-grep-1.3.0/jsongrep/VERSION
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.3.0/jsongrep/__init__.py
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/jsongrep/libs/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.3.0/jsongrep/libs/__init__.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      766 2023-06-27 07:16:08.000000 json-grep-1.3.0/jsongrep/libs/cli_colors.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     4519 2023-07-26 09:38:08.000000 json-grep-1.3.0/jsongrep/libs/json_filter.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.3.0/jsongrep/libs/setuptools.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     2681 2023-07-26 09:34:46.000000 json-grep-1.3.0/jsongrep/main.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-07-26 09:41:31.294892 json-grep-1.3.0/setup.cfg
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.3.0/setup.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-08-01 12:48:37.309190 json-grep-1.3.1/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.3.1/MANIFEST.in
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     2075 2023-08-01 12:48:37.309190 json-grep-1.3.1/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1654 2023-08-01 12:47:34.000000 json-grep-1.3.1/README.md
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-08-01 12:48:37.309190 json-grep-1.3.1/json_grep.egg-info/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     2075 2023-08-01 12:48:37.000000 json-grep-1.3.1/json_grep.egg-info/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      396 2023-08-01 12:48:37.000000 json-grep-1.3.1/json_grep.egg-info/SOURCES.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-08-01 12:48:37.000000 json-grep-1.3.1/json_grep.egg-info/dependency_links.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-08-01 12:48:37.000000 json-grep-1.3.1/json_grep.egg-info/entry_points.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-07-26 09:41:31.000000 json-grep-1.3.1/json_grep.egg-info/not-zip-safe
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-08-01 12:48:37.000000 json-grep-1.3.1/json_grep.egg-info/top_level.txt
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-08-01 12:48:37.309190 json-grep-1.3.1/jsongrep/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-08-01 12:46:21.000000 json-grep-1.3.1/jsongrep/VERSION
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.3.1/jsongrep/__init__.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-08-01 12:48:37.309190 json-grep-1.3.1/jsongrep/libs/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.3.1/jsongrep/libs/__init__.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      766 2023-06-27 07:16:08.000000 json-grep-1.3.1/jsongrep/libs/cli_colors.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     4573 2023-08-01 12:29:48.000000 json-grep-1.3.1/jsongrep/libs/json_filter.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.3.1/jsongrep/libs/setuptools.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     3121 2023-08-01 12:44:28.000000 json-grep-1.3.1/jsongrep/main.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-08-01 12:48:37.309190 json-grep-1.3.1/setup.cfg
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.3.1/setup.py
```

### Comparing `json-grep-1.3.0/PKG-INFO` & `json-grep-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.3.0
+Version: 1.3.1
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,18 +16,17 @@
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
+usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] [-f INPUT_FILE] filter_keys [filter_keys ...]
 
-usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] filter_keys [filter_keys ...]
-
-JSON GREP v1.3.0 is utility for filtering selected keys from json string piped from STDOUT
+JSON GREP v1.3.1 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
   filter_keys           List of keys which you want to filter from json dict. If key is in deeper level of tree structure use '.' separator to specify how deep is key in dict tree structure. You can also use '*' at the end of key name to filter keys as 'beginning with'. You can also specify value of item which you want to pass only by operator '=' or
                         '~'. '~' means that value is somewhere in string.
 
 options:
   -h, --help            show this help message and exit
@@ -35,14 +34,16 @@
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
   -l HIGHLIGHT, --hl HIGHLIGHT
                         Highlight case sensitively words in filtered results
   -i IHIGHLIGHT, --ihl IHIGHLIGHT
                         Highlight case insensitively words in filtered results
   -e, --show-errors     Show errors caused by json decode
+  -f INPUT_FILE, --file INPUT_FILE
+                        Input file instead of PIPE
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
 cd json-grep-master/ && \
```

### Comparing `json-grep-1.3.0/README.md` & `json-grep-1.3.1/json_grep.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,32 @@
+Metadata-Version: 2.1
+Name: json-grep
+Version: 1.3.1
+Summary: Filtering JSON dict keys from STDOUT
+Home-page: https://gitlab.com/alda78/json-grep
+Author: Ales Adamek
+Author-email: alda78@seznam.cz
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # json-grep
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
+usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] [-f INPUT_FILE] filter_keys [filter_keys ...]
 
-usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] filter_keys [filter_keys ...]
-
-JSON GREP v1.3.0 is utility for filtering selected keys from json string piped from STDOUT
+JSON GREP v1.3.1 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
   filter_keys           List of keys which you want to filter from json dict. If key is in deeper level of tree structure use '.' separator to specify how deep is key in dict tree structure. You can also use '*' at the end of key name to filter keys as 'beginning with'. You can also specify value of item which you want to pass only by operator '=' or
                         '~'. '~' means that value is somewhere in string.
 
 options:
   -h, --help            show this help message and exit
@@ -21,14 +34,16 @@
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
   -l HIGHLIGHT, --hl HIGHLIGHT
                         Highlight case sensitively words in filtered results
   -i IHIGHLIGHT, --ihl IHIGHLIGHT
                         Highlight case insensitively words in filtered results
   -e, --show-errors     Show errors caused by json decode
+  -f INPUT_FILE, --file INPUT_FILE
+                        Input file instead of PIPE
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
 cd json-grep-master/ && \
@@ -36,8 +51,8 @@
 cd ../ &&  \
 sudo rm -rf json-grep-master
 ```
 
 or simply
 ```bash
 pip3 install json-grep
-```
+```
```

### Comparing `json-grep-1.3.0/json_grep.egg-info/PKG-INFO` & `json-grep-1.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: json-grep
-Version: 1.3.0
-Summary: Filtering JSON dict keys from STDOUT
-Home-page: https://gitlab.com/alda78/json-grep
-Author: Ales Adamek
-Author-email: alda78@seznam.cz
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # json-grep
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
+usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] [-f INPUT_FILE] filter_keys [filter_keys ...]
 
-usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] filter_keys [filter_keys ...]
-
-JSON GREP v1.3.0 is utility for filtering selected keys from json string piped from STDOUT
+JSON GREP v1.3.1 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
   filter_keys           List of keys which you want to filter from json dict. If key is in deeper level of tree structure use '.' separator to specify how deep is key in dict tree structure. You can also use '*' at the end of key name to filter keys as 'beginning with'. You can also specify value of item which you want to pass only by operator '=' or
                         '~'. '~' means that value is somewhere in string.
 
 options:
   -h, --help            show this help message and exit
@@ -35,14 +20,16 @@
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
   -l HIGHLIGHT, --hl HIGHLIGHT
                         Highlight case sensitively words in filtered results
   -i IHIGHLIGHT, --ihl IHIGHLIGHT
                         Highlight case insensitively words in filtered results
   -e, --show-errors     Show errors caused by json decode
+  -f INPUT_FILE, --file INPUT_FILE
+                        Input file instead of PIPE
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
 cd json-grep-master/ && \
@@ -50,8 +37,8 @@
 cd ../ &&  \
 sudo rm -rf json-grep-master
 ```
 
 or simply
 ```bash
 pip3 install json-grep
-```
+```
```

### Comparing `json-grep-1.3.0/jsongrep/libs/cli_colors.py` & `json-grep-1.3.1/jsongrep/libs/cli_colors.py`

 * *Files identical despite different names*

### Comparing `json-grep-1.3.0/jsongrep/libs/json_filter.py` & `json-grep-1.3.1/jsongrep/libs/json_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,19 +87,19 @@
                 ret = f"{ret}\"{FG.green}{CMD.bold}{key}{CMD.reset}\": \"{FG.cyan}{value}{CMD.reset}\"{br_line}"
         return f"{ret}\n"
 
     def _highlight_value(self, value: str) -> str:
         for highlight in self.highlight_values:
             if found_results := re.findall(f"({highlight})+", value):
                 for found in found_results:
-                    value = value.replace(found, f"{FG.red}{found}{CMD.reset}")
+                    value = value.replace(found, f"{FG.orange}{BG.lightgrey}{CMD.bold}{found}{CMD.reset}")
         return value
 
     def _ihighlight_value(self, value: str) -> str:
         for highlight in self.ihighlight_values:
             if found_results := re.findall(f"({highlight})+", value, re.IGNORECASE):
                 for found in found_results:
-                    value = value.replace(found, f"{FG.red}{found}{CMD.reset}")
+                    value = value.replace(found, f"{FG.orange}{BG.lightgrey}{CMD.bold}{found}{CMD.reset}")
         return value
 
     def _check_is_value_operator_used(self) -> bool:
         return any([True for key in self.filter_keys if self.parse_key(key)[2]])
```

### Comparing `json-grep-1.3.0/jsongrep/main.py` & `json-grep-1.3.1/jsongrep/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,33 +21,46 @@
         "at the end of key name to filter keys as 'beginning with'. "
         "You can also specify value of item which you want to pass "
         "only by operator '=' or '~'. '~' means "
         "that value is somewhere in string.")
                         )
     parser.add_argument("-m", "--multiline-output", dest="multiline_output", default=False, action="store_true", help="Use multiline output for filtered result")
     parser.add_argument("-v", "--values_only", dest="values_only", default=False, action="store_true", help="Show only values without keys description")
-    parser.add_argument("-l", "--hl", dest="highlight", action="append", help="Highlight case sensitively words in filtered results")
-    parser.add_argument("-i", "--ihl", dest="ihighlight", action="append", help="Highlight case insensitively words in filtered results")
+    parser.add_argument("-l", "--hl", type=str, dest="highlight", action="append", help="Highlight case sensitively words in filtered results")
+    parser.add_argument("-i", "--ihl", type=str, dest="ihighlight", action="append", help="Highlight case insensitively words in filtered results")
     parser.add_argument("-e", "--show-errors", dest="show_errors", default=False, action="store_true", help="Show errors caused by json decode")
+    parser.add_argument("-f", "--file", type=str, dest="input_file", help="Input file instead of PIPE")
 
     args = parser.parse_args()
     return args
 
 
+def read_input_file(path: str) -> list[str]:
+    with open(path, "r") as f:
+        while line := f.readline():
+            yield line
+
+
 def main():
     signal.signal(signal.SIGINT, _handle_exit)
     args = _handle_args()
 
     json_filter = JsonFilter(args.filter_keys)
     json_filter.multiline_output = args.multiline_output
     json_filter.values_only = args.values_only
     json_filter.highlight_values = args.highlight
     json_filter.ihighlight_values = args.ihighlight
 
-    for line in sys.stdin:
+    try:
+        input_lines = read_input_file(args.input_file) if args.input_file else sys.stdin
+    except Exception as ex:
+        print(f"I/O error: {ex}")
+        exit(1)
+
+    for line in input_lines:
         try:
             filtered_data = json_filter.filter_keys_and_values(line)
             if filtered_data:
                 output = json_filter.format_result(filtered_data)
                 sys.stdout.write(output)
         except JsonFilterException as ex:
             if args.show_errors:
```

### Comparing `json-grep-1.3.0/setup.py` & `json-grep-1.3.1/setup.py`

 * *Files identical despite different names*

