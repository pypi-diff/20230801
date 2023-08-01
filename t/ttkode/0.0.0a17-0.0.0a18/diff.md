# Comparing `tmp/ttkode-0.0.0a17.tar.gz` & `tmp/ttkode-0.0.0a18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttkode-0.0.0a17.tar", last modified: Fri May 26 18:33:18 2023, max compression
+gzip compressed data, was "ttkode-0.0.0a18.tar", last modified: Tue Aug  1 12:13:48 2023, max compression
```

## Comparing `ttkode-0.0.0a17.tar` & `ttkode-0.0.0a18.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/
--rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1673 2023-05-26 18:33:14.000000 ttkode-0.0.0a17/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1286 2023-05-26 18:33:14.000000 ttkode-0.0.0a17/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/ttkode/
--rwxrwxr-x   0 one       (1000) one       (1000)     1239 2022-09-28 07:52:57.000000 ttkode-0.0.0a17/ttkode/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1242 2022-09-28 07:52:57.000000 ttkode-0.0.0a17/ttkode/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/ttkode/app/
--rw-rw-r--   0 one       (1000) one       (1000)     1290 2023-05-26 17:28:55.000000 ttkode-0.0.0a17/ttkode/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     2817 2023-05-26 17:26:14.000000 ttkode-0.0.0a17/ttkode/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     2135 2023-05-26 18:33:14.000000 ttkode-0.0.0a17/ttkode/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)     6442 2022-11-16 08:57:30.000000 ttkode-0.0.0a17/ttkode/app/kodeformatter.py
--rw-rw-r--   0 one       (1000) one       (1000)     6196 2022-11-15 23:03:40.000000 ttkode-0.0.0a17/ttkode/app/kodetextdocument.py
--rw-rw-r--   0 one       (1000) one       (1000)     1440 2022-10-07 16:42:58.000000 ttkode-0.0.0a17/ttkode/app/kodetextedit.py
--rw-rw-r--   0 one       (1000) one       (1000)     6157 2023-05-26 18:24:45.000000 ttkode-0.0.0a17/ttkode/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)     3182 2022-09-28 07:52:57.000000 ttkode-0.0.0a17/ttkode/app/options.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/ttkode.egg-info/
--rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)      426 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       39 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       44 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)        7 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-08-01 12:13:48.034076 ttkode-0.0.0a18/
+-rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-08-01 12:13:48.034076 ttkode-0.0.0a18/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1673 2023-08-01 12:13:44.000000 ttkode-0.0.0a18/README.md
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2023-08-01 12:13:48.034076 ttkode-0.0.0a18/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     1286 2023-08-01 12:13:44.000000 ttkode-0.0.0a18/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-08-01 12:13:48.034076 ttkode-0.0.0a18/ttkode/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1239 2022-09-28 07:52:57.000000 ttkode-0.0.0a18/ttkode/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1242 2022-09-28 07:52:57.000000 ttkode-0.0.0a18/ttkode/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-08-01 12:13:48.034076 ttkode-0.0.0a18/ttkode/app/
+-rw-rw-r--   0 one       (1000) one       (1000)     1290 2023-05-26 17:28:55.000000 ttkode-0.0.0a18/ttkode/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2817 2023-05-26 17:26:14.000000 ttkode-0.0.0a18/ttkode/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2135 2023-08-01 12:13:44.000000 ttkode-0.0.0a18/ttkode/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6442 2022-11-16 08:57:30.000000 ttkode-0.0.0a18/ttkode/app/kodeformatter.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6196 2022-11-15 23:03:40.000000 ttkode-0.0.0a18/ttkode/app/kodetextdocument.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1440 2022-10-07 16:42:58.000000 ttkode-0.0.0a18/ttkode/app/kodetextedit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6159 2023-05-26 18:49:37.000000 ttkode-0.0.0a18/ttkode/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3182 2022-09-28 07:52:57.000000 ttkode-0.0.0a18/ttkode/app/options.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-08-01 12:13:48.034076 ttkode-0.0.0a18/ttkode.egg-info/
+-rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-08-01 12:13:48.000000 ttkode-0.0.0a18/ttkode.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)      426 2023-08-01 12:13:48.000000 ttkode-0.0.0a18/ttkode.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2023-08-01 12:13:48.000000 ttkode-0.0.0a18/ttkode.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       39 2023-08-01 12:13:48.000000 ttkode-0.0.0a18/ttkode.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       44 2023-08-01 12:13:48.000000 ttkode-0.0.0a18/ttkode.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        7 2023-08-01 12:13:48.000000 ttkode-0.0.0a18/ttkode.egg-info/top_level.txt
```

### Comparing `ttkode-0.0.0a17/PKG-INFO` & `ttkode-0.0.0a18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttkode
-Version: 0.0.0a17
+Version: 0.0.0a18
 Summary: Terminal ToolKit Studio Code editor
 Home-page: https://github.com/ceccopierangiolieugenio/ttkode
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ttkode-0.0.0a17/README.md` & `ttkode-0.0.0a18/README.md`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/setup.py` & `ttkode-0.0.0a18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.0.0a17"
+version = "0.0.0a18"
 name = "ttkode"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
```

### Comparing `ttkode-0.0.0a17/ttkode/__init__.py` & `ttkode-0.0.0a18/ttkode/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode/__main__.py` & `ttkode-0.0.0a18/ttkode/__main__.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode/app/__init__.py` & `ttkode-0.0.0a18/ttkode/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode/app/about.py` & `ttkode-0.0.0a18/ttkode/app/about.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode/app/cfg.py` & `ttkode-0.0.0a18/ttkode/app/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import yaml
 
 class TTKodeCfg:
-    version="0.0.0a17"
+    version="0.0.0a18"
     name="ttkode"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
 
     @staticmethod
```

### Comparing `ttkode-0.0.0a17/ttkode/app/kodeformatter.py` & `ttkode-0.0.0a18/ttkode/app/kodeformatter.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode/app/kodetextdocument.py` & `ttkode-0.0.0a18/ttkode/app/kodetextdocument.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode/app/kodetextedit.py` & `ttkode-0.0.0a18/ttkode/app/kodetextedit.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode/app/main.py` & `ttkode-0.0.0a18/ttkode/app/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     parser = argparse.ArgumentParser()
     # parser.add_argument('-f', help='Full Screen', action='store_true')
     parser.add_argument('-c', help=f'config folder (default: "{TTKodeCfg.pathCfg}")', default=TTKodeCfg.pathCfg)
     parser.add_argument('filename', type=str, nargs='*',
                     help='the filename/s')
     args = parser.parse_args()
 
-    TTkLog.use_default_file_logging()
+    # TTkLog.use_default_file_logging()
 
     TTKodeCfg.pathCfg = args.c
     TTkLog.debug(f"Config Path: {TTKodeCfg.pathCfg}")
 
     TTKodeCfg.load()
 
     # if 'theme' not in TTKodeCfg.options:
```

### Comparing `ttkode-0.0.0a17/ttkode/app/options.py` & `ttkode-0.0.0a18/ttkode/app/options.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a17/ttkode.egg-info/PKG-INFO` & `ttkode-0.0.0a18/ttkode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttkode
-Version: 0.0.0a17
+Version: 0.0.0a18
 Summary: Terminal ToolKit Studio Code editor
 Home-page: https://github.com/ceccopierangiolieugenio/ttkode
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

