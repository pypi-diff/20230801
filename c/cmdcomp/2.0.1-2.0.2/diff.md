# Comparing `tmp/cmdcomp-2.0.1.tar.gz` & `tmp/cmdcomp-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-2.0.1.tar", max compression
+gzip compressed data, was "cmdcomp-2.0.2.tar", max compression
```

## Comparing `cmdcomp-2.0.1.tar` & `cmdcomp-2.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2425 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/README.md
--rw-r--r--   0        0        0       79 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2358 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/app.py
--rw-r--r--   0        0        0      573 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/completion.py
--rw-r--r--   0        0        0      734 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/config.py
--rw-r--r--   0        0        0      444 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/exception.py
--rw-r--r--   0        0        0      115 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/main.py
--rw-r--r--   0        0        0      115 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/model.py
--rw-r--r--   0        0        0      131 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/shell.py
--rw-r--r--   0        0        0        0 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/__init__.py
--rw-r--r--   0        0        0      535 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/app_info.py
--rw-r--r--   0        0        0      261 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/cmdcomp_info.py
--rw-r--r--   0        0        0     3358 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/__init__.py
--rw-r--r--   0        0        0      338 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/option/__init__.py
--rw-r--r--   0        0        0      331 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/option/command_option.py
--rw-r--r--   0        0        0      373 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/option/file_option.py
--rw-r--r--   0        0        0     2103 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/completion.py
--rw-r--r--   0        0        0      377 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/config.py
--rw-r--r--   0        0        0     1732 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1277 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/templates/zsh.sh.jinja
--rw-r--r--   0        0        0        0 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/__init__.py
--rw-r--r--   0        0        0      535 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/app_info.py
--rw-r--r--   0        0        0      261 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/cmdcomp_info.py
--rw-r--r--   0        0        0     6844 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/__init__.py
--rw-r--r--   0        0        0      371 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/__init__.py
--rw-r--r--   0        0        0      789 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/command_argument.py
--rw-r--r--   0        0        0      744 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/file_argument.py
--rw-r--r--   0        0        0      601 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/flag_argument.py
--rw-r--r--   0        0        0     1668 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/values_argument.py
--rw-r--r--   0        0        0      747 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/completion.py
--rw-r--r--   0        0        0      380 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/config.py
--rw-r--r--   0        0        0     4215 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/templates/bash.sh.jinja
--rw-r--r--   0        0        0     2575 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1779 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 cmdcomp-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2425 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/README.md
+-rw-r--r--   0        0        0       79 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2289 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/app.py
+-rw-r--r--   0        0        0      573 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/completion.py
+-rw-r--r--   0        0        0      734 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/config.py
+-rw-r--r--   0        0        0      444 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/exception.py
+-rw-r--r--   0        0        0      115 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/main.py
+-rw-r--r--   0        0        0      115 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     3358 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2103 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1732 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1313 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0     6844 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      789 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      744 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      601 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1668 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/command/argument/values_argument.py
+-rw-r--r--   0        0        0      747 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0     4215 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     2575 2023-08-01 08:56:12.148125 cmdcomp-2.0.2/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1696 2023-08-01 08:56:12.152125 cmdcomp-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.2/PKG-INFO
```

### Comparing `cmdcomp-2.0.1/README.md` & `cmdcomp-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/app.py` & `cmdcomp-2.0.2/cmdcomp/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 class App:
     @classmethod
     def run(cls, args: list[str] | None = None) -> None:
         import logging
         from argparse import ArgumentParser, BooleanOptionalAction, FileType
         from logging import getLogger
 
-        import argcomplete
         from rich.console import Console
         from rich.logging import RichHandler
 
         from cmdcomp import __version__
         from cmdcomp.completion import generate
         from cmdcomp.config import load
         from cmdcomp.shell import ShellType
@@ -50,16 +49,14 @@
 
         parser.add_argument(
             "--verbose",
             action=BooleanOptionalAction,
             help="output verbose log.",
         )
 
