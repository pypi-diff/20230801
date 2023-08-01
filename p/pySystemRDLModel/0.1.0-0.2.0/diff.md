# Comparing `tmp/pySystemRDLModel-0.1.0.tar.gz` & `tmp/pySystemRDLModel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySystemRDLModel-0.1.0.tar", last modified: Sun Jul 30 13:28:13 2023, max compression
+gzip compressed data, was "pySystemRDLModel-0.2.0.tar", last modified: Tue Aug  1 21:31:21 2023, max compression
```

## Comparing `pySystemRDLModel-0.1.0.tar` & `pySystemRDLModel-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:28:13.909213 pySystemRDLModel-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-30 13:28:03.000000 pySystemRDLModel-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-30 13:28:13.909213 pySystemRDLModel-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-30 13:28:03.000000 pySystemRDLModel-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:28:13.905213 pySystemRDLModel-0.1.0/pySystemRDLModel/
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-30 13:28:03.000000 pySystemRDLModel-0.1.0/pySystemRDLModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:28:13.905213 pySystemRDLModel-0.1.0/pySystemRDLModel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-30 13:28:13.000000 pySystemRDLModel-0.1.0/pySystemRDLModel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-30 13:28:13.000000 pySystemRDLModel-0.1.0/pySystemRDLModel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 13:28:13.000000 pySystemRDLModel-0.1.0/pySystemRDLModel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-30 13:28:13.000000 pySystemRDLModel-0.1.0/pySystemRDLModel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 13:28:13.000000 pySystemRDLModel-0.1.0/pySystemRDLModel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-30 13:28:03.000000 pySystemRDLModel-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 13:28:13.909213 pySystemRDLModel-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-30 13:28:03.000000 pySystemRDLModel-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:31:21.376505 pySystemRDLModel-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-08-01 21:31:12.000000 pySystemRDLModel-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-01 21:31:21.376505 pySystemRDLModel-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-08-01 21:31:12.000000 pySystemRDLModel-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:31:21.376505 pySystemRDLModel-0.2.0/pySystemRDLModel/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-08-01 21:31:12.000000 pySystemRDLModel-0.2.0/pySystemRDLModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:31:21.376505 pySystemRDLModel-0.2.0/pySystemRDLModel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-01 21:31:21.000000 pySystemRDLModel-0.2.0/pySystemRDLModel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 21:31:21.000000 pySystemRDLModel-0.2.0/pySystemRDLModel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:31:21.000000 pySystemRDLModel-0.2.0/pySystemRDLModel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-01 21:31:21.000000 pySystemRDLModel-0.2.0/pySystemRDLModel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 21:31:21.000000 pySystemRDLModel-0.2.0/pySystemRDLModel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 21:31:12.000000 pySystemRDLModel-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:31:21.376505 pySystemRDLModel-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-08-01 21:31:12.000000 pySystemRDLModel-0.2.0/setup.py
```

### Comparing `pySystemRDLModel-0.1.0/LICENSE.md` & `pySystemRDLModel-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pySystemRDLModel-0.1.0/PKG-INFO` & `pySystemRDLModel-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySystemRDLModel
-Version: 0.1.0
+Version: 0.2.0
 Summary: An abstract SystemRDL language model.
 Home-page: https://GitHub.com/edaa-org/pySystemRDLModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pySystemRDLModel
 Project-URL: Source Code, https://GitHub.com/edaa-org/pySystemRDLModel
```

### Comparing `pySystemRDLModel-0.1.0/README.md` & `pySystemRDLModel-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pySystemRDLModel-0.1.0/pySystemRDLModel/__init__.py` & `pySystemRDLModel-0.2.0/pySystemRDLModel/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,58 +40,61 @@
 from pyTooling.Decorators import export
 
 
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2023-2023, Patrick Lehmann"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.1.0"
+__version__ =   "0.2.0"
 
 
 @export
 @unique
 class SystemRDLVersion(Enum):
