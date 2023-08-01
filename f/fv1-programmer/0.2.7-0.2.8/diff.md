# Comparing `tmp/fv1_programmer-0.2.7.tar.gz` & `tmp/fv1_programmer-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.2.7.tar", max compression
+gzip compressed data, was "fv1_programmer-0.2.8.tar", max compression
```

## Comparing `fv1_programmer-0.2.7.tar` & `fv1_programmer-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/LICENSE
--rw-r--r--   0        0        0      613 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/README.md
--rw-r--r--   0        0        0     1140 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/adaptor/mcp2221.py
--rw-r--r--   0        0        0       30 2023-08-01 20:33:17.468468 fv1_programmer-0.2.7/asfv1/.git
--rw-r--r--   0        0        0     1157 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/LICENSE
--rw-r--r--   0        0        0    36334 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/README.md
--rw-r--r--   0        0        0    54482 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/asfv1.py
--rw-r--r--   0        0        0      561 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/example.asm
--rw-r--r--   0        0        0      801 2023-08-01 20:33:18.664525 fv1_programmer-0.2.7/asfv1/setup.py
--rw-r--r--   0        0        0       31 2023-08-01 20:33:17.864487 fv1_programmer-0.2.7/disfv1/.git
--rw-r--r--   0        0        0     1157 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/LICENSE
--rw-r--r--   0        0        0     4816 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/README.md
--rw-r--r--   0        0        0    17532 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/disfv1.py
--rw-r--r--   0        0        0      512 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/example.bin
--rw-r--r--   0        0        0      798 2023-08-01 20:33:18.672525 fv1_programmer-0.2.7/disfv1/setup.py
--rw-r--r--   0        0        0     6747 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/eeprom/eeprom.py
--rw-r--r--   0        0        0     1717 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/fv1.py
--rw-r--r--   0        0        0     3081 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/main.py
--rw-r--r--   0        0        0     3160 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/tui.css
--rw-r--r--   0        0        0    22358 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/fv1_programmer/tui.py
--rw-r--r--   0        0        0     1267 2023-08-01 20:33:16.688431 fv1_programmer-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 fv1_programmer-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/LICENSE
+-rw-r--r--   0        0        0      613 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/README.md
+-rw-r--r--   0        0        0     1140 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2023-08-01 20:49:20.371855 fv1_programmer-0.2.8/asfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2023-08-01 20:49:21.771947 fv1_programmer-0.2.8/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2023-08-01 20:49:20.959894 fv1_programmer-0.2.8/disfv1/.git
+-rw-r--r--   0        0        0     1157 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2023-08-01 20:49:21.775947 fv1_programmer-0.2.8/disfv1/setup.py
+-rw-r--r--   0        0        0     6747 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1717 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3081 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/main.py
+-rw-r--r--   0        0        0     3160 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    22380 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1267 2023-08-01 20:49:19.703810 fv1_programmer-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 fv1_programmer-0.2.8/PKG-INFO
```

### Comparing `fv1_programmer-0.2.7/LICENSE` & `fv1_programmer-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/README.md` & `fv1_programmer-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/adaptor/adapter.py` & `fv1_programmer-0.2.8/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/adaptor/mcp2221.py` & `fv1_programmer-0.2.8/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/asfv1/.gitignore` & `fv1_programmer-0.2.8/asfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/asfv1/LICENSE` & `fv1_programmer-0.2.8/asfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/asfv1/README.md` & `fv1_programmer-0.2.8/asfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/asfv1/asfv1.py` & `fv1_programmer-0.2.8/asfv1/asfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/asfv1/example.asm` & `fv1_programmer-0.2.8/asfv1/example.asm`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/asfv1/setup.py` & `fv1_programmer-0.2.8/asfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/disfv1/.gitignore` & `fv1_programmer-0.2.8/disfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/disfv1/LICENSE` & `fv1_programmer-0.2.8/disfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/disfv1/README.md` & `fv1_programmer-0.2.8/disfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/disfv1/disfv1.py` & `fv1_programmer-0.2.8/disfv1/disfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/disfv1/setup.py` & `fv1_programmer-0.2.8/disfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/eeprom/eeprom.py` & `fv1_programmer-0.2.8/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/fv1_programmer/fv1.py` & `fv1_programmer-0.2.8/fv1_programmer/fv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/fv1_programmer/main.py` & `fv1_programmer-0.2.8/fv1_programmer/main.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/fv1_programmer/tui.css` & `fv1_programmer-0.2.8/fv1_programmer/tui.css`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.7/fv1_programmer/tui.py` & `fv1_programmer-0.2.8/fv1_programmer/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 from typing import Iterable
 from pathlib import Path
 from fv1_programmer.fv1 import FV1Program, FV1_PROGRAM_MAX_BYTES
 import pyperclip
 
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 _title = "FV1 Programmer"
 
 class BusyScreen(ModalScreen):
     def __init__(self, message : str) -> None:
         self.message = message
         super().__init__()
@@ -371,14 +371,15 @@
             adaptor.open()
             return I2CEEPROM(adaptor, self.app.cmdline_args.ee_size,
                              page_size_in_bytes=self.app.cmdline_args.ee_page_size)
 
     @work(exclusive=True)
     def write_eeprom(self, programs : Iterable[dict], simulate : bool) -> None:
         worker = get_current_worker()
+        eeprom = None
         try:
             eeprom = self._get_eeprom()
         except Exception as e:
             if not worker.is_cancelled:
                 self.post_message(self.WriteEepromResult(programs, error=e))
 
         if eeprom is not None:
```

### Comparing `fv1_programmer-0.2.7/pyproject.toml` & `fv1_programmer-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.2.7"
+version = "0.2.8"
 description = "An EEPROM programming tool for the FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `fv1_programmer-0.2.7/PKG-INFO` & `fv1_programmer-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fv1-programmer
-Version: 0.2.7
+Version: 0.2.8
 Summary: An EEPROM programming tool for the FV-1 DSP
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@audiofab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

