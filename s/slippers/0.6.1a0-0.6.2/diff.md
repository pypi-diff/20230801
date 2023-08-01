# Comparing `tmp/slippers-0.6.1a0.tar.gz` & `tmp/slippers-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippers-0.6.1a0.tar", max compression
+gzip compressed data, was "slippers-0.6.2.tar", max compression
```

## Comparing `slippers-0.6.1a0.tar` & `slippers-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-07-27 15:26:20.255319 slippers-0.6.1a0/LICENSE
--rw-r--r--   0        0        0     2059 2023-07-27 15:26:20.255319 slippers-0.6.1a0/README.md
--rw-r--r--   0        0        0     1213 2023-07-27 15:26:20.267319 slippers-0.6.1a0/pyproject.toml
--rw-r--r--   0        0        0       52 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/__init__.py
--rw-r--r--   0        0        0     1861 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/apps.py
--rw-r--r--   0        0        0      783 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/conf.py
--rw-r--r--   0        0        0     4833 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/props.py
--rw-r--r--   0        0        0     7361 2023-07-27 15:27:36.693054 slippers-0.6.1a0/slippers/static/slippers/main.css
--rw-r--r--   0        0        0   146850 2023-07-27 15:27:36.693054 slippers-0.6.1a0/slippers/static/slippers/main.js
--rw-r--r--   0        0        0     5801 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/template.py
--rw-r--r--   0        0        0      327 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templates/slippers/overlay.html
--rw-r--r--   0        0        0        0 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templatetags/__init__.py
--rw-r--r--   0        0        0     8957 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templatetags/slippers.py
--rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 slippers-0.6.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-01 05:03:10.146541 slippers-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2059 2023-08-01 05:03:10.146541 slippers-0.6.2/README.md
+-rw-r--r--   0        0        0     1144 2023-08-01 05:03:10.158541 slippers-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/__init__.py
+-rw-r--r--   0        0        0     1861 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/apps.py
+-rw-r--r--   0        0        0      670 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/conf.py
+-rw-r--r--   0        0        0     4698 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/props.py
+-rw-r--r--   0        0        0     7361 2023-08-01 05:04:12.667132 slippers-0.6.2/slippers/static/slippers/main.css
+-rw-r--r--   0        0        0   146850 2023-08-01 05:04:12.667132 slippers-0.6.2/slippers/static/slippers/main.js
+-rw-r--r--   0        0        0     5774 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/template.py
+-rw-r--r--   0        0        0      327 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/templates/slippers/overlay.html
+-rw-r--r--   0        0        0        0 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/templatetags/__init__.py
+-rw-r--r--   0        0        0     8973 2023-08-01 05:03:10.158541 slippers-0.6.2/slippers/templatetags/slippers.py
+-rw-r--r--   0        0        0     3245 1970-01-01 00:00:00.000000 slippers-0.6.2/PKG-INFO
```

### Comparing `slippers-0.6.1a0/LICENSE` & `slippers-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1a0/README.md` & `slippers-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1a0/pyproject.toml` & `slippers-0.6.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 [tool.poetry]
 name = "slippers"
