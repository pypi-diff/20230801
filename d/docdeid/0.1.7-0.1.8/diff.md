# Comparing `tmp/docdeid-0.1.7.tar.gz` & `tmp/docdeid-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docdeid-0.1.7.tar", max compression
+gzip compressed data, was "docdeid-0.1.8.tar", max compression
```

## Comparing `docdeid-0.1.7.tar` & `docdeid-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1033 2023-07-26 09:11:40.718201 docdeid-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     3972 2023-07-26 09:11:40.718201 docdeid-0.1.7/README.md
--rw-r--r--   0        0        0      291 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/__init__.py
--rw-r--r--   0        0        0     4203 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/annotation.py
--rw-r--r--   0        0        0     2289 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/deidentifier.py
--rw-r--r--   0        0        0     4677 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/document.py
--rw-r--r--   0        0        0      103 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/ds/__init__.py
--rw-r--r--   0        0        0      243 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/ds/ds.py
--rw-r--r--   0        0        0     9440 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/ds/lookup.py
--rw-r--r--   0        0        0     2028 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/pattern.py
--rw-r--r--   0        0        0      372 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/__init__.py
--rw-r--r--   0        0        0     7970 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/annotation_set.py
--rw-r--r--   0        0        0     7824 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/annotator.py
--rw-r--r--   0        0        0     4079 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/doc.py
--rw-r--r--   0        0        0     5366 2023-07-26 09:11:40.718201 docdeid-0.1.7/docdeid/process/redactor.py
--rw-r--r--   0        0        0        0 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/py.typed
--rw-r--r--   0        0        0      247 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/str/__init__.py
--rw-r--r--   0        0        0     3930 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/str/processor.py
--rw-r--r--   0        0        0    10273 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/tokenize.py
--rw-r--r--   0        0        0      879 2023-07-26 09:11:40.722201 docdeid-0.1.7/docdeid/utils.py
--rw-r--r--   0        0        0     1464 2023-07-26 09:11:40.722201 docdeid-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 docdeid-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1033 2023-08-01 13:30:20.826626 docdeid-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     3972 2023-08-01 13:30:20.826626 docdeid-0.1.8/README.md
+-rw-r--r--   0        0        0      291 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/__init__.py
+-rw-r--r--   0        0        0     4368 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/annotation.py
+-rw-r--r--   0        0        0     2289 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/deidentifier.py
+-rw-r--r--   0        0        0     4677 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/document.py
+-rw-r--r--   0        0        0      103 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/ds/__init__.py
+-rw-r--r--   0        0        0      243 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/ds/ds.py
+-rw-r--r--   0        0        0     9440 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/ds/lookup.py
+-rw-r--r--   0        0        0     2028 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/pattern.py
+-rw-r--r--   0        0        0      372 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/process/__init__.py
+-rw-r--r--   0        0        0     7970 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/process/annotation_set.py
+-rw-r--r--   0        0        0     8014 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/process/annotator.py
+-rw-r--r--   0        0        0     4079 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/process/doc.py
+-rw-r--r--   0        0        0     5366 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/process/redactor.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/py.typed
+-rw-r--r--   0        0        0      247 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/str/__init__.py
+-rw-r--r--   0        0        0     3930 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/str/processor.py
+-rw-r--r--   0        0        0    10273 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/tokenize.py
+-rw-r--r--   0        0        0      879 2023-08-01 13:30:20.826626 docdeid-0.1.8/docdeid/utils.py
+-rw-r--r--   0        0        0     1464 2023-08-01 13:30:20.830626 docdeid-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 docdeid-0.1.8/PKG-INFO
```

### Comparing `docdeid-0.1.7/LICENSE.md` & `docdeid-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/README.md` & `docdeid-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/annotation.py` & `docdeid-0.1.8/docdeid/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
     end_char: int
     """The end character."""
 
     tag: str
     """The tag (e.g. name, location)."""
 
