# Comparing `tmp/python-hole-0.0.7.tar.gz` & `tmp/python-hole-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hole-0.0.7.tar", last modified: Tue Aug  1 12:37:09 2023, max compression
+gzip compressed data, was "python-hole-0.0.8.tar", last modified: Tue Aug  1 13:52:53 2023, max compression
```

## Comparing `python-hole-0.0.7.tar` & `python-hole-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.781131 python-hole-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 12:37:05.000000 python-hole-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-01 12:37:09.781131 python-hole-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-01 12:37:05.000000 python-hole-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:37:09.781131 python-hole-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-01 12:37:05.000000 python-hole-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/pyhole/
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/AstWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/HoleAST.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/Matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PatternMatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PyHoleErrorListener.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PyHoleParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    40290 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/PyHoleVisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/pyhole/antlr/
--rw-r--r--   0 runner    (1001) docker     (123)    52568 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27385 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Listener.py
--rw-r--r--   0 runner    (1001) docker     (123)   339487 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/Python3Visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/antlr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.777131 python-hole-0.0.7/src/pyhole/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/visualizer/Visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:05.000000 python-hole-0.0.7/src/pyhole/visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:37:09.781131 python-hole-0.0.7/src/python_hole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:37:09.000000 python-hole-0.0.7/src/python_hole.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:53.600147 python-hole-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 13:52:44.000000 python-hole-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-01 13:52:53.600147 python-hole-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-01 13:52:44.000000 python-hole-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:52:53.600147 python-hole-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-01 13:52:44.000000 python-hole-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:53.596147 python-hole-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:53.596147 python-hole-0.0.8/src/pyhole/
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/AstWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/HoleAST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/Matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/PatternMatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/PyHoleErrorListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/PyHoleParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40275 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/PyHoleVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:53.600147 python-hole-0.0.8/src/pyhole/antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)    52568 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/antlr/Python3Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27385 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/antlr/Python3Listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   339858 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/antlr/Python3Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/antlr/Python3Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/antlr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:53.600147 python-hole-0.0.8/src/pyhole/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/visualizer/Visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:44.000000 python-hole-0.0.8/src/pyhole/visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:52:53.600147 python-hole-0.0.8/src/python_hole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-01 13:52:53.000000 python-hole-0.0.8/src/python_hole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-01 13:52:53.000000 python-hole-0.0.8/src/python_hole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:52:53.000000 python-hole-0.0.8/src/python_hole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 13:52:53.000000 python-hole-0.0.8/src/python_hole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 13:52:53.000000 python-hole-0.0.8/src/python_hole.egg-info/top_level.txt
```

### Comparing `python-hole-0.0.7/LICENSE` & `python-hole-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/PKG-INFO` & `python-hole-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hole
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package to build code patterns
 Home-page: https://github.com/JulienLie/python-hole
 Author: Julien Lienard
 Author-email: julien.lienard@uclouvain.be
 License: MIT
 Description: # Python Hole
```

### Comparing `python-hole-0.0.7/README.md` & `python-hole-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/setup.py` & `python-hole-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='python-hole',
-    version='0.0.7',
+    version='0.0.8',
     packages=['pyhole', 'pyhole.antlr', 'pyhole.visualizer'],
     package_dir={'': 'src'},
     url='https://github.com/JulienLie/python-hole',
     license='MIT',
     author='Julien Lienard',
     author_email='julien.lienard@uclouvain.be',
     description="Python package to build code patterns",
```

### Comparing `python-hole-0.0.7/src/pyhole/AstWalker.py` & `python-hole-0.0.8/src/pyhole/AstWalker.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/HoleAST.py` & `python-hole-0.0.8/src/pyhole/HoleAST.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,15 @@
             next_code_node = matcher.code_walker.next_parent()
 
             if next_pattern_node is None:
                 if next_code_node is None or not matcher.strict:
                     if lineno and lineno not in matcher.pattern_match.pattern_match:
                         matcher.pattern_match.add_pattern_match(lineno, self)
                     return True
-                else:
-                    return False
+                return False
             else:
                 if lineno and lineno not in matcher.pattern_match.pattern_match and next_code_node is not None:
                     matcher.pattern_match.add_pattern_match(lineno, self)
                     end_lineno = next_code_node.lineno - 1
                     if lineno != end_lineno:
                         matcher.pattern_match.add_line_skip_match(lineno, end_lineno)
                 return matcher.rec_match(next_pattern_node, next_code_node)
