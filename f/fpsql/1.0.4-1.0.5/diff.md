# Comparing `tmp/fpsql-1.0.4.tar.gz` & `tmp/fpsql-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpsql-1.0.4.tar", max compression
+gzip compressed data, was "fpsql-1.0.5.tar", max compression
```

## Comparing `fpsql-1.0.4.tar` & `fpsql-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.000000 fpsql-1.0.4/LICENSE
--rw-r--r--   0        0        0      278 2023-05-26 02:00:04.970677 fpsql-1.0.4/README.md
--rw-r--r--   0        0        0      864 2023-05-26 01:59:56.442686 fpsql-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4956 2023-05-26 02:02:22.638531 fpsql-1.0.4/src/fpsql/__init__.py
--rw-r--r--   0        0        0      513 2023-05-26 02:00:39.094641 fpsql-1.0.4/src/fpsql/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-26 01:31:02.620528 fpsql-1.0.4/src/fpsql/py.typed
--rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 fpsql-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.000000 fpsql-1.0.5/LICENSE
+-rw-r--r--   0        0        0      338 2023-08-01 01:48:24.663700 fpsql-1.0.5/README.md
+-rw-r--r--   0        0        0      864 2023-08-01 01:47:43.267742 fpsql-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5006 2023-08-01 01:49:35.899631 fpsql-1.0.5/src/fpsql/__init__.py
+-rw-r--r--   0        0        0      513 2023-08-01 01:47:13.283775 fpsql-1.0.5/src/fpsql/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 01:31:02.620528 fpsql-1.0.5/src/fpsql/py.typed
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 fpsql-1.0.5/PKG-INFO
```

### Comparing `fpsql-1.0.4/LICENSE` & `fpsql-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fpsql-1.0.4/pyproject.toml` & `fpsql-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fpsql"
-version = "1.0.4"
+version = "1.0.5"
 authors = ["Firepup650 <firepyp650@gmail.com>"]
 description = "An easy to use SQLite package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `fpsql-1.0.4/src/fpsql/__init__.py` & `fpsql-1.0.5/src/fpsql/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
             + pydoc.text.document(Function)
         )
         return f
 
     return decorator
 
 
-__VERSION__ = "1.0.2"
-__NEW__ = "Fix internal vars"
+__VERSION__ = "1.0.5"
+__NEW__ = "Double check mypy problems and resolve them"
 __LICENSE__ = "MIT"
 
 
 class sql:
     def addTable(self, tableName: str, mode: int = 0, address: str = "") -> None:
         """# Function: sql.addTable
           Adds a table to the database
@@ -169,10 +169,10 @@
 
         # Returns:
           None
 
         # Raises:
           None"""
         self.__con.close()
-        self.__con = None
-        self.__db = None
-        self.__table = None
+        self.__con = None  # type: ignore[assignment]
+        self.__db = ""
+        self.__table = ""
```

### Comparing `fpsql-1.0.4/src/fpsql/__init__.pyi` & `fpsql-1.0.5/src/fpsql/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fpsql-1.0.4/PKG-INFO` & `fpsql-1.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpsql
-Version: 1.0.4
+Version: 1.0.5
 Summary: An easy to use SQLite package
 Home-page: https://github.com/F1repup650/firepup650-SQL
 License: MIT
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,14 +22,16 @@
 Project-URL: Repository, https://github.com/F1repup650/firepup650-SQL
 Project-URL: Replit, https://replit.com/@Firepup650/firepup650-SQL-Package
 Description-Content-Type: text/markdown
 
 # FPSQL
 An easy to use SQLite package
 #### Change log:
+###### v.1.0.5:
+Double check mypy problems and resolve them
 ###### v.1.0.4:
 Fix all mypy stub issues
 ###### v.1.0.3:
 Provide a mypy stub file
 ###### v.1.0.2:
 Fix internal vars
 ###### v.1.0.1:
```