+    priority: Optional[int] = field(default=0, repr=True, compare=False)
+    """An additional priority attribute, that can be used for resolving overlap/merges."""
+
     start_token: Optional[Token] = field(default=None, repr=False, compare=False)
     """
     Optionally, the first :class:`.Token` in the sequence of tokens corresponding to this annotation.
 
     Should only be used when the annotation starts on a token boundary.
     """
```

### Comparing `docdeid-0.1.7/docdeid/deidentifier.py` & `docdeid-0.1.8/docdeid/deidentifier.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/document.py` & `docdeid-0.1.8/docdeid/document.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/ds/lookup.py` & `docdeid-0.1.8/docdeid/ds/lookup.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/pattern.py` & `docdeid-0.1.8/docdeid/pattern.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/process/annotation_set.py` & `docdeid-0.1.8/docdeid/process/annotation_set.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/process/annotator.py` & `docdeid-0.1.8/docdeid/process/annotator.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     Abstract class for annotators, which are responsible for generating annotations from a given document. Instatiations
     should implement the annotate method.
 
     Args:
         tag: The tag to use in the annotations.
     """
 
-    def __init__(self, tag: str) -> None:
+    def __init__(self, tag: str, priority: Optional[int] = 0) -> None:
         self.tag = tag
+        self.priority = priority
 
     def process(self, doc: Document, **kwargs) -> None:
         """
         Process a document, by adding annotations to its :class:`.AnnotationSet`.
 
         Args:
             doc: The document to be processed.
@@ -84,14 +85,15 @@
 
         return [
             Annotation(
                 text=token.text,
                 start_char=token.start_char,
                 end_char=token.end_char,
                 tag=self.tag,
+                priority=self.priority,
                 start_token=token,
                 end_token=token,
             )
             for token in tokens
         ]
 
     def annotate(self, doc: Document) -> list[Annotation]:
@@ -153,14 +155,15 @@
 
             annotations.append(
                 Annotation(
                     text=doc.text[start_char:end_char],
                     start_char=start_char,
                     end_char=end_char,
                     tag=self.tag,
+                    priority=self.priority,
                 )
             )
 
             if not self.overlapping:
                 i += len(longest_matching_prefix)  # skip ahead
 
         return annotations
@@ -228,13 +231,14 @@
 
             annotations.append(
                 Annotation(
                     text=doc.text[start_token.start_char : end_token.end_char],
                     start_char=start_token.start_char,
                     end_char=end_token.end_char,
                     tag=self.pattern.tag,
+                    priority=self.priority,
                     start_token=start_token,
                     end_token=end_token,
                 )
             )
 
         return annotations
```

### Comparing `docdeid-0.1.7/docdeid/process/doc.py` & `docdeid-0.1.8/docdeid/process/doc.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/process/redactor.py` & `docdeid-0.1.8/docdeid/process/redactor.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/str/processor.py` & `docdeid-0.1.8/docdeid/str/processor.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/tokenize.py` & `docdeid-0.1.8/docdeid/tokenize.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/docdeid/utils.py` & `docdeid-0.1.8/docdeid/utils.py`

 * *Files identical despite different names*

### Comparing `docdeid-0.1.7/pyproject.toml` & `docdeid-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docdeid"
-version = "0.1.7"
+version = "0.1.8"
 description = "Create your own document de-identifier using docdeid, a simple framework independent of language or domain."
 license = "MIT"
 authors = [
     "Vincent Menger <vmenger@protonmail.com>"
     ]
 readme = "README.md"
 keywords = ["python", "document de-identification", "de-identification", "document de-identifier", "de-identifier"]
```

### Comparing `docdeid-0.1.7/PKG-INFO` & `docdeid-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docdeid
-Version: 0.1.7
+Version: 0.1.8
 Summary: Create your own document de-identifier using docdeid, a simple framework independent of language or domain.
 License: MIT
 Keywords: python,document de-identification,de-identification,document de-identifier,de-identifier
 Author: Vincent Menger
 Author-email: vmenger@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