@@ -264,8 +263,8 @@
     Yield a tuple of ``(fieldname, value)`` for each field in ``node._fields``
     that is present on *node*.
     """
     for field in node._fields:
         try:
             yield field, getattr(node, field)
         except AttributeError:
-            print(f"No such attribute: {field} in {node} with attributes: {node.__dict__}")
+            print(f"No such attribute: {field} in {node} with attributes: {node.__dict__}")
```

### Comparing `python-hole-0.0.7/src/pyhole/Matcher.py` & `python-hole-0.0.8/src/pyhole/Matcher.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/PatternMatch.py` & `python-hole-0.0.8/src/pyhole/PatternMatch.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/PyHoleErrorListener.py` & `python-hole-0.0.8/src/pyhole/PyHoleErrorListener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/PyHoleParser.py` & `python-hole-0.0.8/src/pyhole/PyHoleParser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/PyHoleVisitor.py` & `python-hole-0.0.8/src/pyhole/PyHoleVisitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,18 +47,19 @@
     '^=': BitXor,
     '<<=': LShift,
     '>>=': RShift,
     '**=': Pow,
     '//=': FloorDiv
 }
 
+
 def set_lineno(obj, ctx):
     start = ctx.start.line
     end = ctx.stop.line
-    if isinstance(obj, stmt) or isinstance(obj, HoleAST):
+    if isinstance(obj, (stmt, HoleAST)):
         obj.lineno = start
         obj.lineno_end = end
 
 
 # This class defines a complete generic visitor for a parse tree produced by Python3Parser.
 
 class PyHoleVisitor(Python3Visitor):
@@ -78,15 +79,15 @@
         else:
             return [aggregate, next_result]
 
     def visitChildren(self, ctx):
         children = super().visitChildren(ctx)
         if not isinstance(children, list):
             set_lineno(children, ctx)
-        #print(type(ctx).__name__ + " " + str(children))
+        # print(type(ctx).__name__ + " " + str(children))
         return children
 
     # Visit a parse tree produced by Python3Parser#single_input.
     def visitSingle_input(self, ctx: Python3Parser.Single_inputContext):
         return self.visitChildren(ctx)
 
     # Visit a parse tree produced by Python3Parser#file_input.
```

### Comparing `python-hole-0.0.7/src/pyhole/antlr/Python3Lexer.py` & `python-hole-0.0.8/src/pyhole/antlr/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/antlr/Python3Listener.py` & `python-hole-0.0.8/src/pyhole/antlr/Python3Listener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/antlr/Python3Parser.py` & `python-hole-0.0.8/src/pyhole/antlr/Python3Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,107 +74,107 @@
         buf.write(",\3,\3,\5,\u02a4\n,\3-\3-\3-\3-\3-\3-\3-\3-\3-\5-\u02af")
         buf.write("\n-\3.\3.\3.\3.\3.\3.\3.\6.\u02b8\n.\r.\16.\u02b9\3.\3")
         buf.write(".\3.\5.\u02bf\n.\3.\3.\3.\5.\u02c4\n.\3.\3.\3.\5.\u02c9")
         buf.write("\n.\3/\3/\3/\3/\7/\u02cf\n/\f/\16/\u02d2\13/\3/\3/\3/")
         buf.write("\3\60\3\60\3\60\5\60\u02da\n\60\3\61\3\61\3\61\3\61\5")
         buf.write("\61\u02e0\n\61\5\61\u02e2\n\61\3\62\3\62\3\62\3\62\6\62")
         buf.write("\u02e8\n\62\r\62\16\62\u02e9\3\62\3\62\5\62\u02ee\n\62")
-        buf.write("\3\63\3\63\3\63\3\63\3\63\3\63\5\63\u02f6\n\63\3\63\3")
-        buf.write("\63\5\63\u02fa\n\63\3\64\3\64\5\64\u02fe\n\64\3\65\3\65")
-        buf.write("\5\65\u0302\n\65\3\65\3\65\3\65\3\66\3\66\5\66\u0309\n")
-        buf.write("\66\3\66\3\66\3\66\3\67\3\67\3\67\7\67\u0311\n\67\f\67")
-        buf.write("\16\67\u0314\13\67\38\38\38\78\u0319\n8\f8\168\u031c\13")
-        buf.write("8\39\39\39\59\u0321\n9\3:\3:\3:\3:\7:\u0327\n:\f:\16:")
-        buf.write("\u032a\13:\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\5;\u0339")
-        buf.write("\n;\3<\3<\3<\3=\3=\3=\7=\u0341\n=\f=\16=\u0344\13=\3>")
-        buf.write("\3>\3>\7>\u0349\n>\f>\16>\u034c\13>\3?\3?\3?\7?\u0351")
-        buf.write("\n?\f?\16?\u0354\13?\3@\3@\3@\7@\u0359\n@\f@\16@\u035c")
-        buf.write("\13@\3A\3A\3A\7A\u0361\nA\fA\16A\u0364\13A\3B\3B\3B\7")
-        buf.write("B\u0369\nB\fB\16B\u036c\13B\3C\3C\3C\5C\u0371\nC\3D\3")
-        buf.write("D\3D\5D\u0376\nD\3E\5E\u0379\nE\3E\3E\7E\u037d\nE\fE\16")
-        buf.write("E\u0380\13E\3F\3F\3F\5F\u0385\nF\3F\3F\3F\5F\u038a\nF")
-        buf.write("\3F\3F\3F\5F\u038f\nF\3F\3F\3F\3F\3F\6F\u0396\nF\rF\16")
-        buf.write("F\u0397\3F\3F\3F\3F\5F\u039e\nF\3G\3G\5G\u03a2\nG\3G\3")
-        buf.write("G\3G\3G\5G\u03a8\nG\7G\u03aa\nG\fG\16G\u03ad\13G\3G\5")
-        buf.write("G\u03b0\nG\5G\u03b2\nG\3H\3H\5H\u03b6\nH\3H\3H\3H\3H\3")
-        buf.write("H\3H\3H\5H\u03bf\nH\3I\3I\3I\7I\u03c4\nI\fI\16I\u03c7")
-        buf.write("\13I\3I\5I\u03ca\nI\3J\3J\5J\u03ce\nJ\3J\3J\5J\u03d2\n")
-        buf.write("J\3J\5J\u03d5\nJ\5J\u03d7\nJ\3K\3K\5K\u03db\nK\3L\3L\5")
-        buf.write("L\u03df\nL\3L\3L\3L\5L\u03e4\nL\7L\u03e6\nL\fL\16L\u03e9")
-        buf.write("\13L\3L\5L\u03ec\nL\3M\3M\3M\7M\u03f1\nM\fM\16M\u03f4")
-        buf.write("\13M\3M\5M\u03f7\nM\3N\3N\3N\3N\3N\3N\5N\u03ff\nN\3N\3")
-        buf.write("N\3N\3N\3N\3N\3N\3N\5N\u0409\nN\7N\u040b\nN\fN\16N\u040e")
-        buf.write("\13N\3N\5N\u0411\nN\5N\u0413\nN\3N\3N\5N\u0417\nN\3N\3")
-        buf.write("N\3N\3N\5N\u041d\nN\7N\u041f\nN\fN\16N\u0422\13N\3N\5")
-        buf.write("N\u0425\nN\5N\u0427\nN\5N\u0429\nN\3O\3O\3O\3O\5O\u042f")
-        buf.write("\nO\3O\5O\u0432\nO\3O\3O\3O\3P\3P\3P\7P\u043a\nP\fP\16")
-        buf.write("P\u043d\13P\3P\5P\u0440\nP\3Q\3Q\5Q\u0444\nQ\3Q\3Q\3Q")
-        buf.write("\3Q\3Q\3Q\3Q\3Q\5Q\u044e\nQ\3R\3R\5R\u0452\nR\3S\5S\u0455")
-        buf.write("\nS\3S\3S\3S\3S\3S\5S\u045c\nS\3T\3T\3T\5T\u0461\nT\3")
-        buf.write("U\3U\3V\3V\5V\u0467\nV\3W\3W\3W\5W\u046c\nW\3X\3X\5X\u0470")
-        buf.write("\nX\3Y\3Y\3Z\3Z\3[\3[\3[\3\\\3\\\3\\\5\\\u047c\n\\\3]")
-        buf.write("\3]\3]\3]\3^\3^\3^\3^\3_\3_\3_\3_\6_\u048a\n_\r_\16_\u048b")
-        buf.write("\5_\u048e\n_\3_\3_\3_\3_\2\2`\2\4\6\b\n\f\16\20\22\24")
-        buf.write("\26\30\32\34\36 \"$&(*,.\60\62\64\668:<>@BDFHJLNPRTVX")
-        buf.write("Z\\^`bdfhjlnprtvxz|~\u0080\u0082\u0084\u0086\u0088\u008a")
-        buf.write("\u008c\u008e\u0090\u0092\u0094\u0096\u0098\u009a\u009c")
-        buf.write("\u009e\u00a0\u00a2\u00a4\u00a6\u00a8\u00aa\u00ac\u00ae")
-        buf.write("\u00b0\u00b2\u00b4\u00b6\u00b8\u00ba\u00bc\2\b\3\2Xd\3")
-        buf.write("\2\66\67\3\2EF\3\2GH\5\288IKVV\4\2GHLL\2\u0514\2\u00c3")
-        buf.write("\3\2\2\2\4\u00c9\3\2\2\2\6\u00ce\3\2\2\2\b\u00d7\3\2\2")
-        buf.write("\2\n\u00e3\3\2\2\2\f\u00e7\3\2\2\2\16\u00ed\3\2\2\2\20")
-        buf.write("\u00f0\3\2\2\2\22\u00fd\3\2\2\2\24\u0154\3\2\2\2\26\u015c")
-        buf.write("\3\2\2\2\30\u01af\3\2\2\2\32\u01b3\3\2\2\2\34\u01b7\3")
-        buf.write("\2\2\2\36\u01b9\3\2\2\2 \u01cf\3\2\2\2\"\u01d1\3\2\2\2")
-        buf.write("$\u01e4\3\2\2\2&\u01ec\3\2\2\2(\u01fb\3\2\2\2*\u01fd\3")
-        buf.write("\2\2\2,\u0200\3\2\2\2.\u0207\3\2\2\2\60\u0209\3\2\2\2")
-        buf.write("\62\u020b\3\2\2\2\64\u020d\3\2\2\2\66\u0211\3\2\2\28\u0213")
-        buf.write("\3\2\2\2:\u021d\3\2\2\2<\u021f\3\2\2\2>\u0222\3\2\2\2")
-        buf.write("@\u023a\3\2\2\2B\u023f\3\2\2\2D\u0244\3\2\2\2F\u024f\3")
-        buf.write("\2\2\2H\u0257\3\2\2\2J\u025f\3\2\2\2L\u0268\3\2\2\2N\u0271")
-        buf.write("\3\2\2\2P\u0281\3\2\2\2R\u0283\3\2\2\2T\u0289\3\2\2\2")
-        buf.write("V\u029c\3\2\2\2X\u02a5\3\2\2\2Z\u02b0\3\2\2\2\\\u02ca")
-        buf.write("\3\2\2\2^\u02d6\3\2\2\2`\u02db\3\2\2\2b\u02ed\3\2\2\2")
-        buf.write("d\u02f9\3\2\2\2f\u02fd\3\2\2\2h\u02ff\3\2\2\2j\u0306\3")
-        buf.write("\2\2\2l\u030d\3\2\2\2n\u0315\3\2\2\2p\u0320\3\2\2\2r\u0322")
-        buf.write("\3\2\2\2t\u0338\3\2\2\2v\u033a\3\2\2\2x\u033d\3\2\2\2")
-        buf.write("z\u0345\3\2\2\2|\u034d\3\2\2\2~\u0355\3\2\2\2\u0080\u035d")
-        buf.write("\3\2\2\2\u0082\u0365\3\2\2\2\u0084\u0370\3\2\2\2\u0086")
-        buf.write("\u0372\3\2\2\2\u0088\u0378\3\2\2\2\u008a\u039d\3\2\2\2")
-        buf.write("\u008c\u03a1\3\2\2\2\u008e\u03be\3\2\2\2\u0090\u03c0\3")
-        buf.write("\2\2\2\u0092\u03d6\3\2\2\2\u0094\u03d8\3\2\2\2\u0096\u03de")
-        buf.write("\3\2\2\2\u0098\u03ed\3\2\2\2\u009a\u0428\3\2\2\2\u009c")
-        buf.write("\u042a\3\2\2\2\u009e\u0436\3\2\2\2\u00a0\u044d\3\2\2\2")
-        buf.write("\u00a2\u0451\3\2\2\2\u00a4\u0454\3\2\2\2\u00a6\u045d\3")
-        buf.write("\2\2\2\u00a8\u0462\3\2\2\2\u00aa\u0464\3\2\2\2\u00ac\u046b")
-        buf.write("\3\2\2\2\u00ae\u046f\3\2\2\2\u00b0\u0471\3\2\2\2\u00b2")
-        buf.write("\u0473\3\2\2\2\u00b4\u0475\3\2\2\2\u00b6\u047b\3\2\2\2")
-        buf.write("\u00b8\u047d\3\2\2\2\u00ba\u0481\3\2\2\2\u00bc\u0485\3")
-        buf.write("\2\2\2\u00be\u00c4\7,\2\2\u00bf\u00c4\5\36\20\2\u00c0")
-        buf.write("\u00c1\5P)\2\u00c1\u00c2\7,\2\2\u00c2\u00c4\3\2\2\2\u00c3")
-        buf.write("\u00be\3\2\2\2\u00c3\u00bf\3\2\2\2\u00c3\u00c0\3\2\2\2")
-        buf.write("\u00c4\3\3\2\2\2\u00c5\u00c8\7,\2\2\u00c6\u00c8\5\34\17")
-        buf.write("\2\u00c7\u00c5\3\2\2\2\u00c7\u00c6\3\2\2\2\u00c8\u00cb")
-        buf.write("\3\2\2\2\u00c9\u00c7\3\2\2\2\u00c9\u00ca\3\2\2\2\u00ca")
-        buf.write("\u00cc\3\2\2\2\u00cb\u00c9\3\2\2\2\u00cc\u00cd\7\2\2\3")
-        buf.write("\u00cd\5\3\2\2\2\u00ce\u00d2\5\u0098M\2\u00cf\u00d1\7")
-        buf.write(",\2\2\u00d0\u00cf\3\2\2\2\u00d1\u00d4\3\2\2\2\u00d2\u00d0")
-        buf.write("\3\2\2\2\u00d2\u00d3\3\2\2\2\u00d3\u00d5\3\2\2\2\u00d4")
-        buf.write("\u00d2\3\2\2\2\u00d5\u00d6\7\2\2\3\u00d6\7\3\2\2\2\u00d7")
-        buf.write("\u00d8\7V\2\2\u00d8\u00de\5H%\2\u00d9\u00db\79\2\2\u00da")
-        buf.write("\u00dc\5\u009eP\2\u00db\u00da\3\2\2\2\u00db\u00dc\3\2")
-        buf.write("\2\2\u00dc\u00dd\3\2\2\2\u00dd\u00df\7:\2\2\u00de\u00d9")
-        buf.write("\3\2\2\2\u00de\u00df\3\2\2\2\u00df\u00e0\3\2\2\2\u00e0")
-        buf.write("\u00e1\7,\2\2\u00e1\t\3\2\2\2\u00e2\u00e4\5\b\5\2\u00e3")
-        buf.write("\u00e2\3\2\2\2\u00e4\u00e5\3\2\2\2\u00e5\u00e3\3\2\2\2")
-        buf.write("\u00e5\u00e6\3\2\2\2\u00e6\13\3\2\2\2\u00e7\u00eb\5\n")
-        buf.write("\6\2\u00e8\u00ec\5\u009cO\2\u00e9\u00ec\5\20\t\2\u00ea")
-        buf.write("\u00ec\5\16\b\2\u00eb\u00e8\3\2\2\2\u00eb\u00e9\3\2\2")
-        buf.write("\2\u00eb\u00ea\3\2\2\2\u00ec\r\3\2\2\2\u00ed\u00ee\7*")
-        buf.write("\2\2\u00ee\u00ef\5\20\t\2\u00ef\17\3\2\2\2\u00f0\u00f3")
+        buf.write("\3\63\3\63\3\63\3\63\3\63\3\63\5\63\u02f6\n\63\3\63\5")
+        buf.write("\63\u02f9\n\63\3\64\3\64\5\64\u02fd\n\64\3\65\3\65\5\65")
+        buf.write("\u0301\n\65\3\65\3\65\3\65\3\66\3\66\5\66\u0308\n\66\3")
+        buf.write("\66\3\66\3\66\3\67\3\67\3\67\7\67\u0310\n\67\f\67\16\67")
+        buf.write("\u0313\13\67\38\38\38\78\u0318\n8\f8\168\u031b\138\39")
+        buf.write("\39\39\59\u0320\n9\3:\3:\3:\3:\7:\u0326\n:\f:\16:\u0329")
+        buf.write("\13:\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\3;\5;\u0338\n")
+        buf.write(";\3<\3<\3<\3=\3=\3=\7=\u0340\n=\f=\16=\u0343\13=\3>\3")
+        buf.write(">\3>\7>\u0348\n>\f>\16>\u034b\13>\3?\3?\3?\7?\u0350\n")
+        buf.write("?\f?\16?\u0353\13?\3@\3@\3@\7@\u0358\n@\f@\16@\u035b\13")
+        buf.write("@\3A\3A\3A\7A\u0360\nA\fA\16A\u0363\13A\3B\3B\3B\7B\u0368")
+        buf.write("\nB\fB\16B\u036b\13B\3C\3C\3C\5C\u0370\nC\3D\3D\3D\5D")
+        buf.write("\u0375\nD\3E\5E\u0378\nE\3E\3E\7E\u037c\nE\fE\16E\u037f")
+        buf.write("\13E\3F\3F\3F\5F\u0384\nF\3F\3F\3F\5F\u0389\nF\3F\3F\3")
+        buf.write("F\5F\u038e\nF\3F\3F\3F\3F\3F\6F\u0395\nF\rF\16F\u0396")
+        buf.write("\3F\3F\3F\3F\5F\u039d\nF\3G\3G\5G\u03a1\nG\3G\3G\3G\3")
+        buf.write("G\5G\u03a7\nG\7G\u03a9\nG\fG\16G\u03ac\13G\3G\5G\u03af")
+        buf.write("\nG\5G\u03b1\nG\3H\3H\5H\u03b5\nH\3H\3H\3H\3H\3H\3H\3")
+        buf.write("H\5H\u03be\nH\3I\3I\3I\7I\u03c3\nI\fI\16I\u03c6\13I\3")
+        buf.write("I\5I\u03c9\nI\3J\3J\5J\u03cd\nJ\3J\3J\5J\u03d1\nJ\3J\5")
+        buf.write("J\u03d4\nJ\5J\u03d6\nJ\3K\3K\5K\u03da\nK\3L\3L\5L\u03de")
+        buf.write("\nL\3L\3L\3L\5L\u03e3\nL\7L\u03e5\nL\fL\16L\u03e8\13L")
+        buf.write("\3L\5L\u03eb\nL\3M\3M\3M\7M\u03f0\nM\fM\16M\u03f3\13M")
+        buf.write("\3M\5M\u03f6\nM\3N\3N\3N\3N\3N\3N\5N\u03fe\nN\3N\3N\3")
+        buf.write("N\3N\3N\3N\3N\3N\5N\u0408\nN\7N\u040a\nN\fN\16N\u040d")
+        buf.write("\13N\3N\5N\u0410\nN\5N\u0412\nN\3N\3N\5N\u0416\nN\3N\3")
+        buf.write("N\3N\3N\5N\u041c\nN\7N\u041e\nN\fN\16N\u0421\13N\3N\5")
+        buf.write("N\u0424\nN\5N\u0426\nN\5N\u0428\nN\3O\3O\3O\3O\5O\u042e")
+        buf.write("\nO\3O\5O\u0431\nO\3O\3O\3O\3P\3P\3P\7P\u0439\nP\fP\16")
+        buf.write("P\u043c\13P\3P\5P\u043f\nP\3Q\3Q\5Q\u0443\nQ\3Q\3Q\3Q")
+        buf.write("\3Q\3Q\3Q\3Q\3Q\5Q\u044d\nQ\3R\3R\5R\u0451\nR\3S\5S\u0454")
+        buf.write("\nS\3S\3S\3S\3S\3S\5S\u045b\nS\3T\3T\3T\5T\u0460\nT\3")
+        buf.write("U\3U\3V\3V\5V\u0466\nV\3W\3W\3W\5W\u046b\nW\3X\3X\3X\5")
+        buf.write("X\u0470\nX\3Y\3Y\3Z\3Z\3[\3[\3[\3\\\3\\\3\\\5\\\u047c")
+        buf.write("\n\\\3]\3]\3]\3]\3^\3^\3^\3^\3_\3_\3_\3_\6_\u048a\n_\r")
+        buf.write("_\16_\u048b\5_\u048e\n_\3_\3_\3_\3_\2\2`\2\4\6\b\n\f\16")
+        buf.write("\20\22\24\26\30\32\34\36 \"$&(*,.\60\62\64\668:<>@BDF")
+        buf.write("HJLNPRTVXZ\\^`bdfhjlnprtvxz|~\u0080\u0082\u0084\u0086")
+        buf.write("\u0088\u008a\u008c\u008e\u0090\u0092\u0094\u0096\u0098")
+        buf.write("\u009a\u009c\u009e\u00a0\u00a2\u00a4\u00a6\u00a8\u00aa")
+        buf.write("\u00ac\u00ae\u00b0\u00b2\u00b4\u00b6\u00b8\u00ba\u00bc")
+        buf.write("\2\b\3\2Xd\3\2\66\67\3\2EF\3\2GH\5\288IKVV\4\2GHLL\2\u0514")
+        buf.write("\2\u00c3\3\2\2\2\4\u00c9\3\2\2\2\6\u00ce\3\2\2\2\b\u00d7")
+        buf.write("\3\2\2\2\n\u00e3\3\2\2\2\f\u00e7\3\2\2\2\16\u00ed\3\2")
+        buf.write("\2\2\20\u00f0\3\2\2\2\22\u00fd\3\2\2\2\24\u0154\3\2\2")
+        buf.write("\2\26\u015c\3\2\2\2\30\u01af\3\2\2\2\32\u01b3\3\2\2\2")
+        buf.write("\34\u01b7\3\2\2\2\36\u01b9\3\2\2\2 \u01cf\3\2\2\2\"\u01d1")
+        buf.write("\3\2\2\2$\u01e4\3\2\2\2&\u01ec\3\2\2\2(\u01fb\3\2\2\2")
+        buf.write("*\u01fd\3\2\2\2,\u0200\3\2\2\2.\u0207\3\2\2\2\60\u0209")
+        buf.write("\3\2\2\2\62\u020b\3\2\2\2\64\u020d\3\2\2\2\66\u0211\3")
+        buf.write("\2\2\28\u0213\3\2\2\2:\u021d\3\2\2\2<\u021f\3\2\2\2>\u0222")
+        buf.write("\3\2\2\2@\u023a\3\2\2\2B\u023f\3\2\2\2D\u0244\3\2\2\2")
+        buf.write("F\u024f\3\2\2\2H\u0257\3\2\2\2J\u025f\3\2\2\2L\u0268\3")
+        buf.write("\2\2\2N\u0271\3\2\2\2P\u0281\3\2\2\2R\u0283\3\2\2\2T\u0289")
+        buf.write("\3\2\2\2V\u029c\3\2\2\2X\u02a5\3\2\2\2Z\u02b0\3\2\2\2")
+        buf.write("\\\u02ca\3\2\2\2^\u02d6\3\2\2\2`\u02db\3\2\2\2b\u02ed")
+        buf.write("\3\2\2\2d\u02f8\3\2\2\2f\u02fc\3\2\2\2h\u02fe\3\2\2\2")
+        buf.write("j\u0305\3\2\2\2l\u030c\3\2\2\2n\u0314\3\2\2\2p\u031f\3")
+        buf.write("\2\2\2r\u0321\3\2\2\2t\u0337\3\2\2\2v\u0339\3\2\2\2x\u033c")
+        buf.write("\3\2\2\2z\u0344\3\2\2\2|\u034c\3\2\2\2~\u0354\3\2\2\2")
+        buf.write("\u0080\u035c\3\2\2\2\u0082\u0364\3\2\2\2\u0084\u036f\3")
+        buf.write("\2\2\2\u0086\u0371\3\2\2\2\u0088\u0377\3\2\2\2\u008a\u039c")
+        buf.write("\3\2\2\2\u008c\u03a0\3\2\2\2\u008e\u03bd\3\2\2\2\u0090")
+        buf.write("\u03bf\3\2\2\2\u0092\u03d5\3\2\2\2\u0094\u03d7\3\2\2\2")
+        buf.write("\u0096\u03dd\3\2\2\2\u0098\u03ec\3\2\2\2\u009a\u0427\3")
+        buf.write("\2\2\2\u009c\u0429\3\2\2\2\u009e\u0435\3\2\2\2\u00a0\u044c")
+        buf.write("\3\2\2\2\u00a2\u0450\3\2\2\2\u00a4\u0453\3\2\2\2\u00a6")
+        buf.write("\u045c\3\2\2\2\u00a8\u0461\3\2\2\2\u00aa\u0463\3\2\2\2")
+        buf.write("\u00ac\u046a\3\2\2\2\u00ae\u046f\3\2\2\2\u00b0\u0471\3")
+        buf.write("\2\2\2\u00b2\u0473\3\2\2\2\u00b4\u0475\3\2\2\2\u00b6\u047b")
+        buf.write("\3\2\2\2\u00b8\u047d\3\2\2\2\u00ba\u0481\3\2\2\2\u00bc")
+        buf.write("\u0485\3\2\2\2\u00be\u00c4\7,\2\2\u00bf\u00c4\5\36\20")
+        buf.write("\2\u00c0\u00c1\5P)\2\u00c1\u00c2\7,\2\2\u00c2\u00c4\3")
+        buf.write("\2\2\2\u00c3\u00be\3\2\2\2\u00c3\u00bf\3\2\2\2\u00c3\u00c0")
+        buf.write("\3\2\2\2\u00c4\3\3\2\2\2\u00c5\u00c8\7,\2\2\u00c6\u00c8")
+        buf.write("\5\34\17\2\u00c7\u00c5\3\2\2\2\u00c7\u00c6\3\2\2\2\u00c8")
+        buf.write("\u00cb\3\2\2\2\u00c9\u00c7\3\2\2\2\u00c9\u00ca\3\2\2\2")
+        buf.write("\u00ca\u00cc\3\2\2\2\u00cb\u00c9\3\2\2\2\u00cc\u00cd\7")
+        buf.write("\2\2\3\u00cd\5\3\2\2\2\u00ce\u00d2\5\u0098M\2\u00cf\u00d1")
+        buf.write("\7,\2\2\u00d0\u00cf\3\2\2\2\u00d1\u00d4\3\2\2\2\u00d2")
+        buf.write("\u00d0\3\2\2\2\u00d2\u00d3\3\2\2\2\u00d3\u00d5\3\2\2\2")
+        buf.write("\u00d4\u00d2\3\2\2\2\u00d5\u00d6\7\2\2\3\u00d6\7\3\2\2")
+        buf.write("\2\u00d7\u00d8\7V\2\2\u00d8\u00de\5H%\2\u00d9\u00db\7")
+        buf.write("9\2\2\u00da\u00dc\5\u009eP\2\u00db\u00da\3\2\2\2\u00db")
+        buf.write("\u00dc\3\2\2\2\u00dc\u00dd\3\2\2\2\u00dd\u00df\7:\2\2")
+        buf.write("\u00de\u00d9\3\2\2\2\u00de\u00df\3\2\2\2\u00df\u00e0\3")
+        buf.write("\2\2\2\u00e0\u00e1\7,\2\2\u00e1\t\3\2\2\2\u00e2\u00e4")
+        buf.write("\5\b\5\2\u00e3\u00e2\3\2\2\2\u00e4\u00e5\3\2\2\2\u00e5")
+        buf.write("\u00e3\3\2\2\2\u00e5\u00e6\3\2\2\2\u00e6\13\3\2\2\2\u00e7")
+        buf.write("\u00eb\5\n\6\2\u00e8\u00ec\5\u009cO\2\u00e9\u00ec\5\20")
+        buf.write("\t\2\u00ea\u00ec\5\16\b\2\u00eb\u00e8\3\2\2\2\u00eb\u00e9")
+        buf.write("\3\2\2\2\u00eb\u00ea\3\2\2\2\u00ec\r\3\2\2\2\u00ed\u00ee")
+        buf.write("\7*\2\2\u00ee\u00ef\5\20\t\2\u00ef\17\3\2\2\2\u00f0\u00f3")
         buf.write("\7\t\2\2\u00f1\u00f4\7-\2\2\u00f2\u00f4\5\u00b0Y\2\u00f3")
         buf.write("\u00f1\3\2\2\2\u00f3\u00f2\3\2\2\2\u00f4\u00f5\3\2\2\2")
         buf.write("\u00f5\u00f8\5\22\n\2\u00f6\u00f7\7W\2\2\u00f7\u00f9\5")
         buf.write("d\63\2\u00f8\u00f6\3\2\2\2\u00f8\u00f9\3\2\2\2\u00f9\u00fa")
         buf.write("\3\2\2\2\u00fa\u00fb\7<\2\2\u00fb\u00fc\5b\62\2\u00fc")
         buf.write("\21\3\2\2\2\u00fd\u00ff\79\2\2\u00fe\u0100\5\24\13\2\u00ff")
         buf.write("\u00fe\3\2\2\2\u00ff\u0100\3\2\2\2\u0100\u0101\3\2\2\2")
@@ -396,218 +396,219 @@
         buf.write("\u02e5\7,\2\2\u02e5\u02e7\7g\2\2\u02e6\u02e8\5\34\17\2")
         buf.write("\u02e7\u02e6\3\2\2\2\u02e8\u02e9\3\2\2\2\u02e9\u02e7\3")
         buf.write("\2\2\2\u02e9\u02ea\3\2\2\2\u02ea\u02eb\3\2\2\2\u02eb\u02ec")
         buf.write("\7h\2\2\u02ec\u02ee\3\2\2\2\u02ed\u02e3\3\2\2\2\u02ed")
         buf.write("\u02e4\3\2\2\2\u02eec\3\2\2\2\u02ef\u02f5\5l\67\2\u02f0")
         buf.write("\u02f1\7\22\2\2\u02f1\u02f2\5l\67\2\u02f2\u02f3\7\24\2")
         buf.write("\2\u02f3\u02f4\5d\63\2\u02f4\u02f6\3\2\2\2\u02f5\u02f0")
-        buf.write("\3\2\2\2\u02f5\u02f6\3\2\2\2\u02f6\u02fa\3\2\2\2\u02f7")
-        buf.write("\u02fa\5h\65\2\u02f8\u02fa\5\u00b4[\2\u02f9\u02ef\3\2")
-        buf.write("\2\2\u02f9\u02f7\3\2\2\2\u02f9\u02f8\3\2\2\2\u02fae\3")
-        buf.write("\2\2\2\u02fb\u02fe\5l\67\2\u02fc\u02fe\5j\66\2\u02fd\u02fb")
-        buf.write("\3\2\2\2\u02fd\u02fc\3\2\2\2\u02feg\3\2\2\2\u02ff\u0301")
-        buf.write("\7\34\2\2\u0300\u0302\5\30\r\2\u0301\u0300\3\2\2\2\u0301")
-        buf.write("\u0302\3\2\2\2\u0302\u0303\3\2\2\2\u0303\u0304\7<\2\2")
-        buf.write("\u0304\u0305\5d\63\2\u0305i\3\2\2\2\u0306\u0308\7\34\2")
-        buf.write("\2\u0307\u0309\5\30\r\2\u0308\u0307\3\2\2\2\u0308\u0309")
-        buf.write("\3\2\2\2\u0309\u030a\3\2\2\2\u030a\u030b\7<\2\2\u030b")
-        buf.write("\u030c\5f\64\2\u030ck\3\2\2\2\u030d\u0312\5n8\2\u030e")
-        buf.write("\u030f\7\35\2\2\u030f\u0311\5n8\2\u0310\u030e\3\2\2\2")
-        buf.write("\u0311\u0314\3\2\2\2\u0312\u0310\3\2\2\2\u0312\u0313\3")
-        buf.write("\2\2\2\u0313m\3\2\2\2\u0314\u0312\3\2\2\2\u0315\u031a")
-        buf.write("\5p9\2\u0316\u0317\7\36\2\2\u0317\u0319\5p9\2\u0318\u0316")
-        buf.write("\3\2\2\2\u0319\u031c\3\2\2\2\u031a\u0318\3\2\2\2\u031a")
-        buf.write("\u031b\3\2\2\2\u031bo\3\2\2\2\u031c\u031a\3\2\2\2\u031d")
-        buf.write("\u031e\7\37\2\2\u031e\u0321\5p9\2\u031f\u0321\5r:\2\u0320")
-        buf.write("\u031d\3\2\2\2\u0320\u031f\3\2\2\2\u0321q\3\2\2\2\u0322")
-        buf.write("\u0328\5x=\2\u0323\u0324\5t;\2\u0324\u0325\5x=\2\u0325")
-        buf.write("\u0327\3\2\2\2\u0326\u0323\3\2\2\2\u0327\u032a\3\2\2\2")
-        buf.write("\u0328\u0326\3\2\2\2\u0328\u0329\3\2\2\2\u0329s\3\2\2")
-        buf.write("\2\u032a\u0328\3\2\2\2\u032b\u0339\7O\2\2\u032c\u0339")
-        buf.write("\7P\2\2\u032d\u0339\7Q\2\2\u032e\u0339\7R\2\2\u032f\u0339")
-        buf.write("\7S\2\2\u0330\u0339\7T\2\2\u0331\u0339\7U\2\2\u0332\u0339")
-        buf.write("\7\27\2\2\u0333\u0334\7\37\2\2\u0334\u0339\7\27\2\2\u0335")
-        buf.write("\u0339\7 \2\2\u0336\u0337\7 \2\2\u0337\u0339\7\37\2\2")
-        buf.write("\u0338\u032b\3\2\2\2\u0338\u032c\3\2\2\2\u0338\u032d\3")
-        buf.write("\2\2\2\u0338\u032e\3\2\2\2\u0338\u032f\3\2\2\2\u0338\u0330")
-        buf.write("\3\2\2\2\u0338\u0331\3\2\2\2\u0338\u0332\3\2\2\2\u0338")
-        buf.write("\u0333\3\2\2\2\u0338\u0335\3\2\2\2\u0338\u0336\3\2\2\2")
-        buf.write("\u0339u\3\2\2\2\u033a\u033b\78\2\2\u033b\u033c\5x=\2\u033c")
-        buf.write("w\3\2\2\2\u033d\u0342\5z>\2\u033e\u033f\7B\2\2\u033f\u0341")
-        buf.write("\5z>\2\u0340\u033e\3\2\2\2\u0341\u0344\3\2\2\2\u0342\u0340")
-        buf.write("\3\2\2\2\u0342\u0343\3\2\2\2\u0343y\3\2\2\2\u0344\u0342")
-        buf.write("\3\2\2\2\u0345\u034a\5|?\2\u0346\u0347\7C\2\2\u0347\u0349")
-        buf.write("\5|?\2\u0348\u0346\3\2\2\2\u0349\u034c\3\2\2\2\u034a\u0348")
-        buf.write("\3\2\2\2\u034a\u034b\3\2\2\2\u034b{\3\2\2\2\u034c\u034a")
-        buf.write("\3\2\2\2\u034d\u0352\5~@\2\u034e\u034f\7D\2\2\u034f\u0351")
-        buf.write("\5~@\2\u0350\u034e\3\2\2\2\u0351\u0354\3\2\2\2\u0352\u0350")
-        buf.write("\3\2\2\2\u0352\u0353\3\2\2\2\u0353}\3\2\2\2\u0354\u0352")
-        buf.write("\3\2\2\2\u0355\u035a\5\u0080A\2\u0356\u0357\t\4\2\2\u0357")
-        buf.write("\u0359\5\u0080A\2\u0358\u0356\3\2\2\2\u0359\u035c\3\2")
-        buf.write("\2\2\u035a\u0358\3\2\2\2\u035a\u035b\3\2\2\2\u035b\177")
-        buf.write("\3\2\2\2\u035c\u035a\3\2\2\2\u035d\u0362\5\u0082B\2\u035e")
-        buf.write("\u035f\t\5\2\2\u035f\u0361\5\u0082B\2\u0360\u035e\3\2")
-        buf.write("\2\2\u0361\u0364\3\2\2\2\u0362\u0360\3\2\2\2\u0362\u0363")
-        buf.write("\3\2\2\2\u0363\u0081\3\2\2\2\u0364\u0362\3\2\2\2\u0365")
-        buf.write("\u036a\5\u0084C\2\u0366\u0367\t\6\2\2\u0367\u0369\5\u0084")
-        buf.write("C\2\u0368\u0366\3\2\2\2\u0369\u036c\3\2\2\2\u036a\u0368")
-        buf.write("\3\2\2\2\u036a\u036b\3\2\2\2\u036b\u0083\3\2\2\2\u036c")
-        buf.write("\u036a\3\2\2\2\u036d\u036e\t\7\2\2\u036e\u0371\5\u0084")
-        buf.write("C\2\u036f\u0371\5\u0086D\2\u0370\u036d\3\2\2\2\u0370\u036f")
-        buf.write("\3\2\2\2\u0371\u0085\3\2\2\2\u0372\u0375\5\u0088E\2\u0373")
-        buf.write("\u0374\7>\2\2\u0374\u0376\5\u0084C\2\u0375\u0373\3\2\2")
-        buf.write("\2\u0375\u0376\3\2\2\2\u0376\u0087\3\2\2\2\u0377\u0379")
-        buf.write("\7+\2\2\u0378\u0377\3\2\2\2\u0378\u0379\3\2\2\2\u0379")
-        buf.write("\u037a\3\2\2\2\u037a\u037e\5\u008aF\2\u037b\u037d\5\u008e")
-        buf.write("H\2\u037c\u037b\3\2\2\2\u037d\u0380\3\2\2\2\u037e\u037c")
-        buf.write("\3\2\2\2\u037e\u037f\3\2\2\2\u037f\u0089\3\2\2\2\u0380")
-        buf.write("\u037e\3\2\2\2\u0381\u0384\79\2\2\u0382\u0385\5\u00aa")
-        buf.write("V\2\u0383\u0385\5\u008cG\2\u0384\u0382\3\2\2\2\u0384\u0383")
-        buf.write("\3\2\2\2\u0384\u0385\3\2\2\2\u0385\u0386\3\2\2\2\u0386")
-        buf.write("\u039e\7:\2\2\u0387\u0389\7@\2\2\u0388\u038a\5\u008cG")
-        buf.write("\2\u0389\u0388\3\2\2\2\u0389\u038a\3\2\2\2\u038a\u038b")
-        buf.write("\3\2\2\2\u038b\u039e\7A\2\2\u038c\u038e\7M\2\2\u038d\u038f")
-        buf.write("\5\u009aN\2\u038e\u038d\3\2\2\2\u038e\u038f\3\2\2\2\u038f")
-        buf.write("\u0390\3\2\2\2\u0390\u039e\7N\2\2\u0391\u039e\5\u00ae")
-        buf.write("X\2\u0392\u039e\7-\2\2\u0393\u039e\7\7\2\2\u0394\u0396")
-        buf.write("\7\6\2\2\u0395\u0394\3\2\2\2\u0396\u0397\3\2\2\2\u0397")
-        buf.write("\u0395\3\2\2\2\u0397\u0398\3\2\2\2\u0398\u039e\3\2\2\2")
-        buf.write("\u0399\u039e\7\67\2\2\u039a\u039e\7!\2\2\u039b\u039e\7")
-        buf.write("\"\2\2\u039c\u039e\7#\2\2\u039d\u0381\3\2\2\2\u039d\u0387")
-        buf.write("\3\2\2\2\u039d\u038c\3\2\2\2\u039d\u0391\3\2\2\2\u039d")
-        buf.write("\u0392\3\2\2\2\u039d\u0393\3\2\2\2\u039d\u0395\3\2\2\2")
-        buf.write("\u039d\u0399\3\2\2\2\u039d\u039a\3\2\2\2\u039d\u039b\3")
-        buf.write("\2\2\2\u039d\u039c\3\2\2\2\u039e\u008b\3\2\2\2\u039f\u03a2")
-        buf.write("\5d\63\2\u03a0\u03a2\5v<\2\u03a1\u039f\3\2\2\2\u03a1\u03a0")
-        buf.write("\3\2\2\2\u03a2\u03b1\3\2\2\2\u03a3\u03b2\5\u00a4S\2\u03a4")
-        buf.write("\u03a7\7;\2\2\u03a5\u03a8\5d\63\2\u03a6\u03a8\5v<\2\u03a7")
-        buf.write("\u03a5\3\2\2\2\u03a7\u03a6\3\2\2\2\u03a8\u03aa\3\2\2\2")
-        buf.write("\u03a9\u03a4\3\2\2\2\u03aa\u03ad\3\2\2\2\u03ab\u03a9\3")
-        buf.write("\2\2\2\u03ab\u03ac\3\2\2\2\u03ac\u03af\3\2\2\2\u03ad\u03ab")
-        buf.write("\3\2\2\2\u03ae\u03b0\7;\2\2\u03af\u03ae\3\2\2\2\u03af")
-        buf.write("\u03b0\3\2\2\2\u03b0\u03b2\3\2\2\2\u03b1\u03a3\3\2\2\2")
-        buf.write("\u03b1\u03ab\3\2\2\2\u03b2\u008d\3\2\2\2\u03b3\u03b5\7")
-        buf.write("9\2\2\u03b4\u03b6\5\u009eP\2\u03b5\u03b4\3\2\2\2\u03b5")
-        buf.write("\u03b6\3\2\2\2\u03b6\u03b7\3\2\2\2\u03b7\u03bf\7:\2\2")
-        buf.write("\u03b8\u03b9\7@\2\2\u03b9\u03ba\5\u0090I\2\u03ba\u03bb")
-        buf.write("\7A\2\2\u03bb\u03bf\3\2\2\2\u03bc\u03bd\7\66\2\2\u03bd")
-        buf.write("\u03bf\7-\2\2\u03be\u03b3\3\2\2\2\u03be\u03b8\3\2\2\2")
-        buf.write("\u03be\u03bc\3\2\2\2\u03bf\u008f\3\2\2\2\u03c0\u03c5\5")
-        buf.write("\u0092J\2\u03c1\u03c2\7;\2\2\u03c2\u03c4\5\u0092J\2\u03c3")
-        buf.write("\u03c1\3\2\2\2\u03c4\u03c7\3\2\2\2\u03c5\u03c3\3\2\2\2")
-        buf.write("\u03c5\u03c6\3\2\2\2\u03c6\u03c9\3\2\2\2\u03c7\u03c5\3")
-        buf.write("\2\2\2\u03c8\u03ca\7;\2\2\u03c9\u03c8\3\2\2\2\u03c9\u03ca")
-        buf.write("\3\2\2\2\u03ca\u0091\3\2\2\2\u03cb\u03d7\5d\63\2\u03cc")
-        buf.write("\u03ce\5d\63\2\u03cd\u03cc\3\2\2\2\u03cd\u03ce\3\2\2\2")
-        buf.write("\u03ce\u03cf\3\2\2\2\u03cf\u03d1\7<\2\2\u03d0\u03d2\5")
-        buf.write("d\63\2\u03d1\u03d0\3\2\2\2\u03d1\u03d2\3\2\2\2\u03d2\u03d4")
-        buf.write("\3\2\2\2\u03d3\u03d5\5\u0094K\2\u03d4\u03d3\3\2\2\2\u03d4")
-        buf.write("\u03d5\3\2\2\2\u03d5\u03d7\3\2\2\2\u03d6\u03cb\3\2\2\2")
-        buf.write("\u03d6\u03cd\3\2\2\2\u03d7\u0093\3\2\2\2\u03d8\u03da\7")
-        buf.write("<\2\2\u03d9\u03db\5d\63\2\u03da\u03d9\3\2\2\2\u03da\u03db")
-        buf.write("\3\2\2\2\u03db\u0095\3\2\2\2\u03dc\u03df\5x=\2\u03dd\u03df")
-        buf.write("\5v<\2\u03de\u03dc\3\2\2\2\u03de\u03dd\3\2\2\2\u03df\u03e7")
-        buf.write("\3\2\2\2\u03e0\u03e3\7;\2\2\u03e1\u03e4\5x=\2\u03e2\u03e4")
-        buf.write("\5v<\2\u03e3\u03e1\3\2\2\2\u03e3\u03e2\3\2\2\2\u03e4\u03e6")
-        buf.write("\3\2\2\2\u03e5\u03e0\3\2\2\2\u03e6\u03e9\3\2\2\2\u03e7")
-        buf.write("\u03e5\3\2\2\2\u03e7\u03e8\3\2\2\2\u03e8\u03eb\3\2\2\2")
-        buf.write("\u03e9\u03e7\3\2\2\2\u03ea\u03ec\7;\2\2\u03eb\u03ea\3")
-        buf.write("\2\2\2\u03eb\u03ec\3\2\2\2\u03ec\u0097\3\2\2\2\u03ed\u03f2")
-        buf.write("\5d\63\2\u03ee\u03ef\7;\2\2\u03ef\u03f1\5d\63\2\u03f0")
-        buf.write("\u03ee\3\2\2\2\u03f1\u03f4\3\2\2\2\u03f2\u03f0\3\2\2\2")
-        buf.write("\u03f2\u03f3\3\2\2\2\u03f3\u03f6\3\2\2\2\u03f4\u03f2\3")
-        buf.write("\2\2\2\u03f5\u03f7\7;\2\2\u03f6\u03f5\3\2\2\2\u03f6\u03f7")
-        buf.write("\3\2\2\2\u03f7\u0099\3\2\2\2\u03f8\u03f9\5d\63\2\u03f9")
-        buf.write("\u03fa\7<\2\2\u03fa\u03fb\5d\63\2\u03fb\u03ff\3\2\2\2")
-        buf.write("\u03fc\u03fd\7>\2\2\u03fd\u03ff\5x=\2\u03fe\u03f8\3\2")
-        buf.write("\2\2\u03fe\u03fc\3\2\2\2\u03ff\u0412\3\2\2\2\u0400\u0413")
-        buf.write("\5\u00a4S\2\u0401\u0408\7;\2\2\u0402\u0403\5d\63\2\u0403")
-        buf.write("\u0404\7<\2\2\u0404\u0405\5d\63\2\u0405\u0409\3\2\2\2")
-        buf.write("\u0406\u0407\7>\2\2\u0407\u0409\5x=\2\u0408\u0402\3\2")
-        buf.write("\2\2\u0408\u0406\3\2\2\2\u0409\u040b\3\2\2\2\u040a\u0401")
-        buf.write("\3\2\2\2\u040b\u040e\3\2\2\2\u040c\u040a\3\2\2\2\u040c")
-        buf.write("\u040d\3\2\2\2\u040d\u0410\3\2\2\2\u040e\u040c\3\2\2\2")
-        buf.write("\u040f\u0411\7;\2\2\u0410\u040f\3\2\2\2\u0410\u0411\3")
-        buf.write("\2\2\2\u0411\u0413\3\2\2\2\u0412\u0400\3\2\2\2\u0412\u040c")
-        buf.write("\3\2\2\2\u0413\u0429\3\2\2\2\u0414\u0417\5d\63\2\u0415")
-        buf.write("\u0417\5v<\2\u0416\u0414\3\2\2\2\u0416\u0415\3\2\2\2\u0417")
-        buf.write("\u0426\3\2\2\2\u0418\u0427\5\u00a4S\2\u0419\u041c\7;\2")
-        buf.write("\2\u041a\u041d\5d\63\2\u041b\u041d\5v<\2\u041c\u041a\3")
-        buf.write("\2\2\2\u041c\u041b\3\2\2\2\u041d\u041f\3\2\2\2\u041e\u0419")
-        buf.write("\3\2\2\2\u041f\u0422\3\2\2\2\u0420\u041e\3\2\2\2\u0420")
-        buf.write("\u0421\3\2\2\2\u0421\u0424\3\2\2\2\u0422\u0420\3\2\2\2")
-        buf.write("\u0423\u0425\7;\2\2\u0424\u0423\3\2\2\2\u0424\u0425\3")
-        buf.write("\2\2\2\u0425\u0427\3\2\2\2\u0426\u0418\3\2\2\2\u0426\u0420")
-        buf.write("\3\2\2\2\u0427\u0429\3\2\2\2\u0428\u03fe\3\2\2\2\u0428")
-        buf.write("\u0416\3\2\2\2\u0429\u009b\3\2\2\2\u042a\u042b\7$\2\2")
-        buf.write("\u042b\u0431\7-\2\2\u042c\u042e\79\2\2\u042d\u042f\5\u009e")
-        buf.write("P\2\u042e\u042d\3\2\2\2\u042e\u042f\3\2\2\2\u042f\u0430")
-        buf.write("\3\2\2\2\u0430\u0432\7:\2\2\u0431\u042c\3\2\2\2\u0431")
-        buf.write("\u0432\3\2\2\2\u0432\u0433\3\2\2\2\u0433\u0434\7<\2\2")
-        buf.write("\u0434\u0435\5b\62\2\u0435\u009d\3\2\2\2\u0436\u043b\5")
-        buf.write("\u00a0Q\2\u0437\u0438\7;\2\2\u0438\u043a\5\u00a0Q\2\u0439")
-        buf.write("\u0437\3\2\2\2\u043a\u043d\3\2\2\2\u043b\u0439\3\2\2\2")
-        buf.write("\u043b\u043c\3\2\2\2\u043c\u043f\3\2\2\2\u043d\u043b\3")
-        buf.write("\2\2\2\u043e\u0440\7;\2\2\u043f\u043e\3\2\2\2\u043f\u0440")
-        buf.write("\3\2\2\2\u0440\u009f\3\2\2\2\u0441\u0443\5d\63\2\u0442")
-        buf.write("\u0444\5\u00a4S\2\u0443\u0442\3\2\2\2\u0443\u0444\3\2")
-        buf.write("\2\2\u0444\u044e\3\2\2\2\u0445\u0446\5d\63\2\u0446\u0447")
-        buf.write("\7?\2\2\u0447\u0448\5d\63\2\u0448\u044e\3\2\2\2\u0449")
-        buf.write("\u044a\7>\2\2\u044a\u044e\5d\63\2\u044b\u044c\78\2\2\u044c")
-        buf.write("\u044e\5d\63\2\u044d\u0441\3\2\2\2\u044d\u0445\3\2\2\2")
-        buf.write("\u044d\u0449\3\2\2\2\u044d\u044b\3\2\2\2\u044e\u00a1\3")
-        buf.write("\2\2\2\u044f\u0452\5\u00a4S\2\u0450\u0452\5\u00a6T\2\u0451")
-        buf.write("\u044f\3\2\2\2\u0451\u0450\3\2\2\2\u0452\u00a3\3\2\2\2")
-        buf.write("\u0453\u0455\7*\2\2\u0454\u0453\3\2\2\2\u0454\u0455\3")
-        buf.write("\2\2\2\u0455\u0456\3\2\2\2\u0456\u0457\7\26\2\2\u0457")
-        buf.write("\u0458\5\u0096L\2\u0458\u0459\7\27\2\2\u0459\u045b\5l")
-        buf.write("\67\2\u045a\u045c\5\u00a2R\2\u045b\u045a\3\2\2\2\u045b")
-        buf.write("\u045c\3\2\2\2\u045c\u00a5\3\2\2\2\u045d\u045e\7\22\2")
-        buf.write("\2\u045e\u0460\5f\64\2\u045f\u0461\5\u00a2R\2\u0460\u045f")
-        buf.write("\3\2\2\2\u0460\u0461\3\2\2\2\u0461\u00a7\3\2\2\2\u0462")
-        buf.write("\u0463\7-\2\2\u0463\u00a9\3\2\2\2\u0464\u0466\7%\2\2\u0465")
-        buf.write("\u0467\5\u00acW\2\u0466\u0465\3\2\2\2\u0466\u0467\3\2")
-        buf.write("\2\2\u0467\u00ab\3\2\2\2\u0468\u0469\7\f\2\2\u0469\u046c")
-        buf.write("\5d\63\2\u046a\u046c\5\u0098M\2\u046b\u0468\3\2\2\2\u046b")
-        buf.write("\u046a\3\2\2\2\u046c\u00ad\3\2\2\2\u046d\u0470\5\u00b0")
-        buf.write("Y\2\u046e\u0470\5\u00b2Z\2\u046f\u046d\3\2\2\2\u046f\u046e")
-        buf.write("\3\2\2\2\u0470\u00af\3\2\2\2\u0471\u0472\7\3\2\2\u0472")
-        buf.write("\u00b1\3\2\2\2\u0473\u0474\7\4\2\2\u0474\u00b3\3\2\2\2")
-        buf.write("\u0475\u0476\7\3\2\2\u0476\u0477\7-\2\2\u0477\u00b5\3")
-        buf.write("\2\2\2\u0478\u047c\5\u00b8]\2\u0479\u047c\5\u00ba^\2\u047a")
-        buf.write("\u047c\5\u00bc_\2\u047b\u0478\3\2\2\2\u047b\u0479\3\2")
-        buf.write("\2\2\u047b\u047a\3\2\2\2\u047c\u00b7\3\2\2\2\u047d\u047e")
-        buf.write("\7\3\2\2\u047e\u047f\7<\2\2\u047f\u0480\5b\62\2\u0480")
-        buf.write("\u00b9\3\2\2\2\u0481\u0482\7\4\2\2\u0482\u0483\7<\2\2")
-        buf.write("\u0483\u0484\5b\62\2\u0484\u00bb\3\2\2\2\u0485\u048d\7")
-        buf.write("\5\2\2\u0486\u048e\5\36\20\2\u0487\u0489\7,\2\2\u0488")
-        buf.write("\u048a\5\34\17\2\u0489\u0488\3\2\2\2\u048a\u048b\3\2\2")
-        buf.write("\2\u048b\u0489\3\2\2\2\u048b\u048c\3\2\2\2\u048c\u048e")
-        buf.write("\3\2\2\2\u048d\u0486\3\2\2\2\u048d\u0487\3\2\2\2\u048e")
-        buf.write("\u048f\3\2\2\2\u048f\u0490\7A\2\2\u0490\u0491\7,\2\2\u0491")
-        buf.write("\u00bd\3\2\2\2\u00af\u00c3\u00c7\u00c9\u00d2\u00db\u00de")
-        buf.write("\u00e5\u00eb\u00f3\u00f8\u00ff\u0106\u010c\u0110\u0116")
-        buf.write("\u011c\u0120\u0127\u0129\u012b\u0130\u0132\u0134\u0138")
-        buf.write("\u013e\u0142\u0149\u014b\u014d\u0152\u0154\u0159\u015c")
-        buf.write("\u0161\u0167\u016b\u0171\u0177\u017b\u0182\u0184\u0186")
-        buf.write("\u018b\u018d\u018f\u0193\u0199\u019d\u01a4\u01a6\u01a8")
-        buf.write("\u01ad\u01af\u01b3\u01b7\u01be\u01c2\u01cf\u01d6\u01db")
-        buf.write("\u01df\u01e2\u01e8\u01ec\u01f1\u01f5\u01f9\u0207\u020f")
-        buf.write("\u0217\u0219\u021d\u0226\u022d\u022f\u0238\u023d\u0242")
-        buf.write("\u0249\u024d\u0254\u025c\u0265\u026e\u0275\u0281\u0287")
-        buf.write("\u0294\u029a\u02a3\u02ae\u02b9\u02be\u02c3\u02c8\u02d0")
-        buf.write("\u02d9\u02df\u02e1\u02e9\u02ed\u02f5\u02f9\u02fd\u0301")
-        buf.write("\u0308\u0312\u031a\u0320\u0328\u0338\u0342\u034a\u0352")
-        buf.write("\u035a\u0362\u036a\u0370\u0375\u0378\u037e\u0384\u0389")
-        buf.write("\u038e\u0397\u039d\u03a1\u03a7\u03ab\u03af\u03b1\u03b5")
-        buf.write("\u03be\u03c5\u03c9\u03cd\u03d1\u03d4\u03d6\u03da\u03de")
-        buf.write("\u03e3\u03e7\u03eb\u03f2\u03f6\u03fe\u0408\u040c\u0410")
-        buf.write("\u0412\u0416\u041c\u0420\u0424\u0426\u0428\u042e\u0431")
-        buf.write("\u043b\u043f\u0443\u044d\u0451\u0454\u045b\u0460\u0466")
-        buf.write("\u046b\u046f\u047b\u048b\u048d")
+        buf.write("\3\2\2\2\u02f5\u02f6\3\2\2\2\u02f6\u02f9\3\2\2\2\u02f7")
+        buf.write("\u02f9\5h\65\2\u02f8\u02ef\3\2\2\2\u02f8\u02f7\3\2\2\2")
+        buf.write("\u02f9e\3\2\2\2\u02fa\u02fd\5l\67\2\u02fb\u02fd\5j\66")
+        buf.write("\2\u02fc\u02fa\3\2\2\2\u02fc\u02fb\3\2\2\2\u02fdg\3\2")
+        buf.write("\2\2\u02fe\u0300\7\34\2\2\u02ff\u0301\5\30\r\2\u0300\u02ff")
+        buf.write("\3\2\2\2\u0300\u0301\3\2\2\2\u0301\u0302\3\2\2\2\u0302")
+        buf.write("\u0303\7<\2\2\u0303\u0304\5d\63\2\u0304i\3\2\2\2\u0305")
+        buf.write("\u0307\7\34\2\2\u0306\u0308\5\30\r\2\u0307\u0306\3\2\2")
+        buf.write("\2\u0307\u0308\3\2\2\2\u0308\u0309\3\2\2\2\u0309\u030a")
+        buf.write("\7<\2\2\u030a\u030b\5f\64\2\u030bk\3\2\2\2\u030c\u0311")
+        buf.write("\5n8\2\u030d\u030e\7\35\2\2\u030e\u0310\5n8\2\u030f\u030d")
+        buf.write("\3\2\2\2\u0310\u0313\3\2\2\2\u0311\u030f\3\2\2\2\u0311")
+        buf.write("\u0312\3\2\2\2\u0312m\3\2\2\2\u0313\u0311\3\2\2\2\u0314")
+        buf.write("\u0319\5p9\2\u0315\u0316\7\36\2\2\u0316\u0318\5p9\2\u0317")
+        buf.write("\u0315\3\2\2\2\u0318\u031b\3\2\2\2\u0319\u0317\3\2\2\2")
+        buf.write("\u0319\u031a\3\2\2\2\u031ao\3\2\2\2\u031b\u0319\3\2\2")
+        buf.write("\2\u031c\u031d\7\37\2\2\u031d\u0320\5p9\2\u031e\u0320")
+        buf.write("\5r:\2\u031f\u031c\3\2\2\2\u031f\u031e\3\2\2\2\u0320q")
+        buf.write("\3\2\2\2\u0321\u0327\5x=\2\u0322\u0323\5t;\2\u0323\u0324")
+        buf.write("\5x=\2\u0324\u0326\3\2\2\2\u0325\u0322\3\2\2\2\u0326\u0329")
+        buf.write("\3\2\2\2\u0327\u0325\3\2\2\2\u0327\u0328\3\2\2\2\u0328")
+        buf.write("s\3\2\2\2\u0329\u0327\3\2\2\2\u032a\u0338\7O\2\2\u032b")
+        buf.write("\u0338\7P\2\2\u032c\u0338\7Q\2\2\u032d\u0338\7R\2\2\u032e")
+        buf.write("\u0338\7S\2\2\u032f\u0338\7T\2\2\u0330\u0338\7U\2\2\u0331")
+        buf.write("\u0338\7\27\2\2\u0332\u0333\7\37\2\2\u0333\u0338\7\27")
+        buf.write("\2\2\u0334\u0338\7 \2\2\u0335\u0336\7 \2\2\u0336\u0338")
+        buf.write("\7\37\2\2\u0337\u032a\3\2\2\2\u0337\u032b\3\2\2\2\u0337")
+        buf.write("\u032c\3\2\2\2\u0337\u032d\3\2\2\2\u0337\u032e\3\2\2\2")
+        buf.write("\u0337\u032f\3\2\2\2\u0337\u0330\3\2\2\2\u0337\u0331\3")
+        buf.write("\2\2\2\u0337\u0332\3\2\2\2\u0337\u0334\3\2\2\2\u0337\u0335")
+        buf.write("\3\2\2\2\u0338u\3\2\2\2\u0339\u033a\78\2\2\u033a\u033b")
+        buf.write("\5x=\2\u033bw\3\2\2\2\u033c\u0341\5z>\2\u033d\u033e\7")
+        buf.write("B\2\2\u033e\u0340\5z>\2\u033f\u033d\3\2\2\2\u0340\u0343")
+        buf.write("\3\2\2\2\u0341\u033f\3\2\2\2\u0341\u0342\3\2\2\2\u0342")
+        buf.write("y\3\2\2\2\u0343\u0341\3\2\2\2\u0344\u0349\5|?\2\u0345")
+        buf.write("\u0346\7C\2\2\u0346\u0348\5|?\2\u0347\u0345\3\2\2\2\u0348")
+        buf.write("\u034b\3\2\2\2\u0349\u0347\3\2\2\2\u0349\u034a\3\2\2\2")
+        buf.write("\u034a{\3\2\2\2\u034b\u0349\3\2\2\2\u034c\u0351\5~@\2")
+        buf.write("\u034d\u034e\7D\2\2\u034e\u0350\5~@\2\u034f\u034d\3\2")
+        buf.write("\2\2\u0350\u0353\3\2\2\2\u0351\u034f\3\2\2\2\u0351\u0352")
+        buf.write("\3\2\2\2\u0352}\3\2\2\2\u0353\u0351\3\2\2\2\u0354\u0359")
+        buf.write("\5\u0080A\2\u0355\u0356\t\4\2\2\u0356\u0358\5\u0080A\2")
+        buf.write("\u0357\u0355\3\2\2\2\u0358\u035b\3\2\2\2\u0359\u0357\3")
+        buf.write("\2\2\2\u0359\u035a\3\2\2\2\u035a\177\3\2\2\2\u035b\u0359")
+        buf.write("\3\2\2\2\u035c\u0361\5\u0082B\2\u035d\u035e\t\5\2\2\u035e")
+        buf.write("\u0360\5\u0082B\2\u035f\u035d\3\2\2\2\u0360\u0363\3\2")
+        buf.write("\2\2\u0361\u035f\3\2\2\2\u0361\u0362\3\2\2\2\u0362\u0081")
+        buf.write("\3\2\2\2\u0363\u0361\3\2\2\2\u0364\u0369\5\u0084C\2\u0365")
+        buf.write("\u0366\t\6\2\2\u0366\u0368\5\u0084C\2\u0367\u0365\3\2")
+        buf.write("\2\2\u0368\u036b\3\2\2\2\u0369\u0367\3\2\2\2\u0369\u036a")
+        buf.write("\3\2\2\2\u036a\u0083\3\2\2\2\u036b\u0369\3\2\2\2\u036c")
+        buf.write("\u036d\t\7\2\2\u036d\u0370\5\u0084C\2\u036e\u0370\5\u0086")
+        buf.write("D\2\u036f\u036c\3\2\2\2\u036f\u036e\3\2\2\2\u0370\u0085")
+        buf.write("\3\2\2\2\u0371\u0374\5\u0088E\2\u0372\u0373\7>\2\2\u0373")
+        buf.write("\u0375\5\u0084C\2\u0374\u0372\3\2\2\2\u0374\u0375\3\2")
+        buf.write("\2\2\u0375\u0087\3\2\2\2\u0376\u0378\7+\2\2\u0377\u0376")
+        buf.write("\3\2\2\2\u0377\u0378\3\2\2\2\u0378\u0379\3\2\2\2\u0379")
+        buf.write("\u037d\5\u008aF\2\u037a\u037c\5\u008eH\2\u037b\u037a\3")
+        buf.write("\2\2\2\u037c\u037f\3\2\2\2\u037d\u037b\3\2\2\2\u037d\u037e")
+        buf.write("\3\2\2\2\u037e\u0089\3\2\2\2\u037f\u037d\3\2\2\2\u0380")
+        buf.write("\u0383\79\2\2\u0381\u0384\5\u00aaV\2\u0382\u0384\5\u008c")
+        buf.write("G\2\u0383\u0381\3\2\2\2\u0383\u0382\3\2\2\2\u0383\u0384")
+        buf.write("\3\2\2\2\u0384\u0385\3\2\2\2\u0385\u039d\7:\2\2\u0386")
+        buf.write("\u0388\7@\2\2\u0387\u0389\5\u008cG\2\u0388\u0387\3\2\2")
+        buf.write("\2\u0388\u0389\3\2\2\2\u0389\u038a\3\2\2\2\u038a\u039d")
+        buf.write("\7A\2\2\u038b\u038d\7M\2\2\u038c\u038e\5\u009aN\2\u038d")
+        buf.write("\u038c\3\2\2\2\u038d\u038e\3\2\2\2\u038e\u038f\3\2\2\2")
+        buf.write("\u038f\u039d\7N\2\2\u0390\u039d\5\u00aeX\2\u0391\u039d")
+        buf.write("\7-\2\2\u0392\u039d\7\7\2\2\u0393\u0395\7\6\2\2\u0394")
+        buf.write("\u0393\3\2\2\2\u0395\u0396\3\2\2\2\u0396\u0394\3\2\2\2")
+        buf.write("\u0396\u0397\3\2\2\2\u0397\u039d\3\2\2\2\u0398\u039d\7")
+        buf.write("\67\2\2\u0399\u039d\7!\2\2\u039a\u039d\7\"\2\2\u039b\u039d")
+        buf.write("\7#\2\2\u039c\u0380\3\2\2\2\u039c\u0386\3\2\2\2\u039c")
+        buf.write("\u038b\3\2\2\2\u039c\u0390\3\2\2\2\u039c\u0391\3\2\2\2")
+        buf.write("\u039c\u0392\3\2\2\2\u039c\u0394\3\2\2\2\u039c\u0398\3")
+        buf.write("\2\2\2\u039c\u0399\3\2\2\2\u039c\u039a\3\2\2\2\u039c\u039b")
+        buf.write("\3\2\2\2\u039d\u008b\3\2\2\2\u039e\u03a1\5d\63\2\u039f")
+        buf.write("\u03a1\5v<\2\u03a0\u039e\3\2\2\2\u03a0\u039f\3\2\2\2\u03a1")
+        buf.write("\u03b0\3\2\2\2\u03a2\u03b1\5\u00a4S\2\u03a3\u03a6\7;\2")
+        buf.write("\2\u03a4\u03a7\5d\63\2\u03a5\u03a7\5v<\2\u03a6\u03a4\3")
+        buf.write("\2\2\2\u03a6\u03a5\3\2\2\2\u03a7\u03a9\3\2\2\2\u03a8\u03a3")
+        buf.write("\3\2\2\2\u03a9\u03ac\3\2\2\2\u03aa\u03a8\3\2\2\2\u03aa")
+        buf.write("\u03ab\3\2\2\2\u03ab\u03ae\3\2\2\2\u03ac\u03aa\3\2\2\2")
+        buf.write("\u03ad\u03af\7;\2\2\u03ae\u03ad\3\2\2\2\u03ae\u03af\3")
+        buf.write("\2\2\2\u03af\u03b1\3\2\2\2\u03b0\u03a2\3\2\2\2\u03b0\u03aa")
+        buf.write("\3\2\2\2\u03b1\u008d\3\2\2\2\u03b2\u03b4\79\2\2\u03b3")
+        buf.write("\u03b5\5\u009eP\2\u03b4\u03b3\3\2\2\2\u03b4\u03b5\3\2")
+        buf.write("\2\2\u03b5\u03b6\3\2\2\2\u03b6\u03be\7:\2\2\u03b7\u03b8")
+        buf.write("\7@\2\2\u03b8\u03b9\5\u0090I\2\u03b9\u03ba\7A\2\2\u03ba")
+        buf.write("\u03be\3\2\2\2\u03bb\u03bc\7\66\2\2\u03bc\u03be\7-\2\2")
+        buf.write("\u03bd\u03b2\3\2\2\2\u03bd\u03b7\3\2\2\2\u03bd\u03bb\3")
+        buf.write("\2\2\2\u03be\u008f\3\2\2\2\u03bf\u03c4\5\u0092J\2\u03c0")
+        buf.write("\u03c1\7;\2\2\u03c1\u03c3\5\u0092J\2\u03c2\u03c0\3\2\2")
+        buf.write("\2\u03c3\u03c6\3\2\2\2\u03c4\u03c2\3\2\2\2\u03c4\u03c5")
+        buf.write("\3\2\2\2\u03c5\u03c8\3\2\2\2\u03c6\u03c4\3\2\2\2\u03c7")
+        buf.write("\u03c9\7;\2\2\u03c8\u03c7\3\2\2\2\u03c8\u03c9\3\2\2\2")
+        buf.write("\u03c9\u0091\3\2\2\2\u03ca\u03d6\5d\63\2\u03cb\u03cd\5")
+        buf.write("d\63\2\u03cc\u03cb\3\2\2\2\u03cc\u03cd\3\2\2\2\u03cd\u03ce")
+        buf.write("\3\2\2\2\u03ce\u03d0\7<\2\2\u03cf\u03d1\5d\63\2\u03d0")
+        buf.write("\u03cf\3\2\2\2\u03d0\u03d1\3\2\2\2\u03d1\u03d3\3\2\2\2")
+        buf.write("\u03d2\u03d4\5\u0094K\2\u03d3\u03d2\3\2\2\2\u03d3\u03d4")
+        buf.write("\3\2\2\2\u03d4\u03d6\3\2\2\2\u03d5\u03ca\3\2\2\2\u03d5")
+        buf.write("\u03cc\3\2\2\2\u03d6\u0093\3\2\2\2\u03d7\u03d9\7<\2\2")
+        buf.write("\u03d8\u03da\5d\63\2\u03d9\u03d8\3\2\2\2\u03d9\u03da\3")
+        buf.write("\2\2\2\u03da\u0095\3\2\2\2\u03db\u03de\5x=\2\u03dc\u03de")
+        buf.write("\5v<\2\u03dd\u03db\3\2\2\2\u03dd\u03dc\3\2\2\2\u03de\u03e6")
+        buf.write("\3\2\2\2\u03df\u03e2\7;\2\2\u03e0\u03e3\5x=\2\u03e1\u03e3")
+        buf.write("\5v<\2\u03e2\u03e0\3\2\2\2\u03e2\u03e1\3\2\2\2\u03e3\u03e5")
+        buf.write("\3\2\2\2\u03e4\u03df\3\2\2\2\u03e5\u03e8\3\2\2\2\u03e6")
+        buf.write("\u03e4\3\2\2\2\u03e6\u03e7\3\2\2\2\u03e7\u03ea\3\2\2\2")
+        buf.write("\u03e8\u03e6\3\2\2\2\u03e9\u03eb\7;\2\2\u03ea\u03e9\3")
+        buf.write("\2\2\2\u03ea\u03eb\3\2\2\2\u03eb\u0097\3\2\2\2\u03ec\u03f1")
+        buf.write("\5d\63\2\u03ed\u03ee\7;\2\2\u03ee\u03f0\5d\63\2\u03ef")
+        buf.write("\u03ed\3\2\2\2\u03f0\u03f3\3\2\2\2\u03f1\u03ef\3\2\2\2")
+        buf.write("\u03f1\u03f2\3\2\2\2\u03f2\u03f5\3\2\2\2\u03f3\u03f1\3")
+        buf.write("\2\2\2\u03f4\u03f6\7;\2\2\u03f5\u03f4\3\2\2\2\u03f5\u03f6")
+        buf.write("\3\2\2\2\u03f6\u0099\3\2\2\2\u03f7\u03f8\5d\63\2\u03f8")
+        buf.write("\u03f9\7<\2\2\u03f9\u03fa\5d\63\2\u03fa\u03fe\3\2\2\2")
+        buf.write("\u03fb\u03fc\7>\2\2\u03fc\u03fe\5x=\2\u03fd\u03f7\3\2")
+        buf.write("\2\2\u03fd\u03fb\3\2\2\2\u03fe\u0411\3\2\2\2\u03ff\u0412")
+        buf.write("\5\u00a4S\2\u0400\u0407\7;\2\2\u0401\u0402\5d\63\2\u0402")
+        buf.write("\u0403\7<\2\2\u0403\u0404\5d\63\2\u0404\u0408\3\2\2\2")
+        buf.write("\u0405\u0406\7>\2\2\u0406\u0408\5x=\2\u0407\u0401\3\2")
+        buf.write("\2\2\u0407\u0405\3\2\2\2\u0408\u040a\3\2\2\2\u0409\u0400")
+        buf.write("\3\2\2\2\u040a\u040d\3\2\2\2\u040b\u0409\3\2\2\2\u040b")
+        buf.write("\u040c\3\2\2\2\u040c\u040f\3\2\2\2\u040d\u040b\3\2\2\2")
+        buf.write("\u040e\u0410\7;\2\2\u040f\u040e\3\2\2\2\u040f\u0410\3")
+        buf.write("\2\2\2\u0410\u0412\3\2\2\2\u0411\u03ff\3\2\2\2\u0411\u040b")
+        buf.write("\3\2\2\2\u0412\u0428\3\2\2\2\u0413\u0416\5d\63\2\u0414")
+        buf.write("\u0416\5v<\2\u0415\u0413\3\2\2\2\u0415\u0414\3\2\2\2\u0416")
+        buf.write("\u0425\3\2\2\2\u0417\u0426\5\u00a4S\2\u0418\u041b\7;\2")
+        buf.write("\2\u0419\u041c\5d\63\2\u041a\u041c\5v<\2\u041b\u0419\3")
+        buf.write("\2\2\2\u041b\u041a\3\2\2\2\u041c\u041e\3\2\2\2\u041d\u0418")
+        buf.write("\3\2\2\2\u041e\u0421\3\2\2\2\u041f\u041d\3\2\2\2\u041f")
+        buf.write("\u0420\3\2\2\2\u0420\u0423\3\2\2\2\u0421\u041f\3\2\2\2")
+        buf.write("\u0422\u0424\7;\2\2\u0423\u0422\3\2\2\2\u0423\u0424\3")
+        buf.write("\2\2\2\u0424\u0426\3\2\2\2\u0425\u0417\3\2\2\2\u0425\u041f")
+        buf.write("\3\2\2\2\u0426\u0428\3\2\2\2\u0427\u03fd\3\2\2\2\u0427")
+        buf.write("\u0415\3\2\2\2\u0428\u009b\3\2\2\2\u0429\u042a\7$\2\2")
+        buf.write("\u042a\u0430\7-\2\2\u042b\u042d\79\2\2\u042c\u042e\5\u009e")
+        buf.write("P\2\u042d\u042c\3\2\2\2\u042d\u042e\3\2\2\2\u042e\u042f")
+        buf.write("\3\2\2\2\u042f\u0431\7:\2\2\u0430\u042b\3\2\2\2\u0430")
+        buf.write("\u0431\3\2\2\2\u0431\u0432\3\2\2\2\u0432\u0433\7<\2\2")
+        buf.write("\u0433\u0434\5b\62\2\u0434\u009d\3\2\2\2\u0435\u043a\5")
+        buf.write("\u00a0Q\2\u0436\u0437\7;\2\2\u0437\u0439\5\u00a0Q\2\u0438")
+        buf.write("\u0436\3\2\2\2\u0439\u043c\3\2\2\2\u043a\u0438\3\2\2\2")
+        buf.write("\u043a\u043b\3\2\2\2\u043b\u043e\3\2\2\2\u043c\u043a\3")
+        buf.write("\2\2\2\u043d\u043f\7;\2\2\u043e\u043d\3\2\2\2\u043e\u043f")
+        buf.write("\3\2\2\2\u043f\u009f\3\2\2\2\u0440\u0442\5d\63\2\u0441")
+        buf.write("\u0443\5\u00a4S\2\u0442\u0441\3\2\2\2\u0442\u0443\3\2")
+        buf.write("\2\2\u0443\u044d\3\2\2\2\u0444\u0445\5d\63\2\u0445\u0446")
+        buf.write("\7?\2\2\u0446\u0447\5d\63\2\u0447\u044d\3\2\2\2\u0448")
+        buf.write("\u0449\7>\2\2\u0449\u044d\5d\63\2\u044a\u044b\78\2\2\u044b")
+        buf.write("\u044d\5d\63\2\u044c\u0440\3\2\2\2\u044c\u0444\3\2\2\2")
+        buf.write("\u044c\u0448\3\2\2\2\u044c\u044a\3\2\2\2\u044d\u00a1\3")
+        buf.write("\2\2\2\u044e\u0451\5\u00a4S\2\u044f\u0451\5\u00a6T\2\u0450")
+        buf.write("\u044e\3\2\2\2\u0450\u044f\3\2\2\2\u0451\u00a3\3\2\2\2")
+        buf.write("\u0452\u0454\7*\2\2\u0453\u0452\3\2\2\2\u0453\u0454\3")
+        buf.write("\2\2\2\u0454\u0455\3\2\2\2\u0455\u0456\7\26\2\2\u0456")
+        buf.write("\u0457\5\u0096L\2\u0457\u0458\7\27\2\2\u0458\u045a\5l")
+        buf.write("\67\2\u0459\u045b\5\u00a2R\2\u045a\u0459\3\2\2\2\u045a")
+        buf.write("\u045b\3\2\2\2\u045b\u00a5\3\2\2\2\u045c\u045d\7\22\2")
+        buf.write("\2\u045d\u045f\5f\64\2\u045e\u0460\5\u00a2R\2\u045f\u045e")
+        buf.write("\3\2\2\2\u045f\u0460\3\2\2\2\u0460\u00a7\3\2\2\2\u0461")
+        buf.write("\u0462\7-\2\2\u0462\u00a9\3\2\2\2\u0463\u0465\7%\2\2\u0464")
+        buf.write("\u0466\5\u00acW\2\u0465\u0464\3\2\2\2\u0465\u0466\3\2")
+        buf.write("\2\2\u0466\u00ab\3\2\2\2\u0467\u0468\7\f\2\2\u0468\u046b")
+        buf.write("\5d\63\2\u0469\u046b\5\u0098M\2\u046a\u0467\3\2\2\2\u046a")
+        buf.write("\u0469\3\2\2\2\u046b\u00ad\3\2\2\2\u046c\u0470\5\u00b0")
+        buf.write("Y\2\u046d\u0470\5\u00b2Z\2\u046e\u0470\5\u00b4[\2\u046f")
+        buf.write("\u046c\3\2\2\2\u046f\u046d\3\2\2\2\u046f\u046e\3\2\2\2")
+        buf.write("\u0470\u00af\3\2\2\2\u0471\u0472\7\3\2\2\u0472\u00b1\3")
+        buf.write("\2\2\2\u0473\u0474\7\4\2\2\u0474\u00b3\3\2\2\2\u0475\u0476")
+        buf.write("\7\3\2\2\u0476\u0477\7-\2\2\u0477\u00b5\3\2\2\2\u0478")
+        buf.write("\u047c\5\u00b8]\2\u0479\u047c\5\u00ba^\2\u047a\u047c\5")
+        buf.write("\u00bc_\2\u047b\u0478\3\2\2\2\u047b\u0479\3\2\2\2\u047b")
+        buf.write("\u047a\3\2\2\2\u047c\u00b7\3\2\2\2\u047d\u047e\7\3\2\2")
+        buf.write("\u047e\u047f\7<\2\2\u047f\u0480\5b\62\2\u0480\u00b9\3")
+        buf.write("\2\2\2\u0481\u0482\7\4\2\2\u0482\u0483\7<\2\2\u0483\u0484")
+        buf.write("\5b\62\2\u0484\u00bb\3\2\2\2\u0485\u048d\7\5\2\2\u0486")
+        buf.write("\u048e\5\36\20\2\u0487\u0489\7,\2\2\u0488\u048a\5\34\17")
+        buf.write("\2\u0489\u0488\3\2\2\2\u048a\u048b\3\2\2\2\u048b\u0489")
+        buf.write("\3\2\2\2\u048b\u048c\3\2\2\2\u048c\u048e\3\2\2\2\u048d")
+        buf.write("\u0486\3\2\2\2\u048d\u0487\3\2\2\2\u048e\u048f\3\2\2\2")
+        buf.write("\u048f\u0490\7A\2\2\u0490\u0491\7,\2\2\u0491\u00bd\3\2")
+        buf.write("\2\2\u00af\u00c3\u00c7\u00c9\u00d2\u00db\u00de\u00e5\u00eb")
+        buf.write("\u00f3\u00f8\u00ff\u0106\u010c\u0110\u0116\u011c\u0120")
+        buf.write("\u0127\u0129\u012b\u0130\u0132\u0134\u0138\u013e\u0142")
+        buf.write("\u0149\u014b\u014d\u0152\u0154\u0159\u015c\u0161\u0167")
+        buf.write("\u016b\u0171\u0177\u017b\u0182\u0184\u0186\u018b\u018d")
+        buf.write("\u018f\u0193\u0199\u019d\u01a4\u01a6\u01a8\u01ad\u01af")
+        buf.write("\u01b3\u01b7\u01be\u01c2\u01cf\u01d6\u01db\u01df\u01e2")
+        buf.write("\u01e8\u01ec\u01f1\u01f5\u01f9\u0207\u020f\u0217\u0219")
+        buf.write("\u021d\u0226\u022d\u022f\u0238\u023d\u0242\u0249\u024d")
+        buf.write("\u0254\u025c\u0265\u026e\u0275\u0281\u0287\u0294\u029a")
+        buf.write("\u02a3\u02ae\u02b9\u02be\u02c3\u02c8\u02d0\u02d9\u02df")
+        buf.write("\u02e1\u02e9\u02ed\u02f5\u02f8\u02fc\u0300\u0307\u0311")
+        buf.write("\u0319\u031f\u0327\u0337\u0341\u0349\u0351\u0359\u0361")
+        buf.write("\u0369\u036f\u0374\u0377\u037d\u0383\u0388\u038d\u0396")
+        buf.write("\u039c\u03a0\u03a6\u03aa\u03ae\u03b0\u03b4\u03bd\u03c4")
+        buf.write("\u03c8\u03cc\u03d0\u03d3\u03d5\u03d9\u03dd\u03e2\u03e6")
+        buf.write("\u03ea\u03f1\u03f5\u03fd\u0407\u040b\u040f\u0411\u0415")
+        buf.write("\u041b\u041f\u0423\u0425\u0427\u042d\u0430\u043a\u043e")
+        buf.write("\u0442\u044c\u0450\u0453\u045a\u045f\u0465\u046a\u046f")
+        buf.write("\u047b\u048b\u048d")
         return buf.getvalue()
 
 
 class Python3Parser ( Parser ):
 
     grammarFileName = "Python3.g4"
 
@@ -5142,18 +5143,14 @@
             return self.getTypedRuleContext(Python3Parser.TestContext,0)
 
 
         def lambdef(self):
             return self.getTypedRuleContext(Python3Parser.LambdefContext,0)
 
 
-        def var_hole(self):
-            return self.getTypedRuleContext(Python3Parser.Var_holeContext,0)
-
-
         def getRuleIndex(self):
             return Python3Parser.RULE_test
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterTest" ):
                 listener.enterTest(self)
 
@@ -5172,18 +5169,18 @@
 
     def test(self):
 
         localctx = Python3Parser.TestContext(self, self._ctx, self.state)
         self.enterRule(localctx, 98, self.RULE_test)
         self._la = 0 # Token type
         try:
-            self.state = 759
+            self.state = 758
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,102,self._ctx)
-            if la_ == 1:
+            token = self._input.LA(1)
+            if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
                 self.enterOuterAlt(localctx, 1)
                 self.state = 749
                 self.or_test()
                 self.state = 755
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==Python3Parser.IF:
@@ -5194,27 +5191,21 @@
                     self.state = 752
                     self.match(Python3Parser.ELSE)
                     self.state = 753
                     self.test()
 
 
                 pass
-
-            elif la_ == 2:
+            elif token in [Python3Parser.LAMBDA]:
                 self.enterOuterAlt(localctx, 2)
                 self.state = 757
                 self.lambdef()
                 pass
-
-            elif la_ == 3:
-                self.enterOuterAlt(localctx, 3)
-                self.state = 758
-                self.var_hole()
-                pass
-
+            else:
+                raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5255,25 +5246,25 @@
 
 
     def test_nocond(self):
 
         localctx = Python3Parser.Test_nocondContext(self, self._ctx, self.state)
         self.enterRule(localctx, 100, self.RULE_test_nocond)
         try:
-            self.state = 763
+            self.state = 762
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 761
+                self.state = 760
                 self.or_test()
                 pass
             elif token in [Python3Parser.LAMBDA]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 762
+                self.state = 761
                 self.lambdef_nocond()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -5326,27 +5317,27 @@
     def lambdef(self):
 
         localctx = Python3Parser.LambdefContext(self, self._ctx, self.state)
         self.enterRule(localctx, 102, self.RULE_lambdef)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 765
+            self.state = 764
             self.match(Python3Parser.LAMBDA)
-            self.state = 767
+            self.state = 766
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.NAME) | (1 << Python3Parser.STAR) | (1 << Python3Parser.POWER))) != 0):
-                self.state = 766
+                self.state = 765
                 self.varargslist()
 
 
-            self.state = 769
+            self.state = 768
             self.match(Python3Parser.COLON)
-            self.state = 770
+            self.state = 769
             self.test()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5395,27 +5386,27 @@
     def lambdef_nocond(self):
 
         localctx = Python3Parser.Lambdef_nocondContext(self, self._ctx, self.state)
         self.enterRule(localctx, 104, self.RULE_lambdef_nocond)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 772
+            self.state = 771
             self.match(Python3Parser.LAMBDA)
-            self.state = 774
+            self.state = 773
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.NAME) | (1 << Python3Parser.STAR) | (1 << Python3Parser.POWER))) != 0):
-                self.state = 773
+                self.state = 772
                 self.varargslist()
 
 
-            self.state = 776
+            self.state = 775
             self.match(Python3Parser.COLON)
-            self.state = 777
+            self.state = 776
             self.test_nocond()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5463,25 +5454,25 @@
     def or_test(self):
 
         localctx = Python3Parser.Or_testContext(self, self._ctx, self.state)
         self.enterRule(localctx, 106, self.RULE_or_test)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 779
+            self.state = 778
             self.and_test()
-            self.state = 784
+            self.state = 783
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==Python3Parser.OR:
-                self.state = 780
+                self.state = 779
                 self.match(Python3Parser.OR)
-                self.state = 781
+                self.state = 780
                 self.and_test()
-                self.state = 786
+                self.state = 785
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5531,25 +5522,25 @@
     def and_test(self):
 
         localctx = Python3Parser.And_testContext(self, self._ctx, self.state)
         self.enterRule(localctx, 108, self.RULE_and_test)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 787
+            self.state = 786
             self.not_test()
-            self.state = 792
+            self.state = 791
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==Python3Parser.AND:
-                self.state = 788
+                self.state = 787
                 self.match(Python3Parser.AND)
-                self.state = 789
+                self.state = 788
                 self.not_test()
-                self.state = 794
+                self.state = 793
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5595,27 +5586,27 @@
 
 
     def not_test(self):
 
         localctx = Python3Parser.Not_testContext(self, self._ctx, self.state)
         self.enterRule(localctx, 110, self.RULE_not_test)
         try:
-            self.state = 798
+            self.state = 797
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.NOT]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 795
+                self.state = 794
                 self.match(Python3Parser.NOT)
-                self.state = 796
+                self.state = 795
                 self.not_test()
                 pass
             elif token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 797
+                self.state = 796
                 self.comparison()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -5668,25 +5659,25 @@
     def comparison(self):
 
         localctx = Python3Parser.ComparisonContext(self, self._ctx, self.state)
         self.enterRule(localctx, 112, self.RULE_comparison)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 800
+            self.state = 799
             self.expr()
-            self.state = 806
+            self.state = 805
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while ((((_la - 21)) & ~0x3f) == 0 and ((1 << (_la - 21)) & ((1 << (Python3Parser.IN - 21)) | (1 << (Python3Parser.NOT - 21)) | (1 << (Python3Parser.IS - 21)) | (1 << (Python3Parser.LESS_THAN - 21)) | (1 << (Python3Parser.GREATER_THAN - 21)) | (1 << (Python3Parser.EQUALS - 21)) | (1 << (Python3Parser.GT_EQ - 21)) | (1 << (Python3Parser.LT_EQ - 21)) | (1 << (Python3Parser.NOT_EQ_1 - 21)) | (1 << (Python3Parser.NOT_EQ_2 - 21)))) != 0):
-                self.state = 801
+                self.state = 800
                 self.comp_op()
-                self.state = 802
+                self.state = 801
                 self.expr()
-                self.state = 808
+                self.state = 807
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5751,84 +5742,84 @@
 
 
     def comp_op(self):
 
         localctx = Python3Parser.Comp_opContext(self, self._ctx, self.state)
         self.enterRule(localctx, 114, self.RULE_comp_op)
         try:
-            self.state = 822
+            self.state = 821
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,110,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 809
+                self.state = 808
                 self.match(Python3Parser.LESS_THAN)
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 810
+                self.state = 809
                 self.match(Python3Parser.GREATER_THAN)
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 811
+                self.state = 810
                 self.match(Python3Parser.EQUALS)
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 812
+                self.state = 811
                 self.match(Python3Parser.GT_EQ)
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 813
+                self.state = 812
                 self.match(Python3Parser.LT_EQ)
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 814
+                self.state = 813
                 self.match(Python3Parser.NOT_EQ_1)
                 pass
 
             elif la_ == 7:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 815
+                self.state = 814
                 self.match(Python3Parser.NOT_EQ_2)
                 pass
 
             elif la_ == 8:
                 self.enterOuterAlt(localctx, 8)
-                self.state = 816
+                self.state = 815
                 self.match(Python3Parser.IN)
                 pass
 
             elif la_ == 9:
                 self.enterOuterAlt(localctx, 9)
-                self.state = 817
+                self.state = 816
                 self.match(Python3Parser.NOT)
-                self.state = 818
+                self.state = 817
                 self.match(Python3Parser.IN)
                 pass
 
             elif la_ == 10:
                 self.enterOuterAlt(localctx, 10)
-                self.state = 819
+                self.state = 818
                 self.match(Python3Parser.IS)
                 pass
 
             elif la_ == 11:
                 self.enterOuterAlt(localctx, 11)
-                self.state = 820
+                self.state = 819
                 self.match(Python3Parser.IS)
-                self.state = 821
+                self.state = 820
                 self.match(Python3Parser.NOT)
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -5872,17 +5863,17 @@
 
     def star_expr(self):
 
         localctx = Python3Parser.Star_exprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 116, self.RULE_star_expr)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 824
+            self.state = 823
             self.match(Python3Parser.STAR)
-            self.state = 825
+            self.state = 824
             self.expr()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5930,25 +5921,25 @@
     def expr(self):
 
         localctx = Python3Parser.ExprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 118, self.RULE_expr)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 827
+            self.state = 826
             self.xor_expr()
-            self.state = 832
+            self.state = 831
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==Python3Parser.OR_OP:
-                self.state = 828
+                self.state = 827
                 self.match(Python3Parser.OR_OP)
-                self.state = 829
+                self.state = 828
                 self.xor_expr()
-                self.state = 834
+                self.state = 833
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5998,25 +5989,25 @@
     def xor_expr(self):
 
         localctx = Python3Parser.Xor_exprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 120, self.RULE_xor_expr)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 835
+            self.state = 834
             self.and_expr()
-            self.state = 840
+            self.state = 839
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==Python3Parser.XOR:
-                self.state = 836
+                self.state = 835
                 self.match(Python3Parser.XOR)
-                self.state = 837
+                self.state = 836
                 self.and_expr()
-                self.state = 842
+                self.state = 841
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6066,25 +6057,25 @@
     def and_expr(self):
 
         localctx = Python3Parser.And_exprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 122, self.RULE_and_expr)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 843
+            self.state = 842
             self.shift_expr()
-            self.state = 848
+            self.state = 847
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==Python3Parser.AND_OP:
-                self.state = 844
+                self.state = 843
                 self.match(Python3Parser.AND_OP)
-                self.state = 845
+                self.state = 844
                 self.shift_expr()
-                self.state = 850
+                self.state = 849
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6140,30 +6131,30 @@
     def shift_expr(self):
 
         localctx = Python3Parser.Shift_exprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 124, self.RULE_shift_expr)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 851
+            self.state = 850
             self.arith_expr()
-            self.state = 856
+            self.state = 855
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==Python3Parser.LEFT_SHIFT or _la==Python3Parser.RIGHT_SHIFT:
-                self.state = 852
+                self.state = 851
                 _la = self._input.LA(1)
                 if not(_la==Python3Parser.LEFT_SHIFT or _la==Python3Parser.RIGHT_SHIFT):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 853
+                self.state = 852
                 self.arith_expr()
-                self.state = 858
+                self.state = 857
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6219,30 +6210,30 @@
     def arith_expr(self):
 
         localctx = Python3Parser.Arith_exprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 126, self.RULE_arith_expr)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 859
+            self.state = 858
             self.term()
-            self.state = 864
+            self.state = 863
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==Python3Parser.ADD or _la==Python3Parser.MINUS:
-                self.state = 860
+                self.state = 859
                 _la = self._input.LA(1)
                 if not(_la==Python3Parser.ADD or _la==Python3Parser.MINUS):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 861
+                self.state = 860
                 self.term()
-                self.state = 866
+                self.state = 865
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6316,30 +6307,30 @@
     def term(self):
 
         localctx = Python3Parser.TermContext(self, self._ctx, self.state)
         self.enterRule(localctx, 128, self.RULE_term)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 867
+            self.state = 866
             self.factor()
-            self.state = 872
+            self.state = 871
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while ((((_la - 54)) & ~0x3f) == 0 and ((1 << (_la - 54)) & ((1 << (Python3Parser.STAR - 54)) | (1 << (Python3Parser.DIV - 54)) | (1 << (Python3Parser.MOD - 54)) | (1 << (Python3Parser.IDIV - 54)) | (1 << (Python3Parser.AT - 54)))) != 0):
-                self.state = 868
+                self.state = 867
                 _la = self._input.LA(1)
                 if not(((((_la - 54)) & ~0x3f) == 0 and ((1 << (_la - 54)) & ((1 << (Python3Parser.STAR - 54)) | (1 << (Python3Parser.DIV - 54)) | (1 << (Python3Parser.MOD - 54)) | (1 << (Python3Parser.IDIV - 54)) | (1 << (Python3Parser.AT - 54)))) != 0)):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 869
+                self.state = 868
                 self.factor()
-                self.state = 874
+                self.state = 873
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6392,32 +6383,32 @@
 
     def factor(self):
 
         localctx = Python3Parser.FactorContext(self, self._ctx, self.state)
         self.enterRule(localctx, 130, self.RULE_factor)
         self._la = 0 # Token type
         try:
-            self.state = 878
+            self.state = 877
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 875
+                self.state = 874
                 _la = self._input.LA(1)
                 if not(((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)))) != 0)):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 876
+                self.state = 875
                 self.factor()
                 pass
             elif token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.OPEN_BRACE]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 877
+                self.state = 876
                 self.power()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -6467,23 +6458,23 @@
     def power(self):
 
         localctx = Python3Parser.PowerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 132, self.RULE_power)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 880
+            self.state = 879
             self.atom_expr()
-            self.state = 883
+            self.state = 882
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.POWER:
-                self.state = 881
+                self.state = 880
                 self.match(Python3Parser.POWER)
-                self.state = 882
+                self.state = 881
                 self.factor()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6534,31 +6525,31 @@
     def atom_expr(self):
 
         localctx = Python3Parser.Atom_exprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 134, self.RULE_atom_expr)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 886
+            self.state = 885
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.AWAIT:
-                self.state = 885
+                self.state = 884
                 self.match(Python3Parser.AWAIT)
 
 
-            self.state = 888
+            self.state = 887
             self.atom()
-            self.state = 892
+            self.state = 891
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.DOT) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.OPEN_BRACK))) != 0):
-                self.state = 889
+                self.state = 888
                 self.trailer()
-                self.state = 894
+                self.state = 893
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6653,106 +6644,106 @@
     def atom(self):
 
         localctx = Python3Parser.AtomContext(self, self._ctx, self.state)
         self.enterRule(localctx, 136, self.RULE_atom)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 923
+            self.state = 922
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.OPEN_PAREN]:
-                self.state = 895
+                self.state = 894
                 self.match(Python3Parser.OPEN_PAREN)
-                self.state = 898
+                self.state = 897
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [Python3Parser.YIELD]:
-                    self.state = 896
+                    self.state = 895
                     self.yield_expr()
                     pass
                 elif token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.STAR, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                    self.state = 897
+                    self.state = 896
                     self.testlist_comp()
                     pass
                 elif token in [Python3Parser.CLOSE_PAREN]:
                     pass
                 else:
                     pass
-                self.state = 900
+                self.state = 899
                 self.match(Python3Parser.CLOSE_PAREN)
                 pass
             elif token in [Python3Parser.OPEN_BRACK]:
-                self.state = 901
+                self.state = 900
                 self.match(Python3Parser.OPEN_BRACK)
-                self.state = 903
+                self.state = 902
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.STAR) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                    self.state = 902
+                    self.state = 901
                     self.testlist_comp()
 
 
-                self.state = 905
+                self.state = 904
                 self.match(Python3Parser.CLOSE_BRACK)
                 pass
             elif token in [Python3Parser.OPEN_BRACE]:
-                self.state = 906
+                self.state = 905
                 self.match(Python3Parser.OPEN_BRACE)
-                self.state = 908
+                self.state = 907
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.STAR) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.POWER) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                    self.state = 907
+                    self.state = 906
                     self.dictorsetmaker()
 
 
-                self.state = 910
+                self.state = 909
                 self.match(Python3Parser.CLOSE_BRACE)
                 pass
             elif token in [Python3Parser.T__0, Python3Parser.T__1]:
-                self.state = 911
+                self.state = 910
                 self.expr_hole()
                 pass
             elif token in [Python3Parser.NAME]:
-                self.state = 912
+                self.state = 911
                 self.match(Python3Parser.NAME)
                 pass
             elif token in [Python3Parser.NUMBER]:
-                self.state = 913
+                self.state = 912
                 self.match(Python3Parser.NUMBER)
                 pass
             elif token in [Python3Parser.STRING]:
-                self.state = 915 
+                self.state = 914 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 914
+                    self.state = 913
                     self.match(Python3Parser.STRING)
-                    self.state = 917 
+                    self.state = 916 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if not (_la==Python3Parser.STRING):
                         break
 
                 pass
             elif token in [Python3Parser.ELLIPSIS]:
-                self.state = 919
+                self.state = 918
                 self.match(Python3Parser.ELLIPSIS)
                 pass
             elif token in [Python3Parser.NONE]:
-                self.state = 920
+                self.state = 919
                 self.match(Python3Parser.NONE)
                 pass
             elif token in [Python3Parser.TRUE]:
-                self.state = 921
+                self.state = 920
                 self.match(Python3Parser.TRUE)
                 pass
             elif token in [Python3Parser.FALSE]:
-                self.state = 922
+                self.state = 921
                 self.match(Python3Parser.FALSE)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -6815,66 +6806,66 @@
     def testlist_comp(self):
 
         localctx = Python3Parser.Testlist_compContext(self, self._ctx, self.state)
         self.enterRule(localctx, 138, self.RULE_testlist_comp)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 927
+            self.state = 926
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                self.state = 925
+                self.state = 924
                 self.test()
                 pass
             elif token in [Python3Parser.STAR]:
-                self.state = 926
+                self.state = 925
                 self.star_expr()
                 pass
             else:
                 raise NoViableAltException(self)
 
-            self.state = 943
+            self.state = 942
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.FOR, Python3Parser.ASYNC]:
-                self.state = 929
+                self.state = 928
                 self.comp_for()
                 pass
             elif token in [Python3Parser.CLOSE_PAREN, Python3Parser.COMMA, Python3Parser.CLOSE_BRACK]:
-                self.state = 937
+                self.state = 936
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,128,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 930
+                        self.state = 929
                         self.match(Python3Parser.COMMA)
-                        self.state = 933
+                        self.state = 932
                         self._errHandler.sync(self)
                         token = self._input.LA(1)
                         if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                            self.state = 931
+                            self.state = 930
                             self.test()
                             pass
                         elif token in [Python3Parser.STAR]:
-                            self.state = 932
+                            self.state = 931
                             self.star_expr()
                             pass
                         else:
                             raise NoViableAltException(self)
                  
-                    self.state = 939
+                    self.state = 938
                     self._errHandler.sync(self)
                     _alt = self._interp.adaptivePredict(self._input,128,self._ctx)
 
-                self.state = 941
+                self.state = 940
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==Python3Parser.COMMA:
-                    self.state = 940
+                    self.state = 939
                     self.match(Python3Parser.COMMA)
 
 
                 pass
             else:
                 raise NoViableAltException(self)
 
@@ -6940,46 +6931,46 @@
 
     def trailer(self):
 
         localctx = Python3Parser.TrailerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 140, self.RULE_trailer)
         self._la = 0 # Token type
         try:
-            self.state = 956
+            self.state = 955
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.OPEN_PAREN]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 945
+                self.state = 944
                 self.match(Python3Parser.OPEN_PAREN)
-                self.state = 947
+                self.state = 946
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.STAR) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.POWER) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                    self.state = 946
+                    self.state = 945
                     self.arglist()
 
 
-                self.state = 949
+                self.state = 948
                 self.match(Python3Parser.CLOSE_PAREN)
                 pass
             elif token in [Python3Parser.OPEN_BRACK]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 950
+                self.state = 949
                 self.match(Python3Parser.OPEN_BRACK)
-                self.state = 951
+                self.state = 950
                 self.subscriptlist()
-                self.state = 952
+                self.state = 951
                 self.match(Python3Parser.CLOSE_BRACK)
                 pass
             elif token in [Python3Parser.DOT]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 954
+                self.state = 953
                 self.match(Python3Parser.DOT)
-                self.state = 955
+                self.state = 954
                 self.match(Python3Parser.NAME)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -7031,34 +7022,34 @@
     def subscriptlist(self):
 
         localctx = Python3Parser.SubscriptlistContext(self, self._ctx, self.state)
         self.enterRule(localctx, 142, self.RULE_subscriptlist)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 958
+            self.state = 957
             self.subscript()
-            self.state = 963
+            self.state = 962
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,133,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 959
+                    self.state = 958
                     self.match(Python3Parser.COMMA)
-                    self.state = 960
+                    self.state = 959
                     self.subscript() 
-                self.state = 965
+                self.state = 964
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,133,self._ctx)
 
-            self.state = 967
+            self.state = 966
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.COMMA:
-                self.state = 966
+                self.state = 965
                 self.match(Python3Parser.COMMA)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -7108,48 +7099,48 @@
 
     def subscript(self):
 
         localctx = Python3Parser.SubscriptContext(self, self._ctx, self.state)
         self.enterRule(localctx, 144, self.RULE_subscript)
         self._la = 0 # Token type
         try:
-            self.state = 980
+            self.state = 979
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,138,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 969
+                self.state = 968
                 self.test()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 971
+                self.state = 970
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                    self.state = 970
+                    self.state = 969
                     self.test()
 
 
-                self.state = 973
+                self.state = 972
                 self.match(Python3Parser.COLON)
-                self.state = 975
+                self.state = 974
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                    self.state = 974
+                    self.state = 973
                     self.test()
 
 
-                self.state = 978
+                self.state = 977
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==Python3Parser.COLON:
-                    self.state = 977
+                    self.state = 976
                     self.sliceop()
 
 
                 pass
 
 
         except RecognitionException as re:
@@ -7196,21 +7187,21 @@
     def sliceop(self):
 
         localctx = Python3Parser.SliceopContext(self, self._ctx, self.state)
         self.enterRule(localctx, 146, self.RULE_sliceop)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 982
+            self.state = 981
             self.match(Python3Parser.COLON)
-            self.state = 984
+            self.state = 983
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                self.state = 983
+                self.state = 982
                 self.test()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -7267,58 +7258,58 @@
     def exprlist(self):
 
         localctx = Python3Parser.ExprlistContext(self, self._ctx, self.state)
         self.enterRule(localctx, 148, self.RULE_exprlist)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 988
+            self.state = 987
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                self.state = 986
+                self.state = 985
                 self.expr()
                 pass
             elif token in [Python3Parser.STAR]:
-                self.state = 987
+                self.state = 986
                 self.star_expr()
                 pass
             else:
                 raise NoViableAltException(self)
 
-            self.state = 997
+            self.state = 996
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,142,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 990
+                    self.state = 989
                     self.match(Python3Parser.COMMA)
-                    self.state = 993
+                    self.state = 992
                     self._errHandler.sync(self)
                     token = self._input.LA(1)
                     if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                        self.state = 991
+                        self.state = 990
                         self.expr()
                         pass
                     elif token in [Python3Parser.STAR]:
-                        self.state = 992
+                        self.state = 991
                         self.star_expr()
                         pass
                     else:
                         raise NoViableAltException(self)
              
-                self.state = 999
+                self.state = 998
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,142,self._ctx)
 
-            self.state = 1001
+            self.state = 1000
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.COMMA:
-                self.state = 1000
+                self.state = 999
                 self.match(Python3Parser.COMMA)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -7368,34 +7359,34 @@
     def testlist(self):
 
         localctx = Python3Parser.TestlistContext(self, self._ctx, self.state)
         self.enterRule(localctx, 150, self.RULE_testlist)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1003
+            self.state = 1002
             self.test()
-            self.state = 1008
+            self.state = 1007
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,144,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 1004
+                    self.state = 1003
                     self.match(Python3Parser.COMMA)
-                    self.state = 1005
+                    self.state = 1004
                     self.test() 
-                self.state = 1010
+                self.state = 1009
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,144,self._ctx)
 
-            self.state = 1012
+            self.state = 1011
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.COMMA:
-                self.state = 1011
+                self.state = 1010
                 self.match(Python3Parser.COMMA)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -7475,144 +7466,144 @@
     def dictorsetmaker(self):
 
         localctx = Python3Parser.DictorsetmakerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 152, self.RULE_dictorsetmaker)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1062
+            self.state = 1061
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,156,self._ctx)
             if la_ == 1:
-                self.state = 1020
+                self.state = 1019
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                    self.state = 1014
+                    self.state = 1013
                     self.test()
-                    self.state = 1015
+                    self.state = 1014
                     self.match(Python3Parser.COLON)
-                    self.state = 1016
+                    self.state = 1015
                     self.test()
                     pass
                 elif token in [Python3Parser.POWER]:
-                    self.state = 1018
+                    self.state = 1017
                     self.match(Python3Parser.POWER)
-                    self.state = 1019
+                    self.state = 1018
                     self.expr()
                     pass
                 else:
                     raise NoViableAltException(self)
 
-                self.state = 1040
+                self.state = 1039
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [Python3Parser.FOR, Python3Parser.ASYNC]:
-                    self.state = 1022
+                    self.state = 1021
                     self.comp_for()
                     pass
                 elif token in [Python3Parser.COMMA, Python3Parser.CLOSE_BRACE]:
-                    self.state = 1034
+                    self.state = 1033
                     self._errHandler.sync(self)
                     _alt = self._interp.adaptivePredict(self._input,148,self._ctx)
                     while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                         if _alt==1:
-                            self.state = 1023
+                            self.state = 1022
                             self.match(Python3Parser.COMMA)
-                            self.state = 1030
+                            self.state = 1029
                             self._errHandler.sync(self)
                             token = self._input.LA(1)
                             if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                                self.state = 1024
+                                self.state = 1023
                                 self.test()
-                                self.state = 1025
+                                self.state = 1024
                                 self.match(Python3Parser.COLON)
-                                self.state = 1026
+                                self.state = 1025
                                 self.test()
                                 pass
                             elif token in [Python3Parser.POWER]:
-                                self.state = 1028
+                                self.state = 1027
                                 self.match(Python3Parser.POWER)
-                                self.state = 1029
+                                self.state = 1028
                                 self.expr()
                                 pass
                             else:
                                 raise NoViableAltException(self)
                      
-                        self.state = 1036
+                        self.state = 1035
                         self._errHandler.sync(self)
                         _alt = self._interp.adaptivePredict(self._input,148,self._ctx)
 
-                    self.state = 1038
+                    self.state = 1037
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==Python3Parser.COMMA:
-                        self.state = 1037
+                        self.state = 1036
                         self.match(Python3Parser.COMMA)
 
 
                     pass
                 else:
                     raise NoViableAltException(self)
 
                 pass
 
             elif la_ == 2:
-                self.state = 1044
+                self.state = 1043
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                    self.state = 1042
+                    self.state = 1041
                     self.test()
                     pass
                 elif token in [Python3Parser.STAR]:
-                    self.state = 1043
+                    self.state = 1042
                     self.star_expr()
                     pass
                 else:
                     raise NoViableAltException(self)
 
-                self.state = 1060
+                self.state = 1059
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [Python3Parser.FOR, Python3Parser.ASYNC]:
-                    self.state = 1046
+                    self.state = 1045
                     self.comp_for()
                     pass
                 elif token in [Python3Parser.COMMA, Python3Parser.CLOSE_BRACE]:
-                    self.state = 1054
+                    self.state = 1053
                     self._errHandler.sync(self)
                     _alt = self._interp.adaptivePredict(self._input,153,self._ctx)
                     while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                         if _alt==1:
-                            self.state = 1047
+                            self.state = 1046
                             self.match(Python3Parser.COMMA)
-                            self.state = 1050
+                            self.state = 1049
                             self._errHandler.sync(self)
                             token = self._input.LA(1)
                             if token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
-                                self.state = 1048
+                                self.state = 1047
                                 self.test()
                                 pass
                             elif token in [Python3Parser.STAR]:
-                                self.state = 1049
+                                self.state = 1048
                                 self.star_expr()
                                 pass
                             else:
                                 raise NoViableAltException(self)
                      
-                        self.state = 1056
+                        self.state = 1055
                         self._errHandler.sync(self)
                         _alt = self._interp.adaptivePredict(self._input,153,self._ctx)
 
-                    self.state = 1058
+                    self.state = 1057
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==Python3Parser.COMMA:
-                        self.state = 1057
+                        self.state = 1056
                         self.match(Python3Parser.COMMA)
 
 
                     pass
                 else:
                     raise NoViableAltException(self)
 
@@ -7679,39 +7670,39 @@
     def classdef(self):
 
         localctx = Python3Parser.ClassdefContext(self, self._ctx, self.state)
         self.enterRule(localctx, 154, self.RULE_classdef)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1064
+            self.state = 1063
             self.match(Python3Parser.CLASS)
-            self.state = 1065
+            self.state = 1064
             self.match(Python3Parser.NAME)
-            self.state = 1071
+            self.state = 1070
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.OPEN_PAREN:
-                self.state = 1066
+                self.state = 1065
                 self.match(Python3Parser.OPEN_PAREN)
-                self.state = 1068
+                self.state = 1067
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.STAR) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.POWER) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                    self.state = 1067
+                    self.state = 1066
                     self.arglist()
 
 
-                self.state = 1070
+                self.state = 1069
                 self.match(Python3Parser.CLOSE_PAREN)
 
 
-            self.state = 1073
+            self.state = 1072
             self.match(Python3Parser.COLON)
-            self.state = 1074
+            self.state = 1073
             self.suite()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -7759,34 +7750,34 @@
     def arglist(self):
 
         localctx = Python3Parser.ArglistContext(self, self._ctx, self.state)
         self.enterRule(localctx, 156, self.RULE_arglist)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1076
+            self.state = 1075
             self.argument()
-            self.state = 1081
+            self.state = 1080
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,159,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 1077
+                    self.state = 1076
                     self.match(Python3Parser.COMMA)
-                    self.state = 1078
+                    self.state = 1077
                     self.argument() 
-                self.state = 1083
+                self.state = 1082
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,159,self._ctx)
 
-            self.state = 1085
+            self.state = 1084
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.COMMA:
-                self.state = 1084
+                self.state = 1083
                 self.match(Python3Parser.COMMA)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -7843,50 +7834,50 @@
     def argument(self):
 
         localctx = Python3Parser.ArgumentContext(self, self._ctx, self.state)
         self.enterRule(localctx, 158, self.RULE_argument)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1099
+            self.state = 1098
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,162,self._ctx)
             if la_ == 1:
-                self.state = 1087
+                self.state = 1086
                 self.test()
-                self.state = 1089
+                self.state = 1088
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==Python3Parser.FOR or _la==Python3Parser.ASYNC:
-                    self.state = 1088
+                    self.state = 1087
                     self.comp_for()
 
 
                 pass
 
             elif la_ == 2:
-                self.state = 1091
+                self.state = 1090
                 self.test()
-                self.state = 1092
+                self.state = 1091
                 self.match(Python3Parser.ASSIGN)
-                self.state = 1093
+                self.state = 1092
                 self.test()
                 pass
 
             elif la_ == 3:
-                self.state = 1095
+                self.state = 1094
                 self.match(Python3Parser.POWER)
-                self.state = 1096
+                self.state = 1095
                 self.test()
                 pass
 
             elif la_ == 4:
-                self.state = 1097
+                self.state = 1096
                 self.match(Python3Parser.STAR)
-                self.state = 1098
+                self.state = 1097
                 self.test()
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -7930,25 +7921,25 @@
 
 
     def comp_iter(self):
 
         localctx = Python3Parser.Comp_iterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 160, self.RULE_comp_iter)
         try:
-            self.state = 1103
+            self.state = 1102
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.FOR, Python3Parser.ASYNC]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1101
+                self.state = 1100
                 self.comp_for()
                 pass
             elif token in [Python3Parser.IF]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1102
+                self.state = 1101
                 self.comp_if()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -8008,35 +7999,35 @@
     def comp_for(self):
 
         localctx = Python3Parser.Comp_forContext(self, self._ctx, self.state)
         self.enterRule(localctx, 162, self.RULE_comp_for)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1106
+            self.state = 1105
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==Python3Parser.ASYNC:
-                self.state = 1105
+                self.state = 1104
                 self.match(Python3Parser.ASYNC)
 
 
-            self.state = 1108
+            self.state = 1107
             self.match(Python3Parser.FOR)
-            self.state = 1109
+            self.state = 1108
             self.exprlist()
-            self.state = 1110
+            self.state = 1109
             self.match(Python3Parser.IN)
-            self.state = 1111
+            self.state = 1110
             self.or_test()
-            self.state = 1113
+            self.state = 1112
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.IF) | (1 << Python3Parser.FOR) | (1 << Python3Parser.ASYNC))) != 0):
-                self.state = 1112
+                self.state = 1111
                 self.comp_iter()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -8084,23 +8075,23 @@
     def comp_if(self):
 
         localctx = Python3Parser.Comp_ifContext(self, self._ctx, self.state)
         self.enterRule(localctx, 164, self.RULE_comp_if)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1115
+            self.state = 1114
             self.match(Python3Parser.IF)
-            self.state = 1116
+            self.state = 1115
             self.test_nocond()
-            self.state = 1118
+            self.state = 1117
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.IF) | (1 << Python3Parser.FOR) | (1 << Python3Parser.ASYNC))) != 0):
-                self.state = 1117
+                self.state = 1116
                 self.comp_iter()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -8139,15 +8130,15 @@
 
     def encoding_decl(self):
 
         localctx = Python3Parser.Encoding_declContext(self, self._ctx, self.state)
         self.enterRule(localctx, 166, self.RULE_encoding_decl)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1120
+            self.state = 1119
             self.match(Python3Parser.NAME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8189,21 +8180,21 @@
     def yield_expr(self):
 
         localctx = Python3Parser.Yield_exprContext(self, self._ctx, self.state)
         self.enterRule(localctx, 168, self.RULE_yield_expr)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1122
+            self.state = 1121
             self.match(Python3Parser.YIELD)
-            self.state = 1124
+            self.state = 1123
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << Python3Parser.T__0) | (1 << Python3Parser.T__1) | (1 << Python3Parser.STRING) | (1 << Python3Parser.NUMBER) | (1 << Python3Parser.FROM) | (1 << Python3Parser.LAMBDA) | (1 << Python3Parser.NOT) | (1 << Python3Parser.NONE) | (1 << Python3Parser.TRUE) | (1 << Python3Parser.FALSE) | (1 << Python3Parser.AWAIT) | (1 << Python3Parser.NAME) | (1 << Python3Parser.ELLIPSIS) | (1 << Python3Parser.OPEN_PAREN) | (1 << Python3Parser.OPEN_BRACK))) != 0) or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & ((1 << (Python3Parser.ADD - 69)) | (1 << (Python3Parser.MINUS - 69)) | (1 << (Python3Parser.NOT_OP - 69)) | (1 << (Python3Parser.OPEN_BRACE - 69)))) != 0):
-                self.state = 1123
+                self.state = 1122
                 self.yield_arg()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -8249,27 +8240,27 @@
 
 
     def yield_arg(self):
 
         localctx = Python3Parser.Yield_argContext(self, self._ctx, self.state)
         self.enterRule(localctx, 170, self.RULE_yield_arg)
         try:
-            self.state = 1129
+            self.state = 1128
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [Python3Parser.FROM]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1126
+                self.state = 1125
                 self.match(Python3Parser.FROM)
-                self.state = 1127
+                self.state = 1126
                 self.test()
                 pass
             elif token in [Python3Parser.T__0, Python3Parser.T__1, Python3Parser.STRING, Python3Parser.NUMBER, Python3Parser.LAMBDA, Python3Parser.NOT, Python3Parser.NONE, Python3Parser.TRUE, Python3Parser.FALSE, Python3Parser.AWAIT, Python3Parser.NAME, Python3Parser.ELLIPSIS, Python3Parser.OPEN_PAREN, Python3Parser.OPEN_BRACK, Python3Parser.ADD, Python3Parser.MINUS, Python3Parser.NOT_OP, Python3Parser.OPEN_BRACE]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1128
+                self.state = 1127
                 self.testlist()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -8289,14 +8280,18 @@
             return self.getTypedRuleContext(Python3Parser.Simple_holeContext,0)
 
 
         def double_hole(self):
             return self.getTypedRuleContext(Python3Parser.Double_holeContext,0)
 
 
+        def var_hole(self):
+            return self.getTypedRuleContext(Python3Parser.Var_holeContext,0)
+
+
         def getRuleIndex(self):
             return Python3Parser.RULE_expr_hole
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterExpr_hole" ):
                 listener.enterExpr_hole(self)
 
@@ -8316,27 +8311,33 @@
     def expr_hole(self):
 
         localctx = Python3Parser.Expr_holeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 172, self.RULE_expr_hole)
         try:
             self.state = 1133
             self._errHandler.sync(self)
-            token = self._input.LA(1)
-            if token in [Python3Parser.T__0]:
+            la_ = self._interp.adaptivePredict(self._input,169,self._ctx)
+            if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1131
+                self.state = 1130
                 self.simple_hole()
                 pass
-            elif token in [Python3Parser.T__1]:
+
+            elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1132
+                self.state = 1131
                 self.double_hole()
                 pass
-            else:
-                raise NoViableAltException(self)
+
+            elif la_ == 3:
+                self.enterOuterAlt(localctx, 3)
+                self.state = 1132
+                self.var_hole()
+                pass
+
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
```

### Comparing `python-hole-0.0.7/src/pyhole/antlr/Python3Visitor.py` & `python-hole-0.0.8/src/pyhole/antlr/Python3Visitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/pyhole/visualizer/Visualizer.py` & `python-hole-0.0.8/src/pyhole/visualizer/Visualizer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.7/src/python_hole.egg-info/PKG-INFO` & `python-hole-0.0.8/src/python_hole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hole
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package to build code patterns
 Home-page: https://github.com/JulienLie/python-hole
 Author: Julien Lienard
 Author-email: julien.lienard@uclouvain.be
 License: MIT
 Description: # Python Hole
```

### Comparing `python-hole-0.0.7/src/python_hole.egg-info/SOURCES.txt` & `python-hole-0.0.8/src/python_hole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