-	Any =                 -1
-	SystemVerilog2005 = 2005
-	SystemVerilog2009 = 2009
-	SystemVerilog2012 = 2012
-	SystemVerilog2017 = 2017
+	Any =             -1
+	SystemRDL2005 = 2005
+	SystemRDL2009 = 2009
+	SystemRDL2012 = 2012
+	SystemRDL2017 = 2017
 
 	__VERSION_MAPPINGS__: Dict[Union[int, str], Enum] = {
-		5:      SystemVerilog2005,
-		9:      SystemVerilog2009,
-		12:     SystemVerilog2012,
-		17:     SystemVerilog2017,
-		2005:   SystemVerilog2005,
-		2009:   SystemVerilog2009,
-		2012:   SystemVerilog2012,
-		2017:   SystemVerilog2017,
+		-1:     Any,
+		5:      SystemRDL2005,
+		9:      SystemRDL2009,
+		12:     SystemRDL2012,
+		17:     SystemRDL2017,
+		2005:   SystemRDL2005,
+		2009:   SystemRDL2009,
+		2012:   SystemRDL2012,
+		2017:   SystemRDL2017,
 		"Any":  Any,
-		"05":   SystemVerilog2005,
-		"09":   SystemVerilog2009,
-		"12":   SystemVerilog2012,
-		"17":   SystemVerilog2017,
-		"2005": SystemVerilog2005,
-		"2009": SystemVerilog2009,
-		"2012": SystemVerilog2012,
-		"2017": SystemVerilog2017,
+		"05":   SystemRDL2005,
+		"09":   SystemRDL2009,
+		"12":   SystemRDL2012,
+		"17":   SystemRDL2017,
+		"2005": SystemRDL2005,
+		"2009": SystemRDL2009,
+		"2012": SystemRDL2012,
+		"2017": SystemRDL2017,
 	}
 
 	def __init__(self, *_):
 		"""Patch the embedded MAP dictionary"""
-		for k, v in self.__class__.__VERSION_MAPPINGS__.items():
-			if (not isinstance(v, self.__class__)) and (v == self.value):
-				self.__class__.__VERSION_MAPPINGS__[k] = self
+		cls = self.__class__
+		for k, v in cls.__VERSION_MAPPINGS__.items():
+			if (not isinstance(v, cls)) and (v == self.value):
+				print(f"patching {k}:{v} with {self}")
+				cls.__VERSION_MAPPINGS__[k] = self
 
 	@classmethod
-	def Parse(cls, value):
+	def Parse(cls, value: Union[int, str]) -> "SystemRDLVersion":
 		try:
 			return cls.__VERSION_MAPPINGS__[value]
 		except KeyError:
-			ValueError(f"Value '{value!s}' cannot be parsed to member of {cls.__name__}.")
+			raise ValueError(f"Value '{value!s}' cannot be parsed to member of {cls.__name__}.")
 
 	def __lt__(self, other):
 		return self.value < other.value
 
 	def __le__(self, other):
 		return self.value <= other.value
 
@@ -106,12 +109,18 @@
 
 	def __eq__(self, other):
 		if (self is self.__class__.Any) or (other is self.__class__.Any):
 			return True
 		else:
 			return self.value == other.value
 
-	def __str__(self):
-		return "SV'" + str(self.value)[-2:]
+	def __str__(self) -> str:
+		if self.value == -1:
+			return "SystemRDL'Any"
+		else:
+			return f"SystemRDL'{str(self.value)[-2:]}"
 
-	def __repr__(self):
-		return str(self.value)
+	def __repr__(self) -> str:
+		if self.value == -1:
+			return "Any"
+		else:
+			return str(self.value)
```

### Comparing `pySystemRDLModel-0.1.0/pySystemRDLModel.egg-info/PKG-INFO` & `pySystemRDLModel-0.2.0/pySystemRDLModel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySystemRDLModel
-Version: 0.1.0
+Version: 0.2.0
 Summary: An abstract SystemRDL language model.
 Home-page: https://GitHub.com/edaa-org/pySystemRDLModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pySystemRDLModel
 Project-URL: Source Code, https://GitHub.com/edaa-org/pySystemRDLModel
```

### Comparing `pySystemRDLModel-0.1.0/pyproject.toml` & `pySystemRDLModel-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pySystemRDLModel-0.1.0/setup.py` & `pySystemRDLModel-0.2.0/setup.py`

 * *Files identical despite different names*

