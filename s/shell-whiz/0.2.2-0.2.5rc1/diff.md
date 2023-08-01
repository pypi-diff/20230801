# Comparing `tmp/shell_whiz-0.2.2.tar.gz` & `tmp/shell_whiz-0.2.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.2.2.tar", max compression
+gzip compressed data, was "shell_whiz-0.2.5rc1.tar", max compression
```

## Comparing `shell_whiz-0.2.2.tar` & `shell_whiz-0.2.5rc1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-25 23:02:35.900916 shell_whiz-0.2.2/LICENSE
--rw-r--r--   0        0        0     3294 2023-07-25 23:02:35.900916 shell_whiz-0.2.2/README.md
--rw-r--r--   0        0        0      538 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4186 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1686 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/config.py
--rw-r--r--   0        0        0      378 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     8293 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/openai.py
--rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 shell_whiz-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 18:42:49.046074 shell_whiz-0.2.5rc1/LICENSE
+-rw-r--r--   0        0        0     3141 2023-08-01 18:42:49.046074 shell_whiz-0.2.5rc1/README.md
+-rw-r--r--   0        0        0      539 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/argparse.py
+-rw-r--r--   0        0        0     6761 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/cli.py
+-rw-r--r--   0        0        0     1686 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/config.py
+-rw-r--r--   0        0        0       54 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/console.py
+-rw-r--r--   0        0        0      207 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/constants.py
+-rw-r--r--   0        0        0      152 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0    10011 2023-08-01 18:42:49.054075 shell_whiz-0.2.5rc1/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 shell_whiz-0.2.5rc1/PKG-INFO
```

### Comparing `shell_whiz-0.2.2/LICENSE` & `shell_whiz-0.2.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.2/README.md` & `shell_whiz-0.2.5rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 
 Shell Whiz will help you generate shell commands from your natural language queries. It is powered by OpenAI's `gpt-3.5-turbo` and is free to use.
 
 ## All features
 - **Pay as you go:** you only pay for what you use; no subscription is required. Just receive an API key from https://platform.openai.com/account/api-keys.
 - **Easy to install:** run `pip install shell-whiz` and you're good to go.
 - **Easy to use:** Shell Whiz is a command-line tool.
-    - Run `sw ask` to generate shell commands from your natural language queries.
-    - Run `sw explain` to get an explanation of any shell command.
 
 ## Supported platforms
 Shell Whiz is designed to work on various platforms and shells, but it is best suited for Bash on Linux. However, it may sometimes suggest commands that are not compatible with your specific platform or terminal.
 
 ## Installation and setup
 To install Shell Whiz, run the following command:
 ```
@@ -43,27 +41,27 @@
 
 Then, run `sw config` to set up your API key.
 
 ### Free API plan for new users
 New users receive $5 for free to try and test the API during the first 3 months. However, it is recommended to upgrade to a paid plan in order to have a more comfortable experience using Shell Whiz. This is because the free plan has restrictions on the number of requests allowed per minute.
 
 ## Upgrading
-To upgrade GitHub Copilot CLI, run the following command:
+To upgrade Shell Whiz, run the following command:
 ```
 $ pip install --upgrade shell-whiz
 ```
 
 ## Usage
 <p align="center">
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/files_modified_in_the_last_7_days.gif?raw=true"
   />
 </p>
 
-You can run Shell Whiz directly using `sw`, but I recommend creating an alias for it. For example, you can add the following line to your `.bashrc` file:
+You can run Shell Whiz directly using `sw ask`, but I recommend creating an alias for it. For example, you can add the following line to your `.bashrc` file:
 ```
 alias ??='sw ask'
 ```
 
 To track API usage and costs, you can check the [OpenAI API Usage](https://platform.openai.com/account/usage) page.
 
 ## More examples
```

### Comparing `shell_whiz-0.2.2/pyproject.toml` & `shell_whiz-0.2.5rc1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.2.2"
+version = "0.2.5rc1"
 description = "Shell Whiz: AI assistant right in your terminal"
+license = "GPL-3.0-only"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 openai = "^0.27.8"
 inquirer = "^3.1.3"
 yaspin = "^2.3.0"
-prompt-toolkit = "^3.0.39"
-colorama = "^0.4.6"
 jsonschema = "^4.18.4"
+rich = "^13.4.2"
 
 [tool.poetry.scripts]
-sw = "shell_whiz:main"
+sw = "shell_whiz.cli:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shell_whiz-0.2.2/shell_whiz/config.py` & `shell_whiz-0.2.5rc1/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.2/PKG-INFO` & `shell_whiz-0.2.5rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.2.2
+Version: 0.2.5rc1
 Summary: Shell Whiz: AI assistant right in your terminal
+License: GPL-3.0-only
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: prompt-toolkit (>=3.0.39,<4.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/beimzhan/shell-whiz/raw/main/images/shell-whiz.png" />
 </p>
 
@@ -38,16 +39,14 @@
 
 Shell Whiz will help you generate shell commands from your natural language queries. It is powered by OpenAI's `gpt-3.5-turbo` and is free to use.
 
 ## All features
 - **Pay as you go:** you only pay for what you use; no subscription is required. Just receive an API key from https://platform.openai.com/account/api-keys.
 - **Easy to install:** run `pip install shell-whiz` and you're good to go.
 - **Easy to use:** Shell Whiz is a command-line tool.
-    - Run `sw ask` to generate shell commands from your natural language queries.
-    - Run `sw explain` to get an explanation of any shell command.
 
 ## Supported platforms
 Shell Whiz is designed to work on various platforms and shells, but it is best suited for Bash on Linux. However, it may sometimes suggest commands that are not compatible with your specific platform or terminal.
 
 ## Installation and setup
 To install Shell Whiz, run the following command:
 ```
@@ -60,27 +59,27 @@
 
 Then, run `sw config` to set up your API key.
 
 ### Free API plan for new users
 New users receive $5 for free to try and test the API during the first 3 months. However, it is recommended to upgrade to a paid plan in order to have a more comfortable experience using Shell Whiz. This is because the free plan has restrictions on the number of requests allowed per minute.
 
 ## Upgrading
-To upgrade GitHub Copilot CLI, run the following command:
+To upgrade Shell Whiz, run the following command:
 ```
 $ pip install --upgrade shell-whiz
 ```
 
 ## Usage
 <p align="center">
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/files_modified_in_the_last_7_days.gif?raw=true"
   />
 </p>
 
-You can run Shell Whiz directly using `sw`, but I recommend creating an alias for it. For example, you can add the following line to your `.bashrc` file:
+You can run Shell Whiz directly using `sw ask`, but I recommend creating an alias for it. For example, you can add the following line to your `.bashrc` file:
 ```
 alias ??='sw ask'
 ```
 
 To track API usage and costs, you can check the [OpenAI API Usage](https://platform.openai.com/account/usage) page.
 
 ## More examples
```

