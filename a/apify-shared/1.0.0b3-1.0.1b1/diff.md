# Comparing `tmp/apify_shared-1.0.0b3.tar.gz` & `tmp/apify_shared-1.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_shared-1.0.0b3.tar", last modified: Tue Jul 25 14:42:52 2023, max compression
+gzip compressed data, was "apify_shared-1.0.1b1.tar", last modified: Tue Aug  1 08:29:58 2023, max compression
```

## Comparing `apify_shared-1.0.0b3.tar` & `apify_shared-1.0.1b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-25 14:42:48.000000 apify_shared-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/src/apify_shared/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/src/apify_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.832959 apify_shared-1.0.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 08:29:55.000000 apify_shared-1.0.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:29:58.832959 apify_shared-1.0.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/src/apify_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-08-01 08:29:32.000000 apify_shared-1.0.1b1/src/apify_shared/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:29:58.828958 apify_shared-1.0.1b1/src/apify_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 08:29:58.000000 apify_shared-1.0.1b1/src/apify_shared.egg-info/top_level.txt
```

### Comparing `apify_shared-1.0.0b3/LICENSE` & `apify_shared-1.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b3/PKG-INFO` & `apify_shared-1.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_shared
-Version: 1.0.0b3
+Version: 1.0.1b1
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.0b3/README.md` & `apify_shared-1.0.1b1/README.md`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b3/pyproject.toml` & `apify_shared-1.0.1b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dependencies = []
 description = "Tools and constants shared across Apify projects."
 keywords = ["apify", "api", "shared", "scraping", "automation"]
 license = {text = "Apache Software License"}
 name = "apify_shared"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.0.0b3"
+version = "1.0.1b1"
 
 [project.optional-dependencies]
 dev = [
   "autopep8 ~= 2.0.2",
   "build ~= 0.10.0",
   "flake8 ~= 6.0.0",
   "flake8-bugbear ~= 23.5.9",
@@ -33,15 +33,15 @@
   "flake8-encodings ~= 0.5.0",
   "flake8-isort ~= 6.0.0",
   "flake8-noqa ~= 1.3.1",
   "flake8-pytest-style ~= 1.7.2",
   "flake8-quotes ~= 3.3.2",
   "flake8-unused-arguments ~= 0.0.13",
   "isort ~= 5.12.0",
-  "mypy ~= 1.3.0",
+  "mypy ~= 1.4.0",
   "pep8-naming ~= 0.13.3",
   "pre-commit ~= 3.3.2",
   "pytest ~= 7.3.1",
   "pytest-asyncio ~= 0.21.0",
   "pytest-only ~= 2.0.0",
   "pytest-randomly ~= 3.12.0",
   "pytest-timeout ~= 2.1.0",
```

### Comparing `apify_shared-1.0.0b3/src/apify_shared/consts.py` & `apify_shared-1.0.1b1/src/apify_shared/consts.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b3/src/apify_shared/models.py` & `apify_shared-1.0.1b1/src/apify_shared/models.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b3/src/apify_shared/utils.py` & `apify_shared-1.0.1b1/src/apify_shared/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,26 @@
 PARSE_DATE_FIELDS_MAX_DEPTH = 3
 PARSE_DATE_FIELDS_KEY_SUFFIX = 'At'
 
 ListOrDict = TypeVar('ListOrDict', List, Dict)
 T = TypeVar('T')
 
 
+def ignore_docs(method: T) -> T:
+    """Mark that a method's documentation should not be rendered. Functionally, this decorator is a noop."""
+    return method
+
+
+@ignore_docs
 def filter_out_none_values_recursively(dictionary: Dict) -> Dict:
     """Return copy of the dictionary, recursively omitting all keys for which values are None."""
     return cast(dict, _filter_out_none_values_recursively_internal(dictionary))
 
 