-        argcomplete.autocomplete(parser)
-
         space = parser.parse_args(args)
 
         logging.basicConfig(
             format="%(message)s",
             handlers=[
                 RichHandler(
                     level=logging.DEBUG if space.verbose else logging.INFO,
```

### Comparing `cmdcomp-2.0.1/cmdcomp/completion.py` & `cmdcomp-2.0.2/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/config.py` & `cmdcomp-2.0.2/cmdcomp/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v1/app_info.py` & `cmdcomp-2.0.2/cmdcomp/v1/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v1/command/__init__.py` & `cmdcomp-2.0.2/cmdcomp/v1/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v1/completion.py` & `cmdcomp-2.0.2/cmdcomp/v1/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v1/templates/bash.sh.jinja` & `cmdcomp-2.0.2/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v1/templates/zsh.sh.jinja` & `cmdcomp-2.0.2/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,21 @@
                 {{ name }})
 {%- if completion is mapping %}
                     case ${words[{{ loop.depth + 1 }}]} in
 {{- loop(completion.items())|indent(width=8) }}
                     esac
                     ;;
 {%- elif completion|first is mapping and 'command' in completion|first %}
-                    _values '{{ name }}' {{ (completion|first).command }}
+                    _values '{{ name|replace("-", "_") }}' {{ (completion|first).command }}
                     ;;
 {%- elif completion|first is mapping and 'file' in completion|first %}
                     _files -W "{{ (completion|first).file }}"
                     ;;
 {%- else %}
-                    _values '{{ name }}' {{ completion|join(" ") }}
+                    _values '{{ name|replace("-", "_") }}' {{ completion|join(" ") }}
                     ;;
 {%- endif %}
 {%- endfor %}
             esac
             ;;
 {%- endfor %}
     esac
```

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/app_info.py` & `cmdcomp-2.0.2/cmdcomp/v2/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/command/__init__.py` & `cmdcomp-2.0.2/cmdcomp/v2/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/command/argument/command_argument.py` & `cmdcomp-2.0.2/cmdcomp/v2/command/argument/command_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/command/argument/file_argument.py` & `cmdcomp-2.0.2/cmdcomp/v2/command/argument/file_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/command/argument/flag_argument.py` & `cmdcomp-2.0.2/cmdcomp/v2/command/argument/flag_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/command/argument/values_argument.py` & `cmdcomp-2.0.2/cmdcomp/v2/command/argument/values_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/completion.py` & `cmdcomp-2.0.2/cmdcomp/v2/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/templates/bash.sh.jinja` & `cmdcomp-2.0.2/cmdcomp/v2/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/cmdcomp/v2/templates/zsh.sh.jinja` & `cmdcomp-2.0.2/cmdcomp/v2/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.1/pyproject.toml` & `cmdcomp-2.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "2.0.1"
+version = "2.0.2"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -18,27 +18,25 @@
 ]
 
 [tool.poetry.scripts]
 cmdcomp = "cmdcomp.main:main"
 
 [tool.taskipy.tasks]
 generate-json-schema = "python tasks/generate_json_schema.py > docs/config.schema.json"
-generate-completion = "register-python-argcomplete cmdcomp"
 test = "pytest"
 format = "black --target-version py310 ."
 lint = "pyright cmdcomp/** tests/**"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0"
 jinja2 = "^3.1.2"
 mergedeep = "^1.3.4"
 pyyaml = "^6.0"
 rich = "^13.4.2"
-argcomplete = "^3.1.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest = "^7.2.2"
 pyright = "^1.1.300"
```

### Comparing `cmdcomp-2.0.1/PKG-INFO` & `cmdcomp-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 2.0.1
+Version: 2.0.2
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Dist: argcomplete (>=3.1.1,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Repository, https://github.com/yassun4dev/cmdcomp
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.1 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.2 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Software Development Classifier: Typing :: Typed Requires-Dist: argcomplete
-(>=3.1.1,<4.0.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-Dist:
-mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Requires-Dist:
-pyyaml (>=6.0,<7.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Project-URL:
-Repository, https://github.com/yassun4dev/cmdcomp Description-Content-Type:
-text/markdown # Command Completion Generator Tool
+Software Development Classifier: Typing :: Typed Requires-Dist: jinja2
+(>=3.1.2,<4.0.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
+pydantic (>=2.0,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: rich
+(>=13.4.2,<14.0.0) Project-URL: Repository, https://github.com/yassun4dev/
+cmdcomp Description-Content-Type: text/markdown # Command Completion Generator
+Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
 `cmdcomp` generate shell completion file (`bash` or `zsh`) from config `json`/
 `yaml`/`toml` file. ## Install ```shell pip install cmdcomp ``` ## Usage ###
 Local ```shell cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ###
 Docker ```shell docker run --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --
 file ${YOUR_CONFIG_FILE} --shell-type bash ``` ## Config Configuration can be
 written in `JSON`, `YAML`, and `TOML` file formats. ### Sample ```yaml cmdcomp:
```

