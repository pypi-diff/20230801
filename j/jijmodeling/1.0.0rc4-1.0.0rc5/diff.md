# Comparing `tmp/jijmodeling-1.0.0rc4-cp39-none-win_amd64.whl.zip` & `tmp/jijmodeling-1.0.0rc5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 759942 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2902 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/WHEEL
--rw-r--r--  4.6 unx     3445 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx      127 b- defN 23-Jul-25 12:34 jijmodeling/__init__.py
--rw-r--r--  4.6 unx   131169 b- defN 23-Jul-25 12:34 jijmodeling/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-25 12:34 jijmodeling/py.typed
--rwxr-xr-x  4.6 unx  2202624 b- defN 23-Jul-25 12:34 jijmodeling/jijmodeling.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      678 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/RECORD
-8 files, 2341039 bytes uncompressed, 758758 bytes compressed:  67.6%
+Zip file size: 776480 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2902 b- defN 23-Aug-01 14:09 jijmodeling-1.0.0rc5.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Aug-01 14:09 jijmodeling-1.0.0rc5.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3445 b- defN 23-Aug-01 14:09 jijmodeling-1.0.0rc5.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx      127 b- defN 23-Aug-01 14:09 jijmodeling/__init__.py
+-rw-r--r--  4.6 unx   132884 b- defN 23-Aug-01 14:09 jijmodeling/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Aug-01 14:09 jijmodeling/py.typed
+-rwxr-xr-x  4.6 unx  2241024 b- defN 23-Aug-01 14:09 jijmodeling/jijmodeling.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      678 b- defN 23-Aug-01 14:09 jijmodeling-1.0.0rc5.dist-info/RECORD
+8 files, 2381154 bytes uncompressed, 775296 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: jijmodeling-1.0.0rc4.dist-info/METADATA
+Filename: jijmodeling-1.0.0rc5.dist-info/METADATA
 Comment: 
 
-Filename: jijmodeling-1.0.0rc4.dist-info/WHEEL
+Filename: jijmodeling-1.0.0rc5.dist-info/WHEEL
 Comment: 
 
-Filename: jijmodeling-1.0.0rc4.dist-info/license_files/LICENSE.txt
+Filename: jijmodeling-1.0.0rc5.dist-info/license_files/LICENSE.txt
 Comment: 
 
 Filename: jijmodeling/__init__.py
 Comment: 
 
 Filename: jijmodeling/__init__.pyi
 Comment: 
 
 Filename: jijmodeling/py.typed
 Comment: 
 
 Filename: jijmodeling/jijmodeling.cp39-win_amd64.pyd
 Comment: 
 
-Filename: jijmodeling-1.0.0rc4.dist-info/RECORD
+Filename: jijmodeling-1.0.0rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jijmodeling/__init__.pyi