-version = "0.6.1a0"
+version = "0.6.2"
 description = "Build reusable components in Django without writing a single line of Python."
 authors = ["Mitchel Cabuloy <mixxorz@gmail.com>"]
 keywords = ["django", "components"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/mixxorz/slippers"
 repository = "https://github.com/mixxorz/slippers"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
 ]
 include = [
     "LICENSE",
     "slippers/static/slippers/main.js",
     "slippers/static/slippers/main.css",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7.0"
+python = ">=3.8.0"
 Django = ">=3.2"
 PyYAML = ">=5.4.0"
 typeguard = "^2.13.3"
 typing-extensions = ">=4.4.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
-isort = "^5.9.2"
-flake8 = "^3.9.2"
-ipdb = "^0.13.9"
-tox = "^3.23.1"
-twine = "^4.0.1"
+black = "^23.7.0"
+isort = "^5.12.0"
+flake8 = "^6.0.0"
+ipdb = "^0.13.13"
+tox = "^4.6.4"
+twine = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `slippers-0.6.1a0/slippers/apps.py` & `slippers-0.6.2/slippers/apps.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1a0/slippers/conf.py` & `slippers-0.6.2/slippers/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-import sys
-from typing import List
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+from typing import List, Literal
 
 from django.conf import settings as django_settings
 
 
 class Settings:
     @property
     def SLIPPERS_RUNTIME_TYPE_CHECKING(self) -> bool:
```

### Comparing `slippers-0.6.1a0/slippers/props.py` & `slippers-0.6.2/slippers/props.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import json
-import sys
 from collections.abc import Mapping
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
-
-if sys.version_info >= (3, 8):
-    from typing import Literal, get_args, get_origin
-else:
-    from typing_extensions import Literal, get_args, get_origin
+from typing import Any, Dict, List, Literal, Optional, Union, get_args, get_origin
 
 from django.utils.html import SafeString
 from django.utils.safestring import mark_safe
 
 from typeguard import check_type, get_type_name
```

### Comparing `slippers-0.6.1a0/slippers/static/slippers/main.css` & `slippers-0.6.2/slippers/static/slippers/main.css`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1a0/slippers/static/slippers/main.js` & `slippers-0.6.2/slippers/static/slippers/main.js`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1a0/slippers/template.py` & `slippers-0.6.2/slippers/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,33 +17,33 @@
 ########################################################################################################################
 # Custom FilterExpression
 #
 # This is a copy of the original FilterExpression. The only difference is to allow variable names to have extra special
 # characters: -, :, and @
 ########################################################################################################################
 filter_raw_string = r"""
-^(?P<constant>%(constant)s)|
-^(?P<var>[%(var_chars)s]+|%(num)s)|
- (?:\s*%(filter_sep)s\s*
+^(?P<constant>{constant})|
+^(?P<var>[{var_chars}]+|{num})|
+ (?:\s*{filter_sep}\s*
      (?P<filter_name>\w+)
-         (?:%(arg_sep)s
+         (?:{arg_sep}
              (?:
-              (?P<constant_arg>%(constant)s)|
-              (?P<var_arg>[%(var_chars)s]+|%(num)s)
+              (?P<constant_arg>{constant})|
+              (?P<var_arg>[{var_chars}]+|{num})
              )
          )?
- )""" % {
-    "constant": constant_string,
-    "num": r"[-+\.]?\d[\d\.e]*",
+ )""".format(
+    constant=constant_string,
+    num=r"[-+\.]?\d[\d\.e]*",
     # The following is the only difference from the original FilterExpression. We allow variable names to have extra
     # special characters: -, :, and @
-    "var_chars": r"\w\-\:\@\.",
-    "filter_sep": re.escape(FILTER_SEPARATOR),
-    "arg_sep": re.escape(FILTER_ARGUMENT_SEPARATOR),
-}
+    var_chars=r"\w\-\:\@\.",
+    filter_sep=re.escape(FILTER_SEPARATOR),
+    arg_sep=re.escape(FILTER_ARGUMENT_SEPARATOR),
+)
 
 filter_re = _lazy_re_compile(filter_raw_string, re.VERBOSE)
 
 
 class SlippersFilterExpression(FilterExpression):
     def __init__(self, token, parser):
         # This method is exactly the same as the original FilterExpression.__init__ method, the only difference being
```

### Comparing `slippers-0.6.1a0/slippers/templatetags/slippers.py` & `slippers-0.6.2/slippers/templatetags/slippers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import Any, Dict, Tuple
 from warnings import warn
 
 from django import template
 from django.conf import settings as django_settings
-from django.template import Context
+from django.template import Context, NodeList
 from django.utils.safestring import mark_safe
 
 from slippers.conf import settings
 from slippers.props import Props, check_prop_types, render_error_html
 from slippers.template import slippers_token_kwargs
 
 register = template.Library()
@@ -22,15 +22,15 @@
 
         # Block components start with `#`
         # Expect a closing tag
         if tag_name[0] == "#":
             nodelist = parser.parse((f"/{tag_name[1:]}",))
             parser.delete_first_token()
         else:
-            nodelist = None
+            nodelist = NodeList()
 
         # Bits that are not keyword args are interpreted as `True` values
         all_bits = [bit if "=" in bit else f"{bit}=True" for bit in remaining_bits]
 
         raw_attributes = slippers_token_kwargs(all_bits, parser)
 
         # Allow component fragment to be assigned to a variable
```

### Comparing `slippers-0.6.1a0/PKG-INFO` & `slippers-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: slippers
-Version: 0.6.1a0
+Version: 0.6.2
 Summary: Build reusable components in Django without writing a single line of Python.
 Home-page: https://github.com/mixxorz/slippers
 License: MIT
 Keywords: django,components
 Author: Mitchel Cabuloy
 Author-email: mixxorz@gmail.com
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=3.2)
 Requires-Dist: PyYAML (>=5.4.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
```

