# Comparing `tmp/cmdcomp-2.0.2.tar.gz` & `tmp/cmdcomp-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-2.0.2.tar", max compression
+gzip compressed data, was "cmdcomp-2.0.3.tar", max compression
```

## Comparing `cmdcomp-2.0.2.tar` & `cmdcomp-2.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2425 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/README.md
--rw-r--r--   0        0        0       79 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2289 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/app.py
--rw-r--r--   0        0        0      573 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/completion.py
--rw-r--r--   0        0        0      734 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/config.py
--rw-r--r--   0        0        0      444 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/exception.py
--rw-r--r--   0        0        0      115 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/main.py
--rw-r--r--   0        0        0      115 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/model.py
--rw-r--r--   0        0        0      131 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/shell.py
--rw-r--r--   0        0        0        0 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/__init__.py
--rw-r--r--   0        0        0      535 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/app_info.py
--rw-r--r--   0        0        0      261 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/cmdcomp_info.py
--rw-r--r--   0        0        0     3358 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/__init__.py
--rw-r--r--   0        0        0      338 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/option/__init__.py
--rw-r--r--   0        0        0      331 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/option/command_option.py
--rw-r--r--   0        0        0      373 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/option/file_option.py
--rw-r--r--   0        0        0     2103 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/completion.py
--rw-r--r--   0        0        0      377 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/config.py
--rw-r--r--   0        0        0     1732 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1313 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/templates/zsh.sh.jinja
--rw-r--r--   0        0        0        0 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/__init__.py
--rw-r--r--   0        0        0      535 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/app_info.py
--rw-r--r--   0        0        0      261 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/cmdcomp_info.py
--rw-r--r--   0        0        0     6844 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/__init__.py
--rw-r--r--   0        0        0      371 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/__init__.py
--rw-r--r--   0        0        0      789 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/command_argument.py
--rw-r--r--   0        0        0      744 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/file_argument.py
--rw-r--r--   0        0        0      601 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/flag_argument.py
--rw-r--r--   0        0        0     1668 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/values_argument.py
--rw-r--r--   0        0        0      747 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/completion.py
--rw-r--r--   0        0        0      380 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/config.py
--rw-r--r--   0        0        0     4215 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/templates/bash.sh.jinja
--rw-r--r--   0        0        0     2575 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1696 2023-08-01 08:56:12.152125 cmdcomp-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2425 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/README.md
+-rw-r--r--   0        0        0       79 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2289 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/app.py
+-rw-r--r--   0        0        0      573 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/completion.py
+-rw-r--r--   0        0        0      734 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/config.py
+-rw-r--r--   0        0        0      444 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/exception.py
+-rw-r--r--   0        0        0      115 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/main.py
+-rw-r--r--   0        0        0      115 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     3358 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2103 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1732 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1313 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0     6844 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      789 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      744 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      601 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1668 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/command/argument/values_argument.py
+-rw-r--r--   0        0        0      808 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0     4369 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     2729 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1696 2023-08-01 12:51:34.451143 cmdcomp-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.3/PKG-INFO
```

### Comparing `cmdcomp-2.0.2/README.md` & `cmdcomp-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/app.py` & `cmdcomp-2.0.3/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/completion.py` & `cmdcomp-2.0.3/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/config.py` & `cmdcomp-2.0.3/cmdcomp/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v1/app_info.py` & `cmdcomp-2.0.3/cmdcomp/v1/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v1/command/__init__.py` & `cmdcomp-2.0.3/cmdcomp/v1/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v1/completion.py` & `cmdcomp-2.0.3/cmdcomp/v1/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v1/templates/bash.sh.jinja` & `cmdcomp-2.0.3/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v1/templates/zsh.sh.jinja` & `cmdcomp-2.0.3/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/app_info.py` & `cmdcomp-2.0.3/cmdcomp/v2/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/command/__init__.py` & `cmdcomp-2.0.3/cmdcomp/v2/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/command/argument/command_argument.py` & `cmdcomp-2.0.3/cmdcomp/v2/command/argument/command_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/command/argument/file_argument.py` & `cmdcomp-2.0.3/cmdcomp/v2/command/argument/file_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/command/argument/flag_argument.py` & `cmdcomp-2.0.3/cmdcomp/v2/command/argument/flag_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/command/argument/values_argument.py` & `cmdcomp-2.0.3/cmdcomp/v2/command/argument/values_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/completion.py` & `cmdcomp-2.0.3/cmdcomp/v2/completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 from typing import Any
 
+from cmdcomp import __version__
 from cmdcomp.shell import ShellType
 from cmdcomp.v2.config import V2Config
 
 
 def generate_v2(shell: ShellType, config: V2Config) -> str:
     from jinja2 import Environment, FileSystemLoader
 
@@ -14,12 +15,13 @@
     template = env.get_template(f"{shell.value}.sh.jinja")
 
     return template.render(
         app_name=config.app.name,
         app_aliases=config.app.aliases + config.root.aliases,
         commands={config.app.name: config.root},
         append_key_tag=_append_key_tag,
+        version=__version__,
     )
 
 
 def _append_key_tag(d: dict[str, Any], tag: str) -> dict[tuple[str, str], Any]:
     return {(tag, k): v for k, v in d.items()}
```

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/templates/bash.sh.jinja` & `cmdcomp-2.0.3/cmdcomp/v2/templates/bash.sh.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,18 @@
 {%- endmacro -%}
 
 {#- macro def -#}
 {%- macro file_completion(base_path) -%}
 {%- endmacro -%}
 
 #!/bin/bash
+#
+# Code generated by cmdcomp "{{ version }}". DO NOT EDIT.
+# For more information about cmdcomp, please refer to https://github.com/yassun4dev/cmdcomp
+#
 
 {{ func_name }}() {
   local word cmd opts cur cmd_cur opts_cur
   COMPREPLY=()
   cmd=""
   opts=""
   cur=0
```

### Comparing `cmdcomp-2.0.2/cmdcomp/v2/templates/zsh.sh.jinja` & `cmdcomp-2.0.3/cmdcomp/v2/templates/zsh.sh.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,18 @@
   {%- elif argument.type == 'command' -%}
           :command:_values '{{ arg_name|trim("-") }}' $({{ argument.execute }})
   {%- elif argument.type == 'flag' -%}
   {%- endif -%}
 {%- endmacro -%}
 
 #!/bin/zsh
+#
+# Code generated by cmdcomp "{{ version }}". DO NOT EDIT.
+# For more information about cmdcomp, please refer to https://github.com/yassun4dev/cmdcomp
+#
 
 {{ func_name }}() {
   local context curcontext=$curcontext state line
   declare -A opt_args
   local ret=1
   local cmd_name={{ app_name }}
```

### Comparing `cmdcomp-2.0.2/pyproject.toml` & `cmdcomp-2.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "2.0.2"
+version = "2.0.3"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-2.0.2/PKG-INFO` & `cmdcomp-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 2.0.2
+Version: 2.0.3
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.2 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.3 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