```diff
@@ -579,21 +579,35 @@
     def __rsub__(self, value, /):
         """
         Return value-self.
         """
         pass
 
 
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
     def __sub__(self, value, /):
         """
         Return self-value.
         """
         pass
 
 
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
     def _repr_latex_(self, /):
         """
         
         """
         pass
 
 
@@ -763,37 +777,36 @@
     Expression:
         Create an equality constraint that the sum of $N$ binary variables is equal to one.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N,))
-        >>> jm.Constraint("constraint", jm.sum(i, x[i]) == 1)
-        {'expression': sum(i in [0..N), x[i]) == 1}
+        >>> repr(jm.Constraint("constraint", jm.sum(i, x[i]) == 1))
+        'Constraint(name="constraint", expression=sum(i in [0..N), x[i]) == 1)'
     
         Create an inequality constraint with forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N, N))
-        >>> jm.Constraint("constraint", jm.sum(i, x[i,j]) == 1, forall=j)
-        {'expression': sum(i in [0..N), x[i, j]) == 1, 'forall': [j]}
+        >>> repr(jm.Constraint("constraint", jm.sum(i, x[i,j]) == 1, forall=j))
+        'Constraint(name="constraint", expression=sum(i in [0..N), x[i, j]) == 1, forall=[j])'
     
         Create an inequality constraint with conditional forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N, N))
-        >>> jm.Constraint("constraint", x[i,j] <= 2, forall=[i, (j, j != i)])
-        {'expression': x[i, j] <= 2, 'forall': [i, (j, j != i)]}
-        
+        >>> repr(jm.Constraint("constraint", x[i,j] <= 2, forall=[i, (j, j != i)]))
+        'Constraint(name="constraint", expression=x[i, j] <= 2, forall=[i, (j, j != i)])'
     """
     def __new__(cls, name: str, expression, *, forall=None):
         pass
 
     def _repr_latex_(self, /):
         """
         
@@ -972,21 +985,35 @@
     def __rsub__(self, value, /):
         """
         Return value-self.
         """
         pass
 
 
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
     def __sub__(self, value, /):
         """
         Return self-value.
         """
         pass
 
 
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
     def _repr_latex_(self, /):
         """
         
         """
         pass
 
 
@@ -1030,36 +1057,36 @@
     Expression:
         Create a custom penalty term.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N,))
-        >>> jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i]) - 1)**2)  # doctest: +ELLIPSIS
-        <jijmodeling.CustomPenaltyTerm object at 0x...>
+        >>> repr(jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i]) - 1)**2))  # doctest: +ELLIPSIS
+        'CustomPenaltyTerm(name="custom penalty term", expression=((sum(i in [0..N), x[i]) - 1) ** 2))'
     
         Create a custom penalty term with forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N, N))
-        >>> jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i,j]) - 1)**2, forall=j)  # doctest: +ELLIPSIS
-        <jijmodeling.CustomPenaltyTerm object at 0x...>
+        >>> repr(jm.CustomPenaltyTerm("custom penalty term", (jm.sum(i, x[i,j]) - 1)**2, forall=j))  # doctest: +ELLIPSIS
+        'CustomPenaltyTerm(name="custom penalty term", expression=((sum(i in [0..N), x[i, j]) - 1) ** 2), forall=[j])'
     
         Create a custom penalty term with conditional forall.
     
         >>> import jijmodeling as jm
         >>> N = jm.Placeholder("N")
         >>> i = jm.Element("i", belong_to=N)
         >>> j = jm.Element("j", belong_to=N)
         >>> x = jm.BinaryVar("x", shape=(N, N))
-        >>> jm.CustomPenaltyTerm("custom penalty term", (x[i,j] - 2)**2, forall=[i, (j, j != i)])  # doctest: +ELLIPSIS
-        <jijmodeling.CustomPenaltyTerm object at 0x...>
+        >>> repr(jm.CustomPenaltyTerm("custom penalty term", (x[i,j] - 2)**2, forall=[i, (j, j != i)]))  # doctest: +ELLIPSIS
+        'CustomPenaltyTerm(name="custom penalty term", expression=((x[i, j] - 2) ** 2), forall=[i, (j, j != i)])'
     """
     def __new__(cls, name: str, expression, *, forall=None):
         pass
 
     def _repr_latex_(self, /):
         """
         
@@ -1919,21 +1946,35 @@
     def __rsub__(self, value, /):
         """
         Return value-self.
         """
         pass
 
 
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
     def __sub__(self, value, /):
         """
         Return self-value.
         """
         pass
 
 
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
     def _repr_latex_(self, /):
         """
         
         """
         pass
 
 
@@ -4369,21 +4410,35 @@
     def __rsub__(self, value, /):
         """
         Return value-self.
         """
         pass
 
 
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
     def __sub__(self, value, /):
         """
         Return self-value.
         """
         pass
 
 
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
     def _repr_latex_(self, /):
         """
         
         """
         pass
 
 
@@ -4522,21 +4577,35 @@
     def __rsub__(self, value, /):
         """
         Return value-self.
         """
         pass
 
 
+    def __rtruediv__(self, value, /):
+        """
+        Return value/self.
+        """
+        pass
+
+
     def __sub__(self, value, /):
         """
         Return self-value.
         """
         pass
 
 
+    def __truediv__(self, value, /):
+        """
+        Return self/value.
+        """
+        pass
+
+
     def _repr_latex_(self, /):
         """
         
         """
         pass
 
 
@@ -4753,14 +4822,25 @@
         """
         
         """
         pass
 
 
     ndim: int
+    def set_latex(self, /, latex=None):
+        """
+        Set the LaTeX representation of the object.
+        If the LaTeX representation is not set, the default representation is set.
+        
+        Args:
+            latex (str, optional): LaTeX representation of the object. Defaults to None.
+        """
+        pass
+
+
     shape: tuple
     subscripts: typing.Any
     variable: typing.Any
 @typing.final
 class SumOp:
     """
     A class for representing summation
```

## Comparing `jijmodeling-1.0.0rc4.dist-info/METADATA` & `jijmodeling-1.0.0rc5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jijmodeling
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `jijmodeling-1.0.0rc4.dist-info/license_files/LICENSE.txt` & `jijmodeling-1.0.0rc5.dist-info/license_files/LICENSE.txt`

 * *Files identical despite different names*

