# Comparing `tmp/pyssp_standard-0.1.tar.gz` & `tmp/pyssp_standard-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyssp_standard-0.1.tar", last modified: Tue Aug  1 15:58:06 2023, max compression
+gzip compressed data, was "pyssp_standard-0.2.tar", last modified: Tue Aug  1 16:16:48 2023, max compression
```

## Comparing `pyssp_standard-0.1.tar` & `pyssp_standard-0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:58:06.802193 pyssp_standard-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 15:57:54.000000 pyssp_standard-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 15:58:06.802193 pyssp_standard-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-01 15:57:54.000000 pyssp_standard-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:58:06.802193 pyssp_standard-0.1/pyssp_standard/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/common_content_ssc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/fmu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/ssb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/ssd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/ssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/ssv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/transformation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-01 15:57:54.000000 pyssp_standard-0.1/pyssp_standard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:58:06.802193 pyssp_standard-0.1/pyssp_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 15:58:06.000000 pyssp_standard-0.1/pyssp_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 15:58:06.000000 pyssp_standard-0.1/pyssp_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:58:06.000000 pyssp_standard-0.1/pyssp_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 15:58:06.000000 pyssp_standard-0.1/pyssp_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 15:58:06.000000 pyssp_standard-0.1/pyssp_standard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 15:58:06.806194 pyssp_standard-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-01 15:57:54.000000 pyssp_standard-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:16:48.835430 pyssp_standard-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 16:16:36.000000 pyssp_standard-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 16:16:48.835430 pyssp_standard-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-01 16:16:36.000000 pyssp_standard-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:16:48.831430 pyssp_standard-0.2/pyssp_standard/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/common_content_ssc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/fmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/ssv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/transformation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-01 16:16:36.000000 pyssp_standard-0.2/pyssp_standard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:16:48.835430 pyssp_standard-0.2/pyssp_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 16:16:48.000000 pyssp_standard-0.2/pyssp_standard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 16:16:48.835430 pyssp_standard-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-01 16:16:36.000000 pyssp_standard-0.2/setup.py
```

### Comparing `pyssp_standard-0.1/LICENSE` & `pyssp_standard-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.1/PKG-INFO` & `pyssp_standard-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssp_standard
-Version: 0.1
+Version: 0.2
 Summary: Simple python package for reading, modifying and creating files, specified in the SSP Standard
 Home-page: https://github.com/FGHaider/pyssp
 Download-URL: https://github.com/FGHaider/pyssp/archive/refs/tags/v_01.tar.gz
 Author: Fredrik Haider
 Author-email: 
 License: MIT
 Keywords: SSP,system,engineering
```

### Comparing `pyssp_standard-0.1/README.md` & `pyssp_standard-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.1/pyssp_standard/common_content_ssc.py` & `pyssp_standard-0.2/pyssp_standard/common_content_ssc.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.1/pyssp_standard/fmu.py` & `pyssp_standard-0.2/pyssp_standard/fmu.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.1/pyssp_standard/parameter_types.py` & `pyssp_standard-0.2/pyssp_standard/parameter_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypedDict
 from lxml import etree as ET
 from lxml.etree import QName
 
-from utils import SSPStandard
+from pyssp_standard.utils import SSPStandard
 
 
 class ParameterType(SSPStandard):
 
     def __init__(self, parameter_type=None, attributes=None, namespace='ssv'):
         self.namespace = namespace
```

### Comparing `pyssp_standard-0.1/pyssp_standard/ssb.py` & `pyssp_standard-0.2/pyssp_standard/ssb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xmlschema
 
-from parameter_types import ParameterType
-from common_content_ssc import Annotations, Enumerations, Annotation, Enumeration
-from unit import Unit, Units
-from utils import SSPStandard, SSPFile
+from pyssp_standard.parameter_types import ParameterType
+from pyssp_standard.common_content_ssc import Annotations, Enumerations, Annotation, Enumeration
+from pyssp_standard.unit import Unit, Units
+from pyssp_standard.utils import SSPStandard, SSPFile
 from lxml import etree as ET
 from lxml.etree import QName
 from typing import TypedDict, List
 
 
 class DictionaryEntry(TypedDict):
     name: str
