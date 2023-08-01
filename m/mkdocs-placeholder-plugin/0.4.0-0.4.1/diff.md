# Comparing `tmp/mkdocs-placeholder-plugin-0.4.0.tar.gz` & `tmp/mkdocs-placeholder-plugin-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-placeholder-plugin-0.4.0.tar", last modified: Sat May 20 15:16:05 2023, max compression
+gzip compressed data, was "mkdocs-placeholder-plugin-0.4.1.tar", last modified: Tue Aug  1 18:12:14 2023, max compression
```

## Comparing `mkdocs-placeholder-plugin-0.4.0.tar` & `mkdocs-placeholder-plugin-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.483419 mkdocs-placeholder-plugin-0.4.0/
--rw-r--r--   0 user       (501) staff       (20)     1063 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.4.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       65 2023-03-27 05:22:55.000000 mkdocs-placeholder-plugin-0.4.0/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     9691 2023-05-20 15:16:05.483501 mkdocs-placeholder-plugin-0.4.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     9053 2023-05-20 15:14:57.000000 mkdocs-placeholder-plugin-0.4.0/README.md
--rw-r--r--   0 user       (501) staff       (20)       85 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.4.0/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)      897 2023-05-20 15:16:05.483852 mkdocs-placeholder-plugin-0.4.0/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.473693 mkdocs-placeholder-plugin-0.4.0/src/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.474890 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.476815 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/
--rw-r--r--   0 user       (501) staff       (20)     2944 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      312 2023-03-27 05:34:32.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder-data.js
--rw-r--r--   0 user       (501) staff       (20)    27967 2023-05-20 14:27:02.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js
--rw-r--r--   0 user       (501) staff       (20)   110866 2023-05-20 14:27:02.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.479618 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/
--rw-r--r--   0 user       (501) staff       (20)      911 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.481209 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/
--rw-r--r--   0 user       (501) staff       (20)      277 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4971 2023-05-18 19:10:30.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/configuration.py
--rw-r--r--   0 user       (501) staff       (20)     4601 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/parser_utils.py
--rw-r--r--   0 user       (501) staff       (20)    10414 2023-05-13 17:10:01.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/placeholder.py
--rw-r--r--   0 user       (501) staff       (20)     3491 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/validator.py
--rw-r--r--   0 user       (501) staff       (20)     2552 2023-05-20 14:26:55.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/generic_style.py
--rw-r--r--   0 user       (501) staff       (20)     4885 2023-05-13 17:36:39.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_handler.py
--rw-r--r--   0 user       (501) staff       (20)     1315 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_parser.py
--rw-r--r--   0 user       (501) staff       (20)     4371 2023-05-18 18:43:12.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/json_generator.py
--rw-r--r--   0 user       (501) staff       (20)     2209 2023-05-20 14:14:46.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/page_processor.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.482277 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2383 2023-05-13 15:32:30.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/input_elements.py
--rw-r--r--   0 user       (501) staff       (20)     5157 2023-05-13 17:38:11.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/placeholder_replacer.py
--rw-r--r--   0 user       (501) staff       (20)     4168 2023-05-13 16:30:00.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/table_generator.py
--rw-r--r--   0 user       (501) staff       (20)     1348 2023-05-13 15:52:07.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/table_replacer.py
--rw-r--r--   0 user       (501) staff       (20)     3742 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/validator_functions.py
--rw-r--r--   0 user       (501) staff       (20)     8731 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/validators_predefined.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.483279 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/
--rw-r--r--   0 user       (501) staff       (20)      114 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3048 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/plugin.py
--rw-r--r--   0 user       (501) staff       (20)      983 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/plugin_config.py
--rw-r--r--   0 user       (501) staff       (20)     1466 2023-05-18 11:04:08.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/style.py
--rw-r--r--   0 user       (501) staff       (20)     4661 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/utils.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.475559 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     9691 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1950 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       82 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       26 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.528182 mkdocs-placeholder-plugin-0.4.1/
+-rw-r--r--   0 user       (501) staff       (20)     1063 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.4.1/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       65 2023-03-27 05:22:55.000000 mkdocs-placeholder-plugin-0.4.1/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     9915 2023-08-01 18:12:14.528267 mkdocs-placeholder-plugin-0.4.1/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     9277 2023-08-01 18:11:41.000000 mkdocs-placeholder-plugin-0.4.1/README.md
+-rw-r--r--   0 user       (501) staff       (20)       85 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.4.1/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)      897 2023-08-01 18:12:14.528831 mkdocs-placeholder-plugin-0.4.1/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.517788 mkdocs-placeholder-plugin-0.4.1/src/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.518941 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.520772 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/
+-rw-r--r--   0 user       (501) staff       (20)     2944 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      312 2023-03-27 05:34:32.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/placeholder-data.js
+-rw-r--r--   0 user       (501) staff       (20)    27967 2023-05-27 14:19:36.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js
+-rw-r--r--   0 user       (501) staff       (20)   110866 2023-05-27 14:19:36.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.523629 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/
+-rw-r--r--   0 user       (501) staff       (20)      911 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.524787 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/
+-rw-r--r--   0 user       (501) staff       (20)      307 2023-05-21 14:38:52.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4768 2023-05-21 15:30:38.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/configuration.py
+-rw-r--r--   0 user       (501) staff       (20)     5500 2023-05-21 15:57:21.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/parser_utils.py
+-rw-r--r--   0 user       (501) staff       (20)    10370 2023-05-21 14:03:20.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/placeholder.py
+-rw-r--r--   0 user       (501) staff       (20)     3553 2023-08-01 18:10:00.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/validator.py
+-rw-r--r--   0 user       (501) staff       (20)     2706 2023-05-27 14:07:43.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/generic_style.py
+-rw-r--r--   0 user       (501) staff       (20)     4885 2023-05-13 17:36:39.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/html_tag_handler.py
+-rw-r--r--   0 user       (501) staff       (20)     1315 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/html_tag_parser.py
+-rw-r--r--   0 user       (501) staff       (20)     4371 2023-05-18 18:43:12.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/json_generator.py
+-rw-r--r--   0 user       (501) staff       (20)     2364 2023-05-27 14:19:32.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/page_processor.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.525780 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2383 2023-05-13 15:32:30.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/input_elements.py
+-rw-r--r--   0 user       (501) staff       (20)     5157 2023-05-13 17:38:11.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/placeholder_replacer.py
+-rw-r--r--   0 user       (501) staff       (20)     4253 2023-05-27 14:01:49.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/table_generator.py
+-rw-r--r--   0 user       (501) staff       (20)     1348 2023-05-13 15:52:07.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/table_replacer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.526851 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/validators/
+-rw-r--r--   0 user       (501) staff       (20)     7425 2023-08-01 17:38:34.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/validators/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1136 2023-08-01 17:29:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/validators/files.py
+-rw-r--r--   0 user       (501) staff       (20)     2120 2023-05-21 16:46:30.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/validators/internet.py
+-rw-r--r--   0 user       (501) staff       (20)     3476 2023-05-21 14:02:02.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/validators/ip_address.py
+-rw-r--r--   0 user       (501) staff       (20)     1517 2023-08-01 18:07:37.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/validators/network.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.527912 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/
+-rw-r--r--   0 user       (501) staff       (20)      114 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3016 2023-08-01 18:11:19.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/plugin.py
+-rw-r--r--   0 user       (501) staff       (20)      983 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/plugin_config.py
+-rw-r--r--   0 user       (501) staff       (20)     1466 2023-05-18 11:04:08.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/style.py
+-rw-r--r--   0 user       (501) staff       (20)     5184 2023-08-01 17:13:13.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-01 18:12:14.519627 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     9915 2023-08-01 18:12:14.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     2129 2023-08-01 18:12:14.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-08-01 18:12:14.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       82 2023-08-01 18:12:14.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-08-01 18:12:14.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       26 2023-08-01 18:12:14.000000 mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/top_level.txt
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/LICENSE` & `mkdocs-placeholder-plugin-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/PKG-INFO` & `mkdocs-placeholder-plugin-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-placeholder-plugin
-Version: 0.4.0
+Version: 0.4.1
 Summary: Add dynamic placeholders to your mkdocs page
 Home-page: https://github.com/six-two/mkdocs-placeholder-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -25,37 +25,34 @@
 This plugin allows you to have placeholders in your site, that can be dynamically replaced at runtime using JavaScript (see [demo page](https://mkdocs-placeholder-plugin.six-two.dev/demo/)).
 
 
 ## Documentation
 
 This README is just a short intro to the package.
 For a quick start and detailed information please see the [documentation for the last release](https://mkdocs-placeholder-plugin.six-two.dev/).
-The documentation is also available in the `docs` folder of the source code and can be built localy with [MkDocs](https://www.mkdocs.org/).
+The documentation is also available in the `docs` folder of the source code and can be built locally with [MkDocs](https://www.mkdocs.org/).
 
 ## Development version
 
 If you want to use the latest development version (may be broken/buggy from time to time), you can install it by:
 
 1. Cloning the repository:
     ```bash
     git clone https://github.com/six-two/mkdocs-placeholder-plugin
     cd mkdocs-placeholder-plugin
     ```
 2. Building/Downloading the JavaScript files.
     Choose any of the following ways:
     
     - Build it with npm (natively), by running the `./build-docs.sh` script.
-    - Build it in a (docker/podman) container by using the `Doeckerfile` in the `typescript` directory:
+    - Build it in a (docker/podman) container by using the `Dockerfile` in the `typescript` directory.
+        The whole thing can be done by running the `buils.sh` script in the root directory:
         ```bash
-        cd typescript
-        podman build --tag placeholder-npm .
-        cd ..
+        ./build.sh
         ```
-
-        And then running the `./build.sh` script.
         Once you see mkdocs running, you can terminate it with `Ctrl-C`.
     - Downloading the files from the development version of the documentation (hosted and built by Vercel):
         ```bash
         curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js
         curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js.map -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
         ```
 3. Installing the package with pip:
@@ -63,15 +60,20 @@
     python3 -m pip install .
     ```
 
 The corresponding documentation is hosted at <https://dev.mkdocs-placeholder-plugin.six-two.dev>.
 
 ## Notable changes
 
-### HEAD
+### Version 0.4.1
+
+- Validators can copy rules from other validators via the `import_rules_from` attribute
+- New validators: `email`, `linux_interface`, `mac_address`, `uuid`
+
+### Version 0.4.0
 
 - Configuration format changed:
     - Validators are no longer defined in-line and instead defined in a `validators` section -> easier to reuse custom validators.
     - Placeholders now need to be specified in a `placeholders` section.
     - Most settings are now in the configuration file instead of in your `mkdocs.yml`.
 - Some actions can now be toggled by visitors of the site. The settings open when you click the gear icon on a (dynamic) placeholder input table.
 - (By default) values are saved when the focus leaves a text field.
@@ -173,21 +175,22 @@
     mypy src
     ```
     ```
     pyflakes src
     ```
 2. Update the changelog in this README file.
 3. Update version number in `setup.cfg`.
-4. Build and update package.
-5. Create a commit for the release (`Version 0.X.Y`) and push it.
-6. Add a tag named `0.X.Y`:
+4. Disable `debug_javascript` in `placeholder-plugin.yaml`.
+5. Build and update package.
+6. Create a commit for the release (`Version 0.X.Y`) and push it.
+7. Add a tag named `0.X.Y`:
     ```
     git tag 0.X.Y
     ```
-7. Update the `latest-release` branch, so that the documentation website gets updated:
+8. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
     git push --tags origin latest-release
     ```
 
 ### Updating python dependencies
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/README.md` & `mkdocs-placeholder-plugin-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,34 @@
 This plugin allows you to have placeholders in your site, that can be dynamically replaced at runtime using JavaScript (see [demo page](https://mkdocs-placeholder-plugin.six-two.dev/demo/)).
 
 
 ## Documentation
 
 This README is just a short intro to the package.
 For a quick start and detailed information please see the [documentation for the last release](https://mkdocs-placeholder-plugin.six-two.dev/).
-The documentation is also available in the `docs` folder of the source code and can be built localy with [MkDocs](https://www.mkdocs.org/).
+The documentation is also available in the `docs` folder of the source code and can be built locally with [MkDocs](https://www.mkdocs.org/).
 
 ## Development version
 
 If you want to use the latest development version (may be broken/buggy from time to time), you can install it by:
 
 1. Cloning the repository:
     ```bash
     git clone https://github.com/six-two/mkdocs-placeholder-plugin
     cd mkdocs-placeholder-plugin
     ```
 2. Building/Downloading the JavaScript files.
     Choose any of the following ways:
     
     - Build it with npm (natively), by running the `./build-docs.sh` script.
-    - Build it in a (docker/podman) container by using the `Doeckerfile` in the `typescript` directory:
+    - Build it in a (docker/podman) container by using the `Dockerfile` in the `typescript` directory.
+        The whole thing can be done by running the `buils.sh` script in the root directory:
         ```bash
-        cd typescript
-        podman build --tag placeholder-npm .
-        cd ..
+        ./build.sh
         ```
-
-        And then running the `./build.sh` script.
         Once you see mkdocs running, you can terminate it with `Ctrl-C`.
     - Downloading the files from the development version of the documentation (hosted and built by Vercel):
         ```bash
         curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js
         curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js.map -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
         ```
 3. Installing the package with pip:
@@ -45,15 +42,20 @@
     python3 -m pip install .
     ```
 
 The corresponding documentation is hosted at <https://dev.mkdocs-placeholder-plugin.six-two.dev>.
 
 ## Notable changes
 
-### HEAD
+### Version 0.4.1
+
+- Validators can copy rules from other validators via the `import_rules_from` attribute
+- New validators: `email`, `linux_interface`, `mac_address`, `uuid`
+
+### Version 0.4.0
 
 - Configuration format changed:
     - Validators are no longer defined in-line and instead defined in a `validators` section -> easier to reuse custom validators.
     - Placeholders now need to be specified in a `placeholders` section.
     - Most settings are now in the configuration file instead of in your `mkdocs.yml`.
 - Some actions can now be toggled by visitors of the site. The settings open when you click the gear icon on a (dynamic) placeholder input table.
 - (By default) values are saved when the focus leaves a text field.
@@ -155,21 +157,22 @@
     mypy src
     ```
     ```
     pyflakes src
     ```
 2. Update the changelog in this README file.
 3. Update version number in `setup.cfg`.
-4. Build and update package.
-5. Create a commit for the release (`Version 0.X.Y`) and push it.
-6. Add a tag named `0.X.Y`:
+4. Disable `debug_javascript` in `placeholder-plugin.yaml`.
+5. Build and update package.
+6. Create a commit for the release (`Version 0.X.Y`) and push it.
+7. Add a tag named `0.X.Y`:
     ```
     git tag 0.X.Y
     ```
-7. Update the `latest-release` branch, so that the documentation website gets updated:
+8. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
     git push --tags origin latest-release
     ```
 
 ### Updating python dependencies
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/setup.cfg` & `mkdocs-placeholder-plugin-0.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-placeholder-plugin
-version = 0.4.0
+version = 0.4.1
 author = six-two
 author_email = pip@six-two.dev
 description = Add dynamic placeholders to your mkdocs page
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/six-two/mkdocs-placeholder-plugin
 license = MIT License
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/__init__.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/__init__.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/configuration.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # pip packages
 import yaml
 # local
 from .. import PlaceholderConfigError
 from .parser_utils import assert_no_unknown_fields, get_bool, get_int, get_string, get_dict, add_problematic_data_to_exceptions
 from .validator import Validator, parse_validators
 from .placeholder import Placeholder, parse_placeholders
-from ..validators_predefined import VALIDATOR_PRESETS
 
 CONFIGURATION_FIELD_NAMES = {
     "placeholders",
     "settings",
     "validators",
 }
 
@@ -115,19 +114,15 @@
 def parse_configuration(data: dict, location: str) -> PlaceholderConfig:
     assert_no_unknown_fields(data, CONFIGURATION_FIELD_NAMES)
 
     settings_data = get_dict(data, "settings", default={})
     settings = parse_settings(settings_data, f"{location}.settings")
 
     validator_data = get_dict(data, "validators", default={})
-    validators = parse_validators(validator_data, f"{location}.validators")
-
-    # Clone presets and merge/overwrite them with the custom ones
-    merged_validators = dict(VALIDATOR_PRESETS)
-    merged_validators.update(validators)
+    merged_validators = parse_validators(validator_data, f"{location}.validators")
 
     placeholder_data = get_dict(data, "placeholders")
     placeholders = parse_placeholders(placeholder_data, f"{location}.placeholders", merged_validators)
 
     return PlaceholderConfig(
         placeholders=placeholders,
         settings=settings,
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/parser_utils.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/parser_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import wraps
 import json
-from typing import Callable, Optional
+from typing import Callable, Optional, Type
 # local
 from .. import PlaceholderConfigError
 
 class PlaceholderConfigErrorWithData(PlaceholderConfigError):
     """
     Config exception that already has data of what caused it appended.
     This makes finding the error in your configuration much easier.
@@ -14,15 +14,15 @@
         super().__init__(f"{message}\n\nCaused by data at {location}: {json.dumps(data, indent=4)}")
         self.error_location = location
         self.error_data = data
 
 def assert_no_unknown_fields(data: dict, known_field_names: set[str]) -> None:
     unexpected_fields = set(data).difference(known_field_names)
     if unexpected_fields:
-        raise PlaceholderConfigError(f"Unexpected field(s): {', '.join(unexpected_fields)}")
+        raise PlaceholderConfigError(f"Unexpected field(s): {', '.join(unexpected_fields)}\n[Hint] Allowed fields are: {', '.join(known_field_names)}")
 
 def add_problematic_data_to_exceptions(function: Callable) -> Callable:
     @wraps(function)
     def wrap(data: dict, location: str, *args, **kwargs):
         try:
             return function(data, location, *args, **kwargs)
         except PlaceholderConfigErrorWithData:
@@ -64,14 +64,34 @@
 
     if type(value) == dict:
         return value
     else:
         raise PlaceholderConfigError(f"Wrong type for key '{name}': Expected 'dict', got '{type(value).__name__}'")
 
 
+def get_list(data: dict, name: str, item_type: Type, default: Optional[list] = None) -> list:
+    """
+    Reads the given key from data. If no value is used, default is used.
+    If default is None/not set then a KeyError will be thrown.
+    It will also be ensured, that each item has the specified type.
+    """
+    if default == None:
+        value = data[name]
+    else:
+        value = data.get(name, default)
+
+    if type(value) == list:
+        for index, item in enumerate(value):
+            if type(item) != item_type:
+                raise PlaceholderConfigError(f"Wrong type for key '{name}' at index {index}: Expected '{item_type.__name__}', got '{type(item).__name__}'")
+        return value
+    else:
+        raise PlaceholderConfigError(f"Wrong type for key '{name}': Expected 'list', got '{type(value).__name__}'")
+
+
 def get_string(data: dict, name: str, default: Optional[str] = None, allow_empty_string: bool = True, allow_numeric: bool = False) -> str:
     """
     Reads the given key from data. If no value is used, default is used.
     If default is None/not set then a KeyError will be thrown
     """
     if default == None:
         value = data[name]
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/placeholder.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/config/placeholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from enum import Enum, auto
 import re
 from typing import NamedTuple, Any
 # local
 from .. import warning, PlaceholderConfigError
 from .validator import Validator
-from ..validator_functions import assert_matches_one_validator
-from ..validators_predefined import VALIDATOR_PRESETS
+from ..validators import assert_matches_one_validator, VALIDATOR_PRESETS
 from .parser_utils import assert_no_unknown_fields, add_problematic_data_to_exceptions, get_bool, get_string
 
 
 # Should only contain letters, numbers, and underscores (hopefully prevents them from being broken up by syntax highlighting)
 # Should not begin with a number (this prevents placeholders like `1`)
 # Should not begin or end with a underscore (they are reserved for internal purposes like state tracking)
 VARIABLE_NAME_REGEX = re.compile("^[A-Z]([A-Z0-9_]*[A-Z0-9])?$")
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/generic_style.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/generic_style.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
     width: 1.1em;
     height: 1.1em;
     cursor: pointer;
     margin: 0 auto;
     display: block;
 }
 
+/* Hide empty auto input tables' borders & co if JS is disabled (not working in Firefox) */
+.auto-input-table:has(noscript:empty) {
+    display: none;
+}
+
 .auto-input-table .button-bar {
     margin-top: 10px;
     display: flex;
 }
 
 .auto-input-table button {
     padding: 4px;
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_handler.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/html_tag_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_parser.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/html_tag_parser.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/json_generator.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/json_generator.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/page_processor.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/page_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .config import PlaceholderConfig
 from .static.placeholder_replacer import DynamicPlaceholderPreprocessor
 from .static.table_replacer import StaticHtmlElementTableFallbackReplacer
 from .static.table_generator import TableGenerator
 from .static.input_elements import StaticInputElementReplacer
 from .html_tag_handler import NormalHtmlInputElementHandler, HtmlTagHandler
 
+END_OF_TITLE = "</h1>"
+
 class PageProcessor:
     def __init__(self, config: PlaceholderConfig) -> None:
         self.config = config
         self.dynamic_placeholder_preprocessor = DynamicPlaceholderPreprocessor(config)
         self.table_generator = TableGenerator(config)
         self.generate_fallback = self.config.settings.create_no_js_fallback
 
@@ -23,20 +25,21 @@
         
         self.input_tag_modifier: HtmlTagHandler = StaticInputElementReplacer(config.placeholders, add_line_in_warning) \
             if self.generate_fallback else NormalHtmlInputElementHandler(config.placeholders, add_line_in_warning)
 
     def process_page_markdown(self, markdown: str) -> str:
         if self.config.settings.create_no_js_fallback:
             markdown = self.dynamic_placeholder_preprocessor.handle_markdown_page(markdown)
-        
-        if self.config.settings.auto_placeholder_tables:
-            markdown = '<div class="auto-input-table" data-hide-empty data-columns="description-or-name,input"></div>\n\n' + markdown
-        
+                
         return markdown
 
     def process_page_html(self, file_path: str, html: str) -> str:
+        if self.config.settings.auto_placeholder_tables:
+            # Add directly behind the title. Looks better than simply appending before everything else
+            html = html.replace(END_OF_TITLE, f'{END_OF_TITLE}<div class="auto-input-table" data-hide-empty data-columns="description-or-name,input"></div>', 1) 
+
         if self.config.settings.create_no_js_fallback:
             html = self.dynamic_placeholder_preprocessor.handle_html_page(html)
             html = self.html_table_replacer.process_string(file_path, html)
 
         html = self.input_tag_modifier.process_string(file_path, html)
         return html
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/input_elements.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/input_elements.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/placeholder_replacer.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/placeholder_replacer.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/table_generator.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/table_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         column_list = ["description-or-name", "input"]
 
         no_js_table = ""
         if create_no_js_version:
             used_placeholders = self.get_placeholders_for_table(page_markdown)
             no_js_table = self.generate_table_html(used_placeholders, column_list)
 
-        return f'<div class="auto-input-table" data-columns="{",".join(column_list)}">{no_js_table}</div>'
+        return f'<div class="auto-input-table" data-columns="{",".join(column_list)}"><noscript>{no_js_table}</noscript></div>'
 
     def get_placeholders_for_table(self, page_markdown: str) -> list[Placeholder]:
         directly_referenced = [placeholder for placeholder in self.config.placeholders.values()
                 if not placeholder.read_only and self.is_placeholder_on_page(placeholder, page_markdown)]
         
         all_used_placeholders = list(directly_referenced)
         for placeholder in directly_referenced:
@@ -43,14 +43,17 @@
                 return True
         
         # Already preprocessed element that will use the placeholder via the dynamic replacement method
         # Looks like this: <span class="placeholder-value" data-placeholder="DEMO_FILENAME">file_to_transfer.txtp</span>
         return f'data-placeholder="{placeholder.name}"' in page_markdown
 
     def generate_table_html(self, placeholder_list: list[Placeholder], column_list: list[str]) -> str:
+        if not placeholder_list:
+            return ""
+        
         #@TODO: actually handle the passed columns? Would be more complicated but also more consistent
         rows = []
         for placeholder in placeholder_list:
             description_or_name = placeholder.description if placeholder.description else placeholder.name
             input_element = create_disabled_input_html(placeholder)
             rows.append(f"<tr><td>{html.escape(description_or_name)}</td><td>{input_element}</td></tr>")
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/table_replacer.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/generic/static/table_replacer.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/plugin.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import wraps
 import traceback
 from typing import Callable
 # pip dependency
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
-from mkdocs.config.base import Config
 from mkdocs.exceptions import PluginError
 # local files
 from .plugin_config import PlaceholderPluginConfig
 from ..generic import warning, PlaceholderConfigError, PlaceholderPageError
 from ..generic.page_processor import PageProcessor
 from .utils import initialize_plugin, copy_assets_to_mkdocs_site_directory
 
@@ -28,15 +27,15 @@
                 # Add the information, that it is a normal uncaught excaption
                 raise PluginError(f"[placeholder] Uncaught exception: {ex}")
     return wrap
 
 
 class PlaceholderPlugin(BasePlugin[PlaceholderPluginConfig]):
     @convert_exceptions
-    def on_config(self, config: MkDocsConfig, **kwargs) -> Config:
+    def on_config(self, config: MkDocsConfig, **kwargs) -> MkDocsConfig:
         """
         Called once when the config is loaded.
         It will make modify the config and initialize this plugin.
         """
         if self.config.enabled:
             self.configuration = initialize_plugin(config, self.config)
             self.page_processor = PageProcessor(self.configuration)
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/plugin_config.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/plugin_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/style.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/style.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/utils.py` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin/mkdocs/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import logging
 import os
 # pip dependency
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.exceptions import PluginError
 from ..generic import set_logger
-from mkdocs.utils import warning_filter
 
 # local files
 # local
 from ..generic.config import PlaceholderConfig
 from .style import generate_mkdocs_style_sheet
 from .plugin_config import PlaceholderPluginConfig
 from ..generic.config.configuration import parse_configuration_file
 from ..assets import copy_assets_to_directory_debuggable, copy_assets_to_directory_combined, COMBINED_FILE_NAME, DEBUGGABLE_CODE_FILE_NAME, DEBUGGABLE_DATA_FILE_NAME
 from ..generic import set_warnings_enabled
 
 def initialize_plugin(mkdocs_config: MkDocsConfig, plugin_config: PlaceholderPluginConfig) -> PlaceholderConfig:
     # To get the correct looks, the logger needs to have the correct name
     logger = logging.getLogger("mkdocs.plugins.placeholder")
-    logger.addFilter(warning_filter)
     set_logger(logger)
 
     placeholder_config = find_and_parse_configuration_file(mkdocs_config, plugin_config)
     set_warnings_enabled(placeholder_config.settings.show_warnings)
 
     register_asset_files(mkdocs_config, plugin_config, placeholder_config)
 
@@ -31,14 +29,18 @@
 
 def register_asset_files(mkdocs_config: MkDocsConfig, plugin_config: PlaceholderPluginConfig, placeholder_config: PlaceholderConfig) -> None:
     # Make sure that the custom JS is included on every page
     # Which output files are generated is determined by whether the debugging is enabled
     js_file_name_list = [DEBUGGABLE_CODE_FILE_NAME, DEBUGGABLE_DATA_FILE_NAME] if placeholder_config.settings.debug_javascript else [COMBINED_FILE_NAME]
     for file_name in js_file_name_list:
         js_file_path = os.path.join(plugin_config.js_output_dir, file_name)
+        # The linter gives a warning here, but it should be fine:
+        # Breaking change: config.extra_javascript is no longer a plain list of strings, but instead a list of ExtraScriptValue items. So you can no longer treat the list values as strings. If you want to keep compatibility with old versions, just always reference the items as str(item) instead. And you can still append plain strings to the list if you wish.
+        # Source: https://www.mkdocs.org/about/release-notes/#version-150-2023-07-26
+        # My note: If I upgraded to use the correct type, it would require MkDocs 1.5.0
         add_to_list_if_not_already_exists(mkdocs_config.extra_javascript, js_file_path)
 
     # Make sure that the custom CSS is included on every page
     if plugin_config.placeholder_css:
         add_to_list_if_not_already_exists(mkdocs_config.extra_css, plugin_config.placeholder_css)
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-placeholder-plugin
-Version: 0.4.0
+Version: 0.4.1
 Summary: Add dynamic placeholders to your mkdocs page
 Home-page: https://github.com/six-two/mkdocs-placeholder-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -25,37 +25,34 @@
 This plugin allows you to have placeholders in your site, that can be dynamically replaced at runtime using JavaScript (see [demo page](https://mkdocs-placeholder-plugin.six-two.dev/demo/)).
 
 
 ## Documentation
 
 This README is just a short intro to the package.
 For a quick start and detailed information please see the [documentation for the last release](https://mkdocs-placeholder-plugin.six-two.dev/).
-The documentation is also available in the `docs` folder of the source code and can be built localy with [MkDocs](https://www.mkdocs.org/).
+The documentation is also available in the `docs` folder of the source code and can be built locally with [MkDocs](https://www.mkdocs.org/).
 
 ## Development version
 
 If you want to use the latest development version (may be broken/buggy from time to time), you can install it by:
 
 1. Cloning the repository:
     ```bash
     git clone https://github.com/six-two/mkdocs-placeholder-plugin
     cd mkdocs-placeholder-plugin
     ```
 2. Building/Downloading the JavaScript files.
     Choose any of the following ways:
     
     - Build it with npm (natively), by running the `./build-docs.sh` script.
-    - Build it in a (docker/podman) container by using the `Doeckerfile` in the `typescript` directory:
+    - Build it in a (docker/podman) container by using the `Dockerfile` in the `typescript` directory.
+        The whole thing can be done by running the `buils.sh` script in the root directory:
         ```bash
-        cd typescript
-        podman build --tag placeholder-npm .
-        cd ..
+        ./build.sh
         ```
-
-        And then running the `./build.sh` script.
         Once you see mkdocs running, you can terminate it with `Ctrl-C`.
     - Downloading the files from the development version of the documentation (hosted and built by Vercel):
         ```bash
         curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js
         curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js.map -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
         ```
 3. Installing the package with pip:
@@ -63,15 +60,20 @@
     python3 -m pip install .
     ```
 
 The corresponding documentation is hosted at <https://dev.mkdocs-placeholder-plugin.six-two.dev>.
 
 ## Notable changes
 
-### HEAD
+### Version 0.4.1
+
+- Validators can copy rules from other validators via the `import_rules_from` attribute
+- New validators: `email`, `linux_interface`, `mac_address`, `uuid`
+
+### Version 0.4.0
 
 - Configuration format changed:
     - Validators are no longer defined in-line and instead defined in a `validators` section -> easier to reuse custom validators.
     - Placeholders now need to be specified in a `placeholders` section.
     - Most settings are now in the configuration file instead of in your `mkdocs.yml`.
 - Some actions can now be toggled by visitors of the site. The settings open when you click the gear icon on a (dynamic) placeholder input table.
 - (By default) values are saved when the focus leaves a text field.
@@ -173,21 +175,22 @@
     mypy src
     ```
     ```
     pyflakes src
     ```
 2. Update the changelog in this README file.
 3. Update version number in `setup.cfg`.
-4. Build and update package.
-5. Create a commit for the release (`Version 0.X.Y`) and push it.
-6. Add a tag named `0.X.Y`:
+4. Disable `debug_javascript` in `placeholder-plugin.yaml`.
+5. Build and update package.
+6. Create a commit for the release (`Version 0.X.Y`) and push it.
+7. Add a tag named `0.X.Y`:
     ```
     git tag 0.X.Y
     ```
-7. Update the `latest-release` branch, so that the documentation website gets updated:
+8. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
     git push --tags origin latest-release
     ```
 
 ### Updating python dependencies
```

### Comparing `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt` & `mkdocs-placeholder-plugin-0.4.1/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,27 @@
 src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
 src/mkdocs_placeholder_plugin/generic/__init__.py
 src/mkdocs_placeholder_plugin/generic/generic_style.py
 src/mkdocs_placeholder_plugin/generic/html_tag_handler.py
 src/mkdocs_placeholder_plugin/generic/html_tag_parser.py
 src/mkdocs_placeholder_plugin/generic/json_generator.py
 src/mkdocs_placeholder_plugin/generic/page_processor.py
-src/mkdocs_placeholder_plugin/generic/validator_functions.py
-src/mkdocs_placeholder_plugin/generic/validators_predefined.py
 src/mkdocs_placeholder_plugin/generic/config/__init__.py
 src/mkdocs_placeholder_plugin/generic/config/configuration.py
 src/mkdocs_placeholder_plugin/generic/config/parser_utils.py
 src/mkdocs_placeholder_plugin/generic/config/placeholder.py
 src/mkdocs_placeholder_plugin/generic/config/validator.py
 src/mkdocs_placeholder_plugin/generic/static/__init__.py
 src/mkdocs_placeholder_plugin/generic/static/input_elements.py
 src/mkdocs_placeholder_plugin/generic/static/placeholder_replacer.py
 src/mkdocs_placeholder_plugin/generic/static/table_generator.py
 src/mkdocs_placeholder_plugin/generic/static/table_replacer.py
+src/mkdocs_placeholder_plugin/generic/validators/__init__.py
+src/mkdocs_placeholder_plugin/generic/validators/files.py
+src/mkdocs_placeholder_plugin/generic/validators/internet.py
+src/mkdocs_placeholder_plugin/generic/validators/ip_address.py
+src/mkdocs_placeholder_plugin/generic/validators/network.py
 src/mkdocs_placeholder_plugin/mkdocs/__init__.py
 src/mkdocs_placeholder_plugin/mkdocs/plugin.py
 src/mkdocs_placeholder_plugin/mkdocs/plugin_config.py
 src/mkdocs_placeholder_plugin/mkdocs/style.py
 src/mkdocs_placeholder_plugin/mkdocs/utils.py
```