+@ignore_docs
 def _filter_out_none_values_recursively_internal(
     dictionary: Dict,
     remove_empty_dicts: Optional[bool] = None,
 ) -> Optional[Dict]:
     """Recursively filters out None values from a dictionary.
 
     Unfortunately, it's necessary to have an internal function for the correct result typing,
@@ -33,56 +40,58 @@
         if v is not None:
             result[k] = v
     if not result and remove_empty_dicts:
         return None
     return result
 
 
-def ignore_docs(method: T) -> T:
-    """Mark that a method's documentation should not be rendered. Functionally, this decorator is a noop."""
-    return method
-
-
+@ignore_docs
 def is_content_type_json(content_type: str) -> bool:
     """Check if the given content type is JSON."""
     return bool(re.search(r'^application/json', content_type, flags=re.IGNORECASE))
 
 
+@ignore_docs
 def is_content_type_xml(content_type: str) -> bool:
     """Check if the given content type is XML."""
     return bool(re.search(r'^application/.*xml$', content_type, flags=re.IGNORECASE))
 
 
+@ignore_docs
 def is_content_type_text(content_type: str) -> bool:
     """Check if the given content type is text."""
     return bool(re.search(r'^text/', content_type, flags=re.IGNORECASE))
 
 
+@ignore_docs
 def is_file_or_bytes(value: Any) -> bool:
     """Check if the input value is a file-like object or bytes.
 
     The check for IOBase is not ideal, it would be better to use duck typing,
     but then the check would be super complex, judging from how the 'requests' library does it.
     This way should be good enough for the vast majority of use cases, if it causes issues, we can improve it later.
     """
     return isinstance(value, (bytes, bytearray, io.IOBase))
 
 
+@ignore_docs
 def json_dumps(obj: Any) -> str:
     """Dump JSON to a string with the correct settings and serializer."""
     return json.dumps(obj, ensure_ascii=False, indent=2, default=str)
 
 
+@ignore_docs
 def maybe_extract_enum_member_value(maybe_enum_member: Any) -> Any:
     """Extract the value of an enumeration member if it is an Enum, otherwise return the original value."""
     if isinstance(maybe_enum_member, Enum):
         return maybe_enum_member.value
     return maybe_enum_member
 
 
+@ignore_docs
 def parse_date_fields(data: ListOrDict, max_depth: int = PARSE_DATE_FIELDS_MAX_DEPTH) -> ListOrDict:
     """Recursively parse date fields in a list or dictionary up to the specified depth."""
     if max_depth < 0:
         return data
 
     if isinstance(data, list):
         return [parse_date_fields(item, max_depth - 1) for item in data]
@@ -94,13 +103,13 @@
                 try:
                     parsed_value = datetime.strptime(value, '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc)
                 except ValueError:
                     pass
             elif isinstance(value, dict):
                 parsed_value = parse_date_fields(value, max_depth - 1)
             elif isinstance(value, list):
-                parsed_value = parse_date_fields(value, max_depth)
+                parsed_value = parse_date_fields(value, max_depth)  # type: ignore # mypy doesn't work with decorators and recursive calls well
             return parsed_value
 
         return {key: parse(key, value) for (key, value) in data.items()}
 
     return data
```

### Comparing `apify_shared-1.0.0b3/src/apify_shared.egg-info/PKG-INFO` & `apify_shared-1.0.1b1/src/apify_shared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-shared
-Version: 1.0.0b3
+Version: 1.0.1b1
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.0b3/src/apify_shared.egg-info/requires.txt` & `apify_shared-1.0.1b1/src/apify_shared.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 flake8-encodings~=0.5.0
 flake8-isort~=6.0.0
 flake8-noqa~=1.3.1
 flake8-pytest-style~=1.7.2
 flake8-quotes~=3.3.2
 flake8-unused-arguments~=0.0.13
 isort~=5.12.0
-mypy~=1.3.0
+mypy~=1.4.0
 pep8-naming~=0.13.3
 pre-commit~=3.3.2
 pytest~=7.3.1
 pytest-asyncio~=0.21.0
 pytest-only~=2.0.0
 pytest-randomly~=3.12.0
 pytest-timeout~=2.1.0
```