```

### Comparing `pyssp_standard-0.1/pyssp_standard/ssd.py` & `pyssp_standard-0.2/pyssp_standard/ssd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
-from common_content_ssc import Enumerations, Annotations, Annotation
-from unit import Units
-from utils import SSPStandard, SSPFile
+from pyssp_standard.common_content_ssc import Enumerations, Annotations, Annotation
+from pyssp_standard.unit import Units
+from pyssp_standard.utils import SSPStandard, SSPFile
 from lxml import etree as ET
 import xmlschema
 
 
 class Connection(SSPStandard):
 
     def __init__(self, element):
```

### Comparing `pyssp_standard-0.1/pyssp_standard/ssm.py` & `pyssp_standard-0.2/pyssp_standard/ssm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import xmlschema
-from transformation_types import Transformation
-from common_content_ssc import Annotations, Annotation, BaseElement, TopLevelMetaData
-from utils import SSPStandard, SSPFile
+from pyssp_standard.transformation_types import Transformation
+from pyssp_standard.common_content_ssc import Annotations, Annotation, BaseElement, TopLevelMetaData
+from pyssp_standard.utils import SSPStandard, SSPFile
 from lxml import etree as et
 from lxml.etree import QName
 from typing import TypedDict
 
 
 class MappingEntry(TypedDict):
     source: str
```

### Comparing `pyssp_standard-0.1/pyssp_standard/ssp.py` & `pyssp_standard-0.2/pyssp_standard/ssp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 import tempfile
 import zipfile
 import shutil
 from pathlib import Path, PosixPath
 
-from ssd import SSD
-from ssb import SSB
-from ssv import SSV
-from ssm import SSM
-from fmu import FMU
-from utils import SSPStandard
+from pyssp_standard.ssd import SSD
+from pyssp_standard.ssb import SSB
+from pyssp_standard.ssv import SSV
+from pyssp_standard.ssm import SSM
+from pyssp_standard.fmu import FMU
+from pyssp_standard.utils import SSPStandard
 
 
 class SSP(SSPStandard):
 
     def __enter__(self):
         return self
```

### Comparing `pyssp_standard-0.1/pyssp_standard/ssv.py` & `pyssp_standard-0.2/pyssp_standard/ssv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from lxml import etree as ET
 from typing import TypedDict, List
 
 from lxml.etree import QName
 
-from common_content_ssc import BaseElement, TopLevelMetaData
-from parameter_types import ParameterType
+from pyssp_standard.common_content_ssc import BaseElement, TopLevelMetaData
+from pyssp_standard.parameter_types import ParameterType
 import xmlschema
 
-from unit import BaseUnit, Unit, Units
-from utils import SSPStandard, SSPFile
+from pyssp_standard.unit import BaseUnit, Unit, Units
+from pyssp_standard.utils import SSPStandard, SSPFile
 
 
 class Parameter(TypedDict):
     name: str
     type_name: str
     type_value: ParameterType
```

### Comparing `pyssp_standard-0.1/pyssp_standard/transformation_types.py` & `pyssp_standard-0.2/pyssp_standard/transformation_types.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.1/pyssp_standard/unit.py` & `pyssp_standard-0.2/pyssp_standard/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, asdict
 from lxml import etree as ET
 from lxml.etree import QName
 
-from utils import SSPElement, SSPStandard
+from pyssp_standard.utils import SSPElement, SSPStandard
 
 
 @dataclass
 class BaseUnit:
     kg: int = None
     m: int = None
     s: int = None
```

### Comparing `pyssp_standard-0.1/pyssp_standard/utils.py` & `pyssp_standard-0.2/pyssp_standard/utils.py`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.1/pyssp_standard.egg-info/PKG-INFO` & `pyssp_standard-0.2/pyssp_standard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyssp-standard
-Version: 0.1
+Version: 0.2
 Summary: Simple python package for reading, modifying and creating files, specified in the SSP Standard
 Home-page: https://github.com/FGHaider/pyssp
 Download-URL: https://github.com/FGHaider/pyssp/archive/refs/tags/v_01.tar.gz
 Author: Fredrik Haider
 Author-email: 
 License: MIT
 Keywords: SSP,system,engineering
```

### Comparing `pyssp_standard-0.1/pyssp_standard.egg-info/SOURCES.txt` & `pyssp_standard-0.2/pyssp_standard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyssp_standard-0.1/setup.py` & `pyssp_standard-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='pyssp_standard',
     packages=['pyssp_standard'],
-    version='0.1',
+    version='0.2',
     license='MIT',
     description='Simple python package for reading, modifying and creating files, specified in the SSP Standard',
     long_description='',
     long_description_content_type='text/markdown',
     author='Fredrik Haider',
     author_email='',
     url='https://github.com/FGHaider/pyssp',
```

